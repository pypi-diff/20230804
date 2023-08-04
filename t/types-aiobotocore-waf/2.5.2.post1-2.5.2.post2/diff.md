# Comparing `tmp/types-aiobotocore-waf-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-waf-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-waf-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:09 2023, max compression
+gzip compressed data, was "types-aiobotocore-waf-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:29 2023, max compression
```

## Comparing `types-aiobotocore-waf-2.5.2.post1.tar` & `types-aiobotocore-waf-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:09.233430 types-aiobotocore-waf-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:50:55.000000 types-aiobotocore-waf-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    24895 2023-08-02 14:53:09.233430 types-aiobotocore-waf-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23393 2023-08-02 14:50:55.000000 types-aiobotocore-waf-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:09.233430 types-aiobotocore-waf-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-02 14:50:55.000000 types-aiobotocore-waf-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:09.233430 types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf/
--rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-08-02 14:50:55.000000 types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-08-02 14:50:55.000000 types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-02 14:50:55.000000 types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52680 2023-08-02 14:50:55.000000 types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    52578 2023-08-02 14:50:55.000000 types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13679 2023-08-02 14:50:55.000000 types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13677 2023-08-02 14:50:55.000000 types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18479 2023-08-02 14:50:55.000000 types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    18461 2023-08-02 14:50:55.000000 types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:50:55.000000 types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    61264 2023-08-02 14:50:57.000000 types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    61213 2023-08-02 14:50:56.000000 types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:50:55.000000 types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:09.233430 types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24895 2023-08-02 14:53:09.000000 types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-02 14:53:09.000000 types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:09.000000 types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:09.000000 types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:09.000000 types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 14:53:09.000000 types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:29.566643 types-aiobotocore-waf-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:55:35.000000 types-aiobotocore-waf-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    15098 2023-08-04 13:59:29.566643 types-aiobotocore-waf-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13596 2023-08-04 13:55:35.000000 types-aiobotocore-waf-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:29.576643 types-aiobotocore-waf-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2020 2023-08-04 13:55:35.000000 types-aiobotocore-waf-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:29.566643 types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     4013 2023-08-04 13:55:35.000000 types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     4012 2023-08-04 13:55:35.000000 types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      916 2023-08-04 13:55:35.000000 types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    52660 2023-08-04 13:55:36.000000 types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    52558 2023-08-04 13:55:35.000000 types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13774 2023-08-04 13:55:36.000000 types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13772 2023-08-04 13:55:36.000000 types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    18479 2023-08-04 13:55:36.000000 types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    18461 2023-08-04 13:55:36.000000 types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:55:35.000000 types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    59140 2023-08-04 13:55:38.000000 types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    59093 2023-08-04 13:55:37.000000 types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:55:35.000000 types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:29.566643 types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    15098 2023-08-04 13:59:29.000000 types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      737 2023-08-04 13:59:29.000000 types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:29.000000 types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:29.000000 types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:29.000000 types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       22 2023-08-04 13:59:29.000000 types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-waf-2.5.2.post1/LICENSE` & `types-aiobotocore-waf-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-waf-2.5.2.post1/setup.py` & `types-aiobotocore-waf-2.5.2.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-waf",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_waf"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.WAF 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf/__init__.py` & `types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf/__init__.pyi` & `types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf/__main__.py` & `types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.WAF 2.5.2\nVersion:         2.5.2.post1\nBuilder version:"
-        " 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.WAF 2.5.2\nVersion:         2.5.2.post2\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF\nOther"
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

### Comparing `types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf/client.py` & `types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,24 +97,24 @@
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
@@ -600,15 +600,15 @@
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.get_rule_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/client/#get_rule_group)
         """
 
     async def get_sampled_requests(
-        self, *, WebAclId: str, RuleId: str, TimeWindow: TimeWindowUnionTypeDef, MaxItems: int
+        self, *, WebAclId: str, RuleId: str, TimeWindow: TimeWindowTypeDef, MaxItems: int
     ) -> GetSampledRequestsResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.get_sampled_requests)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/client/#get_sampled_requests)
         """
@@ -806,15 +806,15 @@
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.list_xss_match_sets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/client/#list_xss_match_sets)
         """
 
     async def put_logging_configuration(
-        self, *, LoggingConfiguration: LoggingConfigurationUnionTypeDef
+        self, *, LoggingConfiguration: LoggingConfigurationTypeDef
     ) -> PutLoggingConfigurationResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.put_logging_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/client/#put_logging_configuration)
         """
```

### Comparing `types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf/client.pyi` & `types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -97,24 +97,24 @@
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.get_rule_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/client/#get_rule_group)
         """
     async def get_sampled_requests(
-        self, *, WebAclId: str, RuleId: str, TimeWindow: TimeWindowUnionTypeDef, MaxItems: int
+        self, *, WebAclId: str, RuleId: str, TimeWindow: TimeWindowTypeDef, MaxItems: int
     ) -> GetSampledRequestsResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.get_sampled_requests)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/client/#get_sampled_requests)
         """
@@ -737,15 +737,15 @@
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.list_xss_match_sets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/client/#list_xss_match_sets)
         """
     async def put_logging_configuration(
-        self, *, LoggingConfiguration: LoggingConfigurationUnionTypeDef
+        self, *, LoggingConfiguration: LoggingConfigurationTypeDef
     ) -> PutLoggingConfigurationResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.put_logging_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/client/#put_logging_configuration)
         """
```

### Comparing `types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf/literals.py` & `types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -363,14 +363,15 @@
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
@@ -466,14 +467,15 @@
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
@@ -552,26 +554,28 @@
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

### Comparing `types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf/literals.pyi` & `types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -361,14 +361,15 @@
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
@@ -464,14 +465,15 @@
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
@@ -550,26 +552,28 @@
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

### Comparing `types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf/paginator.py` & `types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf/paginator.pyi` & `types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf/type_defs.py` & `types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,15 @@
     from types_aiobotocore_waf.type_defs import ExcludedRuleTypeDef
 
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
@@ -42,15 +40,14 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "ExcludedRuleTypeDef",
     "WafActionTypeDef",
     "WafOverrideActionTypeDef",
-    "BlobTypeDef",
     "ByteMatchSetSummaryTypeDef",
     "FieldToMatchTypeDef",
     "CreateByteMatchSetRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CreateGeoMatchSetRequestRequestTypeDef",
     "CreateIPSetRequestRequestTypeDef",
     "TagTypeDef",
@@ -87,15 +84,14 @@
     "PaginatorConfigTypeDef",
     "GetRateBasedRuleManagedKeysRequestRequestTypeDef",
     "GetRateBasedRuleRequestRequestTypeDef",
     "GetRegexMatchSetRequestRequestTypeDef",
     "GetRegexPatternSetRequestRequestTypeDef",
     "GetRuleGroupRequestRequestTypeDef",
     "GetRuleRequestRequestTypeDef",
-    "TimeWindowOutputTypeDef",
     "GetSizeConstraintSetRequestRequestTypeDef",
     "GetSqlInjectionMatchSetRequestRequestTypeDef",
     "GetWebACLRequestRequestTypeDef",
     "GetXssMatchSetRequestRequestTypeDef",
     "HTTPHeaderTypeDef",
     "IPSetDescriptorTypeDef",
     "IPSetSummaryTypeDef",
@@ -125,19 +121,16 @@
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
@@ -214,24 +207,23 @@
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
@@ -247,18 +239,17 @@
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
@@ -291,15 +282,14 @@
 WafOverrideActionTypeDef = TypedDict(
     "WafOverrideActionTypeDef",
     {
         "Type": WafOverrideActionTypeType,
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
@@ -686,22 +676,14 @@
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
 
@@ -1013,115 +995,58 @@
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
@@ -1942,25 +1867,33 @@
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
@@ -1970,35 +1903,27 @@
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
@@ -2017,43 +1942,40 @@
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
@@ -2303,15 +2225,23 @@
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
@@ -2321,23 +2251,14 @@
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
@@ -2488,11 +2409,11 @@
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

### Comparing `types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf/type_defs.pyi` & `types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,15 @@
     from types_aiobotocore_waf.type_defs import ExcludedRuleTypeDef
 
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
@@ -41,15 +39,14 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "ExcludedRuleTypeDef",
     "WafActionTypeDef",
     "WafOverrideActionTypeDef",
-    "BlobTypeDef",
     "ByteMatchSetSummaryTypeDef",
     "FieldToMatchTypeDef",
     "CreateByteMatchSetRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CreateGeoMatchSetRequestRequestTypeDef",
     "CreateIPSetRequestRequestTypeDef",
     "TagTypeDef",
@@ -86,15 +83,14 @@
     "PaginatorConfigTypeDef",
     "GetRateBasedRuleManagedKeysRequestRequestTypeDef",
     "GetRateBasedRuleRequestRequestTypeDef",
     "GetRegexMatchSetRequestRequestTypeDef",
     "GetRegexPatternSetRequestRequestTypeDef",
     "GetRuleGroupRequestRequestTypeDef",
     "GetRuleRequestRequestTypeDef",
-    "TimeWindowOutputTypeDef",
     "GetSizeConstraintSetRequestRequestTypeDef",
     "GetSqlInjectionMatchSetRequestRequestTypeDef",
     "GetWebACLRequestRequestTypeDef",
     "GetXssMatchSetRequestRequestTypeDef",
     "HTTPHeaderTypeDef",
     "IPSetDescriptorTypeDef",
     "IPSetSummaryTypeDef",
@@ -124,19 +120,16 @@
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
@@ -213,24 +206,23 @@
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
@@ -246,18 +238,17 @@
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
@@ -290,15 +281,14 @@
 WafOverrideActionTypeDef = TypedDict(
     "WafOverrideActionTypeDef",
     {
         "Type": WafOverrideActionTypeType,
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
@@ -677,22 +667,14 @@
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
 
@@ -1002,109 +984,56 @@
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
@@ -1905,25 +1834,33 @@
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
@@ -1931,35 +1868,27 @@
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
@@ -1976,43 +1905,40 @@
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
@@ -2254,15 +2180,23 @@
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
@@ -2272,23 +2206,14 @@
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
@@ -2437,11 +2362,11 @@
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

### Comparing `types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf.egg-info/SOURCES.txt` & `types-aiobotocore-waf-2.5.2.post2/types_aiobotocore_waf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

