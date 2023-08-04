# Comparing `tmp/types-aiobotocore-ssm-contacts-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-ssm-contacts-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-ssm-contacts-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:03 2023, max compression
+gzip compressed data, was "types-aiobotocore-ssm-contacts-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:27 2023, max compression
```

## Comparing `types-aiobotocore-ssm-contacts-2.5.2.post1.tar` & `types-aiobotocore-ssm-contacts-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:03.949449 types-aiobotocore-ssm-contacts-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:50:09.000000 types-aiobotocore-ssm-contacts-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19177 2023-08-02 14:53:03.945449 types-aiobotocore-ssm-contacts-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17640 2023-08-02 14:50:09.000000 types-aiobotocore-ssm-contacts-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:03.949449 types-aiobotocore-ssm-contacts-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-08-02 14:50:09.000000 types-aiobotocore-ssm-contacts-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:03.945449 types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts/
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-08-02 14:50:09.000000 types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-08-02 14:50:09.000000 types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-08-02 14:50:09.000000 types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34358 2023-08-02 14:50:09.000000 types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    34299 2023-08-02 14:50:09.000000 types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9739 2023-08-02 14:50:10.000000 types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9737 2023-08-02 14:50:10.000000 types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14402 2023-08-02 14:50:10.000000 types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    14389 2023-08-02 14:50:10.000000 types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:50:09.000000 types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    40767 2023-08-02 14:50:10.000000 types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    40690 2023-08-02 14:50:10.000000 types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:50:09.000000 types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:03.945449 types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19177 2023-08-02 14:53:03.000000 types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-02 14:53:03.000000 types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:03.000000 types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:03.000000 types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:03.000000 types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 14:53:03.000000 types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:27.476643 types-aiobotocore-ssm-contacts-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:54:18.000000 types-aiobotocore-ssm-contacts-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14792 2023-08-04 13:59:27.476643 types-aiobotocore-ssm-contacts-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13255 2023-08-04 13:54:18.000000 types-aiobotocore-ssm-contacts-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:27.476643 types-aiobotocore-ssm-contacts-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2106 2023-08-04 13:54:18.000000 types-aiobotocore-ssm-contacts-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:27.466643 types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2886 2023-08-04 13:54:18.000000 types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2885 2023-08-04 13:54:18.000000 types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      961 2023-08-04 13:54:18.000000 types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    34323 2023-08-04 13:54:19.000000 types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    34264 2023-08-04 13:54:19.000000 types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10176 2023-08-04 13:54:19.000000 types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10174 2023-08-04 13:54:19.000000 types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14392 2023-08-04 13:54:19.000000 types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14379 2023-08-04 13:54:19.000000 types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:54:18.000000 types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    39429 2023-08-04 13:54:20.000000 types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    39354 2023-08-04 13:54:20.000000 types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:54:18.000000 types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:27.466643 types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14792 2023-08-04 13:59:27.000000 types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      908 2023-08-04 13:59:27.000000 types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:27.000000 types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:27.000000 types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:27.000000 types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       31 2023-08-04 13:59:27.000000 types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-ssm-contacts-2.5.2.post1/LICENSE` & `types-aiobotocore-ssm-contacts-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-contacts-2.5.2.post1/setup.py` & `types-aiobotocore-ssm-contacts-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-ssm-contacts",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_ssm_contacts"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.SSMContacts 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts/__init__.py` & `types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts/__init__.pyi` & `types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts/__main__.py` & `types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SSMContacts 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.SSMContacts 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts\nOther"
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

### Comparing `types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts/client.py` & `types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,17 +55,17 @@
     ListPagesByContactResultTypeDef,
     ListPagesByEngagementResultTypeDef,
     ListPreviewRotationShiftsResultTypeDef,
     ListRotationOverridesResultTypeDef,
     ListRotationShiftsResultTypeDef,
     ListRotationsResultTypeDef,
     ListTagsForResourceResultTypeDef,
-    PlanUnionTypeDef,
+    PlanTypeDef,
     PreviewOverrideTypeDef,
-    RecurrenceSettingsUnionTypeDef,
+    RecurrenceSettingsTypeDef,
     StartEngagementResultTypeDef,
     TagTypeDef,
     TimeRangeTypeDef,
     TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -158,15 +158,15 @@
         """
 
     async def create_contact(
         self,
         *,
         Alias: str,
         Type: ContactTypeType,
-        Plan: PlanUnionTypeDef,
+        Plan: PlanTypeDef,
         DisplayName: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         IdempotencyToken: str = ...
     ) -> CreateContactResultTypeDef:
         """
         Contacts are either the contacts that Incident Manager engages during an
         incident or the escalation plans that Incident Manager uses to engage contacts
@@ -196,15 +196,15 @@
 
     async def create_rotation(
         self,
         *,
         Name: str,
         ContactIds: Sequence[str],
         TimeZoneId: str,
-        Recurrence: RecurrenceSettingsUnionTypeDef,
+        Recurrence: RecurrenceSettingsTypeDef,
         StartTime: TimestampTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         IdempotencyToken: str = ...
     ) -> CreateRotationResultTypeDef:
         """
         Creates a rotation in an on-call schedule.
 
@@ -428,15 +428,15 @@
 
     async def list_preview_rotation_shifts(
         self,
         *,
         EndTime: TimestampTypeDef,
         Members: Sequence[str],
         TimeZoneId: str,
-        Recurrence: RecurrenceSettingsUnionTypeDef,
+        Recurrence: RecurrenceSettingsTypeDef,
         RotationStartTime: TimestampTypeDef = ...,
         StartTime: TimestampTypeDef = ...,
         Overrides: Sequence[PreviewOverrideTypeDef] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListPreviewRotationShiftsResultTypeDef:
         """
@@ -553,15 +553,15 @@
         Removes tags from the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/client/#untag_resource)
         """
 
     async def update_contact(
-        self, *, ContactId: str, DisplayName: str = ..., Plan: PlanUnionTypeDef = ...
+        self, *, ContactId: str, DisplayName: str = ..., Plan: PlanTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates the contact or escalation plan specified.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.update_contact)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/client/#update_contact)
         """
@@ -580,15 +580,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/client/#update_contact_channel)
         """
 
     async def update_rotation(
         self,
         *,
         RotationId: str,
-        Recurrence: RecurrenceSettingsUnionTypeDef,
+        Recurrence: RecurrenceSettingsTypeDef,
         ContactIds: Sequence[str] = ...,
         StartTime: TimestampTypeDef = ...,
         TimeZoneId: str = ...
     ) -> Dict[str, Any]:
         """
         Updates the information specified for an on-call rotation.
```

### Comparing `types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts/client.pyi` & `types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -55,17 +55,17 @@
     ListPagesByContactResultTypeDef,
     ListPagesByEngagementResultTypeDef,
     ListPreviewRotationShiftsResultTypeDef,
     ListRotationOverridesResultTypeDef,
     ListRotationShiftsResultTypeDef,
     ListRotationsResultTypeDef,
     ListTagsForResourceResultTypeDef,
-    PlanUnionTypeDef,
+    PlanTypeDef,
     PreviewOverrideTypeDef,
-    RecurrenceSettingsUnionTypeDef,
+    RecurrenceSettingsTypeDef,
     StartEngagementResultTypeDef,
     TagTypeDef,
     TimeRangeTypeDef,
     TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -149,15 +149,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/client/#close)
         """
     async def create_contact(
         self,
         *,
         Alias: str,
         Type: ContactTypeType,
-        Plan: PlanUnionTypeDef,
+        Plan: PlanTypeDef,
         DisplayName: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         IdempotencyToken: str = ...
     ) -> CreateContactResultTypeDef:
         """
         Contacts are either the contacts that Incident Manager engages during an
         incident or the escalation plans that Incident Manager uses to engage contacts
@@ -185,15 +185,15 @@
         """
     async def create_rotation(
         self,
         *,
         Name: str,
         ContactIds: Sequence[str],
         TimeZoneId: str,
-        Recurrence: RecurrenceSettingsUnionTypeDef,
+        Recurrence: RecurrenceSettingsTypeDef,
         StartTime: TimestampTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         IdempotencyToken: str = ...
     ) -> CreateRotationResultTypeDef:
         """
         Creates a rotation in an on-call schedule.
 
@@ -395,15 +395,15 @@
         """
     async def list_preview_rotation_shifts(
         self,
         *,
         EndTime: TimestampTypeDef,
         Members: Sequence[str],
         TimeZoneId: str,
-        Recurrence: RecurrenceSettingsUnionTypeDef,
+        Recurrence: RecurrenceSettingsTypeDef,
         RotationStartTime: TimestampTypeDef = ...,
         StartTime: TimestampTypeDef = ...,
         Overrides: Sequence[PreviewOverrideTypeDef] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListPreviewRotationShiftsResultTypeDef:
         """
@@ -509,15 +509,15 @@
         """
         Removes tags from the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/client/#untag_resource)
         """
     async def update_contact(
-        self, *, ContactId: str, DisplayName: str = ..., Plan: PlanUnionTypeDef = ...
+        self, *, ContactId: str, DisplayName: str = ..., Plan: PlanTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates the contact or escalation plan specified.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.update_contact)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/client/#update_contact)
         """
@@ -534,15 +534,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.update_contact_channel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/client/#update_contact_channel)
         """
     async def update_rotation(
         self,
         *,
         RotationId: str,
-        Recurrence: RecurrenceSettingsUnionTypeDef,
+        Recurrence: RecurrenceSettingsTypeDef,
         ContactIds: Sequence[str] = ...,
         StartTime: TimestampTypeDef = ...,
         TimeZoneId: str = ...
     ) -> Dict[str, Any]:
         """
         Updates the information specified for an on-call rotation.
```

### Comparing `types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts/literals.py` & `types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts/literals.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     "ListRotationsPaginatorName",
     "ReceiptTypeType",
     "ShiftTypeType",
     "SSMContactsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
+    "RegionName",
 )
 
 
 AcceptCodeValidationType = Literal["ENFORCE", "IGNORE"]
 AcceptTypeType = Literal["DELIVERED", "READ"]
 ActivationStatusType = Literal["ACTIVATED", "NOT_ACTIVATED"]
 ChannelTypeType = Literal["EMAIL", "SMS", "VOICE"]
@@ -77,14 +78,15 @@
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
@@ -180,14 +182,15 @@
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
@@ -266,26 +269,28 @@
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
@@ -438,7 +443,25 @@
     "list_pages_by_contact",
     "list_pages_by_engagement",
     "list_preview_rotation_shifts",
     "list_rotation_overrides",
     "list_rotation_shifts",
     "list_rotations",
 ]
+RegionName = Literal[
+    "ap-northeast-1",
+    "ap-northeast-2",
+    "ap-south-1",
+    "ap-southeast-1",
+    "ap-southeast-2",
+    "ca-central-1",
+    "eu-central-1",
+    "eu-north-1",
+    "eu-west-1",
+    "eu-west-2",
+    "eu-west-3",
+    "sa-east-1",
+    "us-east-1",
+    "us-east-2",
+    "us-west-1",
+    "us-west-2",
+]
```

### Comparing `types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts/literals.pyi` & `types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     "ListRotationsPaginatorName",
     "ReceiptTypeType",
     "ShiftTypeType",
     "SSMContactsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
+    "RegionName",
 )
 
 AcceptCodeValidationType = Literal["ENFORCE", "IGNORE"]
 AcceptTypeType = Literal["DELIVERED", "READ"]
 ActivationStatusType = Literal["ACTIVATED", "NOT_ACTIVATED"]
 ChannelTypeType = Literal["EMAIL", "SMS", "VOICE"]
 ContactTypeType = Literal["ESCALATION", "ONCALL_SCHEDULE", "PERSONAL"]
@@ -75,14 +76,15 @@
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
@@ -178,14 +180,15 @@
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
@@ -264,26 +267,28 @@
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
@@ -436,7 +441,25 @@
     "list_pages_by_contact",
     "list_pages_by_engagement",
     "list_preview_rotation_shifts",
     "list_rotation_overrides",
     "list_rotation_shifts",
     "list_rotations",
 ]
+RegionName = Literal[
+    "ap-northeast-1",
+    "ap-northeast-2",
+    "ap-south-1",
+    "ap-southeast-1",
+    "ap-southeast-2",
+    "ca-central-1",
+    "eu-central-1",
+    "eu-north-1",
+    "eu-west-1",
+    "eu-west-2",
+    "eu-west-3",
+    "sa-east-1",
+    "us-east-1",
+    "us-east-2",
+    "us-west-1",
+    "us-west-2",
+]
```

### Comparing `types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts/paginator.py` & `types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     ListPagesByEngagementResultTypeDef,
     ListPreviewRotationShiftsResultTypeDef,
     ListRotationOverridesResultTypeDef,
     ListRotationShiftsResultTypeDef,
     ListRotationsResultTypeDef,
     PaginatorConfigTypeDef,
     PreviewOverrideTypeDef,
-    RecurrenceSettingsUnionTypeDef,
+    RecurrenceSettingsTypeDef,
     TimeRangeTypeDef,
     TimestampTypeDef,
 )
 
 __all__ = (
     "ListContactChannelsPaginator",
     "ListContactsPaginator",
@@ -211,15 +211,15 @@
 
     def paginate(
         self,
         *,
         EndTime: TimestampTypeDef,
         Members: Sequence[str],
         TimeZoneId: str,
-        Recurrence: RecurrenceSettingsUnionTypeDef,
+        Recurrence: RecurrenceSettingsTypeDef,
         RotationStartTime: TimestampTypeDef = ...,
         StartTime: TimestampTypeDef = ...,
         Overrides: Sequence[PreviewOverrideTypeDef] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPreviewRotationShiftsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPreviewRotationShifts.paginate)
```

### Comparing `types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts/paginator.pyi` & `types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     ListPagesByEngagementResultTypeDef,
     ListPreviewRotationShiftsResultTypeDef,
     ListRotationOverridesResultTypeDef,
     ListRotationShiftsResultTypeDef,
     ListRotationsResultTypeDef,
     PaginatorConfigTypeDef,
     PreviewOverrideTypeDef,
-    RecurrenceSettingsUnionTypeDef,
+    RecurrenceSettingsTypeDef,
     TimeRangeTypeDef,
     TimestampTypeDef,
 )
 
 __all__ = (
     "ListContactChannelsPaginator",
     "ListContactsPaginator",
@@ -201,15 +201,15 @@
 
     def paginate(
         self,
         *,
         EndTime: TimestampTypeDef,
         Members: Sequence[str],
         TimeZoneId: str,
-        Recurrence: RecurrenceSettingsUnionTypeDef,
+        Recurrence: RecurrenceSettingsTypeDef,
         RotationStartTime: TimestampTypeDef = ...,
         StartTime: TimestampTypeDef = ...,
         Overrides: Sequence[PreviewOverrideTypeDef] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPreviewRotationShiftsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPreviewRotationShifts.paginate)
```

### Comparing `types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts/type_defs.py` & `types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,34 +113,29 @@
     "ListPageReceiptsResultTypeDef",
     "ListPageResolutionsResultTypeDef",
     "ListPagesByContactResultTypeDef",
     "ListPagesByEngagementResultTypeDef",
     "ListRotationOverridesResultTypeDef",
     "RotationShiftTypeDef",
     "ListContactChannelsResultTypeDef",
-    "StageOutputTypeDef",
     "StageTypeDef",
-    "RecurrenceSettingsOutputTypeDef",
     "RecurrenceSettingsTypeDef",
     "ListEngagementsRequestListEngagementsPaginateTypeDef",
     "ListEngagementsRequestRequestTypeDef",
     "ListPreviewRotationShiftsResultTypeDef",
     "ListRotationShiftsResultTypeDef",
-    "PlanOutputTypeDef",
     "PlanTypeDef",
-    "GetRotationResultTypeDef",
-    "RotationTypeDef",
     "CreateRotationRequestRequestTypeDef",
+    "GetRotationResultTypeDef",
     "ListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef",
     "ListPreviewRotationShiftsRequestRequestTypeDef",
-    "RecurrenceSettingsUnionTypeDef",
+    "RotationTypeDef",
     "UpdateRotationRequestRequestTypeDef",
-    "GetContactResultTypeDef",
     "CreateContactRequestRequestTypeDef",
-    "PlanUnionTypeDef",
+    "GetContactResultTypeDef",
     "UpdateContactRequestRequestTypeDef",
     "ListRotationsResultTypeDef",
 )
 
 _RequiredAcceptPageRequestRequestTypeDef = TypedDict(
     "_RequiredAcceptPageRequestRequestTypeDef",
     {
@@ -1285,55 +1280,22 @@
     {
         "NextToken": str,
         "ContactChannels": List[ContactChannelTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StageOutputTypeDef = TypedDict(
-    "StageOutputTypeDef",
-    {
-        "DurationInMinutes": int,
-        "Targets": List[TargetTypeDef],
-    },
-)
-
 StageTypeDef = TypedDict(
     "StageTypeDef",
     {
         "DurationInMinutes": int,
         "Targets": Sequence[TargetTypeDef],
     },
 )
 
-_RequiredRecurrenceSettingsOutputTypeDef = TypedDict(
-    "_RequiredRecurrenceSettingsOutputTypeDef",
-    {
-        "NumberOfOnCalls": int,
-        "RecurrenceMultiplier": int,
-    },
-)
-_OptionalRecurrenceSettingsOutputTypeDef = TypedDict(
-    "_OptionalRecurrenceSettingsOutputTypeDef",
-    {
-        "MonthlySettings": List[MonthlySettingTypeDef],
-        "WeeklySettings": List[WeeklySettingTypeDef],
-        "DailySettings": List[HandOffTimeTypeDef],
-        "ShiftCoverages": Dict[DayOfWeekType, List[CoverageTimeTypeDef]],
-    },
-    total=False,
-)
-
-
-class RecurrenceSettingsOutputTypeDef(
-    _RequiredRecurrenceSettingsOutputTypeDef, _OptionalRecurrenceSettingsOutputTypeDef
-):
-    pass
-
-
 _RequiredRecurrenceSettingsTypeDef = TypedDict(
     "_RequiredRecurrenceSettingsTypeDef",
     {
         "NumberOfOnCalls": int,
         "RecurrenceMultiplier": int,
     },
 )
@@ -1390,68 +1352,23 @@
     {
         "RotationShifts": List[RotationShiftTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PlanOutputTypeDef = TypedDict(
-    "PlanOutputTypeDef",
-    {
-        "Stages": List[StageOutputTypeDef],
-        "RotationIds": List[str],
-    },
-    total=False,
-)
-
 PlanTypeDef = TypedDict(
     "PlanTypeDef",
     {
         "Stages": Sequence[StageTypeDef],
         "RotationIds": Sequence[str],
     },
     total=False,
 )
 
-GetRotationResultTypeDef = TypedDict(
-    "GetRotationResultTypeDef",
-    {
-        "RotationArn": str,
-        "Name": str,
-        "ContactIds": List[str],
-        "StartTime": datetime,
-        "TimeZoneId": str,
-        "Recurrence": RecurrenceSettingsOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredRotationTypeDef = TypedDict(
-    "_RequiredRotationTypeDef",
-    {
-        "RotationArn": str,
-        "Name": str,
-    },
-)
-_OptionalRotationTypeDef = TypedDict(
-    "_OptionalRotationTypeDef",
-    {
-        "ContactIds": List[str],
-        "StartTime": datetime,
-        "TimeZoneId": str,
-        "Recurrence": RecurrenceSettingsOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class RotationTypeDef(_RequiredRotationTypeDef, _OptionalRotationTypeDef):
-    pass
-
-
 _RequiredCreateRotationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRotationRequestRequestTypeDef",
     {
         "Name": str,
         "ContactIds": Sequence[str],
         "TimeZoneId": str,
         "Recurrence": RecurrenceSettingsTypeDef,
@@ -1470,14 +1387,27 @@
 
 class CreateRotationRequestRequestTypeDef(
     _RequiredCreateRotationRequestRequestTypeDef, _OptionalCreateRotationRequestRequestTypeDef
 ):
     pass
 
 
+GetRotationResultTypeDef = TypedDict(
+    "GetRotationResultTypeDef",
+    {
+        "RotationArn": str,
+        "Name": str,
+        "ContactIds": List[str],
+        "StartTime": datetime,
+        "TimeZoneId": str,
+        "Recurrence": RecurrenceSettingsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef = TypedDict(
     "_RequiredListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef",
     {
         "EndTime": TimestampTypeDef,
         "Members": Sequence[str],
         "TimeZoneId": str,
         "Recurrence": RecurrenceSettingsTypeDef,
@@ -1527,15 +1457,37 @@
 class ListPreviewRotationShiftsRequestRequestTypeDef(
     _RequiredListPreviewRotationShiftsRequestRequestTypeDef,
     _OptionalListPreviewRotationShiftsRequestRequestTypeDef,
 ):
     pass
 
 
-RecurrenceSettingsUnionTypeDef = Union[RecurrenceSettingsTypeDef, RecurrenceSettingsOutputTypeDef]
+_RequiredRotationTypeDef = TypedDict(
+    "_RequiredRotationTypeDef",
+    {
+        "RotationArn": str,
+        "Name": str,
+    },
+)
+_OptionalRotationTypeDef = TypedDict(
+    "_OptionalRotationTypeDef",
+    {
+        "ContactIds": List[str],
+        "StartTime": datetime,
+        "TimeZoneId": str,
+        "Recurrence": RecurrenceSettingsTypeDef,
+    },
+    total=False,
+)
+
+
+class RotationTypeDef(_RequiredRotationTypeDef, _OptionalRotationTypeDef):
+    pass
+
+
 _RequiredUpdateRotationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRotationRequestRequestTypeDef",
     {
         "RotationId": str,
         "Recurrence": RecurrenceSettingsTypeDef,
     },
 )
@@ -1552,26 +1504,14 @@
 
 class UpdateRotationRequestRequestTypeDef(
     _RequiredUpdateRotationRequestRequestTypeDef, _OptionalUpdateRotationRequestRequestTypeDef
 ):
     pass
 
 
-GetContactResultTypeDef = TypedDict(
-    "GetContactResultTypeDef",
-    {
-        "ContactArn": str,
-        "Alias": str,
-        "DisplayName": str,
-        "Type": ContactTypeType,
-        "Plan": PlanOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateContactRequestRequestTypeDef = TypedDict(
     "_RequiredCreateContactRequestRequestTypeDef",
     {
         "Alias": str,
         "Type": ContactTypeType,
         "Plan": PlanTypeDef,
     },
@@ -1589,15 +1529,26 @@
 
 class CreateContactRequestRequestTypeDef(
     _RequiredCreateContactRequestRequestTypeDef, _OptionalCreateContactRequestRequestTypeDef
 ):
     pass
 
 
-PlanUnionTypeDef = Union[PlanTypeDef, PlanOutputTypeDef]
+GetContactResultTypeDef = TypedDict(
+    "GetContactResultTypeDef",
+    {
+        "ContactArn": str,
+        "Alias": str,
+        "DisplayName": str,
+        "Type": ContactTypeType,
+        "Plan": PlanTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateContactRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateContactRequestRequestTypeDef",
     {
         "ContactId": str,
     },
 )
 _OptionalUpdateContactRequestRequestTypeDef = TypedDict(
```

### Comparing `types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts/type_defs.pyi` & `types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts/type_defs.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -112,34 +112,29 @@
     "ListPageReceiptsResultTypeDef",
     "ListPageResolutionsResultTypeDef",
     "ListPagesByContactResultTypeDef",
     "ListPagesByEngagementResultTypeDef",
     "ListRotationOverridesResultTypeDef",
     "RotationShiftTypeDef",
     "ListContactChannelsResultTypeDef",
-    "StageOutputTypeDef",
     "StageTypeDef",
-    "RecurrenceSettingsOutputTypeDef",
     "RecurrenceSettingsTypeDef",
     "ListEngagementsRequestListEngagementsPaginateTypeDef",
     "ListEngagementsRequestRequestTypeDef",
     "ListPreviewRotationShiftsResultTypeDef",
     "ListRotationShiftsResultTypeDef",
-    "PlanOutputTypeDef",
     "PlanTypeDef",
-    "GetRotationResultTypeDef",
-    "RotationTypeDef",
     "CreateRotationRequestRequestTypeDef",
+    "GetRotationResultTypeDef",
     "ListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef",
     "ListPreviewRotationShiftsRequestRequestTypeDef",
-    "RecurrenceSettingsUnionTypeDef",
+    "RotationTypeDef",
     "UpdateRotationRequestRequestTypeDef",
-    "GetContactResultTypeDef",
     "CreateContactRequestRequestTypeDef",
-    "PlanUnionTypeDef",
+    "GetContactResultTypeDef",
     "UpdateContactRequestRequestTypeDef",
     "ListRotationsResultTypeDef",
 )
 
 _RequiredAcceptPageRequestRequestTypeDef = TypedDict(
     "_RequiredAcceptPageRequestRequestTypeDef",
     {
@@ -1226,53 +1221,22 @@
     {
         "NextToken": str,
         "ContactChannels": List[ContactChannelTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StageOutputTypeDef = TypedDict(
-    "StageOutputTypeDef",
-    {
-        "DurationInMinutes": int,
-        "Targets": List[TargetTypeDef],
-    },
-)
-
 StageTypeDef = TypedDict(
     "StageTypeDef",
     {
         "DurationInMinutes": int,
         "Targets": Sequence[TargetTypeDef],
     },
 )
 
-_RequiredRecurrenceSettingsOutputTypeDef = TypedDict(
-    "_RequiredRecurrenceSettingsOutputTypeDef",
-    {
-        "NumberOfOnCalls": int,
-        "RecurrenceMultiplier": int,
-    },
-)
-_OptionalRecurrenceSettingsOutputTypeDef = TypedDict(
-    "_OptionalRecurrenceSettingsOutputTypeDef",
-    {
-        "MonthlySettings": List[MonthlySettingTypeDef],
-        "WeeklySettings": List[WeeklySettingTypeDef],
-        "DailySettings": List[HandOffTimeTypeDef],
-        "ShiftCoverages": Dict[DayOfWeekType, List[CoverageTimeTypeDef]],
-    },
-    total=False,
-)
-
-class RecurrenceSettingsOutputTypeDef(
-    _RequiredRecurrenceSettingsOutputTypeDef, _OptionalRecurrenceSettingsOutputTypeDef
-):
-    pass
-
 _RequiredRecurrenceSettingsTypeDef = TypedDict(
     "_RequiredRecurrenceSettingsTypeDef",
     {
         "NumberOfOnCalls": int,
         "RecurrenceMultiplier": int,
     },
 )
@@ -1327,66 +1291,23 @@
     {
         "RotationShifts": List[RotationShiftTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PlanOutputTypeDef = TypedDict(
-    "PlanOutputTypeDef",
-    {
-        "Stages": List[StageOutputTypeDef],
-        "RotationIds": List[str],
-    },
-    total=False,
-)
-
 PlanTypeDef = TypedDict(
     "PlanTypeDef",
     {
         "Stages": Sequence[StageTypeDef],
         "RotationIds": Sequence[str],
     },
     total=False,
 )
 
-GetRotationResultTypeDef = TypedDict(
-    "GetRotationResultTypeDef",
-    {
-        "RotationArn": str,
-        "Name": str,
-        "ContactIds": List[str],
-        "StartTime": datetime,
-        "TimeZoneId": str,
-        "Recurrence": RecurrenceSettingsOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredRotationTypeDef = TypedDict(
-    "_RequiredRotationTypeDef",
-    {
-        "RotationArn": str,
-        "Name": str,
-    },
-)
-_OptionalRotationTypeDef = TypedDict(
-    "_OptionalRotationTypeDef",
-    {
-        "ContactIds": List[str],
-        "StartTime": datetime,
-        "TimeZoneId": str,
-        "Recurrence": RecurrenceSettingsOutputTypeDef,
-    },
-    total=False,
-)
-
-class RotationTypeDef(_RequiredRotationTypeDef, _OptionalRotationTypeDef):
-    pass
-
 _RequiredCreateRotationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRotationRequestRequestTypeDef",
     {
         "Name": str,
         "ContactIds": Sequence[str],
         "TimeZoneId": str,
         "Recurrence": RecurrenceSettingsTypeDef,
@@ -1403,14 +1324,27 @@
 )
 
 class CreateRotationRequestRequestTypeDef(
     _RequiredCreateRotationRequestRequestTypeDef, _OptionalCreateRotationRequestRequestTypeDef
 ):
     pass
 
+GetRotationResultTypeDef = TypedDict(
+    "GetRotationResultTypeDef",
+    {
+        "RotationArn": str,
+        "Name": str,
+        "ContactIds": List[str],
+        "StartTime": datetime,
+        "TimeZoneId": str,
+        "Recurrence": RecurrenceSettingsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef = TypedDict(
     "_RequiredListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef",
     {
         "EndTime": TimestampTypeDef,
         "Members": Sequence[str],
         "TimeZoneId": str,
         "Recurrence": RecurrenceSettingsTypeDef,
@@ -1456,15 +1390,35 @@
 
 class ListPreviewRotationShiftsRequestRequestTypeDef(
     _RequiredListPreviewRotationShiftsRequestRequestTypeDef,
     _OptionalListPreviewRotationShiftsRequestRequestTypeDef,
 ):
     pass
 
-RecurrenceSettingsUnionTypeDef = Union[RecurrenceSettingsTypeDef, RecurrenceSettingsOutputTypeDef]
+_RequiredRotationTypeDef = TypedDict(
+    "_RequiredRotationTypeDef",
+    {
+        "RotationArn": str,
+        "Name": str,
+    },
+)
+_OptionalRotationTypeDef = TypedDict(
+    "_OptionalRotationTypeDef",
+    {
+        "ContactIds": List[str],
+        "StartTime": datetime,
+        "TimeZoneId": str,
+        "Recurrence": RecurrenceSettingsTypeDef,
+    },
+    total=False,
+)
+
+class RotationTypeDef(_RequiredRotationTypeDef, _OptionalRotationTypeDef):
+    pass
+
 _RequiredUpdateRotationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRotationRequestRequestTypeDef",
     {
         "RotationId": str,
         "Recurrence": RecurrenceSettingsTypeDef,
     },
 )
@@ -1479,26 +1433,14 @@
 )
 
 class UpdateRotationRequestRequestTypeDef(
     _RequiredUpdateRotationRequestRequestTypeDef, _OptionalUpdateRotationRequestRequestTypeDef
 ):
     pass
 
-GetContactResultTypeDef = TypedDict(
-    "GetContactResultTypeDef",
-    {
-        "ContactArn": str,
-        "Alias": str,
-        "DisplayName": str,
-        "Type": ContactTypeType,
-        "Plan": PlanOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateContactRequestRequestTypeDef = TypedDict(
     "_RequiredCreateContactRequestRequestTypeDef",
     {
         "Alias": str,
         "Type": ContactTypeType,
         "Plan": PlanTypeDef,
     },
@@ -1514,15 +1456,26 @@
 )
 
 class CreateContactRequestRequestTypeDef(
     _RequiredCreateContactRequestRequestTypeDef, _OptionalCreateContactRequestRequestTypeDef
 ):
     pass
 
-PlanUnionTypeDef = Union[PlanTypeDef, PlanOutputTypeDef]
+GetContactResultTypeDef = TypedDict(
+    "GetContactResultTypeDef",
+    {
+        "ContactArn": str,
+        "Alias": str,
+        "DisplayName": str,
+        "Type": ContactTypeType,
+        "Plan": PlanTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateContactRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateContactRequestRequestTypeDef",
     {
         "ContactId": str,
     },
 )
 _OptionalUpdateContactRequestRequestTypeDef = TypedDict(
```

### Comparing `types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts.egg-info/SOURCES.txt` & `types-aiobotocore-ssm-contacts-2.5.2.post2/types_aiobotocore_ssm_contacts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

