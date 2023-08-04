# Comparing `tmp/types-aiobotocore-mgn-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-mgn-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-mgn-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:40 2023, max compression
+gzip compressed data, was "types-aiobotocore-mgn-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:18 2023, max compression
```

## Comparing `types-aiobotocore-mgn-2.5.2.post1.tar` & `types-aiobotocore-mgn-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:40.945520 types-aiobotocore-mgn-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:43:36.000000 types-aiobotocore-mgn-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23449 2023-08-02 14:52:40.945520 types-aiobotocore-mgn-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21947 2023-08-02 14:43:36.000000 types-aiobotocore-mgn-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:40.945520 types-aiobotocore-mgn-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-02 14:43:36.000000 types-aiobotocore-mgn-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:40.941520 types-aiobotocore-mgn-2.5.2.post1/types_aiobotocore_mgn/
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-08-02 14:43:36.000000 types-aiobotocore-mgn-2.5.2.post1/types_aiobotocore_mgn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-08-02 14:43:36.000000 types-aiobotocore-mgn-2.5.2.post1/types_aiobotocore_mgn/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-02 14:43:36.000000 types-aiobotocore-mgn-2.5.2.post1/types_aiobotocore_mgn/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50879 2023-08-02 14:43:38.000000 types-aiobotocore-mgn-2.5.2.post1/types_aiobotocore_mgn/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    50795 2023-08-02 14:43:38.000000 types-aiobotocore-mgn-2.5.2.post1/types_aiobotocore_mgn/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15390 2023-08-02 14:43:39.000000 types-aiobotocore-mgn-2.5.2.post1/types_aiobotocore_mgn/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15388 2023-08-02 14:43:39.000000 types-aiobotocore-mgn-2.5.2.post1/types_aiobotocore_mgn/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17550 2023-08-02 14:43:38.000000 types-aiobotocore-mgn-2.5.2.post1/types_aiobotocore_mgn/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17534 2023-08-02 14:43:38.000000 types-aiobotocore-mgn-2.5.2.post1/types_aiobotocore_mgn/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:43:36.000000 types-aiobotocore-mgn-2.5.2.post1/types_aiobotocore_mgn/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    69562 2023-08-02 14:43:40.000000 types-aiobotocore-mgn-2.5.2.post1/types_aiobotocore_mgn/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    69495 2023-08-02 14:43:39.000000 types-aiobotocore-mgn-2.5.2.post1/types_aiobotocore_mgn/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:43:36.000000 types-aiobotocore-mgn-2.5.2.post1/types_aiobotocore_mgn/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:40.945520 types-aiobotocore-mgn-2.5.2.post1/types_aiobotocore_mgn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23449 2023-08-02 14:52:40.000000 types-aiobotocore-mgn-2.5.2.post1/types_aiobotocore_mgn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-02 14:52:40.000000 types-aiobotocore-mgn-2.5.2.post1/types_aiobotocore_mgn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:40.000000 types-aiobotocore-mgn-2.5.2.post1/types_aiobotocore_mgn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:40.000000 types-aiobotocore-mgn-2.5.2.post1/types_aiobotocore_mgn.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:40.000000 types-aiobotocore-mgn-2.5.2.post1/types_aiobotocore_mgn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 14:52:40.000000 types-aiobotocore-mgn-2.5.2.post1/types_aiobotocore_mgn.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:18.526643 types-aiobotocore-mgn-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:44:58.000000 types-aiobotocore-mgn-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14966 2023-08-04 13:59:18.526643 types-aiobotocore-mgn-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13464 2023-08-04 13:44:58.000000 types-aiobotocore-mgn-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:18.526643 types-aiobotocore-mgn-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2020 2023-08-04 13:44:58.000000 types-aiobotocore-mgn-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:18.526643 types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     3813 2023-08-04 13:44:58.000000 types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     3812 2023-08-04 13:44:58.000000 types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      916 2023-08-04 13:44:58.000000 types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    54555 2023-08-04 13:44:58.000000 types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    54466 2023-08-04 13:44:58.000000 types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    15622 2023-08-04 13:44:59.000000 types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    15620 2023-08-04 13:44:59.000000 types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    18818 2023-08-04 13:44:59.000000 types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    18801 2023-08-04 13:44:59.000000 types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:44:58.000000 types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    79861 2023-08-04 13:45:02.000000 types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    79746 2023-08-04 13:45:01.000000 types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:44:58.000000 types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:18.526643 types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14966 2023-08-04 13:59:18.000000 types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      737 2023-08-04 13:59:18.000000 types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:18.000000 types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:18.000000 types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:18.000000 types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       22 2023-08-04 13:59:18.000000 types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-mgn-2.5.2.post1/LICENSE` & `types-aiobotocore-mgn-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mgn-2.5.2.post1/setup.py` & `types-aiobotocore-mgn-2.5.2.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-mgn",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_mgn"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.mgn 2.5.2 service generated with mypy-boto3-builder"
-        " 7.17.1"
+        " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

### Comparing `types-aiobotocore-mgn-2.5.2.post1/types_aiobotocore_mgn/__init__.py` & `types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
         DescribeSourceServersPaginator,
         DescribeVcenterClientsPaginator,
         ListApplicationsPaginator,
         ListExportErrorsPaginator,
         ListExportsPaginator,
         ListImportErrorsPaginator,
         ListImportsPaginator,
+        ListManagedAccountsPaginator,
         ListSourceServerActionsPaginator,
         ListTemplateActionsPaginator,
         ListWavesPaginator,
         mgnClient,
     )
 
     session = get_session()
@@ -37,14 +38,15 @@
     describe_source_servers_paginator: DescribeSourceServersPaginator = client.get_paginator("describe_source_servers")
     describe_vcenter_clients_paginator: DescribeVcenterClientsPaginator = client.get_paginator("describe_vcenter_clients")
     list_applications_paginator: ListApplicationsPaginator = client.get_paginator("list_applications")
     list_export_errors_paginator: ListExportErrorsPaginator = client.get_paginator("list_export_errors")
     list_exports_paginator: ListExportsPaginator = client.get_paginator("list_exports")
     list_import_errors_paginator: ListImportErrorsPaginator = client.get_paginator("list_import_errors")
     list_imports_paginator: ListImportsPaginator = client.get_paginator("list_imports")
+    list_managed_accounts_paginator: ListManagedAccountsPaginator = client.get_paginator("list_managed_accounts")
     list_source_server_actions_paginator: ListSourceServerActionsPaginator = client.get_paginator("list_source_server_actions")
     list_template_actions_paginator: ListTemplateActionsPaginator = client.get_paginator("list_template_actions")
     list_waves_paginator: ListWavesPaginator = client.get_paginator("list_waves")
     ```
 """
 from .client import mgnClient
 from .paginator import (
@@ -55,14 +57,15 @@
     DescribeSourceServersPaginator,
     DescribeVcenterClientsPaginator,
     ListApplicationsPaginator,
     ListExportErrorsPaginator,
     ListExportsPaginator,
     ListImportErrorsPaginator,
     ListImportsPaginator,
+    ListManagedAccountsPaginator,
     ListSourceServerActionsPaginator,
     ListTemplateActionsPaginator,
     ListWavesPaginator,
 )
 
 Client = mgnClient
 
@@ -76,12 +79,13 @@
     "DescribeSourceServersPaginator",
     "DescribeVcenterClientsPaginator",
     "ListApplicationsPaginator",
     "ListExportErrorsPaginator",
     "ListExportsPaginator",
     "ListImportErrorsPaginator",
     "ListImportsPaginator",
+    "ListManagedAccountsPaginator",
     "ListSourceServerActionsPaginator",
     "ListTemplateActionsPaginator",
     "ListWavesPaginator",
     "mgnClient",
 )
```

### Comparing `types-aiobotocore-mgn-2.5.2.post1/types_aiobotocore_mgn/__init__.pyi` & `types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn/__init__.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
         DescribeSourceServersPaginator,
         DescribeVcenterClientsPaginator,
         ListApplicationsPaginator,
         ListExportErrorsPaginator,
         ListExportsPaginator,
         ListImportErrorsPaginator,
         ListImportsPaginator,
+        ListManagedAccountsPaginator,
         ListSourceServerActionsPaginator,
         ListTemplateActionsPaginator,
         ListWavesPaginator,
         mgnClient,
     )
 
     session = get_session()
@@ -37,14 +38,15 @@
     describe_source_servers_paginator: DescribeSourceServersPaginator = client.get_paginator("describe_source_servers")
     describe_vcenter_clients_paginator: DescribeVcenterClientsPaginator = client.get_paginator("describe_vcenter_clients")
     list_applications_paginator: ListApplicationsPaginator = client.get_paginator("list_applications")
     list_export_errors_paginator: ListExportErrorsPaginator = client.get_paginator("list_export_errors")
     list_exports_paginator: ListExportsPaginator = client.get_paginator("list_exports")
     list_import_errors_paginator: ListImportErrorsPaginator = client.get_paginator("list_import_errors")
     list_imports_paginator: ListImportsPaginator = client.get_paginator("list_imports")
+    list_managed_accounts_paginator: ListManagedAccountsPaginator = client.get_paginator("list_managed_accounts")
     list_source_server_actions_paginator: ListSourceServerActionsPaginator = client.get_paginator("list_source_server_actions")
     list_template_actions_paginator: ListTemplateActionsPaginator = client.get_paginator("list_template_actions")
     list_waves_paginator: ListWavesPaginator = client.get_paginator("list_waves")
     ```
 """
 from .client import mgnClient
 from .paginator import (
@@ -55,14 +57,15 @@
     DescribeSourceServersPaginator,
     DescribeVcenterClientsPaginator,
     ListApplicationsPaginator,
     ListExportErrorsPaginator,
     ListExportsPaginator,
     ListImportErrorsPaginator,
     ListImportsPaginator,
+    ListManagedAccountsPaginator,
     ListSourceServerActionsPaginator,
     ListTemplateActionsPaginator,
     ListWavesPaginator,
 )
 
 Client = mgnClient
 
@@ -75,12 +78,13 @@
     "DescribeSourceServersPaginator",
     "DescribeVcenterClientsPaginator",
     "ListApplicationsPaginator",
     "ListExportErrorsPaginator",
     "ListExportsPaginator",
     "ListImportErrorsPaginator",
     "ListImportsPaginator",
+    "ListManagedAccountsPaginator",
     "ListSourceServerActionsPaginator",
     "ListTemplateActionsPaginator",
     "ListWavesPaginator",
     "mgnClient",
 )
```

### Comparing `types-aiobotocore-mgn-2.5.2.post1/types_aiobotocore_mgn/__main__.py` & `types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.mgn 2.5.2\nVersion:         2.5.2.post1\nBuilder version:"
-        " 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.mgn 2.5.2\nVersion:         2.5.2.post2\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn\nOther"
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

### Comparing `types-aiobotocore-mgn-2.5.2.post1/types_aiobotocore_mgn/client.py` & `types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     DescribeSourceServersPaginator,
     DescribeVcenterClientsPaginator,
     ListApplicationsPaginator,
     ListExportErrorsPaginator,
     ListExportsPaginator,
     ListImportErrorsPaginator,
     ListImportsPaginator,
+    ListManagedAccountsPaginator,
     ListSourceServerActionsPaginator,
     ListTemplateActionsPaginator,
     ListWavesPaginator,
 )
 from .type_defs import (
     ApplicationResponseTypeDef,
     ChangeServerLifeCycleStateSourceServerLifecycleTypeDef,
@@ -66,20 +67,21 @@
     ListApplicationsResponseTypeDef,
     ListExportErrorsResponseTypeDef,
     ListExportsRequestFiltersTypeDef,
     ListExportsResponseTypeDef,
     ListImportErrorsResponseTypeDef,
     ListImportsRequestFiltersTypeDef,
     ListImportsResponseTypeDef,
+    ListManagedAccountsResponseTypeDef,
     ListSourceServerActionsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTemplateActionsResponseTypeDef,
     ListWavesRequestFiltersTypeDef,
     ListWavesResponseTypeDef,
-    PostLaunchActionsUnionTypeDef,
+    PostLaunchActionsTypeDef,
     ReplicationConfigurationReplicatedDiskTypeDef,
     ReplicationConfigurationTemplateResponseTypeDef,
     ReplicationConfigurationTypeDef,
     S3BucketSourceTypeDef,
     SourceServerActionDocumentResponseTypeDef,
     SourceServerActionsRequestFiltersTypeDef,
     SourceServerResponseTypeDef,
@@ -137,42 +139,44 @@
         """
         mgnClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#exceptions)
         """
 
-    async def archive_application(self, *, applicationID: str) -> ApplicationResponseTypeDef:
+    async def archive_application(
+        self, *, applicationID: str, accountID: str = ...
+    ) -> ApplicationResponseTypeDef:
         """
         Archive application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.archive_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#archive_application)
         """
 
-    async def archive_wave(self, *, waveID: str) -> WaveResponseTypeDef:
+    async def archive_wave(self, *, waveID: str, accountID: str = ...) -> WaveResponseTypeDef:
         """
         Archive wave.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.archive_wave)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#archive_wave)
         """
 
     async def associate_applications(
-        self, *, applicationIDs: Sequence[str], waveID: str
+        self, *, applicationIDs: Sequence[str], waveID: str, accountID: str = ...
     ) -> Dict[str, Any]:
         """
         Associate applications to wave.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.associate_applications)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#associate_applications)
         """
 
     async def associate_source_servers(
-        self, *, applicationID: str, sourceServerIDs: Sequence[str]
+        self, *, applicationID: str, sourceServerIDs: Sequence[str], accountID: str = ...
     ) -> Dict[str, Any]:
         """
         Associate source servers to application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.associate_source_servers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#associate_source_servers)
         """
@@ -185,15 +189,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#can_paginate)
         """
 
     async def change_server_life_cycle_state(
         self,
         *,
         lifeCycle: ChangeServerLifeCycleStateSourceServerLifecycleTypeDef,
-        sourceServerID: str
+        sourceServerID: str,
+        accountID: str = ...
     ) -> SourceServerResponseTypeDef:
         """
         Allows the user to set the SourceServer.LifeCycle.state property for specific
         Source Server IDs to one of the following: READY_FOR_TEST or READY_FOR_CUTOVER.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.change_server_life_cycle_state)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#change_server_life_cycle_state)
@@ -204,15 +209,20 @@
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#close)
         """
 
     async def create_application(
-        self, *, name: str, description: str = ..., tags: Mapping[str, str] = ...
+        self,
+        *,
+        name: str,
+        accountID: str = ...,
+        description: str = ...,
+        tags: Mapping[str, str] = ...
     ) -> ApplicationResponseTypeDef:
         """
         Create application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.create_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#create_application)
         """
@@ -225,15 +235,15 @@
         copyPrivateIp: bool = ...,
         copyTags: bool = ...,
         enableMapAutoTagging: bool = ...,
         largeVolumeConf: LaunchTemplateDiskConfTypeDef = ...,
         launchDisposition: LaunchDispositionType = ...,
         licensing: LicensingTypeDef = ...,
         mapAutoTaggingMpeID: str = ...,
-        postLaunchActions: PostLaunchActionsUnionTypeDef = ...,
+        postLaunchActions: PostLaunchActionsTypeDef = ...,
         smallVolumeConf: LaunchTemplateDiskConfTypeDef = ...,
         smallVolumeMaxSize: int = ...,
         tags: Mapping[str, str] = ...,
         targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType = ...
     ) -> LaunchConfigurationTemplateResponseTypeDef:
         """
         Creates a new Launch Configuration Template.
@@ -253,42 +263,50 @@
         ebsEncryption: ReplicationConfigurationEbsEncryptionType,
         replicationServerInstanceType: str,
         replicationServersSecurityGroupsIDs: Sequence[str],
         stagingAreaSubnetId: str,
         stagingAreaTags: Mapping[str, str],
         useDedicatedReplicationServer: bool,
         ebsEncryptionKeyArn: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
+        useFipsEndpoint: bool = ...
     ) -> ReplicationConfigurationTemplateResponseTypeDef:
         """
         Creates a new ReplicationConfigurationTemplate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.create_replication_configuration_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#create_replication_configuration_template)
         """
 
     async def create_wave(
-        self, *, name: str, description: str = ..., tags: Mapping[str, str] = ...
+        self,
+        *,
+        name: str,
+        accountID: str = ...,
+        description: str = ...,
+        tags: Mapping[str, str] = ...
     ) -> WaveResponseTypeDef:
         """
         Create wave.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.create_wave)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#create_wave)
         """
 
-    async def delete_application(self, *, applicationID: str) -> Dict[str, Any]:
+    async def delete_application(
+        self, *, applicationID: str, accountID: str = ...
+    ) -> Dict[str, Any]:
         """
         Delete application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.delete_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#delete_application)
         """
 
-    async def delete_job(self, *, jobID: str) -> Dict[str, Any]:
+    async def delete_job(self, *, jobID: str, accountID: str = ...) -> Dict[str, Any]:
         """
         Deletes a single Job by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.delete_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#delete_job)
         """
 
@@ -309,15 +327,17 @@
         Deletes a single Replication Configuration Template by ID See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/mgn-2020-02-26/DeleteReplicationConfigurationTemplate).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.delete_replication_configuration_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#delete_replication_configuration_template)
         """
 
-    async def delete_source_server(self, *, sourceServerID: str) -> Dict[str, Any]:
+    async def delete_source_server(
+        self, *, sourceServerID: str, accountID: str = ...
+    ) -> Dict[str, Any]:
         """
         Deletes a single source server by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.delete_source_server)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#delete_source_server)
         """
 
@@ -325,35 +345,36 @@
         """
         Deletes a given vCenter client by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.delete_vcenter_client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#delete_vcenter_client)
         """
 
-    async def delete_wave(self, *, waveID: str) -> Dict[str, Any]:
+    async def delete_wave(self, *, waveID: str, accountID: str = ...) -> Dict[str, Any]:
         """
         Delete wave.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.delete_wave)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#delete_wave)
         """
 
     async def describe_job_log_items(
-        self, *, jobID: str, maxResults: int = ..., nextToken: str = ...
+        self, *, jobID: str, accountID: str = ..., maxResults: int = ..., nextToken: str = ...
     ) -> DescribeJobLogItemsResponseTypeDef:
         """
         Retrieves detailed job log items with paging.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.describe_job_log_items)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#describe_job_log_items)
         """
 
     async def describe_jobs(
         self,
         *,
+        accountID: str = ...,
         filters: DescribeJobsRequestFiltersTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> DescribeJobsResponseTypeDef:
         """
         Returns a list of Jobs.
 
@@ -390,14 +411,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.describe_replication_configuration_templates)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#describe_replication_configuration_templates)
         """
 
     async def describe_source_servers(
         self,
         *,
+        accountID: str = ...,
         filters: DescribeSourceServersRequestFiltersTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> DescribeSourceServersResponseTypeDef:
         """
         Retrieves all SourceServers or multiple SourceServers by ID.
 
@@ -412,42 +434,46 @@
         Returns a list of the installed vCenter clients.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.describe_vcenter_clients)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#describe_vcenter_clients)
         """
 
     async def disassociate_applications(
-        self, *, applicationIDs: Sequence[str], waveID: str
+        self, *, applicationIDs: Sequence[str], waveID: str, accountID: str = ...
     ) -> Dict[str, Any]:
         """
         Disassociate applications from wave.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.disassociate_applications)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#disassociate_applications)
         """
 
     async def disassociate_source_servers(
-        self, *, applicationID: str, sourceServerIDs: Sequence[str]
+        self, *, applicationID: str, sourceServerIDs: Sequence[str], accountID: str = ...
     ) -> Dict[str, Any]:
         """
         Disassociate source servers from application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.disassociate_source_servers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#disassociate_source_servers)
         """
 
-    async def disconnect_from_service(self, *, sourceServerID: str) -> SourceServerResponseTypeDef:
+    async def disconnect_from_service(
+        self, *, sourceServerID: str, accountID: str = ...
+    ) -> SourceServerResponseTypeDef:
         """
         Disconnects specific Source Servers from Application Migration Service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.disconnect_from_service)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#disconnect_from_service)
         """
 
-    async def finalize_cutover(self, *, sourceServerID: str) -> SourceServerResponseTypeDef:
+    async def finalize_cutover(
+        self, *, sourceServerID: str, accountID: str = ...
+    ) -> SourceServerResponseTypeDef:
         """
         Finalizes the cutover immediately for specific Source Servers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.finalize_cutover)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#finalize_cutover)
         """
 
@@ -461,24 +487,26 @@
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#generate_presigned_url)
         """
 
-    async def get_launch_configuration(self, *, sourceServerID: str) -> LaunchConfigurationTypeDef:
+    async def get_launch_configuration(
+        self, *, sourceServerID: str, accountID: str = ...
+    ) -> LaunchConfigurationTypeDef:
         """
         Lists all LaunchConfigurations available, filtered by Source Server IDs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.get_launch_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#get_launch_configuration)
         """
 
     async def get_replication_configuration(
-        self, *, sourceServerID: str
+        self, *, sourceServerID: str, accountID: str = ...
     ) -> ReplicationConfigurationTypeDef:
         """
         Lists all ReplicationConfigurations, filtered by Source Server ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.get_replication_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#get_replication_configuration)
         """
@@ -490,14 +518,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.initialize_service)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#initialize_service)
         """
 
     async def list_applications(
         self,
         *,
+        accountID: str = ...,
         filters: ListApplicationsRequestFiltersTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListApplicationsResponseTypeDef:
         """
         Retrieves all applications or multiple applications by ID.
 
@@ -549,18 +578,29 @@
         """
         List imports.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.list_imports)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#list_imports)
         """
 
+    async def list_managed_accounts(
+        self, *, maxResults: int = ..., nextToken: str = ...
+    ) -> ListManagedAccountsResponseTypeDef:
+        """
+        List Managed Accounts.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.list_managed_accounts)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#list_managed_accounts)
+        """
+
     async def list_source_server_actions(
         self,
         *,
         sourceServerID: str,
+        accountID: str = ...,
         filters: SourceServerActionsRequestFiltersTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListSourceServerActionsResponseTypeDef:
         """
         List source server post migration custom actions.
 
@@ -592,42 +632,56 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.list_template_actions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#list_template_actions)
         """
 
     async def list_waves(
         self,
         *,
+        accountID: str = ...,
         filters: ListWavesRequestFiltersTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListWavesResponseTypeDef:
         """
         Retrieves all waves or multiple waves by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.list_waves)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#list_waves)
         """
 
-    async def mark_as_archived(self, *, sourceServerID: str) -> SourceServerResponseTypeDef:
+    async def mark_as_archived(
+        self, *, sourceServerID: str, accountID: str = ...
+    ) -> SourceServerResponseTypeDef:
         """
         Archives specific Source Servers by setting the SourceServer.isArchived property
         to true for specified SourceServers by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.mark_as_archived)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#mark_as_archived)
         """
 
+    async def pause_replication(
+        self, *, sourceServerID: str, accountID: str = ...
+    ) -> SourceServerResponseTypeDef:
+        """
+        Pause Replication.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.pause_replication)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#pause_replication)
+        """
+
     async def put_source_server_action(
         self,
         *,
         actionID: str,
         actionName: str,
         documentIdentifier: str,
         order: int,
         sourceServerID: str,
+        accountID: str = ...,
         active: bool = ...,
         category: ActionCategoryType = ...,
         description: str = ...,
         documentVersion: str = ...,
         externalParameters: Mapping[str, SsmExternalParameterTypeDef] = ...,
         mustSucceedForCutover: bool = ...,
         parameters: Mapping[str, Sequence[SsmParameterStoreParameterTypeDef]] = ...,
@@ -662,15 +716,15 @@
         Put template post migration custom action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.put_template_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#put_template_action)
         """
 
     async def remove_source_server_action(
-        self, *, actionID: str, sourceServerID: str
+        self, *, actionID: str, sourceServerID: str, accountID: str = ...
     ) -> Dict[str, Any]:
         """
         Remove source server post migration custom action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.remove_source_server_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#remove_source_server_action)
         """
@@ -681,26 +735,38 @@
         """
         Remove template post migration custom action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.remove_template_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#remove_template_action)
         """
 
-    async def retry_data_replication(self, *, sourceServerID: str) -> SourceServerResponseTypeDef:
+    async def resume_replication(
+        self, *, sourceServerID: str, accountID: str = ...
+    ) -> SourceServerResponseTypeDef:
+        """
+        Resume Replication.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.resume_replication)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#resume_replication)
+        """
+
+    async def retry_data_replication(
+        self, *, sourceServerID: str, accountID: str = ...
+    ) -> SourceServerResponseTypeDef:
         """
         Causes the data replication initiation sequence to begin immediately upon next
         Handshake for specified SourceServer IDs, regardless of when the previous
         initiation started.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.retry_data_replication)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#retry_data_replication)
         """
 
     async def start_cutover(
-        self, *, sourceServerIDs: Sequence[str], tags: Mapping[str, str] = ...
+        self, *, sourceServerIDs: Sequence[str], accountID: str = ..., tags: Mapping[str, str] = ...
     ) -> StartCutoverResponseTypeDef:
         """
         Launches a Cutover Instance for specific Source Servers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.start_cutover)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#start_cutover)
         """
@@ -721,62 +787,76 @@
         """
         Start import.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.start_import)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#start_import)
         """
 
-    async def start_replication(self, *, sourceServerID: str) -> SourceServerResponseTypeDef:
+    async def start_replication(
+        self, *, sourceServerID: str, accountID: str = ...
+    ) -> SourceServerResponseTypeDef:
         """
         Starts replication for SNAPSHOT_SHIPPING agents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.start_replication)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#start_replication)
         """
 
     async def start_test(
-        self, *, sourceServerIDs: Sequence[str], tags: Mapping[str, str] = ...
+        self, *, sourceServerIDs: Sequence[str], accountID: str = ..., tags: Mapping[str, str] = ...
     ) -> StartTestResponseTypeDef:
         """
         Launches a Test Instance for specific Source Servers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.start_test)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#start_test)
         """
 
+    async def stop_replication(
+        self, *, sourceServerID: str, accountID: str = ...
+    ) -> SourceServerResponseTypeDef:
+        """
+        Stop Replication.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.stop_replication)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#stop_replication)
+        """
+
     async def tag_resource(
         self, *, resourceArn: str, tags: Mapping[str, str]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Adds or overwrites only the specified tags for the specified Application
         Migration Service resource or resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#tag_resource)
         """
 
     async def terminate_target_instances(
-        self, *, sourceServerIDs: Sequence[str], tags: Mapping[str, str] = ...
+        self, *, sourceServerIDs: Sequence[str], accountID: str = ..., tags: Mapping[str, str] = ...
     ) -> TerminateTargetInstancesResponseTypeDef:
         """
         Starts a job that terminates specific launched EC2 Test and Cutover instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.terminate_target_instances)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#terminate_target_instances)
         """
 
-    async def unarchive_application(self, *, applicationID: str) -> ApplicationResponseTypeDef:
+    async def unarchive_application(
+        self, *, applicationID: str, accountID: str = ...
+    ) -> ApplicationResponseTypeDef:
         """
         Unarchive application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.unarchive_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#unarchive_application)
         """
 
-    async def unarchive_wave(self, *, waveID: str) -> WaveResponseTypeDef:
+    async def unarchive_wave(self, *, waveID: str, accountID: str = ...) -> WaveResponseTypeDef:
         """
         Unarchive wave.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.unarchive_wave)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#unarchive_wave)
         """
 
@@ -788,36 +868,37 @@
         Migration Service resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#untag_resource)
         """
 
     async def update_application(
-        self, *, applicationID: str, description: str = ..., name: str = ...
+        self, *, applicationID: str, accountID: str = ..., description: str = ..., name: str = ...
     ) -> ApplicationResponseTypeDef:
         """
         Update application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#update_application)
         """
 
     async def update_launch_configuration(
         self,
         *,
         sourceServerID: str,
+        accountID: str = ...,
         bootMode: BootModeType = ...,
         copyPrivateIp: bool = ...,
         copyTags: bool = ...,
         enableMapAutoTagging: bool = ...,
         launchDisposition: LaunchDispositionType = ...,
         licensing: LicensingTypeDef = ...,
         mapAutoTaggingMpeID: str = ...,
         name: str = ...,
-        postLaunchActions: PostLaunchActionsUnionTypeDef = ...,
+        postLaunchActions: PostLaunchActionsTypeDef = ...,
         targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType = ...
     ) -> LaunchConfigurationTypeDef:
         """
         Updates multiple LaunchConfigurations by Source Server ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_launch_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#update_launch_configuration)
@@ -832,15 +913,15 @@
         copyPrivateIp: bool = ...,
         copyTags: bool = ...,
         enableMapAutoTagging: bool = ...,
         largeVolumeConf: LaunchTemplateDiskConfTypeDef = ...,
         launchDisposition: LaunchDispositionType = ...,
         licensing: LicensingTypeDef = ...,
         mapAutoTaggingMpeID: str = ...,
-        postLaunchActions: PostLaunchActionsUnionTypeDef = ...,
+        postLaunchActions: PostLaunchActionsTypeDef = ...,
         smallVolumeConf: LaunchTemplateDiskConfTypeDef = ...,
         smallVolumeMaxSize: int = ...,
         targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType = ...
     ) -> LaunchConfigurationTemplateResponseTypeDef:
         """
         Updates an existing Launch Configuration Template by ID.
 
@@ -848,28 +929,30 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#update_launch_configuration_template)
         """
 
     async def update_replication_configuration(
         self,
         *,
         sourceServerID: str,
+        accountID: str = ...,
         associateDefaultSecurityGroup: bool = ...,
         bandwidthThrottling: int = ...,
         createPublicIP: bool = ...,
         dataPlaneRouting: ReplicationConfigurationDataPlaneRoutingType = ...,
         defaultLargeStagingDiskType: ReplicationConfigurationDefaultLargeStagingDiskTypeType = ...,
         ebsEncryption: ReplicationConfigurationEbsEncryptionType = ...,
         ebsEncryptionKeyArn: str = ...,
         name: str = ...,
         replicatedDisks: Sequence[ReplicationConfigurationReplicatedDiskTypeDef] = ...,
         replicationServerInstanceType: str = ...,
         replicationServersSecurityGroupsIDs: Sequence[str] = ...,
         stagingAreaSubnetId: str = ...,
         stagingAreaTags: Mapping[str, str] = ...,
-        useDedicatedReplicationServer: bool = ...
+        useDedicatedReplicationServer: bool = ...,
+        useFipsEndpoint: bool = ...
     ) -> ReplicationConfigurationTypeDef:
         """
         Allows you to update multiple ReplicationConfigurations by Source Server ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_replication_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#update_replication_configuration)
         """
@@ -886,36 +969,37 @@
         defaultLargeStagingDiskType: ReplicationConfigurationDefaultLargeStagingDiskTypeType = ...,
         ebsEncryption: ReplicationConfigurationEbsEncryptionType = ...,
         ebsEncryptionKeyArn: str = ...,
         replicationServerInstanceType: str = ...,
         replicationServersSecurityGroupsIDs: Sequence[str] = ...,
         stagingAreaSubnetId: str = ...,
         stagingAreaTags: Mapping[str, str] = ...,
-        useDedicatedReplicationServer: bool = ...
+        useDedicatedReplicationServer: bool = ...,
+        useFipsEndpoint: bool = ...
     ) -> ReplicationConfigurationTemplateResponseTypeDef:
         """
         Updates multiple ReplicationConfigurationTemplates by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_replication_configuration_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#update_replication_configuration_template)
         """
 
     async def update_source_server_replication_type(
-        self, *, replicationType: ReplicationTypeType, sourceServerID: str
+        self, *, replicationType: ReplicationTypeType, sourceServerID: str, accountID: str = ...
     ) -> SourceServerResponseTypeDef:
         """
         Allows you to change between the AGENT_BASED replication type and the
         SNAPSHOT_SHIPPING replication type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_source_server_replication_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#update_source_server_replication_type)
         """
 
     async def update_wave(
-        self, *, waveID: str, description: str = ..., name: str = ...
+        self, *, waveID: str, accountID: str = ..., description: str = ..., name: str = ...
     ) -> WaveResponseTypeDef:
         """
         Update wave.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_wave)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#update_wave)
         """
@@ -1011,14 +1095,23 @@
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#get_paginator)
         """
 
     @overload
     def get_paginator(
+        self, operation_name: Literal["list_managed_accounts"]
+    ) -> ListManagedAccountsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.get_paginator)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(
         self, operation_name: Literal["list_source_server_actions"]
     ) -> ListSourceServerActionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#get_paginator)
         """
```

### Comparing `types-aiobotocore-mgn-2.5.2.post1/types_aiobotocore_mgn/client.pyi` & `types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn/client.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     DescribeSourceServersPaginator,
     DescribeVcenterClientsPaginator,
     ListApplicationsPaginator,
     ListExportErrorsPaginator,
     ListExportsPaginator,
     ListImportErrorsPaginator,
     ListImportsPaginator,
+    ListManagedAccountsPaginator,
     ListSourceServerActionsPaginator,
     ListTemplateActionsPaginator,
     ListWavesPaginator,
 )
 from .type_defs import (
     ApplicationResponseTypeDef,
     ChangeServerLifeCycleStateSourceServerLifecycleTypeDef,
@@ -66,20 +67,21 @@
     ListApplicationsResponseTypeDef,
     ListExportErrorsResponseTypeDef,
     ListExportsRequestFiltersTypeDef,
     ListExportsResponseTypeDef,
     ListImportErrorsResponseTypeDef,
     ListImportsRequestFiltersTypeDef,
     ListImportsResponseTypeDef,
+    ListManagedAccountsResponseTypeDef,
     ListSourceServerActionsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTemplateActionsResponseTypeDef,
     ListWavesRequestFiltersTypeDef,
     ListWavesResponseTypeDef,
-    PostLaunchActionsUnionTypeDef,
+    PostLaunchActionsTypeDef,
     ReplicationConfigurationReplicatedDiskTypeDef,
     ReplicationConfigurationTemplateResponseTypeDef,
     ReplicationConfigurationTypeDef,
     S3BucketSourceTypeDef,
     SourceServerActionDocumentResponseTypeDef,
     SourceServerActionsRequestFiltersTypeDef,
     SourceServerResponseTypeDef,
@@ -132,39 +134,41 @@
     def exceptions(self) -> Exceptions:
         """
         mgnClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#exceptions)
         """
-    async def archive_application(self, *, applicationID: str) -> ApplicationResponseTypeDef:
+    async def archive_application(
+        self, *, applicationID: str, accountID: str = ...
+    ) -> ApplicationResponseTypeDef:
         """
         Archive application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.archive_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#archive_application)
         """
-    async def archive_wave(self, *, waveID: str) -> WaveResponseTypeDef:
+    async def archive_wave(self, *, waveID: str, accountID: str = ...) -> WaveResponseTypeDef:
         """
         Archive wave.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.archive_wave)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#archive_wave)
         """
     async def associate_applications(
-        self, *, applicationIDs: Sequence[str], waveID: str
+        self, *, applicationIDs: Sequence[str], waveID: str, accountID: str = ...
     ) -> Dict[str, Any]:
         """
         Associate applications to wave.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.associate_applications)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#associate_applications)
         """
     async def associate_source_servers(
-        self, *, applicationID: str, sourceServerIDs: Sequence[str]
+        self, *, applicationID: str, sourceServerIDs: Sequence[str], accountID: str = ...
     ) -> Dict[str, Any]:
         """
         Associate source servers to application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.associate_source_servers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#associate_source_servers)
         """
@@ -175,15 +179,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#can_paginate)
         """
     async def change_server_life_cycle_state(
         self,
         *,
         lifeCycle: ChangeServerLifeCycleStateSourceServerLifecycleTypeDef,
-        sourceServerID: str
+        sourceServerID: str,
+        accountID: str = ...
     ) -> SourceServerResponseTypeDef:
         """
         Allows the user to set the SourceServer.LifeCycle.state property for specific
         Source Server IDs to one of the following: READY_FOR_TEST or READY_FOR_CUTOVER.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.change_server_life_cycle_state)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#change_server_life_cycle_state)
@@ -192,15 +197,20 @@
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#close)
         """
     async def create_application(
-        self, *, name: str, description: str = ..., tags: Mapping[str, str] = ...
+        self,
+        *,
+        name: str,
+        accountID: str = ...,
+        description: str = ...,
+        tags: Mapping[str, str] = ...
     ) -> ApplicationResponseTypeDef:
         """
         Create application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.create_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#create_application)
         """
@@ -212,15 +222,15 @@
         copyPrivateIp: bool = ...,
         copyTags: bool = ...,
         enableMapAutoTagging: bool = ...,
         largeVolumeConf: LaunchTemplateDiskConfTypeDef = ...,
         launchDisposition: LaunchDispositionType = ...,
         licensing: LicensingTypeDef = ...,
         mapAutoTaggingMpeID: str = ...,
-        postLaunchActions: PostLaunchActionsUnionTypeDef = ...,
+        postLaunchActions: PostLaunchActionsTypeDef = ...,
         smallVolumeConf: LaunchTemplateDiskConfTypeDef = ...,
         smallVolumeMaxSize: int = ...,
         tags: Mapping[str, str] = ...,
         targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType = ...
     ) -> LaunchConfigurationTemplateResponseTypeDef:
         """
         Creates a new Launch Configuration Template.
@@ -239,39 +249,47 @@
         ebsEncryption: ReplicationConfigurationEbsEncryptionType,
         replicationServerInstanceType: str,
         replicationServersSecurityGroupsIDs: Sequence[str],
         stagingAreaSubnetId: str,
         stagingAreaTags: Mapping[str, str],
         useDedicatedReplicationServer: bool,
         ebsEncryptionKeyArn: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
+        useFipsEndpoint: bool = ...
     ) -> ReplicationConfigurationTemplateResponseTypeDef:
         """
         Creates a new ReplicationConfigurationTemplate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.create_replication_configuration_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#create_replication_configuration_template)
         """
     async def create_wave(
-        self, *, name: str, description: str = ..., tags: Mapping[str, str] = ...
+        self,
+        *,
+        name: str,
+        accountID: str = ...,
+        description: str = ...,
+        tags: Mapping[str, str] = ...
     ) -> WaveResponseTypeDef:
         """
         Create wave.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.create_wave)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#create_wave)
         """
-    async def delete_application(self, *, applicationID: str) -> Dict[str, Any]:
+    async def delete_application(
+        self, *, applicationID: str, accountID: str = ...
+    ) -> Dict[str, Any]:
         """
         Delete application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.delete_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#delete_application)
         """
-    async def delete_job(self, *, jobID: str) -> Dict[str, Any]:
+    async def delete_job(self, *, jobID: str, accountID: str = ...) -> Dict[str, Any]:
         """
         Deletes a single Job by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.delete_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#delete_job)
         """
     async def delete_launch_configuration_template(
@@ -289,47 +307,50 @@
         """
         Deletes a single Replication Configuration Template by ID See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/mgn-2020-02-26/DeleteReplicationConfigurationTemplate).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.delete_replication_configuration_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#delete_replication_configuration_template)
         """
-    async def delete_source_server(self, *, sourceServerID: str) -> Dict[str, Any]:
+    async def delete_source_server(
+        self, *, sourceServerID: str, accountID: str = ...
+    ) -> Dict[str, Any]:
         """
         Deletes a single source server by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.delete_source_server)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#delete_source_server)
         """
     async def delete_vcenter_client(self, *, vcenterClientID: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a given vCenter client by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.delete_vcenter_client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#delete_vcenter_client)
         """
-    async def delete_wave(self, *, waveID: str) -> Dict[str, Any]:
+    async def delete_wave(self, *, waveID: str, accountID: str = ...) -> Dict[str, Any]:
         """
         Delete wave.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.delete_wave)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#delete_wave)
         """
     async def describe_job_log_items(
-        self, *, jobID: str, maxResults: int = ..., nextToken: str = ...
+        self, *, jobID: str, accountID: str = ..., maxResults: int = ..., nextToken: str = ...
     ) -> DescribeJobLogItemsResponseTypeDef:
         """
         Retrieves detailed job log items with paging.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.describe_job_log_items)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#describe_job_log_items)
         """
     async def describe_jobs(
         self,
         *,
+        accountID: str = ...,
         filters: DescribeJobsRequestFiltersTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> DescribeJobsResponseTypeDef:
         """
         Returns a list of Jobs.
 
@@ -363,14 +384,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.describe_replication_configuration_templates)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#describe_replication_configuration_templates)
         """
     async def describe_source_servers(
         self,
         *,
+        accountID: str = ...,
         filters: DescribeSourceServersRequestFiltersTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> DescribeSourceServersResponseTypeDef:
         """
         Retrieves all SourceServers or multiple SourceServers by ID.
 
@@ -383,39 +405,43 @@
         """
         Returns a list of the installed vCenter clients.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.describe_vcenter_clients)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#describe_vcenter_clients)
         """
     async def disassociate_applications(
-        self, *, applicationIDs: Sequence[str], waveID: str
+        self, *, applicationIDs: Sequence[str], waveID: str, accountID: str = ...
     ) -> Dict[str, Any]:
         """
         Disassociate applications from wave.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.disassociate_applications)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#disassociate_applications)
         """
     async def disassociate_source_servers(
-        self, *, applicationID: str, sourceServerIDs: Sequence[str]
+        self, *, applicationID: str, sourceServerIDs: Sequence[str], accountID: str = ...
     ) -> Dict[str, Any]:
         """
         Disassociate source servers from application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.disassociate_source_servers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#disassociate_source_servers)
         """
-    async def disconnect_from_service(self, *, sourceServerID: str) -> SourceServerResponseTypeDef:
+    async def disconnect_from_service(
+        self, *, sourceServerID: str, accountID: str = ...
+    ) -> SourceServerResponseTypeDef:
         """
         Disconnects specific Source Servers from Application Migration Service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.disconnect_from_service)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#disconnect_from_service)
         """
-    async def finalize_cutover(self, *, sourceServerID: str) -> SourceServerResponseTypeDef:
+    async def finalize_cutover(
+        self, *, sourceServerID: str, accountID: str = ...
+    ) -> SourceServerResponseTypeDef:
         """
         Finalizes the cutover immediately for specific Source Servers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.finalize_cutover)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#finalize_cutover)
         """
     async def generate_presigned_url(
@@ -427,23 +453,25 @@
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#generate_presigned_url)
         """
-    async def get_launch_configuration(self, *, sourceServerID: str) -> LaunchConfigurationTypeDef:
+    async def get_launch_configuration(
+        self, *, sourceServerID: str, accountID: str = ...
+    ) -> LaunchConfigurationTypeDef:
         """
         Lists all LaunchConfigurations available, filtered by Source Server IDs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.get_launch_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#get_launch_configuration)
         """
     async def get_replication_configuration(
-        self, *, sourceServerID: str
+        self, *, sourceServerID: str, accountID: str = ...
     ) -> ReplicationConfigurationTypeDef:
         """
         Lists all ReplicationConfigurations, filtered by Source Server ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.get_replication_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#get_replication_configuration)
         """
@@ -453,14 +481,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.initialize_service)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#initialize_service)
         """
     async def list_applications(
         self,
         *,
+        accountID: str = ...,
         filters: ListApplicationsRequestFiltersTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListApplicationsResponseTypeDef:
         """
         Retrieves all applications or multiple applications by ID.
 
@@ -507,18 +536,28 @@
     ) -> ListImportsResponseTypeDef:
         """
         List imports.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.list_imports)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#list_imports)
         """
+    async def list_managed_accounts(
+        self, *, maxResults: int = ..., nextToken: str = ...
+    ) -> ListManagedAccountsResponseTypeDef:
+        """
+        List Managed Accounts.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.list_managed_accounts)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#list_managed_accounts)
+        """
     async def list_source_server_actions(
         self,
         *,
         sourceServerID: str,
+        accountID: str = ...,
         filters: SourceServerActionsRequestFiltersTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListSourceServerActionsResponseTypeDef:
         """
         List source server post migration custom actions.
 
@@ -547,40 +586,53 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.list_template_actions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#list_template_actions)
         """
     async def list_waves(
         self,
         *,
+        accountID: str = ...,
         filters: ListWavesRequestFiltersTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListWavesResponseTypeDef:
         """
         Retrieves all waves or multiple waves by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.list_waves)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#list_waves)
         """
-    async def mark_as_archived(self, *, sourceServerID: str) -> SourceServerResponseTypeDef:
+    async def mark_as_archived(
+        self, *, sourceServerID: str, accountID: str = ...
+    ) -> SourceServerResponseTypeDef:
         """
         Archives specific Source Servers by setting the SourceServer.isArchived property
         to true for specified SourceServers by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.mark_as_archived)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#mark_as_archived)
         """
+    async def pause_replication(
+        self, *, sourceServerID: str, accountID: str = ...
+    ) -> SourceServerResponseTypeDef:
+        """
+        Pause Replication.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.pause_replication)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#pause_replication)
+        """
     async def put_source_server_action(
         self,
         *,
         actionID: str,
         actionName: str,
         documentIdentifier: str,
         order: int,
         sourceServerID: str,
+        accountID: str = ...,
         active: bool = ...,
         category: ActionCategoryType = ...,
         description: str = ...,
         documentVersion: str = ...,
         externalParameters: Mapping[str, SsmExternalParameterTypeDef] = ...,
         mustSucceedForCutover: bool = ...,
         parameters: Mapping[str, Sequence[SsmParameterStoreParameterTypeDef]] = ...,
@@ -613,15 +665,15 @@
         """
         Put template post migration custom action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.put_template_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#put_template_action)
         """
     async def remove_source_server_action(
-        self, *, actionID: str, sourceServerID: str
+        self, *, actionID: str, sourceServerID: str, accountID: str = ...
     ) -> Dict[str, Any]:
         """
         Remove source server post migration custom action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.remove_source_server_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#remove_source_server_action)
         """
@@ -630,25 +682,36 @@
     ) -> Dict[str, Any]:
         """
         Remove template post migration custom action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.remove_template_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#remove_template_action)
         """
-    async def retry_data_replication(self, *, sourceServerID: str) -> SourceServerResponseTypeDef:
+    async def resume_replication(
+        self, *, sourceServerID: str, accountID: str = ...
+    ) -> SourceServerResponseTypeDef:
+        """
+        Resume Replication.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.resume_replication)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#resume_replication)
+        """
+    async def retry_data_replication(
+        self, *, sourceServerID: str, accountID: str = ...
+    ) -> SourceServerResponseTypeDef:
         """
         Causes the data replication initiation sequence to begin immediately upon next
         Handshake for specified SourceServer IDs, regardless of when the previous
         initiation started.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.retry_data_replication)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#retry_data_replication)
         """
     async def start_cutover(
-        self, *, sourceServerIDs: Sequence[str], tags: Mapping[str, str] = ...
+        self, *, sourceServerIDs: Sequence[str], accountID: str = ..., tags: Mapping[str, str] = ...
     ) -> StartCutoverResponseTypeDef:
         """
         Launches a Cutover Instance for specific Source Servers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.start_cutover)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#start_cutover)
         """
@@ -666,57 +729,70 @@
     ) -> StartImportResponseTypeDef:
         """
         Start import.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.start_import)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#start_import)
         """
-    async def start_replication(self, *, sourceServerID: str) -> SourceServerResponseTypeDef:
+    async def start_replication(
+        self, *, sourceServerID: str, accountID: str = ...
+    ) -> SourceServerResponseTypeDef:
         """
         Starts replication for SNAPSHOT_SHIPPING agents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.start_replication)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#start_replication)
         """
     async def start_test(
-        self, *, sourceServerIDs: Sequence[str], tags: Mapping[str, str] = ...
+        self, *, sourceServerIDs: Sequence[str], accountID: str = ..., tags: Mapping[str, str] = ...
     ) -> StartTestResponseTypeDef:
         """
         Launches a Test Instance for specific Source Servers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.start_test)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#start_test)
         """
+    async def stop_replication(
+        self, *, sourceServerID: str, accountID: str = ...
+    ) -> SourceServerResponseTypeDef:
+        """
+        Stop Replication.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.stop_replication)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#stop_replication)
+        """
     async def tag_resource(
         self, *, resourceArn: str, tags: Mapping[str, str]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Adds or overwrites only the specified tags for the specified Application
         Migration Service resource or resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#tag_resource)
         """
     async def terminate_target_instances(
-        self, *, sourceServerIDs: Sequence[str], tags: Mapping[str, str] = ...
+        self, *, sourceServerIDs: Sequence[str], accountID: str = ..., tags: Mapping[str, str] = ...
     ) -> TerminateTargetInstancesResponseTypeDef:
         """
         Starts a job that terminates specific launched EC2 Test and Cutover instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.terminate_target_instances)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#terminate_target_instances)
         """
-    async def unarchive_application(self, *, applicationID: str) -> ApplicationResponseTypeDef:
+    async def unarchive_application(
+        self, *, applicationID: str, accountID: str = ...
+    ) -> ApplicationResponseTypeDef:
         """
         Unarchive application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.unarchive_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#unarchive_application)
         """
-    async def unarchive_wave(self, *, waveID: str) -> WaveResponseTypeDef:
+    async def unarchive_wave(self, *, waveID: str, accountID: str = ...) -> WaveResponseTypeDef:
         """
         Unarchive wave.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.unarchive_wave)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#unarchive_wave)
         """
     async def untag_resource(
@@ -726,35 +802,36 @@
         Deletes the specified set of tags from the specified set of Application
         Migration Service resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#untag_resource)
         """
     async def update_application(
-        self, *, applicationID: str, description: str = ..., name: str = ...
+        self, *, applicationID: str, accountID: str = ..., description: str = ..., name: str = ...
     ) -> ApplicationResponseTypeDef:
         """
         Update application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#update_application)
         """
     async def update_launch_configuration(
         self,
         *,
         sourceServerID: str,
+        accountID: str = ...,
         bootMode: BootModeType = ...,
         copyPrivateIp: bool = ...,
         copyTags: bool = ...,
         enableMapAutoTagging: bool = ...,
         launchDisposition: LaunchDispositionType = ...,
         licensing: LicensingTypeDef = ...,
         mapAutoTaggingMpeID: str = ...,
         name: str = ...,
-        postLaunchActions: PostLaunchActionsUnionTypeDef = ...,
+        postLaunchActions: PostLaunchActionsTypeDef = ...,
         targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType = ...
     ) -> LaunchConfigurationTypeDef:
         """
         Updates multiple LaunchConfigurations by Source Server ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_launch_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#update_launch_configuration)
@@ -768,43 +845,45 @@
         copyPrivateIp: bool = ...,
         copyTags: bool = ...,
         enableMapAutoTagging: bool = ...,
         largeVolumeConf: LaunchTemplateDiskConfTypeDef = ...,
         launchDisposition: LaunchDispositionType = ...,
         licensing: LicensingTypeDef = ...,
         mapAutoTaggingMpeID: str = ...,
-        postLaunchActions: PostLaunchActionsUnionTypeDef = ...,
+        postLaunchActions: PostLaunchActionsTypeDef = ...,
         smallVolumeConf: LaunchTemplateDiskConfTypeDef = ...,
         smallVolumeMaxSize: int = ...,
         targetInstanceTypeRightSizingMethod: TargetInstanceTypeRightSizingMethodType = ...
     ) -> LaunchConfigurationTemplateResponseTypeDef:
         """
         Updates an existing Launch Configuration Template by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_launch_configuration_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#update_launch_configuration_template)
         """
     async def update_replication_configuration(
         self,
         *,
         sourceServerID: str,
+        accountID: str = ...,
         associateDefaultSecurityGroup: bool = ...,
         bandwidthThrottling: int = ...,
         createPublicIP: bool = ...,
         dataPlaneRouting: ReplicationConfigurationDataPlaneRoutingType = ...,
         defaultLargeStagingDiskType: ReplicationConfigurationDefaultLargeStagingDiskTypeType = ...,
         ebsEncryption: ReplicationConfigurationEbsEncryptionType = ...,
         ebsEncryptionKeyArn: str = ...,
         name: str = ...,
         replicatedDisks: Sequence[ReplicationConfigurationReplicatedDiskTypeDef] = ...,
         replicationServerInstanceType: str = ...,
         replicationServersSecurityGroupsIDs: Sequence[str] = ...,
         stagingAreaSubnetId: str = ...,
         stagingAreaTags: Mapping[str, str] = ...,
-        useDedicatedReplicationServer: bool = ...
+        useDedicatedReplicationServer: bool = ...,
+        useFipsEndpoint: bool = ...
     ) -> ReplicationConfigurationTypeDef:
         """
         Allows you to update multiple ReplicationConfigurations by Source Server ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_replication_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#update_replication_configuration)
         """
@@ -820,34 +899,35 @@
         defaultLargeStagingDiskType: ReplicationConfigurationDefaultLargeStagingDiskTypeType = ...,
         ebsEncryption: ReplicationConfigurationEbsEncryptionType = ...,
         ebsEncryptionKeyArn: str = ...,
         replicationServerInstanceType: str = ...,
         replicationServersSecurityGroupsIDs: Sequence[str] = ...,
         stagingAreaSubnetId: str = ...,
         stagingAreaTags: Mapping[str, str] = ...,
-        useDedicatedReplicationServer: bool = ...
+        useDedicatedReplicationServer: bool = ...,
+        useFipsEndpoint: bool = ...
     ) -> ReplicationConfigurationTemplateResponseTypeDef:
         """
         Updates multiple ReplicationConfigurationTemplates by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_replication_configuration_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#update_replication_configuration_template)
         """
     async def update_source_server_replication_type(
-        self, *, replicationType: ReplicationTypeType, sourceServerID: str
+        self, *, replicationType: ReplicationTypeType, sourceServerID: str, accountID: str = ...
     ) -> SourceServerResponseTypeDef:
         """
         Allows you to change between the AGENT_BASED replication type and the
         SNAPSHOT_SHIPPING replication type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_source_server_replication_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#update_source_server_replication_type)
         """
     async def update_wave(
-        self, *, waveID: str, description: str = ..., name: str = ...
+        self, *, waveID: str, accountID: str = ..., description: str = ..., name: str = ...
     ) -> WaveResponseTypeDef:
         """
         Update wave.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.update_wave)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#update_wave)
         """
@@ -931,14 +1011,22 @@
     def get_paginator(self, operation_name: Literal["list_imports"]) -> ListImportsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#get_paginator)
         """
     @overload
     def get_paginator(
+        self, operation_name: Literal["list_managed_accounts"]
+    ) -> ListManagedAccountsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.get_paginator)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#get_paginator)
+        """
+    @overload
+    def get_paginator(
         self, operation_name: Literal["list_source_server_actions"]
     ) -> ListSourceServerActionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/client/#get_paginator)
         """
     @overload
```

### Comparing `types-aiobotocore-mgn-2.5.2.post1/types_aiobotocore_mgn/literals.py` & `types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
     "LaunchStatusType",
     "LifeCycleStateType",
     "ListApplicationsPaginatorName",
     "ListExportErrorsPaginatorName",
     "ListExportsPaginatorName",
     "ListImportErrorsPaginatorName",
     "ListImportsPaginatorName",
+    "ListManagedAccountsPaginatorName",
     "ListSourceServerActionsPaginatorName",
     "ListTemplateActionsPaginatorName",
     "ListWavesPaginatorName",
     "PostLaunchActionExecutionStatusType",
     "PostLaunchActionsDeploymentTypeType",
     "ReplicationConfigurationDataPlaneRoutingType",
     "ReplicationConfigurationDefaultLargeStagingDiskTypeType",
@@ -191,14 +192,15 @@
     "TESTING",
 ]
 ListApplicationsPaginatorName = Literal["list_applications"]
 ListExportErrorsPaginatorName = Literal["list_export_errors"]
 ListExportsPaginatorName = Literal["list_exports"]
 ListImportErrorsPaginatorName = Literal["list_import_errors"]
 ListImportsPaginatorName = Literal["list_imports"]
+ListManagedAccountsPaginatorName = Literal["list_managed_accounts"]
 ListSourceServerActionsPaginatorName = Literal["list_source_server_actions"]
 ListTemplateActionsPaginatorName = Literal["list_template_actions"]
 ListWavesPaginatorName = Literal["list_waves"]
 PostLaunchActionExecutionStatusType = Literal["FAILED", "IN_PROGRESS", "SUCCESS"]
 PostLaunchActionsDeploymentTypeType = Literal["CUTOVER_ONLY", "TEST_AND_CUTOVER", "TEST_ONLY"]
 ReplicationConfigurationDataPlaneRoutingType = Literal["PRIVATE_IP", "PUBLIC_IP"]
 ReplicationConfigurationDefaultLargeStagingDiskTypeType = Literal["GP2", "GP3", "ST1"]
@@ -225,14 +227,15 @@
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
@@ -328,14 +331,15 @@
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
@@ -414,26 +418,28 @@
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
@@ -585,14 +591,15 @@
     "describe_source_servers",
     "describe_vcenter_clients",
     "list_applications",
     "list_export_errors",
     "list_exports",
     "list_import_errors",
     "list_imports",
+    "list_managed_accounts",
     "list_source_server_actions",
     "list_template_actions",
     "list_waves",
 ]
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
```

### Comparing `types-aiobotocore-mgn-2.5.2.post1/types_aiobotocore_mgn/literals.pyi` & `types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     "LaunchStatusType",
     "LifeCycleStateType",
     "ListApplicationsPaginatorName",
     "ListExportErrorsPaginatorName",
     "ListExportsPaginatorName",
     "ListImportErrorsPaginatorName",
     "ListImportsPaginatorName",
+    "ListManagedAccountsPaginatorName",
     "ListSourceServerActionsPaginatorName",
     "ListTemplateActionsPaginatorName",
     "ListWavesPaginatorName",
     "PostLaunchActionExecutionStatusType",
     "PostLaunchActionsDeploymentTypeType",
     "ReplicationConfigurationDataPlaneRoutingType",
     "ReplicationConfigurationDefaultLargeStagingDiskTypeType",
@@ -189,14 +190,15 @@
     "TESTING",
 ]
 ListApplicationsPaginatorName = Literal["list_applications"]
 ListExportErrorsPaginatorName = Literal["list_export_errors"]
 ListExportsPaginatorName = Literal["list_exports"]
 ListImportErrorsPaginatorName = Literal["list_import_errors"]
 ListImportsPaginatorName = Literal["list_imports"]
+ListManagedAccountsPaginatorName = Literal["list_managed_accounts"]
 ListSourceServerActionsPaginatorName = Literal["list_source_server_actions"]
 ListTemplateActionsPaginatorName = Literal["list_template_actions"]
 ListWavesPaginatorName = Literal["list_waves"]
 PostLaunchActionExecutionStatusType = Literal["FAILED", "IN_PROGRESS", "SUCCESS"]
 PostLaunchActionsDeploymentTypeType = Literal["CUTOVER_ONLY", "TEST_AND_CUTOVER", "TEST_ONLY"]
 ReplicationConfigurationDataPlaneRoutingType = Literal["PRIVATE_IP", "PUBLIC_IP"]
 ReplicationConfigurationDefaultLargeStagingDiskTypeType = Literal["GP2", "GP3", "ST1"]
@@ -223,14 +225,15 @@
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
@@ -326,14 +329,15 @@
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
@@ -412,26 +416,28 @@
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
@@ -583,14 +589,15 @@
     "describe_source_servers",
     "describe_vcenter_clients",
     "list_applications",
     "list_export_errors",
     "list_exports",
     "list_import_errors",
     "list_imports",
+    "list_managed_accounts",
     "list_source_server_actions",
     "list_template_actions",
     "list_waves",
 ]
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
```

### Comparing `types-aiobotocore-mgn-2.5.2.post1/types_aiobotocore_mgn/paginator.py` & `types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
         DescribeSourceServersPaginator,
         DescribeVcenterClientsPaginator,
         ListApplicationsPaginator,
         ListExportErrorsPaginator,
         ListExportsPaginator,
         ListImportErrorsPaginator,
         ListImportsPaginator,
+        ListManagedAccountsPaginator,
         ListSourceServerActionsPaginator,
         ListTemplateActionsPaginator,
         ListWavesPaginator,
     )
 
     session = get_session()
     with session.create_client("mgn") as client:
@@ -37,14 +38,15 @@
         describe_source_servers_paginator: DescribeSourceServersPaginator = client.get_paginator("describe_source_servers")
         describe_vcenter_clients_paginator: DescribeVcenterClientsPaginator = client.get_paginator("describe_vcenter_clients")
         list_applications_paginator: ListApplicationsPaginator = client.get_paginator("list_applications")
         list_export_errors_paginator: ListExportErrorsPaginator = client.get_paginator("list_export_errors")
         list_exports_paginator: ListExportsPaginator = client.get_paginator("list_exports")
         list_import_errors_paginator: ListImportErrorsPaginator = client.get_paginator("list_import_errors")
         list_imports_paginator: ListImportsPaginator = client.get_paginator("list_imports")
+        list_managed_accounts_paginator: ListManagedAccountsPaginator = client.get_paginator("list_managed_accounts")
         list_source_server_actions_paginator: ListSourceServerActionsPaginator = client.get_paginator("list_source_server_actions")
         list_template_actions_paginator: ListTemplateActionsPaginator = client.get_paginator("list_template_actions")
         list_waves_paginator: ListWavesPaginator = client.get_paginator("list_waves")
     ```
 """
 from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar
 
@@ -64,14 +66,15 @@
     ListApplicationsResponseTypeDef,
     ListExportErrorsResponseTypeDef,
     ListExportsRequestFiltersTypeDef,
     ListExportsResponseTypeDef,
     ListImportErrorsResponseTypeDef,
     ListImportsRequestFiltersTypeDef,
     ListImportsResponseTypeDef,
+    ListManagedAccountsResponseTypeDef,
     ListSourceServerActionsResponseTypeDef,
     ListTemplateActionsResponseTypeDef,
     ListWavesRequestFiltersTypeDef,
     ListWavesResponseTypeDef,
     PaginatorConfigTypeDef,
     SourceServerActionsRequestFiltersTypeDef,
     TemplateActionsRequestFiltersTypeDef,
@@ -85,14 +88,15 @@
     "DescribeSourceServersPaginator",
     "DescribeVcenterClientsPaginator",
     "ListApplicationsPaginator",
     "ListExportErrorsPaginator",
     "ListExportsPaginator",
     "ListImportErrorsPaginator",
     "ListImportsPaginator",
+    "ListManagedAccountsPaginator",
     "ListSourceServerActionsPaginator",
     "ListTemplateActionsPaginator",
     "ListWavesPaginator",
 )
 
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
@@ -108,15 +112,15 @@
 class DescribeJobLogItemsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeJobLogItems)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/paginators/#describejoblogitemspaginator)
     """
 
     def paginate(
-        self, *, jobID: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, jobID: str, accountID: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeJobLogItemsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeJobLogItems.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/paginators/#describejoblogitemspaginator)
         """
 
 
@@ -125,14 +129,15 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeJobs)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/paginators/#describejobspaginator)
     """
 
     def paginate(
         self,
         *,
+        accountID: str = ...,
         filters: DescribeJobsRequestFiltersTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/paginators/#describejobspaginator)
         """
@@ -179,14 +184,15 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeSourceServers)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/paginators/#describesourceserverspaginator)
     """
 
     def paginate(
         self,
         *,
+        accountID: str = ...,
         filters: DescribeSourceServersRequestFiltersTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeSourceServersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeSourceServers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/paginators/#describesourceserverspaginator)
         """
@@ -212,14 +218,15 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListApplications)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/paginators/#listapplicationspaginator)
     """
 
     def paginate(
         self,
         *,
+        accountID: str = ...,
         filters: ListApplicationsRequestFiltersTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListApplications.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/paginators/#listapplicationspaginator)
         """
@@ -287,24 +294,40 @@
     ) -> AsyncIterator[ListImportsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListImports.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/paginators/#listimportspaginator)
         """
 
 
+class ListManagedAccountsPaginator(AioPaginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListManagedAccounts)
+    [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/paginators/#listmanagedaccountspaginator)
+    """
+
+    def paginate(
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+    ) -> AsyncIterator[ListManagedAccountsResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListManagedAccounts.paginate)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/paginators/#listmanagedaccountspaginator)
+        """
+
+
 class ListSourceServerActionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListSourceServerActions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/paginators/#listsourceserveractionspaginator)
     """
 
     def paginate(
         self,
         *,
         sourceServerID: str,
+        accountID: str = ...,
         filters: SourceServerActionsRequestFiltersTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSourceServerActionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListSourceServerActions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/paginators/#listsourceserveractionspaginator)
         """
@@ -334,14 +357,15 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListWaves)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/paginators/#listwavespaginator)
     """
 
     def paginate(
         self,
         *,
+        accountID: str = ...,
         filters: ListWavesRequestFiltersTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListWavesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListWaves.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/paginators/#listwavespaginator)
         """
```

### Comparing `types-aiobotocore-mgn-2.5.2.post1/types_aiobotocore_mgn/paginator.pyi` & `types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
         DescribeSourceServersPaginator,
         DescribeVcenterClientsPaginator,
         ListApplicationsPaginator,
         ListExportErrorsPaginator,
         ListExportsPaginator,
         ListImportErrorsPaginator,
         ListImportsPaginator,
+        ListManagedAccountsPaginator,
         ListSourceServerActionsPaginator,
         ListTemplateActionsPaginator,
         ListWavesPaginator,
     )
 
     session = get_session()
     with session.create_client("mgn") as client:
@@ -37,14 +38,15 @@
         describe_source_servers_paginator: DescribeSourceServersPaginator = client.get_paginator("describe_source_servers")
         describe_vcenter_clients_paginator: DescribeVcenterClientsPaginator = client.get_paginator("describe_vcenter_clients")
         list_applications_paginator: ListApplicationsPaginator = client.get_paginator("list_applications")
         list_export_errors_paginator: ListExportErrorsPaginator = client.get_paginator("list_export_errors")
         list_exports_paginator: ListExportsPaginator = client.get_paginator("list_exports")
         list_import_errors_paginator: ListImportErrorsPaginator = client.get_paginator("list_import_errors")
         list_imports_paginator: ListImportsPaginator = client.get_paginator("list_imports")
+        list_managed_accounts_paginator: ListManagedAccountsPaginator = client.get_paginator("list_managed_accounts")
         list_source_server_actions_paginator: ListSourceServerActionsPaginator = client.get_paginator("list_source_server_actions")
         list_template_actions_paginator: ListTemplateActionsPaginator = client.get_paginator("list_template_actions")
         list_waves_paginator: ListWavesPaginator = client.get_paginator("list_waves")
     ```
 """
 from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar
 
@@ -64,14 +66,15 @@
     ListApplicationsResponseTypeDef,
     ListExportErrorsResponseTypeDef,
     ListExportsRequestFiltersTypeDef,
     ListExportsResponseTypeDef,
     ListImportErrorsResponseTypeDef,
     ListImportsRequestFiltersTypeDef,
     ListImportsResponseTypeDef,
+    ListManagedAccountsResponseTypeDef,
     ListSourceServerActionsResponseTypeDef,
     ListTemplateActionsResponseTypeDef,
     ListWavesRequestFiltersTypeDef,
     ListWavesResponseTypeDef,
     PaginatorConfigTypeDef,
     SourceServerActionsRequestFiltersTypeDef,
     TemplateActionsRequestFiltersTypeDef,
@@ -85,14 +88,15 @@
     "DescribeSourceServersPaginator",
     "DescribeVcenterClientsPaginator",
     "ListApplicationsPaginator",
     "ListExportErrorsPaginator",
     "ListExportsPaginator",
     "ListImportErrorsPaginator",
     "ListImportsPaginator",
+    "ListManagedAccountsPaginator",
     "ListSourceServerActionsPaginator",
     "ListTemplateActionsPaginator",
     "ListWavesPaginator",
 )
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
@@ -105,15 +109,15 @@
 class DescribeJobLogItemsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeJobLogItems)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/paginators/#describejoblogitemspaginator)
     """
 
     def paginate(
-        self, *, jobID: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, jobID: str, accountID: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeJobLogItemsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeJobLogItems.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/paginators/#describejoblogitemspaginator)
         """
 
 class DescribeJobsPaginator(AioPaginator):
@@ -121,14 +125,15 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeJobs)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/paginators/#describejobspaginator)
     """
 
     def paginate(
         self,
         *,
+        accountID: str = ...,
         filters: DescribeJobsRequestFiltersTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/paginators/#describejobspaginator)
         """
@@ -172,14 +177,15 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeSourceServers)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/paginators/#describesourceserverspaginator)
     """
 
     def paginate(
         self,
         *,
+        accountID: str = ...,
         filters: DescribeSourceServersRequestFiltersTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeSourceServersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeSourceServers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/paginators/#describesourceserverspaginator)
         """
@@ -203,14 +209,15 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListApplications)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/paginators/#listapplicationspaginator)
     """
 
     def paginate(
         self,
         *,
+        accountID: str = ...,
         filters: ListApplicationsRequestFiltersTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListApplications.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/paginators/#listapplicationspaginator)
         """
@@ -273,24 +280,39 @@
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListImportsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListImports.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/paginators/#listimportspaginator)
         """
 
+class ListManagedAccountsPaginator(AioPaginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListManagedAccounts)
+    [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/paginators/#listmanagedaccountspaginator)
+    """
+
+    def paginate(
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+    ) -> AsyncIterator[ListManagedAccountsResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListManagedAccounts.paginate)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/paginators/#listmanagedaccountspaginator)
+        """
+
 class ListSourceServerActionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListSourceServerActions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/paginators/#listsourceserveractionspaginator)
     """
 
     def paginate(
         self,
         *,
         sourceServerID: str,
+        accountID: str = ...,
         filters: SourceServerActionsRequestFiltersTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSourceServerActionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListSourceServerActions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/paginators/#listsourceserveractionspaginator)
         """
@@ -318,14 +340,15 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListWaves)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/paginators/#listwavespaginator)
     """
 
     def paginate(
         self,
         *,
+        accountID: str = ...,
         filters: ListWavesRequestFiltersTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListWavesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.ListWaves.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mgn/paginators/#listwavespaginator)
         """
```

### Comparing `types-aiobotocore-mgn-2.5.2.post1/types_aiobotocore_mgn/type_defs.py` & `types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn/type_defs.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     ```python
     from types_aiobotocore_mgn.type_defs import ApplicationAggregatedStatusTypeDef
 
     data: ApplicationAggregatedStatusTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     ActionCategoryType,
     ApplicationHealthStatusType,
     ApplicationProgressStatusType,
     BootModeType,
     ChangeServerLifeCycleStateSourceServerLifecycleStateType,
@@ -116,31 +116,36 @@
     "LifeCycleLastTestInitiatedTypeDef",
     "LifeCycleLastTestRevertedTypeDef",
     "ListApplicationsRequestFiltersTypeDef",
     "ListExportErrorsRequestRequestTypeDef",
     "ListExportsRequestFiltersTypeDef",
     "ListImportErrorsRequestRequestTypeDef",
     "ListImportsRequestFiltersTypeDef",
+    "ListManagedAccountsRequestRequestTypeDef",
+    "ManagedAccountTypeDef",
     "SourceServerActionsRequestFiltersTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TemplateActionsRequestFiltersTypeDef",
     "ListWavesRequestFiltersTypeDef",
     "MarkAsArchivedRequestRequestTypeDef",
     "NetworkInterfaceTypeDef",
     "OSTypeDef",
+    "PauseReplicationRequestRequestTypeDef",
     "SsmExternalParameterTypeDef",
     "SsmParameterStoreParameterTypeDef",
     "RemoveSourceServerActionRequestRequestTypeDef",
     "RemoveTemplateActionRequestRequestTypeDef",
     "ReplicationConfigurationReplicatedDiskTypeDef",
+    "ResumeReplicationRequestRequestTypeDef",
     "RetryDataReplicationRequestRequestTypeDef",
     "StartCutoverRequestRequestTypeDef",
     "StartExportRequestRequestTypeDef",
     "StartReplicationRequestRequestTypeDef",
     "StartTestRequestRequestTypeDef",
+    "StopReplicationRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TerminateTargetInstancesRequestRequestTypeDef",
     "UnarchiveApplicationRequestRequestTypeDef",
     "UnarchiveWaveRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
     "UpdateReplicationConfigurationTemplateRequestRequestTypeDef",
@@ -156,14 +161,15 @@
     "DataReplicationInitiationTypeDef",
     "DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef",
     "DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef",
     "DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef",
     "DescribeVcenterClientsRequestDescribeVcenterClientsPaginateTypeDef",
     "ListExportErrorsRequestListExportErrorsPaginateTypeDef",
     "ListImportErrorsRequestListImportErrorsPaginateTypeDef",
+    "ListManagedAccountsRequestListManagedAccountsPaginateTypeDef",
     "DescribeJobsRequestDescribeJobsPaginateTypeDef",
     "DescribeJobsRequestRequestTypeDef",
     "DescribeReplicationConfigurationTemplatesResponseTypeDef",
     "DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef",
     "DescribeSourceServersRequestRequestTypeDef",
     "DescribeVcenterClientsResponseTypeDef",
     "ExportTaskErrorTypeDef",
@@ -176,26 +182,26 @@
     "LifeCycleLastTestTypeDef",
     "ListApplicationsRequestListApplicationsPaginateTypeDef",
     "ListApplicationsRequestRequestTypeDef",
     "ListExportsRequestListExportsPaginateTypeDef",
     "ListExportsRequestRequestTypeDef",
     "ListImportsRequestListImportsPaginateTypeDef",
     "ListImportsRequestRequestTypeDef",
+    "ListManagedAccountsResponseTypeDef",
     "ListSourceServerActionsRequestListSourceServerActionsPaginateTypeDef",
     "ListSourceServerActionsRequestRequestTypeDef",
     "ListTemplateActionsRequestListTemplateActionsPaginateTypeDef",
     "ListTemplateActionsRequestRequestTypeDef",
     "ListWavesRequestListWavesPaginateTypeDef",
     "ListWavesRequestRequestTypeDef",
     "SourcePropertiesTypeDef",
     "PutSourceServerActionRequestRequestTypeDef",
     "PutTemplateActionRequestRequestTypeDef",
     "SourceServerActionDocumentResponseTypeDef",
     "SourceServerActionDocumentTypeDef",
-    "SsmDocumentOutputTypeDef",
     "SsmDocumentTypeDef",
     "TemplateActionDocumentResponseTypeDef",
     "TemplateActionDocumentTypeDef",
     "ReplicationConfigurationTypeDef",
     "UpdateReplicationConfigurationRequestRequestTypeDef",
     "WaveResponseTypeDef",
     "WaveTypeDef",
@@ -206,28 +212,26 @@
     "StartExportResponseTypeDef",
     "ListImportErrorsResponseTypeDef",
     "ImportTaskTypeDef",
     "DescribeJobLogItemsResponseTypeDef",
     "LifeCycleTypeDef",
     "ListSourceServerActionsResponseTypeDef",
     "JobPostLaunchActionsLaunchStatusTypeDef",
-    "PostLaunchActionsOutputTypeDef",
     "PostLaunchActionsTypeDef",
     "ListTemplateActionsResponseTypeDef",
     "ListWavesResponseTypeDef",
     "ListImportsResponseTypeDef",
     "StartImportResponseTypeDef",
     "SourceServerResponseTypeDef",
     "SourceServerTypeDef",
     "PostLaunchActionsStatusTypeDef",
+    "CreateLaunchConfigurationTemplateRequestRequestTypeDef",
     "LaunchConfigurationTemplateResponseTypeDef",
     "LaunchConfigurationTemplateTypeDef",
     "LaunchConfigurationTypeDef",
-    "CreateLaunchConfigurationTemplateRequestRequestTypeDef",
-    "PostLaunchActionsUnionTypeDef",
     "UpdateLaunchConfigurationRequestRequestTypeDef",
     "UpdateLaunchConfigurationTemplateRequestRequestTypeDef",
     "DescribeSourceServersResponseTypeDef",
     "ParticipatingServerTypeDef",
     "DescribeLaunchConfigurationTemplatesResponseTypeDef",
     "JobTypeDef",
     "DescribeJobsResponseTypeDef",
@@ -254,43 +258,102 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-ArchiveApplicationRequestRequestTypeDef = TypedDict(
-    "ArchiveApplicationRequestRequestTypeDef",
+_RequiredArchiveApplicationRequestRequestTypeDef = TypedDict(
+    "_RequiredArchiveApplicationRequestRequestTypeDef",
     {
         "applicationID": str,
     },
 )
+_OptionalArchiveApplicationRequestRequestTypeDef = TypedDict(
+    "_OptionalArchiveApplicationRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
 
-ArchiveWaveRequestRequestTypeDef = TypedDict(
-    "ArchiveWaveRequestRequestTypeDef",
+
+class ArchiveApplicationRequestRequestTypeDef(
+    _RequiredArchiveApplicationRequestRequestTypeDef,
+    _OptionalArchiveApplicationRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredArchiveWaveRequestRequestTypeDef = TypedDict(
+    "_RequiredArchiveWaveRequestRequestTypeDef",
     {
         "waveID": str,
     },
 )
+_OptionalArchiveWaveRequestRequestTypeDef = TypedDict(
+    "_OptionalArchiveWaveRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
 
-AssociateApplicationsRequestRequestTypeDef = TypedDict(
-    "AssociateApplicationsRequestRequestTypeDef",
+
+class ArchiveWaveRequestRequestTypeDef(
+    _RequiredArchiveWaveRequestRequestTypeDef, _OptionalArchiveWaveRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredAssociateApplicationsRequestRequestTypeDef = TypedDict(
+    "_RequiredAssociateApplicationsRequestRequestTypeDef",
     {
         "applicationIDs": Sequence[str],
         "waveID": str,
     },
 )
+_OptionalAssociateApplicationsRequestRequestTypeDef = TypedDict(
+    "_OptionalAssociateApplicationsRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
 
-AssociateSourceServersRequestRequestTypeDef = TypedDict(
-    "AssociateSourceServersRequestRequestTypeDef",
+
+class AssociateApplicationsRequestRequestTypeDef(
+    _RequiredAssociateApplicationsRequestRequestTypeDef,
+    _OptionalAssociateApplicationsRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredAssociateSourceServersRequestRequestTypeDef = TypedDict(
+    "_RequiredAssociateSourceServersRequestRequestTypeDef",
     {
         "applicationID": str,
         "sourceServerIDs": Sequence[str],
     },
 )
+_OptionalAssociateSourceServersRequestRequestTypeDef = TypedDict(
+    "_OptionalAssociateSourceServersRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+
+class AssociateSourceServersRequestRequestTypeDef(
+    _RequiredAssociateSourceServersRequestRequestTypeDef,
+    _OptionalAssociateSourceServersRequestRequestTypeDef,
+):
+    pass
+
 
 CPUTypeDef = TypedDict(
     "CPUTypeDef",
     {
         "cores": int,
         "modelName": str,
     },
@@ -309,14 +372,15 @@
     {
         "name": str,
     },
 )
 _OptionalCreateApplicationRequestRequestTypeDef = TypedDict(
     "_OptionalCreateApplicationRequestRequestTypeDef",
     {
+        "accountID": str,
         "description": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
 
@@ -361,14 +425,15 @@
     },
 )
 _OptionalCreateReplicationConfigurationTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalCreateReplicationConfigurationTemplateRequestRequestTypeDef",
     {
         "ebsEncryptionKeyArn": str,
         "tags": Mapping[str, str],
+        "useFipsEndpoint": bool,
     },
     total=False,
 )
 
 
 class CreateReplicationConfigurationTemplateRequestRequestTypeDef(
     _RequiredCreateReplicationConfigurationTemplateRequestRequestTypeDef,
@@ -382,14 +447,15 @@
     {
         "name": str,
     },
 )
 _OptionalCreateWaveRequestRequestTypeDef = TypedDict(
     "_OptionalCreateWaveRequestRequestTypeDef",
     {
+        "accountID": str,
         "description": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
 
@@ -425,27 +491,55 @@
     {
         "name": DataReplicationInitiationStepNameType,
         "status": DataReplicationInitiationStepStatusType,
     },
     total=False,
 )
 
-DeleteApplicationRequestRequestTypeDef = TypedDict(
-    "DeleteApplicationRequestRequestTypeDef",
+_RequiredDeleteApplicationRequestRequestTypeDef = TypedDict(
+    "_RequiredDeleteApplicationRequestRequestTypeDef",
     {
         "applicationID": str,
     },
 )
+_OptionalDeleteApplicationRequestRequestTypeDef = TypedDict(
+    "_OptionalDeleteApplicationRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
 
-DeleteJobRequestRequestTypeDef = TypedDict(
-    "DeleteJobRequestRequestTypeDef",
+
+class DeleteApplicationRequestRequestTypeDef(
+    _RequiredDeleteApplicationRequestRequestTypeDef, _OptionalDeleteApplicationRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredDeleteJobRequestRequestTypeDef = TypedDict(
+    "_RequiredDeleteJobRequestRequestTypeDef",
     {
         "jobID": str,
     },
 )
+_OptionalDeleteJobRequestRequestTypeDef = TypedDict(
+    "_OptionalDeleteJobRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+
+class DeleteJobRequestRequestTypeDef(
+    _RequiredDeleteJobRequestRequestTypeDef, _OptionalDeleteJobRequestRequestTypeDef
+):
+    pass
+
 
 DeleteLaunchConfigurationTemplateRequestRequestTypeDef = TypedDict(
     "DeleteLaunchConfigurationTemplateRequestRequestTypeDef",
     {
         "launchConfigurationTemplateID": str,
     },
 )
@@ -453,34 +547,63 @@
 DeleteReplicationConfigurationTemplateRequestRequestTypeDef = TypedDict(
     "DeleteReplicationConfigurationTemplateRequestRequestTypeDef",
     {
         "replicationConfigurationTemplateID": str,
     },
 )
 
-DeleteSourceServerRequestRequestTypeDef = TypedDict(
-    "DeleteSourceServerRequestRequestTypeDef",
+_RequiredDeleteSourceServerRequestRequestTypeDef = TypedDict(
+    "_RequiredDeleteSourceServerRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
+_OptionalDeleteSourceServerRequestRequestTypeDef = TypedDict(
+    "_OptionalDeleteSourceServerRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+
+class DeleteSourceServerRequestRequestTypeDef(
+    _RequiredDeleteSourceServerRequestRequestTypeDef,
+    _OptionalDeleteSourceServerRequestRequestTypeDef,
+):
+    pass
+
 
 DeleteVcenterClientRequestRequestTypeDef = TypedDict(
     "DeleteVcenterClientRequestRequestTypeDef",
     {
         "vcenterClientID": str,
     },
 )
 
-DeleteWaveRequestRequestTypeDef = TypedDict(
-    "DeleteWaveRequestRequestTypeDef",
+_RequiredDeleteWaveRequestRequestTypeDef = TypedDict(
+    "_RequiredDeleteWaveRequestRequestTypeDef",
     {
         "waveID": str,
     },
 )
+_OptionalDeleteWaveRequestRequestTypeDef = TypedDict(
+    "_OptionalDeleteWaveRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+
+class DeleteWaveRequestRequestTypeDef(
+    _RequiredDeleteWaveRequestRequestTypeDef, _OptionalDeleteWaveRequestRequestTypeDef
+):
+    pass
+
 
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
@@ -493,14 +616,15 @@
     {
         "jobID": str,
     },
 )
 _OptionalDescribeJobLogItemsRequestRequestTypeDef = TypedDict(
     "_OptionalDescribeJobLogItemsRequestRequestTypeDef",
     {
+        "accountID": str,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
 
@@ -560,14 +684,15 @@
         "ebsEncryptionKeyArn": str,
         "replicationServerInstanceType": str,
         "replicationServersSecurityGroupsIDs": List[str],
         "stagingAreaSubnetId": str,
         "stagingAreaTags": Dict[str, str],
         "tags": Dict[str, str],
         "useDedicatedReplicationServer": bool,
+        "useFipsEndpoint": bool,
     },
     total=False,
 )
 
 
 class ReplicationConfigurationTemplateTypeDef(
     _RequiredReplicationConfigurationTemplateTypeDef,
@@ -608,36 +733,81 @@
         "tags": Dict[str, str],
         "vcenterClientID": str,
         "vcenterUUID": str,
     },
     total=False,
 )
 
-DisassociateApplicationsRequestRequestTypeDef = TypedDict(
-    "DisassociateApplicationsRequestRequestTypeDef",
+_RequiredDisassociateApplicationsRequestRequestTypeDef = TypedDict(
+    "_RequiredDisassociateApplicationsRequestRequestTypeDef",
     {
         "applicationIDs": Sequence[str],
         "waveID": str,
     },
 )
+_OptionalDisassociateApplicationsRequestRequestTypeDef = TypedDict(
+    "_OptionalDisassociateApplicationsRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
 
-DisassociateSourceServersRequestRequestTypeDef = TypedDict(
-    "DisassociateSourceServersRequestRequestTypeDef",
+
+class DisassociateApplicationsRequestRequestTypeDef(
+    _RequiredDisassociateApplicationsRequestRequestTypeDef,
+    _OptionalDisassociateApplicationsRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredDisassociateSourceServersRequestRequestTypeDef = TypedDict(
+    "_RequiredDisassociateSourceServersRequestRequestTypeDef",
     {
         "applicationID": str,
         "sourceServerIDs": Sequence[str],
     },
 )
+_OptionalDisassociateSourceServersRequestRequestTypeDef = TypedDict(
+    "_OptionalDisassociateSourceServersRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
 
-DisconnectFromServiceRequestRequestTypeDef = TypedDict(
-    "DisconnectFromServiceRequestRequestTypeDef",
+
+class DisassociateSourceServersRequestRequestTypeDef(
+    _RequiredDisassociateSourceServersRequestRequestTypeDef,
+    _OptionalDisassociateSourceServersRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredDisconnectFromServiceRequestRequestTypeDef = TypedDict(
+    "_RequiredDisconnectFromServiceRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
+_OptionalDisconnectFromServiceRequestRequestTypeDef = TypedDict(
+    "_OptionalDisconnectFromServiceRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+
+class DisconnectFromServiceRequestRequestTypeDef(
+    _RequiredDisconnectFromServiceRequestRequestTypeDef,
+    _OptionalDisconnectFromServiceRequestRequestTypeDef,
+):
+    pass
+
 
 DiskTypeDef = TypedDict(
     "DiskTypeDef",
     {
         "bytes": int,
         "deviceName": str,
     },
@@ -658,34 +828,78 @@
         "applicationsCount": int,
         "serversCount": int,
         "wavesCount": int,
     },
     total=False,
 )
 
-FinalizeCutoverRequestRequestTypeDef = TypedDict(
-    "FinalizeCutoverRequestRequestTypeDef",
+_RequiredFinalizeCutoverRequestRequestTypeDef = TypedDict(
+    "_RequiredFinalizeCutoverRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
+_OptionalFinalizeCutoverRequestRequestTypeDef = TypedDict(
+    "_OptionalFinalizeCutoverRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
 
-GetLaunchConfigurationRequestRequestTypeDef = TypedDict(
-    "GetLaunchConfigurationRequestRequestTypeDef",
+
+class FinalizeCutoverRequestRequestTypeDef(
+    _RequiredFinalizeCutoverRequestRequestTypeDef, _OptionalFinalizeCutoverRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredGetLaunchConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredGetLaunchConfigurationRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
+_OptionalGetLaunchConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalGetLaunchConfigurationRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
 
-GetReplicationConfigurationRequestRequestTypeDef = TypedDict(
-    "GetReplicationConfigurationRequestRequestTypeDef",
+
+class GetLaunchConfigurationRequestRequestTypeDef(
+    _RequiredGetLaunchConfigurationRequestRequestTypeDef,
+    _OptionalGetLaunchConfigurationRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredGetReplicationConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredGetReplicationConfigurationRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
+_OptionalGetReplicationConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalGetReplicationConfigurationRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+
+class GetReplicationConfigurationRequestRequestTypeDef(
+    _RequiredGetReplicationConfigurationRequestRequestTypeDef,
+    _OptionalGetReplicationConfigurationRequestRequestTypeDef,
+):
+    pass
+
 
 IdentificationHintsTypeDef = TypedDict(
     "IdentificationHintsTypeDef",
     {
         "awsInstanceID": str,
         "fqdn": str,
         "hostname": str,
@@ -694,14 +908,15 @@
     },
     total=False,
 )
 
 ImportErrorDataTypeDef = TypedDict(
     "ImportErrorDataTypeDef",
     {
+        "accountID": str,
         "applicationID": str,
         "ec2LaunchTemplateID": str,
         "rawError": str,
         "rowNumber": int,
         "sourceServerID": str,
         "waveID": str,
     },
@@ -892,14 +1107,31 @@
     "ListImportsRequestFiltersTypeDef",
     {
         "importIDs": Sequence[str],
     },
     total=False,
 )
 
+ListManagedAccountsRequestRequestTypeDef = TypedDict(
+    "ListManagedAccountsRequestRequestTypeDef",
+    {
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+ManagedAccountTypeDef = TypedDict(
+    "ManagedAccountTypeDef",
+    {
+        "accountId": str,
+    },
+    total=False,
+)
+
 SourceServerActionsRequestFiltersTypeDef = TypedDict(
     "SourceServerActionsRequestFiltersTypeDef",
     {
         "actionIDs": Sequence[str],
     },
     total=False,
 )
@@ -924,20 +1156,34 @@
     {
         "isArchived": bool,
         "waveIDs": Sequence[str],
     },
     total=False,
 )
 
-MarkAsArchivedRequestRequestTypeDef = TypedDict(
-    "MarkAsArchivedRequestRequestTypeDef",
+_RequiredMarkAsArchivedRequestRequestTypeDef = TypedDict(
+    "_RequiredMarkAsArchivedRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
+_OptionalMarkAsArchivedRequestRequestTypeDef = TypedDict(
+    "_OptionalMarkAsArchivedRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+
+class MarkAsArchivedRequestRequestTypeDef(
+    _RequiredMarkAsArchivedRequestRequestTypeDef, _OptionalMarkAsArchivedRequestRequestTypeDef
+):
+    pass
+
 
 NetworkInterfaceTypeDef = TypedDict(
     "NetworkInterfaceTypeDef",
     {
         "ips": List[str],
         "isPrimary": bool,
         "macAddress": str,
@@ -949,14 +1195,35 @@
     "OSTypeDef",
     {
         "fullString": str,
     },
     total=False,
 )
 
+_RequiredPauseReplicationRequestRequestTypeDef = TypedDict(
+    "_RequiredPauseReplicationRequestRequestTypeDef",
+    {
+        "sourceServerID": str,
+    },
+)
+_OptionalPauseReplicationRequestRequestTypeDef = TypedDict(
+    "_OptionalPauseReplicationRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+
+class PauseReplicationRequestRequestTypeDef(
+    _RequiredPauseReplicationRequestRequestTypeDef, _OptionalPauseReplicationRequestRequestTypeDef
+):
+    pass
+
+
 SsmExternalParameterTypeDef = TypedDict(
     "SsmExternalParameterTypeDef",
     {
         "dynamicPath": str,
     },
     total=False,
 )
@@ -965,21 +1232,36 @@
     "SsmParameterStoreParameterTypeDef",
     {
         "parameterName": str,
         "parameterType": Literal["STRING"],
     },
 )
 
-RemoveSourceServerActionRequestRequestTypeDef = TypedDict(
-    "RemoveSourceServerActionRequestRequestTypeDef",
+_RequiredRemoveSourceServerActionRequestRequestTypeDef = TypedDict(
+    "_RequiredRemoveSourceServerActionRequestRequestTypeDef",
     {
         "actionID": str,
         "sourceServerID": str,
     },
 )
+_OptionalRemoveSourceServerActionRequestRequestTypeDef = TypedDict(
+    "_OptionalRemoveSourceServerActionRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+
+class RemoveSourceServerActionRequestRequestTypeDef(
+    _RequiredRemoveSourceServerActionRequestRequestTypeDef,
+    _OptionalRemoveSourceServerActionRequestRequestTypeDef,
+):
+    pass
+
 
 RemoveTemplateActionRequestRequestTypeDef = TypedDict(
     "RemoveTemplateActionRequestRequestTypeDef",
     {
         "actionID": str,
         "launchConfigurationTemplateID": str,
     },
@@ -993,30 +1275,67 @@
         "isBootDisk": bool,
         "stagingDiskType": ReplicationConfigurationReplicatedDiskStagingDiskTypeType,
         "throughput": int,
     },
     total=False,
 )
 
-RetryDataReplicationRequestRequestTypeDef = TypedDict(
-    "RetryDataReplicationRequestRequestTypeDef",
+_RequiredResumeReplicationRequestRequestTypeDef = TypedDict(
+    "_RequiredResumeReplicationRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
+_OptionalResumeReplicationRequestRequestTypeDef = TypedDict(
+    "_OptionalResumeReplicationRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+
+class ResumeReplicationRequestRequestTypeDef(
+    _RequiredResumeReplicationRequestRequestTypeDef, _OptionalResumeReplicationRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredRetryDataReplicationRequestRequestTypeDef = TypedDict(
+    "_RequiredRetryDataReplicationRequestRequestTypeDef",
+    {
+        "sourceServerID": str,
+    },
+)
+_OptionalRetryDataReplicationRequestRequestTypeDef = TypedDict(
+    "_OptionalRetryDataReplicationRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+
+class RetryDataReplicationRequestRequestTypeDef(
+    _RequiredRetryDataReplicationRequestRequestTypeDef,
+    _OptionalRetryDataReplicationRequestRequestTypeDef,
+):
+    pass
+
 
 _RequiredStartCutoverRequestRequestTypeDef = TypedDict(
     "_RequiredStartCutoverRequestRequestTypeDef",
     {
         "sourceServerIDs": Sequence[str],
     },
 )
 _OptionalStartCutoverRequestRequestTypeDef = TypedDict(
     "_OptionalStartCutoverRequestRequestTypeDef",
     {
+        "accountID": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
 
 class StartCutoverRequestRequestTypeDef(
@@ -1043,42 +1362,78 @@
 
 class StartExportRequestRequestTypeDef(
     _RequiredStartExportRequestRequestTypeDef, _OptionalStartExportRequestRequestTypeDef
 ):
     pass
 
 
-StartReplicationRequestRequestTypeDef = TypedDict(
-    "StartReplicationRequestRequestTypeDef",
+_RequiredStartReplicationRequestRequestTypeDef = TypedDict(
+    "_RequiredStartReplicationRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
+_OptionalStartReplicationRequestRequestTypeDef = TypedDict(
+    "_OptionalStartReplicationRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+
+class StartReplicationRequestRequestTypeDef(
+    _RequiredStartReplicationRequestRequestTypeDef, _OptionalStartReplicationRequestRequestTypeDef
+):
+    pass
+
 
 _RequiredStartTestRequestRequestTypeDef = TypedDict(
     "_RequiredStartTestRequestRequestTypeDef",
     {
         "sourceServerIDs": Sequence[str],
     },
 )
 _OptionalStartTestRequestRequestTypeDef = TypedDict(
     "_OptionalStartTestRequestRequestTypeDef",
     {
+        "accountID": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
 
 class StartTestRequestRequestTypeDef(
     _RequiredStartTestRequestRequestTypeDef, _OptionalStartTestRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredStopReplicationRequestRequestTypeDef = TypedDict(
+    "_RequiredStopReplicationRequestRequestTypeDef",
+    {
+        "sourceServerID": str,
+    },
+)
+_OptionalStopReplicationRequestRequestTypeDef = TypedDict(
+    "_OptionalStopReplicationRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+
+class StopReplicationRequestRequestTypeDef(
+    _RequiredStopReplicationRequestRequestTypeDef, _OptionalStopReplicationRequestRequestTypeDef
+):
+    pass
+
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -1088,40 +1443,70 @@
     {
         "sourceServerIDs": Sequence[str],
     },
 )
 _OptionalTerminateTargetInstancesRequestRequestTypeDef = TypedDict(
     "_OptionalTerminateTargetInstancesRequestRequestTypeDef",
     {
+        "accountID": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
 
 class TerminateTargetInstancesRequestRequestTypeDef(
     _RequiredTerminateTargetInstancesRequestRequestTypeDef,
     _OptionalTerminateTargetInstancesRequestRequestTypeDef,
 ):
     pass
 
 
-UnarchiveApplicationRequestRequestTypeDef = TypedDict(
-    "UnarchiveApplicationRequestRequestTypeDef",
+_RequiredUnarchiveApplicationRequestRequestTypeDef = TypedDict(
+    "_RequiredUnarchiveApplicationRequestRequestTypeDef",
     {
         "applicationID": str,
     },
 )
+_OptionalUnarchiveApplicationRequestRequestTypeDef = TypedDict(
+    "_OptionalUnarchiveApplicationRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
 
-UnarchiveWaveRequestRequestTypeDef = TypedDict(
-    "UnarchiveWaveRequestRequestTypeDef",
+
+class UnarchiveApplicationRequestRequestTypeDef(
+    _RequiredUnarchiveApplicationRequestRequestTypeDef,
+    _OptionalUnarchiveApplicationRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredUnarchiveWaveRequestRequestTypeDef = TypedDict(
+    "_RequiredUnarchiveWaveRequestRequestTypeDef",
     {
         "waveID": str,
     },
 )
+_OptionalUnarchiveWaveRequestRequestTypeDef = TypedDict(
+    "_OptionalUnarchiveWaveRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+
+class UnarchiveWaveRequestRequestTypeDef(
+    _RequiredUnarchiveWaveRequestRequestTypeDef, _OptionalUnarchiveWaveRequestRequestTypeDef
+):
+    pass
+
 
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
@@ -1132,14 +1517,15 @@
     {
         "applicationID": str,
     },
 )
 _OptionalUpdateApplicationRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateApplicationRequestRequestTypeDef",
     {
+        "accountID": str,
         "description": str,
         "name": str,
     },
     total=False,
 )
 
 
@@ -1167,43 +1553,60 @@
         "ebsEncryption": ReplicationConfigurationEbsEncryptionType,
         "ebsEncryptionKeyArn": str,
         "replicationServerInstanceType": str,
         "replicationServersSecurityGroupsIDs": Sequence[str],
         "stagingAreaSubnetId": str,
         "stagingAreaTags": Mapping[str, str],
         "useDedicatedReplicationServer": bool,
+        "useFipsEndpoint": bool,
     },
     total=False,
 )
 
 
 class UpdateReplicationConfigurationTemplateRequestRequestTypeDef(
     _RequiredUpdateReplicationConfigurationTemplateRequestRequestTypeDef,
     _OptionalUpdateReplicationConfigurationTemplateRequestRequestTypeDef,
 ):
     pass
 
 
-UpdateSourceServerReplicationTypeRequestRequestTypeDef = TypedDict(
-    "UpdateSourceServerReplicationTypeRequestRequestTypeDef",
+_RequiredUpdateSourceServerReplicationTypeRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateSourceServerReplicationTypeRequestRequestTypeDef",
     {
         "replicationType": ReplicationTypeType,
         "sourceServerID": str,
     },
 )
+_OptionalUpdateSourceServerReplicationTypeRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateSourceServerReplicationTypeRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+
+class UpdateSourceServerReplicationTypeRequestRequestTypeDef(
+    _RequiredUpdateSourceServerReplicationTypeRequestRequestTypeDef,
+    _OptionalUpdateSourceServerReplicationTypeRequestRequestTypeDef,
+):
+    pass
+
 
 _RequiredUpdateWaveRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWaveRequestRequestTypeDef",
     {
         "waveID": str,
     },
 )
 _OptionalUpdateWaveRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateWaveRequestRequestTypeDef",
     {
+        "accountID": str,
         "description": str,
         "name": str,
     },
     total=False,
 )
 
 
@@ -1288,25 +1691,41 @@
         "replicationConfigurationTemplateID": str,
         "replicationServerInstanceType": str,
         "replicationServersSecurityGroupsIDs": List[str],
         "stagingAreaSubnetId": str,
         "stagingAreaTags": Dict[str, str],
         "tags": Dict[str, str],
         "useDedicatedReplicationServer": bool,
+        "useFipsEndpoint": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ChangeServerLifeCycleStateRequestRequestTypeDef = TypedDict(
-    "ChangeServerLifeCycleStateRequestRequestTypeDef",
+_RequiredChangeServerLifeCycleStateRequestRequestTypeDef = TypedDict(
+    "_RequiredChangeServerLifeCycleStateRequestRequestTypeDef",
     {
         "lifeCycle": ChangeServerLifeCycleStateSourceServerLifecycleTypeDef,
         "sourceServerID": str,
     },
 )
+_OptionalChangeServerLifeCycleStateRequestRequestTypeDef = TypedDict(
+    "_OptionalChangeServerLifeCycleStateRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+
+class ChangeServerLifeCycleStateRequestRequestTypeDef(
+    _RequiredChangeServerLifeCycleStateRequestRequestTypeDef,
+    _OptionalChangeServerLifeCycleStateRequestRequestTypeDef,
+):
+    pass
+
 
 DataReplicationInitiationTypeDef = TypedDict(
     "DataReplicationInitiationTypeDef",
     {
         "nextAttemptDateTime": str,
         "startDateTime": str,
         "steps": List[DataReplicationInitiationStepTypeDef],
@@ -1319,14 +1738,15 @@
     {
         "jobID": str,
     },
 )
 _OptionalDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef = TypedDict(
     "_OptionalDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef",
     {
+        "accountID": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef(
@@ -1402,26 +1822,36 @@
 class ListImportErrorsRequestListImportErrorsPaginateTypeDef(
     _RequiredListImportErrorsRequestListImportErrorsPaginateTypeDef,
     _OptionalListImportErrorsRequestListImportErrorsPaginateTypeDef,
 ):
     pass
 
 
+ListManagedAccountsRequestListManagedAccountsPaginateTypeDef = TypedDict(
+    "ListManagedAccountsRequestListManagedAccountsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 DescribeJobsRequestDescribeJobsPaginateTypeDef = TypedDict(
     "DescribeJobsRequestDescribeJobsPaginateTypeDef",
     {
+        "accountID": str,
         "filters": DescribeJobsRequestFiltersTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeJobsRequestRequestTypeDef = TypedDict(
     "DescribeJobsRequestRequestTypeDef",
     {
+        "accountID": str,
         "filters": DescribeJobsRequestFiltersTypeDef,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
@@ -1433,23 +1863,25 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef = TypedDict(
     "DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef",
     {
+        "accountID": str,
         "filters": DescribeSourceServersRequestFiltersTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeSourceServersRequestRequestTypeDef = TypedDict(
     "DescribeSourceServersRequestRequestTypeDef",
     {
+        "accountID": str,
         "filters": DescribeSourceServersRequestFiltersTypeDef,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
@@ -1557,23 +1989,25 @@
     },
     total=False,
 )
 
 ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
     "ListApplicationsRequestListApplicationsPaginateTypeDef",
     {
+        "accountID": str,
         "filters": ListApplicationsRequestFiltersTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListApplicationsRequestRequestTypeDef = TypedDict(
     "ListApplicationsRequestRequestTypeDef",
     {
+        "accountID": str,
         "filters": ListApplicationsRequestFiltersTypeDef,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
@@ -1611,23 +2045,33 @@
         "filters": ListImportsRequestFiltersTypeDef,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+ListManagedAccountsResponseTypeDef = TypedDict(
+    "ListManagedAccountsResponseTypeDef",
+    {
+        "items": List[ManagedAccountTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredListSourceServerActionsRequestListSourceServerActionsPaginateTypeDef = TypedDict(
     "_RequiredListSourceServerActionsRequestListSourceServerActionsPaginateTypeDef",
     {
         "sourceServerID": str,
     },
 )
 _OptionalListSourceServerActionsRequestListSourceServerActionsPaginateTypeDef = TypedDict(
     "_OptionalListSourceServerActionsRequestListSourceServerActionsPaginateTypeDef",
     {
+        "accountID": str,
         "filters": SourceServerActionsRequestFiltersTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
@@ -1643,14 +2087,15 @@
     {
         "sourceServerID": str,
     },
 )
 _OptionalListSourceServerActionsRequestRequestTypeDef = TypedDict(
     "_OptionalListSourceServerActionsRequestRequestTypeDef",
     {
+        "accountID": str,
         "filters": SourceServerActionsRequestFiltersTypeDef,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
@@ -1708,23 +2153,25 @@
 ):
     pass
 
 
 ListWavesRequestListWavesPaginateTypeDef = TypedDict(
     "ListWavesRequestListWavesPaginateTypeDef",
     {
+        "accountID": str,
         "filters": ListWavesRequestFiltersTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListWavesRequestRequestTypeDef = TypedDict(
     "ListWavesRequestRequestTypeDef",
     {
+        "accountID": str,
         "filters": ListWavesRequestFiltersTypeDef,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
@@ -1752,14 +2199,15 @@
         "order": int,
         "sourceServerID": str,
     },
 )
 _OptionalPutSourceServerActionRequestRequestTypeDef = TypedDict(
     "_OptionalPutSourceServerActionRequestRequestTypeDef",
     {
+        "accountID": str,
         "active": bool,
         "category": ActionCategoryType,
         "description": str,
         "documentVersion": str,
         "externalParameters": Mapping[str, SsmExternalParameterTypeDef],
         "mustSucceedForCutover": bool,
         "parameters": Mapping[str, Sequence[SsmParameterStoreParameterTypeDef]],
@@ -1843,39 +2291,14 @@
         "order": int,
         "parameters": Dict[str, List[SsmParameterStoreParameterTypeDef]],
         "timeoutSeconds": int,
     },
     total=False,
 )
 
-_RequiredSsmDocumentOutputTypeDef = TypedDict(
-    "_RequiredSsmDocumentOutputTypeDef",
-    {
-        "actionName": str,
-        "ssmDocumentName": str,
-    },
-)
-_OptionalSsmDocumentOutputTypeDef = TypedDict(
-    "_OptionalSsmDocumentOutputTypeDef",
-    {
-        "externalParameters": Dict[str, SsmExternalParameterTypeDef],
-        "mustSucceedForCutover": bool,
-        "parameters": Dict[str, List[SsmParameterStoreParameterTypeDef]],
-        "timeoutSeconds": int,
-    },
-    total=False,
-)
-
-
-class SsmDocumentOutputTypeDef(
-    _RequiredSsmDocumentOutputTypeDef, _OptionalSsmDocumentOutputTypeDef
-):
-    pass
-
-
 _RequiredSsmDocumentTypeDef = TypedDict(
     "_RequiredSsmDocumentTypeDef",
     {
         "actionName": str,
         "ssmDocumentName": str,
     },
 )
@@ -1949,41 +2372,44 @@
         "replicatedDisks": List[ReplicationConfigurationReplicatedDiskTypeDef],
         "replicationServerInstanceType": str,
         "replicationServersSecurityGroupsIDs": List[str],
         "sourceServerID": str,
         "stagingAreaSubnetId": str,
         "stagingAreaTags": Dict[str, str],
         "useDedicatedReplicationServer": bool,
+        "useFipsEndpoint": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateReplicationConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateReplicationConfigurationRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
 _OptionalUpdateReplicationConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateReplicationConfigurationRequestRequestTypeDef",
     {
+        "accountID": str,
         "associateDefaultSecurityGroup": bool,
         "bandwidthThrottling": int,
         "createPublicIP": bool,
         "dataPlaneRouting": ReplicationConfigurationDataPlaneRoutingType,
         "defaultLargeStagingDiskType": ReplicationConfigurationDefaultLargeStagingDiskTypeType,
         "ebsEncryption": ReplicationConfigurationEbsEncryptionType,
         "ebsEncryptionKeyArn": str,
         "name": str,
         "replicatedDisks": Sequence[ReplicationConfigurationReplicatedDiskTypeDef],
         "replicationServerInstanceType": str,
         "replicationServersSecurityGroupsIDs": Sequence[str],
         "stagingAreaSubnetId": str,
         "stagingAreaTags": Mapping[str, str],
         "useDedicatedReplicationServer": bool,
+        "useFipsEndpoint": bool,
     },
     total=False,
 )
 
 
 class UpdateReplicationConfigurationRequestRequestTypeDef(
     _RequiredUpdateReplicationConfigurationRequestRequestTypeDef,
@@ -2130,32 +2556,20 @@
 
 JobPostLaunchActionsLaunchStatusTypeDef = TypedDict(
     "JobPostLaunchActionsLaunchStatusTypeDef",
     {
         "executionID": str,
         "executionStatus": PostLaunchActionExecutionStatusType,
         "failureReason": str,
-        "ssmDocument": SsmDocumentOutputTypeDef,
+        "ssmDocument": SsmDocumentTypeDef,
         "ssmDocumentType": SsmDocumentTypeType,
     },
     total=False,
 )
 
-PostLaunchActionsOutputTypeDef = TypedDict(
-    "PostLaunchActionsOutputTypeDef",
-    {
-        "cloudWatchLogGroupName": str,
-        "deployment": PostLaunchActionsDeploymentTypeType,
-        "s3LogBucket": str,
-        "s3OutputKeyPrefix": str,
-        "ssmDocuments": List[SsmDocumentOutputTypeDef],
-    },
-    total=False,
-)
-
 PostLaunchActionsTypeDef = TypedDict(
     "PostLaunchActionsTypeDef",
     {
         "cloudWatchLogGroupName": str,
         "deployment": PostLaunchActionsDeploymentTypeType,
         "s3LogBucket": str,
         "s3OutputKeyPrefix": str,
@@ -2244,14 +2658,35 @@
     {
         "postLaunchActionsLaunchStatusList": List[JobPostLaunchActionsLaunchStatusTypeDef],
         "ssmAgentDiscoveryDatetime": str,
     },
     total=False,
 )
 
+CreateLaunchConfigurationTemplateRequestRequestTypeDef = TypedDict(
+    "CreateLaunchConfigurationTemplateRequestRequestTypeDef",
+    {
+        "associatePublicIpAddress": bool,
+        "bootMode": BootModeType,
+        "copyPrivateIp": bool,
+        "copyTags": bool,
+        "enableMapAutoTagging": bool,
+        "largeVolumeConf": LaunchTemplateDiskConfTypeDef,
+        "launchDisposition": LaunchDispositionType,
+        "licensing": LicensingTypeDef,
+        "mapAutoTaggingMpeID": str,
+        "postLaunchActions": PostLaunchActionsTypeDef,
+        "smallVolumeConf": LaunchTemplateDiskConfTypeDef,
+        "smallVolumeMaxSize": int,
+        "tags": Mapping[str, str],
+        "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
+    },
+    total=False,
+)
+
 LaunchConfigurationTemplateResponseTypeDef = TypedDict(
     "LaunchConfigurationTemplateResponseTypeDef",
     {
         "arn": str,
         "associatePublicIpAddress": bool,
         "bootMode": BootModeType,
         "copyPrivateIp": bool,
@@ -2259,15 +2694,15 @@
         "ec2LaunchTemplateID": str,
         "enableMapAutoTagging": bool,
         "largeVolumeConf": LaunchTemplateDiskConfTypeDef,
         "launchConfigurationTemplateID": str,
         "launchDisposition": LaunchDispositionType,
         "licensing": LicensingTypeDef,
         "mapAutoTaggingMpeID": str,
-        "postLaunchActions": PostLaunchActionsOutputTypeDef,
+        "postLaunchActions": PostLaunchActionsTypeDef,
         "smallVolumeConf": LaunchTemplateDiskConfTypeDef,
         "smallVolumeMaxSize": int,
         "tags": Dict[str, str],
         "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2288,15 +2723,15 @@
         "copyTags": bool,
         "ec2LaunchTemplateID": str,
         "enableMapAutoTagging": bool,
         "largeVolumeConf": LaunchTemplateDiskConfTypeDef,
         "launchDisposition": LaunchDispositionType,
         "licensing": LicensingTypeDef,
         "mapAutoTaggingMpeID": str,
-        "postLaunchActions": PostLaunchActionsOutputTypeDef,
+        "postLaunchActions": PostLaunchActionsTypeDef,
         "smallVolumeConf": LaunchTemplateDiskConfTypeDef,
         "smallVolumeMaxSize": int,
         "tags": Dict[str, str],
         "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
     },
     total=False,
 )
@@ -2316,52 +2751,31 @@
         "copyTags": bool,
         "ec2LaunchTemplateID": str,
         "enableMapAutoTagging": bool,
         "launchDisposition": LaunchDispositionType,
         "licensing": LicensingTypeDef,
         "mapAutoTaggingMpeID": str,
         "name": str,
-        "postLaunchActions": PostLaunchActionsOutputTypeDef,
+        "postLaunchActions": PostLaunchActionsTypeDef,
         "sourceServerID": str,
         "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateLaunchConfigurationTemplateRequestRequestTypeDef = TypedDict(
-    "CreateLaunchConfigurationTemplateRequestRequestTypeDef",
-    {
-        "associatePublicIpAddress": bool,
-        "bootMode": BootModeType,
-        "copyPrivateIp": bool,
-        "copyTags": bool,
-        "enableMapAutoTagging": bool,
-        "largeVolumeConf": LaunchTemplateDiskConfTypeDef,
-        "launchDisposition": LaunchDispositionType,
-        "licensing": LicensingTypeDef,
-        "mapAutoTaggingMpeID": str,
-        "postLaunchActions": PostLaunchActionsTypeDef,
-        "smallVolumeConf": LaunchTemplateDiskConfTypeDef,
-        "smallVolumeMaxSize": int,
-        "tags": Mapping[str, str],
-        "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
-    },
-    total=False,
-)
-
-PostLaunchActionsUnionTypeDef = Union[PostLaunchActionsTypeDef, PostLaunchActionsOutputTypeDef]
 _RequiredUpdateLaunchConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLaunchConfigurationRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
 _OptionalUpdateLaunchConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateLaunchConfigurationRequestRequestTypeDef",
     {
+        "accountID": str,
         "bootMode": BootModeType,
         "copyPrivateIp": bool,
         "copyTags": bool,
         "enableMapAutoTagging": bool,
         "launchDisposition": LaunchDispositionType,
         "licensing": LicensingTypeDef,
         "mapAutoTaggingMpeID": str,
```

### Comparing `types-aiobotocore-mgn-2.5.2.post1/types_aiobotocore_mgn/type_defs.pyi` & `types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn/type_defs.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     ```python
     from types_aiobotocore_mgn.type_defs import ApplicationAggregatedStatusTypeDef
 
     data: ApplicationAggregatedStatusTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     ActionCategoryType,
     ApplicationHealthStatusType,
     ApplicationProgressStatusType,
     BootModeType,
     ChangeServerLifeCycleStateSourceServerLifecycleStateType,
@@ -115,31 +115,36 @@
     "LifeCycleLastTestInitiatedTypeDef",
     "LifeCycleLastTestRevertedTypeDef",
     "ListApplicationsRequestFiltersTypeDef",
     "ListExportErrorsRequestRequestTypeDef",
     "ListExportsRequestFiltersTypeDef",
     "ListImportErrorsRequestRequestTypeDef",
     "ListImportsRequestFiltersTypeDef",
+    "ListManagedAccountsRequestRequestTypeDef",
+    "ManagedAccountTypeDef",
     "SourceServerActionsRequestFiltersTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TemplateActionsRequestFiltersTypeDef",
     "ListWavesRequestFiltersTypeDef",
     "MarkAsArchivedRequestRequestTypeDef",
     "NetworkInterfaceTypeDef",
     "OSTypeDef",
+    "PauseReplicationRequestRequestTypeDef",
     "SsmExternalParameterTypeDef",
     "SsmParameterStoreParameterTypeDef",
     "RemoveSourceServerActionRequestRequestTypeDef",
     "RemoveTemplateActionRequestRequestTypeDef",
     "ReplicationConfigurationReplicatedDiskTypeDef",
+    "ResumeReplicationRequestRequestTypeDef",
     "RetryDataReplicationRequestRequestTypeDef",
     "StartCutoverRequestRequestTypeDef",
     "StartExportRequestRequestTypeDef",
     "StartReplicationRequestRequestTypeDef",
     "StartTestRequestRequestTypeDef",
+    "StopReplicationRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TerminateTargetInstancesRequestRequestTypeDef",
     "UnarchiveApplicationRequestRequestTypeDef",
     "UnarchiveWaveRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
     "UpdateReplicationConfigurationTemplateRequestRequestTypeDef",
@@ -155,14 +160,15 @@
     "DataReplicationInitiationTypeDef",
     "DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef",
     "DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef",
     "DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef",
     "DescribeVcenterClientsRequestDescribeVcenterClientsPaginateTypeDef",
     "ListExportErrorsRequestListExportErrorsPaginateTypeDef",
     "ListImportErrorsRequestListImportErrorsPaginateTypeDef",
+    "ListManagedAccountsRequestListManagedAccountsPaginateTypeDef",
     "DescribeJobsRequestDescribeJobsPaginateTypeDef",
     "DescribeJobsRequestRequestTypeDef",
     "DescribeReplicationConfigurationTemplatesResponseTypeDef",
     "DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef",
     "DescribeSourceServersRequestRequestTypeDef",
     "DescribeVcenterClientsResponseTypeDef",
     "ExportTaskErrorTypeDef",
@@ -175,26 +181,26 @@
     "LifeCycleLastTestTypeDef",
     "ListApplicationsRequestListApplicationsPaginateTypeDef",
     "ListApplicationsRequestRequestTypeDef",
     "ListExportsRequestListExportsPaginateTypeDef",
     "ListExportsRequestRequestTypeDef",
     "ListImportsRequestListImportsPaginateTypeDef",
     "ListImportsRequestRequestTypeDef",
+    "ListManagedAccountsResponseTypeDef",
     "ListSourceServerActionsRequestListSourceServerActionsPaginateTypeDef",
     "ListSourceServerActionsRequestRequestTypeDef",
     "ListTemplateActionsRequestListTemplateActionsPaginateTypeDef",
     "ListTemplateActionsRequestRequestTypeDef",
     "ListWavesRequestListWavesPaginateTypeDef",
     "ListWavesRequestRequestTypeDef",
     "SourcePropertiesTypeDef",
     "PutSourceServerActionRequestRequestTypeDef",
     "PutTemplateActionRequestRequestTypeDef",
     "SourceServerActionDocumentResponseTypeDef",
     "SourceServerActionDocumentTypeDef",
-    "SsmDocumentOutputTypeDef",
     "SsmDocumentTypeDef",
     "TemplateActionDocumentResponseTypeDef",
     "TemplateActionDocumentTypeDef",
     "ReplicationConfigurationTypeDef",
     "UpdateReplicationConfigurationRequestRequestTypeDef",
     "WaveResponseTypeDef",
     "WaveTypeDef",
@@ -205,28 +211,26 @@
     "StartExportResponseTypeDef",
     "ListImportErrorsResponseTypeDef",
     "ImportTaskTypeDef",
     "DescribeJobLogItemsResponseTypeDef",
     "LifeCycleTypeDef",
     "ListSourceServerActionsResponseTypeDef",
     "JobPostLaunchActionsLaunchStatusTypeDef",
-    "PostLaunchActionsOutputTypeDef",
     "PostLaunchActionsTypeDef",
     "ListTemplateActionsResponseTypeDef",
     "ListWavesResponseTypeDef",
     "ListImportsResponseTypeDef",
     "StartImportResponseTypeDef",
     "SourceServerResponseTypeDef",
     "SourceServerTypeDef",
     "PostLaunchActionsStatusTypeDef",
+    "CreateLaunchConfigurationTemplateRequestRequestTypeDef",
     "LaunchConfigurationTemplateResponseTypeDef",
     "LaunchConfigurationTemplateTypeDef",
     "LaunchConfigurationTypeDef",
-    "CreateLaunchConfigurationTemplateRequestRequestTypeDef",
-    "PostLaunchActionsUnionTypeDef",
     "UpdateLaunchConfigurationRequestRequestTypeDef",
     "UpdateLaunchConfigurationTemplateRequestRequestTypeDef",
     "DescribeSourceServersResponseTypeDef",
     "ParticipatingServerTypeDef",
     "DescribeLaunchConfigurationTemplatesResponseTypeDef",
     "JobTypeDef",
     "DescribeJobsResponseTypeDef",
@@ -253,43 +257,94 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-ArchiveApplicationRequestRequestTypeDef = TypedDict(
-    "ArchiveApplicationRequestRequestTypeDef",
+_RequiredArchiveApplicationRequestRequestTypeDef = TypedDict(
+    "_RequiredArchiveApplicationRequestRequestTypeDef",
     {
         "applicationID": str,
     },
 )
+_OptionalArchiveApplicationRequestRequestTypeDef = TypedDict(
+    "_OptionalArchiveApplicationRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
 
-ArchiveWaveRequestRequestTypeDef = TypedDict(
-    "ArchiveWaveRequestRequestTypeDef",
+class ArchiveApplicationRequestRequestTypeDef(
+    _RequiredArchiveApplicationRequestRequestTypeDef,
+    _OptionalArchiveApplicationRequestRequestTypeDef,
+):
+    pass
+
+_RequiredArchiveWaveRequestRequestTypeDef = TypedDict(
+    "_RequiredArchiveWaveRequestRequestTypeDef",
     {
         "waveID": str,
     },
 )
+_OptionalArchiveWaveRequestRequestTypeDef = TypedDict(
+    "_OptionalArchiveWaveRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
 
-AssociateApplicationsRequestRequestTypeDef = TypedDict(
-    "AssociateApplicationsRequestRequestTypeDef",
+class ArchiveWaveRequestRequestTypeDef(
+    _RequiredArchiveWaveRequestRequestTypeDef, _OptionalArchiveWaveRequestRequestTypeDef
+):
+    pass
+
+_RequiredAssociateApplicationsRequestRequestTypeDef = TypedDict(
+    "_RequiredAssociateApplicationsRequestRequestTypeDef",
     {
         "applicationIDs": Sequence[str],
         "waveID": str,
     },
 )
+_OptionalAssociateApplicationsRequestRequestTypeDef = TypedDict(
+    "_OptionalAssociateApplicationsRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
 
-AssociateSourceServersRequestRequestTypeDef = TypedDict(
-    "AssociateSourceServersRequestRequestTypeDef",
+class AssociateApplicationsRequestRequestTypeDef(
+    _RequiredAssociateApplicationsRequestRequestTypeDef,
+    _OptionalAssociateApplicationsRequestRequestTypeDef,
+):
+    pass
+
+_RequiredAssociateSourceServersRequestRequestTypeDef = TypedDict(
+    "_RequiredAssociateSourceServersRequestRequestTypeDef",
     {
         "applicationID": str,
         "sourceServerIDs": Sequence[str],
     },
 )
+_OptionalAssociateSourceServersRequestRequestTypeDef = TypedDict(
+    "_OptionalAssociateSourceServersRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+class AssociateSourceServersRequestRequestTypeDef(
+    _RequiredAssociateSourceServersRequestRequestTypeDef,
+    _OptionalAssociateSourceServersRequestRequestTypeDef,
+):
+    pass
 
 CPUTypeDef = TypedDict(
     "CPUTypeDef",
     {
         "cores": int,
         "modelName": str,
     },
@@ -308,14 +363,15 @@
     {
         "name": str,
     },
 )
 _OptionalCreateApplicationRequestRequestTypeDef = TypedDict(
     "_OptionalCreateApplicationRequestRequestTypeDef",
     {
+        "accountID": str,
         "description": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
 class CreateApplicationRequestRequestTypeDef(
@@ -358,14 +414,15 @@
     },
 )
 _OptionalCreateReplicationConfigurationTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalCreateReplicationConfigurationTemplateRequestRequestTypeDef",
     {
         "ebsEncryptionKeyArn": str,
         "tags": Mapping[str, str],
+        "useFipsEndpoint": bool,
     },
     total=False,
 )
 
 class CreateReplicationConfigurationTemplateRequestRequestTypeDef(
     _RequiredCreateReplicationConfigurationTemplateRequestRequestTypeDef,
     _OptionalCreateReplicationConfigurationTemplateRequestRequestTypeDef,
@@ -377,14 +434,15 @@
     {
         "name": str,
     },
 )
 _OptionalCreateWaveRequestRequestTypeDef = TypedDict(
     "_OptionalCreateWaveRequestRequestTypeDef",
     {
+        "accountID": str,
         "description": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
 class CreateWaveRequestRequestTypeDef(
@@ -418,27 +476,51 @@
     {
         "name": DataReplicationInitiationStepNameType,
         "status": DataReplicationInitiationStepStatusType,
     },
     total=False,
 )
 
-DeleteApplicationRequestRequestTypeDef = TypedDict(
-    "DeleteApplicationRequestRequestTypeDef",
+_RequiredDeleteApplicationRequestRequestTypeDef = TypedDict(
+    "_RequiredDeleteApplicationRequestRequestTypeDef",
     {
         "applicationID": str,
     },
 )
+_OptionalDeleteApplicationRequestRequestTypeDef = TypedDict(
+    "_OptionalDeleteApplicationRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
 
-DeleteJobRequestRequestTypeDef = TypedDict(
-    "DeleteJobRequestRequestTypeDef",
+class DeleteApplicationRequestRequestTypeDef(
+    _RequiredDeleteApplicationRequestRequestTypeDef, _OptionalDeleteApplicationRequestRequestTypeDef
+):
+    pass
+
+_RequiredDeleteJobRequestRequestTypeDef = TypedDict(
+    "_RequiredDeleteJobRequestRequestTypeDef",
     {
         "jobID": str,
     },
 )
+_OptionalDeleteJobRequestRequestTypeDef = TypedDict(
+    "_OptionalDeleteJobRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+class DeleteJobRequestRequestTypeDef(
+    _RequiredDeleteJobRequestRequestTypeDef, _OptionalDeleteJobRequestRequestTypeDef
+):
+    pass
 
 DeleteLaunchConfigurationTemplateRequestRequestTypeDef = TypedDict(
     "DeleteLaunchConfigurationTemplateRequestRequestTypeDef",
     {
         "launchConfigurationTemplateID": str,
     },
 )
@@ -446,34 +528,59 @@
 DeleteReplicationConfigurationTemplateRequestRequestTypeDef = TypedDict(
     "DeleteReplicationConfigurationTemplateRequestRequestTypeDef",
     {
         "replicationConfigurationTemplateID": str,
     },
 )
 
-DeleteSourceServerRequestRequestTypeDef = TypedDict(
-    "DeleteSourceServerRequestRequestTypeDef",
+_RequiredDeleteSourceServerRequestRequestTypeDef = TypedDict(
+    "_RequiredDeleteSourceServerRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
+_OptionalDeleteSourceServerRequestRequestTypeDef = TypedDict(
+    "_OptionalDeleteSourceServerRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+class DeleteSourceServerRequestRequestTypeDef(
+    _RequiredDeleteSourceServerRequestRequestTypeDef,
+    _OptionalDeleteSourceServerRequestRequestTypeDef,
+):
+    pass
 
 DeleteVcenterClientRequestRequestTypeDef = TypedDict(
     "DeleteVcenterClientRequestRequestTypeDef",
     {
         "vcenterClientID": str,
     },
 )
 
-DeleteWaveRequestRequestTypeDef = TypedDict(
-    "DeleteWaveRequestRequestTypeDef",
+_RequiredDeleteWaveRequestRequestTypeDef = TypedDict(
+    "_RequiredDeleteWaveRequestRequestTypeDef",
     {
         "waveID": str,
     },
 )
+_OptionalDeleteWaveRequestRequestTypeDef = TypedDict(
+    "_OptionalDeleteWaveRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+class DeleteWaveRequestRequestTypeDef(
+    _RequiredDeleteWaveRequestRequestTypeDef, _OptionalDeleteWaveRequestRequestTypeDef
+):
+    pass
 
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
@@ -486,14 +593,15 @@
     {
         "jobID": str,
     },
 )
 _OptionalDescribeJobLogItemsRequestRequestTypeDef = TypedDict(
     "_OptionalDescribeJobLogItemsRequestRequestTypeDef",
     {
+        "accountID": str,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
 class DescribeJobLogItemsRequestRequestTypeDef(
@@ -551,14 +659,15 @@
         "ebsEncryptionKeyArn": str,
         "replicationServerInstanceType": str,
         "replicationServersSecurityGroupsIDs": List[str],
         "stagingAreaSubnetId": str,
         "stagingAreaTags": Dict[str, str],
         "tags": Dict[str, str],
         "useDedicatedReplicationServer": bool,
+        "useFipsEndpoint": bool,
     },
     total=False,
 )
 
 class ReplicationConfigurationTemplateTypeDef(
     _RequiredReplicationConfigurationTemplateTypeDef,
     _OptionalReplicationConfigurationTemplateTypeDef,
@@ -597,36 +706,75 @@
         "tags": Dict[str, str],
         "vcenterClientID": str,
         "vcenterUUID": str,
     },
     total=False,
 )
 
-DisassociateApplicationsRequestRequestTypeDef = TypedDict(
-    "DisassociateApplicationsRequestRequestTypeDef",
+_RequiredDisassociateApplicationsRequestRequestTypeDef = TypedDict(
+    "_RequiredDisassociateApplicationsRequestRequestTypeDef",
     {
         "applicationIDs": Sequence[str],
         "waveID": str,
     },
 )
+_OptionalDisassociateApplicationsRequestRequestTypeDef = TypedDict(
+    "_OptionalDisassociateApplicationsRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
 
-DisassociateSourceServersRequestRequestTypeDef = TypedDict(
-    "DisassociateSourceServersRequestRequestTypeDef",
+class DisassociateApplicationsRequestRequestTypeDef(
+    _RequiredDisassociateApplicationsRequestRequestTypeDef,
+    _OptionalDisassociateApplicationsRequestRequestTypeDef,
+):
+    pass
+
+_RequiredDisassociateSourceServersRequestRequestTypeDef = TypedDict(
+    "_RequiredDisassociateSourceServersRequestRequestTypeDef",
     {
         "applicationID": str,
         "sourceServerIDs": Sequence[str],
     },
 )
+_OptionalDisassociateSourceServersRequestRequestTypeDef = TypedDict(
+    "_OptionalDisassociateSourceServersRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
 
-DisconnectFromServiceRequestRequestTypeDef = TypedDict(
-    "DisconnectFromServiceRequestRequestTypeDef",
+class DisassociateSourceServersRequestRequestTypeDef(
+    _RequiredDisassociateSourceServersRequestRequestTypeDef,
+    _OptionalDisassociateSourceServersRequestRequestTypeDef,
+):
+    pass
+
+_RequiredDisconnectFromServiceRequestRequestTypeDef = TypedDict(
+    "_RequiredDisconnectFromServiceRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
+_OptionalDisconnectFromServiceRequestRequestTypeDef = TypedDict(
+    "_OptionalDisconnectFromServiceRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+class DisconnectFromServiceRequestRequestTypeDef(
+    _RequiredDisconnectFromServiceRequestRequestTypeDef,
+    _OptionalDisconnectFromServiceRequestRequestTypeDef,
+):
+    pass
 
 DiskTypeDef = TypedDict(
     "DiskTypeDef",
     {
         "bytes": int,
         "deviceName": str,
     },
@@ -647,34 +795,72 @@
         "applicationsCount": int,
         "serversCount": int,
         "wavesCount": int,
     },
     total=False,
 )
 
-FinalizeCutoverRequestRequestTypeDef = TypedDict(
-    "FinalizeCutoverRequestRequestTypeDef",
+_RequiredFinalizeCutoverRequestRequestTypeDef = TypedDict(
+    "_RequiredFinalizeCutoverRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
+_OptionalFinalizeCutoverRequestRequestTypeDef = TypedDict(
+    "_OptionalFinalizeCutoverRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
 
-GetLaunchConfigurationRequestRequestTypeDef = TypedDict(
-    "GetLaunchConfigurationRequestRequestTypeDef",
+class FinalizeCutoverRequestRequestTypeDef(
+    _RequiredFinalizeCutoverRequestRequestTypeDef, _OptionalFinalizeCutoverRequestRequestTypeDef
+):
+    pass
+
+_RequiredGetLaunchConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredGetLaunchConfigurationRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
+_OptionalGetLaunchConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalGetLaunchConfigurationRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
 
-GetReplicationConfigurationRequestRequestTypeDef = TypedDict(
-    "GetReplicationConfigurationRequestRequestTypeDef",
+class GetLaunchConfigurationRequestRequestTypeDef(
+    _RequiredGetLaunchConfigurationRequestRequestTypeDef,
+    _OptionalGetLaunchConfigurationRequestRequestTypeDef,
+):
+    pass
+
+_RequiredGetReplicationConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredGetReplicationConfigurationRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
+_OptionalGetReplicationConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalGetReplicationConfigurationRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+class GetReplicationConfigurationRequestRequestTypeDef(
+    _RequiredGetReplicationConfigurationRequestRequestTypeDef,
+    _OptionalGetReplicationConfigurationRequestRequestTypeDef,
+):
+    pass
 
 IdentificationHintsTypeDef = TypedDict(
     "IdentificationHintsTypeDef",
     {
         "awsInstanceID": str,
         "fqdn": str,
         "hostname": str,
@@ -683,14 +869,15 @@
     },
     total=False,
 )
 
 ImportErrorDataTypeDef = TypedDict(
     "ImportErrorDataTypeDef",
     {
+        "accountID": str,
         "applicationID": str,
         "ec2LaunchTemplateID": str,
         "rawError": str,
         "rowNumber": int,
         "sourceServerID": str,
         "waveID": str,
     },
@@ -875,14 +1062,31 @@
     "ListImportsRequestFiltersTypeDef",
     {
         "importIDs": Sequence[str],
     },
     total=False,
 )
 
+ListManagedAccountsRequestRequestTypeDef = TypedDict(
+    "ListManagedAccountsRequestRequestTypeDef",
+    {
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+ManagedAccountTypeDef = TypedDict(
+    "ManagedAccountTypeDef",
+    {
+        "accountId": str,
+    },
+    total=False,
+)
+
 SourceServerActionsRequestFiltersTypeDef = TypedDict(
     "SourceServerActionsRequestFiltersTypeDef",
     {
         "actionIDs": Sequence[str],
     },
     total=False,
 )
@@ -907,20 +1111,32 @@
     {
         "isArchived": bool,
         "waveIDs": Sequence[str],
     },
     total=False,
 )
 
-MarkAsArchivedRequestRequestTypeDef = TypedDict(
-    "MarkAsArchivedRequestRequestTypeDef",
+_RequiredMarkAsArchivedRequestRequestTypeDef = TypedDict(
+    "_RequiredMarkAsArchivedRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
+_OptionalMarkAsArchivedRequestRequestTypeDef = TypedDict(
+    "_OptionalMarkAsArchivedRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+class MarkAsArchivedRequestRequestTypeDef(
+    _RequiredMarkAsArchivedRequestRequestTypeDef, _OptionalMarkAsArchivedRequestRequestTypeDef
+):
+    pass
 
 NetworkInterfaceTypeDef = TypedDict(
     "NetworkInterfaceTypeDef",
     {
         "ips": List[str],
         "isPrimary": bool,
         "macAddress": str,
@@ -932,14 +1148,33 @@
     "OSTypeDef",
     {
         "fullString": str,
     },
     total=False,
 )
 
+_RequiredPauseReplicationRequestRequestTypeDef = TypedDict(
+    "_RequiredPauseReplicationRequestRequestTypeDef",
+    {
+        "sourceServerID": str,
+    },
+)
+_OptionalPauseReplicationRequestRequestTypeDef = TypedDict(
+    "_OptionalPauseReplicationRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+class PauseReplicationRequestRequestTypeDef(
+    _RequiredPauseReplicationRequestRequestTypeDef, _OptionalPauseReplicationRequestRequestTypeDef
+):
+    pass
+
 SsmExternalParameterTypeDef = TypedDict(
     "SsmExternalParameterTypeDef",
     {
         "dynamicPath": str,
     },
     total=False,
 )
@@ -948,21 +1183,34 @@
     "SsmParameterStoreParameterTypeDef",
     {
         "parameterName": str,
         "parameterType": Literal["STRING"],
     },
 )
 
-RemoveSourceServerActionRequestRequestTypeDef = TypedDict(
-    "RemoveSourceServerActionRequestRequestTypeDef",
+_RequiredRemoveSourceServerActionRequestRequestTypeDef = TypedDict(
+    "_RequiredRemoveSourceServerActionRequestRequestTypeDef",
     {
         "actionID": str,
         "sourceServerID": str,
     },
 )
+_OptionalRemoveSourceServerActionRequestRequestTypeDef = TypedDict(
+    "_OptionalRemoveSourceServerActionRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+class RemoveSourceServerActionRequestRequestTypeDef(
+    _RequiredRemoveSourceServerActionRequestRequestTypeDef,
+    _OptionalRemoveSourceServerActionRequestRequestTypeDef,
+):
+    pass
 
 RemoveTemplateActionRequestRequestTypeDef = TypedDict(
     "RemoveTemplateActionRequestRequestTypeDef",
     {
         "actionID": str,
         "launchConfigurationTemplateID": str,
     },
@@ -976,30 +1224,63 @@
         "isBootDisk": bool,
         "stagingDiskType": ReplicationConfigurationReplicatedDiskStagingDiskTypeType,
         "throughput": int,
     },
     total=False,
 )
 
-RetryDataReplicationRequestRequestTypeDef = TypedDict(
-    "RetryDataReplicationRequestRequestTypeDef",
+_RequiredResumeReplicationRequestRequestTypeDef = TypedDict(
+    "_RequiredResumeReplicationRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
+_OptionalResumeReplicationRequestRequestTypeDef = TypedDict(
+    "_OptionalResumeReplicationRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+class ResumeReplicationRequestRequestTypeDef(
+    _RequiredResumeReplicationRequestRequestTypeDef, _OptionalResumeReplicationRequestRequestTypeDef
+):
+    pass
+
+_RequiredRetryDataReplicationRequestRequestTypeDef = TypedDict(
+    "_RequiredRetryDataReplicationRequestRequestTypeDef",
+    {
+        "sourceServerID": str,
+    },
+)
+_OptionalRetryDataReplicationRequestRequestTypeDef = TypedDict(
+    "_OptionalRetryDataReplicationRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+class RetryDataReplicationRequestRequestTypeDef(
+    _RequiredRetryDataReplicationRequestRequestTypeDef,
+    _OptionalRetryDataReplicationRequestRequestTypeDef,
+):
+    pass
 
 _RequiredStartCutoverRequestRequestTypeDef = TypedDict(
     "_RequiredStartCutoverRequestRequestTypeDef",
     {
         "sourceServerIDs": Sequence[str],
     },
 )
 _OptionalStartCutoverRequestRequestTypeDef = TypedDict(
     "_OptionalStartCutoverRequestRequestTypeDef",
     {
+        "accountID": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
 class StartCutoverRequestRequestTypeDef(
     _RequiredStartCutoverRequestRequestTypeDef, _OptionalStartCutoverRequestRequestTypeDef
@@ -1022,40 +1303,72 @@
 )
 
 class StartExportRequestRequestTypeDef(
     _RequiredStartExportRequestRequestTypeDef, _OptionalStartExportRequestRequestTypeDef
 ):
     pass
 
-StartReplicationRequestRequestTypeDef = TypedDict(
-    "StartReplicationRequestRequestTypeDef",
+_RequiredStartReplicationRequestRequestTypeDef = TypedDict(
+    "_RequiredStartReplicationRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
+_OptionalStartReplicationRequestRequestTypeDef = TypedDict(
+    "_OptionalStartReplicationRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+class StartReplicationRequestRequestTypeDef(
+    _RequiredStartReplicationRequestRequestTypeDef, _OptionalStartReplicationRequestRequestTypeDef
+):
+    pass
 
 _RequiredStartTestRequestRequestTypeDef = TypedDict(
     "_RequiredStartTestRequestRequestTypeDef",
     {
         "sourceServerIDs": Sequence[str],
     },
 )
 _OptionalStartTestRequestRequestTypeDef = TypedDict(
     "_OptionalStartTestRequestRequestTypeDef",
     {
+        "accountID": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
 class StartTestRequestRequestTypeDef(
     _RequiredStartTestRequestRequestTypeDef, _OptionalStartTestRequestRequestTypeDef
 ):
     pass
 
+_RequiredStopReplicationRequestRequestTypeDef = TypedDict(
+    "_RequiredStopReplicationRequestRequestTypeDef",
+    {
+        "sourceServerID": str,
+    },
+)
+_OptionalStopReplicationRequestRequestTypeDef = TypedDict(
+    "_OptionalStopReplicationRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+class StopReplicationRequestRequestTypeDef(
+    _RequiredStopReplicationRequestRequestTypeDef, _OptionalStopReplicationRequestRequestTypeDef
+):
+    pass
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -1065,38 +1378,64 @@
     {
         "sourceServerIDs": Sequence[str],
     },
 )
 _OptionalTerminateTargetInstancesRequestRequestTypeDef = TypedDict(
     "_OptionalTerminateTargetInstancesRequestRequestTypeDef",
     {
+        "accountID": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
 class TerminateTargetInstancesRequestRequestTypeDef(
     _RequiredTerminateTargetInstancesRequestRequestTypeDef,
     _OptionalTerminateTargetInstancesRequestRequestTypeDef,
 ):
     pass
 
-UnarchiveApplicationRequestRequestTypeDef = TypedDict(
-    "UnarchiveApplicationRequestRequestTypeDef",
+_RequiredUnarchiveApplicationRequestRequestTypeDef = TypedDict(
+    "_RequiredUnarchiveApplicationRequestRequestTypeDef",
     {
         "applicationID": str,
     },
 )
+_OptionalUnarchiveApplicationRequestRequestTypeDef = TypedDict(
+    "_OptionalUnarchiveApplicationRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
 
-UnarchiveWaveRequestRequestTypeDef = TypedDict(
-    "UnarchiveWaveRequestRequestTypeDef",
+class UnarchiveApplicationRequestRequestTypeDef(
+    _RequiredUnarchiveApplicationRequestRequestTypeDef,
+    _OptionalUnarchiveApplicationRequestRequestTypeDef,
+):
+    pass
+
+_RequiredUnarchiveWaveRequestRequestTypeDef = TypedDict(
+    "_RequiredUnarchiveWaveRequestRequestTypeDef",
     {
         "waveID": str,
     },
 )
+_OptionalUnarchiveWaveRequestRequestTypeDef = TypedDict(
+    "_OptionalUnarchiveWaveRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+class UnarchiveWaveRequestRequestTypeDef(
+    _RequiredUnarchiveWaveRequestRequestTypeDef, _OptionalUnarchiveWaveRequestRequestTypeDef
+):
+    pass
 
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
@@ -1107,14 +1446,15 @@
     {
         "applicationID": str,
     },
 )
 _OptionalUpdateApplicationRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateApplicationRequestRequestTypeDef",
     {
+        "accountID": str,
         "description": str,
         "name": str,
     },
     total=False,
 )
 
 class UpdateApplicationRequestRequestTypeDef(
@@ -1140,41 +1480,56 @@
         "ebsEncryption": ReplicationConfigurationEbsEncryptionType,
         "ebsEncryptionKeyArn": str,
         "replicationServerInstanceType": str,
         "replicationServersSecurityGroupsIDs": Sequence[str],
         "stagingAreaSubnetId": str,
         "stagingAreaTags": Mapping[str, str],
         "useDedicatedReplicationServer": bool,
+        "useFipsEndpoint": bool,
     },
     total=False,
 )
 
 class UpdateReplicationConfigurationTemplateRequestRequestTypeDef(
     _RequiredUpdateReplicationConfigurationTemplateRequestRequestTypeDef,
     _OptionalUpdateReplicationConfigurationTemplateRequestRequestTypeDef,
 ):
     pass
 
-UpdateSourceServerReplicationTypeRequestRequestTypeDef = TypedDict(
-    "UpdateSourceServerReplicationTypeRequestRequestTypeDef",
+_RequiredUpdateSourceServerReplicationTypeRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateSourceServerReplicationTypeRequestRequestTypeDef",
     {
         "replicationType": ReplicationTypeType,
         "sourceServerID": str,
     },
 )
+_OptionalUpdateSourceServerReplicationTypeRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateSourceServerReplicationTypeRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+class UpdateSourceServerReplicationTypeRequestRequestTypeDef(
+    _RequiredUpdateSourceServerReplicationTypeRequestRequestTypeDef,
+    _OptionalUpdateSourceServerReplicationTypeRequestRequestTypeDef,
+):
+    pass
 
 _RequiredUpdateWaveRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWaveRequestRequestTypeDef",
     {
         "waveID": str,
     },
 )
 _OptionalUpdateWaveRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateWaveRequestRequestTypeDef",
     {
+        "accountID": str,
         "description": str,
         "name": str,
     },
     total=False,
 )
 
 class UpdateWaveRequestRequestTypeDef(
@@ -1257,25 +1612,39 @@
         "replicationConfigurationTemplateID": str,
         "replicationServerInstanceType": str,
         "replicationServersSecurityGroupsIDs": List[str],
         "stagingAreaSubnetId": str,
         "stagingAreaTags": Dict[str, str],
         "tags": Dict[str, str],
         "useDedicatedReplicationServer": bool,
+        "useFipsEndpoint": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ChangeServerLifeCycleStateRequestRequestTypeDef = TypedDict(
-    "ChangeServerLifeCycleStateRequestRequestTypeDef",
+_RequiredChangeServerLifeCycleStateRequestRequestTypeDef = TypedDict(
+    "_RequiredChangeServerLifeCycleStateRequestRequestTypeDef",
     {
         "lifeCycle": ChangeServerLifeCycleStateSourceServerLifecycleTypeDef,
         "sourceServerID": str,
     },
 )
+_OptionalChangeServerLifeCycleStateRequestRequestTypeDef = TypedDict(
+    "_OptionalChangeServerLifeCycleStateRequestRequestTypeDef",
+    {
+        "accountID": str,
+    },
+    total=False,
+)
+
+class ChangeServerLifeCycleStateRequestRequestTypeDef(
+    _RequiredChangeServerLifeCycleStateRequestRequestTypeDef,
+    _OptionalChangeServerLifeCycleStateRequestRequestTypeDef,
+):
+    pass
 
 DataReplicationInitiationTypeDef = TypedDict(
     "DataReplicationInitiationTypeDef",
     {
         "nextAttemptDateTime": str,
         "startDateTime": str,
         "steps": List[DataReplicationInitiationStepTypeDef],
@@ -1288,14 +1657,15 @@
     {
         "jobID": str,
     },
 )
 _OptionalDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef = TypedDict(
     "_OptionalDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef",
     {
+        "accountID": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef(
     _RequiredDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef,
@@ -1365,26 +1735,36 @@
 
 class ListImportErrorsRequestListImportErrorsPaginateTypeDef(
     _RequiredListImportErrorsRequestListImportErrorsPaginateTypeDef,
     _OptionalListImportErrorsRequestListImportErrorsPaginateTypeDef,
 ):
     pass
 
+ListManagedAccountsRequestListManagedAccountsPaginateTypeDef = TypedDict(
+    "ListManagedAccountsRequestListManagedAccountsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 DescribeJobsRequestDescribeJobsPaginateTypeDef = TypedDict(
     "DescribeJobsRequestDescribeJobsPaginateTypeDef",
     {
+        "accountID": str,
         "filters": DescribeJobsRequestFiltersTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeJobsRequestRequestTypeDef = TypedDict(
     "DescribeJobsRequestRequestTypeDef",
     {
+        "accountID": str,
         "filters": DescribeJobsRequestFiltersTypeDef,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
@@ -1396,23 +1776,25 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef = TypedDict(
     "DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef",
     {
+        "accountID": str,
         "filters": DescribeSourceServersRequestFiltersTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeSourceServersRequestRequestTypeDef = TypedDict(
     "DescribeSourceServersRequestRequestTypeDef",
     {
+        "accountID": str,
         "filters": DescribeSourceServersRequestFiltersTypeDef,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
@@ -1518,23 +1900,25 @@
     },
     total=False,
 )
 
 ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
     "ListApplicationsRequestListApplicationsPaginateTypeDef",
     {
+        "accountID": str,
         "filters": ListApplicationsRequestFiltersTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListApplicationsRequestRequestTypeDef = TypedDict(
     "ListApplicationsRequestRequestTypeDef",
     {
+        "accountID": str,
         "filters": ListApplicationsRequestFiltersTypeDef,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
@@ -1572,23 +1956,33 @@
         "filters": ListImportsRequestFiltersTypeDef,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+ListManagedAccountsResponseTypeDef = TypedDict(
+    "ListManagedAccountsResponseTypeDef",
+    {
+        "items": List[ManagedAccountTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredListSourceServerActionsRequestListSourceServerActionsPaginateTypeDef = TypedDict(
     "_RequiredListSourceServerActionsRequestListSourceServerActionsPaginateTypeDef",
     {
         "sourceServerID": str,
     },
 )
 _OptionalListSourceServerActionsRequestListSourceServerActionsPaginateTypeDef = TypedDict(
     "_OptionalListSourceServerActionsRequestListSourceServerActionsPaginateTypeDef",
     {
+        "accountID": str,
         "filters": SourceServerActionsRequestFiltersTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class ListSourceServerActionsRequestListSourceServerActionsPaginateTypeDef(
@@ -1602,14 +1996,15 @@
     {
         "sourceServerID": str,
     },
 )
 _OptionalListSourceServerActionsRequestRequestTypeDef = TypedDict(
     "_OptionalListSourceServerActionsRequestRequestTypeDef",
     {
+        "accountID": str,
         "filters": SourceServerActionsRequestFiltersTypeDef,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
@@ -1661,23 +2056,25 @@
     _OptionalListTemplateActionsRequestRequestTypeDef,
 ):
     pass
 
 ListWavesRequestListWavesPaginateTypeDef = TypedDict(
     "ListWavesRequestListWavesPaginateTypeDef",
     {
+        "accountID": str,
         "filters": ListWavesRequestFiltersTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListWavesRequestRequestTypeDef = TypedDict(
     "ListWavesRequestRequestTypeDef",
     {
+        "accountID": str,
         "filters": ListWavesRequestFiltersTypeDef,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
@@ -1705,14 +2102,15 @@
         "order": int,
         "sourceServerID": str,
     },
 )
 _OptionalPutSourceServerActionRequestRequestTypeDef = TypedDict(
     "_OptionalPutSourceServerActionRequestRequestTypeDef",
     {
+        "accountID": str,
         "active": bool,
         "category": ActionCategoryType,
         "description": str,
         "documentVersion": str,
         "externalParameters": Mapping[str, SsmExternalParameterTypeDef],
         "mustSucceedForCutover": bool,
         "parameters": Mapping[str, Sequence[SsmParameterStoreParameterTypeDef]],
@@ -1792,37 +2190,14 @@
         "order": int,
         "parameters": Dict[str, List[SsmParameterStoreParameterTypeDef]],
         "timeoutSeconds": int,
     },
     total=False,
 )
 
-_RequiredSsmDocumentOutputTypeDef = TypedDict(
-    "_RequiredSsmDocumentOutputTypeDef",
-    {
-        "actionName": str,
-        "ssmDocumentName": str,
-    },
-)
-_OptionalSsmDocumentOutputTypeDef = TypedDict(
-    "_OptionalSsmDocumentOutputTypeDef",
-    {
-        "externalParameters": Dict[str, SsmExternalParameterTypeDef],
-        "mustSucceedForCutover": bool,
-        "parameters": Dict[str, List[SsmParameterStoreParameterTypeDef]],
-        "timeoutSeconds": int,
-    },
-    total=False,
-)
-
-class SsmDocumentOutputTypeDef(
-    _RequiredSsmDocumentOutputTypeDef, _OptionalSsmDocumentOutputTypeDef
-):
-    pass
-
 _RequiredSsmDocumentTypeDef = TypedDict(
     "_RequiredSsmDocumentTypeDef",
     {
         "actionName": str,
         "ssmDocumentName": str,
     },
 )
@@ -1894,41 +2269,44 @@
         "replicatedDisks": List[ReplicationConfigurationReplicatedDiskTypeDef],
         "replicationServerInstanceType": str,
         "replicationServersSecurityGroupsIDs": List[str],
         "sourceServerID": str,
         "stagingAreaSubnetId": str,
         "stagingAreaTags": Dict[str, str],
         "useDedicatedReplicationServer": bool,
+        "useFipsEndpoint": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateReplicationConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateReplicationConfigurationRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
 _OptionalUpdateReplicationConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateReplicationConfigurationRequestRequestTypeDef",
     {
+        "accountID": str,
         "associateDefaultSecurityGroup": bool,
         "bandwidthThrottling": int,
         "createPublicIP": bool,
         "dataPlaneRouting": ReplicationConfigurationDataPlaneRoutingType,
         "defaultLargeStagingDiskType": ReplicationConfigurationDefaultLargeStagingDiskTypeType,
         "ebsEncryption": ReplicationConfigurationEbsEncryptionType,
         "ebsEncryptionKeyArn": str,
         "name": str,
         "replicatedDisks": Sequence[ReplicationConfigurationReplicatedDiskTypeDef],
         "replicationServerInstanceType": str,
         "replicationServersSecurityGroupsIDs": Sequence[str],
         "stagingAreaSubnetId": str,
         "stagingAreaTags": Mapping[str, str],
         "useDedicatedReplicationServer": bool,
+        "useFipsEndpoint": bool,
     },
     total=False,
 )
 
 class UpdateReplicationConfigurationRequestRequestTypeDef(
     _RequiredUpdateReplicationConfigurationRequestRequestTypeDef,
     _OptionalUpdateReplicationConfigurationRequestRequestTypeDef,
@@ -2073,32 +2451,20 @@
 
 JobPostLaunchActionsLaunchStatusTypeDef = TypedDict(
     "JobPostLaunchActionsLaunchStatusTypeDef",
     {
         "executionID": str,
         "executionStatus": PostLaunchActionExecutionStatusType,
         "failureReason": str,
-        "ssmDocument": SsmDocumentOutputTypeDef,
+        "ssmDocument": SsmDocumentTypeDef,
         "ssmDocumentType": SsmDocumentTypeType,
     },
     total=False,
 )
 
-PostLaunchActionsOutputTypeDef = TypedDict(
-    "PostLaunchActionsOutputTypeDef",
-    {
-        "cloudWatchLogGroupName": str,
-        "deployment": PostLaunchActionsDeploymentTypeType,
-        "s3LogBucket": str,
-        "s3OutputKeyPrefix": str,
-        "ssmDocuments": List[SsmDocumentOutputTypeDef],
-    },
-    total=False,
-)
-
 PostLaunchActionsTypeDef = TypedDict(
     "PostLaunchActionsTypeDef",
     {
         "cloudWatchLogGroupName": str,
         "deployment": PostLaunchActionsDeploymentTypeType,
         "s3LogBucket": str,
         "s3OutputKeyPrefix": str,
@@ -2187,14 +2553,35 @@
     {
         "postLaunchActionsLaunchStatusList": List[JobPostLaunchActionsLaunchStatusTypeDef],
         "ssmAgentDiscoveryDatetime": str,
     },
     total=False,
 )
 
+CreateLaunchConfigurationTemplateRequestRequestTypeDef = TypedDict(
+    "CreateLaunchConfigurationTemplateRequestRequestTypeDef",
+    {
+        "associatePublicIpAddress": bool,
+        "bootMode": BootModeType,
+        "copyPrivateIp": bool,
+        "copyTags": bool,
+        "enableMapAutoTagging": bool,
+        "largeVolumeConf": LaunchTemplateDiskConfTypeDef,
+        "launchDisposition": LaunchDispositionType,
+        "licensing": LicensingTypeDef,
+        "mapAutoTaggingMpeID": str,
+        "postLaunchActions": PostLaunchActionsTypeDef,
+        "smallVolumeConf": LaunchTemplateDiskConfTypeDef,
+        "smallVolumeMaxSize": int,
+        "tags": Mapping[str, str],
+        "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
+    },
+    total=False,
+)
+
 LaunchConfigurationTemplateResponseTypeDef = TypedDict(
     "LaunchConfigurationTemplateResponseTypeDef",
     {
         "arn": str,
         "associatePublicIpAddress": bool,
         "bootMode": BootModeType,
         "copyPrivateIp": bool,
@@ -2202,15 +2589,15 @@
         "ec2LaunchTemplateID": str,
         "enableMapAutoTagging": bool,
         "largeVolumeConf": LaunchTemplateDiskConfTypeDef,
         "launchConfigurationTemplateID": str,
         "launchDisposition": LaunchDispositionType,
         "licensing": LicensingTypeDef,
         "mapAutoTaggingMpeID": str,
-        "postLaunchActions": PostLaunchActionsOutputTypeDef,
+        "postLaunchActions": PostLaunchActionsTypeDef,
         "smallVolumeConf": LaunchTemplateDiskConfTypeDef,
         "smallVolumeMaxSize": int,
         "tags": Dict[str, str],
         "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2231,15 +2618,15 @@
         "copyTags": bool,
         "ec2LaunchTemplateID": str,
         "enableMapAutoTagging": bool,
         "largeVolumeConf": LaunchTemplateDiskConfTypeDef,
         "launchDisposition": LaunchDispositionType,
         "licensing": LicensingTypeDef,
         "mapAutoTaggingMpeID": str,
-        "postLaunchActions": PostLaunchActionsOutputTypeDef,
+        "postLaunchActions": PostLaunchActionsTypeDef,
         "smallVolumeConf": LaunchTemplateDiskConfTypeDef,
         "smallVolumeMaxSize": int,
         "tags": Dict[str, str],
         "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
     },
     total=False,
 )
@@ -2257,52 +2644,31 @@
         "copyTags": bool,
         "ec2LaunchTemplateID": str,
         "enableMapAutoTagging": bool,
         "launchDisposition": LaunchDispositionType,
         "licensing": LicensingTypeDef,
         "mapAutoTaggingMpeID": str,
         "name": str,
-        "postLaunchActions": PostLaunchActionsOutputTypeDef,
+        "postLaunchActions": PostLaunchActionsTypeDef,
         "sourceServerID": str,
         "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateLaunchConfigurationTemplateRequestRequestTypeDef = TypedDict(
-    "CreateLaunchConfigurationTemplateRequestRequestTypeDef",
-    {
-        "associatePublicIpAddress": bool,
-        "bootMode": BootModeType,
-        "copyPrivateIp": bool,
-        "copyTags": bool,
-        "enableMapAutoTagging": bool,
-        "largeVolumeConf": LaunchTemplateDiskConfTypeDef,
-        "launchDisposition": LaunchDispositionType,
-        "licensing": LicensingTypeDef,
-        "mapAutoTaggingMpeID": str,
-        "postLaunchActions": PostLaunchActionsTypeDef,
-        "smallVolumeConf": LaunchTemplateDiskConfTypeDef,
-        "smallVolumeMaxSize": int,
-        "tags": Mapping[str, str],
-        "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
-    },
-    total=False,
-)
-
-PostLaunchActionsUnionTypeDef = Union[PostLaunchActionsTypeDef, PostLaunchActionsOutputTypeDef]
 _RequiredUpdateLaunchConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLaunchConfigurationRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
 _OptionalUpdateLaunchConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateLaunchConfigurationRequestRequestTypeDef",
     {
+        "accountID": str,
         "bootMode": BootModeType,
         "copyPrivateIp": bool,
         "copyTags": bool,
         "enableMapAutoTagging": bool,
         "launchDisposition": LaunchDispositionType,
         "licensing": LicensingTypeDef,
         "mapAutoTaggingMpeID": str,
```

### Comparing `types-aiobotocore-mgn-2.5.2.post1/types_aiobotocore_mgn.egg-info/SOURCES.txt` & `types-aiobotocore-mgn-2.5.2.post2/types_aiobotocore_mgn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

