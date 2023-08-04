# Comparing `tmp/types-aiobotocore-elb-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-elb-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-elb-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:16 2023, max compression
+gzip compressed data, was "types-aiobotocore-elb-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:52 2023, max compression
```

## Comparing `types-aiobotocore-elb-2.5.2.post1.tar` & `types-aiobotocore-elb-2.5.2.post2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:16.653589 types-aiobotocore-elb-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:38:18.000000 types-aiobotocore-elb-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17478 2023-08-02 14:52:16.653589 types-aiobotocore-elb-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15959 2023-08-02 14:38:18.000000 types-aiobotocore-elb-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:16.653589 types-aiobotocore-elb-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-08-02 14:38:18.000000 types-aiobotocore-elb-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:16.653589 types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb/
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-08-02 14:38:18.000000 types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-08-02 14:38:18.000000 types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-08-02 14:38:18.000000 types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26730 2023-08-02 14:38:18.000000 types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    26687 2023-08-02 14:38:18.000000 types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-08-02 14:38:18.000000 types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-08-02 14:38:18.000000 types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-08-02 14:38:18.000000 types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-08-02 14:38:18.000000 types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:18.000000 types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    25207 2023-08-02 14:38:20.000000 types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25184 2023-08-02 14:38:20.000000 types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:38:18.000000 types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-08-02 14:38:18.000000 types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-08-02 14:38:18.000000 types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:16.653589 types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17478 2023-08-02 14:52:16.000000 types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-02 14:52:16.000000 types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:16.000000 types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:16.000000 types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:16.000000 types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 14:52:16.000000 types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:52.564148 types-aiobotocore-elb-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:45:46.000000 types-aiobotocore-elb-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14111 2023-08-04 12:00:52.564148 types-aiobotocore-elb-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12592 2023-08-04 11:45:46.000000 types-aiobotocore-elb-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:52.564148 types-aiobotocore-elb-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-08-04 11:45:46.000000 types-aiobotocore-elb-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:52.564148 types-aiobotocore-elb-2.5.2.post2/types_aiobotocore_elb/
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-08-04 11:45:46.000000 types-aiobotocore-elb-2.5.2.post2/types_aiobotocore_elb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-08-04 11:45:46.000000 types-aiobotocore-elb-2.5.2.post2/types_aiobotocore_elb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-08-04 11:45:46.000000 types-aiobotocore-elb-2.5.2.post2/types_aiobotocore_elb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26720 2023-08-04 11:45:47.000000 types-aiobotocore-elb-2.5.2.post2/types_aiobotocore_elb/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26677 2023-08-04 11:45:46.000000 types-aiobotocore-elb-2.5.2.post2/types_aiobotocore_elb/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-08-04 11:45:47.000000 types-aiobotocore-elb-2.5.2.post2/types_aiobotocore_elb/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-08-04 11:45:47.000000 types-aiobotocore-elb-2.5.2.post2/types_aiobotocore_elb/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-08-04 11:45:47.000000 types-aiobotocore-elb-2.5.2.post2/types_aiobotocore_elb/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-08-04 11:45:47.000000 types-aiobotocore-elb-2.5.2.post2/types_aiobotocore_elb/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:45:46.000000 types-aiobotocore-elb-2.5.2.post2/types_aiobotocore_elb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    24573 2023-08-04 11:45:49.000000 types-aiobotocore-elb-2.5.2.post2/types_aiobotocore_elb/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24550 2023-08-04 11:45:48.000000 types-aiobotocore-elb-2.5.2.post2/types_aiobotocore_elb/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:45:46.000000 types-aiobotocore-elb-2.5.2.post2/types_aiobotocore_elb/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-08-04 11:45:47.000000 types-aiobotocore-elb-2.5.2.post2/types_aiobotocore_elb/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-08-04 11:45:47.000000 types-aiobotocore-elb-2.5.2.post2/types_aiobotocore_elb/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:52.564148 types-aiobotocore-elb-2.5.2.post2/types_aiobotocore_elb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14111 2023-08-04 12:00:52.000000 types-aiobotocore-elb-2.5.2.post2/types_aiobotocore_elb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-04 12:00:52.000000 types-aiobotocore-elb-2.5.2.post2/types_aiobotocore_elb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:52.000000 types-aiobotocore-elb-2.5.2.post2/types_aiobotocore_elb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:52.000000 types-aiobotocore-elb-2.5.2.post2/types_aiobotocore_elb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:52.000000 types-aiobotocore-elb-2.5.2.post2/types_aiobotocore_elb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 12:00:52.000000 types-aiobotocore-elb-2.5.2.post2/types_aiobotocore_elb.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-elb-2.5.2.post1/LICENSE` & `types-aiobotocore-elb-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elb-2.5.2.post1/README.md` & `types-aiobotocore-elb-2.5.2.post2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-elb
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.ElasticLoadBalancing 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elb/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore elb type-annotations botocore mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="types-aiobotocore-elb"></a>
 
 # types-aiobotocore-elb
 
 [![PyPI - types-aiobotocore-elb](https://img.shields.io/pypi/v/types-aiobotocore-elb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-elb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elb)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elb/)
@@ -15,15 +47,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.17.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [types-aiobotocore](https://pypi.org/project/types-aiobotocore/) page and in
 [types-aiobotocore-elb docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -297,126 +329,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_elb.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
+Full list of `ElasticLoadBalancing` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elb/literals/).
+
 ```python
-from types_aiobotocore_elb.literals import (
-    AnyInstanceInServiceWaiterName,
-    DescribeAccountLimitsPaginatorName,
-    DescribeLoadBalancersPaginatorName,
-    InstanceDeregisteredWaiterName,
-    InstanceInServiceWaiterName,
-    ElasticLoadBalancingServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    WaiterName,
-    RegionName,
-)
+from types_aiobotocore_elb.literals import AnyInstanceInServiceWaiterName
 
 
 def check_value(value: AnyInstanceInServiceWaiterName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_elb.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `ElasticLoadBalancing` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elb/type_defs/).
+
 ```python
-from types_aiobotocore_elb.type_defs import (
-    AccessLogTypeDef,
-    AddAvailabilityZonesInputRequestTypeDef,
-    ResponseMetadataTypeDef,
-    TagTypeDef,
-    AdditionalAttributeTypeDef,
-    AppCookieStickinessPolicyTypeDef,
-    ApplySecurityGroupsToLoadBalancerInputRequestTypeDef,
-    AttachLoadBalancerToSubnetsInputRequestTypeDef,
-    BackendServerDescriptionTypeDef,
-    HealthCheckTypeDef,
-    ConnectionDrainingTypeDef,
-    ConnectionSettingsTypeDef,
-    ListenerTypeDef,
-    CreateAppCookieStickinessPolicyInputRequestTypeDef,
-    CreateLBCookieStickinessPolicyInputRequestTypeDef,
-    PolicyAttributeTypeDef,
-    CrossZoneLoadBalancingTypeDef,
-    DeleteAccessPointInputRequestTypeDef,
-    DeleteLoadBalancerListenerInputRequestTypeDef,
-    DeleteLoadBalancerPolicyInputRequestTypeDef,
-    InstanceTypeDef,
-    PaginatorConfigTypeDef,
-    DescribeAccessPointsInputRequestTypeDef,
-    DescribeAccountLimitsInputRequestTypeDef,
-    LimitTypeDef,
-    WaiterConfigTypeDef,
-    InstanceStateTypeDef,
-    DescribeLoadBalancerAttributesInputRequestTypeDef,
-    DescribeLoadBalancerPoliciesInputRequestTypeDef,
-    DescribeLoadBalancerPolicyTypesInputRequestTypeDef,
-    DescribeTagsInputRequestTypeDef,
-    DetachLoadBalancerFromSubnetsInputRequestTypeDef,
-    LBCookieStickinessPolicyTypeDef,
-    SourceSecurityGroupTypeDef,
-    PolicyAttributeDescriptionTypeDef,
-    PolicyAttributeTypeDescriptionTypeDef,
-    RemoveAvailabilityZonesInputRequestTypeDef,
-    TagKeyOnlyTypeDef,
-    SetLoadBalancerListenerSSLCertificateInputRequestTypeDef,
-    SetLoadBalancerPoliciesForBackendServerInputRequestTypeDef,
-    SetLoadBalancerPoliciesOfListenerInputRequestTypeDef,
-    AddAvailabilityZonesOutputTypeDef,
-    ApplySecurityGroupsToLoadBalancerOutputTypeDef,
-    AttachLoadBalancerToSubnetsOutputTypeDef,
-    CreateAccessPointOutputTypeDef,
-    DetachLoadBalancerFromSubnetsOutputTypeDef,
-    RemoveAvailabilityZonesOutputTypeDef,
-    AddTagsInputRequestTypeDef,
-    TagDescriptionTypeDef,
-    ConfigureHealthCheckInputRequestTypeDef,
-    ConfigureHealthCheckOutputTypeDef,
-    CreateAccessPointInputRequestTypeDef,
-    CreateLoadBalancerListenerInputRequestTypeDef,
-    ListenerDescriptionTypeDef,
-    CreateLoadBalancerPolicyInputRequestTypeDef,
-    LoadBalancerAttributesOutputTypeDef,
-    LoadBalancerAttributesTypeDef,
-    DeregisterEndPointsInputRequestTypeDef,
-    DeregisterEndPointsOutputTypeDef,
-    DescribeEndPointStateInputRequestTypeDef,
-    RegisterEndPointsInputRequestTypeDef,
-    RegisterEndPointsOutputTypeDef,
-    DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef,
-    DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef,
-    DescribeAccountLimitsOutputTypeDef,
-    DescribeEndPointStateInputAnyInstanceInServiceWaitTypeDef,
-    DescribeEndPointStateInputInstanceDeregisteredWaitTypeDef,
-    DescribeEndPointStateInputInstanceInServiceWaitTypeDef,
-    DescribeEndPointStateOutputTypeDef,
-    PoliciesTypeDef,
-    PolicyDescriptionTypeDef,
-    PolicyTypeDescriptionTypeDef,
-    RemoveTagsInputRequestTypeDef,
-    DescribeTagsOutputTypeDef,
-    DescribeLoadBalancerAttributesOutputTypeDef,
-    ModifyLoadBalancerAttributesOutputTypeDef,
-    LoadBalancerAttributesUnionTypeDef,
-    ModifyLoadBalancerAttributesInputRequestTypeDef,
-    LoadBalancerDescriptionTypeDef,
-    DescribeLoadBalancerPoliciesOutputTypeDef,
-    DescribeLoadBalancerPolicyTypesOutputTypeDef,
-    DescribeAccessPointsOutputTypeDef,
-)
+from types_aiobotocore_elb.type_defs import AccessLogTypeDef
 
 
 def get_value() -> AccessLogTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-elb-2.5.2.post1/setup.py` & `types-aiobotocore-elb-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-elb",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_elb"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ElasticLoadBalancing 2.5.2 service generated with"
-        " mypy-boto3-builder 7.17.1"
+        " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

### Comparing `types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb/__init__.py` & `types-aiobotocore-elb-2.5.2.post2/types_aiobotocore_elb/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb/__init__.pyi` & `types-aiobotocore-elb-2.5.2.post2/types_aiobotocore_elb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb/__main__.py` & `types-aiobotocore-elb-2.5.2.post2/types_aiobotocore_elb/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.ElasticLoadBalancing 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elb//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("2.5.2.post1")
+    print("2.5.2.post2")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb/client.py` & `types-aiobotocore-elb-2.5.2.post2/types_aiobotocore_elb/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     DescribeLoadBalancerPoliciesOutputTypeDef,
     DescribeLoadBalancerPolicyTypesOutputTypeDef,
     DescribeTagsOutputTypeDef,
     DetachLoadBalancerFromSubnetsOutputTypeDef,
     HealthCheckTypeDef,
     InstanceTypeDef,
     ListenerTypeDef,
-    LoadBalancerAttributesUnionTypeDef,
+    LoadBalancerAttributesTypeDef,
     ModifyLoadBalancerAttributesOutputTypeDef,
     PolicyAttributeTypeDef,
     RegisterEndPointsOutputTypeDef,
     RemoveAvailabilityZonesOutputTypeDef,
     TagKeyOnlyTypeDef,
     TagTypeDef,
 )
@@ -386,15 +386,15 @@
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elb/client/#generate_presigned_url)
         """
 
     async def modify_load_balancer_attributes(
-        self, *, LoadBalancerName: str, LoadBalancerAttributes: LoadBalancerAttributesUnionTypeDef
+        self, *, LoadBalancerName: str, LoadBalancerAttributes: LoadBalancerAttributesTypeDef
     ) -> ModifyLoadBalancerAttributesOutputTypeDef:
         """
         Modifies the attributes of the specified load balancer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing.Client.modify_load_balancer_attributes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elb/client/#modify_load_balancer_attributes)
         """
```

### Comparing `types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb/client.pyi` & `types-aiobotocore-elb-2.5.2.post2/types_aiobotocore_elb/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     DescribeLoadBalancerPoliciesOutputTypeDef,
     DescribeLoadBalancerPolicyTypesOutputTypeDef,
     DescribeTagsOutputTypeDef,
     DetachLoadBalancerFromSubnetsOutputTypeDef,
     HealthCheckTypeDef,
     InstanceTypeDef,
     ListenerTypeDef,
-    LoadBalancerAttributesUnionTypeDef,
+    LoadBalancerAttributesTypeDef,
     ModifyLoadBalancerAttributesOutputTypeDef,
     PolicyAttributeTypeDef,
     RegisterEndPointsOutputTypeDef,
     RemoveAvailabilityZonesOutputTypeDef,
     TagKeyOnlyTypeDef,
     TagTypeDef,
 )
@@ -355,15 +355,15 @@
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elb/client/#generate_presigned_url)
         """
     async def modify_load_balancer_attributes(
-        self, *, LoadBalancerName: str, LoadBalancerAttributes: LoadBalancerAttributesUnionTypeDef
+        self, *, LoadBalancerName: str, LoadBalancerAttributes: LoadBalancerAttributesTypeDef
     ) -> ModifyLoadBalancerAttributesOutputTypeDef:
         """
         Modifies the attributes of the specified load balancer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#ElasticLoadBalancing.Client.modify_load_balancer_attributes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elb/client/#modify_load_balancer_attributes)
         """
```

### Comparing `types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb/literals.py` & `types-aiobotocore-elb-2.5.2.post2/types_aiobotocore_elb/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb/literals.pyi` & `types-aiobotocore-elb-2.5.2.post2/types_aiobotocore_elb/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb/paginator.py` & `types-aiobotocore-elb-2.5.2.post2/types_aiobotocore_elb/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb/paginator.pyi` & `types-aiobotocore-elb-2.5.2.post2/types_aiobotocore_elb/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb/type_defs.py` & `types-aiobotocore-elb-2.5.2.post2/types_aiobotocore_elb/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_elb.type_defs import AccessLogTypeDef
 
     data: AccessLogTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Sequence
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
@@ -73,15 +73,14 @@
     "TagDescriptionTypeDef",
     "ConfigureHealthCheckInputRequestTypeDef",
     "ConfigureHealthCheckOutputTypeDef",
     "CreateAccessPointInputRequestTypeDef",
     "CreateLoadBalancerListenerInputRequestTypeDef",
     "ListenerDescriptionTypeDef",
     "CreateLoadBalancerPolicyInputRequestTypeDef",
-    "LoadBalancerAttributesOutputTypeDef",
     "LoadBalancerAttributesTypeDef",
     "DeregisterEndPointsInputRequestTypeDef",
     "DeregisterEndPointsOutputTypeDef",
     "DescribeEndPointStateInputRequestTypeDef",
     "RegisterEndPointsInputRequestTypeDef",
     "RegisterEndPointsOutputTypeDef",
     "DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef",
@@ -93,17 +92,16 @@
     "DescribeEndPointStateOutputTypeDef",
     "PoliciesTypeDef",
     "PolicyDescriptionTypeDef",
     "PolicyTypeDescriptionTypeDef",
     "RemoveTagsInputRequestTypeDef",
     "DescribeTagsOutputTypeDef",
     "DescribeLoadBalancerAttributesOutputTypeDef",
-    "ModifyLoadBalancerAttributesOutputTypeDef",
-    "LoadBalancerAttributesUnionTypeDef",
     "ModifyLoadBalancerAttributesInputRequestTypeDef",
+    "ModifyLoadBalancerAttributesOutputTypeDef",
     "LoadBalancerDescriptionTypeDef",
     "DescribeLoadBalancerPoliciesOutputTypeDef",
     "DescribeLoadBalancerPolicyTypesOutputTypeDef",
     "DescribeAccessPointsOutputTypeDef",
 )
 
 _RequiredAccessLogTypeDef = TypedDict(
@@ -671,34 +669,22 @@
 class CreateLoadBalancerPolicyInputRequestTypeDef(
     _RequiredCreateLoadBalancerPolicyInputRequestTypeDef,
     _OptionalCreateLoadBalancerPolicyInputRequestTypeDef,
 ):
     pass
 
 
-LoadBalancerAttributesOutputTypeDef = TypedDict(
-    "LoadBalancerAttributesOutputTypeDef",
-    {
-        "CrossZoneLoadBalancing": CrossZoneLoadBalancingTypeDef,
-        "AccessLog": AccessLogTypeDef,
-        "ConnectionDraining": ConnectionDrainingTypeDef,
-        "ConnectionSettings": ConnectionSettingsTypeDef,
-        "AdditionalAttributes": List[AdditionalAttributeTypeDef],
-    },
-    total=False,
-)
-
 LoadBalancerAttributesTypeDef = TypedDict(
     "LoadBalancerAttributesTypeDef",
     {
         "CrossZoneLoadBalancing": CrossZoneLoadBalancingTypeDef,
         "AccessLog": AccessLogTypeDef,
         "ConnectionDraining": ConnectionDrainingTypeDef,
         "ConnectionSettings": ConnectionSettingsTypeDef,
-        "AdditionalAttributes": Sequence[AdditionalAttributeTypeDef],
+        "AdditionalAttributes": List[AdditionalAttributeTypeDef],
     },
     total=False,
 )
 
 DeregisterEndPointsInputRequestTypeDef = TypedDict(
     "DeregisterEndPointsInputRequestTypeDef",
     {
@@ -901,36 +887,33 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeLoadBalancerAttributesOutputTypeDef = TypedDict(
     "DescribeLoadBalancerAttributesOutputTypeDef",
     {
-        "LoadBalancerAttributes": LoadBalancerAttributesOutputTypeDef,
+        "LoadBalancerAttributes": LoadBalancerAttributesTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ModifyLoadBalancerAttributesOutputTypeDef = TypedDict(
-    "ModifyLoadBalancerAttributesOutputTypeDef",
+ModifyLoadBalancerAttributesInputRequestTypeDef = TypedDict(
+    "ModifyLoadBalancerAttributesInputRequestTypeDef",
     {
         "LoadBalancerName": str,
-        "LoadBalancerAttributes": LoadBalancerAttributesOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "LoadBalancerAttributes": LoadBalancerAttributesTypeDef,
     },
 )
 
-LoadBalancerAttributesUnionTypeDef = Union[
-    LoadBalancerAttributesTypeDef, LoadBalancerAttributesOutputTypeDef
-]
-ModifyLoadBalancerAttributesInputRequestTypeDef = TypedDict(
-    "ModifyLoadBalancerAttributesInputRequestTypeDef",
+ModifyLoadBalancerAttributesOutputTypeDef = TypedDict(
+    "ModifyLoadBalancerAttributesOutputTypeDef",
     {
         "LoadBalancerName": str,
         "LoadBalancerAttributes": LoadBalancerAttributesTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LoadBalancerDescriptionTypeDef = TypedDict(
     "LoadBalancerDescriptionTypeDef",
     {
         "LoadBalancerName": str,
```

### Comparing `types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb/type_defs.pyi` & `types-aiobotocore-elb-2.5.2.post2/types_aiobotocore_elb/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_elb.type_defs import AccessLogTypeDef
 
     data: AccessLogTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Sequence
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
@@ -72,15 +72,14 @@
     "TagDescriptionTypeDef",
     "ConfigureHealthCheckInputRequestTypeDef",
     "ConfigureHealthCheckOutputTypeDef",
     "CreateAccessPointInputRequestTypeDef",
     "CreateLoadBalancerListenerInputRequestTypeDef",
     "ListenerDescriptionTypeDef",
     "CreateLoadBalancerPolicyInputRequestTypeDef",
-    "LoadBalancerAttributesOutputTypeDef",
     "LoadBalancerAttributesTypeDef",
     "DeregisterEndPointsInputRequestTypeDef",
     "DeregisterEndPointsOutputTypeDef",
     "DescribeEndPointStateInputRequestTypeDef",
     "RegisterEndPointsInputRequestTypeDef",
     "RegisterEndPointsOutputTypeDef",
     "DescribeAccessPointsInputDescribeLoadBalancersPaginateTypeDef",
@@ -92,17 +91,16 @@
     "DescribeEndPointStateOutputTypeDef",
     "PoliciesTypeDef",
     "PolicyDescriptionTypeDef",
     "PolicyTypeDescriptionTypeDef",
     "RemoveTagsInputRequestTypeDef",
     "DescribeTagsOutputTypeDef",
     "DescribeLoadBalancerAttributesOutputTypeDef",
-    "ModifyLoadBalancerAttributesOutputTypeDef",
-    "LoadBalancerAttributesUnionTypeDef",
     "ModifyLoadBalancerAttributesInputRequestTypeDef",
+    "ModifyLoadBalancerAttributesOutputTypeDef",
     "LoadBalancerDescriptionTypeDef",
     "DescribeLoadBalancerPoliciesOutputTypeDef",
     "DescribeLoadBalancerPolicyTypesOutputTypeDef",
     "DescribeAccessPointsOutputTypeDef",
 )
 
 _RequiredAccessLogTypeDef = TypedDict(
@@ -656,34 +654,22 @@
 
 class CreateLoadBalancerPolicyInputRequestTypeDef(
     _RequiredCreateLoadBalancerPolicyInputRequestTypeDef,
     _OptionalCreateLoadBalancerPolicyInputRequestTypeDef,
 ):
     pass
 
-LoadBalancerAttributesOutputTypeDef = TypedDict(
-    "LoadBalancerAttributesOutputTypeDef",
-    {
-        "CrossZoneLoadBalancing": CrossZoneLoadBalancingTypeDef,
-        "AccessLog": AccessLogTypeDef,
-        "ConnectionDraining": ConnectionDrainingTypeDef,
-        "ConnectionSettings": ConnectionSettingsTypeDef,
-        "AdditionalAttributes": List[AdditionalAttributeTypeDef],
-    },
-    total=False,
-)
-
 LoadBalancerAttributesTypeDef = TypedDict(
     "LoadBalancerAttributesTypeDef",
     {
         "CrossZoneLoadBalancing": CrossZoneLoadBalancingTypeDef,
         "AccessLog": AccessLogTypeDef,
         "ConnectionDraining": ConnectionDrainingTypeDef,
         "ConnectionSettings": ConnectionSettingsTypeDef,
-        "AdditionalAttributes": Sequence[AdditionalAttributeTypeDef],
+        "AdditionalAttributes": List[AdditionalAttributeTypeDef],
     },
     total=False,
 )
 
 DeregisterEndPointsInputRequestTypeDef = TypedDict(
     "DeregisterEndPointsInputRequestTypeDef",
     {
@@ -878,36 +864,33 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeLoadBalancerAttributesOutputTypeDef = TypedDict(
     "DescribeLoadBalancerAttributesOutputTypeDef",
     {
-        "LoadBalancerAttributes": LoadBalancerAttributesOutputTypeDef,
+        "LoadBalancerAttributes": LoadBalancerAttributesTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ModifyLoadBalancerAttributesOutputTypeDef = TypedDict(
-    "ModifyLoadBalancerAttributesOutputTypeDef",
+ModifyLoadBalancerAttributesInputRequestTypeDef = TypedDict(
+    "ModifyLoadBalancerAttributesInputRequestTypeDef",
     {
         "LoadBalancerName": str,
-        "LoadBalancerAttributes": LoadBalancerAttributesOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "LoadBalancerAttributes": LoadBalancerAttributesTypeDef,
     },
 )
 
-LoadBalancerAttributesUnionTypeDef = Union[
-    LoadBalancerAttributesTypeDef, LoadBalancerAttributesOutputTypeDef
-]
-ModifyLoadBalancerAttributesInputRequestTypeDef = TypedDict(
-    "ModifyLoadBalancerAttributesInputRequestTypeDef",
+ModifyLoadBalancerAttributesOutputTypeDef = TypedDict(
+    "ModifyLoadBalancerAttributesOutputTypeDef",
     {
         "LoadBalancerName": str,
         "LoadBalancerAttributes": LoadBalancerAttributesTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LoadBalancerDescriptionTypeDef = TypedDict(
     "LoadBalancerDescriptionTypeDef",
     {
         "LoadBalancerName": str,
```

### Comparing `types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb/waiter.py` & `types-aiobotocore-elb-2.5.2.post2/types_aiobotocore_elb/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb/waiter.pyi` & `types-aiobotocore-elb-2.5.2.post2/types_aiobotocore_elb/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elb-2.5.2.post1/types_aiobotocore_elb.egg-info/SOURCES.txt` & `types-aiobotocore-elb-2.5.2.post2/types_aiobotocore_elb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

