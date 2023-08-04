# Comparing `tmp/types-aiobotocore-waf-regional-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-waf-regional-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-waf-regional-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:09 2023, max compression
+gzip compressed data, was "types-aiobotocore-waf-regional-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:29 2023, max compression
```

## Comparing `types-aiobotocore-waf-regional-2.5.2.post1.tar` & `types-aiobotocore-waf-regional-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:09.309430 types-aiobotocore-waf-regional-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:50:58.000000 types-aiobotocore-waf-regional-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20810 2023-08-02 14:53:09.301430 types-aiobotocore-waf-regional-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19273 2023-08-02 14:50:58.000000 types-aiobotocore-waf-regional-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:09.309430 types-aiobotocore-waf-regional-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-08-02 14:50:57.000000 types-aiobotocore-waf-regional-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:09.301430 types-aiobotocore-waf-regional-2.5.2.post1/types_aiobotocore_waf_regional/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-08-02 14:50:58.000000 types-aiobotocore-waf-regional-2.5.2.post1/types_aiobotocore_waf_regional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-08-02 14:50:58.000000 types-aiobotocore-waf-regional-2.5.2.post1/types_aiobotocore_waf_regional/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-08-02 14:50:58.000000 types-aiobotocore-waf-regional-2.5.2.post1/types_aiobotocore_waf_regional/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49316 2023-08-02 14:50:58.000000 types-aiobotocore-waf-regional-2.5.2.post1/types_aiobotocore_waf_regional/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    49226 2023-08-02 14:50:58.000000 types-aiobotocore-waf-regional-2.5.2.post1/types_aiobotocore_waf_regional/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12123 2023-08-02 14:50:58.000000 types-aiobotocore-waf-regional-2.5.2.post1/types_aiobotocore_waf_regional/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12121 2023-08-02 14:50:58.000000 types-aiobotocore-waf-regional-2.5.2.post1/types_aiobotocore_waf_regional/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:50:58.000000 types-aiobotocore-waf-regional-2.5.2.post1/types_aiobotocore_waf_regional/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    57536 2023-08-02 14:50:59.000000 types-aiobotocore-waf-regional-2.5.2.post1/types_aiobotocore_waf_regional/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    57485 2023-08-02 14:50:59.000000 types-aiobotocore-waf-regional-2.5.2.post1/types_aiobotocore_waf_regional/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:50:58.000000 types-aiobotocore-waf-regional-2.5.2.post1/types_aiobotocore_waf_regional/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:09.301430 types-aiobotocore-waf-regional-2.5.2.post1/types_aiobotocore_waf_regional.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20810 2023-08-02 14:53:09.000000 types-aiobotocore-waf-regional-2.5.2.post1/types_aiobotocore_waf_regional.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-08-02 14:53:09.000000 types-aiobotocore-waf-regional-2.5.2.post1/types_aiobotocore_waf_regional.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:09.000000 types-aiobotocore-waf-regional-2.5.2.post1/types_aiobotocore_waf_regional.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:09.000000 types-aiobotocore-waf-regional-2.5.2.post1/types_aiobotocore_waf_regional.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:09.000000 types-aiobotocore-waf-regional-2.5.2.post1/types_aiobotocore_waf_regional.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 14:53:09.000000 types-aiobotocore-waf-regional-2.5.2.post1/types_aiobotocore_waf_regional.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:29.576643 types-aiobotocore-waf-regional-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:55:40.000000 types-aiobotocore-waf-regional-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12436 2023-08-04 13:59:29.576643 types-aiobotocore-waf-regional-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10899 2023-08-04 13:55:40.000000 types-aiobotocore-waf-regional-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:29.576643 types-aiobotocore-waf-regional-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2106 2023-08-04 13:55:39.000000 types-aiobotocore-waf-regional-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:29.576643 types-aiobotocore-waf-regional-2.5.2.post2/types_aiobotocore_waf_regional/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      477 2023-08-04 13:55:40.000000 types-aiobotocore-waf-regional-2.5.2.post2/types_aiobotocore_waf_regional/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      476 2023-08-04 13:55:40.000000 types-aiobotocore-waf-regional-2.5.2.post2/types_aiobotocore_waf_regional/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      961 2023-08-04 13:55:40.000000 types-aiobotocore-waf-regional-2.5.2.post2/types_aiobotocore_waf_regional/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    49296 2023-08-04 13:55:40.000000 types-aiobotocore-waf-regional-2.5.2.post2/types_aiobotocore_waf_regional/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    49206 2023-08-04 13:55:40.000000 types-aiobotocore-waf-regional-2.5.2.post2/types_aiobotocore_waf_regional/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12238 2023-08-04 13:55:40.000000 types-aiobotocore-waf-regional-2.5.2.post2/types_aiobotocore_waf_regional/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12236 2023-08-04 13:55:40.000000 types-aiobotocore-waf-regional-2.5.2.post2/types_aiobotocore_waf_regional/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:55:40.000000 types-aiobotocore-waf-regional-2.5.2.post2/types_aiobotocore_waf_regional/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    55412 2023-08-04 13:55:42.000000 types-aiobotocore-waf-regional-2.5.2.post2/types_aiobotocore_waf_regional/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    55365 2023-08-04 13:55:41.000000 types-aiobotocore-waf-regional-2.5.2.post2/types_aiobotocore_waf_regional/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:55:40.000000 types-aiobotocore-waf-regional-2.5.2.post2/types_aiobotocore_waf_regional/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:29.576643 types-aiobotocore-waf-regional-2.5.2.post2/types_aiobotocore_waf_regional.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12436 2023-08-04 13:59:29.000000 types-aiobotocore-waf-regional-2.5.2.post2/types_aiobotocore_waf_regional.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      819 2023-08-04 13:59:29.000000 types-aiobotocore-waf-regional-2.5.2.post2/types_aiobotocore_waf_regional.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:29.000000 types-aiobotocore-waf-regional-2.5.2.post2/types_aiobotocore_waf_regional.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:29.000000 types-aiobotocore-waf-regional-2.5.2.post2/types_aiobotocore_waf_regional.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:29.000000 types-aiobotocore-waf-regional-2.5.2.post2/types_aiobotocore_waf_regional.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       31 2023-08-04 13:59:29.000000 types-aiobotocore-waf-regional-2.5.2.post2/types_aiobotocore_waf_regional.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-waf-regional-2.5.2.post1/LICENSE` & `types-aiobotocore-waf-regional-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-waf-regional-2.5.2.post1/setup.py` & `types-aiobotocore-waf-regional-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-waf-regional",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_waf_regional"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.WAFRegional 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-waf-regional-2.5.2.post1/types_aiobotocore_waf_regional/__main__.py` & `types-aiobotocore-waf-regional-2.5.2.post2/types_aiobotocore_waf_regional/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.WAFRegional 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.WAFRegional 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf_regional//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional\nOther"
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

### Comparing `types-aiobotocore-waf-regional-2.5.2.post1/types_aiobotocore_waf_regional/client.py` & `types-aiobotocore-waf-regional-2.5.2.post2/types_aiobotocore_waf_regional/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,24 +82,24 @@
     ListRulesResponseTypeDef,
     ListSizeConstraintSetsResponseTypeDef,
     ListSqlInjectionMatchSetsResponseTypeDef,
     ListSubscribedRuleGroupsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWebACLsResponseTypeDef,
     ListXssMatchSetsResponseTypeDef,
-    LoggingConfigurationUnionTypeDef,
+    LoggingConfigurationTypeDef,
     PutLoggingConfigurationResponseTypeDef,
     RegexMatchSetUpdateTypeDef,
     RegexPatternSetUpdateTypeDef,
     RuleGroupUpdateTypeDef,
     RuleUpdateTypeDef,
     SizeConstraintSetUpdateTypeDef,
     SqlInjectionMatchSetUpdateTypeDef,
     TagTypeDef,
-    TimeWindowUnionTypeDef,
+    TimeWindowTypeDef,
     UpdateByteMatchSetResponseTypeDef,
     UpdateGeoMatchSetResponseTypeDef,
     UpdateIPSetResponseTypeDef,
     UpdateRateBasedRuleResponseTypeDef,
     UpdateRegexMatchSetResponseTypeDef,
     UpdateRegexPatternSetResponseTypeDef,
     UpdateRuleGroupResponseTypeDef,
@@ -602,15 +602,15 @@
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.get_rule_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf_regional/client/#get_rule_group)
         """
 
     async def get_sampled_requests(
-        self, *, WebAclId: str, RuleId: str, TimeWindow: TimeWindowUnionTypeDef, MaxItems: int
+        self, *, WebAclId: str, RuleId: str, TimeWindow: TimeWindowTypeDef, MaxItems: int
     ) -> GetSampledRequestsResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.get_sampled_requests)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf_regional/client/#get_sampled_requests)
         """
@@ -828,15 +828,15 @@
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.list_xss_match_sets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf_regional/client/#list_xss_match_sets)
         """
 
     async def put_logging_configuration(
-        self, *, LoggingConfiguration: LoggingConfigurationUnionTypeDef
+        self, *, LoggingConfiguration: LoggingConfigurationTypeDef
     ) -> PutLoggingConfigurationResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.put_logging_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf_regional/client/#put_logging_configuration)
         """
```

### Comparing `types-aiobotocore-waf-regional-2.5.2.post1/types_aiobotocore_waf_regional/client.pyi` & `types-aiobotocore-waf-regional-2.5.2.post2/types_aiobotocore_waf_regional/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -82,24 +82,24 @@
     ListRulesResponseTypeDef,
     ListSizeConstraintSetsResponseTypeDef,
     ListSqlInjectionMatchSetsResponseTypeDef,
     ListSubscribedRuleGroupsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWebACLsResponseTypeDef,
     ListXssMatchSetsResponseTypeDef,
-    LoggingConfigurationUnionTypeDef,
+    LoggingConfigurationTypeDef,
     PutLoggingConfigurationResponseTypeDef,
     RegexMatchSetUpdateTypeDef,
     RegexPatternSetUpdateTypeDef,
     RuleGroupUpdateTypeDef,
     RuleUpdateTypeDef,
     SizeConstraintSetUpdateTypeDef,
     SqlInjectionMatchSetUpdateTypeDef,
     TagTypeDef,
-    TimeWindowUnionTypeDef,
+    TimeWindowTypeDef,
     UpdateByteMatchSetResponseTypeDef,
     UpdateGeoMatchSetResponseTypeDef,
     UpdateIPSetResponseTypeDef,
     UpdateRateBasedRuleResponseTypeDef,
     UpdateRegexMatchSetResponseTypeDef,
     UpdateRegexPatternSetResponseTypeDef,
     UpdateRuleGroupResponseTypeDef,
@@ -552,15 +552,15 @@
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.get_rule_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf_regional/client/#get_rule_group)
         """
     async def get_sampled_requests(
-        self, *, WebAclId: str, RuleId: str, TimeWindow: TimeWindowUnionTypeDef, MaxItems: int
+        self, *, WebAclId: str, RuleId: str, TimeWindow: TimeWindowTypeDef, MaxItems: int
     ) -> GetSampledRequestsResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.get_sampled_requests)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf_regional/client/#get_sampled_requests)
         """
@@ -755,15 +755,15 @@
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.list_xss_match_sets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf_regional/client/#list_xss_match_sets)
         """
     async def put_logging_configuration(
-        self, *, LoggingConfiguration: LoggingConfigurationUnionTypeDef
+        self, *, LoggingConfiguration: LoggingConfigurationTypeDef
     ) -> PutLoggingConfigurationResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.put_logging_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf_regional/client/#put_logging_configuration)
         """
```

### Comparing `types-aiobotocore-waf-regional-2.5.2.post1/types_aiobotocore_waf_regional/literals.py` & `types-aiobotocore-waf-regional-2.5.2.post2/types_aiobotocore_waf_regional/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -333,14 +333,15 @@
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
@@ -436,14 +437,15 @@
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
@@ -522,26 +524,28 @@
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
@@ -702,14 +706,15 @@
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "il-central-1",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
```

### Comparing `types-aiobotocore-waf-regional-2.5.2.post1/types_aiobotocore_waf_regional/literals.pyi` & `types-aiobotocore-waf-regional-2.5.2.post2/types_aiobotocore_waf_regional/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -331,14 +331,15 @@
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
@@ -434,14 +435,15 @@
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
@@ -520,26 +522,28 @@
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
@@ -700,14 +704,15 @@
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "il-central-1",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
```

### Comparing `types-aiobotocore-waf-regional-2.5.2.post1/types_aiobotocore_waf_regional/type_defs.py` & `types-aiobotocore-waf-regional-2.5.2.post2/types_aiobotocore_waf_regional/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,15 @@
     from types_aiobotocore_waf_regional.type_defs import ExcludedRuleTypeDef
 
     data: ExcludedRuleTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import IO, Any, Dict, List, Sequence, Union
-
-from aiobotocore.response import StreamingBody
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     ChangeActionType,
     ChangeTokenStatusType,
     ComparisonOperatorType,
     GeoMatchConstraintValueType,
     IPSetDescriptorTypeType,
@@ -44,15 +42,14 @@
 
 
 __all__ = (
     "ExcludedRuleTypeDef",
     "WafActionTypeDef",
     "WafOverrideActionTypeDef",
     "AssociateWebACLRequestRequestTypeDef",
-    "BlobTypeDef",
     "ByteMatchSetSummaryTypeDef",
     "FieldToMatchTypeDef",
     "CreateByteMatchSetRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CreateGeoMatchSetRequestRequestTypeDef",
     "CreateIPSetRequestRequestTypeDef",
     "TagTypeDef",
@@ -89,15 +86,14 @@
     "GetPermissionPolicyRequestRequestTypeDef",
     "GetRateBasedRuleManagedKeysRequestRequestTypeDef",
     "GetRateBasedRuleRequestRequestTypeDef",
     "GetRegexMatchSetRequestRequestTypeDef",
     "GetRegexPatternSetRequestRequestTypeDef",
     "GetRuleGroupRequestRequestTypeDef",
     "GetRuleRequestRequestTypeDef",
-    "TimeWindowOutputTypeDef",
     "GetSizeConstraintSetRequestRequestTypeDef",
     "GetSqlInjectionMatchSetRequestRequestTypeDef",
     "GetWebACLForResourceRequestRequestTypeDef",
     "WebACLSummaryTypeDef",
     "GetWebACLRequestRequestTypeDef",
     "GetXssMatchSetRequestRequestTypeDef",
     "HTTPHeaderTypeDef",
@@ -129,19 +125,16 @@
     "ListXssMatchSetsRequestRequestTypeDef",
     "XssMatchSetSummaryTypeDef",
     "PredicateTypeDef",
     "PutPermissionPolicyRequestRequestTypeDef",
     "RegexPatternSetUpdateTypeDef",
     "TimestampTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "ActivatedRuleOutputTypeDef",
     "ActivatedRuleTypeDef",
-    "ByteMatchTupleOutputTypeDef",
     "ByteMatchTupleTypeDef",
-    "LoggingConfigurationOutputTypeDef",
     "LoggingConfigurationTypeDef",
     "RegexMatchTupleTypeDef",
     "SizeConstraintTypeDef",
     "SqlInjectionMatchTupleTypeDef",
     "XssMatchTupleTypeDef",
     "CreateWebACLMigrationStackResponseTypeDef",
     "DeleteByteMatchSetResponseTypeDef",
@@ -204,24 +197,23 @@
     "ListXssMatchSetsResponseTypeDef",
     "RateBasedRuleTypeDef",
     "RuleTypeDef",
     "RuleUpdateTypeDef",
     "UpdateRegexPatternSetRequestRequestTypeDef",
     "TimeWindowTypeDef",
     "ListActivatedRulesInRuleGroupResponseTypeDef",
-    "WebACLTypeDef",
     "RuleGroupUpdateTypeDef",
+    "WebACLTypeDef",
     "WebACLUpdateTypeDef",
     "ByteMatchSetTypeDef",
     "ByteMatchSetUpdateTypeDef",
     "GetLoggingConfigurationResponseTypeDef",
     "ListLoggingConfigurationsResponseTypeDef",
-    "PutLoggingConfigurationResponseTypeDef",
-    "LoggingConfigurationUnionTypeDef",
     "PutLoggingConfigurationRequestRequestTypeDef",
+    "PutLoggingConfigurationResponseTypeDef",
     "RegexMatchSetTypeDef",
     "RegexMatchSetUpdateTypeDef",
     "SizeConstraintSetTypeDef",
     "SizeConstraintSetUpdateTypeDef",
     "SqlInjectionMatchSetTypeDef",
     "SqlInjectionMatchSetUpdateTypeDef",
     "XssMatchSetTypeDef",
@@ -237,18 +229,17 @@
     "CreateRateBasedRuleResponseTypeDef",
     "GetRateBasedRuleResponseTypeDef",
     "CreateRuleResponseTypeDef",
     "GetRuleResponseTypeDef",
     "UpdateRateBasedRuleRequestRequestTypeDef",
     "UpdateRuleRequestRequestTypeDef",
     "GetSampledRequestsRequestRequestTypeDef",
-    "TimeWindowUnionTypeDef",
+    "UpdateRuleGroupRequestRequestTypeDef",
     "CreateWebACLResponseTypeDef",
     "GetWebACLResponseTypeDef",
-    "UpdateRuleGroupRequestRequestTypeDef",
     "UpdateWebACLRequestRequestTypeDef",
     "CreateByteMatchSetResponseTypeDef",
     "GetByteMatchSetResponseTypeDef",
     "UpdateByteMatchSetRequestRequestTypeDef",
     "CreateRegexMatchSetResponseTypeDef",
     "GetRegexMatchSetResponseTypeDef",
     "UpdateRegexMatchSetRequestRequestTypeDef",
@@ -289,15 +280,14 @@
     "AssociateWebACLRequestRequestTypeDef",
     {
         "WebACLId": str,
         "ResourceArn": str,
     },
 )
 
-BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 ByteMatchSetSummaryTypeDef = TypedDict(
     "ByteMatchSetSummaryTypeDef",
     {
         "ByteMatchSetId": str,
         "Name": str,
     },
 )
@@ -681,22 +671,14 @@
 GetRuleRequestRequestTypeDef = TypedDict(
     "GetRuleRequestRequestTypeDef",
     {
         "RuleId": str,
     },
 )
 
-TimeWindowOutputTypeDef = TypedDict(
-    "TimeWindowOutputTypeDef",
-    {
-        "StartTime": datetime,
-        "EndTime": datetime,
-    },
-)
-
 GetSizeConstraintSetRequestRequestTypeDef = TypedDict(
     "GetSizeConstraintSetRequestRequestTypeDef",
     {
         "SizeConstraintSetId": str,
     },
 )
 
@@ -1037,115 +1019,58 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
 
-_RequiredActivatedRuleOutputTypeDef = TypedDict(
-    "_RequiredActivatedRuleOutputTypeDef",
-    {
-        "Priority": int,
-        "RuleId": str,
-    },
-)
-_OptionalActivatedRuleOutputTypeDef = TypedDict(
-    "_OptionalActivatedRuleOutputTypeDef",
-    {
-        "Action": WafActionTypeDef,
-        "OverrideAction": WafOverrideActionTypeDef,
-        "Type": WafRuleTypeType,
-        "ExcludedRules": List[ExcludedRuleTypeDef],
-    },
-    total=False,
-)
-
-
-class ActivatedRuleOutputTypeDef(
-    _RequiredActivatedRuleOutputTypeDef, _OptionalActivatedRuleOutputTypeDef
-):
-    pass
-
-
 _RequiredActivatedRuleTypeDef = TypedDict(
     "_RequiredActivatedRuleTypeDef",
     {
         "Priority": int,
         "RuleId": str,
     },
 )
 _OptionalActivatedRuleTypeDef = TypedDict(
     "_OptionalActivatedRuleTypeDef",
     {
         "Action": WafActionTypeDef,
         "OverrideAction": WafOverrideActionTypeDef,
         "Type": WafRuleTypeType,
-        "ExcludedRules": Sequence[ExcludedRuleTypeDef],
+        "ExcludedRules": List[ExcludedRuleTypeDef],
     },
     total=False,
 )
 
 
 class ActivatedRuleTypeDef(_RequiredActivatedRuleTypeDef, _OptionalActivatedRuleTypeDef):
     pass
 
 
-ByteMatchTupleOutputTypeDef = TypedDict(
-    "ByteMatchTupleOutputTypeDef",
-    {
-        "FieldToMatch": FieldToMatchTypeDef,
-        "TargetString": bytes,
-        "TextTransformation": TextTransformationType,
-        "PositionalConstraint": PositionalConstraintType,
-    },
-)
-
 ByteMatchTupleTypeDef = TypedDict(
     "ByteMatchTupleTypeDef",
     {
         "FieldToMatch": FieldToMatchTypeDef,
-        "TargetString": BlobTypeDef,
+        "TargetString": bytes,
         "TextTransformation": TextTransformationType,
         "PositionalConstraint": PositionalConstraintType,
     },
 )
 
-_RequiredLoggingConfigurationOutputTypeDef = TypedDict(
-    "_RequiredLoggingConfigurationOutputTypeDef",
-    {
-        "ResourceArn": str,
-        "LogDestinationConfigs": List[str],
-    },
-)
-_OptionalLoggingConfigurationOutputTypeDef = TypedDict(
-    "_OptionalLoggingConfigurationOutputTypeDef",
-    {
-        "RedactedFields": List[FieldToMatchTypeDef],
-    },
-    total=False,
-)
-
-
-class LoggingConfigurationOutputTypeDef(
-    _RequiredLoggingConfigurationOutputTypeDef, _OptionalLoggingConfigurationOutputTypeDef
-):
-    pass
-
-
 _RequiredLoggingConfigurationTypeDef = TypedDict(
     "_RequiredLoggingConfigurationTypeDef",
     {
         "ResourceArn": str,
-        "LogDestinationConfigs": Sequence[str],
+        "LogDestinationConfigs": List[str],
     },
 )
 _OptionalLoggingConfigurationTypeDef = TypedDict(
     "_OptionalLoggingConfigurationTypeDef",
     {
-        "RedactedFields": Sequence[FieldToMatchTypeDef],
+        "RedactedFields": List[FieldToMatchTypeDef],
     },
     total=False,
 )
 
 
 class LoggingConfigurationTypeDef(
     _RequiredLoggingConfigurationTypeDef, _OptionalLoggingConfigurationTypeDef
@@ -1839,25 +1764,33 @@
     },
 )
 
 ListActivatedRulesInRuleGroupResponseTypeDef = TypedDict(
     "ListActivatedRulesInRuleGroupResponseTypeDef",
     {
         "NextMarker": str,
-        "ActivatedRules": List[ActivatedRuleOutputTypeDef],
+        "ActivatedRules": List[ActivatedRuleTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+RuleGroupUpdateTypeDef = TypedDict(
+    "RuleGroupUpdateTypeDef",
+    {
+        "Action": ChangeActionType,
+        "ActivatedRule": ActivatedRuleTypeDef,
+    },
+)
+
 _RequiredWebACLTypeDef = TypedDict(
     "_RequiredWebACLTypeDef",
     {
         "WebACLId": str,
         "DefaultAction": WafActionTypeDef,
-        "Rules": List[ActivatedRuleOutputTypeDef],
+        "Rules": List[ActivatedRuleTypeDef],
     },
 )
 _OptionalWebACLTypeDef = TypedDict(
     "_OptionalWebACLTypeDef",
     {
         "Name": str,
         "MetricName": str,
@@ -1867,35 +1800,27 @@
 )
 
 
 class WebACLTypeDef(_RequiredWebACLTypeDef, _OptionalWebACLTypeDef):
     pass
 
 
-RuleGroupUpdateTypeDef = TypedDict(
-    "RuleGroupUpdateTypeDef",
-    {
-        "Action": ChangeActionType,
-        "ActivatedRule": ActivatedRuleTypeDef,
-    },
-)
-
 WebACLUpdateTypeDef = TypedDict(
     "WebACLUpdateTypeDef",
     {
         "Action": ChangeActionType,
         "ActivatedRule": ActivatedRuleTypeDef,
     },
 )
 
 _RequiredByteMatchSetTypeDef = TypedDict(
     "_RequiredByteMatchSetTypeDef",
     {
         "ByteMatchSetId": str,
-        "ByteMatchTuples": List[ByteMatchTupleOutputTypeDef],
+        "ByteMatchTuples": List[ByteMatchTupleTypeDef],
     },
 )
 _OptionalByteMatchSetTypeDef = TypedDict(
     "_OptionalByteMatchSetTypeDef",
     {
         "Name": str,
     },
@@ -1914,43 +1839,40 @@
         "ByteMatchTuple": ByteMatchTupleTypeDef,
     },
 )
 
 GetLoggingConfigurationResponseTypeDef = TypedDict(
     "GetLoggingConfigurationResponseTypeDef",
     {
-        "LoggingConfiguration": LoggingConfigurationOutputTypeDef,
+        "LoggingConfiguration": LoggingConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLoggingConfigurationsResponseTypeDef = TypedDict(
     "ListLoggingConfigurationsResponseTypeDef",
     {
-        "LoggingConfigurations": List[LoggingConfigurationOutputTypeDef],
+        "LoggingConfigurations": List[LoggingConfigurationTypeDef],
         "NextMarker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutLoggingConfigurationResponseTypeDef = TypedDict(
-    "PutLoggingConfigurationResponseTypeDef",
+PutLoggingConfigurationRequestRequestTypeDef = TypedDict(
+    "PutLoggingConfigurationRequestRequestTypeDef",
     {
-        "LoggingConfiguration": LoggingConfigurationOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "LoggingConfiguration": LoggingConfigurationTypeDef,
     },
 )
 
-LoggingConfigurationUnionTypeDef = Union[
-    LoggingConfigurationTypeDef, LoggingConfigurationOutputTypeDef
-]
-PutLoggingConfigurationRequestRequestTypeDef = TypedDict(
-    "PutLoggingConfigurationRequestRequestTypeDef",
+PutLoggingConfigurationResponseTypeDef = TypedDict(
+    "PutLoggingConfigurationResponseTypeDef",
     {
         "LoggingConfiguration": LoggingConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RegexMatchSetTypeDef = TypedDict(
     "RegexMatchSetTypeDef",
     {
         "RegexMatchSetId": str,
@@ -2200,15 +2122,23 @@
         "WebAclId": str,
         "RuleId": str,
         "TimeWindow": TimeWindowTypeDef,
         "MaxItems": int,
     },
 )
 
-TimeWindowUnionTypeDef = Union[TimeWindowTypeDef, TimeWindowOutputTypeDef]
+UpdateRuleGroupRequestRequestTypeDef = TypedDict(
+    "UpdateRuleGroupRequestRequestTypeDef",
+    {
+        "RuleGroupId": str,
+        "Updates": Sequence[RuleGroupUpdateTypeDef],
+        "ChangeToken": str,
+    },
+)
+
 CreateWebACLResponseTypeDef = TypedDict(
     "CreateWebACLResponseTypeDef",
     {
         "WebACL": WebACLTypeDef,
         "ChangeToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2218,23 +2148,14 @@
     "GetWebACLResponseTypeDef",
     {
         "WebACL": WebACLTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateRuleGroupRequestRequestTypeDef = TypedDict(
-    "UpdateRuleGroupRequestRequestTypeDef",
-    {
-        "RuleGroupId": str,
-        "Updates": Sequence[RuleGroupUpdateTypeDef],
-        "ChangeToken": str,
-    },
-)
-
 _RequiredUpdateWebACLRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWebACLRequestRequestTypeDef",
     {
         "WebACLId": str,
         "ChangeToken": str,
     },
 )
@@ -2385,11 +2306,11 @@
 )
 
 GetSampledRequestsResponseTypeDef = TypedDict(
     "GetSampledRequestsResponseTypeDef",
     {
         "SampledRequests": List[SampledHTTPRequestTypeDef],
         "PopulationSize": int,
-        "TimeWindow": TimeWindowOutputTypeDef,
+        "TimeWindow": TimeWindowTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-waf-regional-2.5.2.post1/types_aiobotocore_waf_regional/type_defs.pyi` & `types-aiobotocore-waf-regional-2.5.2.post2/types_aiobotocore_waf_regional/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,15 @@
     from types_aiobotocore_waf_regional.type_defs import ExcludedRuleTypeDef
 
     data: ExcludedRuleTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import IO, Any, Dict, List, Sequence, Union
-
-from aiobotocore.response import StreamingBody
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     ChangeActionType,
     ChangeTokenStatusType,
     ComparisonOperatorType,
     GeoMatchConstraintValueType,
     IPSetDescriptorTypeType,
@@ -43,15 +41,14 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "ExcludedRuleTypeDef",
     "WafActionTypeDef",
     "WafOverrideActionTypeDef",
     "AssociateWebACLRequestRequestTypeDef",
-    "BlobTypeDef",
     "ByteMatchSetSummaryTypeDef",
     "FieldToMatchTypeDef",
     "CreateByteMatchSetRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CreateGeoMatchSetRequestRequestTypeDef",
     "CreateIPSetRequestRequestTypeDef",
     "TagTypeDef",
@@ -88,15 +85,14 @@
     "GetPermissionPolicyRequestRequestTypeDef",
     "GetRateBasedRuleManagedKeysRequestRequestTypeDef",
     "GetRateBasedRuleRequestRequestTypeDef",
     "GetRegexMatchSetRequestRequestTypeDef",
     "GetRegexPatternSetRequestRequestTypeDef",
     "GetRuleGroupRequestRequestTypeDef",
     "GetRuleRequestRequestTypeDef",
-    "TimeWindowOutputTypeDef",
     "GetSizeConstraintSetRequestRequestTypeDef",
     "GetSqlInjectionMatchSetRequestRequestTypeDef",
     "GetWebACLForResourceRequestRequestTypeDef",
     "WebACLSummaryTypeDef",
     "GetWebACLRequestRequestTypeDef",
     "GetXssMatchSetRequestRequestTypeDef",
     "HTTPHeaderTypeDef",
@@ -128,19 +124,16 @@
     "ListXssMatchSetsRequestRequestTypeDef",
     "XssMatchSetSummaryTypeDef",
     "PredicateTypeDef",
     "PutPermissionPolicyRequestRequestTypeDef",
     "RegexPatternSetUpdateTypeDef",
     "TimestampTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "ActivatedRuleOutputTypeDef",
     "ActivatedRuleTypeDef",
-    "ByteMatchTupleOutputTypeDef",
     "ByteMatchTupleTypeDef",
-    "LoggingConfigurationOutputTypeDef",
     "LoggingConfigurationTypeDef",
     "RegexMatchTupleTypeDef",
     "SizeConstraintTypeDef",
     "SqlInjectionMatchTupleTypeDef",
     "XssMatchTupleTypeDef",
     "CreateWebACLMigrationStackResponseTypeDef",
     "DeleteByteMatchSetResponseTypeDef",
@@ -203,24 +196,23 @@
     "ListXssMatchSetsResponseTypeDef",
     "RateBasedRuleTypeDef",
     "RuleTypeDef",
     "RuleUpdateTypeDef",
     "UpdateRegexPatternSetRequestRequestTypeDef",
     "TimeWindowTypeDef",
     "ListActivatedRulesInRuleGroupResponseTypeDef",
-    "WebACLTypeDef",
     "RuleGroupUpdateTypeDef",
+    "WebACLTypeDef",
     "WebACLUpdateTypeDef",
     "ByteMatchSetTypeDef",
     "ByteMatchSetUpdateTypeDef",
     "GetLoggingConfigurationResponseTypeDef",
     "ListLoggingConfigurationsResponseTypeDef",
-    "PutLoggingConfigurationResponseTypeDef",
-    "LoggingConfigurationUnionTypeDef",
     "PutLoggingConfigurationRequestRequestTypeDef",
+    "PutLoggingConfigurationResponseTypeDef",
     "RegexMatchSetTypeDef",
     "RegexMatchSetUpdateTypeDef",
     "SizeConstraintSetTypeDef",
     "SizeConstraintSetUpdateTypeDef",
     "SqlInjectionMatchSetTypeDef",
     "SqlInjectionMatchSetUpdateTypeDef",
     "XssMatchSetTypeDef",
@@ -236,18 +228,17 @@
     "CreateRateBasedRuleResponseTypeDef",
     "GetRateBasedRuleResponseTypeDef",
     "CreateRuleResponseTypeDef",
     "GetRuleResponseTypeDef",
     "UpdateRateBasedRuleRequestRequestTypeDef",
     "UpdateRuleRequestRequestTypeDef",
     "GetSampledRequestsRequestRequestTypeDef",
-    "TimeWindowUnionTypeDef",
+    "UpdateRuleGroupRequestRequestTypeDef",
     "CreateWebACLResponseTypeDef",
     "GetWebACLResponseTypeDef",
-    "UpdateRuleGroupRequestRequestTypeDef",
     "UpdateWebACLRequestRequestTypeDef",
     "CreateByteMatchSetResponseTypeDef",
     "GetByteMatchSetResponseTypeDef",
     "UpdateByteMatchSetRequestRequestTypeDef",
     "CreateRegexMatchSetResponseTypeDef",
     "GetRegexMatchSetResponseTypeDef",
     "UpdateRegexMatchSetRequestRequestTypeDef",
@@ -288,15 +279,14 @@
     "AssociateWebACLRequestRequestTypeDef",
     {
         "WebACLId": str,
         "ResourceArn": str,
     },
 )
 
-BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 ByteMatchSetSummaryTypeDef = TypedDict(
     "ByteMatchSetSummaryTypeDef",
     {
         "ByteMatchSetId": str,
         "Name": str,
     },
 )
@@ -672,22 +662,14 @@
 GetRuleRequestRequestTypeDef = TypedDict(
     "GetRuleRequestRequestTypeDef",
     {
         "RuleId": str,
     },
 )
 
-TimeWindowOutputTypeDef = TypedDict(
-    "TimeWindowOutputTypeDef",
-    {
-        "StartTime": datetime,
-        "EndTime": datetime,
-    },
-)
-
 GetSizeConstraintSetRequestRequestTypeDef = TypedDict(
     "GetSizeConstraintSetRequestRequestTypeDef",
     {
         "SizeConstraintSetId": str,
     },
 )
 
@@ -1024,109 +1006,56 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
 
-_RequiredActivatedRuleOutputTypeDef = TypedDict(
-    "_RequiredActivatedRuleOutputTypeDef",
-    {
-        "Priority": int,
-        "RuleId": str,
-    },
-)
-_OptionalActivatedRuleOutputTypeDef = TypedDict(
-    "_OptionalActivatedRuleOutputTypeDef",
-    {
-        "Action": WafActionTypeDef,
-        "OverrideAction": WafOverrideActionTypeDef,
-        "Type": WafRuleTypeType,
-        "ExcludedRules": List[ExcludedRuleTypeDef],
-    },
-    total=False,
-)
-
-class ActivatedRuleOutputTypeDef(
-    _RequiredActivatedRuleOutputTypeDef, _OptionalActivatedRuleOutputTypeDef
-):
-    pass
-
 _RequiredActivatedRuleTypeDef = TypedDict(
     "_RequiredActivatedRuleTypeDef",
     {
         "Priority": int,
         "RuleId": str,
     },
 )
 _OptionalActivatedRuleTypeDef = TypedDict(
     "_OptionalActivatedRuleTypeDef",
     {
         "Action": WafActionTypeDef,
         "OverrideAction": WafOverrideActionTypeDef,
         "Type": WafRuleTypeType,
-        "ExcludedRules": Sequence[ExcludedRuleTypeDef],
+        "ExcludedRules": List[ExcludedRuleTypeDef],
     },
     total=False,
 )
 
 class ActivatedRuleTypeDef(_RequiredActivatedRuleTypeDef, _OptionalActivatedRuleTypeDef):
     pass
 
-ByteMatchTupleOutputTypeDef = TypedDict(
-    "ByteMatchTupleOutputTypeDef",
-    {
-        "FieldToMatch": FieldToMatchTypeDef,
-        "TargetString": bytes,
-        "TextTransformation": TextTransformationType,
-        "PositionalConstraint": PositionalConstraintType,
-    },
-)
-
 ByteMatchTupleTypeDef = TypedDict(
     "ByteMatchTupleTypeDef",
     {
         "FieldToMatch": FieldToMatchTypeDef,
-        "TargetString": BlobTypeDef,
+        "TargetString": bytes,
         "TextTransformation": TextTransformationType,
         "PositionalConstraint": PositionalConstraintType,
     },
 )
 
-_RequiredLoggingConfigurationOutputTypeDef = TypedDict(
-    "_RequiredLoggingConfigurationOutputTypeDef",
-    {
-        "ResourceArn": str,
-        "LogDestinationConfigs": List[str],
-    },
-)
-_OptionalLoggingConfigurationOutputTypeDef = TypedDict(
-    "_OptionalLoggingConfigurationOutputTypeDef",
-    {
-        "RedactedFields": List[FieldToMatchTypeDef],
-    },
-    total=False,
-)
-
-class LoggingConfigurationOutputTypeDef(
-    _RequiredLoggingConfigurationOutputTypeDef, _OptionalLoggingConfigurationOutputTypeDef
-):
-    pass
-
 _RequiredLoggingConfigurationTypeDef = TypedDict(
     "_RequiredLoggingConfigurationTypeDef",
     {
         "ResourceArn": str,
-        "LogDestinationConfigs": Sequence[str],
+        "LogDestinationConfigs": List[str],
     },
 )
 _OptionalLoggingConfigurationTypeDef = TypedDict(
     "_OptionalLoggingConfigurationTypeDef",
     {
-        "RedactedFields": Sequence[FieldToMatchTypeDef],
+        "RedactedFields": List[FieldToMatchTypeDef],
     },
     total=False,
 )
 
 class LoggingConfigurationTypeDef(
     _RequiredLoggingConfigurationTypeDef, _OptionalLoggingConfigurationTypeDef
 ):
@@ -1802,25 +1731,33 @@
     },
 )
 
 ListActivatedRulesInRuleGroupResponseTypeDef = TypedDict(
     "ListActivatedRulesInRuleGroupResponseTypeDef",
     {
         "NextMarker": str,
-        "ActivatedRules": List[ActivatedRuleOutputTypeDef],
+        "ActivatedRules": List[ActivatedRuleTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+RuleGroupUpdateTypeDef = TypedDict(
+    "RuleGroupUpdateTypeDef",
+    {
+        "Action": ChangeActionType,
+        "ActivatedRule": ActivatedRuleTypeDef,
+    },
+)
+
 _RequiredWebACLTypeDef = TypedDict(
     "_RequiredWebACLTypeDef",
     {
         "WebACLId": str,
         "DefaultAction": WafActionTypeDef,
-        "Rules": List[ActivatedRuleOutputTypeDef],
+        "Rules": List[ActivatedRuleTypeDef],
     },
 )
 _OptionalWebACLTypeDef = TypedDict(
     "_OptionalWebACLTypeDef",
     {
         "Name": str,
         "MetricName": str,
@@ -1828,35 +1765,27 @@
     },
     total=False,
 )
 
 class WebACLTypeDef(_RequiredWebACLTypeDef, _OptionalWebACLTypeDef):
     pass
 
-RuleGroupUpdateTypeDef = TypedDict(
-    "RuleGroupUpdateTypeDef",
-    {
-        "Action": ChangeActionType,
-        "ActivatedRule": ActivatedRuleTypeDef,
-    },
-)
-
 WebACLUpdateTypeDef = TypedDict(
     "WebACLUpdateTypeDef",
     {
         "Action": ChangeActionType,
         "ActivatedRule": ActivatedRuleTypeDef,
     },
 )
 
 _RequiredByteMatchSetTypeDef = TypedDict(
     "_RequiredByteMatchSetTypeDef",
     {
         "ByteMatchSetId": str,
-        "ByteMatchTuples": List[ByteMatchTupleOutputTypeDef],
+        "ByteMatchTuples": List[ByteMatchTupleTypeDef],
     },
 )
 _OptionalByteMatchSetTypeDef = TypedDict(
     "_OptionalByteMatchSetTypeDef",
     {
         "Name": str,
     },
@@ -1873,43 +1802,40 @@
         "ByteMatchTuple": ByteMatchTupleTypeDef,
     },
 )
 
 GetLoggingConfigurationResponseTypeDef = TypedDict(
     "GetLoggingConfigurationResponseTypeDef",
     {
-        "LoggingConfiguration": LoggingConfigurationOutputTypeDef,
+        "LoggingConfiguration": LoggingConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLoggingConfigurationsResponseTypeDef = TypedDict(
     "ListLoggingConfigurationsResponseTypeDef",
     {
-        "LoggingConfigurations": List[LoggingConfigurationOutputTypeDef],
+        "LoggingConfigurations": List[LoggingConfigurationTypeDef],
         "NextMarker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutLoggingConfigurationResponseTypeDef = TypedDict(
-    "PutLoggingConfigurationResponseTypeDef",
+PutLoggingConfigurationRequestRequestTypeDef = TypedDict(
+    "PutLoggingConfigurationRequestRequestTypeDef",
     {
-        "LoggingConfiguration": LoggingConfigurationOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "LoggingConfiguration": LoggingConfigurationTypeDef,
     },
 )
 
-LoggingConfigurationUnionTypeDef = Union[
-    LoggingConfigurationTypeDef, LoggingConfigurationOutputTypeDef
-]
-PutLoggingConfigurationRequestRequestTypeDef = TypedDict(
-    "PutLoggingConfigurationRequestRequestTypeDef",
+PutLoggingConfigurationResponseTypeDef = TypedDict(
+    "PutLoggingConfigurationResponseTypeDef",
     {
         "LoggingConfiguration": LoggingConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RegexMatchSetTypeDef = TypedDict(
     "RegexMatchSetTypeDef",
     {
         "RegexMatchSetId": str,
@@ -2151,15 +2077,23 @@
         "WebAclId": str,
         "RuleId": str,
         "TimeWindow": TimeWindowTypeDef,
         "MaxItems": int,
     },
 )
 
-TimeWindowUnionTypeDef = Union[TimeWindowTypeDef, TimeWindowOutputTypeDef]
+UpdateRuleGroupRequestRequestTypeDef = TypedDict(
+    "UpdateRuleGroupRequestRequestTypeDef",
+    {
+        "RuleGroupId": str,
+        "Updates": Sequence[RuleGroupUpdateTypeDef],
+        "ChangeToken": str,
+    },
+)
+
 CreateWebACLResponseTypeDef = TypedDict(
     "CreateWebACLResponseTypeDef",
     {
         "WebACL": WebACLTypeDef,
         "ChangeToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2169,23 +2103,14 @@
     "GetWebACLResponseTypeDef",
     {
         "WebACL": WebACLTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateRuleGroupRequestRequestTypeDef = TypedDict(
-    "UpdateRuleGroupRequestRequestTypeDef",
-    {
-        "RuleGroupId": str,
-        "Updates": Sequence[RuleGroupUpdateTypeDef],
-        "ChangeToken": str,
-    },
-)
-
 _RequiredUpdateWebACLRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWebACLRequestRequestTypeDef",
     {
         "WebACLId": str,
         "ChangeToken": str,
     },
 )
@@ -2334,11 +2259,11 @@
 )
 
 GetSampledRequestsResponseTypeDef = TypedDict(
     "GetSampledRequestsResponseTypeDef",
     {
         "SampledRequests": List[SampledHTTPRequestTypeDef],
         "PopulationSize": int,
-        "TimeWindow": TimeWindowOutputTypeDef,
+        "TimeWindow": TimeWindowTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-waf-regional-2.5.2.post1/types_aiobotocore_waf_regional.egg-info/SOURCES.txt` & `types-aiobotocore-waf-regional-2.5.2.post2/types_aiobotocore_waf_regional.egg-info/SOURCES.txt`

 * *Files identical despite different names*

