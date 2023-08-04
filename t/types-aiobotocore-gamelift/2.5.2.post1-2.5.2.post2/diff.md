# Comparing `tmp/types-aiobotocore-gamelift-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-gamelift-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-gamelift-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:19 2023, max compression
+gzip compressed data, was "types-aiobotocore-gamelift-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:56 2023, max compression
```

## Comparing `types-aiobotocore-gamelift-2.5.2.post1.tar` & `types-aiobotocore-gamelift-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:19.581581 types-aiobotocore-gamelift-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:39:08.000000 types-aiobotocore-gamelift-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    29720 2023-08-02 14:52:19.577582 types-aiobotocore-gamelift-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    28198 2023-08-02 14:39:08.000000 types-aiobotocore-gamelift-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:19.581581 types-aiobotocore-gamelift-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-08-02 14:39:08.000000 types-aiobotocore-gamelift-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:19.573581 types-aiobotocore-gamelift-2.5.2.post1/types_aiobotocore_gamelift/
--rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-08-02 14:39:08.000000 types-aiobotocore-gamelift-2.5.2.post1/types_aiobotocore_gamelift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-08-02 14:39:08.000000 types-aiobotocore-gamelift-2.5.2.post1/types_aiobotocore_gamelift/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-02 14:39:08.000000 types-aiobotocore-gamelift-2.5.2.post1/types_aiobotocore_gamelift/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    88713 2023-08-02 14:39:09.000000 types-aiobotocore-gamelift-2.5.2.post1/types_aiobotocore_gamelift/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    88578 2023-08-02 14:39:09.000000 types-aiobotocore-gamelift-2.5.2.post1/types_aiobotocore_gamelift/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    20628 2023-08-02 14:39:11.000000 types-aiobotocore-gamelift-2.5.2.post1/types_aiobotocore_gamelift/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    20626 2023-08-02 14:39:11.000000 types-aiobotocore-gamelift-2.5.2.post1/types_aiobotocore_gamelift/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    27633 2023-08-02 14:39:09.000000 types-aiobotocore-gamelift-2.5.2.post1/types_aiobotocore_gamelift/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    27609 2023-08-02 14:39:09.000000 types-aiobotocore-gamelift-2.5.2.post1/types_aiobotocore_gamelift/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:39:08.000000 types-aiobotocore-gamelift-2.5.2.post1/types_aiobotocore_gamelift/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    99954 2023-08-02 14:39:13.000000 types-aiobotocore-gamelift-2.5.2.post1/types_aiobotocore_gamelift/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    99855 2023-08-02 14:39:12.000000 types-aiobotocore-gamelift-2.5.2.post1/types_aiobotocore_gamelift/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:39:08.000000 types-aiobotocore-gamelift-2.5.2.post1/types_aiobotocore_gamelift/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:19.577582 types-aiobotocore-gamelift-2.5.2.post1/types_aiobotocore_gamelift.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    29720 2023-08-02 14:52:19.000000 types-aiobotocore-gamelift-2.5.2.post1/types_aiobotocore_gamelift.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-02 14:52:19.000000 types-aiobotocore-gamelift-2.5.2.post1/types_aiobotocore_gamelift.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:19.000000 types-aiobotocore-gamelift-2.5.2.post1/types_aiobotocore_gamelift.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:19.000000 types-aiobotocore-gamelift-2.5.2.post1/types_aiobotocore_gamelift.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:19.000000 types-aiobotocore-gamelift-2.5.2.post1/types_aiobotocore_gamelift.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-02 14:52:19.000000 types-aiobotocore-gamelift-2.5.2.post1/types_aiobotocore_gamelift.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:56.044276 types-aiobotocore-gamelift-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:46:39.000000 types-aiobotocore-gamelift-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16377 2023-08-04 12:00:56.040275 types-aiobotocore-gamelift-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14855 2023-08-04 11:46:39.000000 types-aiobotocore-gamelift-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:56.044276 types-aiobotocore-gamelift-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-08-04 11:46:39.000000 types-aiobotocore-gamelift-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:56.040275 types-aiobotocore-gamelift-2.5.2.post2/types_aiobotocore_gamelift/
+-rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-08-04 11:46:39.000000 types-aiobotocore-gamelift-2.5.2.post2/types_aiobotocore_gamelift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-08-04 11:46:39.000000 types-aiobotocore-gamelift-2.5.2.post2/types_aiobotocore_gamelift/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-04 11:46:39.000000 types-aiobotocore-gamelift-2.5.2.post2/types_aiobotocore_gamelift/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88653 2023-08-04 11:46:40.000000 types-aiobotocore-gamelift-2.5.2.post2/types_aiobotocore_gamelift/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88518 2023-08-04 11:46:39.000000 types-aiobotocore-gamelift-2.5.2.post2/types_aiobotocore_gamelift/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    20628 2023-08-04 11:46:40.000000 types-aiobotocore-gamelift-2.5.2.post2/types_aiobotocore_gamelift/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20626 2023-08-04 11:46:40.000000 types-aiobotocore-gamelift-2.5.2.post2/types_aiobotocore_gamelift/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    27633 2023-08-04 11:46:40.000000 types-aiobotocore-gamelift-2.5.2.post2/types_aiobotocore_gamelift/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27609 2023-08-04 11:46:40.000000 types-aiobotocore-gamelift-2.5.2.post2/types_aiobotocore_gamelift/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:46:39.000000 types-aiobotocore-gamelift-2.5.2.post2/types_aiobotocore_gamelift/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    98077 2023-08-04 11:46:44.000000 types-aiobotocore-gamelift-2.5.2.post2/types_aiobotocore_gamelift/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97978 2023-08-04 11:46:43.000000 types-aiobotocore-gamelift-2.5.2.post2/types_aiobotocore_gamelift/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:46:39.000000 types-aiobotocore-gamelift-2.5.2.post2/types_aiobotocore_gamelift/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:56.040275 types-aiobotocore-gamelift-2.5.2.post2/types_aiobotocore_gamelift.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16377 2023-08-04 12:00:55.000000 types-aiobotocore-gamelift-2.5.2.post2/types_aiobotocore_gamelift.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-04 12:00:55.000000 types-aiobotocore-gamelift-2.5.2.post2/types_aiobotocore_gamelift.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:55.000000 types-aiobotocore-gamelift-2.5.2.post2/types_aiobotocore_gamelift.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:55.000000 types-aiobotocore-gamelift-2.5.2.post2/types_aiobotocore_gamelift.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:55.000000 types-aiobotocore-gamelift-2.5.2.post2/types_aiobotocore_gamelift.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-04 12:00:55.000000 types-aiobotocore-gamelift-2.5.2.post2/types_aiobotocore_gamelift.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-gamelift-2.5.2.post1/LICENSE` & `types-aiobotocore-gamelift-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-gamelift-2.5.2.post1/setup.py` & `types-aiobotocore-gamelift-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-gamelift",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_gamelift"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.GameLift 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-gamelift-2.5.2.post1/types_aiobotocore_gamelift/__init__.py` & `types-aiobotocore-gamelift-2.5.2.post2/types_aiobotocore_gamelift/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-gamelift-2.5.2.post1/types_aiobotocore_gamelift/__init__.pyi` & `types-aiobotocore-gamelift-2.5.2.post2/types_aiobotocore_gamelift/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-gamelift-2.5.2.post1/types_aiobotocore_gamelift/__main__.py` & `types-aiobotocore-gamelift-2.5.2.post2/types_aiobotocore_gamelift/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.GameLift 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.GameLift 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift\nOther"
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

### Comparing `types-aiobotocore-gamelift-2.5.2.post1/types_aiobotocore_gamelift/client.py` & `types-aiobotocore-gamelift-2.5.2.post2/types_aiobotocore_gamelift/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,15 +117,15 @@
     DescribeRuntimeConfigurationOutputTypeDef,
     DescribeScalingPoliciesOutputTypeDef,
     DescribeScriptOutputTypeDef,
     DescribeVpcPeeringAuthorizationsOutputTypeDef,
     DescribeVpcPeeringConnectionsOutputTypeDef,
     DesiredPlayerSessionTypeDef,
     EmptyResponseMetadataTypeDef,
-    FilterConfigurationUnionTypeDef,
+    FilterConfigurationTypeDef,
     GamePropertyTypeDef,
     GameServerGroupAutoScalingPolicyTypeDef,
     GameSessionQueueDestinationTypeDef,
     GetComputeAccessOutputTypeDef,
     GetComputeAuthTokenOutputTypeDef,
     GetGameSessionLogUrlOutputTypeDef,
     GetInstanceAccessOutputTypeDef,
@@ -140,25 +140,25 @@
     ListGameServersOutputTypeDef,
     ListLocationsOutputTypeDef,
     ListScriptsOutputTypeDef,
     ListTagsForResourceResponseTypeDef,
     LocationConfigurationTypeDef,
     PlayerLatencyPolicyTypeDef,
     PlayerLatencyTypeDef,
-    PlayerUnionTypeDef,
-    PriorityConfigurationUnionTypeDef,
+    PlayerTypeDef,
+    PriorityConfigurationTypeDef,
     PutScalingPolicyOutputTypeDef,
     RegisterComputeOutputTypeDef,
     RegisterGameServerOutputTypeDef,
     RequestUploadCredentialsOutputTypeDef,
     ResolveAliasOutputTypeDef,
     ResourceCreationLimitPolicyTypeDef,
     ResumeGameServerGroupOutputTypeDef,
     RoutingStrategyTypeDef,
-    RuntimeConfigurationUnionTypeDef,
+    RuntimeConfigurationTypeDef,
     S3LocationTypeDef,
     SearchGameSessionsOutputTypeDef,
     StartFleetActionsOutputTypeDef,
     StartGameSessionPlacementOutputTypeDef,
     StartMatchBackfillOutputTypeDef,
     StartMatchmakingOutputTypeDef,
     StopFleetActionsOutputTypeDef,
@@ -319,15 +319,15 @@
         ScriptId: str = ...,
         ServerLaunchPath: str = ...,
         ServerLaunchParameters: str = ...,
         LogPaths: Sequence[str] = ...,
         EC2InstanceType: EC2InstanceTypeType = ...,
         EC2InboundPermissions: Sequence[IpPermissionTypeDef] = ...,
         NewGameSessionProtectionPolicy: ProtectionPolicyType = ...,
-        RuntimeConfiguration: RuntimeConfigurationUnionTypeDef = ...,
+        RuntimeConfiguration: RuntimeConfigurationTypeDef = ...,
         ResourceCreationLimitPolicy: ResourceCreationLimitPolicyTypeDef = ...,
         MetricGroups: Sequence[str] = ...,
         PeerVpcAwsAccountId: str = ...,
         PeerVpcId: str = ...,
         FleetType: FleetTypeType = ...,
         InstanceRoleArn: str = ...,
         CertificateConfiguration: CertificateConfigurationTypeDef = ...,
@@ -404,16 +404,16 @@
     async def create_game_session_queue(
         self,
         *,
         Name: str,
         TimeoutInSeconds: int = ...,
         PlayerLatencyPolicies: Sequence[PlayerLatencyPolicyTypeDef] = ...,
         Destinations: Sequence[GameSessionQueueDestinationTypeDef] = ...,
-        FilterConfiguration: FilterConfigurationUnionTypeDef = ...,
-        PriorityConfiguration: PriorityConfigurationUnionTypeDef = ...,
+        FilterConfiguration: FilterConfigurationTypeDef = ...,
+        PriorityConfiguration: PriorityConfigurationTypeDef = ...,
         CustomEventData: str = ...,
         NotificationTarget: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateGameSessionQueueOutputTypeDef:
         """
         Creates a placement queue that processes requests for new game sessions.
 
@@ -1316,27 +1316,27 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/client/#start_game_session_placement)
         """
 
     async def start_match_backfill(
         self,
         *,
         ConfigurationName: str,
-        Players: Sequence[PlayerUnionTypeDef],
+        Players: Sequence[PlayerTypeDef],
         TicketId: str = ...,
         GameSessionArn: str = ...
     ) -> StartMatchBackfillOutputTypeDef:
         """
         Finds new players to fill open slots in currently running game sessions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.start_match_backfill)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/client/#start_match_backfill)
         """
 
     async def start_matchmaking(
-        self, *, ConfigurationName: str, Players: Sequence[PlayerUnionTypeDef], TicketId: str = ...
+        self, *, ConfigurationName: str, Players: Sequence[PlayerTypeDef], TicketId: str = ...
     ) -> StartMatchmakingOutputTypeDef:
         """
         Uses FlexMatch to create a game match for a group of players based on custom
         matchmaking rules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.start_matchmaking)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/client/#start_matchmaking)
@@ -1532,16 +1532,16 @@
     async def update_game_session_queue(
         self,
         *,
         Name: str,
         TimeoutInSeconds: int = ...,
         PlayerLatencyPolicies: Sequence[PlayerLatencyPolicyTypeDef] = ...,
         Destinations: Sequence[GameSessionQueueDestinationTypeDef] = ...,
-        FilterConfiguration: FilterConfigurationUnionTypeDef = ...,
-        PriorityConfiguration: PriorityConfigurationUnionTypeDef = ...,
+        FilterConfiguration: FilterConfigurationTypeDef = ...,
+        PriorityConfiguration: PriorityConfigurationTypeDef = ...,
         CustomEventData: str = ...,
         NotificationTarget: str = ...
     ) -> UpdateGameSessionQueueOutputTypeDef:
         """
         Updates the configuration of a game session queue, which determines how the
         queue processes new game session requests.
 
@@ -1571,15 +1571,15 @@
         Updates settings for a FlexMatch matchmaking configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.update_matchmaking_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/client/#update_matchmaking_configuration)
         """
 
     async def update_runtime_configuration(
-        self, *, FleetId: str, RuntimeConfiguration: RuntimeConfigurationUnionTypeDef
+        self, *, FleetId: str, RuntimeConfiguration: RuntimeConfigurationTypeDef
     ) -> UpdateRuntimeConfigurationOutputTypeDef:
         """
         Updates the current runtime configuration for the specified fleet, which tells
         Amazon GameLift how to launch server processes on all instances in the fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.update_runtime_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/client/#update_runtime_configuration)
```

### Comparing `types-aiobotocore-gamelift-2.5.2.post1/types_aiobotocore_gamelift/client.pyi` & `types-aiobotocore-gamelift-2.5.2.post2/types_aiobotocore_gamelift/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -117,15 +117,15 @@
     DescribeRuntimeConfigurationOutputTypeDef,
     DescribeScalingPoliciesOutputTypeDef,
     DescribeScriptOutputTypeDef,
     DescribeVpcPeeringAuthorizationsOutputTypeDef,
     DescribeVpcPeeringConnectionsOutputTypeDef,
     DesiredPlayerSessionTypeDef,
     EmptyResponseMetadataTypeDef,
-    FilterConfigurationUnionTypeDef,
+    FilterConfigurationTypeDef,
     GamePropertyTypeDef,
     GameServerGroupAutoScalingPolicyTypeDef,
     GameSessionQueueDestinationTypeDef,
     GetComputeAccessOutputTypeDef,
     GetComputeAuthTokenOutputTypeDef,
     GetGameSessionLogUrlOutputTypeDef,
     GetInstanceAccessOutputTypeDef,
@@ -140,25 +140,25 @@
     ListGameServersOutputTypeDef,
     ListLocationsOutputTypeDef,
     ListScriptsOutputTypeDef,
     ListTagsForResourceResponseTypeDef,
     LocationConfigurationTypeDef,
     PlayerLatencyPolicyTypeDef,
     PlayerLatencyTypeDef,
-    PlayerUnionTypeDef,
-    PriorityConfigurationUnionTypeDef,
+    PlayerTypeDef,
+    PriorityConfigurationTypeDef,
     PutScalingPolicyOutputTypeDef,
     RegisterComputeOutputTypeDef,
     RegisterGameServerOutputTypeDef,
     RequestUploadCredentialsOutputTypeDef,
     ResolveAliasOutputTypeDef,
     ResourceCreationLimitPolicyTypeDef,
     ResumeGameServerGroupOutputTypeDef,
     RoutingStrategyTypeDef,
-    RuntimeConfigurationUnionTypeDef,
+    RuntimeConfigurationTypeDef,
     S3LocationTypeDef,
     SearchGameSessionsOutputTypeDef,
     StartFleetActionsOutputTypeDef,
     StartGameSessionPlacementOutputTypeDef,
     StartMatchBackfillOutputTypeDef,
     StartMatchmakingOutputTypeDef,
     StopFleetActionsOutputTypeDef,
@@ -308,15 +308,15 @@
         ScriptId: str = ...,
         ServerLaunchPath: str = ...,
         ServerLaunchParameters: str = ...,
         LogPaths: Sequence[str] = ...,
         EC2InstanceType: EC2InstanceTypeType = ...,
         EC2InboundPermissions: Sequence[IpPermissionTypeDef] = ...,
         NewGameSessionProtectionPolicy: ProtectionPolicyType = ...,
-        RuntimeConfiguration: RuntimeConfigurationUnionTypeDef = ...,
+        RuntimeConfiguration: RuntimeConfigurationTypeDef = ...,
         ResourceCreationLimitPolicy: ResourceCreationLimitPolicyTypeDef = ...,
         MetricGroups: Sequence[str] = ...,
         PeerVpcAwsAccountId: str = ...,
         PeerVpcId: str = ...,
         FleetType: FleetTypeType = ...,
         InstanceRoleArn: str = ...,
         CertificateConfiguration: CertificateConfigurationTypeDef = ...,
@@ -389,16 +389,16 @@
     async def create_game_session_queue(
         self,
         *,
         Name: str,
         TimeoutInSeconds: int = ...,
         PlayerLatencyPolicies: Sequence[PlayerLatencyPolicyTypeDef] = ...,
         Destinations: Sequence[GameSessionQueueDestinationTypeDef] = ...,
-        FilterConfiguration: FilterConfigurationUnionTypeDef = ...,
-        PriorityConfiguration: PriorityConfigurationUnionTypeDef = ...,
+        FilterConfiguration: FilterConfigurationTypeDef = ...,
+        PriorityConfiguration: PriorityConfigurationTypeDef = ...,
         CustomEventData: str = ...,
         NotificationTarget: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateGameSessionQueueOutputTypeDef:
         """
         Creates a placement queue that processes requests for new game sessions.
 
@@ -1225,26 +1225,26 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.start_game_session_placement)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/client/#start_game_session_placement)
         """
     async def start_match_backfill(
         self,
         *,
         ConfigurationName: str,
-        Players: Sequence[PlayerUnionTypeDef],
+        Players: Sequence[PlayerTypeDef],
         TicketId: str = ...,
         GameSessionArn: str = ...
     ) -> StartMatchBackfillOutputTypeDef:
         """
         Finds new players to fill open slots in currently running game sessions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.start_match_backfill)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/client/#start_match_backfill)
         """
     async def start_matchmaking(
-        self, *, ConfigurationName: str, Players: Sequence[PlayerUnionTypeDef], TicketId: str = ...
+        self, *, ConfigurationName: str, Players: Sequence[PlayerTypeDef], TicketId: str = ...
     ) -> StartMatchmakingOutputTypeDef:
         """
         Uses FlexMatch to create a game match for a group of players based on custom
         matchmaking rules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.start_matchmaking)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/client/#start_matchmaking)
@@ -1425,16 +1425,16 @@
     async def update_game_session_queue(
         self,
         *,
         Name: str,
         TimeoutInSeconds: int = ...,
         PlayerLatencyPolicies: Sequence[PlayerLatencyPolicyTypeDef] = ...,
         Destinations: Sequence[GameSessionQueueDestinationTypeDef] = ...,
-        FilterConfiguration: FilterConfigurationUnionTypeDef = ...,
-        PriorityConfiguration: PriorityConfigurationUnionTypeDef = ...,
+        FilterConfiguration: FilterConfigurationTypeDef = ...,
+        PriorityConfiguration: PriorityConfigurationTypeDef = ...,
         CustomEventData: str = ...,
         NotificationTarget: str = ...
     ) -> UpdateGameSessionQueueOutputTypeDef:
         """
         Updates the configuration of a game session queue, which determines how the
         queue processes new game session requests.
 
@@ -1462,15 +1462,15 @@
         """
         Updates settings for a FlexMatch matchmaking configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.update_matchmaking_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/client/#update_matchmaking_configuration)
         """
     async def update_runtime_configuration(
-        self, *, FleetId: str, RuntimeConfiguration: RuntimeConfigurationUnionTypeDef
+        self, *, FleetId: str, RuntimeConfiguration: RuntimeConfigurationTypeDef
     ) -> UpdateRuntimeConfigurationOutputTypeDef:
         """
         Updates the current runtime configuration for the specified fleet, which tells
         Amazon GameLift how to launch server processes on all instances in the fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.update_runtime_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamelift/client/#update_runtime_configuration)
```

### Comparing `types-aiobotocore-gamelift-2.5.2.post1/types_aiobotocore_gamelift/literals.py` & `types-aiobotocore-gamelift-2.5.2.post2/types_aiobotocore_gamelift/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-gamelift-2.5.2.post1/types_aiobotocore_gamelift/literals.pyi` & `types-aiobotocore-gamelift-2.5.2.post2/types_aiobotocore_gamelift/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-gamelift-2.5.2.post1/types_aiobotocore_gamelift/paginator.py` & `types-aiobotocore-gamelift-2.5.2.post2/types_aiobotocore_gamelift/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-gamelift-2.5.2.post1/types_aiobotocore_gamelift/paginator.pyi` & `types-aiobotocore-gamelift-2.5.2.post2/types_aiobotocore_gamelift/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-gamelift-2.5.2.post1/types_aiobotocore_gamelift/type_defs.py` & `types-aiobotocore-gamelift-2.5.2.post2/types_aiobotocore_gamelift/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,14 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AcceptMatchInputRequestTypeDef",
     "RoutingStrategyTypeDef",
     "AnywhereConfigurationTypeDef",
-    "AttributeValueOutputTypeDef",
     "AttributeValueTypeDef",
     "AwsCredentialsTypeDef",
     "BlobTypeDef",
     "BuildTypeDef",
     "CertificateConfigurationTypeDef",
     "ClaimFilterOptionTypeDef",
     "GameServerTypeDef",
@@ -149,20 +148,18 @@
     "DescribePlayerSessionsInputRequestTypeDef",
     "DescribeRuntimeConfigurationInputRequestTypeDef",
     "DescribeScalingPoliciesInputRequestTypeDef",
     "DescribeScriptInputRequestTypeDef",
     "DescribeVpcPeeringConnectionsInputRequestTypeDef",
     "DesiredPlayerSessionTypeDef",
     "EC2InstanceCountsTypeDef",
-    "FilterConfigurationOutputTypeDef",
     "TargetTrackingConfigurationTypeDef",
     "MatchedPlayerSessionTypeDef",
     "PlacedPlayerSessionTypeDef",
     "PlayerLatencyTypeDef",
-    "PriorityConfigurationOutputTypeDef",
     "GetComputeAccessInputRequestTypeDef",
     "GetComputeAuthTokenInputRequestTypeDef",
     "GetGameSessionLogUrlInputRequestTypeDef",
     "GetInstanceAccessInputRequestTypeDef",
     "InstanceCredentialsTypeDef",
     "ListAliasesInputRequestTypeDef",
     "ListBuildsInputRequestTypeDef",
@@ -191,15 +188,14 @@
     "UpdateFleetCapacityInputRequestTypeDef",
     "UpdateGameServerInputRequestTypeDef",
     "UpdateGameSessionInputRequestTypeDef",
     "ValidateMatchmakingRuleSetInputRequestTypeDef",
     "VpcPeeringConnectionStatusTypeDef",
     "AliasTypeDef",
     "UpdateAliasInputRequestTypeDef",
-    "PlayerOutputTypeDef",
     "PlayerTypeDef",
     "ClaimGameServerInputRequestTypeDef",
     "ClaimGameServerOutputTypeDef",
     "DescribeBuildOutputTypeDef",
     "DescribeGameServerOutputTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetComputeAccessOutputTypeDef",
@@ -245,14 +241,15 @@
     "UpdateGameServerGroupInputRequestTypeDef",
     "CreateGameSessionInputRequestTypeDef",
     "CreateMatchmakingConfigurationInputRequestTypeDef",
     "GameSessionTypeDef",
     "MatchmakingConfigurationTypeDef",
     "UpdateMatchmakingConfigurationInputRequestTypeDef",
     "CreateGameSessionQueueInputRequestTypeDef",
+    "GameSessionQueueTypeDef",
     "UpdateGameSessionQueueInputRequestTypeDef",
     "CreateLocationOutputTypeDef",
     "ListLocationsOutputTypeDef",
     "CreateMatchmakingRuleSetOutputTypeDef",
     "DescribeMatchmakingRuleSetsOutputTypeDef",
     "CreatePlayerSessionOutputTypeDef",
     "CreatePlayerSessionsOutputTypeDef",
@@ -285,32 +282,29 @@
     "DescribeFleetEventsInputRequestTypeDef",
     "DescribeFleetEventsOutputTypeDef",
     "DescribeFleetLocationUtilizationOutputTypeDef",
     "DescribeFleetUtilizationOutputTypeDef",
     "DescribeGameServerInstancesOutputTypeDef",
     "DescribeInstancesOutputTypeDef",
     "FleetCapacityTypeDef",
-    "FilterConfigurationUnionTypeDef",
     "GameServerGroupAutoScalingPolicyTypeDef",
     "GameSessionConnectionInfoTypeDef",
     "GameSessionPlacementTypeDef",
     "StartGameSessionPlacementInputRequestTypeDef",
-    "GameSessionQueueTypeDef",
-    "PriorityConfigurationUnionTypeDef",
     "InstanceAccessTypeDef",
     "PutScalingPolicyInputRequestTypeDef",
     "ScalingPolicyTypeDef",
-    "RuntimeConfigurationOutputTypeDef",
     "RuntimeConfigurationTypeDef",
     "VpcPeeringConnectionTypeDef",
     "CreateAliasOutputTypeDef",
     "DescribeAliasOutputTypeDef",
     "ListAliasesOutputTypeDef",
     "UpdateAliasOutputTypeDef",
-    "PlayerUnionTypeDef",
+    "StartMatchBackfillInputRequestTypeDef",
+    "StartMatchmakingInputRequestTypeDef",
     "CreateScriptOutputTypeDef",
     "DescribeScriptOutputTypeDef",
     "ListScriptsOutputTypeDef",
     "UpdateScriptOutputTypeDef",
     "CreateFleetOutputTypeDef",
     "DescribeFleetAttributesOutputTypeDef",
     "DescribeFleetLocationAttributesOutputTypeDef",
@@ -325,34 +319,31 @@
     "DescribeGameSessionsOutputTypeDef",
     "GameSessionDetailTypeDef",
     "SearchGameSessionsOutputTypeDef",
     "UpdateGameSessionOutputTypeDef",
     "CreateMatchmakingConfigurationOutputTypeDef",
     "DescribeMatchmakingConfigurationsOutputTypeDef",
     "UpdateMatchmakingConfigurationOutputTypeDef",
+    "CreateGameSessionQueueOutputTypeDef",
+    "DescribeGameSessionQueuesOutputTypeDef",
+    "UpdateGameSessionQueueOutputTypeDef",
     "DescribeFleetCapacityOutputTypeDef",
     "DescribeFleetLocationCapacityOutputTypeDef",
     "CreateGameServerGroupInputRequestTypeDef",
     "MatchmakingTicketTypeDef",
     "DescribeGameSessionPlacementOutputTypeDef",
     "StartGameSessionPlacementOutputTypeDef",
     "StopGameSessionPlacementOutputTypeDef",
-    "CreateGameSessionQueueOutputTypeDef",
-    "DescribeGameSessionQueuesOutputTypeDef",
-    "UpdateGameSessionQueueOutputTypeDef",
     "GetInstanceAccessOutputTypeDef",
     "DescribeScalingPoliciesOutputTypeDef",
-    "DescribeRuntimeConfigurationOutputTypeDef",
-    "UpdateRuntimeConfigurationOutputTypeDef",
     "CreateFleetInputRequestTypeDef",
-    "RuntimeConfigurationUnionTypeDef",
+    "DescribeRuntimeConfigurationOutputTypeDef",
     "UpdateRuntimeConfigurationInputRequestTypeDef",
+    "UpdateRuntimeConfigurationOutputTypeDef",
     "DescribeVpcPeeringConnectionsOutputTypeDef",
-    "StartMatchBackfillInputRequestTypeDef",
-    "StartMatchmakingInputRequestTypeDef",
     "DescribeGameSessionDetailsOutputTypeDef",
     "DescribeMatchmakingOutputTypeDef",
     "StartMatchBackfillOutputTypeDef",
     "StartMatchmakingOutputTypeDef",
 )
 
 AcceptMatchInputRequestTypeDef = TypedDict(
@@ -377,32 +368,21 @@
 AnywhereConfigurationTypeDef = TypedDict(
     "AnywhereConfigurationTypeDef",
     {
         "Cost": str,
     },
 )
 
-AttributeValueOutputTypeDef = TypedDict(
-    "AttributeValueOutputTypeDef",
-    {
-        "S": str,
-        "N": float,
-        "SL": List[str],
-        "SDM": Dict[str, float],
-    },
-    total=False,
-)
-
 AttributeValueTypeDef = TypedDict(
     "AttributeValueTypeDef",
     {
         "S": str,
         "N": float,
-        "SL": Sequence[str],
-        "SDM": Mapping[str, float],
+        "SL": List[str],
+        "SDM": Dict[str, float],
     },
     total=False,
 )
 
 AwsCredentialsTypeDef = TypedDict(
     "AwsCredentialsTypeDef",
     {
@@ -1286,22 +1266,14 @@
         "ACTIVE": int,
         "IDLE": int,
         "TERMINATING": int,
     },
     total=False,
 )
 
-FilterConfigurationOutputTypeDef = TypedDict(
-    "FilterConfigurationOutputTypeDef",
-    {
-        "AllowedLocations": List[str],
-    },
-    total=False,
-)
-
 TargetTrackingConfigurationTypeDef = TypedDict(
     "TargetTrackingConfigurationTypeDef",
     {
         "TargetValue": float,
     },
 )
 
@@ -1329,23 +1301,14 @@
         "PlayerId": str,
         "RegionIdentifier": str,
         "LatencyInMilliseconds": float,
     },
     total=False,
 )
 
-PriorityConfigurationOutputTypeDef = TypedDict(
-    "PriorityConfigurationOutputTypeDef",
-    {
-        "PriorityOrder": List[PriorityTypeType],
-        "LocationOrder": List[str],
-    },
-    total=False,
-)
-
 GetComputeAccessInputRequestTypeDef = TypedDict(
     "GetComputeAccessInputRequestTypeDef",
     {
         "FleetId": str,
         "ComputeName": str,
     },
 )
@@ -1824,32 +1787,21 @@
 
 class UpdateAliasInputRequestTypeDef(
     _RequiredUpdateAliasInputRequestTypeDef, _OptionalUpdateAliasInputRequestTypeDef
 ):
     pass
 
 
-PlayerOutputTypeDef = TypedDict(
-    "PlayerOutputTypeDef",
-    {
-        "PlayerId": str,
-        "PlayerAttributes": Dict[str, AttributeValueOutputTypeDef],
-        "Team": str,
-        "LatencyInMs": Dict[str, int],
-    },
-    total=False,
-)
-
 PlayerTypeDef = TypedDict(
     "PlayerTypeDef",
     {
         "PlayerId": str,
-        "PlayerAttributes": Mapping[str, AttributeValueTypeDef],
+        "PlayerAttributes": Dict[str, AttributeValueTypeDef],
         "Team": str,
-        "LatencyInMs": Mapping[str, int],
+        "LatencyInMs": Dict[str, int],
     },
     total=False,
 )
 
 _RequiredClaimGameServerInputRequestTypeDef = TypedDict(
     "_RequiredClaimGameServerInputRequestTypeDef",
     {
@@ -2598,14 +2550,30 @@
 class CreateGameSessionQueueInputRequestTypeDef(
     _RequiredCreateGameSessionQueueInputRequestTypeDef,
     _OptionalCreateGameSessionQueueInputRequestTypeDef,
 ):
     pass
 
 
+GameSessionQueueTypeDef = TypedDict(
+    "GameSessionQueueTypeDef",
+    {
+        "Name": str,
+        "GameSessionQueueArn": str,
+        "TimeoutInSeconds": int,
+        "PlayerLatencyPolicies": List[PlayerLatencyPolicyTypeDef],
+        "Destinations": List[GameSessionQueueDestinationTypeDef],
+        "FilterConfiguration": FilterConfigurationTypeDef,
+        "PriorityConfiguration": PriorityConfigurationTypeDef,
+        "CustomEventData": str,
+        "NotificationTarget": str,
+    },
+    total=False,
+)
+
 _RequiredUpdateGameSessionQueueInputRequestTypeDef = TypedDict(
     "_RequiredUpdateGameSessionQueueInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateGameSessionQueueInputRequestTypeDef = TypedDict(
@@ -3090,17 +3058,14 @@
         "InstanceType": EC2InstanceTypeType,
         "InstanceCounts": EC2InstanceCountsTypeDef,
         "Location": str,
     },
     total=False,
 )
 
-FilterConfigurationUnionTypeDef = Union[
-    FilterConfigurationTypeDef, FilterConfigurationOutputTypeDef
-]
 _RequiredGameServerGroupAutoScalingPolicyTypeDef = TypedDict(
     "_RequiredGameServerGroupAutoScalingPolicyTypeDef",
     {
         "TargetTrackingConfiguration": TargetTrackingConfigurationTypeDef,
     },
 )
 _OptionalGameServerGroupAutoScalingPolicyTypeDef = TypedDict(
@@ -3180,33 +3145,14 @@
 class StartGameSessionPlacementInputRequestTypeDef(
     _RequiredStartGameSessionPlacementInputRequestTypeDef,
     _OptionalStartGameSessionPlacementInputRequestTypeDef,
 ):
     pass
 
 
-GameSessionQueueTypeDef = TypedDict(
-    "GameSessionQueueTypeDef",
-    {
-        "Name": str,
-        "GameSessionQueueArn": str,
-        "TimeoutInSeconds": int,
-        "PlayerLatencyPolicies": List[PlayerLatencyPolicyTypeDef],
-        "Destinations": List[GameSessionQueueDestinationTypeDef],
-        "FilterConfiguration": FilterConfigurationOutputTypeDef,
-        "PriorityConfiguration": PriorityConfigurationOutputTypeDef,
-        "CustomEventData": str,
-        "NotificationTarget": str,
-    },
-    total=False,
-)
-
-PriorityConfigurationUnionTypeDef = Union[
-    PriorityConfigurationTypeDef, PriorityConfigurationOutputTypeDef
-]
 InstanceAccessTypeDef = TypedDict(
     "InstanceAccessTypeDef",
     {
         "FleetId": str,
         "InstanceId": str,
         "IpAddress": str,
         "OperatingSystem": OperatingSystemType,
@@ -3261,24 +3207,14 @@
         "TargetConfiguration": TargetConfigurationTypeDef,
         "UpdateStatus": Literal["PENDING_UPDATE"],
         "Location": str,
     },
     total=False,
 )
 
-RuntimeConfigurationOutputTypeDef = TypedDict(
-    "RuntimeConfigurationOutputTypeDef",
-    {
-        "ServerProcesses": List[ServerProcessTypeDef],
-        "MaxConcurrentGameSessionActivations": int,
-        "GameSessionActivationTimeoutSeconds": int,
-    },
-    total=False,
-)
-
 RuntimeConfigurationTypeDef = TypedDict(
     "RuntimeConfigurationTypeDef",
     {
         "ServerProcesses": Sequence[ServerProcessTypeDef],
         "MaxConcurrentGameSessionActivations": int,
         "GameSessionActivationTimeoutSeconds": int,
     },
@@ -3328,15 +3264,59 @@
     "UpdateAliasOutputTypeDef",
     {
         "Alias": AliasTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PlayerUnionTypeDef = Union[PlayerTypeDef, PlayerOutputTypeDef]
+_RequiredStartMatchBackfillInputRequestTypeDef = TypedDict(
+    "_RequiredStartMatchBackfillInputRequestTypeDef",
+    {
+        "ConfigurationName": str,
+        "Players": Sequence[PlayerTypeDef],
+    },
+)
+_OptionalStartMatchBackfillInputRequestTypeDef = TypedDict(
+    "_OptionalStartMatchBackfillInputRequestTypeDef",
+    {
+        "TicketId": str,
+        "GameSessionArn": str,
+    },
+    total=False,
+)
+
+
+class StartMatchBackfillInputRequestTypeDef(
+    _RequiredStartMatchBackfillInputRequestTypeDef, _OptionalStartMatchBackfillInputRequestTypeDef
+):
+    pass
+
+
+_RequiredStartMatchmakingInputRequestTypeDef = TypedDict(
+    "_RequiredStartMatchmakingInputRequestTypeDef",
+    {
+        "ConfigurationName": str,
+        "Players": Sequence[PlayerTypeDef],
+    },
+)
+_OptionalStartMatchmakingInputRequestTypeDef = TypedDict(
+    "_OptionalStartMatchmakingInputRequestTypeDef",
+    {
+        "TicketId": str,
+    },
+    total=False,
+)
+
+
+class StartMatchmakingInputRequestTypeDef(
+    _RequiredStartMatchmakingInputRequestTypeDef, _OptionalStartMatchmakingInputRequestTypeDef
+):
+    pass
+
+
 CreateScriptOutputTypeDef = TypedDict(
     "CreateScriptOutputTypeDef",
     {
         "Script": ScriptTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3516,14 +3496,39 @@
     "UpdateMatchmakingConfigurationOutputTypeDef",
     {
         "Configuration": MatchmakingConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CreateGameSessionQueueOutputTypeDef = TypedDict(
+    "CreateGameSessionQueueOutputTypeDef",
+    {
+        "GameSessionQueue": GameSessionQueueTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeGameSessionQueuesOutputTypeDef = TypedDict(
+    "DescribeGameSessionQueuesOutputTypeDef",
+    {
+        "GameSessionQueues": List[GameSessionQueueTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateGameSessionQueueOutputTypeDef = TypedDict(
+    "UpdateGameSessionQueueOutputTypeDef",
+    {
+        "GameSessionQueue": GameSessionQueueTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeFleetCapacityOutputTypeDef = TypedDict(
     "DescribeFleetCapacityOutputTypeDef",
     {
         "FleetCapacity": List[FleetCapacityTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -3575,15 +3580,15 @@
         "ConfigurationName": str,
         "ConfigurationArn": str,
         "Status": MatchmakingConfigurationStatusType,
         "StatusReason": str,
         "StatusMessage": str,
         "StartTime": datetime,
         "EndTime": datetime,
-        "Players": List[PlayerOutputTypeDef],
+        "Players": List[PlayerTypeDef],
         "GameSessionConnectionInfo": GameSessionConnectionInfoTypeDef,
         "EstimatedWaitTime": int,
     },
     total=False,
 )
 
 DescribeGameSessionPlacementOutputTypeDef = TypedDict(
@@ -3606,39 +3611,14 @@
     "StopGameSessionPlacementOutputTypeDef",
     {
         "GameSessionPlacement": GameSessionPlacementTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateGameSessionQueueOutputTypeDef = TypedDict(
-    "CreateGameSessionQueueOutputTypeDef",
-    {
-        "GameSessionQueue": GameSessionQueueTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeGameSessionQueuesOutputTypeDef = TypedDict(
-    "DescribeGameSessionQueuesOutputTypeDef",
-    {
-        "GameSessionQueues": List[GameSessionQueueTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateGameSessionQueueOutputTypeDef = TypedDict(
-    "UpdateGameSessionQueueOutputTypeDef",
-    {
-        "GameSessionQueue": GameSessionQueueTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 GetInstanceAccessOutputTypeDef = TypedDict(
     "GetInstanceAccessOutputTypeDef",
     {
         "InstanceAccess": InstanceAccessTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3648,30 +3628,14 @@
     {
         "ScalingPolicies": List[ScalingPolicyTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeRuntimeConfigurationOutputTypeDef = TypedDict(
-    "DescribeRuntimeConfigurationOutputTypeDef",
-    {
-        "RuntimeConfiguration": RuntimeConfigurationOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateRuntimeConfigurationOutputTypeDef = TypedDict(
-    "UpdateRuntimeConfigurationOutputTypeDef",
-    {
-        "RuntimeConfiguration": RuntimeConfigurationOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateFleetInputRequestTypeDef = TypedDict(
     "_RequiredCreateFleetInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreateFleetInputRequestTypeDef = TypedDict(
@@ -3705,78 +3669,46 @@
 
 class CreateFleetInputRequestTypeDef(
     _RequiredCreateFleetInputRequestTypeDef, _OptionalCreateFleetInputRequestTypeDef
 ):
     pass
 
 
-RuntimeConfigurationUnionTypeDef = Union[
-    RuntimeConfigurationTypeDef, RuntimeConfigurationOutputTypeDef
-]
-UpdateRuntimeConfigurationInputRequestTypeDef = TypedDict(
-    "UpdateRuntimeConfigurationInputRequestTypeDef",
+DescribeRuntimeConfigurationOutputTypeDef = TypedDict(
+    "DescribeRuntimeConfigurationOutputTypeDef",
     {
-        "FleetId": str,
         "RuntimeConfiguration": RuntimeConfigurationTypeDef,
-    },
-)
-
-DescribeVpcPeeringConnectionsOutputTypeDef = TypedDict(
-    "DescribeVpcPeeringConnectionsOutputTypeDef",
-    {
-        "VpcPeeringConnections": List[VpcPeeringConnectionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredStartMatchBackfillInputRequestTypeDef = TypedDict(
-    "_RequiredStartMatchBackfillInputRequestTypeDef",
-    {
-        "ConfigurationName": str,
-        "Players": Sequence[PlayerUnionTypeDef],
-    },
-)
-_OptionalStartMatchBackfillInputRequestTypeDef = TypedDict(
-    "_OptionalStartMatchBackfillInputRequestTypeDef",
+UpdateRuntimeConfigurationInputRequestTypeDef = TypedDict(
+    "UpdateRuntimeConfigurationInputRequestTypeDef",
     {
-        "TicketId": str,
-        "GameSessionArn": str,
+        "FleetId": str,
+        "RuntimeConfiguration": RuntimeConfigurationTypeDef,
     },
-    total=False,
 )
 
-
-class StartMatchBackfillInputRequestTypeDef(
-    _RequiredStartMatchBackfillInputRequestTypeDef, _OptionalStartMatchBackfillInputRequestTypeDef
-):
-    pass
-
-
-_RequiredStartMatchmakingInputRequestTypeDef = TypedDict(
-    "_RequiredStartMatchmakingInputRequestTypeDef",
+UpdateRuntimeConfigurationOutputTypeDef = TypedDict(
+    "UpdateRuntimeConfigurationOutputTypeDef",
     {
-        "ConfigurationName": str,
-        "Players": Sequence[PlayerUnionTypeDef],
+        "RuntimeConfiguration": RuntimeConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalStartMatchmakingInputRequestTypeDef = TypedDict(
-    "_OptionalStartMatchmakingInputRequestTypeDef",
+
+DescribeVpcPeeringConnectionsOutputTypeDef = TypedDict(
+    "DescribeVpcPeeringConnectionsOutputTypeDef",
     {
-        "TicketId": str,
+        "VpcPeeringConnections": List[VpcPeeringConnectionTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class StartMatchmakingInputRequestTypeDef(
-    _RequiredStartMatchmakingInputRequestTypeDef, _OptionalStartMatchmakingInputRequestTypeDef
-):
-    pass
-
-
 DescribeGameSessionDetailsOutputTypeDef = TypedDict(
     "DescribeGameSessionDetailsOutputTypeDef",
     {
         "GameSessionDetails": List[GameSessionDetailTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `types-aiobotocore-gamelift-2.5.2.post1/types_aiobotocore_gamelift/type_defs.pyi` & `types-aiobotocore-gamelift-2.5.2.post2/types_aiobotocore_gamelift/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,14 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AcceptMatchInputRequestTypeDef",
     "RoutingStrategyTypeDef",
     "AnywhereConfigurationTypeDef",
-    "AttributeValueOutputTypeDef",
     "AttributeValueTypeDef",
     "AwsCredentialsTypeDef",
     "BlobTypeDef",
     "BuildTypeDef",
     "CertificateConfigurationTypeDef",
     "ClaimFilterOptionTypeDef",
     "GameServerTypeDef",
@@ -148,20 +147,18 @@
     "DescribePlayerSessionsInputRequestTypeDef",
     "DescribeRuntimeConfigurationInputRequestTypeDef",
     "DescribeScalingPoliciesInputRequestTypeDef",
     "DescribeScriptInputRequestTypeDef",
     "DescribeVpcPeeringConnectionsInputRequestTypeDef",
     "DesiredPlayerSessionTypeDef",
     "EC2InstanceCountsTypeDef",
-    "FilterConfigurationOutputTypeDef",
     "TargetTrackingConfigurationTypeDef",
     "MatchedPlayerSessionTypeDef",
     "PlacedPlayerSessionTypeDef",
     "PlayerLatencyTypeDef",
-    "PriorityConfigurationOutputTypeDef",
     "GetComputeAccessInputRequestTypeDef",
     "GetComputeAuthTokenInputRequestTypeDef",
     "GetGameSessionLogUrlInputRequestTypeDef",
     "GetInstanceAccessInputRequestTypeDef",
     "InstanceCredentialsTypeDef",
     "ListAliasesInputRequestTypeDef",
     "ListBuildsInputRequestTypeDef",
@@ -190,15 +187,14 @@
     "UpdateFleetCapacityInputRequestTypeDef",
     "UpdateGameServerInputRequestTypeDef",
     "UpdateGameSessionInputRequestTypeDef",
     "ValidateMatchmakingRuleSetInputRequestTypeDef",
     "VpcPeeringConnectionStatusTypeDef",
     "AliasTypeDef",
     "UpdateAliasInputRequestTypeDef",
-    "PlayerOutputTypeDef",
     "PlayerTypeDef",
     "ClaimGameServerInputRequestTypeDef",
     "ClaimGameServerOutputTypeDef",
     "DescribeBuildOutputTypeDef",
     "DescribeGameServerOutputTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetComputeAccessOutputTypeDef",
@@ -244,14 +240,15 @@
     "UpdateGameServerGroupInputRequestTypeDef",
     "CreateGameSessionInputRequestTypeDef",
     "CreateMatchmakingConfigurationInputRequestTypeDef",
     "GameSessionTypeDef",
     "MatchmakingConfigurationTypeDef",
     "UpdateMatchmakingConfigurationInputRequestTypeDef",
     "CreateGameSessionQueueInputRequestTypeDef",
+    "GameSessionQueueTypeDef",
     "UpdateGameSessionQueueInputRequestTypeDef",
     "CreateLocationOutputTypeDef",
     "ListLocationsOutputTypeDef",
     "CreateMatchmakingRuleSetOutputTypeDef",
     "DescribeMatchmakingRuleSetsOutputTypeDef",
     "CreatePlayerSessionOutputTypeDef",
     "CreatePlayerSessionsOutputTypeDef",
@@ -284,32 +281,29 @@
     "DescribeFleetEventsInputRequestTypeDef",
     "DescribeFleetEventsOutputTypeDef",
     "DescribeFleetLocationUtilizationOutputTypeDef",
     "DescribeFleetUtilizationOutputTypeDef",
     "DescribeGameServerInstancesOutputTypeDef",
     "DescribeInstancesOutputTypeDef",
     "FleetCapacityTypeDef",
-    "FilterConfigurationUnionTypeDef",
     "GameServerGroupAutoScalingPolicyTypeDef",
     "GameSessionConnectionInfoTypeDef",
     "GameSessionPlacementTypeDef",
     "StartGameSessionPlacementInputRequestTypeDef",
-    "GameSessionQueueTypeDef",
-    "PriorityConfigurationUnionTypeDef",
     "InstanceAccessTypeDef",
     "PutScalingPolicyInputRequestTypeDef",
     "ScalingPolicyTypeDef",
-    "RuntimeConfigurationOutputTypeDef",
     "RuntimeConfigurationTypeDef",
     "VpcPeeringConnectionTypeDef",
     "CreateAliasOutputTypeDef",
     "DescribeAliasOutputTypeDef",
     "ListAliasesOutputTypeDef",
     "UpdateAliasOutputTypeDef",
-    "PlayerUnionTypeDef",
+    "StartMatchBackfillInputRequestTypeDef",
+    "StartMatchmakingInputRequestTypeDef",
     "CreateScriptOutputTypeDef",
     "DescribeScriptOutputTypeDef",
     "ListScriptsOutputTypeDef",
     "UpdateScriptOutputTypeDef",
     "CreateFleetOutputTypeDef",
     "DescribeFleetAttributesOutputTypeDef",
     "DescribeFleetLocationAttributesOutputTypeDef",
@@ -324,34 +318,31 @@
     "DescribeGameSessionsOutputTypeDef",
     "GameSessionDetailTypeDef",
     "SearchGameSessionsOutputTypeDef",
     "UpdateGameSessionOutputTypeDef",
     "CreateMatchmakingConfigurationOutputTypeDef",
     "DescribeMatchmakingConfigurationsOutputTypeDef",
     "UpdateMatchmakingConfigurationOutputTypeDef",
+    "CreateGameSessionQueueOutputTypeDef",
+    "DescribeGameSessionQueuesOutputTypeDef",
+    "UpdateGameSessionQueueOutputTypeDef",
     "DescribeFleetCapacityOutputTypeDef",
     "DescribeFleetLocationCapacityOutputTypeDef",
     "CreateGameServerGroupInputRequestTypeDef",
     "MatchmakingTicketTypeDef",
     "DescribeGameSessionPlacementOutputTypeDef",
     "StartGameSessionPlacementOutputTypeDef",
     "StopGameSessionPlacementOutputTypeDef",
-    "CreateGameSessionQueueOutputTypeDef",
-    "DescribeGameSessionQueuesOutputTypeDef",
-    "UpdateGameSessionQueueOutputTypeDef",
     "GetInstanceAccessOutputTypeDef",
     "DescribeScalingPoliciesOutputTypeDef",
-    "DescribeRuntimeConfigurationOutputTypeDef",
-    "UpdateRuntimeConfigurationOutputTypeDef",
     "CreateFleetInputRequestTypeDef",
-    "RuntimeConfigurationUnionTypeDef",
+    "DescribeRuntimeConfigurationOutputTypeDef",
     "UpdateRuntimeConfigurationInputRequestTypeDef",
+    "UpdateRuntimeConfigurationOutputTypeDef",
     "DescribeVpcPeeringConnectionsOutputTypeDef",
-    "StartMatchBackfillInputRequestTypeDef",
-    "StartMatchmakingInputRequestTypeDef",
     "DescribeGameSessionDetailsOutputTypeDef",
     "DescribeMatchmakingOutputTypeDef",
     "StartMatchBackfillOutputTypeDef",
     "StartMatchmakingOutputTypeDef",
 )
 
 AcceptMatchInputRequestTypeDef = TypedDict(
@@ -376,32 +367,21 @@
 AnywhereConfigurationTypeDef = TypedDict(
     "AnywhereConfigurationTypeDef",
     {
         "Cost": str,
     },
 )
 
-AttributeValueOutputTypeDef = TypedDict(
-    "AttributeValueOutputTypeDef",
-    {
-        "S": str,
-        "N": float,
-        "SL": List[str],
-        "SDM": Dict[str, float],
-    },
-    total=False,
-)
-
 AttributeValueTypeDef = TypedDict(
     "AttributeValueTypeDef",
     {
         "S": str,
         "N": float,
-        "SL": Sequence[str],
-        "SDM": Mapping[str, float],
+        "SL": List[str],
+        "SDM": Dict[str, float],
     },
     total=False,
 )
 
 AwsCredentialsTypeDef = TypedDict(
     "AwsCredentialsTypeDef",
     {
@@ -1265,22 +1245,14 @@
         "ACTIVE": int,
         "IDLE": int,
         "TERMINATING": int,
     },
     total=False,
 )
 
-FilterConfigurationOutputTypeDef = TypedDict(
-    "FilterConfigurationOutputTypeDef",
-    {
-        "AllowedLocations": List[str],
-    },
-    total=False,
-)
-
 TargetTrackingConfigurationTypeDef = TypedDict(
     "TargetTrackingConfigurationTypeDef",
     {
         "TargetValue": float,
     },
 )
 
@@ -1308,23 +1280,14 @@
         "PlayerId": str,
         "RegionIdentifier": str,
         "LatencyInMilliseconds": float,
     },
     total=False,
 )
 
-PriorityConfigurationOutputTypeDef = TypedDict(
-    "PriorityConfigurationOutputTypeDef",
-    {
-        "PriorityOrder": List[PriorityTypeType],
-        "LocationOrder": List[str],
-    },
-    total=False,
-)
-
 GetComputeAccessInputRequestTypeDef = TypedDict(
     "GetComputeAccessInputRequestTypeDef",
     {
         "FleetId": str,
         "ComputeName": str,
     },
 )
@@ -1779,32 +1742,21 @@
 )
 
 class UpdateAliasInputRequestTypeDef(
     _RequiredUpdateAliasInputRequestTypeDef, _OptionalUpdateAliasInputRequestTypeDef
 ):
     pass
 
-PlayerOutputTypeDef = TypedDict(
-    "PlayerOutputTypeDef",
-    {
-        "PlayerId": str,
-        "PlayerAttributes": Dict[str, AttributeValueOutputTypeDef],
-        "Team": str,
-        "LatencyInMs": Dict[str, int],
-    },
-    total=False,
-)
-
 PlayerTypeDef = TypedDict(
     "PlayerTypeDef",
     {
         "PlayerId": str,
-        "PlayerAttributes": Mapping[str, AttributeValueTypeDef],
+        "PlayerAttributes": Dict[str, AttributeValueTypeDef],
         "Team": str,
-        "LatencyInMs": Mapping[str, int],
+        "LatencyInMs": Dict[str, int],
     },
     total=False,
 )
 
 _RequiredClaimGameServerInputRequestTypeDef = TypedDict(
     "_RequiredClaimGameServerInputRequestTypeDef",
     {
@@ -2529,14 +2481,30 @@
 
 class CreateGameSessionQueueInputRequestTypeDef(
     _RequiredCreateGameSessionQueueInputRequestTypeDef,
     _OptionalCreateGameSessionQueueInputRequestTypeDef,
 ):
     pass
 
+GameSessionQueueTypeDef = TypedDict(
+    "GameSessionQueueTypeDef",
+    {
+        "Name": str,
+        "GameSessionQueueArn": str,
+        "TimeoutInSeconds": int,
+        "PlayerLatencyPolicies": List[PlayerLatencyPolicyTypeDef],
+        "Destinations": List[GameSessionQueueDestinationTypeDef],
+        "FilterConfiguration": FilterConfigurationTypeDef,
+        "PriorityConfiguration": PriorityConfigurationTypeDef,
+        "CustomEventData": str,
+        "NotificationTarget": str,
+    },
+    total=False,
+)
+
 _RequiredUpdateGameSessionQueueInputRequestTypeDef = TypedDict(
     "_RequiredUpdateGameSessionQueueInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateGameSessionQueueInputRequestTypeDef = TypedDict(
@@ -3005,17 +2973,14 @@
         "InstanceType": EC2InstanceTypeType,
         "InstanceCounts": EC2InstanceCountsTypeDef,
         "Location": str,
     },
     total=False,
 )
 
-FilterConfigurationUnionTypeDef = Union[
-    FilterConfigurationTypeDef, FilterConfigurationOutputTypeDef
-]
 _RequiredGameServerGroupAutoScalingPolicyTypeDef = TypedDict(
     "_RequiredGameServerGroupAutoScalingPolicyTypeDef",
     {
         "TargetTrackingConfiguration": TargetTrackingConfigurationTypeDef,
     },
 )
 _OptionalGameServerGroupAutoScalingPolicyTypeDef = TypedDict(
@@ -3091,33 +3056,14 @@
 
 class StartGameSessionPlacementInputRequestTypeDef(
     _RequiredStartGameSessionPlacementInputRequestTypeDef,
     _OptionalStartGameSessionPlacementInputRequestTypeDef,
 ):
     pass
 
-GameSessionQueueTypeDef = TypedDict(
-    "GameSessionQueueTypeDef",
-    {
-        "Name": str,
-        "GameSessionQueueArn": str,
-        "TimeoutInSeconds": int,
-        "PlayerLatencyPolicies": List[PlayerLatencyPolicyTypeDef],
-        "Destinations": List[GameSessionQueueDestinationTypeDef],
-        "FilterConfiguration": FilterConfigurationOutputTypeDef,
-        "PriorityConfiguration": PriorityConfigurationOutputTypeDef,
-        "CustomEventData": str,
-        "NotificationTarget": str,
-    },
-    total=False,
-)
-
-PriorityConfigurationUnionTypeDef = Union[
-    PriorityConfigurationTypeDef, PriorityConfigurationOutputTypeDef
-]
 InstanceAccessTypeDef = TypedDict(
     "InstanceAccessTypeDef",
     {
         "FleetId": str,
         "InstanceId": str,
         "IpAddress": str,
         "OperatingSystem": OperatingSystemType,
@@ -3170,24 +3116,14 @@
         "TargetConfiguration": TargetConfigurationTypeDef,
         "UpdateStatus": Literal["PENDING_UPDATE"],
         "Location": str,
     },
     total=False,
 )
 
-RuntimeConfigurationOutputTypeDef = TypedDict(
-    "RuntimeConfigurationOutputTypeDef",
-    {
-        "ServerProcesses": List[ServerProcessTypeDef],
-        "MaxConcurrentGameSessionActivations": int,
-        "GameSessionActivationTimeoutSeconds": int,
-    },
-    total=False,
-)
-
 RuntimeConfigurationTypeDef = TypedDict(
     "RuntimeConfigurationTypeDef",
     {
         "ServerProcesses": Sequence[ServerProcessTypeDef],
         "MaxConcurrentGameSessionActivations": int,
         "GameSessionActivationTimeoutSeconds": int,
     },
@@ -3237,15 +3173,55 @@
     "UpdateAliasOutputTypeDef",
     {
         "Alias": AliasTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PlayerUnionTypeDef = Union[PlayerTypeDef, PlayerOutputTypeDef]
+_RequiredStartMatchBackfillInputRequestTypeDef = TypedDict(
+    "_RequiredStartMatchBackfillInputRequestTypeDef",
+    {
+        "ConfigurationName": str,
+        "Players": Sequence[PlayerTypeDef],
+    },
+)
+_OptionalStartMatchBackfillInputRequestTypeDef = TypedDict(
+    "_OptionalStartMatchBackfillInputRequestTypeDef",
+    {
+        "TicketId": str,
+        "GameSessionArn": str,
+    },
+    total=False,
+)
+
+class StartMatchBackfillInputRequestTypeDef(
+    _RequiredStartMatchBackfillInputRequestTypeDef, _OptionalStartMatchBackfillInputRequestTypeDef
+):
+    pass
+
+_RequiredStartMatchmakingInputRequestTypeDef = TypedDict(
+    "_RequiredStartMatchmakingInputRequestTypeDef",
+    {
+        "ConfigurationName": str,
+        "Players": Sequence[PlayerTypeDef],
+    },
+)
+_OptionalStartMatchmakingInputRequestTypeDef = TypedDict(
+    "_OptionalStartMatchmakingInputRequestTypeDef",
+    {
+        "TicketId": str,
+    },
+    total=False,
+)
+
+class StartMatchmakingInputRequestTypeDef(
+    _RequiredStartMatchmakingInputRequestTypeDef, _OptionalStartMatchmakingInputRequestTypeDef
+):
+    pass
+
 CreateScriptOutputTypeDef = TypedDict(
     "CreateScriptOutputTypeDef",
     {
         "Script": ScriptTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3425,14 +3401,39 @@
     "UpdateMatchmakingConfigurationOutputTypeDef",
     {
         "Configuration": MatchmakingConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CreateGameSessionQueueOutputTypeDef = TypedDict(
+    "CreateGameSessionQueueOutputTypeDef",
+    {
+        "GameSessionQueue": GameSessionQueueTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeGameSessionQueuesOutputTypeDef = TypedDict(
+    "DescribeGameSessionQueuesOutputTypeDef",
+    {
+        "GameSessionQueues": List[GameSessionQueueTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateGameSessionQueueOutputTypeDef = TypedDict(
+    "UpdateGameSessionQueueOutputTypeDef",
+    {
+        "GameSessionQueue": GameSessionQueueTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeFleetCapacityOutputTypeDef = TypedDict(
     "DescribeFleetCapacityOutputTypeDef",
     {
         "FleetCapacity": List[FleetCapacityTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -3482,15 +3483,15 @@
         "ConfigurationName": str,
         "ConfigurationArn": str,
         "Status": MatchmakingConfigurationStatusType,
         "StatusReason": str,
         "StatusMessage": str,
         "StartTime": datetime,
         "EndTime": datetime,
-        "Players": List[PlayerOutputTypeDef],
+        "Players": List[PlayerTypeDef],
         "GameSessionConnectionInfo": GameSessionConnectionInfoTypeDef,
         "EstimatedWaitTime": int,
     },
     total=False,
 )
 
 DescribeGameSessionPlacementOutputTypeDef = TypedDict(
@@ -3513,39 +3514,14 @@
     "StopGameSessionPlacementOutputTypeDef",
     {
         "GameSessionPlacement": GameSessionPlacementTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateGameSessionQueueOutputTypeDef = TypedDict(
-    "CreateGameSessionQueueOutputTypeDef",
-    {
-        "GameSessionQueue": GameSessionQueueTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeGameSessionQueuesOutputTypeDef = TypedDict(
-    "DescribeGameSessionQueuesOutputTypeDef",
-    {
-        "GameSessionQueues": List[GameSessionQueueTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateGameSessionQueueOutputTypeDef = TypedDict(
-    "UpdateGameSessionQueueOutputTypeDef",
-    {
-        "GameSessionQueue": GameSessionQueueTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 GetInstanceAccessOutputTypeDef = TypedDict(
     "GetInstanceAccessOutputTypeDef",
     {
         "InstanceAccess": InstanceAccessTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3555,30 +3531,14 @@
     {
         "ScalingPolicies": List[ScalingPolicyTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeRuntimeConfigurationOutputTypeDef = TypedDict(
-    "DescribeRuntimeConfigurationOutputTypeDef",
-    {
-        "RuntimeConfiguration": RuntimeConfigurationOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateRuntimeConfigurationOutputTypeDef = TypedDict(
-    "UpdateRuntimeConfigurationOutputTypeDef",
-    {
-        "RuntimeConfiguration": RuntimeConfigurationOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateFleetInputRequestTypeDef = TypedDict(
     "_RequiredCreateFleetInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreateFleetInputRequestTypeDef = TypedDict(
@@ -3610,74 +3570,46 @@
 )
 
 class CreateFleetInputRequestTypeDef(
     _RequiredCreateFleetInputRequestTypeDef, _OptionalCreateFleetInputRequestTypeDef
 ):
     pass
 
-RuntimeConfigurationUnionTypeDef = Union[
-    RuntimeConfigurationTypeDef, RuntimeConfigurationOutputTypeDef
-]
-UpdateRuntimeConfigurationInputRequestTypeDef = TypedDict(
-    "UpdateRuntimeConfigurationInputRequestTypeDef",
+DescribeRuntimeConfigurationOutputTypeDef = TypedDict(
+    "DescribeRuntimeConfigurationOutputTypeDef",
     {
-        "FleetId": str,
         "RuntimeConfiguration": RuntimeConfigurationTypeDef,
-    },
-)
-
-DescribeVpcPeeringConnectionsOutputTypeDef = TypedDict(
-    "DescribeVpcPeeringConnectionsOutputTypeDef",
-    {
-        "VpcPeeringConnections": List[VpcPeeringConnectionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredStartMatchBackfillInputRequestTypeDef = TypedDict(
-    "_RequiredStartMatchBackfillInputRequestTypeDef",
-    {
-        "ConfigurationName": str,
-        "Players": Sequence[PlayerUnionTypeDef],
-    },
-)
-_OptionalStartMatchBackfillInputRequestTypeDef = TypedDict(
-    "_OptionalStartMatchBackfillInputRequestTypeDef",
+UpdateRuntimeConfigurationInputRequestTypeDef = TypedDict(
+    "UpdateRuntimeConfigurationInputRequestTypeDef",
     {
-        "TicketId": str,
-        "GameSessionArn": str,
+        "FleetId": str,
+        "RuntimeConfiguration": RuntimeConfigurationTypeDef,
     },
-    total=False,
 )
 
-class StartMatchBackfillInputRequestTypeDef(
-    _RequiredStartMatchBackfillInputRequestTypeDef, _OptionalStartMatchBackfillInputRequestTypeDef
-):
-    pass
-
-_RequiredStartMatchmakingInputRequestTypeDef = TypedDict(
-    "_RequiredStartMatchmakingInputRequestTypeDef",
+UpdateRuntimeConfigurationOutputTypeDef = TypedDict(
+    "UpdateRuntimeConfigurationOutputTypeDef",
     {
-        "ConfigurationName": str,
-        "Players": Sequence[PlayerUnionTypeDef],
+        "RuntimeConfiguration": RuntimeConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalStartMatchmakingInputRequestTypeDef = TypedDict(
-    "_OptionalStartMatchmakingInputRequestTypeDef",
+
+DescribeVpcPeeringConnectionsOutputTypeDef = TypedDict(
+    "DescribeVpcPeeringConnectionsOutputTypeDef",
     {
-        "TicketId": str,
+        "VpcPeeringConnections": List[VpcPeeringConnectionTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class StartMatchmakingInputRequestTypeDef(
-    _RequiredStartMatchmakingInputRequestTypeDef, _OptionalStartMatchmakingInputRequestTypeDef
-):
-    pass
-
 DescribeGameSessionDetailsOutputTypeDef = TypedDict(
     "DescribeGameSessionDetailsOutputTypeDef",
     {
         "GameSessionDetails": List[GameSessionDetailTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `types-aiobotocore-gamelift-2.5.2.post1/types_aiobotocore_gamelift.egg-info/SOURCES.txt` & `types-aiobotocore-gamelift-2.5.2.post2/types_aiobotocore_gamelift.egg-info/SOURCES.txt`

 * *Files identical despite different names*

