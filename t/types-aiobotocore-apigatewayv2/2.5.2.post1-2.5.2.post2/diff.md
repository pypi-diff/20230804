# Comparing `tmp/types-aiobotocore-apigatewayv2-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-apigatewayv2-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-apigatewayv2-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:50 2023, max compression
+gzip compressed data, was "types-aiobotocore-apigatewayv2-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:22 2023, max compression
```

## Comparing `types-aiobotocore-apigatewayv2-2.5.2.post1.tar` & `types-aiobotocore-apigatewayv2-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:50.545660 types-aiobotocore-apigatewayv2-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:33:02.000000 types-aiobotocore-apigatewayv2-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21011 2023-08-02 14:51:50.545660 types-aiobotocore-apigatewayv2-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19473 2023-08-02 14:33:02.000000 types-aiobotocore-apigatewayv2-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:50.545660 types-aiobotocore-apigatewayv2-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-02 14:33:02.000000 types-aiobotocore-apigatewayv2-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:50.541660 types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2/
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-08-02 14:33:02.000000 types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-08-02 14:33:02.000000 types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-02 14:33:02.000000 types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    54835 2023-08-02 14:33:03.000000 types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    54744 2023-08-02 14:33:03.000000 types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10680 2023-08-02 14:33:04.000000 types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10678 2023-08-02 14:33:04.000000 types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11883 2023-08-02 14:33:04.000000 types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11871 2023-08-02 14:33:03.000000 types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:33:02.000000 types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    76777 2023-08-02 14:33:06.000000 types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    76667 2023-08-02 14:33:04.000000 types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:33:02.000000 types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:50.545660 types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21011 2023-08-02 14:51:50.000000 types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-02 14:51:50.000000 types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:50.000000 types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:50.000000 types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:50.000000 types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 14:51:50.000000 types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:22.759005 types-aiobotocore-apigatewayv2-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:40:10.000000 types-aiobotocore-apigatewayv2-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14347 2023-08-04 12:00:22.759005 types-aiobotocore-apigatewayv2-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12809 2023-08-04 11:40:10.000000 types-aiobotocore-apigatewayv2-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:22.759005 types-aiobotocore-apigatewayv2-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-04 11:40:09.000000 types-aiobotocore-apigatewayv2-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:22.755005 types-aiobotocore-apigatewayv2-2.5.2.post2/types_aiobotocore_apigatewayv2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-08-04 11:40:10.000000 types-aiobotocore-apigatewayv2-2.5.2.post2/types_aiobotocore_apigatewayv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-08-04 11:40:10.000000 types-aiobotocore-apigatewayv2-2.5.2.post2/types_aiobotocore_apigatewayv2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-04 11:40:10.000000 types-aiobotocore-apigatewayv2-2.5.2.post2/types_aiobotocore_apigatewayv2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54790 2023-08-04 11:40:10.000000 types-aiobotocore-apigatewayv2-2.5.2.post2/types_aiobotocore_apigatewayv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54699 2023-08-04 11:40:10.000000 types-aiobotocore-apigatewayv2-2.5.2.post2/types_aiobotocore_apigatewayv2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10680 2023-08-04 11:40:10.000000 types-aiobotocore-apigatewayv2-2.5.2.post2/types_aiobotocore_apigatewayv2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10678 2023-08-04 11:40:10.000000 types-aiobotocore-apigatewayv2-2.5.2.post2/types_aiobotocore_apigatewayv2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11883 2023-08-04 11:40:10.000000 types-aiobotocore-apigatewayv2-2.5.2.post2/types_aiobotocore_apigatewayv2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11871 2023-08-04 11:40:10.000000 types-aiobotocore-apigatewayv2-2.5.2.post2/types_aiobotocore_apigatewayv2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:40:10.000000 types-aiobotocore-apigatewayv2-2.5.2.post2/types_aiobotocore_apigatewayv2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    75222 2023-08-04 11:40:13.000000 types-aiobotocore-apigatewayv2-2.5.2.post2/types_aiobotocore_apigatewayv2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75111 2023-08-04 11:40:12.000000 types-aiobotocore-apigatewayv2-2.5.2.post2/types_aiobotocore_apigatewayv2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:40:10.000000 types-aiobotocore-apigatewayv2-2.5.2.post2/types_aiobotocore_apigatewayv2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:22.759005 types-aiobotocore-apigatewayv2-2.5.2.post2/types_aiobotocore_apigatewayv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14347 2023-08-04 12:00:22.000000 types-aiobotocore-apigatewayv2-2.5.2.post2/types_aiobotocore_apigatewayv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-04 12:00:22.000000 types-aiobotocore-apigatewayv2-2.5.2.post2/types_aiobotocore_apigatewayv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:22.000000 types-aiobotocore-apigatewayv2-2.5.2.post2/types_aiobotocore_apigatewayv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:22.000000 types-aiobotocore-apigatewayv2-2.5.2.post2/types_aiobotocore_apigatewayv2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:22.000000 types-aiobotocore-apigatewayv2-2.5.2.post2/types_aiobotocore_apigatewayv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-04 12:00:22.000000 types-aiobotocore-apigatewayv2-2.5.2.post2/types_aiobotocore_apigatewayv2.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-apigatewayv2-2.5.2.post1/LICENSE` & `types-aiobotocore-apigatewayv2-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apigatewayv2-2.5.2.post1/setup.py` & `types-aiobotocore-apigatewayv2-2.5.2.post2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-apigatewayv2",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_apigatewayv2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ApiGatewayV2 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2/__init__.py` & `types-aiobotocore-apigatewayv2-2.5.2.post2/types_aiobotocore_apigatewayv2/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2/__init__.pyi` & `types-aiobotocore-apigatewayv2-2.5.2.post2/types_aiobotocore_apigatewayv2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2/__main__.py` & `types-aiobotocore-apigatewayv2-2.5.2.post2/types_aiobotocore_apigatewayv2/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ApiGatewayV2 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.ApiGatewayV2 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2\nOther"
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

### Comparing `types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2/client.py` & `types-aiobotocore-apigatewayv2-2.5.2.post2/types_aiobotocore_apigatewayv2/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,28 +40,28 @@
     GetModelsPaginator,
     GetRouteResponsesPaginator,
     GetRoutesPaginator,
     GetStagesPaginator,
 )
 from .type_defs import (
     AccessLogSettingsTypeDef,
-    CorsUnionTypeDef,
+    CorsTypeDef,
     CreateApiMappingResponseTypeDef,
     CreateApiResponseTypeDef,
     CreateAuthorizerResponseTypeDef,
     CreateDeploymentResponseTypeDef,
     CreateDomainNameResponseTypeDef,
     CreateIntegrationResponseResponseTypeDef,
     CreateIntegrationResultTypeDef,
     CreateModelResponseTypeDef,
     CreateRouteResponseResponseTypeDef,
     CreateRouteResultTypeDef,
     CreateStageResponseTypeDef,
     CreateVpcLinkResponseTypeDef,
-    DomainNameConfigurationUnionTypeDef,
+    DomainNameConfigurationTypeDef,
     EmptyResponseMetadataTypeDef,
     ExportApiResponseTypeDef,
     GetApiMappingResponseTypeDef,
     GetApiMappingsResponseTypeDef,
     GetApiResponseTypeDef,
     GetApisResponseTypeDef,
     GetAuthorizerResponseTypeDef,
@@ -83,15 +83,15 @@
     GetRoutesResponseTypeDef,
     GetStageResponseTypeDef,
     GetStagesResponseTypeDef,
     GetTagsResponseTypeDef,
     GetVpcLinkResponseTypeDef,
     GetVpcLinksResponseTypeDef,
     ImportApiResponseTypeDef,
-    JWTConfigurationUnionTypeDef,
+    JWTConfigurationTypeDef,
     MutualTlsAuthenticationInputTypeDef,
     ParameterConstraintsTypeDef,
     ReimportApiResponseTypeDef,
     RouteSettingsTypeDef,
     TlsConfigInputTypeDef,
     UpdateApiMappingResponseTypeDef,
     UpdateApiResponseTypeDef,
@@ -168,15 +168,15 @@
 
     async def create_api(
         self,
         *,
         Name: str,
         ProtocolType: ProtocolTypeType,
         ApiKeySelectionExpression: str = ...,
-        CorsConfiguration: CorsUnionTypeDef = ...,
+        CorsConfiguration: CorsTypeDef = ...,
         CredentialsArn: str = ...,
         Description: str = ...,
         DisableSchemaValidation: bool = ...,
         DisableExecuteApiEndpoint: bool = ...,
         RouteKey: str = ...,
         RouteSelectionExpression: str = ...,
         Tags: Mapping[str, str] = ...,
@@ -209,15 +209,15 @@
         Name: str,
         AuthorizerCredentialsArn: str = ...,
         AuthorizerPayloadFormatVersion: str = ...,
         AuthorizerResultTtlInSeconds: int = ...,
         AuthorizerUri: str = ...,
         EnableSimpleResponses: bool = ...,
         IdentityValidationExpression: str = ...,
-        JwtConfiguration: JWTConfigurationUnionTypeDef = ...
+        JwtConfiguration: JWTConfigurationTypeDef = ...
     ) -> CreateAuthorizerResponseTypeDef:
         """
         Creates an Authorizer for an API.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.create_authorizer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/client/#create_authorizer)
         """
@@ -232,15 +232,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/client/#create_deployment)
         """
 
     async def create_domain_name(
         self,
         *,
         DomainName: str,
-        DomainNameConfigurations: Sequence[DomainNameConfigurationUnionTypeDef] = ...,
+        DomainNameConfigurations: Sequence[DomainNameConfigurationTypeDef] = ...,
         MutualTlsAuthentication: MutualTlsAuthenticationInputTypeDef = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateDomainNameResponseTypeDef:
         """
         Creates a domain name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.create_domain_name)
@@ -856,15 +856,15 @@
         """
 
     async def update_api(
         self,
         *,
         ApiId: str,
         ApiKeySelectionExpression: str = ...,
-        CorsConfiguration: CorsUnionTypeDef = ...,
+        CorsConfiguration: CorsTypeDef = ...,
         CredentialsArn: str = ...,
         Description: str = ...,
         DisableSchemaValidation: bool = ...,
         DisableExecuteApiEndpoint: bool = ...,
         Name: str = ...,
         RouteKey: str = ...,
         RouteSelectionExpression: str = ...,
@@ -903,15 +903,15 @@
         AuthorizerPayloadFormatVersion: str = ...,
         AuthorizerResultTtlInSeconds: int = ...,
         AuthorizerType: AuthorizerTypeType = ...,
         AuthorizerUri: str = ...,
         EnableSimpleResponses: bool = ...,
         IdentitySource: Sequence[str] = ...,
         IdentityValidationExpression: str = ...,
-        JwtConfiguration: JWTConfigurationUnionTypeDef = ...,
+        JwtConfiguration: JWTConfigurationTypeDef = ...,
         Name: str = ...
     ) -> UpdateAuthorizerResponseTypeDef:
         """
         Updates an Authorizer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.update_authorizer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/client/#update_authorizer)
@@ -927,15 +927,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/client/#update_deployment)
         """
 
     async def update_domain_name(
         self,
         *,
         DomainName: str,
-        DomainNameConfigurations: Sequence[DomainNameConfigurationUnionTypeDef] = ...,
+        DomainNameConfigurations: Sequence[DomainNameConfigurationTypeDef] = ...,
         MutualTlsAuthentication: MutualTlsAuthenticationInputTypeDef = ...
     ) -> UpdateDomainNameResponseTypeDef:
         """
         Updates a domain name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.update_domain_name)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/client/#update_domain_name)
```

### Comparing `types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2/client.pyi` & `types-aiobotocore-apigatewayv2-2.5.2.post2/types_aiobotocore_apigatewayv2/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -40,28 +40,28 @@
     GetModelsPaginator,
     GetRouteResponsesPaginator,
     GetRoutesPaginator,
     GetStagesPaginator,
 )
 from .type_defs import (
     AccessLogSettingsTypeDef,
-    CorsUnionTypeDef,
+    CorsTypeDef,
     CreateApiMappingResponseTypeDef,
     CreateApiResponseTypeDef,
     CreateAuthorizerResponseTypeDef,
     CreateDeploymentResponseTypeDef,
     CreateDomainNameResponseTypeDef,
     CreateIntegrationResponseResponseTypeDef,
     CreateIntegrationResultTypeDef,
     CreateModelResponseTypeDef,
     CreateRouteResponseResponseTypeDef,
     CreateRouteResultTypeDef,
     CreateStageResponseTypeDef,
     CreateVpcLinkResponseTypeDef,
-    DomainNameConfigurationUnionTypeDef,
+    DomainNameConfigurationTypeDef,
     EmptyResponseMetadataTypeDef,
     ExportApiResponseTypeDef,
     GetApiMappingResponseTypeDef,
     GetApiMappingsResponseTypeDef,
     GetApiResponseTypeDef,
     GetApisResponseTypeDef,
     GetAuthorizerResponseTypeDef,
@@ -83,15 +83,15 @@
     GetRoutesResponseTypeDef,
     GetStageResponseTypeDef,
     GetStagesResponseTypeDef,
     GetTagsResponseTypeDef,
     GetVpcLinkResponseTypeDef,
     GetVpcLinksResponseTypeDef,
     ImportApiResponseTypeDef,
-    JWTConfigurationUnionTypeDef,
+    JWTConfigurationTypeDef,
     MutualTlsAuthenticationInputTypeDef,
     ParameterConstraintsTypeDef,
     ReimportApiResponseTypeDef,
     RouteSettingsTypeDef,
     TlsConfigInputTypeDef,
     UpdateApiMappingResponseTypeDef,
     UpdateApiResponseTypeDef,
@@ -161,15 +161,15 @@
         """
     async def create_api(
         self,
         *,
         Name: str,
         ProtocolType: ProtocolTypeType,
         ApiKeySelectionExpression: str = ...,
-        CorsConfiguration: CorsUnionTypeDef = ...,
+        CorsConfiguration: CorsTypeDef = ...,
         CredentialsArn: str = ...,
         Description: str = ...,
         DisableSchemaValidation: bool = ...,
         DisableExecuteApiEndpoint: bool = ...,
         RouteKey: str = ...,
         RouteSelectionExpression: str = ...,
         Tags: Mapping[str, str] = ...,
@@ -200,15 +200,15 @@
         Name: str,
         AuthorizerCredentialsArn: str = ...,
         AuthorizerPayloadFormatVersion: str = ...,
         AuthorizerResultTtlInSeconds: int = ...,
         AuthorizerUri: str = ...,
         EnableSimpleResponses: bool = ...,
         IdentityValidationExpression: str = ...,
-        JwtConfiguration: JWTConfigurationUnionTypeDef = ...
+        JwtConfiguration: JWTConfigurationTypeDef = ...
     ) -> CreateAuthorizerResponseTypeDef:
         """
         Creates an Authorizer for an API.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.create_authorizer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/client/#create_authorizer)
         """
@@ -221,15 +221,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.create_deployment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/client/#create_deployment)
         """
     async def create_domain_name(
         self,
         *,
         DomainName: str,
-        DomainNameConfigurations: Sequence[DomainNameConfigurationUnionTypeDef] = ...,
+        DomainNameConfigurations: Sequence[DomainNameConfigurationTypeDef] = ...,
         MutualTlsAuthentication: MutualTlsAuthenticationInputTypeDef = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateDomainNameResponseTypeDef:
         """
         Creates a domain name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.create_domain_name)
@@ -788,15 +788,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/client/#untag_resource)
         """
     async def update_api(
         self,
         *,
         ApiId: str,
         ApiKeySelectionExpression: str = ...,
-        CorsConfiguration: CorsUnionTypeDef = ...,
+        CorsConfiguration: CorsTypeDef = ...,
         CredentialsArn: str = ...,
         Description: str = ...,
         DisableSchemaValidation: bool = ...,
         DisableExecuteApiEndpoint: bool = ...,
         Name: str = ...,
         RouteKey: str = ...,
         RouteSelectionExpression: str = ...,
@@ -833,15 +833,15 @@
         AuthorizerPayloadFormatVersion: str = ...,
         AuthorizerResultTtlInSeconds: int = ...,
         AuthorizerType: AuthorizerTypeType = ...,
         AuthorizerUri: str = ...,
         EnableSimpleResponses: bool = ...,
         IdentitySource: Sequence[str] = ...,
         IdentityValidationExpression: str = ...,
-        JwtConfiguration: JWTConfigurationUnionTypeDef = ...,
+        JwtConfiguration: JWTConfigurationTypeDef = ...,
         Name: str = ...
     ) -> UpdateAuthorizerResponseTypeDef:
         """
         Updates an Authorizer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.update_authorizer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/client/#update_authorizer)
@@ -855,15 +855,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.update_deployment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/client/#update_deployment)
         """
     async def update_domain_name(
         self,
         *,
         DomainName: str,
-        DomainNameConfigurations: Sequence[DomainNameConfigurationUnionTypeDef] = ...,
+        DomainNameConfigurations: Sequence[DomainNameConfigurationTypeDef] = ...,
         MutualTlsAuthentication: MutualTlsAuthenticationInputTypeDef = ...
     ) -> UpdateDomainNameResponseTypeDef:
         """
         Updates a domain name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.update_domain_name)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/client/#update_domain_name)
```

### Comparing `types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2/literals.py` & `types-aiobotocore-apigatewayv2-2.5.2.post2/types_aiobotocore_apigatewayv2/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2/literals.pyi` & `types-aiobotocore-apigatewayv2-2.5.2.post2/types_aiobotocore_apigatewayv2/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2/paginator.py` & `types-aiobotocore-apigatewayv2-2.5.2.post2/types_aiobotocore_apigatewayv2/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2/paginator.pyi` & `types-aiobotocore-apigatewayv2-2.5.2.post2/types_aiobotocore_apigatewayv2/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2/type_defs.py` & `types-aiobotocore-apigatewayv2-2.5.2.post2/types_aiobotocore_apigatewayv2/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,23 +43,20 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AccessLogSettingsTypeDef",
     "ApiMappingTypeDef",
-    "CorsOutputTypeDef",
-    "JWTConfigurationOutputTypeDef",
     "CorsTypeDef",
+    "JWTConfigurationTypeDef",
     "CreateApiMappingRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
-    "JWTConfigurationTypeDef",
     "CreateDeploymentRequestRequestTypeDef",
     "MutualTlsAuthenticationInputTypeDef",
-    "DomainNameConfigurationOutputTypeDef",
     "MutualTlsAuthenticationTypeDef",
     "TlsConfigInputTypeDef",
     "CreateIntegrationResponseRequestRequestTypeDef",
     "TlsConfigTypeDef",
     "CreateModelRequestRequestTypeDef",
     "ParameterConstraintsTypeDef",
     "RouteSettingsTypeDef",
@@ -120,18 +117,19 @@
     "UntagResourceRequestRequestTypeDef",
     "UpdateApiMappingRequestRequestTypeDef",
     "UpdateDeploymentRequestRequestTypeDef",
     "UpdateIntegrationResponseRequestRequestTypeDef",
     "UpdateModelRequestRequestTypeDef",
     "UpdateVpcLinkRequestRequestTypeDef",
     "ApiTypeDef",
-    "AuthorizerTypeDef",
-    "CorsUnionTypeDef",
     "CreateApiRequestRequestTypeDef",
     "UpdateApiRequestRequestTypeDef",
+    "AuthorizerTypeDef",
+    "CreateAuthorizerRequestRequestTypeDef",
+    "UpdateAuthorizerRequestRequestTypeDef",
     "CreateApiMappingResponseTypeDef",
     "CreateApiResponseTypeDef",
     "CreateAuthorizerResponseTypeDef",
     "CreateDeploymentResponseTypeDef",
     "CreateIntegrationResponseResponseTypeDef",
     "CreateModelResponseTypeDef",
     "CreateVpcLinkResponseTypeDef",
@@ -152,21 +150,14 @@
     "UpdateApiMappingResponseTypeDef",
     "UpdateApiResponseTypeDef",
     "UpdateAuthorizerResponseTypeDef",
     "UpdateDeploymentResponseTypeDef",
     "UpdateIntegrationResponseResponseTypeDef",
     "UpdateModelResponseTypeDef",
     "UpdateVpcLinkResponseTypeDef",
-    "CreateAuthorizerRequestRequestTypeDef",
-    "JWTConfigurationUnionTypeDef",
-    "UpdateAuthorizerRequestRequestTypeDef",
-    "CreateDomainNameResponseTypeDef",
-    "DomainNameTypeDef",
-    "GetDomainNameResponseTypeDef",
-    "UpdateDomainNameResponseTypeDef",
     "CreateIntegrationRequestRequestTypeDef",
     "UpdateIntegrationRequestRequestTypeDef",
     "CreateIntegrationResultTypeDef",
     "GetIntegrationResultTypeDef",
     "IntegrationTypeDef",
     "UpdateIntegrationResultTypeDef",
     "CreateRouteRequestRequestTypeDef",
@@ -200,22 +191,25 @@
     "GetRoutesRequestGetRoutesPaginateTypeDef",
     "GetStagesRequestGetStagesPaginateTypeDef",
     "GetIntegrationResponsesResponseTypeDef",
     "GetModelsResponseTypeDef",
     "GetVpcLinksResponseTypeDef",
     "GetApisResponseTypeDef",
     "GetAuthorizersResponseTypeDef",
-    "GetDomainNamesResponseTypeDef",
     "GetIntegrationsResponseTypeDef",
     "GetRouteResponsesResponseTypeDef",
     "GetRoutesResponseTypeDef",
     "GetStagesResponseTypeDef",
-    "DomainNameConfigurationUnionTypeDef",
     "CreateDomainNameRequestRequestTypeDef",
+    "CreateDomainNameResponseTypeDef",
+    "DomainNameTypeDef",
+    "GetDomainNameResponseTypeDef",
     "UpdateDomainNameRequestRequestTypeDef",
+    "UpdateDomainNameResponseTypeDef",
+    "GetDomainNamesResponseTypeDef",
 )
 
 AccessLogSettingsTypeDef = TypedDict(
     "AccessLogSettingsTypeDef",
     {
         "DestinationArn": str,
         "Format": str,
@@ -240,49 +234,36 @@
 )
 
 
 class ApiMappingTypeDef(_RequiredApiMappingTypeDef, _OptionalApiMappingTypeDef):
     pass
 
 
-CorsOutputTypeDef = TypedDict(
-    "CorsOutputTypeDef",
-    {
-        "AllowCredentials": bool,
-        "AllowHeaders": List[str],
-        "AllowMethods": List[str],
-        "AllowOrigins": List[str],
-        "ExposeHeaders": List[str],
-        "MaxAge": int,
-    },
-    total=False,
-)
-
-JWTConfigurationOutputTypeDef = TypedDict(
-    "JWTConfigurationOutputTypeDef",
-    {
-        "Audience": List[str],
-        "Issuer": str,
-    },
-    total=False,
-)
-
 CorsTypeDef = TypedDict(
     "CorsTypeDef",
     {
         "AllowCredentials": bool,
         "AllowHeaders": Sequence[str],
         "AllowMethods": Sequence[str],
         "AllowOrigins": Sequence[str],
         "ExposeHeaders": Sequence[str],
         "MaxAge": int,
     },
     total=False,
 )
 
+JWTConfigurationTypeDef = TypedDict(
+    "JWTConfigurationTypeDef",
+    {
+        "Audience": Sequence[str],
+        "Issuer": str,
+    },
+    total=False,
+)
+
 _RequiredCreateApiMappingRequestRequestTypeDef = TypedDict(
     "_RequiredCreateApiMappingRequestRequestTypeDef",
     {
         "ApiId": str,
         "DomainName": str,
         "Stage": str,
     },
@@ -309,23 +290,14 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-JWTConfigurationTypeDef = TypedDict(
-    "JWTConfigurationTypeDef",
-    {
-        "Audience": Sequence[str],
-        "Issuer": str,
-    },
-    total=False,
-)
-
 _RequiredCreateDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDeploymentRequestRequestTypeDef",
     {
         "ApiId": str,
     },
 )
 _OptionalCreateDeploymentRequestRequestTypeDef = TypedDict(
@@ -349,31 +321,14 @@
     {
         "TruststoreUri": str,
         "TruststoreVersion": str,
     },
     total=False,
 )
 
-DomainNameConfigurationOutputTypeDef = TypedDict(
-    "DomainNameConfigurationOutputTypeDef",
-    {
-        "ApiGatewayDomainName": str,
-        "CertificateArn": str,
-        "CertificateName": str,
-        "CertificateUploadDate": datetime,
-        "DomainNameStatus": DomainNameStatusType,
-        "DomainNameStatusMessage": str,
-        "EndpointType": EndpointTypeType,
-        "HostedZoneId": str,
-        "SecurityPolicy": SecurityPolicyType,
-        "OwnershipVerificationCertificateArn": str,
-    },
-    total=False,
-)
-
 MutualTlsAuthenticationTypeDef = TypedDict(
     "MutualTlsAuthenticationTypeDef",
     {
         "TruststoreUri": str,
         "TruststoreVersion": str,
         "TruststoreWarnings": List[str],
     },
@@ -1291,15 +1246,15 @@
 _OptionalApiTypeDef = TypedDict(
     "_OptionalApiTypeDef",
     {
         "ApiEndpoint": str,
         "ApiGatewayManaged": bool,
         "ApiId": str,
         "ApiKeySelectionExpression": str,
-        "CorsConfiguration": CorsOutputTypeDef,
+        "CorsConfiguration": CorsTypeDef,
         "CreatedDate": datetime,
         "Description": str,
         "DisableSchemaValidation": bool,
         "DisableExecuteApiEndpoint": bool,
         "ImportInfo": List[str],
         "Tags": Dict[str, str],
         "Version": str,
@@ -1309,43 +1264,14 @@
 )
 
 
 class ApiTypeDef(_RequiredApiTypeDef, _OptionalApiTypeDef):
     pass
 
 
-_RequiredAuthorizerTypeDef = TypedDict(
-    "_RequiredAuthorizerTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalAuthorizerTypeDef = TypedDict(
-    "_OptionalAuthorizerTypeDef",
-    {
-        "AuthorizerCredentialsArn": str,
-        "AuthorizerId": str,
-        "AuthorizerPayloadFormatVersion": str,
-        "AuthorizerResultTtlInSeconds": int,
-        "AuthorizerType": AuthorizerTypeType,
-        "AuthorizerUri": str,
-        "EnableSimpleResponses": bool,
-        "IdentitySource": List[str],
-        "IdentityValidationExpression": str,
-        "JwtConfiguration": JWTConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class AuthorizerTypeDef(_RequiredAuthorizerTypeDef, _OptionalAuthorizerTypeDef):
-    pass
-
-
-CorsUnionTypeDef = Union[CorsTypeDef, CorsOutputTypeDef]
 _RequiredCreateApiRequestRequestTypeDef = TypedDict(
     "_RequiredCreateApiRequestRequestTypeDef",
     {
         "Name": str,
         "ProtocolType": ProtocolTypeType,
     },
 )
@@ -1401,14 +1327,103 @@
 
 class UpdateApiRequestRequestTypeDef(
     _RequiredUpdateApiRequestRequestTypeDef, _OptionalUpdateApiRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredAuthorizerTypeDef = TypedDict(
+    "_RequiredAuthorizerTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalAuthorizerTypeDef = TypedDict(
+    "_OptionalAuthorizerTypeDef",
+    {
+        "AuthorizerCredentialsArn": str,
+        "AuthorizerId": str,
+        "AuthorizerPayloadFormatVersion": str,
+        "AuthorizerResultTtlInSeconds": int,
+        "AuthorizerType": AuthorizerTypeType,
+        "AuthorizerUri": str,
+        "EnableSimpleResponses": bool,
+        "IdentitySource": List[str],
+        "IdentityValidationExpression": str,
+        "JwtConfiguration": JWTConfigurationTypeDef,
+    },
+    total=False,
+)
+
+
+class AuthorizerTypeDef(_RequiredAuthorizerTypeDef, _OptionalAuthorizerTypeDef):
+    pass
+
+
+_RequiredCreateAuthorizerRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAuthorizerRequestRequestTypeDef",
+    {
+        "ApiId": str,
+        "AuthorizerType": AuthorizerTypeType,
+        "IdentitySource": Sequence[str],
+        "Name": str,
+    },
+)
+_OptionalCreateAuthorizerRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAuthorizerRequestRequestTypeDef",
+    {
+        "AuthorizerCredentialsArn": str,
+        "AuthorizerPayloadFormatVersion": str,
+        "AuthorizerResultTtlInSeconds": int,
+        "AuthorizerUri": str,
+        "EnableSimpleResponses": bool,
+        "IdentityValidationExpression": str,
+        "JwtConfiguration": JWTConfigurationTypeDef,
+    },
+    total=False,
+)
+
+
+class CreateAuthorizerRequestRequestTypeDef(
+    _RequiredCreateAuthorizerRequestRequestTypeDef, _OptionalCreateAuthorizerRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredUpdateAuthorizerRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateAuthorizerRequestRequestTypeDef",
+    {
+        "ApiId": str,
+        "AuthorizerId": str,
+    },
+)
+_OptionalUpdateAuthorizerRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateAuthorizerRequestRequestTypeDef",
+    {
+        "AuthorizerCredentialsArn": str,
+        "AuthorizerPayloadFormatVersion": str,
+        "AuthorizerResultTtlInSeconds": int,
+        "AuthorizerType": AuthorizerTypeType,
+        "AuthorizerUri": str,
+        "EnableSimpleResponses": bool,
+        "IdentitySource": Sequence[str],
+        "IdentityValidationExpression": str,
+        "JwtConfiguration": JWTConfigurationTypeDef,
+        "Name": str,
+    },
+    total=False,
+)
+
+
+class UpdateAuthorizerRequestRequestTypeDef(
+    _RequiredUpdateAuthorizerRequestRequestTypeDef, _OptionalUpdateAuthorizerRequestRequestTypeDef
+):
+    pass
+
+
 CreateApiMappingResponseTypeDef = TypedDict(
     "CreateApiMappingResponseTypeDef",
     {
         "ApiId": str,
         "ApiMappingId": str,
         "ApiMappingKey": str,
         "Stage": str,
@@ -1419,15 +1434,15 @@
 CreateApiResponseTypeDef = TypedDict(
     "CreateApiResponseTypeDef",
     {
         "ApiEndpoint": str,
         "ApiGatewayManaged": bool,
         "ApiId": str,
         "ApiKeySelectionExpression": str,
-        "CorsConfiguration": CorsOutputTypeDef,
+        "CorsConfiguration": CorsTypeDef,
         "CreatedDate": datetime,
         "Description": str,
         "DisableSchemaValidation": bool,
         "DisableExecuteApiEndpoint": bool,
         "ImportInfo": List[str],
         "Name": str,
         "ProtocolType": ProtocolTypeType,
@@ -1447,15 +1462,15 @@
         "AuthorizerPayloadFormatVersion": str,
         "AuthorizerResultTtlInSeconds": int,
         "AuthorizerType": AuthorizerTypeType,
         "AuthorizerUri": str,
         "EnableSimpleResponses": bool,
         "IdentitySource": List[str],
         "IdentityValidationExpression": str,
-        "JwtConfiguration": JWTConfigurationOutputTypeDef,
+        "JwtConfiguration": JWTConfigurationTypeDef,
         "Name": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDeploymentResponseTypeDef = TypedDict(
     "CreateDeploymentResponseTypeDef",
@@ -1549,15 +1564,15 @@
 GetApiResponseTypeDef = TypedDict(
     "GetApiResponseTypeDef",
     {
         "ApiEndpoint": str,
         "ApiGatewayManaged": bool,
         "ApiId": str,
         "ApiKeySelectionExpression": str,
-        "CorsConfiguration": CorsOutputTypeDef,
+        "CorsConfiguration": CorsTypeDef,
         "CreatedDate": datetime,
         "Description": str,
         "DisableSchemaValidation": bool,
         "DisableExecuteApiEndpoint": bool,
         "ImportInfo": List[str],
         "Name": str,
         "ProtocolType": ProtocolTypeType,
@@ -1577,15 +1592,15 @@
         "AuthorizerPayloadFormatVersion": str,
         "AuthorizerResultTtlInSeconds": int,
         "AuthorizerType": AuthorizerTypeType,
         "AuthorizerUri": str,
         "EnableSimpleResponses": bool,
         "IdentitySource": List[str],
         "IdentityValidationExpression": str,
-        "JwtConfiguration": JWTConfigurationOutputTypeDef,
+        "JwtConfiguration": JWTConfigurationTypeDef,
         "Name": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDeploymentResponseTypeDef = TypedDict(
     "GetDeploymentResponseTypeDef",
@@ -1660,15 +1675,15 @@
 ImportApiResponseTypeDef = TypedDict(
     "ImportApiResponseTypeDef",
     {
         "ApiEndpoint": str,
         "ApiGatewayManaged": bool,
         "ApiId": str,
         "ApiKeySelectionExpression": str,
-        "CorsConfiguration": CorsOutputTypeDef,
+        "CorsConfiguration": CorsTypeDef,
         "CreatedDate": datetime,
         "Description": str,
         "DisableSchemaValidation": bool,
         "DisableExecuteApiEndpoint": bool,
         "ImportInfo": List[str],
         "Name": str,
         "ProtocolType": ProtocolTypeType,
@@ -1683,15 +1698,15 @@
 ReimportApiResponseTypeDef = TypedDict(
     "ReimportApiResponseTypeDef",
     {
         "ApiEndpoint": str,
         "ApiGatewayManaged": bool,
         "ApiId": str,
         "ApiKeySelectionExpression": str,
-        "CorsConfiguration": CorsOutputTypeDef,
+        "CorsConfiguration": CorsTypeDef,
         "CreatedDate": datetime,
         "Description": str,
         "DisableSchemaValidation": bool,
         "DisableExecuteApiEndpoint": bool,
         "ImportInfo": List[str],
         "Name": str,
         "ProtocolType": ProtocolTypeType,
@@ -1717,15 +1732,15 @@
 UpdateApiResponseTypeDef = TypedDict(
     "UpdateApiResponseTypeDef",
     {
         "ApiEndpoint": str,
         "ApiGatewayManaged": bool,
         "ApiId": str,
         "ApiKeySelectionExpression": str,
-        "CorsConfiguration": CorsOutputTypeDef,
+        "CorsConfiguration": CorsTypeDef,
         "CreatedDate": datetime,
         "Description": str,
         "DisableSchemaValidation": bool,
         "DisableExecuteApiEndpoint": bool,
         "ImportInfo": List[str],
         "Name": str,
         "ProtocolType": ProtocolTypeType,
@@ -1745,15 +1760,15 @@
         "AuthorizerPayloadFormatVersion": str,
         "AuthorizerResultTtlInSeconds": int,
         "AuthorizerType": AuthorizerTypeType,
         "AuthorizerUri": str,
         "EnableSimpleResponses": bool,
         "IdentitySource": List[str],
         "IdentityValidationExpression": str,
-        "JwtConfiguration": JWTConfigurationOutputTypeDef,
+        "JwtConfiguration": JWTConfigurationTypeDef,
         "Name": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDeploymentResponseTypeDef = TypedDict(
     "UpdateDeploymentResponseTypeDef",
@@ -1805,134 +1820,14 @@
         "VpcLinkStatus": VpcLinkStatusType,
         "VpcLinkStatusMessage": str,
         "VpcLinkVersion": Literal["V2"],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateAuthorizerRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateAuthorizerRequestRequestTypeDef",
-    {
-        "ApiId": str,
-        "AuthorizerType": AuthorizerTypeType,
-        "IdentitySource": Sequence[str],
-        "Name": str,
-    },
-)
-_OptionalCreateAuthorizerRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateAuthorizerRequestRequestTypeDef",
-    {
-        "AuthorizerCredentialsArn": str,
-        "AuthorizerPayloadFormatVersion": str,
-        "AuthorizerResultTtlInSeconds": int,
-        "AuthorizerUri": str,
-        "EnableSimpleResponses": bool,
-        "IdentityValidationExpression": str,
-        "JwtConfiguration": JWTConfigurationTypeDef,
-    },
-    total=False,
-)
-
-
-class CreateAuthorizerRequestRequestTypeDef(
-    _RequiredCreateAuthorizerRequestRequestTypeDef, _OptionalCreateAuthorizerRequestRequestTypeDef
-):
-    pass
-
-
-JWTConfigurationUnionTypeDef = Union[JWTConfigurationTypeDef, JWTConfigurationOutputTypeDef]
-_RequiredUpdateAuthorizerRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateAuthorizerRequestRequestTypeDef",
-    {
-        "ApiId": str,
-        "AuthorizerId": str,
-    },
-)
-_OptionalUpdateAuthorizerRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateAuthorizerRequestRequestTypeDef",
-    {
-        "AuthorizerCredentialsArn": str,
-        "AuthorizerPayloadFormatVersion": str,
-        "AuthorizerResultTtlInSeconds": int,
-        "AuthorizerType": AuthorizerTypeType,
-        "AuthorizerUri": str,
-        "EnableSimpleResponses": bool,
-        "IdentitySource": Sequence[str],
-        "IdentityValidationExpression": str,
-        "JwtConfiguration": JWTConfigurationTypeDef,
-        "Name": str,
-    },
-    total=False,
-)
-
-
-class UpdateAuthorizerRequestRequestTypeDef(
-    _RequiredUpdateAuthorizerRequestRequestTypeDef, _OptionalUpdateAuthorizerRequestRequestTypeDef
-):
-    pass
-
-
-CreateDomainNameResponseTypeDef = TypedDict(
-    "CreateDomainNameResponseTypeDef",
-    {
-        "ApiMappingSelectionExpression": str,
-        "DomainName": str,
-        "DomainNameConfigurations": List[DomainNameConfigurationOutputTypeDef],
-        "MutualTlsAuthentication": MutualTlsAuthenticationTypeDef,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredDomainNameTypeDef = TypedDict(
-    "_RequiredDomainNameTypeDef",
-    {
-        "DomainName": str,
-    },
-)
-_OptionalDomainNameTypeDef = TypedDict(
-    "_OptionalDomainNameTypeDef",
-    {
-        "ApiMappingSelectionExpression": str,
-        "DomainNameConfigurations": List[DomainNameConfigurationOutputTypeDef],
-        "MutualTlsAuthentication": MutualTlsAuthenticationTypeDef,
-        "Tags": Dict[str, str],
-    },
-    total=False,
-)
-
-
-class DomainNameTypeDef(_RequiredDomainNameTypeDef, _OptionalDomainNameTypeDef):
-    pass
-
-
-GetDomainNameResponseTypeDef = TypedDict(
-    "GetDomainNameResponseTypeDef",
-    {
-        "ApiMappingSelectionExpression": str,
-        "DomainName": str,
-        "DomainNameConfigurations": List[DomainNameConfigurationOutputTypeDef],
-        "MutualTlsAuthentication": MutualTlsAuthenticationTypeDef,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateDomainNameResponseTypeDef = TypedDict(
-    "UpdateDomainNameResponseTypeDef",
-    {
-        "ApiMappingSelectionExpression": str,
-        "DomainName": str,
-        "DomainNameConfigurations": List[DomainNameConfigurationOutputTypeDef],
-        "MutualTlsAuthentication": MutualTlsAuthenticationTypeDef,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateIntegrationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateIntegrationRequestRequestTypeDef",
     {
         "ApiId": str,
         "IntegrationType": IntegrationTypeType,
     },
 )
@@ -2790,23 +2685,14 @@
     {
         "Items": List[AuthorizerTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetDomainNamesResponseTypeDef = TypedDict(
-    "GetDomainNamesResponseTypeDef",
-    {
-        "Items": List[DomainNameTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 GetIntegrationsResponseTypeDef = TypedDict(
     "GetIntegrationsResponseTypeDef",
     {
         "Items": List[IntegrationTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2835,53 +2721,118 @@
     {
         "Items": List[StageTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DomainNameConfigurationUnionTypeDef = Union[
-    DomainNameConfigurationTypeDef, DomainNameConfigurationOutputTypeDef
-]
 _RequiredCreateDomainNameRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDomainNameRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalCreateDomainNameRequestRequestTypeDef = TypedDict(
     "_OptionalCreateDomainNameRequestRequestTypeDef",
     {
-        "DomainNameConfigurations": Sequence[DomainNameConfigurationUnionTypeDef],
+        "DomainNameConfigurations": Sequence[DomainNameConfigurationTypeDef],
         "MutualTlsAuthentication": MutualTlsAuthenticationInputTypeDef,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
 
 class CreateDomainNameRequestRequestTypeDef(
     _RequiredCreateDomainNameRequestRequestTypeDef, _OptionalCreateDomainNameRequestRequestTypeDef
 ):
     pass
 
 
+CreateDomainNameResponseTypeDef = TypedDict(
+    "CreateDomainNameResponseTypeDef",
+    {
+        "ApiMappingSelectionExpression": str,
+        "DomainName": str,
+        "DomainNameConfigurations": List[DomainNameConfigurationTypeDef],
+        "MutualTlsAuthentication": MutualTlsAuthenticationTypeDef,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredDomainNameTypeDef = TypedDict(
+    "_RequiredDomainNameTypeDef",
+    {
+        "DomainName": str,
+    },
+)
+_OptionalDomainNameTypeDef = TypedDict(
+    "_OptionalDomainNameTypeDef",
+    {
+        "ApiMappingSelectionExpression": str,
+        "DomainNameConfigurations": List[DomainNameConfigurationTypeDef],
+        "MutualTlsAuthentication": MutualTlsAuthenticationTypeDef,
+        "Tags": Dict[str, str],
+    },
+    total=False,
+)
+
+
+class DomainNameTypeDef(_RequiredDomainNameTypeDef, _OptionalDomainNameTypeDef):
+    pass
+
+
+GetDomainNameResponseTypeDef = TypedDict(
+    "GetDomainNameResponseTypeDef",
+    {
+        "ApiMappingSelectionExpression": str,
+        "DomainName": str,
+        "DomainNameConfigurations": List[DomainNameConfigurationTypeDef],
+        "MutualTlsAuthentication": MutualTlsAuthenticationTypeDef,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateDomainNameRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDomainNameRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalUpdateDomainNameRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateDomainNameRequestRequestTypeDef",
     {
-        "DomainNameConfigurations": Sequence[DomainNameConfigurationUnionTypeDef],
+        "DomainNameConfigurations": Sequence[DomainNameConfigurationTypeDef],
         "MutualTlsAuthentication": MutualTlsAuthenticationInputTypeDef,
     },
     total=False,
 )
 
 
 class UpdateDomainNameRequestRequestTypeDef(
     _RequiredUpdateDomainNameRequestRequestTypeDef, _OptionalUpdateDomainNameRequestRequestTypeDef
 ):
     pass
+
+
+UpdateDomainNameResponseTypeDef = TypedDict(
+    "UpdateDomainNameResponseTypeDef",
+    {
+        "ApiMappingSelectionExpression": str,
+        "DomainName": str,
+        "DomainNameConfigurations": List[DomainNameConfigurationTypeDef],
+        "MutualTlsAuthentication": MutualTlsAuthenticationTypeDef,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDomainNamesResponseTypeDef = TypedDict(
+    "GetDomainNamesResponseTypeDef",
+    {
+        "Items": List[DomainNameTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2/type_defs.pyi` & `types-aiobotocore-apigatewayv2-2.5.2.post2/types_aiobotocore_apigatewayv2/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -42,23 +42,20 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AccessLogSettingsTypeDef",
     "ApiMappingTypeDef",
-    "CorsOutputTypeDef",
-    "JWTConfigurationOutputTypeDef",
     "CorsTypeDef",
+    "JWTConfigurationTypeDef",
     "CreateApiMappingRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
-    "JWTConfigurationTypeDef",
     "CreateDeploymentRequestRequestTypeDef",
     "MutualTlsAuthenticationInputTypeDef",
-    "DomainNameConfigurationOutputTypeDef",
     "MutualTlsAuthenticationTypeDef",
     "TlsConfigInputTypeDef",
     "CreateIntegrationResponseRequestRequestTypeDef",
     "TlsConfigTypeDef",
     "CreateModelRequestRequestTypeDef",
     "ParameterConstraintsTypeDef",
     "RouteSettingsTypeDef",
@@ -119,18 +116,19 @@
     "UntagResourceRequestRequestTypeDef",
     "UpdateApiMappingRequestRequestTypeDef",
     "UpdateDeploymentRequestRequestTypeDef",
     "UpdateIntegrationResponseRequestRequestTypeDef",
     "UpdateModelRequestRequestTypeDef",
     "UpdateVpcLinkRequestRequestTypeDef",
     "ApiTypeDef",
-    "AuthorizerTypeDef",
-    "CorsUnionTypeDef",
     "CreateApiRequestRequestTypeDef",
     "UpdateApiRequestRequestTypeDef",
+    "AuthorizerTypeDef",
+    "CreateAuthorizerRequestRequestTypeDef",
+    "UpdateAuthorizerRequestRequestTypeDef",
     "CreateApiMappingResponseTypeDef",
     "CreateApiResponseTypeDef",
     "CreateAuthorizerResponseTypeDef",
     "CreateDeploymentResponseTypeDef",
     "CreateIntegrationResponseResponseTypeDef",
     "CreateModelResponseTypeDef",
     "CreateVpcLinkResponseTypeDef",
@@ -151,21 +149,14 @@
     "UpdateApiMappingResponseTypeDef",
     "UpdateApiResponseTypeDef",
     "UpdateAuthorizerResponseTypeDef",
     "UpdateDeploymentResponseTypeDef",
     "UpdateIntegrationResponseResponseTypeDef",
     "UpdateModelResponseTypeDef",
     "UpdateVpcLinkResponseTypeDef",
-    "CreateAuthorizerRequestRequestTypeDef",
-    "JWTConfigurationUnionTypeDef",
-    "UpdateAuthorizerRequestRequestTypeDef",
-    "CreateDomainNameResponseTypeDef",
-    "DomainNameTypeDef",
-    "GetDomainNameResponseTypeDef",
-    "UpdateDomainNameResponseTypeDef",
     "CreateIntegrationRequestRequestTypeDef",
     "UpdateIntegrationRequestRequestTypeDef",
     "CreateIntegrationResultTypeDef",
     "GetIntegrationResultTypeDef",
     "IntegrationTypeDef",
     "UpdateIntegrationResultTypeDef",
     "CreateRouteRequestRequestTypeDef",
@@ -199,22 +190,25 @@
     "GetRoutesRequestGetRoutesPaginateTypeDef",
     "GetStagesRequestGetStagesPaginateTypeDef",
     "GetIntegrationResponsesResponseTypeDef",
     "GetModelsResponseTypeDef",
     "GetVpcLinksResponseTypeDef",
     "GetApisResponseTypeDef",
     "GetAuthorizersResponseTypeDef",
-    "GetDomainNamesResponseTypeDef",
     "GetIntegrationsResponseTypeDef",
     "GetRouteResponsesResponseTypeDef",
     "GetRoutesResponseTypeDef",
     "GetStagesResponseTypeDef",
-    "DomainNameConfigurationUnionTypeDef",
     "CreateDomainNameRequestRequestTypeDef",
+    "CreateDomainNameResponseTypeDef",
+    "DomainNameTypeDef",
+    "GetDomainNameResponseTypeDef",
     "UpdateDomainNameRequestRequestTypeDef",
+    "UpdateDomainNameResponseTypeDef",
+    "GetDomainNamesResponseTypeDef",
 )
 
 AccessLogSettingsTypeDef = TypedDict(
     "AccessLogSettingsTypeDef",
     {
         "DestinationArn": str,
         "Format": str,
@@ -237,49 +231,36 @@
     },
     total=False,
 )
 
 class ApiMappingTypeDef(_RequiredApiMappingTypeDef, _OptionalApiMappingTypeDef):
     pass
 
-CorsOutputTypeDef = TypedDict(
-    "CorsOutputTypeDef",
-    {
-        "AllowCredentials": bool,
-        "AllowHeaders": List[str],
-        "AllowMethods": List[str],
-        "AllowOrigins": List[str],
-        "ExposeHeaders": List[str],
-        "MaxAge": int,
-    },
-    total=False,
-)
-
-JWTConfigurationOutputTypeDef = TypedDict(
-    "JWTConfigurationOutputTypeDef",
-    {
-        "Audience": List[str],
-        "Issuer": str,
-    },
-    total=False,
-)
-
 CorsTypeDef = TypedDict(
     "CorsTypeDef",
     {
         "AllowCredentials": bool,
         "AllowHeaders": Sequence[str],
         "AllowMethods": Sequence[str],
         "AllowOrigins": Sequence[str],
         "ExposeHeaders": Sequence[str],
         "MaxAge": int,
     },
     total=False,
 )
 
+JWTConfigurationTypeDef = TypedDict(
+    "JWTConfigurationTypeDef",
+    {
+        "Audience": Sequence[str],
+        "Issuer": str,
+    },
+    total=False,
+)
+
 _RequiredCreateApiMappingRequestRequestTypeDef = TypedDict(
     "_RequiredCreateApiMappingRequestRequestTypeDef",
     {
         "ApiId": str,
         "DomainName": str,
         "Stage": str,
     },
@@ -304,23 +285,14 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-JWTConfigurationTypeDef = TypedDict(
-    "JWTConfigurationTypeDef",
-    {
-        "Audience": Sequence[str],
-        "Issuer": str,
-    },
-    total=False,
-)
-
 _RequiredCreateDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDeploymentRequestRequestTypeDef",
     {
         "ApiId": str,
     },
 )
 _OptionalCreateDeploymentRequestRequestTypeDef = TypedDict(
@@ -342,31 +314,14 @@
     {
         "TruststoreUri": str,
         "TruststoreVersion": str,
     },
     total=False,
 )
 
-DomainNameConfigurationOutputTypeDef = TypedDict(
-    "DomainNameConfigurationOutputTypeDef",
-    {
-        "ApiGatewayDomainName": str,
-        "CertificateArn": str,
-        "CertificateName": str,
-        "CertificateUploadDate": datetime,
-        "DomainNameStatus": DomainNameStatusType,
-        "DomainNameStatusMessage": str,
-        "EndpointType": EndpointTypeType,
-        "HostedZoneId": str,
-        "SecurityPolicy": SecurityPolicyType,
-        "OwnershipVerificationCertificateArn": str,
-    },
-    total=False,
-)
-
 MutualTlsAuthenticationTypeDef = TypedDict(
     "MutualTlsAuthenticationTypeDef",
     {
         "TruststoreUri": str,
         "TruststoreVersion": str,
         "TruststoreWarnings": List[str],
     },
@@ -1236,15 +1191,15 @@
 _OptionalApiTypeDef = TypedDict(
     "_OptionalApiTypeDef",
     {
         "ApiEndpoint": str,
         "ApiGatewayManaged": bool,
         "ApiId": str,
         "ApiKeySelectionExpression": str,
-        "CorsConfiguration": CorsOutputTypeDef,
+        "CorsConfiguration": CorsTypeDef,
         "CreatedDate": datetime,
         "Description": str,
         "DisableSchemaValidation": bool,
         "DisableExecuteApiEndpoint": bool,
         "ImportInfo": List[str],
         "Tags": Dict[str, str],
         "Version": str,
@@ -1252,41 +1207,14 @@
     },
     total=False,
 )
 
 class ApiTypeDef(_RequiredApiTypeDef, _OptionalApiTypeDef):
     pass
 
-_RequiredAuthorizerTypeDef = TypedDict(
-    "_RequiredAuthorizerTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalAuthorizerTypeDef = TypedDict(
-    "_OptionalAuthorizerTypeDef",
-    {
-        "AuthorizerCredentialsArn": str,
-        "AuthorizerId": str,
-        "AuthorizerPayloadFormatVersion": str,
-        "AuthorizerResultTtlInSeconds": int,
-        "AuthorizerType": AuthorizerTypeType,
-        "AuthorizerUri": str,
-        "EnableSimpleResponses": bool,
-        "IdentitySource": List[str],
-        "IdentityValidationExpression": str,
-        "JwtConfiguration": JWTConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-class AuthorizerTypeDef(_RequiredAuthorizerTypeDef, _OptionalAuthorizerTypeDef):
-    pass
-
-CorsUnionTypeDef = Union[CorsTypeDef, CorsOutputTypeDef]
 _RequiredCreateApiRequestRequestTypeDef = TypedDict(
     "_RequiredCreateApiRequestRequestTypeDef",
     {
         "Name": str,
         "ProtocolType": ProtocolTypeType,
     },
 )
@@ -1338,14 +1266,97 @@
 )
 
 class UpdateApiRequestRequestTypeDef(
     _RequiredUpdateApiRequestRequestTypeDef, _OptionalUpdateApiRequestRequestTypeDef
 ):
     pass
 
+_RequiredAuthorizerTypeDef = TypedDict(
+    "_RequiredAuthorizerTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalAuthorizerTypeDef = TypedDict(
+    "_OptionalAuthorizerTypeDef",
+    {
+        "AuthorizerCredentialsArn": str,
+        "AuthorizerId": str,
+        "AuthorizerPayloadFormatVersion": str,
+        "AuthorizerResultTtlInSeconds": int,
+        "AuthorizerType": AuthorizerTypeType,
+        "AuthorizerUri": str,
+        "EnableSimpleResponses": bool,
+        "IdentitySource": List[str],
+        "IdentityValidationExpression": str,
+        "JwtConfiguration": JWTConfigurationTypeDef,
+    },
+    total=False,
+)
+
+class AuthorizerTypeDef(_RequiredAuthorizerTypeDef, _OptionalAuthorizerTypeDef):
+    pass
+
+_RequiredCreateAuthorizerRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAuthorizerRequestRequestTypeDef",
+    {
+        "ApiId": str,
+        "AuthorizerType": AuthorizerTypeType,
+        "IdentitySource": Sequence[str],
+        "Name": str,
+    },
+)
+_OptionalCreateAuthorizerRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAuthorizerRequestRequestTypeDef",
+    {
+        "AuthorizerCredentialsArn": str,
+        "AuthorizerPayloadFormatVersion": str,
+        "AuthorizerResultTtlInSeconds": int,
+        "AuthorizerUri": str,
+        "EnableSimpleResponses": bool,
+        "IdentityValidationExpression": str,
+        "JwtConfiguration": JWTConfigurationTypeDef,
+    },
+    total=False,
+)
+
+class CreateAuthorizerRequestRequestTypeDef(
+    _RequiredCreateAuthorizerRequestRequestTypeDef, _OptionalCreateAuthorizerRequestRequestTypeDef
+):
+    pass
+
+_RequiredUpdateAuthorizerRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateAuthorizerRequestRequestTypeDef",
+    {
+        "ApiId": str,
+        "AuthorizerId": str,
+    },
+)
+_OptionalUpdateAuthorizerRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateAuthorizerRequestRequestTypeDef",
+    {
+        "AuthorizerCredentialsArn": str,
+        "AuthorizerPayloadFormatVersion": str,
+        "AuthorizerResultTtlInSeconds": int,
+        "AuthorizerType": AuthorizerTypeType,
+        "AuthorizerUri": str,
+        "EnableSimpleResponses": bool,
+        "IdentitySource": Sequence[str],
+        "IdentityValidationExpression": str,
+        "JwtConfiguration": JWTConfigurationTypeDef,
+        "Name": str,
+    },
+    total=False,
+)
+
+class UpdateAuthorizerRequestRequestTypeDef(
+    _RequiredUpdateAuthorizerRequestRequestTypeDef, _OptionalUpdateAuthorizerRequestRequestTypeDef
+):
+    pass
+
 CreateApiMappingResponseTypeDef = TypedDict(
     "CreateApiMappingResponseTypeDef",
     {
         "ApiId": str,
         "ApiMappingId": str,
         "ApiMappingKey": str,
         "Stage": str,
@@ -1356,15 +1367,15 @@
 CreateApiResponseTypeDef = TypedDict(
     "CreateApiResponseTypeDef",
     {
         "ApiEndpoint": str,
         "ApiGatewayManaged": bool,
         "ApiId": str,
         "ApiKeySelectionExpression": str,
-        "CorsConfiguration": CorsOutputTypeDef,
+        "CorsConfiguration": CorsTypeDef,
         "CreatedDate": datetime,
         "Description": str,
         "DisableSchemaValidation": bool,
         "DisableExecuteApiEndpoint": bool,
         "ImportInfo": List[str],
         "Name": str,
         "ProtocolType": ProtocolTypeType,
@@ -1384,15 +1395,15 @@
         "AuthorizerPayloadFormatVersion": str,
         "AuthorizerResultTtlInSeconds": int,
         "AuthorizerType": AuthorizerTypeType,
         "AuthorizerUri": str,
         "EnableSimpleResponses": bool,
         "IdentitySource": List[str],
         "IdentityValidationExpression": str,
-        "JwtConfiguration": JWTConfigurationOutputTypeDef,
+        "JwtConfiguration": JWTConfigurationTypeDef,
         "Name": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDeploymentResponseTypeDef = TypedDict(
     "CreateDeploymentResponseTypeDef",
@@ -1486,15 +1497,15 @@
 GetApiResponseTypeDef = TypedDict(
     "GetApiResponseTypeDef",
     {
         "ApiEndpoint": str,
         "ApiGatewayManaged": bool,
         "ApiId": str,
         "ApiKeySelectionExpression": str,
-        "CorsConfiguration": CorsOutputTypeDef,
+        "CorsConfiguration": CorsTypeDef,
         "CreatedDate": datetime,
         "Description": str,
         "DisableSchemaValidation": bool,
         "DisableExecuteApiEndpoint": bool,
         "ImportInfo": List[str],
         "Name": str,
         "ProtocolType": ProtocolTypeType,
@@ -1514,15 +1525,15 @@
         "AuthorizerPayloadFormatVersion": str,
         "AuthorizerResultTtlInSeconds": int,
         "AuthorizerType": AuthorizerTypeType,
         "AuthorizerUri": str,
         "EnableSimpleResponses": bool,
         "IdentitySource": List[str],
         "IdentityValidationExpression": str,
-        "JwtConfiguration": JWTConfigurationOutputTypeDef,
+        "JwtConfiguration": JWTConfigurationTypeDef,
         "Name": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDeploymentResponseTypeDef = TypedDict(
     "GetDeploymentResponseTypeDef",
@@ -1597,15 +1608,15 @@
 ImportApiResponseTypeDef = TypedDict(
     "ImportApiResponseTypeDef",
     {
         "ApiEndpoint": str,
         "ApiGatewayManaged": bool,
         "ApiId": str,
         "ApiKeySelectionExpression": str,
-        "CorsConfiguration": CorsOutputTypeDef,
+        "CorsConfiguration": CorsTypeDef,
         "CreatedDate": datetime,
         "Description": str,
         "DisableSchemaValidation": bool,
         "DisableExecuteApiEndpoint": bool,
         "ImportInfo": List[str],
         "Name": str,
         "ProtocolType": ProtocolTypeType,
@@ -1620,15 +1631,15 @@
 ReimportApiResponseTypeDef = TypedDict(
     "ReimportApiResponseTypeDef",
     {
         "ApiEndpoint": str,
         "ApiGatewayManaged": bool,
         "ApiId": str,
         "ApiKeySelectionExpression": str,
-        "CorsConfiguration": CorsOutputTypeDef,
+        "CorsConfiguration": CorsTypeDef,
         "CreatedDate": datetime,
         "Description": str,
         "DisableSchemaValidation": bool,
         "DisableExecuteApiEndpoint": bool,
         "ImportInfo": List[str],
         "Name": str,
         "ProtocolType": ProtocolTypeType,
@@ -1654,15 +1665,15 @@
 UpdateApiResponseTypeDef = TypedDict(
     "UpdateApiResponseTypeDef",
     {
         "ApiEndpoint": str,
         "ApiGatewayManaged": bool,
         "ApiId": str,
         "ApiKeySelectionExpression": str,
-        "CorsConfiguration": CorsOutputTypeDef,
+        "CorsConfiguration": CorsTypeDef,
         "CreatedDate": datetime,
         "Description": str,
         "DisableSchemaValidation": bool,
         "DisableExecuteApiEndpoint": bool,
         "ImportInfo": List[str],
         "Name": str,
         "ProtocolType": ProtocolTypeType,
@@ -1682,15 +1693,15 @@
         "AuthorizerPayloadFormatVersion": str,
         "AuthorizerResultTtlInSeconds": int,
         "AuthorizerType": AuthorizerTypeType,
         "AuthorizerUri": str,
         "EnableSimpleResponses": bool,
         "IdentitySource": List[str],
         "IdentityValidationExpression": str,
-        "JwtConfiguration": JWTConfigurationOutputTypeDef,
+        "JwtConfiguration": JWTConfigurationTypeDef,
         "Name": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDeploymentResponseTypeDef = TypedDict(
     "UpdateDeploymentResponseTypeDef",
@@ -1742,128 +1753,14 @@
         "VpcLinkStatus": VpcLinkStatusType,
         "VpcLinkStatusMessage": str,
         "VpcLinkVersion": Literal["V2"],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateAuthorizerRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateAuthorizerRequestRequestTypeDef",
-    {
-        "ApiId": str,
-        "AuthorizerType": AuthorizerTypeType,
-        "IdentitySource": Sequence[str],
-        "Name": str,
-    },
-)
-_OptionalCreateAuthorizerRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateAuthorizerRequestRequestTypeDef",
-    {
-        "AuthorizerCredentialsArn": str,
-        "AuthorizerPayloadFormatVersion": str,
-        "AuthorizerResultTtlInSeconds": int,
-        "AuthorizerUri": str,
-        "EnableSimpleResponses": bool,
-        "IdentityValidationExpression": str,
-        "JwtConfiguration": JWTConfigurationTypeDef,
-    },
-    total=False,
-)
-
-class CreateAuthorizerRequestRequestTypeDef(
-    _RequiredCreateAuthorizerRequestRequestTypeDef, _OptionalCreateAuthorizerRequestRequestTypeDef
-):
-    pass
-
-JWTConfigurationUnionTypeDef = Union[JWTConfigurationTypeDef, JWTConfigurationOutputTypeDef]
-_RequiredUpdateAuthorizerRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateAuthorizerRequestRequestTypeDef",
-    {
-        "ApiId": str,
-        "AuthorizerId": str,
-    },
-)
-_OptionalUpdateAuthorizerRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateAuthorizerRequestRequestTypeDef",
-    {
-        "AuthorizerCredentialsArn": str,
-        "AuthorizerPayloadFormatVersion": str,
-        "AuthorizerResultTtlInSeconds": int,
-        "AuthorizerType": AuthorizerTypeType,
-        "AuthorizerUri": str,
-        "EnableSimpleResponses": bool,
-        "IdentitySource": Sequence[str],
-        "IdentityValidationExpression": str,
-        "JwtConfiguration": JWTConfigurationTypeDef,
-        "Name": str,
-    },
-    total=False,
-)
-
-class UpdateAuthorizerRequestRequestTypeDef(
-    _RequiredUpdateAuthorizerRequestRequestTypeDef, _OptionalUpdateAuthorizerRequestRequestTypeDef
-):
-    pass
-
-CreateDomainNameResponseTypeDef = TypedDict(
-    "CreateDomainNameResponseTypeDef",
-    {
-        "ApiMappingSelectionExpression": str,
-        "DomainName": str,
-        "DomainNameConfigurations": List[DomainNameConfigurationOutputTypeDef],
-        "MutualTlsAuthentication": MutualTlsAuthenticationTypeDef,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredDomainNameTypeDef = TypedDict(
-    "_RequiredDomainNameTypeDef",
-    {
-        "DomainName": str,
-    },
-)
-_OptionalDomainNameTypeDef = TypedDict(
-    "_OptionalDomainNameTypeDef",
-    {
-        "ApiMappingSelectionExpression": str,
-        "DomainNameConfigurations": List[DomainNameConfigurationOutputTypeDef],
-        "MutualTlsAuthentication": MutualTlsAuthenticationTypeDef,
-        "Tags": Dict[str, str],
-    },
-    total=False,
-)
-
-class DomainNameTypeDef(_RequiredDomainNameTypeDef, _OptionalDomainNameTypeDef):
-    pass
-
-GetDomainNameResponseTypeDef = TypedDict(
-    "GetDomainNameResponseTypeDef",
-    {
-        "ApiMappingSelectionExpression": str,
-        "DomainName": str,
-        "DomainNameConfigurations": List[DomainNameConfigurationOutputTypeDef],
-        "MutualTlsAuthentication": MutualTlsAuthenticationTypeDef,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateDomainNameResponseTypeDef = TypedDict(
-    "UpdateDomainNameResponseTypeDef",
-    {
-        "ApiMappingSelectionExpression": str,
-        "DomainName": str,
-        "DomainNameConfigurations": List[DomainNameConfigurationOutputTypeDef],
-        "MutualTlsAuthentication": MutualTlsAuthenticationTypeDef,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateIntegrationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateIntegrationRequestRequestTypeDef",
     {
         "ApiId": str,
         "IntegrationType": IntegrationTypeType,
     },
 )
@@ -2683,23 +2580,14 @@
     {
         "Items": List[AuthorizerTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetDomainNamesResponseTypeDef = TypedDict(
-    "GetDomainNamesResponseTypeDef",
-    {
-        "Items": List[DomainNameTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 GetIntegrationsResponseTypeDef = TypedDict(
     "GetIntegrationsResponseTypeDef",
     {
         "Items": List[IntegrationTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2728,50 +2616,112 @@
     {
         "Items": List[StageTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DomainNameConfigurationUnionTypeDef = Union[
-    DomainNameConfigurationTypeDef, DomainNameConfigurationOutputTypeDef
-]
 _RequiredCreateDomainNameRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDomainNameRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalCreateDomainNameRequestRequestTypeDef = TypedDict(
     "_OptionalCreateDomainNameRequestRequestTypeDef",
     {
-        "DomainNameConfigurations": Sequence[DomainNameConfigurationUnionTypeDef],
+        "DomainNameConfigurations": Sequence[DomainNameConfigurationTypeDef],
         "MutualTlsAuthentication": MutualTlsAuthenticationInputTypeDef,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
 class CreateDomainNameRequestRequestTypeDef(
     _RequiredCreateDomainNameRequestRequestTypeDef, _OptionalCreateDomainNameRequestRequestTypeDef
 ):
     pass
 
+CreateDomainNameResponseTypeDef = TypedDict(
+    "CreateDomainNameResponseTypeDef",
+    {
+        "ApiMappingSelectionExpression": str,
+        "DomainName": str,
+        "DomainNameConfigurations": List[DomainNameConfigurationTypeDef],
+        "MutualTlsAuthentication": MutualTlsAuthenticationTypeDef,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredDomainNameTypeDef = TypedDict(
+    "_RequiredDomainNameTypeDef",
+    {
+        "DomainName": str,
+    },
+)
+_OptionalDomainNameTypeDef = TypedDict(
+    "_OptionalDomainNameTypeDef",
+    {
+        "ApiMappingSelectionExpression": str,
+        "DomainNameConfigurations": List[DomainNameConfigurationTypeDef],
+        "MutualTlsAuthentication": MutualTlsAuthenticationTypeDef,
+        "Tags": Dict[str, str],
+    },
+    total=False,
+)
+
+class DomainNameTypeDef(_RequiredDomainNameTypeDef, _OptionalDomainNameTypeDef):
+    pass
+
+GetDomainNameResponseTypeDef = TypedDict(
+    "GetDomainNameResponseTypeDef",
+    {
+        "ApiMappingSelectionExpression": str,
+        "DomainName": str,
+        "DomainNameConfigurations": List[DomainNameConfigurationTypeDef],
+        "MutualTlsAuthentication": MutualTlsAuthenticationTypeDef,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateDomainNameRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDomainNameRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalUpdateDomainNameRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateDomainNameRequestRequestTypeDef",
     {
-        "DomainNameConfigurations": Sequence[DomainNameConfigurationUnionTypeDef],
+        "DomainNameConfigurations": Sequence[DomainNameConfigurationTypeDef],
         "MutualTlsAuthentication": MutualTlsAuthenticationInputTypeDef,
     },
     total=False,
 )
 
 class UpdateDomainNameRequestRequestTypeDef(
     _RequiredUpdateDomainNameRequestRequestTypeDef, _OptionalUpdateDomainNameRequestRequestTypeDef
 ):
     pass
+
+UpdateDomainNameResponseTypeDef = TypedDict(
+    "UpdateDomainNameResponseTypeDef",
+    {
+        "ApiMappingSelectionExpression": str,
+        "DomainName": str,
+        "DomainNameConfigurations": List[DomainNameConfigurationTypeDef],
+        "MutualTlsAuthentication": MutualTlsAuthenticationTypeDef,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDomainNamesResponseTypeDef = TypedDict(
+    "GetDomainNamesResponseTypeDef",
+    {
+        "Items": List[DomainNameTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2.egg-info/SOURCES.txt` & `types-aiobotocore-apigatewayv2-2.5.2.post2/types_aiobotocore_apigatewayv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

