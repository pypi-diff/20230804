# Comparing `tmp/pulumi_eks-1.1.0a1690710619.tar.gz` & `tmp/pulumi_eks-1.1.0a1691162979.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_eks-1.1.0a1690710619.tar", last modified: Sun Jul 30 09:58:32 2023, max compression
+gzip compressed data, was "pulumi_eks-1.1.0a1691162979.tar", last modified: Fri Aug  4 16:51:38 2023, max compression
```

## Comparing `pulumi_eks-1.1.0a1690710619.tar` & `pulumi_eks-1.1.0a1691162979.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 09:58:32.883986 pulumi_eks-1.1.0a1690710619/
--rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-07-30 09:58:32.883986 pulumi_eks-1.1.0a1690710619/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-07-30 09:58:32.000000 pulumi_eks-1.1.0a1690710619/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 09:58:32.883986 pulumi_eks-1.1.0a1690710619/pulumi_eks/
--rw-------   0 runner    (1001) docker     (123)     1150 2023-07-30 09:58:32.000000 pulumi_eks-1.1.0a1690710619/pulumi_eks/__init__.py
--rw-------   0 runner    (1001) docker     (123)    84186 2023-07-30 09:58:32.000000 pulumi_eks-1.1.0a1690710619/pulumi_eks/_inputs.py
--rw-------   0 runner    (1001) docker     (123)     8055 2023-07-30 09:58:32.000000 pulumi_eks-1.1.0a1690710619/pulumi_eks/_utilities.py
--rw-------   0 runner    (1001) docker     (123)    90114 2023-07-30 09:58:32.000000 pulumi_eks-1.1.0a1690710619/pulumi_eks/cluster.py
--rw-------   0 runner    (1001) docker     (123)     4860 2023-07-30 09:58:32.000000 pulumi_eks-1.1.0a1690710619/pulumi_eks/cluster_creation_role_provider.py
--rw-------   0 runner    (1001) docker     (123)    30218 2023-07-30 09:58:32.000000 pulumi_eks-1.1.0a1690710619/pulumi_eks/managed_node_group.py
--rw-------   0 runner    (1001) docker     (123)    45851 2023-07-30 09:58:32.000000 pulumi_eks-1.1.0a1690710619/pulumi_eks/node_group.py
--rw-------   0 runner    (1001) docker     (123)     8405 2023-07-30 09:58:32.000000 pulumi_eks-1.1.0a1690710619/pulumi_eks/node_group_security_group.py
--rw-------   0 runner    (1001) docker     (123)    48763 2023-07-30 09:58:32.000000 pulumi_eks-1.1.0a1690710619/pulumi_eks/node_group_v2.py
--rw-------   0 runner    (1001) docker     (123)    38606 2023-07-30 09:58:32.000000 pulumi_eks-1.1.0a1690710619/pulumi_eks/outputs.py
--rw-------   0 runner    (1001) docker     (123)     2715 2023-07-30 09:58:32.000000 pulumi_eks-1.1.0a1690710619/pulumi_eks/provider.py
--rw-------   0 runner    (1001) docker     (123)       40 2023-07-30 09:58:32.000000 pulumi_eks-1.1.0a1690710619/pulumi_eks/pulumi-plugin.json
--rw-------   0 runner    (1001) docker     (123)        0 2023-07-30 09:58:32.000000 pulumi_eks-1.1.0a1690710619/pulumi_eks/py.typed
--rw-------   0 runner    (1001) docker     (123)    37656 2023-07-30 09:58:32.000000 pulumi_eks-1.1.0a1690710619/pulumi_eks/vpc_cni.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 09:58:32.883986 pulumi_eks-1.1.0a1690710619/pulumi_eks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-07-30 09:58:32.000000 pulumi_eks-1.1.0a1690710619/pulumi_eks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-30 09:58:32.000000 pulumi_eks-1.1.0a1690710619/pulumi_eks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 09:58:32.000000 pulumi_eks-1.1.0a1690710619/pulumi_eks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 09:58:32.000000 pulumi_eks-1.1.0a1690710619/pulumi_eks.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-30 09:58:32.000000 pulumi_eks-1.1.0a1690710619/pulumi_eks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-30 09:58:32.000000 pulumi_eks-1.1.0a1690710619/pulumi_eks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 09:58:32.883986 pulumi_eks-1.1.0a1690710619/setup.cfg
--rw-------   0 runner    (1001) docker     (123)     2175 2023-07-30 09:58:32.000000 pulumi_eks-1.1.0a1690710619/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:51:38.743485 pulumi_eks-1.1.0a1691162979/
+-rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-08-04 16:51:38.743485 pulumi_eks-1.1.0a1691162979/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-08-04 16:51:38.000000 pulumi_eks-1.1.0a1691162979/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:51:38.739485 pulumi_eks-1.1.0a1691162979/pulumi_eks/
+-rw-------   0 runner    (1001) docker     (123)     1150 2023-08-04 16:51:38.000000 pulumi_eks-1.1.0a1691162979/pulumi_eks/__init__.py
+-rw-------   0 runner    (1001) docker     (123)    84186 2023-08-04 16:51:38.000000 pulumi_eks-1.1.0a1691162979/pulumi_eks/_inputs.py
+-rw-------   0 runner    (1001) docker     (123)     8055 2023-08-04 16:51:38.000000 pulumi_eks-1.1.0a1691162979/pulumi_eks/_utilities.py
+-rw-------   0 runner    (1001) docker     (123)    90114 2023-08-04 16:51:38.000000 pulumi_eks-1.1.0a1691162979/pulumi_eks/cluster.py
+-rw-------   0 runner    (1001) docker     (123)     4860 2023-08-04 16:51:38.000000 pulumi_eks-1.1.0a1691162979/pulumi_eks/cluster_creation_role_provider.py
+-rw-------   0 runner    (1001) docker     (123)    30218 2023-08-04 16:51:38.000000 pulumi_eks-1.1.0a1691162979/pulumi_eks/managed_node_group.py
+-rw-------   0 runner    (1001) docker     (123)    45851 2023-08-04 16:51:38.000000 pulumi_eks-1.1.0a1691162979/pulumi_eks/node_group.py
+-rw-------   0 runner    (1001) docker     (123)     8405 2023-08-04 16:51:38.000000 pulumi_eks-1.1.0a1691162979/pulumi_eks/node_group_security_group.py
+-rw-------   0 runner    (1001) docker     (123)    48763 2023-08-04 16:51:38.000000 pulumi_eks-1.1.0a1691162979/pulumi_eks/node_group_v2.py
+-rw-------   0 runner    (1001) docker     (123)    38606 2023-08-04 16:51:38.000000 pulumi_eks-1.1.0a1691162979/pulumi_eks/outputs.py
+-rw-------   0 runner    (1001) docker     (123)     2715 2023-08-04 16:51:38.000000 pulumi_eks-1.1.0a1691162979/pulumi_eks/provider.py
+-rw-------   0 runner    (1001) docker     (123)       40 2023-08-04 16:51:38.000000 pulumi_eks-1.1.0a1691162979/pulumi_eks/pulumi-plugin.json
+-rw-------   0 runner    (1001) docker     (123)        0 2023-08-04 16:51:38.000000 pulumi_eks-1.1.0a1691162979/pulumi_eks/py.typed
+-rw-------   0 runner    (1001) docker     (123)    37656 2023-08-04 16:51:38.000000 pulumi_eks-1.1.0a1691162979/pulumi_eks/vpc_cni.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:51:38.743485 pulumi_eks-1.1.0a1691162979/pulumi_eks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-08-04 16:51:38.000000 pulumi_eks-1.1.0a1691162979/pulumi_eks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-08-04 16:51:38.000000 pulumi_eks-1.1.0a1691162979/pulumi_eks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 16:51:38.000000 pulumi_eks-1.1.0a1691162979/pulumi_eks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 16:51:38.000000 pulumi_eks-1.1.0a1691162979/pulumi_eks.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-04 16:51:38.000000 pulumi_eks-1.1.0a1691162979/pulumi_eks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-04 16:51:38.000000 pulumi_eks-1.1.0a1691162979/pulumi_eks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 16:51:38.743485 pulumi_eks-1.1.0a1691162979/setup.cfg
+-rw-------   0 runner    (1001) docker     (123)     2175 2023-08-04 16:51:38.000000 pulumi_eks-1.1.0a1691162979/setup.py
```

### Comparing `pulumi_eks-1.1.0a1690710619/PKG-INFO` & `pulumi_eks-1.1.0a1691162979/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_eks
-Version: 1.1.0a1690710619
+Version: 1.1.0a1691162979
 Summary: Pulumi Amazon Web Services (AWS) EKS Components.
 Home-page: https://pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-eks
 Description: [![Build Status](https://github.com/pulumi/pulumi-eks/actions/workflows/master.yml/badge.svg)](https://github.com/pulumi/pulumi-eks/actions/workflows/master.yml)
         [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
         [![npm version](https://badge.fury.io/js/@pulumi%2Feks.svg)](https://badge.fury.io/js/@pulumi%2Feks)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pulumi_eks Version: 1.1.0a1690710619 Summary:
+Metadata-Version: 2.1 Name: pulumi_eks Version: 1.1.0a1691162979 Summary:
 Pulumi Amazon Web Services (AWS) EKS Components. Home-page: https://pulumi.com
 License: Apache-2.0 Project-URL: Repository, https://github.com/pulumi/pulumi-
 eks Description: [![Build Status](https://github.com/pulumi/pulumi-eks/actions/
 workflows/master.yml/badge.svg)](https://github.com/pulumi/pulumi-eks/actions/
 workflows/master.yml) [![Slack](http://www.pulumi.com/images/docs/badges/
 slack.svg)](https://slack.pulumi.com) [![npm version](https://badge.fury.io/js/
 @pulumi%2Feks.svg)](https://badge.fury.io/js/@pulumi%2Feks) [![Python version]
```

### Comparing `pulumi_eks-1.1.0a1690710619/README.md` & `pulumi_eks-1.1.0a1691162979/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_eks-1.1.0a1690710619/pulumi_eks/__init__.py` & `pulumi_eks-1.1.0a1691162979/pulumi_eks/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_eks-1.1.0a1690710619/pulumi_eks/_inputs.py` & `pulumi_eks-1.1.0a1691162979/pulumi_eks/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_eks-1.1.0a1690710619/pulumi_eks/_utilities.py` & `pulumi_eks-1.1.0a1691162979/pulumi_eks/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_eks-1.1.0a1690710619/pulumi_eks/cluster.py` & `pulumi_eks-1.1.0a1691162979/pulumi_eks/cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_eks-1.1.0a1690710619/pulumi_eks/cluster_creation_role_provider.py` & `pulumi_eks-1.1.0a1691162979/pulumi_eks/cluster_creation_role_provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_eks-1.1.0a1690710619/pulumi_eks/managed_node_group.py` & `pulumi_eks-1.1.0a1691162979/pulumi_eks/managed_node_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_eks-1.1.0a1690710619/pulumi_eks/node_group.py` & `pulumi_eks-1.1.0a1691162979/pulumi_eks/node_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_eks-1.1.0a1690710619/pulumi_eks/node_group_security_group.py` & `pulumi_eks-1.1.0a1691162979/pulumi_eks/node_group_security_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_eks-1.1.0a1690710619/pulumi_eks/node_group_v2.py` & `pulumi_eks-1.1.0a1691162979/pulumi_eks/node_group_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_eks-1.1.0a1690710619/pulumi_eks/outputs.py` & `pulumi_eks-1.1.0a1691162979/pulumi_eks/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_eks-1.1.0a1690710619/pulumi_eks/provider.py` & `pulumi_eks-1.1.0a1691162979/pulumi_eks/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_eks-1.1.0a1690710619/pulumi_eks/vpc_cni.py` & `pulumi_eks-1.1.0a1691162979/pulumi_eks/vpc_cni.py`

 * *Files identical despite different names*

### Comparing `pulumi_eks-1.1.0a1690710619/pulumi_eks.egg-info/PKG-INFO` & `pulumi_eks-1.1.0a1691162979/pulumi_eks.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-eks
-Version: 1.1.0a1690710619
+Version: 1.1.0a1691162979
 Summary: Pulumi Amazon Web Services (AWS) EKS Components.
 Home-page: https://pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-eks
 Description: [![Build Status](https://github.com/pulumi/pulumi-eks/actions/workflows/master.yml/badge.svg)](https://github.com/pulumi/pulumi-eks/actions/workflows/master.yml)
         [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
         [![npm version](https://badge.fury.io/js/@pulumi%2Feks.svg)](https://badge.fury.io/js/@pulumi%2Feks)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pulumi-eks Version: 1.1.0a1690710619 Summary:
+Metadata-Version: 2.1 Name: pulumi-eks Version: 1.1.0a1691162979 Summary:
 Pulumi Amazon Web Services (AWS) EKS Components. Home-page: https://pulumi.com
 License: Apache-2.0 Project-URL: Repository, https://github.com/pulumi/pulumi-
 eks Description: [![Build Status](https://github.com/pulumi/pulumi-eks/actions/
 workflows/master.yml/badge.svg)](https://github.com/pulumi/pulumi-eks/actions/
 workflows/master.yml) [![Slack](http://www.pulumi.com/images/docs/badges/
 slack.svg)](https://slack.pulumi.com) [![npm version](https://badge.fury.io/js/
 @pulumi%2Feks.svg)](https://badge.fury.io/js/@pulumi%2Feks) [![Python version]
```

### Comparing `pulumi_eks-1.1.0a1690710619/pulumi_eks.egg-info/SOURCES.txt` & `pulumi_eks-1.1.0a1691162979/pulumi_eks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_eks-1.1.0a1690710619/setup.py` & `pulumi_eks-1.1.0a1691162979/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "1.1.0a1690710619"
-PLUGIN_VERSION = "1.1.0-alpha.1690710619+4ff430d0"
+VERSION = "1.1.0a1691162979"
+PLUGIN_VERSION = "1.1.0-alpha.1691162979+6e8c6415"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'eks', PLUGIN_VERSION])
         except OSError as error:
```

