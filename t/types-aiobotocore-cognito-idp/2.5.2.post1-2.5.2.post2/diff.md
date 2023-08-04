# Comparing `tmp/types-aiobotocore-cognito-idp-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-cognito-idp-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-cognito-idp-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:05 2023, max compression
+gzip compressed data, was "types-aiobotocore-cognito-idp-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:39 2023, max compression
```

## Comparing `types-aiobotocore-cognito-idp-2.5.2.post1.tar` & `types-aiobotocore-cognito-idp-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:04.993618 types-aiobotocore-cognito-idp-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:35:20.000000 types-aiobotocore-cognito-idp-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    25922 2023-08-02 14:52:04.993618 types-aiobotocore-cognito-idp-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24376 2023-08-02 14:35:20.000000 types-aiobotocore-cognito-idp-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:04.993618 types-aiobotocore-cognito-idp-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-08-02 14:35:20.000000 types-aiobotocore-cognito-idp-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:04.993618 types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp/
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-08-02 14:35:20.000000 types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-08-02 14:35:20.000000 types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-08-02 14:35:20.000000 types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    82516 2023-08-02 14:35:20.000000 types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    82397 2023-08-02 14:35:20.000000 types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13626 2023-08-02 14:35:21.000000 types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13624 2023-08-02 14:35:21.000000 types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11573 2023-08-02 14:35:21.000000 types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11562 2023-08-02 14:35:20.000000 types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:35:20.000000 types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    99761 2023-08-02 14:35:24.000000 types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    99620 2023-08-02 14:35:23.000000 types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:35:20.000000 types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:04.993618 types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25922 2023-08-02 14:52:04.000000 types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-08-02 14:52:04.000000 types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:04.000000 types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:04.000000 types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:04.000000 types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-02 14:52:04.000000 types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:39.391645 types-aiobotocore-cognito-idp-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:42:37.000000 types-aiobotocore-cognito-idp-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14538 2023-08-04 12:00:39.387645 types-aiobotocore-cognito-idp-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12992 2023-08-04 11:42:37.000000 types-aiobotocore-cognito-idp-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:39.391645 types-aiobotocore-cognito-idp-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-08-04 11:42:37.000000 types-aiobotocore-cognito-idp-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:39.387645 types-aiobotocore-cognito-idp-2.5.2.post2/types_aiobotocore_cognito_idp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-08-04 11:42:37.000000 types-aiobotocore-cognito-idp-2.5.2.post2/types_aiobotocore_cognito_idp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-08-04 11:42:37.000000 types-aiobotocore-cognito-idp-2.5.2.post2/types_aiobotocore_cognito_idp/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-08-04 11:42:37.000000 types-aiobotocore-cognito-idp-2.5.2.post2/types_aiobotocore_cognito_idp/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82466 2023-08-04 11:42:38.000000 types-aiobotocore-cognito-idp-2.5.2.post2/types_aiobotocore_cognito_idp/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82347 2023-08-04 11:42:37.000000 types-aiobotocore-cognito-idp-2.5.2.post2/types_aiobotocore_cognito_idp/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13626 2023-08-04 11:42:39.000000 types-aiobotocore-cognito-idp-2.5.2.post2/types_aiobotocore_cognito_idp/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13624 2023-08-04 11:42:38.000000 types-aiobotocore-cognito-idp-2.5.2.post2/types_aiobotocore_cognito_idp/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11573 2023-08-04 11:42:38.000000 types-aiobotocore-cognito-idp-2.5.2.post2/types_aiobotocore_cognito_idp/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11562 2023-08-04 11:42:38.000000 types-aiobotocore-cognito-idp-2.5.2.post2/types_aiobotocore_cognito_idp/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:42:37.000000 types-aiobotocore-cognito-idp-2.5.2.post2/types_aiobotocore_cognito_idp/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    97370 2023-08-04 11:42:41.000000 types-aiobotocore-cognito-idp-2.5.2.post2/types_aiobotocore_cognito_idp/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97231 2023-08-04 11:42:40.000000 types-aiobotocore-cognito-idp-2.5.2.post2/types_aiobotocore_cognito_idp/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:42:37.000000 types-aiobotocore-cognito-idp-2.5.2.post2/types_aiobotocore_cognito_idp/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:39.387645 types-aiobotocore-cognito-idp-2.5.2.post2/types_aiobotocore_cognito_idp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14538 2023-08-04 12:00:39.000000 types-aiobotocore-cognito-idp-2.5.2.post2/types_aiobotocore_cognito_idp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-08-04 12:00:39.000000 types-aiobotocore-cognito-idp-2.5.2.post2/types_aiobotocore_cognito_idp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:39.000000 types-aiobotocore-cognito-idp-2.5.2.post2/types_aiobotocore_cognito_idp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:39.000000 types-aiobotocore-cognito-idp-2.5.2.post2/types_aiobotocore_cognito_idp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:39.000000 types-aiobotocore-cognito-idp-2.5.2.post2/types_aiobotocore_cognito_idp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-04 12:00:39.000000 types-aiobotocore-cognito-idp-2.5.2.post2/types_aiobotocore_cognito_idp.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-cognito-idp-2.5.2.post1/LICENSE` & `types-aiobotocore-cognito-idp-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cognito-idp-2.5.2.post1/setup.py` & `types-aiobotocore-cognito-idp-2.5.2.post2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-cognito-idp",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_cognito_idp"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CognitoIdentityProvider 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp/__init__.py` & `types-aiobotocore-cognito-idp-2.5.2.post2/types_aiobotocore_cognito_idp/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp/__init__.pyi` & `types-aiobotocore-cognito-idp-2.5.2.post2/types_aiobotocore_cognito_idp/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp/__main__.py` & `types-aiobotocore-cognito-idp-2.5.2.post2/types_aiobotocore_cognito_idp/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.CognitoIdentityProvider 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider\nOther"
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

### Comparing `types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp/client.py` & `types-aiobotocore-cognito-idp-2.5.2.post2/types_aiobotocore_cognito_idp/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     ListResourceServersPaginator,
     ListUserPoolClientsPaginator,
     ListUserPoolsPaginator,
     ListUsersInGroupPaginator,
     ListUsersPaginator,
 )
 from .type_defs import (
-    AccountRecoverySettingTypeUnionTypeDef,
+    AccountRecoverySettingTypeTypeDef,
     AccountTakeoverRiskConfigurationTypeTypeDef,
     AdminCreateUserConfigTypeTypeDef,
     AdminCreateUserResponseTypeDef,
     AdminGetDeviceResponseTypeDef,
     AdminGetUserResponseTypeDef,
     AdminInitiateAuthResponseTypeDef,
     AdminListDevicesResponseTypeDef,
@@ -61,15 +61,15 @@
     AdminListUserAuthEventsResponseTypeDef,
     AdminRespondToAuthChallengeResponseTypeDef,
     AnalyticsConfigurationTypeTypeDef,
     AnalyticsMetadataTypeTypeDef,
     AssociateSoftwareTokenResponseTypeDef,
     AttributeTypeTypeDef,
     BlobTypeDef,
-    CompromisedCredentialsRiskConfigurationTypeUnionTypeDef,
+    CompromisedCredentialsRiskConfigurationTypeTypeDef,
     ConfirmDeviceResponseTypeDef,
     ContextDataTypeTypeDef,
     CreateGroupResponseTypeDef,
     CreateIdentityProviderResponseTypeDef,
     CreateResourceServerResponseTypeDef,
     CreateUserImportJobResponseTypeDef,
     CreateUserPoolClientResponseTypeDef,
@@ -110,15 +110,15 @@
     ListUsersInGroupResponseTypeDef,
     ListUsersResponseTypeDef,
     MFAOptionTypeTypeDef,
     ProviderUserIdentifierTypeTypeDef,
     ResendConfirmationCodeResponseTypeDef,
     ResourceServerScopeTypeTypeDef,
     RespondToAuthChallengeResponseTypeDef,
-    RiskExceptionConfigurationTypeUnionTypeDef,
+    RiskExceptionConfigurationTypeTypeDef,
     SchemaAttributeTypeTypeDef,
     SetRiskConfigurationResponseTypeDef,
     SetUICustomizationResponseTypeDef,
     SetUserPoolMfaConfigResponseTypeDef,
     SignUpResponseTypeDef,
     SmsConfigurationTypeTypeDef,
     SmsMfaConfigTypeTypeDef,
@@ -130,15 +130,15 @@
     TokenValidityUnitsTypeTypeDef,
     UpdateGroupResponseTypeDef,
     UpdateIdentityProviderResponseTypeDef,
     UpdateResourceServerResponseTypeDef,
     UpdateUserAttributesResponseTypeDef,
     UpdateUserPoolClientResponseTypeDef,
     UpdateUserPoolDomainResponseTypeDef,
-    UserAttributeUpdateSettingsTypeUnionTypeDef,
+    UserAttributeUpdateSettingsTypeTypeDef,
     UserContextDataTypeTypeDef,
     UsernameConfigurationTypeTypeDef,
     UserPoolAddOnsTypeTypeDef,
     UserPoolPolicyTypeTypeDef,
     VerificationMessageTemplateTypeTypeDef,
     VerifySoftwareTokenResponseTypeDef,
 )
@@ -700,24 +700,24 @@
         UsernameAttributes: Sequence[UsernameAttributeTypeType] = ...,
         SmsVerificationMessage: str = ...,
         EmailVerificationMessage: str = ...,
         EmailVerificationSubject: str = ...,
         VerificationMessageTemplate: VerificationMessageTemplateTypeTypeDef = ...,
         SmsAuthenticationMessage: str = ...,
         MfaConfiguration: UserPoolMfaTypeType = ...,
-        UserAttributeUpdateSettings: UserAttributeUpdateSettingsTypeUnionTypeDef = ...,
+        UserAttributeUpdateSettings: UserAttributeUpdateSettingsTypeTypeDef = ...,
         DeviceConfiguration: DeviceConfigurationTypeTypeDef = ...,
         EmailConfiguration: EmailConfigurationTypeTypeDef = ...,
         SmsConfiguration: SmsConfigurationTypeTypeDef = ...,
         UserPoolTags: Mapping[str, str] = ...,
         AdminCreateUserConfig: AdminCreateUserConfigTypeTypeDef = ...,
         Schema: Sequence[SchemaAttributeTypeTypeDef] = ...,
         UserPoolAddOns: UserPoolAddOnsTypeTypeDef = ...,
         UsernameConfiguration: UsernameConfigurationTypeTypeDef = ...,
-        AccountRecoverySetting: AccountRecoverySettingTypeUnionTypeDef = ...
+        AccountRecoverySetting: AccountRecoverySettingTypeTypeDef = ...
     ) -> CreateUserPoolResponseTypeDef:
         """
         Creates a new Amazon Cognito user pool and sets the password policy for the
         pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.create_user_pool)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#create_user_pool)
@@ -1221,17 +1221,17 @@
         """
 
     async def set_risk_configuration(
         self,
         *,
         UserPoolId: str,
         ClientId: str = ...,
-        CompromisedCredentialsRiskConfiguration: CompromisedCredentialsRiskConfigurationTypeUnionTypeDef = ...,
+        CompromisedCredentialsRiskConfiguration: CompromisedCredentialsRiskConfigurationTypeTypeDef = ...,
         AccountTakeoverRiskConfiguration: AccountTakeoverRiskConfigurationTypeTypeDef = ...,
-        RiskExceptionConfiguration: RiskExceptionConfigurationTypeUnionTypeDef = ...
+        RiskExceptionConfiguration: RiskExceptionConfigurationTypeTypeDef = ...
     ) -> SetRiskConfigurationResponseTypeDef:
         """
         Configures actions on detected risks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.set_risk_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#set_risk_configuration)
         """
@@ -1445,23 +1445,23 @@
         LambdaConfig: LambdaConfigTypeTypeDef = ...,
         AutoVerifiedAttributes: Sequence[VerifiedAttributeTypeType] = ...,
         SmsVerificationMessage: str = ...,
         EmailVerificationMessage: str = ...,
         EmailVerificationSubject: str = ...,
         VerificationMessageTemplate: VerificationMessageTemplateTypeTypeDef = ...,
         SmsAuthenticationMessage: str = ...,
-        UserAttributeUpdateSettings: UserAttributeUpdateSettingsTypeUnionTypeDef = ...,
+        UserAttributeUpdateSettings: UserAttributeUpdateSettingsTypeTypeDef = ...,
         MfaConfiguration: UserPoolMfaTypeType = ...,
         DeviceConfiguration: DeviceConfigurationTypeTypeDef = ...,
         EmailConfiguration: EmailConfigurationTypeTypeDef = ...,
         SmsConfiguration: SmsConfigurationTypeTypeDef = ...,
         UserPoolTags: Mapping[str, str] = ...,
         AdminCreateUserConfig: AdminCreateUserConfigTypeTypeDef = ...,
         UserPoolAddOns: UserPoolAddOnsTypeTypeDef = ...,
-        AccountRecoverySetting: AccountRecoverySettingTypeUnionTypeDef = ...
+        AccountRecoverySetting: AccountRecoverySettingTypeTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates the specified user pool with the specified attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.update_user_pool)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#update_user_pool)
         """
```

### Comparing `types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp/client.pyi` & `types-aiobotocore-cognito-idp-2.5.2.post2/types_aiobotocore_cognito_idp/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     ListResourceServersPaginator,
     ListUserPoolClientsPaginator,
     ListUserPoolsPaginator,
     ListUsersInGroupPaginator,
     ListUsersPaginator,
 )
 from .type_defs import (
-    AccountRecoverySettingTypeUnionTypeDef,
+    AccountRecoverySettingTypeTypeDef,
     AccountTakeoverRiskConfigurationTypeTypeDef,
     AdminCreateUserConfigTypeTypeDef,
     AdminCreateUserResponseTypeDef,
     AdminGetDeviceResponseTypeDef,
     AdminGetUserResponseTypeDef,
     AdminInitiateAuthResponseTypeDef,
     AdminListDevicesResponseTypeDef,
@@ -61,15 +61,15 @@
     AdminListUserAuthEventsResponseTypeDef,
     AdminRespondToAuthChallengeResponseTypeDef,
     AnalyticsConfigurationTypeTypeDef,
     AnalyticsMetadataTypeTypeDef,
     AssociateSoftwareTokenResponseTypeDef,
     AttributeTypeTypeDef,
     BlobTypeDef,
-    CompromisedCredentialsRiskConfigurationTypeUnionTypeDef,
+    CompromisedCredentialsRiskConfigurationTypeTypeDef,
     ConfirmDeviceResponseTypeDef,
     ContextDataTypeTypeDef,
     CreateGroupResponseTypeDef,
     CreateIdentityProviderResponseTypeDef,
     CreateResourceServerResponseTypeDef,
     CreateUserImportJobResponseTypeDef,
     CreateUserPoolClientResponseTypeDef,
@@ -110,15 +110,15 @@
     ListUsersInGroupResponseTypeDef,
     ListUsersResponseTypeDef,
     MFAOptionTypeTypeDef,
     ProviderUserIdentifierTypeTypeDef,
     ResendConfirmationCodeResponseTypeDef,
     ResourceServerScopeTypeTypeDef,
     RespondToAuthChallengeResponseTypeDef,
-    RiskExceptionConfigurationTypeUnionTypeDef,
+    RiskExceptionConfigurationTypeTypeDef,
     SchemaAttributeTypeTypeDef,
     SetRiskConfigurationResponseTypeDef,
     SetUICustomizationResponseTypeDef,
     SetUserPoolMfaConfigResponseTypeDef,
     SignUpResponseTypeDef,
     SmsConfigurationTypeTypeDef,
     SmsMfaConfigTypeTypeDef,
@@ -130,15 +130,15 @@
     TokenValidityUnitsTypeTypeDef,
     UpdateGroupResponseTypeDef,
     UpdateIdentityProviderResponseTypeDef,
     UpdateResourceServerResponseTypeDef,
     UpdateUserAttributesResponseTypeDef,
     UpdateUserPoolClientResponseTypeDef,
     UpdateUserPoolDomainResponseTypeDef,
-    UserAttributeUpdateSettingsTypeUnionTypeDef,
+    UserAttributeUpdateSettingsTypeTypeDef,
     UserContextDataTypeTypeDef,
     UsernameConfigurationTypeTypeDef,
     UserPoolAddOnsTypeTypeDef,
     UserPoolPolicyTypeTypeDef,
     VerificationMessageTemplateTypeTypeDef,
     VerifySoftwareTokenResponseTypeDef,
 )
@@ -657,24 +657,24 @@
         UsernameAttributes: Sequence[UsernameAttributeTypeType] = ...,
         SmsVerificationMessage: str = ...,
         EmailVerificationMessage: str = ...,
         EmailVerificationSubject: str = ...,
         VerificationMessageTemplate: VerificationMessageTemplateTypeTypeDef = ...,
         SmsAuthenticationMessage: str = ...,
         MfaConfiguration: UserPoolMfaTypeType = ...,
-        UserAttributeUpdateSettings: UserAttributeUpdateSettingsTypeUnionTypeDef = ...,
+        UserAttributeUpdateSettings: UserAttributeUpdateSettingsTypeTypeDef = ...,
         DeviceConfiguration: DeviceConfigurationTypeTypeDef = ...,
         EmailConfiguration: EmailConfigurationTypeTypeDef = ...,
         SmsConfiguration: SmsConfigurationTypeTypeDef = ...,
         UserPoolTags: Mapping[str, str] = ...,
         AdminCreateUserConfig: AdminCreateUserConfigTypeTypeDef = ...,
         Schema: Sequence[SchemaAttributeTypeTypeDef] = ...,
         UserPoolAddOns: UserPoolAddOnsTypeTypeDef = ...,
         UsernameConfiguration: UsernameConfigurationTypeTypeDef = ...,
-        AccountRecoverySetting: AccountRecoverySettingTypeUnionTypeDef = ...
+        AccountRecoverySetting: AccountRecoverySettingTypeTypeDef = ...
     ) -> CreateUserPoolResponseTypeDef:
         """
         Creates a new Amazon Cognito user pool and sets the password policy for the
         pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.create_user_pool)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#create_user_pool)
@@ -1133,17 +1133,17 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#revoke_token)
         """
     async def set_risk_configuration(
         self,
         *,
         UserPoolId: str,
         ClientId: str = ...,
-        CompromisedCredentialsRiskConfiguration: CompromisedCredentialsRiskConfigurationTypeUnionTypeDef = ...,
+        CompromisedCredentialsRiskConfiguration: CompromisedCredentialsRiskConfigurationTypeTypeDef = ...,
         AccountTakeoverRiskConfiguration: AccountTakeoverRiskConfigurationTypeTypeDef = ...,
-        RiskExceptionConfiguration: RiskExceptionConfigurationTypeUnionTypeDef = ...
+        RiskExceptionConfiguration: RiskExceptionConfigurationTypeTypeDef = ...
     ) -> SetRiskConfigurationResponseTypeDef:
         """
         Configures actions on detected risks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.set_risk_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#set_risk_configuration)
         """
@@ -1341,23 +1341,23 @@
         LambdaConfig: LambdaConfigTypeTypeDef = ...,
         AutoVerifiedAttributes: Sequence[VerifiedAttributeTypeType] = ...,
         SmsVerificationMessage: str = ...,
         EmailVerificationMessage: str = ...,
         EmailVerificationSubject: str = ...,
         VerificationMessageTemplate: VerificationMessageTemplateTypeTypeDef = ...,
         SmsAuthenticationMessage: str = ...,
-        UserAttributeUpdateSettings: UserAttributeUpdateSettingsTypeUnionTypeDef = ...,
+        UserAttributeUpdateSettings: UserAttributeUpdateSettingsTypeTypeDef = ...,
         MfaConfiguration: UserPoolMfaTypeType = ...,
         DeviceConfiguration: DeviceConfigurationTypeTypeDef = ...,
         EmailConfiguration: EmailConfigurationTypeTypeDef = ...,
         SmsConfiguration: SmsConfigurationTypeTypeDef = ...,
         UserPoolTags: Mapping[str, str] = ...,
         AdminCreateUserConfig: AdminCreateUserConfigTypeTypeDef = ...,
         UserPoolAddOns: UserPoolAddOnsTypeTypeDef = ...,
-        AccountRecoverySetting: AccountRecoverySettingTypeUnionTypeDef = ...
+        AccountRecoverySetting: AccountRecoverySettingTypeTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates the specified user pool with the specified attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.update_user_pool)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_idp/client/#update_user_pool)
         """
```

### Comparing `types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp/literals.py` & `types-aiobotocore-cognito-idp-2.5.2.post2/types_aiobotocore_cognito_idp/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp/literals.pyi` & `types-aiobotocore-cognito-idp-2.5.2.post2/types_aiobotocore_cognito_idp/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp/paginator.py` & `types-aiobotocore-cognito-idp-2.5.2.post2/types_aiobotocore_cognito_idp/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp/paginator.pyi` & `types-aiobotocore-cognito-idp-2.5.2.post2/types_aiobotocore_cognito_idp/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp/type_defs.py` & `types-aiobotocore-cognito-idp-2.5.2.post2/types_aiobotocore_cognito_idp/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,29 +167,26 @@
     "ListUserPoolsRequestRequestTypeDef",
     "ListUsersInGroupRequestRequestTypeDef",
     "ListUsersRequestRequestTypeDef",
     "NotifyEmailTypeTypeDef",
     "NumberAttributeConstraintsTypeTypeDef",
     "PasswordPolicyTypeTypeDef",
     "RevokeTokenRequestRequestTypeDef",
-    "RiskExceptionConfigurationTypeOutputTypeDef",
     "RiskExceptionConfigurationTypeTypeDef",
     "StringAttributeConstraintsTypeTypeDef",
     "StartUserImportJobRequestRequestTypeDef",
     "StopUserImportJobRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAuthEventFeedbackRequestRequestTypeDef",
     "UpdateDeviceStatusRequestRequestTypeDef",
     "UpdateGroupRequestRequestTypeDef",
     "UpdateIdentityProviderRequestRequestTypeDef",
-    "UserAttributeUpdateSettingsTypeOutputTypeDef",
     "VerifySoftwareTokenRequestRequestTypeDef",
     "VerifyUserAttributeRequestRequestTypeDef",
-    "AccountRecoverySettingTypeOutputTypeDef",
     "AccountRecoverySettingTypeTypeDef",
     "AccountTakeoverActionsTypeTypeDef",
     "AdminCreateUserConfigTypeTypeDef",
     "AdminCreateUserRequestRequestTypeDef",
     "AdminUpdateUserAttributesRequestRequestTypeDef",
     "DeviceTypeTypeDef",
     "UpdateUserAttributesRequestRequestTypeDef",
@@ -229,15 +226,14 @@
     "AuthenticationResultTypeTypeDef",
     "SetUICustomizationRequestRequestTypeDef",
     "ForgotPasswordResponseTypeDef",
     "GetUserAttributeVerificationCodeResponseTypeDef",
     "ResendConfirmationCodeResponseTypeDef",
     "SignUpResponseTypeDef",
     "UpdateUserAttributesResponseTypeDef",
-    "CompromisedCredentialsRiskConfigurationTypeOutputTypeDef",
     "CompromisedCredentialsRiskConfigurationTypeTypeDef",
     "ConfirmDeviceRequestRequestTypeDef",
     "ConfirmForgotPasswordRequestRequestTypeDef",
     "ConfirmSignUpRequestRequestTypeDef",
     "ForgotPasswordRequestRequestTypeDef",
     "InitiateAuthRequestRequestTypeDef",
     "ResendConfirmationCodeRequestRequestTypeDef",
@@ -266,31 +262,27 @@
     "LambdaConfigTypeTypeDef",
     "GetUICustomizationResponseTypeDef",
     "SetUICustomizationResponseTypeDef",
     "ListIdentityProvidersResponseTypeDef",
     "ListUserPoolClientsResponseTypeDef",
     "NotifyConfigurationTypeTypeDef",
     "UserPoolPolicyTypeTypeDef",
-    "RiskExceptionConfigurationTypeUnionTypeDef",
     "SchemaAttributeTypeTypeDef",
-    "UserAttributeUpdateSettingsTypeUnionTypeDef",
-    "AccountRecoverySettingTypeUnionTypeDef",
     "AdminGetDeviceResponseTypeDef",
     "AdminListDevicesResponseTypeDef",
     "GetDeviceResponseTypeDef",
     "ListDevicesResponseTypeDef",
     "AdminCreateUserResponseTypeDef",
     "ListUsersInGroupResponseTypeDef",
     "ListUsersResponseTypeDef",
     "AdminListUserAuthEventsResponseTypeDef",
     "AdminInitiateAuthResponseTypeDef",
     "AdminRespondToAuthChallengeResponseTypeDef",
     "InitiateAuthResponseTypeDef",
     "RespondToAuthChallengeResponseTypeDef",
-    "CompromisedCredentialsRiskConfigurationTypeUnionTypeDef",
     "AdminInitiateAuthRequestRequestTypeDef",
     "AdminRespondToAuthChallengeRequestRequestTypeDef",
     "CreateResourceServerResponseTypeDef",
     "DescribeResourceServerResponseTypeDef",
     "ListResourceServersResponseTypeDef",
     "UpdateResourceServerResponseTypeDef",
     "CreateUserPoolClientResponseTypeDef",
@@ -1632,28 +1624,19 @@
 
 class RevokeTokenRequestRequestTypeDef(
     _RequiredRevokeTokenRequestRequestTypeDef, _OptionalRevokeTokenRequestRequestTypeDef
 ):
     pass
 
 
-RiskExceptionConfigurationTypeOutputTypeDef = TypedDict(
-    "RiskExceptionConfigurationTypeOutputTypeDef",
-    {
-        "BlockedIPRangeList": List[str],
-        "SkippedIPRangeList": List[str],
-    },
-    total=False,
-)
-
 RiskExceptionConfigurationTypeTypeDef = TypedDict(
     "RiskExceptionConfigurationTypeTypeDef",
     {
-        "BlockedIPRangeList": Sequence[str],
-        "SkippedIPRangeList": Sequence[str],
+        "BlockedIPRangeList": List[str],
+        "SkippedIPRangeList": List[str],
     },
     total=False,
 )
 
 StringAttributeConstraintsTypeTypeDef = TypedDict(
     "StringAttributeConstraintsTypeTypeDef",
     {
@@ -1774,22 +1757,14 @@
 class UpdateIdentityProviderRequestRequestTypeDef(
     _RequiredUpdateIdentityProviderRequestRequestTypeDef,
     _OptionalUpdateIdentityProviderRequestRequestTypeDef,
 ):
     pass
 
 
-UserAttributeUpdateSettingsTypeOutputTypeDef = TypedDict(
-    "UserAttributeUpdateSettingsTypeOutputTypeDef",
-    {
-        "AttributesRequireVerificationBeforeUpdate": List[VerifiedAttributeTypeType],
-    },
-    total=False,
-)
-
 _RequiredVerifySoftwareTokenRequestRequestTypeDef = TypedDict(
     "_RequiredVerifySoftwareTokenRequestRequestTypeDef",
     {
         "UserCode": str,
     },
 )
 _OptionalVerifySoftwareTokenRequestRequestTypeDef = TypedDict(
@@ -1815,22 +1790,14 @@
     {
         "AccessToken": str,
         "AttributeName": str,
         "Code": str,
     },
 )
 
-AccountRecoverySettingTypeOutputTypeDef = TypedDict(
-    "AccountRecoverySettingTypeOutputTypeDef",
-    {
-        "RecoveryMechanisms": List[RecoveryOptionTypeTypeDef],
-    },
-    total=False,
-)
-
 AccountRecoverySettingTypeTypeDef = TypedDict(
     "AccountRecoverySettingTypeTypeDef",
     {
         "RecoveryMechanisms": Sequence[RecoveryOptionTypeTypeDef],
     },
     total=False,
 )
@@ -2460,46 +2427,24 @@
     "UpdateUserAttributesResponseTypeDef",
     {
         "CodeDeliveryDetailsList": List[CodeDeliveryDetailsTypeTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCompromisedCredentialsRiskConfigurationTypeOutputTypeDef = TypedDict(
-    "_RequiredCompromisedCredentialsRiskConfigurationTypeOutputTypeDef",
-    {
-        "Actions": CompromisedCredentialsActionsTypeTypeDef,
-    },
-)
-_OptionalCompromisedCredentialsRiskConfigurationTypeOutputTypeDef = TypedDict(
-    "_OptionalCompromisedCredentialsRiskConfigurationTypeOutputTypeDef",
-    {
-        "EventFilter": List[EventFilterTypeType],
-    },
-    total=False,
-)
-
-
-class CompromisedCredentialsRiskConfigurationTypeOutputTypeDef(
-    _RequiredCompromisedCredentialsRiskConfigurationTypeOutputTypeDef,
-    _OptionalCompromisedCredentialsRiskConfigurationTypeOutputTypeDef,
-):
-    pass
-
-
 _RequiredCompromisedCredentialsRiskConfigurationTypeTypeDef = TypedDict(
     "_RequiredCompromisedCredentialsRiskConfigurationTypeTypeDef",
     {
         "Actions": CompromisedCredentialsActionsTypeTypeDef,
     },
 )
 _OptionalCompromisedCredentialsRiskConfigurationTypeTypeDef = TypedDict(
     "_OptionalCompromisedCredentialsRiskConfigurationTypeTypeDef",
     {
-        "EventFilter": Sequence[EventFilterTypeType],
+        "EventFilter": List[EventFilterTypeType],
     },
     total=False,
 )
 
 
 class CompromisedCredentialsRiskConfigurationTypeTypeDef(
     _RequiredCompromisedCredentialsRiskConfigurationTypeTypeDef,
@@ -3126,37 +3071,28 @@
     "UserPoolPolicyTypeTypeDef",
     {
         "PasswordPolicy": PasswordPolicyTypeTypeDef,
     },
     total=False,
 )
 
-RiskExceptionConfigurationTypeUnionTypeDef = Union[
-    RiskExceptionConfigurationTypeTypeDef, RiskExceptionConfigurationTypeOutputTypeDef
-]
 SchemaAttributeTypeTypeDef = TypedDict(
     "SchemaAttributeTypeTypeDef",
     {
         "Name": str,
         "AttributeDataType": AttributeDataTypeType,
         "DeveloperOnlyAttribute": bool,
         "Mutable": bool,
         "Required": bool,
         "NumberAttributeConstraints": NumberAttributeConstraintsTypeTypeDef,
         "StringAttributeConstraints": StringAttributeConstraintsTypeTypeDef,
     },
     total=False,
 )
 
-UserAttributeUpdateSettingsTypeUnionTypeDef = Union[
-    UserAttributeUpdateSettingsTypeTypeDef, UserAttributeUpdateSettingsTypeOutputTypeDef
-]
-AccountRecoverySettingTypeUnionTypeDef = Union[
-    AccountRecoverySettingTypeTypeDef, AccountRecoverySettingTypeOutputTypeDef
-]
 AdminGetDeviceResponseTypeDef = TypedDict(
     "AdminGetDeviceResponseTypeDef",
     {
         "Device": DeviceTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3262,18 +3198,14 @@
         "Session": str,
         "ChallengeParameters": Dict[str, str],
         "AuthenticationResult": AuthenticationResultTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CompromisedCredentialsRiskConfigurationTypeUnionTypeDef = Union[
-    CompromisedCredentialsRiskConfigurationTypeTypeDef,
-    CompromisedCredentialsRiskConfigurationTypeOutputTypeDef,
-]
 _RequiredAdminInitiateAuthRequestRequestTypeDef = TypedDict(
     "_RequiredAdminInitiateAuthRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "ClientId": str,
         "AuthFlow": AuthFlowTypeType,
     },
@@ -3572,30 +3504,30 @@
         "AliasAttributes": List[AliasAttributeTypeType],
         "UsernameAttributes": List[UsernameAttributeTypeType],
         "SmsVerificationMessage": str,
         "EmailVerificationMessage": str,
         "EmailVerificationSubject": str,
         "VerificationMessageTemplate": VerificationMessageTemplateTypeTypeDef,
         "SmsAuthenticationMessage": str,
-        "UserAttributeUpdateSettings": UserAttributeUpdateSettingsTypeOutputTypeDef,
+        "UserAttributeUpdateSettings": UserAttributeUpdateSettingsTypeTypeDef,
         "MfaConfiguration": UserPoolMfaTypeType,
         "DeviceConfiguration": DeviceConfigurationTypeTypeDef,
         "EstimatedNumberOfUsers": int,
         "EmailConfiguration": EmailConfigurationTypeTypeDef,
         "SmsConfiguration": SmsConfigurationTypeTypeDef,
         "UserPoolTags": Dict[str, str],
         "SmsConfigurationFailure": str,
         "EmailConfigurationFailure": str,
         "Domain": str,
         "CustomDomain": str,
         "AdminCreateUserConfig": AdminCreateUserConfigTypeTypeDef,
         "UserPoolAddOns": UserPoolAddOnsTypeTypeDef,
         "UsernameConfiguration": UsernameConfigurationTypeTypeDef,
         "Arn": str,
-        "AccountRecoverySetting": AccountRecoverySettingTypeOutputTypeDef,
+        "AccountRecoverySetting": AccountRecoverySettingTypeTypeDef,
     },
     total=False,
 )
 
 ListUserPoolsResponseTypeDef = TypedDict(
     "ListUserPoolsResponseTypeDef",
     {
@@ -3607,18 +3539,18 @@
 
 RiskConfigurationTypeTypeDef = TypedDict(
     "RiskConfigurationTypeTypeDef",
     {
         "UserPoolId": str,
         "ClientId": str,
         "CompromisedCredentialsRiskConfiguration": (
-            CompromisedCredentialsRiskConfigurationTypeOutputTypeDef
+            CompromisedCredentialsRiskConfigurationTypeTypeDef
         ),
         "AccountTakeoverRiskConfiguration": AccountTakeoverRiskConfigurationTypeTypeDef,
-        "RiskExceptionConfiguration": RiskExceptionConfigurationTypeOutputTypeDef,
+        "RiskExceptionConfiguration": RiskExceptionConfigurationTypeTypeDef,
         "LastModifiedDate": datetime,
     },
     total=False,
 )
 
 _RequiredSetRiskConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredSetRiskConfigurationRequestRequestTypeDef",
```

### Comparing `types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp/type_defs.pyi` & `types-aiobotocore-cognito-idp-2.5.2.post2/types_aiobotocore_cognito_idp/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -166,29 +166,26 @@
     "ListUserPoolsRequestRequestTypeDef",
     "ListUsersInGroupRequestRequestTypeDef",
     "ListUsersRequestRequestTypeDef",
     "NotifyEmailTypeTypeDef",
     "NumberAttributeConstraintsTypeTypeDef",
     "PasswordPolicyTypeTypeDef",
     "RevokeTokenRequestRequestTypeDef",
-    "RiskExceptionConfigurationTypeOutputTypeDef",
     "RiskExceptionConfigurationTypeTypeDef",
     "StringAttributeConstraintsTypeTypeDef",
     "StartUserImportJobRequestRequestTypeDef",
     "StopUserImportJobRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAuthEventFeedbackRequestRequestTypeDef",
     "UpdateDeviceStatusRequestRequestTypeDef",
     "UpdateGroupRequestRequestTypeDef",
     "UpdateIdentityProviderRequestRequestTypeDef",
-    "UserAttributeUpdateSettingsTypeOutputTypeDef",
     "VerifySoftwareTokenRequestRequestTypeDef",
     "VerifyUserAttributeRequestRequestTypeDef",
-    "AccountRecoverySettingTypeOutputTypeDef",
     "AccountRecoverySettingTypeTypeDef",
     "AccountTakeoverActionsTypeTypeDef",
     "AdminCreateUserConfigTypeTypeDef",
     "AdminCreateUserRequestRequestTypeDef",
     "AdminUpdateUserAttributesRequestRequestTypeDef",
     "DeviceTypeTypeDef",
     "UpdateUserAttributesRequestRequestTypeDef",
@@ -228,15 +225,14 @@
     "AuthenticationResultTypeTypeDef",
     "SetUICustomizationRequestRequestTypeDef",
     "ForgotPasswordResponseTypeDef",
     "GetUserAttributeVerificationCodeResponseTypeDef",
     "ResendConfirmationCodeResponseTypeDef",
     "SignUpResponseTypeDef",
     "UpdateUserAttributesResponseTypeDef",
-    "CompromisedCredentialsRiskConfigurationTypeOutputTypeDef",
     "CompromisedCredentialsRiskConfigurationTypeTypeDef",
     "ConfirmDeviceRequestRequestTypeDef",
     "ConfirmForgotPasswordRequestRequestTypeDef",
     "ConfirmSignUpRequestRequestTypeDef",
     "ForgotPasswordRequestRequestTypeDef",
     "InitiateAuthRequestRequestTypeDef",
     "ResendConfirmationCodeRequestRequestTypeDef",
@@ -265,31 +261,27 @@
     "LambdaConfigTypeTypeDef",
     "GetUICustomizationResponseTypeDef",
     "SetUICustomizationResponseTypeDef",
     "ListIdentityProvidersResponseTypeDef",
     "ListUserPoolClientsResponseTypeDef",
     "NotifyConfigurationTypeTypeDef",
     "UserPoolPolicyTypeTypeDef",
-    "RiskExceptionConfigurationTypeUnionTypeDef",
     "SchemaAttributeTypeTypeDef",
-    "UserAttributeUpdateSettingsTypeUnionTypeDef",
-    "AccountRecoverySettingTypeUnionTypeDef",
     "AdminGetDeviceResponseTypeDef",
     "AdminListDevicesResponseTypeDef",
     "GetDeviceResponseTypeDef",
     "ListDevicesResponseTypeDef",
     "AdminCreateUserResponseTypeDef",
     "ListUsersInGroupResponseTypeDef",
     "ListUsersResponseTypeDef",
     "AdminListUserAuthEventsResponseTypeDef",
     "AdminInitiateAuthResponseTypeDef",
     "AdminRespondToAuthChallengeResponseTypeDef",
     "InitiateAuthResponseTypeDef",
     "RespondToAuthChallengeResponseTypeDef",
-    "CompromisedCredentialsRiskConfigurationTypeUnionTypeDef",
     "AdminInitiateAuthRequestRequestTypeDef",
     "AdminRespondToAuthChallengeRequestRequestTypeDef",
     "CreateResourceServerResponseTypeDef",
     "DescribeResourceServerResponseTypeDef",
     "ListResourceServersResponseTypeDef",
     "UpdateResourceServerResponseTypeDef",
     "CreateUserPoolClientResponseTypeDef",
@@ -1575,28 +1567,19 @@
 )
 
 class RevokeTokenRequestRequestTypeDef(
     _RequiredRevokeTokenRequestRequestTypeDef, _OptionalRevokeTokenRequestRequestTypeDef
 ):
     pass
 
-RiskExceptionConfigurationTypeOutputTypeDef = TypedDict(
-    "RiskExceptionConfigurationTypeOutputTypeDef",
-    {
-        "BlockedIPRangeList": List[str],
-        "SkippedIPRangeList": List[str],
-    },
-    total=False,
-)
-
 RiskExceptionConfigurationTypeTypeDef = TypedDict(
     "RiskExceptionConfigurationTypeTypeDef",
     {
-        "BlockedIPRangeList": Sequence[str],
-        "SkippedIPRangeList": Sequence[str],
+        "BlockedIPRangeList": List[str],
+        "SkippedIPRangeList": List[str],
     },
     total=False,
 )
 
 StringAttributeConstraintsTypeTypeDef = TypedDict(
     "StringAttributeConstraintsTypeTypeDef",
     {
@@ -1711,22 +1694,14 @@
 
 class UpdateIdentityProviderRequestRequestTypeDef(
     _RequiredUpdateIdentityProviderRequestRequestTypeDef,
     _OptionalUpdateIdentityProviderRequestRequestTypeDef,
 ):
     pass
 
-UserAttributeUpdateSettingsTypeOutputTypeDef = TypedDict(
-    "UserAttributeUpdateSettingsTypeOutputTypeDef",
-    {
-        "AttributesRequireVerificationBeforeUpdate": List[VerifiedAttributeTypeType],
-    },
-    total=False,
-)
-
 _RequiredVerifySoftwareTokenRequestRequestTypeDef = TypedDict(
     "_RequiredVerifySoftwareTokenRequestRequestTypeDef",
     {
         "UserCode": str,
     },
 )
 _OptionalVerifySoftwareTokenRequestRequestTypeDef = TypedDict(
@@ -1750,22 +1725,14 @@
     {
         "AccessToken": str,
         "AttributeName": str,
         "Code": str,
     },
 )
 
-AccountRecoverySettingTypeOutputTypeDef = TypedDict(
-    "AccountRecoverySettingTypeOutputTypeDef",
-    {
-        "RecoveryMechanisms": List[RecoveryOptionTypeTypeDef],
-    },
-    total=False,
-)
-
 AccountRecoverySettingTypeTypeDef = TypedDict(
     "AccountRecoverySettingTypeTypeDef",
     {
         "RecoveryMechanisms": Sequence[RecoveryOptionTypeTypeDef],
     },
     total=False,
 )
@@ -2367,44 +2334,24 @@
     "UpdateUserAttributesResponseTypeDef",
     {
         "CodeDeliveryDetailsList": List[CodeDeliveryDetailsTypeTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCompromisedCredentialsRiskConfigurationTypeOutputTypeDef = TypedDict(
-    "_RequiredCompromisedCredentialsRiskConfigurationTypeOutputTypeDef",
-    {
-        "Actions": CompromisedCredentialsActionsTypeTypeDef,
-    },
-)
-_OptionalCompromisedCredentialsRiskConfigurationTypeOutputTypeDef = TypedDict(
-    "_OptionalCompromisedCredentialsRiskConfigurationTypeOutputTypeDef",
-    {
-        "EventFilter": List[EventFilterTypeType],
-    },
-    total=False,
-)
-
-class CompromisedCredentialsRiskConfigurationTypeOutputTypeDef(
-    _RequiredCompromisedCredentialsRiskConfigurationTypeOutputTypeDef,
-    _OptionalCompromisedCredentialsRiskConfigurationTypeOutputTypeDef,
-):
-    pass
-
 _RequiredCompromisedCredentialsRiskConfigurationTypeTypeDef = TypedDict(
     "_RequiredCompromisedCredentialsRiskConfigurationTypeTypeDef",
     {
         "Actions": CompromisedCredentialsActionsTypeTypeDef,
     },
 )
 _OptionalCompromisedCredentialsRiskConfigurationTypeTypeDef = TypedDict(
     "_OptionalCompromisedCredentialsRiskConfigurationTypeTypeDef",
     {
-        "EventFilter": Sequence[EventFilterTypeType],
+        "EventFilter": List[EventFilterTypeType],
     },
     total=False,
 )
 
 class CompromisedCredentialsRiskConfigurationTypeTypeDef(
     _RequiredCompromisedCredentialsRiskConfigurationTypeTypeDef,
     _OptionalCompromisedCredentialsRiskConfigurationTypeTypeDef,
@@ -2999,37 +2946,28 @@
     "UserPoolPolicyTypeTypeDef",
     {
         "PasswordPolicy": PasswordPolicyTypeTypeDef,
     },
     total=False,
 )
 
-RiskExceptionConfigurationTypeUnionTypeDef = Union[
-    RiskExceptionConfigurationTypeTypeDef, RiskExceptionConfigurationTypeOutputTypeDef
-]
 SchemaAttributeTypeTypeDef = TypedDict(
     "SchemaAttributeTypeTypeDef",
     {
         "Name": str,
         "AttributeDataType": AttributeDataTypeType,
         "DeveloperOnlyAttribute": bool,
         "Mutable": bool,
         "Required": bool,
         "NumberAttributeConstraints": NumberAttributeConstraintsTypeTypeDef,
         "StringAttributeConstraints": StringAttributeConstraintsTypeTypeDef,
     },
     total=False,
 )
 
-UserAttributeUpdateSettingsTypeUnionTypeDef = Union[
-    UserAttributeUpdateSettingsTypeTypeDef, UserAttributeUpdateSettingsTypeOutputTypeDef
-]
-AccountRecoverySettingTypeUnionTypeDef = Union[
-    AccountRecoverySettingTypeTypeDef, AccountRecoverySettingTypeOutputTypeDef
-]
 AdminGetDeviceResponseTypeDef = TypedDict(
     "AdminGetDeviceResponseTypeDef",
     {
         "Device": DeviceTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3135,18 +3073,14 @@
         "Session": str,
         "ChallengeParameters": Dict[str, str],
         "AuthenticationResult": AuthenticationResultTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CompromisedCredentialsRiskConfigurationTypeUnionTypeDef = Union[
-    CompromisedCredentialsRiskConfigurationTypeTypeDef,
-    CompromisedCredentialsRiskConfigurationTypeOutputTypeDef,
-]
 _RequiredAdminInitiateAuthRequestRequestTypeDef = TypedDict(
     "_RequiredAdminInitiateAuthRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "ClientId": str,
         "AuthFlow": AuthFlowTypeType,
     },
@@ -3433,30 +3367,30 @@
         "AliasAttributes": List[AliasAttributeTypeType],
         "UsernameAttributes": List[UsernameAttributeTypeType],
         "SmsVerificationMessage": str,
         "EmailVerificationMessage": str,
         "EmailVerificationSubject": str,
         "VerificationMessageTemplate": VerificationMessageTemplateTypeTypeDef,
         "SmsAuthenticationMessage": str,
-        "UserAttributeUpdateSettings": UserAttributeUpdateSettingsTypeOutputTypeDef,
+        "UserAttributeUpdateSettings": UserAttributeUpdateSettingsTypeTypeDef,
         "MfaConfiguration": UserPoolMfaTypeType,
         "DeviceConfiguration": DeviceConfigurationTypeTypeDef,
         "EstimatedNumberOfUsers": int,
         "EmailConfiguration": EmailConfigurationTypeTypeDef,
         "SmsConfiguration": SmsConfigurationTypeTypeDef,
         "UserPoolTags": Dict[str, str],
         "SmsConfigurationFailure": str,
         "EmailConfigurationFailure": str,
         "Domain": str,
         "CustomDomain": str,
         "AdminCreateUserConfig": AdminCreateUserConfigTypeTypeDef,
         "UserPoolAddOns": UserPoolAddOnsTypeTypeDef,
         "UsernameConfiguration": UsernameConfigurationTypeTypeDef,
         "Arn": str,
-        "AccountRecoverySetting": AccountRecoverySettingTypeOutputTypeDef,
+        "AccountRecoverySetting": AccountRecoverySettingTypeTypeDef,
     },
     total=False,
 )
 
 ListUserPoolsResponseTypeDef = TypedDict(
     "ListUserPoolsResponseTypeDef",
     {
@@ -3468,18 +3402,18 @@
 
 RiskConfigurationTypeTypeDef = TypedDict(
     "RiskConfigurationTypeTypeDef",
     {
         "UserPoolId": str,
         "ClientId": str,
         "CompromisedCredentialsRiskConfiguration": (
-            CompromisedCredentialsRiskConfigurationTypeOutputTypeDef
+            CompromisedCredentialsRiskConfigurationTypeTypeDef
         ),
         "AccountTakeoverRiskConfiguration": AccountTakeoverRiskConfigurationTypeTypeDef,
-        "RiskExceptionConfiguration": RiskExceptionConfigurationTypeOutputTypeDef,
+        "RiskExceptionConfiguration": RiskExceptionConfigurationTypeTypeDef,
         "LastModifiedDate": datetime,
     },
     total=False,
 )
 
 _RequiredSetRiskConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredSetRiskConfigurationRequestRequestTypeDef",
```

### Comparing `types-aiobotocore-cognito-idp-2.5.2.post1/types_aiobotocore_cognito_idp.egg-info/SOURCES.txt` & `types-aiobotocore-cognito-idp-2.5.2.post2/types_aiobotocore_cognito_idp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

