# Comparing `tmp/pulumi_awsx-1.0.2.tar.gz` & `tmp/pulumi_awsx-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_awsx-1.0.2.tar", last modified: Tue Feb  7 11:34:30 2023, max compression
+gzip compressed data, was "pulumi_awsx-1.0.3.tar", last modified: Thu Aug  3 10:23:40 2023, max compression
```

## Comparing `pulumi_awsx-1.0.2.tar` & `pulumi_awsx-1.0.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:34:30.839109 pulumi_awsx-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-02-07 11:34:30.839109 pulumi_awsx-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:34:30.827108 pulumi_awsx-1.0.2/pulumi_awsx/
--rw-------   0 runner    (1001) docker     (123)     2193 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx/__init__.py
--rw-------   0 runner    (1001) docker     (123)     7642 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:34:30.827108 pulumi_awsx-1.0.2/pulumi_awsx/awsx/
--rw-------   0 runner    (1001) docker     (123)      223 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx/awsx/__init__.py
--rw-------   0 runner    (1001) docker     (123)    56292 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx/awsx/_inputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:34:30.831109 pulumi_awsx-1.0.2/pulumi_awsx/cloudtrail/
--rw-------   0 runner    (1001) docker     (123)      265 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx/cloudtrail/__init__.py
--rw-------   0 runner    (1001) docker     (123)    23442 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx/cloudtrail/trail.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:34:30.831109 pulumi_awsx-1.0.2/pulumi_awsx/ec2/
--rw-------   0 runner    (1001) docker     (123)      366 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx/ec2/__init__.py
--rw-------   0 runner    (1001) docker     (123)     1345 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx/ec2/_enums.py
--rw-------   0 runner    (1001) docker     (123)    30936 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx/ec2/_inputs.py
--rw-------   0 runner    (1001) docker     (123)     3890 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx/ec2/default_vpc.py
--rw-------   0 runner    (1001) docker     (123)     3017 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx/ec2/get_default_vpc.py
--rw-------   0 runner    (1001) docker     (123)    36064 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx/ec2/vpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:34:30.831109 pulumi_awsx-1.0.2/pulumi_awsx/ecr/
--rw-------   0 runner    (1001) docker     (123)      336 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx/ecr/__init__.py
--rw-------   0 runner    (1001) docker     (123)      521 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx/ecr/_enums.py
--rw-------   0 runner    (1001) docker     (123)     7566 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx/ecr/_inputs.py
--rw-------   0 runner    (1001) docker     (123)    12944 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx/ecr/image.py
--rw-------   0 runner    (1001) docker     (123)    14482 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx/ecr/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:34:30.835109 pulumi_awsx-1.0.2/pulumi_awsx/ecs/
--rw-------   0 runner    (1001) docker     (123)      399 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx/ecs/__init__.py
--rw-------   0 runner    (1001) docker     (123)    84791 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx/ecs/_inputs.py
--rw-------   0 runner    (1001) docker     (123)    41699 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx/ecs/ec2_service.py
--rw-------   0 runner    (1001) docker     (123)    31315 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx/ecs/ec2_task_definition.py
--rw-------   0 runner    (1001) docker     (123)    40415 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx/ecs/fargate_service.py
--rw-------   0 runner    (1001) docker     (123)    30218 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx/ecs/fargate_task_definition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:34:30.835109 pulumi_awsx-1.0.2/pulumi_awsx/lb/
--rw-------   0 runner    (1001) docker     (123)      384 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx/lb/__init__.py
--rw-------   0 runner    (1001) docker     (123)    87068 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx/lb/_inputs.py
--rw-------   0 runner    (1001) docker     (123)    34637 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx/lb/application_load_balancer.py
--rw-------   0 runner    (1001) docker     (123)    32049 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx/lb/network_load_balancer.py
--rw-------   0 runner    (1001) docker     (123)    11164 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx/lb/target_group_attachment.py
--rw-------   0 runner    (1001) docker     (123)     2770 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx/provider.py
--rw-------   0 runner    (1001) docker     (123)       41 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx/pulumi-plugin.json
--rw-------   0 runner    (1001) docker     (123)        0 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:34:30.827108 pulumi_awsx-1.0.2/pulumi_awsx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-07 11:34:30.839109 pulumi_awsx-1.0.2/setup.cfg
--rw-------   0 runner    (1001) docker     (123)     2145 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:40.636603 pulumi_awsx-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-08-03 10:23:40.632603 pulumi_awsx-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5992 2023-08-03 10:23:40.000000 pulumi_awsx-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:40.628603 pulumi_awsx-1.0.3/pulumi_awsx/
+-rw-------   0 runner    (1001) docker     (123)     2193 2023-08-03 10:23:40.000000 pulumi_awsx-1.0.3/pulumi_awsx/__init__.py
+-rw-------   0 runner    (1001) docker     (123)     8056 2023-08-03 10:23:40.000000 pulumi_awsx-1.0.3/pulumi_awsx/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:40.632603 pulumi_awsx-1.0.3/pulumi_awsx/awsx/
+-rw-------   0 runner    (1001) docker     (123)      223 2023-08-03 10:23:40.000000 pulumi_awsx-1.0.3/pulumi_awsx/awsx/__init__.py
+-rw-------   0 runner    (1001) docker     (123)    58990 2023-08-03 10:23:40.000000 pulumi_awsx-1.0.3/pulumi_awsx/awsx/_inputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:40.632603 pulumi_awsx-1.0.3/pulumi_awsx/cloudtrail/
+-rw-------   0 runner    (1001) docker     (123)      265 2023-08-03 10:23:40.000000 pulumi_awsx-1.0.3/pulumi_awsx/cloudtrail/__init__.py
+-rw-------   0 runner    (1001) docker     (123)    23412 2023-08-03 10:23:40.000000 pulumi_awsx-1.0.3/pulumi_awsx/cloudtrail/trail.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:40.632603 pulumi_awsx-1.0.3/pulumi_awsx/ec2/
+-rw-------   0 runner    (1001) docker     (123)      366 2023-08-03 10:23:40.000000 pulumi_awsx-1.0.3/pulumi_awsx/ec2/__init__.py
+-rw-------   0 runner    (1001) docker     (123)     1345 2023-08-03 10:23:40.000000 pulumi_awsx-1.0.3/pulumi_awsx/ec2/_enums.py
+-rw-------   0 runner    (1001) docker     (123)    31665 2023-08-03 10:23:40.000000 pulumi_awsx-1.0.3/pulumi_awsx/ec2/_inputs.py
+-rw-------   0 runner    (1001) docker     (123)     3839 2023-08-03 10:23:40.000000 pulumi_awsx-1.0.3/pulumi_awsx/ec2/default_vpc.py
+-rw-------   0 runner    (1001) docker     (123)     2976 2023-08-03 10:23:40.000000 pulumi_awsx-1.0.3/pulumi_awsx/ec2/get_default_vpc.py
+-rw-------   0 runner    (1001) docker     (123)    37477 2023-08-03 10:23:40.000000 pulumi_awsx-1.0.3/pulumi_awsx/ec2/vpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:40.632603 pulumi_awsx-1.0.3/pulumi_awsx/ecr/
+-rw-------   0 runner    (1001) docker     (123)      336 2023-08-03 10:23:40.000000 pulumi_awsx-1.0.3/pulumi_awsx/ecr/__init__.py
+-rw-------   0 runner    (1001) docker     (123)      521 2023-08-03 10:23:40.000000 pulumi_awsx-1.0.3/pulumi_awsx/ecr/_enums.py
+-rw-------   0 runner    (1001) docker     (123)     7578 2023-08-03 10:23:40.000000 pulumi_awsx-1.0.3/pulumi_awsx/ecr/_inputs.py
+-rw-------   0 runner    (1001) docker     (123)    12893 2023-08-03 10:23:40.000000 pulumi_awsx-1.0.3/pulumi_awsx/ecr/image.py
+-rw-------   0 runner    (1001) docker     (123)    14431 2023-08-03 10:23:40.000000 pulumi_awsx-1.0.3/pulumi_awsx/ecr/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:40.632603 pulumi_awsx-1.0.3/pulumi_awsx/ecs/
+-rw-------   0 runner    (1001) docker     (123)      399 2023-08-03 10:23:40.000000 pulumi_awsx-1.0.3/pulumi_awsx/ecs/__init__.py
+-rw-------   0 runner    (1001) docker     (123)    84803 2023-08-03 10:23:40.000000 pulumi_awsx-1.0.3/pulumi_awsx/ecs/_inputs.py
+-rw-------   0 runner    (1001) docker     (123)    46115 2023-08-03 10:23:40.000000 pulumi_awsx-1.0.3/pulumi_awsx/ecs/ec2_service.py
+-rw-------   0 runner    (1001) docker     (123)    31264 2023-08-03 10:23:40.000000 pulumi_awsx-1.0.3/pulumi_awsx/ecs/ec2_task_definition.py
+-rw-------   0 runner    (1001) docker     (123)    44831 2023-08-03 10:23:40.000000 pulumi_awsx-1.0.3/pulumi_awsx/ecs/fargate_service.py
+-rw-------   0 runner    (1001) docker     (123)    30167 2023-08-03 10:23:40.000000 pulumi_awsx-1.0.3/pulumi_awsx/ecs/fargate_task_definition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:40.632603 pulumi_awsx-1.0.3/pulumi_awsx/lb/
+-rw-------   0 runner    (1001) docker     (123)      384 2023-08-03 10:23:40.000000 pulumi_awsx-1.0.3/pulumi_awsx/lb/__init__.py
+-rw-------   0 runner    (1001) docker     (123)    90587 2023-08-03 10:23:40.000000 pulumi_awsx-1.0.3/pulumi_awsx/lb/_inputs.py
+-rw-------   0 runner    (1001) docker     (123)    40071 2023-08-03 10:23:40.000000 pulumi_awsx-1.0.3/pulumi_awsx/lb/application_load_balancer.py
+-rw-------   0 runner    (1001) docker     (123)    37892 2023-08-03 10:23:40.000000 pulumi_awsx-1.0.3/pulumi_awsx/lb/network_load_balancer.py
+-rw-------   0 runner    (1001) docker     (123)    11113 2023-08-03 10:23:40.000000 pulumi_awsx-1.0.3/pulumi_awsx/lb/target_group_attachment.py
+-rw-------   0 runner    (1001) docker     (123)     2719 2023-08-03 10:23:40.000000 pulumi_awsx-1.0.3/pulumi_awsx/provider.py
+-rw-------   0 runner    (1001) docker     (123)       41 2023-08-03 10:23:40.000000 pulumi_awsx-1.0.3/pulumi_awsx/pulumi-plugin.json
+-rw-------   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:40.000000 pulumi_awsx-1.0.3/pulumi_awsx/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:23:40.632603 pulumi_awsx-1.0.3/pulumi_awsx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-08-03 10:23:40.000000 pulumi_awsx-1.0.3/pulumi_awsx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-08-03 10:23:40.000000 pulumi_awsx-1.0.3/pulumi_awsx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 10:23:40.000000 pulumi_awsx-1.0.3/pulumi_awsx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 10:23:40.000000 pulumi_awsx-1.0.3/pulumi_awsx.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-08-03 10:23:40.000000 pulumi_awsx-1.0.3/pulumi_awsx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-03 10:23:40.000000 pulumi_awsx-1.0.3/pulumi_awsx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 10:23:40.636603 pulumi_awsx-1.0.3/setup.cfg
+-rw-------   0 runner    (1001) docker     (123)     2176 2023-08-03 10:23:40.000000 pulumi_awsx-1.0.3/setup.py
```

### Comparing `pulumi_awsx-1.0.2/PKG-INFO` & `pulumi_awsx-1.0.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,110 +1,110 @@
 Metadata-Version: 2.1
 Name: pulumi_awsx
-Version: 1.0.2
+Version: 1.0.3
 Summary: Pulumi Amazon Web Services (AWS) AWSX Components.
 Home-page: https://pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-awsx
-Description: [![Actions Status](https://github.com/pulumi/pulumi-awsx/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-awsx/actions)
-        [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
-        [![NPM version](https://badge.fury.io/js/%40pulumi%2Fawsx.svg)](https://www.npmjs.com/package/@pulumi/awsx)
-        [![Python version](https://badge.fury.io/py/pulumi-awsx.svg)](https://pypi.org/project/pulumi-awsx)
-        [![NuGet version](https://badge.fury.io/nu/pulumi.awsx.svg)](https://badge.fury.io/nu/pulumi.awsx)
-        [![PkgGoDev](https://pkg.go.dev/badge/github.com/pulumi/pulumi-awsx/sdk/go)](https://pkg.go.dev/github.com/pulumi/pulumi-awsx/sdk/go)
-        [![License](https://img.shields.io/npm/l/%40pulumi%2Fawsx.svg)](https://github.com/pulumi/pulumi-awsx/blob/master/LICENSE)
-        
-        ## Pulumi AWS Infrastructure Components
-        
-        Pulumi's framework for Amazon Web Services (AWS) infrastructure.
-        
-        To use this package, [install the Pulumi CLI](https://www.pulumi.com/docs/get-started/install/). For a streamlined Pulumi walkthrough, including language runtime installation and AWS configuration, see the [Crosswalk for AWS documentation](https://www.pulumi.com/docs/guides/crosswalk/aws/).
-        
-        The AWS Infrastructure package is intended to provide [component](https://www.pulumi.com/docs/intro/concepts/resources/components/) wrappers around many core AWS 'raw' resources to make them easier and more convenient to use.  In general, the `@pulumi/awsx` package mirrors the module structure of `@pulumi/aws` (i.e. `@pulumi/awsx/ecs` or `@pulumi/awsx/ec2`).  These [components](https://www.pulumi.com/docs/intro/concepts/resources/components/) are designed to take care of much of the redundancy and boilerplate necessary when using the raw AWS resources, while still striving to expose all underlying functionality if needed.
-        
-        The AWS Infrastructure package undergoes constant improvements and additions.  While we will strive to maintain backward compatability here, we will occasionally make breaks here as appropriate if it helps improve the overall quality of this package.
-        
-        The AWS Infrastructure package exposes many high level abstractions.  Including:
-        
-        * [`ec2`](https://github.com/pulumi/pulumi-awsx/blob/master/awsx/ec2).  A module that makes it easier to work with your AWS network, subnets, and security groups.  By default, the resources in the package follow the [AWS Best Practices](
-          https://aws.amazon.com/answers/networking/aws-single-vpc-design/), but can be configured as desired in whatever ways you want.  Most commonly, this package is used to acquire the default Vpc for a region (using `awsx.ec2.DefaultNetwork`).  However, it can also be used to easily create or augment an existing Vpc.
-        
-        * [`ecs`](https://github.com/pulumi/pulumi-awsx/blob/master/awsx/ecs).  A module that makes it easy to create and configure clusters, tasks and services for running containers. Convenience resources are created to make the common tasks of creating EC2 or Fargate services and tasks much simpler.
-        
-        * [`lb`](https://github.com/pulumi/pulumi-awsx/tree/master/awsx/lb).  A module for simply setting up [Elastic Load Balancing](https://aws.amazon.com/elasticloadbalancing/). This module provides convenient ways to set up either `Network` or `Application` load balancers, along with the appropriate ELB Target Groups and Listeners in order to have a high availability, automatically-scaled service.  These ELB components also work well with the other awsx components.  For example, an `lb.defaultTarget` can be passed in directly as the `portMapping` target of an `ecs.FargateService`.
-        
-        <div>
-            <a href="https://www.pulumi.com/docs/guides/crosswalk/aws/" title="Get Started">
-               <img src="https://www.pulumi.com/images/get-started.svg?" width="120">
-            </a>
-        </div>
-        
-        ## Installing
-        
-        This package is available in many languages in the standard packaging formats.
-        
-        ### Node.js (Java/TypeScript)
-        
-        To use from JavaScript or TypeScript in Node.js, install using either `npm`:
-        
-        ```bash
-        npm install @pulumi/awsx
-        ```
-        
-        or `yarn`:
-        
-        ```bash
-        yarn add @pulumi/awsx
-        ```
-        
-        ### Python
-        
-        To use from Python, install using `pip`:
-        
-        ```bash
-        pip install pulumi-awsx
-        ```
-        
-        ### Go
-        
-        To use from Go, use `go get` to grab the latest version of the library
-        
-        ```bash
-        go get github.com/pulumi/pulumi-awsx/sdk
-        ```
-        
-        ### .NET
-        
-        To use from .NET, install using `dotnet add package`:
-        
-        ```bash
-        dotnet add package Pulumi.Awsx
-        ```
-        
-        ## Configuration
-        
-        The configuration options available for this provider mirror those of the [Pulumi AWS Classic Provider](https://github.com/pulumi/pulumi-aws#configuration)
-        
-        ## Migration from 0.x to 1.0
-        
-        Before version 1, this package only supported components in TypeScript. All the existing components from the 0.x releases are now available in the `classic` namespace. The `classic` namespace will remain until the next major version release but will only receive updates for critical security fixes.
-        
-        1. Change references from `@pulumi/awsx` to `@pulumi/awsx/classic` to maintain existing behaviour.
-        2. Refactor to replace the classic components with the new top-level components.
-        
-        **Note:** The new top-level components (outside the `classic` namespace) may require additional code changes and resource re-creation.
-        
-        ### Notable changes
-        
-        - Removed ECS Cluster as this did not add any functionaly over the [AWS Classic ECS Cluster resource](https://www.pulumi.com/registry/packages/aws/api-docs/ecs/cluster/).
-        - Removed `Vpc.fromExistingIds()` as this was originally added because other components depended on the concrete VPC component class. The new components in v1 no longer have hard dependencies on other resources, so instead the subnets from the existing VPC can be passed into other components directly.
-        
-        ## References
-        
-        * [Tutorial](https://www.pulumi.com/blog/crosswalk-for-aws-1-0/)
-        * [API Reference Documentation](https://www.pulumi.com/registry/packages/awsx/api-docs/)
-        * [Examples](./examples)
-        * [Crosswalk for AWS Guide](https://www.pulumi.com/docs/guides/crosswalk/aws/)
-        
 Keywords: pulumi aws awsx kind/component category/cloud
-Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+
+[![Actions Status](https://github.com/pulumi/pulumi-awsx/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-awsx/actions)
+[![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
+[![NPM version](https://badge.fury.io/js/%40pulumi%2Fawsx.svg)](https://www.npmjs.com/package/@pulumi/awsx)
+[![Python version](https://badge.fury.io/py/pulumi-awsx.svg)](https://pypi.org/project/pulumi-awsx)
+[![NuGet version](https://badge.fury.io/nu/pulumi.awsx.svg)](https://badge.fury.io/nu/pulumi.awsx)
+[![PkgGoDev](https://pkg.go.dev/badge/github.com/pulumi/pulumi-awsx/sdk/go)](https://pkg.go.dev/github.com/pulumi/pulumi-awsx/sdk/go)
+[![License](https://img.shields.io/npm/l/%40pulumi%2Fawsx.svg)](https://github.com/pulumi/pulumi-awsx/blob/master/LICENSE)
+
+## Pulumi AWS Infrastructure Components
+
+Pulumi's framework for Amazon Web Services (AWS) infrastructure.
+
+To use this package, [install the Pulumi CLI](https://www.pulumi.com/docs/get-started/install/). For a streamlined Pulumi walkthrough, including language runtime installation and AWS configuration, see the [Crosswalk for AWS documentation](https://www.pulumi.com/docs/guides/crosswalk/aws/).
+
+The AWS Infrastructure package is intended to provide [component](https://www.pulumi.com/docs/intro/concepts/resources/components/) wrappers around many core AWS 'raw' resources to make them easier and more convenient to use.  In general, the `@pulumi/awsx` package mirrors the module structure of `@pulumi/aws` (i.e. `@pulumi/awsx/ecs` or `@pulumi/awsx/ec2`).  These [components](https://www.pulumi.com/docs/intro/concepts/resources/components/) are designed to take care of much of the redundancy and boilerplate necessary when using the raw AWS resources, while still striving to expose all underlying functionality if needed.
+
+The AWS Infrastructure package undergoes constant improvements and additions.  While we will strive to maintain backward compatability here, we will occasionally make breaks here as appropriate if it helps improve the overall quality of this package.
+
+The AWS Infrastructure package exposes many high level abstractions.  Including:
+
+* [`ec2`](https://github.com/pulumi/pulumi-awsx/blob/master/awsx/ec2).  A module that makes it easier to work with your AWS network, subnets, and security groups.  By default, the resources in the package follow the [AWS Best Practices](
+  https://aws.amazon.com/answers/networking/aws-single-vpc-design/), but can be configured as desired in whatever ways you want.  Most commonly, this package is used to acquire the default Vpc for a region (using `awsx.ec2.DefaultNetwork`).  However, it can also be used to easily create or augment an existing Vpc.
+
+* [`ecs`](https://github.com/pulumi/pulumi-awsx/blob/master/awsx/ecs).  A module that makes it easy to create and configure clusters, tasks and services for running containers. Convenience resources are created to make the common tasks of creating EC2 or Fargate services and tasks much simpler.
+
+* [`lb`](https://github.com/pulumi/pulumi-awsx/tree/master/awsx/lb).  A module for simply setting up [Elastic Load Balancing](https://aws.amazon.com/elasticloadbalancing/). This module provides convenient ways to set up either `Network` or `Application` load balancers, along with the appropriate ELB Target Groups and Listeners in order to have a high availability, automatically-scaled service.  These ELB components also work well with the other awsx components.  For example, an `lb.defaultTarget` can be passed in directly as the `portMapping` target of an `ecs.FargateService`.
+
+<div>
+    <a href="https://www.pulumi.com/docs/guides/crosswalk/aws/" title="Get Started">
+       <img src="https://www.pulumi.com/images/get-started.svg?" width="120">
+    </a>
+</div>
+
+## Installing
+
+This package is available in many languages in the standard packaging formats.
+
+### Node.js (Java/TypeScript)
+
+To use from JavaScript or TypeScript in Node.js, install using either `npm`:
+
+```bash
+npm install @pulumi/awsx
+```
+
+or `yarn`:
+
+```bash
+yarn add @pulumi/awsx
+```
+
+### Python
+
+To use from Python, install using `pip`:
+
+```bash
+pip install pulumi-awsx
+```
+
+### Go
+
+To use from Go, use `go get` to grab the latest version of the library
+
+```bash
+go get github.com/pulumi/pulumi-awsx/sdk
+```
+
+### .NET
+
+To use from .NET, install using `dotnet add package`:
+
+```bash
+dotnet add package Pulumi.Awsx
+```
+
+## Configuration
+
+The configuration options available for this provider mirror those of the [Pulumi AWS Classic Provider](https://github.com/pulumi/pulumi-aws#configuration)
+
+## Migration from 0.x to 1.0
+
+Before version 1, this package only supported components in TypeScript. All the existing components from the 0.x releases are now available in the `classic` namespace. The `classic` namespace will remain until the next major version release but will only receive updates for critical security fixes.
+
+1. Change references from `@pulumi/awsx` to `@pulumi/awsx/classic` to maintain existing behaviour.
+2. Refactor to replace the classic components with the new top-level components.
+
+**Note:** The new top-level components (outside the `classic` namespace) may require additional code changes and resource re-creation.
+
+### Notable changes
+
+- Removed ECS Cluster as this did not add any functionality over the [AWS Classic ECS Cluster resource](https://www.pulumi.com/registry/packages/aws/api-docs/ecs/cluster/).
+- Removed `Vpc.fromExistingIds()` as this was originally added because other components depended on the concrete VPC component class. The new components in v1 no longer have hard dependencies on other resources, so instead the subnets from the existing VPC can be passed into other components directly.
+
+## References
+
+* [Tutorial](https://www.pulumi.com/blog/crosswalk-for-aws-1-0/)
+* [API Reference Documentation](https://www.pulumi.com/registry/packages/awsx/api-docs/)
+* [Examples](./examples)
+* [Crosswalk for AWS Guide](https://www.pulumi.com/docs/guides/crosswalk/aws/)
```

#### html2text {}

```diff
@@ -1,14 +1,15 @@
-Metadata-Version: 2.1 Name: pulumi_awsx Version: 1.0.2 Summary: Pulumi Amazon
+Metadata-Version: 2.1 Name: pulumi_awsx Version: 1.0.3 Summary: Pulumi Amazon
 Web Services (AWS) AWSX Components. Home-page: https://pulumi.com License:
 Apache-2.0 Project-URL: Repository, https://github.com/pulumi/pulumi-awsx
-Description: [![Actions Status](https://github.com/pulumi/pulumi-awsx/
-workflows/master/badge.svg)](https://github.com/pulumi/pulumi-awsx/actions) [!
-[Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://
-slack.pulumi.com) [![NPM version](https://badge.fury.io/js/
+Keywords: pulumi aws awsx kind/component category/cloud Requires-Python: >=3.7
+Description-Content-Type: text/markdown [![Actions Status](https://github.com/
+pulumi/pulumi-awsx/workflows/master/badge.svg)](https://github.com/pulumi/
+pulumi-awsx/actions) [![Slack](http://www.pulumi.com/images/docs/badges/
+slack.svg)](https://slack.pulumi.com) [![NPM version](https://badge.fury.io/js/
 %40pulumi%2Fawsx.svg)](https://www.npmjs.com/package/@pulumi/awsx) [![Python
 version](https://badge.fury.io/py/pulumi-awsx.svg)](https://pypi.org/project/
 pulumi-awsx) [![NuGet version](https://badge.fury.io/nu/pulumi.awsx.svg)]
 (https://badge.fury.io/nu/pulumi.awsx) [![PkgGoDev](https://pkg.go.dev/badge/
 github.com/pulumi/pulumi-awsx/sdk/go)](https://pkg.go.dev/github.com/pulumi/
 pulumi-awsx/sdk/go) [![License](https://img.shields.io/npm/l/
 %40pulumi%2Fawsx.svg)](https://github.com/pulumi/pulumi-awsx/blob/master/
@@ -65,19 +66,17 @@
 0.x releases are now available in the `classic` namespace. The `classic`
 namespace will remain until the next major version release but will only
 receive updates for critical security fixes. 1. Change references from
 `@pulumi/awsx` to `@pulumi/awsx/classic` to maintain existing behaviour. 2.
 Refactor to replace the classic components with the new top-level components.
 **Note:** The new top-level components (outside the `classic` namespace) may
 require additional code changes and resource re-creation. ### Notable changes -
-Removed ECS Cluster as this did not add any functionaly over the [AWS Classic
+Removed ECS Cluster as this did not add any functionality over the [AWS Classic
 ECS Cluster resource](https://www.pulumi.com/registry/packages/aws/api-docs/
 ecs/cluster/). - Removed `Vpc.fromExistingIds()` as this was originally added
 because other components depended on the concrete VPC component class. The new
 components in v1 no longer have hard dependencies on other resources, so
 instead the subnets from the existing VPC can be passed into other components
 directly. ## References * [Tutorial](https://www.pulumi.com/blog/crosswalk-for-
 aws-1-0/) * [API Reference Documentation](https://www.pulumi.com/registry/
 packages/awsx/api-docs/) * [Examples](./examples) * [Crosswalk for AWS Guide]
-(https://www.pulumi.com/docs/guides/crosswalk/aws/) Keywords: pulumi aws awsx
-kind/component category/cloud Platform: UNKNOWN Description-Content-Type: text/
-markdown
+(https://www.pulumi.com/docs/guides/crosswalk/aws/)
```

### Comparing `pulumi_awsx-1.0.2/README.md` & `pulumi_awsx-1.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 1. Change references from `@pulumi/awsx` to `@pulumi/awsx/classic` to maintain existing behaviour.
 2. Refactor to replace the classic components with the new top-level components.
 
 **Note:** The new top-level components (outside the `classic` namespace) may require additional code changes and resource re-creation.
 
 ### Notable changes
 
-- Removed ECS Cluster as this did not add any functionaly over the [AWS Classic ECS Cluster resource](https://www.pulumi.com/registry/packages/aws/api-docs/ecs/cluster/).
+- Removed ECS Cluster as this did not add any functionality over the [AWS Classic ECS Cluster resource](https://www.pulumi.com/registry/packages/aws/api-docs/ecs/cluster/).
 - Removed `Vpc.fromExistingIds()` as this was originally added because other components depended on the concrete VPC component class. The new components in v1 no longer have hard dependencies on other resources, so instead the subnets from the existing VPC can be passed into other components directly.
 
 ## References
 
 * [Tutorial](https://www.pulumi.com/blog/crosswalk-for-aws-1-0/)
 * [API Reference Documentation](https://www.pulumi.com/registry/packages/awsx/api-docs/)
 * [Examples](./examples)
```

#### html2text {}

```diff
@@ -61,15 +61,15 @@
 0.x releases are now available in the `classic` namespace. The `classic`
 namespace will remain until the next major version release but will only
 receive updates for critical security fixes. 1. Change references from
 `@pulumi/awsx` to `@pulumi/awsx/classic` to maintain existing behaviour. 2.
 Refactor to replace the classic components with the new top-level components.
 **Note:** The new top-level components (outside the `classic` namespace) may
 require additional code changes and resource re-creation. ### Notable changes -
-Removed ECS Cluster as this did not add any functionaly over the [AWS Classic
+Removed ECS Cluster as this did not add any functionality over the [AWS Classic
 ECS Cluster resource](https://www.pulumi.com/registry/packages/aws/api-docs/
 ecs/cluster/). - Removed `Vpc.fromExistingIds()` as this was originally added
 because other components depended on the concrete VPC component class. The new
 components in v1 no longer have hard dependencies on other resources, so
 instead the subnets from the existing VPC can be passed into other components
 directly. ## References * [Tutorial](https://www.pulumi.com/blog/crosswalk-for-
 aws-1-0/) * [API Reference Documentation](https://www.pulumi.com/registry/
```

### Comparing `pulumi_awsx-1.0.2/pulumi_awsx/__init__.py` & `pulumi_awsx-1.0.3/pulumi_awsx/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-1.0.2/pulumi_awsx/_utilities.py` & `pulumi_awsx-1.0.3/pulumi_awsx/_utilities.py`

 * *Files 10% similar despite different names*

```diff
@@ -94,14 +94,25 @@
 _version = _get_semver_version()
 _version_str = str(_version)
 
 
 def get_version():
     return _version_str
 
+def get_resource_opts_defaults() -> pulumi.ResourceOptions:
+    return pulumi.ResourceOptions(
+        version=get_version(),
+        plugin_download_url=get_plugin_download_url(),
+    )
+
+def get_invoke_opts_defaults() -> pulumi.InvokeOptions:
+    return pulumi.InvokeOptions(
+        version=get_version(),
+        plugin_download_url=get_plugin_download_url(),
+    )
 
 def get_resource_args_opts(resource_args_type, resource_options_type, *args, **kwargs):
     """
     Return the resource args and options given the *args and **kwargs of a resource's
     __init__ method.
     """
 
@@ -230,7 +241,10 @@
             'args': args_list,
             'kwargs': bound_args.kwargs
         }).apply(lambda resolved_args: func(*resolved_args['args'],
                                             opts=opts,
                                             **resolved_args['kwargs']))
 
     return (lambda _: lifted_func)
+
+def get_plugin_download_url():
+	return None
```

### Comparing `pulumi_awsx-1.0.2/pulumi_awsx/awsx/_inputs.py` & `pulumi_awsx-1.0.3/pulumi_awsx/awsx/_inputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by pulumi-gen-awsx. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 import pulumi_aws
 
@@ -640,37 +641,45 @@
 @pulumi.input_type
 class LogGroupArgs:
     def __init__(__self__, *,
                  kms_key_id: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  name_prefix: Optional[pulumi.Input[str]] = None,
                  retention_in_days: Optional[pulumi.Input[int]] = None,
-                 tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
+                 skip_destroy: Optional[pulumi.Input[bool]] = None,
+                 tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
+                 tags_all: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
         """
         The set of arguments for constructing a LogGroup resource.
         :param pulumi.Input[str] kms_key_id: The ARN of the KMS Key to use when encrypting log data. Please note, after the AWS KMS CMK is disassociated from the log group,
                AWS CloudWatch Logs stops encrypting newly ingested data for the log group. All previously ingested data remains encrypted, and AWS CloudWatch Logs requires
                permissions for the CMK whenever the encrypted data is requested.
         :param pulumi.Input[str] name: The name of the log group. If omitted, this provider will assign a random, unique name.
         :param pulumi.Input[str] name_prefix: Creates a unique name beginning with the specified prefix. Conflicts with `name`.
         :param pulumi.Input[int] retention_in_days: Specifies the number of days
-               you want to retain log events in the specified log group.  Possible values are: 1, 3, 5, 7, 14, 30, 60, 90, 120, 150, 180, 365, 400, 545, 731, 1827, 3653, and 0.
+               you want to retain log events in the specified log group.  Possible values are: 1, 3, 5, 7, 14, 30, 60, 90, 120, 150, 180, 365, 400, 545, 731, 1096, 1827, 2192, 2557, 2922, 3288, 3653, and 0.
                If you select 0, the events in the log group are always retained and never expire.
+        :param pulumi.Input[bool] skip_destroy: Set to true if you do not wish the log group (and any logs it may contain) to be deleted at destroy time, and instead just remove the log group from the state.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: A map of tags to assign to the resource. .If configured with a provider `default_tags` configuration block present, tags with matching keys will overwrite those defined at the provider-level.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags_all: A map of tags assigned to the resource, including those inherited from the provider `default_tags` configuration block.
         """
         if kms_key_id is not None:
             pulumi.set(__self__, "kms_key_id", kms_key_id)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if name_prefix is not None:
             pulumi.set(__self__, "name_prefix", name_prefix)
         if retention_in_days is not None:
             pulumi.set(__self__, "retention_in_days", retention_in_days)
+        if skip_destroy is not None:
+            pulumi.set(__self__, "skip_destroy", skip_destroy)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
+        if tags_all is not None:
+            pulumi.set(__self__, "tags_all", tags_all)
 
     @property
     @pulumi.getter(name="kmsKeyId")
     def kms_key_id(self) -> Optional[pulumi.Input[str]]:
         """
         The ARN of the KMS Key to use when encrypting log data. Please note, after the AWS KMS CMK is disassociated from the log group,
         AWS CloudWatch Logs stops encrypting newly ingested data for the log group. All previously ingested data remains encrypted, and AWS CloudWatch Logs requires
@@ -707,35 +716,59 @@
         pulumi.set(self, "name_prefix", value)
 
     @property
     @pulumi.getter(name="retentionInDays")
     def retention_in_days(self) -> Optional[pulumi.Input[int]]:
         """
         Specifies the number of days
-        you want to retain log events in the specified log group.  Possible values are: 1, 3, 5, 7, 14, 30, 60, 90, 120, 150, 180, 365, 400, 545, 731, 1827, 3653, and 0.
+        you want to retain log events in the specified log group.  Possible values are: 1, 3, 5, 7, 14, 30, 60, 90, 120, 150, 180, 365, 400, 545, 731, 1096, 1827, 2192, 2557, 2922, 3288, 3653, and 0.
         If you select 0, the events in the log group are always retained and never expire.
         """
         return pulumi.get(self, "retention_in_days")
 
     @retention_in_days.setter
     def retention_in_days(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "retention_in_days", value)
 
     @property
+    @pulumi.getter(name="skipDestroy")
+    def skip_destroy(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Set to true if you do not wish the log group (and any logs it may contain) to be deleted at destroy time, and instead just remove the log group from the state.
+        """
+        return pulumi.get(self, "skip_destroy")
+
+    @skip_destroy.setter
+    def skip_destroy(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "skip_destroy", value)
+
+    @property
     @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         A map of tags to assign to the resource. .If configured with a provider `default_tags` configuration block present, tags with matching keys will overwrite those defined at the provider-level.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
     def tags(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "tags", value)
 
+    @property
+    @pulumi.getter(name="tagsAll")
+    def tags_all(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+        """
+        A map of tags assigned to the resource, including those inherited from the provider `default_tags` configuration block.
+        """
+        return pulumi.get(self, "tags_all")
+
+    @tags_all.setter
+    def tags_all(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
+        pulumi.set(self, "tags_all", value)
+
 
 @pulumi.input_type
 class OptionalLogGroupArgs:
     def __init__(__self__, *,
                  args: Optional['LogGroupArgs'] = None,
                  enable: Optional[bool] = None,
                  existing: Optional['ExistingLogGroupArgs'] = None):
@@ -838,28 +871,29 @@
                  managed_policy_arns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  max_session_duration: Optional[pulumi.Input[int]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  name_prefix: Optional[pulumi.Input[str]] = None,
                  path: Optional[pulumi.Input[str]] = None,
                  permissions_boundary: Optional[pulumi.Input[str]] = None,
                  policy_arns: Optional[Sequence[str]] = None,
-                 tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
+                 tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
+                 tags_all: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
         """
         The set of arguments for constructing a Role resource and Policy attachments.
         :param pulumi.Input[str] description: Description of the role.
         :param pulumi.Input[bool] force_detach_policies: Whether to force detaching any policies the role has before destroying it. Defaults to `false`.
-        :param pulumi.Input[Sequence[pulumi.Input['pulumi_aws.iam.RoleInlinePolicyArgs']]] inline_policies: Configuration block defining an exclusive set of IAM inline policies associated with the IAM role. See below. If no blocks are configured, this provider will not manage any inline policies in this resource. Configuring one empty block (i.e., `inline_policy {}`) will cause the provider to remove _all_ inline policies added out of band on `apply`.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] managed_policy_arns: Set of exclusive IAM managed policy ARNs to attach to the IAM role. If this attribute is not configured, this provider will ignore policy attachments to this resource. When configured, the provider will align the role's managed policy attachments with this set by attaching or detaching managed policies. Configuring an empty set (i.e., `managed_policy_arns = []`) will cause the provider to remove _all_ managed policy attachments.
+        :param pulumi.Input[Sequence[pulumi.Input['pulumi_aws.iam.RoleInlinePolicyArgs']]] inline_policies: Configuration block defining an exclusive set of IAM inline policies associated with the IAM role. See below. If no blocks are configured, the provider will not manage any inline policies in this resource. Configuring one empty block (i.e., `inline_policy {}`) will cause the provider to remove _all_ inline policies added out of band on `apply`.
         :param pulumi.Input[int] max_session_duration: Maximum session duration (in seconds) that you want to set for the specified role. If you do not specify a value for this setting, the default maximum of one hour is applied. This setting can have a value from 1 hour to 12 hours.
-        :param pulumi.Input[str] name: Name of the role policy.
+        :param pulumi.Input[str] name: Friendly name of the role. If omitted, this provider will assign a random, unique name. See [IAM Identifiers](https://docs.aws.amazon.com/IAM/latest/UserGuide/Using_Identifiers.html) for more information.
         :param pulumi.Input[str] name_prefix: Creates a unique friendly name beginning with the specified prefix. Conflicts with `name`.
         :param pulumi.Input[str] path: Path to the role. See [IAM Identifiers](https://docs.aws.amazon.com/IAM/latest/UserGuide/Using_Identifiers.html) for more information.
         :param pulumi.Input[str] permissions_boundary: ARN of the policy that is used to set the permissions boundary for the role.
         :param Sequence[str] policy_arns: ARNs of the policies to attach to the created role.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Key-value mapping of tags for the IAM role. If configured with a provider `default_tags` configuration block present, tags with matching keys will overwrite those defined at the provider-level.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags_all: A map of tags assigned to the resource, including those inherited from the provider `default_tags` configuration block.
         """
         if description is not None:
             pulumi.set(__self__, "description", description)
         if force_detach_policies is not None:
             pulumi.set(__self__, "force_detach_policies", force_detach_policies)
         if inline_policies is not None:
             pulumi.set(__self__, "inline_policies", inline_policies)
@@ -875,14 +909,16 @@
             pulumi.set(__self__, "path", path)
         if permissions_boundary is not None:
             pulumi.set(__self__, "permissions_boundary", permissions_boundary)
         if policy_arns is not None:
             pulumi.set(__self__, "policy_arns", policy_arns)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
+        if tags_all is not None:
+            pulumi.set(__self__, "tags_all", tags_all)
 
     @property
     @pulumi.getter
     def description(self) -> Optional[pulumi.Input[str]]:
         """
         Description of the role.
         """
@@ -904,28 +940,25 @@
     def force_detach_policies(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "force_detach_policies", value)
 
     @property
     @pulumi.getter(name="inlinePolicies")
     def inline_policies(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.iam.RoleInlinePolicyArgs']]]]:
         """
-        Configuration block defining an exclusive set of IAM inline policies associated with the IAM role. See below. If no blocks are configured, this provider will not manage any inline policies in this resource. Configuring one empty block (i.e., `inline_policy {}`) will cause the provider to remove _all_ inline policies added out of band on `apply`.
+        Configuration block defining an exclusive set of IAM inline policies associated with the IAM role. See below. If no blocks are configured, the provider will not manage any inline policies in this resource. Configuring one empty block (i.e., `inline_policy {}`) will cause the provider to remove _all_ inline policies added out of band on `apply`.
         """
         return pulumi.get(self, "inline_policies")
 
     @inline_policies.setter
     def inline_policies(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.iam.RoleInlinePolicyArgs']]]]):
         pulumi.set(self, "inline_policies", value)
 
     @property
     @pulumi.getter(name="managedPolicyArns")
     def managed_policy_arns(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        """
-        Set of exclusive IAM managed policy ARNs to attach to the IAM role. If this attribute is not configured, this provider will ignore policy attachments to this resource. When configured, the provider will align the role's managed policy attachments with this set by attaching or detaching managed policies. Configuring an empty set (i.e., `managed_policy_arns = []`) will cause the provider to remove _all_ managed policy attachments.
-        """
         return pulumi.get(self, "managed_policy_arns")
 
     @managed_policy_arns.setter
     def managed_policy_arns(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "managed_policy_arns", value)
 
     @property
@@ -940,15 +973,15 @@
     def max_session_duration(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "max_session_duration", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Name of the role policy.
+        Friendly name of the role. If omitted, this provider will assign a random, unique name. See [IAM Identifiers](https://docs.aws.amazon.com/IAM/latest/UserGuide/Using_Identifiers.html) for more information.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -1008,37 +1041,48 @@
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
     def tags(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "tags", value)
 
+    @property
+    @pulumi.getter(name="tagsAll")
+    def tags_all(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+        """
+        A map of tags assigned to the resource, including those inherited from the provider `default_tags` configuration block.
+        """
+        return pulumi.get(self, "tags_all")
+
+    @tags_all.setter
+    def tags_all(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
+        pulumi.set(self, "tags_all", value)
+
 
 @pulumi.input_type
 class SecurityGroupArgs:
     def __init__(__self__, *,
                  description: Optional[pulumi.Input[str]] = None,
                  egress: Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ec2.SecurityGroupEgressArgs']]]] = None,
                  ingress: Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ec2.SecurityGroupIngressArgs']]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  name_prefix: Optional[pulumi.Input[str]] = None,
                  revoke_rules_on_delete: Optional[pulumi.Input[bool]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  vpc_id: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a Security Group resource.
-        :param pulumi.Input[str] description: Description of this egress rule.
-        :param pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ec2.SecurityGroupEgressArgs']]] egress: Configuration block for egress rules. Can be specified multiple times for each egress rule. Each egress block supports fields documented below.
-        :param pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ec2.SecurityGroupIngressArgs']]] ingress: Configuration block for egress rules. Can be specified multiple times for each ingress rule. Each ingress block supports fields documented below.
+        :param pulumi.Input[str] description: Security group description. Defaults to `Managed by Pulumi`. Cannot be `""`. **NOTE**: This field maps to the AWS `GroupDescription` attribute, for which there is no Update API. If you'd like to classify your security groups in a way that can be updated, use `tags`.
+        :param pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ec2.SecurityGroupEgressArgs']]] egress: Configuration block for egress rules. Can be specified multiple times for each egress rule. Each egress block supports fields documented below. This argument is processed in attribute-as-blocks mode.
+        :param pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ec2.SecurityGroupIngressArgs']]] ingress: Configuration block for ingress rules. Can be specified multiple times for each ingress rule. Each ingress block supports fields documented below. This argument is processed in attribute-as-blocks mode.
         :param pulumi.Input[str] name: Name of the security group. If omitted, this provider will assign a random, unique name.
         :param pulumi.Input[str] name_prefix: Creates a unique name beginning with the specified prefix. Conflicts with `name`.
-        :param pulumi.Input[bool] revoke_rules_on_delete: Instruct this provider to revoke all of the Security Groups attached ingress and egress rules before deleting the rule itself. This is normally not needed, however certain AWS services such as Elastic Map Reduce may automatically add required rules to security groups used with the service, and those rules may contain a cyclic dependency that prevent the security groups from being destroyed without removing the dependency first. Default `false`.
+        :param pulumi.Input[bool] revoke_rules_on_delete: Instruct the provider to revoke all of the Security Groups attached ingress and egress rules before deleting the rule itself. This is normally not needed, however certain AWS services such as Elastic Map Reduce may automatically add required rules to security groups used with the service, and those rules may contain a cyclic dependency that prevent the security groups from being destroyed without removing the dependency first. Default `false`.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Map of tags to assign to the resource. If configured with a provider `default_tags` configuration block present, tags with matching keys will overwrite those defined at the provider-level.
-        :param pulumi.Input[str] vpc_id: VPC ID.
-               Defaults to the region's default VPC.
+        :param pulumi.Input[str] vpc_id: VPC ID. Defaults to the region's default VPC.
         """
         if description is None:
             description = 'Managed by Pulumi'
         if description is not None:
             pulumi.set(__self__, "description", description)
         if egress is not None:
             pulumi.set(__self__, "egress", egress)
@@ -1055,39 +1099,39 @@
         if vpc_id is not None:
             pulumi.set(__self__, "vpc_id", vpc_id)
 
     @property
     @pulumi.getter
     def description(self) -> Optional[pulumi.Input[str]]:
         """
-        Description of this egress rule.
+        Security group description. Defaults to `Managed by Pulumi`. Cannot be `""`. **NOTE**: This field maps to the AWS `GroupDescription` attribute, for which there is no Update API. If you'd like to classify your security groups in a way that can be updated, use `tags`.
         """
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter
     def egress(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ec2.SecurityGroupEgressArgs']]]]:
         """
-        Configuration block for egress rules. Can be specified multiple times for each egress rule. Each egress block supports fields documented below.
+        Configuration block for egress rules. Can be specified multiple times for each egress rule. Each egress block supports fields documented below. This argument is processed in attribute-as-blocks mode.
         """
         return pulumi.get(self, "egress")
 
     @egress.setter
     def egress(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ec2.SecurityGroupEgressArgs']]]]):
         pulumi.set(self, "egress", value)
 
     @property
     @pulumi.getter
     def ingress(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ec2.SecurityGroupIngressArgs']]]]:
         """
-        Configuration block for egress rules. Can be specified multiple times for each ingress rule. Each ingress block supports fields documented below.
+        Configuration block for ingress rules. Can be specified multiple times for each ingress rule. Each ingress block supports fields documented below. This argument is processed in attribute-as-blocks mode.
         """
         return pulumi.get(self, "ingress")
 
     @ingress.setter
     def ingress(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ec2.SecurityGroupIngressArgs']]]]):
         pulumi.set(self, "ingress", value)
 
@@ -1115,15 +1159,15 @@
     def name_prefix(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name_prefix", value)
 
     @property
     @pulumi.getter(name="revokeRulesOnDelete")
     def revoke_rules_on_delete(self) -> Optional[pulumi.Input[bool]]:
         """
-        Instruct this provider to revoke all of the Security Groups attached ingress and egress rules before deleting the rule itself. This is normally not needed, however certain AWS services such as Elastic Map Reduce may automatically add required rules to security groups used with the service, and those rules may contain a cyclic dependency that prevent the security groups from being destroyed without removing the dependency first. Default `false`.
+        Instruct the provider to revoke all of the Security Groups attached ingress and egress rules before deleting the rule itself. This is normally not needed, however certain AWS services such as Elastic Map Reduce may automatically add required rules to security groups used with the service, and those rules may contain a cyclic dependency that prevent the security groups from being destroyed without removing the dependency first. Default `false`.
         """
         return pulumi.get(self, "revoke_rules_on_delete")
 
     @revoke_rules_on_delete.setter
     def revoke_rules_on_delete(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "revoke_rules_on_delete", value)
 
@@ -1139,16 +1183,15 @@
     def tags(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "tags", value)
 
     @property
     @pulumi.getter(name="vpcId")
     def vpc_id(self) -> Optional[pulumi.Input[str]]:
         """
-        VPC ID.
-        Defaults to the region's default VPC.
+        VPC ID. Defaults to the region's default VPC.
         """
         return pulumi.get(self, "vpc_id")
 
     @vpc_id.setter
     def vpc_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "vpc_id", value)
```

### Comparing `pulumi_awsx-1.0.2/pulumi_awsx/cloudtrail/trail.py` & `pulumi_awsx-1.0.3/pulumi_awsx/cloudtrail/trail.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by pulumi-gen-awsx. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from .. import awsx as _awsx
 import pulumi_aws
@@ -38,19 +39,19 @@
         :param pulumi.Input[bool] enable_logging: Enables logging for the trail. Defaults to `true`. Setting this to `false` will pause logging.
         :param pulumi.Input[Sequence[pulumi.Input['pulumi_aws.cloudtrail.TrailEventSelectorArgs']]] event_selectors: Specifies an event selector for enabling data event logging. Fields documented below. Please note the [CloudTrail limits](https://docs.aws.amazon.com/awscloudtrail/latest/userguide/WhatIsCloudTrail-Limits.html) when configuring these. Conflicts with `advanced_event_selector`.
         :param pulumi.Input[bool] include_global_service_events: Whether the trail is publishing events from global services such as IAM to the log files. Defaults to `true`.
         :param pulumi.Input[Sequence[pulumi.Input['pulumi_aws.cloudtrail.TrailInsightSelectorArgs']]] insight_selectors: Configuration block for identifying unusual operational activity. See details below.
         :param pulumi.Input[bool] is_multi_region_trail: Whether the trail is created in the current region or in all regions. Defaults to `false`.
         :param pulumi.Input[bool] is_organization_trail: Whether the trail is an AWS Organizations trail. Organization trails log events for the master account and all member accounts. Can only be created in the organization master account. Defaults to `false`.
         :param pulumi.Input[str] kms_key_id: KMS key ARN to use to encrypt the logs delivered by CloudTrail.
-        :param pulumi.Input[str] name: Name of the advanced event selector.
+        :param pulumi.Input[str] name: Name of the trail.
         :param '_awsx.RequiredBucketArgs' s3_bucket: S3 bucket designated for publishing log files.
         :param pulumi.Input[str] s3_key_prefix: S3 key prefix that follows the name of the bucket you have designated for log file delivery.
         :param pulumi.Input[str] sns_topic_name: Name of the Amazon SNS topic defined for notification of log file delivery.
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Map of tags to assign to the trail. If configured with provider defaultTags present, tags with matching keys will overwrite those defined at the provider-level.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Map of tags to assign to the trail. If configured with a provider `default_tags` configuration block present, tags with matching keys will overwrite those defined at the provider-level.
         """
         if advanced_event_selectors is not None:
             pulumi.set(__self__, "advanced_event_selectors", advanced_event_selectors)
         if cloud_watch_logs_group is not None:
             pulumi.set(__self__, "cloud_watch_logs_group", cloud_watch_logs_group)
         if enable_log_file_validation is not None:
             pulumi.set(__self__, "enable_log_file_validation", enable_log_file_validation)
@@ -199,15 +200,15 @@
     def kms_key_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "kms_key_id", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Name of the advanced event selector.
+        Name of the trail.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -247,15 +248,15 @@
     def sns_topic_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "sns_topic_name", value)
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
-        Map of tags to assign to the trail. If configured with provider defaultTags present, tags with matching keys will overwrite those defined at the provider-level.
+        Map of tags to assign to the trail. If configured with a provider `default_tags` configuration block present, tags with matching keys will overwrite those defined at the provider-level.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
     def tags(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "tags", value)
 
@@ -291,19 +292,19 @@
         :param pulumi.Input[bool] enable_logging: Enables logging for the trail. Defaults to `true`. Setting this to `false` will pause logging.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['pulumi_aws.cloudtrail.TrailEventSelectorArgs']]]] event_selectors: Specifies an event selector for enabling data event logging. Fields documented below. Please note the [CloudTrail limits](https://docs.aws.amazon.com/awscloudtrail/latest/userguide/WhatIsCloudTrail-Limits.html) when configuring these. Conflicts with `advanced_event_selector`.
         :param pulumi.Input[bool] include_global_service_events: Whether the trail is publishing events from global services such as IAM to the log files. Defaults to `true`.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['pulumi_aws.cloudtrail.TrailInsightSelectorArgs']]]] insight_selectors: Configuration block for identifying unusual operational activity. See details below.
         :param pulumi.Input[bool] is_multi_region_trail: Whether the trail is created in the current region or in all regions. Defaults to `false`.
         :param pulumi.Input[bool] is_organization_trail: Whether the trail is an AWS Organizations trail. Organization trails log events for the master account and all member accounts. Can only be created in the organization master account. Defaults to `false`.
         :param pulumi.Input[str] kms_key_id: KMS key ARN to use to encrypt the logs delivered by CloudTrail.
-        :param pulumi.Input[str] name: Name of the advanced event selector.
+        :param pulumi.Input[str] name: Name of the trail.
         :param pulumi.InputType['_awsx.RequiredBucketArgs'] s3_bucket: S3 bucket designated for publishing log files.
         :param pulumi.Input[str] s3_key_prefix: S3 key prefix that follows the name of the bucket you have designated for log file delivery.
         :param pulumi.Input[str] sns_topic_name: Name of the Amazon SNS topic defined for notification of log file delivery.
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Map of tags to assign to the trail. If configured with provider defaultTags present, tags with matching keys will overwrite those defined at the provider-level.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Map of tags to assign to the trail. If configured with a provider `default_tags` configuration block present, tags with matching keys will overwrite those defined at the provider-level.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[TrailArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -336,20 +337,17 @@
                  kms_key_id: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  s3_bucket: Optional[pulumi.InputType['_awsx.RequiredBucketArgs']] = None,
                  s3_key_prefix: Optional[pulumi.Input[str]] = None,
                  sns_topic_name: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = TrailArgs.__new__(TrailArgs)
```

### Comparing `pulumi_awsx-1.0.2/pulumi_awsx/ec2/_enums.py` & `pulumi_awsx-1.0.3/pulumi_awsx/ec2/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-1.0.2/pulumi_awsx/ec2/_inputs.py` & `pulumi_awsx-1.0.3/pulumi_awsx/ec2/_inputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by pulumi-gen-awsx. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from ._enums import *
 import pulumi_aws
@@ -137,14 +138,24 @@
                  private_dns_enabled: Optional[bool] = None,
                  route_table_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  security_group_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  subnet_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  vpc_endpoint_type: Optional[pulumi.Input[str]] = None):
         """
+        Provides a VPC Endpoint resource.
+
+        > **NOTE on VPC Endpoints and VPC Endpoint Associations:** The provider provides both standalone VPC Endpoint Associations for
+        Route Tables - (an association between a VPC endpoint and a single `route_table_id`),
+        Security Groups - (an association between a VPC endpoint and a single `security_group_id`),
+        and Subnets - (an association between a VPC endpoint and a single `subnet_id`) and
+        a VPC Endpoint resource with `route_table_ids` and `subnet_ids` attributes.
+        Do not use the same resource ID in both a VPC Endpoint resource and a VPC Endpoint Association resource.
+        Doing so will cause a conflict of associations and will overwrite the association.
+
         {{% examples %}}
         ## Example Usage
         {{% example %}}
         ### Basic
 
         ```typescript
         import * as pulumi from "@pulumi/pulumi";
@@ -405,15 +416,15 @@
         func main() {
         	pulumi.Run(func(ctx *pulumi.Context) error {
         		_, err := ec2.NewVpcEndpoint(ctx, "ec2", &ec2.VpcEndpointArgs{
         			VpcId:           pulumi.Any(aws_vpc.Main.Id),
         			ServiceName:     pulumi.String("com.amazonaws.us-west-2.ec2"),
         			VpcEndpointType: pulumi.String("Interface"),
         			SecurityGroupIds: pulumi.StringArray{
-        				pulumi.Any(aws_security_group.Sg1.Id),
+        				aws_security_group.Sg1.Id,
         			},
         			PrivateDnsEnabled: pulumi.Bool(true),
         		})
         		if err != nil {
         			return err
         		}
         		return nil
@@ -549,27 +560,27 @@
         		current, err := aws.GetCallerIdentity(ctx, nil, nil)
         		if err != nil {
         			return err
         		}
         		exampleVpcEndpointService, err := ec2.NewVpcEndpointService(ctx, "exampleVpcEndpointService", &ec2.VpcEndpointServiceArgs{
         			AcceptanceRequired: pulumi.Bool(false),
         			AllowedPrincipals: pulumi.StringArray{
-        				pulumi.String(current.Arn),
+        				*pulumi.String(current.Arn),
         			},
         			GatewayLoadBalancerArns: pulumi.StringArray{
-        				pulumi.Any(aws_lb.Example.Arn),
+        				aws_lb.Example.Arn,
         			},
         		})
         		if err != nil {
         			return err
         		}
         		_, err = ec2.NewVpcEndpoint(ctx, "exampleVpcEndpoint", &ec2.VpcEndpointArgs{
         			ServiceName: exampleVpcEndpointService.ServiceName,
         			SubnetIds: pulumi.StringArray{
-        				pulumi.Any(aws_subnet.Example.Id),
+        				aws_subnet.Example.Id,
         			},
         			VpcEndpointType: exampleVpcEndpointService.ServiceType,
         			VpcId:           pulumi.Any(aws_vpc.Example.Id),
         		})
         		if err != nil {
         			return err
         		}
@@ -635,15 +646,15 @@
               serviceName: ${exampleVpcEndpointService.serviceName}
               subnetIds:
                 - ${aws_subnet.example.id}
               vpcEndpointType: ${exampleVpcEndpointService.serviceType}
               vpcId: ${aws_vpc.example.id}
         variables:
           current:
-            Fn::Invoke:
+            fn::invoke:
               Function: aws:getCallerIdentity
               Arguments: {}
         ```
         {{% /example %}}
         {{% /examples %}}
 
         ## Import
```

### Comparing `pulumi_awsx-1.0.2/pulumi_awsx/ec2/default_vpc.py` & `pulumi_awsx-1.0.3/pulumi_awsx/ec2/default_vpc.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by pulumi-gen-awsx. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['DefaultVpcArgs', 'DefaultVpc']
@@ -52,20 +53,17 @@
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = DefaultVpcArgs.__new__(DefaultVpcArgs)
```

### Comparing `pulumi_awsx-1.0.2/pulumi_awsx/ec2/get_default_vpc.py` & `pulumi_awsx-1.0.3/pulumi_awsx/ec2/get_default_vpc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by pulumi-gen-awsx. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
@@ -64,17 +65,14 @@
 
 def get_default_vpc(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetDefaultVpcResult:
     """
     [NOT YET IMPLEMENTED] Get the Default VPC for a region.
     """
     pulumi.log.warn("""get_default_vpc is deprecated: Waiting for https://github.com/pulumi/pulumi/issues/7583. Use the DefaultVpc resource until resolved.""")
     __args__ = dict()
-    if opts is None:
-        opts = pulumi.InvokeOptions()
-    if opts.version is None:
-        opts.version = _utilities.get_version()
+    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('awsx:ec2:getDefaultVpc', __args__, opts=opts, typ=GetDefaultVpcResult).value
 
     return AwaitableGetDefaultVpcResult(
         private_subnet_ids=__ret__.private_subnet_ids,
         public_subnet_ids=__ret__.public_subnet_ids,
         vpc_id=__ret__.vpc_id)
```

### Comparing `pulumi_awsx-1.0.2/pulumi_awsx/ec2/vpc.py` & `pulumi_awsx-1.0.3/pulumi_awsx/ec2/vpc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by pulumi-gen-awsx. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from ._enums import *
 from ._inputs import *
@@ -19,14 +20,15 @@
                  assign_generated_ipv6_cidr_block: Optional[pulumi.Input[bool]] = None,
                  availability_zone_names: Optional[Sequence[str]] = None,
                  cidr_block: Optional[str] = None,
                  enable_classiclink: Optional[pulumi.Input[bool]] = None,
                  enable_classiclink_dns_support: Optional[pulumi.Input[bool]] = None,
                  enable_dns_hostnames: Optional[pulumi.Input[bool]] = None,
                  enable_dns_support: Optional[pulumi.Input[bool]] = None,
+                 enable_network_address_usage_metrics: Optional[pulumi.Input[bool]] = None,
                  instance_tenancy: Optional[pulumi.Input[str]] = None,
                  ipv4_ipam_pool_id: Optional[pulumi.Input[str]] = None,
                  ipv4_netmask_length: Optional[pulumi.Input[int]] = None,
                  ipv6_cidr_block: Optional[pulumi.Input[str]] = None,
                  ipv6_cidr_block_network_border_group: Optional[pulumi.Input[str]] = None,
                  ipv6_ipam_pool_id: Optional[pulumi.Input[str]] = None,
                  ipv6_netmask_length: Optional[pulumi.Input[int]] = None,
@@ -42,15 +44,16 @@
         :param str cidr_block: The CIDR block for the VPC. Optional. Defaults to 10.0.0.0/16.
         :param pulumi.Input[bool] enable_classiclink: A boolean flag to enable/disable ClassicLink
                for the VPC. Only valid in regions and accounts that support EC2 Classic.
                See the [ClassicLink documentation](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/vpc-classiclink.html) for more information. Defaults false.
         :param pulumi.Input[bool] enable_classiclink_dns_support: A boolean flag to enable/disable ClassicLink DNS Support for the VPC.
                Only valid in regions and accounts that support EC2 Classic.
         :param pulumi.Input[bool] enable_dns_hostnames: A boolean flag to enable/disable DNS hostnames in the VPC. Defaults false.
-        :param pulumi.Input[bool] enable_dns_support: A boolean flag to enable/disable DNS support in the VPC. Defaults true.
+        :param pulumi.Input[bool] enable_dns_support: A boolean flag to enable/disable DNS support in the VPC. Defaults to true.
+        :param pulumi.Input[bool] enable_network_address_usage_metrics: Indicates whether Network Address Usage metrics are enabled for your VPC. Defaults to false.
         :param pulumi.Input[str] instance_tenancy: A tenancy option for instances launched into the VPC. Default is `default`, which ensures that EC2 instances launched in this VPC use the EC2 instance tenancy attribute specified when the EC2 instance is launched. The only other option is `dedicated`, which ensures that EC2 instances launched in this VPC are run on dedicated tenancy instances regardless of the tenancy attribute specified at launch. This has a dedicated per region fee of $2 per hour, plus an hourly per instance usage fee.
         :param pulumi.Input[str] ipv4_ipam_pool_id: The ID of an IPv4 IPAM pool you want to use for allocating this VPC's CIDR. IPAM is a VPC feature that you can use to automate your IP address management workflows including assigning, tracking, troubleshooting, and auditing IP addresses across AWS Regions and accounts. Using IPAM you can monitor IP address usage throughout your AWS Organization.
         :param pulumi.Input[int] ipv4_netmask_length: The netmask length of the IPv4 CIDR you want to allocate to this VPC. Requires specifying a `ipv4_ipam_pool_id`.
         :param pulumi.Input[str] ipv6_cidr_block: IPv6 CIDR block to request from an IPAM Pool. Can be set explicitly or derived from IPAM using `ipv6_netmask_length`.
         :param pulumi.Input[str] ipv6_cidr_block_network_border_group: By default when an IPv6 CIDR is assigned to a VPC a default ipv6_cidr_block_network_border_group will be set to the region of the VPC. This can be changed to restrict advertisement of public addresses to specific Network Border Groups such as LocalZones.
         :param pulumi.Input[str] ipv6_ipam_pool_id: IPAM Pool ID for a IPv6 pool. Conflicts with `assign_generated_ipv6_cidr_block`.
         :param pulumi.Input[int] ipv6_netmask_length: Netmask length to request from IPAM Pool. Conflicts with `ipv6_cidr_block`. This can be omitted if IPAM pool as a `allocation_default_netmask_length` set. Valid values: `56`.
@@ -76,14 +79,16 @@
             pulumi.log.warn("""enable_classiclink_dns_support is deprecated: With the retirement of EC2-Classic the enable_classiclink_dns_support attribute has been deprecated and will be removed in a future version.""")
         if enable_classiclink_dns_support is not None:
             pulumi.set(__self__, "enable_classiclink_dns_support", enable_classiclink_dns_support)
         if enable_dns_hostnames is not None:
             pulumi.set(__self__, "enable_dns_hostnames", enable_dns_hostnames)
         if enable_dns_support is not None:
             pulumi.set(__self__, "enable_dns_support", enable_dns_support)
+        if enable_network_address_usage_metrics is not None:
+            pulumi.set(__self__, "enable_network_address_usage_metrics", enable_network_address_usage_metrics)
         if instance_tenancy is not None:
             pulumi.set(__self__, "instance_tenancy", instance_tenancy)
         if ipv4_ipam_pool_id is not None:
             pulumi.set(__self__, "ipv4_ipam_pool_id", ipv4_ipam_pool_id)
         if ipv4_netmask_length is not None:
             pulumi.set(__self__, "ipv4_netmask_length", ipv4_netmask_length)
         if ipv6_cidr_block is not None:
@@ -180,23 +185,35 @@
     def enable_dns_hostnames(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enable_dns_hostnames", value)
 
     @property
     @pulumi.getter(name="enableDnsSupport")
     def enable_dns_support(self) -> Optional[pulumi.Input[bool]]:
         """
-        A boolean flag to enable/disable DNS support in the VPC. Defaults true.
+        A boolean flag to enable/disable DNS support in the VPC. Defaults to true.
         """
         return pulumi.get(self, "enable_dns_support")
 
     @enable_dns_support.setter
     def enable_dns_support(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enable_dns_support", value)
 
     @property
+    @pulumi.getter(name="enableNetworkAddressUsageMetrics")
+    def enable_network_address_usage_metrics(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Indicates whether Network Address Usage metrics are enabled for your VPC. Defaults to false.
+        """
+        return pulumi.get(self, "enable_network_address_usage_metrics")
+
+    @enable_network_address_usage_metrics.setter
+    def enable_network_address_usage_metrics(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "enable_network_address_usage_metrics", value)
+
+    @property
     @pulumi.getter(name="instanceTenancy")
     def instance_tenancy(self) -> Optional[pulumi.Input[str]]:
         """
         A tenancy option for instances launched into the VPC. Default is `default`, which ensures that EC2 instances launched in this VPC use the EC2 instance tenancy attribute specified when the EC2 instance is launched. The only other option is `dedicated`, which ensures that EC2 instances launched in this VPC are run on dedicated tenancy instances regardless of the tenancy attribute specified at launch. This has a dedicated per region fee of $2 per hour, plus an hourly per instance usage fee.
         """
         return pulumi.get(self, "instance_tenancy")
 
@@ -345,14 +362,15 @@
                  assign_generated_ipv6_cidr_block: Optional[pulumi.Input[bool]] = None,
                  availability_zone_names: Optional[Sequence[str]] = None,
                  cidr_block: Optional[str] = None,
                  enable_classiclink: Optional[pulumi.Input[bool]] = None,
                  enable_classiclink_dns_support: Optional[pulumi.Input[bool]] = None,
                  enable_dns_hostnames: Optional[pulumi.Input[bool]] = None,
                  enable_dns_support: Optional[pulumi.Input[bool]] = None,
+                 enable_network_address_usage_metrics: Optional[pulumi.Input[bool]] = None,
                  instance_tenancy: Optional[pulumi.Input[str]] = None,
                  ipv4_ipam_pool_id: Optional[pulumi.Input[str]] = None,
                  ipv4_netmask_length: Optional[pulumi.Input[int]] = None,
                  ipv6_cidr_block: Optional[pulumi.Input[str]] = None,
                  ipv6_cidr_block_network_border_group: Optional[pulumi.Input[str]] = None,
                  ipv6_ipam_pool_id: Optional[pulumi.Input[str]] = None,
                  ipv6_netmask_length: Optional[pulumi.Input[int]] = None,
@@ -371,15 +389,16 @@
         :param str cidr_block: The CIDR block for the VPC. Optional. Defaults to 10.0.0.0/16.
         :param pulumi.Input[bool] enable_classiclink: A boolean flag to enable/disable ClassicLink
                for the VPC. Only valid in regions and accounts that support EC2 Classic.
                See the [ClassicLink documentation](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/vpc-classiclink.html) for more information. Defaults false.
         :param pulumi.Input[bool] enable_classiclink_dns_support: A boolean flag to enable/disable ClassicLink DNS Support for the VPC.
                Only valid in regions and accounts that support EC2 Classic.
         :param pulumi.Input[bool] enable_dns_hostnames: A boolean flag to enable/disable DNS hostnames in the VPC. Defaults false.
-        :param pulumi.Input[bool] enable_dns_support: A boolean flag to enable/disable DNS support in the VPC. Defaults true.
+        :param pulumi.Input[bool] enable_dns_support: A boolean flag to enable/disable DNS support in the VPC. Defaults to true.
+        :param pulumi.Input[bool] enable_network_address_usage_metrics: Indicates whether Network Address Usage metrics are enabled for your VPC. Defaults to false.
         :param pulumi.Input[str] instance_tenancy: A tenancy option for instances launched into the VPC. Default is `default`, which ensures that EC2 instances launched in this VPC use the EC2 instance tenancy attribute specified when the EC2 instance is launched. The only other option is `dedicated`, which ensures that EC2 instances launched in this VPC are run on dedicated tenancy instances regardless of the tenancy attribute specified at launch. This has a dedicated per region fee of $2 per hour, plus an hourly per instance usage fee.
         :param pulumi.Input[str] ipv4_ipam_pool_id: The ID of an IPv4 IPAM pool you want to use for allocating this VPC's CIDR. IPAM is a VPC feature that you can use to automate your IP address management workflows including assigning, tracking, troubleshooting, and auditing IP addresses across AWS Regions and accounts. Using IPAM you can monitor IP address usage throughout your AWS Organization.
         :param pulumi.Input[int] ipv4_netmask_length: The netmask length of the IPv4 CIDR you want to allocate to this VPC. Requires specifying a `ipv4_ipam_pool_id`.
         :param pulumi.Input[str] ipv6_cidr_block: IPv6 CIDR block to request from an IPAM Pool. Can be set explicitly or derived from IPAM using `ipv6_netmask_length`.
         :param pulumi.Input[str] ipv6_cidr_block_network_border_group: By default when an IPv6 CIDR is assigned to a VPC a default ipv6_cidr_block_network_border_group will be set to the region of the VPC. This can be changed to restrict advertisement of public addresses to specific Network Border Groups such as LocalZones.
         :param pulumi.Input[str] ipv6_ipam_pool_id: IPAM Pool ID for a IPv6 pool. Conflicts with `assign_generated_ipv6_cidr_block`.
         :param pulumi.Input[int] ipv6_netmask_length: Netmask length to request from IPAM Pool. Conflicts with `ipv6_cidr_block`. This can be omitted if IPAM pool as a `allocation_default_netmask_length` set. Valid values: `56`.
@@ -415,33 +434,31 @@
                  assign_generated_ipv6_cidr_block: Optional[pulumi.Input[bool]] = None,
                  availability_zone_names: Optional[Sequence[str]] = None,
                  cidr_block: Optional[str] = None,
                  enable_classiclink: Optional[pulumi.Input[bool]] = None,
                  enable_classiclink_dns_support: Optional[pulumi.Input[bool]] = None,
                  enable_dns_hostnames: Optional[pulumi.Input[bool]] = None,
                  enable_dns_support: Optional[pulumi.Input[bool]] = None,
+                 enable_network_address_usage_metrics: Optional[pulumi.Input[bool]] = None,
                  instance_tenancy: Optional[pulumi.Input[str]] = None,
                  ipv4_ipam_pool_id: Optional[pulumi.Input[str]] = None,
                  ipv4_netmask_length: Optional[pulumi.Input[int]] = None,
                  ipv6_cidr_block: Optional[pulumi.Input[str]] = None,
                  ipv6_cidr_block_network_border_group: Optional[pulumi.Input[str]] = None,
                  ipv6_ipam_pool_id: Optional[pulumi.Input[str]] = None,
                  ipv6_netmask_length: Optional[pulumi.Input[int]] = None,
                  nat_gateways: Optional[pulumi.InputType['NatGatewayConfigurationArgs']] = None,
                  number_of_availability_zones: Optional[int] = None,
                  subnet_specs: Optional[Sequence[pulumi.InputType['SubnetSpecArgs']]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  vpc_endpoint_specs: Optional[Sequence[pulumi.InputType['VpcEndpointSpecArgs']]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = VpcArgs.__new__(VpcArgs)
 
@@ -454,14 +471,15 @@
             __props__.__dict__["enable_classiclink"] = enable_classiclink
             if enable_classiclink_dns_support is not None and not opts.urn:
                 warnings.warn("""With the retirement of EC2-Classic the enable_classiclink_dns_support attribute has been deprecated and will be removed in a future version.""", DeprecationWarning)
                 pulumi.log.warn("""enable_classiclink_dns_support is deprecated: With the retirement of EC2-Classic the enable_classiclink_dns_support attribute has been deprecated and will be removed in a future version.""")
             __props__.__dict__["enable_classiclink_dns_support"] = enable_classiclink_dns_support
             __props__.__dict__["enable_dns_hostnames"] = enable_dns_hostnames
             __props__.__dict__["enable_dns_support"] = enable_dns_support
+            __props__.__dict__["enable_network_address_usage_metrics"] = enable_network_address_usage_metrics
             __props__.__dict__["instance_tenancy"] = instance_tenancy
             __props__.__dict__["ipv4_ipam_pool_id"] = ipv4_ipam_pool_id
             __props__.__dict__["ipv4_netmask_length"] = ipv4_netmask_length
             __props__.__dict__["ipv6_cidr_block"] = ipv6_cidr_block
             __props__.__dict__["ipv6_cidr_block_network_border_group"] = ipv6_cidr_block_network_border_group
             __props__.__dict__["ipv6_ipam_pool_id"] = ipv6_ipam_pool_id
             __props__.__dict__["ipv6_netmask_length"] = ipv6_netmask_length
```

### Comparing `pulumi_awsx-1.0.2/pulumi_awsx/ecr/_enums.py` & `pulumi_awsx-1.0.3/pulumi_awsx/ecr/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-1.0.2/pulumi_awsx/ecr/_inputs.py` & `pulumi_awsx-1.0.3/pulumi_awsx/ecr/_inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by pulumi-gen-awsx. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from ._enums import *
```

### Comparing `pulumi_awsx-1.0.2/pulumi_awsx/ecr/image.py` & `pulumi_awsx-1.0.3/pulumi_awsx/ecr/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by pulumi-gen-awsx. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = ['ImageArgs', 'Image']
@@ -202,20 +203,17 @@
                  dockerfile: Optional[pulumi.Input[str]] = None,
                  env: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  extra_options: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  path: Optional[pulumi.Input[str]] = None,
                  repository_url: Optional[pulumi.Input[str]] = None,
                  target: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ImageArgs.__new__(ImageArgs)
```

### Comparing `pulumi_awsx-1.0.2/pulumi_awsx/ecr/repository.py` & `pulumi_awsx-1.0.3/pulumi_awsx/ecr/repository.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by pulumi-gen-awsx. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from ._enums import *
 from ._inputs import *
@@ -194,20 +195,17 @@
                  force_delete: Optional[pulumi.Input[bool]] = None,
                  image_scanning_configuration: Optional[pulumi.Input[pulumi.InputType['pulumi_aws.ecr.RepositoryImageScanningConfigurationArgs']]] = None,
                  image_tag_mutability: Optional[pulumi.Input[str]] = None,
                  lifecycle_policy: Optional[pulumi.InputType['LifecyclePolicyArgs']] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = RepositoryArgs.__new__(RepositoryArgs)
```

### Comparing `pulumi_awsx-1.0.2/pulumi_awsx/ecs/_inputs.py` & `pulumi_awsx-1.0.3/pulumi_awsx/ecs/_inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by pulumi-gen-awsx. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from .. import awsx as _awsx
 import pulumi_aws
```

### Comparing `pulumi_awsx-1.0.2/pulumi_awsx/ecs/ec2_service.py` & `pulumi_awsx-1.0.3/pulumi_awsx/ecs/ec2_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 # coding=utf-8
 # *** WARNING: this file was generated by pulumi-gen-awsx. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from .. import awsx as _awsx
 from ._inputs import *
 import pulumi_aws
 
 __all__ = ['EC2ServiceArgs', 'EC2Service']
 
 @pulumi.input_type
 class EC2ServiceArgs:
     def __init__(__self__, *,
+                 alarms: Optional[pulumi.Input['pulumi_aws.ecs.ServiceAlarmsArgs']] = None,
                  cluster: Optional[pulumi.Input[str]] = None,
                  continue_before_steady_state: Optional[pulumi.Input[bool]] = None,
                  deployment_circuit_breaker: Optional[pulumi.Input['pulumi_aws.ecs.ServiceDeploymentCircuitBreakerArgs']] = None,
                  deployment_controller: Optional[pulumi.Input['pulumi_aws.ecs.ServiceDeploymentControllerArgs']] = None,
                  deployment_maximum_percent: Optional[pulumi.Input[int]] = None,
                  deployment_minimum_healthy_percent: Optional[pulumi.Input[int]] = None,
                  desired_count: Optional[pulumi.Input[int]] = None,
@@ -32,20 +34,23 @@
                  name: Optional[pulumi.Input[str]] = None,
                  network_configuration: Optional[pulumi.Input['pulumi_aws.ecs.ServiceNetworkConfigurationArgs']] = None,
                  ordered_placement_strategies: Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ecs.ServiceOrderedPlacementStrategyArgs']]]] = None,
                  placement_constraints: Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ecs.ServicePlacementConstraintArgs']]]] = None,
                  platform_version: Optional[pulumi.Input[str]] = None,
                  propagate_tags: Optional[pulumi.Input[str]] = None,
                  scheduling_strategy: Optional[pulumi.Input[str]] = None,
+                 service_connect_configuration: Optional[pulumi.Input['pulumi_aws.ecs.ServiceServiceConnectConfigurationArgs']] = None,
                  service_registries: Optional[pulumi.Input['pulumi_aws.ecs.ServiceServiceRegistriesArgs']] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  task_definition: Optional[pulumi.Input[str]] = None,
-                 task_definition_args: Optional['EC2ServiceTaskDefinitionArgs'] = None):
+                 task_definition_args: Optional['EC2ServiceTaskDefinitionArgs'] = None,
+                 triggers: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
         """
         The set of arguments for constructing a EC2Service resource.
+        :param pulumi.Input['pulumi_aws.ecs.ServiceAlarmsArgs'] alarms: Information about the CloudWatch alarms. See below.
         :param pulumi.Input[str] cluster: ARN of an ECS cluster.
         :param pulumi.Input[bool] continue_before_steady_state: If `true`, this provider will not wait for the service to reach a steady state (like [`aws ecs wait services-stable`](https://docs.aws.amazon.com/cli/latest/reference/ecs/wait/services-stable.html)) before continuing. Default `false`.
         :param pulumi.Input['pulumi_aws.ecs.ServiceDeploymentCircuitBreakerArgs'] deployment_circuit_breaker: Configuration block for deployment circuit breaker. See below.
         :param pulumi.Input['pulumi_aws.ecs.ServiceDeploymentControllerArgs'] deployment_controller: Configuration block for deployment controller configuration. See below.
         :param pulumi.Input[int] deployment_maximum_percent: Upper limit (as a percentage of the service's desiredCount) of the number of running tasks that can be running in a service during a deployment. Not valid when using the `DAEMON` scheduling strategy.
         :param pulumi.Input[int] deployment_minimum_healthy_percent: Lower limit (as a percentage of the service's desiredCount) of the number of running tasks that must remain running and healthy in a service during a deployment.
         :param pulumi.Input[int] desired_count: Number of instances of the task definition to place and keep running. Defaults to 0. Do not specify if using the `DAEMON` scheduling strategy.
@@ -58,19 +63,23 @@
         :param pulumi.Input[str] name: Name of the service (up to 255 letters, numbers, hyphens, and underscores)
         :param pulumi.Input['pulumi_aws.ecs.ServiceNetworkConfigurationArgs'] network_configuration: Network configuration for the service. This parameter is required for task definitions that use the `awsvpc` network mode to receive their own Elastic Network Interface, and it is not supported for other network modes. See below.
         :param pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ecs.ServiceOrderedPlacementStrategyArgs']]] ordered_placement_strategies: Service level strategy rules that are taken into consideration during task placement. List from top to bottom in order of precedence. Updates to this configuration will take effect next task deployment unless `force_new_deployment` is enabled. The maximum number of `ordered_placement_strategy` blocks is `5`. See below.
         :param pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ecs.ServicePlacementConstraintArgs']]] placement_constraints: Rules that are taken into consideration during task placement. Updates to this configuration will take effect next task deployment unless `force_new_deployment` is enabled. Maximum number of `placement_constraints` is `10`. See below.
         :param pulumi.Input[str] platform_version: Platform version on which to run your service. Only applicable for `launch_type` set to `FARGATE`. Defaults to `LATEST`. More information about Fargate platform versions can be found in the [AWS ECS User Guide](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/platform_versions.html).
         :param pulumi.Input[str] propagate_tags: Specifies whether to propagate the tags from the task definition or the service to the tasks. The valid values are `SERVICE` and `TASK_DEFINITION`.
         :param pulumi.Input[str] scheduling_strategy: Scheduling strategy to use for the service. The valid values are `REPLICA` and `DAEMON`. Defaults to `REPLICA`. Note that [*Tasks using the Fargate launch type or the `CODE_DEPLOY` or `EXTERNAL` deployment controller types don't support the `DAEMON` scheduling strategy*](https://docs.aws.amazon.com/AmazonECS/latest/APIReference/API_CreateService.html).
+        :param pulumi.Input['pulumi_aws.ecs.ServiceServiceConnectConfigurationArgs'] service_connect_configuration: The ECS Service Connect configuration for this service to discover and connect to services, and be discovered by, and connected from, other services within a namespace. See below.
         :param pulumi.Input['pulumi_aws.ecs.ServiceServiceRegistriesArgs'] service_registries: Service discovery registries for the service. The maximum number of `service_registries` blocks is `1`. See below.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Key-value map of resource tags. If configured with a provider `default_tags` configuration block present, tags with matching keys will overwrite those defined at the provider-level.
         :param pulumi.Input[str] task_definition: Family and revision (`family:revision`) or full ARN of the task definition that you want to run in your service. Either [taskDefinition] or [taskDefinitionArgs] must be provided.
         :param 'EC2ServiceTaskDefinitionArgs' task_definition_args: The args of task definition that you want to run in your service. Either [taskDefinition] or [taskDefinitionArgs] must be provided.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] triggers: Map of arbitrary keys and values that, when changed, will trigger an in-place update (redeployment). Useful with `timestamp()`. See example above.
         """
+        if alarms is not None:
+            pulumi.set(__self__, "alarms", alarms)
         if cluster is not None:
             pulumi.set(__self__, "cluster", cluster)
         if continue_before_steady_state is not None:
             pulumi.set(__self__, "continue_before_steady_state", continue_before_steady_state)
         if deployment_circuit_breaker is not None:
             pulumi.set(__self__, "deployment_circuit_breaker", deployment_circuit_breaker)
         if deployment_controller is not None:
@@ -103,22 +112,38 @@
             pulumi.set(__self__, "placement_constraints", placement_constraints)
         if platform_version is not None:
             pulumi.set(__self__, "platform_version", platform_version)
         if propagate_tags is not None:
             pulumi.set(__self__, "propagate_tags", propagate_tags)
         if scheduling_strategy is not None:
             pulumi.set(__self__, "scheduling_strategy", scheduling_strategy)
+        if service_connect_configuration is not None:
+            pulumi.set(__self__, "service_connect_configuration", service_connect_configuration)
         if service_registries is not None:
             pulumi.set(__self__, "service_registries", service_registries)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if task_definition is not None:
             pulumi.set(__self__, "task_definition", task_definition)
         if task_definition_args is not None:
             pulumi.set(__self__, "task_definition_args", task_definition_args)
+        if triggers is not None:
+            pulumi.set(__self__, "triggers", triggers)
+
+    @property
+    @pulumi.getter
+    def alarms(self) -> Optional[pulumi.Input['pulumi_aws.ecs.ServiceAlarmsArgs']]:
+        """
+        Information about the CloudWatch alarms. See below.
+        """
+        return pulumi.get(self, "alarms")
+
+    @alarms.setter
+    def alarms(self, value: Optional[pulumi.Input['pulumi_aws.ecs.ServiceAlarmsArgs']]):
+        pulumi.set(self, "alarms", value)
 
     @property
     @pulumi.getter
     def cluster(self) -> Optional[pulumi.Input[str]]:
         """
         ARN of an ECS cluster.
         """
@@ -353,14 +378,26 @@
         return pulumi.get(self, "scheduling_strategy")
 
     @scheduling_strategy.setter
     def scheduling_strategy(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "scheduling_strategy", value)
 
     @property
+    @pulumi.getter(name="serviceConnectConfiguration")
+    def service_connect_configuration(self) -> Optional[pulumi.Input['pulumi_aws.ecs.ServiceServiceConnectConfigurationArgs']]:
+        """
+        The ECS Service Connect configuration for this service to discover and connect to services, and be discovered by, and connected from, other services within a namespace. See below.
+        """
+        return pulumi.get(self, "service_connect_configuration")
+
+    @service_connect_configuration.setter
+    def service_connect_configuration(self, value: Optional[pulumi.Input['pulumi_aws.ecs.ServiceServiceConnectConfigurationArgs']]):
+        pulumi.set(self, "service_connect_configuration", value)
+
+    @property
     @pulumi.getter(name="serviceRegistries")
     def service_registries(self) -> Optional[pulumi.Input['pulumi_aws.ecs.ServiceServiceRegistriesArgs']]:
         """
         Service discovery registries for the service. The maximum number of `service_registries` blocks is `1`. See below.
         """
         return pulumi.get(self, "service_registries")
 
@@ -400,20 +437,33 @@
         """
         return pulumi.get(self, "task_definition_args")
 
     @task_definition_args.setter
     def task_definition_args(self, value: Optional['EC2ServiceTaskDefinitionArgs']):
         pulumi.set(self, "task_definition_args", value)
 
+    @property
+    @pulumi.getter
+    def triggers(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+        """
+        Map of arbitrary keys and values that, when changed, will trigger an in-place update (redeployment). Useful with `timestamp()`. See example above.
+        """
+        return pulumi.get(self, "triggers")
+
+    @triggers.setter
+    def triggers(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
+        pulumi.set(self, "triggers", value)
+
 
 class EC2Service(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
+                 alarms: Optional[pulumi.Input[pulumi.InputType['pulumi_aws.ecs.ServiceAlarmsArgs']]] = None,
                  cluster: Optional[pulumi.Input[str]] = None,
                  continue_before_steady_state: Optional[pulumi.Input[bool]] = None,
                  deployment_circuit_breaker: Optional[pulumi.Input[pulumi.InputType['pulumi_aws.ecs.ServiceDeploymentCircuitBreakerArgs']]] = None,
                  deployment_controller: Optional[pulumi.Input[pulumi.InputType['pulumi_aws.ecs.ServiceDeploymentControllerArgs']]] = None,
                  deployment_maximum_percent: Optional[pulumi.Input[int]] = None,
                  deployment_minimum_healthy_percent: Optional[pulumi.Input[int]] = None,
                  desired_count: Optional[pulumi.Input[int]] = None,
@@ -426,25 +476,28 @@
                  name: Optional[pulumi.Input[str]] = None,
                  network_configuration: Optional[pulumi.Input[pulumi.InputType['pulumi_aws.ecs.ServiceNetworkConfigurationArgs']]] = None,
                  ordered_placement_strategies: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['pulumi_aws.ecs.ServiceOrderedPlacementStrategyArgs']]]]] = None,
                  placement_constraints: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['pulumi_aws.ecs.ServicePlacementConstraintArgs']]]]] = None,
                  platform_version: Optional[pulumi.Input[str]] = None,
                  propagate_tags: Optional[pulumi.Input[str]] = None,
                  scheduling_strategy: Optional[pulumi.Input[str]] = None,
+                 service_connect_configuration: Optional[pulumi.Input[pulumi.InputType['pulumi_aws.ecs.ServiceServiceConnectConfigurationArgs']]] = None,
                  service_registries: Optional[pulumi.Input[pulumi.InputType['pulumi_aws.ecs.ServiceServiceRegistriesArgs']]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  task_definition: Optional[pulumi.Input[str]] = None,
                  task_definition_args: Optional[pulumi.InputType['EC2ServiceTaskDefinitionArgs']] = None,
+                 triggers: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  __props__=None):
         """
         Create an ECS Service resource for EC2 with the given unique name, arguments, and options.
         Creates Task definition if `taskDefinitionArgs` is specified.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[pulumi.InputType['pulumi_aws.ecs.ServiceAlarmsArgs']] alarms: Information about the CloudWatch alarms. See below.
         :param pulumi.Input[str] cluster: ARN of an ECS cluster.
         :param pulumi.Input[bool] continue_before_steady_state: If `true`, this provider will not wait for the service to reach a steady state (like [`aws ecs wait services-stable`](https://docs.aws.amazon.com/cli/latest/reference/ecs/wait/services-stable.html)) before continuing. Default `false`.
         :param pulumi.Input[pulumi.InputType['pulumi_aws.ecs.ServiceDeploymentCircuitBreakerArgs']] deployment_circuit_breaker: Configuration block for deployment circuit breaker. See below.
         :param pulumi.Input[pulumi.InputType['pulumi_aws.ecs.ServiceDeploymentControllerArgs']] deployment_controller: Configuration block for deployment controller configuration. See below.
         :param pulumi.Input[int] deployment_maximum_percent: Upper limit (as a percentage of the service's desiredCount) of the number of running tasks that can be running in a service during a deployment. Not valid when using the `DAEMON` scheduling strategy.
         :param pulumi.Input[int] deployment_minimum_healthy_percent: Lower limit (as a percentage of the service's desiredCount) of the number of running tasks that must remain running and healthy in a service during a deployment.
         :param pulumi.Input[int] desired_count: Number of instances of the task definition to place and keep running. Defaults to 0. Do not specify if using the `DAEMON` scheduling strategy.
@@ -457,18 +510,20 @@
         :param pulumi.Input[str] name: Name of the service (up to 255 letters, numbers, hyphens, and underscores)
         :param pulumi.Input[pulumi.InputType['pulumi_aws.ecs.ServiceNetworkConfigurationArgs']] network_configuration: Network configuration for the service. This parameter is required for task definitions that use the `awsvpc` network mode to receive their own Elastic Network Interface, and it is not supported for other network modes. See below.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['pulumi_aws.ecs.ServiceOrderedPlacementStrategyArgs']]]] ordered_placement_strategies: Service level strategy rules that are taken into consideration during task placement. List from top to bottom in order of precedence. Updates to this configuration will take effect next task deployment unless `force_new_deployment` is enabled. The maximum number of `ordered_placement_strategy` blocks is `5`. See below.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['pulumi_aws.ecs.ServicePlacementConstraintArgs']]]] placement_constraints: Rules that are taken into consideration during task placement. Updates to this configuration will take effect next task deployment unless `force_new_deployment` is enabled. Maximum number of `placement_constraints` is `10`. See below.
         :param pulumi.Input[str] platform_version: Platform version on which to run your service. Only applicable for `launch_type` set to `FARGATE`. Defaults to `LATEST`. More information about Fargate platform versions can be found in the [AWS ECS User Guide](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/platform_versions.html).
         :param pulumi.Input[str] propagate_tags: Specifies whether to propagate the tags from the task definition or the service to the tasks. The valid values are `SERVICE` and `TASK_DEFINITION`.
         :param pulumi.Input[str] scheduling_strategy: Scheduling strategy to use for the service. The valid values are `REPLICA` and `DAEMON`. Defaults to `REPLICA`. Note that [*Tasks using the Fargate launch type or the `CODE_DEPLOY` or `EXTERNAL` deployment controller types don't support the `DAEMON` scheduling strategy*](https://docs.aws.amazon.com/AmazonECS/latest/APIReference/API_CreateService.html).
+        :param pulumi.Input[pulumi.InputType['pulumi_aws.ecs.ServiceServiceConnectConfigurationArgs']] service_connect_configuration: The ECS Service Connect configuration for this service to discover and connect to services, and be discovered by, and connected from, other services within a namespace. See below.
         :param pulumi.Input[pulumi.InputType['pulumi_aws.ecs.ServiceServiceRegistriesArgs']] service_registries: Service discovery registries for the service. The maximum number of `service_registries` blocks is `1`. See below.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Key-value map of resource tags. If configured with a provider `default_tags` configuration block present, tags with matching keys will overwrite those defined at the provider-level.
         :param pulumi.Input[str] task_definition: Family and revision (`family:revision`) or full ARN of the task definition that you want to run in your service. Either [taskDefinition] or [taskDefinitionArgs] must be provided.
         :param pulumi.InputType['EC2ServiceTaskDefinitionArgs'] task_definition_args: The args of task definition that you want to run in your service. Either [taskDefinition] or [taskDefinitionArgs] must be provided.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] triggers: Map of arbitrary keys and values that, when changed, will trigger an in-place update (redeployment). Useful with `timestamp()`. See example above.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[EC2ServiceArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -487,14 +542,15 @@
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
+                 alarms: Optional[pulumi.Input[pulumi.InputType['pulumi_aws.ecs.ServiceAlarmsArgs']]] = None,
                  cluster: Optional[pulumi.Input[str]] = None,
                  continue_before_steady_state: Optional[pulumi.Input[bool]] = None,
                  deployment_circuit_breaker: Optional[pulumi.Input[pulumi.InputType['pulumi_aws.ecs.ServiceDeploymentCircuitBreakerArgs']]] = None,
                  deployment_controller: Optional[pulumi.Input[pulumi.InputType['pulumi_aws.ecs.ServiceDeploymentControllerArgs']]] = None,
                  deployment_maximum_percent: Optional[pulumi.Input[int]] = None,
                  deployment_minimum_healthy_percent: Optional[pulumi.Input[int]] = None,
                  desired_count: Optional[pulumi.Input[int]] = None,
@@ -507,32 +563,32 @@
                  name: Optional[pulumi.Input[str]] = None,
                  network_configuration: Optional[pulumi.Input[pulumi.InputType['pulumi_aws.ecs.ServiceNetworkConfigurationArgs']]] = None,
                  ordered_placement_strategies: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['pulumi_aws.ecs.ServiceOrderedPlacementStrategyArgs']]]]] = None,
                  placement_constraints: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['pulumi_aws.ecs.ServicePlacementConstraintArgs']]]]] = None,
                  platform_version: Optional[pulumi.Input[str]] = None,
                  propagate_tags: Optional[pulumi.Input[str]] = None,
                  scheduling_strategy: Optional[pulumi.Input[str]] = None,
+                 service_connect_configuration: Optional[pulumi.Input[pulumi.InputType['pulumi_aws.ecs.ServiceServiceConnectConfigurationArgs']]] = None,
                  service_registries: Optional[pulumi.Input[pulumi.InputType['pulumi_aws.ecs.ServiceServiceRegistriesArgs']]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  task_definition: Optional[pulumi.Input[str]] = None,
                  task_definition_args: Optional[pulumi.InputType['EC2ServiceTaskDefinitionArgs']] = None,
+                 triggers: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = EC2ServiceArgs.__new__(EC2ServiceArgs)
 
+            __props__.__dict__["alarms"] = alarms
             __props__.__dict__["cluster"] = cluster
             __props__.__dict__["continue_before_steady_state"] = continue_before_steady_state
             __props__.__dict__["deployment_circuit_breaker"] = deployment_circuit_breaker
             __props__.__dict__["deployment_controller"] = deployment_controller
             __props__.__dict__["deployment_maximum_percent"] = deployment_maximum_percent
             __props__.__dict__["deployment_minimum_healthy_percent"] = deployment_minimum_healthy_percent
             __props__.__dict__["desired_count"] = desired_count
@@ -545,18 +601,20 @@
             __props__.__dict__["name"] = name
             __props__.__dict__["network_configuration"] = network_configuration
             __props__.__dict__["ordered_placement_strategies"] = ordered_placement_strategies
             __props__.__dict__["placement_constraints"] = placement_constraints
             __props__.__dict__["platform_version"] = platform_version
             __props__.__dict__["propagate_tags"] = propagate_tags
             __props__.__dict__["scheduling_strategy"] = scheduling_strategy
+            __props__.__dict__["service_connect_configuration"] = service_connect_configuration
             __props__.__dict__["service_registries"] = service_registries
             __props__.__dict__["tags"] = tags
             __props__.__dict__["task_definition"] = task_definition
             __props__.__dict__["task_definition_args"] = task_definition_args
+            __props__.__dict__["triggers"] = triggers
             __props__.__dict__["service"] = None
         super(EC2Service, __self__).__init__(
             'awsx:ecs:EC2Service',
             resource_name,
             __props__,
             opts,
             remote=True)
```

### Comparing `pulumi_awsx-1.0.2/pulumi_awsx/ecs/ec2_task_definition.py` & `pulumi_awsx-1.0.3/pulumi_awsx/ecs/ec2_task_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by pulumi-gen-awsx. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from .. import awsx as _awsx
 from ._inputs import *
@@ -446,20 +447,17 @@
                  proxy_configuration: Optional[pulumi.Input[pulumi.InputType['pulumi_aws.ecs.TaskDefinitionProxyConfigurationArgs']]] = None,
                  runtime_platform: Optional[pulumi.Input[pulumi.InputType['pulumi_aws.ecs.TaskDefinitionRuntimePlatformArgs']]] = None,
                  skip_destroy: Optional[pulumi.Input[bool]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  task_role: Optional[pulumi.InputType['_awsx.DefaultRoleWithPolicyArgs']] = None,
                  volumes: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['pulumi_aws.ecs.TaskDefinitionVolumeArgs']]]]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = EC2TaskDefinitionArgs.__new__(EC2TaskDefinitionArgs)
```

### Comparing `pulumi_awsx-1.0.2/pulumi_awsx/ecs/fargate_service.py` & `pulumi_awsx-1.0.3/pulumi_awsx/lb/network_load_balancer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,579 +1,603 @@
 # coding=utf-8
 # *** WARNING: this file was generated by pulumi-gen-awsx. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
-from .. import awsx as _awsx
 from ._inputs import *
 import pulumi_aws
 
-__all__ = ['FargateServiceArgs', 'FargateService']
+__all__ = ['NetworkLoadBalancerArgs', 'NetworkLoadBalancer']
 
 @pulumi.input_type
-class FargateServiceArgs:
+class NetworkLoadBalancerArgs:
     def __init__(__self__, *,
-                 assign_public_ip: Optional[pulumi.Input[bool]] = None,
-                 cluster: Optional[pulumi.Input[str]] = None,
-                 continue_before_steady_state: Optional[pulumi.Input[bool]] = None,
-                 deployment_circuit_breaker: Optional[pulumi.Input['pulumi_aws.ecs.ServiceDeploymentCircuitBreakerArgs']] = None,
-                 deployment_controller: Optional[pulumi.Input['pulumi_aws.ecs.ServiceDeploymentControllerArgs']] = None,
-                 deployment_maximum_percent: Optional[pulumi.Input[int]] = None,
-                 deployment_minimum_healthy_percent: Optional[pulumi.Input[int]] = None,
-                 desired_count: Optional[pulumi.Input[int]] = None,
-                 enable_ecs_managed_tags: Optional[pulumi.Input[bool]] = None,
-                 enable_execute_command: Optional[pulumi.Input[bool]] = None,
-                 force_new_deployment: Optional[pulumi.Input[bool]] = None,
-                 health_check_grace_period_seconds: Optional[pulumi.Input[int]] = None,
-                 iam_role: Optional[pulumi.Input[str]] = None,
-                 load_balancers: Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ecs.ServiceLoadBalancerArgs']]]] = None,
+                 access_logs: Optional[pulumi.Input['pulumi_aws.lb.LoadBalancerAccessLogsArgs']] = None,
+                 customer_owned_ipv4_pool: Optional[pulumi.Input[str]] = None,
+                 default_target_group: Optional['TargetGroupArgs'] = None,
+                 default_target_group_port: Optional[pulumi.Input[int]] = None,
+                 desync_mitigation_mode: Optional[pulumi.Input[str]] = None,
+                 drop_invalid_header_fields: Optional[pulumi.Input[bool]] = None,
+                 enable_cross_zone_load_balancing: Optional[pulumi.Input[bool]] = None,
+                 enable_deletion_protection: Optional[pulumi.Input[bool]] = None,
+                 enable_tls_version_and_cipher_suite_headers: Optional[pulumi.Input[bool]] = None,
+                 enable_waf_fail_open: Optional[pulumi.Input[bool]] = None,
+                 enable_xff_client_port: Optional[pulumi.Input[bool]] = None,
+                 idle_timeout: Optional[pulumi.Input[int]] = None,
+                 internal: Optional[pulumi.Input[bool]] = None,
+                 ip_address_type: Optional[pulumi.Input[str]] = None,
+                 listener: Optional['ListenerArgs'] = None,
+                 listeners: Optional[Sequence['ListenerArgs']] = None,
                  name: Optional[pulumi.Input[str]] = None,
-                 network_configuration: Optional[pulumi.Input['pulumi_aws.ecs.ServiceNetworkConfigurationArgs']] = None,
-                 placement_constraints: Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ecs.ServicePlacementConstraintArgs']]]] = None,
-                 platform_version: Optional[pulumi.Input[str]] = None,
-                 propagate_tags: Optional[pulumi.Input[str]] = None,
-                 scheduling_strategy: Optional[pulumi.Input[str]] = None,
-                 service_registries: Optional[pulumi.Input['pulumi_aws.ecs.ServiceServiceRegistriesArgs']] = None,
+                 name_prefix: Optional[pulumi.Input[str]] = None,
+                 preserve_host_header: Optional[pulumi.Input[bool]] = None,
+                 subnet_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 subnet_mappings: Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.lb.LoadBalancerSubnetMappingArgs']]]] = None,
+                 subnets: Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ec2.Subnet']]]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
-                 task_definition: Optional[pulumi.Input[str]] = None,
-                 task_definition_args: Optional['FargateServiceTaskDefinitionArgs'] = None):
+                 xff_header_processing_mode: Optional[pulumi.Input[str]] = None):
         """
-        The set of arguments for constructing a FargateService resource.
-        :param pulumi.Input[bool] assign_public_ip: Assign a public IP address to the ENI (Fargate launch type only). Valid values are `true` or `false`. Default `false`.
-        :param pulumi.Input[str] cluster: ARN of an ECS cluster.
-        :param pulumi.Input[bool] continue_before_steady_state: If `true`, this provider will not wait for the service to reach a steady state (like [`aws ecs wait services-stable`](https://docs.aws.amazon.com/cli/latest/reference/ecs/wait/services-stable.html)) before continuing. Default `false`.
-        :param pulumi.Input['pulumi_aws.ecs.ServiceDeploymentCircuitBreakerArgs'] deployment_circuit_breaker: Configuration block for deployment circuit breaker. See below.
-        :param pulumi.Input['pulumi_aws.ecs.ServiceDeploymentControllerArgs'] deployment_controller: Configuration block for deployment controller configuration. See below.
-        :param pulumi.Input[int] deployment_maximum_percent: Upper limit (as a percentage of the service's desiredCount) of the number of running tasks that can be running in a service during a deployment. Not valid when using the `DAEMON` scheduling strategy.
-        :param pulumi.Input[int] deployment_minimum_healthy_percent: Lower limit (as a percentage of the service's desiredCount) of the number of running tasks that must remain running and healthy in a service during a deployment.
-        :param pulumi.Input[int] desired_count: Number of instances of the task definition to place and keep running. Defaults to 0. Do not specify if using the `DAEMON` scheduling strategy.
-        :param pulumi.Input[bool] enable_ecs_managed_tags: Specifies whether to enable Amazon ECS managed tags for the tasks within the service.
-        :param pulumi.Input[bool] enable_execute_command: Specifies whether to enable Amazon ECS Exec for the tasks within the service.
-        :param pulumi.Input[bool] force_new_deployment: Enable to force a new task deployment of the service. This can be used to update tasks to use a newer Docker image with same image/tag combination (e.g., `myimage:latest`), roll Fargate tasks onto a newer platform version, or immediately deploy `ordered_placement_strategy` and `placement_constraints` updates.
-        :param pulumi.Input[int] health_check_grace_period_seconds: Seconds to ignore failing load balancer health checks on newly instantiated tasks to prevent premature shutdown, up to 2147483647. Only valid for services configured to use load balancers.
-        :param pulumi.Input[str] iam_role: ARN of the IAM role that allows Amazon ECS to make calls to your load balancer on your behalf. This parameter is required if you are using a load balancer with your service, but only if your task definition does not use the `awsvpc` network mode. If using `awsvpc` network mode, do not specify this role. If your account has already created the Amazon ECS service-linked role, that role is used by default for your service unless you specify a role here.
-        :param pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ecs.ServiceLoadBalancerArgs']]] load_balancers: Configuration block for load balancers. See below.
-        :param pulumi.Input[str] name: Name of the service (up to 255 letters, numbers, hyphens, and underscores)
-        :param pulumi.Input['pulumi_aws.ecs.ServiceNetworkConfigurationArgs'] network_configuration: Network configuration for the service. This parameter is required for task definitions that use the `awsvpc` network mode to receive their own Elastic Network Interface, and it is not supported for other network modes. See below.
-        :param pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ecs.ServicePlacementConstraintArgs']]] placement_constraints: Rules that are taken into consideration during task placement. Updates to this configuration will take effect next task deployment unless `force_new_deployment` is enabled. Maximum number of `placement_constraints` is `10`. See below.
-        :param pulumi.Input[str] platform_version: Platform version on which to run your service. Only applicable for `launch_type` set to `FARGATE`. Defaults to `LATEST`. More information about Fargate platform versions can be found in the [AWS ECS User Guide](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/platform_versions.html).
-        :param pulumi.Input[str] propagate_tags: Specifies whether to propagate the tags from the task definition or the service to the tasks. The valid values are `SERVICE` and `TASK_DEFINITION`.
-        :param pulumi.Input[str] scheduling_strategy: Scheduling strategy to use for the service. The valid values are `REPLICA` and `DAEMON`. Defaults to `REPLICA`. Note that [*Tasks using the Fargate launch type or the `CODE_DEPLOY` or `EXTERNAL` deployment controller types don't support the `DAEMON` scheduling strategy*](https://docs.aws.amazon.com/AmazonECS/latest/APIReference/API_CreateService.html).
-        :param pulumi.Input['pulumi_aws.ecs.ServiceServiceRegistriesArgs'] service_registries: Service discovery registries for the service. The maximum number of `service_registries` blocks is `1`. See below.
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Key-value map of resource tags. If configured with a provider `default_tags` configuration block present, tags with matching keys will overwrite those defined at the provider-level.
-        :param pulumi.Input[str] task_definition: Family and revision (`family:revision`) or full ARN of the task definition that you want to run in your service. Either [taskDefinition] or [taskDefinitionArgs] must be provided.
-        :param 'FargateServiceTaskDefinitionArgs' task_definition_args: The args of task definition that you want to run in your service. Either [taskDefinition] or [taskDefinitionArgs] must be provided.
-        """
-        if assign_public_ip is not None:
-            pulumi.set(__self__, "assign_public_ip", assign_public_ip)
-        if cluster is not None:
-            pulumi.set(__self__, "cluster", cluster)
-        if continue_before_steady_state is not None:
-            pulumi.set(__self__, "continue_before_steady_state", continue_before_steady_state)
-        if deployment_circuit_breaker is not None:
-            pulumi.set(__self__, "deployment_circuit_breaker", deployment_circuit_breaker)
-        if deployment_controller is not None:
-            pulumi.set(__self__, "deployment_controller", deployment_controller)
-        if deployment_maximum_percent is not None:
-            pulumi.set(__self__, "deployment_maximum_percent", deployment_maximum_percent)
-        if deployment_minimum_healthy_percent is not None:
-            pulumi.set(__self__, "deployment_minimum_healthy_percent", deployment_minimum_healthy_percent)
-        if desired_count is not None:
-            pulumi.set(__self__, "desired_count", desired_count)
-        if enable_ecs_managed_tags is not None:
-            pulumi.set(__self__, "enable_ecs_managed_tags", enable_ecs_managed_tags)
-        if enable_execute_command is not None:
-            pulumi.set(__self__, "enable_execute_command", enable_execute_command)
-        if force_new_deployment is not None:
-            pulumi.set(__self__, "force_new_deployment", force_new_deployment)
-        if health_check_grace_period_seconds is not None:
-            pulumi.set(__self__, "health_check_grace_period_seconds", health_check_grace_period_seconds)
-        if iam_role is not None:
-            pulumi.set(__self__, "iam_role", iam_role)
-        if load_balancers is not None:
-            pulumi.set(__self__, "load_balancers", load_balancers)
+        The set of arguments for constructing a NetworkLoadBalancer resource.
+        :param pulumi.Input['pulumi_aws.lb.LoadBalancerAccessLogsArgs'] access_logs: An Access Logs block. Access Logs documented below.
+        :param pulumi.Input[str] customer_owned_ipv4_pool: The ID of the customer owned ipv4 pool to use for this load balancer.
+        :param 'TargetGroupArgs' default_target_group: Options creating a default target group.
+        :param pulumi.Input[int] default_target_group_port: Port to use to connect with the target. Valid values are ports 1-65535. Defaults to 80.
+        :param pulumi.Input[str] desync_mitigation_mode: Determines how the load balancer handles requests that might pose a security risk to an application due to HTTP desync. Valid values are `monitor`, `defensive` (default), `strictest`.
+        :param pulumi.Input[bool] drop_invalid_header_fields: Indicates whether HTTP headers with header fields that are not valid are removed by the load balancer (true) or routed to targets (false). The default is false. Elastic Load Balancing requires that message header names contain only alphanumeric characters and hyphens. Only valid for Load Balancers of type `application`.
+        :param pulumi.Input[bool] enable_cross_zone_load_balancing: If true, cross-zone load balancing of the load balancer will be enabled. For `network` and `gateway` type load balancers, this feature is disabled by default (`false`). For `application` load balancer this feature is always enabled (`true`) and cannot be disabled. Defaults to `false`.
+        :param pulumi.Input[bool] enable_deletion_protection: If true, deletion of the load balancer will be disabled via the AWS API. This will prevent this provider from deleting the load balancer. Defaults to `false`.
+        :param pulumi.Input[bool] enable_tls_version_and_cipher_suite_headers: Indicates whether the two headers (`x-amzn-tls-version` and `x-amzn-tls-cipher-suite`), which contain information about the negotiated TLS version and cipher suite, are added to the client request before sending it to the target. Only valid for Load Balancers of type `application`. Defaults to `false`
+        :param pulumi.Input[bool] enable_waf_fail_open: Indicates whether to allow a WAF-enabled load balancer to route requests to targets if it is unable to forward the request to AWS WAF. Defaults to `false`.
+        :param pulumi.Input[bool] enable_xff_client_port: Indicates whether the X-Forwarded-For header should preserve the source port that the client used to connect to the load balancer in `application` load balancers. Defaults to `true`.
+        :param pulumi.Input[int] idle_timeout: The time in seconds that the connection is allowed to be idle. Only valid for Load Balancers of type `application`. Default: 60.
+        :param pulumi.Input[bool] internal: If true, the LB will be internal.
+        :param pulumi.Input[str] ip_address_type: The type of IP addresses used by the subnets for your load balancer. The possible values are `ipv4` and `dualstack`.
+        :param 'ListenerArgs' listener: A listener to create. Only one of [listener] and [listeners] can be specified.
+        :param Sequence['ListenerArgs'] listeners: List of listeners to create. Only one of [listener] and [listeners] can be specified.
+        :param pulumi.Input[str] name: The name of the LB. This name must be unique within your AWS account, can have a maximum of 32 characters,
+               must contain only alphanumeric characters or hyphens, and must not begin or end with a hyphen. If not specified,
+               this provider will autogenerate a name beginning with `tf-lb`.
+        :param pulumi.Input[str] name_prefix: Creates a unique name beginning with the specified prefix. Conflicts with `name`.
+        :param pulumi.Input[bool] preserve_host_header: Indicates whether the Application Load Balancer should preserve the Host header in the HTTP request and send it to the target without any change. Defaults to `false`.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] subnet_ids: A list of subnet IDs to attach to the LB. Subnets
+               cannot be updated for Load Balancers of type `network`. Changing this value
+               for load balancers of type `network` will force a recreation of the resource.
+        :param pulumi.Input[Sequence[pulumi.Input['pulumi_aws.lb.LoadBalancerSubnetMappingArgs']]] subnet_mappings: A subnet mapping block as documented below.
+        :param pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ec2.Subnet']]] subnets: A list of subnets to attach to the LB. Only one of [subnets], [subnetIds] or [subnetMappings] can be specified
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: A map of tags to assign to the resource. If configured with a provider `default_tags` configuration block present, tags with matching keys will overwrite those defined at the provider-level.
+        :param pulumi.Input[str] xff_header_processing_mode: Determines how the load balancer modifies the `X-Forwarded-For` header in the HTTP request before sending the request to the target. The possible values are `append`, `preserve`, and `remove`. Only valid for Load Balancers of type `application`. The default is `append`.
+        """
+        if access_logs is not None:
+            pulumi.set(__self__, "access_logs", access_logs)
+        if customer_owned_ipv4_pool is not None:
+            pulumi.set(__self__, "customer_owned_ipv4_pool", customer_owned_ipv4_pool)
+        if default_target_group is not None:
+            pulumi.set(__self__, "default_target_group", default_target_group)
+        if default_target_group_port is not None:
+            pulumi.set(__self__, "default_target_group_port", default_target_group_port)
+        if desync_mitigation_mode is not None:
+            pulumi.set(__self__, "desync_mitigation_mode", desync_mitigation_mode)
+        if drop_invalid_header_fields is not None:
+            pulumi.set(__self__, "drop_invalid_header_fields", drop_invalid_header_fields)
+        if enable_cross_zone_load_balancing is not None:
+            pulumi.set(__self__, "enable_cross_zone_load_balancing", enable_cross_zone_load_balancing)
+        if enable_deletion_protection is not None:
+            pulumi.set(__self__, "enable_deletion_protection", enable_deletion_protection)
+        if enable_tls_version_and_cipher_suite_headers is not None:
+            pulumi.set(__self__, "enable_tls_version_and_cipher_suite_headers", enable_tls_version_and_cipher_suite_headers)
+        if enable_waf_fail_open is not None:
+            pulumi.set(__self__, "enable_waf_fail_open", enable_waf_fail_open)
+        if enable_xff_client_port is not None:
+            pulumi.set(__self__, "enable_xff_client_port", enable_xff_client_port)
+        if idle_timeout is not None:
+            pulumi.set(__self__, "idle_timeout", idle_timeout)
+        if internal is not None:
+            pulumi.set(__self__, "internal", internal)
+        if ip_address_type is not None:
+            pulumi.set(__self__, "ip_address_type", ip_address_type)
+        if listener is not None:
+            pulumi.set(__self__, "listener", listener)
+        if listeners is not None:
+            pulumi.set(__self__, "listeners", listeners)
         if name is not None:
             pulumi.set(__self__, "name", name)
-        if network_configuration is not None:
-            pulumi.set(__self__, "network_configuration", network_configuration)
-        if placement_constraints is not None:
-            pulumi.set(__self__, "placement_constraints", placement_constraints)
-        if platform_version is not None:
-            pulumi.set(__self__, "platform_version", platform_version)
-        if propagate_tags is not None:
-            pulumi.set(__self__, "propagate_tags", propagate_tags)
-        if scheduling_strategy is not None:
-            pulumi.set(__self__, "scheduling_strategy", scheduling_strategy)
-        if service_registries is not None:
-            pulumi.set(__self__, "service_registries", service_registries)
+        if name_prefix is not None:
+            pulumi.set(__self__, "name_prefix", name_prefix)
+        if preserve_host_header is not None:
+            pulumi.set(__self__, "preserve_host_header", preserve_host_header)
+        if subnet_ids is not None:
+            pulumi.set(__self__, "subnet_ids", subnet_ids)
+        if subnet_mappings is not None:
+            pulumi.set(__self__, "subnet_mappings", subnet_mappings)
+        if subnets is not None:
+            pulumi.set(__self__, "subnets", subnets)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
-        if task_definition is not None:
-            pulumi.set(__self__, "task_definition", task_definition)
-        if task_definition_args is not None:
-            pulumi.set(__self__, "task_definition_args", task_definition_args)
+        if xff_header_processing_mode is not None:
+            pulumi.set(__self__, "xff_header_processing_mode", xff_header_processing_mode)
 
     @property
-    @pulumi.getter(name="assignPublicIp")
-    def assign_public_ip(self) -> Optional[pulumi.Input[bool]]:
+    @pulumi.getter(name="accessLogs")
+    def access_logs(self) -> Optional[pulumi.Input['pulumi_aws.lb.LoadBalancerAccessLogsArgs']]:
         """
-        Assign a public IP address to the ENI (Fargate launch type only). Valid values are `true` or `false`. Default `false`.
+        An Access Logs block. Access Logs documented below.
         """
-        return pulumi.get(self, "assign_public_ip")
+        return pulumi.get(self, "access_logs")
 
-    @assign_public_ip.setter
-    def assign_public_ip(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "assign_public_ip", value)
+    @access_logs.setter
+    def access_logs(self, value: Optional[pulumi.Input['pulumi_aws.lb.LoadBalancerAccessLogsArgs']]):
+        pulumi.set(self, "access_logs", value)
 
     @property
-    @pulumi.getter
-    def cluster(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="customerOwnedIpv4Pool")
+    def customer_owned_ipv4_pool(self) -> Optional[pulumi.Input[str]]:
         """
-        ARN of an ECS cluster.
+        The ID of the customer owned ipv4 pool to use for this load balancer.
         """
-        return pulumi.get(self, "cluster")
+        return pulumi.get(self, "customer_owned_ipv4_pool")
 
-    @cluster.setter
-    def cluster(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "cluster", value)
+    @customer_owned_ipv4_pool.setter
+    def customer_owned_ipv4_pool(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "customer_owned_ipv4_pool", value)
 
     @property
-    @pulumi.getter(name="continueBeforeSteadyState")
-    def continue_before_steady_state(self) -> Optional[pulumi.Input[bool]]:
+    @pulumi.getter(name="defaultTargetGroup")
+    def default_target_group(self) -> Optional['TargetGroupArgs']:
         """
-        If `true`, this provider will not wait for the service to reach a steady state (like [`aws ecs wait services-stable`](https://docs.aws.amazon.com/cli/latest/reference/ecs/wait/services-stable.html)) before continuing. Default `false`.
+        Options creating a default target group.
         """
-        return pulumi.get(self, "continue_before_steady_state")
+        return pulumi.get(self, "default_target_group")
 
-    @continue_before_steady_state.setter
-    def continue_before_steady_state(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "continue_before_steady_state", value)
+    @default_target_group.setter
+    def default_target_group(self, value: Optional['TargetGroupArgs']):
+        pulumi.set(self, "default_target_group", value)
 
     @property
-    @pulumi.getter(name="deploymentCircuitBreaker")
-    def deployment_circuit_breaker(self) -> Optional[pulumi.Input['pulumi_aws.ecs.ServiceDeploymentCircuitBreakerArgs']]:
+    @pulumi.getter(name="defaultTargetGroupPort")
+    def default_target_group_port(self) -> Optional[pulumi.Input[int]]:
         """
-        Configuration block for deployment circuit breaker. See below.
+        Port to use to connect with the target. Valid values are ports 1-65535. Defaults to 80.
         """
-        return pulumi.get(self, "deployment_circuit_breaker")
+        return pulumi.get(self, "default_target_group_port")
 
-    @deployment_circuit_breaker.setter
-    def deployment_circuit_breaker(self, value: Optional[pulumi.Input['pulumi_aws.ecs.ServiceDeploymentCircuitBreakerArgs']]):
-        pulumi.set(self, "deployment_circuit_breaker", value)
+    @default_target_group_port.setter
+    def default_target_group_port(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "default_target_group_port", value)
 
     @property
-    @pulumi.getter(name="deploymentController")
-    def deployment_controller(self) -> Optional[pulumi.Input['pulumi_aws.ecs.ServiceDeploymentControllerArgs']]:
+    @pulumi.getter(name="desyncMitigationMode")
+    def desync_mitigation_mode(self) -> Optional[pulumi.Input[str]]:
         """
-        Configuration block for deployment controller configuration. See below.
+        Determines how the load balancer handles requests that might pose a security risk to an application due to HTTP desync. Valid values are `monitor`, `defensive` (default), `strictest`.
         """
-        return pulumi.get(self, "deployment_controller")
+        return pulumi.get(self, "desync_mitigation_mode")
 
-    @deployment_controller.setter
-    def deployment_controller(self, value: Optional[pulumi.Input['pulumi_aws.ecs.ServiceDeploymentControllerArgs']]):
-        pulumi.set(self, "deployment_controller", value)
+    @desync_mitigation_mode.setter
+    def desync_mitigation_mode(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "desync_mitigation_mode", value)
 
     @property
-    @pulumi.getter(name="deploymentMaximumPercent")
-    def deployment_maximum_percent(self) -> Optional[pulumi.Input[int]]:
+    @pulumi.getter(name="dropInvalidHeaderFields")
+    def drop_invalid_header_fields(self) -> Optional[pulumi.Input[bool]]:
         """
-        Upper limit (as a percentage of the service's desiredCount) of the number of running tasks that can be running in a service during a deployment. Not valid when using the `DAEMON` scheduling strategy.
+        Indicates whether HTTP headers with header fields that are not valid are removed by the load balancer (true) or routed to targets (false). The default is false. Elastic Load Balancing requires that message header names contain only alphanumeric characters and hyphens. Only valid for Load Balancers of type `application`.
         """
-        return pulumi.get(self, "deployment_maximum_percent")
+        return pulumi.get(self, "drop_invalid_header_fields")
 
-    @deployment_maximum_percent.setter
-    def deployment_maximum_percent(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "deployment_maximum_percent", value)
+    @drop_invalid_header_fields.setter
+    def drop_invalid_header_fields(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "drop_invalid_header_fields", value)
 
     @property
-    @pulumi.getter(name="deploymentMinimumHealthyPercent")
-    def deployment_minimum_healthy_percent(self) -> Optional[pulumi.Input[int]]:
+    @pulumi.getter(name="enableCrossZoneLoadBalancing")
+    def enable_cross_zone_load_balancing(self) -> Optional[pulumi.Input[bool]]:
         """
-        Lower limit (as a percentage of the service's desiredCount) of the number of running tasks that must remain running and healthy in a service during a deployment.
+        If true, cross-zone load balancing of the load balancer will be enabled. For `network` and `gateway` type load balancers, this feature is disabled by default (`false`). For `application` load balancer this feature is always enabled (`true`) and cannot be disabled. Defaults to `false`.
         """
-        return pulumi.get(self, "deployment_minimum_healthy_percent")
+        return pulumi.get(self, "enable_cross_zone_load_balancing")
 
-    @deployment_minimum_healthy_percent.setter
-    def deployment_minimum_healthy_percent(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "deployment_minimum_healthy_percent", value)
+    @enable_cross_zone_load_balancing.setter
+    def enable_cross_zone_load_balancing(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "enable_cross_zone_load_balancing", value)
 
     @property
-    @pulumi.getter(name="desiredCount")
-    def desired_count(self) -> Optional[pulumi.Input[int]]:
+    @pulumi.getter(name="enableDeletionProtection")
+    def enable_deletion_protection(self) -> Optional[pulumi.Input[bool]]:
         """
-        Number of instances of the task definition to place and keep running. Defaults to 0. Do not specify if using the `DAEMON` scheduling strategy.
+        If true, deletion of the load balancer will be disabled via the AWS API. This will prevent this provider from deleting the load balancer. Defaults to `false`.
         """
-        return pulumi.get(self, "desired_count")
+        return pulumi.get(self, "enable_deletion_protection")
 
-    @desired_count.setter
-    def desired_count(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "desired_count", value)
+    @enable_deletion_protection.setter
+    def enable_deletion_protection(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "enable_deletion_protection", value)
 
     @property
-    @pulumi.getter(name="enableEcsManagedTags")
-    def enable_ecs_managed_tags(self) -> Optional[pulumi.Input[bool]]:
+    @pulumi.getter(name="enableTlsVersionAndCipherSuiteHeaders")
+    def enable_tls_version_and_cipher_suite_headers(self) -> Optional[pulumi.Input[bool]]:
         """
-        Specifies whether to enable Amazon ECS managed tags for the tasks within the service.
+        Indicates whether the two headers (`x-amzn-tls-version` and `x-amzn-tls-cipher-suite`), which contain information about the negotiated TLS version and cipher suite, are added to the client request before sending it to the target. Only valid for Load Balancers of type `application`. Defaults to `false`
         """
-        return pulumi.get(self, "enable_ecs_managed_tags")
+        return pulumi.get(self, "enable_tls_version_and_cipher_suite_headers")
 
-    @enable_ecs_managed_tags.setter
-    def enable_ecs_managed_tags(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "enable_ecs_managed_tags", value)
+    @enable_tls_version_and_cipher_suite_headers.setter
+    def enable_tls_version_and_cipher_suite_headers(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "enable_tls_version_and_cipher_suite_headers", value)
 
     @property
-    @pulumi.getter(name="enableExecuteCommand")
-    def enable_execute_command(self) -> Optional[pulumi.Input[bool]]:
+    @pulumi.getter(name="enableWafFailOpen")
+    def enable_waf_fail_open(self) -> Optional[pulumi.Input[bool]]:
         """
-        Specifies whether to enable Amazon ECS Exec for the tasks within the service.
+        Indicates whether to allow a WAF-enabled load balancer to route requests to targets if it is unable to forward the request to AWS WAF. Defaults to `false`.
         """
-        return pulumi.get(self, "enable_execute_command")
+        return pulumi.get(self, "enable_waf_fail_open")
 
-    @enable_execute_command.setter
-    def enable_execute_command(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "enable_execute_command", value)
+    @enable_waf_fail_open.setter
+    def enable_waf_fail_open(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "enable_waf_fail_open", value)
 
     @property
-    @pulumi.getter(name="forceNewDeployment")
-    def force_new_deployment(self) -> Optional[pulumi.Input[bool]]:
+    @pulumi.getter(name="enableXffClientPort")
+    def enable_xff_client_port(self) -> Optional[pulumi.Input[bool]]:
         """
-        Enable to force a new task deployment of the service. This can be used to update tasks to use a newer Docker image with same image/tag combination (e.g., `myimage:latest`), roll Fargate tasks onto a newer platform version, or immediately deploy `ordered_placement_strategy` and `placement_constraints` updates.
+        Indicates whether the X-Forwarded-For header should preserve the source port that the client used to connect to the load balancer in `application` load balancers. Defaults to `true`.
         """
-        return pulumi.get(self, "force_new_deployment")
+        return pulumi.get(self, "enable_xff_client_port")
 
-    @force_new_deployment.setter
-    def force_new_deployment(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "force_new_deployment", value)
+    @enable_xff_client_port.setter
+    def enable_xff_client_port(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "enable_xff_client_port", value)
 
     @property
-    @pulumi.getter(name="healthCheckGracePeriodSeconds")
-    def health_check_grace_period_seconds(self) -> Optional[pulumi.Input[int]]:
+    @pulumi.getter(name="idleTimeout")
+    def idle_timeout(self) -> Optional[pulumi.Input[int]]:
         """
-        Seconds to ignore failing load balancer health checks on newly instantiated tasks to prevent premature shutdown, up to 2147483647. Only valid for services configured to use load balancers.
+        The time in seconds that the connection is allowed to be idle. Only valid for Load Balancers of type `application`. Default: 60.
         """
-        return pulumi.get(self, "health_check_grace_period_seconds")
+        return pulumi.get(self, "idle_timeout")
 
-    @health_check_grace_period_seconds.setter
-    def health_check_grace_period_seconds(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "health_check_grace_period_seconds", value)
+    @idle_timeout.setter
+    def idle_timeout(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "idle_timeout", value)
 
     @property
-    @pulumi.getter(name="iamRole")
-    def iam_role(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def internal(self) -> Optional[pulumi.Input[bool]]:
         """
-        ARN of the IAM role that allows Amazon ECS to make calls to your load balancer on your behalf. This parameter is required if you are using a load balancer with your service, but only if your task definition does not use the `awsvpc` network mode. If using `awsvpc` network mode, do not specify this role. If your account has already created the Amazon ECS service-linked role, that role is used by default for your service unless you specify a role here.
+        If true, the LB will be internal.
         """
-        return pulumi.get(self, "iam_role")
+        return pulumi.get(self, "internal")
 
-    @iam_role.setter
-    def iam_role(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "iam_role", value)
+    @internal.setter
+    def internal(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "internal", value)
 
     @property
-    @pulumi.getter(name="loadBalancers")
-    def load_balancers(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ecs.ServiceLoadBalancerArgs']]]]:
+    @pulumi.getter(name="ipAddressType")
+    def ip_address_type(self) -> Optional[pulumi.Input[str]]:
         """
-        Configuration block for load balancers. See below.
+        The type of IP addresses used by the subnets for your load balancer. The possible values are `ipv4` and `dualstack`.
         """
-        return pulumi.get(self, "load_balancers")
+        return pulumi.get(self, "ip_address_type")
 
-    @load_balancers.setter
-    def load_balancers(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ecs.ServiceLoadBalancerArgs']]]]):
-        pulumi.set(self, "load_balancers", value)
+    @ip_address_type.setter
+    def ip_address_type(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "ip_address_type", value)
 
     @property
     @pulumi.getter
-    def name(self) -> Optional[pulumi.Input[str]]:
+    def listener(self) -> Optional['ListenerArgs']:
         """
-        Name of the service (up to 255 letters, numbers, hyphens, and underscores)
+        A listener to create. Only one of [listener] and [listeners] can be specified.
         """
-        return pulumi.get(self, "name")
+        return pulumi.get(self, "listener")
 
-    @name.setter
-    def name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "name", value)
+    @listener.setter
+    def listener(self, value: Optional['ListenerArgs']):
+        pulumi.set(self, "listener", value)
 
     @property
-    @pulumi.getter(name="networkConfiguration")
-    def network_configuration(self) -> Optional[pulumi.Input['pulumi_aws.ecs.ServiceNetworkConfigurationArgs']]:
+    @pulumi.getter
+    def listeners(self) -> Optional[Sequence['ListenerArgs']]:
         """
-        Network configuration for the service. This parameter is required for task definitions that use the `awsvpc` network mode to receive their own Elastic Network Interface, and it is not supported for other network modes. See below.
+        List of listeners to create. Only one of [listener] and [listeners] can be specified.
         """
-        return pulumi.get(self, "network_configuration")
+        return pulumi.get(self, "listeners")
 
-    @network_configuration.setter
-    def network_configuration(self, value: Optional[pulumi.Input['pulumi_aws.ecs.ServiceNetworkConfigurationArgs']]):
-        pulumi.set(self, "network_configuration", value)
+    @listeners.setter
+    def listeners(self, value: Optional[Sequence['ListenerArgs']]):
+        pulumi.set(self, "listeners", value)
 
     @property
-    @pulumi.getter(name="placementConstraints")
-    def placement_constraints(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ecs.ServicePlacementConstraintArgs']]]]:
+    @pulumi.getter
+    def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Rules that are taken into consideration during task placement. Updates to this configuration will take effect next task deployment unless `force_new_deployment` is enabled. Maximum number of `placement_constraints` is `10`. See below.
+        The name of the LB. This name must be unique within your AWS account, can have a maximum of 32 characters,
+        must contain only alphanumeric characters or hyphens, and must not begin or end with a hyphen. If not specified,
+        this provider will autogenerate a name beginning with `tf-lb`.
         """
-        return pulumi.get(self, "placement_constraints")
+        return pulumi.get(self, "name")
 
-    @placement_constraints.setter
-    def placement_constraints(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ecs.ServicePlacementConstraintArgs']]]]):
-        pulumi.set(self, "placement_constraints", value)
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
 
     @property
-    @pulumi.getter(name="platformVersion")
-    def platform_version(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="namePrefix")
+    def name_prefix(self) -> Optional[pulumi.Input[str]]:
         """
-        Platform version on which to run your service. Only applicable for `launch_type` set to `FARGATE`. Defaults to `LATEST`. More information about Fargate platform versions can be found in the [AWS ECS User Guide](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/platform_versions.html).
+        Creates a unique name beginning with the specified prefix. Conflicts with `name`.
         """
-        return pulumi.get(self, "platform_version")
+        return pulumi.get(self, "name_prefix")
 
-    @platform_version.setter
-    def platform_version(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "platform_version", value)
+    @name_prefix.setter
+    def name_prefix(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name_prefix", value)
 
     @property
-    @pulumi.getter(name="propagateTags")
-    def propagate_tags(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="preserveHostHeader")
+    def preserve_host_header(self) -> Optional[pulumi.Input[bool]]:
         """
-        Specifies whether to propagate the tags from the task definition or the service to the tasks. The valid values are `SERVICE` and `TASK_DEFINITION`.
+        Indicates whether the Application Load Balancer should preserve the Host header in the HTTP request and send it to the target without any change. Defaults to `false`.
         """
-        return pulumi.get(self, "propagate_tags")
+        return pulumi.get(self, "preserve_host_header")
 
-    @propagate_tags.setter
-    def propagate_tags(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "propagate_tags", value)
+    @preserve_host_header.setter
+    def preserve_host_header(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "preserve_host_header", value)
 
     @property
-    @pulumi.getter(name="schedulingStrategy")
-    def scheduling_strategy(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="subnetIds")
+    def subnet_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Scheduling strategy to use for the service. The valid values are `REPLICA` and `DAEMON`. Defaults to `REPLICA`. Note that [*Tasks using the Fargate launch type or the `CODE_DEPLOY` or `EXTERNAL` deployment controller types don't support the `DAEMON` scheduling strategy*](https://docs.aws.amazon.com/AmazonECS/latest/APIReference/API_CreateService.html).
+        A list of subnet IDs to attach to the LB. Subnets
+        cannot be updated for Load Balancers of type `network`. Changing this value
+        for load balancers of type `network` will force a recreation of the resource.
         """
-        return pulumi.get(self, "scheduling_strategy")
+        return pulumi.get(self, "subnet_ids")
 
-    @scheduling_strategy.setter
-    def scheduling_strategy(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "scheduling_strategy", value)
+    @subnet_ids.setter
+    def subnet_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "subnet_ids", value)
 
     @property
-    @pulumi.getter(name="serviceRegistries")
-    def service_registries(self) -> Optional[pulumi.Input['pulumi_aws.ecs.ServiceServiceRegistriesArgs']]:
+    @pulumi.getter(name="subnetMappings")
+    def subnet_mappings(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.lb.LoadBalancerSubnetMappingArgs']]]]:
         """
-        Service discovery registries for the service. The maximum number of `service_registries` blocks is `1`. See below.
+        A subnet mapping block as documented below.
         """
-        return pulumi.get(self, "service_registries")
+        return pulumi.get(self, "subnet_mappings")
 
-    @service_registries.setter
-    def service_registries(self, value: Optional[pulumi.Input['pulumi_aws.ecs.ServiceServiceRegistriesArgs']]):
-        pulumi.set(self, "service_registries", value)
+    @subnet_mappings.setter
+    def subnet_mappings(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.lb.LoadBalancerSubnetMappingArgs']]]]):
+        pulumi.set(self, "subnet_mappings", value)
 
     @property
     @pulumi.getter
-    def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+    def subnets(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ec2.Subnet']]]]:
         """
-        Key-value map of resource tags. If configured with a provider `default_tags` configuration block present, tags with matching keys will overwrite those defined at the provider-level.
+        A list of subnets to attach to the LB. Only one of [subnets], [subnetIds] or [subnetMappings] can be specified
         """
-        return pulumi.get(self, "tags")
+        return pulumi.get(self, "subnets")
 
-    @tags.setter
-    def tags(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
-        pulumi.set(self, "tags", value)
+    @subnets.setter
+    def subnets(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ec2.Subnet']]]]):
+        pulumi.set(self, "subnets", value)
 
     @property
-    @pulumi.getter(name="taskDefinition")
-    def task_definition(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
-        Family and revision (`family:revision`) or full ARN of the task definition that you want to run in your service. Either [taskDefinition] or [taskDefinitionArgs] must be provided.
+        A map of tags to assign to the resource. If configured with a provider `default_tags` configuration block present, tags with matching keys will overwrite those defined at the provider-level.
         """
-        return pulumi.get(self, "task_definition")
+        return pulumi.get(self, "tags")
 
-    @task_definition.setter
-    def task_definition(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "task_definition", value)
+    @tags.setter
+    def tags(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
+        pulumi.set(self, "tags", value)
 
     @property
-    @pulumi.getter(name="taskDefinitionArgs")
-    def task_definition_args(self) -> Optional['FargateServiceTaskDefinitionArgs']:
+    @pulumi.getter(name="xffHeaderProcessingMode")
+    def xff_header_processing_mode(self) -> Optional[pulumi.Input[str]]:
         """
-        The args of task definition that you want to run in your service. Either [taskDefinition] or [taskDefinitionArgs] must be provided.
+        Determines how the load balancer modifies the `X-Forwarded-For` header in the HTTP request before sending the request to the target. The possible values are `append`, `preserve`, and `remove`. Only valid for Load Balancers of type `application`. The default is `append`.
         """
-        return pulumi.get(self, "task_definition_args")
+        return pulumi.get(self, "xff_header_processing_mode")
 
-    @task_definition_args.setter
-    def task_definition_args(self, value: Optional['FargateServiceTaskDefinitionArgs']):
-        pulumi.set(self, "task_definition_args", value)
+    @xff_header_processing_mode.setter
+    def xff_header_processing_mode(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "xff_header_processing_mode", value)
 
 
-class FargateService(pulumi.ComponentResource):
+class NetworkLoadBalancer(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 assign_public_ip: Optional[pulumi.Input[bool]] = None,
-                 cluster: Optional[pulumi.Input[str]] = None,
-                 continue_before_steady_state: Optional[pulumi.Input[bool]] = None,
-                 deployment_circuit_breaker: Optional[pulumi.Input[pulumi.InputType['pulumi_aws.ecs.ServiceDeploymentCircuitBreakerArgs']]] = None,
-                 deployment_controller: Optional[pulumi.Input[pulumi.InputType['pulumi_aws.ecs.ServiceDeploymentControllerArgs']]] = None,
-                 deployment_maximum_percent: Optional[pulumi.Input[int]] = None,
-                 deployment_minimum_healthy_percent: Optional[pulumi.Input[int]] = None,
-                 desired_count: Optional[pulumi.Input[int]] = None,
-                 enable_ecs_managed_tags: Optional[pulumi.Input[bool]] = None,
-                 enable_execute_command: Optional[pulumi.Input[bool]] = None,
-                 force_new_deployment: Optional[pulumi.Input[bool]] = None,
-                 health_check_grace_period_seconds: Optional[pulumi.Input[int]] = None,
-                 iam_role: Optional[pulumi.Input[str]] = None,
-                 load_balancers: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['pulumi_aws.ecs.ServiceLoadBalancerArgs']]]]] = None,
+                 access_logs: Optional[pulumi.Input[pulumi.InputType['pulumi_aws.lb.LoadBalancerAccessLogsArgs']]] = None,
+                 customer_owned_ipv4_pool: Optional[pulumi.Input[str]] = None,
+                 default_target_group: Optional[pulumi.InputType['TargetGroupArgs']] = None,
+                 default_target_group_port: Optional[pulumi.Input[int]] = None,
+                 desync_mitigation_mode: Optional[pulumi.Input[str]] = None,
+                 drop_invalid_header_fields: Optional[pulumi.Input[bool]] = None,
+                 enable_cross_zone_load_balancing: Optional[pulumi.Input[bool]] = None,
+                 enable_deletion_protection: Optional[pulumi.Input[bool]] = None,
+                 enable_tls_version_and_cipher_suite_headers: Optional[pulumi.Input[bool]] = None,
+                 enable_waf_fail_open: Optional[pulumi.Input[bool]] = None,
+                 enable_xff_client_port: Optional[pulumi.Input[bool]] = None,
+                 idle_timeout: Optional[pulumi.Input[int]] = None,
+                 internal: Optional[pulumi.Input[bool]] = None,
+                 ip_address_type: Optional[pulumi.Input[str]] = None,
+                 listener: Optional[pulumi.InputType['ListenerArgs']] = None,
+                 listeners: Optional[Sequence[pulumi.InputType['ListenerArgs']]] = None,
                  name: Optional[pulumi.Input[str]] = None,
-                 network_configuration: Optional[pulumi.Input[pulumi.InputType['pulumi_aws.ecs.ServiceNetworkConfigurationArgs']]] = None,
-                 placement_constraints: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['pulumi_aws.ecs.ServicePlacementConstraintArgs']]]]] = None,
-                 platform_version: Optional[pulumi.Input[str]] = None,
-                 propagate_tags: Optional[pulumi.Input[str]] = None,
-                 scheduling_strategy: Optional[pulumi.Input[str]] = None,
-                 service_registries: Optional[pulumi.Input[pulumi.InputType['pulumi_aws.ecs.ServiceServiceRegistriesArgs']]] = None,
+                 name_prefix: Optional[pulumi.Input[str]] = None,
+                 preserve_host_header: Optional[pulumi.Input[bool]] = None,
+                 subnet_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 subnet_mappings: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['pulumi_aws.lb.LoadBalancerSubnetMappingArgs']]]]] = None,
+                 subnets: Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ec2.Subnet']]]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
-                 task_definition: Optional[pulumi.Input[str]] = None,
-                 task_definition_args: Optional[pulumi.InputType['FargateServiceTaskDefinitionArgs']] = None,
+                 xff_header_processing_mode: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Create an ECS Service resource for Fargate with the given unique name, arguments, and options.
-        Creates Task definition if `taskDefinitionArgs` is specified.
+        Provides a Network Load Balancer resource with listeners and default target group.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[bool] assign_public_ip: Assign a public IP address to the ENI (Fargate launch type only). Valid values are `true` or `false`. Default `false`.
-        :param pulumi.Input[str] cluster: ARN of an ECS cluster.
-        :param pulumi.Input[bool] continue_before_steady_state: If `true`, this provider will not wait for the service to reach a steady state (like [`aws ecs wait services-stable`](https://docs.aws.amazon.com/cli/latest/reference/ecs/wait/services-stable.html)) before continuing. Default `false`.
-        :param pulumi.Input[pulumi.InputType['pulumi_aws.ecs.ServiceDeploymentCircuitBreakerArgs']] deployment_circuit_breaker: Configuration block for deployment circuit breaker. See below.
-        :param pulumi.Input[pulumi.InputType['pulumi_aws.ecs.ServiceDeploymentControllerArgs']] deployment_controller: Configuration block for deployment controller configuration. See below.
-        :param pulumi.Input[int] deployment_maximum_percent: Upper limit (as a percentage of the service's desiredCount) of the number of running tasks that can be running in a service during a deployment. Not valid when using the `DAEMON` scheduling strategy.
-        :param pulumi.Input[int] deployment_minimum_healthy_percent: Lower limit (as a percentage of the service's desiredCount) of the number of running tasks that must remain running and healthy in a service during a deployment.
-        :param pulumi.Input[int] desired_count: Number of instances of the task definition to place and keep running. Defaults to 0. Do not specify if using the `DAEMON` scheduling strategy.
-        :param pulumi.Input[bool] enable_ecs_managed_tags: Specifies whether to enable Amazon ECS managed tags for the tasks within the service.
-        :param pulumi.Input[bool] enable_execute_command: Specifies whether to enable Amazon ECS Exec for the tasks within the service.
-        :param pulumi.Input[bool] force_new_deployment: Enable to force a new task deployment of the service. This can be used to update tasks to use a newer Docker image with same image/tag combination (e.g., `myimage:latest`), roll Fargate tasks onto a newer platform version, or immediately deploy `ordered_placement_strategy` and `placement_constraints` updates.
-        :param pulumi.Input[int] health_check_grace_period_seconds: Seconds to ignore failing load balancer health checks on newly instantiated tasks to prevent premature shutdown, up to 2147483647. Only valid for services configured to use load balancers.
-        :param pulumi.Input[str] iam_role: ARN of the IAM role that allows Amazon ECS to make calls to your load balancer on your behalf. This parameter is required if you are using a load balancer with your service, but only if your task definition does not use the `awsvpc` network mode. If using `awsvpc` network mode, do not specify this role. If your account has already created the Amazon ECS service-linked role, that role is used by default for your service unless you specify a role here.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['pulumi_aws.ecs.ServiceLoadBalancerArgs']]]] load_balancers: Configuration block for load balancers. See below.
-        :param pulumi.Input[str] name: Name of the service (up to 255 letters, numbers, hyphens, and underscores)
-        :param pulumi.Input[pulumi.InputType['pulumi_aws.ecs.ServiceNetworkConfigurationArgs']] network_configuration: Network configuration for the service. This parameter is required for task definitions that use the `awsvpc` network mode to receive their own Elastic Network Interface, and it is not supported for other network modes. See below.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['pulumi_aws.ecs.ServicePlacementConstraintArgs']]]] placement_constraints: Rules that are taken into consideration during task placement. Updates to this configuration will take effect next task deployment unless `force_new_deployment` is enabled. Maximum number of `placement_constraints` is `10`. See below.
-        :param pulumi.Input[str] platform_version: Platform version on which to run your service. Only applicable for `launch_type` set to `FARGATE`. Defaults to `LATEST`. More information about Fargate platform versions can be found in the [AWS ECS User Guide](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/platform_versions.html).
-        :param pulumi.Input[str] propagate_tags: Specifies whether to propagate the tags from the task definition or the service to the tasks. The valid values are `SERVICE` and `TASK_DEFINITION`.
-        :param pulumi.Input[str] scheduling_strategy: Scheduling strategy to use for the service. The valid values are `REPLICA` and `DAEMON`. Defaults to `REPLICA`. Note that [*Tasks using the Fargate launch type or the `CODE_DEPLOY` or `EXTERNAL` deployment controller types don't support the `DAEMON` scheduling strategy*](https://docs.aws.amazon.com/AmazonECS/latest/APIReference/API_CreateService.html).
-        :param pulumi.Input[pulumi.InputType['pulumi_aws.ecs.ServiceServiceRegistriesArgs']] service_registries: Service discovery registries for the service. The maximum number of `service_registries` blocks is `1`. See below.
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Key-value map of resource tags. If configured with a provider `default_tags` configuration block present, tags with matching keys will overwrite those defined at the provider-level.
-        :param pulumi.Input[str] task_definition: Family and revision (`family:revision`) or full ARN of the task definition that you want to run in your service. Either [taskDefinition] or [taskDefinitionArgs] must be provided.
-        :param pulumi.InputType['FargateServiceTaskDefinitionArgs'] task_definition_args: The args of task definition that you want to run in your service. Either [taskDefinition] or [taskDefinitionArgs] must be provided.
+        :param pulumi.Input[pulumi.InputType['pulumi_aws.lb.LoadBalancerAccessLogsArgs']] access_logs: An Access Logs block. Access Logs documented below.
+        :param pulumi.Input[str] customer_owned_ipv4_pool: The ID of the customer owned ipv4 pool to use for this load balancer.
+        :param pulumi.InputType['TargetGroupArgs'] default_target_group: Options creating a default target group.
+        :param pulumi.Input[int] default_target_group_port: Port to use to connect with the target. Valid values are ports 1-65535. Defaults to 80.
+        :param pulumi.Input[str] desync_mitigation_mode: Determines how the load balancer handles requests that might pose a security risk to an application due to HTTP desync. Valid values are `monitor`, `defensive` (default), `strictest`.
+        :param pulumi.Input[bool] drop_invalid_header_fields: Indicates whether HTTP headers with header fields that are not valid are removed by the load balancer (true) or routed to targets (false). The default is false. Elastic Load Balancing requires that message header names contain only alphanumeric characters and hyphens. Only valid for Load Balancers of type `application`.
+        :param pulumi.Input[bool] enable_cross_zone_load_balancing: If true, cross-zone load balancing of the load balancer will be enabled. For `network` and `gateway` type load balancers, this feature is disabled by default (`false`). For `application` load balancer this feature is always enabled (`true`) and cannot be disabled. Defaults to `false`.
+        :param pulumi.Input[bool] enable_deletion_protection: If true, deletion of the load balancer will be disabled via the AWS API. This will prevent this provider from deleting the load balancer. Defaults to `false`.
+        :param pulumi.Input[bool] enable_tls_version_and_cipher_suite_headers: Indicates whether the two headers (`x-amzn-tls-version` and `x-amzn-tls-cipher-suite`), which contain information about the negotiated TLS version and cipher suite, are added to the client request before sending it to the target. Only valid for Load Balancers of type `application`. Defaults to `false`
+        :param pulumi.Input[bool] enable_waf_fail_open: Indicates whether to allow a WAF-enabled load balancer to route requests to targets if it is unable to forward the request to AWS WAF. Defaults to `false`.
+        :param pulumi.Input[bool] enable_xff_client_port: Indicates whether the X-Forwarded-For header should preserve the source port that the client used to connect to the load balancer in `application` load balancers. Defaults to `true`.
+        :param pulumi.Input[int] idle_timeout: The time in seconds that the connection is allowed to be idle. Only valid for Load Balancers of type `application`. Default: 60.
+        :param pulumi.Input[bool] internal: If true, the LB will be internal.
+        :param pulumi.Input[str] ip_address_type: The type of IP addresses used by the subnets for your load balancer. The possible values are `ipv4` and `dualstack`.
+        :param pulumi.InputType['ListenerArgs'] listener: A listener to create. Only one of [listener] and [listeners] can be specified.
+        :param Sequence[pulumi.InputType['ListenerArgs']] listeners: List of listeners to create. Only one of [listener] and [listeners] can be specified.
+        :param pulumi.Input[str] name: The name of the LB. This name must be unique within your AWS account, can have a maximum of 32 characters,
+               must contain only alphanumeric characters or hyphens, and must not begin or end with a hyphen. If not specified,
+               this provider will autogenerate a name beginning with `tf-lb`.
+        :param pulumi.Input[str] name_prefix: Creates a unique name beginning with the specified prefix. Conflicts with `name`.
+        :param pulumi.Input[bool] preserve_host_header: Indicates whether the Application Load Balancer should preserve the Host header in the HTTP request and send it to the target without any change. Defaults to `false`.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] subnet_ids: A list of subnet IDs to attach to the LB. Subnets
+               cannot be updated for Load Balancers of type `network`. Changing this value
+               for load balancers of type `network` will force a recreation of the resource.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['pulumi_aws.lb.LoadBalancerSubnetMappingArgs']]]] subnet_mappings: A subnet mapping block as documented below.
+        :param pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ec2.Subnet']]] subnets: A list of subnets to attach to the LB. Only one of [subnets], [subnetIds] or [subnetMappings] can be specified
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: A map of tags to assign to the resource. If configured with a provider `default_tags` configuration block present, tags with matching keys will overwrite those defined at the provider-level.
+        :param pulumi.Input[str] xff_header_processing_mode: Determines how the load balancer modifies the `X-Forwarded-For` header in the HTTP request before sending the request to the target. The possible values are `append`, `preserve`, and `remove`. Only valid for Load Balancers of type `application`. The default is `append`.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: Optional[FargateServiceArgs] = None,
+                 args: Optional[NetworkLoadBalancerArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Create an ECS Service resource for Fargate with the given unique name, arguments, and options.
-        Creates Task definition if `taskDefinitionArgs` is specified.
+        Provides a Network Load Balancer resource with listeners and default target group.
 
         :param str resource_name: The name of the resource.
-        :param FargateServiceArgs args: The arguments to use to populate this resource's properties.
+        :param NetworkLoadBalancerArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(FargateServiceArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(NetworkLoadBalancerArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 assign_public_ip: Optional[pulumi.Input[bool]] = None,
-                 cluster: Optional[pulumi.Input[str]] = None,
-                 continue_before_steady_state: Optional[pulumi.Input[bool]] = None,
-                 deployment_circuit_breaker: Optional[pulumi.Input[pulumi.InputType['pulumi_aws.ecs.ServiceDeploymentCircuitBreakerArgs']]] = None,
-                 deployment_controller: Optional[pulumi.Input[pulumi.InputType['pulumi_aws.ecs.ServiceDeploymentControllerArgs']]] = None,
-                 deployment_maximum_percent: Optional[pulumi.Input[int]] = None,
-                 deployment_minimum_healthy_percent: Optional[pulumi.Input[int]] = None,
-                 desired_count: Optional[pulumi.Input[int]] = None,
-                 enable_ecs_managed_tags: Optional[pulumi.Input[bool]] = None,
-                 enable_execute_command: Optional[pulumi.Input[bool]] = None,
-                 force_new_deployment: Optional[pulumi.Input[bool]] = None,
-                 health_check_grace_period_seconds: Optional[pulumi.Input[int]] = None,
-                 iam_role: Optional[pulumi.Input[str]] = None,
-                 load_balancers: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['pulumi_aws.ecs.ServiceLoadBalancerArgs']]]]] = None,
+                 access_logs: Optional[pulumi.Input[pulumi.InputType['pulumi_aws.lb.LoadBalancerAccessLogsArgs']]] = None,
+                 customer_owned_ipv4_pool: Optional[pulumi.Input[str]] = None,
+                 default_target_group: Optional[pulumi.InputType['TargetGroupArgs']] = None,
+                 default_target_group_port: Optional[pulumi.Input[int]] = None,
+                 desync_mitigation_mode: Optional[pulumi.Input[str]] = None,
+                 drop_invalid_header_fields: Optional[pulumi.Input[bool]] = None,
+                 enable_cross_zone_load_balancing: Optional[pulumi.Input[bool]] = None,
+                 enable_deletion_protection: Optional[pulumi.Input[bool]] = None,
+                 enable_tls_version_and_cipher_suite_headers: Optional[pulumi.Input[bool]] = None,
+                 enable_waf_fail_open: Optional[pulumi.Input[bool]] = None,
+                 enable_xff_client_port: Optional[pulumi.Input[bool]] = None,
+                 idle_timeout: Optional[pulumi.Input[int]] = None,
+                 internal: Optional[pulumi.Input[bool]] = None,
+                 ip_address_type: Optional[pulumi.Input[str]] = None,
+                 listener: Optional[pulumi.InputType['ListenerArgs']] = None,
+                 listeners: Optional[Sequence[pulumi.InputType['ListenerArgs']]] = None,
                  name: Optional[pulumi.Input[str]] = None,
-                 network_configuration: Optional[pulumi.Input[pulumi.InputType['pulumi_aws.ecs.ServiceNetworkConfigurationArgs']]] = None,
-                 placement_constraints: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['pulumi_aws.ecs.ServicePlacementConstraintArgs']]]]] = None,
-                 platform_version: Optional[pulumi.Input[str]] = None,
-                 propagate_tags: Optional[pulumi.Input[str]] = None,
-                 scheduling_strategy: Optional[pulumi.Input[str]] = None,
-                 service_registries: Optional[pulumi.Input[pulumi.InputType['pulumi_aws.ecs.ServiceServiceRegistriesArgs']]] = None,
+                 name_prefix: Optional[pulumi.Input[str]] = None,
+                 preserve_host_header: Optional[pulumi.Input[bool]] = None,
+                 subnet_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 subnet_mappings: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['pulumi_aws.lb.LoadBalancerSubnetMappingArgs']]]]] = None,
+                 subnets: Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ec2.Subnet']]]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
-                 task_definition: Optional[pulumi.Input[str]] = None,
-                 task_definition_args: Optional[pulumi.InputType['FargateServiceTaskDefinitionArgs']] = None,
+                 xff_header_processing_mode: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = FargateServiceArgs.__new__(FargateServiceArgs)
+            __props__ = NetworkLoadBalancerArgs.__new__(NetworkLoadBalancerArgs)
 
-            __props__.__dict__["assign_public_ip"] = assign_public_ip
-            __props__.__dict__["cluster"] = cluster
-            __props__.__dict__["continue_before_steady_state"] = continue_before_steady_state
-            __props__.__dict__["deployment_circuit_breaker"] = deployment_circuit_breaker
-            __props__.__dict__["deployment_controller"] = deployment_controller
-            __props__.__dict__["deployment_maximum_percent"] = deployment_maximum_percent
-            __props__.__dict__["deployment_minimum_healthy_percent"] = deployment_minimum_healthy_percent
-            __props__.__dict__["desired_count"] = desired_count
-            __props__.__dict__["enable_ecs_managed_tags"] = enable_ecs_managed_tags
-            __props__.__dict__["enable_execute_command"] = enable_execute_command
-            __props__.__dict__["force_new_deployment"] = force_new_deployment
-            __props__.__dict__["health_check_grace_period_seconds"] = health_check_grace_period_seconds
-            __props__.__dict__["iam_role"] = iam_role
-            __props__.__dict__["load_balancers"] = load_balancers
+            __props__.__dict__["access_logs"] = access_logs
+            __props__.__dict__["customer_owned_ipv4_pool"] = customer_owned_ipv4_pool
+            __props__.__dict__["default_target_group"] = default_target_group
+            __props__.__dict__["default_target_group_port"] = default_target_group_port
+            __props__.__dict__["desync_mitigation_mode"] = desync_mitigation_mode
+            __props__.__dict__["drop_invalid_header_fields"] = drop_invalid_header_fields
+            __props__.__dict__["enable_cross_zone_load_balancing"] = enable_cross_zone_load_balancing
+            __props__.__dict__["enable_deletion_protection"] = enable_deletion_protection
+            __props__.__dict__["enable_tls_version_and_cipher_suite_headers"] = enable_tls_version_and_cipher_suite_headers
+            __props__.__dict__["enable_waf_fail_open"] = enable_waf_fail_open
+            __props__.__dict__["enable_xff_client_port"] = enable_xff_client_port
+            __props__.__dict__["idle_timeout"] = idle_timeout
+            __props__.__dict__["internal"] = internal
+            __props__.__dict__["ip_address_type"] = ip_address_type
+            __props__.__dict__["listener"] = listener
+            __props__.__dict__["listeners"] = listeners
             __props__.__dict__["name"] = name
-            __props__.__dict__["network_configuration"] = network_configuration
-            __props__.__dict__["placement_constraints"] = placement_constraints
-            __props__.__dict__["platform_version"] = platform_version
-            __props__.__dict__["propagate_tags"] = propagate_tags
-            __props__.__dict__["scheduling_strategy"] = scheduling_strategy
-            __props__.__dict__["service_registries"] = service_registries
+            __props__.__dict__["name_prefix"] = name_prefix
+            __props__.__dict__["preserve_host_header"] = preserve_host_header
+            __props__.__dict__["subnet_ids"] = subnet_ids
+            __props__.__dict__["subnet_mappings"] = subnet_mappings
+            __props__.__dict__["subnets"] = subnets
             __props__.__dict__["tags"] = tags
-            __props__.__dict__["task_definition"] = task_definition
-            __props__.__dict__["task_definition_args"] = task_definition_args
-            __props__.__dict__["service"] = None
-        super(FargateService, __self__).__init__(
-            'awsx:ecs:FargateService',
+            __props__.__dict__["xff_header_processing_mode"] = xff_header_processing_mode
+            __props__.__dict__["load_balancer"] = None
+            __props__.__dict__["vpc_id"] = None
+        super(NetworkLoadBalancer, __self__).__init__(
+            'awsx:lb:NetworkLoadBalancer',
             resource_name,
             __props__,
             opts,
             remote=True)
 
     @property
+    @pulumi.getter(name="defaultTargetGroup")
+    def default_target_group(self) -> pulumi.Output['pulumi_aws.lb.TargetGroup']:
+        """
+        Default target group, if auto-created
+        """
+        return pulumi.get(self, "default_target_group")
+
+    @property
     @pulumi.getter
-    def service(self) -> pulumi.Output['pulumi_aws.ecs.Service']:
+    def listeners(self) -> pulumi.Output[Optional[Sequence['pulumi_aws.lb.Listener']]]:
+        """
+        Listeners created as part of this load balancer
+        """
+        return pulumi.get(self, "listeners")
+
+    @property
+    @pulumi.getter(name="loadBalancer")
+    def load_balancer(self) -> pulumi.Output['pulumi_aws.lb.LoadBalancer']:
         """
-        Underlying ECS Service resource
+        Underlying Load Balancer resource
         """
-        return pulumi.get(self, "service")
+        return pulumi.get(self, "load_balancer")
 
     @property
-    @pulumi.getter(name="taskDefinition")
-    def task_definition(self) -> pulumi.Output[Optional['pulumi_aws.ecs.TaskDefinition']]:
+    @pulumi.getter(name="vpcId")
+    def vpc_id(self) -> pulumi.Output[Optional[str]]:
         """
-        Underlying Fargate component resource if created from args
+        Id of the VPC in which this load balancer is operating
         """
-        return pulumi.get(self, "task_definition")
+        return pulumi.get(self, "vpc_id")
```

### Comparing `pulumi_awsx-1.0.2/pulumi_awsx/ecs/fargate_task_definition.py` & `pulumi_awsx-1.0.3/pulumi_awsx/ecs/fargate_task_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by pulumi-gen-awsx. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from .. import awsx as _awsx
 from ._inputs import *
@@ -427,20 +428,17 @@
                  proxy_configuration: Optional[pulumi.Input[pulumi.InputType['pulumi_aws.ecs.TaskDefinitionProxyConfigurationArgs']]] = None,
                  runtime_platform: Optional[pulumi.Input[pulumi.InputType['pulumi_aws.ecs.TaskDefinitionRuntimePlatformArgs']]] = None,
                  skip_destroy: Optional[pulumi.Input[bool]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  task_role: Optional[pulumi.InputType['_awsx.DefaultRoleWithPolicyArgs']] = None,
                  volumes: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['pulumi_aws.ecs.TaskDefinitionVolumeArgs']]]]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = FargateTaskDefinitionArgs.__new__(FargateTaskDefinitionArgs)
```

### Comparing `pulumi_awsx-1.0.2/pulumi_awsx/lb/_inputs.py` & `pulumi_awsx-1.0.3/pulumi_awsx/lb/_inputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by pulumi-gen-awsx. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 import pulumi_aws
 
@@ -192,15 +193,15 @@
             type: aws:lb:LoadBalancer
           frontEndTargetGroup:
             type: aws:lb:TargetGroup
           frontEndListener:
             type: aws:lb:Listener
             properties:
               loadBalancerArn: ${frontEndLoadBalancer.arn}
-              port: 443
+              port: '443'
               protocol: HTTPS
               sslPolicy: ELBSecurityPolicy-2016-08
               certificateArn: arn:aws:iam::187416307283:server-certificate/test_cert_rab3wuqwgja25ct3n4jdj2tzu4
               defaultActions:
                 - type: forward
                   targetGroupArn: ${frontEndTargetGroup.arn}
         ```
@@ -333,15 +334,15 @@
         ```
         ```yaml
         resources:
           frontEnd:
             type: aws:lb:Listener
             properties:
               loadBalancerArn: ${aws_lb.front_end.arn}
-              port: 443
+              port: '443'
               protocol: TLS
               certificateArn: arn:aws:iam::187416307283:server-certificate/test_cert_rab3wuqwgja25ct3n4jdj2tzu4
               alpnPolicy: HTTP2Preferred
               defaultActions:
                 - type: forward
                   targetGroupArn: ${aws_lb_target_group.front_end.arn}
         ```
@@ -503,20 +504,20 @@
         resources:
           frontEndLoadBalancer:
             type: aws:lb:LoadBalancer
           frontEndListener:
             type: aws:lb:Listener
             properties:
               loadBalancerArn: ${frontEndLoadBalancer.arn}
-              port: 80
+              port: '80'
               protocol: HTTP
               defaultActions:
                 - type: redirect
                   redirect:
-                    port: 443
+                    port: '443'
                     protocol: HTTPS
                     statusCode: HTTP_301
         ```
         {{% /example %}}
         {{% example %}}
         ### Fixed-response Action
 
@@ -674,22 +675,22 @@
         resources:
           frontEndLoadBalancer:
             type: aws:lb:LoadBalancer
           frontEndListener:
             type: aws:lb:Listener
             properties:
               loadBalancerArn: ${frontEndLoadBalancer.arn}
-              port: 80
+              port: '80'
               protocol: HTTP
               defaultActions:
                 - type: fixed-response
                   fixedResponse:
                     contentType: text/plain
                     messageBody: Fixed response content
-                    statusCode: 200
+                    statusCode: '200'
         ```
         {{% /example %}}
         {{% example %}}
         ### Authenticate-cognito Action
 
         ```typescript
         import * as pulumi from "@pulumi/pulumi";
@@ -936,15 +937,15 @@
             type: aws:cognito:UserPoolClient
           domain:
             type: aws:cognito:UserPoolDomain
           frontEndListener:
             type: aws:lb:Listener
             properties:
               loadBalancerArn: ${frontEndLoadBalancer.arn}
-              port: 80
+              port: '80'
               protocol: HTTP
               defaultActions:
                 - type: authenticate-cognito
                   authenticateCognito:
                     userPoolArn: ${pool.arn}
                     userPoolClientId: ${client.id}
                     userPoolDomain: ${domain.domain}
@@ -1166,15 +1167,15 @@
             type: aws:lb:LoadBalancer
           frontEndTargetGroup:
             type: aws:lb:TargetGroup
           frontEndListener:
             type: aws:lb:Listener
             properties:
               loadBalancerArn: ${frontEndLoadBalancer.arn}
-              port: 80
+              port: '80'
               protocol: HTTP
               defaultActions:
                 - type: authenticate-oidc
                   authenticateOidc:
                     authorizationEndpoint: https://example.com/authorization_endpoint
                     clientId: client_id
                     clientSecret: client_secret
@@ -1426,16 +1427,16 @@
          $ pulumi import aws:lb/listener:Listener front_end arn:aws:elasticloadbalancing:us-west-2:187416307283:listener/app/front-end-alb/8e4497da625e2d8a/9ab28ade35828f96
         ```
 
          
         :param pulumi.Input[str] alpn_policy: Name of the Application-Layer Protocol Negotiation (ALPN) policy. Can be set if `protocol` is `TLS`. Valid values are `HTTP1Only`, `HTTP2Only`, `HTTP2Optional`, `HTTP2Preferred`, and `None`.
         :param pulumi.Input[str] certificate_arn: ARN of the default SSL server certificate. Exactly one certificate is required if the protocol is HTTPS. For adding additional SSL certificates, see the `aws.lb.ListenerCertificate` resource.
         :param pulumi.Input[Sequence[pulumi.Input['pulumi_aws.lb.ListenerDefaultActionArgs']]] default_actions: Configuration block for default actions. Detailed below.
-        :param pulumi.Input[int] port: Port. Specify a value from `1` to `65535` or `#{port}`. Defaults to `#{port}`.
-        :param pulumi.Input[str] protocol: Protocol. Valid values are `HTTP`, `HTTPS`, or `#{protocol}`. Defaults to `#{protocol}`.
+        :param pulumi.Input[int] port: Port on which the load balancer is listening. Not valid for Gateway Load Balancers.
+        :param pulumi.Input[str] protocol: Protocol for connections from clients to the load balancer. For Application Load Balancers, valid values are `HTTP` and `HTTPS`, with a default of `HTTP`. For Network Load Balancers, valid values are `TCP`, `TLS`, `UDP`, and `TCP_UDP`. Not valid to use `UDP` or `TCP_UDP` if dual-stack mode is enabled. Not valid for Gateway Load Balancers.
         :param pulumi.Input[str] ssl_policy: Name of the SSL Policy for the listener. Required if `protocol` is `HTTPS` or `TLS`.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: A map of tags to assign to the resource. .If configured with a provider `default_tags` configuration block present, tags with matching keys will overwrite those defined at the provider-level.
         """
         if alpn_policy is not None:
             pulumi.set(__self__, "alpn_policy", alpn_policy)
         if certificate_arn is not None:
             pulumi.set(__self__, "certificate_arn", certificate_arn)
@@ -1486,27 +1487,27 @@
     def default_actions(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.lb.ListenerDefaultActionArgs']]]]):
         pulumi.set(self, "default_actions", value)
 
     @property
     @pulumi.getter
     def port(self) -> Optional[pulumi.Input[int]]:
         """
-        Port. Specify a value from `1` to `65535` or `#{port}`. Defaults to `#{port}`.
+        Port on which the load balancer is listening. Not valid for Gateway Load Balancers.
         """
         return pulumi.get(self, "port")
 
     @port.setter
     def port(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "port", value)
 
     @property
     @pulumi.getter
     def protocol(self) -> Optional[pulumi.Input[str]]:
         """
-        Protocol. Valid values are `HTTP`, `HTTPS`, or `#{protocol}`. Defaults to `#{protocol}`.
+        Protocol for connections from clients to the load balancer. For Application Load Balancers, valid values are `HTTP` and `HTTPS`, with a default of `HTTP`. For Network Load Balancers, valid values are `TCP`, `TLS`, `UDP`, and `TCP_UDP`. Not valid to use `UDP` or `TCP_UDP` if dual-stack mode is enabled. Not valid for Gateway Load Balancers.
         """
         return pulumi.get(self, "protocol")
 
     @protocol.setter
     def protocol(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "protocol", value)
 
@@ -1540,24 +1541,26 @@
     def __init__(__self__, *,
                  connection_termination: Optional[pulumi.Input[bool]] = None,
                  deregistration_delay: Optional[pulumi.Input[int]] = None,
                  health_check: Optional[pulumi.Input['pulumi_aws.lb.TargetGroupHealthCheckArgs']] = None,
                  ip_address_type: Optional[pulumi.Input[str]] = None,
                  lambda_multi_value_headers_enabled: Optional[pulumi.Input[bool]] = None,
                  load_balancing_algorithm_type: Optional[pulumi.Input[str]] = None,
+                 load_balancing_cross_zone_enabled: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  name_prefix: Optional[pulumi.Input[str]] = None,
                  port: Optional[pulumi.Input[int]] = None,
                  preserve_client_ip: Optional[pulumi.Input[str]] = None,
                  protocol: Optional[pulumi.Input[str]] = None,
                  protocol_version: Optional[pulumi.Input[str]] = None,
                  proxy_protocol_v2: Optional[pulumi.Input[bool]] = None,
                  slow_start: Optional[pulumi.Input[int]] = None,
                  stickiness: Optional[pulumi.Input['pulumi_aws.lb.TargetGroupStickinessArgs']] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
+                 target_failovers: Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.lb.TargetGroupTargetFailoverArgs']]]] = None,
                  target_type: Optional[pulumi.Input[str]] = None,
                  vpc_id: Optional[pulumi.Input[str]] = None):
         """
         Provides a Target Group resource for use with Load Balancer resources.
 
         > **Note:** `aws.alb.TargetGroup` is known as `aws.lb.TargetGroup`. The functionality is identical.
 
@@ -1820,17 +1823,15 @@
         {{% example %}}
         ### Lambda Target Group
 
         ```typescript
         import * as pulumi from "@pulumi/pulumi";
         import * as aws from "@pulumi/aws";
 
-        const lambda_example = new aws.lb.TargetGroup("lambda-example", {
-            targetType: "lambda",
-        });
+        const lambda_example = new aws.lb.TargetGroup("lambda-example", {targetType: "lambda"});
         ```
         ```python
         import pulumi
         import pulumi_aws as aws
 
         lambda_example = aws.lb.TargetGroup("lambda-example", target_type="lambda")
         ```
@@ -2023,24 +2024,26 @@
          
         :param pulumi.Input[bool] connection_termination: Whether to terminate connections at the end of the deregistration timeout on Network Load Balancers. See [doc](https://docs.aws.amazon.com/elasticloadbalancing/latest/network/load-balancer-target-groups.html#deregistration-delay) for more information. Default is `false`.
         :param pulumi.Input[int] deregistration_delay: Amount time for Elastic Load Balancing to wait before changing the state of a deregistering target from draining to unused. The range is 0-3600 seconds. The default value is 300 seconds.
         :param pulumi.Input['pulumi_aws.lb.TargetGroupHealthCheckArgs'] health_check: Health Check configuration block. Detailed below.
         :param pulumi.Input[str] ip_address_type: The type of IP addresses used by the target group, only supported when target type is set to `ip`. Possible values are `ipv4` or `ipv6`.
         :param pulumi.Input[bool] lambda_multi_value_headers_enabled: Whether the request and response headers exchanged between the load balancer and the Lambda function include arrays of values or strings. Only applies when `target_type` is `lambda`. Default is `false`.
         :param pulumi.Input[str] load_balancing_algorithm_type: Determines how the load balancer selects targets when routing requests. Only applicable for Application Load Balancer Target Groups. The value is `round_robin` or `least_outstanding_requests`. The default is `round_robin`.
-        :param pulumi.Input[str] name: Name of the target group. If omitted, this provider will assign a random, unique name.
+        :param pulumi.Input[str] load_balancing_cross_zone_enabled: Indicates whether cross zone load balancing is enabled. The value is `"true"`, `"false"` or `"use_load_balancer_configuration"`. The default is `"use_load_balancer_configuration"`.
+        :param pulumi.Input[str] name: Name of the target group. If omitted, this provider will assign a random, unique name. This name must be unique per region per account, can have a maximum of 32 characters, must contain only alphanumeric characters or hyphens, and must not begin or end with a hyphen.
         :param pulumi.Input[str] name_prefix: Creates a unique name beginning with the specified prefix. Conflicts with `name`. Cannot be longer than 6 characters.
-        :param pulumi.Input[int] port: Port to use to connect with the target. Valid values are either ports 1-65535, or `traffic-port`. Defaults to `traffic-port`.
+        :param pulumi.Input[int] port: Port on which targets receive traffic, unless overridden when registering a specific target. Required when `target_type` is `instance`, `ip` or `alb`. Does not apply when `target_type` is `lambda`.
         :param pulumi.Input[str] preserve_client_ip: Whether client IP preservation is enabled. See [doc](https://docs.aws.amazon.com/elasticloadbalancing/latest/network/load-balancer-target-groups.html#client-ip-preservation) for more information.
-        :param pulumi.Input[str] protocol: Protocol to use to connect with the target. Defaults to `HTTP`. Not applicable when `target_type` is `lambda`.
-        :param pulumi.Input[str] protocol_version: Only applicable when `protocol` is `HTTP` or `HTTPS`. The protocol version. Specify GRPC to send requests to targets using gRPC. Specify HTTP2 to send requests to targets using HTTP/2. The default is HTTP1, which sends requests to targets using HTTP/1.1
+        :param pulumi.Input[str] protocol: Protocol to use for routing traffic to the targets. Should be one of `GENEVE`, `HTTP`, `HTTPS`, `TCP`, `TCP_UDP`, `TLS`, or `UDP`. Required when `target_type` is `instance`, `ip` or `alb`. Does not apply when `target_type` is `lambda`.
+        :param pulumi.Input[str] protocol_version: Only applicable when `protocol` is `HTTP` or `HTTPS`. The protocol version. Specify `GRPC` to send requests to targets using gRPC. Specify `HTTP2` to send requests to targets using HTTP/2. The default is `HTTP1`, which sends requests to targets using HTTP/1.1
         :param pulumi.Input[bool] proxy_protocol_v2: Whether to enable support for proxy protocol v2 on Network Load Balancers. See [doc](https://docs.aws.amazon.com/elasticloadbalancing/latest/network/load-balancer-target-groups.html#proxy-protocol) for more information. Default is `false`.
         :param pulumi.Input[int] slow_start: Amount time for targets to warm up before the load balancer sends them a full share of requests. The range is 30-900 seconds or 0 to disable. The default value is 0 seconds.
         :param pulumi.Input['pulumi_aws.lb.TargetGroupStickinessArgs'] stickiness: Stickiness configuration block. Detailed below.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Map of tags to assign to the resource. If configured with a provider `default_tags` configuration block present, tags with matching keys will overwrite those defined at the provider-level.
+        :param pulumi.Input[Sequence[pulumi.Input['pulumi_aws.lb.TargetGroupTargetFailoverArgs']]] target_failovers: Target failover block. Only applicable for Gateway Load Balancer target groups. See target_failover for more information.
         :param pulumi.Input[str] target_type: Type of target that you must specify when registering targets with this target group. See [doc](https://docs.aws.amazon.com/elasticloadbalancing/latest/APIReference/API_CreateTargetGroup.html) for supported values. The default is `instance`.
         :param pulumi.Input[str] vpc_id: Identifier of the VPC in which to create the target group. Required when `target_type` is `instance`, `ip` or `alb`. Does not apply when `target_type` is `lambda`.
         """
         if connection_termination is not None:
             pulumi.set(__self__, "connection_termination", connection_termination)
         if deregistration_delay is not None:
             pulumi.set(__self__, "deregistration_delay", deregistration_delay)
@@ -2048,14 +2051,16 @@
             pulumi.set(__self__, "health_check", health_check)
         if ip_address_type is not None:
             pulumi.set(__self__, "ip_address_type", ip_address_type)
         if lambda_multi_value_headers_enabled is not None:
             pulumi.set(__self__, "lambda_multi_value_headers_enabled", lambda_multi_value_headers_enabled)
         if load_balancing_algorithm_type is not None:
             pulumi.set(__self__, "load_balancing_algorithm_type", load_balancing_algorithm_type)
+        if load_balancing_cross_zone_enabled is not None:
+            pulumi.set(__self__, "load_balancing_cross_zone_enabled", load_balancing_cross_zone_enabled)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if name_prefix is not None:
             pulumi.set(__self__, "name_prefix", name_prefix)
         if port is not None:
             pulumi.set(__self__, "port", port)
         if preserve_client_ip is not None:
@@ -2068,14 +2073,16 @@
             pulumi.set(__self__, "proxy_protocol_v2", proxy_protocol_v2)
         if slow_start is not None:
             pulumi.set(__self__, "slow_start", slow_start)
         if stickiness is not None:
             pulumi.set(__self__, "stickiness", stickiness)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
+        if target_failovers is not None:
+            pulumi.set(__self__, "target_failovers", target_failovers)
         if target_type is not None:
             pulumi.set(__self__, "target_type", target_type)
         if vpc_id is not None:
             pulumi.set(__self__, "vpc_id", vpc_id)
 
     @property
     @pulumi.getter(name="connectionTermination")
@@ -2146,18 +2153,30 @@
         return pulumi.get(self, "load_balancing_algorithm_type")
 
     @load_balancing_algorithm_type.setter
     def load_balancing_algorithm_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "load_balancing_algorithm_type", value)
 
     @property
+    @pulumi.getter(name="loadBalancingCrossZoneEnabled")
+    def load_balancing_cross_zone_enabled(self) -> Optional[pulumi.Input[str]]:
+        """
+        Indicates whether cross zone load balancing is enabled. The value is `"true"`, `"false"` or `"use_load_balancer_configuration"`. The default is `"use_load_balancer_configuration"`.
+        """
+        return pulumi.get(self, "load_balancing_cross_zone_enabled")
+
+    @load_balancing_cross_zone_enabled.setter
+    def load_balancing_cross_zone_enabled(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "load_balancing_cross_zone_enabled", value)
+
+    @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Name of the target group. If omitted, this provider will assign a random, unique name.
+        Name of the target group. If omitted, this provider will assign a random, unique name. This name must be unique per region per account, can have a maximum of 32 characters, must contain only alphanumeric characters or hyphens, and must not begin or end with a hyphen.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -2173,15 +2192,15 @@
     def name_prefix(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name_prefix", value)
 
     @property
     @pulumi.getter
     def port(self) -> Optional[pulumi.Input[int]]:
         """
-        Port to use to connect with the target. Valid values are either ports 1-65535, or `traffic-port`. Defaults to `traffic-port`.
+        Port on which targets receive traffic, unless overridden when registering a specific target. Required when `target_type` is `instance`, `ip` or `alb`. Does not apply when `target_type` is `lambda`.
         """
         return pulumi.get(self, "port")
 
     @port.setter
     def port(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "port", value)
 
@@ -2197,27 +2216,27 @@
     def preserve_client_ip(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "preserve_client_ip", value)
 
     @property
     @pulumi.getter
     def protocol(self) -> Optional[pulumi.Input[str]]:
         """
-        Protocol to use to connect with the target. Defaults to `HTTP`. Not applicable when `target_type` is `lambda`.
+        Protocol to use for routing traffic to the targets. Should be one of `GENEVE`, `HTTP`, `HTTPS`, `TCP`, `TCP_UDP`, `TLS`, or `UDP`. Required when `target_type` is `instance`, `ip` or `alb`. Does not apply when `target_type` is `lambda`.
         """
         return pulumi.get(self, "protocol")
 
     @protocol.setter
     def protocol(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "protocol", value)
 
     @property
     @pulumi.getter(name="protocolVersion")
     def protocol_version(self) -> Optional[pulumi.Input[str]]:
         """
-        Only applicable when `protocol` is `HTTP` or `HTTPS`. The protocol version. Specify GRPC to send requests to targets using gRPC. Specify HTTP2 to send requests to targets using HTTP/2. The default is HTTP1, which sends requests to targets using HTTP/1.1
+        Only applicable when `protocol` is `HTTP` or `HTTPS`. The protocol version. Specify `GRPC` to send requests to targets using gRPC. Specify `HTTP2` to send requests to targets using HTTP/2. The default is `HTTP1`, which sends requests to targets using HTTP/1.1
         """
         return pulumi.get(self, "protocol_version")
 
     @protocol_version.setter
     def protocol_version(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "protocol_version", value)
 
@@ -2266,14 +2285,26 @@
         return pulumi.get(self, "tags")
 
     @tags.setter
     def tags(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "tags", value)
 
     @property
+    @pulumi.getter(name="targetFailovers")
+    def target_failovers(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.lb.TargetGroupTargetFailoverArgs']]]]:
+        """
+        Target failover block. Only applicable for Gateway Load Balancer target groups. See target_failover for more information.
+        """
+        return pulumi.get(self, "target_failovers")
+
+    @target_failovers.setter
+    def target_failovers(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.lb.TargetGroupTargetFailoverArgs']]]]):
+        pulumi.set(self, "target_failovers", value)
+
+    @property
     @pulumi.getter(name="targetType")
     def target_type(self) -> Optional[pulumi.Input[str]]:
         """
         Type of target that you must specify when registering targets with this target group. See [doc](https://docs.aws.amazon.com/elasticloadbalancing/latest/APIReference/API_CreateTargetGroup.html) for supported values. The default is `instance`.
         """
         return pulumi.get(self, "target_type")
```

### Comparing `pulumi_awsx-1.0.2/pulumi_awsx/lb/application_load_balancer.py` & `pulumi_awsx-1.0.3/pulumi_awsx/lb/application_load_balancer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by pulumi-gen-awsx. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from .. import awsx as _awsx
 from ._inputs import *
@@ -21,58 +22,63 @@
                  default_security_group: Optional['_awsx.DefaultSecurityGroupArgs'] = None,
                  default_target_group: Optional['TargetGroupArgs'] = None,
                  default_target_group_port: Optional[pulumi.Input[int]] = None,
                  desync_mitigation_mode: Optional[pulumi.Input[str]] = None,
                  drop_invalid_header_fields: Optional[pulumi.Input[bool]] = None,
                  enable_deletion_protection: Optional[pulumi.Input[bool]] = None,
                  enable_http2: Optional[pulumi.Input[bool]] = None,
+                 enable_tls_version_and_cipher_suite_headers: Optional[pulumi.Input[bool]] = None,
                  enable_waf_fail_open: Optional[pulumi.Input[bool]] = None,
+                 enable_xff_client_port: Optional[pulumi.Input[bool]] = None,
                  idle_timeout: Optional[pulumi.Input[int]] = None,
                  internal: Optional[pulumi.Input[bool]] = None,
                  ip_address_type: Optional[pulumi.Input[str]] = None,
                  listener: Optional['ListenerArgs'] = None,
                  listeners: Optional[Sequence['ListenerArgs']] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  name_prefix: Optional[pulumi.Input[str]] = None,
                  preserve_host_header: Optional[pulumi.Input[bool]] = None,
                  security_groups: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  subnet_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  subnet_mappings: Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.lb.LoadBalancerSubnetMappingArgs']]]] = None,
                  subnets: Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ec2.Subnet']]]] = None,
-                 tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
+                 tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
+                 xff_header_processing_mode: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a ApplicationLoadBalancer resource.
         :param pulumi.Input['pulumi_aws.lb.LoadBalancerAccessLogsArgs'] access_logs: An Access Logs block. Access Logs documented below.
         :param pulumi.Input[str] customer_owned_ipv4_pool: The ID of the customer owned ipv4 pool to use for this load balancer.
         :param '_awsx.DefaultSecurityGroupArgs' default_security_group: Options for creating a default security group if [securityGroups] not specified.
         :param 'TargetGroupArgs' default_target_group: Options creating a default target group.
         :param pulumi.Input[int] default_target_group_port: Port to use to connect with the target. Valid values are ports 1-65535. Defaults to 80.
         :param pulumi.Input[str] desync_mitigation_mode: Determines how the load balancer handles requests that might pose a security risk to an application due to HTTP desync. Valid values are `monitor`, `defensive` (default), `strictest`.
         :param pulumi.Input[bool] drop_invalid_header_fields: Indicates whether HTTP headers with header fields that are not valid are removed by the load balancer (true) or routed to targets (false). The default is false. Elastic Load Balancing requires that message header names contain only alphanumeric characters and hyphens. Only valid for Load Balancers of type `application`.
-        :param pulumi.Input[bool] enable_deletion_protection: If true, deletion of the load balancer will be disabled via
-               the AWS API. This will prevent this provider from deleting the load balancer. Defaults to `false`.
+        :param pulumi.Input[bool] enable_deletion_protection: If true, deletion of the load balancer will be disabled via the AWS API. This will prevent this provider from deleting the load balancer. Defaults to `false`.
         :param pulumi.Input[bool] enable_http2: Indicates whether HTTP/2 is enabled in `application` load balancers. Defaults to `true`.
+        :param pulumi.Input[bool] enable_tls_version_and_cipher_suite_headers: Indicates whether the two headers (`x-amzn-tls-version` and `x-amzn-tls-cipher-suite`), which contain information about the negotiated TLS version and cipher suite, are added to the client request before sending it to the target. Only valid for Load Balancers of type `application`. Defaults to `false`
         :param pulumi.Input[bool] enable_waf_fail_open: Indicates whether to allow a WAF-enabled load balancer to route requests to targets if it is unable to forward the request to AWS WAF. Defaults to `false`.
+        :param pulumi.Input[bool] enable_xff_client_port: Indicates whether the X-Forwarded-For header should preserve the source port that the client used to connect to the load balancer in `application` load balancers. Defaults to `true`.
         :param pulumi.Input[int] idle_timeout: The time in seconds that the connection is allowed to be idle. Only valid for Load Balancers of type `application`. Default: 60.
         :param pulumi.Input[bool] internal: If true, the LB will be internal.
-        :param pulumi.Input[str] ip_address_type: The type of IP addresses used by the subnets for your load balancer. The possible values are `ipv4` and `dualstack`
+        :param pulumi.Input[str] ip_address_type: The type of IP addresses used by the subnets for your load balancer. The possible values are `ipv4` and `dualstack`.
         :param 'ListenerArgs' listener: A listener to create. Only one of [listener] and [listeners] can be specified.
         :param Sequence['ListenerArgs'] listeners: List of listeners to create. Only one of [listener] and [listeners] can be specified.
         :param pulumi.Input[str] name: The name of the LB. This name must be unique within your AWS account, can have a maximum of 32 characters,
                must contain only alphanumeric characters or hyphens, and must not begin or end with a hyphen. If not specified,
                this provider will autogenerate a name beginning with `tf-lb`.
         :param pulumi.Input[str] name_prefix: Creates a unique name beginning with the specified prefix. Conflicts with `name`.
         :param pulumi.Input[bool] preserve_host_header: Indicates whether the Application Load Balancer should preserve the Host header in the HTTP request and send it to the target without any change. Defaults to `false`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] security_groups: A list of security group IDs to assign to the LB. Only valid for Load Balancers of type `application`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] subnet_ids: A list of subnet IDs to attach to the LB. Subnets
                cannot be updated for Load Balancers of type `network`. Changing this value
                for load balancers of type `network` will force a recreation of the resource.
         :param pulumi.Input[Sequence[pulumi.Input['pulumi_aws.lb.LoadBalancerSubnetMappingArgs']]] subnet_mappings: A subnet mapping block as documented below.
         :param pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ec2.Subnet']]] subnets: A list of subnets to attach to the LB. Only one of [subnets], [subnetIds] or [subnetMappings] can be specified
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: A map of tags to assign to the resource. If configured with a provider `default_tags` configuration block present, tags with matching keys will overwrite those defined at the provider-level.
+        :param pulumi.Input[str] xff_header_processing_mode: Determines how the load balancer modifies the `X-Forwarded-For` header in the HTTP request before sending the request to the target. The possible values are `append`, `preserve`, and `remove`. Only valid for Load Balancers of type `application`. The default is `append`.
         """
         if access_logs is not None:
             pulumi.set(__self__, "access_logs", access_logs)
         if customer_owned_ipv4_pool is not None:
             pulumi.set(__self__, "customer_owned_ipv4_pool", customer_owned_ipv4_pool)
         if default_security_group is not None:
             pulumi.set(__self__, "default_security_group", default_security_group)
@@ -84,16 +90,20 @@
             pulumi.set(__self__, "desync_mitigation_mode", desync_mitigation_mode)
         if drop_invalid_header_fields is not None:
             pulumi.set(__self__, "drop_invalid_header_fields", drop_invalid_header_fields)
         if enable_deletion_protection is not None:
             pulumi.set(__self__, "enable_deletion_protection", enable_deletion_protection)
         if enable_http2 is not None:
             pulumi.set(__self__, "enable_http2", enable_http2)
+        if enable_tls_version_and_cipher_suite_headers is not None:
+            pulumi.set(__self__, "enable_tls_version_and_cipher_suite_headers", enable_tls_version_and_cipher_suite_headers)
         if enable_waf_fail_open is not None:
             pulumi.set(__self__, "enable_waf_fail_open", enable_waf_fail_open)
+        if enable_xff_client_port is not None:
+            pulumi.set(__self__, "enable_xff_client_port", enable_xff_client_port)
         if idle_timeout is not None:
             pulumi.set(__self__, "idle_timeout", idle_timeout)
         if internal is not None:
             pulumi.set(__self__, "internal", internal)
         if ip_address_type is not None:
             pulumi.set(__self__, "ip_address_type", ip_address_type)
         if listener is not None:
@@ -112,14 +122,16 @@
             pulumi.set(__self__, "subnet_ids", subnet_ids)
         if subnet_mappings is not None:
             pulumi.set(__self__, "subnet_mappings", subnet_mappings)
         if subnets is not None:
             pulumi.set(__self__, "subnets", subnets)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
+        if xff_header_processing_mode is not None:
+            pulumi.set(__self__, "xff_header_processing_mode", xff_header_processing_mode)
 
     @property
     @pulumi.getter(name="accessLogs")
     def access_logs(self) -> Optional[pulumi.Input['pulumi_aws.lb.LoadBalancerAccessLogsArgs']]:
         """
         An Access Logs block. Access Logs documented below.
         """
@@ -201,16 +213,15 @@
     def drop_invalid_header_fields(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "drop_invalid_header_fields", value)
 
     @property
     @pulumi.getter(name="enableDeletionProtection")
     def enable_deletion_protection(self) -> Optional[pulumi.Input[bool]]:
         """
-        If true, deletion of the load balancer will be disabled via
-        the AWS API. This will prevent this provider from deleting the load balancer. Defaults to `false`.
+        If true, deletion of the load balancer will be disabled via the AWS API. This will prevent this provider from deleting the load balancer. Defaults to `false`.
         """
         return pulumi.get(self, "enable_deletion_protection")
 
     @enable_deletion_protection.setter
     def enable_deletion_protection(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enable_deletion_protection", value)
 
@@ -223,26 +234,50 @@
         return pulumi.get(self, "enable_http2")
 
     @enable_http2.setter
     def enable_http2(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enable_http2", value)
 
     @property
+    @pulumi.getter(name="enableTlsVersionAndCipherSuiteHeaders")
+    def enable_tls_version_and_cipher_suite_headers(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Indicates whether the two headers (`x-amzn-tls-version` and `x-amzn-tls-cipher-suite`), which contain information about the negotiated TLS version and cipher suite, are added to the client request before sending it to the target. Only valid for Load Balancers of type `application`. Defaults to `false`
+        """
+        return pulumi.get(self, "enable_tls_version_and_cipher_suite_headers")
+
+    @enable_tls_version_and_cipher_suite_headers.setter
+    def enable_tls_version_and_cipher_suite_headers(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "enable_tls_version_and_cipher_suite_headers", value)
+
+    @property
     @pulumi.getter(name="enableWafFailOpen")
     def enable_waf_fail_open(self) -> Optional[pulumi.Input[bool]]:
         """
         Indicates whether to allow a WAF-enabled load balancer to route requests to targets if it is unable to forward the request to AWS WAF. Defaults to `false`.
         """
         return pulumi.get(self, "enable_waf_fail_open")
 
     @enable_waf_fail_open.setter
     def enable_waf_fail_open(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enable_waf_fail_open", value)
 
     @property
+    @pulumi.getter(name="enableXffClientPort")
+    def enable_xff_client_port(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Indicates whether the X-Forwarded-For header should preserve the source port that the client used to connect to the load balancer in `application` load balancers. Defaults to `true`.
+        """
+        return pulumi.get(self, "enable_xff_client_port")
+
+    @enable_xff_client_port.setter
+    def enable_xff_client_port(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "enable_xff_client_port", value)
+
+    @property
     @pulumi.getter(name="idleTimeout")
     def idle_timeout(self) -> Optional[pulumi.Input[int]]:
         """
         The time in seconds that the connection is allowed to be idle. Only valid for Load Balancers of type `application`. Default: 60.
         """
         return pulumi.get(self, "idle_timeout")
 
@@ -262,15 +297,15 @@
     def internal(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "internal", value)
 
     @property
     @pulumi.getter(name="ipAddressType")
     def ip_address_type(self) -> Optional[pulumi.Input[str]]:
         """
-        The type of IP addresses used by the subnets for your load balancer. The possible values are `ipv4` and `dualstack`
+        The type of IP addresses used by the subnets for your load balancer. The possible values are `ipv4` and `dualstack`.
         """
         return pulumi.get(self, "ip_address_type")
 
     @ip_address_type.setter
     def ip_address_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "ip_address_type", value)
 
@@ -394,14 +429,26 @@
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
     def tags(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "tags", value)
 
+    @property
+    @pulumi.getter(name="xffHeaderProcessingMode")
+    def xff_header_processing_mode(self) -> Optional[pulumi.Input[str]]:
+        """
+        Determines how the load balancer modifies the `X-Forwarded-For` header in the HTTP request before sending the request to the target. The possible values are `append`, `preserve`, and `remove`. Only valid for Load Balancers of type `application`. The default is `append`.
+        """
+        return pulumi.get(self, "xff_header_processing_mode")
+
+    @xff_header_processing_mode.setter
+    def xff_header_processing_mode(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "xff_header_processing_mode", value)
+
 
 class ApplicationLoadBalancer(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  access_logs: Optional[pulumi.Input[pulumi.InputType['pulumi_aws.lb.LoadBalancerAccessLogsArgs']]] = None,
@@ -409,62 +456,67 @@
                  default_security_group: Optional[pulumi.InputType['_awsx.DefaultSecurityGroupArgs']] = None,
                  default_target_group: Optional[pulumi.InputType['TargetGroupArgs']] = None,
                  default_target_group_port: Optional[pulumi.Input[int]] = None,
                  desync_mitigation_mode: Optional[pulumi.Input[str]] = None,
                  drop_invalid_header_fields: Optional[pulumi.Input[bool]] = None,
                  enable_deletion_protection: Optional[pulumi.Input[bool]] = None,
                  enable_http2: Optional[pulumi.Input[bool]] = None,
+                 enable_tls_version_and_cipher_suite_headers: Optional[pulumi.Input[bool]] = None,
                  enable_waf_fail_open: Optional[pulumi.Input[bool]] = None,
+                 enable_xff_client_port: Optional[pulumi.Input[bool]] = None,
                  idle_timeout: Optional[pulumi.Input[int]] = None,
                  internal: Optional[pulumi.Input[bool]] = None,
                  ip_address_type: Optional[pulumi.Input[str]] = None,
                  listener: Optional[pulumi.InputType['ListenerArgs']] = None,
                  listeners: Optional[Sequence[pulumi.InputType['ListenerArgs']]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  name_prefix: Optional[pulumi.Input[str]] = None,
                  preserve_host_header: Optional[pulumi.Input[bool]] = None,
                  security_groups: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  subnet_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  subnet_mappings: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['pulumi_aws.lb.LoadBalancerSubnetMappingArgs']]]]] = None,
                  subnets: Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ec2.Subnet']]]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
+                 xff_header_processing_mode: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Provides an Application Load Balancer resource with listeners, default target group and default security group.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['pulumi_aws.lb.LoadBalancerAccessLogsArgs']] access_logs: An Access Logs block. Access Logs documented below.
         :param pulumi.Input[str] customer_owned_ipv4_pool: The ID of the customer owned ipv4 pool to use for this load balancer.
         :param pulumi.InputType['_awsx.DefaultSecurityGroupArgs'] default_security_group: Options for creating a default security group if [securityGroups] not specified.
         :param pulumi.InputType['TargetGroupArgs'] default_target_group: Options creating a default target group.
         :param pulumi.Input[int] default_target_group_port: Port to use to connect with the target. Valid values are ports 1-65535. Defaults to 80.
         :param pulumi.Input[str] desync_mitigation_mode: Determines how the load balancer handles requests that might pose a security risk to an application due to HTTP desync. Valid values are `monitor`, `defensive` (default), `strictest`.
         :param pulumi.Input[bool] drop_invalid_header_fields: Indicates whether HTTP headers with header fields that are not valid are removed by the load balancer (true) or routed to targets (false). The default is false. Elastic Load Balancing requires that message header names contain only alphanumeric characters and hyphens. Only valid for Load Balancers of type `application`.
-        :param pulumi.Input[bool] enable_deletion_protection: If true, deletion of the load balancer will be disabled via
-               the AWS API. This will prevent this provider from deleting the load balancer. Defaults to `false`.
+        :param pulumi.Input[bool] enable_deletion_protection: If true, deletion of the load balancer will be disabled via the AWS API. This will prevent this provider from deleting the load balancer. Defaults to `false`.
         :param pulumi.Input[bool] enable_http2: Indicates whether HTTP/2 is enabled in `application` load balancers. Defaults to `true`.
+        :param pulumi.Input[bool] enable_tls_version_and_cipher_suite_headers: Indicates whether the two headers (`x-amzn-tls-version` and `x-amzn-tls-cipher-suite`), which contain information about the negotiated TLS version and cipher suite, are added to the client request before sending it to the target. Only valid for Load Balancers of type `application`. Defaults to `false`
         :param pulumi.Input[bool] enable_waf_fail_open: Indicates whether to allow a WAF-enabled load balancer to route requests to targets if it is unable to forward the request to AWS WAF. Defaults to `false`.
+        :param pulumi.Input[bool] enable_xff_client_port: Indicates whether the X-Forwarded-For header should preserve the source port that the client used to connect to the load balancer in `application` load balancers. Defaults to `true`.
         :param pulumi.Input[int] idle_timeout: The time in seconds that the connection is allowed to be idle. Only valid for Load Balancers of type `application`. Default: 60.
         :param pulumi.Input[bool] internal: If true, the LB will be internal.
-        :param pulumi.Input[str] ip_address_type: The type of IP addresses used by the subnets for your load balancer. The possible values are `ipv4` and `dualstack`
+        :param pulumi.Input[str] ip_address_type: The type of IP addresses used by the subnets for your load balancer. The possible values are `ipv4` and `dualstack`.
         :param pulumi.InputType['ListenerArgs'] listener: A listener to create. Only one of [listener] and [listeners] can be specified.
         :param Sequence[pulumi.InputType['ListenerArgs']] listeners: List of listeners to create. Only one of [listener] and [listeners] can be specified.
         :param pulumi.Input[str] name: The name of the LB. This name must be unique within your AWS account, can have a maximum of 32 characters,
                must contain only alphanumeric characters or hyphens, and must not begin or end with a hyphen. If not specified,
                this provider will autogenerate a name beginning with `tf-lb`.
         :param pulumi.Input[str] name_prefix: Creates a unique name beginning with the specified prefix. Conflicts with `name`.
         :param pulumi.Input[bool] preserve_host_header: Indicates whether the Application Load Balancer should preserve the Host header in the HTTP request and send it to the target without any change. Defaults to `false`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] security_groups: A list of security group IDs to assign to the LB. Only valid for Load Balancers of type `application`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] subnet_ids: A list of subnet IDs to attach to the LB. Subnets
                cannot be updated for Load Balancers of type `network`. Changing this value
                for load balancers of type `network` will force a recreation of the resource.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['pulumi_aws.lb.LoadBalancerSubnetMappingArgs']]]] subnet_mappings: A subnet mapping block as documented below.
         :param pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ec2.Subnet']]] subnets: A list of subnets to attach to the LB. Only one of [subnets], [subnetIds] or [subnetMappings] can be specified
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: A map of tags to assign to the resource. If configured with a provider `default_tags` configuration block present, tags with matching keys will overwrite those defined at the provider-level.
+        :param pulumi.Input[str] xff_header_processing_mode: Determines how the load balancer modifies the `X-Forwarded-For` header in the HTTP request before sending the request to the target. The possible values are `append`, `preserve`, and `remove`. Only valid for Load Balancers of type `application`. The default is `append`.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[ApplicationLoadBalancerArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -491,35 +543,35 @@
                  default_security_group: Optional[pulumi.InputType['_awsx.DefaultSecurityGroupArgs']] = None,
                  default_target_group: Optional[pulumi.InputType['TargetGroupArgs']] = None,
                  default_target_group_port: Optional[pulumi.Input[int]] = None,
                  desync_mitigation_mode: Optional[pulumi.Input[str]] = None,
                  drop_invalid_header_fields: Optional[pulumi.Input[bool]] = None,
                  enable_deletion_protection: Optional[pulumi.Input[bool]] = None,
                  enable_http2: Optional[pulumi.Input[bool]] = None,
+                 enable_tls_version_and_cipher_suite_headers: Optional[pulumi.Input[bool]] = None,
                  enable_waf_fail_open: Optional[pulumi.Input[bool]] = None,
+                 enable_xff_client_port: Optional[pulumi.Input[bool]] = None,
                  idle_timeout: Optional[pulumi.Input[int]] = None,
                  internal: Optional[pulumi.Input[bool]] = None,
                  ip_address_type: Optional[pulumi.Input[str]] = None,
                  listener: Optional[pulumi.InputType['ListenerArgs']] = None,
                  listeners: Optional[Sequence[pulumi.InputType['ListenerArgs']]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  name_prefix: Optional[pulumi.Input[str]] = None,
                  preserve_host_header: Optional[pulumi.Input[bool]] = None,
                  security_groups: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  subnet_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  subnet_mappings: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['pulumi_aws.lb.LoadBalancerSubnetMappingArgs']]]]] = None,
                  subnets: Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ec2.Subnet']]]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
+                 xff_header_processing_mode: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ApplicationLoadBalancerArgs.__new__(ApplicationLoadBalancerArgs)
 
@@ -528,28 +580,31 @@
             __props__.__dict__["default_security_group"] = default_security_group
             __props__.__dict__["default_target_group"] = default_target_group
             __props__.__dict__["default_target_group_port"] = default_target_group_port
             __props__.__dict__["desync_mitigation_mode"] = desync_mitigation_mode
             __props__.__dict__["drop_invalid_header_fields"] = drop_invalid_header_fields
             __props__.__dict__["enable_deletion_protection"] = enable_deletion_protection
             __props__.__dict__["enable_http2"] = enable_http2
+            __props__.__dict__["enable_tls_version_and_cipher_suite_headers"] = enable_tls_version_and_cipher_suite_headers
             __props__.__dict__["enable_waf_fail_open"] = enable_waf_fail_open
+            __props__.__dict__["enable_xff_client_port"] = enable_xff_client_port
             __props__.__dict__["idle_timeout"] = idle_timeout
             __props__.__dict__["internal"] = internal
             __props__.__dict__["ip_address_type"] = ip_address_type
             __props__.__dict__["listener"] = listener
             __props__.__dict__["listeners"] = listeners
             __props__.__dict__["name"] = name
             __props__.__dict__["name_prefix"] = name_prefix
             __props__.__dict__["preserve_host_header"] = preserve_host_header
             __props__.__dict__["security_groups"] = security_groups
             __props__.__dict__["subnet_ids"] = subnet_ids
             __props__.__dict__["subnet_mappings"] = subnet_mappings
             __props__.__dict__["subnets"] = subnets
             __props__.__dict__["tags"] = tags
+            __props__.__dict__["xff_header_processing_mode"] = xff_header_processing_mode
             __props__.__dict__["load_balancer"] = None
             __props__.__dict__["vpc_id"] = None
         super(ApplicationLoadBalancer, __self__).__init__(
             'awsx:lb:ApplicationLoadBalancer',
             resource_name,
             __props__,
             opts,
```

### Comparing `pulumi_awsx-1.0.2/pulumi_awsx/lb/target_group_attachment.py` & `pulumi_awsx-1.0.3/pulumi_awsx/lb/target_group_attachment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by pulumi-gen-awsx. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 import pulumi_aws
 
@@ -166,20 +167,17 @@
                  instance: Optional[pulumi.Input['pulumi_aws.ec2.Instance']] = None,
                  instance_id: Optional[pulumi.Input[str]] = None,
                  lambda_: Optional[pulumi.Input['pulumi_aws.lambda_.Function']] = None,
                  lambda_arn: Optional[pulumi.Input[str]] = None,
                  target_group: Optional[pulumi.Input['pulumi_aws.lb.TargetGroup']] = None,
                  target_group_arn: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = TargetGroupAttachmentArgs.__new__(TargetGroupAttachmentArgs)
```

### Comparing `pulumi_awsx-1.0.2/pulumi_awsx/provider.py` & `pulumi_awsx-1.0.3/pulumi_awsx/provider.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by pulumi-gen-awsx. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = ['ProviderArgs', 'Provider']
@@ -50,20 +51,17 @@
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ProviderArgs.__new__(ProviderArgs)
 
         super(Provider, __self__).__init__(
             'awsx',
```

### Comparing `pulumi_awsx-1.0.2/pulumi_awsx.egg-info/PKG-INFO` & `pulumi_awsx-1.0.3/pulumi_awsx.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,110 +1,110 @@
 Metadata-Version: 2.1
 Name: pulumi-awsx
-Version: 1.0.2
+Version: 1.0.3
 Summary: Pulumi Amazon Web Services (AWS) AWSX Components.
 Home-page: https://pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-awsx
-Description: [![Actions Status](https://github.com/pulumi/pulumi-awsx/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-awsx/actions)
-        [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
-        [![NPM version](https://badge.fury.io/js/%40pulumi%2Fawsx.svg)](https://www.npmjs.com/package/@pulumi/awsx)
-        [![Python version](https://badge.fury.io/py/pulumi-awsx.svg)](https://pypi.org/project/pulumi-awsx)
-        [![NuGet version](https://badge.fury.io/nu/pulumi.awsx.svg)](https://badge.fury.io/nu/pulumi.awsx)
-        [![PkgGoDev](https://pkg.go.dev/badge/github.com/pulumi/pulumi-awsx/sdk/go)](https://pkg.go.dev/github.com/pulumi/pulumi-awsx/sdk/go)
-        [![License](https://img.shields.io/npm/l/%40pulumi%2Fawsx.svg)](https://github.com/pulumi/pulumi-awsx/blob/master/LICENSE)
-        
-        ## Pulumi AWS Infrastructure Components
-        
-        Pulumi's framework for Amazon Web Services (AWS) infrastructure.
-        
-        To use this package, [install the Pulumi CLI](https://www.pulumi.com/docs/get-started/install/). For a streamlined Pulumi walkthrough, including language runtime installation and AWS configuration, see the [Crosswalk for AWS documentation](https://www.pulumi.com/docs/guides/crosswalk/aws/).
-        
-        The AWS Infrastructure package is intended to provide [component](https://www.pulumi.com/docs/intro/concepts/resources/components/) wrappers around many core AWS 'raw' resources to make them easier and more convenient to use.  In general, the `@pulumi/awsx` package mirrors the module structure of `@pulumi/aws` (i.e. `@pulumi/awsx/ecs` or `@pulumi/awsx/ec2`).  These [components](https://www.pulumi.com/docs/intro/concepts/resources/components/) are designed to take care of much of the redundancy and boilerplate necessary when using the raw AWS resources, while still striving to expose all underlying functionality if needed.
-        
-        The AWS Infrastructure package undergoes constant improvements and additions.  While we will strive to maintain backward compatability here, we will occasionally make breaks here as appropriate if it helps improve the overall quality of this package.
-        
-        The AWS Infrastructure package exposes many high level abstractions.  Including:
-        
-        * [`ec2`](https://github.com/pulumi/pulumi-awsx/blob/master/awsx/ec2).  A module that makes it easier to work with your AWS network, subnets, and security groups.  By default, the resources in the package follow the [AWS Best Practices](
-          https://aws.amazon.com/answers/networking/aws-single-vpc-design/), but can be configured as desired in whatever ways you want.  Most commonly, this package is used to acquire the default Vpc for a region (using `awsx.ec2.DefaultNetwork`).  However, it can also be used to easily create or augment an existing Vpc.
-        
-        * [`ecs`](https://github.com/pulumi/pulumi-awsx/blob/master/awsx/ecs).  A module that makes it easy to create and configure clusters, tasks and services for running containers. Convenience resources are created to make the common tasks of creating EC2 or Fargate services and tasks much simpler.
-        
-        * [`lb`](https://github.com/pulumi/pulumi-awsx/tree/master/awsx/lb).  A module for simply setting up [Elastic Load Balancing](https://aws.amazon.com/elasticloadbalancing/). This module provides convenient ways to set up either `Network` or `Application` load balancers, along with the appropriate ELB Target Groups and Listeners in order to have a high availability, automatically-scaled service.  These ELB components also work well with the other awsx components.  For example, an `lb.defaultTarget` can be passed in directly as the `portMapping` target of an `ecs.FargateService`.
-        
-        <div>
-            <a href="https://www.pulumi.com/docs/guides/crosswalk/aws/" title="Get Started">
-               <img src="https://www.pulumi.com/images/get-started.svg?" width="120">
-            </a>
-        </div>
-        
-        ## Installing
-        
-        This package is available in many languages in the standard packaging formats.
-        
-        ### Node.js (Java/TypeScript)
-        
-        To use from JavaScript or TypeScript in Node.js, install using either `npm`:
-        
-        ```bash
-        npm install @pulumi/awsx
-        ```
-        
-        or `yarn`:
-        
-        ```bash
-        yarn add @pulumi/awsx
-        ```
-        
-        ### Python
-        
-        To use from Python, install using `pip`:
-        
-        ```bash
-        pip install pulumi-awsx
-        ```
-        
-        ### Go
-        
-        To use from Go, use `go get` to grab the latest version of the library
-        
-        ```bash
-        go get github.com/pulumi/pulumi-awsx/sdk
-        ```
-        
-        ### .NET
-        
-        To use from .NET, install using `dotnet add package`:
-        
-        ```bash
-        dotnet add package Pulumi.Awsx
-        ```
-        
-        ## Configuration
-        
-        The configuration options available for this provider mirror those of the [Pulumi AWS Classic Provider](https://github.com/pulumi/pulumi-aws#configuration)
-        
-        ## Migration from 0.x to 1.0
-        
-        Before version 1, this package only supported components in TypeScript. All the existing components from the 0.x releases are now available in the `classic` namespace. The `classic` namespace will remain until the next major version release but will only receive updates for critical security fixes.
-        
-        1. Change references from `@pulumi/awsx` to `@pulumi/awsx/classic` to maintain existing behaviour.
-        2. Refactor to replace the classic components with the new top-level components.
-        
-        **Note:** The new top-level components (outside the `classic` namespace) may require additional code changes and resource re-creation.
-        
-        ### Notable changes
-        
-        - Removed ECS Cluster as this did not add any functionaly over the [AWS Classic ECS Cluster resource](https://www.pulumi.com/registry/packages/aws/api-docs/ecs/cluster/).
-        - Removed `Vpc.fromExistingIds()` as this was originally added because other components depended on the concrete VPC component class. The new components in v1 no longer have hard dependencies on other resources, so instead the subnets from the existing VPC can be passed into other components directly.
-        
-        ## References
-        
-        * [Tutorial](https://www.pulumi.com/blog/crosswalk-for-aws-1-0/)
-        * [API Reference Documentation](https://www.pulumi.com/registry/packages/awsx/api-docs/)
-        * [Examples](./examples)
-        * [Crosswalk for AWS Guide](https://www.pulumi.com/docs/guides/crosswalk/aws/)
-        
 Keywords: pulumi aws awsx kind/component category/cloud
-Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+
+[![Actions Status](https://github.com/pulumi/pulumi-awsx/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-awsx/actions)
+[![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
+[![NPM version](https://badge.fury.io/js/%40pulumi%2Fawsx.svg)](https://www.npmjs.com/package/@pulumi/awsx)
+[![Python version](https://badge.fury.io/py/pulumi-awsx.svg)](https://pypi.org/project/pulumi-awsx)
+[![NuGet version](https://badge.fury.io/nu/pulumi.awsx.svg)](https://badge.fury.io/nu/pulumi.awsx)
+[![PkgGoDev](https://pkg.go.dev/badge/github.com/pulumi/pulumi-awsx/sdk/go)](https://pkg.go.dev/github.com/pulumi/pulumi-awsx/sdk/go)
+[![License](https://img.shields.io/npm/l/%40pulumi%2Fawsx.svg)](https://github.com/pulumi/pulumi-awsx/blob/master/LICENSE)
+
+## Pulumi AWS Infrastructure Components
+
+Pulumi's framework for Amazon Web Services (AWS) infrastructure.
+
+To use this package, [install the Pulumi CLI](https://www.pulumi.com/docs/get-started/install/). For a streamlined Pulumi walkthrough, including language runtime installation and AWS configuration, see the [Crosswalk for AWS documentation](https://www.pulumi.com/docs/guides/crosswalk/aws/).
+
+The AWS Infrastructure package is intended to provide [component](https://www.pulumi.com/docs/intro/concepts/resources/components/) wrappers around many core AWS 'raw' resources to make them easier and more convenient to use.  In general, the `@pulumi/awsx` package mirrors the module structure of `@pulumi/aws` (i.e. `@pulumi/awsx/ecs` or `@pulumi/awsx/ec2`).  These [components](https://www.pulumi.com/docs/intro/concepts/resources/components/) are designed to take care of much of the redundancy and boilerplate necessary when using the raw AWS resources, while still striving to expose all underlying functionality if needed.
+
+The AWS Infrastructure package undergoes constant improvements and additions.  While we will strive to maintain backward compatability here, we will occasionally make breaks here as appropriate if it helps improve the overall quality of this package.
+
+The AWS Infrastructure package exposes many high level abstractions.  Including:
+
+* [`ec2`](https://github.com/pulumi/pulumi-awsx/blob/master/awsx/ec2).  A module that makes it easier to work with your AWS network, subnets, and security groups.  By default, the resources in the package follow the [AWS Best Practices](
+  https://aws.amazon.com/answers/networking/aws-single-vpc-design/), but can be configured as desired in whatever ways you want.  Most commonly, this package is used to acquire the default Vpc for a region (using `awsx.ec2.DefaultNetwork`).  However, it can also be used to easily create or augment an existing Vpc.
+
+* [`ecs`](https://github.com/pulumi/pulumi-awsx/blob/master/awsx/ecs).  A module that makes it easy to create and configure clusters, tasks and services for running containers. Convenience resources are created to make the common tasks of creating EC2 or Fargate services and tasks much simpler.
+
+* [`lb`](https://github.com/pulumi/pulumi-awsx/tree/master/awsx/lb).  A module for simply setting up [Elastic Load Balancing](https://aws.amazon.com/elasticloadbalancing/). This module provides convenient ways to set up either `Network` or `Application` load balancers, along with the appropriate ELB Target Groups and Listeners in order to have a high availability, automatically-scaled service.  These ELB components also work well with the other awsx components.  For example, an `lb.defaultTarget` can be passed in directly as the `portMapping` target of an `ecs.FargateService`.
+
+<div>
+    <a href="https://www.pulumi.com/docs/guides/crosswalk/aws/" title="Get Started">
+       <img src="https://www.pulumi.com/images/get-started.svg?" width="120">
+    </a>
+</div>
+
+## Installing
+
+This package is available in many languages in the standard packaging formats.
+
+### Node.js (Java/TypeScript)
+
+To use from JavaScript or TypeScript in Node.js, install using either `npm`:
+
+```bash
+npm install @pulumi/awsx
+```
+
+or `yarn`:
+
+```bash
+yarn add @pulumi/awsx
+```
+
+### Python
+
+To use from Python, install using `pip`:
+
+```bash
+pip install pulumi-awsx
+```
+
+### Go
+
+To use from Go, use `go get` to grab the latest version of the library
+
+```bash
+go get github.com/pulumi/pulumi-awsx/sdk
+```
+
+### .NET
+
+To use from .NET, install using `dotnet add package`:
+
+```bash
+dotnet add package Pulumi.Awsx
+```
+
+## Configuration
+
+The configuration options available for this provider mirror those of the [Pulumi AWS Classic Provider](https://github.com/pulumi/pulumi-aws#configuration)
+
+## Migration from 0.x to 1.0
+
+Before version 1, this package only supported components in TypeScript. All the existing components from the 0.x releases are now available in the `classic` namespace. The `classic` namespace will remain until the next major version release but will only receive updates for critical security fixes.
+
+1. Change references from `@pulumi/awsx` to `@pulumi/awsx/classic` to maintain existing behaviour.
+2. Refactor to replace the classic components with the new top-level components.
+
+**Note:** The new top-level components (outside the `classic` namespace) may require additional code changes and resource re-creation.
+
+### Notable changes
+
+- Removed ECS Cluster as this did not add any functionality over the [AWS Classic ECS Cluster resource](https://www.pulumi.com/registry/packages/aws/api-docs/ecs/cluster/).
+- Removed `Vpc.fromExistingIds()` as this was originally added because other components depended on the concrete VPC component class. The new components in v1 no longer have hard dependencies on other resources, so instead the subnets from the existing VPC can be passed into other components directly.
+
+## References
+
+* [Tutorial](https://www.pulumi.com/blog/crosswalk-for-aws-1-0/)
+* [API Reference Documentation](https://www.pulumi.com/registry/packages/awsx/api-docs/)
+* [Examples](./examples)
+* [Crosswalk for AWS Guide](https://www.pulumi.com/docs/guides/crosswalk/aws/)
```

#### html2text {}

```diff
@@ -1,14 +1,15 @@
-Metadata-Version: 2.1 Name: pulumi-awsx Version: 1.0.2 Summary: Pulumi Amazon
+Metadata-Version: 2.1 Name: pulumi-awsx Version: 1.0.3 Summary: Pulumi Amazon
 Web Services (AWS) AWSX Components. Home-page: https://pulumi.com License:
 Apache-2.0 Project-URL: Repository, https://github.com/pulumi/pulumi-awsx
-Description: [![Actions Status](https://github.com/pulumi/pulumi-awsx/
-workflows/master/badge.svg)](https://github.com/pulumi/pulumi-awsx/actions) [!
-[Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://
-slack.pulumi.com) [![NPM version](https://badge.fury.io/js/
+Keywords: pulumi aws awsx kind/component category/cloud Requires-Python: >=3.7
+Description-Content-Type: text/markdown [![Actions Status](https://github.com/
+pulumi/pulumi-awsx/workflows/master/badge.svg)](https://github.com/pulumi/
+pulumi-awsx/actions) [![Slack](http://www.pulumi.com/images/docs/badges/
+slack.svg)](https://slack.pulumi.com) [![NPM version](https://badge.fury.io/js/
 %40pulumi%2Fawsx.svg)](https://www.npmjs.com/package/@pulumi/awsx) [![Python
 version](https://badge.fury.io/py/pulumi-awsx.svg)](https://pypi.org/project/
 pulumi-awsx) [![NuGet version](https://badge.fury.io/nu/pulumi.awsx.svg)]
 (https://badge.fury.io/nu/pulumi.awsx) [![PkgGoDev](https://pkg.go.dev/badge/
 github.com/pulumi/pulumi-awsx/sdk/go)](https://pkg.go.dev/github.com/pulumi/
 pulumi-awsx/sdk/go) [![License](https://img.shields.io/npm/l/
 %40pulumi%2Fawsx.svg)](https://github.com/pulumi/pulumi-awsx/blob/master/
@@ -65,19 +66,17 @@
 0.x releases are now available in the `classic` namespace. The `classic`
 namespace will remain until the next major version release but will only
 receive updates for critical security fixes. 1. Change references from
 `@pulumi/awsx` to `@pulumi/awsx/classic` to maintain existing behaviour. 2.
 Refactor to replace the classic components with the new top-level components.
 **Note:** The new top-level components (outside the `classic` namespace) may
 require additional code changes and resource re-creation. ### Notable changes -
-Removed ECS Cluster as this did not add any functionaly over the [AWS Classic
+Removed ECS Cluster as this did not add any functionality over the [AWS Classic
 ECS Cluster resource](https://www.pulumi.com/registry/packages/aws/api-docs/
 ecs/cluster/). - Removed `Vpc.fromExistingIds()` as this was originally added
 because other components depended on the concrete VPC component class. The new
 components in v1 no longer have hard dependencies on other resources, so
 instead the subnets from the existing VPC can be passed into other components
 directly. ## References * [Tutorial](https://www.pulumi.com/blog/crosswalk-for-
 aws-1-0/) * [API Reference Documentation](https://www.pulumi.com/registry/
 packages/awsx/api-docs/) * [Examples](./examples) * [Crosswalk for AWS Guide]
-(https://www.pulumi.com/docs/guides/crosswalk/aws/) Keywords: pulumi aws awsx
-kind/component category/cloud Platform: UNKNOWN Description-Content-Type: text/
-markdown
+(https://www.pulumi.com/docs/guides/crosswalk/aws/)
```

### Comparing `pulumi_awsx-1.0.2/pulumi_awsx.egg-info/SOURCES.txt` & `pulumi_awsx-1.0.3/pulumi_awsx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-1.0.2/setup.py` & `pulumi_awsx-1.0.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "1.0.2"
-PLUGIN_VERSION = "1.0.2"
+VERSION = "1.0.3"
+PLUGIN_VERSION = "1.0.3"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'awsx', PLUGIN_VERSION])
         except OSError as error:
@@ -34,14 +34,15 @@
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "awsx Pulumi Package - Development Version"
 
 
 setup(name='pulumi_awsx',
+      python_requires='>=3.7',
       version=VERSION,
       description="Pulumi Amazon Web Services (AWS) AWSX Components.",
       long_description=readme(),
       long_description_content_type='text/markdown',
       cmdclass={
           'install': InstallPluginCommand,
       },
@@ -57,12 +58,12 @@
               'py.typed',
               'pulumi-plugin.json',
           ]
       },
       install_requires=[
           'parver>=0.2.1',
           'pulumi>=3.47.2,<4.0.0',
-          'pulumi-aws>=5.16.2,<6.0.0',
+          'pulumi-aws>=5.35.0,<6.0.0',
           'pulumi-docker>=3.6.1,<4.0.0',
           'semver>=2.8.1'
       ],
       zip_safe=False)
```

