# Comparing `tmp/types-aiobotocore-appmesh-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-appmesh-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-appmesh-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:52 2023, max compression
+gzip compressed data, was "types-aiobotocore-appmesh-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:25 2023, max compression
```

## Comparing `types-aiobotocore-appmesh-2.5.2.post1.tar` & `types-aiobotocore-appmesh-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:52.809654 types-aiobotocore-appmesh-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:33:17.000000 types-aiobotocore-appmesh-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    24847 2023-08-02 14:51:52.805654 types-aiobotocore-appmesh-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23329 2023-08-02 14:33:17.000000 types-aiobotocore-appmesh-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:52.809654 types-aiobotocore-appmesh-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-08-02 14:33:17.000000 types-aiobotocore-appmesh-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:52.801654 types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh/
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-08-02 14:33:17.000000 types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-08-02 14:33:17.000000 types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-02 14:33:17.000000 types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32381 2023-08-02 14:33:18.000000 types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    32326 2023-08-02 14:33:18.000000 types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11040 2023-08-02 14:33:18.000000 types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-08-02 14:33:18.000000 types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9947 2023-08-02 14:33:18.000000 types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9937 2023-08-02 14:33:18.000000 types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:33:17.000000 types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   100998 2023-08-02 14:33:20.000000 types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   100807 2023-08-02 14:33:19.000000 types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:33:17.000000 types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:52.805654 types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24847 2023-08-02 14:51:52.000000 types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-02 14:51:52.000000 types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:52.000000 types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:52.000000 types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:52.000000 types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-02 14:51:52.000000 types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:25.519114 types-aiobotocore-appmesh-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:40:26.000000 types-aiobotocore-appmesh-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14004 2023-08-04 12:00:25.515114 types-aiobotocore-appmesh-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12486 2023-08-04 11:40:26.000000 types-aiobotocore-appmesh-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:25.519114 types-aiobotocore-appmesh-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-08-04 11:40:26.000000 types-aiobotocore-appmesh-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:25.511114 types-aiobotocore-appmesh-2.5.2.post2/types_aiobotocore_appmesh/
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-08-04 11:40:26.000000 types-aiobotocore-appmesh-2.5.2.post2/types_aiobotocore_appmesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-08-04 11:40:26.000000 types-aiobotocore-appmesh-2.5.2.post2/types_aiobotocore_appmesh/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-04 11:40:26.000000 types-aiobotocore-appmesh-2.5.2.post2/types_aiobotocore_appmesh/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32306 2023-08-04 11:40:27.000000 types-aiobotocore-appmesh-2.5.2.post2/types_aiobotocore_appmesh/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32251 2023-08-04 11:40:26.000000 types-aiobotocore-appmesh-2.5.2.post2/types_aiobotocore_appmesh/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11040 2023-08-04 11:40:27.000000 types-aiobotocore-appmesh-2.5.2.post2/types_aiobotocore_appmesh/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-08-04 11:40:27.000000 types-aiobotocore-appmesh-2.5.2.post2/types_aiobotocore_appmesh/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9947 2023-08-04 11:40:27.000000 types-aiobotocore-appmesh-2.5.2.post2/types_aiobotocore_appmesh/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9937 2023-08-04 11:40:27.000000 types-aiobotocore-appmesh-2.5.2.post2/types_aiobotocore_appmesh/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:40:26.000000 types-aiobotocore-appmesh-2.5.2.post2/types_aiobotocore_appmesh/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    80416 2023-08-04 11:40:29.000000 types-aiobotocore-appmesh-2.5.2.post2/types_aiobotocore_appmesh/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80265 2023-08-04 11:40:28.000000 types-aiobotocore-appmesh-2.5.2.post2/types_aiobotocore_appmesh/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:40:26.000000 types-aiobotocore-appmesh-2.5.2.post2/types_aiobotocore_appmesh/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:25.515114 types-aiobotocore-appmesh-2.5.2.post2/types_aiobotocore_appmesh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14004 2023-08-04 12:00:25.000000 types-aiobotocore-appmesh-2.5.2.post2/types_aiobotocore_appmesh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-04 12:00:25.000000 types-aiobotocore-appmesh-2.5.2.post2/types_aiobotocore_appmesh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:25.000000 types-aiobotocore-appmesh-2.5.2.post2/types_aiobotocore_appmesh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:25.000000 types-aiobotocore-appmesh-2.5.2.post2/types_aiobotocore_appmesh.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:25.000000 types-aiobotocore-appmesh-2.5.2.post2/types_aiobotocore_appmesh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-04 12:00:25.000000 types-aiobotocore-appmesh-2.5.2.post2/types_aiobotocore_appmesh.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-appmesh-2.5.2.post1/LICENSE` & `types-aiobotocore-appmesh-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appmesh-2.5.2.post1/setup.py` & `types-aiobotocore-appmesh-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-appmesh",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_appmesh"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.AppMesh 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh/__init__.py` & `types-aiobotocore-appmesh-2.5.2.post2/types_aiobotocore_appmesh/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh/__init__.pyi` & `types-aiobotocore-appmesh-2.5.2.post2/types_aiobotocore_appmesh/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh/__main__.py` & `types-aiobotocore-appmesh-2.5.2.post2/types_aiobotocore_appmesh/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.AppMesh 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.AppMesh 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh\nOther"
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

### Comparing `types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh/client.py` & `types-aiobotocore-appmesh-2.5.2.post2/types_aiobotocore_appmesh/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,36 +48,36 @@
     DescribeGatewayRouteOutputTypeDef,
     DescribeMeshOutputTypeDef,
     DescribeRouteOutputTypeDef,
     DescribeVirtualGatewayOutputTypeDef,
     DescribeVirtualNodeOutputTypeDef,
     DescribeVirtualRouterOutputTypeDef,
     DescribeVirtualServiceOutputTypeDef,
-    GatewayRouteSpecUnionTypeDef,
+    GatewayRouteSpecTypeDef,
     ListGatewayRoutesOutputTypeDef,
     ListMeshesOutputTypeDef,
     ListRoutesOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     ListVirtualGatewaysOutputTypeDef,
     ListVirtualNodesOutputTypeDef,
     ListVirtualRoutersOutputTypeDef,
     ListVirtualServicesOutputTypeDef,
     MeshSpecTypeDef,
-    RouteSpecUnionTypeDef,
+    RouteSpecTypeDef,
     TagRefTypeDef,
     UpdateGatewayRouteOutputTypeDef,
     UpdateMeshOutputTypeDef,
     UpdateRouteOutputTypeDef,
     UpdateVirtualGatewayOutputTypeDef,
     UpdateVirtualNodeOutputTypeDef,
     UpdateVirtualRouterOutputTypeDef,
     UpdateVirtualServiceOutputTypeDef,
-    VirtualGatewaySpecUnionTypeDef,
-    VirtualNodeSpecUnionTypeDef,
-    VirtualRouterSpecUnionTypeDef,
+    VirtualGatewaySpecTypeDef,
+    VirtualNodeSpecTypeDef,
+    VirtualRouterSpecTypeDef,
     VirtualServiceSpecTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -142,15 +142,15 @@
         """
 
     async def create_gateway_route(
         self,
         *,
         gatewayRouteName: str,
         meshName: str,
-        spec: GatewayRouteSpecUnionTypeDef,
+        spec: GatewayRouteSpecTypeDef,
         virtualGatewayName: str,
         clientToken: str = ...,
         meshOwner: str = ...,
         tags: Sequence[TagRefTypeDef] = ...
     ) -> CreateGatewayRouteOutputTypeDef:
         """
         Creates a gateway route.
@@ -175,15 +175,15 @@
         """
 
     async def create_route(
         self,
         *,
         meshName: str,
         routeName: str,
-        spec: RouteSpecUnionTypeDef,
+        spec: RouteSpecTypeDef,
         virtualRouterName: str,
         clientToken: str = ...,
         meshOwner: str = ...,
         tags: Sequence[TagRefTypeDef] = ...
     ) -> CreateRouteOutputTypeDef:
         """
         Creates a route that is associated with a virtual router.
@@ -192,15 +192,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#create_route)
         """
 
     async def create_virtual_gateway(
         self,
         *,
         meshName: str,
-        spec: VirtualGatewaySpecUnionTypeDef,
+        spec: VirtualGatewaySpecTypeDef,
         virtualGatewayName: str,
         clientToken: str = ...,
         meshOwner: str = ...,
         tags: Sequence[TagRefTypeDef] = ...
     ) -> CreateVirtualGatewayOutputTypeDef:
         """
         Creates a virtual gateway.
@@ -209,15 +209,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#create_virtual_gateway)
         """
 
     async def create_virtual_node(
         self,
         *,
         meshName: str,
-        spec: VirtualNodeSpecUnionTypeDef,
+        spec: VirtualNodeSpecTypeDef,
         virtualNodeName: str,
         clientToken: str = ...,
         meshOwner: str = ...,
         tags: Sequence[TagRefTypeDef] = ...
     ) -> CreateVirtualNodeOutputTypeDef:
         """
         Creates a virtual node within a service mesh.
@@ -226,15 +226,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#create_virtual_node)
         """
 
     async def create_virtual_router(
         self,
         *,
         meshName: str,
-        spec: VirtualRouterSpecUnionTypeDef,
+        spec: VirtualRouterSpecTypeDef,
         virtualRouterName: str,
         clientToken: str = ...,
         meshOwner: str = ...,
         tags: Sequence[TagRefTypeDef] = ...
     ) -> CreateVirtualRouterOutputTypeDef:
         """
         Creates a virtual router within a service mesh.
@@ -524,15 +524,15 @@
         """
 
     async def update_gateway_route(
         self,
         *,
         gatewayRouteName: str,
         meshName: str,
-        spec: GatewayRouteSpecUnionTypeDef,
+        spec: GatewayRouteSpecTypeDef,
         virtualGatewayName: str,
         clientToken: str = ...,
         meshOwner: str = ...
     ) -> UpdateGatewayRouteOutputTypeDef:
         """
         Updates an existing gateway route that is associated to a specified virtual
         gateway in a service mesh.
@@ -552,15 +552,15 @@
         """
 
     async def update_route(
         self,
         *,
         meshName: str,
         routeName: str,
-        spec: RouteSpecUnionTypeDef,
+        spec: RouteSpecTypeDef,
         virtualRouterName: str,
         clientToken: str = ...,
         meshOwner: str = ...
     ) -> UpdateRouteOutputTypeDef:
         """
         Updates an existing route for a specified service mesh and virtual router.
 
@@ -568,15 +568,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#update_route)
         """
 
     async def update_virtual_gateway(
         self,
         *,
         meshName: str,
-        spec: VirtualGatewaySpecUnionTypeDef,
+        spec: VirtualGatewaySpecTypeDef,
         virtualGatewayName: str,
         clientToken: str = ...,
         meshOwner: str = ...
     ) -> UpdateVirtualGatewayOutputTypeDef:
         """
         Updates an existing virtual gateway in a specified service mesh.
 
@@ -584,15 +584,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#update_virtual_gateway)
         """
 
     async def update_virtual_node(
         self,
         *,
         meshName: str,
-        spec: VirtualNodeSpecUnionTypeDef,
+        spec: VirtualNodeSpecTypeDef,
         virtualNodeName: str,
         clientToken: str = ...,
         meshOwner: str = ...
     ) -> UpdateVirtualNodeOutputTypeDef:
         """
         Updates an existing virtual node in a specified service mesh.
 
@@ -600,15 +600,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#update_virtual_node)
         """
 
     async def update_virtual_router(
         self,
         *,
         meshName: str,
-        spec: VirtualRouterSpecUnionTypeDef,
+        spec: VirtualRouterSpecTypeDef,
         virtualRouterName: str,
         clientToken: str = ...,
         meshOwner: str = ...
     ) -> UpdateVirtualRouterOutputTypeDef:
         """
         Updates an existing virtual router in a specified service mesh.
```

### Comparing `types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh/client.pyi` & `types-aiobotocore-appmesh-2.5.2.post2/types_aiobotocore_appmesh/client.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -48,36 +48,36 @@
     DescribeGatewayRouteOutputTypeDef,
     DescribeMeshOutputTypeDef,
     DescribeRouteOutputTypeDef,
     DescribeVirtualGatewayOutputTypeDef,
     DescribeVirtualNodeOutputTypeDef,
     DescribeVirtualRouterOutputTypeDef,
     DescribeVirtualServiceOutputTypeDef,
-    GatewayRouteSpecUnionTypeDef,
+    GatewayRouteSpecTypeDef,
     ListGatewayRoutesOutputTypeDef,
     ListMeshesOutputTypeDef,
     ListRoutesOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     ListVirtualGatewaysOutputTypeDef,
     ListVirtualNodesOutputTypeDef,
     ListVirtualRoutersOutputTypeDef,
     ListVirtualServicesOutputTypeDef,
     MeshSpecTypeDef,
-    RouteSpecUnionTypeDef,
+    RouteSpecTypeDef,
     TagRefTypeDef,
     UpdateGatewayRouteOutputTypeDef,
     UpdateMeshOutputTypeDef,
     UpdateRouteOutputTypeDef,
     UpdateVirtualGatewayOutputTypeDef,
     UpdateVirtualNodeOutputTypeDef,
     UpdateVirtualRouterOutputTypeDef,
     UpdateVirtualServiceOutputTypeDef,
-    VirtualGatewaySpecUnionTypeDef,
-    VirtualNodeSpecUnionTypeDef,
-    VirtualRouterSpecUnionTypeDef,
+    VirtualGatewaySpecTypeDef,
+    VirtualNodeSpecTypeDef,
+    VirtualRouterSpecTypeDef,
     VirtualServiceSpecTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -135,15 +135,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#close)
         """
     async def create_gateway_route(
         self,
         *,
         gatewayRouteName: str,
         meshName: str,
-        spec: GatewayRouteSpecUnionTypeDef,
+        spec: GatewayRouteSpecTypeDef,
         virtualGatewayName: str,
         clientToken: str = ...,
         meshOwner: str = ...,
         tags: Sequence[TagRefTypeDef] = ...
     ) -> CreateGatewayRouteOutputTypeDef:
         """
         Creates a gateway route.
@@ -166,15 +166,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#create_mesh)
         """
     async def create_route(
         self,
         *,
         meshName: str,
         routeName: str,
-        spec: RouteSpecUnionTypeDef,
+        spec: RouteSpecTypeDef,
         virtualRouterName: str,
         clientToken: str = ...,
         meshOwner: str = ...,
         tags: Sequence[TagRefTypeDef] = ...
     ) -> CreateRouteOutputTypeDef:
         """
         Creates a route that is associated with a virtual router.
@@ -182,15 +182,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.create_route)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#create_route)
         """
     async def create_virtual_gateway(
         self,
         *,
         meshName: str,
-        spec: VirtualGatewaySpecUnionTypeDef,
+        spec: VirtualGatewaySpecTypeDef,
         virtualGatewayName: str,
         clientToken: str = ...,
         meshOwner: str = ...,
         tags: Sequence[TagRefTypeDef] = ...
     ) -> CreateVirtualGatewayOutputTypeDef:
         """
         Creates a virtual gateway.
@@ -198,15 +198,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.create_virtual_gateway)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#create_virtual_gateway)
         """
     async def create_virtual_node(
         self,
         *,
         meshName: str,
-        spec: VirtualNodeSpecUnionTypeDef,
+        spec: VirtualNodeSpecTypeDef,
         virtualNodeName: str,
         clientToken: str = ...,
         meshOwner: str = ...,
         tags: Sequence[TagRefTypeDef] = ...
     ) -> CreateVirtualNodeOutputTypeDef:
         """
         Creates a virtual node within a service mesh.
@@ -214,15 +214,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.create_virtual_node)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#create_virtual_node)
         """
     async def create_virtual_router(
         self,
         *,
         meshName: str,
-        spec: VirtualRouterSpecUnionTypeDef,
+        spec: VirtualRouterSpecTypeDef,
         virtualRouterName: str,
         clientToken: str = ...,
         meshOwner: str = ...,
         tags: Sequence[TagRefTypeDef] = ...
     ) -> CreateVirtualRouterOutputTypeDef:
         """
         Creates a virtual router within a service mesh.
@@ -485,15 +485,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#untag_resource)
         """
     async def update_gateway_route(
         self,
         *,
         gatewayRouteName: str,
         meshName: str,
-        spec: GatewayRouteSpecUnionTypeDef,
+        spec: GatewayRouteSpecTypeDef,
         virtualGatewayName: str,
         clientToken: str = ...,
         meshOwner: str = ...
     ) -> UpdateGatewayRouteOutputTypeDef:
         """
         Updates an existing gateway route that is associated to a specified virtual
         gateway in a service mesh.
@@ -511,60 +511,60 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#update_mesh)
         """
     async def update_route(
         self,
         *,
         meshName: str,
         routeName: str,
-        spec: RouteSpecUnionTypeDef,
+        spec: RouteSpecTypeDef,
         virtualRouterName: str,
         clientToken: str = ...,
         meshOwner: str = ...
     ) -> UpdateRouteOutputTypeDef:
         """
         Updates an existing route for a specified service mesh and virtual router.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.update_route)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#update_route)
         """
     async def update_virtual_gateway(
         self,
         *,
         meshName: str,
-        spec: VirtualGatewaySpecUnionTypeDef,
+        spec: VirtualGatewaySpecTypeDef,
         virtualGatewayName: str,
         clientToken: str = ...,
         meshOwner: str = ...
     ) -> UpdateVirtualGatewayOutputTypeDef:
         """
         Updates an existing virtual gateway in a specified service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.update_virtual_gateway)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#update_virtual_gateway)
         """
     async def update_virtual_node(
         self,
         *,
         meshName: str,
-        spec: VirtualNodeSpecUnionTypeDef,
+        spec: VirtualNodeSpecTypeDef,
         virtualNodeName: str,
         clientToken: str = ...,
         meshOwner: str = ...
     ) -> UpdateVirtualNodeOutputTypeDef:
         """
         Updates an existing virtual node in a specified service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.update_virtual_node)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#update_virtual_node)
         """
     async def update_virtual_router(
         self,
         *,
         meshName: str,
-        spec: VirtualRouterSpecUnionTypeDef,
+        spec: VirtualRouterSpecTypeDef,
         virtualRouterName: str,
         clientToken: str = ...,
         meshOwner: str = ...
     ) -> UpdateVirtualRouterOutputTypeDef:
         """
         Updates an existing virtual router in a specified service mesh.
```

### Comparing `types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh/literals.py` & `types-aiobotocore-appmesh-2.5.2.post2/types_aiobotocore_appmesh/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh/literals.pyi` & `types-aiobotocore-appmesh-2.5.2.post2/types_aiobotocore_appmesh/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh/paginator.py` & `types-aiobotocore-appmesh-2.5.2.post2/types_aiobotocore_appmesh/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh/paginator.pyi` & `types-aiobotocore-appmesh-2.5.2.post2/types_aiobotocore_appmesh/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh/type_defs.py` & `types-aiobotocore-appmesh-2.5.2.post2/types_aiobotocore_appmesh/type_defs.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_appmesh.type_defs import AwsCloudMapInstanceAttributeTypeDef
 
     data: AwsCloudMapInstanceAttributeTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Sequence
 
 from .literals import (
     DefaultGatewayRouteRewriteType,
     DnsResponseTypeType,
     DurationUnitType,
     EgressFilterTypeType,
     GatewayRouteStatusCodeType,
@@ -95,77 +95,67 @@
     "VirtualGatewayRefTypeDef",
     "ListVirtualNodesInputRequestTypeDef",
     "VirtualNodeRefTypeDef",
     "ListVirtualRoutersInputRequestTypeDef",
     "VirtualRouterRefTypeDef",
     "ListVirtualServicesInputRequestTypeDef",
     "VirtualServiceRefTypeDef",
-    "PortMappingTypeDef",
     "ListenerTlsAcmCertificateTypeDef",
     "TlsValidationContextFileTrustTypeDef",
     "TlsValidationContextSdsTrustTypeDef",
+    "PortMappingTypeDef",
     "MeshStatusTypeDef",
     "MeshServiceDiscoveryTypeDef",
     "RouteStatusTypeDef",
-    "SubjectAlternativeNameMatchersOutputTypeDef",
     "SubjectAlternativeNameMatchersTypeDef",
     "TcpRouteMatchTypeDef",
-    "TlsValidationContextAcmTrustOutputTypeDef",
     "TlsValidationContextAcmTrustTypeDef",
     "UntagResourceInputRequestTypeDef",
     "VirtualGatewayListenerTlsFileCertificateTypeDef",
     "VirtualGatewayListenerTlsSdsCertificateTypeDef",
     "VirtualGatewayGrpcConnectionPoolTypeDef",
     "VirtualGatewayHttp2ConnectionPoolTypeDef",
     "VirtualGatewayHttpConnectionPoolTypeDef",
     "VirtualGatewayStatusTypeDef",
     "VirtualGatewayHealthCheckPolicyTypeDef",
-    "VirtualGatewayPortMappingTypeDef",
     "VirtualGatewayListenerTlsAcmCertificateTypeDef",
     "VirtualGatewayTlsValidationContextFileTrustTypeDef",
     "VirtualGatewayTlsValidationContextSdsTrustTypeDef",
-    "VirtualGatewayTlsValidationContextAcmTrustOutputTypeDef",
+    "VirtualGatewayPortMappingTypeDef",
     "VirtualGatewayTlsValidationContextAcmTrustTypeDef",
     "VirtualNodeGrpcConnectionPoolTypeDef",
     "VirtualNodeHttp2ConnectionPoolTypeDef",
     "VirtualNodeHttpConnectionPoolTypeDef",
     "VirtualNodeTcpConnectionPoolTypeDef",
     "VirtualNodeStatusTypeDef",
     "VirtualNodeServiceProviderTypeDef",
     "VirtualRouterStatusTypeDef",
     "VirtualRouterServiceProviderTypeDef",
     "VirtualServiceStatusTypeDef",
-    "AwsCloudMapServiceDiscoveryOutputTypeDef",
     "AwsCloudMapServiceDiscoveryTypeDef",
     "ClientTlsCertificateTypeDef",
     "TagResourceInputRequestTypeDef",
     "ListTagsForResourceOutputTypeDef",
-    "GrpcRetryPolicyOutputTypeDef",
     "GrpcRetryPolicyTypeDef",
     "GrpcTimeoutTypeDef",
-    "HttpRetryPolicyOutputTypeDef",
     "HttpRetryPolicyTypeDef",
     "HttpTimeoutTypeDef",
     "OutlierDetectionTypeDef",
     "TcpTimeoutTypeDef",
     "GrpcGatewayRouteRewriteTypeDef",
     "ListGatewayRoutesOutputTypeDef",
     "GatewayRouteTargetTypeDef",
     "GrpcMetadataMatchMethodTypeDef",
     "GrpcRouteMetadataMatchMethodTypeDef",
     "HeaderMatchMethodTypeDef",
-    "GrpcRouteActionOutputTypeDef",
     "GrpcRouteActionTypeDef",
-    "HttpRouteActionOutputTypeDef",
     "HttpRouteActionTypeDef",
-    "TcpRouteActionOutputTypeDef",
     "TcpRouteActionTypeDef",
     "HttpGatewayRouteRewriteTypeDef",
     "HttpQueryParameterTypeDef",
-    "LoggingFormatOutputTypeDef",
     "LoggingFormatTypeDef",
     "ListGatewayRoutesInputListGatewayRoutesPaginateTypeDef",
     "ListMeshesInputListMeshesPaginateTypeDef",
     "ListRoutesInputListRoutesPaginateTypeDef",
     "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
     "ListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef",
     "ListVirtualNodesInputListVirtualNodesPaginateTypeDef",
@@ -173,158 +163,113 @@
     "ListVirtualServicesInputListVirtualServicesPaginateTypeDef",
     "ListMeshesOutputTypeDef",
     "ListRoutesOutputTypeDef",
     "ListVirtualGatewaysOutputTypeDef",
     "ListVirtualNodesOutputTypeDef",
     "ListVirtualRoutersOutputTypeDef",
     "ListVirtualServicesOutputTypeDef",
-    "VirtualRouterListenerTypeDef",
     "ListenerTlsCertificateTypeDef",
     "ListenerTlsValidationContextTrustTypeDef",
+    "VirtualRouterListenerTypeDef",
     "MeshSpecTypeDef",
-    "SubjectAlternativeNamesOutputTypeDef",
     "SubjectAlternativeNamesTypeDef",
-    "TlsValidationContextTrustOutputTypeDef",
     "TlsValidationContextTrustTypeDef",
     "VirtualGatewayClientTlsCertificateTypeDef",
     "VirtualGatewayConnectionPoolTypeDef",
     "VirtualGatewayListenerTlsCertificateTypeDef",
     "VirtualGatewayListenerTlsValidationContextTrustTypeDef",
-    "VirtualGatewayTlsValidationContextTrustOutputTypeDef",
     "VirtualGatewayTlsValidationContextTrustTypeDef",
     "VirtualNodeConnectionPoolTypeDef",
     "VirtualServiceProviderTypeDef",
-    "ServiceDiscoveryOutputTypeDef",
     "ServiceDiscoveryTypeDef",
     "ListenerTimeoutTypeDef",
     "GrpcGatewayRouteActionTypeDef",
     "GrpcGatewayRouteMetadataTypeDef",
     "GrpcRouteMetadataTypeDef",
     "HttpGatewayRouteHeaderTypeDef",
     "HttpRouteHeaderTypeDef",
-    "TcpRouteOutputTypeDef",
     "TcpRouteTypeDef",
     "HttpGatewayRouteActionTypeDef",
-    "FileAccessLogOutputTypeDef",
-    "VirtualGatewayFileAccessLogOutputTypeDef",
     "FileAccessLogTypeDef",
     "VirtualGatewayFileAccessLogTypeDef",
-    "VirtualRouterSpecOutputTypeDef",
     "VirtualRouterSpecTypeDef",
     "CreateMeshInputRequestTypeDef",
     "MeshDataTypeDef",
     "UpdateMeshInputRequestTypeDef",
-    "ListenerTlsValidationContextOutputTypeDef",
     "ListenerTlsValidationContextTypeDef",
-    "TlsValidationContextOutputTypeDef",
     "TlsValidationContextTypeDef",
-    "VirtualGatewayListenerTlsValidationContextOutputTypeDef",
     "VirtualGatewayListenerTlsValidationContextTypeDef",
-    "VirtualGatewayTlsValidationContextOutputTypeDef",
     "VirtualGatewayTlsValidationContextTypeDef",
     "VirtualServiceSpecTypeDef",
-    "GrpcGatewayRouteMatchOutputTypeDef",
     "GrpcGatewayRouteMatchTypeDef",
-    "GrpcRouteMatchOutputTypeDef",
     "GrpcRouteMatchTypeDef",
-    "HttpGatewayRouteMatchOutputTypeDef",
     "HttpGatewayRouteMatchTypeDef",
-    "HttpRouteMatchOutputTypeDef",
     "HttpRouteMatchTypeDef",
-    "AccessLogOutputTypeDef",
-    "VirtualGatewayAccessLogOutputTypeDef",
     "AccessLogTypeDef",
     "VirtualGatewayAccessLogTypeDef",
-    "VirtualRouterDataTypeDef",
     "CreateVirtualRouterInputRequestTypeDef",
     "UpdateVirtualRouterInputRequestTypeDef",
-    "VirtualRouterSpecUnionTypeDef",
+    "VirtualRouterDataTypeDef",
     "CreateMeshOutputTypeDef",
     "DeleteMeshOutputTypeDef",
     "DescribeMeshOutputTypeDef",
     "UpdateMeshOutputTypeDef",
-    "ListenerTlsOutputTypeDef",
     "ListenerTlsTypeDef",
-    "ClientPolicyTlsOutputTypeDef",
     "ClientPolicyTlsTypeDef",
-    "VirtualGatewayListenerTlsOutputTypeDef",
     "VirtualGatewayListenerTlsTypeDef",
-    "VirtualGatewayClientPolicyTlsOutputTypeDef",
     "VirtualGatewayClientPolicyTlsTypeDef",
     "CreateVirtualServiceInputRequestTypeDef",
     "UpdateVirtualServiceInputRequestTypeDef",
     "VirtualServiceDataTypeDef",
-    "GrpcGatewayRouteOutputTypeDef",
     "GrpcGatewayRouteTypeDef",
-    "GrpcRouteOutputTypeDef",
     "GrpcRouteTypeDef",
-    "HttpGatewayRouteOutputTypeDef",
     "HttpGatewayRouteTypeDef",
-    "HttpRouteOutputTypeDef",
     "HttpRouteTypeDef",
-    "LoggingOutputTypeDef",
-    "VirtualGatewayLoggingOutputTypeDef",
     "LoggingTypeDef",
     "VirtualGatewayLoggingTypeDef",
     "CreateVirtualRouterOutputTypeDef",
     "DeleteVirtualRouterOutputTypeDef",
     "DescribeVirtualRouterOutputTypeDef",
     "UpdateVirtualRouterOutputTypeDef",
-    "ListenerOutputTypeDef",
     "ListenerTypeDef",
-    "ClientPolicyOutputTypeDef",
     "ClientPolicyTypeDef",
-    "VirtualGatewayListenerOutputTypeDef",
     "VirtualGatewayListenerTypeDef",
-    "VirtualGatewayClientPolicyOutputTypeDef",
     "VirtualGatewayClientPolicyTypeDef",
     "CreateVirtualServiceOutputTypeDef",
     "DeleteVirtualServiceOutputTypeDef",
     "DescribeVirtualServiceOutputTypeDef",
     "UpdateVirtualServiceOutputTypeDef",
-    "GatewayRouteSpecOutputTypeDef",
     "GatewayRouteSpecTypeDef",
-    "RouteSpecOutputTypeDef",
     "RouteSpecTypeDef",
-    "BackendDefaultsOutputTypeDef",
-    "VirtualServiceBackendOutputTypeDef",
     "BackendDefaultsTypeDef",
     "VirtualServiceBackendTypeDef",
-    "VirtualGatewayBackendDefaultsOutputTypeDef",
     "VirtualGatewayBackendDefaultsTypeDef",
-    "GatewayRouteDataTypeDef",
     "CreateGatewayRouteInputRequestTypeDef",
-    "GatewayRouteSpecUnionTypeDef",
+    "GatewayRouteDataTypeDef",
     "UpdateGatewayRouteInputRequestTypeDef",
-    "RouteDataTypeDef",
     "CreateRouteInputRequestTypeDef",
-    "RouteSpecUnionTypeDef",
+    "RouteDataTypeDef",
     "UpdateRouteInputRequestTypeDef",
-    "BackendOutputTypeDef",
     "BackendTypeDef",
-    "VirtualGatewaySpecOutputTypeDef",
     "VirtualGatewaySpecTypeDef",
     "CreateGatewayRouteOutputTypeDef",
     "DeleteGatewayRouteOutputTypeDef",
     "DescribeGatewayRouteOutputTypeDef",
     "UpdateGatewayRouteOutputTypeDef",
     "CreateRouteOutputTypeDef",
     "DeleteRouteOutputTypeDef",
     "DescribeRouteOutputTypeDef",
     "UpdateRouteOutputTypeDef",
-    "VirtualNodeSpecOutputTypeDef",
     "VirtualNodeSpecTypeDef",
-    "VirtualGatewayDataTypeDef",
     "CreateVirtualGatewayInputRequestTypeDef",
     "UpdateVirtualGatewayInputRequestTypeDef",
-    "VirtualGatewaySpecUnionTypeDef",
-    "VirtualNodeDataTypeDef",
+    "VirtualGatewayDataTypeDef",
     "CreateVirtualNodeInputRequestTypeDef",
     "UpdateVirtualNodeInputRequestTypeDef",
-    "VirtualNodeSpecUnionTypeDef",
+    "VirtualNodeDataTypeDef",
     "CreateVirtualGatewayOutputTypeDef",
     "DeleteVirtualGatewayOutputTypeDef",
     "DescribeVirtualGatewayOutputTypeDef",
     "UpdateVirtualGatewayOutputTypeDef",
     "CreateVirtualNodeOutputTypeDef",
     "DeleteVirtualNodeOutputTypeDef",
     "DescribeVirtualNodeOutputTypeDef",
@@ -1129,22 +1074,14 @@
         "meshOwner": str,
         "resourceOwner": str,
         "version": int,
         "virtualServiceName": str,
     },
 )
 
-PortMappingTypeDef = TypedDict(
-    "PortMappingTypeDef",
-    {
-        "port": int,
-        "protocol": PortProtocolType,
-    },
-)
-
 ListenerTlsAcmCertificateTypeDef = TypedDict(
     "ListenerTlsAcmCertificateTypeDef",
     {
         "certificateArn": str,
     },
 )
 
@@ -1158,14 +1095,22 @@
 TlsValidationContextSdsTrustTypeDef = TypedDict(
     "TlsValidationContextSdsTrustTypeDef",
     {
         "secretName": str,
     },
 )
 
+PortMappingTypeDef = TypedDict(
+    "PortMappingTypeDef",
+    {
+        "port": int,
+        "protocol": PortProtocolType,
+    },
+)
+
 MeshStatusTypeDef = TypedDict(
     "MeshStatusTypeDef",
     {
         "status": MeshStatusCodeType,
     },
     total=False,
 )
@@ -1181,21 +1126,14 @@
 RouteStatusTypeDef = TypedDict(
     "RouteStatusTypeDef",
     {
         "status": RouteStatusCodeType,
     },
 )
 
-SubjectAlternativeNameMatchersOutputTypeDef = TypedDict(
-    "SubjectAlternativeNameMatchersOutputTypeDef",
-    {
-        "exact": List[str],
-    },
-)
-
 SubjectAlternativeNameMatchersTypeDef = TypedDict(
     "SubjectAlternativeNameMatchersTypeDef",
     {
         "exact": Sequence[str],
     },
 )
 
@@ -1203,21 +1141,14 @@
     "TcpRouteMatchTypeDef",
     {
         "port": int,
     },
     total=False,
 )
 
-TlsValidationContextAcmTrustOutputTypeDef = TypedDict(
-    "TlsValidationContextAcmTrustOutputTypeDef",
-    {
-        "certificateAuthorityArns": List[str],
-    },
-)
-
 TlsValidationContextAcmTrustTypeDef = TypedDict(
     "TlsValidationContextAcmTrustTypeDef",
     {
         "certificateAuthorityArns": Sequence[str],
     },
 )
 
@@ -1309,22 +1240,14 @@
 
 class VirtualGatewayHealthCheckPolicyTypeDef(
     _RequiredVirtualGatewayHealthCheckPolicyTypeDef, _OptionalVirtualGatewayHealthCheckPolicyTypeDef
 ):
     pass
 
 
-VirtualGatewayPortMappingTypeDef = TypedDict(
-    "VirtualGatewayPortMappingTypeDef",
-    {
-        "port": int,
-        "protocol": VirtualGatewayPortProtocolType,
-    },
-)
-
 VirtualGatewayListenerTlsAcmCertificateTypeDef = TypedDict(
     "VirtualGatewayListenerTlsAcmCertificateTypeDef",
     {
         "certificateArn": str,
     },
 )
 
@@ -1338,18 +1261,19 @@
 VirtualGatewayTlsValidationContextSdsTrustTypeDef = TypedDict(
     "VirtualGatewayTlsValidationContextSdsTrustTypeDef",
     {
         "secretName": str,
     },
 )
 
-VirtualGatewayTlsValidationContextAcmTrustOutputTypeDef = TypedDict(
-    "VirtualGatewayTlsValidationContextAcmTrustOutputTypeDef",
+VirtualGatewayPortMappingTypeDef = TypedDict(
+    "VirtualGatewayPortMappingTypeDef",
     {
-        "certificateAuthorityArns": List[str],
+        "port": int,
+        "protocol": VirtualGatewayPortProtocolType,
     },
 )
 
 VirtualGatewayTlsValidationContextAcmTrustTypeDef = TypedDict(
     "VirtualGatewayTlsValidationContextAcmTrustTypeDef",
     {
         "certificateAuthorityArns": Sequence[str],
@@ -1429,38 +1353,14 @@
 VirtualServiceStatusTypeDef = TypedDict(
     "VirtualServiceStatusTypeDef",
     {
         "status": VirtualServiceStatusCodeType,
     },
 )
 
-_RequiredAwsCloudMapServiceDiscoveryOutputTypeDef = TypedDict(
-    "_RequiredAwsCloudMapServiceDiscoveryOutputTypeDef",
-    {
-        "namespaceName": str,
-        "serviceName": str,
-    },
-)
-_OptionalAwsCloudMapServiceDiscoveryOutputTypeDef = TypedDict(
-    "_OptionalAwsCloudMapServiceDiscoveryOutputTypeDef",
-    {
-        "attributes": List[AwsCloudMapInstanceAttributeTypeDef],
-        "ipPreference": IpPreferenceType,
-    },
-    total=False,
-)
-
-
-class AwsCloudMapServiceDiscoveryOutputTypeDef(
-    _RequiredAwsCloudMapServiceDiscoveryOutputTypeDef,
-    _OptionalAwsCloudMapServiceDiscoveryOutputTypeDef,
-):
-    pass
-
-
 _RequiredAwsCloudMapServiceDiscoveryTypeDef = TypedDict(
     "_RequiredAwsCloudMapServiceDiscoveryTypeDef",
     {
         "namespaceName": str,
         "serviceName": str,
     },
 )
@@ -1502,38 +1402,14 @@
     {
         "nextToken": str,
         "tags": List[TagRefTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredGrpcRetryPolicyOutputTypeDef = TypedDict(
-    "_RequiredGrpcRetryPolicyOutputTypeDef",
-    {
-        "maxRetries": int,
-        "perRetryTimeout": DurationTypeDef,
-    },
-)
-_OptionalGrpcRetryPolicyOutputTypeDef = TypedDict(
-    "_OptionalGrpcRetryPolicyOutputTypeDef",
-    {
-        "grpcRetryEvents": List[GrpcRetryPolicyEventType],
-        "httpRetryEvents": List[str],
-        "tcpRetryEvents": List[Literal["connection-error"]],
-    },
-    total=False,
-)
-
-
-class GrpcRetryPolicyOutputTypeDef(
-    _RequiredGrpcRetryPolicyOutputTypeDef, _OptionalGrpcRetryPolicyOutputTypeDef
-):
-    pass
-
-
 _RequiredGrpcRetryPolicyTypeDef = TypedDict(
     "_RequiredGrpcRetryPolicyTypeDef",
     {
         "maxRetries": int,
         "perRetryTimeout": DurationTypeDef,
     },
 )
@@ -1557,37 +1433,14 @@
     {
         "idle": DurationTypeDef,
         "perRequest": DurationTypeDef,
     },
     total=False,
 )
 
-_RequiredHttpRetryPolicyOutputTypeDef = TypedDict(
-    "_RequiredHttpRetryPolicyOutputTypeDef",
-    {
-        "maxRetries": int,
-        "perRetryTimeout": DurationTypeDef,
-    },
-)
-_OptionalHttpRetryPolicyOutputTypeDef = TypedDict(
-    "_OptionalHttpRetryPolicyOutputTypeDef",
-    {
-        "httpRetryEvents": List[str],
-        "tcpRetryEvents": List[Literal["connection-error"]],
-    },
-    total=False,
-)
-
-
-class HttpRetryPolicyOutputTypeDef(
-    _RequiredHttpRetryPolicyOutputTypeDef, _OptionalHttpRetryPolicyOutputTypeDef
-):
-    pass
-
-
 _RequiredHttpRetryPolicyTypeDef = TypedDict(
     "_RequiredHttpRetryPolicyTypeDef",
     {
         "maxRetries": int,
         "perRetryTimeout": DurationTypeDef,
     },
 )
@@ -1702,49 +1555,28 @@
         "range": MatchRangeTypeDef,
         "regex": str,
         "suffix": str,
     },
     total=False,
 )
 
-GrpcRouteActionOutputTypeDef = TypedDict(
-    "GrpcRouteActionOutputTypeDef",
-    {
-        "weightedTargets": List[WeightedTargetTypeDef],
-    },
-)
-
 GrpcRouteActionTypeDef = TypedDict(
     "GrpcRouteActionTypeDef",
     {
         "weightedTargets": Sequence[WeightedTargetTypeDef],
     },
 )
 
-HttpRouteActionOutputTypeDef = TypedDict(
-    "HttpRouteActionOutputTypeDef",
-    {
-        "weightedTargets": List[WeightedTargetTypeDef],
-    },
-)
-
 HttpRouteActionTypeDef = TypedDict(
     "HttpRouteActionTypeDef",
     {
         "weightedTargets": Sequence[WeightedTargetTypeDef],
     },
 )
 
-TcpRouteActionOutputTypeDef = TypedDict(
-    "TcpRouteActionOutputTypeDef",
-    {
-        "weightedTargets": List[WeightedTargetTypeDef],
-    },
-)
-
 TcpRouteActionTypeDef = TypedDict(
     "TcpRouteActionTypeDef",
     {
         "weightedTargets": Sequence[WeightedTargetTypeDef],
     },
 )
 
@@ -1775,23 +1607,14 @@
 
 class HttpQueryParameterTypeDef(
     _RequiredHttpQueryParameterTypeDef, _OptionalHttpQueryParameterTypeDef
 ):
     pass
 
 
-LoggingFormatOutputTypeDef = TypedDict(
-    "LoggingFormatOutputTypeDef",
-    {
-        "json": List[JsonFormatRefTypeDef],
-        "text": str,
-    },
-    total=False,
-)
-
 LoggingFormatTypeDef = TypedDict(
     "LoggingFormatTypeDef",
     {
         "json": Sequence[JsonFormatRefTypeDef],
         "text": str,
     },
     total=False,
@@ -2017,21 +1840,14 @@
     {
         "nextToken": str,
         "virtualServices": List[VirtualServiceRefTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-VirtualRouterListenerTypeDef = TypedDict(
-    "VirtualRouterListenerTypeDef",
-    {
-        "portMapping": PortMappingTypeDef,
-    },
-)
-
 ListenerTlsCertificateTypeDef = TypedDict(
     "ListenerTlsCertificateTypeDef",
     {
         "acm": ListenerTlsAcmCertificateTypeDef,
         "file": ListenerTlsFileCertificateTypeDef,
         "sds": ListenerTlsSdsCertificateTypeDef,
     },
@@ -2043,47 +1859,37 @@
     {
         "file": TlsValidationContextFileTrustTypeDef,
         "sds": TlsValidationContextSdsTrustTypeDef,
     },
     total=False,
 )
 
+VirtualRouterListenerTypeDef = TypedDict(
+    "VirtualRouterListenerTypeDef",
+    {
+        "portMapping": PortMappingTypeDef,
+    },
+)
+
 MeshSpecTypeDef = TypedDict(
     "MeshSpecTypeDef",
     {
         "egressFilter": EgressFilterTypeDef,
         "serviceDiscovery": MeshServiceDiscoveryTypeDef,
     },
     total=False,
 )
 
-SubjectAlternativeNamesOutputTypeDef = TypedDict(
-    "SubjectAlternativeNamesOutputTypeDef",
-    {
-        "match": SubjectAlternativeNameMatchersOutputTypeDef,
-    },
-)
-
 SubjectAlternativeNamesTypeDef = TypedDict(
     "SubjectAlternativeNamesTypeDef",
     {
         "match": SubjectAlternativeNameMatchersTypeDef,
     },
 )
 
-TlsValidationContextTrustOutputTypeDef = TypedDict(
-    "TlsValidationContextTrustOutputTypeDef",
-    {
-        "acm": TlsValidationContextAcmTrustOutputTypeDef,
-        "file": TlsValidationContextFileTrustTypeDef,
-        "sds": TlsValidationContextSdsTrustTypeDef,
-    },
-    total=False,
-)
-
 TlsValidationContextTrustTypeDef = TypedDict(
     "TlsValidationContextTrustTypeDef",
     {
         "acm": TlsValidationContextAcmTrustTypeDef,
         "file": TlsValidationContextFileTrustTypeDef,
         "sds": TlsValidationContextSdsTrustTypeDef,
     },
@@ -2124,24 +1930,14 @@
     {
         "file": VirtualGatewayTlsValidationContextFileTrustTypeDef,
         "sds": VirtualGatewayTlsValidationContextSdsTrustTypeDef,
     },
     total=False,
 )
 
-VirtualGatewayTlsValidationContextTrustOutputTypeDef = TypedDict(
-    "VirtualGatewayTlsValidationContextTrustOutputTypeDef",
-    {
-        "acm": VirtualGatewayTlsValidationContextAcmTrustOutputTypeDef,
-        "file": VirtualGatewayTlsValidationContextFileTrustTypeDef,
-        "sds": VirtualGatewayTlsValidationContextSdsTrustTypeDef,
-    },
-    total=False,
-)
-
 VirtualGatewayTlsValidationContextTrustTypeDef = TypedDict(
     "VirtualGatewayTlsValidationContextTrustTypeDef",
     {
         "acm": VirtualGatewayTlsValidationContextAcmTrustTypeDef,
         "file": VirtualGatewayTlsValidationContextFileTrustTypeDef,
         "sds": VirtualGatewayTlsValidationContextSdsTrustTypeDef,
     },
@@ -2164,23 +1960,14 @@
     {
         "virtualNode": VirtualNodeServiceProviderTypeDef,
         "virtualRouter": VirtualRouterServiceProviderTypeDef,
     },
     total=False,
 )
 
-ServiceDiscoveryOutputTypeDef = TypedDict(
-    "ServiceDiscoveryOutputTypeDef",
-    {
-        "awsCloudMap": AwsCloudMapServiceDiscoveryOutputTypeDef,
-        "dns": DnsServiceDiscoveryTypeDef,
-    },
-    total=False,
-)
-
 ServiceDiscoveryTypeDef = TypedDict(
     "ServiceDiscoveryTypeDef",
     {
         "awsCloudMap": AwsCloudMapServiceDiscoveryTypeDef,
         "dns": DnsServiceDiscoveryTypeDef,
     },
     total=False,
@@ -2300,34 +2087,14 @@
 )
 
 
 class HttpRouteHeaderTypeDef(_RequiredHttpRouteHeaderTypeDef, _OptionalHttpRouteHeaderTypeDef):
     pass
 
 
-_RequiredTcpRouteOutputTypeDef = TypedDict(
-    "_RequiredTcpRouteOutputTypeDef",
-    {
-        "action": TcpRouteActionOutputTypeDef,
-    },
-)
-_OptionalTcpRouteOutputTypeDef = TypedDict(
-    "_OptionalTcpRouteOutputTypeDef",
-    {
-        "match": TcpRouteMatchTypeDef,
-        "timeout": TcpTimeoutTypeDef,
-    },
-    total=False,
-)
-
-
-class TcpRouteOutputTypeDef(_RequiredTcpRouteOutputTypeDef, _OptionalTcpRouteOutputTypeDef):
-    pass
-
-
 _RequiredTcpRouteTypeDef = TypedDict(
     "_RequiredTcpRouteTypeDef",
     {
         "action": TcpRouteActionTypeDef,
     },
 )
 _OptionalTcpRouteTypeDef = TypedDict(
@@ -2361,57 +2128,14 @@
 
 class HttpGatewayRouteActionTypeDef(
     _RequiredHttpGatewayRouteActionTypeDef, _OptionalHttpGatewayRouteActionTypeDef
 ):
     pass
 
 
-_RequiredFileAccessLogOutputTypeDef = TypedDict(
-    "_RequiredFileAccessLogOutputTypeDef",
-    {
-        "path": str,
-    },
-)
-_OptionalFileAccessLogOutputTypeDef = TypedDict(
-    "_OptionalFileAccessLogOutputTypeDef",
-    {
-        "format": LoggingFormatOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class FileAccessLogOutputTypeDef(
-    _RequiredFileAccessLogOutputTypeDef, _OptionalFileAccessLogOutputTypeDef
-):
-    pass
-
-
-_RequiredVirtualGatewayFileAccessLogOutputTypeDef = TypedDict(
-    "_RequiredVirtualGatewayFileAccessLogOutputTypeDef",
-    {
-        "path": str,
-    },
-)
-_OptionalVirtualGatewayFileAccessLogOutputTypeDef = TypedDict(
-    "_OptionalVirtualGatewayFileAccessLogOutputTypeDef",
-    {
-        "format": LoggingFormatOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class VirtualGatewayFileAccessLogOutputTypeDef(
-    _RequiredVirtualGatewayFileAccessLogOutputTypeDef,
-    _OptionalVirtualGatewayFileAccessLogOutputTypeDef,
-):
-    pass
-
-
 _RequiredFileAccessLogTypeDef = TypedDict(
     "_RequiredFileAccessLogTypeDef",
     {
         "path": str,
     },
 )
 _OptionalFileAccessLogTypeDef = TypedDict(
@@ -2444,22 +2168,14 @@
 
 class VirtualGatewayFileAccessLogTypeDef(
     _RequiredVirtualGatewayFileAccessLogTypeDef, _OptionalVirtualGatewayFileAccessLogTypeDef
 ):
     pass
 
 
-VirtualRouterSpecOutputTypeDef = TypedDict(
-    "VirtualRouterSpecOutputTypeDef",
-    {
-        "listeners": List[VirtualRouterListenerTypeDef],
-    },
-    total=False,
-)
-
 VirtualRouterSpecTypeDef = TypedDict(
     "VirtualRouterSpecTypeDef",
     {
         "listeners": Sequence[VirtualRouterListenerTypeDef],
     },
     total=False,
 )
@@ -2515,36 +2231,14 @@
 
 class UpdateMeshInputRequestTypeDef(
     _RequiredUpdateMeshInputRequestTypeDef, _OptionalUpdateMeshInputRequestTypeDef
 ):
     pass
 
 
-_RequiredListenerTlsValidationContextOutputTypeDef = TypedDict(
-    "_RequiredListenerTlsValidationContextOutputTypeDef",
-    {
-        "trust": ListenerTlsValidationContextTrustTypeDef,
-    },
-)
-_OptionalListenerTlsValidationContextOutputTypeDef = TypedDict(
-    "_OptionalListenerTlsValidationContextOutputTypeDef",
-    {
-        "subjectAlternativeNames": SubjectAlternativeNamesOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class ListenerTlsValidationContextOutputTypeDef(
-    _RequiredListenerTlsValidationContextOutputTypeDef,
-    _OptionalListenerTlsValidationContextOutputTypeDef,
-):
-    pass
-
-
 _RequiredListenerTlsValidationContextTypeDef = TypedDict(
     "_RequiredListenerTlsValidationContextTypeDef",
     {
         "trust": ListenerTlsValidationContextTrustTypeDef,
     },
 )
 _OptionalListenerTlsValidationContextTypeDef = TypedDict(
@@ -2558,35 +2252,14 @@
 
 class ListenerTlsValidationContextTypeDef(
     _RequiredListenerTlsValidationContextTypeDef, _OptionalListenerTlsValidationContextTypeDef
 ):
     pass
 
 
-_RequiredTlsValidationContextOutputTypeDef = TypedDict(
-    "_RequiredTlsValidationContextOutputTypeDef",
-    {
-        "trust": TlsValidationContextTrustOutputTypeDef,
-    },
-)
-_OptionalTlsValidationContextOutputTypeDef = TypedDict(
-    "_OptionalTlsValidationContextOutputTypeDef",
-    {
-        "subjectAlternativeNames": SubjectAlternativeNamesOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class TlsValidationContextOutputTypeDef(
-    _RequiredTlsValidationContextOutputTypeDef, _OptionalTlsValidationContextOutputTypeDef
-):
-    pass
-
-
 _RequiredTlsValidationContextTypeDef = TypedDict(
     "_RequiredTlsValidationContextTypeDef",
     {
         "trust": TlsValidationContextTrustTypeDef,
     },
 )
 _OptionalTlsValidationContextTypeDef = TypedDict(
@@ -2600,36 +2273,14 @@
 
 class TlsValidationContextTypeDef(
     _RequiredTlsValidationContextTypeDef, _OptionalTlsValidationContextTypeDef
 ):
     pass
 
 
-_RequiredVirtualGatewayListenerTlsValidationContextOutputTypeDef = TypedDict(
-    "_RequiredVirtualGatewayListenerTlsValidationContextOutputTypeDef",
-    {
-        "trust": VirtualGatewayListenerTlsValidationContextTrustTypeDef,
-    },
-)
-_OptionalVirtualGatewayListenerTlsValidationContextOutputTypeDef = TypedDict(
-    "_OptionalVirtualGatewayListenerTlsValidationContextOutputTypeDef",
-    {
-        "subjectAlternativeNames": SubjectAlternativeNamesOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class VirtualGatewayListenerTlsValidationContextOutputTypeDef(
-    _RequiredVirtualGatewayListenerTlsValidationContextOutputTypeDef,
-    _OptionalVirtualGatewayListenerTlsValidationContextOutputTypeDef,
-):
-    pass
-
-
 _RequiredVirtualGatewayListenerTlsValidationContextTypeDef = TypedDict(
     "_RequiredVirtualGatewayListenerTlsValidationContextTypeDef",
     {
         "trust": VirtualGatewayListenerTlsValidationContextTrustTypeDef,
     },
 )
 _OptionalVirtualGatewayListenerTlsValidationContextTypeDef = TypedDict(
@@ -2644,36 +2295,14 @@
 class VirtualGatewayListenerTlsValidationContextTypeDef(
     _RequiredVirtualGatewayListenerTlsValidationContextTypeDef,
     _OptionalVirtualGatewayListenerTlsValidationContextTypeDef,
 ):
     pass
 
 
-_RequiredVirtualGatewayTlsValidationContextOutputTypeDef = TypedDict(
-    "_RequiredVirtualGatewayTlsValidationContextOutputTypeDef",
-    {
-        "trust": VirtualGatewayTlsValidationContextTrustOutputTypeDef,
-    },
-)
-_OptionalVirtualGatewayTlsValidationContextOutputTypeDef = TypedDict(
-    "_OptionalVirtualGatewayTlsValidationContextOutputTypeDef",
-    {
-        "subjectAlternativeNames": SubjectAlternativeNamesOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class VirtualGatewayTlsValidationContextOutputTypeDef(
-    _RequiredVirtualGatewayTlsValidationContextOutputTypeDef,
-    _OptionalVirtualGatewayTlsValidationContextOutputTypeDef,
-):
-    pass
-
-
 _RequiredVirtualGatewayTlsValidationContextTypeDef = TypedDict(
     "_RequiredVirtualGatewayTlsValidationContextTypeDef",
     {
         "trust": VirtualGatewayTlsValidationContextTrustTypeDef,
     },
 )
 _OptionalVirtualGatewayTlsValidationContextTypeDef = TypedDict(
@@ -2696,130 +2325,64 @@
     "VirtualServiceSpecTypeDef",
     {
         "provider": VirtualServiceProviderTypeDef,
     },
     total=False,
 )
 
-GrpcGatewayRouteMatchOutputTypeDef = TypedDict(
-    "GrpcGatewayRouteMatchOutputTypeDef",
-    {
-        "hostname": GatewayRouteHostnameMatchTypeDef,
-        "metadata": List[GrpcGatewayRouteMetadataTypeDef],
-        "port": int,
-        "serviceName": str,
-    },
-    total=False,
-)
-
 GrpcGatewayRouteMatchTypeDef = TypedDict(
     "GrpcGatewayRouteMatchTypeDef",
     {
         "hostname": GatewayRouteHostnameMatchTypeDef,
         "metadata": Sequence[GrpcGatewayRouteMetadataTypeDef],
         "port": int,
         "serviceName": str,
     },
     total=False,
 )
 
-GrpcRouteMatchOutputTypeDef = TypedDict(
-    "GrpcRouteMatchOutputTypeDef",
-    {
-        "metadata": List[GrpcRouteMetadataTypeDef],
-        "methodName": str,
-        "port": int,
-        "serviceName": str,
-    },
-    total=False,
-)
-
 GrpcRouteMatchTypeDef = TypedDict(
     "GrpcRouteMatchTypeDef",
     {
         "metadata": Sequence[GrpcRouteMetadataTypeDef],
         "methodName": str,
         "port": int,
         "serviceName": str,
     },
     total=False,
 )
 
-HttpGatewayRouteMatchOutputTypeDef = TypedDict(
-    "HttpGatewayRouteMatchOutputTypeDef",
-    {
-        "headers": List[HttpGatewayRouteHeaderTypeDef],
-        "hostname": GatewayRouteHostnameMatchTypeDef,
-        "method": HttpMethodType,
-        "path": HttpPathMatchTypeDef,
-        "port": int,
-        "prefix": str,
-        "queryParameters": List[HttpQueryParameterTypeDef],
-    },
-    total=False,
-)
-
 HttpGatewayRouteMatchTypeDef = TypedDict(
     "HttpGatewayRouteMatchTypeDef",
     {
         "headers": Sequence[HttpGatewayRouteHeaderTypeDef],
         "hostname": GatewayRouteHostnameMatchTypeDef,
         "method": HttpMethodType,
         "path": HttpPathMatchTypeDef,
         "port": int,
         "prefix": str,
         "queryParameters": Sequence[HttpQueryParameterTypeDef],
     },
     total=False,
 )
 
-HttpRouteMatchOutputTypeDef = TypedDict(
-    "HttpRouteMatchOutputTypeDef",
-    {
-        "headers": List[HttpRouteHeaderTypeDef],
-        "method": HttpMethodType,
-        "path": HttpPathMatchTypeDef,
-        "port": int,
-        "prefix": str,
-        "queryParameters": List[HttpQueryParameterTypeDef],
-        "scheme": HttpSchemeType,
-    },
-    total=False,
-)
-
 HttpRouteMatchTypeDef = TypedDict(
     "HttpRouteMatchTypeDef",
     {
         "headers": Sequence[HttpRouteHeaderTypeDef],
         "method": HttpMethodType,
         "path": HttpPathMatchTypeDef,
         "port": int,
         "prefix": str,
         "queryParameters": Sequence[HttpQueryParameterTypeDef],
         "scheme": HttpSchemeType,
     },
     total=False,
 )
 
-AccessLogOutputTypeDef = TypedDict(
-    "AccessLogOutputTypeDef",
-    {
-        "file": FileAccessLogOutputTypeDef,
-    },
-    total=False,
-)
-
-VirtualGatewayAccessLogOutputTypeDef = TypedDict(
-    "VirtualGatewayAccessLogOutputTypeDef",
-    {
-        "file": VirtualGatewayFileAccessLogOutputTypeDef,
-    },
-    total=False,
-)
-
 AccessLogTypeDef = TypedDict(
     "AccessLogTypeDef",
     {
         "file": FileAccessLogTypeDef,
     },
     total=False,
 )
@@ -2828,25 +2391,14 @@
     "VirtualGatewayAccessLogTypeDef",
     {
         "file": VirtualGatewayFileAccessLogTypeDef,
     },
     total=False,
 )
 
-VirtualRouterDataTypeDef = TypedDict(
-    "VirtualRouterDataTypeDef",
-    {
-        "meshName": str,
-        "metadata": ResourceMetadataTypeDef,
-        "spec": VirtualRouterSpecOutputTypeDef,
-        "status": VirtualRouterStatusTypeDef,
-        "virtualRouterName": str,
-    },
-)
-
 _RequiredCreateVirtualRouterInputRequestTypeDef = TypedDict(
     "_RequiredCreateVirtualRouterInputRequestTypeDef",
     {
         "meshName": str,
         "spec": VirtualRouterSpecTypeDef,
         "virtualRouterName": str,
     },
@@ -2888,15 +2440,25 @@
 
 class UpdateVirtualRouterInputRequestTypeDef(
     _RequiredUpdateVirtualRouterInputRequestTypeDef, _OptionalUpdateVirtualRouterInputRequestTypeDef
 ):
     pass
 
 
-VirtualRouterSpecUnionTypeDef = Union[VirtualRouterSpecTypeDef, VirtualRouterSpecOutputTypeDef]
+VirtualRouterDataTypeDef = TypedDict(
+    "VirtualRouterDataTypeDef",
+    {
+        "meshName": str,
+        "metadata": ResourceMetadataTypeDef,
+        "spec": VirtualRouterSpecTypeDef,
+        "status": VirtualRouterStatusTypeDef,
+        "virtualRouterName": str,
+    },
+)
+
 CreateMeshOutputTypeDef = TypedDict(
     "CreateMeshOutputTypeDef",
     {
         "mesh": MeshDataTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2921,36 +2483,14 @@
     "UpdateMeshOutputTypeDef",
     {
         "mesh": MeshDataTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredListenerTlsOutputTypeDef = TypedDict(
-    "_RequiredListenerTlsOutputTypeDef",
-    {
-        "certificate": ListenerTlsCertificateTypeDef,
-        "mode": ListenerTlsModeType,
-    },
-)
-_OptionalListenerTlsOutputTypeDef = TypedDict(
-    "_OptionalListenerTlsOutputTypeDef",
-    {
-        "validation": ListenerTlsValidationContextOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class ListenerTlsOutputTypeDef(
-    _RequiredListenerTlsOutputTypeDef, _OptionalListenerTlsOutputTypeDef
-):
-    pass
-
-
 _RequiredListenerTlsTypeDef = TypedDict(
     "_RequiredListenerTlsTypeDef",
     {
         "certificate": ListenerTlsCertificateTypeDef,
         "mode": ListenerTlsModeType,
     },
 )
@@ -2963,37 +2503,14 @@
 )
 
 
 class ListenerTlsTypeDef(_RequiredListenerTlsTypeDef, _OptionalListenerTlsTypeDef):
     pass
 
 
-_RequiredClientPolicyTlsOutputTypeDef = TypedDict(
-    "_RequiredClientPolicyTlsOutputTypeDef",
-    {
-        "validation": TlsValidationContextOutputTypeDef,
-    },
-)
-_OptionalClientPolicyTlsOutputTypeDef = TypedDict(
-    "_OptionalClientPolicyTlsOutputTypeDef",
-    {
-        "certificate": ClientTlsCertificateTypeDef,
-        "enforce": bool,
-        "ports": List[int],
-    },
-    total=False,
-)
-
-
-class ClientPolicyTlsOutputTypeDef(
-    _RequiredClientPolicyTlsOutputTypeDef, _OptionalClientPolicyTlsOutputTypeDef
-):
-    pass
-
-
 _RequiredClientPolicyTlsTypeDef = TypedDict(
     "_RequiredClientPolicyTlsTypeDef",
     {
         "validation": TlsValidationContextTypeDef,
     },
 )
 _OptionalClientPolicyTlsTypeDef = TypedDict(
@@ -3007,36 +2524,14 @@
 )
 
 
 class ClientPolicyTlsTypeDef(_RequiredClientPolicyTlsTypeDef, _OptionalClientPolicyTlsTypeDef):
     pass
 
 
-_RequiredVirtualGatewayListenerTlsOutputTypeDef = TypedDict(
-    "_RequiredVirtualGatewayListenerTlsOutputTypeDef",
-    {
-        "certificate": VirtualGatewayListenerTlsCertificateTypeDef,
-        "mode": VirtualGatewayListenerTlsModeType,
-    },
-)
-_OptionalVirtualGatewayListenerTlsOutputTypeDef = TypedDict(
-    "_OptionalVirtualGatewayListenerTlsOutputTypeDef",
-    {
-        "validation": VirtualGatewayListenerTlsValidationContextOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class VirtualGatewayListenerTlsOutputTypeDef(
-    _RequiredVirtualGatewayListenerTlsOutputTypeDef, _OptionalVirtualGatewayListenerTlsOutputTypeDef
-):
-    pass
-
-
 _RequiredVirtualGatewayListenerTlsTypeDef = TypedDict(
     "_RequiredVirtualGatewayListenerTlsTypeDef",
     {
         "certificate": VirtualGatewayListenerTlsCertificateTypeDef,
         "mode": VirtualGatewayListenerTlsModeType,
     },
 )
@@ -3051,38 +2546,14 @@
 
 class VirtualGatewayListenerTlsTypeDef(
     _RequiredVirtualGatewayListenerTlsTypeDef, _OptionalVirtualGatewayListenerTlsTypeDef
 ):
     pass
 
 
-_RequiredVirtualGatewayClientPolicyTlsOutputTypeDef = TypedDict(
-    "_RequiredVirtualGatewayClientPolicyTlsOutputTypeDef",
-    {
-        "validation": VirtualGatewayTlsValidationContextOutputTypeDef,
-    },
-)
-_OptionalVirtualGatewayClientPolicyTlsOutputTypeDef = TypedDict(
-    "_OptionalVirtualGatewayClientPolicyTlsOutputTypeDef",
-    {
-        "certificate": VirtualGatewayClientTlsCertificateTypeDef,
-        "enforce": bool,
-        "ports": List[int],
-    },
-    total=False,
-)
-
-
-class VirtualGatewayClientPolicyTlsOutputTypeDef(
-    _RequiredVirtualGatewayClientPolicyTlsOutputTypeDef,
-    _OptionalVirtualGatewayClientPolicyTlsOutputTypeDef,
-):
-    pass
-
-
 _RequiredVirtualGatewayClientPolicyTlsTypeDef = TypedDict(
     "_RequiredVirtualGatewayClientPolicyTlsTypeDef",
     {
         "validation": VirtualGatewayTlsValidationContextTypeDef,
     },
 )
 _OptionalVirtualGatewayClientPolicyTlsTypeDef = TypedDict(
@@ -3160,51 +2631,22 @@
         "metadata": ResourceMetadataTypeDef,
         "spec": VirtualServiceSpecTypeDef,
         "status": VirtualServiceStatusTypeDef,
         "virtualServiceName": str,
     },
 )
 
-GrpcGatewayRouteOutputTypeDef = TypedDict(
-    "GrpcGatewayRouteOutputTypeDef",
-    {
-        "action": GrpcGatewayRouteActionTypeDef,
-        "match": GrpcGatewayRouteMatchOutputTypeDef,
-    },
-)
-
 GrpcGatewayRouteTypeDef = TypedDict(
     "GrpcGatewayRouteTypeDef",
     {
         "action": GrpcGatewayRouteActionTypeDef,
         "match": GrpcGatewayRouteMatchTypeDef,
     },
 )
 
-_RequiredGrpcRouteOutputTypeDef = TypedDict(
-    "_RequiredGrpcRouteOutputTypeDef",
-    {
-        "action": GrpcRouteActionOutputTypeDef,
-        "match": GrpcRouteMatchOutputTypeDef,
-    },
-)
-_OptionalGrpcRouteOutputTypeDef = TypedDict(
-    "_OptionalGrpcRouteOutputTypeDef",
-    {
-        "retryPolicy": GrpcRetryPolicyOutputTypeDef,
-        "timeout": GrpcTimeoutTypeDef,
-    },
-    total=False,
-)
-
-
-class GrpcRouteOutputTypeDef(_RequiredGrpcRouteOutputTypeDef, _OptionalGrpcRouteOutputTypeDef):
-    pass
-
-
 _RequiredGrpcRouteTypeDef = TypedDict(
     "_RequiredGrpcRouteTypeDef",
     {
         "action": GrpcRouteActionTypeDef,
         "match": GrpcRouteMatchTypeDef,
     },
 )
@@ -3218,51 +2660,22 @@
 )
 
 
 class GrpcRouteTypeDef(_RequiredGrpcRouteTypeDef, _OptionalGrpcRouteTypeDef):
     pass
 
 
-HttpGatewayRouteOutputTypeDef = TypedDict(
-    "HttpGatewayRouteOutputTypeDef",
-    {
-        "action": HttpGatewayRouteActionTypeDef,
-        "match": HttpGatewayRouteMatchOutputTypeDef,
-    },
-)
-
 HttpGatewayRouteTypeDef = TypedDict(
     "HttpGatewayRouteTypeDef",
     {
         "action": HttpGatewayRouteActionTypeDef,
         "match": HttpGatewayRouteMatchTypeDef,
     },
 )
 
-_RequiredHttpRouteOutputTypeDef = TypedDict(
-    "_RequiredHttpRouteOutputTypeDef",
-    {
-        "action": HttpRouteActionOutputTypeDef,
-        "match": HttpRouteMatchOutputTypeDef,
-    },
-)
-_OptionalHttpRouteOutputTypeDef = TypedDict(
-    "_OptionalHttpRouteOutputTypeDef",
-    {
-        "retryPolicy": HttpRetryPolicyOutputTypeDef,
-        "timeout": HttpTimeoutTypeDef,
-    },
-    total=False,
-)
-
-
-class HttpRouteOutputTypeDef(_RequiredHttpRouteOutputTypeDef, _OptionalHttpRouteOutputTypeDef):
-    pass
-
-
 _RequiredHttpRouteTypeDef = TypedDict(
     "_RequiredHttpRouteTypeDef",
     {
         "action": HttpRouteActionTypeDef,
         "match": HttpRouteMatchTypeDef,
     },
 )
@@ -3276,30 +2689,14 @@
 )
 
 
 class HttpRouteTypeDef(_RequiredHttpRouteTypeDef, _OptionalHttpRouteTypeDef):
     pass
 
 
-LoggingOutputTypeDef = TypedDict(
-    "LoggingOutputTypeDef",
-    {
-        "accessLog": AccessLogOutputTypeDef,
-    },
-    total=False,
-)
-
-VirtualGatewayLoggingOutputTypeDef = TypedDict(
-    "VirtualGatewayLoggingOutputTypeDef",
-    {
-        "accessLog": VirtualGatewayAccessLogOutputTypeDef,
-    },
-    total=False,
-)
-
 LoggingTypeDef = TypedDict(
     "LoggingTypeDef",
     {
         "accessLog": AccessLogTypeDef,
     },
     total=False,
 )
@@ -3340,37 +2737,14 @@
     "UpdateVirtualRouterOutputTypeDef",
     {
         "virtualRouter": VirtualRouterDataTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredListenerOutputTypeDef = TypedDict(
-    "_RequiredListenerOutputTypeDef",
-    {
-        "portMapping": PortMappingTypeDef,
-    },
-)
-_OptionalListenerOutputTypeDef = TypedDict(
-    "_OptionalListenerOutputTypeDef",
-    {
-        "connectionPool": VirtualNodeConnectionPoolTypeDef,
-        "healthCheck": HealthCheckPolicyTypeDef,
-        "outlierDetection": OutlierDetectionTypeDef,
-        "timeout": ListenerTimeoutTypeDef,
-        "tls": ListenerTlsOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class ListenerOutputTypeDef(_RequiredListenerOutputTypeDef, _OptionalListenerOutputTypeDef):
-    pass
-
-
 _RequiredListenerTypeDef = TypedDict(
     "_RequiredListenerTypeDef",
     {
         "portMapping": PortMappingTypeDef,
     },
 )
 _OptionalListenerTypeDef = TypedDict(
@@ -3386,53 +2760,22 @@
 )
 
 
 class ListenerTypeDef(_RequiredListenerTypeDef, _OptionalListenerTypeDef):
     pass
 
 
-ClientPolicyOutputTypeDef = TypedDict(
-    "ClientPolicyOutputTypeDef",
-    {
-        "tls": ClientPolicyTlsOutputTypeDef,
-    },
-    total=False,
-)
-
 ClientPolicyTypeDef = TypedDict(
     "ClientPolicyTypeDef",
     {
         "tls": ClientPolicyTlsTypeDef,
     },
     total=False,
 )
 
-_RequiredVirtualGatewayListenerOutputTypeDef = TypedDict(
-    "_RequiredVirtualGatewayListenerOutputTypeDef",
-    {
-        "portMapping": VirtualGatewayPortMappingTypeDef,
-    },
-)
-_OptionalVirtualGatewayListenerOutputTypeDef = TypedDict(
-    "_OptionalVirtualGatewayListenerOutputTypeDef",
-    {
-        "connectionPool": VirtualGatewayConnectionPoolTypeDef,
-        "healthCheck": VirtualGatewayHealthCheckPolicyTypeDef,
-        "tls": VirtualGatewayListenerTlsOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class VirtualGatewayListenerOutputTypeDef(
-    _RequiredVirtualGatewayListenerOutputTypeDef, _OptionalVirtualGatewayListenerOutputTypeDef
-):
-    pass
-
-
 _RequiredVirtualGatewayListenerTypeDef = TypedDict(
     "_RequiredVirtualGatewayListenerTypeDef",
     {
         "portMapping": VirtualGatewayPortMappingTypeDef,
     },
 )
 _OptionalVirtualGatewayListenerTypeDef = TypedDict(
@@ -3448,22 +2791,14 @@
 
 class VirtualGatewayListenerTypeDef(
     _RequiredVirtualGatewayListenerTypeDef, _OptionalVirtualGatewayListenerTypeDef
 ):
     pass
 
 
-VirtualGatewayClientPolicyOutputTypeDef = TypedDict(
-    "VirtualGatewayClientPolicyOutputTypeDef",
-    {
-        "tls": VirtualGatewayClientPolicyTlsOutputTypeDef,
-    },
-    total=False,
-)
-
 VirtualGatewayClientPolicyTypeDef = TypedDict(
     "VirtualGatewayClientPolicyTypeDef",
     {
         "tls": VirtualGatewayClientPolicyTlsTypeDef,
     },
     total=False,
 )
@@ -3496,89 +2831,37 @@
     "UpdateVirtualServiceOutputTypeDef",
     {
         "virtualService": VirtualServiceDataTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GatewayRouteSpecOutputTypeDef = TypedDict(
-    "GatewayRouteSpecOutputTypeDef",
-    {
-        "grpcRoute": GrpcGatewayRouteOutputTypeDef,
-        "http2Route": HttpGatewayRouteOutputTypeDef,
-        "httpRoute": HttpGatewayRouteOutputTypeDef,
-        "priority": int,
-    },
-    total=False,
-)
-
 GatewayRouteSpecTypeDef = TypedDict(
     "GatewayRouteSpecTypeDef",
     {
         "grpcRoute": GrpcGatewayRouteTypeDef,
         "http2Route": HttpGatewayRouteTypeDef,
         "httpRoute": HttpGatewayRouteTypeDef,
         "priority": int,
     },
     total=False,
 )
 
-RouteSpecOutputTypeDef = TypedDict(
-    "RouteSpecOutputTypeDef",
-    {
-        "grpcRoute": GrpcRouteOutputTypeDef,
-        "http2Route": HttpRouteOutputTypeDef,
-        "httpRoute": HttpRouteOutputTypeDef,
-        "priority": int,
-        "tcpRoute": TcpRouteOutputTypeDef,
-    },
-    total=False,
-)
-
 RouteSpecTypeDef = TypedDict(
     "RouteSpecTypeDef",
     {
         "grpcRoute": GrpcRouteTypeDef,
         "http2Route": HttpRouteTypeDef,
         "httpRoute": HttpRouteTypeDef,
         "priority": int,
         "tcpRoute": TcpRouteTypeDef,
     },
     total=False,
 )
 
-BackendDefaultsOutputTypeDef = TypedDict(
-    "BackendDefaultsOutputTypeDef",
-    {
-        "clientPolicy": ClientPolicyOutputTypeDef,
-    },
-    total=False,
-)
-
-_RequiredVirtualServiceBackendOutputTypeDef = TypedDict(
-    "_RequiredVirtualServiceBackendOutputTypeDef",
-    {
-        "virtualServiceName": str,
-    },
-)
-_OptionalVirtualServiceBackendOutputTypeDef = TypedDict(
-    "_OptionalVirtualServiceBackendOutputTypeDef",
-    {
-        "clientPolicy": ClientPolicyOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class VirtualServiceBackendOutputTypeDef(
-    _RequiredVirtualServiceBackendOutputTypeDef, _OptionalVirtualServiceBackendOutputTypeDef
-):
-    pass
-
-
 BackendDefaultsTypeDef = TypedDict(
     "BackendDefaultsTypeDef",
     {
         "clientPolicy": ClientPolicyTypeDef,
     },
     total=False,
 )
@@ -3600,42 +2883,22 @@
 
 class VirtualServiceBackendTypeDef(
     _RequiredVirtualServiceBackendTypeDef, _OptionalVirtualServiceBackendTypeDef
 ):
     pass
 
 
-VirtualGatewayBackendDefaultsOutputTypeDef = TypedDict(
-    "VirtualGatewayBackendDefaultsOutputTypeDef",
-    {
-        "clientPolicy": VirtualGatewayClientPolicyOutputTypeDef,
-    },
-    total=False,
-)
-
 VirtualGatewayBackendDefaultsTypeDef = TypedDict(
     "VirtualGatewayBackendDefaultsTypeDef",
     {
         "clientPolicy": VirtualGatewayClientPolicyTypeDef,
     },
     total=False,
 )
 
-GatewayRouteDataTypeDef = TypedDict(
-    "GatewayRouteDataTypeDef",
-    {
-        "gatewayRouteName": str,
-        "meshName": str,
-        "metadata": ResourceMetadataTypeDef,
-        "spec": GatewayRouteSpecOutputTypeDef,
-        "status": GatewayRouteStatusTypeDef,
-        "virtualGatewayName": str,
-    },
-)
-
 _RequiredCreateGatewayRouteInputRequestTypeDef = TypedDict(
     "_RequiredCreateGatewayRouteInputRequestTypeDef",
     {
         "gatewayRouteName": str,
         "meshName": str,
         "spec": GatewayRouteSpecTypeDef,
         "virtualGatewayName": str,
@@ -3654,15 +2917,26 @@
 
 class CreateGatewayRouteInputRequestTypeDef(
     _RequiredCreateGatewayRouteInputRequestTypeDef, _OptionalCreateGatewayRouteInputRequestTypeDef
 ):
     pass
 
 
-GatewayRouteSpecUnionTypeDef = Union[GatewayRouteSpecTypeDef, GatewayRouteSpecOutputTypeDef]
+GatewayRouteDataTypeDef = TypedDict(
+    "GatewayRouteDataTypeDef",
+    {
+        "gatewayRouteName": str,
+        "meshName": str,
+        "metadata": ResourceMetadataTypeDef,
+        "spec": GatewayRouteSpecTypeDef,
+        "status": GatewayRouteStatusTypeDef,
+        "virtualGatewayName": str,
+    },
+)
+
 _RequiredUpdateGatewayRouteInputRequestTypeDef = TypedDict(
     "_RequiredUpdateGatewayRouteInputRequestTypeDef",
     {
         "gatewayRouteName": str,
         "meshName": str,
         "spec": GatewayRouteSpecTypeDef,
         "virtualGatewayName": str,
@@ -3680,26 +2954,14 @@
 
 class UpdateGatewayRouteInputRequestTypeDef(
     _RequiredUpdateGatewayRouteInputRequestTypeDef, _OptionalUpdateGatewayRouteInputRequestTypeDef
 ):
     pass
 
 
-RouteDataTypeDef = TypedDict(
-    "RouteDataTypeDef",
-    {
-        "meshName": str,
-        "metadata": ResourceMetadataTypeDef,
-        "routeName": str,
-        "spec": RouteSpecOutputTypeDef,
-        "status": RouteStatusTypeDef,
-        "virtualRouterName": str,
-    },
-)
-
 _RequiredCreateRouteInputRequestTypeDef = TypedDict(
     "_RequiredCreateRouteInputRequestTypeDef",
     {
         "meshName": str,
         "routeName": str,
         "spec": RouteSpecTypeDef,
         "virtualRouterName": str,
@@ -3718,15 +2980,26 @@
 
 class CreateRouteInputRequestTypeDef(
     _RequiredCreateRouteInputRequestTypeDef, _OptionalCreateRouteInputRequestTypeDef
 ):
     pass
 
 
-RouteSpecUnionTypeDef = Union[RouteSpecTypeDef, RouteSpecOutputTypeDef]
+RouteDataTypeDef = TypedDict(
+    "RouteDataTypeDef",
+    {
+        "meshName": str,
+        "metadata": ResourceMetadataTypeDef,
+        "routeName": str,
+        "spec": RouteSpecTypeDef,
+        "status": RouteStatusTypeDef,
+        "virtualRouterName": str,
+    },
+)
+
 _RequiredUpdateRouteInputRequestTypeDef = TypedDict(
     "_RequiredUpdateRouteInputRequestTypeDef",
     {
         "meshName": str,
         "routeName": str,
         "spec": RouteSpecTypeDef,
         "virtualRouterName": str,
@@ -3744,52 +3017,22 @@
 
 class UpdateRouteInputRequestTypeDef(
     _RequiredUpdateRouteInputRequestTypeDef, _OptionalUpdateRouteInputRequestTypeDef
 ):
     pass
 
 
-BackendOutputTypeDef = TypedDict(
-    "BackendOutputTypeDef",
-    {
-        "virtualService": VirtualServiceBackendOutputTypeDef,
-    },
-    total=False,
-)
-
 BackendTypeDef = TypedDict(
     "BackendTypeDef",
     {
         "virtualService": VirtualServiceBackendTypeDef,
     },
     total=False,
 )
 
-_RequiredVirtualGatewaySpecOutputTypeDef = TypedDict(
-    "_RequiredVirtualGatewaySpecOutputTypeDef",
-    {
-        "listeners": List[VirtualGatewayListenerOutputTypeDef],
-    },
-)
-_OptionalVirtualGatewaySpecOutputTypeDef = TypedDict(
-    "_OptionalVirtualGatewaySpecOutputTypeDef",
-    {
-        "backendDefaults": VirtualGatewayBackendDefaultsOutputTypeDef,
-        "logging": VirtualGatewayLoggingOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class VirtualGatewaySpecOutputTypeDef(
-    _RequiredVirtualGatewaySpecOutputTypeDef, _OptionalVirtualGatewaySpecOutputTypeDef
-):
-    pass
-
-
 _RequiredVirtualGatewaySpecTypeDef = TypedDict(
     "_RequiredVirtualGatewaySpecTypeDef",
     {
         "listeners": Sequence[VirtualGatewayListenerTypeDef],
     },
 )
 _OptionalVirtualGatewaySpecTypeDef = TypedDict(
@@ -3868,49 +3111,26 @@
     "UpdateRouteOutputTypeDef",
     {
         "route": RouteDataTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-VirtualNodeSpecOutputTypeDef = TypedDict(
-    "VirtualNodeSpecOutputTypeDef",
-    {
-        "backendDefaults": BackendDefaultsOutputTypeDef,
-        "backends": List[BackendOutputTypeDef],
-        "listeners": List[ListenerOutputTypeDef],
-        "logging": LoggingOutputTypeDef,
-        "serviceDiscovery": ServiceDiscoveryOutputTypeDef,
-    },
-    total=False,
-)
-
 VirtualNodeSpecTypeDef = TypedDict(
     "VirtualNodeSpecTypeDef",
     {
         "backendDefaults": BackendDefaultsTypeDef,
         "backends": Sequence[BackendTypeDef],
         "listeners": Sequence[ListenerTypeDef],
         "logging": LoggingTypeDef,
         "serviceDiscovery": ServiceDiscoveryTypeDef,
     },
     total=False,
 )
 
-VirtualGatewayDataTypeDef = TypedDict(
-    "VirtualGatewayDataTypeDef",
-    {
-        "meshName": str,
-        "metadata": ResourceMetadataTypeDef,
-        "spec": VirtualGatewaySpecOutputTypeDef,
-        "status": VirtualGatewayStatusTypeDef,
-        "virtualGatewayName": str,
-    },
-)
-
 _RequiredCreateVirtualGatewayInputRequestTypeDef = TypedDict(
     "_RequiredCreateVirtualGatewayInputRequestTypeDef",
     {
         "meshName": str,
         "spec": VirtualGatewaySpecTypeDef,
         "virtualGatewayName": str,
     },
@@ -3954,23 +3174,22 @@
 class UpdateVirtualGatewayInputRequestTypeDef(
     _RequiredUpdateVirtualGatewayInputRequestTypeDef,
     _OptionalUpdateVirtualGatewayInputRequestTypeDef,
 ):
     pass
 
 
-VirtualGatewaySpecUnionTypeDef = Union[VirtualGatewaySpecTypeDef, VirtualGatewaySpecOutputTypeDef]
-VirtualNodeDataTypeDef = TypedDict(
-    "VirtualNodeDataTypeDef",
+VirtualGatewayDataTypeDef = TypedDict(
+    "VirtualGatewayDataTypeDef",
     {
         "meshName": str,
         "metadata": ResourceMetadataTypeDef,
-        "spec": VirtualNodeSpecOutputTypeDef,
-        "status": VirtualNodeStatusTypeDef,
-        "virtualNodeName": str,
+        "spec": VirtualGatewaySpecTypeDef,
+        "status": VirtualGatewayStatusTypeDef,
+        "virtualGatewayName": str,
     },
 )
 
 _RequiredCreateVirtualNodeInputRequestTypeDef = TypedDict(
     "_RequiredCreateVirtualNodeInputRequestTypeDef",
     {
         "meshName": str,
@@ -4015,15 +3234,25 @@
 
 class UpdateVirtualNodeInputRequestTypeDef(
     _RequiredUpdateVirtualNodeInputRequestTypeDef, _OptionalUpdateVirtualNodeInputRequestTypeDef
 ):
     pass
 
 
-VirtualNodeSpecUnionTypeDef = Union[VirtualNodeSpecTypeDef, VirtualNodeSpecOutputTypeDef]
+VirtualNodeDataTypeDef = TypedDict(
+    "VirtualNodeDataTypeDef",
+    {
+        "meshName": str,
+        "metadata": ResourceMetadataTypeDef,
+        "spec": VirtualNodeSpecTypeDef,
+        "status": VirtualNodeStatusTypeDef,
+        "virtualNodeName": str,
+    },
+)
+
 CreateVirtualGatewayOutputTypeDef = TypedDict(
     "CreateVirtualGatewayOutputTypeDef",
     {
         "virtualGateway": VirtualGatewayDataTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh/type_defs.pyi` & `types-aiobotocore-appmesh-2.5.2.post2/types_aiobotocore_appmesh/type_defs.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_appmesh.type_defs import AwsCloudMapInstanceAttributeTypeDef
 
     data: AwsCloudMapInstanceAttributeTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Sequence
 
 from .literals import (
     DefaultGatewayRouteRewriteType,
     DnsResponseTypeType,
     DurationUnitType,
     EgressFilterTypeType,
     GatewayRouteStatusCodeType,
@@ -94,77 +94,67 @@
     "VirtualGatewayRefTypeDef",
     "ListVirtualNodesInputRequestTypeDef",
     "VirtualNodeRefTypeDef",
     "ListVirtualRoutersInputRequestTypeDef",
     "VirtualRouterRefTypeDef",
     "ListVirtualServicesInputRequestTypeDef",
     "VirtualServiceRefTypeDef",
-    "PortMappingTypeDef",
     "ListenerTlsAcmCertificateTypeDef",
     "TlsValidationContextFileTrustTypeDef",
     "TlsValidationContextSdsTrustTypeDef",
+    "PortMappingTypeDef",
     "MeshStatusTypeDef",
     "MeshServiceDiscoveryTypeDef",
     "RouteStatusTypeDef",
-    "SubjectAlternativeNameMatchersOutputTypeDef",
     "SubjectAlternativeNameMatchersTypeDef",
     "TcpRouteMatchTypeDef",
-    "TlsValidationContextAcmTrustOutputTypeDef",
     "TlsValidationContextAcmTrustTypeDef",
     "UntagResourceInputRequestTypeDef",
     "VirtualGatewayListenerTlsFileCertificateTypeDef",
     "VirtualGatewayListenerTlsSdsCertificateTypeDef",
     "VirtualGatewayGrpcConnectionPoolTypeDef",
     "VirtualGatewayHttp2ConnectionPoolTypeDef",
     "VirtualGatewayHttpConnectionPoolTypeDef",
     "VirtualGatewayStatusTypeDef",
     "VirtualGatewayHealthCheckPolicyTypeDef",
-    "VirtualGatewayPortMappingTypeDef",
     "VirtualGatewayListenerTlsAcmCertificateTypeDef",
     "VirtualGatewayTlsValidationContextFileTrustTypeDef",
     "VirtualGatewayTlsValidationContextSdsTrustTypeDef",
-    "VirtualGatewayTlsValidationContextAcmTrustOutputTypeDef",
+    "VirtualGatewayPortMappingTypeDef",
     "VirtualGatewayTlsValidationContextAcmTrustTypeDef",
     "VirtualNodeGrpcConnectionPoolTypeDef",
     "VirtualNodeHttp2ConnectionPoolTypeDef",
     "VirtualNodeHttpConnectionPoolTypeDef",
     "VirtualNodeTcpConnectionPoolTypeDef",
     "VirtualNodeStatusTypeDef",
     "VirtualNodeServiceProviderTypeDef",
     "VirtualRouterStatusTypeDef",
     "VirtualRouterServiceProviderTypeDef",
     "VirtualServiceStatusTypeDef",
-    "AwsCloudMapServiceDiscoveryOutputTypeDef",
     "AwsCloudMapServiceDiscoveryTypeDef",
     "ClientTlsCertificateTypeDef",
     "TagResourceInputRequestTypeDef",
     "ListTagsForResourceOutputTypeDef",
-    "GrpcRetryPolicyOutputTypeDef",
     "GrpcRetryPolicyTypeDef",
     "GrpcTimeoutTypeDef",
-    "HttpRetryPolicyOutputTypeDef",
     "HttpRetryPolicyTypeDef",
     "HttpTimeoutTypeDef",
     "OutlierDetectionTypeDef",
     "TcpTimeoutTypeDef",
     "GrpcGatewayRouteRewriteTypeDef",
     "ListGatewayRoutesOutputTypeDef",
     "GatewayRouteTargetTypeDef",
     "GrpcMetadataMatchMethodTypeDef",
     "GrpcRouteMetadataMatchMethodTypeDef",
     "HeaderMatchMethodTypeDef",
-    "GrpcRouteActionOutputTypeDef",
     "GrpcRouteActionTypeDef",
-    "HttpRouteActionOutputTypeDef",
     "HttpRouteActionTypeDef",
-    "TcpRouteActionOutputTypeDef",
     "TcpRouteActionTypeDef",
     "HttpGatewayRouteRewriteTypeDef",
     "HttpQueryParameterTypeDef",
-    "LoggingFormatOutputTypeDef",
     "LoggingFormatTypeDef",
     "ListGatewayRoutesInputListGatewayRoutesPaginateTypeDef",
     "ListMeshesInputListMeshesPaginateTypeDef",
     "ListRoutesInputListRoutesPaginateTypeDef",
     "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
     "ListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef",
     "ListVirtualNodesInputListVirtualNodesPaginateTypeDef",
@@ -172,158 +162,113 @@
     "ListVirtualServicesInputListVirtualServicesPaginateTypeDef",
     "ListMeshesOutputTypeDef",
     "ListRoutesOutputTypeDef",
     "ListVirtualGatewaysOutputTypeDef",
     "ListVirtualNodesOutputTypeDef",
     "ListVirtualRoutersOutputTypeDef",
     "ListVirtualServicesOutputTypeDef",
-    "VirtualRouterListenerTypeDef",
     "ListenerTlsCertificateTypeDef",
     "ListenerTlsValidationContextTrustTypeDef",
+    "VirtualRouterListenerTypeDef",
     "MeshSpecTypeDef",
-    "SubjectAlternativeNamesOutputTypeDef",
     "SubjectAlternativeNamesTypeDef",
-    "TlsValidationContextTrustOutputTypeDef",
     "TlsValidationContextTrustTypeDef",
     "VirtualGatewayClientTlsCertificateTypeDef",
     "VirtualGatewayConnectionPoolTypeDef",
     "VirtualGatewayListenerTlsCertificateTypeDef",
     "VirtualGatewayListenerTlsValidationContextTrustTypeDef",
-    "VirtualGatewayTlsValidationContextTrustOutputTypeDef",
     "VirtualGatewayTlsValidationContextTrustTypeDef",
     "VirtualNodeConnectionPoolTypeDef",
     "VirtualServiceProviderTypeDef",
-    "ServiceDiscoveryOutputTypeDef",
     "ServiceDiscoveryTypeDef",
     "ListenerTimeoutTypeDef",
     "GrpcGatewayRouteActionTypeDef",
     "GrpcGatewayRouteMetadataTypeDef",
     "GrpcRouteMetadataTypeDef",
     "HttpGatewayRouteHeaderTypeDef",
     "HttpRouteHeaderTypeDef",
-    "TcpRouteOutputTypeDef",
     "TcpRouteTypeDef",
     "HttpGatewayRouteActionTypeDef",
-    "FileAccessLogOutputTypeDef",
-    "VirtualGatewayFileAccessLogOutputTypeDef",
     "FileAccessLogTypeDef",
     "VirtualGatewayFileAccessLogTypeDef",
-    "VirtualRouterSpecOutputTypeDef",
     "VirtualRouterSpecTypeDef",
     "CreateMeshInputRequestTypeDef",
     "MeshDataTypeDef",
     "UpdateMeshInputRequestTypeDef",
-    "ListenerTlsValidationContextOutputTypeDef",
     "ListenerTlsValidationContextTypeDef",
-    "TlsValidationContextOutputTypeDef",
     "TlsValidationContextTypeDef",
-    "VirtualGatewayListenerTlsValidationContextOutputTypeDef",
     "VirtualGatewayListenerTlsValidationContextTypeDef",
-    "VirtualGatewayTlsValidationContextOutputTypeDef",
     "VirtualGatewayTlsValidationContextTypeDef",
     "VirtualServiceSpecTypeDef",
-    "GrpcGatewayRouteMatchOutputTypeDef",
     "GrpcGatewayRouteMatchTypeDef",
-    "GrpcRouteMatchOutputTypeDef",
     "GrpcRouteMatchTypeDef",
-    "HttpGatewayRouteMatchOutputTypeDef",
     "HttpGatewayRouteMatchTypeDef",
-    "HttpRouteMatchOutputTypeDef",
     "HttpRouteMatchTypeDef",
-    "AccessLogOutputTypeDef",
-    "VirtualGatewayAccessLogOutputTypeDef",
     "AccessLogTypeDef",
     "VirtualGatewayAccessLogTypeDef",
-    "VirtualRouterDataTypeDef",
     "CreateVirtualRouterInputRequestTypeDef",
     "UpdateVirtualRouterInputRequestTypeDef",
-    "VirtualRouterSpecUnionTypeDef",
+    "VirtualRouterDataTypeDef",
     "CreateMeshOutputTypeDef",
     "DeleteMeshOutputTypeDef",
     "DescribeMeshOutputTypeDef",
     "UpdateMeshOutputTypeDef",
-    "ListenerTlsOutputTypeDef",
     "ListenerTlsTypeDef",
-    "ClientPolicyTlsOutputTypeDef",
     "ClientPolicyTlsTypeDef",
-    "VirtualGatewayListenerTlsOutputTypeDef",
     "VirtualGatewayListenerTlsTypeDef",
-    "VirtualGatewayClientPolicyTlsOutputTypeDef",
     "VirtualGatewayClientPolicyTlsTypeDef",
     "CreateVirtualServiceInputRequestTypeDef",
     "UpdateVirtualServiceInputRequestTypeDef",
     "VirtualServiceDataTypeDef",
-    "GrpcGatewayRouteOutputTypeDef",
     "GrpcGatewayRouteTypeDef",
-    "GrpcRouteOutputTypeDef",
     "GrpcRouteTypeDef",
-    "HttpGatewayRouteOutputTypeDef",
     "HttpGatewayRouteTypeDef",
-    "HttpRouteOutputTypeDef",
     "HttpRouteTypeDef",
-    "LoggingOutputTypeDef",
-    "VirtualGatewayLoggingOutputTypeDef",
     "LoggingTypeDef",
     "VirtualGatewayLoggingTypeDef",
     "CreateVirtualRouterOutputTypeDef",
     "DeleteVirtualRouterOutputTypeDef",
     "DescribeVirtualRouterOutputTypeDef",
     "UpdateVirtualRouterOutputTypeDef",
-    "ListenerOutputTypeDef",
     "ListenerTypeDef",
-    "ClientPolicyOutputTypeDef",
     "ClientPolicyTypeDef",
-    "VirtualGatewayListenerOutputTypeDef",
     "VirtualGatewayListenerTypeDef",
-    "VirtualGatewayClientPolicyOutputTypeDef",
     "VirtualGatewayClientPolicyTypeDef",
     "CreateVirtualServiceOutputTypeDef",
     "DeleteVirtualServiceOutputTypeDef",
     "DescribeVirtualServiceOutputTypeDef",
     "UpdateVirtualServiceOutputTypeDef",
-    "GatewayRouteSpecOutputTypeDef",
     "GatewayRouteSpecTypeDef",
-    "RouteSpecOutputTypeDef",
     "RouteSpecTypeDef",
-    "BackendDefaultsOutputTypeDef",
-    "VirtualServiceBackendOutputTypeDef",
     "BackendDefaultsTypeDef",
     "VirtualServiceBackendTypeDef",
-    "VirtualGatewayBackendDefaultsOutputTypeDef",
     "VirtualGatewayBackendDefaultsTypeDef",
-    "GatewayRouteDataTypeDef",
     "CreateGatewayRouteInputRequestTypeDef",
-    "GatewayRouteSpecUnionTypeDef",
+    "GatewayRouteDataTypeDef",
     "UpdateGatewayRouteInputRequestTypeDef",
-    "RouteDataTypeDef",
     "CreateRouteInputRequestTypeDef",
-    "RouteSpecUnionTypeDef",
+    "RouteDataTypeDef",
     "UpdateRouteInputRequestTypeDef",
-    "BackendOutputTypeDef",
     "BackendTypeDef",
-    "VirtualGatewaySpecOutputTypeDef",
     "VirtualGatewaySpecTypeDef",
     "CreateGatewayRouteOutputTypeDef",
     "DeleteGatewayRouteOutputTypeDef",
     "DescribeGatewayRouteOutputTypeDef",
     "UpdateGatewayRouteOutputTypeDef",
     "CreateRouteOutputTypeDef",
     "DeleteRouteOutputTypeDef",
     "DescribeRouteOutputTypeDef",
     "UpdateRouteOutputTypeDef",
-    "VirtualNodeSpecOutputTypeDef",
     "VirtualNodeSpecTypeDef",
-    "VirtualGatewayDataTypeDef",
     "CreateVirtualGatewayInputRequestTypeDef",
     "UpdateVirtualGatewayInputRequestTypeDef",
-    "VirtualGatewaySpecUnionTypeDef",
-    "VirtualNodeDataTypeDef",
+    "VirtualGatewayDataTypeDef",
     "CreateVirtualNodeInputRequestTypeDef",
     "UpdateVirtualNodeInputRequestTypeDef",
-    "VirtualNodeSpecUnionTypeDef",
+    "VirtualNodeDataTypeDef",
     "CreateVirtualGatewayOutputTypeDef",
     "DeleteVirtualGatewayOutputTypeDef",
     "DescribeVirtualGatewayOutputTypeDef",
     "UpdateVirtualGatewayOutputTypeDef",
     "CreateVirtualNodeOutputTypeDef",
     "DeleteVirtualNodeOutputTypeDef",
     "DescribeVirtualNodeOutputTypeDef",
@@ -1082,22 +1027,14 @@
         "meshOwner": str,
         "resourceOwner": str,
         "version": int,
         "virtualServiceName": str,
     },
 )
 
-PortMappingTypeDef = TypedDict(
-    "PortMappingTypeDef",
-    {
-        "port": int,
-        "protocol": PortProtocolType,
-    },
-)
-
 ListenerTlsAcmCertificateTypeDef = TypedDict(
     "ListenerTlsAcmCertificateTypeDef",
     {
         "certificateArn": str,
     },
 )
 
@@ -1111,14 +1048,22 @@
 TlsValidationContextSdsTrustTypeDef = TypedDict(
     "TlsValidationContextSdsTrustTypeDef",
     {
         "secretName": str,
     },
 )
 
+PortMappingTypeDef = TypedDict(
+    "PortMappingTypeDef",
+    {
+        "port": int,
+        "protocol": PortProtocolType,
+    },
+)
+
 MeshStatusTypeDef = TypedDict(
     "MeshStatusTypeDef",
     {
         "status": MeshStatusCodeType,
     },
     total=False,
 )
@@ -1134,21 +1079,14 @@
 RouteStatusTypeDef = TypedDict(
     "RouteStatusTypeDef",
     {
         "status": RouteStatusCodeType,
     },
 )
 
-SubjectAlternativeNameMatchersOutputTypeDef = TypedDict(
-    "SubjectAlternativeNameMatchersOutputTypeDef",
-    {
-        "exact": List[str],
-    },
-)
-
 SubjectAlternativeNameMatchersTypeDef = TypedDict(
     "SubjectAlternativeNameMatchersTypeDef",
     {
         "exact": Sequence[str],
     },
 )
 
@@ -1156,21 +1094,14 @@
     "TcpRouteMatchTypeDef",
     {
         "port": int,
     },
     total=False,
 )
 
-TlsValidationContextAcmTrustOutputTypeDef = TypedDict(
-    "TlsValidationContextAcmTrustOutputTypeDef",
-    {
-        "certificateAuthorityArns": List[str],
-    },
-)
-
 TlsValidationContextAcmTrustTypeDef = TypedDict(
     "TlsValidationContextAcmTrustTypeDef",
     {
         "certificateAuthorityArns": Sequence[str],
     },
 )
 
@@ -1258,22 +1189,14 @@
 )
 
 class VirtualGatewayHealthCheckPolicyTypeDef(
     _RequiredVirtualGatewayHealthCheckPolicyTypeDef, _OptionalVirtualGatewayHealthCheckPolicyTypeDef
 ):
     pass
 
-VirtualGatewayPortMappingTypeDef = TypedDict(
-    "VirtualGatewayPortMappingTypeDef",
-    {
-        "port": int,
-        "protocol": VirtualGatewayPortProtocolType,
-    },
-)
-
 VirtualGatewayListenerTlsAcmCertificateTypeDef = TypedDict(
     "VirtualGatewayListenerTlsAcmCertificateTypeDef",
     {
         "certificateArn": str,
     },
 )
 
@@ -1287,18 +1210,19 @@
 VirtualGatewayTlsValidationContextSdsTrustTypeDef = TypedDict(
     "VirtualGatewayTlsValidationContextSdsTrustTypeDef",
     {
         "secretName": str,
     },
 )
 
-VirtualGatewayTlsValidationContextAcmTrustOutputTypeDef = TypedDict(
-    "VirtualGatewayTlsValidationContextAcmTrustOutputTypeDef",
+VirtualGatewayPortMappingTypeDef = TypedDict(
+    "VirtualGatewayPortMappingTypeDef",
     {
-        "certificateAuthorityArns": List[str],
+        "port": int,
+        "protocol": VirtualGatewayPortProtocolType,
     },
 )
 
 VirtualGatewayTlsValidationContextAcmTrustTypeDef = TypedDict(
     "VirtualGatewayTlsValidationContextAcmTrustTypeDef",
     {
         "certificateAuthorityArns": Sequence[str],
@@ -1376,36 +1300,14 @@
 VirtualServiceStatusTypeDef = TypedDict(
     "VirtualServiceStatusTypeDef",
     {
         "status": VirtualServiceStatusCodeType,
     },
 )
 
-_RequiredAwsCloudMapServiceDiscoveryOutputTypeDef = TypedDict(
-    "_RequiredAwsCloudMapServiceDiscoveryOutputTypeDef",
-    {
-        "namespaceName": str,
-        "serviceName": str,
-    },
-)
-_OptionalAwsCloudMapServiceDiscoveryOutputTypeDef = TypedDict(
-    "_OptionalAwsCloudMapServiceDiscoveryOutputTypeDef",
-    {
-        "attributes": List[AwsCloudMapInstanceAttributeTypeDef],
-        "ipPreference": IpPreferenceType,
-    },
-    total=False,
-)
-
-class AwsCloudMapServiceDiscoveryOutputTypeDef(
-    _RequiredAwsCloudMapServiceDiscoveryOutputTypeDef,
-    _OptionalAwsCloudMapServiceDiscoveryOutputTypeDef,
-):
-    pass
-
 _RequiredAwsCloudMapServiceDiscoveryTypeDef = TypedDict(
     "_RequiredAwsCloudMapServiceDiscoveryTypeDef",
     {
         "namespaceName": str,
         "serviceName": str,
     },
 )
@@ -1445,36 +1347,14 @@
     {
         "nextToken": str,
         "tags": List[TagRefTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredGrpcRetryPolicyOutputTypeDef = TypedDict(
-    "_RequiredGrpcRetryPolicyOutputTypeDef",
-    {
-        "maxRetries": int,
-        "perRetryTimeout": DurationTypeDef,
-    },
-)
-_OptionalGrpcRetryPolicyOutputTypeDef = TypedDict(
-    "_OptionalGrpcRetryPolicyOutputTypeDef",
-    {
-        "grpcRetryEvents": List[GrpcRetryPolicyEventType],
-        "httpRetryEvents": List[str],
-        "tcpRetryEvents": List[Literal["connection-error"]],
-    },
-    total=False,
-)
-
-class GrpcRetryPolicyOutputTypeDef(
-    _RequiredGrpcRetryPolicyOutputTypeDef, _OptionalGrpcRetryPolicyOutputTypeDef
-):
-    pass
-
 _RequiredGrpcRetryPolicyTypeDef = TypedDict(
     "_RequiredGrpcRetryPolicyTypeDef",
     {
         "maxRetries": int,
         "perRetryTimeout": DurationTypeDef,
     },
 )
@@ -1496,35 +1376,14 @@
     {
         "idle": DurationTypeDef,
         "perRequest": DurationTypeDef,
     },
     total=False,
 )
 
-_RequiredHttpRetryPolicyOutputTypeDef = TypedDict(
-    "_RequiredHttpRetryPolicyOutputTypeDef",
-    {
-        "maxRetries": int,
-        "perRetryTimeout": DurationTypeDef,
-    },
-)
-_OptionalHttpRetryPolicyOutputTypeDef = TypedDict(
-    "_OptionalHttpRetryPolicyOutputTypeDef",
-    {
-        "httpRetryEvents": List[str],
-        "tcpRetryEvents": List[Literal["connection-error"]],
-    },
-    total=False,
-)
-
-class HttpRetryPolicyOutputTypeDef(
-    _RequiredHttpRetryPolicyOutputTypeDef, _OptionalHttpRetryPolicyOutputTypeDef
-):
-    pass
-
 _RequiredHttpRetryPolicyTypeDef = TypedDict(
     "_RequiredHttpRetryPolicyTypeDef",
     {
         "maxRetries": int,
         "perRetryTimeout": DurationTypeDef,
     },
 )
@@ -1635,49 +1494,28 @@
         "range": MatchRangeTypeDef,
         "regex": str,
         "suffix": str,
     },
     total=False,
 )
 
-GrpcRouteActionOutputTypeDef = TypedDict(
-    "GrpcRouteActionOutputTypeDef",
-    {
-        "weightedTargets": List[WeightedTargetTypeDef],
-    },
-)
-
 GrpcRouteActionTypeDef = TypedDict(
     "GrpcRouteActionTypeDef",
     {
         "weightedTargets": Sequence[WeightedTargetTypeDef],
     },
 )
 
-HttpRouteActionOutputTypeDef = TypedDict(
-    "HttpRouteActionOutputTypeDef",
-    {
-        "weightedTargets": List[WeightedTargetTypeDef],
-    },
-)
-
 HttpRouteActionTypeDef = TypedDict(
     "HttpRouteActionTypeDef",
     {
         "weightedTargets": Sequence[WeightedTargetTypeDef],
     },
 )
 
-TcpRouteActionOutputTypeDef = TypedDict(
-    "TcpRouteActionOutputTypeDef",
-    {
-        "weightedTargets": List[WeightedTargetTypeDef],
-    },
-)
-
 TcpRouteActionTypeDef = TypedDict(
     "TcpRouteActionTypeDef",
     {
         "weightedTargets": Sequence[WeightedTargetTypeDef],
     },
 )
 
@@ -1706,23 +1544,14 @@
 )
 
 class HttpQueryParameterTypeDef(
     _RequiredHttpQueryParameterTypeDef, _OptionalHttpQueryParameterTypeDef
 ):
     pass
 
-LoggingFormatOutputTypeDef = TypedDict(
-    "LoggingFormatOutputTypeDef",
-    {
-        "json": List[JsonFormatRefTypeDef],
-        "text": str,
-    },
-    total=False,
-)
-
 LoggingFormatTypeDef = TypedDict(
     "LoggingFormatTypeDef",
     {
         "json": Sequence[JsonFormatRefTypeDef],
         "text": str,
     },
     total=False,
@@ -1934,21 +1763,14 @@
     {
         "nextToken": str,
         "virtualServices": List[VirtualServiceRefTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-VirtualRouterListenerTypeDef = TypedDict(
-    "VirtualRouterListenerTypeDef",
-    {
-        "portMapping": PortMappingTypeDef,
-    },
-)
-
 ListenerTlsCertificateTypeDef = TypedDict(
     "ListenerTlsCertificateTypeDef",
     {
         "acm": ListenerTlsAcmCertificateTypeDef,
         "file": ListenerTlsFileCertificateTypeDef,
         "sds": ListenerTlsSdsCertificateTypeDef,
     },
@@ -1960,47 +1782,37 @@
     {
         "file": TlsValidationContextFileTrustTypeDef,
         "sds": TlsValidationContextSdsTrustTypeDef,
     },
     total=False,
 )
 
+VirtualRouterListenerTypeDef = TypedDict(
+    "VirtualRouterListenerTypeDef",
+    {
+        "portMapping": PortMappingTypeDef,
+    },
+)
+
 MeshSpecTypeDef = TypedDict(
     "MeshSpecTypeDef",
     {
         "egressFilter": EgressFilterTypeDef,
         "serviceDiscovery": MeshServiceDiscoveryTypeDef,
     },
     total=False,
 )
 
-SubjectAlternativeNamesOutputTypeDef = TypedDict(
-    "SubjectAlternativeNamesOutputTypeDef",
-    {
-        "match": SubjectAlternativeNameMatchersOutputTypeDef,
-    },
-)
-
 SubjectAlternativeNamesTypeDef = TypedDict(
     "SubjectAlternativeNamesTypeDef",
     {
         "match": SubjectAlternativeNameMatchersTypeDef,
     },
 )
 
-TlsValidationContextTrustOutputTypeDef = TypedDict(
-    "TlsValidationContextTrustOutputTypeDef",
-    {
-        "acm": TlsValidationContextAcmTrustOutputTypeDef,
-        "file": TlsValidationContextFileTrustTypeDef,
-        "sds": TlsValidationContextSdsTrustTypeDef,
-    },
-    total=False,
-)
-
 TlsValidationContextTrustTypeDef = TypedDict(
     "TlsValidationContextTrustTypeDef",
     {
         "acm": TlsValidationContextAcmTrustTypeDef,
         "file": TlsValidationContextFileTrustTypeDef,
         "sds": TlsValidationContextSdsTrustTypeDef,
     },
@@ -2041,24 +1853,14 @@
     {
         "file": VirtualGatewayTlsValidationContextFileTrustTypeDef,
         "sds": VirtualGatewayTlsValidationContextSdsTrustTypeDef,
     },
     total=False,
 )
 
-VirtualGatewayTlsValidationContextTrustOutputTypeDef = TypedDict(
-    "VirtualGatewayTlsValidationContextTrustOutputTypeDef",
-    {
-        "acm": VirtualGatewayTlsValidationContextAcmTrustOutputTypeDef,
-        "file": VirtualGatewayTlsValidationContextFileTrustTypeDef,
-        "sds": VirtualGatewayTlsValidationContextSdsTrustTypeDef,
-    },
-    total=False,
-)
-
 VirtualGatewayTlsValidationContextTrustTypeDef = TypedDict(
     "VirtualGatewayTlsValidationContextTrustTypeDef",
     {
         "acm": VirtualGatewayTlsValidationContextAcmTrustTypeDef,
         "file": VirtualGatewayTlsValidationContextFileTrustTypeDef,
         "sds": VirtualGatewayTlsValidationContextSdsTrustTypeDef,
     },
@@ -2081,23 +1883,14 @@
     {
         "virtualNode": VirtualNodeServiceProviderTypeDef,
         "virtualRouter": VirtualRouterServiceProviderTypeDef,
     },
     total=False,
 )
 
-ServiceDiscoveryOutputTypeDef = TypedDict(
-    "ServiceDiscoveryOutputTypeDef",
-    {
-        "awsCloudMap": AwsCloudMapServiceDiscoveryOutputTypeDef,
-        "dns": DnsServiceDiscoveryTypeDef,
-    },
-    total=False,
-)
-
 ServiceDiscoveryTypeDef = TypedDict(
     "ServiceDiscoveryTypeDef",
     {
         "awsCloudMap": AwsCloudMapServiceDiscoveryTypeDef,
         "dns": DnsServiceDiscoveryTypeDef,
     },
     total=False,
@@ -2207,32 +2000,14 @@
     },
     total=False,
 )
 
 class HttpRouteHeaderTypeDef(_RequiredHttpRouteHeaderTypeDef, _OptionalHttpRouteHeaderTypeDef):
     pass
 
-_RequiredTcpRouteOutputTypeDef = TypedDict(
-    "_RequiredTcpRouteOutputTypeDef",
-    {
-        "action": TcpRouteActionOutputTypeDef,
-    },
-)
-_OptionalTcpRouteOutputTypeDef = TypedDict(
-    "_OptionalTcpRouteOutputTypeDef",
-    {
-        "match": TcpRouteMatchTypeDef,
-        "timeout": TcpTimeoutTypeDef,
-    },
-    total=False,
-)
-
-class TcpRouteOutputTypeDef(_RequiredTcpRouteOutputTypeDef, _OptionalTcpRouteOutputTypeDef):
-    pass
-
 _RequiredTcpRouteTypeDef = TypedDict(
     "_RequiredTcpRouteTypeDef",
     {
         "action": TcpRouteActionTypeDef,
     },
 )
 _OptionalTcpRouteTypeDef = TypedDict(
@@ -2262,53 +2037,14 @@
 )
 
 class HttpGatewayRouteActionTypeDef(
     _RequiredHttpGatewayRouteActionTypeDef, _OptionalHttpGatewayRouteActionTypeDef
 ):
     pass
 
-_RequiredFileAccessLogOutputTypeDef = TypedDict(
-    "_RequiredFileAccessLogOutputTypeDef",
-    {
-        "path": str,
-    },
-)
-_OptionalFileAccessLogOutputTypeDef = TypedDict(
-    "_OptionalFileAccessLogOutputTypeDef",
-    {
-        "format": LoggingFormatOutputTypeDef,
-    },
-    total=False,
-)
-
-class FileAccessLogOutputTypeDef(
-    _RequiredFileAccessLogOutputTypeDef, _OptionalFileAccessLogOutputTypeDef
-):
-    pass
-
-_RequiredVirtualGatewayFileAccessLogOutputTypeDef = TypedDict(
-    "_RequiredVirtualGatewayFileAccessLogOutputTypeDef",
-    {
-        "path": str,
-    },
-)
-_OptionalVirtualGatewayFileAccessLogOutputTypeDef = TypedDict(
-    "_OptionalVirtualGatewayFileAccessLogOutputTypeDef",
-    {
-        "format": LoggingFormatOutputTypeDef,
-    },
-    total=False,
-)
-
-class VirtualGatewayFileAccessLogOutputTypeDef(
-    _RequiredVirtualGatewayFileAccessLogOutputTypeDef,
-    _OptionalVirtualGatewayFileAccessLogOutputTypeDef,
-):
-    pass
-
 _RequiredFileAccessLogTypeDef = TypedDict(
     "_RequiredFileAccessLogTypeDef",
     {
         "path": str,
     },
 )
 _OptionalFileAccessLogTypeDef = TypedDict(
@@ -2337,22 +2073,14 @@
 )
 
 class VirtualGatewayFileAccessLogTypeDef(
     _RequiredVirtualGatewayFileAccessLogTypeDef, _OptionalVirtualGatewayFileAccessLogTypeDef
 ):
     pass
 
-VirtualRouterSpecOutputTypeDef = TypedDict(
-    "VirtualRouterSpecOutputTypeDef",
-    {
-        "listeners": List[VirtualRouterListenerTypeDef],
-    },
-    total=False,
-)
-
 VirtualRouterSpecTypeDef = TypedDict(
     "VirtualRouterSpecTypeDef",
     {
         "listeners": Sequence[VirtualRouterListenerTypeDef],
     },
     total=False,
 )
@@ -2404,34 +2132,14 @@
 )
 
 class UpdateMeshInputRequestTypeDef(
     _RequiredUpdateMeshInputRequestTypeDef, _OptionalUpdateMeshInputRequestTypeDef
 ):
     pass
 
-_RequiredListenerTlsValidationContextOutputTypeDef = TypedDict(
-    "_RequiredListenerTlsValidationContextOutputTypeDef",
-    {
-        "trust": ListenerTlsValidationContextTrustTypeDef,
-    },
-)
-_OptionalListenerTlsValidationContextOutputTypeDef = TypedDict(
-    "_OptionalListenerTlsValidationContextOutputTypeDef",
-    {
-        "subjectAlternativeNames": SubjectAlternativeNamesOutputTypeDef,
-    },
-    total=False,
-)
-
-class ListenerTlsValidationContextOutputTypeDef(
-    _RequiredListenerTlsValidationContextOutputTypeDef,
-    _OptionalListenerTlsValidationContextOutputTypeDef,
-):
-    pass
-
 _RequiredListenerTlsValidationContextTypeDef = TypedDict(
     "_RequiredListenerTlsValidationContextTypeDef",
     {
         "trust": ListenerTlsValidationContextTrustTypeDef,
     },
 )
 _OptionalListenerTlsValidationContextTypeDef = TypedDict(
@@ -2443,33 +2151,14 @@
 )
 
 class ListenerTlsValidationContextTypeDef(
     _RequiredListenerTlsValidationContextTypeDef, _OptionalListenerTlsValidationContextTypeDef
 ):
     pass
 
-_RequiredTlsValidationContextOutputTypeDef = TypedDict(
-    "_RequiredTlsValidationContextOutputTypeDef",
-    {
-        "trust": TlsValidationContextTrustOutputTypeDef,
-    },
-)
-_OptionalTlsValidationContextOutputTypeDef = TypedDict(
-    "_OptionalTlsValidationContextOutputTypeDef",
-    {
-        "subjectAlternativeNames": SubjectAlternativeNamesOutputTypeDef,
-    },
-    total=False,
-)
-
-class TlsValidationContextOutputTypeDef(
-    _RequiredTlsValidationContextOutputTypeDef, _OptionalTlsValidationContextOutputTypeDef
-):
-    pass
-
 _RequiredTlsValidationContextTypeDef = TypedDict(
     "_RequiredTlsValidationContextTypeDef",
     {
         "trust": TlsValidationContextTrustTypeDef,
     },
 )
 _OptionalTlsValidationContextTypeDef = TypedDict(
@@ -2481,34 +2170,14 @@
 )
 
 class TlsValidationContextTypeDef(
     _RequiredTlsValidationContextTypeDef, _OptionalTlsValidationContextTypeDef
 ):
     pass
 
-_RequiredVirtualGatewayListenerTlsValidationContextOutputTypeDef = TypedDict(
-    "_RequiredVirtualGatewayListenerTlsValidationContextOutputTypeDef",
-    {
-        "trust": VirtualGatewayListenerTlsValidationContextTrustTypeDef,
-    },
-)
-_OptionalVirtualGatewayListenerTlsValidationContextOutputTypeDef = TypedDict(
-    "_OptionalVirtualGatewayListenerTlsValidationContextOutputTypeDef",
-    {
-        "subjectAlternativeNames": SubjectAlternativeNamesOutputTypeDef,
-    },
-    total=False,
-)
-
-class VirtualGatewayListenerTlsValidationContextOutputTypeDef(
-    _RequiredVirtualGatewayListenerTlsValidationContextOutputTypeDef,
-    _OptionalVirtualGatewayListenerTlsValidationContextOutputTypeDef,
-):
-    pass
-
 _RequiredVirtualGatewayListenerTlsValidationContextTypeDef = TypedDict(
     "_RequiredVirtualGatewayListenerTlsValidationContextTypeDef",
     {
         "trust": VirtualGatewayListenerTlsValidationContextTrustTypeDef,
     },
 )
 _OptionalVirtualGatewayListenerTlsValidationContextTypeDef = TypedDict(
@@ -2521,34 +2190,14 @@
 
 class VirtualGatewayListenerTlsValidationContextTypeDef(
     _RequiredVirtualGatewayListenerTlsValidationContextTypeDef,
     _OptionalVirtualGatewayListenerTlsValidationContextTypeDef,
 ):
     pass
 
-_RequiredVirtualGatewayTlsValidationContextOutputTypeDef = TypedDict(
-    "_RequiredVirtualGatewayTlsValidationContextOutputTypeDef",
-    {
-        "trust": VirtualGatewayTlsValidationContextTrustOutputTypeDef,
-    },
-)
-_OptionalVirtualGatewayTlsValidationContextOutputTypeDef = TypedDict(
-    "_OptionalVirtualGatewayTlsValidationContextOutputTypeDef",
-    {
-        "subjectAlternativeNames": SubjectAlternativeNamesOutputTypeDef,
-    },
-    total=False,
-)
-
-class VirtualGatewayTlsValidationContextOutputTypeDef(
-    _RequiredVirtualGatewayTlsValidationContextOutputTypeDef,
-    _OptionalVirtualGatewayTlsValidationContextOutputTypeDef,
-):
-    pass
-
 _RequiredVirtualGatewayTlsValidationContextTypeDef = TypedDict(
     "_RequiredVirtualGatewayTlsValidationContextTypeDef",
     {
         "trust": VirtualGatewayTlsValidationContextTrustTypeDef,
     },
 )
 _OptionalVirtualGatewayTlsValidationContextTypeDef = TypedDict(
@@ -2569,130 +2218,64 @@
     "VirtualServiceSpecTypeDef",
     {
         "provider": VirtualServiceProviderTypeDef,
     },
     total=False,
 )
 
-GrpcGatewayRouteMatchOutputTypeDef = TypedDict(
-    "GrpcGatewayRouteMatchOutputTypeDef",
-    {
-        "hostname": GatewayRouteHostnameMatchTypeDef,
-        "metadata": List[GrpcGatewayRouteMetadataTypeDef],
-        "port": int,
-        "serviceName": str,
-    },
-    total=False,
-)
-
 GrpcGatewayRouteMatchTypeDef = TypedDict(
     "GrpcGatewayRouteMatchTypeDef",
     {
         "hostname": GatewayRouteHostnameMatchTypeDef,
         "metadata": Sequence[GrpcGatewayRouteMetadataTypeDef],
         "port": int,
         "serviceName": str,
     },
     total=False,
 )
 
-GrpcRouteMatchOutputTypeDef = TypedDict(
-    "GrpcRouteMatchOutputTypeDef",
-    {
-        "metadata": List[GrpcRouteMetadataTypeDef],
-        "methodName": str,
-        "port": int,
-        "serviceName": str,
-    },
-    total=False,
-)
-
 GrpcRouteMatchTypeDef = TypedDict(
     "GrpcRouteMatchTypeDef",
     {
         "metadata": Sequence[GrpcRouteMetadataTypeDef],
         "methodName": str,
         "port": int,
         "serviceName": str,
     },
     total=False,
 )
 
-HttpGatewayRouteMatchOutputTypeDef = TypedDict(
-    "HttpGatewayRouteMatchOutputTypeDef",
-    {
-        "headers": List[HttpGatewayRouteHeaderTypeDef],
-        "hostname": GatewayRouteHostnameMatchTypeDef,
-        "method": HttpMethodType,
-        "path": HttpPathMatchTypeDef,
-        "port": int,
-        "prefix": str,
-        "queryParameters": List[HttpQueryParameterTypeDef],
-    },
-    total=False,
-)
-
 HttpGatewayRouteMatchTypeDef = TypedDict(
     "HttpGatewayRouteMatchTypeDef",
     {
         "headers": Sequence[HttpGatewayRouteHeaderTypeDef],
         "hostname": GatewayRouteHostnameMatchTypeDef,
         "method": HttpMethodType,
         "path": HttpPathMatchTypeDef,
         "port": int,
         "prefix": str,
         "queryParameters": Sequence[HttpQueryParameterTypeDef],
     },
     total=False,
 )
 
-HttpRouteMatchOutputTypeDef = TypedDict(
-    "HttpRouteMatchOutputTypeDef",
-    {
-        "headers": List[HttpRouteHeaderTypeDef],
-        "method": HttpMethodType,
-        "path": HttpPathMatchTypeDef,
-        "port": int,
-        "prefix": str,
-        "queryParameters": List[HttpQueryParameterTypeDef],
-        "scheme": HttpSchemeType,
-    },
-    total=False,
-)
-
 HttpRouteMatchTypeDef = TypedDict(
     "HttpRouteMatchTypeDef",
     {
         "headers": Sequence[HttpRouteHeaderTypeDef],
         "method": HttpMethodType,
         "path": HttpPathMatchTypeDef,
         "port": int,
         "prefix": str,
         "queryParameters": Sequence[HttpQueryParameterTypeDef],
         "scheme": HttpSchemeType,
     },
     total=False,
 )
 
-AccessLogOutputTypeDef = TypedDict(
-    "AccessLogOutputTypeDef",
-    {
-        "file": FileAccessLogOutputTypeDef,
-    },
-    total=False,
-)
-
-VirtualGatewayAccessLogOutputTypeDef = TypedDict(
-    "VirtualGatewayAccessLogOutputTypeDef",
-    {
-        "file": VirtualGatewayFileAccessLogOutputTypeDef,
-    },
-    total=False,
-)
-
 AccessLogTypeDef = TypedDict(
     "AccessLogTypeDef",
     {
         "file": FileAccessLogTypeDef,
     },
     total=False,
 )
@@ -2701,25 +2284,14 @@
     "VirtualGatewayAccessLogTypeDef",
     {
         "file": VirtualGatewayFileAccessLogTypeDef,
     },
     total=False,
 )
 
-VirtualRouterDataTypeDef = TypedDict(
-    "VirtualRouterDataTypeDef",
-    {
-        "meshName": str,
-        "metadata": ResourceMetadataTypeDef,
-        "spec": VirtualRouterSpecOutputTypeDef,
-        "status": VirtualRouterStatusTypeDef,
-        "virtualRouterName": str,
-    },
-)
-
 _RequiredCreateVirtualRouterInputRequestTypeDef = TypedDict(
     "_RequiredCreateVirtualRouterInputRequestTypeDef",
     {
         "meshName": str,
         "spec": VirtualRouterSpecTypeDef,
         "virtualRouterName": str,
     },
@@ -2757,15 +2329,25 @@
 )
 
 class UpdateVirtualRouterInputRequestTypeDef(
     _RequiredUpdateVirtualRouterInputRequestTypeDef, _OptionalUpdateVirtualRouterInputRequestTypeDef
 ):
     pass
 
-VirtualRouterSpecUnionTypeDef = Union[VirtualRouterSpecTypeDef, VirtualRouterSpecOutputTypeDef]
+VirtualRouterDataTypeDef = TypedDict(
+    "VirtualRouterDataTypeDef",
+    {
+        "meshName": str,
+        "metadata": ResourceMetadataTypeDef,
+        "spec": VirtualRouterSpecTypeDef,
+        "status": VirtualRouterStatusTypeDef,
+        "virtualRouterName": str,
+    },
+)
+
 CreateMeshOutputTypeDef = TypedDict(
     "CreateMeshOutputTypeDef",
     {
         "mesh": MeshDataTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2790,34 +2372,14 @@
     "UpdateMeshOutputTypeDef",
     {
         "mesh": MeshDataTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredListenerTlsOutputTypeDef = TypedDict(
-    "_RequiredListenerTlsOutputTypeDef",
-    {
-        "certificate": ListenerTlsCertificateTypeDef,
-        "mode": ListenerTlsModeType,
-    },
-)
-_OptionalListenerTlsOutputTypeDef = TypedDict(
-    "_OptionalListenerTlsOutputTypeDef",
-    {
-        "validation": ListenerTlsValidationContextOutputTypeDef,
-    },
-    total=False,
-)
-
-class ListenerTlsOutputTypeDef(
-    _RequiredListenerTlsOutputTypeDef, _OptionalListenerTlsOutputTypeDef
-):
-    pass
-
 _RequiredListenerTlsTypeDef = TypedDict(
     "_RequiredListenerTlsTypeDef",
     {
         "certificate": ListenerTlsCertificateTypeDef,
         "mode": ListenerTlsModeType,
     },
 )
@@ -2828,35 +2390,14 @@
     },
     total=False,
 )
 
 class ListenerTlsTypeDef(_RequiredListenerTlsTypeDef, _OptionalListenerTlsTypeDef):
     pass
 
-_RequiredClientPolicyTlsOutputTypeDef = TypedDict(
-    "_RequiredClientPolicyTlsOutputTypeDef",
-    {
-        "validation": TlsValidationContextOutputTypeDef,
-    },
-)
-_OptionalClientPolicyTlsOutputTypeDef = TypedDict(
-    "_OptionalClientPolicyTlsOutputTypeDef",
-    {
-        "certificate": ClientTlsCertificateTypeDef,
-        "enforce": bool,
-        "ports": List[int],
-    },
-    total=False,
-)
-
-class ClientPolicyTlsOutputTypeDef(
-    _RequiredClientPolicyTlsOutputTypeDef, _OptionalClientPolicyTlsOutputTypeDef
-):
-    pass
-
 _RequiredClientPolicyTlsTypeDef = TypedDict(
     "_RequiredClientPolicyTlsTypeDef",
     {
         "validation": TlsValidationContextTypeDef,
     },
 )
 _OptionalClientPolicyTlsTypeDef = TypedDict(
@@ -2868,34 +2409,14 @@
     },
     total=False,
 )
 
 class ClientPolicyTlsTypeDef(_RequiredClientPolicyTlsTypeDef, _OptionalClientPolicyTlsTypeDef):
     pass
 
-_RequiredVirtualGatewayListenerTlsOutputTypeDef = TypedDict(
-    "_RequiredVirtualGatewayListenerTlsOutputTypeDef",
-    {
-        "certificate": VirtualGatewayListenerTlsCertificateTypeDef,
-        "mode": VirtualGatewayListenerTlsModeType,
-    },
-)
-_OptionalVirtualGatewayListenerTlsOutputTypeDef = TypedDict(
-    "_OptionalVirtualGatewayListenerTlsOutputTypeDef",
-    {
-        "validation": VirtualGatewayListenerTlsValidationContextOutputTypeDef,
-    },
-    total=False,
-)
-
-class VirtualGatewayListenerTlsOutputTypeDef(
-    _RequiredVirtualGatewayListenerTlsOutputTypeDef, _OptionalVirtualGatewayListenerTlsOutputTypeDef
-):
-    pass
-
 _RequiredVirtualGatewayListenerTlsTypeDef = TypedDict(
     "_RequiredVirtualGatewayListenerTlsTypeDef",
     {
         "certificate": VirtualGatewayListenerTlsCertificateTypeDef,
         "mode": VirtualGatewayListenerTlsModeType,
     },
 )
@@ -2908,36 +2429,14 @@
 )
 
 class VirtualGatewayListenerTlsTypeDef(
     _RequiredVirtualGatewayListenerTlsTypeDef, _OptionalVirtualGatewayListenerTlsTypeDef
 ):
     pass
 
-_RequiredVirtualGatewayClientPolicyTlsOutputTypeDef = TypedDict(
-    "_RequiredVirtualGatewayClientPolicyTlsOutputTypeDef",
-    {
-        "validation": VirtualGatewayTlsValidationContextOutputTypeDef,
-    },
-)
-_OptionalVirtualGatewayClientPolicyTlsOutputTypeDef = TypedDict(
-    "_OptionalVirtualGatewayClientPolicyTlsOutputTypeDef",
-    {
-        "certificate": VirtualGatewayClientTlsCertificateTypeDef,
-        "enforce": bool,
-        "ports": List[int],
-    },
-    total=False,
-)
-
-class VirtualGatewayClientPolicyTlsOutputTypeDef(
-    _RequiredVirtualGatewayClientPolicyTlsOutputTypeDef,
-    _OptionalVirtualGatewayClientPolicyTlsOutputTypeDef,
-):
-    pass
-
 _RequiredVirtualGatewayClientPolicyTlsTypeDef = TypedDict(
     "_RequiredVirtualGatewayClientPolicyTlsTypeDef",
     {
         "validation": VirtualGatewayTlsValidationContextTypeDef,
     },
 )
 _OptionalVirtualGatewayClientPolicyTlsTypeDef = TypedDict(
@@ -3009,49 +2508,22 @@
         "metadata": ResourceMetadataTypeDef,
         "spec": VirtualServiceSpecTypeDef,
         "status": VirtualServiceStatusTypeDef,
         "virtualServiceName": str,
     },
 )
 
-GrpcGatewayRouteOutputTypeDef = TypedDict(
-    "GrpcGatewayRouteOutputTypeDef",
-    {
-        "action": GrpcGatewayRouteActionTypeDef,
-        "match": GrpcGatewayRouteMatchOutputTypeDef,
-    },
-)
-
 GrpcGatewayRouteTypeDef = TypedDict(
     "GrpcGatewayRouteTypeDef",
     {
         "action": GrpcGatewayRouteActionTypeDef,
         "match": GrpcGatewayRouteMatchTypeDef,
     },
 )
 
-_RequiredGrpcRouteOutputTypeDef = TypedDict(
-    "_RequiredGrpcRouteOutputTypeDef",
-    {
-        "action": GrpcRouteActionOutputTypeDef,
-        "match": GrpcRouteMatchOutputTypeDef,
-    },
-)
-_OptionalGrpcRouteOutputTypeDef = TypedDict(
-    "_OptionalGrpcRouteOutputTypeDef",
-    {
-        "retryPolicy": GrpcRetryPolicyOutputTypeDef,
-        "timeout": GrpcTimeoutTypeDef,
-    },
-    total=False,
-)
-
-class GrpcRouteOutputTypeDef(_RequiredGrpcRouteOutputTypeDef, _OptionalGrpcRouteOutputTypeDef):
-    pass
-
 _RequiredGrpcRouteTypeDef = TypedDict(
     "_RequiredGrpcRouteTypeDef",
     {
         "action": GrpcRouteActionTypeDef,
         "match": GrpcRouteMatchTypeDef,
     },
 )
@@ -3063,49 +2535,22 @@
     },
     total=False,
 )
 
 class GrpcRouteTypeDef(_RequiredGrpcRouteTypeDef, _OptionalGrpcRouteTypeDef):
     pass
 
-HttpGatewayRouteOutputTypeDef = TypedDict(
-    "HttpGatewayRouteOutputTypeDef",
-    {
-        "action": HttpGatewayRouteActionTypeDef,
-        "match": HttpGatewayRouteMatchOutputTypeDef,
-    },
-)
-
 HttpGatewayRouteTypeDef = TypedDict(
     "HttpGatewayRouteTypeDef",
     {
         "action": HttpGatewayRouteActionTypeDef,
         "match": HttpGatewayRouteMatchTypeDef,
     },
 )
 
-_RequiredHttpRouteOutputTypeDef = TypedDict(
-    "_RequiredHttpRouteOutputTypeDef",
-    {
-        "action": HttpRouteActionOutputTypeDef,
-        "match": HttpRouteMatchOutputTypeDef,
-    },
-)
-_OptionalHttpRouteOutputTypeDef = TypedDict(
-    "_OptionalHttpRouteOutputTypeDef",
-    {
-        "retryPolicy": HttpRetryPolicyOutputTypeDef,
-        "timeout": HttpTimeoutTypeDef,
-    },
-    total=False,
-)
-
-class HttpRouteOutputTypeDef(_RequiredHttpRouteOutputTypeDef, _OptionalHttpRouteOutputTypeDef):
-    pass
-
 _RequiredHttpRouteTypeDef = TypedDict(
     "_RequiredHttpRouteTypeDef",
     {
         "action": HttpRouteActionTypeDef,
         "match": HttpRouteMatchTypeDef,
     },
 )
@@ -3117,30 +2562,14 @@
     },
     total=False,
 )
 
 class HttpRouteTypeDef(_RequiredHttpRouteTypeDef, _OptionalHttpRouteTypeDef):
     pass
 
-LoggingOutputTypeDef = TypedDict(
-    "LoggingOutputTypeDef",
-    {
-        "accessLog": AccessLogOutputTypeDef,
-    },
-    total=False,
-)
-
-VirtualGatewayLoggingOutputTypeDef = TypedDict(
-    "VirtualGatewayLoggingOutputTypeDef",
-    {
-        "accessLog": VirtualGatewayAccessLogOutputTypeDef,
-    },
-    total=False,
-)
-
 LoggingTypeDef = TypedDict(
     "LoggingTypeDef",
     {
         "accessLog": AccessLogTypeDef,
     },
     total=False,
 )
@@ -3181,35 +2610,14 @@
     "UpdateVirtualRouterOutputTypeDef",
     {
         "virtualRouter": VirtualRouterDataTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredListenerOutputTypeDef = TypedDict(
-    "_RequiredListenerOutputTypeDef",
-    {
-        "portMapping": PortMappingTypeDef,
-    },
-)
-_OptionalListenerOutputTypeDef = TypedDict(
-    "_OptionalListenerOutputTypeDef",
-    {
-        "connectionPool": VirtualNodeConnectionPoolTypeDef,
-        "healthCheck": HealthCheckPolicyTypeDef,
-        "outlierDetection": OutlierDetectionTypeDef,
-        "timeout": ListenerTimeoutTypeDef,
-        "tls": ListenerTlsOutputTypeDef,
-    },
-    total=False,
-)
-
-class ListenerOutputTypeDef(_RequiredListenerOutputTypeDef, _OptionalListenerOutputTypeDef):
-    pass
-
 _RequiredListenerTypeDef = TypedDict(
     "_RequiredListenerTypeDef",
     {
         "portMapping": PortMappingTypeDef,
     },
 )
 _OptionalListenerTypeDef = TypedDict(
@@ -3223,51 +2631,22 @@
     },
     total=False,
 )
 
 class ListenerTypeDef(_RequiredListenerTypeDef, _OptionalListenerTypeDef):
     pass
 
-ClientPolicyOutputTypeDef = TypedDict(
-    "ClientPolicyOutputTypeDef",
-    {
-        "tls": ClientPolicyTlsOutputTypeDef,
-    },
-    total=False,
-)
-
 ClientPolicyTypeDef = TypedDict(
     "ClientPolicyTypeDef",
     {
         "tls": ClientPolicyTlsTypeDef,
     },
     total=False,
 )
 
-_RequiredVirtualGatewayListenerOutputTypeDef = TypedDict(
-    "_RequiredVirtualGatewayListenerOutputTypeDef",
-    {
-        "portMapping": VirtualGatewayPortMappingTypeDef,
-    },
-)
-_OptionalVirtualGatewayListenerOutputTypeDef = TypedDict(
-    "_OptionalVirtualGatewayListenerOutputTypeDef",
-    {
-        "connectionPool": VirtualGatewayConnectionPoolTypeDef,
-        "healthCheck": VirtualGatewayHealthCheckPolicyTypeDef,
-        "tls": VirtualGatewayListenerTlsOutputTypeDef,
-    },
-    total=False,
-)
-
-class VirtualGatewayListenerOutputTypeDef(
-    _RequiredVirtualGatewayListenerOutputTypeDef, _OptionalVirtualGatewayListenerOutputTypeDef
-):
-    pass
-
 _RequiredVirtualGatewayListenerTypeDef = TypedDict(
     "_RequiredVirtualGatewayListenerTypeDef",
     {
         "portMapping": VirtualGatewayPortMappingTypeDef,
     },
 )
 _OptionalVirtualGatewayListenerTypeDef = TypedDict(
@@ -3281,22 +2660,14 @@
 )
 
 class VirtualGatewayListenerTypeDef(
     _RequiredVirtualGatewayListenerTypeDef, _OptionalVirtualGatewayListenerTypeDef
 ):
     pass
 
-VirtualGatewayClientPolicyOutputTypeDef = TypedDict(
-    "VirtualGatewayClientPolicyOutputTypeDef",
-    {
-        "tls": VirtualGatewayClientPolicyTlsOutputTypeDef,
-    },
-    total=False,
-)
-
 VirtualGatewayClientPolicyTypeDef = TypedDict(
     "VirtualGatewayClientPolicyTypeDef",
     {
         "tls": VirtualGatewayClientPolicyTlsTypeDef,
     },
     total=False,
 )
@@ -3329,87 +2700,37 @@
     "UpdateVirtualServiceOutputTypeDef",
     {
         "virtualService": VirtualServiceDataTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GatewayRouteSpecOutputTypeDef = TypedDict(
-    "GatewayRouteSpecOutputTypeDef",
-    {
-        "grpcRoute": GrpcGatewayRouteOutputTypeDef,
-        "http2Route": HttpGatewayRouteOutputTypeDef,
-        "httpRoute": HttpGatewayRouteOutputTypeDef,
-        "priority": int,
-    },
-    total=False,
-)
-
 GatewayRouteSpecTypeDef = TypedDict(
     "GatewayRouteSpecTypeDef",
     {
         "grpcRoute": GrpcGatewayRouteTypeDef,
         "http2Route": HttpGatewayRouteTypeDef,
         "httpRoute": HttpGatewayRouteTypeDef,
         "priority": int,
     },
     total=False,
 )
 
-RouteSpecOutputTypeDef = TypedDict(
-    "RouteSpecOutputTypeDef",
-    {
-        "grpcRoute": GrpcRouteOutputTypeDef,
-        "http2Route": HttpRouteOutputTypeDef,
-        "httpRoute": HttpRouteOutputTypeDef,
-        "priority": int,
-        "tcpRoute": TcpRouteOutputTypeDef,
-    },
-    total=False,
-)
-
 RouteSpecTypeDef = TypedDict(
     "RouteSpecTypeDef",
     {
         "grpcRoute": GrpcRouteTypeDef,
         "http2Route": HttpRouteTypeDef,
         "httpRoute": HttpRouteTypeDef,
         "priority": int,
         "tcpRoute": TcpRouteTypeDef,
     },
     total=False,
 )
 
-BackendDefaultsOutputTypeDef = TypedDict(
-    "BackendDefaultsOutputTypeDef",
-    {
-        "clientPolicy": ClientPolicyOutputTypeDef,
-    },
-    total=False,
-)
-
-_RequiredVirtualServiceBackendOutputTypeDef = TypedDict(
-    "_RequiredVirtualServiceBackendOutputTypeDef",
-    {
-        "virtualServiceName": str,
-    },
-)
-_OptionalVirtualServiceBackendOutputTypeDef = TypedDict(
-    "_OptionalVirtualServiceBackendOutputTypeDef",
-    {
-        "clientPolicy": ClientPolicyOutputTypeDef,
-    },
-    total=False,
-)
-
-class VirtualServiceBackendOutputTypeDef(
-    _RequiredVirtualServiceBackendOutputTypeDef, _OptionalVirtualServiceBackendOutputTypeDef
-):
-    pass
-
 BackendDefaultsTypeDef = TypedDict(
     "BackendDefaultsTypeDef",
     {
         "clientPolicy": ClientPolicyTypeDef,
     },
     total=False,
 )
@@ -3429,42 +2750,22 @@
 )
 
 class VirtualServiceBackendTypeDef(
     _RequiredVirtualServiceBackendTypeDef, _OptionalVirtualServiceBackendTypeDef
 ):
     pass
 
-VirtualGatewayBackendDefaultsOutputTypeDef = TypedDict(
-    "VirtualGatewayBackendDefaultsOutputTypeDef",
-    {
-        "clientPolicy": VirtualGatewayClientPolicyOutputTypeDef,
-    },
-    total=False,
-)
-
 VirtualGatewayBackendDefaultsTypeDef = TypedDict(
     "VirtualGatewayBackendDefaultsTypeDef",
     {
         "clientPolicy": VirtualGatewayClientPolicyTypeDef,
     },
     total=False,
 )
 
-GatewayRouteDataTypeDef = TypedDict(
-    "GatewayRouteDataTypeDef",
-    {
-        "gatewayRouteName": str,
-        "meshName": str,
-        "metadata": ResourceMetadataTypeDef,
-        "spec": GatewayRouteSpecOutputTypeDef,
-        "status": GatewayRouteStatusTypeDef,
-        "virtualGatewayName": str,
-    },
-)
-
 _RequiredCreateGatewayRouteInputRequestTypeDef = TypedDict(
     "_RequiredCreateGatewayRouteInputRequestTypeDef",
     {
         "gatewayRouteName": str,
         "meshName": str,
         "spec": GatewayRouteSpecTypeDef,
         "virtualGatewayName": str,
@@ -3481,15 +2782,26 @@
 )
 
 class CreateGatewayRouteInputRequestTypeDef(
     _RequiredCreateGatewayRouteInputRequestTypeDef, _OptionalCreateGatewayRouteInputRequestTypeDef
 ):
     pass
 
-GatewayRouteSpecUnionTypeDef = Union[GatewayRouteSpecTypeDef, GatewayRouteSpecOutputTypeDef]
+GatewayRouteDataTypeDef = TypedDict(
+    "GatewayRouteDataTypeDef",
+    {
+        "gatewayRouteName": str,
+        "meshName": str,
+        "metadata": ResourceMetadataTypeDef,
+        "spec": GatewayRouteSpecTypeDef,
+        "status": GatewayRouteStatusTypeDef,
+        "virtualGatewayName": str,
+    },
+)
+
 _RequiredUpdateGatewayRouteInputRequestTypeDef = TypedDict(
     "_RequiredUpdateGatewayRouteInputRequestTypeDef",
     {
         "gatewayRouteName": str,
         "meshName": str,
         "spec": GatewayRouteSpecTypeDef,
         "virtualGatewayName": str,
@@ -3505,26 +2817,14 @@
 )
 
 class UpdateGatewayRouteInputRequestTypeDef(
     _RequiredUpdateGatewayRouteInputRequestTypeDef, _OptionalUpdateGatewayRouteInputRequestTypeDef
 ):
     pass
 
-RouteDataTypeDef = TypedDict(
-    "RouteDataTypeDef",
-    {
-        "meshName": str,
-        "metadata": ResourceMetadataTypeDef,
-        "routeName": str,
-        "spec": RouteSpecOutputTypeDef,
-        "status": RouteStatusTypeDef,
-        "virtualRouterName": str,
-    },
-)
-
 _RequiredCreateRouteInputRequestTypeDef = TypedDict(
     "_RequiredCreateRouteInputRequestTypeDef",
     {
         "meshName": str,
         "routeName": str,
         "spec": RouteSpecTypeDef,
         "virtualRouterName": str,
@@ -3541,15 +2841,26 @@
 )
 
 class CreateRouteInputRequestTypeDef(
     _RequiredCreateRouteInputRequestTypeDef, _OptionalCreateRouteInputRequestTypeDef
 ):
     pass
 
-RouteSpecUnionTypeDef = Union[RouteSpecTypeDef, RouteSpecOutputTypeDef]
+RouteDataTypeDef = TypedDict(
+    "RouteDataTypeDef",
+    {
+        "meshName": str,
+        "metadata": ResourceMetadataTypeDef,
+        "routeName": str,
+        "spec": RouteSpecTypeDef,
+        "status": RouteStatusTypeDef,
+        "virtualRouterName": str,
+    },
+)
+
 _RequiredUpdateRouteInputRequestTypeDef = TypedDict(
     "_RequiredUpdateRouteInputRequestTypeDef",
     {
         "meshName": str,
         "routeName": str,
         "spec": RouteSpecTypeDef,
         "virtualRouterName": str,
@@ -3565,50 +2876,22 @@
 )
 
 class UpdateRouteInputRequestTypeDef(
     _RequiredUpdateRouteInputRequestTypeDef, _OptionalUpdateRouteInputRequestTypeDef
 ):
     pass
 
-BackendOutputTypeDef = TypedDict(
-    "BackendOutputTypeDef",
-    {
-        "virtualService": VirtualServiceBackendOutputTypeDef,
-    },
-    total=False,
-)
-
 BackendTypeDef = TypedDict(
     "BackendTypeDef",
     {
         "virtualService": VirtualServiceBackendTypeDef,
     },
     total=False,
 )
 
-_RequiredVirtualGatewaySpecOutputTypeDef = TypedDict(
-    "_RequiredVirtualGatewaySpecOutputTypeDef",
-    {
-        "listeners": List[VirtualGatewayListenerOutputTypeDef],
-    },
-)
-_OptionalVirtualGatewaySpecOutputTypeDef = TypedDict(
-    "_OptionalVirtualGatewaySpecOutputTypeDef",
-    {
-        "backendDefaults": VirtualGatewayBackendDefaultsOutputTypeDef,
-        "logging": VirtualGatewayLoggingOutputTypeDef,
-    },
-    total=False,
-)
-
-class VirtualGatewaySpecOutputTypeDef(
-    _RequiredVirtualGatewaySpecOutputTypeDef, _OptionalVirtualGatewaySpecOutputTypeDef
-):
-    pass
-
 _RequiredVirtualGatewaySpecTypeDef = TypedDict(
     "_RequiredVirtualGatewaySpecTypeDef",
     {
         "listeners": Sequence[VirtualGatewayListenerTypeDef],
     },
 )
 _OptionalVirtualGatewaySpecTypeDef = TypedDict(
@@ -3685,49 +2968,26 @@
     "UpdateRouteOutputTypeDef",
     {
         "route": RouteDataTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-VirtualNodeSpecOutputTypeDef = TypedDict(
-    "VirtualNodeSpecOutputTypeDef",
-    {
-        "backendDefaults": BackendDefaultsOutputTypeDef,
-        "backends": List[BackendOutputTypeDef],
-        "listeners": List[ListenerOutputTypeDef],
-        "logging": LoggingOutputTypeDef,
-        "serviceDiscovery": ServiceDiscoveryOutputTypeDef,
-    },
-    total=False,
-)
-
 VirtualNodeSpecTypeDef = TypedDict(
     "VirtualNodeSpecTypeDef",
     {
         "backendDefaults": BackendDefaultsTypeDef,
         "backends": Sequence[BackendTypeDef],
         "listeners": Sequence[ListenerTypeDef],
         "logging": LoggingTypeDef,
         "serviceDiscovery": ServiceDiscoveryTypeDef,
     },
     total=False,
 )
 
-VirtualGatewayDataTypeDef = TypedDict(
-    "VirtualGatewayDataTypeDef",
-    {
-        "meshName": str,
-        "metadata": ResourceMetadataTypeDef,
-        "spec": VirtualGatewaySpecOutputTypeDef,
-        "status": VirtualGatewayStatusTypeDef,
-        "virtualGatewayName": str,
-    },
-)
-
 _RequiredCreateVirtualGatewayInputRequestTypeDef = TypedDict(
     "_RequiredCreateVirtualGatewayInputRequestTypeDef",
     {
         "meshName": str,
         "spec": VirtualGatewaySpecTypeDef,
         "virtualGatewayName": str,
     },
@@ -3767,23 +3027,22 @@
 
 class UpdateVirtualGatewayInputRequestTypeDef(
     _RequiredUpdateVirtualGatewayInputRequestTypeDef,
     _OptionalUpdateVirtualGatewayInputRequestTypeDef,
 ):
     pass
 
-VirtualGatewaySpecUnionTypeDef = Union[VirtualGatewaySpecTypeDef, VirtualGatewaySpecOutputTypeDef]
-VirtualNodeDataTypeDef = TypedDict(
-    "VirtualNodeDataTypeDef",
+VirtualGatewayDataTypeDef = TypedDict(
+    "VirtualGatewayDataTypeDef",
     {
         "meshName": str,
         "metadata": ResourceMetadataTypeDef,
-        "spec": VirtualNodeSpecOutputTypeDef,
-        "status": VirtualNodeStatusTypeDef,
-        "virtualNodeName": str,
+        "spec": VirtualGatewaySpecTypeDef,
+        "status": VirtualGatewayStatusTypeDef,
+        "virtualGatewayName": str,
     },
 )
 
 _RequiredCreateVirtualNodeInputRequestTypeDef = TypedDict(
     "_RequiredCreateVirtualNodeInputRequestTypeDef",
     {
         "meshName": str,
@@ -3824,15 +3083,25 @@
 )
 
 class UpdateVirtualNodeInputRequestTypeDef(
     _RequiredUpdateVirtualNodeInputRequestTypeDef, _OptionalUpdateVirtualNodeInputRequestTypeDef
 ):
     pass
 
-VirtualNodeSpecUnionTypeDef = Union[VirtualNodeSpecTypeDef, VirtualNodeSpecOutputTypeDef]
+VirtualNodeDataTypeDef = TypedDict(
+    "VirtualNodeDataTypeDef",
+    {
+        "meshName": str,
+        "metadata": ResourceMetadataTypeDef,
+        "spec": VirtualNodeSpecTypeDef,
+        "status": VirtualNodeStatusTypeDef,
+        "virtualNodeName": str,
+    },
+)
+
 CreateVirtualGatewayOutputTypeDef = TypedDict(
     "CreateVirtualGatewayOutputTypeDef",
     {
         "virtualGateway": VirtualGatewayDataTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh.egg-info/SOURCES.txt` & `types-aiobotocore-appmesh-2.5.2.post2/types_aiobotocore_appmesh.egg-info/SOURCES.txt`

 * *Files identical despite different names*

