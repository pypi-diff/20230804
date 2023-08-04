# Comparing `tmp/key_switcheroo-0.0.9.tar.gz` & `tmp/key_switcheroo-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "key_switcheroo-0.0.9.tar", max compression
+gzip compressed data, was "key_switcheroo-1.0.0.tar", max compression
```

## Comparing `key_switcheroo-0.0.9.tar` & `key_switcheroo-1.0.0.tar`

### file list

```diff
@@ -1,25 +1,38 @@
--rw-r--r--   0        0        0     5060 2023-07-12 22:26:14.720254 key_switcheroo-0.0.9/README.md
--rw-r--r--   0        0        0      802 2023-07-13 17:18:04.957594 key_switcheroo-0.0.9/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-12 22:26:14.720254 key_switcheroo-0.0.9/switcheroo/__init__.py
--rw-r--r--   0        0        0      135 2023-07-12 22:26:14.720254 key_switcheroo-0.0.9/switcheroo/base/__init__.py
--rw-r--r--   0        0        0     3654 2023-07-12 22:26:14.720254 key_switcheroo-0.0.9/switcheroo/base/data_store/__init__.py
--rw-r--r--   0        0        0     1909 2023-07-12 22:26:14.720254 key_switcheroo-0.0.9/switcheroo/base/data_store/s3.py
--rw-r--r--   0        0        0       92 2023-07-12 22:26:14.720254 key_switcheroo-0.0.9/switcheroo/base/data_store/util.py
--rw-r--r--   0        0        0      356 2023-07-12 22:26:14.720254 key_switcheroo-0.0.9/switcheroo/base/exceptions/s3.py
--rw-r--r--   0        0        0      287 2023-07-12 22:26:14.720254 key_switcheroo-0.0.9/switcheroo/base/serializer.py
--rw-r--r--   0        0        0     1774 2023-07-12 22:26:14.720254 key_switcheroo-0.0.9/switcheroo/paths.py
--rw-r--r--   0        0        0      205 2023-07-12 22:26:14.720254 key_switcheroo-0.0.9/switcheroo/ssh/__init__.py
--rw-r--r--   0        0        0        0 2023-07-12 22:26:14.720254 key_switcheroo-0.0.9/switcheroo/ssh/data_org/__init__.py
--rw-r--r--   0        0        0     1968 2023-07-12 22:26:14.720254 key_switcheroo-0.0.9/switcheroo/ssh/data_org/publisher/__init__.py
--rw-r--r--   0        0        0     1296 2023-07-12 22:26:14.720254 key_switcheroo-0.0.9/switcheroo/ssh/data_org/publisher/s3.py
--rw-r--r--   0        0        0     2957 2023-07-12 22:26:14.720254 key_switcheroo-0.0.9/switcheroo/ssh/data_org/retriever/__init__.py
--rw-r--r--   0        0        0     1809 2023-07-12 22:26:14.720254 key_switcheroo-0.0.9/switcheroo/ssh/data_org/retriever/s3.py
--rw-r--r--   0        0        0      931 2023-07-12 22:26:14.720254 key_switcheroo-0.0.9/switcheroo/ssh/data_stores/__init__.py
--rw-r--r--   0        0        0      834 2023-07-12 22:26:14.720254 key_switcheroo-0.0.9/switcheroo/ssh/exceptions.py
--rw-r--r--   0        0        0      183 2023-07-12 22:26:14.720254 key_switcheroo-0.0.9/switcheroo/ssh/objects/__init__.py
--rw-r--r--   0        0        0     4638 2023-07-12 22:26:14.720254 key_switcheroo-0.0.9/switcheroo/ssh/objects/key.py
--rw-r--r--   0        0        0        0 2023-07-12 22:26:14.720254 key_switcheroo-0.0.9/switcheroo/ssh/scripts/__init__.py
--rw-r--r--   0        0        0     1966 2023-07-12 22:26:14.720254 key_switcheroo-0.0.9/switcheroo/ssh/scripts/publish.py
--rwxr-xr-x   0        0        0     2002 2023-07-12 22:26:14.720254 key_switcheroo-0.0.9/switcheroo/ssh/scripts/retrieve.py
--rw-r--r--   0        0        0     2997 2023-07-12 22:26:14.720254 key_switcheroo-0.0.9/switcheroo/util.py
--rw-r--r--   0        0        0     5548 1970-01-01 00:00:00.000000 key_switcheroo-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0     8011 2023-08-02 17:20:58.786236 key_switcheroo-1.0.0/README.md
+-rw-r--r--   0        0        0     7773 2023-07-28 19:01:01.542520 key_switcheroo-1.0.0/aws_profiles/__init__.py
+-rw-r--r--   0        0        0      704 2023-07-28 19:01:01.542520 key_switcheroo-1.0.0/aws_profiles/exceptions.py
+-rw-r--r--   0        0        0      157 2023-07-28 19:01:01.542520 key_switcheroo-1.0.0/aws_profiles/profile.py
+-rw-r--r--   0        0        0     2878 2023-07-28 17:54:52.118328 key_switcheroo-1.0.0/metric_system/AWSPublisher.md
+-rw-r--r--   0        0        0        0 2023-07-28 17:54:52.118328 key_switcheroo-1.0.0/metric_system/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-28 17:54:52.118328 key_switcheroo-1.0.0/metric_system/functions/__init__.py
+-rw-r--r--   0        0        0     2555 2023-07-28 19:01:01.542520 key_switcheroo-1.0.0/metric_system/functions/aws_metric_publisher.py
+-rw-r--r--   0        0        0      379 2023-07-28 17:54:52.118328 key_switcheroo-1.0.0/metric_system/functions/exceptions.py
+-rw-r--r--   0        0        0     1897 2023-07-28 19:01:01.542520 key_switcheroo-1.0.0/metric_system/functions/file_metric_publisher.py
+-rw-r--r--   0        0        0     3150 2023-07-28 19:01:01.542520 key_switcheroo-1.0.0/metric_system/functions/metric.py
+-rw-r--r--   0        0        0      304 2023-07-28 17:54:52.118328 key_switcheroo-1.0.0/metric_system/functions/metric_publisher.py
+-rw-r--r--   0        0        0      831 2023-07-28 17:54:52.118328 key_switcheroo-1.0.0/metric_system/functions/metrics.py
+-rw-r--r--   0        0        0      996 2023-07-28 20:01:39.573330 key_switcheroo-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-28 17:54:52.118328 key_switcheroo-1.0.0/switcheroo/__init__.py
+-rw-r--r--   0        0        0      135 2023-08-03 17:05:55.859365 key_switcheroo-1.0.0/switcheroo/base/__init__.py
+-rw-r--r--   0        0        0     6428 2023-07-28 19:01:01.542520 key_switcheroo-1.0.0/switcheroo/base/data_store/__init__.py
+-rw-r--r--   0        0        0      292 2023-07-28 19:01:01.542520 key_switcheroo-1.0.0/switcheroo/base/data_store/exceptions.py
+-rw-r--r--   0        0        0     3028 2023-07-28 19:01:01.542520 key_switcheroo-1.0.0/switcheroo/base/data_store/s3.py
+-rw-r--r--   0        0        0      467 2023-07-28 19:01:01.542520 key_switcheroo-1.0.0/switcheroo/base/exceptions/s3.py
+-rw-r--r--   0        0        0     3243 2023-08-03 17:05:55.859365 key_switcheroo-1.0.0/switcheroo/base/scripts/configure.py
+-rw-r--r--   0        0        0      809 2023-07-28 19:01:01.542520 key_switcheroo-1.0.0/switcheroo/base/serializer.py
+-rw-r--r--   0        0        0     2078 2023-08-03 17:05:55.859365 key_switcheroo-1.0.0/switcheroo/paths.py
+-rw-r--r--   0        0        0      561 2023-07-28 19:01:01.542520 key_switcheroo-1.0.0/switcheroo/ssh/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-28 17:54:52.118328 key_switcheroo-1.0.0/switcheroo/ssh/data_org/__init__.py
+-rw-r--r--   0        0        0     4415 2023-07-28 19:01:01.542520 key_switcheroo-1.0.0/switcheroo/ssh/data_org/publisher/__init__.py
+-rw-r--r--   0        0        0     1570 2023-07-28 19:01:01.542520 key_switcheroo-1.0.0/switcheroo/ssh/data_org/publisher/s3.py
+-rw-r--r--   0        0        0     2957 2023-07-28 17:54:52.118328 key_switcheroo-1.0.0/switcheroo/ssh/data_org/retriever/__init__.py
+-rw-r--r--   0        0        0     2094 2023-07-28 19:01:01.552519 key_switcheroo-1.0.0/switcheroo/ssh/data_org/retriever/s3.py
+-rw-r--r--   0        0        0     1421 2023-07-28 19:01:01.552519 key_switcheroo-1.0.0/switcheroo/ssh/data_stores/__init__.py
+-rw-r--r--   0        0        0      900 2023-07-28 19:01:01.552519 key_switcheroo-1.0.0/switcheroo/ssh/exceptions.py
+-rw-r--r--   0        0        0      183 2023-07-28 17:54:52.118328 key_switcheroo-1.0.0/switcheroo/ssh/objects/__init__.py
+-rw-r--r--   0        0        0     5235 2023-07-28 19:01:01.552519 key_switcheroo-1.0.0/switcheroo/ssh/objects/key.py
+-rw-r--r--   0        0        0      360 2023-08-03 17:05:55.859365 key_switcheroo-1.0.0/switcheroo/ssh/scripts/__init__.py
+-rw-r--r--   0        0        0     5175 2023-08-02 17:20:58.786236 key_switcheroo-1.0.0/switcheroo/ssh/scripts/publish.py
+-rw-r--r--   0        0        0     3421 2023-08-02 17:20:58.786236 key_switcheroo-1.0.0/switcheroo/ssh/scripts/retrieve.py
+-rw-r--r--   0        0        0     2997 2023-07-28 17:54:52.118328 key_switcheroo-1.0.0/switcheroo/util.py
+-rw-r--r--   0        0        0     8476 1970-01-01 00:00:00.000000 key_switcheroo-1.0.0/PKG-INFO
```

### Comparing `key_switcheroo-0.0.9/pyproject.toml` & `key_switcheroo-1.0.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 [tool.poetry]
 name = "key-switcheroo"
 version = "0.1.0"
 description = "Rotate SSH keys, stored in the cloud!"
 authors = ["Your Name <you@example.com>"]
 readme = "README.md"
-packages = [{include = "switcheroo"}]
+packages = [{include = "switcheroo"}, {include="metric_system"}, {include="aws_profiles"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
-paramiko = "^3.2.0"
 pycryptodome = "^3.18.0"
-psutil = "^5.9.5"
 boto3 = "^1.27.0"
+boto3-stubs = {version = "1.28.2", extras = ["cloudwatch", "s3", "sts"]}
 
 [tool.poetry.group.dev.dependencies]
 PyHamcrest = "^2.0.4"
 pyright = "^1.1.316"
 pylint = "^2.17.4"
 black = "^23.3.0"
-boto3-stubs = {version = "1.28.2", extras = ["cloudwatch", "s3", "sts"]}
 pytest = "^7.4.0"
 pytest-asyncio = "^0.21.0"
+moto = {extras = ["cloudwatch", "s3", "sts"], version = "^4.1.13"}
+requests = "^2.31.0"
+paramiko = "^3.3.0"
 
 [tool.poetry.scripts]
 
 switcheroo_publish = "switcheroo.ssh.scripts.publish:main"
 switcheroo_retrieve = "switcheroo.ssh.scripts.retrieve:main"
+switcheroo_configure = "switcheroo.base.scripts.configure:run_with_cli"
 
 [build-system]
 requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+build-backend = "poetry.core.masonry.api"
```

### Comparing `key_switcheroo-0.0.9/switcheroo/base/data_store/s3.py` & `key_switcheroo-1.0.0/switcheroo/base/data_store/s3.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,45 +1,76 @@
 from typing import Any, TypeVar
 from pathlib import Path
 import boto3
 from botocore.exceptions import ClientError
+from mypy_boto3_s3 import S3Client
+from mypy_boto3_sts import STSClient
 from switcheroo.base.data_store import DataStore
 from switcheroo.base.exceptions.s3 import (
     UnconfiguredAWSException,
     NoBucketFoundException,
 )
 
 T = TypeVar("T")
 
 
 class S3DataStore(DataStore):
-    def __init__(self, _bucket_name: str):
+    """See base classes. Stores items in an AWS S3 Bucket. \
+    Credentials for AWS are read from the users AWS command line utility - if AWS command line \
+    is not installed and configured, this class will not work
+    """
+
+    def __init__(
+        self, _bucket_name: str, access_key: str, secret_access_key: str, region: str
+    ):
+        """Initialize the data store. \
+        Uses credentials & region from the AWS CLI utility.
+
+        Args:
+            _bucket_name (str): the name of the S3 bucket to store items in
+
+        Raises:
+            UnconfiguredAWSException: If no AWS credentials are detected
+            NoBucketFoundException: If no bucket with the given name is found
+        """
         super().__init__()
         self._bucket_name = _bucket_name
-        self._s3_client = boto3.client("s3")  # type: ignore
+        self._s3_client: S3Client = boto3.client(
+            "s3",  # type: ignore
+            aws_access_key_id=access_key,
+            aws_secret_access_key=secret_access_key,
+            region_name=region,
+        )
         # Ensure AWS credentials are configured
-        sts_client = boto3.client("sts")  # type: ignore
+        sts_client: STSClient = boto3.client(
+            "sts",  # type: ignore
+            aws_access_key_id=access_key,
+            aws_secret_access_key=secret_access_key,
+            region_name=region,
+        )
         try:
             sts_client.get_caller_identity()
         except ClientError as exc:
             raise UnconfiguredAWSException() from exc
 
         # Ensure bucket exists - will error out otheriwse
         try:
             self._s3_client.head_bucket(Bucket=self._bucket_name)
         except ClientError as exc:
             raise NoBucketFoundException(self._bucket_name) from exc
 
     def publish(self, item: Any, location: Path):
+        """See base class"""
         serialized_data = super().serialize(item)
         self._s3_client.put_object(
             Bucket=self._bucket_name, Key=str(location), Body=serialized_data
         )
 
     def retrieve(self, location: Path, clas: type[T]) -> T | None:
+        """See base class"""
         try:
             response = self._s3_client.get_object(
                 Bucket=self._bucket_name, Key=str(location)
             )
             # Found item
             str_data: str = response["Body"].read().decode()
             deserialized_item: T = super().deserialize(str_data, clas)
```

### Comparing `key_switcheroo-0.0.9/switcheroo/paths.py` & `key_switcheroo-1.0.0/switcheroo/paths.py`

 * *Files 18% similar despite different names*

```diff
@@ -47,7 +47,19 @@
 def cloud_public_key_loc(host: str, user: str) -> Path:
     """Path to the public key (if stored in the cloud) for a host/user"""
     return cloud_key_dir(host, user) / KeyGen.PUBLIC_KEY_NAME
 
 
 def cloud_metadata_loc(host: str, user: str) -> Path:
     return cloud_key_dir(host, user) / KeyMetadata.FILE_NAME
+
+
+def app_data_dir() -> Path:
+    appdata_dir = Path.home() / ".switcheroo"
+    appdata_dir.mkdir(parents=True, exist_ok=True)
+    return appdata_dir
+
+
+def local_metrics_dir() -> Path:
+    metrics_dir = app_data_dir() / "metrics"
+    metrics_dir.mkdir(parents=True, exist_ok=True)
+    return metrics_dir
```

### Comparing `key_switcheroo-0.0.9/switcheroo/ssh/data_org/publisher/__init__.py` & `key_switcheroo-1.0.0/switcheroo/ssh/data_org/publisher/s3.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,57 +1,46 @@
-from abc import ABC, abstractmethod
 from pathlib import Path
 from switcheroo.ssh.objects import Key, KeyMetadata
-from switcheroo.ssh.data_stores import ssh_home_file_ds
+from switcheroo.base.data_store.s3 import S3DataStore
+from switcheroo.ssh.data_stores import sshify, ssh_home_file_ds
+from switcheroo.ssh.data_org.publisher import KeyPublisher
 from switcheroo import paths
 
 
-class KeyPublisher(ABC):
-    @abstractmethod
-    def publish_public_key(self, key: Key.PublicComponent, host: str, user: str):
-        pass
-
-    @abstractmethod
-    def publish_private_key(self, key: Key.PrivateComponent, host: str, user: str):
-        pass
-
-    @abstractmethod
-    def publish_key_metadata(self, metadata: KeyMetadata, host: str, user: str):
-        pass
-
-    def publish_key(
+class S3KeyPublisher(KeyPublisher):
+    def __init__(
         self,
-        host: str,
-        user: str,
-        key: Key | None = None,
-        metadata: KeyMetadata | None = None,
-    ) -> tuple[Key, KeyMetadata]:
-        # Lazy evaluation of default values
-        if key is None:
-            key = Key()
-        if metadata is None:
-            metadata = KeyMetadata.now_by_executing_user()
-        self.publish_public_key(key.public_key, host, user)
-        self.publish_private_key(key.private_key, host, user)
-        self.publish_key_metadata(metadata, host, user)
-        return (key, metadata)
-
-
-class FileKeyPublisher(KeyPublisher):
-    def __init__(self, ssh_home: Path = paths.local_ssh_home()):
-        self._ssh_home = ssh_home
-        self._key_ds = ssh_home_file_ds(ssh_home)
-
-    def publish_public_key(self, key: Key.PublicComponent, host: str, user: str):
-        return self._key_ds.publish(
-            item=key, location=paths.local_relative_public_key_loc(host, user)
+        s3_bucket_name: str,
+        access_key: str,
+        secret_access_key: str,
+        region: str,
+        root_ssh_dir: Path = paths.local_ssh_home(),
+    ):
+        self._s3_bucket_name = s3_bucket_name
+        self._privkey_ds = ssh_home_file_ds(root_ssh_dir)
+        self._pubkey_ds = sshify(
+            S3DataStore(
+                s3_bucket_name,
+                access_key=access_key,
+                secret_access_key=secret_access_key,
+                region=region,
+            )
+        )
+
+    @property
+    def s3_bucket_name(self):
+        return self._s3_bucket_name
+
+    def _publish_public_key(self, key: Key.PublicComponent, host: str, user: str):
+        return self._pubkey_ds.publish(
+            item=key, location=paths.cloud_public_key_loc(host, user)
         )
 
-    def publish_private_key(self, key: Key.PrivateComponent, host: str, user: str):
-        return self._key_ds.publish(
+    def _publish_private_key(self, key: Key.PrivateComponent, host: str, user: str):
+        return self._privkey_ds.publish(
             item=key, location=paths.local_relative_private_key_loc(host, user)
         )
 
-    def publish_key_metadata(self, metadata: KeyMetadata, host: str, user: str):
-        return self._key_ds.publish(
-            item=metadata, location=paths.local_relative_metadata_loc(host, user)
+    def _publish_key_metadata(self, metadata: KeyMetadata, host: str, user: str):
+        return self._pubkey_ds.publish(
+            item=metadata, location=paths.cloud_metadata_loc(host, user)
         )
```

### Comparing `key_switcheroo-0.0.9/switcheroo/ssh/data_org/retriever/__init__.py` & `key_switcheroo-1.0.0/switcheroo/ssh/data_org/retriever/__init__.py`

 * *Files identical despite different names*

### Comparing `key_switcheroo-0.0.9/switcheroo/ssh/data_org/retriever/s3.py` & `key_switcheroo-1.0.0/switcheroo/ssh/data_org/retriever/s3.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,19 +4,33 @@
 from switcheroo.ssh.data_stores import sshify, ssh_home_file_ds
 from switcheroo.ssh.objects import Key, KeyMetadata
 from switcheroo.ssh.data_org.retriever import retrieve_or_throw
 from switcheroo import paths
 
 
 class S3KeyRetriever(KeyRetriever):
-    def __init__(self, ssh_local_dir: Path, bucket_name: str) -> None:
+    def __init__(
+        self,
+        ssh_local_dir: Path,
+        access_key: str,
+        secret_access_key: str,
+        region: str,
+        bucket_name: str,
+    ) -> None:
         self._bucket_name = bucket_name
         self._ssh_local_dir = ssh_local_dir
         self._privatekey_datastore = ssh_home_file_ds(ssh_local_dir)
-        self._pubkey_datastore = sshify(S3DataStore(bucket_name))
+        self._pubkey_datastore = sshify(
+            S3DataStore(
+                bucket_name,
+                access_key=access_key,
+                secret_access_key=secret_access_key,
+                region=region,
+            )
+        )
 
     def retrieve_public_key(self, host: str, user: str) -> Key.PublicComponent:
         return retrieve_or_throw(
             self._pubkey_datastore,
             location=paths.cloud_public_key_loc(host, user),
             clas=Key.PublicComponent,
             ssh_item="public key",
```

### Comparing `key_switcheroo-0.0.9/switcheroo/ssh/data_stores/__init__.py` & `key_switcheroo-1.0.0/switcheroo/ssh/data_stores/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,20 +9,37 @@
     KeyMetadataSerializer,
 )
 
 T = TypeVar("T", bound=DataStore)
 
 
 def sshify(data_store: T) -> T:
+    """Registers all the serializers to have a datastore store ssh things
+
+    Args:
+        data_store (T): The datastore to register
+
+    Returns:
+        T: the datastore
+    """
     data_store.register_serializer(Key.PrivateComponent, PrivateKeySerializer())
     data_store.register_serializer(Key.PublicComponent, PublicKeySerializer())
     data_store.register_serializer(KeyMetadata, KeyMetadataSerializer())
     if isinstance(data_store, FileDataStore):
+        # Private keys require this file permission
         data_store.register_file_permissions(
             Key.PrivateComponent, FileDataStore.FilePermissions(0o600)
         )
     return data_store
 
 
 def ssh_home_file_ds(root_dir: Path) -> FileDataStore:
+    """Return a FileDataStore with it's root having private permissions - needed for ssh to work
+
+    Args:
+        root_dir (Path): The path to the root directory
+
+    Returns:
+        FileDataStore: The FileDataStore, rooted at the root argument
+    """
     ssh_file_ds = FileDataStore(FileDataStore.RootInfo(location=root_dir, mode=0o755))
     return sshify(ssh_file_ds)
```

### Comparing `key_switcheroo-0.0.9/switcheroo/ssh/objects/key.py` & `key_switcheroo-1.0.0/switcheroo/ssh/objects/key.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,35 @@
 from dataclasses import dataclass, field
 import json
 from getpass import getuser
-from typing import IO, ClassVar
+from typing import IO, ClassVar, Self
 from datetime import datetime
 from Crypto.PublicKey import RSA
 from switcheroo.base import Serializer
 
 
 class Key:  # pylint: disable=too-few-public-methods
+    """Enclosing object for a public key and corresponding private key"""
+
     class PrivateComponent:
         def __init__(self, byte_data: bytes):
             self.byte_data = byte_data
 
     class PublicComponent:
         def __init__(self, byte_data: bytes):
             self.byte_data = byte_data
 
     def __init__(self, key_tuple: tuple[bytes, bytes] | None = None) -> None:
+        """Initialize the Key instance
+
+        Args:
+            key_tuple (tuple[bytes, bytes] | None, optional): The key byte data as \
+            (private key, public key). If no data is passed in, a new key is generated. \
+            Defaults to None.
+        """
         super().__init__()
         if key_tuple is None:
             key_tuple = KeyGen.generate_private_public_key()
         self.private_key: Key.PrivateComponent = Key.PrivateComponent(key_tuple[0])
         self.public_key: Key.PublicComponent = Key.PublicComponent(key_tuple[1])
 
 
@@ -52,94 +61,100 @@
         private_key = key.export_key()
         public_key = key.public_key().export_key(format="OpenSSH")
         return private_key, public_key
 
 
 @dataclass(frozen=True)
 class KeyMetadata:
+    """Information about a key - who created it, and when it was generated"""
+
     FILE_NAME: ClassVar[str] = "metadata.json"
     created_by: str
     time_generated: datetime = field(default_factory=datetime.now)
 
     @classmethod
-    def now(cls, created_by: str | None):
-        """Returns a new metadata object
-
-        Create a new key metadata, using now as the creation time
+    def now(cls, created_by: str = "") -> Self:
+        """Create a new KeyMetadata object, using now as the current time.
 
         Args:
-            created_by (str): The user that created this key. Not required.
+            created_by (str): Who created the key. Defaults to empty.
+
+        Returns:
+            KeyMetadata: A new KeyMetadata instance with the provided information
         """
-        if created_by is None:
-            created_by = ""
         return KeyMetadata(created_by=created_by, time_generated=datetime.now())
 
     @classmethod
-    def now_by_executing_user(cls):
-        """Returns a new metadata object
-        
-        Create a new key metadata, using now as the creation time and the current\
-        executing user for the created_by field"""
+    def now_by_executing_user(cls) -> Self:
+        """Create a new KeyMetadata object, using now as the current time and the \
+        executing user (called with getpass.getuser()) as the creator.
+
+        Returns:
+            KeyMetadata: A new KeyMetadata instance
+        """
         return KeyMetadata.now(created_by=getuser())
 
     def _get_serialized_obj(self):
         return {
             "time_generated": str(self.time_generated),
             "created_by": self.created_by,
         }
 
     def serialize(self, target: IO[str]):
-        """
-        Dump the key metadata into the provided target
+        """Dumps the key metadata into the provided target in JSON format
 
         Args:
-            target (IO[str]): Where to dump the data in JSON format
+            target (IO[str]): Where to dump the information
         """
         json.dump(
             self._get_serialized_obj(),
             target,
         )
 
-    def serialize_to_string(self):
-        """
-        Serializes the key metadata to a JSON string that can later be parsed with from_io
+    def serialize_to_string(self) -> str:
+        """Serializes this object into a JSON-formatted string.
+
+        Returns:
+            str: The JSON-formatted representation of this string.
         """
         return json.dumps(self._get_serialized_obj())
 
     @classmethod
-    def from_io(cls, source: IO[str]):
-        """Returns the parsed KeyMetadata
-
-        Parse and return the KeyMetadata from the provided source
+    def from_io(cls, source: IO[str]) -> Self:
+        """Parses and return the KeyMetadata from the provided source
 
         Args:
             source (IO[str]): Where to get the JSON from
+
         Returns:
-            metadata (KeyMetadata): The key metadata
+            KeyMetadata: The key metadata
         """
         return cls.from_string(source.read())
 
     @classmethod
-    def from_string(cls, source: str):
-        """Returns the parsed KeyMetadata
-
-        Parse and return the KeyMetadata from the provided string source
+    def from_string(cls, source: str) -> Self:
+        """Parse and return the KeyMetadata from the provided string source
 
         Args:
             source (str): The JSON in a string
+
         Returns:
-            metadata (KeyMetadata): The key metadata
+            KeyMetadata: The key metadata
         """
         json_obj = json.loads(source)
         time_generated = datetime.strptime(
             json_obj["time_generated"], "%Y-%m-%d %H:%M:%S.%f"
         )
         created_by = json_obj["created_by"]
         return KeyMetadata(created_by, time_generated)
 
 
 class KeyMetadataSerializer(Serializer[KeyMetadata]):
+    """A Serializer for KeyMetadata, to be used by a DataStore."""
+
     def serialize(self, storable: KeyMetadata) -> str:
+        """See base class."""
         return storable.serialize_to_string()
 
     def deserialize(self, data_str: str) -> KeyMetadata:
+        """See base class."""
         return KeyMetadata.from_string(data_str)
```

### Comparing `key_switcheroo-0.0.9/switcheroo/ssh/scripts/retrieve.py` & `key_switcheroo-1.0.0/switcheroo/ssh/scripts/retrieve.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 from argparse import ArgumentParser
 from pathlib import Path
 import socket
 import traceback
 from switcheroo.ssh.data_org.retriever import KeyRetriever, FileKeyRetriever
 from switcheroo.ssh.data_org.retriever.s3 import S3KeyRetriever
+from switcheroo.ssh.scripts import get_credentials
 from switcheroo import paths
 
 
 def create_argument_parser() -> ArgumentParser:
+    """Creates an argument parser to define command line arguments
+
+    Returns:
+        ArgumentParser: parses the inputted command line arguments
+    """
     # pylint: disable=R0801
     argument_parser = ArgumentParser(
-        prog="key_retriever",
+        prog="switcheroo_retrieve",
         description="Fetches the public SSH keys from S3 or the local machine",
-        epilog="Thanks for using key_retriever! :)",
+        epilog="Thanks for using switcheroo_retrieve! :)",
     )
-    argument_parser.add_argument("user")
+    argument_parser.add_argument("user", help="the username of the connecting client")
     argument_parser.add_argument(
         "-ds",
         "--datastore",
         choices=["s3", "local"],
         default="s3",
         help="choose where to fetch the public key from, S3 or the local system (default is S3)",
     )
@@ -33,25 +39,59 @@
         help="The absolute path to\
             the directory that stores local keys (ie /home/you/.ssh)",
         default=paths.local_ssh_home(),
     )
     return argument_parser
 
 
-def main():
+def _local_store(
+    parser: ArgumentParser, sshdir: str, bucket: str | None = None
+) -> FileKeyRetriever:
+    if bucket is not None:
+        parser.error('Invalid argument "--bucket" when retrieving the keys locally')
+    return FileKeyRetriever(Path(sshdir))
+
+
+def _s3_store(
+    parser: ArgumentParser, credentials: tuple, sshdir: str, bucket: str | None = None
+) -> S3KeyRetriever:
+    if bucket is None:
+        parser.error("The s3 option requires a specified bucket name!")
+    return S3KeyRetriever(
+        sshdir,
+        credentials[0],
+        credentials[1],
+        credentials[2],
+        bucket,
+    )
+
+
+def main(arguments: list[str] | None = None):
+    """Main method to parse command line arguments and invoke key retrievers
+
+    Args:
+        arguments (list[str] | None, optional): Input command line args for testing
+
+    Raises:
+        InvalidArgumentError: Exception thrown when the user inputs an invalid argument
+        MissingArgumentError: Exception thrown when the user doesn't input a required argument
+    """
     parser = create_argument_parser()
-    args = parser.parse_args()
-    retriever: KeyRetriever | None = None
 
+    args = parser.parse_args(arguments)
+    retriever: KeyRetriever | None = None
+    credentials = get_credentials()
     if args.datastore == "local":
-        retriever = FileKeyRetriever(Path(args.sshdir))
+        retriever = _local_store(parser, args.sshdir, args.bucket)
     elif args.datastore == "s3":
-        if args.bucket is None:
-            parser.error("The s3 option requires a specified bucket name!")
-        retriever = S3KeyRetriever(paths.local_ssh_home(), args.bucket)
+        if credentials is None:
+            parser.error(
+                "You have no profiles configured, please configure one with switcheroo_configure"
+            )
+        retriever = _s3_store(parser, credentials, args.sshdir, args.bucket)
     try:
         assert retriever is not None
         public_key = retriever.retrieve_public_key(socket.getfqdn(), args.user)
         print(public_key.byte_data.decode())
     except Exception as exc:  # pylint: disable = broad-exception-caught
         print(exc)
         print(traceback.format_exc())
```

### Comparing `key_switcheroo-0.0.9/switcheroo/util.py` & `key_switcheroo-1.0.0/switcheroo/util.py`

 * *Files identical despite different names*

