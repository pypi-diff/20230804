# Comparing `tmp/types-aiobotocore-clouddirectory-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-clouddirectory-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-clouddirectory-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:59 2023, max compression
+gzip compressed data, was "types-aiobotocore-clouddirectory-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:33 2023, max compression
```

## Comparing `types-aiobotocore-clouddirectory-2.5.2.post1.tar` & `types-aiobotocore-clouddirectory-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:59.929637 types-aiobotocore-clouddirectory-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:34:22.000000 types-aiobotocore-clouddirectory-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    26795 2023-08-02 14:51:59.929637 types-aiobotocore-clouddirectory-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    25249 2023-08-02 14:34:22.000000 types-aiobotocore-clouddirectory-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:59.929637 types-aiobotocore-clouddirectory-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-08-02 14:34:21.000000 types-aiobotocore-clouddirectory-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:59.929637 types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory/
--rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-08-02 14:34:22.000000 types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-08-02 14:34:22.000000 types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-02 14:34:22.000000 types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    59814 2023-08-02 14:34:22.000000 types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    59720 2023-08-02 14:34:22.000000 types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11877 2023-08-02 14:34:22.000000 types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11875 2023-08-02 14:34:22.000000 types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    25325 2023-08-02 14:34:22.000000 types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    25304 2023-08-02 14:34:22.000000 types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:34:22.000000 types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    90540 2023-08-02 14:34:25.000000 types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    90408 2023-08-02 14:34:23.000000 types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:34:22.000000 types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:59.929637 types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    26795 2023-08-02 14:51:59.000000 types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-02 14:51:59.000000 types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:59.000000 types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:59.000000 types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:59.000000 types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 14:51:59.000000 types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:33.727429 types-aiobotocore-clouddirectory-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:41:35.000000 types-aiobotocore-clouddirectory-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16301 2023-08-04 12:00:33.723429 types-aiobotocore-clouddirectory-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14755 2023-08-04 11:41:35.000000 types-aiobotocore-clouddirectory-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:33.727429 types-aiobotocore-clouddirectory-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-08-04 11:41:35.000000 types-aiobotocore-clouddirectory-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:33.723429 types-aiobotocore-clouddirectory-2.5.2.post2/types_aiobotocore_clouddirectory/
+-rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-08-04 11:41:35.000000 types-aiobotocore-clouddirectory-2.5.2.post2/types_aiobotocore_clouddirectory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-08-04 11:41:35.000000 types-aiobotocore-clouddirectory-2.5.2.post2/types_aiobotocore_clouddirectory/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-04 11:41:35.000000 types-aiobotocore-clouddirectory-2.5.2.post2/types_aiobotocore_clouddirectory/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59759 2023-08-04 11:41:35.000000 types-aiobotocore-clouddirectory-2.5.2.post2/types_aiobotocore_clouddirectory/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59665 2023-08-04 11:41:35.000000 types-aiobotocore-clouddirectory-2.5.2.post2/types_aiobotocore_clouddirectory/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11877 2023-08-04 11:41:36.000000 types-aiobotocore-clouddirectory-2.5.2.post2/types_aiobotocore_clouddirectory/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11875 2023-08-04 11:41:35.000000 types-aiobotocore-clouddirectory-2.5.2.post2/types_aiobotocore_clouddirectory/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    25325 2023-08-04 11:41:35.000000 types-aiobotocore-clouddirectory-2.5.2.post2/types_aiobotocore_clouddirectory/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25304 2023-08-04 11:41:35.000000 types-aiobotocore-clouddirectory-2.5.2.post2/types_aiobotocore_clouddirectory/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:41:35.000000 types-aiobotocore-clouddirectory-2.5.2.post2/types_aiobotocore_clouddirectory/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    86481 2023-08-04 11:41:38.000000 types-aiobotocore-clouddirectory-2.5.2.post2/types_aiobotocore_clouddirectory/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86354 2023-08-04 11:41:37.000000 types-aiobotocore-clouddirectory-2.5.2.post2/types_aiobotocore_clouddirectory/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:41:35.000000 types-aiobotocore-clouddirectory-2.5.2.post2/types_aiobotocore_clouddirectory/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:33.723429 types-aiobotocore-clouddirectory-2.5.2.post2/types_aiobotocore_clouddirectory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16301 2023-08-04 12:00:33.000000 types-aiobotocore-clouddirectory-2.5.2.post2/types_aiobotocore_clouddirectory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-04 12:00:33.000000 types-aiobotocore-clouddirectory-2.5.2.post2/types_aiobotocore_clouddirectory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:33.000000 types-aiobotocore-clouddirectory-2.5.2.post2/types_aiobotocore_clouddirectory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:33.000000 types-aiobotocore-clouddirectory-2.5.2.post2/types_aiobotocore_clouddirectory.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:33.000000 types-aiobotocore-clouddirectory-2.5.2.post2/types_aiobotocore_clouddirectory.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-04 12:00:33.000000 types-aiobotocore-clouddirectory-2.5.2.post2/types_aiobotocore_clouddirectory.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-clouddirectory-2.5.2.post1/LICENSE` & `types-aiobotocore-clouddirectory-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-clouddirectory-2.5.2.post1/setup.py` & `types-aiobotocore-clouddirectory-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-clouddirectory",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_clouddirectory"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CloudDirectory 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory/__init__.py` & `types-aiobotocore-clouddirectory-2.5.2.post2/types_aiobotocore_clouddirectory/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory/__init__.pyi` & `types-aiobotocore-clouddirectory-2.5.2.post2/types_aiobotocore_clouddirectory/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory/__main__.py` & `types-aiobotocore-clouddirectory-2.5.2.post2/types_aiobotocore_clouddirectory/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.CloudDirectory 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory\nOther"
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

### Comparing `types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory/client.py` & `types-aiobotocore-clouddirectory-2.5.2.post2/types_aiobotocore_clouddirectory/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,17 +43,17 @@
     LookupPolicyPaginator,
 )
 from .type_defs import (
     ApplySchemaResponseTypeDef,
     AttachObjectResponseTypeDef,
     AttachToIndexResponseTypeDef,
     AttachTypedLinkResponseTypeDef,
-    AttributeKeyAndValueUnionTypeDef,
+    AttributeKeyAndValueTypeDef,
     AttributeKeyTypeDef,
-    AttributeNameAndValueUnionTypeDef,
+    AttributeNameAndValueTypeDef,
     BatchReadOperationTypeDef,
     BatchReadResponseTypeDef,
     BatchWriteOperationTypeDef,
     BatchWriteResponseTypeDef,
     CreateDirectoryResponseTypeDef,
     CreateIndexResponseTypeDef,
     CreateObjectResponseTypeDef,
@@ -61,15 +61,15 @@
     DeleteDirectoryResponseTypeDef,
     DeleteSchemaResponseTypeDef,
     DetachFromIndexResponseTypeDef,
     DetachObjectResponseTypeDef,
     DisableDirectoryResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     EnableDirectoryResponseTypeDef,
-    FacetAttributeUnionTypeDef,
+    FacetAttributeTypeDef,
     FacetAttributeUpdateTypeDef,
     GetAppliedSchemaVersionResponseTypeDef,
     GetDirectoryResponseTypeDef,
     GetFacetResponseTypeDef,
     GetLinkAttributesResponseTypeDef,
     GetObjectAttributesResponseTypeDef,
     GetObjectInformationResponseTypeDef,
@@ -104,15 +104,15 @@
     PutSchemaFromJsonResponseTypeDef,
     SchemaFacetTypeDef,
     TagTypeDef,
     TypedLinkAttributeRangeTypeDef,
     TypedLinkFacetAttributeUpdateTypeDef,
     TypedLinkFacetTypeDef,
     TypedLinkSchemaAndFacetNameTypeDef,
-    TypedLinkSpecifierUnionTypeDef,
+    TypedLinkSpecifierTypeDef,
     UpdateObjectAttributesResponseTypeDef,
     UpdateSchemaResponseTypeDef,
     UpgradeAppliedSchemaResponseTypeDef,
     UpgradePublishedSchemaResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -190,15 +190,15 @@
 
     async def add_facet_to_object(
         self,
         *,
         DirectoryArn: str,
         SchemaFacet: SchemaFacetTypeDef,
         ObjectReference: ObjectReferenceTypeDef,
-        ObjectAttributeList: Sequence[AttributeKeyAndValueUnionTypeDef] = ...
+        ObjectAttributeList: Sequence[AttributeKeyAndValueTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Adds a new  Facet to an object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.add_facet_to_object)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#add_facet_to_object)
         """
@@ -260,15 +260,15 @@
     async def attach_typed_link(
         self,
         *,
         DirectoryArn: str,
         SourceObjectReference: ObjectReferenceTypeDef,
         TargetObjectReference: ObjectReferenceTypeDef,
         TypedLinkFacet: TypedLinkSchemaAndFacetNameTypeDef,
-        Attributes: Sequence[AttributeNameAndValueUnionTypeDef]
+        Attributes: Sequence[AttributeNameAndValueTypeDef]
     ) -> AttachTypedLinkResponseTypeDef:
         """
         Attaches a typed link to a specified source and target object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.attach_typed_link)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#attach_typed_link)
         """
@@ -324,15 +324,15 @@
         """
 
     async def create_facet(
         self,
         *,
         SchemaArn: str,
         Name: str,
-        Attributes: Sequence[FacetAttributeUnionTypeDef] = ...,
+        Attributes: Sequence[FacetAttributeTypeDef] = ...,
         ObjectType: ObjectTypeType = ...,
         FacetStyle: FacetStyleType = ...
     ) -> Dict[str, Any]:
         """
         Creates a new  Facet in a schema.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.create_facet)
@@ -356,15 +356,15 @@
         """
 
     async def create_object(
         self,
         *,
         DirectoryArn: str,
         SchemaFacets: Sequence[SchemaFacetTypeDef],
-        ObjectAttributeList: Sequence[AttributeKeyAndValueUnionTypeDef] = ...,
+        ObjectAttributeList: Sequence[AttributeKeyAndValueTypeDef] = ...,
         ParentReference: ObjectReferenceTypeDef = ...,
         LinkName: str = ...
     ) -> CreateObjectResponseTypeDef:
         """
         Creates an object in a  Directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.create_object)
@@ -466,15 +466,15 @@
         Detaches a policy from an object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.detach_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#detach_policy)
         """
 
     async def detach_typed_link(
-        self, *, DirectoryArn: str, TypedLinkSpecifier: TypedLinkSpecifierUnionTypeDef
+        self, *, DirectoryArn: str, TypedLinkSpecifier: TypedLinkSpecifierTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
         Detaches a typed link from a specified source and target object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.detach_typed_link)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#detach_typed_link)
         """
@@ -536,15 +536,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#get_facet)
         """
 
     async def get_link_attributes(
         self,
         *,
         DirectoryArn: str,
-        TypedLinkSpecifier: TypedLinkSpecifierUnionTypeDef,
+        TypedLinkSpecifier: TypedLinkSpecifierTypeDef,
         AttributeNames: Sequence[str],
         ConsistencyLevel: ConsistencyLevelType = ...
     ) -> GetLinkAttributesResponseTypeDef:
         """
         Retrieves attributes that are associated with a typed link.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.get_link_attributes)
@@ -957,15 +957,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#update_facet)
         """
 
     async def update_link_attributes(
         self,
         *,
         DirectoryArn: str,
-        TypedLinkSpecifier: TypedLinkSpecifierUnionTypeDef,
+        TypedLinkSpecifier: TypedLinkSpecifierTypeDef,
         AttributeUpdates: Sequence[LinkAttributeUpdateTypeDef]
     ) -> Dict[str, Any]:
         """
         Updates a given typed link’s attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.update_link_attributes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#update_link_attributes)
```

### Comparing `types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory/client.pyi` & `types-aiobotocore-clouddirectory-2.5.2.post2/types_aiobotocore_clouddirectory/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -43,17 +43,17 @@
     LookupPolicyPaginator,
 )
 from .type_defs import (
     ApplySchemaResponseTypeDef,
     AttachObjectResponseTypeDef,
     AttachToIndexResponseTypeDef,
     AttachTypedLinkResponseTypeDef,
-    AttributeKeyAndValueUnionTypeDef,
+    AttributeKeyAndValueTypeDef,
     AttributeKeyTypeDef,
-    AttributeNameAndValueUnionTypeDef,
+    AttributeNameAndValueTypeDef,
     BatchReadOperationTypeDef,
     BatchReadResponseTypeDef,
     BatchWriteOperationTypeDef,
     BatchWriteResponseTypeDef,
     CreateDirectoryResponseTypeDef,
     CreateIndexResponseTypeDef,
     CreateObjectResponseTypeDef,
@@ -61,15 +61,15 @@
     DeleteDirectoryResponseTypeDef,
     DeleteSchemaResponseTypeDef,
     DetachFromIndexResponseTypeDef,
     DetachObjectResponseTypeDef,
     DisableDirectoryResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     EnableDirectoryResponseTypeDef,
-    FacetAttributeUnionTypeDef,
+    FacetAttributeTypeDef,
     FacetAttributeUpdateTypeDef,
     GetAppliedSchemaVersionResponseTypeDef,
     GetDirectoryResponseTypeDef,
     GetFacetResponseTypeDef,
     GetLinkAttributesResponseTypeDef,
     GetObjectAttributesResponseTypeDef,
     GetObjectInformationResponseTypeDef,
@@ -104,15 +104,15 @@
     PutSchemaFromJsonResponseTypeDef,
     SchemaFacetTypeDef,
     TagTypeDef,
     TypedLinkAttributeRangeTypeDef,
     TypedLinkFacetAttributeUpdateTypeDef,
     TypedLinkFacetTypeDef,
     TypedLinkSchemaAndFacetNameTypeDef,
-    TypedLinkSpecifierUnionTypeDef,
+    TypedLinkSpecifierTypeDef,
     UpdateObjectAttributesResponseTypeDef,
     UpdateSchemaResponseTypeDef,
     UpgradeAppliedSchemaResponseTypeDef,
     UpgradePublishedSchemaResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -185,15 +185,15 @@
         """
     async def add_facet_to_object(
         self,
         *,
         DirectoryArn: str,
         SchemaFacet: SchemaFacetTypeDef,
         ObjectReference: ObjectReferenceTypeDef,
-        ObjectAttributeList: Sequence[AttributeKeyAndValueUnionTypeDef] = ...
+        ObjectAttributeList: Sequence[AttributeKeyAndValueTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Adds a new  Facet to an object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.add_facet_to_object)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#add_facet_to_object)
         """
@@ -250,15 +250,15 @@
     async def attach_typed_link(
         self,
         *,
         DirectoryArn: str,
         SourceObjectReference: ObjectReferenceTypeDef,
         TargetObjectReference: ObjectReferenceTypeDef,
         TypedLinkFacet: TypedLinkSchemaAndFacetNameTypeDef,
-        Attributes: Sequence[AttributeNameAndValueUnionTypeDef]
+        Attributes: Sequence[AttributeNameAndValueTypeDef]
     ) -> AttachTypedLinkResponseTypeDef:
         """
         Attaches a typed link to a specified source and target object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.attach_typed_link)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#attach_typed_link)
         """
@@ -308,15 +308,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#create_directory)
         """
     async def create_facet(
         self,
         *,
         SchemaArn: str,
         Name: str,
-        Attributes: Sequence[FacetAttributeUnionTypeDef] = ...,
+        Attributes: Sequence[FacetAttributeTypeDef] = ...,
         ObjectType: ObjectTypeType = ...,
         FacetStyle: FacetStyleType = ...
     ) -> Dict[str, Any]:
         """
         Creates a new  Facet in a schema.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.create_facet)
@@ -338,15 +338,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#create_index)
         """
     async def create_object(
         self,
         *,
         DirectoryArn: str,
         SchemaFacets: Sequence[SchemaFacetTypeDef],
-        ObjectAttributeList: Sequence[AttributeKeyAndValueUnionTypeDef] = ...,
+        ObjectAttributeList: Sequence[AttributeKeyAndValueTypeDef] = ...,
         ParentReference: ObjectReferenceTypeDef = ...,
         LinkName: str = ...
     ) -> CreateObjectResponseTypeDef:
         """
         Creates an object in a  Directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.create_object)
@@ -437,15 +437,15 @@
         """
         Detaches a policy from an object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.detach_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#detach_policy)
         """
     async def detach_typed_link(
-        self, *, DirectoryArn: str, TypedLinkSpecifier: TypedLinkSpecifierUnionTypeDef
+        self, *, DirectoryArn: str, TypedLinkSpecifier: TypedLinkSpecifierTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
         Detaches a typed link from a specified source and target object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.detach_typed_link)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#detach_typed_link)
         """
@@ -500,15 +500,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.get_facet)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#get_facet)
         """
     async def get_link_attributes(
         self,
         *,
         DirectoryArn: str,
-        TypedLinkSpecifier: TypedLinkSpecifierUnionTypeDef,
+        TypedLinkSpecifier: TypedLinkSpecifierTypeDef,
         AttributeNames: Sequence[str],
         ConsistencyLevel: ConsistencyLevelType = ...
     ) -> GetLinkAttributesResponseTypeDef:
         """
         Retrieves attributes that are associated with a typed link.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.get_link_attributes)
@@ -889,15 +889,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.update_facet)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#update_facet)
         """
     async def update_link_attributes(
         self,
         *,
         DirectoryArn: str,
-        TypedLinkSpecifier: TypedLinkSpecifierUnionTypeDef,
+        TypedLinkSpecifier: TypedLinkSpecifierTypeDef,
         AttributeUpdates: Sequence[LinkAttributeUpdateTypeDef]
     ) -> Dict[str, Any]:
         """
         Updates a given typed link’s attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.update_link_attributes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#update_link_attributes)
```

### Comparing `types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory/literals.py` & `types-aiobotocore-clouddirectory-2.5.2.post2/types_aiobotocore_clouddirectory/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory/literals.pyi` & `types-aiobotocore-clouddirectory-2.5.2.post2/types_aiobotocore_clouddirectory/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory/paginator.py` & `types-aiobotocore-clouddirectory-2.5.2.post2/types_aiobotocore_clouddirectory/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory/paginator.pyi` & `types-aiobotocore-clouddirectory-2.5.2.post2/types_aiobotocore_clouddirectory/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory/type_defs.py` & `types-aiobotocore-clouddirectory-2.5.2.post2/types_aiobotocore_clouddirectory/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 __all__ = (
     "ObjectReferenceTypeDef",
     "SchemaFacetTypeDef",
     "ApplySchemaRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "TypedLinkSchemaAndFacetNameTypeDef",
     "AttributeKeyTypeDef",
-    "TypedAttributeValueOutputTypeDef",
     "BatchAttachObjectResponseTypeDef",
     "BatchAttachToIndexResponseTypeDef",
     "BatchCreateIndexResponseTypeDef",
     "BatchCreateObjectResponseTypeDef",
     "BatchDetachFromIndexResponseTypeDef",
     "BatchDetachObjectResponseTypeDef",
     "BatchListObjectChildrenResponseTypeDef",
@@ -63,15 +62,14 @@
     "DeleteDirectoryRequestRequestTypeDef",
     "DeleteFacetRequestRequestTypeDef",
     "DeleteSchemaRequestRequestTypeDef",
     "DeleteTypedLinkFacetRequestRequestTypeDef",
     "DirectoryTypeDef",
     "DisableDirectoryRequestRequestTypeDef",
     "EnableDirectoryRequestRequestTypeDef",
-    "RuleOutputTypeDef",
     "RuleTypeDef",
     "FacetAttributeReferenceTypeDef",
     "FacetTypeDef",
     "GetAppliedSchemaVersionRequestRequestTypeDef",
     "GetDirectoryRequestRequestTypeDef",
     "GetFacetRequestRequestTypeDef",
     "GetSchemaAsJsonRequestRequestTypeDef",
@@ -164,24 +162,20 @@
     "PutSchemaFromJsonResponseTypeDef",
     "UpdateObjectAttributesResponseTypeDef",
     "UpdateSchemaResponseTypeDef",
     "UpgradeAppliedSchemaResponseTypeDef",
     "UpgradePublishedSchemaResponseTypeDef",
     "BatchCreateIndexTypeDef",
     "CreateIndexRequestRequestTypeDef",
-    "AttributeKeyAndValueOutputTypeDef",
-    "AttributeNameAndValueOutputTypeDef",
     "BatchListObjectParentPathsResponseTypeDef",
     "ListObjectParentPathsResponseTypeDef",
     "BatchListObjectParentsResponseTypeDef",
     "ListObjectParentsResponseTypeDef",
     "GetDirectoryResponseTypeDef",
     "ListDirectoriesResponseTypeDef",
-    "FacetAttributeDefinitionOutputTypeDef",
-    "TypedLinkAttributeDefinitionOutputTypeDef",
     "GetFacetResponseTypeDef",
     "ListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef",
     "ListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef",
     "ListDevelopmentSchemaArnsRequestListDevelopmentSchemaArnsPaginateTypeDef",
     "ListDirectoriesRequestListDirectoriesPaginateTypeDef",
     "ListFacetAttributesRequestListFacetAttributesPaginateTypeDef",
     "ListFacetNamesRequestListFacetNamesPaginateTypeDef",
@@ -195,69 +189,62 @@
     "ListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef",
     "ListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef",
     "LookupPolicyRequestLookupPolicyPaginateTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "PolicyToPathTypeDef",
     "TypedAttributeValueTypeDef",
-    "BatchGetLinkAttributesResponseTypeDef",
-    "BatchGetObjectAttributesResponseTypeDef",
-    "BatchListObjectAttributesResponseTypeDef",
-    "GetLinkAttributesResponseTypeDef",
-    "GetObjectAttributesResponseTypeDef",
-    "IndexAttachmentTypeDef",
-    "ListObjectAttributesResponseTypeDef",
-    "TypedLinkSpecifierOutputTypeDef",
-    "FacetAttributeOutputTypeDef",
-    "ListTypedLinkFacetAttributesResponseTypeDef",
     "BatchLookupPolicyResponseTypeDef",
     "LookupPolicyResponseTypeDef",
     "AttributeKeyAndValueTypeDef",
     "AttributeNameAndValueTypeDef",
     "FacetAttributeDefinitionTypeDef",
     "LinkAttributeActionTypeDef",
     "ObjectAttributeActionTypeDef",
     "TypedAttributeValueRangeTypeDef",
     "TypedLinkAttributeDefinitionTypeDef",
-    "BatchListAttachedIndicesResponseTypeDef",
-    "BatchListIndexResponseTypeDef",
-    "ListAttachedIndicesResponseTypeDef",
-    "ListIndexResponseTypeDef",
-    "AttachTypedLinkResponseTypeDef",
-    "BatchAttachTypedLinkResponseTypeDef",
-    "BatchListIncomingTypedLinksResponseTypeDef",
-    "BatchListOutgoingTypedLinksResponseTypeDef",
-    "ListIncomingTypedLinksResponseTypeDef",
-    "ListOutgoingTypedLinksResponseTypeDef",
-    "ListFacetAttributesResponseTypeDef",
-    "AttributeKeyAndValueUnionTypeDef",
+    "AddFacetToObjectRequestRequestTypeDef",
     "BatchAddFacetToObjectTypeDef",
     "BatchCreateObjectTypeDef",
-    "AttributeNameAndValueUnionTypeDef",
+    "BatchGetLinkAttributesResponseTypeDef",
+    "BatchGetObjectAttributesResponseTypeDef",
+    "BatchListObjectAttributesResponseTypeDef",
+    "CreateObjectRequestRequestTypeDef",
+    "GetLinkAttributesResponseTypeDef",
+    "GetObjectAttributesResponseTypeDef",
+    "IndexAttachmentTypeDef",
+    "ListObjectAttributesResponseTypeDef",
+    "AttachTypedLinkRequestRequestTypeDef",
     "BatchAttachTypedLinkTypeDef",
     "TypedLinkSpecifierTypeDef",
     "FacetAttributeTypeDef",
     "LinkAttributeUpdateTypeDef",
     "ObjectAttributeUpdateTypeDef",
     "ObjectAttributeRangeTypeDef",
     "TypedLinkAttributeRangeTypeDef",
+    "ListTypedLinkFacetAttributesResponseTypeDef",
     "TypedLinkFacetAttributeUpdateTypeDef",
     "TypedLinkFacetTypeDef",
-    "BatchWriteOperationResponseTypeDef",
-    "BatchReadSuccessfulResponseTypeDef",
-    "AddFacetToObjectRequestRequestTypeDef",
-    "CreateObjectRequestRequestTypeDef",
-    "AttachTypedLinkRequestRequestTypeDef",
+    "BatchListAttachedIndicesResponseTypeDef",
+    "BatchListIndexResponseTypeDef",
+    "ListAttachedIndicesResponseTypeDef",
+    "ListIndexResponseTypeDef",
+    "AttachTypedLinkResponseTypeDef",
+    "BatchAttachTypedLinkResponseTypeDef",
     "BatchDetachTypedLinkTypeDef",
     "BatchGetLinkAttributesTypeDef",
+    "BatchListIncomingTypedLinksResponseTypeDef",
+    "BatchListOutgoingTypedLinksResponseTypeDef",
     "DetachTypedLinkRequestRequestTypeDef",
     "GetLinkAttributesRequestRequestTypeDef",
-    "TypedLinkSpecifierUnionTypeDef",
-    "FacetAttributeUnionTypeDef",
+    "ListIncomingTypedLinksResponseTypeDef",
+    "ListOutgoingTypedLinksResponseTypeDef",
+    "CreateFacetRequestRequestTypeDef",
     "FacetAttributeUpdateTypeDef",
+    "ListFacetAttributesResponseTypeDef",
     "BatchUpdateLinkAttributesTypeDef",
     "UpdateLinkAttributesRequestRequestTypeDef",
     "BatchUpdateObjectAttributesTypeDef",
     "UpdateObjectAttributesRequestRequestTypeDef",
     "BatchListIndexTypeDef",
     "ListIndexRequestListIndexPaginateTypeDef",
     "ListIndexRequestRequestTypeDef",
@@ -265,23 +252,24 @@
     "BatchListOutgoingTypedLinksTypeDef",
     "ListIncomingTypedLinksRequestListIncomingTypedLinksPaginateTypeDef",
     "ListIncomingTypedLinksRequestRequestTypeDef",
     "ListOutgoingTypedLinksRequestListOutgoingTypedLinksPaginateTypeDef",
     "ListOutgoingTypedLinksRequestRequestTypeDef",
     "UpdateTypedLinkFacetRequestRequestTypeDef",
     "CreateTypedLinkFacetRequestRequestTypeDef",
-    "BatchWriteResponseTypeDef",
-    "BatchReadOperationResponseTypeDef",
-    "CreateFacetRequestRequestTypeDef",
+    "BatchWriteOperationResponseTypeDef",
+    "BatchReadSuccessfulResponseTypeDef",
     "UpdateFacetRequestRequestTypeDef",
     "BatchWriteOperationTypeDef",
     "BatchReadOperationTypeDef",
-    "BatchReadResponseTypeDef",
+    "BatchWriteResponseTypeDef",
+    "BatchReadOperationResponseTypeDef",
     "BatchWriteRequestRequestTypeDef",
     "BatchReadRequestRequestTypeDef",
+    "BatchReadResponseTypeDef",
 )
 
 ObjectReferenceTypeDef = TypedDict(
     "ObjectReferenceTypeDef",
     {
         "Selector": str,
     },
@@ -329,26 +317,14 @@
     {
         "SchemaArn": str,
         "FacetName": str,
         "Name": str,
     },
 )
 
-TypedAttributeValueOutputTypeDef = TypedDict(
-    "TypedAttributeValueOutputTypeDef",
-    {
-        "StringValue": str,
-        "BinaryValue": bytes,
-        "BooleanValue": bool,
-        "NumberValue": str,
-        "DatetimeValue": datetime,
-    },
-    total=False,
-)
-
 BatchAttachObjectResponseTypeDef = TypedDict(
     "BatchAttachObjectResponseTypeDef",
     {
         "attachedObjectIdentifier": str,
     },
     total=False,
 )
@@ -522,23 +498,14 @@
 EnableDirectoryRequestRequestTypeDef = TypedDict(
     "EnableDirectoryRequestRequestTypeDef",
     {
         "DirectoryArn": str,
     },
 )
 
-RuleOutputTypeDef = TypedDict(
-    "RuleOutputTypeDef",
-    {
-        "Type": RuleTypeType,
-        "Parameters": Dict[str, str],
-    },
-    total=False,
-)
-
 RuleTypeDef = TypedDict(
     "RuleTypeDef",
     {
         "Type": RuleTypeType,
         "Parameters": Mapping[str, str],
     },
     total=False,
@@ -1821,30 +1788,14 @@
 
 class CreateIndexRequestRequestTypeDef(
     _RequiredCreateIndexRequestRequestTypeDef, _OptionalCreateIndexRequestRequestTypeDef
 ):
     pass
 
 
-AttributeKeyAndValueOutputTypeDef = TypedDict(
-    "AttributeKeyAndValueOutputTypeDef",
-    {
-        "Key": AttributeKeyTypeDef,
-        "Value": TypedAttributeValueOutputTypeDef,
-    },
-)
-
-AttributeNameAndValueOutputTypeDef = TypedDict(
-    "AttributeNameAndValueOutputTypeDef",
-    {
-        "AttributeName": str,
-        "Value": TypedAttributeValueOutputTypeDef,
-    },
-)
-
 BatchListObjectParentPathsResponseTypeDef = TypedDict(
     "BatchListObjectParentPathsResponseTypeDef",
     {
         "PathToObjectIdentifiersList": List[PathToObjectIdentifiersTypeDef],
         "NextToken": str,
     },
     total=False,
@@ -1891,63 +1842,14 @@
     {
         "Directories": List[DirectoryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredFacetAttributeDefinitionOutputTypeDef = TypedDict(
-    "_RequiredFacetAttributeDefinitionOutputTypeDef",
-    {
-        "Type": FacetAttributeTypeType,
-    },
-)
-_OptionalFacetAttributeDefinitionOutputTypeDef = TypedDict(
-    "_OptionalFacetAttributeDefinitionOutputTypeDef",
-    {
-        "DefaultValue": TypedAttributeValueOutputTypeDef,
-        "IsImmutable": bool,
-        "Rules": Dict[str, RuleOutputTypeDef],
-    },
-    total=False,
-)
-
-
-class FacetAttributeDefinitionOutputTypeDef(
-    _RequiredFacetAttributeDefinitionOutputTypeDef, _OptionalFacetAttributeDefinitionOutputTypeDef
-):
-    pass
-
-
-_RequiredTypedLinkAttributeDefinitionOutputTypeDef = TypedDict(
-    "_RequiredTypedLinkAttributeDefinitionOutputTypeDef",
-    {
-        "Name": str,
-        "Type": FacetAttributeTypeType,
-        "RequiredBehavior": RequiredAttributeBehaviorType,
-    },
-)
-_OptionalTypedLinkAttributeDefinitionOutputTypeDef = TypedDict(
-    "_OptionalTypedLinkAttributeDefinitionOutputTypeDef",
-    {
-        "DefaultValue": TypedAttributeValueOutputTypeDef,
-        "IsImmutable": bool,
-        "Rules": Dict[str, RuleOutputTypeDef],
-    },
-    total=False,
-)
-
-
-class TypedLinkAttributeDefinitionOutputTypeDef(
-    _RequiredTypedLinkAttributeDefinitionOutputTypeDef,
-    _OptionalTypedLinkAttributeDefinitionOutputTypeDef,
-):
-    pass
-
-
 GetFacetResponseTypeDef = TypedDict(
     "GetFacetResponseTypeDef",
     {
         "Facet": FacetTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2299,115 +2201,14 @@
         "BooleanValue": bool,
         "NumberValue": str,
         "DatetimeValue": TimestampTypeDef,
     },
     total=False,
 )
 
-BatchGetLinkAttributesResponseTypeDef = TypedDict(
-    "BatchGetLinkAttributesResponseTypeDef",
-    {
-        "Attributes": List[AttributeKeyAndValueOutputTypeDef],
-    },
-    total=False,
-)
-
-BatchGetObjectAttributesResponseTypeDef = TypedDict(
-    "BatchGetObjectAttributesResponseTypeDef",
-    {
-        "Attributes": List[AttributeKeyAndValueOutputTypeDef],
-    },
-    total=False,
-)
-
-BatchListObjectAttributesResponseTypeDef = TypedDict(
-    "BatchListObjectAttributesResponseTypeDef",
-    {
-        "Attributes": List[AttributeKeyAndValueOutputTypeDef],
-        "NextToken": str,
-    },
-    total=False,
-)
-
-GetLinkAttributesResponseTypeDef = TypedDict(
-    "GetLinkAttributesResponseTypeDef",
-    {
-        "Attributes": List[AttributeKeyAndValueOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetObjectAttributesResponseTypeDef = TypedDict(
-    "GetObjectAttributesResponseTypeDef",
-    {
-        "Attributes": List[AttributeKeyAndValueOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-IndexAttachmentTypeDef = TypedDict(
-    "IndexAttachmentTypeDef",
-    {
-        "IndexedAttributes": List[AttributeKeyAndValueOutputTypeDef],
-        "ObjectIdentifier": str,
-    },
-    total=False,
-)
-
-ListObjectAttributesResponseTypeDef = TypedDict(
-    "ListObjectAttributesResponseTypeDef",
-    {
-        "Attributes": List[AttributeKeyAndValueOutputTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-TypedLinkSpecifierOutputTypeDef = TypedDict(
-    "TypedLinkSpecifierOutputTypeDef",
-    {
-        "TypedLinkFacet": TypedLinkSchemaAndFacetNameTypeDef,
-        "SourceObjectReference": ObjectReferenceTypeDef,
-        "TargetObjectReference": ObjectReferenceTypeDef,
-        "IdentityAttributeValues": List[AttributeNameAndValueOutputTypeDef],
-    },
-)
-
-_RequiredFacetAttributeOutputTypeDef = TypedDict(
-    "_RequiredFacetAttributeOutputTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalFacetAttributeOutputTypeDef = TypedDict(
-    "_OptionalFacetAttributeOutputTypeDef",
-    {
-        "AttributeDefinition": FacetAttributeDefinitionOutputTypeDef,
-        "AttributeReference": FacetAttributeReferenceTypeDef,
-        "RequiredBehavior": RequiredAttributeBehaviorType,
-    },
-    total=False,
-)
-
-
-class FacetAttributeOutputTypeDef(
-    _RequiredFacetAttributeOutputTypeDef, _OptionalFacetAttributeOutputTypeDef
-):
-    pass
-
-
-ListTypedLinkFacetAttributesResponseTypeDef = TypedDict(
-    "ListTypedLinkFacetAttributesResponseTypeDef",
-    {
-        "Attributes": List[TypedLinkAttributeDefinitionOutputTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 BatchLookupPolicyResponseTypeDef = TypedDict(
     "BatchLookupPolicyResponseTypeDef",
     {
         "PolicyToPathList": List[PolicyToPathTypeDef],
         "NextToken": str,
     },
     total=False,
@@ -2523,150 +2324,164 @@
 
 class TypedLinkAttributeDefinitionTypeDef(
     _RequiredTypedLinkAttributeDefinitionTypeDef, _OptionalTypedLinkAttributeDefinitionTypeDef
 ):
     pass
 
 
-BatchListAttachedIndicesResponseTypeDef = TypedDict(
-    "BatchListAttachedIndicesResponseTypeDef",
+_RequiredAddFacetToObjectRequestRequestTypeDef = TypedDict(
+    "_RequiredAddFacetToObjectRequestRequestTypeDef",
     {
-        "IndexAttachments": List[IndexAttachmentTypeDef],
-        "NextToken": str,
+        "DirectoryArn": str,
+        "SchemaFacet": SchemaFacetTypeDef,
+        "ObjectReference": ObjectReferenceTypeDef,
     },
-    total=False,
 )
-
-BatchListIndexResponseTypeDef = TypedDict(
-    "BatchListIndexResponseTypeDef",
+_OptionalAddFacetToObjectRequestRequestTypeDef = TypedDict(
+    "_OptionalAddFacetToObjectRequestRequestTypeDef",
     {
-        "IndexAttachments": List[IndexAttachmentTypeDef],
-        "NextToken": str,
+        "ObjectAttributeList": Sequence[AttributeKeyAndValueTypeDef],
     },
     total=False,
 )
 
-ListAttachedIndicesResponseTypeDef = TypedDict(
-    "ListAttachedIndicesResponseTypeDef",
+
+class AddFacetToObjectRequestRequestTypeDef(
+    _RequiredAddFacetToObjectRequestRequestTypeDef, _OptionalAddFacetToObjectRequestRequestTypeDef
+):
+    pass
+
+
+BatchAddFacetToObjectTypeDef = TypedDict(
+    "BatchAddFacetToObjectTypeDef",
     {
-        "IndexAttachments": List[IndexAttachmentTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "SchemaFacet": SchemaFacetTypeDef,
+        "ObjectAttributeList": Sequence[AttributeKeyAndValueTypeDef],
+        "ObjectReference": ObjectReferenceTypeDef,
     },
 )
 
-ListIndexResponseTypeDef = TypedDict(
-    "ListIndexResponseTypeDef",
+_RequiredBatchCreateObjectTypeDef = TypedDict(
+    "_RequiredBatchCreateObjectTypeDef",
     {
-        "IndexAttachments": List[IndexAttachmentTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "SchemaFacet": Sequence[SchemaFacetTypeDef],
+        "ObjectAttributeList": Sequence[AttributeKeyAndValueTypeDef],
     },
 )
-
-AttachTypedLinkResponseTypeDef = TypedDict(
-    "AttachTypedLinkResponseTypeDef",
+_OptionalBatchCreateObjectTypeDef = TypedDict(
+    "_OptionalBatchCreateObjectTypeDef",
     {
-        "TypedLinkSpecifier": TypedLinkSpecifierOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ParentReference": ObjectReferenceTypeDef,
+        "LinkName": str,
+        "BatchReferenceName": str,
     },
+    total=False,
 )
 
-BatchAttachTypedLinkResponseTypeDef = TypedDict(
-    "BatchAttachTypedLinkResponseTypeDef",
+
+class BatchCreateObjectTypeDef(
+    _RequiredBatchCreateObjectTypeDef, _OptionalBatchCreateObjectTypeDef
+):
+    pass
+
+
+BatchGetLinkAttributesResponseTypeDef = TypedDict(
+    "BatchGetLinkAttributesResponseTypeDef",
     {
-        "TypedLinkSpecifier": TypedLinkSpecifierOutputTypeDef,
+        "Attributes": List[AttributeKeyAndValueTypeDef],
     },
     total=False,
 )
 
-BatchListIncomingTypedLinksResponseTypeDef = TypedDict(
-    "BatchListIncomingTypedLinksResponseTypeDef",
+BatchGetObjectAttributesResponseTypeDef = TypedDict(
+    "BatchGetObjectAttributesResponseTypeDef",
     {
-        "LinkSpecifiers": List[TypedLinkSpecifierOutputTypeDef],
-        "NextToken": str,
+        "Attributes": List[AttributeKeyAndValueTypeDef],
     },
     total=False,
 )
 
-BatchListOutgoingTypedLinksResponseTypeDef = TypedDict(
-    "BatchListOutgoingTypedLinksResponseTypeDef",
+BatchListObjectAttributesResponseTypeDef = TypedDict(
+    "BatchListObjectAttributesResponseTypeDef",
     {
-        "TypedLinkSpecifiers": List[TypedLinkSpecifierOutputTypeDef],
+        "Attributes": List[AttributeKeyAndValueTypeDef],
         "NextToken": str,
     },
     total=False,
 )
 
-ListIncomingTypedLinksResponseTypeDef = TypedDict(
-    "ListIncomingTypedLinksResponseTypeDef",
+_RequiredCreateObjectRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateObjectRequestRequestTypeDef",
     {
-        "LinkSpecifiers": List[TypedLinkSpecifierOutputTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "DirectoryArn": str,
+        "SchemaFacets": Sequence[SchemaFacetTypeDef],
     },
 )
+_OptionalCreateObjectRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateObjectRequestRequestTypeDef",
+    {
+        "ObjectAttributeList": Sequence[AttributeKeyAndValueTypeDef],
+        "ParentReference": ObjectReferenceTypeDef,
+        "LinkName": str,
+    },
+    total=False,
+)
 
-ListOutgoingTypedLinksResponseTypeDef = TypedDict(
-    "ListOutgoingTypedLinksResponseTypeDef",
+
+class CreateObjectRequestRequestTypeDef(
+    _RequiredCreateObjectRequestRequestTypeDef, _OptionalCreateObjectRequestRequestTypeDef
+):
+    pass
+
+
+GetLinkAttributesResponseTypeDef = TypedDict(
+    "GetLinkAttributesResponseTypeDef",
     {
-        "TypedLinkSpecifiers": List[TypedLinkSpecifierOutputTypeDef],
-        "NextToken": str,
+        "Attributes": List[AttributeKeyAndValueTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListFacetAttributesResponseTypeDef = TypedDict(
-    "ListFacetAttributesResponseTypeDef",
+GetObjectAttributesResponseTypeDef = TypedDict(
+    "GetObjectAttributesResponseTypeDef",
     {
-        "Attributes": List[FacetAttributeOutputTypeDef],
-        "NextToken": str,
+        "Attributes": List[AttributeKeyAndValueTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AttributeKeyAndValueUnionTypeDef = Union[
-    AttributeKeyAndValueTypeDef, AttributeKeyAndValueOutputTypeDef
-]
-BatchAddFacetToObjectTypeDef = TypedDict(
-    "BatchAddFacetToObjectTypeDef",
+IndexAttachmentTypeDef = TypedDict(
+    "IndexAttachmentTypeDef",
     {
-        "SchemaFacet": SchemaFacetTypeDef,
-        "ObjectAttributeList": Sequence[AttributeKeyAndValueTypeDef],
-        "ObjectReference": ObjectReferenceTypeDef,
+        "IndexedAttributes": List[AttributeKeyAndValueTypeDef],
+        "ObjectIdentifier": str,
     },
+    total=False,
 )
 
-_RequiredBatchCreateObjectTypeDef = TypedDict(
-    "_RequiredBatchCreateObjectTypeDef",
+ListObjectAttributesResponseTypeDef = TypedDict(
+    "ListObjectAttributesResponseTypeDef",
     {
-        "SchemaFacet": Sequence[SchemaFacetTypeDef],
-        "ObjectAttributeList": Sequence[AttributeKeyAndValueTypeDef],
+        "Attributes": List[AttributeKeyAndValueTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalBatchCreateObjectTypeDef = TypedDict(
-    "_OptionalBatchCreateObjectTypeDef",
+
+AttachTypedLinkRequestRequestTypeDef = TypedDict(
+    "AttachTypedLinkRequestRequestTypeDef",
     {
-        "ParentReference": ObjectReferenceTypeDef,
-        "LinkName": str,
-        "BatchReferenceName": str,
+        "DirectoryArn": str,
+        "SourceObjectReference": ObjectReferenceTypeDef,
+        "TargetObjectReference": ObjectReferenceTypeDef,
+        "TypedLinkFacet": TypedLinkSchemaAndFacetNameTypeDef,
+        "Attributes": Sequence[AttributeNameAndValueTypeDef],
     },
-    total=False,
 )
 
-
-class BatchCreateObjectTypeDef(
-    _RequiredBatchCreateObjectTypeDef, _OptionalBatchCreateObjectTypeDef
-):
-    pass
-
-
-AttributeNameAndValueUnionTypeDef = Union[
-    AttributeNameAndValueTypeDef, AttributeNameAndValueOutputTypeDef
-]
 BatchAttachTypedLinkTypeDef = TypedDict(
     "BatchAttachTypedLinkTypeDef",
     {
         "SourceObjectReference": ObjectReferenceTypeDef,
         "TargetObjectReference": ObjectReferenceTypeDef,
         "TypedLinkFacet": TypedLinkSchemaAndFacetNameTypeDef,
         "Attributes": Sequence[AttributeNameAndValueTypeDef],
@@ -2675,15 +2490,15 @@
 
 TypedLinkSpecifierTypeDef = TypedDict(
     "TypedLinkSpecifierTypeDef",
     {
         "TypedLinkFacet": TypedLinkSchemaAndFacetNameTypeDef,
         "SourceObjectReference": ObjectReferenceTypeDef,
         "TargetObjectReference": ObjectReferenceTypeDef,
-        "IdentityAttributeValues": Sequence[AttributeNameAndValueTypeDef],
+        "IdentityAttributeValues": List[AttributeNameAndValueTypeDef],
     },
 )
 
 _RequiredFacetAttributeTypeDef = TypedDict(
     "_RequiredFacetAttributeTypeDef",
     {
         "Name": str,
@@ -2748,14 +2563,23 @@
 
 class TypedLinkAttributeRangeTypeDef(
     _RequiredTypedLinkAttributeRangeTypeDef, _OptionalTypedLinkAttributeRangeTypeDef
 ):
     pass
 
 
+ListTypedLinkFacetAttributesResponseTypeDef = TypedDict(
+    "ListTypedLinkFacetAttributesResponseTypeDef",
+    {
+        "Attributes": List[TypedLinkAttributeDefinitionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 TypedLinkFacetAttributeUpdateTypeDef = TypedDict(
     "TypedLinkFacetAttributeUpdateTypeDef",
     {
         "Attribute": TypedLinkAttributeDefinitionTypeDef,
         "Action": UpdateActionTypeType,
     },
 )
@@ -2765,113 +2589,64 @@
     {
         "Name": str,
         "Attributes": Sequence[TypedLinkAttributeDefinitionTypeDef],
         "IdentityAttributeOrder": Sequence[str],
     },
 )
 
-BatchWriteOperationResponseTypeDef = TypedDict(
-    "BatchWriteOperationResponseTypeDef",
+BatchListAttachedIndicesResponseTypeDef = TypedDict(
+    "BatchListAttachedIndicesResponseTypeDef",
     {
-        "CreateObject": BatchCreateObjectResponseTypeDef,
-        "AttachObject": BatchAttachObjectResponseTypeDef,
-        "DetachObject": BatchDetachObjectResponseTypeDef,
-        "UpdateObjectAttributes": BatchUpdateObjectAttributesResponseTypeDef,
-        "DeleteObject": Dict[str, Any],
-        "AddFacetToObject": Dict[str, Any],
-        "RemoveFacetFromObject": Dict[str, Any],
-        "AttachPolicy": Dict[str, Any],
-        "DetachPolicy": Dict[str, Any],
-        "CreateIndex": BatchCreateIndexResponseTypeDef,
-        "AttachToIndex": BatchAttachToIndexResponseTypeDef,
-        "DetachFromIndex": BatchDetachFromIndexResponseTypeDef,
-        "AttachTypedLink": BatchAttachTypedLinkResponseTypeDef,
-        "DetachTypedLink": Dict[str, Any],
-        "UpdateLinkAttributes": Dict[str, Any],
+        "IndexAttachments": List[IndexAttachmentTypeDef],
+        "NextToken": str,
     },
     total=False,
 )
 
-BatchReadSuccessfulResponseTypeDef = TypedDict(
-    "BatchReadSuccessfulResponseTypeDef",
+BatchListIndexResponseTypeDef = TypedDict(
+    "BatchListIndexResponseTypeDef",
     {
-        "ListObjectAttributes": BatchListObjectAttributesResponseTypeDef,
-        "ListObjectChildren": BatchListObjectChildrenResponseTypeDef,
-        "GetObjectInformation": BatchGetObjectInformationResponseTypeDef,
-        "GetObjectAttributes": BatchGetObjectAttributesResponseTypeDef,
-        "ListAttachedIndices": BatchListAttachedIndicesResponseTypeDef,
-        "ListObjectParentPaths": BatchListObjectParentPathsResponseTypeDef,
-        "ListObjectPolicies": BatchListObjectPoliciesResponseTypeDef,
-        "ListPolicyAttachments": BatchListPolicyAttachmentsResponseTypeDef,
-        "LookupPolicy": BatchLookupPolicyResponseTypeDef,
-        "ListIndex": BatchListIndexResponseTypeDef,
-        "ListOutgoingTypedLinks": BatchListOutgoingTypedLinksResponseTypeDef,
-        "ListIncomingTypedLinks": BatchListIncomingTypedLinksResponseTypeDef,
-        "GetLinkAttributes": BatchGetLinkAttributesResponseTypeDef,
-        "ListObjectParents": BatchListObjectParentsResponseTypeDef,
+        "IndexAttachments": List[IndexAttachmentTypeDef],
+        "NextToken": str,
     },
     total=False,
 )
 
-_RequiredAddFacetToObjectRequestRequestTypeDef = TypedDict(
-    "_RequiredAddFacetToObjectRequestRequestTypeDef",
-    {
-        "DirectoryArn": str,
-        "SchemaFacet": SchemaFacetTypeDef,
-        "ObjectReference": ObjectReferenceTypeDef,
-    },
-)
-_OptionalAddFacetToObjectRequestRequestTypeDef = TypedDict(
-    "_OptionalAddFacetToObjectRequestRequestTypeDef",
+ListAttachedIndicesResponseTypeDef = TypedDict(
+    "ListAttachedIndicesResponseTypeDef",
     {
-        "ObjectAttributeList": Sequence[AttributeKeyAndValueUnionTypeDef],
+        "IndexAttachments": List[IndexAttachmentTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class AddFacetToObjectRequestRequestTypeDef(
-    _RequiredAddFacetToObjectRequestRequestTypeDef, _OptionalAddFacetToObjectRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredCreateObjectRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateObjectRequestRequestTypeDef",
+ListIndexResponseTypeDef = TypedDict(
+    "ListIndexResponseTypeDef",
     {
-        "DirectoryArn": str,
-        "SchemaFacets": Sequence[SchemaFacetTypeDef],
+        "IndexAttachments": List[IndexAttachmentTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalCreateObjectRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateObjectRequestRequestTypeDef",
+
+AttachTypedLinkResponseTypeDef = TypedDict(
+    "AttachTypedLinkResponseTypeDef",
     {
-        "ObjectAttributeList": Sequence[AttributeKeyAndValueUnionTypeDef],
-        "ParentReference": ObjectReferenceTypeDef,
-        "LinkName": str,
+        "TypedLinkSpecifier": TypedLinkSpecifierTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class CreateObjectRequestRequestTypeDef(
-    _RequiredCreateObjectRequestRequestTypeDef, _OptionalCreateObjectRequestRequestTypeDef
-):
-    pass
-
-
-AttachTypedLinkRequestRequestTypeDef = TypedDict(
-    "AttachTypedLinkRequestRequestTypeDef",
+BatchAttachTypedLinkResponseTypeDef = TypedDict(
+    "BatchAttachTypedLinkResponseTypeDef",
     {
-        "DirectoryArn": str,
-        "SourceObjectReference": ObjectReferenceTypeDef,
-        "TargetObjectReference": ObjectReferenceTypeDef,
-        "TypedLinkFacet": TypedLinkSchemaAndFacetNameTypeDef,
-        "Attributes": Sequence[AttributeNameAndValueUnionTypeDef],
+        "TypedLinkSpecifier": TypedLinkSpecifierTypeDef,
     },
+    total=False,
 )
 
 BatchDetachTypedLinkTypeDef = TypedDict(
     "BatchDetachTypedLinkTypeDef",
     {
         "TypedLinkSpecifier": TypedLinkSpecifierTypeDef,
     },
@@ -2881,14 +2656,32 @@
     "BatchGetLinkAttributesTypeDef",
     {
         "TypedLinkSpecifier": TypedLinkSpecifierTypeDef,
         "AttributeNames": Sequence[str],
     },
 )
 
+BatchListIncomingTypedLinksResponseTypeDef = TypedDict(
+    "BatchListIncomingTypedLinksResponseTypeDef",
+    {
+        "LinkSpecifiers": List[TypedLinkSpecifierTypeDef],
+        "NextToken": str,
+    },
+    total=False,
+)
+
+BatchListOutgoingTypedLinksResponseTypeDef = TypedDict(
+    "BatchListOutgoingTypedLinksResponseTypeDef",
+    {
+        "TypedLinkSpecifiers": List[TypedLinkSpecifierTypeDef],
+        "NextToken": str,
+    },
+    total=False,
+)
+
 DetachTypedLinkRequestRequestTypeDef = TypedDict(
     "DetachTypedLinkRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "TypedLinkSpecifier": TypedLinkSpecifierTypeDef,
     },
 )
@@ -2912,25 +2705,74 @@
 
 class GetLinkAttributesRequestRequestTypeDef(
     _RequiredGetLinkAttributesRequestRequestTypeDef, _OptionalGetLinkAttributesRequestRequestTypeDef
 ):
     pass
 
 
-TypedLinkSpecifierUnionTypeDef = Union[TypedLinkSpecifierTypeDef, TypedLinkSpecifierOutputTypeDef]
-FacetAttributeUnionTypeDef = Union[FacetAttributeTypeDef, FacetAttributeOutputTypeDef]
+ListIncomingTypedLinksResponseTypeDef = TypedDict(
+    "ListIncomingTypedLinksResponseTypeDef",
+    {
+        "LinkSpecifiers": List[TypedLinkSpecifierTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListOutgoingTypedLinksResponseTypeDef = TypedDict(
+    "ListOutgoingTypedLinksResponseTypeDef",
+    {
+        "TypedLinkSpecifiers": List[TypedLinkSpecifierTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCreateFacetRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateFacetRequestRequestTypeDef",
+    {
+        "SchemaArn": str,
+        "Name": str,
+    },
+)
+_OptionalCreateFacetRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateFacetRequestRequestTypeDef",
+    {
+        "Attributes": Sequence[FacetAttributeTypeDef],
+        "ObjectType": ObjectTypeType,
+        "FacetStyle": FacetStyleType,
+    },
+    total=False,
+)
+
+
+class CreateFacetRequestRequestTypeDef(
+    _RequiredCreateFacetRequestRequestTypeDef, _OptionalCreateFacetRequestRequestTypeDef
+):
+    pass
+
+
 FacetAttributeUpdateTypeDef = TypedDict(
     "FacetAttributeUpdateTypeDef",
     {
         "Attribute": FacetAttributeTypeDef,
         "Action": UpdateActionTypeType,
     },
     total=False,
 )
 
+ListFacetAttributesResponseTypeDef = TypedDict(
+    "ListFacetAttributesResponseTypeDef",
+    {
+        "Attributes": List[FacetAttributeTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 BatchUpdateLinkAttributesTypeDef = TypedDict(
     "BatchUpdateLinkAttributesTypeDef",
     {
         "TypedLinkSpecifier": TypedLinkSpecifierTypeDef,
         "AttributeUpdates": Sequence[LinkAttributeUpdateTypeDef],
     },
 )
@@ -3200,55 +3042,57 @@
     "CreateTypedLinkFacetRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "Facet": TypedLinkFacetTypeDef,
     },
 )
 
-BatchWriteResponseTypeDef = TypedDict(
-    "BatchWriteResponseTypeDef",
-    {
-        "Responses": List[BatchWriteOperationResponseTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-BatchReadOperationResponseTypeDef = TypedDict(
-    "BatchReadOperationResponseTypeDef",
+BatchWriteOperationResponseTypeDef = TypedDict(
+    "BatchWriteOperationResponseTypeDef",
     {
-        "SuccessfulResponse": BatchReadSuccessfulResponseTypeDef,
-        "ExceptionResponse": BatchReadExceptionTypeDef,
+        "CreateObject": BatchCreateObjectResponseTypeDef,
+        "AttachObject": BatchAttachObjectResponseTypeDef,
+        "DetachObject": BatchDetachObjectResponseTypeDef,
+        "UpdateObjectAttributes": BatchUpdateObjectAttributesResponseTypeDef,
+        "DeleteObject": Dict[str, Any],
+        "AddFacetToObject": Dict[str, Any],
+        "RemoveFacetFromObject": Dict[str, Any],
+        "AttachPolicy": Dict[str, Any],
+        "DetachPolicy": Dict[str, Any],
+        "CreateIndex": BatchCreateIndexResponseTypeDef,
+        "AttachToIndex": BatchAttachToIndexResponseTypeDef,
+        "DetachFromIndex": BatchDetachFromIndexResponseTypeDef,
+        "AttachTypedLink": BatchAttachTypedLinkResponseTypeDef,
+        "DetachTypedLink": Dict[str, Any],
+        "UpdateLinkAttributes": Dict[str, Any],
     },
     total=False,
 )
 
-_RequiredCreateFacetRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateFacetRequestRequestTypeDef",
-    {
-        "SchemaArn": str,
-        "Name": str,
-    },
-)
-_OptionalCreateFacetRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateFacetRequestRequestTypeDef",
+BatchReadSuccessfulResponseTypeDef = TypedDict(
+    "BatchReadSuccessfulResponseTypeDef",
     {
-        "Attributes": Sequence[FacetAttributeUnionTypeDef],
-        "ObjectType": ObjectTypeType,
-        "FacetStyle": FacetStyleType,
+        "ListObjectAttributes": BatchListObjectAttributesResponseTypeDef,
+        "ListObjectChildren": BatchListObjectChildrenResponseTypeDef,
+        "GetObjectInformation": BatchGetObjectInformationResponseTypeDef,
+        "GetObjectAttributes": BatchGetObjectAttributesResponseTypeDef,
+        "ListAttachedIndices": BatchListAttachedIndicesResponseTypeDef,
+        "ListObjectParentPaths": BatchListObjectParentPathsResponseTypeDef,
+        "ListObjectPolicies": BatchListObjectPoliciesResponseTypeDef,
+        "ListPolicyAttachments": BatchListPolicyAttachmentsResponseTypeDef,
+        "LookupPolicy": BatchLookupPolicyResponseTypeDef,
+        "ListIndex": BatchListIndexResponseTypeDef,
+        "ListOutgoingTypedLinks": BatchListOutgoingTypedLinksResponseTypeDef,
+        "ListIncomingTypedLinks": BatchListIncomingTypedLinksResponseTypeDef,
+        "GetLinkAttributes": BatchGetLinkAttributesResponseTypeDef,
+        "ListObjectParents": BatchListObjectParentsResponseTypeDef,
     },
     total=False,
 )
 
-
-class CreateFacetRequestRequestTypeDef(
-    _RequiredCreateFacetRequestRequestTypeDef, _OptionalCreateFacetRequestRequestTypeDef
-):
-    pass
-
-
 _RequiredUpdateFacetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFacetRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "Name": str,
     },
 )
@@ -3307,22 +3151,31 @@
         "ListOutgoingTypedLinks": BatchListOutgoingTypedLinksTypeDef,
         "ListIncomingTypedLinks": BatchListIncomingTypedLinksTypeDef,
         "GetLinkAttributes": BatchGetLinkAttributesTypeDef,
     },
     total=False,
 )
 
-BatchReadResponseTypeDef = TypedDict(
-    "BatchReadResponseTypeDef",
+BatchWriteResponseTypeDef = TypedDict(
+    "BatchWriteResponseTypeDef",
     {
-        "Responses": List[BatchReadOperationResponseTypeDef],
+        "Responses": List[BatchWriteOperationResponseTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+BatchReadOperationResponseTypeDef = TypedDict(
+    "BatchReadOperationResponseTypeDef",
+    {
+        "SuccessfulResponse": BatchReadSuccessfulResponseTypeDef,
+        "ExceptionResponse": BatchReadExceptionTypeDef,
+    },
+    total=False,
+)
+
 BatchWriteRequestRequestTypeDef = TypedDict(
     "BatchWriteRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "Operations": Sequence[BatchWriteOperationTypeDef],
     },
 )
@@ -3343,7 +3196,16 @@
 )
 
 
 class BatchReadRequestRequestTypeDef(
     _RequiredBatchReadRequestRequestTypeDef, _OptionalBatchReadRequestRequestTypeDef
 ):
     pass
+
+
+BatchReadResponseTypeDef = TypedDict(
+    "BatchReadResponseTypeDef",
+    {
+        "Responses": List[BatchReadOperationResponseTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory/type_defs.pyi` & `types-aiobotocore-clouddirectory-2.5.2.post2/types_aiobotocore_clouddirectory/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,14 @@
 __all__ = (
     "ObjectReferenceTypeDef",
     "SchemaFacetTypeDef",
     "ApplySchemaRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "TypedLinkSchemaAndFacetNameTypeDef",
     "AttributeKeyTypeDef",
-    "TypedAttributeValueOutputTypeDef",
     "BatchAttachObjectResponseTypeDef",
     "BatchAttachToIndexResponseTypeDef",
     "BatchCreateIndexResponseTypeDef",
     "BatchCreateObjectResponseTypeDef",
     "BatchDetachFromIndexResponseTypeDef",
     "BatchDetachObjectResponseTypeDef",
     "BatchListObjectChildrenResponseTypeDef",
@@ -62,15 +61,14 @@
     "DeleteDirectoryRequestRequestTypeDef",
     "DeleteFacetRequestRequestTypeDef",
     "DeleteSchemaRequestRequestTypeDef",
     "DeleteTypedLinkFacetRequestRequestTypeDef",
     "DirectoryTypeDef",
     "DisableDirectoryRequestRequestTypeDef",
     "EnableDirectoryRequestRequestTypeDef",
-    "RuleOutputTypeDef",
     "RuleTypeDef",
     "FacetAttributeReferenceTypeDef",
     "FacetTypeDef",
     "GetAppliedSchemaVersionRequestRequestTypeDef",
     "GetDirectoryRequestRequestTypeDef",
     "GetFacetRequestRequestTypeDef",
     "GetSchemaAsJsonRequestRequestTypeDef",
@@ -163,24 +161,20 @@
     "PutSchemaFromJsonResponseTypeDef",
     "UpdateObjectAttributesResponseTypeDef",
     "UpdateSchemaResponseTypeDef",
     "UpgradeAppliedSchemaResponseTypeDef",
     "UpgradePublishedSchemaResponseTypeDef",
     "BatchCreateIndexTypeDef",
     "CreateIndexRequestRequestTypeDef",
-    "AttributeKeyAndValueOutputTypeDef",
-    "AttributeNameAndValueOutputTypeDef",
     "BatchListObjectParentPathsResponseTypeDef",
     "ListObjectParentPathsResponseTypeDef",
     "BatchListObjectParentsResponseTypeDef",
     "ListObjectParentsResponseTypeDef",
     "GetDirectoryResponseTypeDef",
     "ListDirectoriesResponseTypeDef",
-    "FacetAttributeDefinitionOutputTypeDef",
-    "TypedLinkAttributeDefinitionOutputTypeDef",
     "GetFacetResponseTypeDef",
     "ListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef",
     "ListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef",
     "ListDevelopmentSchemaArnsRequestListDevelopmentSchemaArnsPaginateTypeDef",
     "ListDirectoriesRequestListDirectoriesPaginateTypeDef",
     "ListFacetAttributesRequestListFacetAttributesPaginateTypeDef",
     "ListFacetNamesRequestListFacetNamesPaginateTypeDef",
@@ -194,69 +188,62 @@
     "ListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef",
     "ListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef",
     "LookupPolicyRequestLookupPolicyPaginateTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "PolicyToPathTypeDef",
     "TypedAttributeValueTypeDef",
-    "BatchGetLinkAttributesResponseTypeDef",
-    "BatchGetObjectAttributesResponseTypeDef",
-    "BatchListObjectAttributesResponseTypeDef",
-    "GetLinkAttributesResponseTypeDef",
-    "GetObjectAttributesResponseTypeDef",
-    "IndexAttachmentTypeDef",
-    "ListObjectAttributesResponseTypeDef",
-    "TypedLinkSpecifierOutputTypeDef",
-    "FacetAttributeOutputTypeDef",
-    "ListTypedLinkFacetAttributesResponseTypeDef",
     "BatchLookupPolicyResponseTypeDef",
     "LookupPolicyResponseTypeDef",
     "AttributeKeyAndValueTypeDef",
     "AttributeNameAndValueTypeDef",
     "FacetAttributeDefinitionTypeDef",
     "LinkAttributeActionTypeDef",
     "ObjectAttributeActionTypeDef",
     "TypedAttributeValueRangeTypeDef",
     "TypedLinkAttributeDefinitionTypeDef",
-    "BatchListAttachedIndicesResponseTypeDef",
-    "BatchListIndexResponseTypeDef",
-    "ListAttachedIndicesResponseTypeDef",
-    "ListIndexResponseTypeDef",
-    "AttachTypedLinkResponseTypeDef",
-    "BatchAttachTypedLinkResponseTypeDef",
-    "BatchListIncomingTypedLinksResponseTypeDef",
-    "BatchListOutgoingTypedLinksResponseTypeDef",
-    "ListIncomingTypedLinksResponseTypeDef",
-    "ListOutgoingTypedLinksResponseTypeDef",
-    "ListFacetAttributesResponseTypeDef",
-    "AttributeKeyAndValueUnionTypeDef",
+    "AddFacetToObjectRequestRequestTypeDef",
     "BatchAddFacetToObjectTypeDef",
     "BatchCreateObjectTypeDef",
-    "AttributeNameAndValueUnionTypeDef",
+    "BatchGetLinkAttributesResponseTypeDef",
+    "BatchGetObjectAttributesResponseTypeDef",
+    "BatchListObjectAttributesResponseTypeDef",
+    "CreateObjectRequestRequestTypeDef",
+    "GetLinkAttributesResponseTypeDef",
+    "GetObjectAttributesResponseTypeDef",
+    "IndexAttachmentTypeDef",
+    "ListObjectAttributesResponseTypeDef",
+    "AttachTypedLinkRequestRequestTypeDef",
     "BatchAttachTypedLinkTypeDef",
     "TypedLinkSpecifierTypeDef",
     "FacetAttributeTypeDef",
     "LinkAttributeUpdateTypeDef",
     "ObjectAttributeUpdateTypeDef",
     "ObjectAttributeRangeTypeDef",
     "TypedLinkAttributeRangeTypeDef",
+    "ListTypedLinkFacetAttributesResponseTypeDef",
     "TypedLinkFacetAttributeUpdateTypeDef",
     "TypedLinkFacetTypeDef",
-    "BatchWriteOperationResponseTypeDef",
-    "BatchReadSuccessfulResponseTypeDef",
-    "AddFacetToObjectRequestRequestTypeDef",
-    "CreateObjectRequestRequestTypeDef",
-    "AttachTypedLinkRequestRequestTypeDef",
+    "BatchListAttachedIndicesResponseTypeDef",
+    "BatchListIndexResponseTypeDef",
+    "ListAttachedIndicesResponseTypeDef",
+    "ListIndexResponseTypeDef",
+    "AttachTypedLinkResponseTypeDef",
+    "BatchAttachTypedLinkResponseTypeDef",
     "BatchDetachTypedLinkTypeDef",
     "BatchGetLinkAttributesTypeDef",
+    "BatchListIncomingTypedLinksResponseTypeDef",
+    "BatchListOutgoingTypedLinksResponseTypeDef",
     "DetachTypedLinkRequestRequestTypeDef",
     "GetLinkAttributesRequestRequestTypeDef",
-    "TypedLinkSpecifierUnionTypeDef",
-    "FacetAttributeUnionTypeDef",
+    "ListIncomingTypedLinksResponseTypeDef",
+    "ListOutgoingTypedLinksResponseTypeDef",
+    "CreateFacetRequestRequestTypeDef",
     "FacetAttributeUpdateTypeDef",
+    "ListFacetAttributesResponseTypeDef",
     "BatchUpdateLinkAttributesTypeDef",
     "UpdateLinkAttributesRequestRequestTypeDef",
     "BatchUpdateObjectAttributesTypeDef",
     "UpdateObjectAttributesRequestRequestTypeDef",
     "BatchListIndexTypeDef",
     "ListIndexRequestListIndexPaginateTypeDef",
     "ListIndexRequestRequestTypeDef",
@@ -264,23 +251,24 @@
     "BatchListOutgoingTypedLinksTypeDef",
     "ListIncomingTypedLinksRequestListIncomingTypedLinksPaginateTypeDef",
     "ListIncomingTypedLinksRequestRequestTypeDef",
     "ListOutgoingTypedLinksRequestListOutgoingTypedLinksPaginateTypeDef",
     "ListOutgoingTypedLinksRequestRequestTypeDef",
     "UpdateTypedLinkFacetRequestRequestTypeDef",
     "CreateTypedLinkFacetRequestRequestTypeDef",
-    "BatchWriteResponseTypeDef",
-    "BatchReadOperationResponseTypeDef",
-    "CreateFacetRequestRequestTypeDef",
+    "BatchWriteOperationResponseTypeDef",
+    "BatchReadSuccessfulResponseTypeDef",
     "UpdateFacetRequestRequestTypeDef",
     "BatchWriteOperationTypeDef",
     "BatchReadOperationTypeDef",
-    "BatchReadResponseTypeDef",
+    "BatchWriteResponseTypeDef",
+    "BatchReadOperationResponseTypeDef",
     "BatchWriteRequestRequestTypeDef",
     "BatchReadRequestRequestTypeDef",
+    "BatchReadResponseTypeDef",
 )
 
 ObjectReferenceTypeDef = TypedDict(
     "ObjectReferenceTypeDef",
     {
         "Selector": str,
     },
@@ -328,26 +316,14 @@
     {
         "SchemaArn": str,
         "FacetName": str,
         "Name": str,
     },
 )
 
-TypedAttributeValueOutputTypeDef = TypedDict(
-    "TypedAttributeValueOutputTypeDef",
-    {
-        "StringValue": str,
-        "BinaryValue": bytes,
-        "BooleanValue": bool,
-        "NumberValue": str,
-        "DatetimeValue": datetime,
-    },
-    total=False,
-)
-
 BatchAttachObjectResponseTypeDef = TypedDict(
     "BatchAttachObjectResponseTypeDef",
     {
         "attachedObjectIdentifier": str,
     },
     total=False,
 )
@@ -521,23 +497,14 @@
 EnableDirectoryRequestRequestTypeDef = TypedDict(
     "EnableDirectoryRequestRequestTypeDef",
     {
         "DirectoryArn": str,
     },
 )
 
-RuleOutputTypeDef = TypedDict(
-    "RuleOutputTypeDef",
-    {
-        "Type": RuleTypeType,
-        "Parameters": Dict[str, str],
-    },
-    total=False,
-)
-
 RuleTypeDef = TypedDict(
     "RuleTypeDef",
     {
         "Type": RuleTypeType,
         "Parameters": Mapping[str, str],
     },
     total=False,
@@ -1760,30 +1727,14 @@
 )
 
 class CreateIndexRequestRequestTypeDef(
     _RequiredCreateIndexRequestRequestTypeDef, _OptionalCreateIndexRequestRequestTypeDef
 ):
     pass
 
-AttributeKeyAndValueOutputTypeDef = TypedDict(
-    "AttributeKeyAndValueOutputTypeDef",
-    {
-        "Key": AttributeKeyTypeDef,
-        "Value": TypedAttributeValueOutputTypeDef,
-    },
-)
-
-AttributeNameAndValueOutputTypeDef = TypedDict(
-    "AttributeNameAndValueOutputTypeDef",
-    {
-        "AttributeName": str,
-        "Value": TypedAttributeValueOutputTypeDef,
-    },
-)
-
 BatchListObjectParentPathsResponseTypeDef = TypedDict(
     "BatchListObjectParentPathsResponseTypeDef",
     {
         "PathToObjectIdentifiersList": List[PathToObjectIdentifiersTypeDef],
         "NextToken": str,
     },
     total=False,
@@ -1830,59 +1781,14 @@
     {
         "Directories": List[DirectoryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredFacetAttributeDefinitionOutputTypeDef = TypedDict(
-    "_RequiredFacetAttributeDefinitionOutputTypeDef",
-    {
-        "Type": FacetAttributeTypeType,
-    },
-)
-_OptionalFacetAttributeDefinitionOutputTypeDef = TypedDict(
-    "_OptionalFacetAttributeDefinitionOutputTypeDef",
-    {
-        "DefaultValue": TypedAttributeValueOutputTypeDef,
-        "IsImmutable": bool,
-        "Rules": Dict[str, RuleOutputTypeDef],
-    },
-    total=False,
-)
-
-class FacetAttributeDefinitionOutputTypeDef(
-    _RequiredFacetAttributeDefinitionOutputTypeDef, _OptionalFacetAttributeDefinitionOutputTypeDef
-):
-    pass
-
-_RequiredTypedLinkAttributeDefinitionOutputTypeDef = TypedDict(
-    "_RequiredTypedLinkAttributeDefinitionOutputTypeDef",
-    {
-        "Name": str,
-        "Type": FacetAttributeTypeType,
-        "RequiredBehavior": RequiredAttributeBehaviorType,
-    },
-)
-_OptionalTypedLinkAttributeDefinitionOutputTypeDef = TypedDict(
-    "_OptionalTypedLinkAttributeDefinitionOutputTypeDef",
-    {
-        "DefaultValue": TypedAttributeValueOutputTypeDef,
-        "IsImmutable": bool,
-        "Rules": Dict[str, RuleOutputTypeDef],
-    },
-    total=False,
-)
-
-class TypedLinkAttributeDefinitionOutputTypeDef(
-    _RequiredTypedLinkAttributeDefinitionOutputTypeDef,
-    _OptionalTypedLinkAttributeDefinitionOutputTypeDef,
-):
-    pass
-
 GetFacetResponseTypeDef = TypedDict(
     "GetFacetResponseTypeDef",
     {
         "Facet": FacetTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2210,113 +2116,14 @@
         "BooleanValue": bool,
         "NumberValue": str,
         "DatetimeValue": TimestampTypeDef,
     },
     total=False,
 )
 
-BatchGetLinkAttributesResponseTypeDef = TypedDict(
-    "BatchGetLinkAttributesResponseTypeDef",
-    {
-        "Attributes": List[AttributeKeyAndValueOutputTypeDef],
-    },
-    total=False,
-)
-
-BatchGetObjectAttributesResponseTypeDef = TypedDict(
-    "BatchGetObjectAttributesResponseTypeDef",
-    {
-        "Attributes": List[AttributeKeyAndValueOutputTypeDef],
-    },
-    total=False,
-)
-
-BatchListObjectAttributesResponseTypeDef = TypedDict(
-    "BatchListObjectAttributesResponseTypeDef",
-    {
-        "Attributes": List[AttributeKeyAndValueOutputTypeDef],
-        "NextToken": str,
-    },
-    total=False,
-)
-
-GetLinkAttributesResponseTypeDef = TypedDict(
-    "GetLinkAttributesResponseTypeDef",
-    {
-        "Attributes": List[AttributeKeyAndValueOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetObjectAttributesResponseTypeDef = TypedDict(
-    "GetObjectAttributesResponseTypeDef",
-    {
-        "Attributes": List[AttributeKeyAndValueOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-IndexAttachmentTypeDef = TypedDict(
-    "IndexAttachmentTypeDef",
-    {
-        "IndexedAttributes": List[AttributeKeyAndValueOutputTypeDef],
-        "ObjectIdentifier": str,
-    },
-    total=False,
-)
-
-ListObjectAttributesResponseTypeDef = TypedDict(
-    "ListObjectAttributesResponseTypeDef",
-    {
-        "Attributes": List[AttributeKeyAndValueOutputTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-TypedLinkSpecifierOutputTypeDef = TypedDict(
-    "TypedLinkSpecifierOutputTypeDef",
-    {
-        "TypedLinkFacet": TypedLinkSchemaAndFacetNameTypeDef,
-        "SourceObjectReference": ObjectReferenceTypeDef,
-        "TargetObjectReference": ObjectReferenceTypeDef,
-        "IdentityAttributeValues": List[AttributeNameAndValueOutputTypeDef],
-    },
-)
-
-_RequiredFacetAttributeOutputTypeDef = TypedDict(
-    "_RequiredFacetAttributeOutputTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalFacetAttributeOutputTypeDef = TypedDict(
-    "_OptionalFacetAttributeOutputTypeDef",
-    {
-        "AttributeDefinition": FacetAttributeDefinitionOutputTypeDef,
-        "AttributeReference": FacetAttributeReferenceTypeDef,
-        "RequiredBehavior": RequiredAttributeBehaviorType,
-    },
-    total=False,
-)
-
-class FacetAttributeOutputTypeDef(
-    _RequiredFacetAttributeOutputTypeDef, _OptionalFacetAttributeOutputTypeDef
-):
-    pass
-
-ListTypedLinkFacetAttributesResponseTypeDef = TypedDict(
-    "ListTypedLinkFacetAttributesResponseTypeDef",
-    {
-        "Attributes": List[TypedLinkAttributeDefinitionOutputTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 BatchLookupPolicyResponseTypeDef = TypedDict(
     "BatchLookupPolicyResponseTypeDef",
     {
         "PolicyToPathList": List[PolicyToPathTypeDef],
         "NextToken": str,
     },
     total=False,
@@ -2426,148 +2233,158 @@
 )
 
 class TypedLinkAttributeDefinitionTypeDef(
     _RequiredTypedLinkAttributeDefinitionTypeDef, _OptionalTypedLinkAttributeDefinitionTypeDef
 ):
     pass
 
-BatchListAttachedIndicesResponseTypeDef = TypedDict(
-    "BatchListAttachedIndicesResponseTypeDef",
+_RequiredAddFacetToObjectRequestRequestTypeDef = TypedDict(
+    "_RequiredAddFacetToObjectRequestRequestTypeDef",
     {
-        "IndexAttachments": List[IndexAttachmentTypeDef],
-        "NextToken": str,
+        "DirectoryArn": str,
+        "SchemaFacet": SchemaFacetTypeDef,
+        "ObjectReference": ObjectReferenceTypeDef,
     },
-    total=False,
 )
-
-BatchListIndexResponseTypeDef = TypedDict(
-    "BatchListIndexResponseTypeDef",
+_OptionalAddFacetToObjectRequestRequestTypeDef = TypedDict(
+    "_OptionalAddFacetToObjectRequestRequestTypeDef",
     {
-        "IndexAttachments": List[IndexAttachmentTypeDef],
-        "NextToken": str,
+        "ObjectAttributeList": Sequence[AttributeKeyAndValueTypeDef],
     },
     total=False,
 )
 
-ListAttachedIndicesResponseTypeDef = TypedDict(
-    "ListAttachedIndicesResponseTypeDef",
+class AddFacetToObjectRequestRequestTypeDef(
+    _RequiredAddFacetToObjectRequestRequestTypeDef, _OptionalAddFacetToObjectRequestRequestTypeDef
+):
+    pass
+
+BatchAddFacetToObjectTypeDef = TypedDict(
+    "BatchAddFacetToObjectTypeDef",
     {
-        "IndexAttachments": List[IndexAttachmentTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "SchemaFacet": SchemaFacetTypeDef,
+        "ObjectAttributeList": Sequence[AttributeKeyAndValueTypeDef],
+        "ObjectReference": ObjectReferenceTypeDef,
     },
 )
 
-ListIndexResponseTypeDef = TypedDict(
-    "ListIndexResponseTypeDef",
+_RequiredBatchCreateObjectTypeDef = TypedDict(
+    "_RequiredBatchCreateObjectTypeDef",
     {
-        "IndexAttachments": List[IndexAttachmentTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "SchemaFacet": Sequence[SchemaFacetTypeDef],
+        "ObjectAttributeList": Sequence[AttributeKeyAndValueTypeDef],
     },
 )
-
-AttachTypedLinkResponseTypeDef = TypedDict(
-    "AttachTypedLinkResponseTypeDef",
+_OptionalBatchCreateObjectTypeDef = TypedDict(
+    "_OptionalBatchCreateObjectTypeDef",
     {
-        "TypedLinkSpecifier": TypedLinkSpecifierOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ParentReference": ObjectReferenceTypeDef,
+        "LinkName": str,
+        "BatchReferenceName": str,
     },
+    total=False,
 )
 
-BatchAttachTypedLinkResponseTypeDef = TypedDict(
-    "BatchAttachTypedLinkResponseTypeDef",
+class BatchCreateObjectTypeDef(
+    _RequiredBatchCreateObjectTypeDef, _OptionalBatchCreateObjectTypeDef
+):
+    pass
+
+BatchGetLinkAttributesResponseTypeDef = TypedDict(
+    "BatchGetLinkAttributesResponseTypeDef",
     {
-        "TypedLinkSpecifier": TypedLinkSpecifierOutputTypeDef,
+        "Attributes": List[AttributeKeyAndValueTypeDef],
     },
     total=False,
 )
 
-BatchListIncomingTypedLinksResponseTypeDef = TypedDict(
-    "BatchListIncomingTypedLinksResponseTypeDef",
+BatchGetObjectAttributesResponseTypeDef = TypedDict(
+    "BatchGetObjectAttributesResponseTypeDef",
     {
-        "LinkSpecifiers": List[TypedLinkSpecifierOutputTypeDef],
-        "NextToken": str,
+        "Attributes": List[AttributeKeyAndValueTypeDef],
     },
     total=False,
 )
 
-BatchListOutgoingTypedLinksResponseTypeDef = TypedDict(
-    "BatchListOutgoingTypedLinksResponseTypeDef",
+BatchListObjectAttributesResponseTypeDef = TypedDict(
+    "BatchListObjectAttributesResponseTypeDef",
     {
-        "TypedLinkSpecifiers": List[TypedLinkSpecifierOutputTypeDef],
+        "Attributes": List[AttributeKeyAndValueTypeDef],
         "NextToken": str,
     },
     total=False,
 )
 
-ListIncomingTypedLinksResponseTypeDef = TypedDict(
-    "ListIncomingTypedLinksResponseTypeDef",
+_RequiredCreateObjectRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateObjectRequestRequestTypeDef",
     {
-        "LinkSpecifiers": List[TypedLinkSpecifierOutputTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "DirectoryArn": str,
+        "SchemaFacets": Sequence[SchemaFacetTypeDef],
+    },
+)
+_OptionalCreateObjectRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateObjectRequestRequestTypeDef",
+    {
+        "ObjectAttributeList": Sequence[AttributeKeyAndValueTypeDef],
+        "ParentReference": ObjectReferenceTypeDef,
+        "LinkName": str,
     },
+    total=False,
 )
 
-ListOutgoingTypedLinksResponseTypeDef = TypedDict(
-    "ListOutgoingTypedLinksResponseTypeDef",
+class CreateObjectRequestRequestTypeDef(
+    _RequiredCreateObjectRequestRequestTypeDef, _OptionalCreateObjectRequestRequestTypeDef
+):
+    pass
+
+GetLinkAttributesResponseTypeDef = TypedDict(
+    "GetLinkAttributesResponseTypeDef",
     {
-        "TypedLinkSpecifiers": List[TypedLinkSpecifierOutputTypeDef],
-        "NextToken": str,
+        "Attributes": List[AttributeKeyAndValueTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListFacetAttributesResponseTypeDef = TypedDict(
-    "ListFacetAttributesResponseTypeDef",
+GetObjectAttributesResponseTypeDef = TypedDict(
+    "GetObjectAttributesResponseTypeDef",
     {
-        "Attributes": List[FacetAttributeOutputTypeDef],
-        "NextToken": str,
+        "Attributes": List[AttributeKeyAndValueTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AttributeKeyAndValueUnionTypeDef = Union[
-    AttributeKeyAndValueTypeDef, AttributeKeyAndValueOutputTypeDef
-]
-BatchAddFacetToObjectTypeDef = TypedDict(
-    "BatchAddFacetToObjectTypeDef",
+IndexAttachmentTypeDef = TypedDict(
+    "IndexAttachmentTypeDef",
     {
-        "SchemaFacet": SchemaFacetTypeDef,
-        "ObjectAttributeList": Sequence[AttributeKeyAndValueTypeDef],
-        "ObjectReference": ObjectReferenceTypeDef,
+        "IndexedAttributes": List[AttributeKeyAndValueTypeDef],
+        "ObjectIdentifier": str,
     },
+    total=False,
 )
 
-_RequiredBatchCreateObjectTypeDef = TypedDict(
-    "_RequiredBatchCreateObjectTypeDef",
+ListObjectAttributesResponseTypeDef = TypedDict(
+    "ListObjectAttributesResponseTypeDef",
     {
-        "SchemaFacet": Sequence[SchemaFacetTypeDef],
-        "ObjectAttributeList": Sequence[AttributeKeyAndValueTypeDef],
+        "Attributes": List[AttributeKeyAndValueTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalBatchCreateObjectTypeDef = TypedDict(
-    "_OptionalBatchCreateObjectTypeDef",
+
+AttachTypedLinkRequestRequestTypeDef = TypedDict(
+    "AttachTypedLinkRequestRequestTypeDef",
     {
-        "ParentReference": ObjectReferenceTypeDef,
-        "LinkName": str,
-        "BatchReferenceName": str,
+        "DirectoryArn": str,
+        "SourceObjectReference": ObjectReferenceTypeDef,
+        "TargetObjectReference": ObjectReferenceTypeDef,
+        "TypedLinkFacet": TypedLinkSchemaAndFacetNameTypeDef,
+        "Attributes": Sequence[AttributeNameAndValueTypeDef],
     },
-    total=False,
 )
 
-class BatchCreateObjectTypeDef(
-    _RequiredBatchCreateObjectTypeDef, _OptionalBatchCreateObjectTypeDef
-):
-    pass
-
-AttributeNameAndValueUnionTypeDef = Union[
-    AttributeNameAndValueTypeDef, AttributeNameAndValueOutputTypeDef
-]
 BatchAttachTypedLinkTypeDef = TypedDict(
     "BatchAttachTypedLinkTypeDef",
     {
         "SourceObjectReference": ObjectReferenceTypeDef,
         "TargetObjectReference": ObjectReferenceTypeDef,
         "TypedLinkFacet": TypedLinkSchemaAndFacetNameTypeDef,
         "Attributes": Sequence[AttributeNameAndValueTypeDef],
@@ -2576,15 +2393,15 @@
 
 TypedLinkSpecifierTypeDef = TypedDict(
     "TypedLinkSpecifierTypeDef",
     {
         "TypedLinkFacet": TypedLinkSchemaAndFacetNameTypeDef,
         "SourceObjectReference": ObjectReferenceTypeDef,
         "TargetObjectReference": ObjectReferenceTypeDef,
-        "IdentityAttributeValues": Sequence[AttributeNameAndValueTypeDef],
+        "IdentityAttributeValues": List[AttributeNameAndValueTypeDef],
     },
 )
 
 _RequiredFacetAttributeTypeDef = TypedDict(
     "_RequiredFacetAttributeTypeDef",
     {
         "Name": str,
@@ -2645,14 +2462,23 @@
 )
 
 class TypedLinkAttributeRangeTypeDef(
     _RequiredTypedLinkAttributeRangeTypeDef, _OptionalTypedLinkAttributeRangeTypeDef
 ):
     pass
 
+ListTypedLinkFacetAttributesResponseTypeDef = TypedDict(
+    "ListTypedLinkFacetAttributesResponseTypeDef",
+    {
+        "Attributes": List[TypedLinkAttributeDefinitionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 TypedLinkFacetAttributeUpdateTypeDef = TypedDict(
     "TypedLinkFacetAttributeUpdateTypeDef",
     {
         "Attribute": TypedLinkAttributeDefinitionTypeDef,
         "Action": UpdateActionTypeType,
     },
 )
@@ -2662,109 +2488,64 @@
     {
         "Name": str,
         "Attributes": Sequence[TypedLinkAttributeDefinitionTypeDef],
         "IdentityAttributeOrder": Sequence[str],
     },
 )
 
-BatchWriteOperationResponseTypeDef = TypedDict(
-    "BatchWriteOperationResponseTypeDef",
+BatchListAttachedIndicesResponseTypeDef = TypedDict(
+    "BatchListAttachedIndicesResponseTypeDef",
     {
-        "CreateObject": BatchCreateObjectResponseTypeDef,
-        "AttachObject": BatchAttachObjectResponseTypeDef,
-        "DetachObject": BatchDetachObjectResponseTypeDef,
-        "UpdateObjectAttributes": BatchUpdateObjectAttributesResponseTypeDef,
-        "DeleteObject": Dict[str, Any],
-        "AddFacetToObject": Dict[str, Any],
-        "RemoveFacetFromObject": Dict[str, Any],
-        "AttachPolicy": Dict[str, Any],
-        "DetachPolicy": Dict[str, Any],
-        "CreateIndex": BatchCreateIndexResponseTypeDef,
-        "AttachToIndex": BatchAttachToIndexResponseTypeDef,
-        "DetachFromIndex": BatchDetachFromIndexResponseTypeDef,
-        "AttachTypedLink": BatchAttachTypedLinkResponseTypeDef,
-        "DetachTypedLink": Dict[str, Any],
-        "UpdateLinkAttributes": Dict[str, Any],
+        "IndexAttachments": List[IndexAttachmentTypeDef],
+        "NextToken": str,
     },
     total=False,
 )
 
-BatchReadSuccessfulResponseTypeDef = TypedDict(
-    "BatchReadSuccessfulResponseTypeDef",
+BatchListIndexResponseTypeDef = TypedDict(
+    "BatchListIndexResponseTypeDef",
     {
-        "ListObjectAttributes": BatchListObjectAttributesResponseTypeDef,
-        "ListObjectChildren": BatchListObjectChildrenResponseTypeDef,
-        "GetObjectInformation": BatchGetObjectInformationResponseTypeDef,
-        "GetObjectAttributes": BatchGetObjectAttributesResponseTypeDef,
-        "ListAttachedIndices": BatchListAttachedIndicesResponseTypeDef,
-        "ListObjectParentPaths": BatchListObjectParentPathsResponseTypeDef,
-        "ListObjectPolicies": BatchListObjectPoliciesResponseTypeDef,
-        "ListPolicyAttachments": BatchListPolicyAttachmentsResponseTypeDef,
-        "LookupPolicy": BatchLookupPolicyResponseTypeDef,
-        "ListIndex": BatchListIndexResponseTypeDef,
-        "ListOutgoingTypedLinks": BatchListOutgoingTypedLinksResponseTypeDef,
-        "ListIncomingTypedLinks": BatchListIncomingTypedLinksResponseTypeDef,
-        "GetLinkAttributes": BatchGetLinkAttributesResponseTypeDef,
-        "ListObjectParents": BatchListObjectParentsResponseTypeDef,
+        "IndexAttachments": List[IndexAttachmentTypeDef],
+        "NextToken": str,
     },
     total=False,
 )
 
-_RequiredAddFacetToObjectRequestRequestTypeDef = TypedDict(
-    "_RequiredAddFacetToObjectRequestRequestTypeDef",
-    {
-        "DirectoryArn": str,
-        "SchemaFacet": SchemaFacetTypeDef,
-        "ObjectReference": ObjectReferenceTypeDef,
-    },
-)
-_OptionalAddFacetToObjectRequestRequestTypeDef = TypedDict(
-    "_OptionalAddFacetToObjectRequestRequestTypeDef",
+ListAttachedIndicesResponseTypeDef = TypedDict(
+    "ListAttachedIndicesResponseTypeDef",
     {
-        "ObjectAttributeList": Sequence[AttributeKeyAndValueUnionTypeDef],
+        "IndexAttachments": List[IndexAttachmentTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class AddFacetToObjectRequestRequestTypeDef(
-    _RequiredAddFacetToObjectRequestRequestTypeDef, _OptionalAddFacetToObjectRequestRequestTypeDef
-):
-    pass
-
-_RequiredCreateObjectRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateObjectRequestRequestTypeDef",
+ListIndexResponseTypeDef = TypedDict(
+    "ListIndexResponseTypeDef",
     {
-        "DirectoryArn": str,
-        "SchemaFacets": Sequence[SchemaFacetTypeDef],
+        "IndexAttachments": List[IndexAttachmentTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalCreateObjectRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateObjectRequestRequestTypeDef",
+
+AttachTypedLinkResponseTypeDef = TypedDict(
+    "AttachTypedLinkResponseTypeDef",
     {
-        "ObjectAttributeList": Sequence[AttributeKeyAndValueUnionTypeDef],
-        "ParentReference": ObjectReferenceTypeDef,
-        "LinkName": str,
+        "TypedLinkSpecifier": TypedLinkSpecifierTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class CreateObjectRequestRequestTypeDef(
-    _RequiredCreateObjectRequestRequestTypeDef, _OptionalCreateObjectRequestRequestTypeDef
-):
-    pass
-
-AttachTypedLinkRequestRequestTypeDef = TypedDict(
-    "AttachTypedLinkRequestRequestTypeDef",
+BatchAttachTypedLinkResponseTypeDef = TypedDict(
+    "BatchAttachTypedLinkResponseTypeDef",
     {
-        "DirectoryArn": str,
-        "SourceObjectReference": ObjectReferenceTypeDef,
-        "TargetObjectReference": ObjectReferenceTypeDef,
-        "TypedLinkFacet": TypedLinkSchemaAndFacetNameTypeDef,
-        "Attributes": Sequence[AttributeNameAndValueUnionTypeDef],
+        "TypedLinkSpecifier": TypedLinkSpecifierTypeDef,
     },
+    total=False,
 )
 
 BatchDetachTypedLinkTypeDef = TypedDict(
     "BatchDetachTypedLinkTypeDef",
     {
         "TypedLinkSpecifier": TypedLinkSpecifierTypeDef,
     },
@@ -2774,14 +2555,32 @@
     "BatchGetLinkAttributesTypeDef",
     {
         "TypedLinkSpecifier": TypedLinkSpecifierTypeDef,
         "AttributeNames": Sequence[str],
     },
 )
 
+BatchListIncomingTypedLinksResponseTypeDef = TypedDict(
+    "BatchListIncomingTypedLinksResponseTypeDef",
+    {
+        "LinkSpecifiers": List[TypedLinkSpecifierTypeDef],
+        "NextToken": str,
+    },
+    total=False,
+)
+
+BatchListOutgoingTypedLinksResponseTypeDef = TypedDict(
+    "BatchListOutgoingTypedLinksResponseTypeDef",
+    {
+        "TypedLinkSpecifiers": List[TypedLinkSpecifierTypeDef],
+        "NextToken": str,
+    },
+    total=False,
+)
+
 DetachTypedLinkRequestRequestTypeDef = TypedDict(
     "DetachTypedLinkRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "TypedLinkSpecifier": TypedLinkSpecifierTypeDef,
     },
 )
@@ -2803,25 +2602,72 @@
 )
 
 class GetLinkAttributesRequestRequestTypeDef(
     _RequiredGetLinkAttributesRequestRequestTypeDef, _OptionalGetLinkAttributesRequestRequestTypeDef
 ):
     pass
 
-TypedLinkSpecifierUnionTypeDef = Union[TypedLinkSpecifierTypeDef, TypedLinkSpecifierOutputTypeDef]
-FacetAttributeUnionTypeDef = Union[FacetAttributeTypeDef, FacetAttributeOutputTypeDef]
+ListIncomingTypedLinksResponseTypeDef = TypedDict(
+    "ListIncomingTypedLinksResponseTypeDef",
+    {
+        "LinkSpecifiers": List[TypedLinkSpecifierTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListOutgoingTypedLinksResponseTypeDef = TypedDict(
+    "ListOutgoingTypedLinksResponseTypeDef",
+    {
+        "TypedLinkSpecifiers": List[TypedLinkSpecifierTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCreateFacetRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateFacetRequestRequestTypeDef",
+    {
+        "SchemaArn": str,
+        "Name": str,
+    },
+)
+_OptionalCreateFacetRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateFacetRequestRequestTypeDef",
+    {
+        "Attributes": Sequence[FacetAttributeTypeDef],
+        "ObjectType": ObjectTypeType,
+        "FacetStyle": FacetStyleType,
+    },
+    total=False,
+)
+
+class CreateFacetRequestRequestTypeDef(
+    _RequiredCreateFacetRequestRequestTypeDef, _OptionalCreateFacetRequestRequestTypeDef
+):
+    pass
+
 FacetAttributeUpdateTypeDef = TypedDict(
     "FacetAttributeUpdateTypeDef",
     {
         "Attribute": FacetAttributeTypeDef,
         "Action": UpdateActionTypeType,
     },
     total=False,
 )
 
+ListFacetAttributesResponseTypeDef = TypedDict(
+    "ListFacetAttributesResponseTypeDef",
+    {
+        "Attributes": List[FacetAttributeTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 BatchUpdateLinkAttributesTypeDef = TypedDict(
     "BatchUpdateLinkAttributesTypeDef",
     {
         "TypedLinkSpecifier": TypedLinkSpecifierTypeDef,
         "AttributeUpdates": Sequence[LinkAttributeUpdateTypeDef],
     },
 )
@@ -3073,53 +2919,57 @@
     "CreateTypedLinkFacetRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "Facet": TypedLinkFacetTypeDef,
     },
 )
 
-BatchWriteResponseTypeDef = TypedDict(
-    "BatchWriteResponseTypeDef",
-    {
-        "Responses": List[BatchWriteOperationResponseTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-BatchReadOperationResponseTypeDef = TypedDict(
-    "BatchReadOperationResponseTypeDef",
+BatchWriteOperationResponseTypeDef = TypedDict(
+    "BatchWriteOperationResponseTypeDef",
     {
-        "SuccessfulResponse": BatchReadSuccessfulResponseTypeDef,
-        "ExceptionResponse": BatchReadExceptionTypeDef,
+        "CreateObject": BatchCreateObjectResponseTypeDef,
+        "AttachObject": BatchAttachObjectResponseTypeDef,
+        "DetachObject": BatchDetachObjectResponseTypeDef,
+        "UpdateObjectAttributes": BatchUpdateObjectAttributesResponseTypeDef,
+        "DeleteObject": Dict[str, Any],
+        "AddFacetToObject": Dict[str, Any],
+        "RemoveFacetFromObject": Dict[str, Any],
+        "AttachPolicy": Dict[str, Any],
+        "DetachPolicy": Dict[str, Any],
+        "CreateIndex": BatchCreateIndexResponseTypeDef,
+        "AttachToIndex": BatchAttachToIndexResponseTypeDef,
+        "DetachFromIndex": BatchDetachFromIndexResponseTypeDef,
+        "AttachTypedLink": BatchAttachTypedLinkResponseTypeDef,
+        "DetachTypedLink": Dict[str, Any],
+        "UpdateLinkAttributes": Dict[str, Any],
     },
     total=False,
 )
 
-_RequiredCreateFacetRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateFacetRequestRequestTypeDef",
-    {
-        "SchemaArn": str,
-        "Name": str,
-    },
-)
-_OptionalCreateFacetRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateFacetRequestRequestTypeDef",
+BatchReadSuccessfulResponseTypeDef = TypedDict(
+    "BatchReadSuccessfulResponseTypeDef",
     {
-        "Attributes": Sequence[FacetAttributeUnionTypeDef],
-        "ObjectType": ObjectTypeType,
-        "FacetStyle": FacetStyleType,
+        "ListObjectAttributes": BatchListObjectAttributesResponseTypeDef,
+        "ListObjectChildren": BatchListObjectChildrenResponseTypeDef,
+        "GetObjectInformation": BatchGetObjectInformationResponseTypeDef,
+        "GetObjectAttributes": BatchGetObjectAttributesResponseTypeDef,
+        "ListAttachedIndices": BatchListAttachedIndicesResponseTypeDef,
+        "ListObjectParentPaths": BatchListObjectParentPathsResponseTypeDef,
+        "ListObjectPolicies": BatchListObjectPoliciesResponseTypeDef,
+        "ListPolicyAttachments": BatchListPolicyAttachmentsResponseTypeDef,
+        "LookupPolicy": BatchLookupPolicyResponseTypeDef,
+        "ListIndex": BatchListIndexResponseTypeDef,
+        "ListOutgoingTypedLinks": BatchListOutgoingTypedLinksResponseTypeDef,
+        "ListIncomingTypedLinks": BatchListIncomingTypedLinksResponseTypeDef,
+        "GetLinkAttributes": BatchGetLinkAttributesResponseTypeDef,
+        "ListObjectParents": BatchListObjectParentsResponseTypeDef,
     },
     total=False,
 )
 
-class CreateFacetRequestRequestTypeDef(
-    _RequiredCreateFacetRequestRequestTypeDef, _OptionalCreateFacetRequestRequestTypeDef
-):
-    pass
-
 _RequiredUpdateFacetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFacetRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "Name": str,
     },
 )
@@ -3176,22 +3026,31 @@
         "ListOutgoingTypedLinks": BatchListOutgoingTypedLinksTypeDef,
         "ListIncomingTypedLinks": BatchListIncomingTypedLinksTypeDef,
         "GetLinkAttributes": BatchGetLinkAttributesTypeDef,
     },
     total=False,
 )
 
-BatchReadResponseTypeDef = TypedDict(
-    "BatchReadResponseTypeDef",
+BatchWriteResponseTypeDef = TypedDict(
+    "BatchWriteResponseTypeDef",
     {
-        "Responses": List[BatchReadOperationResponseTypeDef],
+        "Responses": List[BatchWriteOperationResponseTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+BatchReadOperationResponseTypeDef = TypedDict(
+    "BatchReadOperationResponseTypeDef",
+    {
+        "SuccessfulResponse": BatchReadSuccessfulResponseTypeDef,
+        "ExceptionResponse": BatchReadExceptionTypeDef,
+    },
+    total=False,
+)
+
 BatchWriteRequestRequestTypeDef = TypedDict(
     "BatchWriteRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "Operations": Sequence[BatchWriteOperationTypeDef],
     },
 )
@@ -3211,7 +3070,15 @@
     total=False,
 )
 
 class BatchReadRequestRequestTypeDef(
     _RequiredBatchReadRequestRequestTypeDef, _OptionalBatchReadRequestRequestTypeDef
 ):
     pass
+
+BatchReadResponseTypeDef = TypedDict(
+    "BatchReadResponseTypeDef",
+    {
+        "Responses": List[BatchReadOperationResponseTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory.egg-info/SOURCES.txt` & `types-aiobotocore-clouddirectory-2.5.2.post2/types_aiobotocore_clouddirectory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

