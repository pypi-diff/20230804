# Comparing `tmp/types-aiobotocore-budgets-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-budgets-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-budgets-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:57 2023, max compression
+gzip compressed data, was "types-aiobotocore-budgets-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:30 2023, max compression
```

## Comparing `types-aiobotocore-budgets-2.5.2.post1.tar` & `types-aiobotocore-budgets-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:57.533643 types-aiobotocore-budgets-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:33:54.000000 types-aiobotocore-budgets-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18342 2023-08-02 14:51:57.529643 types-aiobotocore-budgets-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16824 2023-08-02 14:33:54.000000 types-aiobotocore-budgets-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:57.533643 types-aiobotocore-budgets-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-08-02 14:33:53.000000 types-aiobotocore-budgets-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:57.525643 types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets/
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-08-02 14:33:54.000000 types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-08-02 14:33:54.000000 types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-02 14:33:54.000000 types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23698 2023-08-02 14:33:54.000000 types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    23658 2023-08-02 14:33:54.000000 types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10657 2023-08-02 14:33:54.000000 types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10655 2023-08-02 14:33:54.000000 types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11478 2023-08-02 14:33:54.000000 types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11468 2023-08-02 14:33:54.000000 types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:33:54.000000 types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    34558 2023-08-02 14:33:55.000000 types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34503 2023-08-02 14:33:54.000000 types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:33:54.000000 types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:57.529643 types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18342 2023-08-02 14:51:57.000000 types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-02 14:51:57.000000 types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:57.000000 types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:57.000000 types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:57.000000 types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-02 14:51:57.000000 types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:30.907323 types-aiobotocore-budgets-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:41:06.000000 types-aiobotocore-budgets-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14436 2023-08-04 12:00:30.907323 types-aiobotocore-budgets-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12918 2023-08-04 11:41:06.000000 types-aiobotocore-budgets-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:30.911323 types-aiobotocore-budgets-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-08-04 11:41:06.000000 types-aiobotocore-budgets-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:30.907323 types-aiobotocore-budgets-2.5.2.post2/types_aiobotocore_budgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-08-04 11:41:06.000000 types-aiobotocore-budgets-2.5.2.post2/types_aiobotocore_budgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-08-04 11:41:06.000000 types-aiobotocore-budgets-2.5.2.post2/types_aiobotocore_budgets/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-04 11:41:06.000000 types-aiobotocore-budgets-2.5.2.post2/types_aiobotocore_budgets/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23639 2023-08-04 11:41:06.000000 types-aiobotocore-budgets-2.5.2.post2/types_aiobotocore_budgets/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23599 2023-08-04 11:41:06.000000 types-aiobotocore-budgets-2.5.2.post2/types_aiobotocore_budgets/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10657 2023-08-04 11:41:06.000000 types-aiobotocore-budgets-2.5.2.post2/types_aiobotocore_budgets/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10655 2023-08-04 11:41:06.000000 types-aiobotocore-budgets-2.5.2.post2/types_aiobotocore_budgets/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11463 2023-08-04 11:41:06.000000 types-aiobotocore-budgets-2.5.2.post2/types_aiobotocore_budgets/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11453 2023-08-04 11:41:06.000000 types-aiobotocore-budgets-2.5.2.post2/types_aiobotocore_budgets/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:41:06.000000 types-aiobotocore-budgets-2.5.2.post2/types_aiobotocore_budgets/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    31394 2023-08-04 11:41:07.000000 types-aiobotocore-budgets-2.5.2.post2/types_aiobotocore_budgets/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31345 2023-08-04 11:41:07.000000 types-aiobotocore-budgets-2.5.2.post2/types_aiobotocore_budgets/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:41:06.000000 types-aiobotocore-budgets-2.5.2.post2/types_aiobotocore_budgets/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:30.907323 types-aiobotocore-budgets-2.5.2.post2/types_aiobotocore_budgets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14436 2023-08-04 12:00:30.000000 types-aiobotocore-budgets-2.5.2.post2/types_aiobotocore_budgets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-04 12:00:30.000000 types-aiobotocore-budgets-2.5.2.post2/types_aiobotocore_budgets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:30.000000 types-aiobotocore-budgets-2.5.2.post2/types_aiobotocore_budgets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:30.000000 types-aiobotocore-budgets-2.5.2.post2/types_aiobotocore_budgets.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:30.000000 types-aiobotocore-budgets-2.5.2.post2/types_aiobotocore_budgets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-04 12:00:30.000000 types-aiobotocore-budgets-2.5.2.post2/types_aiobotocore_budgets.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-budgets-2.5.2.post1/LICENSE` & `types-aiobotocore-budgets-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-budgets-2.5.2.post1/setup.py` & `types-aiobotocore-budgets-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-budgets",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_budgets"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Budgets 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets/__init__.py` & `types-aiobotocore-budgets-2.5.2.post2/types_aiobotocore_budgets/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets/__init__.pyi` & `types-aiobotocore-budgets-2.5.2.post2/types_aiobotocore_budgets/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets/__main__.py` & `types-aiobotocore-budgets-2.5.2.post2/types_aiobotocore_budgets/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Budgets 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.Budgets 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets\nOther"
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

### Comparing `types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets/client.py` & `types-aiobotocore-budgets-2.5.2.post2/types_aiobotocore_budgets/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,17 +29,17 @@
     DescribeBudgetPerformanceHistoryPaginator,
     DescribeBudgetsPaginator,
     DescribeNotificationsForBudgetPaginator,
     DescribeSubscribersForNotificationPaginator,
 )
 from .type_defs import (
     ActionThresholdTypeDef,
-    BudgetUnionTypeDef,
+    BudgetTypeDef,
     CreateBudgetActionResponseTypeDef,
-    DefinitionUnionTypeDef,
+    DefinitionTypeDef,
     DeleteBudgetActionResponseTypeDef,
     DescribeBudgetActionHistoriesResponseTypeDef,
     DescribeBudgetActionResponseTypeDef,
     DescribeBudgetActionsForAccountResponseTypeDef,
     DescribeBudgetActionsForBudgetResponseTypeDef,
     DescribeBudgetNotificationsForAccountResponseTypeDef,
     DescribeBudgetPerformanceHistoryResponseTypeDef,
@@ -47,15 +47,15 @@
     DescribeBudgetsResponseTypeDef,
     DescribeNotificationsForBudgetResponseTypeDef,
     DescribeSubscribersForNotificationResponseTypeDef,
     ExecuteBudgetActionResponseTypeDef,
     NotificationTypeDef,
     NotificationWithSubscribersTypeDef,
     SubscriberTypeDef,
-    TimePeriodUnionTypeDef,
+    TimePeriodTypeDef,
     UpdateBudgetActionResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -119,15 +119,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/client/#close)
         """
 
     async def create_budget(
         self,
         *,
         AccountId: str,
-        Budget: BudgetUnionTypeDef,
+        Budget: BudgetTypeDef,
         NotificationsWithSubscribers: Sequence[NotificationWithSubscribersTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Creates a budget and, if included, notifications and subscribers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.create_budget)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/client/#create_budget)
@@ -137,15 +137,15 @@
         self,
         *,
         AccountId: str,
         BudgetName: str,
         NotificationType: NotificationTypeType,
         ActionType: ActionTypeType,
         ActionThreshold: ActionThresholdTypeDef,
-        Definition: DefinitionUnionTypeDef,
+        Definition: DefinitionTypeDef,
         ExecutionRoleArn: str,
         ApprovalModel: ApprovalModelType,
         Subscribers: Sequence[SubscriberTypeDef]
     ) -> CreateBudgetActionResponseTypeDef:
         """
         Creates a budget action.
 
@@ -248,15 +248,15 @@
 
     async def describe_budget_action_histories(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         ActionId: str,
-        TimePeriod: TimePeriodUnionTypeDef = ...,
+        TimePeriod: TimePeriodTypeDef = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeBudgetActionHistoriesResponseTypeDef:
         """
         Describes a budget action history detail.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.describe_budget_action_histories)
@@ -294,15 +294,15 @@
         """
 
     async def describe_budget_performance_history(
         self,
         *,
         AccountId: str,
         BudgetName: str,
-        TimePeriod: TimePeriodUnionTypeDef = ...,
+        TimePeriod: TimePeriodTypeDef = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeBudgetPerformanceHistoryResponseTypeDef:
         """
         Describes the history for `DAILY`, `MONTHLY`, and `QUARTERLY` budgets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.describe_budget_performance_history)
@@ -365,17 +365,15 @@
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/client/#generate_presigned_url)
         """
 
-    async def update_budget(
-        self, *, AccountId: str, NewBudget: BudgetUnionTypeDef
-    ) -> Dict[str, Any]:
+    async def update_budget(self, *, AccountId: str, NewBudget: BudgetTypeDef) -> Dict[str, Any]:
         """
         Updates a budget.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.update_budget)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/client/#update_budget)
         """
 
@@ -383,15 +381,15 @@
         self,
         *,
         AccountId: str,
         BudgetName: str,
         ActionId: str,
         NotificationType: NotificationTypeType = ...,
         ActionThreshold: ActionThresholdTypeDef = ...,
-        Definition: DefinitionUnionTypeDef = ...,
+        Definition: DefinitionTypeDef = ...,
         ExecutionRoleArn: str = ...,
         ApprovalModel: ApprovalModelType = ...,
         Subscribers: Sequence[SubscriberTypeDef] = ...
     ) -> UpdateBudgetActionResponseTypeDef:
         """
         Updates a budget action.
```

### Comparing `types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets/client.pyi` & `types-aiobotocore-budgets-2.5.2.post2/types_aiobotocore_budgets/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -29,17 +29,17 @@
     DescribeBudgetPerformanceHistoryPaginator,
     DescribeBudgetsPaginator,
     DescribeNotificationsForBudgetPaginator,
     DescribeSubscribersForNotificationPaginator,
 )
 from .type_defs import (
     ActionThresholdTypeDef,
-    BudgetUnionTypeDef,
+    BudgetTypeDef,
     CreateBudgetActionResponseTypeDef,
-    DefinitionUnionTypeDef,
+    DefinitionTypeDef,
     DeleteBudgetActionResponseTypeDef,
     DescribeBudgetActionHistoriesResponseTypeDef,
     DescribeBudgetActionResponseTypeDef,
     DescribeBudgetActionsForAccountResponseTypeDef,
     DescribeBudgetActionsForBudgetResponseTypeDef,
     DescribeBudgetNotificationsForAccountResponseTypeDef,
     DescribeBudgetPerformanceHistoryResponseTypeDef,
@@ -47,15 +47,15 @@
     DescribeBudgetsResponseTypeDef,
     DescribeNotificationsForBudgetResponseTypeDef,
     DescribeSubscribersForNotificationResponseTypeDef,
     ExecuteBudgetActionResponseTypeDef,
     NotificationTypeDef,
     NotificationWithSubscribersTypeDef,
     SubscriberTypeDef,
-    TimePeriodUnionTypeDef,
+    TimePeriodTypeDef,
     UpdateBudgetActionResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -112,15 +112,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/client/#close)
         """
     async def create_budget(
         self,
         *,
         AccountId: str,
-        Budget: BudgetUnionTypeDef,
+        Budget: BudgetTypeDef,
         NotificationsWithSubscribers: Sequence[NotificationWithSubscribersTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Creates a budget and, if included, notifications and subscribers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.create_budget)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/client/#create_budget)
@@ -129,15 +129,15 @@
         self,
         *,
         AccountId: str,
         BudgetName: str,
         NotificationType: NotificationTypeType,
         ActionType: ActionTypeType,
         ActionThreshold: ActionThresholdTypeDef,
-        Definition: DefinitionUnionTypeDef,
+        Definition: DefinitionTypeDef,
         ExecutionRoleArn: str,
         ApprovalModel: ApprovalModelType,
         Subscribers: Sequence[SubscriberTypeDef]
     ) -> CreateBudgetActionResponseTypeDef:
         """
         Creates a budget action.
 
@@ -231,15 +231,15 @@
         """
     async def describe_budget_action_histories(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         ActionId: str,
-        TimePeriod: TimePeriodUnionTypeDef = ...,
+        TimePeriod: TimePeriodTypeDef = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeBudgetActionHistoriesResponseTypeDef:
         """
         Describes a budget action history detail.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.describe_budget_action_histories)
@@ -273,15 +273,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/client/#describe_budget_notifications_for_account)
         """
     async def describe_budget_performance_history(
         self,
         *,
         AccountId: str,
         BudgetName: str,
-        TimePeriod: TimePeriodUnionTypeDef = ...,
+        TimePeriod: TimePeriodTypeDef = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeBudgetPerformanceHistoryResponseTypeDef:
         """
         Describes the history for `DAILY`, `MONTHLY`, and `QUARTERLY` budgets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.describe_budget_performance_history)
@@ -338,32 +338,30 @@
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/client/#generate_presigned_url)
         """
-    async def update_budget(
-        self, *, AccountId: str, NewBudget: BudgetUnionTypeDef
-    ) -> Dict[str, Any]:
+    async def update_budget(self, *, AccountId: str, NewBudget: BudgetTypeDef) -> Dict[str, Any]:
         """
         Updates a budget.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.update_budget)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/client/#update_budget)
         """
     async def update_budget_action(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         ActionId: str,
         NotificationType: NotificationTypeType = ...,
         ActionThreshold: ActionThresholdTypeDef = ...,
-        Definition: DefinitionUnionTypeDef = ...,
+        Definition: DefinitionTypeDef = ...,
         ExecutionRoleArn: str = ...,
         ApprovalModel: ApprovalModelType = ...,
         Subscribers: Sequence[SubscriberTypeDef] = ...
     ) -> UpdateBudgetActionResponseTypeDef:
         """
         Updates a budget action.
```

### Comparing `types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets/literals.py` & `types-aiobotocore-budgets-2.5.2.post2/types_aiobotocore_budgets/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets/literals.pyi` & `types-aiobotocore-budgets-2.5.2.post2/types_aiobotocore_budgets/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets/paginator.py` & `types-aiobotocore-budgets-2.5.2.post2/types_aiobotocore_budgets/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     DescribeBudgetNotificationsForAccountResponseTypeDef,
     DescribeBudgetPerformanceHistoryResponseTypeDef,
     DescribeBudgetsResponseTypeDef,
     DescribeNotificationsForBudgetResponseTypeDef,
     DescribeSubscribersForNotificationResponseTypeDef,
     NotificationTypeDef,
     PaginatorConfigTypeDef,
-    TimePeriodUnionTypeDef,
+    TimePeriodTypeDef,
 )
 
 __all__ = (
     "DescribeBudgetActionHistoriesPaginator",
     "DescribeBudgetActionsForAccountPaginator",
     "DescribeBudgetActionsForBudgetPaginator",
     "DescribeBudgetNotificationsForAccountPaginator",
@@ -83,15 +83,15 @@
 
     def paginate(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         ActionId: str,
-        TimePeriod: TimePeriodUnionTypeDef = ...,
+        TimePeriod: TimePeriodTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeBudgetActionHistoriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetActionHistories.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/paginators/#describebudgetactionhistoriespaginator)
         """
 
@@ -148,15 +148,15 @@
     """
 
     def paginate(
         self,
         *,
         AccountId: str,
         BudgetName: str,
-        TimePeriod: TimePeriodUnionTypeDef = ...,
+        TimePeriod: TimePeriodTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeBudgetPerformanceHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetPerformanceHistory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/paginators/#describebudgetperformancehistorypaginator)
         """
```

### Comparing `types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets/paginator.pyi` & `types-aiobotocore-budgets-2.5.2.post2/types_aiobotocore_budgets/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     DescribeBudgetNotificationsForAccountResponseTypeDef,
     DescribeBudgetPerformanceHistoryResponseTypeDef,
     DescribeBudgetsResponseTypeDef,
     DescribeNotificationsForBudgetResponseTypeDef,
     DescribeSubscribersForNotificationResponseTypeDef,
     NotificationTypeDef,
     PaginatorConfigTypeDef,
-    TimePeriodUnionTypeDef,
+    TimePeriodTypeDef,
 )
 
 __all__ = (
     "DescribeBudgetActionHistoriesPaginator",
     "DescribeBudgetActionsForAccountPaginator",
     "DescribeBudgetActionsForBudgetPaginator",
     "DescribeBudgetNotificationsForAccountPaginator",
@@ -80,15 +80,15 @@
 
     def paginate(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         ActionId: str,
-        TimePeriod: TimePeriodUnionTypeDef = ...,
+        TimePeriod: TimePeriodTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeBudgetActionHistoriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetActionHistories.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/paginators/#describebudgetactionhistoriespaginator)
         """
 
@@ -141,15 +141,15 @@
     """
 
     def paginate(
         self,
         *,
         AccountId: str,
         BudgetName: str,
-        TimePeriod: TimePeriodUnionTypeDef = ...,
+        TimePeriod: TimePeriodTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeBudgetPerformanceHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetPerformanceHistory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/paginators/#describebudgetperformancehistorypaginator)
         """
```

### Comparing `types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets/type_defs.py` & `types-aiobotocore-budgets-2.5.2.post2/types_aiobotocore_budgets/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,84 +42,74 @@
     "ActionThresholdTypeDef",
     "SubscriberTypeDef",
     "HistoricalOptionsTypeDef",
     "TimestampTypeDef",
     "NotificationTypeDef",
     "CostTypesTypeDef",
     "SpendTypeDef",
-    "TimePeriodOutputTypeDef",
     "ResponseMetadataTypeDef",
-    "IamActionDefinitionOutputTypeDef",
-    "ScpActionDefinitionOutputTypeDef",
-    "SsmActionDefinitionOutputTypeDef",
     "IamActionDefinitionTypeDef",
     "ScpActionDefinitionTypeDef",
     "SsmActionDefinitionTypeDef",
     "DeleteBudgetActionRequestRequestTypeDef",
     "DeleteBudgetRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeBudgetActionRequestRequestTypeDef",
     "DescribeBudgetActionsForAccountRequestRequestTypeDef",
     "DescribeBudgetActionsForBudgetRequestRequestTypeDef",
     "DescribeBudgetNotificationsForAccountRequestRequestTypeDef",
     "DescribeBudgetRequestRequestTypeDef",
     "DescribeBudgetsRequestRequestTypeDef",
     "DescribeNotificationsForBudgetRequestRequestTypeDef",
     "ExecuteBudgetActionRequestRequestTypeDef",
-    "AutoAdjustDataOutputTypeDef",
     "AutoAdjustDataTypeDef",
     "TimePeriodTypeDef",
     "BudgetNotificationsForAccountTypeDef",
     "CreateNotificationRequestRequestTypeDef",
     "CreateSubscriberRequestRequestTypeDef",
     "DeleteNotificationRequestRequestTypeDef",
     "DeleteSubscriberRequestRequestTypeDef",
     "DescribeSubscribersForNotificationRequestRequestTypeDef",
     "NotificationWithSubscribersTypeDef",
     "UpdateNotificationRequestRequestTypeDef",
     "UpdateSubscriberRequestRequestTypeDef",
     "CalculatedSpendTypeDef",
-    "BudgetedAndActualAmountsTypeDef",
     "CreateBudgetActionResponseTypeDef",
     "DescribeNotificationsForBudgetResponseTypeDef",
     "DescribeSubscribersForNotificationResponseTypeDef",
     "ExecuteBudgetActionResponseTypeDef",
-    "DefinitionOutputTypeDef",
     "DefinitionTypeDef",
     "DescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef",
     "DescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef",
     "DescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef",
     "DescribeBudgetsRequestDescribeBudgetsPaginateTypeDef",
     "DescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef",
     "DescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef",
+    "BudgetedAndActualAmountsTypeDef",
     "DescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef",
     "DescribeBudgetActionHistoriesRequestRequestTypeDef",
     "DescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef",
     "DescribeBudgetPerformanceHistoryRequestRequestTypeDef",
-    "TimePeriodUnionTypeDef",
     "DescribeBudgetNotificationsForAccountResponseTypeDef",
-    "BudgetOutputTypeDef",
     "BudgetTypeDef",
-    "BudgetPerformanceHistoryTypeDef",
     "ActionTypeDef",
     "CreateBudgetActionRequestRequestTypeDef",
-    "DefinitionUnionTypeDef",
     "UpdateBudgetActionRequestRequestTypeDef",
+    "BudgetPerformanceHistoryTypeDef",
+    "CreateBudgetRequestRequestTypeDef",
     "DescribeBudgetResponseTypeDef",
     "DescribeBudgetsResponseTypeDef",
-    "BudgetUnionTypeDef",
-    "CreateBudgetRequestRequestTypeDef",
     "UpdateBudgetRequestRequestTypeDef",
-    "DescribeBudgetPerformanceHistoryResponseTypeDef",
     "ActionHistoryDetailsTypeDef",
     "DeleteBudgetActionResponseTypeDef",
     "DescribeBudgetActionResponseTypeDef",
     "DescribeBudgetActionsForAccountResponseTypeDef",
     "DescribeBudgetActionsForBudgetResponseTypeDef",
     "UpdateBudgetActionResponseTypeDef",
+    "DescribeBudgetPerformanceHistoryResponseTypeDef",
     "ActionHistoryTypeDef",
     "DescribeBudgetActionHistoriesResponseTypeDef",
 )
 
 ActionThresholdTypeDef = TypedDict(
     "ActionThresholdTypeDef",
     {
@@ -202,74 +192,25 @@
     "SpendTypeDef",
     {
         "Amount": str,
         "Unit": str,
     },
 )
 
-TimePeriodOutputTypeDef = TypedDict(
-    "TimePeriodOutputTypeDef",
-    {
-        "Start": datetime,
-        "End": datetime,
-    },
-    total=False,
-)
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-_RequiredIamActionDefinitionOutputTypeDef = TypedDict(
-    "_RequiredIamActionDefinitionOutputTypeDef",
-    {
-        "PolicyArn": str,
-    },
-)
-_OptionalIamActionDefinitionOutputTypeDef = TypedDict(
-    "_OptionalIamActionDefinitionOutputTypeDef",
-    {
-        "Roles": List[str],
-        "Groups": List[str],
-        "Users": List[str],
-    },
-    total=False,
-)
-
-
-class IamActionDefinitionOutputTypeDef(
-    _RequiredIamActionDefinitionOutputTypeDef, _OptionalIamActionDefinitionOutputTypeDef
-):
-    pass
-
-
-ScpActionDefinitionOutputTypeDef = TypedDict(
-    "ScpActionDefinitionOutputTypeDef",
-    {
-        "PolicyId": str,
-        "TargetIds": List[str],
-    },
-)
-
-SsmActionDefinitionOutputTypeDef = TypedDict(
-    "SsmActionDefinitionOutputTypeDef",
-    {
-        "ActionSubType": ActionSubTypeType,
-        "Region": str,
-        "InstanceIds": List[str],
-    },
-)
-
 _RequiredIamActionDefinitionTypeDef = TypedDict(
     "_RequiredIamActionDefinitionTypeDef",
     {
         "PolicyArn": str,
     },
 )
 _OptionalIamActionDefinitionTypeDef = TypedDict(
@@ -472,36 +413,14 @@
         "AccountId": str,
         "BudgetName": str,
         "ActionId": str,
         "ExecutionType": ExecutionTypeType,
     },
 )
 
-_RequiredAutoAdjustDataOutputTypeDef = TypedDict(
-    "_RequiredAutoAdjustDataOutputTypeDef",
-    {
-        "AutoAdjustType": AutoAdjustTypeType,
-    },
-)
-_OptionalAutoAdjustDataOutputTypeDef = TypedDict(
-    "_OptionalAutoAdjustDataOutputTypeDef",
-    {
-        "HistoricalOptions": HistoricalOptionsTypeDef,
-        "LastAutoAdjustTime": datetime,
-    },
-    total=False,
-)
-
-
-class AutoAdjustDataOutputTypeDef(
-    _RequiredAutoAdjustDataOutputTypeDef, _OptionalAutoAdjustDataOutputTypeDef
-):
-    pass
-
-
 _RequiredAutoAdjustDataTypeDef = TypedDict(
     "_RequiredAutoAdjustDataTypeDef",
     {
         "AutoAdjustType": AutoAdjustTypeType,
     },
 )
 _OptionalAutoAdjustDataTypeDef = TypedDict(
@@ -644,24 +563,14 @@
 )
 
 
 class CalculatedSpendTypeDef(_RequiredCalculatedSpendTypeDef, _OptionalCalculatedSpendTypeDef):
     pass
 
 
-BudgetedAndActualAmountsTypeDef = TypedDict(
-    "BudgetedAndActualAmountsTypeDef",
-    {
-        "BudgetedAmount": SpendTypeDef,
-        "ActualAmount": SpendTypeDef,
-        "TimePeriod": TimePeriodOutputTypeDef,
-    },
-    total=False,
-)
-
 CreateBudgetActionResponseTypeDef = TypedDict(
     "CreateBudgetActionResponseTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
         "ActionId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -693,24 +602,14 @@
         "BudgetName": str,
         "ActionId": str,
         "ExecutionType": ExecutionTypeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DefinitionOutputTypeDef = TypedDict(
-    "DefinitionOutputTypeDef",
-    {
-        "IamActionDefinition": IamActionDefinitionOutputTypeDef,
-        "ScpActionDefinition": ScpActionDefinitionOutputTypeDef,
-        "SsmActionDefinition": SsmActionDefinitionOutputTypeDef,
-    },
-    total=False,
-)
-
 DefinitionTypeDef = TypedDict(
     "DefinitionTypeDef",
     {
         "IamActionDefinition": IamActionDefinitionTypeDef,
         "ScpActionDefinition": ScpActionDefinitionTypeDef,
         "SsmActionDefinition": SsmActionDefinitionTypeDef,
     },
@@ -849,14 +748,24 @@
 class DescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef(
     _RequiredDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef,
     _OptionalDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef,
 ):
     pass
 
 
+BudgetedAndActualAmountsTypeDef = TypedDict(
+    "BudgetedAndActualAmountsTypeDef",
+    {
+        "BudgetedAmount": SpendTypeDef,
+        "ActualAmount": SpendTypeDef,
+        "TimePeriod": TimePeriodTypeDef,
+    },
+    total=False,
+)
+
 _RequiredDescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef = (
     TypedDict(
         "_RequiredDescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef",
         {
             "AccountId": str,
             "BudgetName": str,
             "ActionId": str,
@@ -953,52 +862,23 @@
 class DescribeBudgetPerformanceHistoryRequestRequestTypeDef(
     _RequiredDescribeBudgetPerformanceHistoryRequestRequestTypeDef,
     _OptionalDescribeBudgetPerformanceHistoryRequestRequestTypeDef,
 ):
     pass
 
 
-TimePeriodUnionTypeDef = Union[TimePeriodTypeDef, TimePeriodOutputTypeDef]
 DescribeBudgetNotificationsForAccountResponseTypeDef = TypedDict(
     "DescribeBudgetNotificationsForAccountResponseTypeDef",
     {
         "BudgetNotificationsForAccount": List[BudgetNotificationsForAccountTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredBudgetOutputTypeDef = TypedDict(
-    "_RequiredBudgetOutputTypeDef",
-    {
-        "BudgetName": str,
-        "TimeUnit": TimeUnitType,
-        "BudgetType": BudgetTypeType,
-    },
-)
-_OptionalBudgetOutputTypeDef = TypedDict(
-    "_OptionalBudgetOutputTypeDef",
-    {
-        "BudgetLimit": SpendTypeDef,
-        "PlannedBudgetLimits": Dict[str, SpendTypeDef],
-        "CostFilters": Dict[str, List[str]],
-        "CostTypes": CostTypesTypeDef,
-        "TimePeriod": TimePeriodOutputTypeDef,
-        "CalculatedSpend": CalculatedSpendTypeDef,
-        "LastUpdatedTime": datetime,
-        "AutoAdjustData": AutoAdjustDataOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class BudgetOutputTypeDef(_RequiredBudgetOutputTypeDef, _OptionalBudgetOutputTypeDef):
-    pass
-
-
 _RequiredBudgetTypeDef = TypedDict(
     "_RequiredBudgetTypeDef",
     {
         "BudgetName": str,
         "TimeUnit": TimeUnitType,
         "BudgetType": BudgetTypeType,
     },
@@ -1019,36 +899,23 @@
 )
 
 
 class BudgetTypeDef(_RequiredBudgetTypeDef, _OptionalBudgetTypeDef):
     pass
 
 
-BudgetPerformanceHistoryTypeDef = TypedDict(
-    "BudgetPerformanceHistoryTypeDef",
-    {
-        "BudgetName": str,
-        "BudgetType": BudgetTypeType,
-        "CostFilters": Dict[str, List[str]],
-        "CostTypes": CostTypesTypeDef,
-        "TimeUnit": TimeUnitType,
-        "BudgetedAndActualAmountsList": List[BudgetedAndActualAmountsTypeDef],
-    },
-    total=False,
-)
-
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
         "ActionId": str,
         "BudgetName": str,
         "NotificationType": NotificationTypeType,
         "ActionType": ActionTypeType,
         "ActionThreshold": ActionThresholdTypeDef,
-        "Definition": DefinitionOutputTypeDef,
+        "Definition": DefinitionTypeDef,
         "ExecutionRoleArn": str,
         "ApprovalModel": ApprovalModelType,
         "Status": ActionStatusType,
         "Subscribers": List[SubscriberTypeDef],
     },
 )
 
@@ -1063,15 +930,14 @@
         "Definition": DefinitionTypeDef,
         "ExecutionRoleArn": str,
         "ApprovalModel": ApprovalModelType,
         "Subscribers": Sequence[SubscriberTypeDef],
     },
 )
 
-DefinitionUnionTypeDef = Union[DefinitionTypeDef, DefinitionOutputTypeDef]
 _RequiredUpdateBudgetActionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateBudgetActionRequestRequestTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
         "ActionId": str,
     },
@@ -1093,32 +959,27 @@
 class UpdateBudgetActionRequestRequestTypeDef(
     _RequiredUpdateBudgetActionRequestRequestTypeDef,
     _OptionalUpdateBudgetActionRequestRequestTypeDef,
 ):
     pass
 
 
-DescribeBudgetResponseTypeDef = TypedDict(
-    "DescribeBudgetResponseTypeDef",
-    {
-        "Budget": BudgetOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeBudgetsResponseTypeDef = TypedDict(
-    "DescribeBudgetsResponseTypeDef",
+BudgetPerformanceHistoryTypeDef = TypedDict(
+    "BudgetPerformanceHistoryTypeDef",
     {
-        "Budgets": List[BudgetOutputTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "BudgetName": str,
+        "BudgetType": BudgetTypeType,
+        "CostFilters": Dict[str, List[str]],
+        "CostTypes": CostTypesTypeDef,
+        "TimeUnit": TimeUnitType,
+        "BudgetedAndActualAmountsList": List[BudgetedAndActualAmountsTypeDef],
     },
+    total=False,
 )
 
-BudgetUnionTypeDef = Union[BudgetTypeDef, BudgetOutputTypeDef]
 _RequiredCreateBudgetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBudgetRequestRequestTypeDef",
     {
         "AccountId": str,
         "Budget": BudgetTypeDef,
     },
 )
@@ -1133,31 +994,39 @@
 
 class CreateBudgetRequestRequestTypeDef(
     _RequiredCreateBudgetRequestRequestTypeDef, _OptionalCreateBudgetRequestRequestTypeDef
 ):
     pass
 
 
-UpdateBudgetRequestRequestTypeDef = TypedDict(
-    "UpdateBudgetRequestRequestTypeDef",
+DescribeBudgetResponseTypeDef = TypedDict(
+    "DescribeBudgetResponseTypeDef",
     {
-        "AccountId": str,
-        "NewBudget": BudgetTypeDef,
+        "Budget": BudgetTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeBudgetPerformanceHistoryResponseTypeDef = TypedDict(
-    "DescribeBudgetPerformanceHistoryResponseTypeDef",
+DescribeBudgetsResponseTypeDef = TypedDict(
+    "DescribeBudgetsResponseTypeDef",
     {
-        "BudgetPerformanceHistory": BudgetPerformanceHistoryTypeDef,
+        "Budgets": List[BudgetTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+UpdateBudgetRequestRequestTypeDef = TypedDict(
+    "UpdateBudgetRequestRequestTypeDef",
+    {
+        "AccountId": str,
+        "NewBudget": BudgetTypeDef,
+    },
+)
+
 ActionHistoryDetailsTypeDef = TypedDict(
     "ActionHistoryDetailsTypeDef",
     {
         "Message": str,
         "Action": ActionTypeDef,
     },
 )
@@ -1207,14 +1076,23 @@
         "BudgetName": str,
         "OldAction": ActionTypeDef,
         "NewAction": ActionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeBudgetPerformanceHistoryResponseTypeDef = TypedDict(
+    "DescribeBudgetPerformanceHistoryResponseTypeDef",
+    {
+        "BudgetPerformanceHistory": BudgetPerformanceHistoryTypeDef,
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ActionHistoryTypeDef = TypedDict(
     "ActionHistoryTypeDef",
     {
         "Timestamp": datetime,
         "Status": ActionStatusType,
         "EventType": EventTypeType,
         "ActionHistoryDetails": ActionHistoryDetailsTypeDef,
```

### Comparing `types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets/type_defs.pyi` & `types-aiobotocore-budgets-2.5.2.post2/types_aiobotocore_budgets/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -41,84 +41,74 @@
     "ActionThresholdTypeDef",
     "SubscriberTypeDef",
     "HistoricalOptionsTypeDef",
     "TimestampTypeDef",
     "NotificationTypeDef",
     "CostTypesTypeDef",
     "SpendTypeDef",
-    "TimePeriodOutputTypeDef",
     "ResponseMetadataTypeDef",
-    "IamActionDefinitionOutputTypeDef",
-    "ScpActionDefinitionOutputTypeDef",
-    "SsmActionDefinitionOutputTypeDef",
     "IamActionDefinitionTypeDef",
     "ScpActionDefinitionTypeDef",
     "SsmActionDefinitionTypeDef",
     "DeleteBudgetActionRequestRequestTypeDef",
     "DeleteBudgetRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeBudgetActionRequestRequestTypeDef",
     "DescribeBudgetActionsForAccountRequestRequestTypeDef",
     "DescribeBudgetActionsForBudgetRequestRequestTypeDef",
     "DescribeBudgetNotificationsForAccountRequestRequestTypeDef",
     "DescribeBudgetRequestRequestTypeDef",
     "DescribeBudgetsRequestRequestTypeDef",
     "DescribeNotificationsForBudgetRequestRequestTypeDef",
     "ExecuteBudgetActionRequestRequestTypeDef",
-    "AutoAdjustDataOutputTypeDef",
     "AutoAdjustDataTypeDef",
     "TimePeriodTypeDef",
     "BudgetNotificationsForAccountTypeDef",
     "CreateNotificationRequestRequestTypeDef",
     "CreateSubscriberRequestRequestTypeDef",
     "DeleteNotificationRequestRequestTypeDef",
     "DeleteSubscriberRequestRequestTypeDef",
     "DescribeSubscribersForNotificationRequestRequestTypeDef",
     "NotificationWithSubscribersTypeDef",
     "UpdateNotificationRequestRequestTypeDef",
     "UpdateSubscriberRequestRequestTypeDef",
     "CalculatedSpendTypeDef",
-    "BudgetedAndActualAmountsTypeDef",
     "CreateBudgetActionResponseTypeDef",
     "DescribeNotificationsForBudgetResponseTypeDef",
     "DescribeSubscribersForNotificationResponseTypeDef",
     "ExecuteBudgetActionResponseTypeDef",
-    "DefinitionOutputTypeDef",
     "DefinitionTypeDef",
     "DescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef",
     "DescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef",
     "DescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef",
     "DescribeBudgetsRequestDescribeBudgetsPaginateTypeDef",
     "DescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef",
     "DescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef",
+    "BudgetedAndActualAmountsTypeDef",
     "DescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef",
     "DescribeBudgetActionHistoriesRequestRequestTypeDef",
     "DescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef",
     "DescribeBudgetPerformanceHistoryRequestRequestTypeDef",
-    "TimePeriodUnionTypeDef",
     "DescribeBudgetNotificationsForAccountResponseTypeDef",
-    "BudgetOutputTypeDef",
     "BudgetTypeDef",
-    "BudgetPerformanceHistoryTypeDef",
     "ActionTypeDef",
     "CreateBudgetActionRequestRequestTypeDef",
-    "DefinitionUnionTypeDef",
     "UpdateBudgetActionRequestRequestTypeDef",
+    "BudgetPerformanceHistoryTypeDef",
+    "CreateBudgetRequestRequestTypeDef",
     "DescribeBudgetResponseTypeDef",
     "DescribeBudgetsResponseTypeDef",
-    "BudgetUnionTypeDef",
-    "CreateBudgetRequestRequestTypeDef",
     "UpdateBudgetRequestRequestTypeDef",
-    "DescribeBudgetPerformanceHistoryResponseTypeDef",
     "ActionHistoryDetailsTypeDef",
     "DeleteBudgetActionResponseTypeDef",
     "DescribeBudgetActionResponseTypeDef",
     "DescribeBudgetActionsForAccountResponseTypeDef",
     "DescribeBudgetActionsForBudgetResponseTypeDef",
     "UpdateBudgetActionResponseTypeDef",
+    "DescribeBudgetPerformanceHistoryResponseTypeDef",
     "ActionHistoryTypeDef",
     "DescribeBudgetActionHistoriesResponseTypeDef",
 )
 
 ActionThresholdTypeDef = TypedDict(
     "ActionThresholdTypeDef",
     {
@@ -197,72 +187,25 @@
     "SpendTypeDef",
     {
         "Amount": str,
         "Unit": str,
     },
 )
 
-TimePeriodOutputTypeDef = TypedDict(
-    "TimePeriodOutputTypeDef",
-    {
-        "Start": datetime,
-        "End": datetime,
-    },
-    total=False,
-)
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-_RequiredIamActionDefinitionOutputTypeDef = TypedDict(
-    "_RequiredIamActionDefinitionOutputTypeDef",
-    {
-        "PolicyArn": str,
-    },
-)
-_OptionalIamActionDefinitionOutputTypeDef = TypedDict(
-    "_OptionalIamActionDefinitionOutputTypeDef",
-    {
-        "Roles": List[str],
-        "Groups": List[str],
-        "Users": List[str],
-    },
-    total=False,
-)
-
-class IamActionDefinitionOutputTypeDef(
-    _RequiredIamActionDefinitionOutputTypeDef, _OptionalIamActionDefinitionOutputTypeDef
-):
-    pass
-
-ScpActionDefinitionOutputTypeDef = TypedDict(
-    "ScpActionDefinitionOutputTypeDef",
-    {
-        "PolicyId": str,
-        "TargetIds": List[str],
-    },
-)
-
-SsmActionDefinitionOutputTypeDef = TypedDict(
-    "SsmActionDefinitionOutputTypeDef",
-    {
-        "ActionSubType": ActionSubTypeType,
-        "Region": str,
-        "InstanceIds": List[str],
-    },
-)
-
 _RequiredIamActionDefinitionTypeDef = TypedDict(
     "_RequiredIamActionDefinitionTypeDef",
     {
         "PolicyArn": str,
     },
 )
 _OptionalIamActionDefinitionTypeDef = TypedDict(
@@ -453,34 +396,14 @@
         "AccountId": str,
         "BudgetName": str,
         "ActionId": str,
         "ExecutionType": ExecutionTypeType,
     },
 )
 
-_RequiredAutoAdjustDataOutputTypeDef = TypedDict(
-    "_RequiredAutoAdjustDataOutputTypeDef",
-    {
-        "AutoAdjustType": AutoAdjustTypeType,
-    },
-)
-_OptionalAutoAdjustDataOutputTypeDef = TypedDict(
-    "_OptionalAutoAdjustDataOutputTypeDef",
-    {
-        "HistoricalOptions": HistoricalOptionsTypeDef,
-        "LastAutoAdjustTime": datetime,
-    },
-    total=False,
-)
-
-class AutoAdjustDataOutputTypeDef(
-    _RequiredAutoAdjustDataOutputTypeDef, _OptionalAutoAdjustDataOutputTypeDef
-):
-    pass
-
 _RequiredAutoAdjustDataTypeDef = TypedDict(
     "_RequiredAutoAdjustDataTypeDef",
     {
         "AutoAdjustType": AutoAdjustTypeType,
     },
 )
 _OptionalAutoAdjustDataTypeDef = TypedDict(
@@ -617,24 +540,14 @@
     },
     total=False,
 )
 
 class CalculatedSpendTypeDef(_RequiredCalculatedSpendTypeDef, _OptionalCalculatedSpendTypeDef):
     pass
 
-BudgetedAndActualAmountsTypeDef = TypedDict(
-    "BudgetedAndActualAmountsTypeDef",
-    {
-        "BudgetedAmount": SpendTypeDef,
-        "ActualAmount": SpendTypeDef,
-        "TimePeriod": TimePeriodOutputTypeDef,
-    },
-    total=False,
-)
-
 CreateBudgetActionResponseTypeDef = TypedDict(
     "CreateBudgetActionResponseTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
         "ActionId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -666,24 +579,14 @@
         "BudgetName": str,
         "ActionId": str,
         "ExecutionType": ExecutionTypeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DefinitionOutputTypeDef = TypedDict(
-    "DefinitionOutputTypeDef",
-    {
-        "IamActionDefinition": IamActionDefinitionOutputTypeDef,
-        "ScpActionDefinition": ScpActionDefinitionOutputTypeDef,
-        "SsmActionDefinition": SsmActionDefinitionOutputTypeDef,
-    },
-    total=False,
-)
-
 DefinitionTypeDef = TypedDict(
     "DefinitionTypeDef",
     {
         "IamActionDefinition": IamActionDefinitionTypeDef,
         "ScpActionDefinition": ScpActionDefinitionTypeDef,
         "SsmActionDefinition": SsmActionDefinitionTypeDef,
     },
@@ -810,14 +713,24 @@
 
 class DescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef(
     _RequiredDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef,
     _OptionalDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef,
 ):
     pass
 
+BudgetedAndActualAmountsTypeDef = TypedDict(
+    "BudgetedAndActualAmountsTypeDef",
+    {
+        "BudgetedAmount": SpendTypeDef,
+        "ActualAmount": SpendTypeDef,
+        "TimePeriod": TimePeriodTypeDef,
+    },
+    total=False,
+)
+
 _RequiredDescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef = (
     TypedDict(
         "_RequiredDescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef",
         {
             "AccountId": str,
             "BudgetName": str,
             "ActionId": str,
@@ -906,50 +819,23 @@
 
 class DescribeBudgetPerformanceHistoryRequestRequestTypeDef(
     _RequiredDescribeBudgetPerformanceHistoryRequestRequestTypeDef,
     _OptionalDescribeBudgetPerformanceHistoryRequestRequestTypeDef,
 ):
     pass
 
-TimePeriodUnionTypeDef = Union[TimePeriodTypeDef, TimePeriodOutputTypeDef]
 DescribeBudgetNotificationsForAccountResponseTypeDef = TypedDict(
     "DescribeBudgetNotificationsForAccountResponseTypeDef",
     {
         "BudgetNotificationsForAccount": List[BudgetNotificationsForAccountTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredBudgetOutputTypeDef = TypedDict(
-    "_RequiredBudgetOutputTypeDef",
-    {
-        "BudgetName": str,
-        "TimeUnit": TimeUnitType,
-        "BudgetType": BudgetTypeType,
-    },
-)
-_OptionalBudgetOutputTypeDef = TypedDict(
-    "_OptionalBudgetOutputTypeDef",
-    {
-        "BudgetLimit": SpendTypeDef,
-        "PlannedBudgetLimits": Dict[str, SpendTypeDef],
-        "CostFilters": Dict[str, List[str]],
-        "CostTypes": CostTypesTypeDef,
-        "TimePeriod": TimePeriodOutputTypeDef,
-        "CalculatedSpend": CalculatedSpendTypeDef,
-        "LastUpdatedTime": datetime,
-        "AutoAdjustData": AutoAdjustDataOutputTypeDef,
-    },
-    total=False,
-)
-
-class BudgetOutputTypeDef(_RequiredBudgetOutputTypeDef, _OptionalBudgetOutputTypeDef):
-    pass
-
 _RequiredBudgetTypeDef = TypedDict(
     "_RequiredBudgetTypeDef",
     {
         "BudgetName": str,
         "TimeUnit": TimeUnitType,
         "BudgetType": BudgetTypeType,
     },
@@ -968,36 +854,23 @@
     },
     total=False,
 )
 
 class BudgetTypeDef(_RequiredBudgetTypeDef, _OptionalBudgetTypeDef):
     pass
 
-BudgetPerformanceHistoryTypeDef = TypedDict(
-    "BudgetPerformanceHistoryTypeDef",
-    {
-        "BudgetName": str,
-        "BudgetType": BudgetTypeType,
-        "CostFilters": Dict[str, List[str]],
-        "CostTypes": CostTypesTypeDef,
-        "TimeUnit": TimeUnitType,
-        "BudgetedAndActualAmountsList": List[BudgetedAndActualAmountsTypeDef],
-    },
-    total=False,
-)
-
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
         "ActionId": str,
         "BudgetName": str,
         "NotificationType": NotificationTypeType,
         "ActionType": ActionTypeType,
         "ActionThreshold": ActionThresholdTypeDef,
-        "Definition": DefinitionOutputTypeDef,
+        "Definition": DefinitionTypeDef,
         "ExecutionRoleArn": str,
         "ApprovalModel": ApprovalModelType,
         "Status": ActionStatusType,
         "Subscribers": List[SubscriberTypeDef],
     },
 )
 
@@ -1012,15 +885,14 @@
         "Definition": DefinitionTypeDef,
         "ExecutionRoleArn": str,
         "ApprovalModel": ApprovalModelType,
         "Subscribers": Sequence[SubscriberTypeDef],
     },
 )
 
-DefinitionUnionTypeDef = Union[DefinitionTypeDef, DefinitionOutputTypeDef]
 _RequiredUpdateBudgetActionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateBudgetActionRequestRequestTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
         "ActionId": str,
     },
@@ -1040,32 +912,27 @@
 
 class UpdateBudgetActionRequestRequestTypeDef(
     _RequiredUpdateBudgetActionRequestRequestTypeDef,
     _OptionalUpdateBudgetActionRequestRequestTypeDef,
 ):
     pass
 
-DescribeBudgetResponseTypeDef = TypedDict(
-    "DescribeBudgetResponseTypeDef",
-    {
-        "Budget": BudgetOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeBudgetsResponseTypeDef = TypedDict(
-    "DescribeBudgetsResponseTypeDef",
+BudgetPerformanceHistoryTypeDef = TypedDict(
+    "BudgetPerformanceHistoryTypeDef",
     {
-        "Budgets": List[BudgetOutputTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "BudgetName": str,
+        "BudgetType": BudgetTypeType,
+        "CostFilters": Dict[str, List[str]],
+        "CostTypes": CostTypesTypeDef,
+        "TimeUnit": TimeUnitType,
+        "BudgetedAndActualAmountsList": List[BudgetedAndActualAmountsTypeDef],
     },
+    total=False,
 )
 
-BudgetUnionTypeDef = Union[BudgetTypeDef, BudgetOutputTypeDef]
 _RequiredCreateBudgetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBudgetRequestRequestTypeDef",
     {
         "AccountId": str,
         "Budget": BudgetTypeDef,
     },
 )
@@ -1078,31 +945,39 @@
 )
 
 class CreateBudgetRequestRequestTypeDef(
     _RequiredCreateBudgetRequestRequestTypeDef, _OptionalCreateBudgetRequestRequestTypeDef
 ):
     pass
 
-UpdateBudgetRequestRequestTypeDef = TypedDict(
-    "UpdateBudgetRequestRequestTypeDef",
+DescribeBudgetResponseTypeDef = TypedDict(
+    "DescribeBudgetResponseTypeDef",
     {
-        "AccountId": str,
-        "NewBudget": BudgetTypeDef,
+        "Budget": BudgetTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeBudgetPerformanceHistoryResponseTypeDef = TypedDict(
-    "DescribeBudgetPerformanceHistoryResponseTypeDef",
+DescribeBudgetsResponseTypeDef = TypedDict(
+    "DescribeBudgetsResponseTypeDef",
     {
-        "BudgetPerformanceHistory": BudgetPerformanceHistoryTypeDef,
+        "Budgets": List[BudgetTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+UpdateBudgetRequestRequestTypeDef = TypedDict(
+    "UpdateBudgetRequestRequestTypeDef",
+    {
+        "AccountId": str,
+        "NewBudget": BudgetTypeDef,
+    },
+)
+
 ActionHistoryDetailsTypeDef = TypedDict(
     "ActionHistoryDetailsTypeDef",
     {
         "Message": str,
         "Action": ActionTypeDef,
     },
 )
@@ -1152,14 +1027,23 @@
         "BudgetName": str,
         "OldAction": ActionTypeDef,
         "NewAction": ActionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeBudgetPerformanceHistoryResponseTypeDef = TypedDict(
+    "DescribeBudgetPerformanceHistoryResponseTypeDef",
+    {
+        "BudgetPerformanceHistory": BudgetPerformanceHistoryTypeDef,
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ActionHistoryTypeDef = TypedDict(
     "ActionHistoryTypeDef",
     {
         "Timestamp": datetime,
         "Status": ActionStatusType,
         "EventType": EventTypeType,
         "ActionHistoryDetails": ActionHistoryDetailsTypeDef,
```

### Comparing `types-aiobotocore-budgets-2.5.2.post1/types_aiobotocore_budgets.egg-info/SOURCES.txt` & `types-aiobotocore-budgets-2.5.2.post2/types_aiobotocore_budgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

