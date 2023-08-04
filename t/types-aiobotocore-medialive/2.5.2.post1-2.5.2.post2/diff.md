# Comparing `tmp/types-aiobotocore-medialive-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-medialive-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-medialive-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:38 2023, max compression
+gzip compressed data, was "types-aiobotocore-medialive-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:17 2023, max compression
```

## Comparing `types-aiobotocore-medialive-2.5.2.post1.tar` & `types-aiobotocore-medialive-2.5.2.post2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:38.341527 types-aiobotocore-medialive-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:43:15.000000 types-aiobotocore-medialive-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    39082 2023-08-02 14:52:38.341527 types-aiobotocore-medialive-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    37556 2023-08-02 14:43:15.000000 types-aiobotocore-medialive-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:38.341527 types-aiobotocore-medialive-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-08-02 14:43:13.000000 types-aiobotocore-medialive-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:38.341527 types-aiobotocore-medialive-2.5.2.post1/types_aiobotocore_medialive/
--rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-08-02 14:43:15.000000 types-aiobotocore-medialive-2.5.2.post1/types_aiobotocore_medialive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-08-02 14:43:15.000000 types-aiobotocore-medialive-2.5.2.post1/types_aiobotocore_medialive/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-02 14:43:15.000000 types-aiobotocore-medialive-2.5.2.post1/types_aiobotocore_medialive/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    53894 2023-08-02 14:43:15.000000 types-aiobotocore-medialive-2.5.2.post1/types_aiobotocore_medialive/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    53805 2023-08-02 14:43:15.000000 types-aiobotocore-medialive-2.5.2.post1/types_aiobotocore_medialive/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    39348 2023-08-02 14:43:16.000000 types-aiobotocore-medialive-2.5.2.post1/types_aiobotocore_medialive/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    39346 2023-08-02 14:43:16.000000 types-aiobotocore-medialive-2.5.2.post1/types_aiobotocore_medialive/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12659 2023-08-02 14:43:15.000000 types-aiobotocore-medialive-2.5.2.post1/types_aiobotocore_medialive/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12647 2023-08-02 14:43:15.000000 types-aiobotocore-medialive-2.5.2.post1/types_aiobotocore_medialive/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:43:15.000000 types-aiobotocore-medialive-2.5.2.post1/types_aiobotocore_medialive/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   170963 2023-08-02 14:43:19.000000 types-aiobotocore-medialive-2.5.2.post1/types_aiobotocore_medialive/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   170786 2023-08-02 14:43:18.000000 types-aiobotocore-medialive-2.5.2.post1/types_aiobotocore_medialive/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:43:15.000000 types-aiobotocore-medialive-2.5.2.post1/types_aiobotocore_medialive/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-08-02 14:43:16.000000 types-aiobotocore-medialive-2.5.2.post1/types_aiobotocore_medialive/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11072 2023-08-02 14:43:15.000000 types-aiobotocore-medialive-2.5.2.post1/types_aiobotocore_medialive/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:38.341527 types-aiobotocore-medialive-2.5.2.post1/types_aiobotocore_medialive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    39082 2023-08-02 14:52:38.000000 types-aiobotocore-medialive-2.5.2.post1/types_aiobotocore_medialive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-08-02 14:52:38.000000 types-aiobotocore-medialive-2.5.2.post1/types_aiobotocore_medialive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:38.000000 types-aiobotocore-medialive-2.5.2.post1/types_aiobotocore_medialive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:38.000000 types-aiobotocore-medialive-2.5.2.post1/types_aiobotocore_medialive.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:38.000000 types-aiobotocore-medialive-2.5.2.post1/types_aiobotocore_medialive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-02 14:52:38.000000 types-aiobotocore-medialive-2.5.2.post1/types_aiobotocore_medialive.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:17.226643 types-aiobotocore-medialive-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:44:22.000000 types-aiobotocore-medialive-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    16214 2023-08-04 13:59:17.226643 types-aiobotocore-medialive-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14688 2023-08-04 13:44:22.000000 types-aiobotocore-medialive-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:17.226643 types-aiobotocore-medialive-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2086 2023-08-04 13:44:22.000000 types-aiobotocore-medialive-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:17.226643 types-aiobotocore-medialive-2.5.2.post2/types_aiobotocore_medialive/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     4506 2023-08-04 13:44:22.000000 types-aiobotocore-medialive-2.5.2.post2/types_aiobotocore_medialive/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     4505 2023-08-04 13:44:22.000000 types-aiobotocore-medialive-2.5.2.post2/types_aiobotocore_medialive/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      951 2023-08-04 13:44:22.000000 types-aiobotocore-medialive-2.5.2.post2/types_aiobotocore_medialive/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    55913 2023-08-04 13:44:23.000000 types-aiobotocore-medialive-2.5.2.post2/types_aiobotocore_medialive/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    55821 2023-08-04 13:44:23.000000 types-aiobotocore-medialive-2.5.2.post2/types_aiobotocore_medialive/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    39604 2023-08-04 13:44:25.000000 types-aiobotocore-medialive-2.5.2.post2/types_aiobotocore_medialive/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    39602 2023-08-04 13:44:23.000000 types-aiobotocore-medialive-2.5.2.post2/types_aiobotocore_medialive/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12659 2023-08-04 13:44:23.000000 types-aiobotocore-medialive-2.5.2.post2/types_aiobotocore_medialive/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12647 2023-08-04 13:44:23.000000 types-aiobotocore-medialive-2.5.2.post2/types_aiobotocore_medialive/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:44:22.000000 types-aiobotocore-medialive-2.5.2.post2/types_aiobotocore_medialive/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   149357 2023-08-04 13:44:30.000000 types-aiobotocore-medialive-2.5.2.post2/types_aiobotocore_medialive/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   149208 2023-08-04 13:44:27.000000 types-aiobotocore-medialive-2.5.2.post2/types_aiobotocore_medialive/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:44:22.000000 types-aiobotocore-medialive-2.5.2.post2/types_aiobotocore_medialive/version.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11083 2023-08-04 13:44:23.000000 types-aiobotocore-medialive-2.5.2.post2/types_aiobotocore_medialive/waiter.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11072 2023-08-04 13:44:23.000000 types-aiobotocore-medialive-2.5.2.post2/types_aiobotocore_medialive/waiter.pyi
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:17.226643 types-aiobotocore-medialive-2.5.2.post2/types_aiobotocore_medialive.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    16214 2023-08-04 13:59:17.000000 types-aiobotocore-medialive-2.5.2.post2/types_aiobotocore_medialive.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      928 2023-08-04 13:59:17.000000 types-aiobotocore-medialive-2.5.2.post2/types_aiobotocore_medialive.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:17.000000 types-aiobotocore-medialive-2.5.2.post2/types_aiobotocore_medialive.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:17.000000 types-aiobotocore-medialive-2.5.2.post2/types_aiobotocore_medialive.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:17.000000 types-aiobotocore-medialive-2.5.2.post2/types_aiobotocore_medialive.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       28 2023-08-04 13:59:17.000000 types-aiobotocore-medialive-2.5.2.post2/types_aiobotocore_medialive.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-medialive-2.5.2.post1/LICENSE` & `types-aiobotocore-medialive-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-medialive-2.5.2.post1/setup.py` & `types-aiobotocore-medialive-2.5.2.post2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-medialive",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_medialive"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.MediaLive 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-medialive-2.5.2.post1/types_aiobotocore_medialive/__init__.py` & `types-aiobotocore-medialive-2.5.2.post2/types_aiobotocore_medialive/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-medialive-2.5.2.post1/types_aiobotocore_medialive/__init__.pyi` & `types-aiobotocore-medialive-2.5.2.post2/types_aiobotocore_medialive/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-medialive-2.5.2.post1/types_aiobotocore_medialive/__main__.py` & `types-aiobotocore-medialive-2.5.2.post2/types_aiobotocore_medialive/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.MediaLive 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.MediaLive 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive\nOther"
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

### Comparing `types-aiobotocore-medialive-2.5.2.post1/types_aiobotocore_medialive/client.py` & `types-aiobotocore-medialive-2.5.2.post2/types_aiobotocore_medialive/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     ListInputsPaginator,
     ListMultiplexesPaginator,
     ListMultiplexProgramsPaginator,
     ListOfferingsPaginator,
     ListReservationsPaginator,
 )
 from .type_defs import (
+    AccountConfigurationTypeDef,
     BatchDeleteResponseTypeDef,
     BatchScheduleActionCreateRequestTypeDef,
     BatchScheduleActionDeleteRequestTypeDef,
     BatchStartResponseTypeDef,
     BatchStopResponseTypeDef,
     BatchUpdateScheduleResponseTypeDef,
     CdiInputSpecificationTypeDef,
@@ -47,27 +48,29 @@
     CreateMultiplexProgramResponseTypeDef,
     CreateMultiplexResponseTypeDef,
     CreatePartnerInputResponseTypeDef,
     DeleteChannelResponseTypeDef,
     DeleteMultiplexProgramResponseTypeDef,
     DeleteMultiplexResponseTypeDef,
     DeleteReservationResponseTypeDef,
+    DescribeAccountConfigurationResponseTypeDef,
     DescribeChannelResponseTypeDef,
     DescribeInputDeviceResponseTypeDef,
     DescribeInputDeviceThumbnailResponseTypeDef,
     DescribeInputResponseTypeDef,
     DescribeInputSecurityGroupResponseTypeDef,
     DescribeMultiplexProgramResponseTypeDef,
     DescribeMultiplexResponseTypeDef,
     DescribeOfferingResponseTypeDef,
     DescribeReservationResponseTypeDef,
     DescribeScheduleResponseTypeDef,
+    DescribeThumbnailsResponseTypeDef,
     EmptyResponseMetadataTypeDef,
-    EncoderSettingsUnionTypeDef,
-    InputAttachmentUnionTypeDef,
+    EncoderSettingsTypeDef,
+    InputAttachmentTypeDef,
     InputDestinationRequestTypeDef,
     InputDeviceConfigurableSettingsTypeDef,
     InputDeviceRequestTypeDef,
     InputDeviceSettingsTypeDef,
     InputSourceRequestTypeDef,
     InputSpecificationTypeDef,
     InputVpcRequestTypeDef,
@@ -83,21 +86,22 @@
     ListReservationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MaintenanceCreateSettingsTypeDef,
     MaintenanceUpdateSettingsTypeDef,
     MediaConnectFlowRequestTypeDef,
     MultiplexProgramSettingsTypeDef,
     MultiplexSettingsTypeDef,
-    OutputDestinationUnionTypeDef,
+    OutputDestinationTypeDef,
     PurchaseOfferingResponseTypeDef,
     RenewalSettingsTypeDef,
     StartChannelResponseTypeDef,
     StartMultiplexResponseTypeDef,
     StopChannelResponseTypeDef,
     StopMultiplexResponseTypeDef,
+    UpdateAccountConfigurationResponseTypeDef,
     UpdateChannelClassResponseTypeDef,
     UpdateChannelResponseTypeDef,
     UpdateInputDeviceResponseTypeDef,
     UpdateInputResponseTypeDef,
     UpdateInputSecurityGroupResponseTypeDef,
     UpdateMultiplexProgramResponseTypeDef,
     UpdateMultiplexResponseTypeDef,
@@ -259,17 +263,17 @@
         """
 
     async def create_channel(
         self,
         *,
         CdiInputSpecification: CdiInputSpecificationTypeDef = ...,
         ChannelClass: ChannelClassType = ...,
-        Destinations: Sequence[OutputDestinationUnionTypeDef] = ...,
-        EncoderSettings: EncoderSettingsUnionTypeDef = ...,
-        InputAttachments: Sequence[InputAttachmentUnionTypeDef] = ...,
+        Destinations: Sequence[OutputDestinationTypeDef] = ...,
+        EncoderSettings: EncoderSettingsTypeDef = ...,
+        InputAttachments: Sequence[InputAttachmentTypeDef] = ...,
         InputSpecification: InputSpecificationTypeDef = ...,
         LogLevel: LogLevelType = ...,
         Maintenance: MaintenanceCreateSettingsTypeDef = ...,
         Name: str = ...,
         RequestId: str = ...,
         Reserved: str = ...,
         RoleArn: str = ...,
@@ -441,14 +445,23 @@
         Removes tags for a resource See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/DeleteTags).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.delete_tags)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/client/#delete_tags)
         """
 
+    async def describe_account_configuration(self) -> DescribeAccountConfigurationResponseTypeDef:
+        """
+        Get account configuration See also: [AWS API
+        Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/DescribeAccountConfiguration).
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.describe_account_configuration)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/client/#describe_account_configuration)
+        """
+
     async def describe_channel(self, *, ChannelId: str) -> DescribeChannelResponseTypeDef:
         """
         Gets details about a channel See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/DescribeChannel).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.describe_channel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/client/#describe_channel)
@@ -538,14 +551,24 @@
         Get a channel schedule See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/DescribeSchedule).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.describe_schedule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/client/#describe_schedule)
         """
 
+    async def describe_thumbnails(
+        self, *, ChannelId: str, PipelineId: str, ThumbnailType: str
+    ) -> DescribeThumbnailsResponseTypeDef:
+        """
+        Describe the latest thumbnails data.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.describe_thumbnails)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/client/#describe_thumbnails)
+        """
+
     async def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
@@ -774,22 +797,33 @@
         """
         Start an input device transfer to another AWS account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.transfer_input_device)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/client/#transfer_input_device)
         """
 
+    async def update_account_configuration(
+        self, *, AccountConfiguration: AccountConfigurationTypeDef = ...
+    ) -> UpdateAccountConfigurationResponseTypeDef:
+        """
+        Update account configuration See also: [AWS API
+        Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/UpdateAccountConfiguration).
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.update_account_configuration)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/client/#update_account_configuration)
+        """
+
     async def update_channel(
         self,
         *,
         ChannelId: str,
         CdiInputSpecification: CdiInputSpecificationTypeDef = ...,
-        Destinations: Sequence[OutputDestinationUnionTypeDef] = ...,
-        EncoderSettings: EncoderSettingsUnionTypeDef = ...,
-        InputAttachments: Sequence[InputAttachmentUnionTypeDef] = ...,
+        Destinations: Sequence[OutputDestinationTypeDef] = ...,
+        EncoderSettings: EncoderSettingsTypeDef = ...,
+        InputAttachments: Sequence[InputAttachmentTypeDef] = ...,
         InputSpecification: InputSpecificationTypeDef = ...,
         LogLevel: LogLevelType = ...,
         Maintenance: MaintenanceUpdateSettingsTypeDef = ...,
         Name: str = ...,
         RoleArn: str = ...
     ) -> UpdateChannelResponseTypeDef:
         """
@@ -800,15 +834,15 @@
         """
 
     async def update_channel_class(
         self,
         *,
         ChannelClass: ChannelClassType,
         ChannelId: str,
-        Destinations: Sequence[OutputDestinationUnionTypeDef] = ...
+        Destinations: Sequence[OutputDestinationTypeDef] = ...
     ) -> UpdateChannelClassResponseTypeDef:
         """
         Changes the class of the channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.update_channel_class)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/client/#update_channel_class)
         """
@@ -834,15 +868,16 @@
 
     async def update_input_device(
         self,
         *,
         InputDeviceId: str,
         HdDeviceSettings: InputDeviceConfigurableSettingsTypeDef = ...,
         Name: str = ...,
-        UhdDeviceSettings: InputDeviceConfigurableSettingsTypeDef = ...
+        UhdDeviceSettings: InputDeviceConfigurableSettingsTypeDef = ...,
+        AvailabilityZone: str = ...
     ) -> UpdateInputDeviceResponseTypeDef:
         """
         Updates the parameters for the input device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.update_input_device)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/client/#update_input_device)
         """
```

### Comparing `types-aiobotocore-medialive-2.5.2.post1/types_aiobotocore_medialive/client.pyi` & `types-aiobotocore-medialive-2.5.2.post2/types_aiobotocore_medialive/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     ListInputsPaginator,
     ListMultiplexesPaginator,
     ListMultiplexProgramsPaginator,
     ListOfferingsPaginator,
     ListReservationsPaginator,
 )
 from .type_defs import (
+    AccountConfigurationTypeDef,
     BatchDeleteResponseTypeDef,
     BatchScheduleActionCreateRequestTypeDef,
     BatchScheduleActionDeleteRequestTypeDef,
     BatchStartResponseTypeDef,
     BatchStopResponseTypeDef,
     BatchUpdateScheduleResponseTypeDef,
     CdiInputSpecificationTypeDef,
@@ -47,27 +48,29 @@
     CreateMultiplexProgramResponseTypeDef,
     CreateMultiplexResponseTypeDef,
     CreatePartnerInputResponseTypeDef,
     DeleteChannelResponseTypeDef,
     DeleteMultiplexProgramResponseTypeDef,
     DeleteMultiplexResponseTypeDef,
     DeleteReservationResponseTypeDef,
+    DescribeAccountConfigurationResponseTypeDef,
     DescribeChannelResponseTypeDef,
     DescribeInputDeviceResponseTypeDef,
     DescribeInputDeviceThumbnailResponseTypeDef,
     DescribeInputResponseTypeDef,
     DescribeInputSecurityGroupResponseTypeDef,
     DescribeMultiplexProgramResponseTypeDef,
     DescribeMultiplexResponseTypeDef,
     DescribeOfferingResponseTypeDef,
     DescribeReservationResponseTypeDef,
     DescribeScheduleResponseTypeDef,
+    DescribeThumbnailsResponseTypeDef,
     EmptyResponseMetadataTypeDef,
-    EncoderSettingsUnionTypeDef,
-    InputAttachmentUnionTypeDef,
+    EncoderSettingsTypeDef,
+    InputAttachmentTypeDef,
     InputDestinationRequestTypeDef,
     InputDeviceConfigurableSettingsTypeDef,
     InputDeviceRequestTypeDef,
     InputDeviceSettingsTypeDef,
     InputSourceRequestTypeDef,
     InputSpecificationTypeDef,
     InputVpcRequestTypeDef,
@@ -83,21 +86,22 @@
     ListReservationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MaintenanceCreateSettingsTypeDef,
     MaintenanceUpdateSettingsTypeDef,
     MediaConnectFlowRequestTypeDef,
     MultiplexProgramSettingsTypeDef,
     MultiplexSettingsTypeDef,
-    OutputDestinationUnionTypeDef,
+    OutputDestinationTypeDef,
     PurchaseOfferingResponseTypeDef,
     RenewalSettingsTypeDef,
     StartChannelResponseTypeDef,
     StartMultiplexResponseTypeDef,
     StopChannelResponseTypeDef,
     StopMultiplexResponseTypeDef,
+    UpdateAccountConfigurationResponseTypeDef,
     UpdateChannelClassResponseTypeDef,
     UpdateChannelResponseTypeDef,
     UpdateInputDeviceResponseTypeDef,
     UpdateInputResponseTypeDef,
     UpdateInputSecurityGroupResponseTypeDef,
     UpdateMultiplexProgramResponseTypeDef,
     UpdateMultiplexResponseTypeDef,
@@ -245,17 +249,17 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/client/#close)
         """
     async def create_channel(
         self,
         *,
         CdiInputSpecification: CdiInputSpecificationTypeDef = ...,
         ChannelClass: ChannelClassType = ...,
-        Destinations: Sequence[OutputDestinationUnionTypeDef] = ...,
-        EncoderSettings: EncoderSettingsUnionTypeDef = ...,
-        InputAttachments: Sequence[InputAttachmentUnionTypeDef] = ...,
+        Destinations: Sequence[OutputDestinationTypeDef] = ...,
+        EncoderSettings: EncoderSettingsTypeDef = ...,
+        InputAttachments: Sequence[InputAttachmentTypeDef] = ...,
         InputSpecification: InputSpecificationTypeDef = ...,
         LogLevel: LogLevelType = ...,
         Maintenance: MaintenanceCreateSettingsTypeDef = ...,
         Name: str = ...,
         RequestId: str = ...,
         Reserved: str = ...,
         RoleArn: str = ...,
@@ -412,14 +416,22 @@
         """
         Removes tags for a resource See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/DeleteTags).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.delete_tags)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/client/#delete_tags)
         """
+    async def describe_account_configuration(self) -> DescribeAccountConfigurationResponseTypeDef:
+        """
+        Get account configuration See also: [AWS API
+        Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/DescribeAccountConfiguration).
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.describe_account_configuration)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/client/#describe_account_configuration)
+        """
     async def describe_channel(self, *, ChannelId: str) -> DescribeChannelResponseTypeDef:
         """
         Gets details about a channel See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/DescribeChannel).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.describe_channel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/client/#describe_channel)
@@ -499,14 +511,23 @@
         """
         Get a channel schedule See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/DescribeSchedule).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.describe_schedule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/client/#describe_schedule)
         """
+    async def describe_thumbnails(
+        self, *, ChannelId: str, PipelineId: str, ThumbnailType: str
+    ) -> DescribeThumbnailsResponseTypeDef:
+        """
+        Describe the latest thumbnails data.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.describe_thumbnails)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/client/#describe_thumbnails)
+        """
     async def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
@@ -715,22 +736,32 @@
     ) -> Dict[str, Any]:
         """
         Start an input device transfer to another AWS account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.transfer_input_device)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/client/#transfer_input_device)
         """
+    async def update_account_configuration(
+        self, *, AccountConfiguration: AccountConfigurationTypeDef = ...
+    ) -> UpdateAccountConfigurationResponseTypeDef:
+        """
+        Update account configuration See also: [AWS API
+        Documentation](https://docs.aws.amazon.com/goto/WebAPI/medialive-2017-10-14/UpdateAccountConfiguration).
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.update_account_configuration)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/client/#update_account_configuration)
+        """
     async def update_channel(
         self,
         *,
         ChannelId: str,
         CdiInputSpecification: CdiInputSpecificationTypeDef = ...,
-        Destinations: Sequence[OutputDestinationUnionTypeDef] = ...,
-        EncoderSettings: EncoderSettingsUnionTypeDef = ...,
-        InputAttachments: Sequence[InputAttachmentUnionTypeDef] = ...,
+        Destinations: Sequence[OutputDestinationTypeDef] = ...,
+        EncoderSettings: EncoderSettingsTypeDef = ...,
+        InputAttachments: Sequence[InputAttachmentTypeDef] = ...,
         InputSpecification: InputSpecificationTypeDef = ...,
         LogLevel: LogLevelType = ...,
         Maintenance: MaintenanceUpdateSettingsTypeDef = ...,
         Name: str = ...,
         RoleArn: str = ...
     ) -> UpdateChannelResponseTypeDef:
         """
@@ -740,15 +771,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/client/#update_channel)
         """
     async def update_channel_class(
         self,
         *,
         ChannelClass: ChannelClassType,
         ChannelId: str,
-        Destinations: Sequence[OutputDestinationUnionTypeDef] = ...
+        Destinations: Sequence[OutputDestinationTypeDef] = ...
     ) -> UpdateChannelClassResponseTypeDef:
         """
         Changes the class of the channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.update_channel_class)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/client/#update_channel_class)
         """
@@ -772,15 +803,16 @@
         """
     async def update_input_device(
         self,
         *,
         InputDeviceId: str,
         HdDeviceSettings: InputDeviceConfigurableSettingsTypeDef = ...,
         Name: str = ...,
-        UhdDeviceSettings: InputDeviceConfigurableSettingsTypeDef = ...
+        UhdDeviceSettings: InputDeviceConfigurableSettingsTypeDef = ...,
+        AvailabilityZone: str = ...
     ) -> UpdateInputDeviceResponseTypeDef:
         """
         Updates the parameters for the input device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.update_input_device)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medialive/client/#update_input_device)
         """
```

### Comparing `types-aiobotocore-medialive-2.5.2.post1/types_aiobotocore_medialive/literals.py` & `types-aiobotocore-medialive-2.5.2.post2/types_aiobotocore_medialive/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -291,14 +291,16 @@
     "SmoothGroupSegmentationModeType",
     "SmoothGroupSparseTrackTypeType",
     "SmoothGroupStreamManifestBehaviorType",
     "SmoothGroupTimestampOffsetModeType",
     "Smpte2038DataPreferenceType",
     "TemporalFilterPostFilterSharpeningType",
     "TemporalFilterStrengthType",
+    "ThumbnailStateType",
+    "ThumbnailTypeType",
     "TimecodeBurninFontSizeType",
     "TimecodeBurninPositionType",
     "TimecodeConfigSourceType",
     "TtmlDestinationStyleControlType",
     "UdpTimedMetadataId3FrameType",
     "VideoDescriptionRespondToAfdType",
     "VideoDescriptionScalingBehaviorType",
@@ -749,14 +751,16 @@
     "STRENGTH_4",
     "STRENGTH_5",
     "STRENGTH_6",
     "STRENGTH_7",
     "STRENGTH_8",
     "STRENGTH_9",
 ]
+ThumbnailStateType = Literal["AUTO", "DISABLED"]
+ThumbnailTypeType = Literal["CURRENT_ACTIVE", "UNSPECIFIED"]
 TimecodeBurninFontSizeType = Literal["EXTRA_SMALL_10", "LARGE_48", "MEDIUM_32", "SMALL_16"]
 TimecodeBurninPositionType = Literal[
     "BOTTOM_CENTER",
     "BOTTOM_LEFT",
     "BOTTOM_RIGHT",
     "MIDDLE_CENTER",
     "MIDDLE_LEFT",
@@ -788,14 +792,15 @@
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
@@ -891,14 +896,15 @@
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
@@ -977,26 +983,28 @@
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

### Comparing `types-aiobotocore-medialive-2.5.2.post1/types_aiobotocore_medialive/literals.pyi` & `types-aiobotocore-medialive-2.5.2.post2/types_aiobotocore_medialive/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -290,14 +290,16 @@
     "SmoothGroupSegmentationModeType",
     "SmoothGroupSparseTrackTypeType",
     "SmoothGroupStreamManifestBehaviorType",
     "SmoothGroupTimestampOffsetModeType",
     "Smpte2038DataPreferenceType",
     "TemporalFilterPostFilterSharpeningType",
     "TemporalFilterStrengthType",
+    "ThumbnailStateType",
+    "ThumbnailTypeType",
     "TimecodeBurninFontSizeType",
     "TimecodeBurninPositionType",
     "TimecodeConfigSourceType",
     "TtmlDestinationStyleControlType",
     "UdpTimedMetadataId3FrameType",
     "VideoDescriptionRespondToAfdType",
     "VideoDescriptionScalingBehaviorType",
@@ -747,14 +749,16 @@
     "STRENGTH_4",
     "STRENGTH_5",
     "STRENGTH_6",
     "STRENGTH_7",
     "STRENGTH_8",
     "STRENGTH_9",
 ]
+ThumbnailStateType = Literal["AUTO", "DISABLED"]
+ThumbnailTypeType = Literal["CURRENT_ACTIVE", "UNSPECIFIED"]
 TimecodeBurninFontSizeType = Literal["EXTRA_SMALL_10", "LARGE_48", "MEDIUM_32", "SMALL_16"]
 TimecodeBurninPositionType = Literal[
     "BOTTOM_CENTER",
     "BOTTOM_LEFT",
     "BOTTOM_RIGHT",
     "MIDDLE_CENTER",
     "MIDDLE_LEFT",
@@ -786,14 +790,15 @@
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
@@ -889,14 +894,15 @@
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
@@ -975,26 +981,28 @@
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

### Comparing `types-aiobotocore-medialive-2.5.2.post1/types_aiobotocore_medialive/paginator.py` & `types-aiobotocore-medialive-2.5.2.post2/types_aiobotocore_medialive/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-medialive-2.5.2.post1/types_aiobotocore_medialive/paginator.pyi` & `types-aiobotocore-medialive-2.5.2.post2/types_aiobotocore_medialive/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-medialive-2.5.2.post1/types_aiobotocore_medialive/type_defs.py` & `types-aiobotocore-medialive-2.5.2.post2/types_aiobotocore_medialive/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_medialive.type_defs import AacSettingsTypeDef
 
     data: AacSettingsTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Any, Dict, List, Mapping, Sequence, Union
+from typing import Any, Dict, List, Mapping, Sequence
 
 from aiobotocore.response import StreamingBody
 
 from .literals import (
     AacCodingModeType,
     AacInputTypeType,
     AacProfileType,
@@ -261,14 +261,16 @@
     SmoothGroupSegmentationModeType,
     SmoothGroupSparseTrackTypeType,
     SmoothGroupStreamManifestBehaviorType,
     SmoothGroupTimestampOffsetModeType,
     Smpte2038DataPreferenceType,
     TemporalFilterPostFilterSharpeningType,
     TemporalFilterStrengthType,
+    ThumbnailStateType,
+    ThumbnailTypeType,
     TimecodeBurninFontSizeType,
     TimecodeBurninPositionType,
     TimecodeConfigSourceType,
     TtmlDestinationStyleControlType,
     UdpTimedMetadataId3FrameType,
     VideoDescriptionRespondToAfdType,
     VideoDescriptionScalingBehaviorType,
@@ -288,14 +290,15 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AacSettingsTypeDef",
     "Ac3SettingsTypeDef",
     "AcceptInputDeviceTransferRequestRequestTypeDef",
+    "AccountConfigurationTypeDef",
     "AncillarySourceSettingsTypeDef",
     "ArchiveS3SettingsTypeDef",
     "OutputLocationRefTypeDef",
     "InputChannelLevelTypeDef",
     "Eac3AtmosSettingsTypeDef",
     "Eac3SettingsTypeDef",
     "Mp2SettingsTypeDef",
@@ -372,30 +375,31 @@
     "InputWhitelistRuleTypeDef",
     "DescribeMultiplexProgramRequestRequestTypeDef",
     "DescribeMultiplexRequestRequestTypeDef",
     "DescribeOfferingRequestRequestTypeDef",
     "DescribeReservationRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeScheduleRequestRequestTypeDef",
+    "DescribeThumbnailsRequestRequestTypeDef",
     "DvbNitSettingsTypeDef",
     "DvbSdtSettingsTypeDef",
     "DvbTdtSettingsTypeDef",
     "FeatureActivationsTypeDef",
     "NielsenConfigurationTypeDef",
+    "ThumbnailConfigurationTypeDef",
     "TimecodeConfigTypeDef",
     "InputLossFailoverSettingsTypeDef",
     "VideoBlackFailoverSettingsTypeDef",
     "FecOutputSettingsTypeDef",
     "FixedModeScheduleActionStartSettingsTypeDef",
     "Fmp4HlsSettingsTypeDef",
     "FollowModeScheduleActionStartSettingsTypeDef",
     "FrameCaptureS3SettingsTypeDef",
     "FrameCaptureOutputSettingsTypeDef",
     "TimecodeBurninSettingsTypeDef",
-    "H264ColorSpaceSettingsOutputTypeDef",
     "H264ColorSpaceSettingsTypeDef",
     "TemporalFilterSettingsTypeDef",
     "Hdr10SettingsTypeDef",
     "HlsAkamaiSettingsTypeDef",
     "HlsBasicPutSettingsTypeDef",
     "HlsMediaStoreSettingsTypeDef",
     "HlsS3SettingsTypeDef",
@@ -420,70 +424,69 @@
     "ListOfferingsRequestRequestTypeDef",
     "ListReservationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "M3u8SettingsTypeDef",
     "MaintenanceUpdateSettingsTypeDef",
     "MediaPackageOutputDestinationSettingsTypeDef",
     "MotionGraphicsActivateScheduleActionSettingsTypeDef",
-    "MotionGraphicsSettingsOutputTypeDef",
     "MotionGraphicsSettingsTypeDef",
     "MsSmoothOutputSettingsTypeDef",
     "MultiplexMediaConnectOutputDestinationSettingsTypeDef",
     "MultiplexProgramChannelDestinationSettingsTypeDef",
     "MultiplexProgramServiceDescriptorTypeDef",
     "MultiplexSettingsSummaryTypeDef",
     "MultiplexStatmuxVideoSettingsTypeDef",
     "NielsenCBETTypeDef",
     "NielsenNaesIiNwTypeDef",
     "OutputDestinationSettingsTypeDef",
-    "RtmpGroupSettingsOutputTypeDef",
-    "UdpGroupSettingsTypeDef",
     "RtmpGroupSettingsTypeDef",
+    "UdpGroupSettingsTypeDef",
     "PipelinePauseStateSettingsTypeDef",
     "RebootInputDeviceRequestRequestTypeDef",
     "RejectInputDeviceTransferRequestRequestTypeDef",
     "Scte35InputScheduleActionSettingsTypeDef",
     "Scte35ReturnToNetworkScheduleActionSettingsTypeDef",
     "Scte35SpliceInsertScheduleActionSettingsTypeDef",
     "StaticImageDeactivateScheduleActionSettingsTypeDef",
     "Scte35DeliveryRestrictionsTypeDef",
     "StartChannelRequestRequestTypeDef",
     "StartInputDeviceMaintenanceWindowRequestRequestTypeDef",
     "StartMultiplexRequestRequestTypeDef",
     "StopChannelRequestRequestTypeDef",
     "StopMultiplexRequestRequestTypeDef",
+    "ThumbnailTypeDef",
     "TransferInputDeviceRequestRequestTypeDef",
     "VideoSelectorPidTypeDef",
     "VideoSelectorProgramIdTypeDef",
+    "UpdateAccountConfigurationRequestRequestTypeDef",
     "ArchiveCdnSettingsTypeDef",
     "MediaPackageGroupSettingsTypeDef",
     "MsSmoothGroupSettingsTypeDef",
     "MultiplexOutputSettingsTypeDef",
     "RtmpOutputSettingsTypeDef",
-    "AudioChannelMappingOutputTypeDef",
     "AudioChannelMappingTypeDef",
-    "AudioCodecSettingsOutputTypeDef",
     "AudioCodecSettingsTypeDef",
     "AudioOnlyHlsSettingsTypeDef",
     "AvailBlankingTypeDef",
     "BlackoutSlateTypeDef",
     "BurnInDestinationSettingsTypeDef",
     "DvbSubDestinationSettingsTypeDef",
     "InputLossBehaviorTypeDef",
     "StaticImageActivateScheduleActionSettingsTypeDef",
     "StaticKeySettingsTypeDef",
-    "AudioTrackSelectionOutputTypeDef",
     "AudioTrackSelectionTypeDef",
     "AvailSettingsTypeDef",
     "BatchDeleteResponseTypeDef",
     "BatchStartResponseTypeDef",
     "BatchStopResponseTypeDef",
+    "DescribeAccountConfigurationResponseTypeDef",
     "DescribeInputDeviceThumbnailResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "UpdateAccountConfigurationResponseTypeDef",
     "TeletextSourceSettingsTypeDef",
     "CreateInputRequestRequestTypeDef",
     "CreateInputSecurityGroupRequestRequestTypeDef",
     "UpdateInputSecurityGroupRequestRequestTypeDef",
     "CreateMultiplexRequestRequestTypeDef",
     "UpdateMultiplexRequestRequestTypeDef",
     "PurchaseOfferingRequestRequestTypeDef",
@@ -517,161 +520,131 @@
     "ListInputsRequestListInputsPaginateTypeDef",
     "ListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef",
     "ListMultiplexesRequestListMultiplexesPaginateTypeDef",
     "ListOfferingsRequestListOfferingsPaginateTypeDef",
     "ListReservationsRequestListReservationsPaginateTypeDef",
     "M2tsSettingsTypeDef",
     "FailoverConditionSettingsTypeDef",
-    "ScheduleActionStartSettingsOutputTypeDef",
     "ScheduleActionStartSettingsTypeDef",
     "FrameCaptureCdnSettingsTypeDef",
     "FrameCaptureSettingsTypeDef",
     "H264FilterSettingsTypeDef",
     "H265FilterSettingsTypeDef",
     "Mpeg2FilterSettingsTypeDef",
-    "H265ColorSpaceSettingsOutputTypeDef",
     "H265ColorSpaceSettingsTypeDef",
     "VideoSelectorColorSpaceSettingsTypeDef",
     "HlsCdnSettingsTypeDef",
     "NetworkInputSettingsTypeDef",
     "InputClippingSettingsTypeDef",
     "InputDestinationTypeDef",
     "UpdateInputDeviceRequestRequestTypeDef",
     "UpdateInputRequestRequestTypeDef",
     "ListInputDeviceTransfersResponseTypeDef",
     "ListMultiplexProgramsResponseTypeDef",
     "StandardHlsSettingsTypeDef",
-    "MotionGraphicsConfigurationOutputTypeDef",
     "MotionGraphicsConfigurationTypeDef",
     "MultiplexOutputDestinationTypeDef",
     "MultiplexSummaryTypeDef",
     "MultiplexVideoSettingsTypeDef",
     "NielsenWatermarksSettingsTypeDef",
-    "OutputDestinationOutputTypeDef",
     "OutputDestinationTypeDef",
-    "PauseStateScheduleActionSettingsOutputTypeDef",
     "PauseStateScheduleActionSettingsTypeDef",
     "Scte35SegmentationDescriptorTypeDef",
+    "ThumbnailDetailTypeDef",
     "VideoSelectorSettingsTypeDef",
     "ArchiveGroupSettingsTypeDef",
-    "RemixSettingsOutputTypeDef",
     "RemixSettingsTypeDef",
-    "CaptionDestinationSettingsOutputTypeDef",
     "CaptionDestinationSettingsTypeDef",
     "GlobalConfigurationTypeDef",
     "KeyProviderSettingsTypeDef",
-    "AudioSelectorSettingsOutputTypeDef",
     "AudioSelectorSettingsTypeDef",
     "AvailConfigurationTypeDef",
-    "CaptionSelectorSettingsOutputTypeDef",
     "CaptionSelectorSettingsTypeDef",
     "ListOfferingsResponseTypeDef",
     "ListReservationsResponseTypeDef",
     "PurchaseOfferingResponseTypeDef",
     "UpdateReservationResponseTypeDef",
     "ListInputDevicesResponseTypeDef",
     "CreateInputSecurityGroupResponseTypeDef",
     "ListInputSecurityGroupsResponseTypeDef",
     "UpdateInputSecurityGroupResponseTypeDef",
     "ArchiveContainerSettingsTypeDef",
     "UdpContainerSettingsTypeDef",
     "FailoverConditionTypeDef",
     "FrameCaptureGroupSettingsTypeDef",
-    "H264SettingsOutputTypeDef",
     "H264SettingsTypeDef",
     "Mpeg2SettingsTypeDef",
-    "H265SettingsOutputTypeDef",
     "H265SettingsTypeDef",
-    "InputPrepareScheduleActionSettingsOutputTypeDef",
     "InputPrepareScheduleActionSettingsTypeDef",
-    "InputSwitchScheduleActionSettingsOutputTypeDef",
     "InputSwitchScheduleActionSettingsTypeDef",
     "DescribeInputResponseTypeDef",
     "InputTypeDef",
     "HlsSettingsTypeDef",
     "DeleteMultiplexResponseTypeDef",
     "DescribeMultiplexResponseTypeDef",
     "MultiplexTypeDef",
     "StartMultiplexResponseTypeDef",
     "StopMultiplexResponseTypeDef",
     "ListMultiplexesResponseTypeDef",
     "MultiplexProgramSettingsTypeDef",
     "AudioWatermarkSettingsTypeDef",
-    "OutputDestinationUnionTypeDef",
+    "UpdateChannelClassRequestRequestTypeDef",
     "Scte35DescriptorSettingsTypeDef",
+    "DescribeThumbnailsResponseTypeDef",
     "VideoSelectorTypeDef",
-    "CaptionDescriptionOutputTypeDef",
     "CaptionDescriptionTypeDef",
-    "HlsGroupSettingsOutputTypeDef",
     "HlsGroupSettingsTypeDef",
-    "AudioSelectorOutputTypeDef",
     "AudioSelectorTypeDef",
-    "CaptionSelectorOutputTypeDef",
     "CaptionSelectorTypeDef",
     "ArchiveOutputSettingsTypeDef",
     "UdpOutputSettingsTypeDef",
-    "AutomaticInputFailoverSettingsOutputTypeDef",
     "AutomaticInputFailoverSettingsTypeDef",
-    "VideoCodecSettingsOutputTypeDef",
     "VideoCodecSettingsTypeDef",
     "CreateInputResponseTypeDef",
     "CreatePartnerInputResponseTypeDef",
     "ListInputsResponseTypeDef",
     "UpdateInputResponseTypeDef",
     "HlsOutputSettingsTypeDef",
     "CreateMultiplexResponseTypeDef",
     "UpdateMultiplexResponseTypeDef",
     "CreateMultiplexProgramRequestRequestTypeDef",
     "DeleteMultiplexProgramResponseTypeDef",
     "DescribeMultiplexProgramResponseTypeDef",
     "MultiplexProgramTypeDef",
     "UpdateMultiplexProgramRequestRequestTypeDef",
-    "AudioDescriptionOutputTypeDef",
     "AudioDescriptionTypeDef",
-    "UpdateChannelClassRequestRequestTypeDef",
     "Scte35DescriptorTypeDef",
-    "OutputGroupSettingsOutputTypeDef",
     "OutputGroupSettingsTypeDef",
-    "InputSettingsOutputTypeDef",
     "InputSettingsTypeDef",
-    "VideoDescriptionOutputTypeDef",
     "VideoDescriptionTypeDef",
     "OutputSettingsTypeDef",
     "CreateMultiplexProgramResponseTypeDef",
     "UpdateMultiplexProgramResponseTypeDef",
-    "Scte35TimeSignalScheduleActionSettingsOutputTypeDef",
     "Scte35TimeSignalScheduleActionSettingsTypeDef",
-    "InputAttachmentOutputTypeDef",
     "InputAttachmentTypeDef",
     "OutputTypeDef",
-    "ScheduleActionSettingsOutputTypeDef",
     "ScheduleActionSettingsTypeDef",
     "ChannelSummaryTypeDef",
-    "InputAttachmentUnionTypeDef",
-    "OutputGroupOutputTypeDef",
     "OutputGroupTypeDef",
-    "ScheduleActionOutputTypeDef",
     "ScheduleActionTypeDef",
     "ListChannelsResponseTypeDef",
-    "EncoderSettingsOutputTypeDef",
     "EncoderSettingsTypeDef",
+    "BatchScheduleActionCreateRequestTypeDef",
     "BatchScheduleActionCreateResultTypeDef",
     "BatchScheduleActionDeleteResultTypeDef",
     "DescribeScheduleResponseTypeDef",
-    "BatchScheduleActionCreateRequestTypeDef",
     "ChannelTypeDef",
+    "CreateChannelRequestRequestTypeDef",
     "DeleteChannelResponseTypeDef",
     "DescribeChannelResponseTypeDef",
     "StartChannelResponseTypeDef",
     "StopChannelResponseTypeDef",
-    "CreateChannelRequestRequestTypeDef",
-    "EncoderSettingsUnionTypeDef",
     "UpdateChannelRequestRequestTypeDef",
-    "BatchUpdateScheduleResponseTypeDef",
     "BatchUpdateScheduleRequestRequestTypeDef",
+    "BatchUpdateScheduleResponseTypeDef",
     "CreateChannelResponseTypeDef",
     "UpdateChannelClassResponseTypeDef",
     "UpdateChannelResponseTypeDef",
 )
 
 AacSettingsTypeDef = TypedDict(
     "AacSettingsTypeDef",
@@ -706,14 +679,22 @@
 AcceptInputDeviceTransferRequestRequestTypeDef = TypedDict(
     "AcceptInputDeviceTransferRequestRequestTypeDef",
     {
         "InputDeviceId": str,
     },
 )
 
+AccountConfigurationTypeDef = TypedDict(
+    "AccountConfigurationTypeDef",
+    {
+        "KmsKeyId": str,
+    },
+    total=False,
+)
+
 AncillarySourceSettingsTypeDef = TypedDict(
     "AncillarySourceSettingsTypeDef",
     {
         "SourceAncillaryChannelNumber": int,
     },
     total=False,
 )
@@ -1616,14 +1597,23 @@
 
 class DescribeScheduleRequestRequestTypeDef(
     _RequiredDescribeScheduleRequestRequestTypeDef, _OptionalDescribeScheduleRequestRequestTypeDef
 ):
     pass
 
 
+DescribeThumbnailsRequestRequestTypeDef = TypedDict(
+    "DescribeThumbnailsRequestRequestTypeDef",
+    {
+        "ChannelId": str,
+        "PipelineId": str,
+        "ThumbnailType": str,
+    },
+)
+
 _RequiredDvbNitSettingsTypeDef = TypedDict(
     "_RequiredDvbNitSettingsTypeDef",
     {
         "NetworkId": int,
         "NetworkName": str,
     },
 )
@@ -1672,14 +1662,21 @@
     {
         "DistributorId": str,
         "NielsenPcmToId3Tagging": NielsenPcmToId3TaggingStateType,
     },
     total=False,
 )
 
+ThumbnailConfigurationTypeDef = TypedDict(
+    "ThumbnailConfigurationTypeDef",
+    {
+        "State": ThumbnailStateType,
+    },
+)
+
 _RequiredTimecodeConfigTypeDef = TypedDict(
     "_RequiredTimecodeConfigTypeDef",
     {
         "Source": TimecodeConfigSourceType,
     },
 )
 _OptionalTimecodeConfigTypeDef = TypedDict(
@@ -1781,24 +1778,14 @@
 
 class TimecodeBurninSettingsTypeDef(
     _RequiredTimecodeBurninSettingsTypeDef, _OptionalTimecodeBurninSettingsTypeDef
 ):
     pass
 
 
-H264ColorSpaceSettingsOutputTypeDef = TypedDict(
-    "H264ColorSpaceSettingsOutputTypeDef",
-    {
-        "ColorSpacePassthroughSettings": Dict[str, Any],
-        "Rec601Settings": Dict[str, Any],
-        "Rec709Settings": Dict[str, Any],
-    },
-    total=False,
-)
-
 H264ColorSpaceSettingsTypeDef = TypedDict(
     "H264ColorSpaceSettingsTypeDef",
     {
         "ColorSpacePassthroughSettings": Mapping[str, Any],
         "Rec601Settings": Mapping[str, Any],
         "Rec709Settings": Mapping[str, Any],
     },
@@ -2155,22 +2142,14 @@
         "PasswordParam": str,
         "Url": str,
         "Username": str,
     },
     total=False,
 )
 
-MotionGraphicsSettingsOutputTypeDef = TypedDict(
-    "MotionGraphicsSettingsOutputTypeDef",
-    {
-        "HtmlMotionGraphicsSettings": Dict[str, Any],
-    },
-    total=False,
-)
-
 MotionGraphicsSettingsTypeDef = TypedDict(
     "MotionGraphicsSettingsTypeDef",
     {
         "HtmlMotionGraphicsSettings": Mapping[str, Any],
     },
     total=False,
 )
@@ -2263,18 +2242,18 @@
         "StreamName": str,
         "Url": str,
         "Username": str,
     },
     total=False,
 )
 
-RtmpGroupSettingsOutputTypeDef = TypedDict(
-    "RtmpGroupSettingsOutputTypeDef",
+RtmpGroupSettingsTypeDef = TypedDict(
+    "RtmpGroupSettingsTypeDef",
     {
-        "AdMarkers": List[Literal["ON_CUE_POINT_SCTE35"]],
+        "AdMarkers": Sequence[Literal["ON_CUE_POINT_SCTE35"]],
         "AuthenticationScheme": AuthenticationSchemeType,
         "CacheFullBehavior": RtmpCacheFullBehaviorType,
         "CacheLength": int,
         "CaptionData": RtmpCaptionDataType,
         "InputLossAction": InputLossActionForRtmpOutType,
         "RestartDelay": int,
     },
@@ -2287,28 +2266,14 @@
         "InputLossAction": InputLossActionForUdpOutType,
         "TimedMetadataId3Frame": UdpTimedMetadataId3FrameType,
         "TimedMetadataId3Period": int,
     },
     total=False,
 )
 
-RtmpGroupSettingsTypeDef = TypedDict(
-    "RtmpGroupSettingsTypeDef",
-    {
-        "AdMarkers": Sequence[Literal["ON_CUE_POINT_SCTE35"]],
-        "AuthenticationScheme": AuthenticationSchemeType,
-        "CacheFullBehavior": RtmpCacheFullBehaviorType,
-        "CacheLength": int,
-        "CaptionData": RtmpCaptionDataType,
-        "InputLossAction": InputLossActionForRtmpOutType,
-        "RestartDelay": int,
-    },
-    total=False,
-)
-
 PipelinePauseStateSettingsTypeDef = TypedDict(
     "PipelinePauseStateSettingsTypeDef",
     {
         "PipelineId": PipelineIdType,
     },
 )
 
@@ -2441,14 +2406,25 @@
 StopMultiplexRequestRequestTypeDef = TypedDict(
     "StopMultiplexRequestRequestTypeDef",
     {
         "MultiplexId": str,
     },
 )
 
+ThumbnailTypeDef = TypedDict(
+    "ThumbnailTypeDef",
+    {
+        "Body": str,
+        "ContentType": str,
+        "ThumbnailType": ThumbnailTypeType,
+        "TimeStamp": datetime,
+    },
+    total=False,
+)
+
 _RequiredTransferInputDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredTransferInputDeviceRequestRequestTypeDef",
     {
         "InputDeviceId": str,
     },
 )
 _OptionalTransferInputDeviceRequestRequestTypeDef = TypedDict(
@@ -2481,14 +2457,22 @@
     "VideoSelectorProgramIdTypeDef",
     {
         "ProgramId": int,
     },
     total=False,
 )
 
+UpdateAccountConfigurationRequestRequestTypeDef = TypedDict(
+    "UpdateAccountConfigurationRequestRequestTypeDef",
+    {
+        "AccountConfiguration": AccountConfigurationTypeDef,
+    },
+    total=False,
+)
+
 ArchiveCdnSettingsTypeDef = TypedDict(
     "ArchiveCdnSettingsTypeDef",
     {
         "ArchiveS3Settings": ArchiveS3SettingsTypeDef,
     },
     total=False,
 )
@@ -2564,44 +2548,22 @@
 
 class RtmpOutputSettingsTypeDef(
     _RequiredRtmpOutputSettingsTypeDef, _OptionalRtmpOutputSettingsTypeDef
 ):
     pass
 
 
-AudioChannelMappingOutputTypeDef = TypedDict(
-    "AudioChannelMappingOutputTypeDef",
-    {
-        "InputChannelLevels": List[InputChannelLevelTypeDef],
-        "OutputChannel": int,
-    },
-)
-
 AudioChannelMappingTypeDef = TypedDict(
     "AudioChannelMappingTypeDef",
     {
         "InputChannelLevels": Sequence[InputChannelLevelTypeDef],
         "OutputChannel": int,
     },
 )
 
-AudioCodecSettingsOutputTypeDef = TypedDict(
-    "AudioCodecSettingsOutputTypeDef",
-    {
-        "AacSettings": AacSettingsTypeDef,
-        "Ac3Settings": Ac3SettingsTypeDef,
-        "Eac3AtmosSettings": Eac3AtmosSettingsTypeDef,
-        "Eac3Settings": Eac3SettingsTypeDef,
-        "Mp2Settings": Mp2SettingsTypeDef,
-        "PassThroughSettings": Dict[str, Any],
-        "WavSettings": WavSettingsTypeDef,
-    },
-    total=False,
-)
-
 AudioCodecSettingsTypeDef = TypedDict(
     "AudioCodecSettingsTypeDef",
     {
         "AacSettings": AacSettingsTypeDef,
         "Ac3Settings": Ac3SettingsTypeDef,
         "Eac3AtmosSettings": Eac3AtmosSettingsTypeDef,
         "Eac3Settings": Eac3SettingsTypeDef,
@@ -2751,35 +2713,14 @@
 
 class StaticKeySettingsTypeDef(
     _RequiredStaticKeySettingsTypeDef, _OptionalStaticKeySettingsTypeDef
 ):
     pass
 
 
-_RequiredAudioTrackSelectionOutputTypeDef = TypedDict(
-    "_RequiredAudioTrackSelectionOutputTypeDef",
-    {
-        "Tracks": List[AudioTrackTypeDef],
-    },
-)
-_OptionalAudioTrackSelectionOutputTypeDef = TypedDict(
-    "_OptionalAudioTrackSelectionOutputTypeDef",
-    {
-        "DolbyEDecode": AudioDolbyEDecodeTypeDef,
-    },
-    total=False,
-)
-
-
-class AudioTrackSelectionOutputTypeDef(
-    _RequiredAudioTrackSelectionOutputTypeDef, _OptionalAudioTrackSelectionOutputTypeDef
-):
-    pass
-
-
 _RequiredAudioTrackSelectionTypeDef = TypedDict(
     "_RequiredAudioTrackSelectionTypeDef",
     {
         "Tracks": Sequence[AudioTrackTypeDef],
     },
 )
 _OptionalAudioTrackSelectionTypeDef = TypedDict(
@@ -2830,14 +2771,22 @@
     {
         "Failed": List[BatchFailedResultModelTypeDef],
         "Successful": List[BatchSuccessfulResultModelTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeAccountConfigurationResponseTypeDef = TypedDict(
+    "DescribeAccountConfigurationResponseTypeDef",
+    {
+        "AccountConfiguration": AccountConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeInputDeviceThumbnailResponseTypeDef = TypedDict(
     "DescribeInputDeviceThumbnailResponseTypeDef",
     {
         "Body": StreamingBody,
         "ContentType": Literal["image/jpeg"],
         "ContentLength": int,
         "ETag": str,
@@ -2857,14 +2806,22 @@
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+UpdateAccountConfigurationResponseTypeDef = TypedDict(
+    "UpdateAccountConfigurationResponseTypeDef",
+    {
+        "AccountConfiguration": AccountConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 TeletextSourceSettingsTypeDef = TypedDict(
     "TeletextSourceSettingsTypeDef",
     {
         "OutputRectangle": CaptionRectangleTypeDef,
         "PageNumber": str,
     },
     total=False,
@@ -3382,14 +3339,15 @@
         "MacAddress": str,
         "Name": str,
         "NetworkSettings": InputDeviceNetworkSettingsTypeDef,
         "SerialNumber": str,
         "Type": InputDeviceTypeType,
         "UhdDeviceSettings": InputDeviceUhdSettingsTypeDef,
         "Tags": Dict[str, str],
+        "AvailabilityZone": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InputDeviceSummaryTypeDef = TypedDict(
     "InputDeviceSummaryTypeDef",
     {
@@ -3402,14 +3360,15 @@
         "MacAddress": str,
         "Name": str,
         "NetworkSettings": InputDeviceNetworkSettingsTypeDef,
         "SerialNumber": str,
         "Type": InputDeviceTypeType,
         "UhdDeviceSettings": InputDeviceUhdSettingsTypeDef,
         "Tags": Dict[str, str],
+        "AvailabilityZone": str,
     },
     total=False,
 )
 
 UpdateInputDeviceResponseTypeDef = TypedDict(
     "UpdateInputDeviceResponseTypeDef",
     {
@@ -3422,14 +3381,15 @@
         "MacAddress": str,
         "Name": str,
         "NetworkSettings": InputDeviceNetworkSettingsTypeDef,
         "SerialNumber": str,
         "Type": InputDeviceTypeType,
         "UhdDeviceSettings": InputDeviceUhdSettingsTypeDef,
         "Tags": Dict[str, str],
+        "AvailabilityZone": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeInputSecurityGroupResponseTypeDef = TypedDict(
     "DescribeInputSecurityGroupResponseTypeDef",
     {
@@ -3657,24 +3617,14 @@
         "AudioSilenceSettings": AudioSilenceFailoverSettingsTypeDef,
         "InputLossSettings": InputLossFailoverSettingsTypeDef,
         "VideoBlackSettings": VideoBlackFailoverSettingsTypeDef,
     },
     total=False,
 )
 
-ScheduleActionStartSettingsOutputTypeDef = TypedDict(
-    "ScheduleActionStartSettingsOutputTypeDef",
-    {
-        "FixedModeScheduleActionStartSettings": FixedModeScheduleActionStartSettingsTypeDef,
-        "FollowModeScheduleActionStartSettings": FollowModeScheduleActionStartSettingsTypeDef,
-        "ImmediateModeScheduleActionStartSettings": Dict[str, Any],
-    },
-    total=False,
-)
-
 ScheduleActionStartSettingsTypeDef = TypedDict(
     "ScheduleActionStartSettingsTypeDef",
     {
         "FixedModeScheduleActionStartSettings": FixedModeScheduleActionStartSettingsTypeDef,
         "FollowModeScheduleActionStartSettings": FollowModeScheduleActionStartSettingsTypeDef,
         "ImmediateModeScheduleActionStartSettings": Mapping[str, Any],
     },
@@ -3719,26 +3669,14 @@
     "Mpeg2FilterSettingsTypeDef",
     {
         "TemporalFilterSettings": TemporalFilterSettingsTypeDef,
     },
     total=False,
 )
 
-H265ColorSpaceSettingsOutputTypeDef = TypedDict(
-    "H265ColorSpaceSettingsOutputTypeDef",
-    {
-        "ColorSpacePassthroughSettings": Dict[str, Any],
-        "DolbyVision81Settings": Dict[str, Any],
-        "Hdr10Settings": Hdr10SettingsTypeDef,
-        "Rec601Settings": Dict[str, Any],
-        "Rec709Settings": Dict[str, Any],
-    },
-    total=False,
-)
-
 H265ColorSpaceSettingsTypeDef = TypedDict(
     "H265ColorSpaceSettingsTypeDef",
     {
         "ColorSpacePassthroughSettings": Mapping[str, Any],
         "DolbyVision81Settings": Mapping[str, Any],
         "Hdr10Settings": Hdr10SettingsTypeDef,
         "Rec601Settings": Mapping[str, Any],
@@ -3817,14 +3755,15 @@
 )
 _OptionalUpdateInputDeviceRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateInputDeviceRequestRequestTypeDef",
     {
         "HdDeviceSettings": InputDeviceConfigurableSettingsTypeDef,
         "Name": str,
         "UhdDeviceSettings": InputDeviceConfigurableSettingsTypeDef,
+        "AvailabilityZone": str,
     },
     total=False,
 )
 
 
 class UpdateInputDeviceRequestRequestTypeDef(
     _RequiredUpdateInputDeviceRequestRequestTypeDef, _OptionalUpdateInputDeviceRequestRequestTypeDef
@@ -3894,36 +3833,14 @@
 
 class StandardHlsSettingsTypeDef(
     _RequiredStandardHlsSettingsTypeDef, _OptionalStandardHlsSettingsTypeDef
 ):
     pass
 
 
-_RequiredMotionGraphicsConfigurationOutputTypeDef = TypedDict(
-    "_RequiredMotionGraphicsConfigurationOutputTypeDef",
-    {
-        "MotionGraphicsSettings": MotionGraphicsSettingsOutputTypeDef,
-    },
-)
-_OptionalMotionGraphicsConfigurationOutputTypeDef = TypedDict(
-    "_OptionalMotionGraphicsConfigurationOutputTypeDef",
-    {
-        "MotionGraphicsInsertion": MotionGraphicsInsertionType,
-    },
-    total=False,
-)
-
-
-class MotionGraphicsConfigurationOutputTypeDef(
-    _RequiredMotionGraphicsConfigurationOutputTypeDef,
-    _OptionalMotionGraphicsConfigurationOutputTypeDef,
-):
-    pass
-
-
 _RequiredMotionGraphicsConfigurationTypeDef = TypedDict(
     "_RequiredMotionGraphicsConfigurationTypeDef",
     {
         "MotionGraphicsSettings": MotionGraphicsSettingsTypeDef,
     },
 )
 _OptionalMotionGraphicsConfigurationTypeDef = TypedDict(
@@ -3980,44 +3897,25 @@
         "NielsenCbetSettings": NielsenCBETTypeDef,
         "NielsenDistributionType": NielsenWatermarksDistributionTypesType,
         "NielsenNaesIiNwSettings": NielsenNaesIiNwTypeDef,
     },
     total=False,
 )
 
-OutputDestinationOutputTypeDef = TypedDict(
-    "OutputDestinationOutputTypeDef",
-    {
-        "Id": str,
-        "MediaPackageSettings": List[MediaPackageOutputDestinationSettingsTypeDef],
-        "MultiplexSettings": MultiplexProgramChannelDestinationSettingsTypeDef,
-        "Settings": List[OutputDestinationSettingsTypeDef],
-    },
-    total=False,
-)
-
 OutputDestinationTypeDef = TypedDict(
     "OutputDestinationTypeDef",
     {
         "Id": str,
         "MediaPackageSettings": Sequence[MediaPackageOutputDestinationSettingsTypeDef],
         "MultiplexSettings": MultiplexProgramChannelDestinationSettingsTypeDef,
         "Settings": Sequence[OutputDestinationSettingsTypeDef],
     },
     total=False,
 )
 
-PauseStateScheduleActionSettingsOutputTypeDef = TypedDict(
-    "PauseStateScheduleActionSettingsOutputTypeDef",
-    {
-        "Pipelines": List[PipelinePauseStateSettingsTypeDef],
-    },
-    total=False,
-)
-
 PauseStateScheduleActionSettingsTypeDef = TypedDict(
     "PauseStateScheduleActionSettingsTypeDef",
     {
         "Pipelines": Sequence[PipelinePauseStateSettingsTypeDef],
     },
     total=False,
 )
@@ -4048,14 +3946,23 @@
 
 class Scte35SegmentationDescriptorTypeDef(
     _RequiredScte35SegmentationDescriptorTypeDef, _OptionalScte35SegmentationDescriptorTypeDef
 ):
     pass
 
 
+ThumbnailDetailTypeDef = TypedDict(
+    "ThumbnailDetailTypeDef",
+    {
+        "PipelineId": str,
+        "Thumbnails": List[ThumbnailTypeDef],
+    },
+    total=False,
+)
+
 VideoSelectorSettingsTypeDef = TypedDict(
     "VideoSelectorSettingsTypeDef",
     {
         "VideoSelectorPid": VideoSelectorPidTypeDef,
         "VideoSelectorProgramId": VideoSelectorProgramIdTypeDef,
     },
     total=False,
@@ -4079,36 +3986,14 @@
 
 class ArchiveGroupSettingsTypeDef(
     _RequiredArchiveGroupSettingsTypeDef, _OptionalArchiveGroupSettingsTypeDef
 ):
     pass
 
 
-_RequiredRemixSettingsOutputTypeDef = TypedDict(
-    "_RequiredRemixSettingsOutputTypeDef",
-    {
-        "ChannelMappings": List[AudioChannelMappingOutputTypeDef],
-    },
-)
-_OptionalRemixSettingsOutputTypeDef = TypedDict(
-    "_OptionalRemixSettingsOutputTypeDef",
-    {
-        "ChannelsIn": int,
-        "ChannelsOut": int,
-    },
-    total=False,
-)
-
-
-class RemixSettingsOutputTypeDef(
-    _RequiredRemixSettingsOutputTypeDef, _OptionalRemixSettingsOutputTypeDef
-):
-    pass
-
-
 _RequiredRemixSettingsTypeDef = TypedDict(
     "_RequiredRemixSettingsTypeDef",
     {
         "ChannelMappings": Sequence[AudioChannelMappingTypeDef],
     },
 )
 _OptionalRemixSettingsTypeDef = TypedDict(
@@ -4121,34 +4006,14 @@
 )
 
 
 class RemixSettingsTypeDef(_RequiredRemixSettingsTypeDef, _OptionalRemixSettingsTypeDef):
     pass
 
 
-CaptionDestinationSettingsOutputTypeDef = TypedDict(
-    "CaptionDestinationSettingsOutputTypeDef",
-    {
-        "AribDestinationSettings": Dict[str, Any],
-        "BurnInDestinationSettings": BurnInDestinationSettingsTypeDef,
-        "DvbSubDestinationSettings": DvbSubDestinationSettingsTypeDef,
-        "EbuTtDDestinationSettings": EbuTtDDestinationSettingsTypeDef,
-        "EmbeddedDestinationSettings": Dict[str, Any],
-        "EmbeddedPlusScte20DestinationSettings": Dict[str, Any],
-        "RtmpCaptionInfoDestinationSettings": Dict[str, Any],
-        "Scte20PlusEmbeddedDestinationSettings": Dict[str, Any],
-        "Scte27DestinationSettings": Dict[str, Any],
-        "SmpteTtDestinationSettings": Dict[str, Any],
-        "TeletextDestinationSettings": Dict[str, Any],
-        "TtmlDestinationSettings": TtmlDestinationSettingsTypeDef,
-        "WebvttDestinationSettings": WebvttDestinationSettingsTypeDef,
-    },
-    total=False,
-)
-
 CaptionDestinationSettingsTypeDef = TypedDict(
     "CaptionDestinationSettingsTypeDef",
     {
         "AribDestinationSettings": Mapping[str, Any],
         "BurnInDestinationSettings": BurnInDestinationSettingsTypeDef,
         "DvbSubDestinationSettings": DvbSubDestinationSettingsTypeDef,
         "EbuTtDDestinationSettings": EbuTtDDestinationSettingsTypeDef,
@@ -4182,25 +4047,14 @@
     "KeyProviderSettingsTypeDef",
     {
         "StaticKeySettings": StaticKeySettingsTypeDef,
     },
     total=False,
 )
 
-AudioSelectorSettingsOutputTypeDef = TypedDict(
-    "AudioSelectorSettingsOutputTypeDef",
-    {
-        "AudioHlsRenditionSelection": AudioHlsRenditionSelectionTypeDef,
-        "AudioLanguageSelection": AudioLanguageSelectionTypeDef,
-        "AudioPidSelection": AudioPidSelectionTypeDef,
-        "AudioTrackSelection": AudioTrackSelectionOutputTypeDef,
-    },
-    total=False,
-)
-
 AudioSelectorSettingsTypeDef = TypedDict(
     "AudioSelectorSettingsTypeDef",
     {
         "AudioHlsRenditionSelection": AudioHlsRenditionSelectionTypeDef,
         "AudioLanguageSelection": AudioLanguageSelectionTypeDef,
         "AudioPidSelection": AudioPidSelectionTypeDef,
         "AudioTrackSelection": AudioTrackSelectionTypeDef,
@@ -4212,28 +4066,14 @@
     "AvailConfigurationTypeDef",
     {
         "AvailSettings": AvailSettingsTypeDef,
     },
     total=False,
 )
 
-CaptionSelectorSettingsOutputTypeDef = TypedDict(
-    "CaptionSelectorSettingsOutputTypeDef",
-    {
-        "AncillarySourceSettings": AncillarySourceSettingsTypeDef,
-        "AribSourceSettings": Dict[str, Any],
-        "DvbSubSourceSettings": DvbSubSourceSettingsTypeDef,
-        "EmbeddedSourceSettings": EmbeddedSourceSettingsTypeDef,
-        "Scte20SourceSettings": Scte20SourceSettingsTypeDef,
-        "Scte27SourceSettings": Scte27SourceSettingsTypeDef,
-        "TeletextSourceSettings": TeletextSourceSettingsTypeDef,
-    },
-    total=False,
-)
-
 CaptionSelectorSettingsTypeDef = TypedDict(
     "CaptionSelectorSettingsTypeDef",
     {
         "AncillarySourceSettings": AncillarySourceSettingsTypeDef,
         "AribSourceSettings": Mapping[str, Any],
         "DvbSubSourceSettings": DvbSubSourceSettingsTypeDef,
         "EmbeddedSourceSettings": EmbeddedSourceSettingsTypeDef,
@@ -4354,63 +4194,14 @@
 
 class FrameCaptureGroupSettingsTypeDef(
     _RequiredFrameCaptureGroupSettingsTypeDef, _OptionalFrameCaptureGroupSettingsTypeDef
 ):
     pass
 
 
-H264SettingsOutputTypeDef = TypedDict(
-    "H264SettingsOutputTypeDef",
-    {
-        "AdaptiveQuantization": H264AdaptiveQuantizationType,
-        "AfdSignaling": AfdSignalingType,
-        "Bitrate": int,
-        "BufFillPct": int,
-        "BufSize": int,
-        "ColorMetadata": H264ColorMetadataType,
-        "ColorSpaceSettings": H264ColorSpaceSettingsOutputTypeDef,
-        "EntropyEncoding": H264EntropyEncodingType,
-        "FilterSettings": H264FilterSettingsTypeDef,
-        "FixedAfd": FixedAfdType,
-        "FlickerAq": H264FlickerAqType,
-        "ForceFieldPictures": H264ForceFieldPicturesType,
-        "FramerateControl": H264FramerateControlType,
-        "FramerateDenominator": int,
-        "FramerateNumerator": int,
-        "GopBReference": H264GopBReferenceType,
-        "GopClosedCadence": int,
-        "GopNumBFrames": int,
-        "GopSize": float,
-        "GopSizeUnits": H264GopSizeUnitsType,
-        "Level": H264LevelType,
-        "LookAheadRateControl": H264LookAheadRateControlType,
-        "MaxBitrate": int,
-        "MinIInterval": int,
-        "NumRefFrames": int,
-        "ParControl": H264ParControlType,
-        "ParDenominator": int,
-        "ParNumerator": int,
-        "Profile": H264ProfileType,
-        "QualityLevel": H264QualityLevelType,
-        "QvbrQualityLevel": int,
-        "RateControlMode": H264RateControlModeType,
-        "ScanType": H264ScanTypeType,
-        "SceneChangeDetect": H264SceneChangeDetectType,
-        "Slices": int,
-        "Softness": int,
-        "SpatialAq": H264SpatialAqType,
-        "SubgopLength": H264SubGopLengthType,
-        "Syntax": H264SyntaxType,
-        "TemporalAq": H264TemporalAqType,
-        "TimecodeInsertion": H264TimecodeInsertionBehaviorType,
-        "TimecodeBurninSettings": TimecodeBurninSettingsTypeDef,
-    },
-    total=False,
-)
-
 H264SettingsTypeDef = TypedDict(
     "H264SettingsTypeDef",
     {
         "AdaptiveQuantization": H264AdaptiveQuantizationType,
         "AfdSignaling": AfdSignalingType,
         "Bitrate": int,
         "BufFillPct": int,
@@ -4486,63 +4277,14 @@
 )
 
 
 class Mpeg2SettingsTypeDef(_RequiredMpeg2SettingsTypeDef, _OptionalMpeg2SettingsTypeDef):
     pass
 
 
-_RequiredH265SettingsOutputTypeDef = TypedDict(
-    "_RequiredH265SettingsOutputTypeDef",
-    {
-        "FramerateDenominator": int,
-        "FramerateNumerator": int,
-    },
-)
-_OptionalH265SettingsOutputTypeDef = TypedDict(
-    "_OptionalH265SettingsOutputTypeDef",
-    {
-        "AdaptiveQuantization": H265AdaptiveQuantizationType,
-        "AfdSignaling": AfdSignalingType,
-        "AlternativeTransferFunction": H265AlternativeTransferFunctionType,
-        "Bitrate": int,
-        "BufSize": int,
-        "ColorMetadata": H265ColorMetadataType,
-        "ColorSpaceSettings": H265ColorSpaceSettingsOutputTypeDef,
-        "FilterSettings": H265FilterSettingsTypeDef,
-        "FixedAfd": FixedAfdType,
-        "FlickerAq": H265FlickerAqType,
-        "GopClosedCadence": int,
-        "GopSize": float,
-        "GopSizeUnits": H265GopSizeUnitsType,
-        "Level": H265LevelType,
-        "LookAheadRateControl": H265LookAheadRateControlType,
-        "MaxBitrate": int,
-        "MinIInterval": int,
-        "ParDenominator": int,
-        "ParNumerator": int,
-        "Profile": H265ProfileType,
-        "QvbrQualityLevel": int,
-        "RateControlMode": H265RateControlModeType,
-        "ScanType": H265ScanTypeType,
-        "SceneChangeDetect": H265SceneChangeDetectType,
-        "Slices": int,
-        "Tier": H265TierType,
-        "TimecodeInsertion": H265TimecodeInsertionBehaviorType,
-        "TimecodeBurninSettings": TimecodeBurninSettingsTypeDef,
-    },
-    total=False,
-)
-
-
-class H265SettingsOutputTypeDef(
-    _RequiredH265SettingsOutputTypeDef, _OptionalH265SettingsOutputTypeDef
-):
-    pass
-
-
 _RequiredH265SettingsTypeDef = TypedDict(
     "_RequiredH265SettingsTypeDef",
     {
         "FramerateDenominator": int,
         "FramerateNumerator": int,
     },
 )
@@ -4582,57 +4324,24 @@
 )
 
 
 class H265SettingsTypeDef(_RequiredH265SettingsTypeDef, _OptionalH265SettingsTypeDef):
     pass
 
 
-InputPrepareScheduleActionSettingsOutputTypeDef = TypedDict(
-    "InputPrepareScheduleActionSettingsOutputTypeDef",
-    {
-        "InputAttachmentNameReference": str,
-        "InputClippingSettings": InputClippingSettingsTypeDef,
-        "UrlPath": List[str],
-    },
-    total=False,
-)
-
 InputPrepareScheduleActionSettingsTypeDef = TypedDict(
     "InputPrepareScheduleActionSettingsTypeDef",
     {
         "InputAttachmentNameReference": str,
         "InputClippingSettings": InputClippingSettingsTypeDef,
         "UrlPath": Sequence[str],
     },
     total=False,
 )
 
-_RequiredInputSwitchScheduleActionSettingsOutputTypeDef = TypedDict(
-    "_RequiredInputSwitchScheduleActionSettingsOutputTypeDef",
-    {
-        "InputAttachmentNameReference": str,
-    },
-)
-_OptionalInputSwitchScheduleActionSettingsOutputTypeDef = TypedDict(
-    "_OptionalInputSwitchScheduleActionSettingsOutputTypeDef",
-    {
-        "InputClippingSettings": InputClippingSettingsTypeDef,
-        "UrlPath": List[str],
-    },
-    total=False,
-)
-
-
-class InputSwitchScheduleActionSettingsOutputTypeDef(
-    _RequiredInputSwitchScheduleActionSettingsOutputTypeDef,
-    _OptionalInputSwitchScheduleActionSettingsOutputTypeDef,
-):
-    pass
-
-
 _RequiredInputSwitchScheduleActionSettingsTypeDef = TypedDict(
     "_RequiredInputSwitchScheduleActionSettingsTypeDef",
     {
         "InputAttachmentNameReference": str,
     },
 )
 _OptionalInputSwitchScheduleActionSettingsTypeDef = TypedDict(
@@ -4830,58 +4539,63 @@
     "AudioWatermarkSettingsTypeDef",
     {
         "NielsenWatermarksSettings": NielsenWatermarksSettingsTypeDef,
     },
     total=False,
 )
 
-OutputDestinationUnionTypeDef = Union[OutputDestinationTypeDef, OutputDestinationOutputTypeDef]
+_RequiredUpdateChannelClassRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateChannelClassRequestRequestTypeDef",
+    {
+        "ChannelClass": ChannelClassType,
+        "ChannelId": str,
+    },
+)
+_OptionalUpdateChannelClassRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateChannelClassRequestRequestTypeDef",
+    {
+        "Destinations": Sequence[OutputDestinationTypeDef],
+    },
+    total=False,
+)
+
+
+class UpdateChannelClassRequestRequestTypeDef(
+    _RequiredUpdateChannelClassRequestRequestTypeDef,
+    _OptionalUpdateChannelClassRequestRequestTypeDef,
+):
+    pass
+
+
 Scte35DescriptorSettingsTypeDef = TypedDict(
     "Scte35DescriptorSettingsTypeDef",
     {
         "SegmentationDescriptorScte35DescriptorSettings": Scte35SegmentationDescriptorTypeDef,
     },
 )
 
+DescribeThumbnailsResponseTypeDef = TypedDict(
+    "DescribeThumbnailsResponseTypeDef",
+    {
+        "ThumbnailDetails": List[ThumbnailDetailTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 VideoSelectorTypeDef = TypedDict(
     "VideoSelectorTypeDef",
     {
         "ColorSpace": VideoSelectorColorSpaceType,
         "ColorSpaceSettings": VideoSelectorColorSpaceSettingsTypeDef,
         "ColorSpaceUsage": VideoSelectorColorSpaceUsageType,
         "SelectorSettings": VideoSelectorSettingsTypeDef,
     },
     total=False,
 )
 
-_RequiredCaptionDescriptionOutputTypeDef = TypedDict(
-    "_RequiredCaptionDescriptionOutputTypeDef",
-    {
-        "CaptionSelectorName": str,
-        "Name": str,
-    },
-)
-_OptionalCaptionDescriptionOutputTypeDef = TypedDict(
-    "_OptionalCaptionDescriptionOutputTypeDef",
-    {
-        "Accessibility": AccessibilityTypeType,
-        "DestinationSettings": CaptionDestinationSettingsOutputTypeDef,
-        "LanguageCode": str,
-        "LanguageDescription": str,
-    },
-    total=False,
-)
-
-
-class CaptionDescriptionOutputTypeDef(
-    _RequiredCaptionDescriptionOutputTypeDef, _OptionalCaptionDescriptionOutputTypeDef
-):
-    pass
-
-
 _RequiredCaptionDescriptionTypeDef = TypedDict(
     "_RequiredCaptionDescriptionTypeDef",
     {
         "CaptionSelectorName": str,
         "Name": str,
     },
 )
@@ -4899,76 +4613,14 @@
 
 class CaptionDescriptionTypeDef(
     _RequiredCaptionDescriptionTypeDef, _OptionalCaptionDescriptionTypeDef
 ):
     pass
 
 
-_RequiredHlsGroupSettingsOutputTypeDef = TypedDict(
-    "_RequiredHlsGroupSettingsOutputTypeDef",
-    {
-        "Destination": OutputLocationRefTypeDef,
-    },
-)
-_OptionalHlsGroupSettingsOutputTypeDef = TypedDict(
-    "_OptionalHlsGroupSettingsOutputTypeDef",
-    {
-        "AdMarkers": List[HlsAdMarkersType],
-        "BaseUrlContent": str,
-        "BaseUrlContent1": str,
-        "BaseUrlManifest": str,
-        "BaseUrlManifest1": str,
-        "CaptionLanguageMappings": List[CaptionLanguageMappingTypeDef],
-        "CaptionLanguageSetting": HlsCaptionLanguageSettingType,
-        "ClientCache": HlsClientCacheType,
-        "CodecSpecification": HlsCodecSpecificationType,
-        "ConstantIv": str,
-        "DirectoryStructure": HlsDirectoryStructureType,
-        "DiscontinuityTags": HlsDiscontinuityTagsType,
-        "EncryptionType": HlsEncryptionTypeType,
-        "HlsCdnSettings": HlsCdnSettingsTypeDef,
-        "HlsId3SegmentTagging": HlsId3SegmentTaggingStateType,
-        "IFrameOnlyPlaylists": IFrameOnlyPlaylistTypeType,
-        "IncompleteSegmentBehavior": HlsIncompleteSegmentBehaviorType,
-        "IndexNSegments": int,
-        "InputLossAction": InputLossActionForHlsOutType,
-        "IvInManifest": HlsIvInManifestType,
-        "IvSource": HlsIvSourceType,
-        "KeepSegments": int,
-        "KeyFormat": str,
-        "KeyFormatVersions": str,
-        "KeyProviderSettings": KeyProviderSettingsTypeDef,
-        "ManifestCompression": HlsManifestCompressionType,
-        "ManifestDurationFormat": HlsManifestDurationFormatType,
-        "MinSegmentLength": int,
-        "Mode": HlsModeType,
-        "OutputSelection": HlsOutputSelectionType,
-        "ProgramDateTime": HlsProgramDateTimeType,
-        "ProgramDateTimeClock": HlsProgramDateTimeClockType,
-        "ProgramDateTimePeriod": int,
-        "RedundantManifest": HlsRedundantManifestType,
-        "SegmentLength": int,
-        "SegmentationMode": HlsSegmentationModeType,
-        "SegmentsPerSubdirectory": int,
-        "StreamInfResolution": HlsStreamInfResolutionType,
-        "TimedMetadataId3Frame": HlsTimedMetadataId3FrameType,
-        "TimedMetadataId3Period": int,
-        "TimestampDeltaMilliseconds": int,
-        "TsFileMode": HlsTsFileModeType,
-    },
-    total=False,
-)
-
-
-class HlsGroupSettingsOutputTypeDef(
-    _RequiredHlsGroupSettingsOutputTypeDef, _OptionalHlsGroupSettingsOutputTypeDef
-):
-    pass
-
-
 _RequiredHlsGroupSettingsTypeDef = TypedDict(
     "_RequiredHlsGroupSettingsTypeDef",
     {
         "Destination": OutputLocationRefTypeDef,
     },
 )
 _OptionalHlsGroupSettingsTypeDef = TypedDict(
@@ -5021,35 +4673,14 @@
 )
 
 
 class HlsGroupSettingsTypeDef(_RequiredHlsGroupSettingsTypeDef, _OptionalHlsGroupSettingsTypeDef):
     pass
 
 
-_RequiredAudioSelectorOutputTypeDef = TypedDict(
-    "_RequiredAudioSelectorOutputTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalAudioSelectorOutputTypeDef = TypedDict(
-    "_OptionalAudioSelectorOutputTypeDef",
-    {
-        "SelectorSettings": AudioSelectorSettingsOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class AudioSelectorOutputTypeDef(
-    _RequiredAudioSelectorOutputTypeDef, _OptionalAudioSelectorOutputTypeDef
-):
-    pass
-
-
 _RequiredAudioSelectorTypeDef = TypedDict(
     "_RequiredAudioSelectorTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalAudioSelectorTypeDef = TypedDict(
@@ -5061,36 +4692,14 @@
 )
 
 
 class AudioSelectorTypeDef(_RequiredAudioSelectorTypeDef, _OptionalAudioSelectorTypeDef):
     pass
 
 
-_RequiredCaptionSelectorOutputTypeDef = TypedDict(
-    "_RequiredCaptionSelectorOutputTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalCaptionSelectorOutputTypeDef = TypedDict(
-    "_OptionalCaptionSelectorOutputTypeDef",
-    {
-        "LanguageCode": str,
-        "SelectorSettings": CaptionSelectorSettingsOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class CaptionSelectorOutputTypeDef(
-    _RequiredCaptionSelectorOutputTypeDef, _OptionalCaptionSelectorOutputTypeDef
-):
-    pass
-
-
 _RequiredCaptionSelectorTypeDef = TypedDict(
     "_RequiredCaptionSelectorTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCaptionSelectorTypeDef = TypedDict(
@@ -5148,38 +4757,14 @@
 
 class UdpOutputSettingsTypeDef(
     _RequiredUdpOutputSettingsTypeDef, _OptionalUdpOutputSettingsTypeDef
 ):
     pass
 
 
-_RequiredAutomaticInputFailoverSettingsOutputTypeDef = TypedDict(
-    "_RequiredAutomaticInputFailoverSettingsOutputTypeDef",
-    {
-        "SecondaryInputId": str,
-    },
-)
-_OptionalAutomaticInputFailoverSettingsOutputTypeDef = TypedDict(
-    "_OptionalAutomaticInputFailoverSettingsOutputTypeDef",
-    {
-        "ErrorClearTimeMsec": int,
-        "FailoverConditions": List[FailoverConditionTypeDef],
-        "InputPreference": InputPreferenceType,
-    },
-    total=False,
-)
-
-
-class AutomaticInputFailoverSettingsOutputTypeDef(
-    _RequiredAutomaticInputFailoverSettingsOutputTypeDef,
-    _OptionalAutomaticInputFailoverSettingsOutputTypeDef,
-):
-    pass
-
-
 _RequiredAutomaticInputFailoverSettingsTypeDef = TypedDict(
     "_RequiredAutomaticInputFailoverSettingsTypeDef",
     {
         "SecondaryInputId": str,
     },
 )
 _OptionalAutomaticInputFailoverSettingsTypeDef = TypedDict(
@@ -5195,25 +4780,14 @@
 
 class AutomaticInputFailoverSettingsTypeDef(
     _RequiredAutomaticInputFailoverSettingsTypeDef, _OptionalAutomaticInputFailoverSettingsTypeDef
 ):
     pass
 
 
-VideoCodecSettingsOutputTypeDef = TypedDict(
-    "VideoCodecSettingsOutputTypeDef",
-    {
-        "FrameCaptureSettings": FrameCaptureSettingsTypeDef,
-        "H264Settings": H264SettingsOutputTypeDef,
-        "H265Settings": H265SettingsOutputTypeDef,
-        "Mpeg2Settings": Mpeg2SettingsTypeDef,
-    },
-    total=False,
-)
-
 VideoCodecSettingsTypeDef = TypedDict(
     "VideoCodecSettingsTypeDef",
     {
         "FrameCaptureSettings": FrameCaptureSettingsTypeDef,
         "H264Settings": H264SettingsTypeDef,
         "H265Settings": H265SettingsTypeDef,
         "Mpeg2Settings": Mpeg2SettingsTypeDef,
@@ -5358,44 +4932,14 @@
 class UpdateMultiplexProgramRequestRequestTypeDef(
     _RequiredUpdateMultiplexProgramRequestRequestTypeDef,
     _OptionalUpdateMultiplexProgramRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredAudioDescriptionOutputTypeDef = TypedDict(
-    "_RequiredAudioDescriptionOutputTypeDef",
-    {
-        "AudioSelectorName": str,
-        "Name": str,
-    },
-)
-_OptionalAudioDescriptionOutputTypeDef = TypedDict(
-    "_OptionalAudioDescriptionOutputTypeDef",
-    {
-        "AudioNormalizationSettings": AudioNormalizationSettingsTypeDef,
-        "AudioType": AudioTypeType,
-        "AudioTypeControl": AudioDescriptionAudioTypeControlType,
-        "AudioWatermarkingSettings": AudioWatermarkSettingsTypeDef,
-        "CodecSettings": AudioCodecSettingsOutputTypeDef,
-        "LanguageCode": str,
-        "LanguageCodeControl": AudioDescriptionLanguageCodeControlType,
-        "RemixSettings": RemixSettingsOutputTypeDef,
-        "StreamName": str,
-    },
-    total=False,
-)
-
-
-class AudioDescriptionOutputTypeDef(
-    _RequiredAudioDescriptionOutputTypeDef, _OptionalAudioDescriptionOutputTypeDef
-):
-    pass
-
-
 _RequiredAudioDescriptionTypeDef = TypedDict(
     "_RequiredAudioDescriptionTypeDef",
     {
         "AudioSelectorName": str,
         "Name": str,
     },
 )
@@ -5416,59 +4960,21 @@
 )
 
 
 class AudioDescriptionTypeDef(_RequiredAudioDescriptionTypeDef, _OptionalAudioDescriptionTypeDef):
     pass
 
 
-_RequiredUpdateChannelClassRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateChannelClassRequestRequestTypeDef",
-    {
-        "ChannelClass": ChannelClassType,
-        "ChannelId": str,
-    },
-)
-_OptionalUpdateChannelClassRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateChannelClassRequestRequestTypeDef",
-    {
-        "Destinations": Sequence[OutputDestinationUnionTypeDef],
-    },
-    total=False,
-)
-
-
-class UpdateChannelClassRequestRequestTypeDef(
-    _RequiredUpdateChannelClassRequestRequestTypeDef,
-    _OptionalUpdateChannelClassRequestRequestTypeDef,
-):
-    pass
-
-
 Scte35DescriptorTypeDef = TypedDict(
     "Scte35DescriptorTypeDef",
     {
         "Scte35DescriptorSettings": Scte35DescriptorSettingsTypeDef,
     },
 )
 
-OutputGroupSettingsOutputTypeDef = TypedDict(
-    "OutputGroupSettingsOutputTypeDef",
-    {
-        "ArchiveGroupSettings": ArchiveGroupSettingsTypeDef,
-        "FrameCaptureGroupSettings": FrameCaptureGroupSettingsTypeDef,
-        "HlsGroupSettings": HlsGroupSettingsOutputTypeDef,
-        "MediaPackageGroupSettings": MediaPackageGroupSettingsTypeDef,
-        "MsSmoothGroupSettings": MsSmoothGroupSettingsTypeDef,
-        "MultiplexGroupSettings": Dict[str, Any],
-        "RtmpGroupSettings": RtmpGroupSettingsOutputTypeDef,
-        "UdpGroupSettings": UdpGroupSettingsTypeDef,
-    },
-    total=False,
-)
-
 OutputGroupSettingsTypeDef = TypedDict(
     "OutputGroupSettingsTypeDef",
     {
         "ArchiveGroupSettings": ArchiveGroupSettingsTypeDef,
         "FrameCaptureGroupSettings": FrameCaptureGroupSettingsTypeDef,
         "HlsGroupSettings": HlsGroupSettingsTypeDef,
         "MediaPackageGroupSettings": MediaPackageGroupSettingsTypeDef,
@@ -5476,32 +4982,14 @@
         "MultiplexGroupSettings": Mapping[str, Any],
         "RtmpGroupSettings": RtmpGroupSettingsTypeDef,
         "UdpGroupSettings": UdpGroupSettingsTypeDef,
     },
     total=False,
 )
 
-InputSettingsOutputTypeDef = TypedDict(
-    "InputSettingsOutputTypeDef",
-    {
-        "AudioSelectors": List[AudioSelectorOutputTypeDef],
-        "CaptionSelectors": List[CaptionSelectorOutputTypeDef],
-        "DeblockFilter": InputDeblockFilterType,
-        "DenoiseFilter": InputDenoiseFilterType,
-        "FilterStrength": int,
-        "InputFilter": InputFilterType,
-        "NetworkInputSettings": NetworkInputSettingsTypeDef,
-        "Scte35Pid": int,
-        "Smpte2038DataPreference": Smpte2038DataPreferenceType,
-        "SourceEndBehavior": InputSourceEndBehaviorType,
-        "VideoSelector": VideoSelectorTypeDef,
-    },
-    total=False,
-)
-
 InputSettingsTypeDef = TypedDict(
     "InputSettingsTypeDef",
     {
         "AudioSelectors": Sequence[AudioSelectorTypeDef],
         "CaptionSelectors": Sequence[CaptionSelectorTypeDef],
         "DeblockFilter": InputDeblockFilterType,
         "DenoiseFilter": InputDenoiseFilterType,
@@ -5512,40 +5000,14 @@
         "Smpte2038DataPreference": Smpte2038DataPreferenceType,
         "SourceEndBehavior": InputSourceEndBehaviorType,
         "VideoSelector": VideoSelectorTypeDef,
     },
     total=False,
 )
 
-_RequiredVideoDescriptionOutputTypeDef = TypedDict(
-    "_RequiredVideoDescriptionOutputTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalVideoDescriptionOutputTypeDef = TypedDict(
-    "_OptionalVideoDescriptionOutputTypeDef",
-    {
-        "CodecSettings": VideoCodecSettingsOutputTypeDef,
-        "Height": int,
-        "RespondToAfd": VideoDescriptionRespondToAfdType,
-        "ScalingBehavior": VideoDescriptionScalingBehaviorType,
-        "Sharpness": int,
-        "Width": int,
-    },
-    total=False,
-)
-
-
-class VideoDescriptionOutputTypeDef(
-    _RequiredVideoDescriptionOutputTypeDef, _OptionalVideoDescriptionOutputTypeDef
-):
-    pass
-
-
 _RequiredVideoDescriptionTypeDef = TypedDict(
     "_RequiredVideoDescriptionTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalVideoDescriptionTypeDef = TypedDict(
@@ -5593,39 +5055,21 @@
     "UpdateMultiplexProgramResponseTypeDef",
     {
         "MultiplexProgram": MultiplexProgramTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-Scte35TimeSignalScheduleActionSettingsOutputTypeDef = TypedDict(
-    "Scte35TimeSignalScheduleActionSettingsOutputTypeDef",
-    {
-        "Scte35Descriptors": List[Scte35DescriptorTypeDef],
-    },
-)
-
 Scte35TimeSignalScheduleActionSettingsTypeDef = TypedDict(
     "Scte35TimeSignalScheduleActionSettingsTypeDef",
     {
         "Scte35Descriptors": Sequence[Scte35DescriptorTypeDef],
     },
 )
 
-InputAttachmentOutputTypeDef = TypedDict(
-    "InputAttachmentOutputTypeDef",
-    {
-        "AutomaticInputFailoverSettings": AutomaticInputFailoverSettingsOutputTypeDef,
-        "InputAttachmentName": str,
-        "InputId": str,
-        "InputSettings": InputSettingsOutputTypeDef,
-    },
-    total=False,
-)
-
 InputAttachmentTypeDef = TypedDict(
     "InputAttachmentTypeDef",
     {
         "AutomaticInputFailoverSettings": AutomaticInputFailoverSettingsTypeDef,
         "InputAttachmentName": str,
         "InputId": str,
         "InputSettings": InputSettingsTypeDef,
@@ -5651,34 +5095,14 @@
 )
 
 
 class OutputTypeDef(_RequiredOutputTypeDef, _OptionalOutputTypeDef):
     pass
 
 
-ScheduleActionSettingsOutputTypeDef = TypedDict(
-    "ScheduleActionSettingsOutputTypeDef",
-    {
-        "HlsId3SegmentTaggingSettings": HlsId3SegmentTaggingScheduleActionSettingsTypeDef,
-        "HlsTimedMetadataSettings": HlsTimedMetadataScheduleActionSettingsTypeDef,
-        "InputPrepareSettings": InputPrepareScheduleActionSettingsOutputTypeDef,
-        "InputSwitchSettings": InputSwitchScheduleActionSettingsOutputTypeDef,
-        "MotionGraphicsImageActivateSettings": MotionGraphicsActivateScheduleActionSettingsTypeDef,
-        "MotionGraphicsImageDeactivateSettings": Dict[str, Any],
-        "PauseStateSettings": PauseStateScheduleActionSettingsOutputTypeDef,
-        "Scte35InputSettings": Scte35InputScheduleActionSettingsTypeDef,
-        "Scte35ReturnToNetworkSettings": Scte35ReturnToNetworkScheduleActionSettingsTypeDef,
-        "Scte35SpliceInsertSettings": Scte35SpliceInsertScheduleActionSettingsTypeDef,
-        "Scte35TimeSignalSettings": Scte35TimeSignalScheduleActionSettingsOutputTypeDef,
-        "StaticImageActivateSettings": StaticImageActivateScheduleActionSettingsTypeDef,
-        "StaticImageDeactivateSettings": StaticImageDeactivateScheduleActionSettingsTypeDef,
-    },
-    total=False,
-)
-
 ScheduleActionSettingsTypeDef = TypedDict(
     "ScheduleActionSettingsTypeDef",
     {
         "HlsId3SegmentTaggingSettings": HlsId3SegmentTaggingScheduleActionSettingsTypeDef,
         "HlsTimedMetadataSettings": HlsTimedMetadataScheduleActionSettingsTypeDef,
         "InputPrepareSettings": InputPrepareScheduleActionSettingsTypeDef,
         "InputSwitchSettings": InputSwitchScheduleActionSettingsTypeDef,
@@ -5697,54 +5121,31 @@
 
 ChannelSummaryTypeDef = TypedDict(
     "ChannelSummaryTypeDef",
     {
         "Arn": str,
         "CdiInputSpecification": CdiInputSpecificationTypeDef,
         "ChannelClass": ChannelClassType,
-        "Destinations": List[OutputDestinationOutputTypeDef],
+        "Destinations": List[OutputDestinationTypeDef],
         "EgressEndpoints": List[ChannelEgressEndpointTypeDef],
         "Id": str,
-        "InputAttachments": List[InputAttachmentOutputTypeDef],
+        "InputAttachments": List[InputAttachmentTypeDef],
         "InputSpecification": InputSpecificationTypeDef,
         "LogLevel": LogLevelType,
         "Maintenance": MaintenanceStatusTypeDef,
         "Name": str,
         "PipelinesRunningCount": int,
         "RoleArn": str,
         "State": ChannelStateType,
         "Tags": Dict[str, str],
         "Vpc": VpcOutputSettingsDescriptionTypeDef,
     },
     total=False,
 )
 
-InputAttachmentUnionTypeDef = Union[InputAttachmentTypeDef, InputAttachmentOutputTypeDef]
-_RequiredOutputGroupOutputTypeDef = TypedDict(
-    "_RequiredOutputGroupOutputTypeDef",
-    {
-        "OutputGroupSettings": OutputGroupSettingsOutputTypeDef,
-        "Outputs": List[OutputTypeDef],
-    },
-)
-_OptionalOutputGroupOutputTypeDef = TypedDict(
-    "_OptionalOutputGroupOutputTypeDef",
-    {
-        "Name": str,
-    },
-    total=False,
-)
-
-
-class OutputGroupOutputTypeDef(
-    _RequiredOutputGroupOutputTypeDef, _OptionalOutputGroupOutputTypeDef
-):
-    pass
-
-
 _RequiredOutputGroupTypeDef = TypedDict(
     "_RequiredOutputGroupTypeDef",
     {
         "OutputGroupSettings": OutputGroupSettingsTypeDef,
         "Outputs": Sequence[OutputTypeDef],
     },
 )
@@ -5757,23 +5158,14 @@
 )
 
 
 class OutputGroupTypeDef(_RequiredOutputGroupTypeDef, _OptionalOutputGroupTypeDef):
     pass
 
 
-ScheduleActionOutputTypeDef = TypedDict(
-    "ScheduleActionOutputTypeDef",
-    {
-        "ActionName": str,
-        "ScheduleActionSettings": ScheduleActionSettingsOutputTypeDef,
-        "ScheduleActionStartSettings": ScheduleActionStartSettingsOutputTypeDef,
-    },
-)
-
 ScheduleActionTypeDef = TypedDict(
     "ScheduleActionTypeDef",
     {
         "ActionName": str,
         "ScheduleActionSettings": ScheduleActionSettingsTypeDef,
         "ScheduleActionStartSettings": ScheduleActionStartSettingsTypeDef,
     },
@@ -5784,45 +5176,14 @@
     {
         "Channels": List[ChannelSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredEncoderSettingsOutputTypeDef = TypedDict(
-    "_RequiredEncoderSettingsOutputTypeDef",
-    {
-        "AudioDescriptions": List[AudioDescriptionOutputTypeDef],
-        "OutputGroups": List[OutputGroupOutputTypeDef],
-        "TimecodeConfig": TimecodeConfigTypeDef,
-        "VideoDescriptions": List[VideoDescriptionOutputTypeDef],
-    },
-)
-_OptionalEncoderSettingsOutputTypeDef = TypedDict(
-    "_OptionalEncoderSettingsOutputTypeDef",
-    {
-        "AvailBlanking": AvailBlankingTypeDef,
-        "AvailConfiguration": AvailConfigurationTypeDef,
-        "BlackoutSlate": BlackoutSlateTypeDef,
-        "CaptionDescriptions": List[CaptionDescriptionOutputTypeDef],
-        "FeatureActivations": FeatureActivationsTypeDef,
-        "GlobalConfiguration": GlobalConfigurationTypeDef,
-        "MotionGraphicsConfiguration": MotionGraphicsConfigurationOutputTypeDef,
-        "NielsenConfiguration": NielsenConfigurationTypeDef,
-    },
-    total=False,
-)
-
-
-class EncoderSettingsOutputTypeDef(
-    _RequiredEncoderSettingsOutputTypeDef, _OptionalEncoderSettingsOutputTypeDef
-):
-    pass
-
-
 _RequiredEncoderSettingsTypeDef = TypedDict(
     "_RequiredEncoderSettingsTypeDef",
     {
         "AudioDescriptions": Sequence[AudioDescriptionTypeDef],
         "OutputGroups": Sequence[OutputGroupTypeDef],
         "TimecodeConfig": TimecodeConfigTypeDef,
         "VideoDescriptions": Sequence[VideoDescriptionTypeDef],
@@ -5835,89 +5196,111 @@
         "AvailConfiguration": AvailConfigurationTypeDef,
         "BlackoutSlate": BlackoutSlateTypeDef,
         "CaptionDescriptions": Sequence[CaptionDescriptionTypeDef],
         "FeatureActivations": FeatureActivationsTypeDef,
         "GlobalConfiguration": GlobalConfigurationTypeDef,
         "MotionGraphicsConfiguration": MotionGraphicsConfigurationTypeDef,
         "NielsenConfiguration": NielsenConfigurationTypeDef,
+        "ThumbnailConfiguration": ThumbnailConfigurationTypeDef,
     },
     total=False,
 )
 
 
 class EncoderSettingsTypeDef(_RequiredEncoderSettingsTypeDef, _OptionalEncoderSettingsTypeDef):
     pass
 
 
+BatchScheduleActionCreateRequestTypeDef = TypedDict(
+    "BatchScheduleActionCreateRequestTypeDef",
+    {
+        "ScheduleActions": Sequence[ScheduleActionTypeDef],
+    },
+)
+
 BatchScheduleActionCreateResultTypeDef = TypedDict(
     "BatchScheduleActionCreateResultTypeDef",
     {
-        "ScheduleActions": List[ScheduleActionOutputTypeDef],
+        "ScheduleActions": List[ScheduleActionTypeDef],
     },
 )
 
 BatchScheduleActionDeleteResultTypeDef = TypedDict(
     "BatchScheduleActionDeleteResultTypeDef",
     {
-        "ScheduleActions": List[ScheduleActionOutputTypeDef],
+        "ScheduleActions": List[ScheduleActionTypeDef],
     },
 )
 
 DescribeScheduleResponseTypeDef = TypedDict(
     "DescribeScheduleResponseTypeDef",
     {
         "NextToken": str,
-        "ScheduleActions": List[ScheduleActionOutputTypeDef],
+        "ScheduleActions": List[ScheduleActionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchScheduleActionCreateRequestTypeDef = TypedDict(
-    "BatchScheduleActionCreateRequestTypeDef",
-    {
-        "ScheduleActions": Sequence[ScheduleActionTypeDef],
-    },
-)
-
 ChannelTypeDef = TypedDict(
     "ChannelTypeDef",
     {
         "Arn": str,
         "CdiInputSpecification": CdiInputSpecificationTypeDef,
         "ChannelClass": ChannelClassType,
-        "Destinations": List[OutputDestinationOutputTypeDef],
+        "Destinations": List[OutputDestinationTypeDef],
         "EgressEndpoints": List[ChannelEgressEndpointTypeDef],
-        "EncoderSettings": EncoderSettingsOutputTypeDef,
+        "EncoderSettings": EncoderSettingsTypeDef,
         "Id": str,
-        "InputAttachments": List[InputAttachmentOutputTypeDef],
+        "InputAttachments": List[InputAttachmentTypeDef],
         "InputSpecification": InputSpecificationTypeDef,
         "LogLevel": LogLevelType,
         "Maintenance": MaintenanceStatusTypeDef,
         "Name": str,
         "PipelineDetails": List[PipelineDetailTypeDef],
         "PipelinesRunningCount": int,
         "RoleArn": str,
         "State": ChannelStateType,
         "Tags": Dict[str, str],
         "Vpc": VpcOutputSettingsDescriptionTypeDef,
     },
     total=False,
 )
 
+CreateChannelRequestRequestTypeDef = TypedDict(
+    "CreateChannelRequestRequestTypeDef",
+    {
+        "CdiInputSpecification": CdiInputSpecificationTypeDef,
+        "ChannelClass": ChannelClassType,
+        "Destinations": Sequence[OutputDestinationTypeDef],
+        "EncoderSettings": EncoderSettingsTypeDef,
+        "InputAttachments": Sequence[InputAttachmentTypeDef],
+        "InputSpecification": InputSpecificationTypeDef,
+        "LogLevel": LogLevelType,
+        "Maintenance": MaintenanceCreateSettingsTypeDef,
+        "Name": str,
+        "RequestId": str,
+        "Reserved": str,
+        "RoleArn": str,
+        "Tags": Mapping[str, str],
+        "Vpc": VpcOutputSettingsTypeDef,
+    },
+    total=False,
+)
+
 DeleteChannelResponseTypeDef = TypedDict(
     "DeleteChannelResponseTypeDef",
     {
         "Arn": str,
         "CdiInputSpecification": CdiInputSpecificationTypeDef,
         "ChannelClass": ChannelClassType,
-        "Destinations": List[OutputDestinationOutputTypeDef],
+        "Destinations": List[OutputDestinationTypeDef],
         "EgressEndpoints": List[ChannelEgressEndpointTypeDef],
-        "EncoderSettings": EncoderSettingsOutputTypeDef,
+        "EncoderSettings": EncoderSettingsTypeDef,
         "Id": str,
-        "InputAttachments": List[InputAttachmentOutputTypeDef],
+        "InputAttachments": List[InputAttachmentTypeDef],
         "InputSpecification": InputSpecificationTypeDef,
         "LogLevel": LogLevelType,
         "Maintenance": MaintenanceStatusTypeDef,
         "Name": str,
         "PipelineDetails": List[PipelineDetailTypeDef],
         "PipelinesRunningCount": int,
         "RoleArn": str,
@@ -5930,19 +5313,19 @@
 
 DescribeChannelResponseTypeDef = TypedDict(
     "DescribeChannelResponseTypeDef",
     {
         "Arn": str,
         "CdiInputSpecification": CdiInputSpecificationTypeDef,
         "ChannelClass": ChannelClassType,
-        "Destinations": List[OutputDestinationOutputTypeDef],
+        "Destinations": List[OutputDestinationTypeDef],
         "EgressEndpoints": List[ChannelEgressEndpointTypeDef],
-        "EncoderSettings": EncoderSettingsOutputTypeDef,
+        "EncoderSettings": EncoderSettingsTypeDef,
         "Id": str,
-        "InputAttachments": List[InputAttachmentOutputTypeDef],
+        "InputAttachments": List[InputAttachmentTypeDef],
         "InputSpecification": InputSpecificationTypeDef,
         "LogLevel": LogLevelType,
         "Maintenance": MaintenanceStatusTypeDef,
         "Name": str,
         "PipelineDetails": List[PipelineDetailTypeDef],
         "PipelinesRunningCount": int,
         "RoleArn": str,
@@ -5955,19 +5338,19 @@
 
 StartChannelResponseTypeDef = TypedDict(
     "StartChannelResponseTypeDef",
     {
         "Arn": str,
         "CdiInputSpecification": CdiInputSpecificationTypeDef,
         "ChannelClass": ChannelClassType,
-        "Destinations": List[OutputDestinationOutputTypeDef],
+        "Destinations": List[OutputDestinationTypeDef],
         "EgressEndpoints": List[ChannelEgressEndpointTypeDef],
-        "EncoderSettings": EncoderSettingsOutputTypeDef,
+        "EncoderSettings": EncoderSettingsTypeDef,
         "Id": str,
-        "InputAttachments": List[InputAttachmentOutputTypeDef],
+        "InputAttachments": List[InputAttachmentTypeDef],
         "InputSpecification": InputSpecificationTypeDef,
         "LogLevel": LogLevelType,
         "Maintenance": MaintenanceStatusTypeDef,
         "Name": str,
         "PipelineDetails": List[PipelineDetailTypeDef],
         "PipelinesRunningCount": int,
         "RoleArn": str,
@@ -5980,68 +5363,46 @@
 
 StopChannelResponseTypeDef = TypedDict(
     "StopChannelResponseTypeDef",
     {
         "Arn": str,
         "CdiInputSpecification": CdiInputSpecificationTypeDef,
         "ChannelClass": ChannelClassType,
-        "Destinations": List[OutputDestinationOutputTypeDef],
+        "Destinations": List[OutputDestinationTypeDef],
         "EgressEndpoints": List[ChannelEgressEndpointTypeDef],
-        "EncoderSettings": EncoderSettingsOutputTypeDef,
+        "EncoderSettings": EncoderSettingsTypeDef,
         "Id": str,
-        "InputAttachments": List[InputAttachmentOutputTypeDef],
+        "InputAttachments": List[InputAttachmentTypeDef],
         "InputSpecification": InputSpecificationTypeDef,
         "LogLevel": LogLevelType,
         "Maintenance": MaintenanceStatusTypeDef,
         "Name": str,
         "PipelineDetails": List[PipelineDetailTypeDef],
         "PipelinesRunningCount": int,
         "RoleArn": str,
         "State": ChannelStateType,
         "Tags": Dict[str, str],
         "Vpc": VpcOutputSettingsDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateChannelRequestRequestTypeDef = TypedDict(
-    "CreateChannelRequestRequestTypeDef",
-    {
-        "CdiInputSpecification": CdiInputSpecificationTypeDef,
-        "ChannelClass": ChannelClassType,
-        "Destinations": Sequence[OutputDestinationUnionTypeDef],
-        "EncoderSettings": EncoderSettingsTypeDef,
-        "InputAttachments": Sequence[InputAttachmentUnionTypeDef],
-        "InputSpecification": InputSpecificationTypeDef,
-        "LogLevel": LogLevelType,
-        "Maintenance": MaintenanceCreateSettingsTypeDef,
-        "Name": str,
-        "RequestId": str,
-        "Reserved": str,
-        "RoleArn": str,
-        "Tags": Mapping[str, str],
-        "Vpc": VpcOutputSettingsTypeDef,
-    },
-    total=False,
-)
-
-EncoderSettingsUnionTypeDef = Union[EncoderSettingsTypeDef, EncoderSettingsOutputTypeDef]
 _RequiredUpdateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateChannelRequestRequestTypeDef",
     {
         "ChannelId": str,
     },
 )
 _OptionalUpdateChannelRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateChannelRequestRequestTypeDef",
     {
         "CdiInputSpecification": CdiInputSpecificationTypeDef,
-        "Destinations": Sequence[OutputDestinationUnionTypeDef],
+        "Destinations": Sequence[OutputDestinationTypeDef],
         "EncoderSettings": EncoderSettingsTypeDef,
-        "InputAttachments": Sequence[InputAttachmentUnionTypeDef],
+        "InputAttachments": Sequence[InputAttachmentTypeDef],
         "InputSpecification": InputSpecificationTypeDef,
         "LogLevel": LogLevelType,
         "Maintenance": MaintenanceUpdateSettingsTypeDef,
         "Name": str,
         "RoleArn": str,
     },
     total=False,
@@ -6050,23 +5411,14 @@
 
 class UpdateChannelRequestRequestTypeDef(
     _RequiredUpdateChannelRequestRequestTypeDef, _OptionalUpdateChannelRequestRequestTypeDef
 ):
     pass
 
 
-BatchUpdateScheduleResponseTypeDef = TypedDict(
-    "BatchUpdateScheduleResponseTypeDef",
-    {
-        "Creates": BatchScheduleActionCreateResultTypeDef,
-        "Deletes": BatchScheduleActionDeleteResultTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredBatchUpdateScheduleRequestRequestTypeDef = TypedDict(
     "_RequiredBatchUpdateScheduleRequestRequestTypeDef",
     {
         "ChannelId": str,
     },
 )
 _OptionalBatchUpdateScheduleRequestRequestTypeDef = TypedDict(
@@ -6082,14 +5434,23 @@
 class BatchUpdateScheduleRequestRequestTypeDef(
     _RequiredBatchUpdateScheduleRequestRequestTypeDef,
     _OptionalBatchUpdateScheduleRequestRequestTypeDef,
 ):
     pass
 
 
+BatchUpdateScheduleResponseTypeDef = TypedDict(
+    "BatchUpdateScheduleResponseTypeDef",
+    {
+        "Creates": BatchScheduleActionCreateResultTypeDef,
+        "Deletes": BatchScheduleActionDeleteResultTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateChannelResponseTypeDef = TypedDict(
     "CreateChannelResponseTypeDef",
     {
         "Channel": ChannelTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-medialive-2.5.2.post1/types_aiobotocore_medialive/type_defs.pyi` & `types-aiobotocore-medialive-2.5.2.post2/types_aiobotocore_medialive/type_defs.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_medialive.type_defs import AacSettingsTypeDef
 
     data: AacSettingsTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Any, Dict, List, Mapping, Sequence, Union
+from typing import Any, Dict, List, Mapping, Sequence
 
 from aiobotocore.response import StreamingBody
 
 from .literals import (
     AacCodingModeType,
     AacInputTypeType,
     AacProfileType,
@@ -261,14 +261,16 @@
     SmoothGroupSegmentationModeType,
     SmoothGroupSparseTrackTypeType,
     SmoothGroupStreamManifestBehaviorType,
     SmoothGroupTimestampOffsetModeType,
     Smpte2038DataPreferenceType,
     TemporalFilterPostFilterSharpeningType,
     TemporalFilterStrengthType,
+    ThumbnailStateType,
+    ThumbnailTypeType,
     TimecodeBurninFontSizeType,
     TimecodeBurninPositionType,
     TimecodeConfigSourceType,
     TtmlDestinationStyleControlType,
     UdpTimedMetadataId3FrameType,
     VideoDescriptionRespondToAfdType,
     VideoDescriptionScalingBehaviorType,
@@ -287,14 +289,15 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AacSettingsTypeDef",
     "Ac3SettingsTypeDef",
     "AcceptInputDeviceTransferRequestRequestTypeDef",
+    "AccountConfigurationTypeDef",
     "AncillarySourceSettingsTypeDef",
     "ArchiveS3SettingsTypeDef",
     "OutputLocationRefTypeDef",
     "InputChannelLevelTypeDef",
     "Eac3AtmosSettingsTypeDef",
     "Eac3SettingsTypeDef",
     "Mp2SettingsTypeDef",
@@ -371,30 +374,31 @@
     "InputWhitelistRuleTypeDef",
     "DescribeMultiplexProgramRequestRequestTypeDef",
     "DescribeMultiplexRequestRequestTypeDef",
     "DescribeOfferingRequestRequestTypeDef",
     "DescribeReservationRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeScheduleRequestRequestTypeDef",
+    "DescribeThumbnailsRequestRequestTypeDef",
     "DvbNitSettingsTypeDef",
     "DvbSdtSettingsTypeDef",
     "DvbTdtSettingsTypeDef",
     "FeatureActivationsTypeDef",
     "NielsenConfigurationTypeDef",
+    "ThumbnailConfigurationTypeDef",
     "TimecodeConfigTypeDef",
     "InputLossFailoverSettingsTypeDef",
     "VideoBlackFailoverSettingsTypeDef",
     "FecOutputSettingsTypeDef",
     "FixedModeScheduleActionStartSettingsTypeDef",
     "Fmp4HlsSettingsTypeDef",
     "FollowModeScheduleActionStartSettingsTypeDef",
     "FrameCaptureS3SettingsTypeDef",
     "FrameCaptureOutputSettingsTypeDef",
     "TimecodeBurninSettingsTypeDef",
-    "H264ColorSpaceSettingsOutputTypeDef",
     "H264ColorSpaceSettingsTypeDef",
     "TemporalFilterSettingsTypeDef",
     "Hdr10SettingsTypeDef",
     "HlsAkamaiSettingsTypeDef",
     "HlsBasicPutSettingsTypeDef",
     "HlsMediaStoreSettingsTypeDef",
     "HlsS3SettingsTypeDef",
@@ -419,70 +423,69 @@
     "ListOfferingsRequestRequestTypeDef",
     "ListReservationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "M3u8SettingsTypeDef",
     "MaintenanceUpdateSettingsTypeDef",
     "MediaPackageOutputDestinationSettingsTypeDef",
     "MotionGraphicsActivateScheduleActionSettingsTypeDef",
-    "MotionGraphicsSettingsOutputTypeDef",
     "MotionGraphicsSettingsTypeDef",
     "MsSmoothOutputSettingsTypeDef",
     "MultiplexMediaConnectOutputDestinationSettingsTypeDef",
     "MultiplexProgramChannelDestinationSettingsTypeDef",
     "MultiplexProgramServiceDescriptorTypeDef",
     "MultiplexSettingsSummaryTypeDef",
     "MultiplexStatmuxVideoSettingsTypeDef",
     "NielsenCBETTypeDef",
     "NielsenNaesIiNwTypeDef",
     "OutputDestinationSettingsTypeDef",
-    "RtmpGroupSettingsOutputTypeDef",
-    "UdpGroupSettingsTypeDef",
     "RtmpGroupSettingsTypeDef",
+    "UdpGroupSettingsTypeDef",
     "PipelinePauseStateSettingsTypeDef",
     "RebootInputDeviceRequestRequestTypeDef",
     "RejectInputDeviceTransferRequestRequestTypeDef",
     "Scte35InputScheduleActionSettingsTypeDef",
     "Scte35ReturnToNetworkScheduleActionSettingsTypeDef",
     "Scte35SpliceInsertScheduleActionSettingsTypeDef",
     "StaticImageDeactivateScheduleActionSettingsTypeDef",
     "Scte35DeliveryRestrictionsTypeDef",
     "StartChannelRequestRequestTypeDef",
     "StartInputDeviceMaintenanceWindowRequestRequestTypeDef",
     "StartMultiplexRequestRequestTypeDef",
     "StopChannelRequestRequestTypeDef",
     "StopMultiplexRequestRequestTypeDef",
+    "ThumbnailTypeDef",
     "TransferInputDeviceRequestRequestTypeDef",
     "VideoSelectorPidTypeDef",
     "VideoSelectorProgramIdTypeDef",
+    "UpdateAccountConfigurationRequestRequestTypeDef",
     "ArchiveCdnSettingsTypeDef",
     "MediaPackageGroupSettingsTypeDef",
     "MsSmoothGroupSettingsTypeDef",
     "MultiplexOutputSettingsTypeDef",
     "RtmpOutputSettingsTypeDef",
-    "AudioChannelMappingOutputTypeDef",
     "AudioChannelMappingTypeDef",
-    "AudioCodecSettingsOutputTypeDef",
     "AudioCodecSettingsTypeDef",
     "AudioOnlyHlsSettingsTypeDef",
     "AvailBlankingTypeDef",
     "BlackoutSlateTypeDef",
     "BurnInDestinationSettingsTypeDef",
     "DvbSubDestinationSettingsTypeDef",
     "InputLossBehaviorTypeDef",
     "StaticImageActivateScheduleActionSettingsTypeDef",
     "StaticKeySettingsTypeDef",
-    "AudioTrackSelectionOutputTypeDef",
     "AudioTrackSelectionTypeDef",
     "AvailSettingsTypeDef",
     "BatchDeleteResponseTypeDef",
     "BatchStartResponseTypeDef",
     "BatchStopResponseTypeDef",
+    "DescribeAccountConfigurationResponseTypeDef",
     "DescribeInputDeviceThumbnailResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "UpdateAccountConfigurationResponseTypeDef",
     "TeletextSourceSettingsTypeDef",
     "CreateInputRequestRequestTypeDef",
     "CreateInputSecurityGroupRequestRequestTypeDef",
     "UpdateInputSecurityGroupRequestRequestTypeDef",
     "CreateMultiplexRequestRequestTypeDef",
     "UpdateMultiplexRequestRequestTypeDef",
     "PurchaseOfferingRequestRequestTypeDef",
@@ -516,161 +519,131 @@
     "ListInputsRequestListInputsPaginateTypeDef",
     "ListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef",
     "ListMultiplexesRequestListMultiplexesPaginateTypeDef",
     "ListOfferingsRequestListOfferingsPaginateTypeDef",
     "ListReservationsRequestListReservationsPaginateTypeDef",
     "M2tsSettingsTypeDef",
     "FailoverConditionSettingsTypeDef",
-    "ScheduleActionStartSettingsOutputTypeDef",
     "ScheduleActionStartSettingsTypeDef",
     "FrameCaptureCdnSettingsTypeDef",
     "FrameCaptureSettingsTypeDef",
     "H264FilterSettingsTypeDef",
     "H265FilterSettingsTypeDef",
     "Mpeg2FilterSettingsTypeDef",
-    "H265ColorSpaceSettingsOutputTypeDef",
     "H265ColorSpaceSettingsTypeDef",
     "VideoSelectorColorSpaceSettingsTypeDef",
     "HlsCdnSettingsTypeDef",
     "NetworkInputSettingsTypeDef",
     "InputClippingSettingsTypeDef",
     "InputDestinationTypeDef",
     "UpdateInputDeviceRequestRequestTypeDef",
     "UpdateInputRequestRequestTypeDef",
     "ListInputDeviceTransfersResponseTypeDef",
     "ListMultiplexProgramsResponseTypeDef",
     "StandardHlsSettingsTypeDef",
-    "MotionGraphicsConfigurationOutputTypeDef",
     "MotionGraphicsConfigurationTypeDef",
     "MultiplexOutputDestinationTypeDef",
     "MultiplexSummaryTypeDef",
     "MultiplexVideoSettingsTypeDef",
     "NielsenWatermarksSettingsTypeDef",
-    "OutputDestinationOutputTypeDef",
     "OutputDestinationTypeDef",
-    "PauseStateScheduleActionSettingsOutputTypeDef",
     "PauseStateScheduleActionSettingsTypeDef",
     "Scte35SegmentationDescriptorTypeDef",
+    "ThumbnailDetailTypeDef",
     "VideoSelectorSettingsTypeDef",
     "ArchiveGroupSettingsTypeDef",
-    "RemixSettingsOutputTypeDef",
     "RemixSettingsTypeDef",
-    "CaptionDestinationSettingsOutputTypeDef",
     "CaptionDestinationSettingsTypeDef",
     "GlobalConfigurationTypeDef",
     "KeyProviderSettingsTypeDef",
-    "AudioSelectorSettingsOutputTypeDef",
     "AudioSelectorSettingsTypeDef",
     "AvailConfigurationTypeDef",
-    "CaptionSelectorSettingsOutputTypeDef",
     "CaptionSelectorSettingsTypeDef",
     "ListOfferingsResponseTypeDef",
     "ListReservationsResponseTypeDef",
     "PurchaseOfferingResponseTypeDef",
     "UpdateReservationResponseTypeDef",
     "ListInputDevicesResponseTypeDef",
     "CreateInputSecurityGroupResponseTypeDef",
     "ListInputSecurityGroupsResponseTypeDef",
     "UpdateInputSecurityGroupResponseTypeDef",
     "ArchiveContainerSettingsTypeDef",
     "UdpContainerSettingsTypeDef",
     "FailoverConditionTypeDef",
     "FrameCaptureGroupSettingsTypeDef",
-    "H264SettingsOutputTypeDef",
     "H264SettingsTypeDef",
     "Mpeg2SettingsTypeDef",
-    "H265SettingsOutputTypeDef",
     "H265SettingsTypeDef",
-    "InputPrepareScheduleActionSettingsOutputTypeDef",
     "InputPrepareScheduleActionSettingsTypeDef",
-    "InputSwitchScheduleActionSettingsOutputTypeDef",
     "InputSwitchScheduleActionSettingsTypeDef",
     "DescribeInputResponseTypeDef",
     "InputTypeDef",
     "HlsSettingsTypeDef",
     "DeleteMultiplexResponseTypeDef",
     "DescribeMultiplexResponseTypeDef",
     "MultiplexTypeDef",
     "StartMultiplexResponseTypeDef",
     "StopMultiplexResponseTypeDef",
     "ListMultiplexesResponseTypeDef",
     "MultiplexProgramSettingsTypeDef",
     "AudioWatermarkSettingsTypeDef",
-    "OutputDestinationUnionTypeDef",
+    "UpdateChannelClassRequestRequestTypeDef",
     "Scte35DescriptorSettingsTypeDef",
+    "DescribeThumbnailsResponseTypeDef",
     "VideoSelectorTypeDef",
-    "CaptionDescriptionOutputTypeDef",
     "CaptionDescriptionTypeDef",
-    "HlsGroupSettingsOutputTypeDef",
     "HlsGroupSettingsTypeDef",
-    "AudioSelectorOutputTypeDef",
     "AudioSelectorTypeDef",
-    "CaptionSelectorOutputTypeDef",
     "CaptionSelectorTypeDef",
     "ArchiveOutputSettingsTypeDef",
     "UdpOutputSettingsTypeDef",
-    "AutomaticInputFailoverSettingsOutputTypeDef",
     "AutomaticInputFailoverSettingsTypeDef",
-    "VideoCodecSettingsOutputTypeDef",
     "VideoCodecSettingsTypeDef",
     "CreateInputResponseTypeDef",
     "CreatePartnerInputResponseTypeDef",
     "ListInputsResponseTypeDef",
     "UpdateInputResponseTypeDef",
     "HlsOutputSettingsTypeDef",
     "CreateMultiplexResponseTypeDef",
     "UpdateMultiplexResponseTypeDef",
     "CreateMultiplexProgramRequestRequestTypeDef",
     "DeleteMultiplexProgramResponseTypeDef",
     "DescribeMultiplexProgramResponseTypeDef",
     "MultiplexProgramTypeDef",
     "UpdateMultiplexProgramRequestRequestTypeDef",
-    "AudioDescriptionOutputTypeDef",
     "AudioDescriptionTypeDef",
-    "UpdateChannelClassRequestRequestTypeDef",
     "Scte35DescriptorTypeDef",
-    "OutputGroupSettingsOutputTypeDef",
     "OutputGroupSettingsTypeDef",
-    "InputSettingsOutputTypeDef",
     "InputSettingsTypeDef",
-    "VideoDescriptionOutputTypeDef",
     "VideoDescriptionTypeDef",
     "OutputSettingsTypeDef",
     "CreateMultiplexProgramResponseTypeDef",
     "UpdateMultiplexProgramResponseTypeDef",
-    "Scte35TimeSignalScheduleActionSettingsOutputTypeDef",
     "Scte35TimeSignalScheduleActionSettingsTypeDef",
-    "InputAttachmentOutputTypeDef",
     "InputAttachmentTypeDef",
     "OutputTypeDef",
-    "ScheduleActionSettingsOutputTypeDef",
     "ScheduleActionSettingsTypeDef",
     "ChannelSummaryTypeDef",
-    "InputAttachmentUnionTypeDef",
-    "OutputGroupOutputTypeDef",
     "OutputGroupTypeDef",
-    "ScheduleActionOutputTypeDef",
     "ScheduleActionTypeDef",
     "ListChannelsResponseTypeDef",
-    "EncoderSettingsOutputTypeDef",
     "EncoderSettingsTypeDef",
+    "BatchScheduleActionCreateRequestTypeDef",
     "BatchScheduleActionCreateResultTypeDef",
     "BatchScheduleActionDeleteResultTypeDef",
     "DescribeScheduleResponseTypeDef",
-    "BatchScheduleActionCreateRequestTypeDef",
     "ChannelTypeDef",
+    "CreateChannelRequestRequestTypeDef",
     "DeleteChannelResponseTypeDef",
     "DescribeChannelResponseTypeDef",
     "StartChannelResponseTypeDef",
     "StopChannelResponseTypeDef",
-    "CreateChannelRequestRequestTypeDef",
-    "EncoderSettingsUnionTypeDef",
     "UpdateChannelRequestRequestTypeDef",
-    "BatchUpdateScheduleResponseTypeDef",
     "BatchUpdateScheduleRequestRequestTypeDef",
+    "BatchUpdateScheduleResponseTypeDef",
     "CreateChannelResponseTypeDef",
     "UpdateChannelClassResponseTypeDef",
     "UpdateChannelResponseTypeDef",
 )
 
 AacSettingsTypeDef = TypedDict(
     "AacSettingsTypeDef",
@@ -705,14 +678,22 @@
 AcceptInputDeviceTransferRequestRequestTypeDef = TypedDict(
     "AcceptInputDeviceTransferRequestRequestTypeDef",
     {
         "InputDeviceId": str,
     },
 )
 
+AccountConfigurationTypeDef = TypedDict(
+    "AccountConfigurationTypeDef",
+    {
+        "KmsKeyId": str,
+    },
+    total=False,
+)
+
 AncillarySourceSettingsTypeDef = TypedDict(
     "AncillarySourceSettingsTypeDef",
     {
         "SourceAncillaryChannelNumber": int,
     },
     total=False,
 )
@@ -1595,14 +1576,23 @@
 )
 
 class DescribeScheduleRequestRequestTypeDef(
     _RequiredDescribeScheduleRequestRequestTypeDef, _OptionalDescribeScheduleRequestRequestTypeDef
 ):
     pass
 
+DescribeThumbnailsRequestRequestTypeDef = TypedDict(
+    "DescribeThumbnailsRequestRequestTypeDef",
+    {
+        "ChannelId": str,
+        "PipelineId": str,
+        "ThumbnailType": str,
+    },
+)
+
 _RequiredDvbNitSettingsTypeDef = TypedDict(
     "_RequiredDvbNitSettingsTypeDef",
     {
         "NetworkId": int,
         "NetworkName": str,
     },
 )
@@ -1649,14 +1639,21 @@
     {
         "DistributorId": str,
         "NielsenPcmToId3Tagging": NielsenPcmToId3TaggingStateType,
     },
     total=False,
 )
 
+ThumbnailConfigurationTypeDef = TypedDict(
+    "ThumbnailConfigurationTypeDef",
+    {
+        "State": ThumbnailStateType,
+    },
+)
+
 _RequiredTimecodeConfigTypeDef = TypedDict(
     "_RequiredTimecodeConfigTypeDef",
     {
         "Source": TimecodeConfigSourceType,
     },
 )
 _OptionalTimecodeConfigTypeDef = TypedDict(
@@ -1754,24 +1751,14 @@
 )
 
 class TimecodeBurninSettingsTypeDef(
     _RequiredTimecodeBurninSettingsTypeDef, _OptionalTimecodeBurninSettingsTypeDef
 ):
     pass
 
-H264ColorSpaceSettingsOutputTypeDef = TypedDict(
-    "H264ColorSpaceSettingsOutputTypeDef",
-    {
-        "ColorSpacePassthroughSettings": Dict[str, Any],
-        "Rec601Settings": Dict[str, Any],
-        "Rec709Settings": Dict[str, Any],
-    },
-    total=False,
-)
-
 H264ColorSpaceSettingsTypeDef = TypedDict(
     "H264ColorSpaceSettingsTypeDef",
     {
         "ColorSpacePassthroughSettings": Mapping[str, Any],
         "Rec601Settings": Mapping[str, Any],
         "Rec709Settings": Mapping[str, Any],
     },
@@ -2124,22 +2111,14 @@
         "PasswordParam": str,
         "Url": str,
         "Username": str,
     },
     total=False,
 )
 
-MotionGraphicsSettingsOutputTypeDef = TypedDict(
-    "MotionGraphicsSettingsOutputTypeDef",
-    {
-        "HtmlMotionGraphicsSettings": Dict[str, Any],
-    },
-    total=False,
-)
-
 MotionGraphicsSettingsTypeDef = TypedDict(
     "MotionGraphicsSettingsTypeDef",
     {
         "HtmlMotionGraphicsSettings": Mapping[str, Any],
     },
     total=False,
 )
@@ -2230,18 +2209,18 @@
         "StreamName": str,
         "Url": str,
         "Username": str,
     },
     total=False,
 )
 
-RtmpGroupSettingsOutputTypeDef = TypedDict(
-    "RtmpGroupSettingsOutputTypeDef",
+RtmpGroupSettingsTypeDef = TypedDict(
+    "RtmpGroupSettingsTypeDef",
     {
-        "AdMarkers": List[Literal["ON_CUE_POINT_SCTE35"]],
+        "AdMarkers": Sequence[Literal["ON_CUE_POINT_SCTE35"]],
         "AuthenticationScheme": AuthenticationSchemeType,
         "CacheFullBehavior": RtmpCacheFullBehaviorType,
         "CacheLength": int,
         "CaptionData": RtmpCaptionDataType,
         "InputLossAction": InputLossActionForRtmpOutType,
         "RestartDelay": int,
     },
@@ -2254,28 +2233,14 @@
         "InputLossAction": InputLossActionForUdpOutType,
         "TimedMetadataId3Frame": UdpTimedMetadataId3FrameType,
         "TimedMetadataId3Period": int,
     },
     total=False,
 )
 
-RtmpGroupSettingsTypeDef = TypedDict(
-    "RtmpGroupSettingsTypeDef",
-    {
-        "AdMarkers": Sequence[Literal["ON_CUE_POINT_SCTE35"]],
-        "AuthenticationScheme": AuthenticationSchemeType,
-        "CacheFullBehavior": RtmpCacheFullBehaviorType,
-        "CacheLength": int,
-        "CaptionData": RtmpCaptionDataType,
-        "InputLossAction": InputLossActionForRtmpOutType,
-        "RestartDelay": int,
-    },
-    total=False,
-)
-
 PipelinePauseStateSettingsTypeDef = TypedDict(
     "PipelinePauseStateSettingsTypeDef",
     {
         "PipelineId": PipelineIdType,
     },
 )
 
@@ -2402,14 +2367,25 @@
 StopMultiplexRequestRequestTypeDef = TypedDict(
     "StopMultiplexRequestRequestTypeDef",
     {
         "MultiplexId": str,
     },
 )
 
+ThumbnailTypeDef = TypedDict(
+    "ThumbnailTypeDef",
+    {
+        "Body": str,
+        "ContentType": str,
+        "ThumbnailType": ThumbnailTypeType,
+        "TimeStamp": datetime,
+    },
+    total=False,
+)
+
 _RequiredTransferInputDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredTransferInputDeviceRequestRequestTypeDef",
     {
         "InputDeviceId": str,
     },
 )
 _OptionalTransferInputDeviceRequestRequestTypeDef = TypedDict(
@@ -2440,14 +2416,22 @@
     "VideoSelectorProgramIdTypeDef",
     {
         "ProgramId": int,
     },
     total=False,
 )
 
+UpdateAccountConfigurationRequestRequestTypeDef = TypedDict(
+    "UpdateAccountConfigurationRequestRequestTypeDef",
+    {
+        "AccountConfiguration": AccountConfigurationTypeDef,
+    },
+    total=False,
+)
+
 ArchiveCdnSettingsTypeDef = TypedDict(
     "ArchiveCdnSettingsTypeDef",
     {
         "ArchiveS3Settings": ArchiveS3SettingsTypeDef,
     },
     total=False,
 )
@@ -2519,44 +2503,22 @@
 )
 
 class RtmpOutputSettingsTypeDef(
     _RequiredRtmpOutputSettingsTypeDef, _OptionalRtmpOutputSettingsTypeDef
 ):
     pass
 
-AudioChannelMappingOutputTypeDef = TypedDict(
-    "AudioChannelMappingOutputTypeDef",
-    {
-        "InputChannelLevels": List[InputChannelLevelTypeDef],
-        "OutputChannel": int,
-    },
-)
-
 AudioChannelMappingTypeDef = TypedDict(
     "AudioChannelMappingTypeDef",
     {
         "InputChannelLevels": Sequence[InputChannelLevelTypeDef],
         "OutputChannel": int,
     },
 )
 
-AudioCodecSettingsOutputTypeDef = TypedDict(
-    "AudioCodecSettingsOutputTypeDef",
-    {
-        "AacSettings": AacSettingsTypeDef,
-        "Ac3Settings": Ac3SettingsTypeDef,
-        "Eac3AtmosSettings": Eac3AtmosSettingsTypeDef,
-        "Eac3Settings": Eac3SettingsTypeDef,
-        "Mp2Settings": Mp2SettingsTypeDef,
-        "PassThroughSettings": Dict[str, Any],
-        "WavSettings": WavSettingsTypeDef,
-    },
-    total=False,
-)
-
 AudioCodecSettingsTypeDef = TypedDict(
     "AudioCodecSettingsTypeDef",
     {
         "AacSettings": AacSettingsTypeDef,
         "Ac3Settings": Ac3SettingsTypeDef,
         "Eac3AtmosSettings": Eac3AtmosSettingsTypeDef,
         "Eac3Settings": Eac3SettingsTypeDef,
@@ -2702,33 +2664,14 @@
 )
 
 class StaticKeySettingsTypeDef(
     _RequiredStaticKeySettingsTypeDef, _OptionalStaticKeySettingsTypeDef
 ):
     pass
 
-_RequiredAudioTrackSelectionOutputTypeDef = TypedDict(
-    "_RequiredAudioTrackSelectionOutputTypeDef",
-    {
-        "Tracks": List[AudioTrackTypeDef],
-    },
-)
-_OptionalAudioTrackSelectionOutputTypeDef = TypedDict(
-    "_OptionalAudioTrackSelectionOutputTypeDef",
-    {
-        "DolbyEDecode": AudioDolbyEDecodeTypeDef,
-    },
-    total=False,
-)
-
-class AudioTrackSelectionOutputTypeDef(
-    _RequiredAudioTrackSelectionOutputTypeDef, _OptionalAudioTrackSelectionOutputTypeDef
-):
-    pass
-
 _RequiredAudioTrackSelectionTypeDef = TypedDict(
     "_RequiredAudioTrackSelectionTypeDef",
     {
         "Tracks": Sequence[AudioTrackTypeDef],
     },
 )
 _OptionalAudioTrackSelectionTypeDef = TypedDict(
@@ -2777,14 +2720,22 @@
     {
         "Failed": List[BatchFailedResultModelTypeDef],
         "Successful": List[BatchSuccessfulResultModelTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeAccountConfigurationResponseTypeDef = TypedDict(
+    "DescribeAccountConfigurationResponseTypeDef",
+    {
+        "AccountConfiguration": AccountConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeInputDeviceThumbnailResponseTypeDef = TypedDict(
     "DescribeInputDeviceThumbnailResponseTypeDef",
     {
         "Body": StreamingBody,
         "ContentType": Literal["image/jpeg"],
         "ContentLength": int,
         "ETag": str,
@@ -2804,14 +2755,22 @@
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+UpdateAccountConfigurationResponseTypeDef = TypedDict(
+    "UpdateAccountConfigurationResponseTypeDef",
+    {
+        "AccountConfiguration": AccountConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 TeletextSourceSettingsTypeDef = TypedDict(
     "TeletextSourceSettingsTypeDef",
     {
         "OutputRectangle": CaptionRectangleTypeDef,
         "PageNumber": str,
     },
     total=False,
@@ -3297,14 +3256,15 @@
         "MacAddress": str,
         "Name": str,
         "NetworkSettings": InputDeviceNetworkSettingsTypeDef,
         "SerialNumber": str,
         "Type": InputDeviceTypeType,
         "UhdDeviceSettings": InputDeviceUhdSettingsTypeDef,
         "Tags": Dict[str, str],
+        "AvailabilityZone": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InputDeviceSummaryTypeDef = TypedDict(
     "InputDeviceSummaryTypeDef",
     {
@@ -3317,14 +3277,15 @@
         "MacAddress": str,
         "Name": str,
         "NetworkSettings": InputDeviceNetworkSettingsTypeDef,
         "SerialNumber": str,
         "Type": InputDeviceTypeType,
         "UhdDeviceSettings": InputDeviceUhdSettingsTypeDef,
         "Tags": Dict[str, str],
+        "AvailabilityZone": str,
     },
     total=False,
 )
 
 UpdateInputDeviceResponseTypeDef = TypedDict(
     "UpdateInputDeviceResponseTypeDef",
     {
@@ -3337,14 +3298,15 @@
         "MacAddress": str,
         "Name": str,
         "NetworkSettings": InputDeviceNetworkSettingsTypeDef,
         "SerialNumber": str,
         "Type": InputDeviceTypeType,
         "UhdDeviceSettings": InputDeviceUhdSettingsTypeDef,
         "Tags": Dict[str, str],
+        "AvailabilityZone": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeInputSecurityGroupResponseTypeDef = TypedDict(
     "DescribeInputSecurityGroupResponseTypeDef",
     {
@@ -3566,24 +3528,14 @@
         "AudioSilenceSettings": AudioSilenceFailoverSettingsTypeDef,
         "InputLossSettings": InputLossFailoverSettingsTypeDef,
         "VideoBlackSettings": VideoBlackFailoverSettingsTypeDef,
     },
     total=False,
 )
 
-ScheduleActionStartSettingsOutputTypeDef = TypedDict(
-    "ScheduleActionStartSettingsOutputTypeDef",
-    {
-        "FixedModeScheduleActionStartSettings": FixedModeScheduleActionStartSettingsTypeDef,
-        "FollowModeScheduleActionStartSettings": FollowModeScheduleActionStartSettingsTypeDef,
-        "ImmediateModeScheduleActionStartSettings": Dict[str, Any],
-    },
-    total=False,
-)
-
 ScheduleActionStartSettingsTypeDef = TypedDict(
     "ScheduleActionStartSettingsTypeDef",
     {
         "FixedModeScheduleActionStartSettings": FixedModeScheduleActionStartSettingsTypeDef,
         "FollowModeScheduleActionStartSettings": FollowModeScheduleActionStartSettingsTypeDef,
         "ImmediateModeScheduleActionStartSettings": Mapping[str, Any],
     },
@@ -3628,26 +3580,14 @@
     "Mpeg2FilterSettingsTypeDef",
     {
         "TemporalFilterSettings": TemporalFilterSettingsTypeDef,
     },
     total=False,
 )
 
-H265ColorSpaceSettingsOutputTypeDef = TypedDict(
-    "H265ColorSpaceSettingsOutputTypeDef",
-    {
-        "ColorSpacePassthroughSettings": Dict[str, Any],
-        "DolbyVision81Settings": Dict[str, Any],
-        "Hdr10Settings": Hdr10SettingsTypeDef,
-        "Rec601Settings": Dict[str, Any],
-        "Rec709Settings": Dict[str, Any],
-    },
-    total=False,
-)
-
 H265ColorSpaceSettingsTypeDef = TypedDict(
     "H265ColorSpaceSettingsTypeDef",
     {
         "ColorSpacePassthroughSettings": Mapping[str, Any],
         "DolbyVision81Settings": Mapping[str, Any],
         "Hdr10Settings": Hdr10SettingsTypeDef,
         "Rec601Settings": Mapping[str, Any],
@@ -3724,14 +3664,15 @@
 )
 _OptionalUpdateInputDeviceRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateInputDeviceRequestRequestTypeDef",
     {
         "HdDeviceSettings": InputDeviceConfigurableSettingsTypeDef,
         "Name": str,
         "UhdDeviceSettings": InputDeviceConfigurableSettingsTypeDef,
+        "AvailabilityZone": str,
     },
     total=False,
 )
 
 class UpdateInputDeviceRequestRequestTypeDef(
     _RequiredUpdateInputDeviceRequestRequestTypeDef, _OptionalUpdateInputDeviceRequestRequestTypeDef
 ):
@@ -3795,34 +3736,14 @@
 )
 
 class StandardHlsSettingsTypeDef(
     _RequiredStandardHlsSettingsTypeDef, _OptionalStandardHlsSettingsTypeDef
 ):
     pass
 
-_RequiredMotionGraphicsConfigurationOutputTypeDef = TypedDict(
-    "_RequiredMotionGraphicsConfigurationOutputTypeDef",
-    {
-        "MotionGraphicsSettings": MotionGraphicsSettingsOutputTypeDef,
-    },
-)
-_OptionalMotionGraphicsConfigurationOutputTypeDef = TypedDict(
-    "_OptionalMotionGraphicsConfigurationOutputTypeDef",
-    {
-        "MotionGraphicsInsertion": MotionGraphicsInsertionType,
-    },
-    total=False,
-)
-
-class MotionGraphicsConfigurationOutputTypeDef(
-    _RequiredMotionGraphicsConfigurationOutputTypeDef,
-    _OptionalMotionGraphicsConfigurationOutputTypeDef,
-):
-    pass
-
 _RequiredMotionGraphicsConfigurationTypeDef = TypedDict(
     "_RequiredMotionGraphicsConfigurationTypeDef",
     {
         "MotionGraphicsSettings": MotionGraphicsSettingsTypeDef,
     },
 )
 _OptionalMotionGraphicsConfigurationTypeDef = TypedDict(
@@ -3877,44 +3798,25 @@
         "NielsenCbetSettings": NielsenCBETTypeDef,
         "NielsenDistributionType": NielsenWatermarksDistributionTypesType,
         "NielsenNaesIiNwSettings": NielsenNaesIiNwTypeDef,
     },
     total=False,
 )
 
-OutputDestinationOutputTypeDef = TypedDict(
-    "OutputDestinationOutputTypeDef",
-    {
-        "Id": str,
-        "MediaPackageSettings": List[MediaPackageOutputDestinationSettingsTypeDef],
-        "MultiplexSettings": MultiplexProgramChannelDestinationSettingsTypeDef,
-        "Settings": List[OutputDestinationSettingsTypeDef],
-    },
-    total=False,
-)
-
 OutputDestinationTypeDef = TypedDict(
     "OutputDestinationTypeDef",
     {
         "Id": str,
         "MediaPackageSettings": Sequence[MediaPackageOutputDestinationSettingsTypeDef],
         "MultiplexSettings": MultiplexProgramChannelDestinationSettingsTypeDef,
         "Settings": Sequence[OutputDestinationSettingsTypeDef],
     },
     total=False,
 )
 
-PauseStateScheduleActionSettingsOutputTypeDef = TypedDict(
-    "PauseStateScheduleActionSettingsOutputTypeDef",
-    {
-        "Pipelines": List[PipelinePauseStateSettingsTypeDef],
-    },
-    total=False,
-)
-
 PauseStateScheduleActionSettingsTypeDef = TypedDict(
     "PauseStateScheduleActionSettingsTypeDef",
     {
         "Pipelines": Sequence[PipelinePauseStateSettingsTypeDef],
     },
     total=False,
 )
@@ -3943,14 +3845,23 @@
 )
 
 class Scte35SegmentationDescriptorTypeDef(
     _RequiredScte35SegmentationDescriptorTypeDef, _OptionalScte35SegmentationDescriptorTypeDef
 ):
     pass
 
+ThumbnailDetailTypeDef = TypedDict(
+    "ThumbnailDetailTypeDef",
+    {
+        "PipelineId": str,
+        "Thumbnails": List[ThumbnailTypeDef],
+    },
+    total=False,
+)
+
 VideoSelectorSettingsTypeDef = TypedDict(
     "VideoSelectorSettingsTypeDef",
     {
         "VideoSelectorPid": VideoSelectorPidTypeDef,
         "VideoSelectorProgramId": VideoSelectorProgramIdTypeDef,
     },
     total=False,
@@ -3972,34 +3883,14 @@
 )
 
 class ArchiveGroupSettingsTypeDef(
     _RequiredArchiveGroupSettingsTypeDef, _OptionalArchiveGroupSettingsTypeDef
 ):
     pass
 
-_RequiredRemixSettingsOutputTypeDef = TypedDict(
-    "_RequiredRemixSettingsOutputTypeDef",
-    {
-        "ChannelMappings": List[AudioChannelMappingOutputTypeDef],
-    },
-)
-_OptionalRemixSettingsOutputTypeDef = TypedDict(
-    "_OptionalRemixSettingsOutputTypeDef",
-    {
-        "ChannelsIn": int,
-        "ChannelsOut": int,
-    },
-    total=False,
-)
-
-class RemixSettingsOutputTypeDef(
-    _RequiredRemixSettingsOutputTypeDef, _OptionalRemixSettingsOutputTypeDef
-):
-    pass
-
 _RequiredRemixSettingsTypeDef = TypedDict(
     "_RequiredRemixSettingsTypeDef",
     {
         "ChannelMappings": Sequence[AudioChannelMappingTypeDef],
     },
 )
 _OptionalRemixSettingsTypeDef = TypedDict(
@@ -4010,34 +3901,14 @@
     },
     total=False,
 )
 
 class RemixSettingsTypeDef(_RequiredRemixSettingsTypeDef, _OptionalRemixSettingsTypeDef):
     pass
 
-CaptionDestinationSettingsOutputTypeDef = TypedDict(
-    "CaptionDestinationSettingsOutputTypeDef",
-    {
-        "AribDestinationSettings": Dict[str, Any],
-        "BurnInDestinationSettings": BurnInDestinationSettingsTypeDef,
-        "DvbSubDestinationSettings": DvbSubDestinationSettingsTypeDef,
-        "EbuTtDDestinationSettings": EbuTtDDestinationSettingsTypeDef,
-        "EmbeddedDestinationSettings": Dict[str, Any],
-        "EmbeddedPlusScte20DestinationSettings": Dict[str, Any],
-        "RtmpCaptionInfoDestinationSettings": Dict[str, Any],
-        "Scte20PlusEmbeddedDestinationSettings": Dict[str, Any],
-        "Scte27DestinationSettings": Dict[str, Any],
-        "SmpteTtDestinationSettings": Dict[str, Any],
-        "TeletextDestinationSettings": Dict[str, Any],
-        "TtmlDestinationSettings": TtmlDestinationSettingsTypeDef,
-        "WebvttDestinationSettings": WebvttDestinationSettingsTypeDef,
-    },
-    total=False,
-)
-
 CaptionDestinationSettingsTypeDef = TypedDict(
     "CaptionDestinationSettingsTypeDef",
     {
         "AribDestinationSettings": Mapping[str, Any],
         "BurnInDestinationSettings": BurnInDestinationSettingsTypeDef,
         "DvbSubDestinationSettings": DvbSubDestinationSettingsTypeDef,
         "EbuTtDDestinationSettings": EbuTtDDestinationSettingsTypeDef,
@@ -4071,25 +3942,14 @@
     "KeyProviderSettingsTypeDef",
     {
         "StaticKeySettings": StaticKeySettingsTypeDef,
     },
     total=False,
 )
 
-AudioSelectorSettingsOutputTypeDef = TypedDict(
-    "AudioSelectorSettingsOutputTypeDef",
-    {
-        "AudioHlsRenditionSelection": AudioHlsRenditionSelectionTypeDef,
-        "AudioLanguageSelection": AudioLanguageSelectionTypeDef,
-        "AudioPidSelection": AudioPidSelectionTypeDef,
-        "AudioTrackSelection": AudioTrackSelectionOutputTypeDef,
-    },
-    total=False,
-)
-
 AudioSelectorSettingsTypeDef = TypedDict(
     "AudioSelectorSettingsTypeDef",
     {
         "AudioHlsRenditionSelection": AudioHlsRenditionSelectionTypeDef,
         "AudioLanguageSelection": AudioLanguageSelectionTypeDef,
         "AudioPidSelection": AudioPidSelectionTypeDef,
         "AudioTrackSelection": AudioTrackSelectionTypeDef,
@@ -4101,28 +3961,14 @@
     "AvailConfigurationTypeDef",
     {
         "AvailSettings": AvailSettingsTypeDef,
     },
     total=False,
 )
 
-CaptionSelectorSettingsOutputTypeDef = TypedDict(
-    "CaptionSelectorSettingsOutputTypeDef",
-    {
-        "AncillarySourceSettings": AncillarySourceSettingsTypeDef,
-        "AribSourceSettings": Dict[str, Any],
-        "DvbSubSourceSettings": DvbSubSourceSettingsTypeDef,
-        "EmbeddedSourceSettings": EmbeddedSourceSettingsTypeDef,
-        "Scte20SourceSettings": Scte20SourceSettingsTypeDef,
-        "Scte27SourceSettings": Scte27SourceSettingsTypeDef,
-        "TeletextSourceSettings": TeletextSourceSettingsTypeDef,
-    },
-    total=False,
-)
-
 CaptionSelectorSettingsTypeDef = TypedDict(
     "CaptionSelectorSettingsTypeDef",
     {
         "AncillarySourceSettings": AncillarySourceSettingsTypeDef,
         "AribSourceSettings": Mapping[str, Any],
         "DvbSubSourceSettings": DvbSubSourceSettingsTypeDef,
         "EmbeddedSourceSettings": EmbeddedSourceSettingsTypeDef,
@@ -4241,63 +4087,14 @@
 )
 
 class FrameCaptureGroupSettingsTypeDef(
     _RequiredFrameCaptureGroupSettingsTypeDef, _OptionalFrameCaptureGroupSettingsTypeDef
 ):
     pass
 
-H264SettingsOutputTypeDef = TypedDict(
-    "H264SettingsOutputTypeDef",
-    {
-        "AdaptiveQuantization": H264AdaptiveQuantizationType,
-        "AfdSignaling": AfdSignalingType,
-        "Bitrate": int,
-        "BufFillPct": int,
-        "BufSize": int,
-        "ColorMetadata": H264ColorMetadataType,
-        "ColorSpaceSettings": H264ColorSpaceSettingsOutputTypeDef,
-        "EntropyEncoding": H264EntropyEncodingType,
-        "FilterSettings": H264FilterSettingsTypeDef,
-        "FixedAfd": FixedAfdType,
-        "FlickerAq": H264FlickerAqType,
-        "ForceFieldPictures": H264ForceFieldPicturesType,
-        "FramerateControl": H264FramerateControlType,
-        "FramerateDenominator": int,
-        "FramerateNumerator": int,
-        "GopBReference": H264GopBReferenceType,
-        "GopClosedCadence": int,
-        "GopNumBFrames": int,
-        "GopSize": float,
-        "GopSizeUnits": H264GopSizeUnitsType,
-        "Level": H264LevelType,
-        "LookAheadRateControl": H264LookAheadRateControlType,
-        "MaxBitrate": int,
-        "MinIInterval": int,
-        "NumRefFrames": int,
-        "ParControl": H264ParControlType,
-        "ParDenominator": int,
-        "ParNumerator": int,
-        "Profile": H264ProfileType,
-        "QualityLevel": H264QualityLevelType,
-        "QvbrQualityLevel": int,
-        "RateControlMode": H264RateControlModeType,
-        "ScanType": H264ScanTypeType,
-        "SceneChangeDetect": H264SceneChangeDetectType,
-        "Slices": int,
-        "Softness": int,
-        "SpatialAq": H264SpatialAqType,
-        "SubgopLength": H264SubGopLengthType,
-        "Syntax": H264SyntaxType,
-        "TemporalAq": H264TemporalAqType,
-        "TimecodeInsertion": H264TimecodeInsertionBehaviorType,
-        "TimecodeBurninSettings": TimecodeBurninSettingsTypeDef,
-    },
-    total=False,
-)
-
 H264SettingsTypeDef = TypedDict(
     "H264SettingsTypeDef",
     {
         "AdaptiveQuantization": H264AdaptiveQuantizationType,
         "AfdSignaling": AfdSignalingType,
         "Bitrate": int,
         "BufFillPct": int,
@@ -4371,61 +4168,14 @@
     },
     total=False,
 )
 
 class Mpeg2SettingsTypeDef(_RequiredMpeg2SettingsTypeDef, _OptionalMpeg2SettingsTypeDef):
     pass
 
-_RequiredH265SettingsOutputTypeDef = TypedDict(
-    "_RequiredH265SettingsOutputTypeDef",
-    {
-        "FramerateDenominator": int,
-        "FramerateNumerator": int,
-    },
-)
-_OptionalH265SettingsOutputTypeDef = TypedDict(
-    "_OptionalH265SettingsOutputTypeDef",
-    {
-        "AdaptiveQuantization": H265AdaptiveQuantizationType,
-        "AfdSignaling": AfdSignalingType,
-        "AlternativeTransferFunction": H265AlternativeTransferFunctionType,
-        "Bitrate": int,
-        "BufSize": int,
-        "ColorMetadata": H265ColorMetadataType,
-        "ColorSpaceSettings": H265ColorSpaceSettingsOutputTypeDef,
-        "FilterSettings": H265FilterSettingsTypeDef,
-        "FixedAfd": FixedAfdType,
-        "FlickerAq": H265FlickerAqType,
-        "GopClosedCadence": int,
-        "GopSize": float,
-        "GopSizeUnits": H265GopSizeUnitsType,
-        "Level": H265LevelType,
-        "LookAheadRateControl": H265LookAheadRateControlType,
-        "MaxBitrate": int,
-        "MinIInterval": int,
-        "ParDenominator": int,
-        "ParNumerator": int,
-        "Profile": H265ProfileType,
-        "QvbrQualityLevel": int,
-        "RateControlMode": H265RateControlModeType,
-        "ScanType": H265ScanTypeType,
-        "SceneChangeDetect": H265SceneChangeDetectType,
-        "Slices": int,
-        "Tier": H265TierType,
-        "TimecodeInsertion": H265TimecodeInsertionBehaviorType,
-        "TimecodeBurninSettings": TimecodeBurninSettingsTypeDef,
-    },
-    total=False,
-)
-
-class H265SettingsOutputTypeDef(
-    _RequiredH265SettingsOutputTypeDef, _OptionalH265SettingsOutputTypeDef
-):
-    pass
-
 _RequiredH265SettingsTypeDef = TypedDict(
     "_RequiredH265SettingsTypeDef",
     {
         "FramerateDenominator": int,
         "FramerateNumerator": int,
     },
 )
@@ -4463,55 +4213,24 @@
     },
     total=False,
 )
 
 class H265SettingsTypeDef(_RequiredH265SettingsTypeDef, _OptionalH265SettingsTypeDef):
     pass
 
-InputPrepareScheduleActionSettingsOutputTypeDef = TypedDict(
-    "InputPrepareScheduleActionSettingsOutputTypeDef",
-    {
-        "InputAttachmentNameReference": str,
-        "InputClippingSettings": InputClippingSettingsTypeDef,
-        "UrlPath": List[str],
-    },
-    total=False,
-)
-
 InputPrepareScheduleActionSettingsTypeDef = TypedDict(
     "InputPrepareScheduleActionSettingsTypeDef",
     {
         "InputAttachmentNameReference": str,
         "InputClippingSettings": InputClippingSettingsTypeDef,
         "UrlPath": Sequence[str],
     },
     total=False,
 )
 
-_RequiredInputSwitchScheduleActionSettingsOutputTypeDef = TypedDict(
-    "_RequiredInputSwitchScheduleActionSettingsOutputTypeDef",
-    {
-        "InputAttachmentNameReference": str,
-    },
-)
-_OptionalInputSwitchScheduleActionSettingsOutputTypeDef = TypedDict(
-    "_OptionalInputSwitchScheduleActionSettingsOutputTypeDef",
-    {
-        "InputClippingSettings": InputClippingSettingsTypeDef,
-        "UrlPath": List[str],
-    },
-    total=False,
-)
-
-class InputSwitchScheduleActionSettingsOutputTypeDef(
-    _RequiredInputSwitchScheduleActionSettingsOutputTypeDef,
-    _OptionalInputSwitchScheduleActionSettingsOutputTypeDef,
-):
-    pass
-
 _RequiredInputSwitchScheduleActionSettingsTypeDef = TypedDict(
     "_RequiredInputSwitchScheduleActionSettingsTypeDef",
     {
         "InputAttachmentNameReference": str,
     },
 )
 _OptionalInputSwitchScheduleActionSettingsTypeDef = TypedDict(
@@ -4705,56 +4424,61 @@
     "AudioWatermarkSettingsTypeDef",
     {
         "NielsenWatermarksSettings": NielsenWatermarksSettingsTypeDef,
     },
     total=False,
 )
 
-OutputDestinationUnionTypeDef = Union[OutputDestinationTypeDef, OutputDestinationOutputTypeDef]
+_RequiredUpdateChannelClassRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateChannelClassRequestRequestTypeDef",
+    {
+        "ChannelClass": ChannelClassType,
+        "ChannelId": str,
+    },
+)
+_OptionalUpdateChannelClassRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateChannelClassRequestRequestTypeDef",
+    {
+        "Destinations": Sequence[OutputDestinationTypeDef],
+    },
+    total=False,
+)
+
+class UpdateChannelClassRequestRequestTypeDef(
+    _RequiredUpdateChannelClassRequestRequestTypeDef,
+    _OptionalUpdateChannelClassRequestRequestTypeDef,
+):
+    pass
+
 Scte35DescriptorSettingsTypeDef = TypedDict(
     "Scte35DescriptorSettingsTypeDef",
     {
         "SegmentationDescriptorScte35DescriptorSettings": Scte35SegmentationDescriptorTypeDef,
     },
 )
 
+DescribeThumbnailsResponseTypeDef = TypedDict(
+    "DescribeThumbnailsResponseTypeDef",
+    {
+        "ThumbnailDetails": List[ThumbnailDetailTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 VideoSelectorTypeDef = TypedDict(
     "VideoSelectorTypeDef",
     {
         "ColorSpace": VideoSelectorColorSpaceType,
         "ColorSpaceSettings": VideoSelectorColorSpaceSettingsTypeDef,
         "ColorSpaceUsage": VideoSelectorColorSpaceUsageType,
         "SelectorSettings": VideoSelectorSettingsTypeDef,
     },
     total=False,
 )
 
-_RequiredCaptionDescriptionOutputTypeDef = TypedDict(
-    "_RequiredCaptionDescriptionOutputTypeDef",
-    {
-        "CaptionSelectorName": str,
-        "Name": str,
-    },
-)
-_OptionalCaptionDescriptionOutputTypeDef = TypedDict(
-    "_OptionalCaptionDescriptionOutputTypeDef",
-    {
-        "Accessibility": AccessibilityTypeType,
-        "DestinationSettings": CaptionDestinationSettingsOutputTypeDef,
-        "LanguageCode": str,
-        "LanguageDescription": str,
-    },
-    total=False,
-)
-
-class CaptionDescriptionOutputTypeDef(
-    _RequiredCaptionDescriptionOutputTypeDef, _OptionalCaptionDescriptionOutputTypeDef
-):
-    pass
-
 _RequiredCaptionDescriptionTypeDef = TypedDict(
     "_RequiredCaptionDescriptionTypeDef",
     {
         "CaptionSelectorName": str,
         "Name": str,
     },
 )
@@ -4770,74 +4494,14 @@
 )
 
 class CaptionDescriptionTypeDef(
     _RequiredCaptionDescriptionTypeDef, _OptionalCaptionDescriptionTypeDef
 ):
     pass
 
-_RequiredHlsGroupSettingsOutputTypeDef = TypedDict(
-    "_RequiredHlsGroupSettingsOutputTypeDef",
-    {
-        "Destination": OutputLocationRefTypeDef,
-    },
-)
-_OptionalHlsGroupSettingsOutputTypeDef = TypedDict(
-    "_OptionalHlsGroupSettingsOutputTypeDef",
-    {
-        "AdMarkers": List[HlsAdMarkersType],
-        "BaseUrlContent": str,
-        "BaseUrlContent1": str,
-        "BaseUrlManifest": str,
-        "BaseUrlManifest1": str,
-        "CaptionLanguageMappings": List[CaptionLanguageMappingTypeDef],
-        "CaptionLanguageSetting": HlsCaptionLanguageSettingType,
-        "ClientCache": HlsClientCacheType,
-        "CodecSpecification": HlsCodecSpecificationType,
-        "ConstantIv": str,
-        "DirectoryStructure": HlsDirectoryStructureType,
-        "DiscontinuityTags": HlsDiscontinuityTagsType,
-        "EncryptionType": HlsEncryptionTypeType,
-        "HlsCdnSettings": HlsCdnSettingsTypeDef,
-        "HlsId3SegmentTagging": HlsId3SegmentTaggingStateType,
-        "IFrameOnlyPlaylists": IFrameOnlyPlaylistTypeType,
-        "IncompleteSegmentBehavior": HlsIncompleteSegmentBehaviorType,
-        "IndexNSegments": int,
-        "InputLossAction": InputLossActionForHlsOutType,
-        "IvInManifest": HlsIvInManifestType,
-        "IvSource": HlsIvSourceType,
-        "KeepSegments": int,
-        "KeyFormat": str,
-        "KeyFormatVersions": str,
-        "KeyProviderSettings": KeyProviderSettingsTypeDef,
-        "ManifestCompression": HlsManifestCompressionType,
-        "ManifestDurationFormat": HlsManifestDurationFormatType,
-        "MinSegmentLength": int,
-        "Mode": HlsModeType,
-        "OutputSelection": HlsOutputSelectionType,
-        "ProgramDateTime": HlsProgramDateTimeType,
-        "ProgramDateTimeClock": HlsProgramDateTimeClockType,
-        "ProgramDateTimePeriod": int,
-        "RedundantManifest": HlsRedundantManifestType,
-        "SegmentLength": int,
-        "SegmentationMode": HlsSegmentationModeType,
-        "SegmentsPerSubdirectory": int,
-        "StreamInfResolution": HlsStreamInfResolutionType,
-        "TimedMetadataId3Frame": HlsTimedMetadataId3FrameType,
-        "TimedMetadataId3Period": int,
-        "TimestampDeltaMilliseconds": int,
-        "TsFileMode": HlsTsFileModeType,
-    },
-    total=False,
-)
-
-class HlsGroupSettingsOutputTypeDef(
-    _RequiredHlsGroupSettingsOutputTypeDef, _OptionalHlsGroupSettingsOutputTypeDef
-):
-    pass
-
 _RequiredHlsGroupSettingsTypeDef = TypedDict(
     "_RequiredHlsGroupSettingsTypeDef",
     {
         "Destination": OutputLocationRefTypeDef,
     },
 )
 _OptionalHlsGroupSettingsTypeDef = TypedDict(
@@ -4888,33 +4552,14 @@
     },
     total=False,
 )
 
 class HlsGroupSettingsTypeDef(_RequiredHlsGroupSettingsTypeDef, _OptionalHlsGroupSettingsTypeDef):
     pass
 
-_RequiredAudioSelectorOutputTypeDef = TypedDict(
-    "_RequiredAudioSelectorOutputTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalAudioSelectorOutputTypeDef = TypedDict(
-    "_OptionalAudioSelectorOutputTypeDef",
-    {
-        "SelectorSettings": AudioSelectorSettingsOutputTypeDef,
-    },
-    total=False,
-)
-
-class AudioSelectorOutputTypeDef(
-    _RequiredAudioSelectorOutputTypeDef, _OptionalAudioSelectorOutputTypeDef
-):
-    pass
-
 _RequiredAudioSelectorTypeDef = TypedDict(
     "_RequiredAudioSelectorTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalAudioSelectorTypeDef = TypedDict(
@@ -4924,34 +4569,14 @@
     },
     total=False,
 )
 
 class AudioSelectorTypeDef(_RequiredAudioSelectorTypeDef, _OptionalAudioSelectorTypeDef):
     pass
 
-_RequiredCaptionSelectorOutputTypeDef = TypedDict(
-    "_RequiredCaptionSelectorOutputTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalCaptionSelectorOutputTypeDef = TypedDict(
-    "_OptionalCaptionSelectorOutputTypeDef",
-    {
-        "LanguageCode": str,
-        "SelectorSettings": CaptionSelectorSettingsOutputTypeDef,
-    },
-    total=False,
-)
-
-class CaptionSelectorOutputTypeDef(
-    _RequiredCaptionSelectorOutputTypeDef, _OptionalCaptionSelectorOutputTypeDef
-):
-    pass
-
 _RequiredCaptionSelectorTypeDef = TypedDict(
     "_RequiredCaptionSelectorTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCaptionSelectorTypeDef = TypedDict(
@@ -5003,36 +4628,14 @@
 )
 
 class UdpOutputSettingsTypeDef(
     _RequiredUdpOutputSettingsTypeDef, _OptionalUdpOutputSettingsTypeDef
 ):
     pass
 
-_RequiredAutomaticInputFailoverSettingsOutputTypeDef = TypedDict(
-    "_RequiredAutomaticInputFailoverSettingsOutputTypeDef",
-    {
-        "SecondaryInputId": str,
-    },
-)
-_OptionalAutomaticInputFailoverSettingsOutputTypeDef = TypedDict(
-    "_OptionalAutomaticInputFailoverSettingsOutputTypeDef",
-    {
-        "ErrorClearTimeMsec": int,
-        "FailoverConditions": List[FailoverConditionTypeDef],
-        "InputPreference": InputPreferenceType,
-    },
-    total=False,
-)
-
-class AutomaticInputFailoverSettingsOutputTypeDef(
-    _RequiredAutomaticInputFailoverSettingsOutputTypeDef,
-    _OptionalAutomaticInputFailoverSettingsOutputTypeDef,
-):
-    pass
-
 _RequiredAutomaticInputFailoverSettingsTypeDef = TypedDict(
     "_RequiredAutomaticInputFailoverSettingsTypeDef",
     {
         "SecondaryInputId": str,
     },
 )
 _OptionalAutomaticInputFailoverSettingsTypeDef = TypedDict(
@@ -5046,25 +4649,14 @@
 )
 
 class AutomaticInputFailoverSettingsTypeDef(
     _RequiredAutomaticInputFailoverSettingsTypeDef, _OptionalAutomaticInputFailoverSettingsTypeDef
 ):
     pass
 
-VideoCodecSettingsOutputTypeDef = TypedDict(
-    "VideoCodecSettingsOutputTypeDef",
-    {
-        "FrameCaptureSettings": FrameCaptureSettingsTypeDef,
-        "H264Settings": H264SettingsOutputTypeDef,
-        "H265Settings": H265SettingsOutputTypeDef,
-        "Mpeg2Settings": Mpeg2SettingsTypeDef,
-    },
-    total=False,
-)
-
 VideoCodecSettingsTypeDef = TypedDict(
     "VideoCodecSettingsTypeDef",
     {
         "FrameCaptureSettings": FrameCaptureSettingsTypeDef,
         "H264Settings": H264SettingsTypeDef,
         "H265Settings": H265SettingsTypeDef,
         "Mpeg2Settings": Mpeg2SettingsTypeDef,
@@ -5205,42 +4797,14 @@
 
 class UpdateMultiplexProgramRequestRequestTypeDef(
     _RequiredUpdateMultiplexProgramRequestRequestTypeDef,
     _OptionalUpdateMultiplexProgramRequestRequestTypeDef,
 ):
     pass
 
-_RequiredAudioDescriptionOutputTypeDef = TypedDict(
-    "_RequiredAudioDescriptionOutputTypeDef",
-    {
-        "AudioSelectorName": str,
-        "Name": str,
-    },
-)
-_OptionalAudioDescriptionOutputTypeDef = TypedDict(
-    "_OptionalAudioDescriptionOutputTypeDef",
-    {
-        "AudioNormalizationSettings": AudioNormalizationSettingsTypeDef,
-        "AudioType": AudioTypeType,
-        "AudioTypeControl": AudioDescriptionAudioTypeControlType,
-        "AudioWatermarkingSettings": AudioWatermarkSettingsTypeDef,
-        "CodecSettings": AudioCodecSettingsOutputTypeDef,
-        "LanguageCode": str,
-        "LanguageCodeControl": AudioDescriptionLanguageCodeControlType,
-        "RemixSettings": RemixSettingsOutputTypeDef,
-        "StreamName": str,
-    },
-    total=False,
-)
-
-class AudioDescriptionOutputTypeDef(
-    _RequiredAudioDescriptionOutputTypeDef, _OptionalAudioDescriptionOutputTypeDef
-):
-    pass
-
 _RequiredAudioDescriptionTypeDef = TypedDict(
     "_RequiredAudioDescriptionTypeDef",
     {
         "AudioSelectorName": str,
         "Name": str,
     },
 )
@@ -5259,57 +4823,21 @@
     },
     total=False,
 )
 
 class AudioDescriptionTypeDef(_RequiredAudioDescriptionTypeDef, _OptionalAudioDescriptionTypeDef):
     pass
 
-_RequiredUpdateChannelClassRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateChannelClassRequestRequestTypeDef",
-    {
-        "ChannelClass": ChannelClassType,
-        "ChannelId": str,
-    },
-)
-_OptionalUpdateChannelClassRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateChannelClassRequestRequestTypeDef",
-    {
-        "Destinations": Sequence[OutputDestinationUnionTypeDef],
-    },
-    total=False,
-)
-
-class UpdateChannelClassRequestRequestTypeDef(
-    _RequiredUpdateChannelClassRequestRequestTypeDef,
-    _OptionalUpdateChannelClassRequestRequestTypeDef,
-):
-    pass
-
 Scte35DescriptorTypeDef = TypedDict(
     "Scte35DescriptorTypeDef",
     {
         "Scte35DescriptorSettings": Scte35DescriptorSettingsTypeDef,
     },
 )
 
-OutputGroupSettingsOutputTypeDef = TypedDict(
-    "OutputGroupSettingsOutputTypeDef",
-    {
-        "ArchiveGroupSettings": ArchiveGroupSettingsTypeDef,
-        "FrameCaptureGroupSettings": FrameCaptureGroupSettingsTypeDef,
-        "HlsGroupSettings": HlsGroupSettingsOutputTypeDef,
-        "MediaPackageGroupSettings": MediaPackageGroupSettingsTypeDef,
-        "MsSmoothGroupSettings": MsSmoothGroupSettingsTypeDef,
-        "MultiplexGroupSettings": Dict[str, Any],
-        "RtmpGroupSettings": RtmpGroupSettingsOutputTypeDef,
-        "UdpGroupSettings": UdpGroupSettingsTypeDef,
-    },
-    total=False,
-)
-
 OutputGroupSettingsTypeDef = TypedDict(
     "OutputGroupSettingsTypeDef",
     {
         "ArchiveGroupSettings": ArchiveGroupSettingsTypeDef,
         "FrameCaptureGroupSettings": FrameCaptureGroupSettingsTypeDef,
         "HlsGroupSettings": HlsGroupSettingsTypeDef,
         "MediaPackageGroupSettings": MediaPackageGroupSettingsTypeDef,
@@ -5317,32 +4845,14 @@
         "MultiplexGroupSettings": Mapping[str, Any],
         "RtmpGroupSettings": RtmpGroupSettingsTypeDef,
         "UdpGroupSettings": UdpGroupSettingsTypeDef,
     },
     total=False,
 )
 
-InputSettingsOutputTypeDef = TypedDict(
-    "InputSettingsOutputTypeDef",
-    {
-        "AudioSelectors": List[AudioSelectorOutputTypeDef],
-        "CaptionSelectors": List[CaptionSelectorOutputTypeDef],
-        "DeblockFilter": InputDeblockFilterType,
-        "DenoiseFilter": InputDenoiseFilterType,
-        "FilterStrength": int,
-        "InputFilter": InputFilterType,
-        "NetworkInputSettings": NetworkInputSettingsTypeDef,
-        "Scte35Pid": int,
-        "Smpte2038DataPreference": Smpte2038DataPreferenceType,
-        "SourceEndBehavior": InputSourceEndBehaviorType,
-        "VideoSelector": VideoSelectorTypeDef,
-    },
-    total=False,
-)
-
 InputSettingsTypeDef = TypedDict(
     "InputSettingsTypeDef",
     {
         "AudioSelectors": Sequence[AudioSelectorTypeDef],
         "CaptionSelectors": Sequence[CaptionSelectorTypeDef],
         "DeblockFilter": InputDeblockFilterType,
         "DenoiseFilter": InputDenoiseFilterType,
@@ -5353,38 +4863,14 @@
         "Smpte2038DataPreference": Smpte2038DataPreferenceType,
         "SourceEndBehavior": InputSourceEndBehaviorType,
         "VideoSelector": VideoSelectorTypeDef,
     },
     total=False,
 )
 
-_RequiredVideoDescriptionOutputTypeDef = TypedDict(
-    "_RequiredVideoDescriptionOutputTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalVideoDescriptionOutputTypeDef = TypedDict(
-    "_OptionalVideoDescriptionOutputTypeDef",
-    {
-        "CodecSettings": VideoCodecSettingsOutputTypeDef,
-        "Height": int,
-        "RespondToAfd": VideoDescriptionRespondToAfdType,
-        "ScalingBehavior": VideoDescriptionScalingBehaviorType,
-        "Sharpness": int,
-        "Width": int,
-    },
-    total=False,
-)
-
-class VideoDescriptionOutputTypeDef(
-    _RequiredVideoDescriptionOutputTypeDef, _OptionalVideoDescriptionOutputTypeDef
-):
-    pass
-
 _RequiredVideoDescriptionTypeDef = TypedDict(
     "_RequiredVideoDescriptionTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalVideoDescriptionTypeDef = TypedDict(
@@ -5430,39 +4916,21 @@
     "UpdateMultiplexProgramResponseTypeDef",
     {
         "MultiplexProgram": MultiplexProgramTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-Scte35TimeSignalScheduleActionSettingsOutputTypeDef = TypedDict(
-    "Scte35TimeSignalScheduleActionSettingsOutputTypeDef",
-    {
-        "Scte35Descriptors": List[Scte35DescriptorTypeDef],
-    },
-)
-
 Scte35TimeSignalScheduleActionSettingsTypeDef = TypedDict(
     "Scte35TimeSignalScheduleActionSettingsTypeDef",
     {
         "Scte35Descriptors": Sequence[Scte35DescriptorTypeDef],
     },
 )
 
-InputAttachmentOutputTypeDef = TypedDict(
-    "InputAttachmentOutputTypeDef",
-    {
-        "AutomaticInputFailoverSettings": AutomaticInputFailoverSettingsOutputTypeDef,
-        "InputAttachmentName": str,
-        "InputId": str,
-        "InputSettings": InputSettingsOutputTypeDef,
-    },
-    total=False,
-)
-
 InputAttachmentTypeDef = TypedDict(
     "InputAttachmentTypeDef",
     {
         "AutomaticInputFailoverSettings": AutomaticInputFailoverSettingsTypeDef,
         "InputAttachmentName": str,
         "InputId": str,
         "InputSettings": InputSettingsTypeDef,
@@ -5486,34 +4954,14 @@
     },
     total=False,
 )
 
 class OutputTypeDef(_RequiredOutputTypeDef, _OptionalOutputTypeDef):
     pass
 
-ScheduleActionSettingsOutputTypeDef = TypedDict(
-    "ScheduleActionSettingsOutputTypeDef",
-    {
-        "HlsId3SegmentTaggingSettings": HlsId3SegmentTaggingScheduleActionSettingsTypeDef,
-        "HlsTimedMetadataSettings": HlsTimedMetadataScheduleActionSettingsTypeDef,
-        "InputPrepareSettings": InputPrepareScheduleActionSettingsOutputTypeDef,
-        "InputSwitchSettings": InputSwitchScheduleActionSettingsOutputTypeDef,
-        "MotionGraphicsImageActivateSettings": MotionGraphicsActivateScheduleActionSettingsTypeDef,
-        "MotionGraphicsImageDeactivateSettings": Dict[str, Any],
-        "PauseStateSettings": PauseStateScheduleActionSettingsOutputTypeDef,
-        "Scte35InputSettings": Scte35InputScheduleActionSettingsTypeDef,
-        "Scte35ReturnToNetworkSettings": Scte35ReturnToNetworkScheduleActionSettingsTypeDef,
-        "Scte35SpliceInsertSettings": Scte35SpliceInsertScheduleActionSettingsTypeDef,
-        "Scte35TimeSignalSettings": Scte35TimeSignalScheduleActionSettingsOutputTypeDef,
-        "StaticImageActivateSettings": StaticImageActivateScheduleActionSettingsTypeDef,
-        "StaticImageDeactivateSettings": StaticImageDeactivateScheduleActionSettingsTypeDef,
-    },
-    total=False,
-)
-
 ScheduleActionSettingsTypeDef = TypedDict(
     "ScheduleActionSettingsTypeDef",
     {
         "HlsId3SegmentTaggingSettings": HlsId3SegmentTaggingScheduleActionSettingsTypeDef,
         "HlsTimedMetadataSettings": HlsTimedMetadataScheduleActionSettingsTypeDef,
         "InputPrepareSettings": InputPrepareScheduleActionSettingsTypeDef,
         "InputSwitchSettings": InputSwitchScheduleActionSettingsTypeDef,
@@ -5532,52 +4980,31 @@
 
 ChannelSummaryTypeDef = TypedDict(
     "ChannelSummaryTypeDef",
     {
         "Arn": str,
         "CdiInputSpecification": CdiInputSpecificationTypeDef,
         "ChannelClass": ChannelClassType,
-        "Destinations": List[OutputDestinationOutputTypeDef],
+        "Destinations": List[OutputDestinationTypeDef],
         "EgressEndpoints": List[ChannelEgressEndpointTypeDef],
         "Id": str,
-        "InputAttachments": List[InputAttachmentOutputTypeDef],
+        "InputAttachments": List[InputAttachmentTypeDef],
         "InputSpecification": InputSpecificationTypeDef,
         "LogLevel": LogLevelType,
         "Maintenance": MaintenanceStatusTypeDef,
         "Name": str,
         "PipelinesRunningCount": int,
         "RoleArn": str,
         "State": ChannelStateType,
         "Tags": Dict[str, str],
         "Vpc": VpcOutputSettingsDescriptionTypeDef,
     },
     total=False,
 )
 
-InputAttachmentUnionTypeDef = Union[InputAttachmentTypeDef, InputAttachmentOutputTypeDef]
-_RequiredOutputGroupOutputTypeDef = TypedDict(
-    "_RequiredOutputGroupOutputTypeDef",
-    {
-        "OutputGroupSettings": OutputGroupSettingsOutputTypeDef,
-        "Outputs": List[OutputTypeDef],
-    },
-)
-_OptionalOutputGroupOutputTypeDef = TypedDict(
-    "_OptionalOutputGroupOutputTypeDef",
-    {
-        "Name": str,
-    },
-    total=False,
-)
-
-class OutputGroupOutputTypeDef(
-    _RequiredOutputGroupOutputTypeDef, _OptionalOutputGroupOutputTypeDef
-):
-    pass
-
 _RequiredOutputGroupTypeDef = TypedDict(
     "_RequiredOutputGroupTypeDef",
     {
         "OutputGroupSettings": OutputGroupSettingsTypeDef,
         "Outputs": Sequence[OutputTypeDef],
     },
 )
@@ -5588,23 +5015,14 @@
     },
     total=False,
 )
 
 class OutputGroupTypeDef(_RequiredOutputGroupTypeDef, _OptionalOutputGroupTypeDef):
     pass
 
-ScheduleActionOutputTypeDef = TypedDict(
-    "ScheduleActionOutputTypeDef",
-    {
-        "ActionName": str,
-        "ScheduleActionSettings": ScheduleActionSettingsOutputTypeDef,
-        "ScheduleActionStartSettings": ScheduleActionStartSettingsOutputTypeDef,
-    },
-)
-
 ScheduleActionTypeDef = TypedDict(
     "ScheduleActionTypeDef",
     {
         "ActionName": str,
         "ScheduleActionSettings": ScheduleActionSettingsTypeDef,
         "ScheduleActionStartSettings": ScheduleActionStartSettingsTypeDef,
     },
@@ -5615,43 +5033,14 @@
     {
         "Channels": List[ChannelSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredEncoderSettingsOutputTypeDef = TypedDict(
-    "_RequiredEncoderSettingsOutputTypeDef",
-    {
-        "AudioDescriptions": List[AudioDescriptionOutputTypeDef],
-        "OutputGroups": List[OutputGroupOutputTypeDef],
-        "TimecodeConfig": TimecodeConfigTypeDef,
-        "VideoDescriptions": List[VideoDescriptionOutputTypeDef],
-    },
-)
-_OptionalEncoderSettingsOutputTypeDef = TypedDict(
-    "_OptionalEncoderSettingsOutputTypeDef",
-    {
-        "AvailBlanking": AvailBlankingTypeDef,
-        "AvailConfiguration": AvailConfigurationTypeDef,
-        "BlackoutSlate": BlackoutSlateTypeDef,
-        "CaptionDescriptions": List[CaptionDescriptionOutputTypeDef],
-        "FeatureActivations": FeatureActivationsTypeDef,
-        "GlobalConfiguration": GlobalConfigurationTypeDef,
-        "MotionGraphicsConfiguration": MotionGraphicsConfigurationOutputTypeDef,
-        "NielsenConfiguration": NielsenConfigurationTypeDef,
-    },
-    total=False,
-)
-
-class EncoderSettingsOutputTypeDef(
-    _RequiredEncoderSettingsOutputTypeDef, _OptionalEncoderSettingsOutputTypeDef
-):
-    pass
-
 _RequiredEncoderSettingsTypeDef = TypedDict(
     "_RequiredEncoderSettingsTypeDef",
     {
         "AudioDescriptions": Sequence[AudioDescriptionTypeDef],
         "OutputGroups": Sequence[OutputGroupTypeDef],
         "TimecodeConfig": TimecodeConfigTypeDef,
         "VideoDescriptions": Sequence[VideoDescriptionTypeDef],
@@ -5664,87 +5053,109 @@
         "AvailConfiguration": AvailConfigurationTypeDef,
         "BlackoutSlate": BlackoutSlateTypeDef,
         "CaptionDescriptions": Sequence[CaptionDescriptionTypeDef],
         "FeatureActivations": FeatureActivationsTypeDef,
         "GlobalConfiguration": GlobalConfigurationTypeDef,
         "MotionGraphicsConfiguration": MotionGraphicsConfigurationTypeDef,
         "NielsenConfiguration": NielsenConfigurationTypeDef,
+        "ThumbnailConfiguration": ThumbnailConfigurationTypeDef,
     },
     total=False,
 )
 
 class EncoderSettingsTypeDef(_RequiredEncoderSettingsTypeDef, _OptionalEncoderSettingsTypeDef):
     pass
 
+BatchScheduleActionCreateRequestTypeDef = TypedDict(
+    "BatchScheduleActionCreateRequestTypeDef",
+    {
+        "ScheduleActions": Sequence[ScheduleActionTypeDef],
+    },
+)
+
 BatchScheduleActionCreateResultTypeDef = TypedDict(
     "BatchScheduleActionCreateResultTypeDef",
     {
-        "ScheduleActions": List[ScheduleActionOutputTypeDef],
+        "ScheduleActions": List[ScheduleActionTypeDef],
     },
 )
 
 BatchScheduleActionDeleteResultTypeDef = TypedDict(
     "BatchScheduleActionDeleteResultTypeDef",
     {
-        "ScheduleActions": List[ScheduleActionOutputTypeDef],
+        "ScheduleActions": List[ScheduleActionTypeDef],
     },
 )
 
 DescribeScheduleResponseTypeDef = TypedDict(
     "DescribeScheduleResponseTypeDef",
     {
         "NextToken": str,
-        "ScheduleActions": List[ScheduleActionOutputTypeDef],
+        "ScheduleActions": List[ScheduleActionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchScheduleActionCreateRequestTypeDef = TypedDict(
-    "BatchScheduleActionCreateRequestTypeDef",
-    {
-        "ScheduleActions": Sequence[ScheduleActionTypeDef],
-    },
-)
-
 ChannelTypeDef = TypedDict(
     "ChannelTypeDef",
     {
         "Arn": str,
         "CdiInputSpecification": CdiInputSpecificationTypeDef,
         "ChannelClass": ChannelClassType,
-        "Destinations": List[OutputDestinationOutputTypeDef],
+        "Destinations": List[OutputDestinationTypeDef],
         "EgressEndpoints": List[ChannelEgressEndpointTypeDef],
-        "EncoderSettings": EncoderSettingsOutputTypeDef,
+        "EncoderSettings": EncoderSettingsTypeDef,
         "Id": str,
-        "InputAttachments": List[InputAttachmentOutputTypeDef],
+        "InputAttachments": List[InputAttachmentTypeDef],
         "InputSpecification": InputSpecificationTypeDef,
         "LogLevel": LogLevelType,
         "Maintenance": MaintenanceStatusTypeDef,
         "Name": str,
         "PipelineDetails": List[PipelineDetailTypeDef],
         "PipelinesRunningCount": int,
         "RoleArn": str,
         "State": ChannelStateType,
         "Tags": Dict[str, str],
         "Vpc": VpcOutputSettingsDescriptionTypeDef,
     },
     total=False,
 )
 
+CreateChannelRequestRequestTypeDef = TypedDict(
+    "CreateChannelRequestRequestTypeDef",
+    {
+        "CdiInputSpecification": CdiInputSpecificationTypeDef,
+        "ChannelClass": ChannelClassType,
+        "Destinations": Sequence[OutputDestinationTypeDef],
+        "EncoderSettings": EncoderSettingsTypeDef,
+        "InputAttachments": Sequence[InputAttachmentTypeDef],
+        "InputSpecification": InputSpecificationTypeDef,
+        "LogLevel": LogLevelType,
+        "Maintenance": MaintenanceCreateSettingsTypeDef,
+        "Name": str,
+        "RequestId": str,
+        "Reserved": str,
+        "RoleArn": str,
+        "Tags": Mapping[str, str],
+        "Vpc": VpcOutputSettingsTypeDef,
+    },
+    total=False,
+)
+
 DeleteChannelResponseTypeDef = TypedDict(
     "DeleteChannelResponseTypeDef",
     {
         "Arn": str,
         "CdiInputSpecification": CdiInputSpecificationTypeDef,
         "ChannelClass": ChannelClassType,
-        "Destinations": List[OutputDestinationOutputTypeDef],
+        "Destinations": List[OutputDestinationTypeDef],
         "EgressEndpoints": List[ChannelEgressEndpointTypeDef],
-        "EncoderSettings": EncoderSettingsOutputTypeDef,
+        "EncoderSettings": EncoderSettingsTypeDef,
         "Id": str,
-        "InputAttachments": List[InputAttachmentOutputTypeDef],
+        "InputAttachments": List[InputAttachmentTypeDef],
         "InputSpecification": InputSpecificationTypeDef,
         "LogLevel": LogLevelType,
         "Maintenance": MaintenanceStatusTypeDef,
         "Name": str,
         "PipelineDetails": List[PipelineDetailTypeDef],
         "PipelinesRunningCount": int,
         "RoleArn": str,
@@ -5757,19 +5168,19 @@
 
 DescribeChannelResponseTypeDef = TypedDict(
     "DescribeChannelResponseTypeDef",
     {
         "Arn": str,
         "CdiInputSpecification": CdiInputSpecificationTypeDef,
         "ChannelClass": ChannelClassType,
-        "Destinations": List[OutputDestinationOutputTypeDef],
+        "Destinations": List[OutputDestinationTypeDef],
         "EgressEndpoints": List[ChannelEgressEndpointTypeDef],
-        "EncoderSettings": EncoderSettingsOutputTypeDef,
+        "EncoderSettings": EncoderSettingsTypeDef,
         "Id": str,
-        "InputAttachments": List[InputAttachmentOutputTypeDef],
+        "InputAttachments": List[InputAttachmentTypeDef],
         "InputSpecification": InputSpecificationTypeDef,
         "LogLevel": LogLevelType,
         "Maintenance": MaintenanceStatusTypeDef,
         "Name": str,
         "PipelineDetails": List[PipelineDetailTypeDef],
         "PipelinesRunningCount": int,
         "RoleArn": str,
@@ -5782,19 +5193,19 @@
 
 StartChannelResponseTypeDef = TypedDict(
     "StartChannelResponseTypeDef",
     {
         "Arn": str,
         "CdiInputSpecification": CdiInputSpecificationTypeDef,
         "ChannelClass": ChannelClassType,
-        "Destinations": List[OutputDestinationOutputTypeDef],
+        "Destinations": List[OutputDestinationTypeDef],
         "EgressEndpoints": List[ChannelEgressEndpointTypeDef],
-        "EncoderSettings": EncoderSettingsOutputTypeDef,
+        "EncoderSettings": EncoderSettingsTypeDef,
         "Id": str,
-        "InputAttachments": List[InputAttachmentOutputTypeDef],
+        "InputAttachments": List[InputAttachmentTypeDef],
         "InputSpecification": InputSpecificationTypeDef,
         "LogLevel": LogLevelType,
         "Maintenance": MaintenanceStatusTypeDef,
         "Name": str,
         "PipelineDetails": List[PipelineDetailTypeDef],
         "PipelinesRunningCount": int,
         "RoleArn": str,
@@ -5807,91 +5218,60 @@
 
 StopChannelResponseTypeDef = TypedDict(
     "StopChannelResponseTypeDef",
     {
         "Arn": str,
         "CdiInputSpecification": CdiInputSpecificationTypeDef,
         "ChannelClass": ChannelClassType,
-        "Destinations": List[OutputDestinationOutputTypeDef],
+        "Destinations": List[OutputDestinationTypeDef],
         "EgressEndpoints": List[ChannelEgressEndpointTypeDef],
-        "EncoderSettings": EncoderSettingsOutputTypeDef,
+        "EncoderSettings": EncoderSettingsTypeDef,
         "Id": str,
-        "InputAttachments": List[InputAttachmentOutputTypeDef],
+        "InputAttachments": List[InputAttachmentTypeDef],
         "InputSpecification": InputSpecificationTypeDef,
         "LogLevel": LogLevelType,
         "Maintenance": MaintenanceStatusTypeDef,
         "Name": str,
         "PipelineDetails": List[PipelineDetailTypeDef],
         "PipelinesRunningCount": int,
         "RoleArn": str,
         "State": ChannelStateType,
         "Tags": Dict[str, str],
         "Vpc": VpcOutputSettingsDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateChannelRequestRequestTypeDef = TypedDict(
-    "CreateChannelRequestRequestTypeDef",
-    {
-        "CdiInputSpecification": CdiInputSpecificationTypeDef,
-        "ChannelClass": ChannelClassType,
-        "Destinations": Sequence[OutputDestinationUnionTypeDef],
-        "EncoderSettings": EncoderSettingsTypeDef,
-        "InputAttachments": Sequence[InputAttachmentUnionTypeDef],
-        "InputSpecification": InputSpecificationTypeDef,
-        "LogLevel": LogLevelType,
-        "Maintenance": MaintenanceCreateSettingsTypeDef,
-        "Name": str,
-        "RequestId": str,
-        "Reserved": str,
-        "RoleArn": str,
-        "Tags": Mapping[str, str],
-        "Vpc": VpcOutputSettingsTypeDef,
-    },
-    total=False,
-)
-
-EncoderSettingsUnionTypeDef = Union[EncoderSettingsTypeDef, EncoderSettingsOutputTypeDef]
 _RequiredUpdateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateChannelRequestRequestTypeDef",
     {
         "ChannelId": str,
     },
 )
 _OptionalUpdateChannelRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateChannelRequestRequestTypeDef",
     {
         "CdiInputSpecification": CdiInputSpecificationTypeDef,
-        "Destinations": Sequence[OutputDestinationUnionTypeDef],
+        "Destinations": Sequence[OutputDestinationTypeDef],
         "EncoderSettings": EncoderSettingsTypeDef,
-        "InputAttachments": Sequence[InputAttachmentUnionTypeDef],
+        "InputAttachments": Sequence[InputAttachmentTypeDef],
         "InputSpecification": InputSpecificationTypeDef,
         "LogLevel": LogLevelType,
         "Maintenance": MaintenanceUpdateSettingsTypeDef,
         "Name": str,
         "RoleArn": str,
     },
     total=False,
 )
 
 class UpdateChannelRequestRequestTypeDef(
     _RequiredUpdateChannelRequestRequestTypeDef, _OptionalUpdateChannelRequestRequestTypeDef
 ):
     pass
 
-BatchUpdateScheduleResponseTypeDef = TypedDict(
-    "BatchUpdateScheduleResponseTypeDef",
-    {
-        "Creates": BatchScheduleActionCreateResultTypeDef,
-        "Deletes": BatchScheduleActionDeleteResultTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredBatchUpdateScheduleRequestRequestTypeDef = TypedDict(
     "_RequiredBatchUpdateScheduleRequestRequestTypeDef",
     {
         "ChannelId": str,
     },
 )
 _OptionalBatchUpdateScheduleRequestRequestTypeDef = TypedDict(
@@ -5905,14 +5285,23 @@
 
 class BatchUpdateScheduleRequestRequestTypeDef(
     _RequiredBatchUpdateScheduleRequestRequestTypeDef,
     _OptionalBatchUpdateScheduleRequestRequestTypeDef,
 ):
     pass
 
+BatchUpdateScheduleResponseTypeDef = TypedDict(
+    "BatchUpdateScheduleResponseTypeDef",
+    {
+        "Creates": BatchScheduleActionCreateResultTypeDef,
+        "Deletes": BatchScheduleActionDeleteResultTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateChannelResponseTypeDef = TypedDict(
     "CreateChannelResponseTypeDef",
     {
         "Channel": ChannelTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-medialive-2.5.2.post1/types_aiobotocore_medialive/waiter.py` & `types-aiobotocore-medialive-2.5.2.post2/types_aiobotocore_medialive/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-medialive-2.5.2.post1/types_aiobotocore_medialive/waiter.pyi` & `types-aiobotocore-medialive-2.5.2.post2/types_aiobotocore_medialive/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-medialive-2.5.2.post1/types_aiobotocore_medialive.egg-info/SOURCES.txt` & `types-aiobotocore-medialive-2.5.2.post2/types_aiobotocore_medialive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

