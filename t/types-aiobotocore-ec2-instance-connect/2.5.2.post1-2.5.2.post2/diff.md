# Comparing `tmp/types-aiobotocore-ec2-instance-connect-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-ec2-instance-connect-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-ec2-instance-connect-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:12 2023, max compression
+gzip compressed data, was "types-aiobotocore-ec2-instance-connect-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:47 2023, max compression
```

## Comparing `types-aiobotocore-ec2-instance-connect-2.5.2.post1.tar` & `types-aiobotocore-ec2-instance-connect-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:12.465600 types-aiobotocore-ec2-instance-connect-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:37:48.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12796 2023-08-02 14:52:12.465600 types-aiobotocore-ec2-instance-connect-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-08-02 14:37:48.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:12.465600 types-aiobotocore-ec2-instance-connect-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-08-02 14:37:48.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:12.457600 types-aiobotocore-ec2-instance-connect-2.5.2.post1/types_aiobotocore_ec2_instance_connect/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-08-02 14:37:48.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post1/types_aiobotocore_ec2_instance_connect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-08-02 14:37:48.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post1/types_aiobotocore_ec2_instance_connect/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-08-02 14:37:48.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post1/types_aiobotocore_ec2_instance_connect/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6245 2023-08-02 14:37:48.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post1/types_aiobotocore_ec2_instance_connect/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-08-02 14:37:48.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post1/types_aiobotocore_ec2_instance_connect/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7614 2023-08-02 14:37:49.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post1/types_aiobotocore_ec2_instance_connect/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7612 2023-08-02 14:37:48.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post1/types_aiobotocore_ec2_instance_connect/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:37:48.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post1/types_aiobotocore_ec2_instance_connect/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-08-02 14:37:49.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post1/types_aiobotocore_ec2_instance_connect/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-08-02 14:37:49.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post1/types_aiobotocore_ec2_instance_connect/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:37:48.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post1/types_aiobotocore_ec2_instance_connect/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:12.465600 types-aiobotocore-ec2-instance-connect-2.5.2.post1/types_aiobotocore_ec2_instance_connect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12796 2023-08-02 14:52:12.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post1/types_aiobotocore_ec2_instance_connect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-02 14:52:12.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post1/types_aiobotocore_ec2_instance_connect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:12.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post1/types_aiobotocore_ec2_instance_connect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:12.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post1/types_aiobotocore_ec2_instance_connect.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:12.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post1/types_aiobotocore_ec2_instance_connect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-02 14:52:12.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post1/types_aiobotocore_ec2_instance_connect.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:47.791967 types-aiobotocore-ec2-instance-connect-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:45:16.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12885 2023-08-04 12:00:47.791967 types-aiobotocore-ec2-instance-connect-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11317 2023-08-04 11:45:16.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:47.791967 types-aiobotocore-ec2-instance-connect-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-08-04 11:45:16.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:47.779966 types-aiobotocore-ec2-instance-connect-2.5.2.post2/types_aiobotocore_ec2_instance_connect/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-08-04 11:45:16.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post2/types_aiobotocore_ec2_instance_connect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-08-04 11:45:16.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post2/types_aiobotocore_ec2_instance_connect/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-08-04 11:45:16.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post2/types_aiobotocore_ec2_instance_connect/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6245 2023-08-04 11:45:16.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post2/types_aiobotocore_ec2_instance_connect/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-08-04 11:45:16.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post2/types_aiobotocore_ec2_instance_connect/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7614 2023-08-04 11:45:16.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post2/types_aiobotocore_ec2_instance_connect/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7612 2023-08-04 11:45:16.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post2/types_aiobotocore_ec2_instance_connect/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:45:16.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post2/types_aiobotocore_ec2_instance_connect/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-08-04 11:45:16.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post2/types_aiobotocore_ec2_instance_connect/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-08-04 11:45:16.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post2/types_aiobotocore_ec2_instance_connect/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:45:16.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post2/types_aiobotocore_ec2_instance_connect/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:47.791967 types-aiobotocore-ec2-instance-connect-2.5.2.post2/types_aiobotocore_ec2_instance_connect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12885 2023-08-04 12:00:47.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post2/types_aiobotocore_ec2_instance_connect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-04 12:00:47.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post2/types_aiobotocore_ec2_instance_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:47.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post2/types_aiobotocore_ec2_instance_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:47.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post2/types_aiobotocore_ec2_instance_connect.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:47.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post2/types_aiobotocore_ec2_instance_connect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-04 12:00:47.000000 types-aiobotocore-ec2-instance-connect-2.5.2.post2/types_aiobotocore_ec2_instance_connect.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-ec2-instance-connect-2.5.2.post1/LICENSE` & `types-aiobotocore-ec2-instance-connect-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ec2-instance-connect-2.5.2.post1/PKG-INFO` & `types-aiobotocore-ec2-instance-connect-2.5.2.post2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ec2-instance-connect
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.EC2InstanceConnect 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.EC2InstanceConnect 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2_instance_connect/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -47,15 +47,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.17.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [types-aiobotocore](https://pypi.org/project/types-aiobotocore/) page and in
 [types-aiobotocore-ec2-instance-connect docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2_instance_connect/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,42 +266,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_ec2_instance_connect.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `EC2InstanceConnect` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2_instance_connect/literals/).
+
 ```python
-from types_aiobotocore_ec2_instance_connect.literals import (
-    EC2InstanceConnectServiceName,
-    ServiceName,
-    ResourceServiceName,
-)
+from types_aiobotocore_ec2_instance_connect.literals import EC2InstanceConnectServiceName
 
 
 def check_value(value: EC2InstanceConnectServiceName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_ec2_instance_connect.type_defs` module contains structures
 and shapes assembled to typed dictionaries and unions for additional type
 checking.
 
+Full list of `EC2InstanceConnect` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2_instance_connect/type_defs/).
+
 ```python
-from types_aiobotocore_ec2_instance_connect.type_defs import (
-    ResponseMetadataTypeDef,
-    SendSSHPublicKeyRequestRequestTypeDef,
-    SendSerialConsoleSSHPublicKeyRequestRequestTypeDef,
-    SendSSHPublicKeyResponseTypeDef,
-    SendSerialConsoleSSHPublicKeyResponseTypeDef,
-)
+from types_aiobotocore_ec2_instance_connect.type_defs import ResponseMetadataTypeDef
 
 
 def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-ec2-instance-connect-2.5.2.post1/README.md` & `types-aiobotocore-ec2-instance-connect-2.5.2.post2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.17.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [types-aiobotocore](https://pypi.org/project/types-aiobotocore/) page and in
 [types-aiobotocore-ec2-instance-connect docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2_instance_connect/).
 
 See how it helps to find and fix potential bugs:
 
@@ -234,42 +234,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_ec2_instance_connect.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `EC2InstanceConnect` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2_instance_connect/literals/).
+
 ```python
-from types_aiobotocore_ec2_instance_connect.literals import (
-    EC2InstanceConnectServiceName,
-    ServiceName,
-    ResourceServiceName,
-)
+from types_aiobotocore_ec2_instance_connect.literals import EC2InstanceConnectServiceName
 
 
 def check_value(value: EC2InstanceConnectServiceName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_ec2_instance_connect.type_defs` module contains structures
 and shapes assembled to typed dictionaries and unions for additional type
 checking.
 
+Full list of `EC2InstanceConnect` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2_instance_connect/type_defs/).
+
 ```python
-from types_aiobotocore_ec2_instance_connect.type_defs import (
-    ResponseMetadataTypeDef,
-    SendSSHPublicKeyRequestRequestTypeDef,
-    SendSerialConsoleSSHPublicKeyRequestRequestTypeDef,
-    SendSSHPublicKeyResponseTypeDef,
-    SendSerialConsoleSSHPublicKeyResponseTypeDef,
-)
+from types_aiobotocore_ec2_instance_connect.type_defs import ResponseMetadataTypeDef
 
 
 def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-ec2-instance-connect-2.5.2.post1/setup.py` & `types-aiobotocore-ec2-instance-connect-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-ec2-instance-connect",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_ec2_instance_connect"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.EC2InstanceConnect 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-ec2-instance-connect-2.5.2.post1/types_aiobotocore_ec2_instance_connect/__init__.py` & `types-aiobotocore-ec2-instance-connect-2.5.2.post2/types_aiobotocore_ec2_instance_connect/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ec2-instance-connect-2.5.2.post1/types_aiobotocore_ec2_instance_connect/__init__.pyi` & `types-aiobotocore-ec2-instance-connect-2.5.2.post2/types_aiobotocore_ec2_instance_connect/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ec2-instance-connect-2.5.2.post1/types_aiobotocore_ec2_instance_connect/__main__.py` & `types-aiobotocore-ec2-instance-connect-2.5.2.post2/types_aiobotocore_ec2_instance_connect/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.EC2InstanceConnect 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2_instance_connect//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2-instance-connect.html#EC2InstanceConnect\nOther"
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

### Comparing `types-aiobotocore-ec2-instance-connect-2.5.2.post1/types_aiobotocore_ec2_instance_connect/client.py` & `types-aiobotocore-ec2-instance-connect-2.5.2.post2/types_aiobotocore_ec2_instance_connect/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ec2-instance-connect-2.5.2.post1/types_aiobotocore_ec2_instance_connect/client.pyi` & `types-aiobotocore-ec2-instance-connect-2.5.2.post2/types_aiobotocore_ec2_instance_connect/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ec2-instance-connect-2.5.2.post1/types_aiobotocore_ec2_instance_connect/literals.py` & `types-aiobotocore-ec2-instance-connect-2.5.2.post2/types_aiobotocore_ec2_instance_connect/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ec2-instance-connect-2.5.2.post1/types_aiobotocore_ec2_instance_connect/literals.pyi` & `types-aiobotocore-ec2-instance-connect-2.5.2.post2/types_aiobotocore_ec2_instance_connect/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ec2-instance-connect-2.5.2.post1/types_aiobotocore_ec2_instance_connect/type_defs.py` & `types-aiobotocore-ec2-instance-connect-2.5.2.post2/types_aiobotocore_ec2_instance_connect/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ec2-instance-connect-2.5.2.post1/types_aiobotocore_ec2_instance_connect/type_defs.pyi` & `types-aiobotocore-ec2-instance-connect-2.5.2.post2/types_aiobotocore_ec2_instance_connect/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ec2-instance-connect-2.5.2.post1/types_aiobotocore_ec2_instance_connect.egg-info/PKG-INFO` & `types-aiobotocore-ec2-instance-connect-2.5.2.post2/types_aiobotocore_ec2_instance_connect.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ec2-instance-connect
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.EC2InstanceConnect 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.EC2InstanceConnect 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2_instance_connect/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -47,15 +47,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.17.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [types-aiobotocore](https://pypi.org/project/types-aiobotocore/) page and in
 [types-aiobotocore-ec2-instance-connect docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2_instance_connect/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,42 +266,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_ec2_instance_connect.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `EC2InstanceConnect` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2_instance_connect/literals/).
+
 ```python
-from types_aiobotocore_ec2_instance_connect.literals import (
-    EC2InstanceConnectServiceName,
-    ServiceName,
-    ResourceServiceName,
-)
+from types_aiobotocore_ec2_instance_connect.literals import EC2InstanceConnectServiceName
 
 
 def check_value(value: EC2InstanceConnectServiceName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_ec2_instance_connect.type_defs` module contains structures
 and shapes assembled to typed dictionaries and unions for additional type
 checking.
 
+Full list of `EC2InstanceConnect` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2_instance_connect/type_defs/).
+
 ```python
-from types_aiobotocore_ec2_instance_connect.type_defs import (
-    ResponseMetadataTypeDef,
-    SendSSHPublicKeyRequestRequestTypeDef,
-    SendSerialConsoleSSHPublicKeyRequestRequestTypeDef,
-    SendSSHPublicKeyResponseTypeDef,
-    SendSerialConsoleSSHPublicKeyResponseTypeDef,
-)
+from types_aiobotocore_ec2_instance_connect.type_defs import ResponseMetadataTypeDef
 
 
 def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-ec2-instance-connect-2.5.2.post1/types_aiobotocore_ec2_instance_connect.egg-info/SOURCES.txt` & `types-aiobotocore-ec2-instance-connect-2.5.2.post2/types_aiobotocore_ec2_instance_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

