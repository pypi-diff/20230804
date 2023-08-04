# Comparing `tmp/types-aiobotocore-codecommit-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-codecommit-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-codecommit-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:02 2023, max compression
+gzip compressed data, was "types-aiobotocore-codecommit-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:36 2023, max compression
```

## Comparing `types-aiobotocore-codecommit-2.5.2.post1.tar` & `types-aiobotocore-codecommit-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:02.577625 types-aiobotocore-codecommit-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:35:00.000000 types-aiobotocore-codecommit-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23331 2023-08-02 14:52:02.573625 types-aiobotocore-codecommit-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21801 2023-08-02 14:35:00.000000 types-aiobotocore-codecommit-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:02.577625 types-aiobotocore-codecommit-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-02 14:35:00.000000 types-aiobotocore-codecommit-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:02.573625 types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit/
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-08-02 14:35:00.000000 types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-08-02 14:35:00.000000 types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-02 14:35:00.000000 types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    74777 2023-08-02 14:35:01.000000 types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    74684 2023-08-02 14:35:00.000000 types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10915 2023-08-02 14:35:01.000000 types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10913 2023-08-02 14:35:01.000000 types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-08-02 14:35:01.000000 types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9876 2023-08-02 14:35:01.000000 types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:35:00.000000 types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    79510 2023-08-02 14:35:03.000000 types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    79413 2023-08-02 14:35:03.000000 types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:35:00.000000 types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:02.573625 types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23331 2023-08-02 14:52:02.000000 types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-02 14:52:02.000000 types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:02.000000 types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:02.000000 types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:02.000000 types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-02 14:52:02.000000 types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:36.619539 types-aiobotocore-codecommit-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:42:16.000000 types-aiobotocore-codecommit-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14107 2023-08-04 12:00:36.619539 types-aiobotocore-codecommit-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12577 2023-08-04 11:42:16.000000 types-aiobotocore-codecommit-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:36.619539 types-aiobotocore-codecommit-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-04 11:42:15.000000 types-aiobotocore-codecommit-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:36.619539 types-aiobotocore-codecommit-2.5.2.post2/types_aiobotocore_codecommit/
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-08-04 11:42:16.000000 types-aiobotocore-codecommit-2.5.2.post2/types_aiobotocore_codecommit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-08-04 11:42:16.000000 types-aiobotocore-codecommit-2.5.2.post2/types_aiobotocore_codecommit/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-04 11:42:16.000000 types-aiobotocore-codecommit-2.5.2.post2/types_aiobotocore_codecommit/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74762 2023-08-04 11:42:17.000000 types-aiobotocore-codecommit-2.5.2.post2/types_aiobotocore_codecommit/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74669 2023-08-04 11:42:16.000000 types-aiobotocore-codecommit-2.5.2.post2/types_aiobotocore_codecommit/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10915 2023-08-04 11:42:17.000000 types-aiobotocore-codecommit-2.5.2.post2/types_aiobotocore_codecommit/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10913 2023-08-04 11:42:17.000000 types-aiobotocore-codecommit-2.5.2.post2/types_aiobotocore_codecommit/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-08-04 11:42:17.000000 types-aiobotocore-codecommit-2.5.2.post2/types_aiobotocore_codecommit/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9876 2023-08-04 11:42:17.000000 types-aiobotocore-codecommit-2.5.2.post2/types_aiobotocore_codecommit/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:42:16.000000 types-aiobotocore-codecommit-2.5.2.post2/types_aiobotocore_codecommit/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    78763 2023-08-04 11:42:19.000000 types-aiobotocore-codecommit-2.5.2.post2/types_aiobotocore_codecommit/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78668 2023-08-04 11:42:18.000000 types-aiobotocore-codecommit-2.5.2.post2/types_aiobotocore_codecommit/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:42:16.000000 types-aiobotocore-codecommit-2.5.2.post2/types_aiobotocore_codecommit/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:36.619539 types-aiobotocore-codecommit-2.5.2.post2/types_aiobotocore_codecommit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14107 2023-08-04 12:00:36.000000 types-aiobotocore-codecommit-2.5.2.post2/types_aiobotocore_codecommit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-04 12:00:36.000000 types-aiobotocore-codecommit-2.5.2.post2/types_aiobotocore_codecommit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:36.000000 types-aiobotocore-codecommit-2.5.2.post2/types_aiobotocore_codecommit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:36.000000 types-aiobotocore-codecommit-2.5.2.post2/types_aiobotocore_codecommit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:36.000000 types-aiobotocore-codecommit-2.5.2.post2/types_aiobotocore_codecommit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-04 12:00:36.000000 types-aiobotocore-codecommit-2.5.2.post2/types_aiobotocore_codecommit.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-codecommit-2.5.2.post1/LICENSE` & `types-aiobotocore-codecommit-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codecommit-2.5.2.post1/setup.py` & `types-aiobotocore-codecommit-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-codecommit",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_codecommit"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CodeCommit 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit/__init__.py` & `types-aiobotocore-codecommit-2.5.2.post2/types_aiobotocore_codecommit/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit/__init__.pyi` & `types-aiobotocore-codecommit-2.5.2.post2/types_aiobotocore_codecommit/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit/__main__.py` & `types-aiobotocore-codecommit-2.5.2.post2/types_aiobotocore_codecommit/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CodeCommit 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.CodeCommit 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit\nOther"
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

### Comparing `types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit/client.py` & `types-aiobotocore-codecommit-2.5.2.post2/types_aiobotocore_codecommit/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,15 @@
     MergePullRequestByThreeWayOutputTypeDef,
     PostCommentForComparedCommitOutputTypeDef,
     PostCommentForPullRequestOutputTypeDef,
     PostCommentReplyOutputTypeDef,
     PutFileEntryTypeDef,
     PutFileOutputTypeDef,
     PutRepositoryTriggersOutputTypeDef,
-    RepositoryTriggerUnionTypeDef,
+    RepositoryTriggerTypeDef,
     SetFileModeEntryTypeDef,
     TargetTypeDef,
     TestRepositoryTriggersOutputTypeDef,
     UpdateApprovalRuleTemplateContentOutputTypeDef,
     UpdateApprovalRuleTemplateDescriptionOutputTypeDef,
     UpdateApprovalRuleTemplateNameOutputTypeDef,
     UpdateCommentOutputTypeDef,
@@ -1200,15 +1200,15 @@
         generates a commit for the addition in the specified branch.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.put_file)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/client/#put_file)
         """
 
     async def put_repository_triggers(
-        self, *, repositoryName: str, triggers: Sequence[RepositoryTriggerUnionTypeDef]
+        self, *, repositoryName: str, triggers: Sequence[RepositoryTriggerTypeDef]
     ) -> PutRepositoryTriggersOutputTypeDef:
         """
         Replaces all triggers for a repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.put_repository_triggers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/client/#put_repository_triggers)
         """
@@ -1220,15 +1220,15 @@
         Adds or updates tags for a resource in AWS CodeCommit.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/client/#tag_resource)
         """
 
     async def test_repository_triggers(
-        self, *, repositoryName: str, triggers: Sequence[RepositoryTriggerUnionTypeDef]
+        self, *, repositoryName: str, triggers: Sequence[RepositoryTriggerTypeDef]
     ) -> TestRepositoryTriggersOutputTypeDef:
         """
         Tests the functionality of repository triggers by sending information to the
         trigger target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.test_repository_triggers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/client/#test_repository_triggers)
```

### Comparing `types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit/client.pyi` & `types-aiobotocore-codecommit-2.5.2.post2/types_aiobotocore_codecommit/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,15 @@
     MergePullRequestByThreeWayOutputTypeDef,
     PostCommentForComparedCommitOutputTypeDef,
     PostCommentForPullRequestOutputTypeDef,
     PostCommentReplyOutputTypeDef,
     PutFileEntryTypeDef,
     PutFileOutputTypeDef,
     PutRepositoryTriggersOutputTypeDef,
-    RepositoryTriggerUnionTypeDef,
+    RepositoryTriggerTypeDef,
     SetFileModeEntryTypeDef,
     TargetTypeDef,
     TestRepositoryTriggersOutputTypeDef,
     UpdateApprovalRuleTemplateContentOutputTypeDef,
     UpdateApprovalRuleTemplateDescriptionOutputTypeDef,
     UpdateApprovalRuleTemplateNameOutputTypeDef,
     UpdateCommentOutputTypeDef,
@@ -1131,15 +1131,15 @@
         Adds or updates a file in a branch in an AWS CodeCommit repository, and
         generates a commit for the addition in the specified branch.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.put_file)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/client/#put_file)
         """
     async def put_repository_triggers(
-        self, *, repositoryName: str, triggers: Sequence[RepositoryTriggerUnionTypeDef]
+        self, *, repositoryName: str, triggers: Sequence[RepositoryTriggerTypeDef]
     ) -> PutRepositoryTriggersOutputTypeDef:
         """
         Replaces all triggers for a repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.put_repository_triggers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/client/#put_repository_triggers)
         """
@@ -1149,15 +1149,15 @@
         """
         Adds or updates tags for a resource in AWS CodeCommit.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/client/#tag_resource)
         """
     async def test_repository_triggers(
-        self, *, repositoryName: str, triggers: Sequence[RepositoryTriggerUnionTypeDef]
+        self, *, repositoryName: str, triggers: Sequence[RepositoryTriggerTypeDef]
     ) -> TestRepositoryTriggersOutputTypeDef:
         """
         Tests the functionality of repository triggers by sending information to the
         trigger target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.test_repository_triggers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/client/#test_repository_triggers)
```

### Comparing `types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit/literals.py` & `types-aiobotocore-codecommit-2.5.2.post2/types_aiobotocore_codecommit/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit/literals.pyi` & `types-aiobotocore-codecommit-2.5.2.post2/types_aiobotocore_codecommit/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit/paginator.py` & `types-aiobotocore-codecommit-2.5.2.post2/types_aiobotocore_codecommit/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit/paginator.pyi` & `types-aiobotocore-codecommit-2.5.2.post2/types_aiobotocore_codecommit/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit/type_defs.py` & `types-aiobotocore-codecommit-2.5.2.post2/types_aiobotocore_codecommit/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
     "GetMergeConflictsInputRequestTypeDef",
     "GetMergeOptionsInputRequestTypeDef",
     "GetPullRequestApprovalStatesInputRequestTypeDef",
     "GetPullRequestInputRequestTypeDef",
     "GetPullRequestOverrideStateInputRequestTypeDef",
     "GetRepositoryInputRequestTypeDef",
     "GetRepositoryTriggersInputRequestTypeDef",
-    "RepositoryTriggerOutputTypeDef",
+    "RepositoryTriggerTypeDef",
     "ListApprovalRuleTemplatesInputRequestTypeDef",
     "ListAssociatedApprovalRuleTemplatesForRepositoryInputRequestTypeDef",
     "ListBranchesInputRequestTypeDef",
     "ListPullRequestsInputRequestTypeDef",
     "ListRepositoriesForApprovalRuleTemplateInputRequestTypeDef",
     "ListRepositoriesInputRequestTypeDef",
     "RepositoryNameIdPairTypeDef",
@@ -132,15 +132,14 @@
     "PullRequestCreatedEventMetadataTypeDef",
     "PullRequestSourceReferenceUpdatedEventMetadataTypeDef",
     "PullRequestStatusChangedEventMetadataTypeDef",
     "PutCommentReactionInputRequestTypeDef",
     "SourceFileSpecifierTypeDef",
     "ReactionValueFormatsTypeDef",
     "RepositoryTriggerExecutionFailureTypeDef",
-    "RepositoryTriggerTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateApprovalRuleTemplateContentInputRequestTypeDef",
     "UpdateApprovalRuleTemplateDescriptionInputRequestTypeDef",
     "UpdateApprovalRuleTemplateNameInputRequestTypeDef",
     "UpdateCommentInputRequestTypeDef",
     "UpdateDefaultBranchInputRequestTypeDef",
@@ -210,22 +209,23 @@
     "GetDifferencesInputGetDifferencesPaginateTypeDef",
     "ListBranchesInputListBranchesPaginateTypeDef",
     "ListPullRequestsInputListPullRequestsPaginateTypeDef",
     "ListRepositoriesInputListRepositoriesPaginateTypeDef",
     "EvaluatePullRequestApprovalRulesOutputTypeDef",
     "GetFolderOutputTypeDef",
     "GetRepositoryTriggersOutputTypeDef",
+    "PutRepositoryTriggersInputRequestTypeDef",
+    "TestRepositoryTriggersInputRequestTypeDef",
     "ListRepositoriesOutputTypeDef",
     "MergeHunkTypeDef",
     "PullRequestMergedStateChangedEventMetadataTypeDef",
     "PullRequestTargetTypeDef",
     "PutFileEntryTypeDef",
     "ReactionForCommentTypeDef",
     "TestRepositoryTriggersOutputTypeDef",
-    "RepositoryTriggerUnionTypeDef",
     "CreatePullRequestApprovalRuleOutputTypeDef",
     "UpdatePullRequestApprovalRuleContentOutputTypeDef",
     "GetDifferencesOutputTypeDef",
     "ConflictResolutionTypeDef",
     "GetCommentsForComparedCommitOutputTypeDef",
     "GetCommentsForPullRequestOutputTypeDef",
     "BatchGetCommitsOutputTypeDef",
@@ -233,16 +233,14 @@
     "GetMergeConflictsOutputTypeDef",
     "ConflictTypeDef",
     "DescribeMergeConflictsOutputTypeDef",
     "PullRequestEventTypeDef",
     "PullRequestTypeDef",
     "CreateCommitInputRequestTypeDef",
     "GetCommentReactionsOutputTypeDef",
-    "PutRepositoryTriggersInputRequestTypeDef",
-    "TestRepositoryTriggersInputRequestTypeDef",
     "CreateUnreferencedMergeCommitInputRequestTypeDef",
     "MergeBranchesBySquashInputRequestTypeDef",
     "MergeBranchesByThreeWayInputRequestTypeDef",
     "MergePullRequestBySquashInputRequestTypeDef",
     "MergePullRequestByThreeWayInputRequestTypeDef",
     "BatchDescribeMergeConflictsOutputTypeDef",
     "DescribePullRequestEventsOutputTypeDef",
@@ -1155,34 +1153,34 @@
 GetRepositoryTriggersInputRequestTypeDef = TypedDict(
     "GetRepositoryTriggersInputRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 
-_RequiredRepositoryTriggerOutputTypeDef = TypedDict(
-    "_RequiredRepositoryTriggerOutputTypeDef",
+_RequiredRepositoryTriggerTypeDef = TypedDict(
+    "_RequiredRepositoryTriggerTypeDef",
     {
         "name": str,
         "destinationArn": str,
         "events": List[RepositoryTriggerEventEnumType],
     },
 )
-_OptionalRepositoryTriggerOutputTypeDef = TypedDict(
-    "_OptionalRepositoryTriggerOutputTypeDef",
+_OptionalRepositoryTriggerTypeDef = TypedDict(
+    "_OptionalRepositoryTriggerTypeDef",
     {
         "customData": str,
         "branches": List[str],
     },
     total=False,
 )
 
 
-class RepositoryTriggerOutputTypeDef(
-    _RequiredRepositoryTriggerOutputTypeDef, _OptionalRepositoryTriggerOutputTypeDef
+class RepositoryTriggerTypeDef(
+    _RequiredRepositoryTriggerTypeDef, _OptionalRepositoryTriggerTypeDef
 ):
     pass
 
 
 ListApprovalRuleTemplatesInputRequestTypeDef = TypedDict(
     "ListApprovalRuleTemplatesInputRequestTypeDef",
     {
@@ -1496,38 +1494,14 @@
     {
         "trigger": str,
         "failureMessage": str,
     },
     total=False,
 )
 
-_RequiredRepositoryTriggerTypeDef = TypedDict(
-    "_RequiredRepositoryTriggerTypeDef",
-    {
-        "name": str,
-        "destinationArn": str,
-        "events": Sequence[RepositoryTriggerEventEnumType],
-    },
-)
-_OptionalRepositoryTriggerTypeDef = TypedDict(
-    "_OptionalRepositoryTriggerTypeDef",
-    {
-        "customData": str,
-        "branches": Sequence[str],
-    },
-    total=False,
-)
-
-
-class RepositoryTriggerTypeDef(
-    _RequiredRepositoryTriggerTypeDef, _OptionalRepositoryTriggerTypeDef
-):
-    pass
-
-
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -2453,19 +2427,35 @@
     },
 )
 
 GetRepositoryTriggersOutputTypeDef = TypedDict(
     "GetRepositoryTriggersOutputTypeDef",
     {
         "configurationId": str,
-        "triggers": List[RepositoryTriggerOutputTypeDef],
+        "triggers": List[RepositoryTriggerTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+PutRepositoryTriggersInputRequestTypeDef = TypedDict(
+    "PutRepositoryTriggersInputRequestTypeDef",
+    {
+        "repositoryName": str,
+        "triggers": Sequence[RepositoryTriggerTypeDef],
+    },
+)
+
+TestRepositoryTriggersInputRequestTypeDef = TypedDict(
+    "TestRepositoryTriggersInputRequestTypeDef",
+    {
+        "repositoryName": str,
+        "triggers": Sequence[RepositoryTriggerTypeDef],
+    },
+)
+
 ListRepositoriesOutputTypeDef = TypedDict(
     "ListRepositoriesOutputTypeDef",
     {
         "repositories": List[RepositoryNameIdPairTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2542,15 +2532,14 @@
     {
         "successfulExecutions": List[str],
         "failedExecutions": List[RepositoryTriggerExecutionFailureTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RepositoryTriggerUnionTypeDef = Union[RepositoryTriggerTypeDef, RepositoryTriggerOutputTypeDef]
 CreatePullRequestApprovalRuleOutputTypeDef = TypedDict(
     "CreatePullRequestApprovalRuleOutputTypeDef",
     {
         "approvalRule": ApprovalRuleTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2726,30 +2715,14 @@
     {
         "reactionsForComment": List[ReactionForCommentTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutRepositoryTriggersInputRequestTypeDef = TypedDict(
-    "PutRepositoryTriggersInputRequestTypeDef",
-    {
-        "repositoryName": str,
-        "triggers": Sequence[RepositoryTriggerUnionTypeDef],
-    },
-)
-
-TestRepositoryTriggersInputRequestTypeDef = TypedDict(
-    "TestRepositoryTriggersInputRequestTypeDef",
-    {
-        "repositoryName": str,
-        "triggers": Sequence[RepositoryTriggerUnionTypeDef],
-    },
-)
-
 _RequiredCreateUnreferencedMergeCommitInputRequestTypeDef = TypedDict(
     "_RequiredCreateUnreferencedMergeCommitInputRequestTypeDef",
     {
         "repositoryName": str,
         "sourceCommitSpecifier": str,
         "destinationCommitSpecifier": str,
         "mergeOption": MergeOptionTypeEnumType,
```

### Comparing `types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit/type_defs.pyi` & `types-aiobotocore-codecommit-2.5.2.post2/types_aiobotocore_codecommit/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
     "GetMergeConflictsInputRequestTypeDef",
     "GetMergeOptionsInputRequestTypeDef",
     "GetPullRequestApprovalStatesInputRequestTypeDef",
     "GetPullRequestInputRequestTypeDef",
     "GetPullRequestOverrideStateInputRequestTypeDef",
     "GetRepositoryInputRequestTypeDef",
     "GetRepositoryTriggersInputRequestTypeDef",
-    "RepositoryTriggerOutputTypeDef",
+    "RepositoryTriggerTypeDef",
     "ListApprovalRuleTemplatesInputRequestTypeDef",
     "ListAssociatedApprovalRuleTemplatesForRepositoryInputRequestTypeDef",
     "ListBranchesInputRequestTypeDef",
     "ListPullRequestsInputRequestTypeDef",
     "ListRepositoriesForApprovalRuleTemplateInputRequestTypeDef",
     "ListRepositoriesInputRequestTypeDef",
     "RepositoryNameIdPairTypeDef",
@@ -131,15 +131,14 @@
     "PullRequestCreatedEventMetadataTypeDef",
     "PullRequestSourceReferenceUpdatedEventMetadataTypeDef",
     "PullRequestStatusChangedEventMetadataTypeDef",
     "PutCommentReactionInputRequestTypeDef",
     "SourceFileSpecifierTypeDef",
     "ReactionValueFormatsTypeDef",
     "RepositoryTriggerExecutionFailureTypeDef",
-    "RepositoryTriggerTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateApprovalRuleTemplateContentInputRequestTypeDef",
     "UpdateApprovalRuleTemplateDescriptionInputRequestTypeDef",
     "UpdateApprovalRuleTemplateNameInputRequestTypeDef",
     "UpdateCommentInputRequestTypeDef",
     "UpdateDefaultBranchInputRequestTypeDef",
@@ -209,22 +208,23 @@
     "GetDifferencesInputGetDifferencesPaginateTypeDef",
     "ListBranchesInputListBranchesPaginateTypeDef",
     "ListPullRequestsInputListPullRequestsPaginateTypeDef",
     "ListRepositoriesInputListRepositoriesPaginateTypeDef",
     "EvaluatePullRequestApprovalRulesOutputTypeDef",
     "GetFolderOutputTypeDef",
     "GetRepositoryTriggersOutputTypeDef",
+    "PutRepositoryTriggersInputRequestTypeDef",
+    "TestRepositoryTriggersInputRequestTypeDef",
     "ListRepositoriesOutputTypeDef",
     "MergeHunkTypeDef",
     "PullRequestMergedStateChangedEventMetadataTypeDef",
     "PullRequestTargetTypeDef",
     "PutFileEntryTypeDef",
     "ReactionForCommentTypeDef",
     "TestRepositoryTriggersOutputTypeDef",
-    "RepositoryTriggerUnionTypeDef",
     "CreatePullRequestApprovalRuleOutputTypeDef",
     "UpdatePullRequestApprovalRuleContentOutputTypeDef",
     "GetDifferencesOutputTypeDef",
     "ConflictResolutionTypeDef",
     "GetCommentsForComparedCommitOutputTypeDef",
     "GetCommentsForPullRequestOutputTypeDef",
     "BatchGetCommitsOutputTypeDef",
@@ -232,16 +232,14 @@
     "GetMergeConflictsOutputTypeDef",
     "ConflictTypeDef",
     "DescribeMergeConflictsOutputTypeDef",
     "PullRequestEventTypeDef",
     "PullRequestTypeDef",
     "CreateCommitInputRequestTypeDef",
     "GetCommentReactionsOutputTypeDef",
-    "PutRepositoryTriggersInputRequestTypeDef",
-    "TestRepositoryTriggersInputRequestTypeDef",
     "CreateUnreferencedMergeCommitInputRequestTypeDef",
     "MergeBranchesBySquashInputRequestTypeDef",
     "MergeBranchesByThreeWayInputRequestTypeDef",
     "MergePullRequestBySquashInputRequestTypeDef",
     "MergePullRequestByThreeWayInputRequestTypeDef",
     "BatchDescribeMergeConflictsOutputTypeDef",
     "DescribePullRequestEventsOutputTypeDef",
@@ -1122,33 +1120,33 @@
 GetRepositoryTriggersInputRequestTypeDef = TypedDict(
     "GetRepositoryTriggersInputRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 
-_RequiredRepositoryTriggerOutputTypeDef = TypedDict(
-    "_RequiredRepositoryTriggerOutputTypeDef",
+_RequiredRepositoryTriggerTypeDef = TypedDict(
+    "_RequiredRepositoryTriggerTypeDef",
     {
         "name": str,
         "destinationArn": str,
         "events": List[RepositoryTriggerEventEnumType],
     },
 )
-_OptionalRepositoryTriggerOutputTypeDef = TypedDict(
-    "_OptionalRepositoryTriggerOutputTypeDef",
+_OptionalRepositoryTriggerTypeDef = TypedDict(
+    "_OptionalRepositoryTriggerTypeDef",
     {
         "customData": str,
         "branches": List[str],
     },
     total=False,
 )
 
-class RepositoryTriggerOutputTypeDef(
-    _RequiredRepositoryTriggerOutputTypeDef, _OptionalRepositoryTriggerOutputTypeDef
+class RepositoryTriggerTypeDef(
+    _RequiredRepositoryTriggerTypeDef, _OptionalRepositoryTriggerTypeDef
 ):
     pass
 
 ListApprovalRuleTemplatesInputRequestTypeDef = TypedDict(
     "ListApprovalRuleTemplatesInputRequestTypeDef",
     {
         "nextToken": str,
@@ -1443,36 +1441,14 @@
     {
         "trigger": str,
         "failureMessage": str,
     },
     total=False,
 )
 
-_RequiredRepositoryTriggerTypeDef = TypedDict(
-    "_RequiredRepositoryTriggerTypeDef",
-    {
-        "name": str,
-        "destinationArn": str,
-        "events": Sequence[RepositoryTriggerEventEnumType],
-    },
-)
-_OptionalRepositoryTriggerTypeDef = TypedDict(
-    "_OptionalRepositoryTriggerTypeDef",
-    {
-        "customData": str,
-        "branches": Sequence[str],
-    },
-    total=False,
-)
-
-class RepositoryTriggerTypeDef(
-    _RequiredRepositoryTriggerTypeDef, _OptionalRepositoryTriggerTypeDef
-):
-    pass
-
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -2370,19 +2346,35 @@
     },
 )
 
 GetRepositoryTriggersOutputTypeDef = TypedDict(
     "GetRepositoryTriggersOutputTypeDef",
     {
         "configurationId": str,
-        "triggers": List[RepositoryTriggerOutputTypeDef],
+        "triggers": List[RepositoryTriggerTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+PutRepositoryTriggersInputRequestTypeDef = TypedDict(
+    "PutRepositoryTriggersInputRequestTypeDef",
+    {
+        "repositoryName": str,
+        "triggers": Sequence[RepositoryTriggerTypeDef],
+    },
+)
+
+TestRepositoryTriggersInputRequestTypeDef = TypedDict(
+    "TestRepositoryTriggersInputRequestTypeDef",
+    {
+        "repositoryName": str,
+        "triggers": Sequence[RepositoryTriggerTypeDef],
+    },
+)
+
 ListRepositoriesOutputTypeDef = TypedDict(
     "ListRepositoriesOutputTypeDef",
     {
         "repositories": List[RepositoryNameIdPairTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2457,15 +2449,14 @@
     {
         "successfulExecutions": List[str],
         "failedExecutions": List[RepositoryTriggerExecutionFailureTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RepositoryTriggerUnionTypeDef = Union[RepositoryTriggerTypeDef, RepositoryTriggerOutputTypeDef]
 CreatePullRequestApprovalRuleOutputTypeDef = TypedDict(
     "CreatePullRequestApprovalRuleOutputTypeDef",
     {
         "approvalRule": ApprovalRuleTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2639,30 +2630,14 @@
     {
         "reactionsForComment": List[ReactionForCommentTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutRepositoryTriggersInputRequestTypeDef = TypedDict(
-    "PutRepositoryTriggersInputRequestTypeDef",
-    {
-        "repositoryName": str,
-        "triggers": Sequence[RepositoryTriggerUnionTypeDef],
-    },
-)
-
-TestRepositoryTriggersInputRequestTypeDef = TypedDict(
-    "TestRepositoryTriggersInputRequestTypeDef",
-    {
-        "repositoryName": str,
-        "triggers": Sequence[RepositoryTriggerUnionTypeDef],
-    },
-)
-
 _RequiredCreateUnreferencedMergeCommitInputRequestTypeDef = TypedDict(
     "_RequiredCreateUnreferencedMergeCommitInputRequestTypeDef",
     {
         "repositoryName": str,
         "sourceCommitSpecifier": str,
         "destinationCommitSpecifier": str,
         "mergeOption": MergeOptionTypeEnumType,
```

### Comparing `types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit.egg-info/SOURCES.txt` & `types-aiobotocore-codecommit-2.5.2.post2/types_aiobotocore_codecommit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

