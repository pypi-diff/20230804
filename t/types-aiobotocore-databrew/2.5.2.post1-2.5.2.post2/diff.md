# Comparing `tmp/types-aiobotocore-databrew-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-databrew-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-databrew-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:09 2023, max compression
+gzip compressed data, was "types-aiobotocore-databrew-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:43 2023, max compression
```

## Comparing `types-aiobotocore-databrew-2.5.2.post1.tar` & `types-aiobotocore-databrew-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:09.285608 types-aiobotocore-databrew-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:36:02.000000 types-aiobotocore-databrew-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19941 2023-08-02 14:52:09.281608 types-aiobotocore-databrew-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18415 2023-08-02 14:36:02.000000 types-aiobotocore-databrew-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:09.285608 types-aiobotocore-databrew-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-08-02 14:36:02.000000 types-aiobotocore-databrew-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:09.277608 types-aiobotocore-databrew-2.5.2.post1/types_aiobotocore_databrew/
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-08-02 14:36:02.000000 types-aiobotocore-databrew-2.5.2.post1/types_aiobotocore_databrew/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-08-02 14:36:02.000000 types-aiobotocore-databrew-2.5.2.post1/types_aiobotocore_databrew/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-02 14:36:02.000000 types-aiobotocore-databrew-2.5.2.post1/types_aiobotocore_databrew/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36094 2023-08-02 14:36:02.000000 types-aiobotocore-databrew-2.5.2.post1/types_aiobotocore_databrew/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    36033 2023-08-02 14:36:02.000000 types-aiobotocore-databrew-2.5.2.post1/types_aiobotocore_databrew/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10661 2023-08-02 14:36:03.000000 types-aiobotocore-databrew-2.5.2.post1/types_aiobotocore_databrew/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10659 2023-08-02 14:36:03.000000 types-aiobotocore-databrew-2.5.2.post1/types_aiobotocore_databrew/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9525 2023-08-02 14:36:02.000000 types-aiobotocore-databrew-2.5.2.post1/types_aiobotocore_databrew/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9515 2023-08-02 14:36:02.000000 types-aiobotocore-databrew-2.5.2.post1/types_aiobotocore_databrew/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:36:02.000000 types-aiobotocore-databrew-2.5.2.post1/types_aiobotocore_databrew/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    60217 2023-08-02 14:36:04.000000 types-aiobotocore-databrew-2.5.2.post1/types_aiobotocore_databrew/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    60107 2023-08-02 14:36:03.000000 types-aiobotocore-databrew-2.5.2.post1/types_aiobotocore_databrew/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:36:02.000000 types-aiobotocore-databrew-2.5.2.post1/types_aiobotocore_databrew/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:09.281608 types-aiobotocore-databrew-2.5.2.post1/types_aiobotocore_databrew.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19941 2023-08-02 14:52:09.000000 types-aiobotocore-databrew-2.5.2.post1/types_aiobotocore_databrew.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-02 14:52:09.000000 types-aiobotocore-databrew-2.5.2.post1/types_aiobotocore_databrew.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:09.000000 types-aiobotocore-databrew-2.5.2.post1/types_aiobotocore_databrew.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:09.000000 types-aiobotocore-databrew-2.5.2.post1/types_aiobotocore_databrew.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:09.000000 types-aiobotocore-databrew-2.5.2.post1/types_aiobotocore_databrew.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-02 14:52:09.000000 types-aiobotocore-databrew-2.5.2.post1/types_aiobotocore_databrew.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:43.683811 types-aiobotocore-databrew-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:43:22.000000 types-aiobotocore-databrew-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13855 2023-08-04 12:00:43.683811 types-aiobotocore-databrew-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12329 2023-08-04 11:43:22.000000 types-aiobotocore-databrew-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:43.683811 types-aiobotocore-databrew-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-08-04 11:43:21.000000 types-aiobotocore-databrew-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:43.683811 types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew/
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-08-04 11:43:22.000000 types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-08-04 11:43:22.000000 types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-04 11:43:22.000000 types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36017 2023-08-04 11:43:22.000000 types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35956 2023-08-04 11:43:22.000000 types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10661 2023-08-04 11:43:22.000000 types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10659 2023-08-04 11:43:22.000000 types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9525 2023-08-04 11:43:22.000000 types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9515 2023-08-04 11:43:22.000000 types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:43:22.000000 types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    54090 2023-08-04 11:43:23.000000 types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53992 2023-08-04 11:43:23.000000 types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:43:22.000000 types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:43.683811 types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13855 2023-08-04 12:00:43.000000 types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-04 12:00:43.000000 types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:43.000000 types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:43.000000 types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:43.000000 types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-04 12:00:43.000000 types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-databrew-2.5.2.post1/LICENSE` & `types-aiobotocore-databrew-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-databrew-2.5.2.post1/setup.py` & `types-aiobotocore-databrew-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-databrew",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_databrew"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.GlueDataBrew 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-databrew-2.5.2.post1/types_aiobotocore_databrew/__init__.py` & `types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-databrew-2.5.2.post1/types_aiobotocore_databrew/__init__.pyi` & `types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-databrew-2.5.2.post1/types_aiobotocore_databrew/__main__.py` & `types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.GlueDataBrew 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.GlueDataBrew 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_databrew//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew\nOther"
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

### Comparing `types-aiobotocore-databrew-2.5.2.post1/types_aiobotocore_databrew/client.py` & `types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,39 +51,39 @@
     DescribeDatasetResponseTypeDef,
     DescribeJobResponseTypeDef,
     DescribeJobRunResponseTypeDef,
     DescribeProjectResponseTypeDef,
     DescribeRecipeResponseTypeDef,
     DescribeRulesetResponseTypeDef,
     DescribeScheduleResponseTypeDef,
-    FormatOptionsUnionTypeDef,
+    FormatOptionsTypeDef,
     InputTypeDef,
     JobSampleTypeDef,
     ListDatasetsResponseTypeDef,
     ListJobRunsResponseTypeDef,
     ListJobsResponseTypeDef,
     ListProjectsResponseTypeDef,
     ListRecipesResponseTypeDef,
     ListRecipeVersionsResponseTypeDef,
     ListRulesetsResponseTypeDef,
     ListSchedulesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    PathOptionsUnionTypeDef,
-    ProfileConfigurationUnionTypeDef,
+    OutputTypeDef,
+    PathOptionsTypeDef,
+    ProfileConfigurationTypeDef,
     PublishRecipeResponseTypeDef,
     RecipeReferenceTypeDef,
-    RecipeStepUnionTypeDef,
-    RuleUnionTypeDef,
+    RecipeStepTypeDef,
+    RuleTypeDef,
     S3LocationTypeDef,
     SampleTypeDef,
     SendProjectSessionActionResponseTypeDef,
     StartJobRunResponseTypeDef,
     StartProjectSessionResponseTypeDef,
     StopJobRunResponseTypeDef,
-    UnionTypeDef,
     UpdateDatasetResponseTypeDef,
     UpdateProfileJobResponseTypeDef,
     UpdateProjectResponseTypeDef,
     UpdateRecipeJobResponseTypeDef,
     UpdateRecipeResponseTypeDef,
     UpdateRulesetResponseTypeDef,
     UpdateScheduleResponseTypeDef,
@@ -163,16 +163,16 @@
 
     async def create_dataset(
         self,
         *,
         Name: str,
         Input: InputTypeDef,
         Format: InputFormatType = ...,
-        FormatOptions: FormatOptionsUnionTypeDef = ...,
-        PathOptions: PathOptionsUnionTypeDef = ...,
+        FormatOptions: FormatOptionsTypeDef = ...,
+        PathOptions: PathOptionsTypeDef = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateDatasetResponseTypeDef:
         """
         Creates a new DataBrew dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.create_dataset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_databrew/client/#create_dataset)
@@ -186,15 +186,15 @@
         OutputLocation: S3LocationTypeDef,
         RoleArn: str,
         EncryptionKeyArn: str = ...,
         EncryptionMode: EncryptionModeType = ...,
         LogSubscription: LogSubscriptionType = ...,
         MaxCapacity: int = ...,
         MaxRetries: int = ...,
-        Configuration: ProfileConfigurationUnionTypeDef = ...,
+        Configuration: ProfileConfigurationTypeDef = ...,
         ValidationConfigurations: Sequence[ValidationConfigurationTypeDef] = ...,
         Tags: Mapping[str, str] = ...,
         Timeout: int = ...,
         JobSample: JobSampleTypeDef = ...
     ) -> CreateProfileJobResponseTypeDef:
         """
         Creates a new job to analyze a dataset and create its data profile.
@@ -220,15 +220,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_databrew/client/#create_project)
         """
 
     async def create_recipe(
         self,
         *,
         Name: str,
-        Steps: Sequence[RecipeStepUnionTypeDef],
+        Steps: Sequence[RecipeStepTypeDef],
         Description: str = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateRecipeResponseTypeDef:
         """
         Creates a new DataBrew recipe.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.create_recipe)
@@ -242,15 +242,15 @@
         RoleArn: str,
         DatasetName: str = ...,
         EncryptionKeyArn: str = ...,
         EncryptionMode: EncryptionModeType = ...,
         LogSubscription: LogSubscriptionType = ...,
         MaxCapacity: int = ...,
         MaxRetries: int = ...,
-        Outputs: Sequence[UnionTypeDef] = ...,
+        Outputs: Sequence[OutputTypeDef] = ...,
         DataCatalogOutputs: Sequence[DataCatalogOutputTypeDef] = ...,
         DatabaseOutputs: Sequence[DatabaseOutputTypeDef] = ...,
         ProjectName: str = ...,
         RecipeReference: RecipeReferenceTypeDef = ...,
         Tags: Mapping[str, str] = ...,
         Timeout: int = ...
     ) -> CreateRecipeJobResponseTypeDef:
@@ -264,15 +264,15 @@
         """
 
     async def create_ruleset(
         self,
         *,
         Name: str,
         TargetArn: str,
-        Rules: Sequence[RuleUnionTypeDef],
+        Rules: Sequence[RuleTypeDef],
         Description: str = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateRulesetResponseTypeDef:
         """
         Creates a new ruleset that can be used in a profile job to validate the data
         quality of a dataset.
 
@@ -525,15 +525,15 @@
         """
 
     async def send_project_session_action(
         self,
         *,
         Name: str,
         Preview: bool = ...,
-        RecipeStep: RecipeStepUnionTypeDef = ...,
+        RecipeStep: RecipeStepTypeDef = ...,
         StepIndex: int = ...,
         ClientSessionId: str = ...,
         ViewFrame: ViewFrameTypeDef = ...
     ) -> SendProjectSessionActionResponseTypeDef:
         """
         Performs a recipe step within an interactive DataBrew session that's currently
         open.
@@ -588,31 +588,31 @@
 
     async def update_dataset(
         self,
         *,
         Name: str,
         Input: InputTypeDef,
         Format: InputFormatType = ...,
-        FormatOptions: FormatOptionsUnionTypeDef = ...,
-        PathOptions: PathOptionsUnionTypeDef = ...
+        FormatOptions: FormatOptionsTypeDef = ...,
+        PathOptions: PathOptionsTypeDef = ...
     ) -> UpdateDatasetResponseTypeDef:
         """
         Modifies the definition of an existing DataBrew dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.update_dataset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_databrew/client/#update_dataset)
         """
 
     async def update_profile_job(
         self,
         *,
         Name: str,
         OutputLocation: S3LocationTypeDef,
         RoleArn: str,
-        Configuration: ProfileConfigurationUnionTypeDef = ...,
+        Configuration: ProfileConfigurationTypeDef = ...,
         EncryptionKeyArn: str = ...,
         EncryptionMode: EncryptionModeType = ...,
         LogSubscription: LogSubscriptionType = ...,
         MaxCapacity: int = ...,
         MaxRetries: int = ...,
         ValidationConfigurations: Sequence[ValidationConfigurationTypeDef] = ...,
         Timeout: int = ...,
@@ -632,15 +632,15 @@
         Modifies the definition of an existing DataBrew project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.update_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_databrew/client/#update_project)
         """
 
     async def update_recipe(
-        self, *, Name: str, Description: str = ..., Steps: Sequence[RecipeStepUnionTypeDef] = ...
+        self, *, Name: str, Description: str = ..., Steps: Sequence[RecipeStepTypeDef] = ...
     ) -> UpdateRecipeResponseTypeDef:
         """
         Modifies the definition of the `LATEST_WORKING` version of a DataBrew recipe.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.update_recipe)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_databrew/client/#update_recipe)
         """
@@ -651,28 +651,28 @@
         Name: str,
         RoleArn: str,
         EncryptionKeyArn: str = ...,
         EncryptionMode: EncryptionModeType = ...,
         LogSubscription: LogSubscriptionType = ...,
         MaxCapacity: int = ...,
         MaxRetries: int = ...,
-        Outputs: Sequence[UnionTypeDef] = ...,
+        Outputs: Sequence[OutputTypeDef] = ...,
         DataCatalogOutputs: Sequence[DataCatalogOutputTypeDef] = ...,
         DatabaseOutputs: Sequence[DatabaseOutputTypeDef] = ...,
         Timeout: int = ...
     ) -> UpdateRecipeJobResponseTypeDef:
         """
         Modifies the definition of an existing DataBrew recipe job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.update_recipe_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_databrew/client/#update_recipe_job)
         """
 
     async def update_ruleset(
-        self, *, Name: str, Rules: Sequence[RuleUnionTypeDef], Description: str = ...
+        self, *, Name: str, Rules: Sequence[RuleTypeDef], Description: str = ...
     ) -> UpdateRulesetResponseTypeDef:
         """
         Updates specified ruleset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.update_ruleset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_databrew/client/#update_ruleset)
         """
```

### Comparing `types-aiobotocore-databrew-2.5.2.post1/types_aiobotocore_databrew/client.pyi` & `types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -51,39 +51,39 @@
     DescribeDatasetResponseTypeDef,
     DescribeJobResponseTypeDef,
     DescribeJobRunResponseTypeDef,
     DescribeProjectResponseTypeDef,
     DescribeRecipeResponseTypeDef,
     DescribeRulesetResponseTypeDef,
     DescribeScheduleResponseTypeDef,
-    FormatOptionsUnionTypeDef,
+    FormatOptionsTypeDef,
     InputTypeDef,
     JobSampleTypeDef,
     ListDatasetsResponseTypeDef,
     ListJobRunsResponseTypeDef,
     ListJobsResponseTypeDef,
     ListProjectsResponseTypeDef,
     ListRecipesResponseTypeDef,
     ListRecipeVersionsResponseTypeDef,
     ListRulesetsResponseTypeDef,
     ListSchedulesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    PathOptionsUnionTypeDef,
-    ProfileConfigurationUnionTypeDef,
+    OutputTypeDef,
+    PathOptionsTypeDef,
+    ProfileConfigurationTypeDef,
     PublishRecipeResponseTypeDef,
     RecipeReferenceTypeDef,
-    RecipeStepUnionTypeDef,
-    RuleUnionTypeDef,
+    RecipeStepTypeDef,
+    RuleTypeDef,
     S3LocationTypeDef,
     SampleTypeDef,
     SendProjectSessionActionResponseTypeDef,
     StartJobRunResponseTypeDef,
     StartProjectSessionResponseTypeDef,
     StopJobRunResponseTypeDef,
-    UnionTypeDef,
     UpdateDatasetResponseTypeDef,
     UpdateProfileJobResponseTypeDef,
     UpdateProjectResponseTypeDef,
     UpdateRecipeJobResponseTypeDef,
     UpdateRecipeResponseTypeDef,
     UpdateRulesetResponseTypeDef,
     UpdateScheduleResponseTypeDef,
@@ -155,16 +155,16 @@
         """
     async def create_dataset(
         self,
         *,
         Name: str,
         Input: InputTypeDef,
         Format: InputFormatType = ...,
-        FormatOptions: FormatOptionsUnionTypeDef = ...,
-        PathOptions: PathOptionsUnionTypeDef = ...,
+        FormatOptions: FormatOptionsTypeDef = ...,
+        PathOptions: PathOptionsTypeDef = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateDatasetResponseTypeDef:
         """
         Creates a new DataBrew dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.create_dataset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_databrew/client/#create_dataset)
@@ -177,15 +177,15 @@
         OutputLocation: S3LocationTypeDef,
         RoleArn: str,
         EncryptionKeyArn: str = ...,
         EncryptionMode: EncryptionModeType = ...,
         LogSubscription: LogSubscriptionType = ...,
         MaxCapacity: int = ...,
         MaxRetries: int = ...,
-        Configuration: ProfileConfigurationUnionTypeDef = ...,
+        Configuration: ProfileConfigurationTypeDef = ...,
         ValidationConfigurations: Sequence[ValidationConfigurationTypeDef] = ...,
         Tags: Mapping[str, str] = ...,
         Timeout: int = ...,
         JobSample: JobSampleTypeDef = ...
     ) -> CreateProfileJobResponseTypeDef:
         """
         Creates a new job to analyze a dataset and create its data profile.
@@ -209,15 +209,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.create_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_databrew/client/#create_project)
         """
     async def create_recipe(
         self,
         *,
         Name: str,
-        Steps: Sequence[RecipeStepUnionTypeDef],
+        Steps: Sequence[RecipeStepTypeDef],
         Description: str = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateRecipeResponseTypeDef:
         """
         Creates a new DataBrew recipe.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.create_recipe)
@@ -230,15 +230,15 @@
         RoleArn: str,
         DatasetName: str = ...,
         EncryptionKeyArn: str = ...,
         EncryptionMode: EncryptionModeType = ...,
         LogSubscription: LogSubscriptionType = ...,
         MaxCapacity: int = ...,
         MaxRetries: int = ...,
-        Outputs: Sequence[UnionTypeDef] = ...,
+        Outputs: Sequence[OutputTypeDef] = ...,
         DataCatalogOutputs: Sequence[DataCatalogOutputTypeDef] = ...,
         DatabaseOutputs: Sequence[DatabaseOutputTypeDef] = ...,
         ProjectName: str = ...,
         RecipeReference: RecipeReferenceTypeDef = ...,
         Tags: Mapping[str, str] = ...,
         Timeout: int = ...
     ) -> CreateRecipeJobResponseTypeDef:
@@ -251,15 +251,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_databrew/client/#create_recipe_job)
         """
     async def create_ruleset(
         self,
         *,
         Name: str,
         TargetArn: str,
-        Rules: Sequence[RuleUnionTypeDef],
+        Rules: Sequence[RuleTypeDef],
         Description: str = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateRulesetResponseTypeDef:
         """
         Creates a new ruleset that can be used in a profile job to validate the data
         quality of a dataset.
 
@@ -486,15 +486,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_databrew/client/#publish_recipe)
         """
     async def send_project_session_action(
         self,
         *,
         Name: str,
         Preview: bool = ...,
-        RecipeStep: RecipeStepUnionTypeDef = ...,
+        RecipeStep: RecipeStepTypeDef = ...,
         StepIndex: int = ...,
         ClientSessionId: str = ...,
         ViewFrame: ViewFrameTypeDef = ...
     ) -> SendProjectSessionActionResponseTypeDef:
         """
         Performs a recipe step within an interactive DataBrew session that's currently
         open.
@@ -543,30 +543,30 @@
         """
     async def update_dataset(
         self,
         *,
         Name: str,
         Input: InputTypeDef,
         Format: InputFormatType = ...,
-        FormatOptions: FormatOptionsUnionTypeDef = ...,
-        PathOptions: PathOptionsUnionTypeDef = ...
+        FormatOptions: FormatOptionsTypeDef = ...,
+        PathOptions: PathOptionsTypeDef = ...
     ) -> UpdateDatasetResponseTypeDef:
         """
         Modifies the definition of an existing DataBrew dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.update_dataset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_databrew/client/#update_dataset)
         """
     async def update_profile_job(
         self,
         *,
         Name: str,
         OutputLocation: S3LocationTypeDef,
         RoleArn: str,
-        Configuration: ProfileConfigurationUnionTypeDef = ...,
+        Configuration: ProfileConfigurationTypeDef = ...,
         EncryptionKeyArn: str = ...,
         EncryptionMode: EncryptionModeType = ...,
         LogSubscription: LogSubscriptionType = ...,
         MaxCapacity: int = ...,
         MaxRetries: int = ...,
         ValidationConfigurations: Sequence[ValidationConfigurationTypeDef] = ...,
         Timeout: int = ...,
@@ -584,15 +584,15 @@
         """
         Modifies the definition of an existing DataBrew project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.update_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_databrew/client/#update_project)
         """
     async def update_recipe(
-        self, *, Name: str, Description: str = ..., Steps: Sequence[RecipeStepUnionTypeDef] = ...
+        self, *, Name: str, Description: str = ..., Steps: Sequence[RecipeStepTypeDef] = ...
     ) -> UpdateRecipeResponseTypeDef:
         """
         Modifies the definition of the `LATEST_WORKING` version of a DataBrew recipe.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.update_recipe)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_databrew/client/#update_recipe)
         """
@@ -602,27 +602,27 @@
         Name: str,
         RoleArn: str,
         EncryptionKeyArn: str = ...,
         EncryptionMode: EncryptionModeType = ...,
         LogSubscription: LogSubscriptionType = ...,
         MaxCapacity: int = ...,
         MaxRetries: int = ...,
-        Outputs: Sequence[UnionTypeDef] = ...,
+        Outputs: Sequence[OutputTypeDef] = ...,
         DataCatalogOutputs: Sequence[DataCatalogOutputTypeDef] = ...,
         DatabaseOutputs: Sequence[DatabaseOutputTypeDef] = ...,
         Timeout: int = ...
     ) -> UpdateRecipeJobResponseTypeDef:
         """
         Modifies the definition of an existing DataBrew recipe job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.update_recipe_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_databrew/client/#update_recipe_job)
         """
     async def update_ruleset(
-        self, *, Name: str, Rules: Sequence[RuleUnionTypeDef], Description: str = ...
+        self, *, Name: str, Rules: Sequence[RuleTypeDef], Description: str = ...
     ) -> UpdateRulesetResponseTypeDef:
         """
         Updates specified ruleset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.update_ruleset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_databrew/client/#update_ruleset)
         """
```

### Comparing `types-aiobotocore-databrew-2.5.2.post1/types_aiobotocore_databrew/literals.py` & `types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-databrew-2.5.2.post1/types_aiobotocore_databrew/literals.pyi` & `types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-databrew-2.5.2.post1/types_aiobotocore_databrew/paginator.py` & `types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-databrew-2.5.2.post1/types_aiobotocore_databrew/paginator.pyi` & `types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-databrew-2.5.2.post1/types_aiobotocore_databrew/type_defs.py` & `types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 Type annotations for databrew service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_databrew/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_databrew.type_defs import AllowedStatisticsOutputTypeDef
+    from types_aiobotocore_databrew.type_defs import AllowedStatisticsTypeDef
 
-    data: AllowedStatisticsOutputTypeDef = ...
+    data: AllowedStatisticsTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AnalyticsModeType,
     CompressionFormatType,
     EncryptionModeType,
     InputFormatType,
     JobRunStateType,
@@ -39,17 +39,15 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
-    "AllowedStatisticsOutputTypeDef",
     "AllowedStatisticsTypeDef",
     "BatchDeleteRecipeVersionRequestRequestTypeDef",
     "RecipeVersionErrorDetailTypeDef",
     "ResponseMetadataTypeDef",
     "ColumnSelectorTypeDef",
     "ConditionExpressionTypeDef",
     "JobSampleTypeDef",
@@ -57,30 +55,28 @@
     "ValidationConfigurationTypeDef",
     "SampleTypeDef",
     "RecipeReferenceTypeDef",
     "CreateScheduleRequestRequestTypeDef",
     "CsvOptionsTypeDef",
     "CsvOutputOptionsTypeDef",
     "DatetimeOptionsTypeDef",
-    "FilterExpressionOutputTypeDef",
     "FilterExpressionTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
     "DeleteJobRequestRequestTypeDef",
     "DeleteProjectRequestRequestTypeDef",
     "DeleteRecipeVersionRequestRequestTypeDef",
     "DeleteRulesetRequestRequestTypeDef",
     "DeleteScheduleRequestRequestTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
     "DescribeJobRequestRequestTypeDef",
     "DescribeJobRunRequestRequestTypeDef",
     "DescribeProjectRequestRequestTypeDef",
     "DescribeRecipeRequestRequestTypeDef",
     "DescribeRulesetRequestRequestTypeDef",
     "DescribeScheduleRequestRequestTypeDef",
-    "ExcelOptionsOutputTypeDef",
     "ExcelOptionsTypeDef",
     "FilesLimitTypeDef",
     "JsonOptionsTypeDef",
     "MetadataTypeDef",
     "PaginatorConfigTypeDef",
     "ListDatasetsRequestRequestTypeDef",
     "ListJobRunsRequestRequestTypeDef",
@@ -90,27 +86,24 @@
     "ListRecipesRequestRequestTypeDef",
     "ListRulesetsRequestRequestTypeDef",
     "RulesetItemTypeDef",
     "ListSchedulesRequestRequestTypeDef",
     "ScheduleTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "PublishRecipeRequestRequestTypeDef",
-    "RecipeActionOutputTypeDef",
     "RecipeActionTypeDef",
     "ThresholdTypeDef",
     "ViewFrameTypeDef",
     "StartJobRunRequestRequestTypeDef",
     "StartProjectSessionRequestRequestTypeDef",
-    "StatisticOverrideOutputTypeDef",
     "StatisticOverrideTypeDef",
     "StopJobRunRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateScheduleRequestRequestTypeDef",
-    "EntityDetectorConfigurationOutputTypeDef",
     "EntityDetectorConfigurationTypeDef",
     "BatchDeleteRecipeVersionResponseTypeDef",
     "CreateDatasetResponseTypeDef",
     "CreateProfileJobResponseTypeDef",
     "CreateProjectResponseTypeDef",
     "CreateRecipeJobResponseTypeDef",
     "CreateRecipeResponseTypeDef",
@@ -141,85 +134,64 @@
     "DatabaseTableOutputOptionsTypeDef",
     "S3TableOutputOptionsTypeDef",
     "CreateProjectRequestRequestTypeDef",
     "DescribeProjectResponseTypeDef",
     "ProjectTypeDef",
     "UpdateProjectRequestRequestTypeDef",
     "OutputFormatOptionsTypeDef",
-    "DatasetParameterOutputTypeDef",
     "DatasetParameterTypeDef",
-    "FormatOptionsOutputTypeDef",
     "FormatOptionsTypeDef",
     "ListDatasetsRequestListDatasetsPaginateTypeDef",
     "ListJobRunsRequestListJobRunsPaginateTypeDef",
     "ListJobsRequestListJobsPaginateTypeDef",
     "ListProjectsRequestListProjectsPaginateTypeDef",
     "ListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef",
     "ListRecipesRequestListRecipesPaginateTypeDef",
     "ListRulesetsRequestListRulesetsPaginateTypeDef",
     "ListSchedulesRequestListSchedulesPaginateTypeDef",
     "ListRulesetsResponseTypeDef",
     "ListSchedulesResponseTypeDef",
-    "RecipeStepOutputTypeDef",
     "RecipeStepTypeDef",
-    "RuleOutputTypeDef",
     "RuleTypeDef",
-    "StatisticsConfigurationOutputTypeDef",
     "StatisticsConfigurationTypeDef",
     "InputTypeDef",
     "DatabaseOutputTypeDef",
     "DataCatalogOutputTypeDef",
     "ListProjectsResponseTypeDef",
     "OutputTypeDef",
-    "PathOptionsOutputTypeDef",
     "PathOptionsTypeDef",
-    "FormatOptionsUnionTypeDef",
+    "CreateRecipeRequestRequestTypeDef",
     "DescribeRecipeResponseTypeDef",
     "RecipeTypeDef",
-    "RecipeStepUnionTypeDef",
     "SendProjectSessionActionRequestRequestTypeDef",
+    "UpdateRecipeRequestRequestTypeDef",
+    "CreateRulesetRequestRequestTypeDef",
     "DescribeRulesetResponseTypeDef",
-    "RuleUnionTypeDef",
-    "ColumnStatisticsConfigurationOutputTypeDef",
+    "UpdateRulesetRequestRequestTypeDef",
     "ColumnStatisticsConfigurationTypeDef",
+    "CreateRecipeJobRequestRequestTypeDef",
     "JobRunTypeDef",
     "JobTypeDef",
-    "UnionTypeDef",
+    "UpdateRecipeJobRequestRequestTypeDef",
+    "CreateDatasetRequestRequestTypeDef",
     "DatasetTypeDef",
     "DescribeDatasetResponseTypeDef",
-    "CreateDatasetRequestRequestTypeDef",
-    "PathOptionsUnionTypeDef",
     "UpdateDatasetRequestRequestTypeDef",
     "ListRecipeVersionsResponseTypeDef",
     "ListRecipesResponseTypeDef",
-    "CreateRecipeRequestRequestTypeDef",
-    "UpdateRecipeRequestRequestTypeDef",
-    "CreateRulesetRequestRequestTypeDef",
-    "UpdateRulesetRequestRequestTypeDef",
-    "ProfileConfigurationOutputTypeDef",
     "ProfileConfigurationTypeDef",
     "ListJobRunsResponseTypeDef",
     "ListJobsResponseTypeDef",
-    "CreateRecipeJobRequestRequestTypeDef",
-    "UpdateRecipeJobRequestRequestTypeDef",
     "ListDatasetsResponseTypeDef",
+    "CreateProfileJobRequestRequestTypeDef",
     "DescribeJobResponseTypeDef",
     "DescribeJobRunResponseTypeDef",
-    "CreateProfileJobRequestRequestTypeDef",
-    "ProfileConfigurationUnionTypeDef",
     "UpdateProfileJobRequestRequestTypeDef",
 )
 
-AllowedStatisticsOutputTypeDef = TypedDict(
-    "AllowedStatisticsOutputTypeDef",
-    {
-        "Statistics": List[str],
-    },
-)
-
 AllowedStatisticsTypeDef = TypedDict(
     "AllowedStatisticsTypeDef",
     {
         "Statistics": Sequence[str],
     },
 )
 
@@ -272,21 +244,19 @@
     "_OptionalConditionExpressionTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
-
 class ConditionExpressionTypeDef(
     _RequiredConditionExpressionTypeDef, _OptionalConditionExpressionTypeDef
 ):
     pass
 
-
 JobSampleTypeDef = TypedDict(
     "JobSampleTypeDef",
     {
         "Mode": SampleModeType,
         "Size": int,
     },
     total=False,
@@ -303,78 +273,70 @@
     {
         "Key": str,
         "BucketOwner": str,
     },
     total=False,
 )
 
-
 class S3LocationTypeDef(_RequiredS3LocationTypeDef, _OptionalS3LocationTypeDef):
     pass
 
-
 _RequiredValidationConfigurationTypeDef = TypedDict(
     "_RequiredValidationConfigurationTypeDef",
     {
         "RulesetArn": str,
     },
 )
 _OptionalValidationConfigurationTypeDef = TypedDict(
     "_OptionalValidationConfigurationTypeDef",
     {
         "ValidationMode": Literal["CHECK_ALL"],
     },
     total=False,
 )
 
-
 class ValidationConfigurationTypeDef(
     _RequiredValidationConfigurationTypeDef, _OptionalValidationConfigurationTypeDef
 ):
     pass
 
-
 _RequiredSampleTypeDef = TypedDict(
     "_RequiredSampleTypeDef",
     {
         "Type": SampleTypeType,
     },
 )
 _OptionalSampleTypeDef = TypedDict(
     "_OptionalSampleTypeDef",
     {
         "Size": int,
     },
     total=False,
 )
 
-
 class SampleTypeDef(_RequiredSampleTypeDef, _OptionalSampleTypeDef):
     pass
 
-
 _RequiredRecipeReferenceTypeDef = TypedDict(
     "_RequiredRecipeReferenceTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalRecipeReferenceTypeDef = TypedDict(
     "_OptionalRecipeReferenceTypeDef",
     {
         "RecipeVersion": str,
     },
     total=False,
 )
 
-
 class RecipeReferenceTypeDef(_RequiredRecipeReferenceTypeDef, _OptionalRecipeReferenceTypeDef):
     pass
 
-
 _RequiredCreateScheduleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateScheduleRequestRequestTypeDef",
     {
         "CronExpression": str,
         "Name": str,
     },
 )
@@ -383,21 +345,19 @@
     {
         "JobNames": Sequence[str],
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateScheduleRequestRequestTypeDef(
     _RequiredCreateScheduleRequestRequestTypeDef, _OptionalCreateScheduleRequestRequestTypeDef
 ):
     pass
 
-
 CsvOptionsTypeDef = TypedDict(
     "CsvOptionsTypeDef",
     {
         "Delimiter": str,
         "HeaderRow": bool,
     },
     total=False,
@@ -422,27 +382,17 @@
     {
         "TimezoneOffset": str,
         "LocaleCode": str,
     },
     total=False,
 )
 
-
 class DatetimeOptionsTypeDef(_RequiredDatetimeOptionsTypeDef, _OptionalDatetimeOptionsTypeDef):
     pass
 
-
-FilterExpressionOutputTypeDef = TypedDict(
-    "FilterExpressionOutputTypeDef",
-    {
-        "Expression": str,
-        "ValuesMap": Dict[str, str],
-    },
-)
-
 FilterExpressionTypeDef = TypedDict(
     "FilterExpressionTypeDef",
     {
         "Expression": str,
         "ValuesMap": Mapping[str, str],
     },
 )
@@ -529,45 +479,33 @@
     "_OptionalDescribeRecipeRequestRequestTypeDef",
     {
         "RecipeVersion": str,
     },
     total=False,
 )
 
-
 class DescribeRecipeRequestRequestTypeDef(
     _RequiredDescribeRecipeRequestRequestTypeDef, _OptionalDescribeRecipeRequestRequestTypeDef
 ):
     pass
 
-
 DescribeRulesetRequestRequestTypeDef = TypedDict(
     "DescribeRulesetRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
 DescribeScheduleRequestRequestTypeDef = TypedDict(
     "DescribeScheduleRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-ExcelOptionsOutputTypeDef = TypedDict(
-    "ExcelOptionsOutputTypeDef",
-    {
-        "SheetNames": List[str],
-        "SheetIndexes": List[int],
-        "HeaderRow": bool,
-    },
-    total=False,
-)
-
 ExcelOptionsTypeDef = TypedDict(
     "ExcelOptionsTypeDef",
     {
         "SheetNames": Sequence[str],
         "SheetIndexes": Sequence[int],
         "HeaderRow": bool,
     },
@@ -585,19 +523,17 @@
     {
         "OrderedBy": Literal["LAST_MODIFIED_DATE"],
         "Order": OrderType,
     },
     total=False,
 )
 
-
 class FilesLimitTypeDef(_RequiredFilesLimitTypeDef, _OptionalFilesLimitTypeDef):
     pass
 
-
 JsonOptionsTypeDef = TypedDict(
     "JsonOptionsTypeDef",
     {
         "MultiLine": bool,
     },
     total=False,
 )
@@ -640,21 +576,19 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListJobRunsRequestRequestTypeDef(
     _RequiredListJobRunsRequestRequestTypeDef, _OptionalListJobRunsRequestRequestTypeDef
 ):
     pass
 
-
 ListJobsRequestRequestTypeDef = TypedDict(
     "ListJobsRequestRequestTypeDef",
     {
         "DatasetName": str,
         "MaxResults": int,
         "NextToken": str,
         "ProjectName": str,
@@ -682,22 +616,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListRecipeVersionsRequestRequestTypeDef(
     _RequiredListRecipeVersionsRequestRequestTypeDef,
     _OptionalListRecipeVersionsRequestRequestTypeDef,
 ):
     pass
 
-
 ListRecipesRequestRequestTypeDef = TypedDict(
     "ListRecipesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "RecipeVersion": str,
     },
@@ -733,19 +665,17 @@
         "ResourceArn": str,
         "RuleCount": int,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
-
 class RulesetItemTypeDef(_RequiredRulesetItemTypeDef, _OptionalRulesetItemTypeDef):
     pass
 
-
 ListSchedulesRequestRequestTypeDef = TypedDict(
     "ListSchedulesRequestRequestTypeDef",
     {
         "JobName": str,
         "MaxResults": int,
         "NextToken": str,
     },
@@ -770,19 +700,17 @@
         "ResourceArn": str,
         "CronExpression": str,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
-
 class ScheduleTypeDef(_RequiredScheduleTypeDef, _OptionalScheduleTypeDef):
     pass
 
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
@@ -796,61 +724,36 @@
     "_OptionalPublishRecipeRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class PublishRecipeRequestRequestTypeDef(
     _RequiredPublishRecipeRequestRequestTypeDef, _OptionalPublishRecipeRequestRequestTypeDef
 ):
     pass
 
-
-_RequiredRecipeActionOutputTypeDef = TypedDict(
-    "_RequiredRecipeActionOutputTypeDef",
-    {
-        "Operation": str,
-    },
-)
-_OptionalRecipeActionOutputTypeDef = TypedDict(
-    "_OptionalRecipeActionOutputTypeDef",
-    {
-        "Parameters": Dict[str, str],
-    },
-    total=False,
-)
-
-
-class RecipeActionOutputTypeDef(
-    _RequiredRecipeActionOutputTypeDef, _OptionalRecipeActionOutputTypeDef
-):
-    pass
-
-
 _RequiredRecipeActionTypeDef = TypedDict(
     "_RequiredRecipeActionTypeDef",
     {
         "Operation": str,
     },
 )
 _OptionalRecipeActionTypeDef = TypedDict(
     "_OptionalRecipeActionTypeDef",
     {
         "Parameters": Mapping[str, str],
     },
     total=False,
 )
 
-
 class RecipeActionTypeDef(_RequiredRecipeActionTypeDef, _OptionalRecipeActionTypeDef):
     pass
 
-
 _RequiredThresholdTypeDef = TypedDict(
     "_RequiredThresholdTypeDef",
     {
         "Value": float,
     },
 )
 _OptionalThresholdTypeDef = TypedDict(
@@ -858,19 +761,17 @@
     {
         "Type": ThresholdTypeType,
         "Unit": ThresholdUnitType,
     },
     total=False,
 )
 
-
 class ThresholdTypeDef(_RequiredThresholdTypeDef, _OptionalThresholdTypeDef):
     pass
 
-
 _RequiredViewFrameTypeDef = TypedDict(
     "_RequiredViewFrameTypeDef",
     {
         "StartColumnIndex": int,
     },
 )
 _OptionalViewFrameTypeDef = TypedDict(
@@ -881,19 +782,17 @@
         "StartRowIndex": int,
         "RowRange": int,
         "Analytics": AnalyticsModeType,
     },
     total=False,
 )
 
-
 class ViewFrameTypeDef(_RequiredViewFrameTypeDef, _OptionalViewFrameTypeDef):
     pass
 
-
 StartJobRunRequestRequestTypeDef = TypedDict(
     "StartJobRunRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -907,30 +806,20 @@
     "_OptionalStartProjectSessionRequestRequestTypeDef",
     {
         "AssumeControl": bool,
     },
     total=False,
 )
 
-
 class StartProjectSessionRequestRequestTypeDef(
     _RequiredStartProjectSessionRequestRequestTypeDef,
     _OptionalStartProjectSessionRequestRequestTypeDef,
 ):
     pass
 
-
-StatisticOverrideOutputTypeDef = TypedDict(
-    "StatisticOverrideOutputTypeDef",
-    {
-        "Statistic": str,
-        "Parameters": Dict[str, str],
-    },
-)
-
 StatisticOverrideTypeDef = TypedDict(
     "StatisticOverrideTypeDef",
     {
         "Statistic": str,
         "Parameters": Mapping[str, str],
     },
 )
@@ -970,64 +859,38 @@
     "_OptionalUpdateScheduleRequestRequestTypeDef",
     {
         "JobNames": Sequence[str],
     },
     total=False,
 )
 
-
 class UpdateScheduleRequestRequestTypeDef(
     _RequiredUpdateScheduleRequestRequestTypeDef, _OptionalUpdateScheduleRequestRequestTypeDef
 ):
     pass
 
-
-_RequiredEntityDetectorConfigurationOutputTypeDef = TypedDict(
-    "_RequiredEntityDetectorConfigurationOutputTypeDef",
-    {
-        "EntityTypes": List[str],
-    },
-)
-_OptionalEntityDetectorConfigurationOutputTypeDef = TypedDict(
-    "_OptionalEntityDetectorConfigurationOutputTypeDef",
-    {
-        "AllowedStatistics": List[AllowedStatisticsOutputTypeDef],
-    },
-    total=False,
-)
-
-
-class EntityDetectorConfigurationOutputTypeDef(
-    _RequiredEntityDetectorConfigurationOutputTypeDef,
-    _OptionalEntityDetectorConfigurationOutputTypeDef,
-):
-    pass
-
-
 _RequiredEntityDetectorConfigurationTypeDef = TypedDict(
     "_RequiredEntityDetectorConfigurationTypeDef",
     {
         "EntityTypes": Sequence[str],
     },
 )
 _OptionalEntityDetectorConfigurationTypeDef = TypedDict(
     "_OptionalEntityDetectorConfigurationTypeDef",
     {
         "AllowedStatistics": Sequence[AllowedStatisticsTypeDef],
     },
     total=False,
 )
 
-
 class EntityDetectorConfigurationTypeDef(
     _RequiredEntityDetectorConfigurationTypeDef, _OptionalEntityDetectorConfigurationTypeDef
 ):
     pass
 
-
 BatchDeleteRecipeVersionResponseTypeDef = TypedDict(
     "BatchDeleteRecipeVersionResponseTypeDef",
     {
         "Name": str,
         "Errors": List[RecipeVersionErrorDetailTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1274,21 +1137,19 @@
     {
         "CatalogId": str,
         "TempDirectory": S3LocationTypeDef,
     },
     total=False,
 )
 
-
 class DataCatalogInputDefinitionTypeDef(
     _RequiredDataCatalogInputDefinitionTypeDef, _OptionalDataCatalogInputDefinitionTypeDef
 ):
     pass
 
-
 _RequiredDatabaseInputDefinitionTypeDef = TypedDict(
     "_RequiredDatabaseInputDefinitionTypeDef",
     {
         "GlueConnectionName": str,
     },
 )
 _OptionalDatabaseInputDefinitionTypeDef = TypedDict(
@@ -1297,42 +1158,38 @@
         "DatabaseTableName": str,
         "TempDirectory": S3LocationTypeDef,
         "QueryString": str,
     },
     total=False,
 )
 
-
 class DatabaseInputDefinitionTypeDef(
     _RequiredDatabaseInputDefinitionTypeDef, _OptionalDatabaseInputDefinitionTypeDef
 ):
     pass
 
-
 _RequiredDatabaseTableOutputOptionsTypeDef = TypedDict(
     "_RequiredDatabaseTableOutputOptionsTypeDef",
     {
         "TableName": str,
     },
 )
 _OptionalDatabaseTableOutputOptionsTypeDef = TypedDict(
     "_OptionalDatabaseTableOutputOptionsTypeDef",
     {
         "TempDirectory": S3LocationTypeDef,
     },
     total=False,
 )
 
-
 class DatabaseTableOutputOptionsTypeDef(
     _RequiredDatabaseTableOutputOptionsTypeDef, _OptionalDatabaseTableOutputOptionsTypeDef
 ):
     pass
 
-
 S3TableOutputOptionsTypeDef = TypedDict(
     "S3TableOutputOptionsTypeDef",
     {
         "Location": S3LocationTypeDef,
     },
 )
 
@@ -1350,21 +1207,19 @@
     {
         "Sample": SampleTypeDef,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateProjectRequestRequestTypeDef(
     _RequiredCreateProjectRequestRequestTypeDef, _OptionalCreateProjectRequestRequestTypeDef
 ):
     pass
 
-
 DescribeProjectResponseTypeDef = TypedDict(
     "DescribeProjectResponseTypeDef",
     {
         "CreateDate": datetime,
         "CreatedBy": str,
         "DatasetName": str,
         "LastModifiedDate": datetime,
@@ -1404,19 +1259,17 @@
         "RoleArn": str,
         "OpenedBy": str,
         "OpenDate": datetime,
     },
     total=False,
 )
 
-
 class ProjectTypeDef(_RequiredProjectTypeDef, _OptionalProjectTypeDef):
     pass
 
-
 _RequiredUpdateProjectRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateProjectRequestRequestTypeDef",
     {
         "RoleArn": str,
         "Name": str,
     },
 )
@@ -1424,53 +1277,27 @@
     "_OptionalUpdateProjectRequestRequestTypeDef",
     {
         "Sample": SampleTypeDef,
     },
     total=False,
 )
 
-
 class UpdateProjectRequestRequestTypeDef(
     _RequiredUpdateProjectRequestRequestTypeDef, _OptionalUpdateProjectRequestRequestTypeDef
 ):
     pass
 
-
 OutputFormatOptionsTypeDef = TypedDict(
     "OutputFormatOptionsTypeDef",
     {
         "Csv": CsvOutputOptionsTypeDef,
     },
     total=False,
 )
 
-_RequiredDatasetParameterOutputTypeDef = TypedDict(
-    "_RequiredDatasetParameterOutputTypeDef",
-    {
-        "Name": str,
-        "Type": ParameterTypeType,
-    },
-)
-_OptionalDatasetParameterOutputTypeDef = TypedDict(
-    "_OptionalDatasetParameterOutputTypeDef",
-    {
-        "DatetimeOptions": DatetimeOptionsTypeDef,
-        "CreateColumn": bool,
-        "Filter": FilterExpressionOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class DatasetParameterOutputTypeDef(
-    _RequiredDatasetParameterOutputTypeDef, _OptionalDatasetParameterOutputTypeDef
-):
-    pass
-
-
 _RequiredDatasetParameterTypeDef = TypedDict(
     "_RequiredDatasetParameterTypeDef",
     {
         "Name": str,
         "Type": ParameterTypeType,
     },
 )
@@ -1480,29 +1307,17 @@
         "DatetimeOptions": DatetimeOptionsTypeDef,
         "CreateColumn": bool,
         "Filter": FilterExpressionTypeDef,
     },
     total=False,
 )
 
-
 class DatasetParameterTypeDef(_RequiredDatasetParameterTypeDef, _OptionalDatasetParameterTypeDef):
     pass
 
-
-FormatOptionsOutputTypeDef = TypedDict(
-    "FormatOptionsOutputTypeDef",
-    {
-        "Json": JsonOptionsTypeDef,
-        "Excel": ExcelOptionsOutputTypeDef,
-        "Csv": CsvOptionsTypeDef,
-    },
-    total=False,
-)
-
 FormatOptionsTypeDef = TypedDict(
     "FormatOptionsTypeDef",
     {
         "Json": JsonOptionsTypeDef,
         "Excel": ExcelOptionsTypeDef,
         "Csv": CsvOptionsTypeDef,
     },
@@ -1527,22 +1342,20 @@
     "_OptionalListJobRunsRequestListJobRunsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListJobRunsRequestListJobRunsPaginateTypeDef(
     _RequiredListJobRunsRequestListJobRunsPaginateTypeDef,
     _OptionalListJobRunsRequestListJobRunsPaginateTypeDef,
 ):
     pass
 
-
 ListJobsRequestListJobsPaginateTypeDef = TypedDict(
     "ListJobsRequestListJobsPaginateTypeDef",
     {
         "DatasetName": str,
         "ProjectName": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -1567,22 +1380,20 @@
     "_OptionalListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef(
     _RequiredListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef,
     _OptionalListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef,
 ):
     pass
 
-
 ListRecipesRequestListRecipesPaginateTypeDef = TypedDict(
     "ListRecipesRequestListRecipesPaginateTypeDef",
     {
         "RecipeVersion": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -1620,75 +1431,31 @@
     {
         "Schedules": List[ScheduleTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredRecipeStepOutputTypeDef = TypedDict(
-    "_RequiredRecipeStepOutputTypeDef",
-    {
-        "Action": RecipeActionOutputTypeDef,
-    },
-)
-_OptionalRecipeStepOutputTypeDef = TypedDict(
-    "_OptionalRecipeStepOutputTypeDef",
-    {
-        "ConditionExpressions": List[ConditionExpressionTypeDef],
-    },
-    total=False,
-)
-
-
-class RecipeStepOutputTypeDef(_RequiredRecipeStepOutputTypeDef, _OptionalRecipeStepOutputTypeDef):
-    pass
-
-
 _RequiredRecipeStepTypeDef = TypedDict(
     "_RequiredRecipeStepTypeDef",
     {
         "Action": RecipeActionTypeDef,
     },
 )
 _OptionalRecipeStepTypeDef = TypedDict(
     "_OptionalRecipeStepTypeDef",
     {
         "ConditionExpressions": Sequence[ConditionExpressionTypeDef],
     },
     total=False,
 )
 
-
 class RecipeStepTypeDef(_RequiredRecipeStepTypeDef, _OptionalRecipeStepTypeDef):
     pass
 
-
-_RequiredRuleOutputTypeDef = TypedDict(
-    "_RequiredRuleOutputTypeDef",
-    {
-        "Name": str,
-        "CheckExpression": str,
-    },
-)
-_OptionalRuleOutputTypeDef = TypedDict(
-    "_OptionalRuleOutputTypeDef",
-    {
-        "Disabled": bool,
-        "SubstitutionMap": Dict[str, str],
-        "Threshold": ThresholdTypeDef,
-        "ColumnSelectors": List[ColumnSelectorTypeDef],
-    },
-    total=False,
-)
-
-
-class RuleOutputTypeDef(_RequiredRuleOutputTypeDef, _OptionalRuleOutputTypeDef):
-    pass
-
-
 _RequiredRuleTypeDef = TypedDict(
     "_RequiredRuleTypeDef",
     {
         "Name": str,
         "CheckExpression": str,
     },
 )
@@ -1699,28 +1466,17 @@
         "SubstitutionMap": Mapping[str, str],
         "Threshold": ThresholdTypeDef,
         "ColumnSelectors": Sequence[ColumnSelectorTypeDef],
     },
     total=False,
 )
 
-
 class RuleTypeDef(_RequiredRuleTypeDef, _OptionalRuleTypeDef):
     pass
 
-
-StatisticsConfigurationOutputTypeDef = TypedDict(
-    "StatisticsConfigurationOutputTypeDef",
-    {
-        "IncludedStatistics": List[str],
-        "Overrides": List[StatisticOverrideOutputTypeDef],
-    },
-    total=False,
-)
-
 StatisticsConfigurationTypeDef = TypedDict(
     "StatisticsConfigurationTypeDef",
     {
         "IncludedStatistics": Sequence[str],
         "Overrides": Sequence[StatisticOverrideTypeDef],
     },
     total=False,
@@ -1748,19 +1504,17 @@
     "_OptionalDatabaseOutputTypeDef",
     {
         "DatabaseOutputMode": Literal["NEW_TABLE"],
     },
     total=False,
 )
 
-
 class DatabaseOutputTypeDef(_RequiredDatabaseOutputTypeDef, _OptionalDatabaseOutputTypeDef):
     pass
 
-
 _RequiredDataCatalogOutputTypeDef = TypedDict(
     "_RequiredDataCatalogOutputTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
     },
 )
@@ -1771,21 +1525,19 @@
         "S3Options": S3TableOutputOptionsTypeDef,
         "DatabaseOptions": DatabaseTableOutputOptionsTypeDef,
         "Overwrite": bool,
     },
     total=False,
 )
 
-
 class DataCatalogOutputTypeDef(
     _RequiredDataCatalogOutputTypeDef, _OptionalDataCatalogOutputTypeDef
 ):
     pass
 
-
 ListProjectsResponseTypeDef = TypedDict(
     "ListProjectsResponseTypeDef",
     {
         "Projects": List[ProjectTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1806,53 +1558,61 @@
         "Overwrite": bool,
         "FormatOptions": OutputFormatOptionsTypeDef,
         "MaxOutputFiles": int,
     },
     total=False,
 )
 
-
 class OutputTypeDef(_RequiredOutputTypeDef, _OptionalOutputTypeDef):
     pass
 
-
-PathOptionsOutputTypeDef = TypedDict(
-    "PathOptionsOutputTypeDef",
+PathOptionsTypeDef = TypedDict(
+    "PathOptionsTypeDef",
     {
-        "LastModifiedDateCondition": FilterExpressionOutputTypeDef,
+        "LastModifiedDateCondition": FilterExpressionTypeDef,
         "FilesLimit": FilesLimitTypeDef,
-        "Parameters": Dict[str, DatasetParameterOutputTypeDef],
+        "Parameters": Mapping[str, DatasetParameterTypeDef],
     },
     total=False,
 )
 
-PathOptionsTypeDef = TypedDict(
-    "PathOptionsTypeDef",
+_RequiredCreateRecipeRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateRecipeRequestRequestTypeDef",
     {
-        "LastModifiedDateCondition": FilterExpressionTypeDef,
-        "FilesLimit": FilesLimitTypeDef,
-        "Parameters": Mapping[str, DatasetParameterTypeDef],
+        "Name": str,
+        "Steps": Sequence[RecipeStepTypeDef],
+    },
+)
+_OptionalCreateRecipeRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateRecipeRequestRequestTypeDef",
+    {
+        "Description": str,
+        "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-FormatOptionsUnionTypeDef = Union[FormatOptionsTypeDef, FormatOptionsOutputTypeDef]
+class CreateRecipeRequestRequestTypeDef(
+    _RequiredCreateRecipeRequestRequestTypeDef, _OptionalCreateRecipeRequestRequestTypeDef
+):
+    pass
+
 DescribeRecipeResponseTypeDef = TypedDict(
     "DescribeRecipeResponseTypeDef",
     {
         "CreatedBy": str,
         "CreateDate": datetime,
         "LastModifiedBy": str,
         "LastModifiedDate": datetime,
         "ProjectName": str,
         "PublishedBy": str,
         "PublishedDate": datetime,
         "Description": str,
         "Name": str,
-        "Steps": List[RecipeStepOutputTypeDef],
+        "Steps": List[RecipeStepTypeDef],
         "Tags": Dict[str, str],
         "ResourceArn": str,
         "RecipeVersion": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -1870,27 +1630,24 @@
         "LastModifiedBy": str,
         "LastModifiedDate": datetime,
         "ProjectName": str,
         "PublishedBy": str,
         "PublishedDate": datetime,
         "Description": str,
         "ResourceArn": str,
-        "Steps": List[RecipeStepOutputTypeDef],
+        "Steps": List[RecipeStepTypeDef],
         "Tags": Dict[str, str],
         "RecipeVersion": str,
     },
     total=False,
 )
 
-
 class RecipeTypeDef(_RequiredRecipeTypeDef, _OptionalRecipeTypeDef):
     pass
 
-
-RecipeStepUnionTypeDef = Union[RecipeStepTypeDef, RecipeStepOutputTypeDef]
 _RequiredSendProjectSessionActionRequestRequestTypeDef = TypedDict(
     "_RequiredSendProjectSessionActionRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalSendProjectSessionActionRequestRequestTypeDef = TypedDict(
@@ -1901,82 +1658,149 @@
         "StepIndex": int,
         "ClientSessionId": str,
         "ViewFrame": ViewFrameTypeDef,
     },
     total=False,
 )
 
-
 class SendProjectSessionActionRequestRequestTypeDef(
     _RequiredSendProjectSessionActionRequestRequestTypeDef,
     _OptionalSendProjectSessionActionRequestRequestTypeDef,
 ):
     pass
 
+_RequiredUpdateRecipeRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateRecipeRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalUpdateRecipeRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateRecipeRequestRequestTypeDef",
+    {
+        "Description": str,
+        "Steps": Sequence[RecipeStepTypeDef],
+    },
+    total=False,
+)
+
+class UpdateRecipeRequestRequestTypeDef(
+    _RequiredUpdateRecipeRequestRequestTypeDef, _OptionalUpdateRecipeRequestRequestTypeDef
+):
+    pass
+
+_RequiredCreateRulesetRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateRulesetRequestRequestTypeDef",
+    {
+        "Name": str,
+        "TargetArn": str,
+        "Rules": Sequence[RuleTypeDef],
+    },
+)
+_OptionalCreateRulesetRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateRulesetRequestRequestTypeDef",
+    {
+        "Description": str,
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class CreateRulesetRequestRequestTypeDef(
+    _RequiredCreateRulesetRequestRequestTypeDef, _OptionalCreateRulesetRequestRequestTypeDef
+):
+    pass
 
 DescribeRulesetResponseTypeDef = TypedDict(
     "DescribeRulesetResponseTypeDef",
     {
         "Name": str,
         "Description": str,
         "TargetArn": str,
-        "Rules": List[RuleOutputTypeDef],
+        "Rules": List[RuleTypeDef],
         "CreateDate": datetime,
         "CreatedBy": str,
         "LastModifiedBy": str,
         "LastModifiedDate": datetime,
         "ResourceArn": str,
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RuleUnionTypeDef = Union[RuleTypeDef, RuleOutputTypeDef]
-_RequiredColumnStatisticsConfigurationOutputTypeDef = TypedDict(
-    "_RequiredColumnStatisticsConfigurationOutputTypeDef",
+_RequiredUpdateRulesetRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateRulesetRequestRequestTypeDef",
     {
-        "Statistics": StatisticsConfigurationOutputTypeDef,
+        "Name": str,
+        "Rules": Sequence[RuleTypeDef],
     },
 )
-_OptionalColumnStatisticsConfigurationOutputTypeDef = TypedDict(
-    "_OptionalColumnStatisticsConfigurationOutputTypeDef",
+_OptionalUpdateRulesetRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateRulesetRequestRequestTypeDef",
     {
-        "Selectors": List[ColumnSelectorTypeDef],
+        "Description": str,
     },
     total=False,
 )
 
-
-class ColumnStatisticsConfigurationOutputTypeDef(
-    _RequiredColumnStatisticsConfigurationOutputTypeDef,
-    _OptionalColumnStatisticsConfigurationOutputTypeDef,
+class UpdateRulesetRequestRequestTypeDef(
+    _RequiredUpdateRulesetRequestRequestTypeDef, _OptionalUpdateRulesetRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredColumnStatisticsConfigurationTypeDef = TypedDict(
     "_RequiredColumnStatisticsConfigurationTypeDef",
     {
         "Statistics": StatisticsConfigurationTypeDef,
     },
 )
 _OptionalColumnStatisticsConfigurationTypeDef = TypedDict(
     "_OptionalColumnStatisticsConfigurationTypeDef",
     {
         "Selectors": Sequence[ColumnSelectorTypeDef],
     },
     total=False,
 )
 
-
 class ColumnStatisticsConfigurationTypeDef(
     _RequiredColumnStatisticsConfigurationTypeDef, _OptionalColumnStatisticsConfigurationTypeDef
 ):
     pass
 
+_RequiredCreateRecipeJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateRecipeJobRequestRequestTypeDef",
+    {
+        "Name": str,
+        "RoleArn": str,
+    },
+)
+_OptionalCreateRecipeJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateRecipeJobRequestRequestTypeDef",
+    {
+        "DatasetName": str,
+        "EncryptionKeyArn": str,
+        "EncryptionMode": EncryptionModeType,
+        "LogSubscription": LogSubscriptionType,
+        "MaxCapacity": int,
+        "MaxRetries": int,
+        "Outputs": Sequence[OutputTypeDef],
+        "DataCatalogOutputs": Sequence[DataCatalogOutputTypeDef],
+        "DatabaseOutputs": Sequence[DatabaseOutputTypeDef],
+        "ProjectName": str,
+        "RecipeReference": RecipeReferenceTypeDef,
+        "Tags": Mapping[str, str],
+        "Timeout": int,
+    },
+    total=False,
+)
+
+class CreateRecipeJobRequestRequestTypeDef(
+    _RequiredCreateRecipeJobRequestRequestTypeDef, _OptionalCreateRecipeJobRequestRequestTypeDef
+):
+    pass
 
 JobRunTypeDef = TypedDict(
     "JobRunTypeDef",
     {
         "Attempt": int,
         "CompletedOn": datetime,
         "DatasetName": str,
@@ -2031,95 +1855,115 @@
         "Tags": Dict[str, str],
         "JobSample": JobSampleTypeDef,
         "ValidationConfigurations": List[ValidationConfigurationTypeDef],
     },
     total=False,
 )
 
-
 class JobTypeDef(_RequiredJobTypeDef, _OptionalJobTypeDef):
     pass
 
+_RequiredUpdateRecipeJobRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateRecipeJobRequestRequestTypeDef",
+    {
+        "Name": str,
+        "RoleArn": str,
+    },
+)
+_OptionalUpdateRecipeJobRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateRecipeJobRequestRequestTypeDef",
+    {
+        "EncryptionKeyArn": str,
+        "EncryptionMode": EncryptionModeType,
+        "LogSubscription": LogSubscriptionType,
+        "MaxCapacity": int,
+        "MaxRetries": int,
+        "Outputs": Sequence[OutputTypeDef],
+        "DataCatalogOutputs": Sequence[DataCatalogOutputTypeDef],
+        "DatabaseOutputs": Sequence[DatabaseOutputTypeDef],
+        "Timeout": int,
+    },
+    total=False,
+)
+
+class UpdateRecipeJobRequestRequestTypeDef(
+    _RequiredUpdateRecipeJobRequestRequestTypeDef, _OptionalUpdateRecipeJobRequestRequestTypeDef
+):
+    pass
+
+_RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDatasetRequestRequestTypeDef",
+    {
+        "Name": str,
+        "Input": InputTypeDef,
+    },
+)
+_OptionalCreateDatasetRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDatasetRequestRequestTypeDef",
+    {
+        "Format": InputFormatType,
+        "FormatOptions": FormatOptionsTypeDef,
+        "PathOptions": PathOptionsTypeDef,
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class CreateDatasetRequestRequestTypeDef(
+    _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
+):
+    pass
 
-UnionTypeDef = Union[OutputTypeDef, OutputTypeDef]
 _RequiredDatasetTypeDef = TypedDict(
     "_RequiredDatasetTypeDef",
     {
         "Name": str,
         "Input": InputTypeDef,
     },
 )
 _OptionalDatasetTypeDef = TypedDict(
     "_OptionalDatasetTypeDef",
     {
         "AccountId": str,
         "CreatedBy": str,
         "CreateDate": datetime,
         "Format": InputFormatType,
-        "FormatOptions": FormatOptionsOutputTypeDef,
+        "FormatOptions": FormatOptionsTypeDef,
         "LastModifiedDate": datetime,
         "LastModifiedBy": str,
         "Source": SourceType,
-        "PathOptions": PathOptionsOutputTypeDef,
+        "PathOptions": PathOptionsTypeDef,
         "Tags": Dict[str, str],
         "ResourceArn": str,
     },
     total=False,
 )
 
-
 class DatasetTypeDef(_RequiredDatasetTypeDef, _OptionalDatasetTypeDef):
     pass
 
-
 DescribeDatasetResponseTypeDef = TypedDict(
     "DescribeDatasetResponseTypeDef",
     {
         "CreatedBy": str,
         "CreateDate": datetime,
         "Name": str,
         "Format": InputFormatType,
-        "FormatOptions": FormatOptionsOutputTypeDef,
+        "FormatOptions": FormatOptionsTypeDef,
         "Input": InputTypeDef,
         "LastModifiedDate": datetime,
         "LastModifiedBy": str,
         "Source": SourceType,
-        "PathOptions": PathOptionsOutputTypeDef,
+        "PathOptions": PathOptionsTypeDef,
         "Tags": Dict[str, str],
         "ResourceArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDatasetRequestRequestTypeDef",
-    {
-        "Name": str,
-        "Input": InputTypeDef,
-    },
-)
-_OptionalCreateDatasetRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDatasetRequestRequestTypeDef",
-    {
-        "Format": InputFormatType,
-        "FormatOptions": FormatOptionsTypeDef,
-        "PathOptions": PathOptionsTypeDef,
-        "Tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class CreateDatasetRequestRequestTypeDef(
-    _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
-):
-    pass
-
-
-PathOptionsUnionTypeDef = Union[PathOptionsTypeDef, PathOptionsOutputTypeDef]
 _RequiredUpdateDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDatasetRequestRequestTypeDef",
     {
         "Name": str,
         "Input": InputTypeDef,
     },
 )
@@ -2129,21 +1973,19 @@
         "Format": InputFormatType,
         "FormatOptions": FormatOptionsTypeDef,
         "PathOptions": PathOptionsTypeDef,
     },
     total=False,
 )
 
-
 class UpdateDatasetRequestRequestTypeDef(
     _RequiredUpdateDatasetRequestRequestTypeDef, _OptionalUpdateDatasetRequestRequestTypeDef
 ):
     pass
 
-
 ListRecipeVersionsResponseTypeDef = TypedDict(
     "ListRecipeVersionsResponseTypeDef",
     {
         "NextToken": str,
         "Recipes": List[RecipeTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2154,116 +1996,14 @@
     {
         "Recipes": List[RecipeTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateRecipeRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateRecipeRequestRequestTypeDef",
-    {
-        "Name": str,
-        "Steps": Sequence[RecipeStepUnionTypeDef],
-    },
-)
-_OptionalCreateRecipeRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateRecipeRequestRequestTypeDef",
-    {
-        "Description": str,
-        "Tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class CreateRecipeRequestRequestTypeDef(
-    _RequiredCreateRecipeRequestRequestTypeDef, _OptionalCreateRecipeRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredUpdateRecipeRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateRecipeRequestRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalUpdateRecipeRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateRecipeRequestRequestTypeDef",
-    {
-        "Description": str,
-        "Steps": Sequence[RecipeStepUnionTypeDef],
-    },
-    total=False,
-)
-
-
-class UpdateRecipeRequestRequestTypeDef(
-    _RequiredUpdateRecipeRequestRequestTypeDef, _OptionalUpdateRecipeRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredCreateRulesetRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateRulesetRequestRequestTypeDef",
-    {
-        "Name": str,
-        "TargetArn": str,
-        "Rules": Sequence[RuleUnionTypeDef],
-    },
-)
-_OptionalCreateRulesetRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateRulesetRequestRequestTypeDef",
-    {
-        "Description": str,
-        "Tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class CreateRulesetRequestRequestTypeDef(
-    _RequiredCreateRulesetRequestRequestTypeDef, _OptionalCreateRulesetRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredUpdateRulesetRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateRulesetRequestRequestTypeDef",
-    {
-        "Name": str,
-        "Rules": Sequence[RuleUnionTypeDef],
-    },
-)
-_OptionalUpdateRulesetRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateRulesetRequestRequestTypeDef",
-    {
-        "Description": str,
-    },
-    total=False,
-)
-
-
-class UpdateRulesetRequestRequestTypeDef(
-    _RequiredUpdateRulesetRequestRequestTypeDef, _OptionalUpdateRulesetRequestRequestTypeDef
-):
-    pass
-
-
-ProfileConfigurationOutputTypeDef = TypedDict(
-    "ProfileConfigurationOutputTypeDef",
-    {
-        "DatasetStatisticsConfiguration": StatisticsConfigurationOutputTypeDef,
-        "ProfileColumns": List[ColumnSelectorTypeDef],
-        "ColumnStatisticsConfigurations": List[ColumnStatisticsConfigurationOutputTypeDef],
-        "EntityDetectorConfiguration": EntityDetectorConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 ProfileConfigurationTypeDef = TypedDict(
     "ProfileConfigurationTypeDef",
     {
         "DatasetStatisticsConfiguration": StatisticsConfigurationTypeDef,
         "ProfileColumns": Sequence[ColumnSelectorTypeDef],
         "ColumnStatisticsConfigurations": Sequence[ColumnStatisticsConfigurationTypeDef],
         "EntityDetectorConfiguration": EntityDetectorConfigurationTypeDef,
@@ -2285,87 +2025,54 @@
     {
         "Jobs": List[JobTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateRecipeJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateRecipeJobRequestRequestTypeDef",
-    {
-        "Name": str,
-        "RoleArn": str,
-    },
-)
-_OptionalCreateRecipeJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateRecipeJobRequestRequestTypeDef",
+ListDatasetsResponseTypeDef = TypedDict(
+    "ListDatasetsResponseTypeDef",
     {
-        "DatasetName": str,
-        "EncryptionKeyArn": str,
-        "EncryptionMode": EncryptionModeType,
-        "LogSubscription": LogSubscriptionType,
-        "MaxCapacity": int,
-        "MaxRetries": int,
-        "Outputs": Sequence[UnionTypeDef],
-        "DataCatalogOutputs": Sequence[DataCatalogOutputTypeDef],
-        "DatabaseOutputs": Sequence[DatabaseOutputTypeDef],
-        "ProjectName": str,
-        "RecipeReference": RecipeReferenceTypeDef,
-        "Tags": Mapping[str, str],
-        "Timeout": int,
+        "Datasets": List[DatasetTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class CreateRecipeJobRequestRequestTypeDef(
-    _RequiredCreateRecipeJobRequestRequestTypeDef, _OptionalCreateRecipeJobRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredUpdateRecipeJobRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateRecipeJobRequestRequestTypeDef",
+_RequiredCreateProfileJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateProfileJobRequestRequestTypeDef",
     {
+        "DatasetName": str,
         "Name": str,
+        "OutputLocation": S3LocationTypeDef,
         "RoleArn": str,
     },
 )
-_OptionalUpdateRecipeJobRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateRecipeJobRequestRequestTypeDef",
+_OptionalCreateProfileJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateProfileJobRequestRequestTypeDef",
     {
         "EncryptionKeyArn": str,
         "EncryptionMode": EncryptionModeType,
         "LogSubscription": LogSubscriptionType,
         "MaxCapacity": int,
         "MaxRetries": int,
-        "Outputs": Sequence[UnionTypeDef],
-        "DataCatalogOutputs": Sequence[DataCatalogOutputTypeDef],
-        "DatabaseOutputs": Sequence[DatabaseOutputTypeDef],
+        "Configuration": ProfileConfigurationTypeDef,
+        "ValidationConfigurations": Sequence[ValidationConfigurationTypeDef],
+        "Tags": Mapping[str, str],
         "Timeout": int,
+        "JobSample": JobSampleTypeDef,
     },
     total=False,
 )
 
-
-class UpdateRecipeJobRequestRequestTypeDef(
-    _RequiredUpdateRecipeJobRequestRequestTypeDef, _OptionalUpdateRecipeJobRequestRequestTypeDef
+class CreateProfileJobRequestRequestTypeDef(
+    _RequiredCreateProfileJobRequestRequestTypeDef, _OptionalCreateProfileJobRequestRequestTypeDef
 ):
     pass
 
-
-ListDatasetsResponseTypeDef = TypedDict(
-    "ListDatasetsResponseTypeDef",
-    {
-        "Datasets": List[DatasetTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DescribeJobResponseTypeDef = TypedDict(
     "DescribeJobResponseTypeDef",
     {
         "CreateDate": datetime,
         "CreatedBy": str,
         "DatasetName": str,
         "EncryptionKeyArn": str,
@@ -2377,15 +2084,15 @@
         "LogSubscription": LogSubscriptionType,
         "MaxCapacity": int,
         "MaxRetries": int,
         "Outputs": List[OutputTypeDef],
         "DataCatalogOutputs": List[DataCatalogOutputTypeDef],
         "DatabaseOutputs": List[DatabaseOutputTypeDef],
         "ProjectName": str,
-        "ProfileConfiguration": ProfileConfigurationOutputTypeDef,
+        "ProfileConfiguration": ProfileConfigurationTypeDef,
         "ValidationConfigurations": List[ValidationConfigurationTypeDef],
         "RecipeReference": RecipeReferenceTypeDef,
         "ResourceArn": str,
         "RoleArn": str,
         "Tags": Dict[str, str],
         "Timeout": int,
         "JobSample": JobSampleTypeDef,
@@ -2398,15 +2105,15 @@
     {
         "Attempt": int,
         "CompletedOn": datetime,
         "DatasetName": str,
         "ErrorMessage": str,
         "ExecutionTime": int,
         "JobName": str,
-        "ProfileConfiguration": ProfileConfigurationOutputTypeDef,
+        "ProfileConfiguration": ProfileConfigurationTypeDef,
         "ValidationConfigurations": List[ValidationConfigurationTypeDef],
         "RunId": str,
         "State": JobRunStateType,
         "LogSubscription": LogSubscriptionType,
         "LogGroupName": str,
         "Outputs": List[OutputTypeDef],
         "DataCatalogOutputs": List[DataCatalogOutputTypeDef],
@@ -2415,50 +2122,14 @@
         "StartedBy": str,
         "StartedOn": datetime,
         "JobSample": JobSampleTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateProfileJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateProfileJobRequestRequestTypeDef",
-    {
-        "DatasetName": str,
-        "Name": str,
-        "OutputLocation": S3LocationTypeDef,
-        "RoleArn": str,
-    },
-)
-_OptionalCreateProfileJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateProfileJobRequestRequestTypeDef",
-    {
-        "EncryptionKeyArn": str,
-        "EncryptionMode": EncryptionModeType,
-        "LogSubscription": LogSubscriptionType,
-        "MaxCapacity": int,
-        "MaxRetries": int,
-        "Configuration": ProfileConfigurationTypeDef,
-        "ValidationConfigurations": Sequence[ValidationConfigurationTypeDef],
-        "Tags": Mapping[str, str],
-        "Timeout": int,
-        "JobSample": JobSampleTypeDef,
-    },
-    total=False,
-)
-
-
-class CreateProfileJobRequestRequestTypeDef(
-    _RequiredCreateProfileJobRequestRequestTypeDef, _OptionalCreateProfileJobRequestRequestTypeDef
-):
-    pass
-
-
-ProfileConfigurationUnionTypeDef = Union[
-    ProfileConfigurationTypeDef, ProfileConfigurationOutputTypeDef
-]
 _RequiredUpdateProfileJobRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateProfileJobRequestRequestTypeDef",
     {
         "Name": str,
         "OutputLocation": S3LocationTypeDef,
         "RoleArn": str,
     },
@@ -2475,12 +2146,11 @@
         "ValidationConfigurations": Sequence[ValidationConfigurationTypeDef],
         "Timeout": int,
         "JobSample": JobSampleTypeDef,
     },
     total=False,
 )
 
-
 class UpdateProfileJobRequestRequestTypeDef(
     _RequiredUpdateProfileJobRequestRequestTypeDef, _OptionalUpdateProfileJobRequestRequestTypeDef
 ):
     pass
```

### Comparing `types-aiobotocore-databrew-2.5.2.post1/types_aiobotocore_databrew/type_defs.pyi` & `types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 Type annotations for databrew service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_databrew/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_databrew.type_defs import AllowedStatisticsOutputTypeDef
+    from types_aiobotocore_databrew.type_defs import AllowedStatisticsTypeDef
 
-    data: AllowedStatisticsOutputTypeDef = ...
+    data: AllowedStatisticsTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AnalyticsModeType,
     CompressionFormatType,
     EncryptionModeType,
     InputFormatType,
     JobRunStateType,
@@ -39,16 +39,16 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
-    "AllowedStatisticsOutputTypeDef",
     "AllowedStatisticsTypeDef",
     "BatchDeleteRecipeVersionRequestRequestTypeDef",
     "RecipeVersionErrorDetailTypeDef",
     "ResponseMetadataTypeDef",
     "ColumnSelectorTypeDef",
     "ConditionExpressionTypeDef",
     "JobSampleTypeDef",
@@ -56,30 +56,28 @@
     "ValidationConfigurationTypeDef",
     "SampleTypeDef",
     "RecipeReferenceTypeDef",
     "CreateScheduleRequestRequestTypeDef",
     "CsvOptionsTypeDef",
     "CsvOutputOptionsTypeDef",
     "DatetimeOptionsTypeDef",
-    "FilterExpressionOutputTypeDef",
     "FilterExpressionTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
     "DeleteJobRequestRequestTypeDef",
     "DeleteProjectRequestRequestTypeDef",
     "DeleteRecipeVersionRequestRequestTypeDef",
     "DeleteRulesetRequestRequestTypeDef",
     "DeleteScheduleRequestRequestTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
     "DescribeJobRequestRequestTypeDef",
     "DescribeJobRunRequestRequestTypeDef",
     "DescribeProjectRequestRequestTypeDef",
     "DescribeRecipeRequestRequestTypeDef",
     "DescribeRulesetRequestRequestTypeDef",
     "DescribeScheduleRequestRequestTypeDef",
-    "ExcelOptionsOutputTypeDef",
     "ExcelOptionsTypeDef",
     "FilesLimitTypeDef",
     "JsonOptionsTypeDef",
     "MetadataTypeDef",
     "PaginatorConfigTypeDef",
     "ListDatasetsRequestRequestTypeDef",
     "ListJobRunsRequestRequestTypeDef",
@@ -89,27 +87,24 @@
     "ListRecipesRequestRequestTypeDef",
     "ListRulesetsRequestRequestTypeDef",
     "RulesetItemTypeDef",
     "ListSchedulesRequestRequestTypeDef",
     "ScheduleTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "PublishRecipeRequestRequestTypeDef",
-    "RecipeActionOutputTypeDef",
     "RecipeActionTypeDef",
     "ThresholdTypeDef",
     "ViewFrameTypeDef",
     "StartJobRunRequestRequestTypeDef",
     "StartProjectSessionRequestRequestTypeDef",
-    "StatisticOverrideOutputTypeDef",
     "StatisticOverrideTypeDef",
     "StopJobRunRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateScheduleRequestRequestTypeDef",
-    "EntityDetectorConfigurationOutputTypeDef",
     "EntityDetectorConfigurationTypeDef",
     "BatchDeleteRecipeVersionResponseTypeDef",
     "CreateDatasetResponseTypeDef",
     "CreateProfileJobResponseTypeDef",
     "CreateProjectResponseTypeDef",
     "CreateRecipeJobResponseTypeDef",
     "CreateRecipeResponseTypeDef",
@@ -140,85 +135,64 @@
     "DatabaseTableOutputOptionsTypeDef",
     "S3TableOutputOptionsTypeDef",
     "CreateProjectRequestRequestTypeDef",
     "DescribeProjectResponseTypeDef",
     "ProjectTypeDef",
     "UpdateProjectRequestRequestTypeDef",
     "OutputFormatOptionsTypeDef",
-    "DatasetParameterOutputTypeDef",
     "DatasetParameterTypeDef",
-    "FormatOptionsOutputTypeDef",
     "FormatOptionsTypeDef",
     "ListDatasetsRequestListDatasetsPaginateTypeDef",
     "ListJobRunsRequestListJobRunsPaginateTypeDef",
     "ListJobsRequestListJobsPaginateTypeDef",
     "ListProjectsRequestListProjectsPaginateTypeDef",
     "ListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef",
     "ListRecipesRequestListRecipesPaginateTypeDef",
     "ListRulesetsRequestListRulesetsPaginateTypeDef",
     "ListSchedulesRequestListSchedulesPaginateTypeDef",
     "ListRulesetsResponseTypeDef",
     "ListSchedulesResponseTypeDef",
-    "RecipeStepOutputTypeDef",
     "RecipeStepTypeDef",
-    "RuleOutputTypeDef",
     "RuleTypeDef",
-    "StatisticsConfigurationOutputTypeDef",
     "StatisticsConfigurationTypeDef",
     "InputTypeDef",
     "DatabaseOutputTypeDef",
     "DataCatalogOutputTypeDef",
     "ListProjectsResponseTypeDef",
     "OutputTypeDef",
-    "PathOptionsOutputTypeDef",
     "PathOptionsTypeDef",
-    "FormatOptionsUnionTypeDef",
+    "CreateRecipeRequestRequestTypeDef",
     "DescribeRecipeResponseTypeDef",
     "RecipeTypeDef",
-    "RecipeStepUnionTypeDef",
     "SendProjectSessionActionRequestRequestTypeDef",
+    "UpdateRecipeRequestRequestTypeDef",
+    "CreateRulesetRequestRequestTypeDef",
     "DescribeRulesetResponseTypeDef",
-    "RuleUnionTypeDef",
-    "ColumnStatisticsConfigurationOutputTypeDef",
+    "UpdateRulesetRequestRequestTypeDef",
     "ColumnStatisticsConfigurationTypeDef",
+    "CreateRecipeJobRequestRequestTypeDef",
     "JobRunTypeDef",
     "JobTypeDef",
-    "UnionTypeDef",
+    "UpdateRecipeJobRequestRequestTypeDef",
+    "CreateDatasetRequestRequestTypeDef",
     "DatasetTypeDef",
     "DescribeDatasetResponseTypeDef",
-    "CreateDatasetRequestRequestTypeDef",
-    "PathOptionsUnionTypeDef",
     "UpdateDatasetRequestRequestTypeDef",
     "ListRecipeVersionsResponseTypeDef",
     "ListRecipesResponseTypeDef",
-    "CreateRecipeRequestRequestTypeDef",
-    "UpdateRecipeRequestRequestTypeDef",
-    "CreateRulesetRequestRequestTypeDef",
-    "UpdateRulesetRequestRequestTypeDef",
-    "ProfileConfigurationOutputTypeDef",
     "ProfileConfigurationTypeDef",
     "ListJobRunsResponseTypeDef",
     "ListJobsResponseTypeDef",
-    "CreateRecipeJobRequestRequestTypeDef",
-    "UpdateRecipeJobRequestRequestTypeDef",
     "ListDatasetsResponseTypeDef",
+    "CreateProfileJobRequestRequestTypeDef",
     "DescribeJobResponseTypeDef",
     "DescribeJobRunResponseTypeDef",
-    "CreateProfileJobRequestRequestTypeDef",
-    "ProfileConfigurationUnionTypeDef",
     "UpdateProfileJobRequestRequestTypeDef",
 )
 
-AllowedStatisticsOutputTypeDef = TypedDict(
-    "AllowedStatisticsOutputTypeDef",
-    {
-        "Statistics": List[str],
-    },
-)
-
 AllowedStatisticsTypeDef = TypedDict(
     "AllowedStatisticsTypeDef",
     {
         "Statistics": Sequence[str],
     },
 )
 
@@ -271,19 +245,21 @@
     "_OptionalConditionExpressionTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
+
 class ConditionExpressionTypeDef(
     _RequiredConditionExpressionTypeDef, _OptionalConditionExpressionTypeDef
 ):
     pass
 
+
 JobSampleTypeDef = TypedDict(
     "JobSampleTypeDef",
     {
         "Mode": SampleModeType,
         "Size": int,
     },
     total=False,
@@ -300,70 +276,78 @@
     {
         "Key": str,
         "BucketOwner": str,
     },
     total=False,
 )
 
+
 class S3LocationTypeDef(_RequiredS3LocationTypeDef, _OptionalS3LocationTypeDef):
     pass
 
+
 _RequiredValidationConfigurationTypeDef = TypedDict(
     "_RequiredValidationConfigurationTypeDef",
     {
         "RulesetArn": str,
     },
 )
 _OptionalValidationConfigurationTypeDef = TypedDict(
     "_OptionalValidationConfigurationTypeDef",
     {
         "ValidationMode": Literal["CHECK_ALL"],
     },
     total=False,
 )
 
+
 class ValidationConfigurationTypeDef(
     _RequiredValidationConfigurationTypeDef, _OptionalValidationConfigurationTypeDef
 ):
     pass
 
+
 _RequiredSampleTypeDef = TypedDict(
     "_RequiredSampleTypeDef",
     {
         "Type": SampleTypeType,
     },
 )
 _OptionalSampleTypeDef = TypedDict(
     "_OptionalSampleTypeDef",
     {
         "Size": int,
     },
     total=False,
 )
 
+
 class SampleTypeDef(_RequiredSampleTypeDef, _OptionalSampleTypeDef):
     pass
 
+
 _RequiredRecipeReferenceTypeDef = TypedDict(
     "_RequiredRecipeReferenceTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalRecipeReferenceTypeDef = TypedDict(
     "_OptionalRecipeReferenceTypeDef",
     {
         "RecipeVersion": str,
     },
     total=False,
 )
 
+
 class RecipeReferenceTypeDef(_RequiredRecipeReferenceTypeDef, _OptionalRecipeReferenceTypeDef):
     pass
 
+
 _RequiredCreateScheduleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateScheduleRequestRequestTypeDef",
     {
         "CronExpression": str,
         "Name": str,
     },
 )
@@ -372,19 +356,21 @@
     {
         "JobNames": Sequence[str],
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateScheduleRequestRequestTypeDef(
     _RequiredCreateScheduleRequestRequestTypeDef, _OptionalCreateScheduleRequestRequestTypeDef
 ):
     pass
 
+
 CsvOptionsTypeDef = TypedDict(
     "CsvOptionsTypeDef",
     {
         "Delimiter": str,
         "HeaderRow": bool,
     },
     total=False,
@@ -409,24 +395,18 @@
     {
         "TimezoneOffset": str,
         "LocaleCode": str,
     },
     total=False,
 )
 
+
 class DatetimeOptionsTypeDef(_RequiredDatetimeOptionsTypeDef, _OptionalDatetimeOptionsTypeDef):
     pass
 
-FilterExpressionOutputTypeDef = TypedDict(
-    "FilterExpressionOutputTypeDef",
-    {
-        "Expression": str,
-        "ValuesMap": Dict[str, str],
-    },
-)
 
 FilterExpressionTypeDef = TypedDict(
     "FilterExpressionTypeDef",
     {
         "Expression": str,
         "ValuesMap": Mapping[str, str],
     },
@@ -514,43 +494,35 @@
     "_OptionalDescribeRecipeRequestRequestTypeDef",
     {
         "RecipeVersion": str,
     },
     total=False,
 )
 
+
 class DescribeRecipeRequestRequestTypeDef(
     _RequiredDescribeRecipeRequestRequestTypeDef, _OptionalDescribeRecipeRequestRequestTypeDef
 ):
     pass
 
+
 DescribeRulesetRequestRequestTypeDef = TypedDict(
     "DescribeRulesetRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
 DescribeScheduleRequestRequestTypeDef = TypedDict(
     "DescribeScheduleRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-ExcelOptionsOutputTypeDef = TypedDict(
-    "ExcelOptionsOutputTypeDef",
-    {
-        "SheetNames": List[str],
-        "SheetIndexes": List[int],
-        "HeaderRow": bool,
-    },
-    total=False,
-)
-
 ExcelOptionsTypeDef = TypedDict(
     "ExcelOptionsTypeDef",
     {
         "SheetNames": Sequence[str],
         "SheetIndexes": Sequence[int],
         "HeaderRow": bool,
     },
@@ -568,17 +540,19 @@
     {
         "OrderedBy": Literal["LAST_MODIFIED_DATE"],
         "Order": OrderType,
     },
     total=False,
 )
 
+
 class FilesLimitTypeDef(_RequiredFilesLimitTypeDef, _OptionalFilesLimitTypeDef):
     pass
 
+
 JsonOptionsTypeDef = TypedDict(
     "JsonOptionsTypeDef",
     {
         "MultiLine": bool,
     },
     total=False,
 )
@@ -621,19 +595,21 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListJobRunsRequestRequestTypeDef(
     _RequiredListJobRunsRequestRequestTypeDef, _OptionalListJobRunsRequestRequestTypeDef
 ):
     pass
 
+
 ListJobsRequestRequestTypeDef = TypedDict(
     "ListJobsRequestRequestTypeDef",
     {
         "DatasetName": str,
         "MaxResults": int,
         "NextToken": str,
         "ProjectName": str,
@@ -661,20 +637,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListRecipeVersionsRequestRequestTypeDef(
     _RequiredListRecipeVersionsRequestRequestTypeDef,
     _OptionalListRecipeVersionsRequestRequestTypeDef,
 ):
     pass
 
+
 ListRecipesRequestRequestTypeDef = TypedDict(
     "ListRecipesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "RecipeVersion": str,
     },
@@ -710,17 +688,19 @@
         "ResourceArn": str,
         "RuleCount": int,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
+
 class RulesetItemTypeDef(_RequiredRulesetItemTypeDef, _OptionalRulesetItemTypeDef):
     pass
 
+
 ListSchedulesRequestRequestTypeDef = TypedDict(
     "ListSchedulesRequestRequestTypeDef",
     {
         "JobName": str,
         "MaxResults": int,
         "NextToken": str,
     },
@@ -745,17 +725,19 @@
         "ResourceArn": str,
         "CronExpression": str,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
+
 class ScheduleTypeDef(_RequiredScheduleTypeDef, _OptionalScheduleTypeDef):
     pass
 
+
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
@@ -769,37 +751,20 @@
     "_OptionalPublishRecipeRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class PublishRecipeRequestRequestTypeDef(
     _RequiredPublishRecipeRequestRequestTypeDef, _OptionalPublishRecipeRequestRequestTypeDef
 ):
     pass
 
-_RequiredRecipeActionOutputTypeDef = TypedDict(
-    "_RequiredRecipeActionOutputTypeDef",
-    {
-        "Operation": str,
-    },
-)
-_OptionalRecipeActionOutputTypeDef = TypedDict(
-    "_OptionalRecipeActionOutputTypeDef",
-    {
-        "Parameters": Dict[str, str],
-    },
-    total=False,
-)
-
-class RecipeActionOutputTypeDef(
-    _RequiredRecipeActionOutputTypeDef, _OptionalRecipeActionOutputTypeDef
-):
-    pass
 
 _RequiredRecipeActionTypeDef = TypedDict(
     "_RequiredRecipeActionTypeDef",
     {
         "Operation": str,
     },
 )
@@ -807,17 +772,19 @@
     "_OptionalRecipeActionTypeDef",
     {
         "Parameters": Mapping[str, str],
     },
     total=False,
 )
 
+
 class RecipeActionTypeDef(_RequiredRecipeActionTypeDef, _OptionalRecipeActionTypeDef):
     pass
 
+
 _RequiredThresholdTypeDef = TypedDict(
     "_RequiredThresholdTypeDef",
     {
         "Value": float,
     },
 )
 _OptionalThresholdTypeDef = TypedDict(
@@ -825,17 +792,19 @@
     {
         "Type": ThresholdTypeType,
         "Unit": ThresholdUnitType,
     },
     total=False,
 )
 
+
 class ThresholdTypeDef(_RequiredThresholdTypeDef, _OptionalThresholdTypeDef):
     pass
 
+
 _RequiredViewFrameTypeDef = TypedDict(
     "_RequiredViewFrameTypeDef",
     {
         "StartColumnIndex": int,
     },
 )
 _OptionalViewFrameTypeDef = TypedDict(
@@ -846,17 +815,19 @@
         "StartRowIndex": int,
         "RowRange": int,
         "Analytics": AnalyticsModeType,
     },
     total=False,
 )
 
+
 class ViewFrameTypeDef(_RequiredViewFrameTypeDef, _OptionalViewFrameTypeDef):
     pass
 
+
 StartJobRunRequestRequestTypeDef = TypedDict(
     "StartJobRunRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -870,27 +841,21 @@
     "_OptionalStartProjectSessionRequestRequestTypeDef",
     {
         "AssumeControl": bool,
     },
     total=False,
 )
 
+
 class StartProjectSessionRequestRequestTypeDef(
     _RequiredStartProjectSessionRequestRequestTypeDef,
     _OptionalStartProjectSessionRequestRequestTypeDef,
 ):
     pass
 
-StatisticOverrideOutputTypeDef = TypedDict(
-    "StatisticOverrideOutputTypeDef",
-    {
-        "Statistic": str,
-        "Parameters": Dict[str, str],
-    },
-)
 
 StatisticOverrideTypeDef = TypedDict(
     "StatisticOverrideTypeDef",
     {
         "Statistic": str,
         "Parameters": Mapping[str, str],
     },
@@ -931,38 +896,20 @@
     "_OptionalUpdateScheduleRequestRequestTypeDef",
     {
         "JobNames": Sequence[str],
     },
     total=False,
 )
 
+
 class UpdateScheduleRequestRequestTypeDef(
     _RequiredUpdateScheduleRequestRequestTypeDef, _OptionalUpdateScheduleRequestRequestTypeDef
 ):
     pass
 
-_RequiredEntityDetectorConfigurationOutputTypeDef = TypedDict(
-    "_RequiredEntityDetectorConfigurationOutputTypeDef",
-    {
-        "EntityTypes": List[str],
-    },
-)
-_OptionalEntityDetectorConfigurationOutputTypeDef = TypedDict(
-    "_OptionalEntityDetectorConfigurationOutputTypeDef",
-    {
-        "AllowedStatistics": List[AllowedStatisticsOutputTypeDef],
-    },
-    total=False,
-)
-
-class EntityDetectorConfigurationOutputTypeDef(
-    _RequiredEntityDetectorConfigurationOutputTypeDef,
-    _OptionalEntityDetectorConfigurationOutputTypeDef,
-):
-    pass
 
 _RequiredEntityDetectorConfigurationTypeDef = TypedDict(
     "_RequiredEntityDetectorConfigurationTypeDef",
     {
         "EntityTypes": Sequence[str],
     },
 )
@@ -970,19 +917,21 @@
     "_OptionalEntityDetectorConfigurationTypeDef",
     {
         "AllowedStatistics": Sequence[AllowedStatisticsTypeDef],
     },
     total=False,
 )
 
+
 class EntityDetectorConfigurationTypeDef(
     _RequiredEntityDetectorConfigurationTypeDef, _OptionalEntityDetectorConfigurationTypeDef
 ):
     pass
 
+
 BatchDeleteRecipeVersionResponseTypeDef = TypedDict(
     "BatchDeleteRecipeVersionResponseTypeDef",
     {
         "Name": str,
         "Errors": List[RecipeVersionErrorDetailTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1229,19 +1178,21 @@
     {
         "CatalogId": str,
         "TempDirectory": S3LocationTypeDef,
     },
     total=False,
 )
 
+
 class DataCatalogInputDefinitionTypeDef(
     _RequiredDataCatalogInputDefinitionTypeDef, _OptionalDataCatalogInputDefinitionTypeDef
 ):
     pass
 
+
 _RequiredDatabaseInputDefinitionTypeDef = TypedDict(
     "_RequiredDatabaseInputDefinitionTypeDef",
     {
         "GlueConnectionName": str,
     },
 )
 _OptionalDatabaseInputDefinitionTypeDef = TypedDict(
@@ -1250,38 +1201,42 @@
         "DatabaseTableName": str,
         "TempDirectory": S3LocationTypeDef,
         "QueryString": str,
     },
     total=False,
 )
 
+
 class DatabaseInputDefinitionTypeDef(
     _RequiredDatabaseInputDefinitionTypeDef, _OptionalDatabaseInputDefinitionTypeDef
 ):
     pass
 
+
 _RequiredDatabaseTableOutputOptionsTypeDef = TypedDict(
     "_RequiredDatabaseTableOutputOptionsTypeDef",
     {
         "TableName": str,
     },
 )
 _OptionalDatabaseTableOutputOptionsTypeDef = TypedDict(
     "_OptionalDatabaseTableOutputOptionsTypeDef",
     {
         "TempDirectory": S3LocationTypeDef,
     },
     total=False,
 )
 
+
 class DatabaseTableOutputOptionsTypeDef(
     _RequiredDatabaseTableOutputOptionsTypeDef, _OptionalDatabaseTableOutputOptionsTypeDef
 ):
     pass
 
+
 S3TableOutputOptionsTypeDef = TypedDict(
     "S3TableOutputOptionsTypeDef",
     {
         "Location": S3LocationTypeDef,
     },
 )
 
@@ -1299,19 +1254,21 @@
     {
         "Sample": SampleTypeDef,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateProjectRequestRequestTypeDef(
     _RequiredCreateProjectRequestRequestTypeDef, _OptionalCreateProjectRequestRequestTypeDef
 ):
     pass
 
+
 DescribeProjectResponseTypeDef = TypedDict(
     "DescribeProjectResponseTypeDef",
     {
         "CreateDate": datetime,
         "CreatedBy": str,
         "DatasetName": str,
         "LastModifiedDate": datetime,
@@ -1351,17 +1308,19 @@
         "RoleArn": str,
         "OpenedBy": str,
         "OpenDate": datetime,
     },
     total=False,
 )
 
+
 class ProjectTypeDef(_RequiredProjectTypeDef, _OptionalProjectTypeDef):
     pass
 
+
 _RequiredUpdateProjectRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateProjectRequestRequestTypeDef",
     {
         "RoleArn": str,
         "Name": str,
     },
 )
@@ -1369,49 +1328,29 @@
     "_OptionalUpdateProjectRequestRequestTypeDef",
     {
         "Sample": SampleTypeDef,
     },
     total=False,
 )
 
+
 class UpdateProjectRequestRequestTypeDef(
     _RequiredUpdateProjectRequestRequestTypeDef, _OptionalUpdateProjectRequestRequestTypeDef
 ):
     pass
 
+
 OutputFormatOptionsTypeDef = TypedDict(
     "OutputFormatOptionsTypeDef",
     {
         "Csv": CsvOutputOptionsTypeDef,
     },
     total=False,
 )
 
-_RequiredDatasetParameterOutputTypeDef = TypedDict(
-    "_RequiredDatasetParameterOutputTypeDef",
-    {
-        "Name": str,
-        "Type": ParameterTypeType,
-    },
-)
-_OptionalDatasetParameterOutputTypeDef = TypedDict(
-    "_OptionalDatasetParameterOutputTypeDef",
-    {
-        "DatetimeOptions": DatetimeOptionsTypeDef,
-        "CreateColumn": bool,
-        "Filter": FilterExpressionOutputTypeDef,
-    },
-    total=False,
-)
-
-class DatasetParameterOutputTypeDef(
-    _RequiredDatasetParameterOutputTypeDef, _OptionalDatasetParameterOutputTypeDef
-):
-    pass
-
 _RequiredDatasetParameterTypeDef = TypedDict(
     "_RequiredDatasetParameterTypeDef",
     {
         "Name": str,
         "Type": ParameterTypeType,
     },
 )
@@ -1421,26 +1360,18 @@
         "DatetimeOptions": DatetimeOptionsTypeDef,
         "CreateColumn": bool,
         "Filter": FilterExpressionTypeDef,
     },
     total=False,
 )
 
+
 class DatasetParameterTypeDef(_RequiredDatasetParameterTypeDef, _OptionalDatasetParameterTypeDef):
     pass
 
-FormatOptionsOutputTypeDef = TypedDict(
-    "FormatOptionsOutputTypeDef",
-    {
-        "Json": JsonOptionsTypeDef,
-        "Excel": ExcelOptionsOutputTypeDef,
-        "Csv": CsvOptionsTypeDef,
-    },
-    total=False,
-)
 
 FormatOptionsTypeDef = TypedDict(
     "FormatOptionsTypeDef",
     {
         "Json": JsonOptionsTypeDef,
         "Excel": ExcelOptionsTypeDef,
         "Csv": CsvOptionsTypeDef,
@@ -1466,20 +1397,22 @@
     "_OptionalListJobRunsRequestListJobRunsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListJobRunsRequestListJobRunsPaginateTypeDef(
     _RequiredListJobRunsRequestListJobRunsPaginateTypeDef,
     _OptionalListJobRunsRequestListJobRunsPaginateTypeDef,
 ):
     pass
 
+
 ListJobsRequestListJobsPaginateTypeDef = TypedDict(
     "ListJobsRequestListJobsPaginateTypeDef",
     {
         "DatasetName": str,
         "ProjectName": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -1504,20 +1437,22 @@
     "_OptionalListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef(
     _RequiredListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef,
     _OptionalListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef,
 ):
     pass
 
+
 ListRecipesRequestListRecipesPaginateTypeDef = TypedDict(
     "ListRecipesRequestListRecipesPaginateTypeDef",
     {
         "RecipeVersion": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -1555,68 +1490,32 @@
     {
         "Schedules": List[ScheduleTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredRecipeStepOutputTypeDef = TypedDict(
-    "_RequiredRecipeStepOutputTypeDef",
-    {
-        "Action": RecipeActionOutputTypeDef,
-    },
-)
-_OptionalRecipeStepOutputTypeDef = TypedDict(
-    "_OptionalRecipeStepOutputTypeDef",
-    {
-        "ConditionExpressions": List[ConditionExpressionTypeDef],
-    },
-    total=False,
-)
-
-class RecipeStepOutputTypeDef(_RequiredRecipeStepOutputTypeDef, _OptionalRecipeStepOutputTypeDef):
-    pass
-
 _RequiredRecipeStepTypeDef = TypedDict(
     "_RequiredRecipeStepTypeDef",
     {
         "Action": RecipeActionTypeDef,
     },
 )
 _OptionalRecipeStepTypeDef = TypedDict(
     "_OptionalRecipeStepTypeDef",
     {
         "ConditionExpressions": Sequence[ConditionExpressionTypeDef],
     },
     total=False,
 )
 
+
 class RecipeStepTypeDef(_RequiredRecipeStepTypeDef, _OptionalRecipeStepTypeDef):
     pass
 
-_RequiredRuleOutputTypeDef = TypedDict(
-    "_RequiredRuleOutputTypeDef",
-    {
-        "Name": str,
-        "CheckExpression": str,
-    },
-)
-_OptionalRuleOutputTypeDef = TypedDict(
-    "_OptionalRuleOutputTypeDef",
-    {
-        "Disabled": bool,
-        "SubstitutionMap": Dict[str, str],
-        "Threshold": ThresholdTypeDef,
-        "ColumnSelectors": List[ColumnSelectorTypeDef],
-    },
-    total=False,
-)
-
-class RuleOutputTypeDef(_RequiredRuleOutputTypeDef, _OptionalRuleOutputTypeDef):
-    pass
 
 _RequiredRuleTypeDef = TypedDict(
     "_RequiredRuleTypeDef",
     {
         "Name": str,
         "CheckExpression": str,
     },
@@ -1628,25 +1527,18 @@
         "SubstitutionMap": Mapping[str, str],
         "Threshold": ThresholdTypeDef,
         "ColumnSelectors": Sequence[ColumnSelectorTypeDef],
     },
     total=False,
 )
 
+
 class RuleTypeDef(_RequiredRuleTypeDef, _OptionalRuleTypeDef):
     pass
 
-StatisticsConfigurationOutputTypeDef = TypedDict(
-    "StatisticsConfigurationOutputTypeDef",
-    {
-        "IncludedStatistics": List[str],
-        "Overrides": List[StatisticOverrideOutputTypeDef],
-    },
-    total=False,
-)
 
 StatisticsConfigurationTypeDef = TypedDict(
     "StatisticsConfigurationTypeDef",
     {
         "IncludedStatistics": Sequence[str],
         "Overrides": Sequence[StatisticOverrideTypeDef],
     },
@@ -1675,17 +1567,19 @@
     "_OptionalDatabaseOutputTypeDef",
     {
         "DatabaseOutputMode": Literal["NEW_TABLE"],
     },
     total=False,
 )
 
+
 class DatabaseOutputTypeDef(_RequiredDatabaseOutputTypeDef, _OptionalDatabaseOutputTypeDef):
     pass
 
+
 _RequiredDataCatalogOutputTypeDef = TypedDict(
     "_RequiredDataCatalogOutputTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
     },
 )
@@ -1696,19 +1590,21 @@
         "S3Options": S3TableOutputOptionsTypeDef,
         "DatabaseOptions": DatabaseTableOutputOptionsTypeDef,
         "Overwrite": bool,
     },
     total=False,
 )
 
+
 class DataCatalogOutputTypeDef(
     _RequiredDataCatalogOutputTypeDef, _OptionalDataCatalogOutputTypeDef
 ):
     pass
 
+
 ListProjectsResponseTypeDef = TypedDict(
     "ListProjectsResponseTypeDef",
     {
         "Projects": List[ProjectTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1729,51 +1625,65 @@
         "Overwrite": bool,
         "FormatOptions": OutputFormatOptionsTypeDef,
         "MaxOutputFiles": int,
     },
     total=False,
 )
 
+
 class OutputTypeDef(_RequiredOutputTypeDef, _OptionalOutputTypeDef):
     pass
 
-PathOptionsOutputTypeDef = TypedDict(
-    "PathOptionsOutputTypeDef",
-    {
-        "LastModifiedDateCondition": FilterExpressionOutputTypeDef,
-        "FilesLimit": FilesLimitTypeDef,
-        "Parameters": Dict[str, DatasetParameterOutputTypeDef],
-    },
-    total=False,
-)
 
 PathOptionsTypeDef = TypedDict(
     "PathOptionsTypeDef",
     {
         "LastModifiedDateCondition": FilterExpressionTypeDef,
         "FilesLimit": FilesLimitTypeDef,
         "Parameters": Mapping[str, DatasetParameterTypeDef],
     },
     total=False,
 )
 
-FormatOptionsUnionTypeDef = Union[FormatOptionsTypeDef, FormatOptionsOutputTypeDef]
+_RequiredCreateRecipeRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateRecipeRequestRequestTypeDef",
+    {
+        "Name": str,
+        "Steps": Sequence[RecipeStepTypeDef],
+    },
+)
+_OptionalCreateRecipeRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateRecipeRequestRequestTypeDef",
+    {
+        "Description": str,
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class CreateRecipeRequestRequestTypeDef(
+    _RequiredCreateRecipeRequestRequestTypeDef, _OptionalCreateRecipeRequestRequestTypeDef
+):
+    pass
+
+
 DescribeRecipeResponseTypeDef = TypedDict(
     "DescribeRecipeResponseTypeDef",
     {
         "CreatedBy": str,
         "CreateDate": datetime,
         "LastModifiedBy": str,
         "LastModifiedDate": datetime,
         "ProjectName": str,
         "PublishedBy": str,
         "PublishedDate": datetime,
         "Description": str,
         "Name": str,
-        "Steps": List[RecipeStepOutputTypeDef],
+        "Steps": List[RecipeStepTypeDef],
         "Tags": Dict[str, str],
         "ResourceArn": str,
         "RecipeVersion": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -1791,25 +1701,26 @@
         "LastModifiedBy": str,
         "LastModifiedDate": datetime,
         "ProjectName": str,
         "PublishedBy": str,
         "PublishedDate": datetime,
         "Description": str,
         "ResourceArn": str,
-        "Steps": List[RecipeStepOutputTypeDef],
+        "Steps": List[RecipeStepTypeDef],
         "Tags": Dict[str, str],
         "RecipeVersion": str,
     },
     total=False,
 )
 
+
 class RecipeTypeDef(_RequiredRecipeTypeDef, _OptionalRecipeTypeDef):
     pass
 
-RecipeStepUnionTypeDef = Union[RecipeStepTypeDef, RecipeStepOutputTypeDef]
+
 _RequiredSendProjectSessionActionRequestRequestTypeDef = TypedDict(
     "_RequiredSendProjectSessionActionRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalSendProjectSessionActionRequestRequestTypeDef = TypedDict(
@@ -1820,77 +1731,162 @@
         "StepIndex": int,
         "ClientSessionId": str,
         "ViewFrame": ViewFrameTypeDef,
     },
     total=False,
 )
 
+
 class SendProjectSessionActionRequestRequestTypeDef(
     _RequiredSendProjectSessionActionRequestRequestTypeDef,
     _OptionalSendProjectSessionActionRequestRequestTypeDef,
 ):
     pass
 
+
+_RequiredUpdateRecipeRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateRecipeRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalUpdateRecipeRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateRecipeRequestRequestTypeDef",
+    {
+        "Description": str,
+        "Steps": Sequence[RecipeStepTypeDef],
+    },
+    total=False,
+)
+
+
+class UpdateRecipeRequestRequestTypeDef(
+    _RequiredUpdateRecipeRequestRequestTypeDef, _OptionalUpdateRecipeRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredCreateRulesetRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateRulesetRequestRequestTypeDef",
+    {
+        "Name": str,
+        "TargetArn": str,
+        "Rules": Sequence[RuleTypeDef],
+    },
+)
+_OptionalCreateRulesetRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateRulesetRequestRequestTypeDef",
+    {
+        "Description": str,
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class CreateRulesetRequestRequestTypeDef(
+    _RequiredCreateRulesetRequestRequestTypeDef, _OptionalCreateRulesetRequestRequestTypeDef
+):
+    pass
+
+
 DescribeRulesetResponseTypeDef = TypedDict(
     "DescribeRulesetResponseTypeDef",
     {
         "Name": str,
         "Description": str,
         "TargetArn": str,
-        "Rules": List[RuleOutputTypeDef],
+        "Rules": List[RuleTypeDef],
         "CreateDate": datetime,
         "CreatedBy": str,
         "LastModifiedBy": str,
         "LastModifiedDate": datetime,
         "ResourceArn": str,
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RuleUnionTypeDef = Union[RuleTypeDef, RuleOutputTypeDef]
-_RequiredColumnStatisticsConfigurationOutputTypeDef = TypedDict(
-    "_RequiredColumnStatisticsConfigurationOutputTypeDef",
+_RequiredUpdateRulesetRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateRulesetRequestRequestTypeDef",
     {
-        "Statistics": StatisticsConfigurationOutputTypeDef,
+        "Name": str,
+        "Rules": Sequence[RuleTypeDef],
     },
 )
-_OptionalColumnStatisticsConfigurationOutputTypeDef = TypedDict(
-    "_OptionalColumnStatisticsConfigurationOutputTypeDef",
+_OptionalUpdateRulesetRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateRulesetRequestRequestTypeDef",
     {
-        "Selectors": List[ColumnSelectorTypeDef],
+        "Description": str,
     },
     total=False,
 )
 
-class ColumnStatisticsConfigurationOutputTypeDef(
-    _RequiredColumnStatisticsConfigurationOutputTypeDef,
-    _OptionalColumnStatisticsConfigurationOutputTypeDef,
+
+class UpdateRulesetRequestRequestTypeDef(
+    _RequiredUpdateRulesetRequestRequestTypeDef, _OptionalUpdateRulesetRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredColumnStatisticsConfigurationTypeDef = TypedDict(
     "_RequiredColumnStatisticsConfigurationTypeDef",
     {
         "Statistics": StatisticsConfigurationTypeDef,
     },
 )
 _OptionalColumnStatisticsConfigurationTypeDef = TypedDict(
     "_OptionalColumnStatisticsConfigurationTypeDef",
     {
         "Selectors": Sequence[ColumnSelectorTypeDef],
     },
     total=False,
 )
 
+
 class ColumnStatisticsConfigurationTypeDef(
     _RequiredColumnStatisticsConfigurationTypeDef, _OptionalColumnStatisticsConfigurationTypeDef
 ):
     pass
 
+
+_RequiredCreateRecipeJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateRecipeJobRequestRequestTypeDef",
+    {
+        "Name": str,
+        "RoleArn": str,
+    },
+)
+_OptionalCreateRecipeJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateRecipeJobRequestRequestTypeDef",
+    {
+        "DatasetName": str,
+        "EncryptionKeyArn": str,
+        "EncryptionMode": EncryptionModeType,
+        "LogSubscription": LogSubscriptionType,
+        "MaxCapacity": int,
+        "MaxRetries": int,
+        "Outputs": Sequence[OutputTypeDef],
+        "DataCatalogOutputs": Sequence[DataCatalogOutputTypeDef],
+        "DatabaseOutputs": Sequence[DatabaseOutputTypeDef],
+        "ProjectName": str,
+        "RecipeReference": RecipeReferenceTypeDef,
+        "Tags": Mapping[str, str],
+        "Timeout": int,
+    },
+    total=False,
+)
+
+
+class CreateRecipeJobRequestRequestTypeDef(
+    _RequiredCreateRecipeJobRequestRequestTypeDef, _OptionalCreateRecipeJobRequestRequestTypeDef
+):
+    pass
+
+
 JobRunTypeDef = TypedDict(
     "JobRunTypeDef",
     {
         "Attempt": int,
         "CompletedOn": datetime,
         "DatasetName": str,
         "ErrorMessage": str,
@@ -1944,89 +1940,123 @@
         "Tags": Dict[str, str],
         "JobSample": JobSampleTypeDef,
         "ValidationConfigurations": List[ValidationConfigurationTypeDef],
     },
     total=False,
 )
 
+
 class JobTypeDef(_RequiredJobTypeDef, _OptionalJobTypeDef):
     pass
 
-UnionTypeDef = Union[OutputTypeDef, OutputTypeDef]
+
+_RequiredUpdateRecipeJobRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateRecipeJobRequestRequestTypeDef",
+    {
+        "Name": str,
+        "RoleArn": str,
+    },
+)
+_OptionalUpdateRecipeJobRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateRecipeJobRequestRequestTypeDef",
+    {
+        "EncryptionKeyArn": str,
+        "EncryptionMode": EncryptionModeType,
+        "LogSubscription": LogSubscriptionType,
+        "MaxCapacity": int,
+        "MaxRetries": int,
+        "Outputs": Sequence[OutputTypeDef],
+        "DataCatalogOutputs": Sequence[DataCatalogOutputTypeDef],
+        "DatabaseOutputs": Sequence[DatabaseOutputTypeDef],
+        "Timeout": int,
+    },
+    total=False,
+)
+
+
+class UpdateRecipeJobRequestRequestTypeDef(
+    _RequiredUpdateRecipeJobRequestRequestTypeDef, _OptionalUpdateRecipeJobRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDatasetRequestRequestTypeDef",
+    {
+        "Name": str,
+        "Input": InputTypeDef,
+    },
+)
+_OptionalCreateDatasetRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDatasetRequestRequestTypeDef",
+    {
+        "Format": InputFormatType,
+        "FormatOptions": FormatOptionsTypeDef,
+        "PathOptions": PathOptionsTypeDef,
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class CreateDatasetRequestRequestTypeDef(
+    _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
+):
+    pass
+
+
 _RequiredDatasetTypeDef = TypedDict(
     "_RequiredDatasetTypeDef",
     {
         "Name": str,
         "Input": InputTypeDef,
     },
 )
 _OptionalDatasetTypeDef = TypedDict(
     "_OptionalDatasetTypeDef",
     {
         "AccountId": str,
         "CreatedBy": str,
         "CreateDate": datetime,
         "Format": InputFormatType,
-        "FormatOptions": FormatOptionsOutputTypeDef,
+        "FormatOptions": FormatOptionsTypeDef,
         "LastModifiedDate": datetime,
         "LastModifiedBy": str,
         "Source": SourceType,
-        "PathOptions": PathOptionsOutputTypeDef,
+        "PathOptions": PathOptionsTypeDef,
         "Tags": Dict[str, str],
         "ResourceArn": str,
     },
     total=False,
 )
 
+
 class DatasetTypeDef(_RequiredDatasetTypeDef, _OptionalDatasetTypeDef):
     pass
 
+
 DescribeDatasetResponseTypeDef = TypedDict(
     "DescribeDatasetResponseTypeDef",
     {
         "CreatedBy": str,
         "CreateDate": datetime,
         "Name": str,
         "Format": InputFormatType,
-        "FormatOptions": FormatOptionsOutputTypeDef,
+        "FormatOptions": FormatOptionsTypeDef,
         "Input": InputTypeDef,
         "LastModifiedDate": datetime,
         "LastModifiedBy": str,
         "Source": SourceType,
-        "PathOptions": PathOptionsOutputTypeDef,
+        "PathOptions": PathOptionsTypeDef,
         "Tags": Dict[str, str],
         "ResourceArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDatasetRequestRequestTypeDef",
-    {
-        "Name": str,
-        "Input": InputTypeDef,
-    },
-)
-_OptionalCreateDatasetRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDatasetRequestRequestTypeDef",
-    {
-        "Format": InputFormatType,
-        "FormatOptions": FormatOptionsTypeDef,
-        "PathOptions": PathOptionsTypeDef,
-        "Tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-class CreateDatasetRequestRequestTypeDef(
-    _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
-):
-    pass
-
-PathOptionsUnionTypeDef = Union[PathOptionsTypeDef, PathOptionsOutputTypeDef]
 _RequiredUpdateDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDatasetRequestRequestTypeDef",
     {
         "Name": str,
         "Input": InputTypeDef,
     },
 )
@@ -2036,19 +2066,21 @@
         "Format": InputFormatType,
         "FormatOptions": FormatOptionsTypeDef,
         "PathOptions": PathOptionsTypeDef,
     },
     total=False,
 )
 
+
 class UpdateDatasetRequestRequestTypeDef(
     _RequiredUpdateDatasetRequestRequestTypeDef, _OptionalUpdateDatasetRequestRequestTypeDef
 ):
     pass
 
+
 ListRecipeVersionsResponseTypeDef = TypedDict(
     "ListRecipeVersionsResponseTypeDef",
     {
         "NextToken": str,
         "Recipes": List[RecipeTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2059,108 +2091,14 @@
     {
         "Recipes": List[RecipeTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateRecipeRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateRecipeRequestRequestTypeDef",
-    {
-        "Name": str,
-        "Steps": Sequence[RecipeStepUnionTypeDef],
-    },
-)
-_OptionalCreateRecipeRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateRecipeRequestRequestTypeDef",
-    {
-        "Description": str,
-        "Tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-class CreateRecipeRequestRequestTypeDef(
-    _RequiredCreateRecipeRequestRequestTypeDef, _OptionalCreateRecipeRequestRequestTypeDef
-):
-    pass
-
-_RequiredUpdateRecipeRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateRecipeRequestRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalUpdateRecipeRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateRecipeRequestRequestTypeDef",
-    {
-        "Description": str,
-        "Steps": Sequence[RecipeStepUnionTypeDef],
-    },
-    total=False,
-)
-
-class UpdateRecipeRequestRequestTypeDef(
-    _RequiredUpdateRecipeRequestRequestTypeDef, _OptionalUpdateRecipeRequestRequestTypeDef
-):
-    pass
-
-_RequiredCreateRulesetRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateRulesetRequestRequestTypeDef",
-    {
-        "Name": str,
-        "TargetArn": str,
-        "Rules": Sequence[RuleUnionTypeDef],
-    },
-)
-_OptionalCreateRulesetRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateRulesetRequestRequestTypeDef",
-    {
-        "Description": str,
-        "Tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-class CreateRulesetRequestRequestTypeDef(
-    _RequiredCreateRulesetRequestRequestTypeDef, _OptionalCreateRulesetRequestRequestTypeDef
-):
-    pass
-
-_RequiredUpdateRulesetRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateRulesetRequestRequestTypeDef",
-    {
-        "Name": str,
-        "Rules": Sequence[RuleUnionTypeDef],
-    },
-)
-_OptionalUpdateRulesetRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateRulesetRequestRequestTypeDef",
-    {
-        "Description": str,
-    },
-    total=False,
-)
-
-class UpdateRulesetRequestRequestTypeDef(
-    _RequiredUpdateRulesetRequestRequestTypeDef, _OptionalUpdateRulesetRequestRequestTypeDef
-):
-    pass
-
-ProfileConfigurationOutputTypeDef = TypedDict(
-    "ProfileConfigurationOutputTypeDef",
-    {
-        "DatasetStatisticsConfiguration": StatisticsConfigurationOutputTypeDef,
-        "ProfileColumns": List[ColumnSelectorTypeDef],
-        "ColumnStatisticsConfigurations": List[ColumnStatisticsConfigurationOutputTypeDef],
-        "EntityDetectorConfiguration": EntityDetectorConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 ProfileConfigurationTypeDef = TypedDict(
     "ProfileConfigurationTypeDef",
     {
         "DatasetStatisticsConfiguration": StatisticsConfigurationTypeDef,
         "ProfileColumns": Sequence[ColumnSelectorTypeDef],
         "ColumnStatisticsConfigurations": Sequence[ColumnStatisticsConfigurationTypeDef],
         "EntityDetectorConfiguration": EntityDetectorConfigurationTypeDef,
@@ -2182,82 +2120,55 @@
     {
         "Jobs": List[JobTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateRecipeJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateRecipeJobRequestRequestTypeDef",
-    {
-        "Name": str,
-        "RoleArn": str,
-    },
-)
-_OptionalCreateRecipeJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateRecipeJobRequestRequestTypeDef",
+ListDatasetsResponseTypeDef = TypedDict(
+    "ListDatasetsResponseTypeDef",
     {
-        "DatasetName": str,
-        "EncryptionKeyArn": str,
-        "EncryptionMode": EncryptionModeType,
-        "LogSubscription": LogSubscriptionType,
-        "MaxCapacity": int,
-        "MaxRetries": int,
-        "Outputs": Sequence[UnionTypeDef],
-        "DataCatalogOutputs": Sequence[DataCatalogOutputTypeDef],
-        "DatabaseOutputs": Sequence[DatabaseOutputTypeDef],
-        "ProjectName": str,
-        "RecipeReference": RecipeReferenceTypeDef,
-        "Tags": Mapping[str, str],
-        "Timeout": int,
+        "Datasets": List[DatasetTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class CreateRecipeJobRequestRequestTypeDef(
-    _RequiredCreateRecipeJobRequestRequestTypeDef, _OptionalCreateRecipeJobRequestRequestTypeDef
-):
-    pass
-
-_RequiredUpdateRecipeJobRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateRecipeJobRequestRequestTypeDef",
+_RequiredCreateProfileJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateProfileJobRequestRequestTypeDef",
     {
+        "DatasetName": str,
         "Name": str,
+        "OutputLocation": S3LocationTypeDef,
         "RoleArn": str,
     },
 )
-_OptionalUpdateRecipeJobRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateRecipeJobRequestRequestTypeDef",
+_OptionalCreateProfileJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateProfileJobRequestRequestTypeDef",
     {
         "EncryptionKeyArn": str,
         "EncryptionMode": EncryptionModeType,
         "LogSubscription": LogSubscriptionType,
         "MaxCapacity": int,
         "MaxRetries": int,
-        "Outputs": Sequence[UnionTypeDef],
-        "DataCatalogOutputs": Sequence[DataCatalogOutputTypeDef],
-        "DatabaseOutputs": Sequence[DatabaseOutputTypeDef],
+        "Configuration": ProfileConfigurationTypeDef,
+        "ValidationConfigurations": Sequence[ValidationConfigurationTypeDef],
+        "Tags": Mapping[str, str],
         "Timeout": int,
+        "JobSample": JobSampleTypeDef,
     },
     total=False,
 )
 
-class UpdateRecipeJobRequestRequestTypeDef(
-    _RequiredUpdateRecipeJobRequestRequestTypeDef, _OptionalUpdateRecipeJobRequestRequestTypeDef
+
+class CreateProfileJobRequestRequestTypeDef(
+    _RequiredCreateProfileJobRequestRequestTypeDef, _OptionalCreateProfileJobRequestRequestTypeDef
 ):
     pass
 
-ListDatasetsResponseTypeDef = TypedDict(
-    "ListDatasetsResponseTypeDef",
-    {
-        "Datasets": List[DatasetTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
 DescribeJobResponseTypeDef = TypedDict(
     "DescribeJobResponseTypeDef",
     {
         "CreateDate": datetime,
         "CreatedBy": str,
         "DatasetName": str,
@@ -2270,15 +2181,15 @@
         "LogSubscription": LogSubscriptionType,
         "MaxCapacity": int,
         "MaxRetries": int,
         "Outputs": List[OutputTypeDef],
         "DataCatalogOutputs": List[DataCatalogOutputTypeDef],
         "DatabaseOutputs": List[DatabaseOutputTypeDef],
         "ProjectName": str,
-        "ProfileConfiguration": ProfileConfigurationOutputTypeDef,
+        "ProfileConfiguration": ProfileConfigurationTypeDef,
         "ValidationConfigurations": List[ValidationConfigurationTypeDef],
         "RecipeReference": RecipeReferenceTypeDef,
         "ResourceArn": str,
         "RoleArn": str,
         "Tags": Dict[str, str],
         "Timeout": int,
         "JobSample": JobSampleTypeDef,
@@ -2291,15 +2202,15 @@
     {
         "Attempt": int,
         "CompletedOn": datetime,
         "DatasetName": str,
         "ErrorMessage": str,
         "ExecutionTime": int,
         "JobName": str,
-        "ProfileConfiguration": ProfileConfigurationOutputTypeDef,
+        "ProfileConfiguration": ProfileConfigurationTypeDef,
         "ValidationConfigurations": List[ValidationConfigurationTypeDef],
         "RunId": str,
         "State": JobRunStateType,
         "LogSubscription": LogSubscriptionType,
         "LogGroupName": str,
         "Outputs": List[OutputTypeDef],
         "DataCatalogOutputs": List[DataCatalogOutputTypeDef],
@@ -2308,48 +2219,14 @@
         "StartedBy": str,
         "StartedOn": datetime,
         "JobSample": JobSampleTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateProfileJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateProfileJobRequestRequestTypeDef",
-    {
-        "DatasetName": str,
-        "Name": str,
-        "OutputLocation": S3LocationTypeDef,
-        "RoleArn": str,
-    },
-)
-_OptionalCreateProfileJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateProfileJobRequestRequestTypeDef",
-    {
-        "EncryptionKeyArn": str,
-        "EncryptionMode": EncryptionModeType,
-        "LogSubscription": LogSubscriptionType,
-        "MaxCapacity": int,
-        "MaxRetries": int,
-        "Configuration": ProfileConfigurationTypeDef,
-        "ValidationConfigurations": Sequence[ValidationConfigurationTypeDef],
-        "Tags": Mapping[str, str],
-        "Timeout": int,
-        "JobSample": JobSampleTypeDef,
-    },
-    total=False,
-)
-
-class CreateProfileJobRequestRequestTypeDef(
-    _RequiredCreateProfileJobRequestRequestTypeDef, _OptionalCreateProfileJobRequestRequestTypeDef
-):
-    pass
-
-ProfileConfigurationUnionTypeDef = Union[
-    ProfileConfigurationTypeDef, ProfileConfigurationOutputTypeDef
-]
 _RequiredUpdateProfileJobRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateProfileJobRequestRequestTypeDef",
     {
         "Name": str,
         "OutputLocation": S3LocationTypeDef,
         "RoleArn": str,
     },
@@ -2366,11 +2243,12 @@
         "ValidationConfigurations": Sequence[ValidationConfigurationTypeDef],
         "Timeout": int,
         "JobSample": JobSampleTypeDef,
     },
     total=False,
 )
 
+
 class UpdateProfileJobRequestRequestTypeDef(
     _RequiredUpdateProfileJobRequestRequestTypeDef, _OptionalUpdateProfileJobRequestRequestTypeDef
 ):
     pass
```

### Comparing `types-aiobotocore-databrew-2.5.2.post1/types_aiobotocore_databrew.egg-info/SOURCES.txt` & `types-aiobotocore-databrew-2.5.2.post2/types_aiobotocore_databrew.egg-info/SOURCES.txt`

 * *Files identical despite different names*

