# Comparing `tmp/types-aiobotocore-service-quotas-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-service-quotas-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-service-quotas-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:59 2023, max compression
+gzip compressed data, was "types-aiobotocore-service-quotas-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:25 2023, max compression
```

## Comparing `types-aiobotocore-service-quotas-2.5.2.post1.tar` & `types-aiobotocore-service-quotas-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:59.901461 types-aiobotocore-service-quotas-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:49:30.000000 types-aiobotocore-service-quotas-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17050 2023-08-02 14:52:59.897461 types-aiobotocore-service-quotas-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15505 2023-08-02 14:49:30.000000 types-aiobotocore-service-quotas-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:59.901461 types-aiobotocore-service-quotas-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-08-02 14:49:30.000000 types-aiobotocore-service-quotas-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:59.897461 types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas/
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-08-02 14:49:30.000000 types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-08-02 14:49:30.000000 types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-08-02 14:49:30.000000 types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21026 2023-08-02 14:49:30.000000 types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20992 2023-08-02 14:49:30.000000 types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9872 2023-08-02 14:49:30.000000 types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9870 2023-08-02 14:49:30.000000 types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-08-02 14:49:30.000000 types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9119 2023-08-02 14:49:30.000000 types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:49:30.000000 types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    17540 2023-08-02 14:49:31.000000 types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17527 2023-08-02 14:49:31.000000 types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:49:30.000000 types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:59.897461 types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17050 2023-08-02 14:52:59.000000 types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-02 14:52:59.000000 types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:59.000000 types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:59.000000 types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:59.000000 types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 14:52:59.000000 types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:25.936643 types-aiobotocore-service-quotas-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:53:15.000000 types-aiobotocore-service-quotas-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14527 2023-08-04 13:59:25.936643 types-aiobotocore-service-quotas-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12982 2023-08-04 13:53:15.000000 types-aiobotocore-service-quotas-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:25.936643 types-aiobotocore-service-quotas-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2120 2023-08-04 13:53:15.000000 types-aiobotocore-service-quotas-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:25.936643 types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2292 2023-08-04 13:53:15.000000 types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2291 2023-08-04 13:53:15.000000 types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      969 2023-08-04 13:53:15.000000 types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    21026 2023-08-04 13:53:15.000000 types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    20992 2023-08-04 13:53:15.000000 types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9967 2023-08-04 13:53:15.000000 types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9965 2023-08-04 13:53:15.000000 types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9127 2023-08-04 13:53:15.000000 types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9119 2023-08-04 13:53:15.000000 types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:53:15.000000 types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    17540 2023-08-04 13:53:16.000000 types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    17527 2023-08-04 13:53:16.000000 types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:53:15.000000 types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:25.936643 types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14527 2023-08-04 13:59:25.000000 types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      946 2023-08-04 13:59:25.000000 types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:25.000000 types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:25.000000 types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:25.000000 types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       33 2023-08-04 13:59:25.000000 types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-service-quotas-2.5.2.post1/LICENSE` & `types-aiobotocore-service-quotas-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-service-quotas-2.5.2.post1/PKG-INFO` & `types-aiobotocore-service-quotas-2.5.2.post2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-service-quotas
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.ServiceQuotas 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.ServiceQuotas 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -47,15 +47,15 @@
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
 [types-aiobotocore-service-quotas docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/).
 
 See how it helps to find and fix potential bugs:
 
@@ -311,93 +311,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_service_quotas.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `ServiceQuotas` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/literals/).
+
 ```python
-from types_aiobotocore_service_quotas.literals import (
-    ErrorCodeType,
-    ListAWSDefaultServiceQuotasPaginatorName,
-    ListRequestedServiceQuotaChangeHistoryByQuotaPaginatorName,
-    ListRequestedServiceQuotaChangeHistoryPaginatorName,
-    ListServiceQuotaIncreaseRequestsInTemplatePaginatorName,
-    ListServiceQuotasPaginatorName,
-    ListServicesPaginatorName,
-    PeriodUnitType,
-    RequestStatusType,
-    ServiceQuotaTemplateAssociationStatusType,
-    ServiceQuotasServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_service_quotas.literals import ErrorCodeType
 
 
 def check_value(value: ErrorCodeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_service_quotas.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `ServiceQuotas` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/type_defs/).
+
 ```python
 from types_aiobotocore_service_quotas.type_defs import (
     DeleteServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef,
-    ErrorReasonTypeDef,
-    GetAWSDefaultServiceQuotaRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    GetRequestedServiceQuotaChangeRequestRequestTypeDef,
-    RequestedServiceQuotaChangeTypeDef,
-    GetServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef,
-    ServiceQuotaIncreaseRequestInTemplateTypeDef,
-    GetServiceQuotaRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListAWSDefaultServiceQuotasRequestRequestTypeDef,
-    ListRequestedServiceQuotaChangeHistoryByQuotaRequestRequestTypeDef,
-    ListRequestedServiceQuotaChangeHistoryRequestRequestTypeDef,
-    ListServiceQuotaIncreaseRequestsInTemplateRequestRequestTypeDef,
-    ListServiceQuotasRequestRequestTypeDef,
-    ListServicesRequestRequestTypeDef,
-    ServiceInfoTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    TagTypeDef,
-    MetricInfoTypeDef,
-    PutServiceQuotaIncreaseRequestIntoTemplateRequestRequestTypeDef,
-    QuotaPeriodTypeDef,
-    RequestServiceQuotaIncreaseRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    GetAssociationForServiceQuotaTemplateResponseTypeDef,
-    GetRequestedServiceQuotaChangeResponseTypeDef,
-    ListRequestedServiceQuotaChangeHistoryByQuotaResponseTypeDef,
-    ListRequestedServiceQuotaChangeHistoryResponseTypeDef,
-    RequestServiceQuotaIncreaseResponseTypeDef,
-    GetServiceQuotaIncreaseRequestFromTemplateResponseTypeDef,
-    ListServiceQuotaIncreaseRequestsInTemplateResponseTypeDef,
-    PutServiceQuotaIncreaseRequestIntoTemplateResponseTypeDef,
-    ListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef,
-    ListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef,
-    ListRequestedServiceQuotaChangeHistoryRequestListRequestedServiceQuotaChangeHistoryPaginateTypeDef,
-    ListServiceQuotaIncreaseRequestsInTemplateRequestListServiceQuotaIncreaseRequestsInTemplatePaginateTypeDef,
-    ListServiceQuotasRequestListServiceQuotasPaginateTypeDef,
-    ListServicesRequestListServicesPaginateTypeDef,
-    ListServicesResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
-    ServiceQuotaTypeDef,
-    GetAWSDefaultServiceQuotaResponseTypeDef,
-    GetServiceQuotaResponseTypeDef,
-    ListAWSDefaultServiceQuotasResponseTypeDef,
-    ListServiceQuotasResponseTypeDef,
 )
 
 
 def get_value() -> DeleteServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `types-aiobotocore-service-quotas-2.5.2.post1/README.md` & `types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-service-quotas
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.ServiceQuotas 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore service-quotas type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-service-quotas"></a>
 
 # types-aiobotocore-service-quotas
 
 [![PyPI - types-aiobotocore-service-quotas](https://img.shields.io/pypi/v/types-aiobotocore-service-quotas.svg?color=blue)](https://pypi.org/project/types-aiobotocore-service-quotas)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-service-quotas.svg?color=blue)](https://pypi.org/project/types-aiobotocore-service-quotas)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/)
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
 [types-aiobotocore-service-quotas docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/).
 
 See how it helps to find and fix potential bugs:
 
@@ -279,93 +311,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_service_quotas.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `ServiceQuotas` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/literals/).
+
 ```python
-from types_aiobotocore_service_quotas.literals import (
-    ErrorCodeType,
-    ListAWSDefaultServiceQuotasPaginatorName,
-    ListRequestedServiceQuotaChangeHistoryByQuotaPaginatorName,
-    ListRequestedServiceQuotaChangeHistoryPaginatorName,
-    ListServiceQuotaIncreaseRequestsInTemplatePaginatorName,
-    ListServiceQuotasPaginatorName,
-    ListServicesPaginatorName,
-    PeriodUnitType,
-    RequestStatusType,
-    ServiceQuotaTemplateAssociationStatusType,
-    ServiceQuotasServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_service_quotas.literals import ErrorCodeType
 
 
 def check_value(value: ErrorCodeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_service_quotas.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `ServiceQuotas` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/type_defs/).
+
 ```python
 from types_aiobotocore_service_quotas.type_defs import (
     DeleteServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef,
-    ErrorReasonTypeDef,
-    GetAWSDefaultServiceQuotaRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    GetRequestedServiceQuotaChangeRequestRequestTypeDef,
-    RequestedServiceQuotaChangeTypeDef,
-    GetServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef,
-    ServiceQuotaIncreaseRequestInTemplateTypeDef,
-    GetServiceQuotaRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListAWSDefaultServiceQuotasRequestRequestTypeDef,
-    ListRequestedServiceQuotaChangeHistoryByQuotaRequestRequestTypeDef,
-    ListRequestedServiceQuotaChangeHistoryRequestRequestTypeDef,
-    ListServiceQuotaIncreaseRequestsInTemplateRequestRequestTypeDef,
-    ListServiceQuotasRequestRequestTypeDef,
-    ListServicesRequestRequestTypeDef,
-    ServiceInfoTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    TagTypeDef,
-    MetricInfoTypeDef,
-    PutServiceQuotaIncreaseRequestIntoTemplateRequestRequestTypeDef,
-    QuotaPeriodTypeDef,
-    RequestServiceQuotaIncreaseRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    GetAssociationForServiceQuotaTemplateResponseTypeDef,
-    GetRequestedServiceQuotaChangeResponseTypeDef,
-    ListRequestedServiceQuotaChangeHistoryByQuotaResponseTypeDef,
-    ListRequestedServiceQuotaChangeHistoryResponseTypeDef,
-    RequestServiceQuotaIncreaseResponseTypeDef,
-    GetServiceQuotaIncreaseRequestFromTemplateResponseTypeDef,
-    ListServiceQuotaIncreaseRequestsInTemplateResponseTypeDef,
-    PutServiceQuotaIncreaseRequestIntoTemplateResponseTypeDef,
-    ListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef,
-    ListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef,
-    ListRequestedServiceQuotaChangeHistoryRequestListRequestedServiceQuotaChangeHistoryPaginateTypeDef,
-    ListServiceQuotaIncreaseRequestsInTemplateRequestListServiceQuotaIncreaseRequestsInTemplatePaginateTypeDef,
-    ListServiceQuotasRequestListServiceQuotasPaginateTypeDef,
-    ListServicesRequestListServicesPaginateTypeDef,
-    ListServicesResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
-    ServiceQuotaTypeDef,
-    GetAWSDefaultServiceQuotaResponseTypeDef,
-    GetServiceQuotaResponseTypeDef,
-    ListAWSDefaultServiceQuotasResponseTypeDef,
-    ListServiceQuotasResponseTypeDef,
 )
 
 
 def get_value() -> DeleteServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `types-aiobotocore-service-quotas-2.5.2.post1/setup.py` & `types-aiobotocore-service-quotas-2.5.2.post2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-service-quotas",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_service_quotas"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ServiceQuotas 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas/__init__.py` & `types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas/__init__.pyi` & `types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas/__main__.py` & `types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.ServiceQuotas 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas\nOther"
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

### Comparing `types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas/client.py` & `types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas/client.pyi` & `types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas/literals.py` & `types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,14 +71,15 @@
     "amplifybackend",
     "amplifyuibuilder",
     "apigateway",
     "apigatewaymanagementapi",
     "apigatewayv2",
     "appconfig",
     "appconfigdata",
+    "appfabric",
     "appflow",
     "appintegrations",
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
@@ -174,14 +175,15 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
+    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -260,26 +262,28 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
+    "managedblockchain-query",
     "marketplace-catalog",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
+    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas/literals.pyi` & `types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -69,14 +69,15 @@
     "amplifybackend",
     "amplifyuibuilder",
     "apigateway",
     "apigatewaymanagementapi",
     "apigatewayv2",
     "appconfig",
     "appconfigdata",
+    "appfabric",
     "appflow",
     "appintegrations",
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
@@ -172,14 +173,15 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
+    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -258,26 +260,28 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
+    "managedblockchain-query",
     "marketplace-catalog",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
+    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas/paginator.py` & `types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas/paginator.pyi` & `types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas/type_defs.py` & `types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas/type_defs.pyi` & `types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas.egg-info/PKG-INFO` & `types-aiobotocore-service-quotas-2.5.2.post2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore-service-quotas
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.ServiceQuotas 2.5.2 service generated with mypy-boto3-builder 7.17.1
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore service-quotas type-annotations botocore mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="types-aiobotocore-service-quotas"></a>
 
 # types-aiobotocore-service-quotas
 
 [![PyPI - types-aiobotocore-service-quotas](https://img.shields.io/pypi/v/types-aiobotocore-service-quotas.svg?color=blue)](https://pypi.org/project/types-aiobotocore-service-quotas)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-service-quotas.svg?color=blue)](https://pypi.org/project/types-aiobotocore-service-quotas)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/)
@@ -47,15 +15,15 @@
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
 [types-aiobotocore-service-quotas docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/).
 
 See how it helps to find and fix potential bugs:
 
@@ -311,93 +279,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_service_quotas.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `ServiceQuotas` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/literals/).
+
 ```python
-from types_aiobotocore_service_quotas.literals import (
-    ErrorCodeType,
-    ListAWSDefaultServiceQuotasPaginatorName,
-    ListRequestedServiceQuotaChangeHistoryByQuotaPaginatorName,
-    ListRequestedServiceQuotaChangeHistoryPaginatorName,
-    ListServiceQuotaIncreaseRequestsInTemplatePaginatorName,
-    ListServiceQuotasPaginatorName,
-    ListServicesPaginatorName,
-    PeriodUnitType,
-    RequestStatusType,
-    ServiceQuotaTemplateAssociationStatusType,
-    ServiceQuotasServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_service_quotas.literals import ErrorCodeType
 
 
 def check_value(value: ErrorCodeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_service_quotas.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `ServiceQuotas` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/type_defs/).
+
 ```python
 from types_aiobotocore_service_quotas.type_defs import (
     DeleteServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef,
-    ErrorReasonTypeDef,
-    GetAWSDefaultServiceQuotaRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    GetRequestedServiceQuotaChangeRequestRequestTypeDef,
-    RequestedServiceQuotaChangeTypeDef,
-    GetServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef,
-    ServiceQuotaIncreaseRequestInTemplateTypeDef,
-    GetServiceQuotaRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListAWSDefaultServiceQuotasRequestRequestTypeDef,
-    ListRequestedServiceQuotaChangeHistoryByQuotaRequestRequestTypeDef,
-    ListRequestedServiceQuotaChangeHistoryRequestRequestTypeDef,
-    ListServiceQuotaIncreaseRequestsInTemplateRequestRequestTypeDef,
-    ListServiceQuotasRequestRequestTypeDef,
-    ListServicesRequestRequestTypeDef,
-    ServiceInfoTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    TagTypeDef,
-    MetricInfoTypeDef,
-    PutServiceQuotaIncreaseRequestIntoTemplateRequestRequestTypeDef,
-    QuotaPeriodTypeDef,
-    RequestServiceQuotaIncreaseRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    GetAssociationForServiceQuotaTemplateResponseTypeDef,
-    GetRequestedServiceQuotaChangeResponseTypeDef,
-    ListRequestedServiceQuotaChangeHistoryByQuotaResponseTypeDef,
-    ListRequestedServiceQuotaChangeHistoryResponseTypeDef,
-    RequestServiceQuotaIncreaseResponseTypeDef,
-    GetServiceQuotaIncreaseRequestFromTemplateResponseTypeDef,
-    ListServiceQuotaIncreaseRequestsInTemplateResponseTypeDef,
-    PutServiceQuotaIncreaseRequestIntoTemplateResponseTypeDef,
-    ListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef,
-    ListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef,
-    ListRequestedServiceQuotaChangeHistoryRequestListRequestedServiceQuotaChangeHistoryPaginateTypeDef,
-    ListServiceQuotaIncreaseRequestsInTemplateRequestListServiceQuotaIncreaseRequestsInTemplatePaginateTypeDef,
-    ListServiceQuotasRequestListServiceQuotasPaginateTypeDef,
-    ListServicesRequestListServicesPaginateTypeDef,
-    ListServicesResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
-    ServiceQuotaTypeDef,
-    GetAWSDefaultServiceQuotaResponseTypeDef,
-    GetServiceQuotaResponseTypeDef,
-    ListAWSDefaultServiceQuotasResponseTypeDef,
-    ListServiceQuotasResponseTypeDef,
 )
 
 
 def get_value() -> DeleteServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas.egg-info/SOURCES.txt` & `types-aiobotocore-service-quotas-2.5.2.post2/types_aiobotocore_service_quotas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

