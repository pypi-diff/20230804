# Comparing `tmp/types-aiobotocore-proton-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-proton-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-proton-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:49 2023, max compression
+gzip compressed data, was "types-aiobotocore-proton-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:21 2023, max compression
```

## Comparing `types-aiobotocore-proton-2.5.2.post1.tar` & `types-aiobotocore-proton-2.5.2.post2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:49.957491 types-aiobotocore-proton-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:45:08.000000 types-aiobotocore-proton-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    31305 2023-08-02 14:52:49.957491 types-aiobotocore-proton-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    29791 2023-08-02 14:45:08.000000 types-aiobotocore-proton-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:49.957491 types-aiobotocore-proton-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-08-02 14:45:07.000000 types-aiobotocore-proton-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:49.957491 types-aiobotocore-proton-2.5.2.post1/types_aiobotocore_proton/
--rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-08-02 14:45:08.000000 types-aiobotocore-proton-2.5.2.post1/types_aiobotocore_proton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7821 2023-08-02 14:45:08.000000 types-aiobotocore-proton-2.5.2.post1/types_aiobotocore_proton/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-08-02 14:45:08.000000 types-aiobotocore-proton-2.5.2.post1/types_aiobotocore_proton/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    75675 2023-08-02 14:45:08.000000 types-aiobotocore-proton-2.5.2.post1/types_aiobotocore_proton/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    75552 2023-08-02 14:45:08.000000 types-aiobotocore-proton-2.5.2.post1/types_aiobotocore_proton/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15582 2023-08-02 14:45:09.000000 types-aiobotocore-proton-2.5.2.post1/types_aiobotocore_proton/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15580 2023-08-02 14:45:08.000000 types-aiobotocore-proton-2.5.2.post1/types_aiobotocore_proton/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    26121 2023-08-02 14:45:08.000000 types-aiobotocore-proton-2.5.2.post1/types_aiobotocore_proton/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    26099 2023-08-02 14:45:08.000000 types-aiobotocore-proton-2.5.2.post1/types_aiobotocore_proton/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:45:08.000000 types-aiobotocore-proton-2.5.2.post1/types_aiobotocore_proton/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   105540 2023-08-02 14:45:12.000000 types-aiobotocore-proton-2.5.2.post1/types_aiobotocore_proton/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   105367 2023-08-02 14:45:09.000000 types-aiobotocore-proton-2.5.2.post1/types_aiobotocore_proton/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:45:08.000000 types-aiobotocore-proton-2.5.2.post1/types_aiobotocore_proton/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-08-02 14:45:08.000000 types-aiobotocore-proton-2.5.2.post1/types_aiobotocore_proton/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10755 2023-08-02 14:45:08.000000 types-aiobotocore-proton-2.5.2.post1/types_aiobotocore_proton/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:49.957491 types-aiobotocore-proton-2.5.2.post1/types_aiobotocore_proton.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    31305 2023-08-02 14:52:49.000000 types-aiobotocore-proton-2.5.2.post1/types_aiobotocore_proton.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-08-02 14:52:49.000000 types-aiobotocore-proton-2.5.2.post1/types_aiobotocore_proton.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:49.000000 types-aiobotocore-proton-2.5.2.post1/types_aiobotocore_proton.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:49.000000 types-aiobotocore-proton-2.5.2.post1/types_aiobotocore_proton.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:49.000000 types-aiobotocore-proton-2.5.2.post1/types_aiobotocore_proton.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-02 14:52:49.000000 types-aiobotocore-proton-2.5.2.post1/types_aiobotocore_proton.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:21.946643 types-aiobotocore-proton-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:47:13.000000 types-aiobotocore-proton-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    18715 2023-08-04 13:59:21.946643 types-aiobotocore-proton-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    17201 2023-08-04 13:47:13.000000 types-aiobotocore-proton-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:21.946643 types-aiobotocore-proton-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2065 2023-08-04 13:47:13.000000 types-aiobotocore-proton-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:21.936643 types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8018 2023-08-04 13:47:13.000000 types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8017 2023-08-04 13:47:13.000000 types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      928 2023-08-04 13:47:13.000000 types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    78108 2023-08-04 13:47:14.000000 types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    77981 2023-08-04 13:47:13.000000 types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    15953 2023-08-04 13:47:16.000000 types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    15951 2023-08-04 13:47:14.000000 types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    27543 2023-08-04 13:47:14.000000 types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    27520 2023-08-04 13:47:14.000000 types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:47:13.000000 types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   112775 2023-08-04 13:47:19.000000 types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   112590 2023-08-04 13:47:17.000000 types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:47:13.000000 types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton/version.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10765 2023-08-04 13:47:14.000000 types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton/waiter.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10755 2023-08-04 13:47:14.000000 types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton/waiter.pyi
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:21.946643 types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    18715 2023-08-04 13:59:21.000000 types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      865 2023-08-04 13:59:21.000000 types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:21.000000 types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:21.000000 types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:21.000000 types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       25 2023-08-04 13:59:21.000000 types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-proton-2.5.2.post1/LICENSE` & `types-aiobotocore-proton-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-proton-2.5.2.post1/setup.py` & `types-aiobotocore-proton-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-proton",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_proton"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Proton 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-proton-2.5.2.post1/types_aiobotocore_proton/__init__.py` & `types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
         ComponentDeletedWaiter,
         ComponentDeployedWaiter,
         EnvironmentDeployedWaiter,
         EnvironmentTemplateVersionRegisteredWaiter,
         ListComponentOutputsPaginator,
         ListComponentProvisionedResourcesPaginator,
         ListComponentsPaginator,
+        ListDeploymentsPaginator,
         ListEnvironmentAccountConnectionsPaginator,
         ListEnvironmentOutputsPaginator,
         ListEnvironmentProvisionedResourcesPaginator,
         ListEnvironmentTemplateVersionsPaginator,
         ListEnvironmentTemplatesPaginator,
         ListEnvironmentsPaginator,
         ListRepositoriesPaginator,
@@ -56,14 +57,15 @@
     service_pipeline_deployed_waiter: ServicePipelineDeployedWaiter = client.get_waiter("service_pipeline_deployed")
     service_template_version_registered_waiter: ServiceTemplateVersionRegisteredWaiter = client.get_waiter("service_template_version_registered")
     service_updated_waiter: ServiceUpdatedWaiter = client.get_waiter("service_updated")
 
     list_component_outputs_paginator: ListComponentOutputsPaginator = client.get_paginator("list_component_outputs")
     list_component_provisioned_resources_paginator: ListComponentProvisionedResourcesPaginator = client.get_paginator("list_component_provisioned_resources")
     list_components_paginator: ListComponentsPaginator = client.get_paginator("list_components")
+    list_deployments_paginator: ListDeploymentsPaginator = client.get_paginator("list_deployments")
     list_environment_account_connections_paginator: ListEnvironmentAccountConnectionsPaginator = client.get_paginator("list_environment_account_connections")
     list_environment_outputs_paginator: ListEnvironmentOutputsPaginator = client.get_paginator("list_environment_outputs")
     list_environment_provisioned_resources_paginator: ListEnvironmentProvisionedResourcesPaginator = client.get_paginator("list_environment_provisioned_resources")
     list_environment_template_versions_paginator: ListEnvironmentTemplateVersionsPaginator = client.get_paginator("list_environment_template_versions")
     list_environment_templates_paginator: ListEnvironmentTemplatesPaginator = client.get_paginator("list_environment_templates")
     list_environments_paginator: ListEnvironmentsPaginator = client.get_paginator("list_environments")
     list_repositories_paginator: ListRepositoriesPaginator = client.get_paginator("list_repositories")
@@ -80,14 +82,15 @@
     ```
 """
 from .client import ProtonClient
 from .paginator import (
     ListComponentOutputsPaginator,
     ListComponentProvisionedResourcesPaginator,
     ListComponentsPaginator,
+    ListDeploymentsPaginator,
     ListEnvironmentAccountConnectionsPaginator,
     ListEnvironmentOutputsPaginator,
     ListEnvironmentProvisionedResourcesPaginator,
     ListEnvironmentsPaginator,
     ListEnvironmentTemplatesPaginator,
     ListEnvironmentTemplateVersionsPaginator,
     ListRepositoriesPaginator,
@@ -123,14 +126,15 @@
     "ComponentDeletedWaiter",
     "ComponentDeployedWaiter",
     "EnvironmentDeployedWaiter",
     "EnvironmentTemplateVersionRegisteredWaiter",
     "ListComponentOutputsPaginator",
     "ListComponentProvisionedResourcesPaginator",
     "ListComponentsPaginator",
+    "ListDeploymentsPaginator",
     "ListEnvironmentAccountConnectionsPaginator",
     "ListEnvironmentOutputsPaginator",
     "ListEnvironmentProvisionedResourcesPaginator",
     "ListEnvironmentTemplateVersionsPaginator",
     "ListEnvironmentTemplatesPaginator",
     "ListEnvironmentsPaginator",
     "ListRepositoriesPaginator",
```

### Comparing `types-aiobotocore-proton-2.5.2.post1/types_aiobotocore_proton/__init__.pyi` & `types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
         ComponentDeletedWaiter,
         ComponentDeployedWaiter,
         EnvironmentDeployedWaiter,
         EnvironmentTemplateVersionRegisteredWaiter,
         ListComponentOutputsPaginator,
         ListComponentProvisionedResourcesPaginator,
         ListComponentsPaginator,
+        ListDeploymentsPaginator,
         ListEnvironmentAccountConnectionsPaginator,
         ListEnvironmentOutputsPaginator,
         ListEnvironmentProvisionedResourcesPaginator,
         ListEnvironmentTemplateVersionsPaginator,
         ListEnvironmentTemplatesPaginator,
         ListEnvironmentsPaginator,
         ListRepositoriesPaginator,
@@ -56,14 +57,15 @@
     service_pipeline_deployed_waiter: ServicePipelineDeployedWaiter = client.get_waiter("service_pipeline_deployed")
     service_template_version_registered_waiter: ServiceTemplateVersionRegisteredWaiter = client.get_waiter("service_template_version_registered")
     service_updated_waiter: ServiceUpdatedWaiter = client.get_waiter("service_updated")
 
     list_component_outputs_paginator: ListComponentOutputsPaginator = client.get_paginator("list_component_outputs")
     list_component_provisioned_resources_paginator: ListComponentProvisionedResourcesPaginator = client.get_paginator("list_component_provisioned_resources")
     list_components_paginator: ListComponentsPaginator = client.get_paginator("list_components")
+    list_deployments_paginator: ListDeploymentsPaginator = client.get_paginator("list_deployments")
     list_environment_account_connections_paginator: ListEnvironmentAccountConnectionsPaginator = client.get_paginator("list_environment_account_connections")
     list_environment_outputs_paginator: ListEnvironmentOutputsPaginator = client.get_paginator("list_environment_outputs")
     list_environment_provisioned_resources_paginator: ListEnvironmentProvisionedResourcesPaginator = client.get_paginator("list_environment_provisioned_resources")
     list_environment_template_versions_paginator: ListEnvironmentTemplateVersionsPaginator = client.get_paginator("list_environment_template_versions")
     list_environment_templates_paginator: ListEnvironmentTemplatesPaginator = client.get_paginator("list_environment_templates")
     list_environments_paginator: ListEnvironmentsPaginator = client.get_paginator("list_environments")
     list_repositories_paginator: ListRepositoriesPaginator = client.get_paginator("list_repositories")
@@ -80,14 +82,15 @@
     ```
 """
 from .client import ProtonClient
 from .paginator import (
     ListComponentOutputsPaginator,
     ListComponentProvisionedResourcesPaginator,
     ListComponentsPaginator,
+    ListDeploymentsPaginator,
     ListEnvironmentAccountConnectionsPaginator,
     ListEnvironmentOutputsPaginator,
     ListEnvironmentProvisionedResourcesPaginator,
     ListEnvironmentsPaginator,
     ListEnvironmentTemplatesPaginator,
     ListEnvironmentTemplateVersionsPaginator,
     ListRepositoriesPaginator,
@@ -122,14 +125,15 @@
     "ComponentDeletedWaiter",
     "ComponentDeployedWaiter",
     "EnvironmentDeployedWaiter",
     "EnvironmentTemplateVersionRegisteredWaiter",
     "ListComponentOutputsPaginator",
     "ListComponentProvisionedResourcesPaginator",
     "ListComponentsPaginator",
+    "ListDeploymentsPaginator",
     "ListEnvironmentAccountConnectionsPaginator",
     "ListEnvironmentOutputsPaginator",
     "ListEnvironmentProvisionedResourcesPaginator",
     "ListEnvironmentTemplateVersionsPaginator",
     "ListEnvironmentTemplatesPaginator",
     "ListEnvironmentsPaginator",
     "ListRepositoriesPaginator",
```

### Comparing `types-aiobotocore-proton-2.5.2.post1/types_aiobotocore_proton/__main__.py` & `types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Proton 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.Proton 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton\nOther"
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

### Comparing `types-aiobotocore-proton-2.5.2.post1/types_aiobotocore_proton/client.py` & `types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     TemplateTypeType,
     TemplateVersionStatusType,
 )
 from .paginator import (
     ListComponentOutputsPaginator,
     ListComponentProvisionedResourcesPaginator,
     ListComponentsPaginator,
+    ListDeploymentsPaginator,
     ListEnvironmentAccountConnectionsPaginator,
     ListEnvironmentOutputsPaginator,
     ListEnvironmentProvisionedResourcesPaginator,
     ListEnvironmentsPaginator,
     ListEnvironmentTemplatesPaginator,
     ListEnvironmentTemplateVersionsPaginator,
     ListRepositoriesPaginator,
@@ -71,27 +72,29 @@
     CreateServiceInstanceOutputTypeDef,
     CreateServiceOutputTypeDef,
     CreateServiceSyncConfigOutputTypeDef,
     CreateServiceTemplateOutputTypeDef,
     CreateServiceTemplateVersionOutputTypeDef,
     CreateTemplateSyncConfigOutputTypeDef,
     DeleteComponentOutputTypeDef,
+    DeleteDeploymentOutputTypeDef,
     DeleteEnvironmentAccountConnectionOutputTypeDef,
     DeleteEnvironmentOutputTypeDef,
     DeleteEnvironmentTemplateOutputTypeDef,
     DeleteEnvironmentTemplateVersionOutputTypeDef,
     DeleteRepositoryOutputTypeDef,
     DeleteServiceOutputTypeDef,
     DeleteServiceSyncConfigOutputTypeDef,
     DeleteServiceTemplateOutputTypeDef,
     DeleteServiceTemplateVersionOutputTypeDef,
     DeleteTemplateSyncConfigOutputTypeDef,
     EnvironmentTemplateFilterTypeDef,
     GetAccountSettingsOutputTypeDef,
     GetComponentOutputTypeDef,
+    GetDeploymentOutputTypeDef,
     GetEnvironmentAccountConnectionOutputTypeDef,
     GetEnvironmentOutputTypeDef,
     GetEnvironmentTemplateOutputTypeDef,
     GetEnvironmentTemplateVersionOutputTypeDef,
     GetRepositoryOutputTypeDef,
     GetRepositorySyncStatusOutputTypeDef,
     GetResourcesSummaryOutputTypeDef,
@@ -103,14 +106,15 @@
     GetServiceTemplateOutputTypeDef,
     GetServiceTemplateVersionOutputTypeDef,
     GetTemplateSyncConfigOutputTypeDef,
     GetTemplateSyncStatusOutputTypeDef,
     ListComponentOutputsOutputTypeDef,
     ListComponentProvisionedResourcesOutputTypeDef,
     ListComponentsOutputTypeDef,
+    ListDeploymentsOutputTypeDef,
     ListEnvironmentAccountConnectionsOutputTypeDef,
     ListEnvironmentOutputsOutputTypeDef,
     ListEnvironmentProvisionedResourcesOutputTypeDef,
     ListEnvironmentsOutputTypeDef,
     ListEnvironmentTemplatesOutputTypeDef,
     ListEnvironmentTemplateVersionsOutputTypeDef,
     ListRepositoriesOutputTypeDef,
@@ -500,14 +504,22 @@
         """
         Delete an Proton component resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_component)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#delete_component)
         """
 
+    async def delete_deployment(self, *, id: str) -> DeleteDeploymentOutputTypeDef:
+        """
+        Delete the deployment.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_deployment)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#delete_deployment)
+        """
+
     async def delete_environment(self, *, name: str) -> DeleteEnvironmentOutputTypeDef:
         """
         Delete an environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#delete_environment)
         """
@@ -628,14 +640,30 @@
         """
         Get detailed data for a component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_component)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#get_component)
         """
 
+    async def get_deployment(
+        self,
+        *,
+        id: str,
+        componentName: str = ...,
+        environmentName: str = ...,
+        serviceInstanceName: str = ...,
+        serviceName: str = ...
+    ) -> GetDeploymentOutputTypeDef:
+        """
+        Get detailed data for a deployment.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_deployment)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#get_deployment)
+        """
+
     async def get_environment(self, *, name: str) -> GetEnvironmentOutputTypeDef:
         """
         Get detailed data for an environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#get_environment)
         """
@@ -785,15 +813,15 @@
         Get the status of a template sync.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_template_sync_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#get_template_sync_status)
         """
 
     async def list_component_outputs(
-        self, *, componentName: str, nextToken: str = ...
+        self, *, componentName: str, deploymentId: str = ..., nextToken: str = ...
     ) -> ListComponentOutputsOutputTypeDef:
         """
         Get a list of component Infrastructure as Code (IaC) outputs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_component_outputs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#list_component_outputs)
         """
@@ -820,14 +848,31 @@
         """
         List components with summary data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_components)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#list_components)
         """
 
+    async def list_deployments(
+        self,
+        *,
+        componentName: str = ...,
+        environmentName: str = ...,
+        maxResults: int = ...,
+        nextToken: str = ...,
+        serviceInstanceName: str = ...,
+        serviceName: str = ...
+    ) -> ListDeploymentsOutputTypeDef:
+        """
+        List deployments.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_deployments)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#list_deployments)
+        """
+
     async def list_environment_account_connections(
         self,
         *,
         requestedBy: EnvironmentAccountConnectionRequesterAccountTypeType,
         environmentName: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
@@ -837,15 +882,15 @@
         View a list of environment account connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_environment_account_connections)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#list_environment_account_connections)
         """
 
     async def list_environment_outputs(
-        self, *, environmentName: str, nextToken: str = ...
+        self, *, environmentName: str, deploymentId: str = ..., nextToken: str = ...
     ) -> ListEnvironmentOutputsOutputTypeDef:
         """
         List the infrastructure as code outputs for your environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_environment_outputs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#list_environment_outputs)
         """
@@ -921,15 +966,20 @@
         List repository sync definitions with detail data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_repository_sync_definitions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#list_repository_sync_definitions)
         """
 
     async def list_service_instance_outputs(
-        self, *, serviceInstanceName: str, serviceName: str, nextToken: str = ...
+        self,
+        *,
+        serviceInstanceName: str,
+        serviceName: str,
+        deploymentId: str = ...,
+        nextToken: str = ...
     ) -> ListServiceInstanceOutputsOutputTypeDef:
         """
         Get a list service of instance Infrastructure as Code (IaC) outputs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_instance_outputs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#list_service_instance_outputs)
         """
@@ -958,15 +1008,15 @@
         List service instances with summary data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_instances)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#list_service_instances)
         """
 
     async def list_service_pipeline_outputs(
-        self, *, serviceName: str, nextToken: str = ...
+        self, *, serviceName: str, deploymentId: str = ..., nextToken: str = ...
     ) -> ListServicePipelineOutputsOutputTypeDef:
         """
         Get a list of service pipeline Infrastructure as Code (IaC) outputs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_pipeline_outputs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#list_service_pipeline_outputs)
         """
@@ -1308,14 +1358,23 @@
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#get_paginator)
         """
 
     @overload
     def get_paginator(
+        self, operation_name: Literal["list_deployments"]
+    ) -> ListDeploymentsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_paginator)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(
         self, operation_name: Literal["list_environment_account_connections"]
     ) -> ListEnvironmentAccountConnectionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#get_paginator)
         """
```

### Comparing `types-aiobotocore-proton-2.5.2.post1/types_aiobotocore_proton/client.pyi` & `types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     TemplateTypeType,
     TemplateVersionStatusType,
 )
 from .paginator import (
     ListComponentOutputsPaginator,
     ListComponentProvisionedResourcesPaginator,
     ListComponentsPaginator,
+    ListDeploymentsPaginator,
     ListEnvironmentAccountConnectionsPaginator,
     ListEnvironmentOutputsPaginator,
     ListEnvironmentProvisionedResourcesPaginator,
     ListEnvironmentsPaginator,
     ListEnvironmentTemplatesPaginator,
     ListEnvironmentTemplateVersionsPaginator,
     ListRepositoriesPaginator,
@@ -71,27 +72,29 @@
     CreateServiceInstanceOutputTypeDef,
     CreateServiceOutputTypeDef,
     CreateServiceSyncConfigOutputTypeDef,
     CreateServiceTemplateOutputTypeDef,
     CreateServiceTemplateVersionOutputTypeDef,
     CreateTemplateSyncConfigOutputTypeDef,
     DeleteComponentOutputTypeDef,
+    DeleteDeploymentOutputTypeDef,
     DeleteEnvironmentAccountConnectionOutputTypeDef,
     DeleteEnvironmentOutputTypeDef,
     DeleteEnvironmentTemplateOutputTypeDef,
     DeleteEnvironmentTemplateVersionOutputTypeDef,
     DeleteRepositoryOutputTypeDef,
     DeleteServiceOutputTypeDef,
     DeleteServiceSyncConfigOutputTypeDef,
     DeleteServiceTemplateOutputTypeDef,
     DeleteServiceTemplateVersionOutputTypeDef,
     DeleteTemplateSyncConfigOutputTypeDef,
     EnvironmentTemplateFilterTypeDef,
     GetAccountSettingsOutputTypeDef,
     GetComponentOutputTypeDef,
+    GetDeploymentOutputTypeDef,
     GetEnvironmentAccountConnectionOutputTypeDef,
     GetEnvironmentOutputTypeDef,
     GetEnvironmentTemplateOutputTypeDef,
     GetEnvironmentTemplateVersionOutputTypeDef,
     GetRepositoryOutputTypeDef,
     GetRepositorySyncStatusOutputTypeDef,
     GetResourcesSummaryOutputTypeDef,
@@ -103,14 +106,15 @@
     GetServiceTemplateOutputTypeDef,
     GetServiceTemplateVersionOutputTypeDef,
     GetTemplateSyncConfigOutputTypeDef,
     GetTemplateSyncStatusOutputTypeDef,
     ListComponentOutputsOutputTypeDef,
     ListComponentProvisionedResourcesOutputTypeDef,
     ListComponentsOutputTypeDef,
+    ListDeploymentsOutputTypeDef,
     ListEnvironmentAccountConnectionsOutputTypeDef,
     ListEnvironmentOutputsOutputTypeDef,
     ListEnvironmentProvisionedResourcesOutputTypeDef,
     ListEnvironmentsOutputTypeDef,
     ListEnvironmentTemplatesOutputTypeDef,
     ListEnvironmentTemplateVersionsOutputTypeDef,
     ListRepositoriesOutputTypeDef,
@@ -475,14 +479,21 @@
     async def delete_component(self, *, name: str) -> DeleteComponentOutputTypeDef:
         """
         Delete an Proton component resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_component)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#delete_component)
         """
+    async def delete_deployment(self, *, id: str) -> DeleteDeploymentOutputTypeDef:
+        """
+        Delete the deployment.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_deployment)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#delete_deployment)
+        """
     async def delete_environment(self, *, name: str) -> DeleteEnvironmentOutputTypeDef:
         """
         Delete an environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.delete_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#delete_environment)
         """
@@ -590,14 +601,29 @@
     async def get_component(self, *, name: str) -> GetComponentOutputTypeDef:
         """
         Get detailed data for a component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_component)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#get_component)
         """
+    async def get_deployment(
+        self,
+        *,
+        id: str,
+        componentName: str = ...,
+        environmentName: str = ...,
+        serviceInstanceName: str = ...,
+        serviceName: str = ...
+    ) -> GetDeploymentOutputTypeDef:
+        """
+        Get detailed data for a deployment.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_deployment)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#get_deployment)
+        """
     async def get_environment(self, *, name: str) -> GetEnvironmentOutputTypeDef:
         """
         Get detailed data for an environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#get_environment)
         """
@@ -731,15 +757,15 @@
         """
         Get the status of a template sync.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_template_sync_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#get_template_sync_status)
         """
     async def list_component_outputs(
-        self, *, componentName: str, nextToken: str = ...
+        self, *, componentName: str, deploymentId: str = ..., nextToken: str = ...
     ) -> ListComponentOutputsOutputTypeDef:
         """
         Get a list of component Infrastructure as Code (IaC) outputs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_component_outputs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#list_component_outputs)
         """
@@ -763,14 +789,30 @@
     ) -> ListComponentsOutputTypeDef:
         """
         List components with summary data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_components)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#list_components)
         """
+    async def list_deployments(
+        self,
+        *,
+        componentName: str = ...,
+        environmentName: str = ...,
+        maxResults: int = ...,
+        nextToken: str = ...,
+        serviceInstanceName: str = ...,
+        serviceName: str = ...
+    ) -> ListDeploymentsOutputTypeDef:
+        """
+        List deployments.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_deployments)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#list_deployments)
+        """
     async def list_environment_account_connections(
         self,
         *,
         requestedBy: EnvironmentAccountConnectionRequesterAccountTypeType,
         environmentName: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
@@ -779,15 +821,15 @@
         """
         View a list of environment account connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_environment_account_connections)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#list_environment_account_connections)
         """
     async def list_environment_outputs(
-        self, *, environmentName: str, nextToken: str = ...
+        self, *, environmentName: str, deploymentId: str = ..., nextToken: str = ...
     ) -> ListEnvironmentOutputsOutputTypeDef:
         """
         List the infrastructure as code outputs for your environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_environment_outputs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#list_environment_outputs)
         """
@@ -856,15 +898,20 @@
         """
         List repository sync definitions with detail data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_repository_sync_definitions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#list_repository_sync_definitions)
         """
     async def list_service_instance_outputs(
-        self, *, serviceInstanceName: str, serviceName: str, nextToken: str = ...
+        self,
+        *,
+        serviceInstanceName: str,
+        serviceName: str,
+        deploymentId: str = ...,
+        nextToken: str = ...
     ) -> ListServiceInstanceOutputsOutputTypeDef:
         """
         Get a list service of instance Infrastructure as Code (IaC) outputs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_instance_outputs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#list_service_instance_outputs)
         """
@@ -890,15 +937,15 @@
         """
         List service instances with summary data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_instances)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#list_service_instances)
         """
     async def list_service_pipeline_outputs(
-        self, *, serviceName: str, nextToken: str = ...
+        self, *, serviceName: str, deploymentId: str = ..., nextToken: str = ...
     ) -> ListServicePipelineOutputsOutputTypeDef:
         """
         Get a list of service pipeline Infrastructure as Code (IaC) outputs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.list_service_pipeline_outputs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#list_service_pipeline_outputs)
         """
@@ -1213,14 +1260,22 @@
     def get_paginator(self, operation_name: Literal["list_components"]) -> ListComponentsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#get_paginator)
         """
     @overload
     def get_paginator(
+        self, operation_name: Literal["list_deployments"]
+    ) -> ListDeploymentsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_paginator)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#get_paginator)
+        """
+    @overload
+    def get_paginator(
         self, operation_name: Literal["list_environment_account_connections"]
     ) -> ListEnvironmentAccountConnectionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/client/#get_paginator)
         """
     @overload
```

### Comparing `types-aiobotocore-proton-2.5.2.post1/types_aiobotocore_proton/literals.py` & `types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -14,30 +14,31 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "BlockerStatusType",
     "BlockerTypeType",
     "ComponentDeletedWaiterName",
     "ComponentDeployedWaiterName",
     "ComponentDeploymentUpdateTypeType",
     "DeploymentStatusType",
+    "DeploymentTargetResourceTypeType",
     "DeploymentUpdateTypeType",
     "EnvironmentAccountConnectionRequesterAccountTypeType",
     "EnvironmentAccountConnectionStatusType",
     "EnvironmentDeployedWaiterName",
     "EnvironmentTemplateVersionRegisteredWaiterName",
     "ListComponentOutputsPaginatorName",
     "ListComponentProvisionedResourcesPaginatorName",
     "ListComponentsPaginatorName",
+    "ListDeploymentsPaginatorName",
     "ListEnvironmentAccountConnectionsPaginatorName",
     "ListEnvironmentOutputsPaginatorName",
     "ListEnvironmentProvisionedResourcesPaginatorName",
     "ListEnvironmentTemplateVersionsPaginatorName",
     "ListEnvironmentTemplatesPaginatorName",
     "ListEnvironmentsPaginatorName",
     "ListRepositoriesPaginatorName",
@@ -75,15 +76,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 BlockerStatusType = Literal["ACTIVE", "RESOLVED"]
 BlockerTypeType = Literal["AUTOMATED"]
 ComponentDeletedWaiterName = Literal["component_deleted"]
 ComponentDeployedWaiterName = Literal["component_deployed"]
 ComponentDeploymentUpdateTypeType = Literal["CURRENT_VERSION", "NONE"]
 DeploymentStatusType = Literal[
     "CANCELLED",
@@ -91,24 +91,28 @@
     "DELETE_COMPLETE",
     "DELETE_FAILED",
     "DELETE_IN_PROGRESS",
     "FAILED",
     "IN_PROGRESS",
     "SUCCEEDED",
 ]
+DeploymentTargetResourceTypeType = Literal[
+    "COMPONENT", "ENVIRONMENT", "SERVICE_INSTANCE", "SERVICE_PIPELINE"
+]
 DeploymentUpdateTypeType = Literal["CURRENT_VERSION", "MAJOR_VERSION", "MINOR_VERSION", "NONE"]
 EnvironmentAccountConnectionRequesterAccountTypeType = Literal[
     "ENVIRONMENT_ACCOUNT", "MANAGEMENT_ACCOUNT"
 ]
 EnvironmentAccountConnectionStatusType = Literal["CONNECTED", "PENDING", "REJECTED"]
 EnvironmentDeployedWaiterName = Literal["environment_deployed"]
 EnvironmentTemplateVersionRegisteredWaiterName = Literal["environment_template_version_registered"]
 ListComponentOutputsPaginatorName = Literal["list_component_outputs"]
 ListComponentProvisionedResourcesPaginatorName = Literal["list_component_provisioned_resources"]
 ListComponentsPaginatorName = Literal["list_components"]
+ListDeploymentsPaginatorName = Literal["list_deployments"]
 ListEnvironmentAccountConnectionsPaginatorName = Literal["list_environment_account_connections"]
 ListEnvironmentOutputsPaginatorName = Literal["list_environment_outputs"]
 ListEnvironmentProvisionedResourcesPaginatorName = Literal["list_environment_provisioned_resources"]
 ListEnvironmentTemplateVersionsPaginatorName = Literal["list_environment_template_versions"]
 ListEnvironmentTemplatesPaginatorName = Literal["list_environment_templates"]
 ListEnvironmentsPaginatorName = Literal["list_environments"]
 ListRepositoriesPaginatorName = Literal["list_repositories"]
@@ -194,14 +198,15 @@
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
@@ -297,14 +302,15 @@
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
@@ -383,26 +389,28 @@
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
@@ -546,14 +554,15 @@
     "sns",
     "sqs",
 ]
 PaginatorName = Literal[
     "list_component_outputs",
     "list_component_provisioned_resources",
     "list_components",
+    "list_deployments",
     "list_environment_account_connections",
     "list_environment_outputs",
     "list_environment_provisioned_resources",
     "list_environment_template_versions",
     "list_environment_templates",
     "list_environments",
     "list_repositories",
```

### Comparing `types-aiobotocore-proton-2.5.2.post1/types_aiobotocore_proton/literals.pyi` & `types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,29 +14,32 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "BlockerStatusType",
     "BlockerTypeType",
     "ComponentDeletedWaiterName",
     "ComponentDeployedWaiterName",
     "ComponentDeploymentUpdateTypeType",
     "DeploymentStatusType",
+    "DeploymentTargetResourceTypeType",
     "DeploymentUpdateTypeType",
     "EnvironmentAccountConnectionRequesterAccountTypeType",
     "EnvironmentAccountConnectionStatusType",
     "EnvironmentDeployedWaiterName",
     "EnvironmentTemplateVersionRegisteredWaiterName",
     "ListComponentOutputsPaginatorName",
     "ListComponentProvisionedResourcesPaginatorName",
     "ListComponentsPaginatorName",
+    "ListDeploymentsPaginatorName",
     "ListEnvironmentAccountConnectionsPaginatorName",
     "ListEnvironmentOutputsPaginatorName",
     "ListEnvironmentProvisionedResourcesPaginatorName",
     "ListEnvironmentTemplateVersionsPaginatorName",
     "ListEnvironmentTemplatesPaginatorName",
     "ListEnvironmentsPaginatorName",
     "ListRepositoriesPaginatorName",
@@ -74,14 +77,15 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
+
 BlockerStatusType = Literal["ACTIVE", "RESOLVED"]
 BlockerTypeType = Literal["AUTOMATED"]
 ComponentDeletedWaiterName = Literal["component_deleted"]
 ComponentDeployedWaiterName = Literal["component_deployed"]
 ComponentDeploymentUpdateTypeType = Literal["CURRENT_VERSION", "NONE"]
 DeploymentStatusType = Literal[
     "CANCELLED",
@@ -89,24 +93,28 @@
     "DELETE_COMPLETE",
     "DELETE_FAILED",
     "DELETE_IN_PROGRESS",
     "FAILED",
     "IN_PROGRESS",
     "SUCCEEDED",
 ]
+DeploymentTargetResourceTypeType = Literal[
+    "COMPONENT", "ENVIRONMENT", "SERVICE_INSTANCE", "SERVICE_PIPELINE"
+]
 DeploymentUpdateTypeType = Literal["CURRENT_VERSION", "MAJOR_VERSION", "MINOR_VERSION", "NONE"]
 EnvironmentAccountConnectionRequesterAccountTypeType = Literal[
     "ENVIRONMENT_ACCOUNT", "MANAGEMENT_ACCOUNT"
 ]
 EnvironmentAccountConnectionStatusType = Literal["CONNECTED", "PENDING", "REJECTED"]
 EnvironmentDeployedWaiterName = Literal["environment_deployed"]
 EnvironmentTemplateVersionRegisteredWaiterName = Literal["environment_template_version_registered"]
 ListComponentOutputsPaginatorName = Literal["list_component_outputs"]
 ListComponentProvisionedResourcesPaginatorName = Literal["list_component_provisioned_resources"]
 ListComponentsPaginatorName = Literal["list_components"]
+ListDeploymentsPaginatorName = Literal["list_deployments"]
 ListEnvironmentAccountConnectionsPaginatorName = Literal["list_environment_account_connections"]
 ListEnvironmentOutputsPaginatorName = Literal["list_environment_outputs"]
 ListEnvironmentProvisionedResourcesPaginatorName = Literal["list_environment_provisioned_resources"]
 ListEnvironmentTemplateVersionsPaginatorName = Literal["list_environment_template_versions"]
 ListEnvironmentTemplatesPaginatorName = Literal["list_environment_templates"]
 ListEnvironmentsPaginatorName = Literal["list_environments"]
 ListRepositoriesPaginatorName = Literal["list_repositories"]
@@ -192,14 +200,15 @@
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
@@ -295,14 +304,15 @@
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
@@ -381,26 +391,28 @@
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
@@ -544,14 +556,15 @@
     "sns",
     "sqs",
 ]
 PaginatorName = Literal[
     "list_component_outputs",
     "list_component_provisioned_resources",
     "list_components",
+    "list_deployments",
     "list_environment_account_connections",
     "list_environment_outputs",
     "list_environment_provisioned_resources",
     "list_environment_template_versions",
     "list_environment_templates",
     "list_environments",
     "list_repositories",
```

### Comparing `types-aiobotocore-proton-2.5.2.post1/types_aiobotocore_proton/paginator.py` & `types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     from aiobotocore.session import get_session
 
     from types_aiobotocore_proton.client import ProtonClient
     from types_aiobotocore_proton.paginator import (
         ListComponentOutputsPaginator,
         ListComponentProvisionedResourcesPaginator,
         ListComponentsPaginator,
+        ListDeploymentsPaginator,
         ListEnvironmentAccountConnectionsPaginator,
         ListEnvironmentOutputsPaginator,
         ListEnvironmentProvisionedResourcesPaginator,
         ListEnvironmentTemplateVersionsPaginator,
         ListEnvironmentTemplatesPaginator,
         ListEnvironmentsPaginator,
         ListRepositoriesPaginator,
@@ -35,14 +36,15 @@
     session = get_session()
     with session.create_client("proton") as client:
         client: ProtonClient
 
         list_component_outputs_paginator: ListComponentOutputsPaginator = client.get_paginator("list_component_outputs")
         list_component_provisioned_resources_paginator: ListComponentProvisionedResourcesPaginator = client.get_paginator("list_component_provisioned_resources")
         list_components_paginator: ListComponentsPaginator = client.get_paginator("list_components")
+        list_deployments_paginator: ListDeploymentsPaginator = client.get_paginator("list_deployments")
         list_environment_account_connections_paginator: ListEnvironmentAccountConnectionsPaginator = client.get_paginator("list_environment_account_connections")
         list_environment_outputs_paginator: ListEnvironmentOutputsPaginator = client.get_paginator("list_environment_outputs")
         list_environment_provisioned_resources_paginator: ListEnvironmentProvisionedResourcesPaginator = client.get_paginator("list_environment_provisioned_resources")
         list_environment_template_versions_paginator: ListEnvironmentTemplateVersionsPaginator = client.get_paginator("list_environment_template_versions")
         list_environment_templates_paginator: ListEnvironmentTemplatesPaginator = client.get_paginator("list_environment_templates")
         list_environments_paginator: ListEnvironmentsPaginator = client.get_paginator("list_environments")
         list_repositories_paginator: ListRepositoriesPaginator = client.get_paginator("list_repositories")
@@ -72,14 +74,15 @@
     SyncTypeType,
 )
 from .type_defs import (
     EnvironmentTemplateFilterTypeDef,
     ListComponentOutputsOutputTypeDef,
     ListComponentProvisionedResourcesOutputTypeDef,
     ListComponentsOutputTypeDef,
+    ListDeploymentsOutputTypeDef,
     ListEnvironmentAccountConnectionsOutputTypeDef,
     ListEnvironmentOutputsOutputTypeDef,
     ListEnvironmentProvisionedResourcesOutputTypeDef,
     ListEnvironmentsOutputTypeDef,
     ListEnvironmentTemplatesOutputTypeDef,
     ListEnvironmentTemplateVersionsOutputTypeDef,
     ListRepositoriesOutputTypeDef,
@@ -97,14 +100,15 @@
     PaginatorConfigTypeDef,
 )
 
 __all__ = (
     "ListComponentOutputsPaginator",
     "ListComponentProvisionedResourcesPaginator",
     "ListComponentsPaginator",
+    "ListDeploymentsPaginator",
     "ListEnvironmentAccountConnectionsPaginator",
     "ListEnvironmentOutputsPaginator",
     "ListEnvironmentProvisionedResourcesPaginator",
     "ListEnvironmentTemplateVersionsPaginator",
     "ListEnvironmentTemplatesPaginator",
     "ListEnvironmentsPaginator",
     "ListRepositoriesPaginator",
@@ -134,15 +138,19 @@
 class ListComponentOutputsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListComponentOutputs)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/paginators/#listcomponentoutputspaginator)
     """
 
     def paginate(
-        self, *, componentName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self,
+        *,
+        componentName: str,
+        deploymentId: str = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListComponentOutputsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListComponentOutputs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/paginators/#listcomponentoutputspaginator)
         """
 
 
@@ -177,14 +185,35 @@
     ) -> AsyncIterator[ListComponentsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListComponents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/paginators/#listcomponentspaginator)
         """
 
 
+class ListDeploymentsPaginator(AioPaginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListDeployments)
+    [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/paginators/#listdeploymentspaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        componentName: str = ...,
+        environmentName: str = ...,
+        serviceInstanceName: str = ...,
+        serviceName: str = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...
+    ) -> AsyncIterator[ListDeploymentsOutputTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListDeployments.paginate)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/paginators/#listdeploymentspaginator)
+        """
+
+
 class ListEnvironmentAccountConnectionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentAccountConnections)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/paginators/#listenvironmentaccountconnectionspaginator)
     """
 
     def paginate(
@@ -204,15 +233,19 @@
 class ListEnvironmentOutputsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentOutputs)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/paginators/#listenvironmentoutputspaginator)
     """
 
     def paginate(
-        self, *, environmentName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self,
+        *,
+        environmentName: str,
+        deploymentId: str = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListEnvironmentOutputsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentOutputs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/paginators/#listenvironmentoutputspaginator)
         """
 
 
@@ -325,14 +358,15 @@
     """
 
     def paginate(
         self,
         *,
         serviceInstanceName: str,
         serviceName: str,
+        deploymentId: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListServiceInstanceOutputsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServiceInstanceOutputs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/paginators/#listserviceinstanceoutputspaginator)
         """
 
@@ -380,15 +414,19 @@
 class ListServicePipelineOutputsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServicePipelineOutputs)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/paginators/#listservicepipelineoutputspaginator)
     """
 
     def paginate(
-        self, *, serviceName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self,
+        *,
+        serviceName: str,
+        deploymentId: str = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListServicePipelineOutputsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServicePipelineOutputs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/paginators/#listservicepipelineoutputspaginator)
         """
```

### Comparing `types-aiobotocore-proton-2.5.2.post1/types_aiobotocore_proton/paginator.pyi` & `types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     from aiobotocore.session import get_session
 
     from types_aiobotocore_proton.client import ProtonClient
     from types_aiobotocore_proton.paginator import (
         ListComponentOutputsPaginator,
         ListComponentProvisionedResourcesPaginator,
         ListComponentsPaginator,
+        ListDeploymentsPaginator,
         ListEnvironmentAccountConnectionsPaginator,
         ListEnvironmentOutputsPaginator,
         ListEnvironmentProvisionedResourcesPaginator,
         ListEnvironmentTemplateVersionsPaginator,
         ListEnvironmentTemplatesPaginator,
         ListEnvironmentsPaginator,
         ListRepositoriesPaginator,
@@ -35,14 +36,15 @@
     session = get_session()
     with session.create_client("proton") as client:
         client: ProtonClient
 
         list_component_outputs_paginator: ListComponentOutputsPaginator = client.get_paginator("list_component_outputs")
         list_component_provisioned_resources_paginator: ListComponentProvisionedResourcesPaginator = client.get_paginator("list_component_provisioned_resources")
         list_components_paginator: ListComponentsPaginator = client.get_paginator("list_components")
+        list_deployments_paginator: ListDeploymentsPaginator = client.get_paginator("list_deployments")
         list_environment_account_connections_paginator: ListEnvironmentAccountConnectionsPaginator = client.get_paginator("list_environment_account_connections")
         list_environment_outputs_paginator: ListEnvironmentOutputsPaginator = client.get_paginator("list_environment_outputs")
         list_environment_provisioned_resources_paginator: ListEnvironmentProvisionedResourcesPaginator = client.get_paginator("list_environment_provisioned_resources")
         list_environment_template_versions_paginator: ListEnvironmentTemplateVersionsPaginator = client.get_paginator("list_environment_template_versions")
         list_environment_templates_paginator: ListEnvironmentTemplatesPaginator = client.get_paginator("list_environment_templates")
         list_environments_paginator: ListEnvironmentsPaginator = client.get_paginator("list_environments")
         list_repositories_paginator: ListRepositoriesPaginator = client.get_paginator("list_repositories")
@@ -72,14 +74,15 @@
     SyncTypeType,
 )
 from .type_defs import (
     EnvironmentTemplateFilterTypeDef,
     ListComponentOutputsOutputTypeDef,
     ListComponentProvisionedResourcesOutputTypeDef,
     ListComponentsOutputTypeDef,
+    ListDeploymentsOutputTypeDef,
     ListEnvironmentAccountConnectionsOutputTypeDef,
     ListEnvironmentOutputsOutputTypeDef,
     ListEnvironmentProvisionedResourcesOutputTypeDef,
     ListEnvironmentsOutputTypeDef,
     ListEnvironmentTemplatesOutputTypeDef,
     ListEnvironmentTemplateVersionsOutputTypeDef,
     ListRepositoriesOutputTypeDef,
@@ -97,14 +100,15 @@
     PaginatorConfigTypeDef,
 )
 
 __all__ = (
     "ListComponentOutputsPaginator",
     "ListComponentProvisionedResourcesPaginator",
     "ListComponentsPaginator",
+    "ListDeploymentsPaginator",
     "ListEnvironmentAccountConnectionsPaginator",
     "ListEnvironmentOutputsPaginator",
     "ListEnvironmentProvisionedResourcesPaginator",
     "ListEnvironmentTemplateVersionsPaginator",
     "ListEnvironmentTemplatesPaginator",
     "ListEnvironmentsPaginator",
     "ListRepositoriesPaginator",
@@ -131,15 +135,19 @@
 class ListComponentOutputsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListComponentOutputs)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/paginators/#listcomponentoutputspaginator)
     """
 
     def paginate(
-        self, *, componentName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self,
+        *,
+        componentName: str,
+        deploymentId: str = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListComponentOutputsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListComponentOutputs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/paginators/#listcomponentoutputspaginator)
         """
 
 class ListComponentProvisionedResourcesPaginator(AioPaginator):
@@ -171,14 +179,34 @@
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListComponentsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListComponents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/paginators/#listcomponentspaginator)
         """
 
+class ListDeploymentsPaginator(AioPaginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListDeployments)
+    [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/paginators/#listdeploymentspaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        componentName: str = ...,
+        environmentName: str = ...,
+        serviceInstanceName: str = ...,
+        serviceName: str = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...
+    ) -> AsyncIterator[ListDeploymentsOutputTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListDeployments.paginate)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/paginators/#listdeploymentspaginator)
+        """
+
 class ListEnvironmentAccountConnectionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentAccountConnections)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/paginators/#listenvironmentaccountconnectionspaginator)
     """
 
     def paginate(
@@ -197,15 +225,19 @@
 class ListEnvironmentOutputsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentOutputs)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/paginators/#listenvironmentoutputspaginator)
     """
 
     def paginate(
-        self, *, environmentName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self,
+        *,
+        environmentName: str,
+        deploymentId: str = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListEnvironmentOutputsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListEnvironmentOutputs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/paginators/#listenvironmentoutputspaginator)
         """
 
 class ListEnvironmentProvisionedResourcesPaginator(AioPaginator):
@@ -311,14 +343,15 @@
     """
 
     def paginate(
         self,
         *,
         serviceInstanceName: str,
         serviceName: str,
+        deploymentId: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListServiceInstanceOutputsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServiceInstanceOutputs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/paginators/#listserviceinstanceoutputspaginator)
         """
 
@@ -363,15 +396,19 @@
 class ListServicePipelineOutputsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServicePipelineOutputs)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/paginators/#listservicepipelineoutputspaginator)
     """
 
     def paginate(
-        self, *, serviceName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self,
+        *,
+        serviceName: str,
+        deploymentId: str = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListServicePipelineOutputsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton.Paginator.ListServicePipelineOutputs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_proton/paginators/#listservicepipelineoutputspaginator)
         """
 
 class ListServicePipelineProvisionedResourcesPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-proton-2.5.2.post1/types_aiobotocore_proton/type_defs.py` & `types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from datetime import datetime
 from typing import Dict, List, Sequence
 
 from .literals import (
     BlockerStatusType,
     ComponentDeploymentUpdateTypeType,
     DeploymentStatusType,
+    DeploymentTargetResourceTypeType,
     DeploymentUpdateTypeType,
     EnvironmentAccountConnectionRequesterAccountTypeType,
     EnvironmentAccountConnectionStatusType,
     ListServiceInstancesFilterByType,
     ListServiceInstancesSortByType,
     ProvisionedResourceEngineType,
     RepositoryProviderType,
@@ -56,44 +57,51 @@
     "CancelEnvironmentDeploymentInputRequestTypeDef",
     "CancelServiceInstanceDeploymentInputRequestTypeDef",
     "ServiceInstanceTypeDef",
     "CancelServicePipelineDeploymentInputRequestTypeDef",
     "ServicePipelineTypeDef",
     "CompatibleEnvironmentTemplateInputTypeDef",
     "CompatibleEnvironmentTemplateTypeDef",
+    "ComponentStateTypeDef",
     "ComponentSummaryTypeDef",
     "ResourceCountsSummaryTypeDef",
     "TagTypeDef",
     "RepositoryBranchInputTypeDef",
     "EnvironmentTemplateTypeDef",
     "EnvironmentTemplateVersionTypeDef",
     "RepositoryTypeDef",
     "CreateServiceSyncConfigInputRequestTypeDef",
     "ServiceSyncConfigTypeDef",
     "ServiceTemplateTypeDef",
     "CreateTemplateSyncConfigInputRequestTypeDef",
     "TemplateSyncConfigTypeDef",
     "DeleteComponentInputRequestTypeDef",
+    "DeleteDeploymentInputRequestTypeDef",
     "DeleteEnvironmentAccountConnectionInputRequestTypeDef",
     "DeleteEnvironmentInputRequestTypeDef",
     "DeleteEnvironmentTemplateInputRequestTypeDef",
     "DeleteEnvironmentTemplateVersionInputRequestTypeDef",
     "DeleteRepositoryInputRequestTypeDef",
     "DeleteServiceInputRequestTypeDef",
     "DeleteServiceSyncConfigInputRequestTypeDef",
     "DeleteServiceTemplateInputRequestTypeDef",
     "DeleteServiceTemplateVersionInputRequestTypeDef",
     "DeleteTemplateSyncConfigInputRequestTypeDef",
+    "EnvironmentStateTypeDef",
+    "ServiceInstanceStateTypeDef",
+    "ServicePipelineStateTypeDef",
+    "DeploymentSummaryTypeDef",
     "EnvironmentAccountConnectionSummaryTypeDef",
     "EnvironmentSummaryTypeDef",
     "EnvironmentTemplateFilterTypeDef",
     "EnvironmentTemplateSummaryTypeDef",
     "EnvironmentTemplateVersionSummaryTypeDef",
     "WaiterConfigTypeDef",
     "GetComponentInputRequestTypeDef",
+    "GetDeploymentInputRequestTypeDef",
     "GetEnvironmentAccountConnectionInputRequestTypeDef",
     "GetEnvironmentInputRequestTypeDef",
     "GetEnvironmentTemplateInputRequestTypeDef",
     "GetEnvironmentTemplateVersionInputRequestTypeDef",
     "GetRepositoryInputRequestTypeDef",
     "GetRepositorySyncStatusInputRequestTypeDef",
     "GetServiceInputRequestTypeDef",
@@ -108,14 +116,15 @@
     "GetTemplateSyncStatusInputRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ListComponentOutputsInputRequestTypeDef",
     "OutputTypeDef",
     "ListComponentProvisionedResourcesInputRequestTypeDef",
     "ProvisionedResourceTypeDef",
     "ListComponentsInputRequestTypeDef",
+    "ListDeploymentsInputRequestTypeDef",
     "ListEnvironmentAccountConnectionsInputRequestTypeDef",
     "ListEnvironmentOutputsInputRequestTypeDef",
     "ListEnvironmentProvisionedResourcesInputRequestTypeDef",
     "ListEnvironmentTemplateVersionsInputRequestTypeDef",
     "ListEnvironmentTemplatesInputRequestTypeDef",
     "ListRepositoriesInputRequestTypeDef",
     "RepositorySummaryTypeDef",
@@ -206,14 +215,16 @@
     "DeleteServiceTemplateOutputTypeDef",
     "GetServiceTemplateOutputTypeDef",
     "UpdateServiceTemplateOutputTypeDef",
     "CreateTemplateSyncConfigOutputTypeDef",
     "DeleteTemplateSyncConfigOutputTypeDef",
     "GetTemplateSyncConfigOutputTypeDef",
     "UpdateTemplateSyncConfigOutputTypeDef",
+    "DeploymentStateTypeDef",
+    "ListDeploymentsOutputTypeDef",
     "ListEnvironmentAccountConnectionsOutputTypeDef",
     "ListEnvironmentsOutputTypeDef",
     "ListEnvironmentsInputRequestTypeDef",
     "ListEnvironmentTemplatesOutputTypeDef",
     "ListEnvironmentTemplateVersionsOutputTypeDef",
     "GetComponentInputComponentDeletedWaitTypeDef",
     "GetComponentInputComponentDeployedWaitTypeDef",
@@ -224,14 +235,15 @@
     "GetServiceInputServicePipelineDeployedWaitTypeDef",
     "GetServiceInputServiceUpdatedWaitTypeDef",
     "GetServiceInstanceInputServiceInstanceDeployedWaitTypeDef",
     "GetServiceTemplateVersionInputServiceTemplateVersionRegisteredWaitTypeDef",
     "ListComponentOutputsInputListComponentOutputsPaginateTypeDef",
     "ListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef",
     "ListComponentsInputListComponentsPaginateTypeDef",
+    "ListDeploymentsInputListDeploymentsPaginateTypeDef",
     "ListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef",
     "ListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef",
     "ListEnvironmentProvisionedResourcesInputListEnvironmentProvisionedResourcesPaginateTypeDef",
     "ListEnvironmentTemplateVersionsInputListEnvironmentTemplateVersionsPaginateTypeDef",
     "ListEnvironmentTemplatesInputListEnvironmentTemplatesPaginateTypeDef",
     "ListEnvironmentsInputListEnvironmentsPaginateTypeDef",
     "ListRepositoriesInputListRepositoriesPaginateTypeDef",
@@ -277,21 +289,24 @@
     "GetServiceOutputTypeDef",
     "UpdateServiceOutputTypeDef",
     "CreateServiceTemplateVersionOutputTypeDef",
     "DeleteServiceTemplateVersionOutputTypeDef",
     "GetServiceTemplateVersionOutputTypeDef",
     "UpdateServiceTemplateVersionOutputTypeDef",
     "GetResourcesSummaryOutputTypeDef",
+    "DeploymentTypeDef",
     "GetRepositorySyncStatusOutputTypeDef",
     "GetServiceInstanceSyncStatusOutputTypeDef",
     "GetTemplateSyncStatusOutputTypeDef",
     "CreateEnvironmentTemplateVersionInputRequestTypeDef",
     "CreateServiceTemplateVersionInputRequestTypeDef",
     "ServiceSyncBlockerSummaryTypeDef",
     "UpdateServiceSyncBlockerOutputTypeDef",
+    "DeleteDeploymentOutputTypeDef",
+    "GetDeploymentOutputTypeDef",
     "GetServiceSyncBlockerSummaryOutputTypeDef",
 )
 
 AcceptEnvironmentAccountConnectionInputRequestTypeDef = TypedDict(
     "AcceptEnvironmentAccountConnectionInputRequestTypeDef",
     {
         "id": str,
@@ -368,17 +383,19 @@
     },
 )
 _OptionalComponentTypeDef = TypedDict(
     "_OptionalComponentTypeDef",
     {
         "deploymentStatusMessage": str,
         "description": str,
+        "lastAttemptedDeploymentId": str,
         "lastClientRequestToken": str,
         "lastDeploymentAttemptedAt": datetime,
         "lastDeploymentSucceededAt": datetime,
+        "lastSucceededDeploymentId": str,
         "serviceInstanceName": str,
         "serviceName": str,
         "serviceSpec": str,
     },
     total=False,
 )
 
@@ -418,15 +435,17 @@
         "templateName": str,
     },
 )
 _OptionalServiceInstanceTypeDef = TypedDict(
     "_OptionalServiceInstanceTypeDef",
     {
         "deploymentStatusMessage": str,
+        "lastAttemptedDeploymentId": str,
         "lastClientRequestToken": str,
+        "lastSucceededDeploymentId": str,
         "spec": str,
     },
     total=False,
 )
 
 
 class ServiceInstanceTypeDef(_RequiredServiceInstanceTypeDef, _OptionalServiceInstanceTypeDef):
@@ -453,14 +472,16 @@
         "templateName": str,
     },
 )
 _OptionalServicePipelineTypeDef = TypedDict(
     "_OptionalServicePipelineTypeDef",
     {
         "deploymentStatusMessage": str,
+        "lastAttemptedDeploymentId": str,
+        "lastSucceededDeploymentId": str,
         "spec": str,
     },
     total=False,
 )
 
 
 class ServicePipelineTypeDef(_RequiredServicePipelineTypeDef, _OptionalServicePipelineTypeDef):
@@ -479,14 +500,25 @@
     "CompatibleEnvironmentTemplateTypeDef",
     {
         "majorVersion": str,
         "templateName": str,
     },
 )
 
+ComponentStateTypeDef = TypedDict(
+    "ComponentStateTypeDef",
+    {
+        "serviceInstanceName": str,
+        "serviceName": str,
+        "serviceSpec": str,
+        "templateFile": str,
+    },
+    total=False,
+)
+
 _RequiredComponentSummaryTypeDef = TypedDict(
     "_RequiredComponentSummaryTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "deploymentStatus": DeploymentStatusType,
         "environmentName": str,
@@ -494,16 +526,18 @@
         "name": str,
     },
 )
 _OptionalComponentSummaryTypeDef = TypedDict(
     "_OptionalComponentSummaryTypeDef",
     {
         "deploymentStatusMessage": str,
+        "lastAttemptedDeploymentId": str,
         "lastDeploymentAttemptedAt": datetime,
         "lastDeploymentSucceededAt": datetime,
+        "lastSucceededDeploymentId": str,
         "serviceInstanceName": str,
         "serviceName": str,
     },
     total=False,
 )
 
 
@@ -734,14 +768,21 @@
 DeleteComponentInputRequestTypeDef = TypedDict(
     "DeleteComponentInputRequestTypeDef",
     {
         "name": str,
     },
 )
 
+DeleteDeploymentInputRequestTypeDef = TypedDict(
+    "DeleteDeploymentInputRequestTypeDef",
+    {
+        "id": str,
+    },
+)
+
 DeleteEnvironmentAccountConnectionInputRequestTypeDef = TypedDict(
     "DeleteEnvironmentAccountConnectionInputRequestTypeDef",
     {
         "id": str,
     },
 )
 
@@ -810,14 +851,118 @@
     "DeleteTemplateSyncConfigInputRequestTypeDef",
     {
         "templateName": str,
         "templateType": TemplateTypeType,
     },
 )
 
+_RequiredEnvironmentStateTypeDef = TypedDict(
+    "_RequiredEnvironmentStateTypeDef",
+    {
+        "templateMajorVersion": str,
+        "templateMinorVersion": str,
+        "templateName": str,
+    },
+)
+_OptionalEnvironmentStateTypeDef = TypedDict(
+    "_OptionalEnvironmentStateTypeDef",
+    {
+        "spec": str,
+    },
+    total=False,
+)
+
+
+class EnvironmentStateTypeDef(_RequiredEnvironmentStateTypeDef, _OptionalEnvironmentStateTypeDef):
+    pass
+
+
+_RequiredServiceInstanceStateTypeDef = TypedDict(
+    "_RequiredServiceInstanceStateTypeDef",
+    {
+        "spec": str,
+        "templateMajorVersion": str,
+        "templateMinorVersion": str,
+        "templateName": str,
+    },
+)
+_OptionalServiceInstanceStateTypeDef = TypedDict(
+    "_OptionalServiceInstanceStateTypeDef",
+    {
+        "lastSuccessfulComponentDeploymentIds": List[str],
+        "lastSuccessfulEnvironmentDeploymentId": str,
+        "lastSuccessfulServicePipelineDeploymentId": str,
+    },
+    total=False,
+)
+
+
+class ServiceInstanceStateTypeDef(
+    _RequiredServiceInstanceStateTypeDef, _OptionalServiceInstanceStateTypeDef
+):
+    pass
+
+
+_RequiredServicePipelineStateTypeDef = TypedDict(
+    "_RequiredServicePipelineStateTypeDef",
+    {
+        "templateMajorVersion": str,
+        "templateMinorVersion": str,
+        "templateName": str,
+    },
+)
+_OptionalServicePipelineStateTypeDef = TypedDict(
+    "_OptionalServicePipelineStateTypeDef",
+    {
+        "spec": str,
+    },
+    total=False,
+)
+
+
+class ServicePipelineStateTypeDef(
+    _RequiredServicePipelineStateTypeDef, _OptionalServicePipelineStateTypeDef
+):
+    pass
+
+
+_RequiredDeploymentSummaryTypeDef = TypedDict(
+    "_RequiredDeploymentSummaryTypeDef",
+    {
+        "arn": str,
+        "createdAt": datetime,
+        "deploymentStatus": DeploymentStatusType,
+        "environmentName": str,
+        "id": str,
+        "lastModifiedAt": datetime,
+        "targetArn": str,
+        "targetResourceCreatedAt": datetime,
+        "targetResourceType": DeploymentTargetResourceTypeType,
+    },
+)
+_OptionalDeploymentSummaryTypeDef = TypedDict(
+    "_OptionalDeploymentSummaryTypeDef",
+    {
+        "completedAt": datetime,
+        "componentName": str,
+        "lastAttemptedDeploymentId": str,
+        "lastSucceededDeploymentId": str,
+        "serviceInstanceName": str,
+        "serviceName": str,
+    },
+    total=False,
+)
+
+
+class DeploymentSummaryTypeDef(
+    _RequiredDeploymentSummaryTypeDef, _OptionalDeploymentSummaryTypeDef
+):
+    pass
+
+
 _RequiredEnvironmentAccountConnectionSummaryTypeDef = TypedDict(
     "_RequiredEnvironmentAccountConnectionSummaryTypeDef",
     {
         "arn": str,
         "environmentAccountId": str,
         "environmentName": str,
         "id": str,
@@ -862,14 +1007,16 @@
     "_OptionalEnvironmentSummaryTypeDef",
     {
         "componentRoleArn": str,
         "deploymentStatusMessage": str,
         "description": str,
         "environmentAccountConnectionId": str,
         "environmentAccountId": str,
+        "lastAttemptedDeploymentId": str,
+        "lastSucceededDeploymentId": str,
         "protonServiceRoleArn": str,
         "provisioning": Literal["CUSTOMER_MANAGED"],
     },
     total=False,
 )
 
 
@@ -956,14 +1103,38 @@
 GetComponentInputRequestTypeDef = TypedDict(
     "GetComponentInputRequestTypeDef",
     {
         "name": str,
     },
 )
 
+_RequiredGetDeploymentInputRequestTypeDef = TypedDict(
+    "_RequiredGetDeploymentInputRequestTypeDef",
+    {
+        "id": str,
+    },
+)
+_OptionalGetDeploymentInputRequestTypeDef = TypedDict(
+    "_OptionalGetDeploymentInputRequestTypeDef",
+    {
+        "componentName": str,
+        "environmentName": str,
+        "serviceInstanceName": str,
+        "serviceName": str,
+    },
+    total=False,
+)
+
+
+class GetDeploymentInputRequestTypeDef(
+    _RequiredGetDeploymentInputRequestTypeDef, _OptionalGetDeploymentInputRequestTypeDef
+):
+    pass
+
+
 GetEnvironmentAccountConnectionInputRequestTypeDef = TypedDict(
     "GetEnvironmentAccountConnectionInputRequestTypeDef",
     {
         "id": str,
     },
 )
 
@@ -1119,14 +1290,15 @@
     {
         "componentName": str,
     },
 )
 _OptionalListComponentOutputsInputRequestTypeDef = TypedDict(
     "_OptionalListComponentOutputsInputRequestTypeDef",
     {
+        "deploymentId": str,
         "nextToken": str,
     },
     total=False,
 )
 
 
 class ListComponentOutputsInputRequestTypeDef(
@@ -1185,14 +1357,27 @@
         "nextToken": str,
         "serviceInstanceName": str,
         "serviceName": str,
     },
     total=False,
 )
 
+ListDeploymentsInputRequestTypeDef = TypedDict(
+    "ListDeploymentsInputRequestTypeDef",
+    {
+        "componentName": str,
+        "environmentName": str,
+        "maxResults": int,
+        "nextToken": str,
+        "serviceInstanceName": str,
+        "serviceName": str,
+    },
+    total=False,
+)
+
 _RequiredListEnvironmentAccountConnectionsInputRequestTypeDef = TypedDict(
     "_RequiredListEnvironmentAccountConnectionsInputRequestTypeDef",
     {
         "requestedBy": EnvironmentAccountConnectionRequesterAccountTypeType,
     },
 )
 _OptionalListEnvironmentAccountConnectionsInputRequestTypeDef = TypedDict(
@@ -1219,14 +1404,15 @@
     {
         "environmentName": str,
     },
 )
 _OptionalListEnvironmentOutputsInputRequestTypeDef = TypedDict(
     "_OptionalListEnvironmentOutputsInputRequestTypeDef",
     {
+        "deploymentId": str,
         "nextToken": str,
     },
     total=False,
 )
 
 
 class ListEnvironmentOutputsInputRequestTypeDef(
@@ -1350,14 +1536,15 @@
         "serviceInstanceName": str,
         "serviceName": str,
     },
 )
 _OptionalListServiceInstanceOutputsInputRequestTypeDef = TypedDict(
     "_OptionalListServiceInstanceOutputsInputRequestTypeDef",
     {
+        "deploymentId": str,
         "nextToken": str,
     },
     total=False,
 )
 
 
 class ListServiceInstanceOutputsInputRequestTypeDef(
@@ -1415,14 +1602,16 @@
         "templateName": str,
     },
 )
 _OptionalServiceInstanceSummaryTypeDef = TypedDict(
     "_OptionalServiceInstanceSummaryTypeDef",
     {
         "deploymentStatusMessage": str,
+        "lastAttemptedDeploymentId": str,
+        "lastSucceededDeploymentId": str,
     },
     total=False,
 )
 
 
 class ServiceInstanceSummaryTypeDef(
     _RequiredServiceInstanceSummaryTypeDef, _OptionalServiceInstanceSummaryTypeDef
@@ -1435,14 +1624,15 @@
     {
         "serviceName": str,
     },
 )
 _OptionalListServicePipelineOutputsInputRequestTypeDef = TypedDict(
     "_OptionalListServicePipelineOutputsInputRequestTypeDef",
     {
+        "deploymentId": str,
         "nextToken": str,
     },
     total=False,
 )
 
 
 class ListServicePipelineOutputsInputRequestTypeDef(
@@ -2014,14 +2204,16 @@
     {
         "codebuildRoleArn": str,
         "componentRoleArn": str,
         "deploymentStatusMessage": str,
         "description": str,
         "environmentAccountConnectionId": str,
         "environmentAccountId": str,
+        "lastAttemptedDeploymentId": str,
+        "lastSucceededDeploymentId": str,
         "protonServiceRoleArn": str,
         "provisioning": Literal["CUSTOMER_MANAGED"],
         "provisioningRepository": RepositoryBranchTypeDef,
         "spec": str,
     },
     total=False,
 )
@@ -2688,14 +2880,34 @@
     "UpdateTemplateSyncConfigOutputTypeDef",
     {
         "templateSyncConfig": TemplateSyncConfigTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DeploymentStateTypeDef = TypedDict(
+    "DeploymentStateTypeDef",
+    {
+        "component": ComponentStateTypeDef,
+        "environment": EnvironmentStateTypeDef,
+        "serviceInstance": ServiceInstanceStateTypeDef,
+        "servicePipeline": ServicePipelineStateTypeDef,
+    },
+    total=False,
+)
+
+ListDeploymentsOutputTypeDef = TypedDict(
+    "ListDeploymentsOutputTypeDef",
+    {
+        "deployments": List[DeploymentSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListEnvironmentAccountConnectionsOutputTypeDef = TypedDict(
     "ListEnvironmentAccountConnectionsOutputTypeDef",
     {
         "environmentAccountConnections": List[EnvironmentAccountConnectionSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2968,14 +3180,15 @@
     {
         "componentName": str,
     },
 )
 _OptionalListComponentOutputsInputListComponentOutputsPaginateTypeDef = TypedDict(
     "_OptionalListComponentOutputsInputListComponentOutputsPaginateTypeDef",
     {
+        "deploymentId": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class ListComponentOutputsInputListComponentOutputsPaginateTypeDef(
@@ -3014,14 +3227,26 @@
         "serviceInstanceName": str,
         "serviceName": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+ListDeploymentsInputListDeploymentsPaginateTypeDef = TypedDict(
+    "ListDeploymentsInputListDeploymentsPaginateTypeDef",
+    {
+        "componentName": str,
+        "environmentName": str,
+        "serviceInstanceName": str,
+        "serviceName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 _RequiredListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef = TypedDict(
     "_RequiredListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef",
     {
         "requestedBy": EnvironmentAccountConnectionRequesterAccountTypeType,
     },
 )
 _OptionalListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef = TypedDict(
@@ -3047,14 +3272,15 @@
     {
         "environmentName": str,
     },
 )
 _OptionalListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef = TypedDict(
     "_OptionalListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef",
     {
+        "deploymentId": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class ListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef(
@@ -3164,14 +3390,15 @@
         "serviceInstanceName": str,
         "serviceName": str,
     },
 )
 _OptionalListServiceInstanceOutputsInputListServiceInstanceOutputsPaginateTypeDef = TypedDict(
     "_OptionalListServiceInstanceOutputsInputListServiceInstanceOutputsPaginateTypeDef",
     {
+        "deploymentId": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class ListServiceInstanceOutputsInputListServiceInstanceOutputsPaginateTypeDef(
@@ -3209,14 +3436,15 @@
     {
         "serviceName": str,
     },
 )
 _OptionalListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef = TypedDict(
     "_OptionalListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef",
     {
+        "deploymentId": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class ListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef(
@@ -3663,14 +3891,49 @@
     "GetResourcesSummaryOutputTypeDef",
     {
         "counts": CountsSummaryTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredDeploymentTypeDef = TypedDict(
+    "_RequiredDeploymentTypeDef",
+    {
+        "arn": str,
+        "createdAt": datetime,
+        "deploymentStatus": DeploymentStatusType,
+        "environmentName": str,
+        "id": str,
+        "lastModifiedAt": datetime,
+        "targetArn": str,
+        "targetResourceCreatedAt": datetime,
+        "targetResourceType": DeploymentTargetResourceTypeType,
+    },
+)
+_OptionalDeploymentTypeDef = TypedDict(
+    "_OptionalDeploymentTypeDef",
+    {
+        "completedAt": datetime,
+        "componentName": str,
+        "deploymentStatusMessage": str,
+        "initialState": DeploymentStateTypeDef,
+        "lastAttemptedDeploymentId": str,
+        "lastSucceededDeploymentId": str,
+        "serviceInstanceName": str,
+        "serviceName": str,
+        "targetState": DeploymentStateTypeDef,
+    },
+    total=False,
+)
+
+
+class DeploymentTypeDef(_RequiredDeploymentTypeDef, _OptionalDeploymentTypeDef):
+    pass
+
+
 GetRepositorySyncStatusOutputTypeDef = TypedDict(
     "GetRepositorySyncStatusOutputTypeDef",
     {
         "latestSync": RepositorySyncAttemptTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3777,14 +4040,30 @@
         "serviceInstanceName": str,
         "serviceName": str,
         "serviceSyncBlocker": SyncBlockerTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DeleteDeploymentOutputTypeDef = TypedDict(
+    "DeleteDeploymentOutputTypeDef",
+    {
+        "deployment": DeploymentTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDeploymentOutputTypeDef = TypedDict(
+    "GetDeploymentOutputTypeDef",
+    {
+        "deployment": DeploymentTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetServiceSyncBlockerSummaryOutputTypeDef = TypedDict(
     "GetServiceSyncBlockerSummaryOutputTypeDef",
     {
         "serviceSyncBlockerSummary": ServiceSyncBlockerSummaryTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-proton-2.5.2.post1/types_aiobotocore_proton/type_defs.pyi` & `types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from datetime import datetime
 from typing import Dict, List, Sequence
 
 from .literals import (
     BlockerStatusType,
     ComponentDeploymentUpdateTypeType,
     DeploymentStatusType,
+    DeploymentTargetResourceTypeType,
     DeploymentUpdateTypeType,
     EnvironmentAccountConnectionRequesterAccountTypeType,
     EnvironmentAccountConnectionStatusType,
     ListServiceInstancesFilterByType,
     ListServiceInstancesSortByType,
     ProvisionedResourceEngineType,
     RepositoryProviderType,
@@ -55,44 +56,51 @@
     "CancelEnvironmentDeploymentInputRequestTypeDef",
     "CancelServiceInstanceDeploymentInputRequestTypeDef",
     "ServiceInstanceTypeDef",
     "CancelServicePipelineDeploymentInputRequestTypeDef",
     "ServicePipelineTypeDef",
     "CompatibleEnvironmentTemplateInputTypeDef",
     "CompatibleEnvironmentTemplateTypeDef",
+    "ComponentStateTypeDef",
     "ComponentSummaryTypeDef",
     "ResourceCountsSummaryTypeDef",
     "TagTypeDef",
     "RepositoryBranchInputTypeDef",
     "EnvironmentTemplateTypeDef",
     "EnvironmentTemplateVersionTypeDef",
     "RepositoryTypeDef",
     "CreateServiceSyncConfigInputRequestTypeDef",
     "ServiceSyncConfigTypeDef",
     "ServiceTemplateTypeDef",
     "CreateTemplateSyncConfigInputRequestTypeDef",
     "TemplateSyncConfigTypeDef",
     "DeleteComponentInputRequestTypeDef",
+    "DeleteDeploymentInputRequestTypeDef",
     "DeleteEnvironmentAccountConnectionInputRequestTypeDef",
     "DeleteEnvironmentInputRequestTypeDef",
     "DeleteEnvironmentTemplateInputRequestTypeDef",
     "DeleteEnvironmentTemplateVersionInputRequestTypeDef",
     "DeleteRepositoryInputRequestTypeDef",
     "DeleteServiceInputRequestTypeDef",
     "DeleteServiceSyncConfigInputRequestTypeDef",
     "DeleteServiceTemplateInputRequestTypeDef",
     "DeleteServiceTemplateVersionInputRequestTypeDef",
     "DeleteTemplateSyncConfigInputRequestTypeDef",
+    "EnvironmentStateTypeDef",
+    "ServiceInstanceStateTypeDef",
+    "ServicePipelineStateTypeDef",
+    "DeploymentSummaryTypeDef",
     "EnvironmentAccountConnectionSummaryTypeDef",
     "EnvironmentSummaryTypeDef",
     "EnvironmentTemplateFilterTypeDef",
     "EnvironmentTemplateSummaryTypeDef",
     "EnvironmentTemplateVersionSummaryTypeDef",
     "WaiterConfigTypeDef",
     "GetComponentInputRequestTypeDef",
+    "GetDeploymentInputRequestTypeDef",
     "GetEnvironmentAccountConnectionInputRequestTypeDef",
     "GetEnvironmentInputRequestTypeDef",
     "GetEnvironmentTemplateInputRequestTypeDef",
     "GetEnvironmentTemplateVersionInputRequestTypeDef",
     "GetRepositoryInputRequestTypeDef",
     "GetRepositorySyncStatusInputRequestTypeDef",
     "GetServiceInputRequestTypeDef",
@@ -107,14 +115,15 @@
     "GetTemplateSyncStatusInputRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ListComponentOutputsInputRequestTypeDef",
     "OutputTypeDef",
     "ListComponentProvisionedResourcesInputRequestTypeDef",
     "ProvisionedResourceTypeDef",
     "ListComponentsInputRequestTypeDef",
+    "ListDeploymentsInputRequestTypeDef",
     "ListEnvironmentAccountConnectionsInputRequestTypeDef",
     "ListEnvironmentOutputsInputRequestTypeDef",
     "ListEnvironmentProvisionedResourcesInputRequestTypeDef",
     "ListEnvironmentTemplateVersionsInputRequestTypeDef",
     "ListEnvironmentTemplatesInputRequestTypeDef",
     "ListRepositoriesInputRequestTypeDef",
     "RepositorySummaryTypeDef",
@@ -205,14 +214,16 @@
     "DeleteServiceTemplateOutputTypeDef",
     "GetServiceTemplateOutputTypeDef",
     "UpdateServiceTemplateOutputTypeDef",
     "CreateTemplateSyncConfigOutputTypeDef",
     "DeleteTemplateSyncConfigOutputTypeDef",
     "GetTemplateSyncConfigOutputTypeDef",
     "UpdateTemplateSyncConfigOutputTypeDef",
+    "DeploymentStateTypeDef",
+    "ListDeploymentsOutputTypeDef",
     "ListEnvironmentAccountConnectionsOutputTypeDef",
     "ListEnvironmentsOutputTypeDef",
     "ListEnvironmentsInputRequestTypeDef",
     "ListEnvironmentTemplatesOutputTypeDef",
     "ListEnvironmentTemplateVersionsOutputTypeDef",
     "GetComponentInputComponentDeletedWaitTypeDef",
     "GetComponentInputComponentDeployedWaitTypeDef",
@@ -223,14 +234,15 @@
     "GetServiceInputServicePipelineDeployedWaitTypeDef",
     "GetServiceInputServiceUpdatedWaitTypeDef",
     "GetServiceInstanceInputServiceInstanceDeployedWaitTypeDef",
     "GetServiceTemplateVersionInputServiceTemplateVersionRegisteredWaitTypeDef",
     "ListComponentOutputsInputListComponentOutputsPaginateTypeDef",
     "ListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef",
     "ListComponentsInputListComponentsPaginateTypeDef",
+    "ListDeploymentsInputListDeploymentsPaginateTypeDef",
     "ListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef",
     "ListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef",
     "ListEnvironmentProvisionedResourcesInputListEnvironmentProvisionedResourcesPaginateTypeDef",
     "ListEnvironmentTemplateVersionsInputListEnvironmentTemplateVersionsPaginateTypeDef",
     "ListEnvironmentTemplatesInputListEnvironmentTemplatesPaginateTypeDef",
     "ListEnvironmentsInputListEnvironmentsPaginateTypeDef",
     "ListRepositoriesInputListRepositoriesPaginateTypeDef",
@@ -276,21 +288,24 @@
     "GetServiceOutputTypeDef",
     "UpdateServiceOutputTypeDef",
     "CreateServiceTemplateVersionOutputTypeDef",
     "DeleteServiceTemplateVersionOutputTypeDef",
     "GetServiceTemplateVersionOutputTypeDef",
     "UpdateServiceTemplateVersionOutputTypeDef",
     "GetResourcesSummaryOutputTypeDef",
+    "DeploymentTypeDef",
     "GetRepositorySyncStatusOutputTypeDef",
     "GetServiceInstanceSyncStatusOutputTypeDef",
     "GetTemplateSyncStatusOutputTypeDef",
     "CreateEnvironmentTemplateVersionInputRequestTypeDef",
     "CreateServiceTemplateVersionInputRequestTypeDef",
     "ServiceSyncBlockerSummaryTypeDef",
     "UpdateServiceSyncBlockerOutputTypeDef",
+    "DeleteDeploymentOutputTypeDef",
+    "GetDeploymentOutputTypeDef",
     "GetServiceSyncBlockerSummaryOutputTypeDef",
 )
 
 AcceptEnvironmentAccountConnectionInputRequestTypeDef = TypedDict(
     "AcceptEnvironmentAccountConnectionInputRequestTypeDef",
     {
         "id": str,
@@ -365,17 +380,19 @@
     },
 )
 _OptionalComponentTypeDef = TypedDict(
     "_OptionalComponentTypeDef",
     {
         "deploymentStatusMessage": str,
         "description": str,
+        "lastAttemptedDeploymentId": str,
         "lastClientRequestToken": str,
         "lastDeploymentAttemptedAt": datetime,
         "lastDeploymentSucceededAt": datetime,
+        "lastSucceededDeploymentId": str,
         "serviceInstanceName": str,
         "serviceName": str,
         "serviceSpec": str,
     },
     total=False,
 )
 
@@ -413,15 +430,17 @@
         "templateName": str,
     },
 )
 _OptionalServiceInstanceTypeDef = TypedDict(
     "_OptionalServiceInstanceTypeDef",
     {
         "deploymentStatusMessage": str,
+        "lastAttemptedDeploymentId": str,
         "lastClientRequestToken": str,
+        "lastSucceededDeploymentId": str,
         "spec": str,
     },
     total=False,
 )
 
 class ServiceInstanceTypeDef(_RequiredServiceInstanceTypeDef, _OptionalServiceInstanceTypeDef):
     pass
@@ -446,14 +465,16 @@
         "templateName": str,
     },
 )
 _OptionalServicePipelineTypeDef = TypedDict(
     "_OptionalServicePipelineTypeDef",
     {
         "deploymentStatusMessage": str,
+        "lastAttemptedDeploymentId": str,
+        "lastSucceededDeploymentId": str,
         "spec": str,
     },
     total=False,
 )
 
 class ServicePipelineTypeDef(_RequiredServicePipelineTypeDef, _OptionalServicePipelineTypeDef):
     pass
@@ -470,14 +491,25 @@
     "CompatibleEnvironmentTemplateTypeDef",
     {
         "majorVersion": str,
         "templateName": str,
     },
 )
 
+ComponentStateTypeDef = TypedDict(
+    "ComponentStateTypeDef",
+    {
+        "serviceInstanceName": str,
+        "serviceName": str,
+        "serviceSpec": str,
+        "templateFile": str,
+    },
+    total=False,
+)
+
 _RequiredComponentSummaryTypeDef = TypedDict(
     "_RequiredComponentSummaryTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "deploymentStatus": DeploymentStatusType,
         "environmentName": str,
@@ -485,16 +517,18 @@
         "name": str,
     },
 )
 _OptionalComponentSummaryTypeDef = TypedDict(
     "_OptionalComponentSummaryTypeDef",
     {
         "deploymentStatusMessage": str,
+        "lastAttemptedDeploymentId": str,
         "lastDeploymentAttemptedAt": datetime,
         "lastDeploymentSucceededAt": datetime,
+        "lastSucceededDeploymentId": str,
         "serviceInstanceName": str,
         "serviceName": str,
     },
     total=False,
 )
 
 class ComponentSummaryTypeDef(_RequiredComponentSummaryTypeDef, _OptionalComponentSummaryTypeDef):
@@ -709,14 +743,21 @@
 DeleteComponentInputRequestTypeDef = TypedDict(
     "DeleteComponentInputRequestTypeDef",
     {
         "name": str,
     },
 )
 
+DeleteDeploymentInputRequestTypeDef = TypedDict(
+    "DeleteDeploymentInputRequestTypeDef",
+    {
+        "id": str,
+    },
+)
+
 DeleteEnvironmentAccountConnectionInputRequestTypeDef = TypedDict(
     "DeleteEnvironmentAccountConnectionInputRequestTypeDef",
     {
         "id": str,
     },
 )
 
@@ -785,14 +826,110 @@
     "DeleteTemplateSyncConfigInputRequestTypeDef",
     {
         "templateName": str,
         "templateType": TemplateTypeType,
     },
 )
 
+_RequiredEnvironmentStateTypeDef = TypedDict(
+    "_RequiredEnvironmentStateTypeDef",
+    {
+        "templateMajorVersion": str,
+        "templateMinorVersion": str,
+        "templateName": str,
+    },
+)
+_OptionalEnvironmentStateTypeDef = TypedDict(
+    "_OptionalEnvironmentStateTypeDef",
+    {
+        "spec": str,
+    },
+    total=False,
+)
+
+class EnvironmentStateTypeDef(_RequiredEnvironmentStateTypeDef, _OptionalEnvironmentStateTypeDef):
+    pass
+
+_RequiredServiceInstanceStateTypeDef = TypedDict(
+    "_RequiredServiceInstanceStateTypeDef",
+    {
+        "spec": str,
+        "templateMajorVersion": str,
+        "templateMinorVersion": str,
+        "templateName": str,
+    },
+)
+_OptionalServiceInstanceStateTypeDef = TypedDict(
+    "_OptionalServiceInstanceStateTypeDef",
+    {
+        "lastSuccessfulComponentDeploymentIds": List[str],
+        "lastSuccessfulEnvironmentDeploymentId": str,
+        "lastSuccessfulServicePipelineDeploymentId": str,
+    },
+    total=False,
+)
+
+class ServiceInstanceStateTypeDef(
+    _RequiredServiceInstanceStateTypeDef, _OptionalServiceInstanceStateTypeDef
+):
+    pass
+
+_RequiredServicePipelineStateTypeDef = TypedDict(
+    "_RequiredServicePipelineStateTypeDef",
+    {
+        "templateMajorVersion": str,
+        "templateMinorVersion": str,
+        "templateName": str,
+    },
+)
+_OptionalServicePipelineStateTypeDef = TypedDict(
+    "_OptionalServicePipelineStateTypeDef",
+    {
+        "spec": str,
+    },
+    total=False,
+)
+
+class ServicePipelineStateTypeDef(
+    _RequiredServicePipelineStateTypeDef, _OptionalServicePipelineStateTypeDef
+):
+    pass
+
+_RequiredDeploymentSummaryTypeDef = TypedDict(
+    "_RequiredDeploymentSummaryTypeDef",
+    {
+        "arn": str,
+        "createdAt": datetime,
+        "deploymentStatus": DeploymentStatusType,
+        "environmentName": str,
+        "id": str,
+        "lastModifiedAt": datetime,
+        "targetArn": str,
+        "targetResourceCreatedAt": datetime,
+        "targetResourceType": DeploymentTargetResourceTypeType,
+    },
+)
+_OptionalDeploymentSummaryTypeDef = TypedDict(
+    "_OptionalDeploymentSummaryTypeDef",
+    {
+        "completedAt": datetime,
+        "componentName": str,
+        "lastAttemptedDeploymentId": str,
+        "lastSucceededDeploymentId": str,
+        "serviceInstanceName": str,
+        "serviceName": str,
+    },
+    total=False,
+)
+
+class DeploymentSummaryTypeDef(
+    _RequiredDeploymentSummaryTypeDef, _OptionalDeploymentSummaryTypeDef
+):
+    pass
+
 _RequiredEnvironmentAccountConnectionSummaryTypeDef = TypedDict(
     "_RequiredEnvironmentAccountConnectionSummaryTypeDef",
     {
         "arn": str,
         "environmentAccountId": str,
         "environmentName": str,
         "id": str,
@@ -835,14 +972,16 @@
     "_OptionalEnvironmentSummaryTypeDef",
     {
         "componentRoleArn": str,
         "deploymentStatusMessage": str,
         "description": str,
         "environmentAccountConnectionId": str,
         "environmentAccountId": str,
+        "lastAttemptedDeploymentId": str,
+        "lastSucceededDeploymentId": str,
         "protonServiceRoleArn": str,
         "provisioning": Literal["CUSTOMER_MANAGED"],
     },
     total=False,
 )
 
 class EnvironmentSummaryTypeDef(
@@ -923,14 +1062,36 @@
 GetComponentInputRequestTypeDef = TypedDict(
     "GetComponentInputRequestTypeDef",
     {
         "name": str,
     },
 )
 
+_RequiredGetDeploymentInputRequestTypeDef = TypedDict(
+    "_RequiredGetDeploymentInputRequestTypeDef",
+    {
+        "id": str,
+    },
+)
+_OptionalGetDeploymentInputRequestTypeDef = TypedDict(
+    "_OptionalGetDeploymentInputRequestTypeDef",
+    {
+        "componentName": str,
+        "environmentName": str,
+        "serviceInstanceName": str,
+        "serviceName": str,
+    },
+    total=False,
+)
+
+class GetDeploymentInputRequestTypeDef(
+    _RequiredGetDeploymentInputRequestTypeDef, _OptionalGetDeploymentInputRequestTypeDef
+):
+    pass
+
 GetEnvironmentAccountConnectionInputRequestTypeDef = TypedDict(
     "GetEnvironmentAccountConnectionInputRequestTypeDef",
     {
         "id": str,
     },
 )
 
@@ -1084,14 +1245,15 @@
     {
         "componentName": str,
     },
 )
 _OptionalListComponentOutputsInputRequestTypeDef = TypedDict(
     "_OptionalListComponentOutputsInputRequestTypeDef",
     {
+        "deploymentId": str,
         "nextToken": str,
     },
     total=False,
 )
 
 class ListComponentOutputsInputRequestTypeDef(
     _RequiredListComponentOutputsInputRequestTypeDef,
@@ -1146,14 +1308,27 @@
         "nextToken": str,
         "serviceInstanceName": str,
         "serviceName": str,
     },
     total=False,
 )
 
+ListDeploymentsInputRequestTypeDef = TypedDict(
+    "ListDeploymentsInputRequestTypeDef",
+    {
+        "componentName": str,
+        "environmentName": str,
+        "maxResults": int,
+        "nextToken": str,
+        "serviceInstanceName": str,
+        "serviceName": str,
+    },
+    total=False,
+)
+
 _RequiredListEnvironmentAccountConnectionsInputRequestTypeDef = TypedDict(
     "_RequiredListEnvironmentAccountConnectionsInputRequestTypeDef",
     {
         "requestedBy": EnvironmentAccountConnectionRequesterAccountTypeType,
     },
 )
 _OptionalListEnvironmentAccountConnectionsInputRequestTypeDef = TypedDict(
@@ -1178,14 +1353,15 @@
     {
         "environmentName": str,
     },
 )
 _OptionalListEnvironmentOutputsInputRequestTypeDef = TypedDict(
     "_OptionalListEnvironmentOutputsInputRequestTypeDef",
     {
+        "deploymentId": str,
         "nextToken": str,
     },
     total=False,
 )
 
 class ListEnvironmentOutputsInputRequestTypeDef(
     _RequiredListEnvironmentOutputsInputRequestTypeDef,
@@ -1301,14 +1477,15 @@
         "serviceInstanceName": str,
         "serviceName": str,
     },
 )
 _OptionalListServiceInstanceOutputsInputRequestTypeDef = TypedDict(
     "_OptionalListServiceInstanceOutputsInputRequestTypeDef",
     {
+        "deploymentId": str,
         "nextToken": str,
     },
     total=False,
 )
 
 class ListServiceInstanceOutputsInputRequestTypeDef(
     _RequiredListServiceInstanceOutputsInputRequestTypeDef,
@@ -1362,14 +1539,16 @@
         "templateName": str,
     },
 )
 _OptionalServiceInstanceSummaryTypeDef = TypedDict(
     "_OptionalServiceInstanceSummaryTypeDef",
     {
         "deploymentStatusMessage": str,
+        "lastAttemptedDeploymentId": str,
+        "lastSucceededDeploymentId": str,
     },
     total=False,
 )
 
 class ServiceInstanceSummaryTypeDef(
     _RequiredServiceInstanceSummaryTypeDef, _OptionalServiceInstanceSummaryTypeDef
 ):
@@ -1380,14 +1559,15 @@
     {
         "serviceName": str,
     },
 )
 _OptionalListServicePipelineOutputsInputRequestTypeDef = TypedDict(
     "_OptionalListServicePipelineOutputsInputRequestTypeDef",
     {
+        "deploymentId": str,
         "nextToken": str,
     },
     total=False,
 )
 
 class ListServicePipelineOutputsInputRequestTypeDef(
     _RequiredListServicePipelineOutputsInputRequestTypeDef,
@@ -1923,14 +2103,16 @@
     {
         "codebuildRoleArn": str,
         "componentRoleArn": str,
         "deploymentStatusMessage": str,
         "description": str,
         "environmentAccountConnectionId": str,
         "environmentAccountId": str,
+        "lastAttemptedDeploymentId": str,
+        "lastSucceededDeploymentId": str,
         "protonServiceRoleArn": str,
         "provisioning": Literal["CUSTOMER_MANAGED"],
         "provisioningRepository": RepositoryBranchTypeDef,
         "spec": str,
     },
     total=False,
 )
@@ -2571,14 +2753,34 @@
     "UpdateTemplateSyncConfigOutputTypeDef",
     {
         "templateSyncConfig": TemplateSyncConfigTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DeploymentStateTypeDef = TypedDict(
+    "DeploymentStateTypeDef",
+    {
+        "component": ComponentStateTypeDef,
+        "environment": EnvironmentStateTypeDef,
+        "serviceInstance": ServiceInstanceStateTypeDef,
+        "servicePipeline": ServicePipelineStateTypeDef,
+    },
+    total=False,
+)
+
+ListDeploymentsOutputTypeDef = TypedDict(
+    "ListDeploymentsOutputTypeDef",
+    {
+        "deployments": List[DeploymentSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListEnvironmentAccountConnectionsOutputTypeDef = TypedDict(
     "ListEnvironmentAccountConnectionsOutputTypeDef",
     {
         "environmentAccountConnections": List[EnvironmentAccountConnectionSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2831,14 +3033,15 @@
     {
         "componentName": str,
     },
 )
 _OptionalListComponentOutputsInputListComponentOutputsPaginateTypeDef = TypedDict(
     "_OptionalListComponentOutputsInputListComponentOutputsPaginateTypeDef",
     {
+        "deploymentId": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class ListComponentOutputsInputListComponentOutputsPaginateTypeDef(
     _RequiredListComponentOutputsInputListComponentOutputsPaginateTypeDef,
@@ -2873,14 +3076,26 @@
         "serviceInstanceName": str,
         "serviceName": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+ListDeploymentsInputListDeploymentsPaginateTypeDef = TypedDict(
+    "ListDeploymentsInputListDeploymentsPaginateTypeDef",
+    {
+        "componentName": str,
+        "environmentName": str,
+        "serviceInstanceName": str,
+        "serviceName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 _RequiredListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef = TypedDict(
     "_RequiredListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef",
     {
         "requestedBy": EnvironmentAccountConnectionRequesterAccountTypeType,
     },
 )
 _OptionalListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef = TypedDict(
@@ -2904,14 +3119,15 @@
     {
         "environmentName": str,
     },
 )
 _OptionalListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef = TypedDict(
     "_OptionalListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef",
     {
+        "deploymentId": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class ListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef(
     _RequiredListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef,
@@ -3013,14 +3229,15 @@
         "serviceInstanceName": str,
         "serviceName": str,
     },
 )
 _OptionalListServiceInstanceOutputsInputListServiceInstanceOutputsPaginateTypeDef = TypedDict(
     "_OptionalListServiceInstanceOutputsInputListServiceInstanceOutputsPaginateTypeDef",
     {
+        "deploymentId": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class ListServiceInstanceOutputsInputListServiceInstanceOutputsPaginateTypeDef(
     _RequiredListServiceInstanceOutputsInputListServiceInstanceOutputsPaginateTypeDef,
@@ -3054,14 +3271,15 @@
     {
         "serviceName": str,
     },
 )
 _OptionalListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef = TypedDict(
     "_OptionalListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef",
     {
+        "deploymentId": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class ListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef(
     _RequiredListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef,
@@ -3496,14 +3714,47 @@
     "GetResourcesSummaryOutputTypeDef",
     {
         "counts": CountsSummaryTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredDeploymentTypeDef = TypedDict(
+    "_RequiredDeploymentTypeDef",
+    {
+        "arn": str,
+        "createdAt": datetime,
+        "deploymentStatus": DeploymentStatusType,
+        "environmentName": str,
+        "id": str,
+        "lastModifiedAt": datetime,
+        "targetArn": str,
+        "targetResourceCreatedAt": datetime,
+        "targetResourceType": DeploymentTargetResourceTypeType,
+    },
+)
+_OptionalDeploymentTypeDef = TypedDict(
+    "_OptionalDeploymentTypeDef",
+    {
+        "completedAt": datetime,
+        "componentName": str,
+        "deploymentStatusMessage": str,
+        "initialState": DeploymentStateTypeDef,
+        "lastAttemptedDeploymentId": str,
+        "lastSucceededDeploymentId": str,
+        "serviceInstanceName": str,
+        "serviceName": str,
+        "targetState": DeploymentStateTypeDef,
+    },
+    total=False,
+)
+
+class DeploymentTypeDef(_RequiredDeploymentTypeDef, _OptionalDeploymentTypeDef):
+    pass
+
 GetRepositorySyncStatusOutputTypeDef = TypedDict(
     "GetRepositorySyncStatusOutputTypeDef",
     {
         "latestSync": RepositorySyncAttemptTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3604,14 +3855,30 @@
         "serviceInstanceName": str,
         "serviceName": str,
         "serviceSyncBlocker": SyncBlockerTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DeleteDeploymentOutputTypeDef = TypedDict(
+    "DeleteDeploymentOutputTypeDef",
+    {
+        "deployment": DeploymentTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDeploymentOutputTypeDef = TypedDict(
+    "GetDeploymentOutputTypeDef",
+    {
+        "deployment": DeploymentTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetServiceSyncBlockerSummaryOutputTypeDef = TypedDict(
     "GetServiceSyncBlockerSummaryOutputTypeDef",
     {
         "serviceSyncBlockerSummary": ServiceSyncBlockerSummaryTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-proton-2.5.2.post1/types_aiobotocore_proton/waiter.py` & `types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-proton-2.5.2.post1/types_aiobotocore_proton/waiter.pyi` & `types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-proton-2.5.2.post1/types_aiobotocore_proton.egg-info/SOURCES.txt` & `types-aiobotocore-proton-2.5.2.post2/types_aiobotocore_proton.egg-info/SOURCES.txt`

 * *Files identical despite different names*

