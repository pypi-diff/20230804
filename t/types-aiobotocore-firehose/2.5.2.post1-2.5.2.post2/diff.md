# Comparing `tmp/types-aiobotocore-firehose-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-firehose-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-firehose-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:19 2023, max compression
+gzip compressed data, was "types-aiobotocore-firehose-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:55 2023, max compression
```

## Comparing `types-aiobotocore-firehose-2.5.2.post1.tar` & `types-aiobotocore-firehose-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:18.993583 types-aiobotocore-firehose-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:38:46.000000 types-aiobotocore-firehose-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16805 2023-08-02 14:52:18.993583 types-aiobotocore-firehose-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15283 2023-08-02 14:38:46.000000 types-aiobotocore-firehose-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:18.993583 types-aiobotocore-firehose-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-08-02 14:38:46.000000 types-aiobotocore-firehose-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:18.993583 types-aiobotocore-firehose-2.5.2.post1/types_aiobotocore_firehose/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-08-02 14:38:46.000000 types-aiobotocore-firehose-2.5.2.post1/types_aiobotocore_firehose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-08-02 14:38:46.000000 types-aiobotocore-firehose-2.5.2.post1/types_aiobotocore_firehose/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-02 14:38:46.000000 types-aiobotocore-firehose-2.5.2.post1/types_aiobotocore_firehose/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14113 2023-08-02 14:38:46.000000 types-aiobotocore-firehose-2.5.2.post1/types_aiobotocore_firehose/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14093 2023-08-02 14:38:46.000000 types-aiobotocore-firehose-2.5.2.post1/types_aiobotocore_firehose/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11308 2023-08-02 14:38:47.000000 types-aiobotocore-firehose-2.5.2.post1/types_aiobotocore_firehose/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11306 2023-08-02 14:38:46.000000 types-aiobotocore-firehose-2.5.2.post1/types_aiobotocore_firehose/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:46.000000 types-aiobotocore-firehose-2.5.2.post1/types_aiobotocore_firehose/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    48448 2023-08-02 14:38:47.000000 types-aiobotocore-firehose-2.5.2.post1/types_aiobotocore_firehose/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    48397 2023-08-02 14:38:47.000000 types-aiobotocore-firehose-2.5.2.post1/types_aiobotocore_firehose/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:38:46.000000 types-aiobotocore-firehose-2.5.2.post1/types_aiobotocore_firehose/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:18.993583 types-aiobotocore-firehose-2.5.2.post1/types_aiobotocore_firehose.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16805 2023-08-02 14:52:18.000000 types-aiobotocore-firehose-2.5.2.post1/types_aiobotocore_firehose.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-08-02 14:52:18.000000 types-aiobotocore-firehose-2.5.2.post1/types_aiobotocore_firehose.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:18.000000 types-aiobotocore-firehose-2.5.2.post1/types_aiobotocore_firehose.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:18.000000 types-aiobotocore-firehose-2.5.2.post1/types_aiobotocore_firehose.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:18.000000 types-aiobotocore-firehose-2.5.2.post1/types_aiobotocore_firehose.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-02 14:52:18.000000 types-aiobotocore-firehose-2.5.2.post1/types_aiobotocore_firehose.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:55.280248 types-aiobotocore-firehose-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:46:16.000000 types-aiobotocore-firehose-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12341 2023-08-04 12:00:55.280248 types-aiobotocore-firehose-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10819 2023-08-04 11:46:16.000000 types-aiobotocore-firehose-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:55.280248 types-aiobotocore-firehose-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-08-04 11:46:16.000000 types-aiobotocore-firehose-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:55.280248 types-aiobotocore-firehose-2.5.2.post2/types_aiobotocore_firehose/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-08-04 11:46:16.000000 types-aiobotocore-firehose-2.5.2.post2/types_aiobotocore_firehose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-08-04 11:46:16.000000 types-aiobotocore-firehose-2.5.2.post2/types_aiobotocore_firehose/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-04 11:46:16.000000 types-aiobotocore-firehose-2.5.2.post2/types_aiobotocore_firehose/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14113 2023-08-04 11:46:16.000000 types-aiobotocore-firehose-2.5.2.post2/types_aiobotocore_firehose/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14093 2023-08-04 11:46:16.000000 types-aiobotocore-firehose-2.5.2.post2/types_aiobotocore_firehose/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11308 2023-08-04 11:46:17.000000 types-aiobotocore-firehose-2.5.2.post2/types_aiobotocore_firehose/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11306 2023-08-04 11:46:16.000000 types-aiobotocore-firehose-2.5.2.post2/types_aiobotocore_firehose/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:46:16.000000 types-aiobotocore-firehose-2.5.2.post2/types_aiobotocore_firehose/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    45062 2023-08-04 11:46:17.000000 types-aiobotocore-firehose-2.5.2.post2/types_aiobotocore_firehose/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45013 2023-08-04 11:46:17.000000 types-aiobotocore-firehose-2.5.2.post2/types_aiobotocore_firehose/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:46:16.000000 types-aiobotocore-firehose-2.5.2.post2/types_aiobotocore_firehose/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:55.280248 types-aiobotocore-firehose-2.5.2.post2/types_aiobotocore_firehose.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12341 2023-08-04 12:00:55.000000 types-aiobotocore-firehose-2.5.2.post2/types_aiobotocore_firehose.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-08-04 12:00:55.000000 types-aiobotocore-firehose-2.5.2.post2/types_aiobotocore_firehose.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:55.000000 types-aiobotocore-firehose-2.5.2.post2/types_aiobotocore_firehose.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:55.000000 types-aiobotocore-firehose-2.5.2.post2/types_aiobotocore_firehose.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:55.000000 types-aiobotocore-firehose-2.5.2.post2/types_aiobotocore_firehose.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-04 12:00:55.000000 types-aiobotocore-firehose-2.5.2.post2/types_aiobotocore_firehose.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-firehose-2.5.2.post1/LICENSE` & `types-aiobotocore-firehose-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-firehose-2.5.2.post1/README.md` & `types-aiobotocore-firehose-2.5.2.post2/types_aiobotocore_firehose/client.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,480 +1,284 @@
-<a id="types-aiobotocore-firehose"></a>
+"""
+Type annotations for firehose service client.
 
-# types-aiobotocore-firehose
+[Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/client/)
 
-[![PyPI - types-aiobotocore-firehose](https://img.shields.io/pypi/v/types-aiobotocore-firehose.svg?color=blue)](https://pypi.org/project/types-aiobotocore-firehose)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-firehose.svg?color=blue)](https://pypi.org/project/types-aiobotocore-firehose)
-[![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-firehose)](https://pepy.tech/project/types-aiobotocore-firehose)
+Usage::
 
-![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
+    ```python
+    from aiobotocore.session import get_session
+    from types_aiobotocore_firehose.client import FirehoseClient
 
-Type annotations for
-[aiobotocore.Firehose 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose)
-service compatible with [VSCode](https://code.visualstudio.com/),
-[PyCharm](https://www.jetbrains.com/pycharm/),
-[Emacs](https://www.gnu.org/software/emacs/),
-[Sublime Text](https://www.sublimetext.com/),
-[mypy](https://github.com/python/mypy),
-[pyright](https://github.com/microsoft/pyright) and other tools.
+    session = get_session()
+    async with session.create_client("firehose") as client:
+        client: FirehoseClient
+    ```
+"""
+from typing import Any, Dict, Mapping, Sequence, Type
 
-Generated by
-[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
+from aiobotocore.client import AioBaseClient
+from botocore.client import ClientMeta
 
-More information can be found on
-[types-aiobotocore](https://pypi.org/project/types-aiobotocore/) page and in
-[types-aiobotocore-firehose docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/).
-
-See how it helps to find and fix potential bugs:
-
-![boto3-stubs demo](https://github.com/youtype/mypy_boto3_builder/raw/main/demo.gif)
-
-- [types-aiobotocore-firehose](#types-aiobotocore-firehose)
-  - [How to install](#how-to-install)
-    - [From PyPI with pip](#from-pypi-with-pip)
-  - [How to uninstall](#how-to-uninstall)
-  - [Usage](#usage)
-    - [VSCode](#vscode)
-    - [PyCharm](#pycharm)
-    - [Emacs](#emacs)
-    - [Sublime Text](#sublime-text)
-    - [Other IDEs](#other-ides)
-    - [mypy](#mypy)
-    - [pyright](#pyright)
-  - [Explicit type annotations](#explicit-type-annotations)
-    - [Client annotations](#client-annotations)
-    - [Literals](#literals)
-    - [Type definitions](#type-definitions)
-  - [How it works](#how-it-works)
-  - [What's new](#what's-new)
-    - [Implemented features](#implemented-features)
-    - [Latest changes](#latest-changes)
-  - [Versioning](#versioning)
-  - [Thank you](#thank-you)
-  - [Documentation](#documentation)
-  - [Support and contributing](#support-and-contributing)
-
-<a id="how-to-install"></a>
-
-## How to install
-
-<a id="from-pypi-with-pip"></a>
-
-### From PyPI with pip
-
-Install `types-aiobotocore` for `Firehose` service.
-
-```bash
-# install with aiobotocore type annotations
-python -m pip install 'types-aiobotocore[firehose]'
-
-
-# Lite version does not provide session.client/resource overloads
-# it is more RAM-friendly, but requires explicit type annotations
-python -m pip install 'types-aiobotocore-lite[firehose]'
-
-
-# standalone installation
-python -m pip install types-aiobotocore-firehose
-```
-
-<a id="how-to-uninstall"></a>
-
-## How to uninstall
-
-```bash
-python -m pip uninstall -y types-aiobotocore-firehose
-```
-
-<a id="usage"></a>
-
-## Usage
-
-<a id="vscode"></a>
-
-### VSCode
-
-- Install
-  [Python extension](https://marketplace.visualstudio.com/items?itemName=ms-python.python)
-- Install
-  [Pylance extension](https://marketplace.visualstudio.com/items?itemName=ms-python.vscode-pylance)
-- Set `Pylance` as your Python Language Server
-- Install `types-aiobotocore[firehose]` in your environment:
-
-```bash
-python -m pip install 'types-aiobotocore[firehose]'
-```
-
-Both type checking and code completion should now work. No explicit type
-annotations required, write your `aiobotocore` code as usual.
-
-<a id="pycharm"></a>
-
-### PyCharm
-
-Install `types-aiobotocore-lite[firehose]` in your environment:
-
-```bash
-python -m pip install 'types-aiobotocore-lite[firehose]'`
-```
-
-Both type checking and code completion should now work. Explicit type
-annotations **are required**.
-
-Use `types-aiobotocore` package instead for implicit type discovery.
-
-<a id="emacs"></a>
-
-### Emacs
-
-- Install `types-aiobotocore` with services you use in your environment:
-
-```bash
-python -m pip install 'types-aiobotocore[firehose]'
-```
-
-- Install [use-package](https://github.com/jwiegley/use-package),
-  [lsp](https://github.com/emacs-lsp/lsp-mode/),
-  [company](https://github.com/company-mode/company-mode) and
-  [flycheck](https://github.com/flycheck/flycheck) packages
-- Install [lsp-pyright](https://github.com/emacs-lsp/lsp-pyright) package
-
-```elisp
-(use-package lsp-pyright
-  :ensure t
-  :hook (python-mode . (lambda ()
-                          (require 'lsp-pyright)
-                          (lsp)))  ; or lsp-deferred
-  :init (when (executable-find "python3")
-          (setq lsp-pyright-python-executable-cmd "python3"))
-  )
-```
-
-- Make sure emacs uses the environment where you have installed
-  `types-aiobotocore`
-
-Type checking should now work. No explicit type annotations required, write
-your `aiobotocore` code as usual.
-
-<a id="sublime-text"></a>
-
-### Sublime Text
-
-- Install `types-aiobotocore[firehose]` with services you use in your
-  environment:
-
-```bash
-python -m pip install 'types-aiobotocore[firehose]'
-```
-
-- Install [LSP-pyright](https://github.com/sublimelsp/LSP-pyright) package
-
-Type checking should now work. No explicit type annotations required, write
-your `aiobotocore` code as usual.
-
-<a id="other-ides"></a>
-
-### Other IDEs
-
-Not tested, but as long as your IDE supports `mypy` or `pyright`, everything
-should work.
-
-<a id="mypy"></a>
-
-### mypy
-
-- Install `mypy`: `python -m pip install mypy`
-- Install `types-aiobotocore[firehose]` in your environment:
-
-```bash
-python -m pip install 'types-aiobotocore[firehose]'`
-```
-
-Type checking should now work. No explicit type annotations required, write
-your `aiobotocore` code as usual.
-
-<a id="pyright"></a>
-
-### pyright
-
-- Install `pyright`: `npm i -g pyright`
-- Install `types-aiobotocore[firehose]` in your environment:
-
-```bash
-python -m pip install 'types-aiobotocore[firehose]'
-```
-
-Optionally, you can install `types-aiobotocore` to `typings` folder.
-
-Type checking should now work. No explicit type annotations required, write
-your `aiobotocore` code as usual.
-
-<a id="explicit-type-annotations"></a>
-
-## Explicit type annotations
-
-<a id="client-annotations"></a>
-
-### Client annotations
-
-`FirehoseClient` provides annotations for `session.create_client("firehose")`.
-
-```python
-from aiobotocore.session import get_session
-
-from types_aiobotocore_firehose import FirehoseClient
-
-session = get_session()
-async with session.create_client("firehose") as client:
-    client: FirehoseClient
-    # now client usage is checked by mypy and IDE should provide code completion
-```
-
-<a id="literals"></a>
-
-### Literals
-
-`types_aiobotocore_firehose.literals` module contains literals extracted from
-shapes that can be used in user code for type checking.
-
-```python
-from types_aiobotocore_firehose.literals import (
-    AmazonOpenSearchServerlessS3BackupModeType,
-    AmazonopensearchserviceIndexRotationPeriodType,
-    AmazonopensearchserviceS3BackupModeType,
-    CompressionFormatType,
-    ContentEncodingType,
-    DeliveryStreamEncryptionStatusType,
-    DeliveryStreamFailureTypeType,
-    DeliveryStreamStatusType,
-    DeliveryStreamTypeType,
-    ElasticsearchIndexRotationPeriodType,
-    ElasticsearchS3BackupModeType,
-    HECEndpointTypeType,
-    HttpEndpointS3BackupModeType,
-    KeyTypeType,
-    NoEncryptionConfigType,
-    OrcCompressionType,
-    OrcFormatVersionType,
-    ParquetCompressionType,
-    ParquetWriterVersionType,
-    ProcessorParameterNameType,
-    ProcessorTypeType,
-    RedshiftS3BackupModeType,
-    S3BackupModeType,
-    SplunkS3BackupModeType,
-    FirehoseServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
-
-
-def check_value(value: AmazonOpenSearchServerlessS3BackupModeType) -> bool:
-    ...
-```
-
-<a id="type-definitions"></a>
-
-### Type definitions
-
-`types_aiobotocore_firehose.type_defs` module contains structures and shapes
-assembled to typed dictionaries and unions for additional type checking.
-
-```python
-from types_aiobotocore_firehose.type_defs import (
-    AmazonOpenSearchServerlessBufferingHintsTypeDef,
-    AmazonOpenSearchServerlessRetryOptionsTypeDef,
-    CloudWatchLoggingOptionsTypeDef,
-    VpcConfigurationTypeDef,
-    VpcConfigurationDescriptionTypeDef,
-    AmazonopensearchserviceBufferingHintsTypeDef,
-    AmazonopensearchserviceRetryOptionsTypeDef,
-    BlobTypeDef,
-    BufferingHintsTypeDef,
-    CopyCommandTypeDef,
-    DeliveryStreamEncryptionConfigurationInputTypeDef,
-    KinesisStreamSourceConfigurationTypeDef,
-    TagTypeDef,
-    ResponseMetadataTypeDef,
-    SchemaConfigurationTypeDef,
-    DeleteDeliveryStreamInputRequestTypeDef,
-    FailureDescriptionTypeDef,
-    DescribeDeliveryStreamInputRequestTypeDef,
-    HiveJsonSerDeOutputTypeDef,
-    OpenXJsonSerDeOutputTypeDef,
-    HiveJsonSerDeTypeDef,
-    OpenXJsonSerDeTypeDef,
-    RetryOptionsTypeDef,
-    ElasticsearchBufferingHintsTypeDef,
-    ElasticsearchRetryOptionsTypeDef,
-    KMSEncryptionConfigTypeDef,
-    HttpEndpointBufferingHintsTypeDef,
-    HttpEndpointCommonAttributeTypeDef,
-    HttpEndpointConfigurationTypeDef,
-    HttpEndpointDescriptionTypeDef,
-    HttpEndpointRetryOptionsTypeDef,
-    KinesisStreamSourceDescriptionTypeDef,
-    ListDeliveryStreamsInputRequestTypeDef,
-    ListTagsForDeliveryStreamInputRequestTypeDef,
-    OrcSerDeOutputTypeDef,
-    OrcSerDeTypeDef,
-    ParquetSerDeTypeDef,
-    ProcessorParameterTypeDef,
-    PutRecordBatchResponseEntryTypeDef,
-    RedshiftRetryOptionsTypeDef,
-    SplunkRetryOptionsTypeDef,
-    StopDeliveryStreamEncryptionInputRequestTypeDef,
-    UntagDeliveryStreamInputRequestTypeDef,
-    RecordTypeDef,
-    StartDeliveryStreamEncryptionInputRequestTypeDef,
-    TagDeliveryStreamInputRequestTypeDef,
-    CreateDeliveryStreamOutputTypeDef,
-    ListDeliveryStreamsOutputTypeDef,
-    ListTagsForDeliveryStreamOutputTypeDef,
-    PutRecordOutputTypeDef,
-    DeliveryStreamEncryptionConfigurationTypeDef,
-    DeserializerOutputTypeDef,
-    DeserializerTypeDef,
-    DynamicPartitioningConfigurationTypeDef,
-    EncryptionConfigurationTypeDef,
-    HttpEndpointRequestConfigurationOutputTypeDef,
-    HttpEndpointRequestConfigurationTypeDef,
-    SourceDescriptionTypeDef,
-    SerializerOutputTypeDef,
-    SerializerTypeDef,
-    ProcessorOutputTypeDef,
-    ProcessorTypeDef,
-    PutRecordBatchOutputTypeDef,
-    PutRecordBatchInputRequestTypeDef,
-    PutRecordInputRequestTypeDef,
-    InputFormatConfigurationOutputTypeDef,
-    InputFormatConfigurationTypeDef,
-    S3DestinationConfigurationTypeDef,
-    S3DestinationDescriptionTypeDef,
-    S3DestinationUpdateTypeDef,
-    OutputFormatConfigurationOutputTypeDef,
-    OutputFormatConfigurationTypeDef,
-    ProcessingConfigurationOutputTypeDef,
-    ProcessingConfigurationTypeDef,
-    DataFormatConversionConfigurationOutputTypeDef,
-    DataFormatConversionConfigurationTypeDef,
-    AmazonOpenSearchServerlessDestinationDescriptionTypeDef,
-    AmazonopensearchserviceDestinationDescriptionTypeDef,
-    ElasticsearchDestinationDescriptionTypeDef,
-    HttpEndpointDestinationDescriptionTypeDef,
-    RedshiftDestinationDescriptionTypeDef,
-    SplunkDestinationDescriptionTypeDef,
+from .literals import DeliveryStreamTypeType
+from .type_defs import (
     AmazonOpenSearchServerlessDestinationConfigurationTypeDef,
     AmazonOpenSearchServerlessDestinationUpdateTypeDef,
     AmazonopensearchserviceDestinationConfigurationTypeDef,
     AmazonopensearchserviceDestinationUpdateTypeDef,
+    CreateDeliveryStreamOutputTypeDef,
+    DeliveryStreamEncryptionConfigurationInputTypeDef,
+    DescribeDeliveryStreamOutputTypeDef,
     ElasticsearchDestinationConfigurationTypeDef,
     ElasticsearchDestinationUpdateTypeDef,
+    ExtendedS3DestinationConfigurationTypeDef,
+    ExtendedS3DestinationUpdateTypeDef,
     HttpEndpointDestinationConfigurationTypeDef,
     HttpEndpointDestinationUpdateTypeDef,
+    KinesisStreamSourceConfigurationTypeDef,
+    ListDeliveryStreamsOutputTypeDef,
+    ListTagsForDeliveryStreamOutputTypeDef,
+    PutRecordBatchOutputTypeDef,
+    PutRecordOutputTypeDef,
+    RecordTypeDef,
     RedshiftDestinationConfigurationTypeDef,
     RedshiftDestinationUpdateTypeDef,
+    S3DestinationConfigurationTypeDef,
+    S3DestinationUpdateTypeDef,
     SplunkDestinationConfigurationTypeDef,
     SplunkDestinationUpdateTypeDef,
-    ExtendedS3DestinationDescriptionTypeDef,
-    ExtendedS3DestinationConfigurationTypeDef,
-    ExtendedS3DestinationUpdateTypeDef,
-    DestinationDescriptionTypeDef,
-    CreateDeliveryStreamInputRequestTypeDef,
-    UpdateDestinationInputRequestTypeDef,
-    DeliveryStreamDescriptionTypeDef,
-    DescribeDeliveryStreamOutputTypeDef,
+    TagTypeDef,
 )
 
+__all__ = ("FirehoseClient",)
 
-def get_value() -> AmazonOpenSearchServerlessBufferingHintsTypeDef:
-    return {...}
-```
-
-<a id="how-it-works"></a>
-
-## How it works
-
-Fully automated
-[mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
-generates type annotations for each service, patiently waiting for
-`aiobotocore` updates. It delivers drop-in type annotations for you and makes
-sure that:
-
-- All available `aiobotocore` services are covered.
-- Each public class and method of every `aiobotocore` service gets valid type
-  annotations extracted from `botocore` schemas.
-- Type annotations include up-to-date documentation.
-- Link to documentation is provided for every method.
-- Code is processed by [black](https://github.com/psf/black) and
-  [isort](https://github.com/PyCQA/isort) for readability.
-
-<a id="what's-new"></a>
-
-## What's new
-
-<a id="implemented-features"></a>
-
-### Implemented features
-
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
-- `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
-  compatibility
-- `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
-  annotations for each service
-- Generated `TypeDefs` for each service
-- Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
-- Auto discovery of types for `client.get_waiter` and `client.get_paginator`
-  calls
-- Auto discovery of types for `ServiceResource` and `Resource` collections
-- Auto discovery of types for `aiobotocore.Session.create_client` calls
-
-<a id="latest-changes"></a>
-
-### Latest changes
-
-Builder changelog can be found in
-[Releases](https://github.com/youtype/mypy_boto3_builder/releases).
-
-<a id="versioning"></a>
-
-## Versioning
-
-`types-aiobotocore-firehose` version is the same as related `aiobotocore`
-version and follows [PEP 440](https://www.python.org/dev/peps/pep-0440/)
-format.
-
-<a id="thank-you"></a>
-
-## Thank you
-
-- [Allie Fitter](https://github.com/alliefitter) for
-  [boto3-type-annotations](https://pypi.org/project/boto3-type-annotations/),
-  this package is based on top of his work
-- [black](https://github.com/psf/black) developers for an awesome formatting
-  tool
-- [Timothy Edmund Crosley](https://github.com/timothycrosley) for
-  [isort](https://github.com/PyCQA/isort) and how flexible it is
-- [mypy](https://github.com/python/mypy) developers for doing all dirty work
-  for us
-- [pyright](https://github.com/microsoft/pyright) team for the new era of typed
-  Python
-
-<a id="documentation"></a>
-
-## Documentation
-
-All services type annotations can be found in
-[aiobotocore docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/)
-
-<a id="support-and-contributing"></a>
 
-## Support and contributing
+class BotocoreClientError(BaseException):
+    MSG_TEMPLATE: str
 
-This package is auto-generated. Please reports any bugs or request new features
-in [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder/issues/)
-repository.
+    def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
+        self.response: Dict[str, Any]
+        self.operation_name: str
+
+
+class Exceptions:
+    ClientError: Type[BotocoreClientError]
+    ConcurrentModificationException: Type[BotocoreClientError]
+    InvalidArgumentException: Type[BotocoreClientError]
+    InvalidKMSResourceException: Type[BotocoreClientError]
+    LimitExceededException: Type[BotocoreClientError]
+    ResourceInUseException: Type[BotocoreClientError]
+    ResourceNotFoundException: Type[BotocoreClientError]
+    ServiceUnavailableException: Type[BotocoreClientError]
+
+
+class FirehoseClient(AioBaseClient):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose.Client)
+    [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/client/)
+    """
+
+    meta: ClientMeta
+
+    @property
+    def exceptions(self) -> Exceptions:
+        """
+        FirehoseClient exceptions.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose.Client.exceptions)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/client/#exceptions)
+        """
+
+    def can_paginate(self, operation_name: str) -> bool:
+        """
+        Check if an operation can be paginated.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose.Client.can_paginate)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/client/#can_paginate)
+        """
+
+    async def close(self) -> None:
+        """
+        Closes underlying endpoint connections.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose.Client.close)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/client/#close)
+        """
+
+    async def create_delivery_stream(
+        self,
+        *,
+        DeliveryStreamName: str,
+        DeliveryStreamType: DeliveryStreamTypeType = ...,
+        KinesisStreamSourceConfiguration: KinesisStreamSourceConfigurationTypeDef = ...,
+        DeliveryStreamEncryptionConfigurationInput: DeliveryStreamEncryptionConfigurationInputTypeDef = ...,
+        S3DestinationConfiguration: S3DestinationConfigurationTypeDef = ...,
+        ExtendedS3DestinationConfiguration: ExtendedS3DestinationConfigurationTypeDef = ...,
+        RedshiftDestinationConfiguration: RedshiftDestinationConfigurationTypeDef = ...,
+        ElasticsearchDestinationConfiguration: ElasticsearchDestinationConfigurationTypeDef = ...,
+        AmazonopensearchserviceDestinationConfiguration: AmazonopensearchserviceDestinationConfigurationTypeDef = ...,
+        SplunkDestinationConfiguration: SplunkDestinationConfigurationTypeDef = ...,
+        HttpEndpointDestinationConfiguration: HttpEndpointDestinationConfigurationTypeDef = ...,
+        Tags: Sequence[TagTypeDef] = ...,
+        AmazonOpenSearchServerlessDestinationConfiguration: AmazonOpenSearchServerlessDestinationConfigurationTypeDef = ...
+    ) -> CreateDeliveryStreamOutputTypeDef:
+        """
+        Creates a Kinesis Data Firehose delivery stream.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose.Client.create_delivery_stream)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/client/#create_delivery_stream)
+        """
+
+    async def delete_delivery_stream(
+        self, *, DeliveryStreamName: str, AllowForceDelete: bool = ...
+    ) -> Dict[str, Any]:
+        """
+        Deletes a delivery stream and its data.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose.Client.delete_delivery_stream)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/client/#delete_delivery_stream)
+        """
+
+    async def describe_delivery_stream(
+        self, *, DeliveryStreamName: str, Limit: int = ..., ExclusiveStartDestinationId: str = ...
+    ) -> DescribeDeliveryStreamOutputTypeDef:
+        """
+        Describes the specified delivery stream and its status.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose.Client.describe_delivery_stream)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/client/#describe_delivery_stream)
+        """
+
+    async def generate_presigned_url(
+        self,
+        ClientMethod: str,
+        Params: Mapping[str, Any] = ...,
+        ExpiresIn: int = 3600,
+        HttpMethod: str = ...,
+    ) -> str:
+        """
+        Generate a presigned url given a client, its method, and arguments.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose.Client.generate_presigned_url)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/client/#generate_presigned_url)
+        """
+
+    async def list_delivery_streams(
+        self,
+        *,
+        Limit: int = ...,
+        DeliveryStreamType: DeliveryStreamTypeType = ...,
+        ExclusiveStartDeliveryStreamName: str = ...
+    ) -> ListDeliveryStreamsOutputTypeDef:
+        """
+        Lists your delivery streams in alphabetical order of their names.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose.Client.list_delivery_streams)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/client/#list_delivery_streams)
+        """
+
+    async def list_tags_for_delivery_stream(
+        self, *, DeliveryStreamName: str, ExclusiveStartTagKey: str = ..., Limit: int = ...
+    ) -> ListTagsForDeliveryStreamOutputTypeDef:
+        """
+        Lists the tags for the specified delivery stream.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose.Client.list_tags_for_delivery_stream)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/client/#list_tags_for_delivery_stream)
+        """
+
+    async def put_record(
+        self, *, DeliveryStreamName: str, Record: RecordTypeDef
+    ) -> PutRecordOutputTypeDef:
+        """
+        Writes a single data record into an Amazon Kinesis Data Firehose delivery
+        stream.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose.Client.put_record)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/client/#put_record)
+        """
+
+    async def put_record_batch(
+        self, *, DeliveryStreamName: str, Records: Sequence[RecordTypeDef]
+    ) -> PutRecordBatchOutputTypeDef:
+        """
+        Writes multiple data records into a delivery stream in a single call, which can
+        achieve higher throughput per producer than when writing single records.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose.Client.put_record_batch)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/client/#put_record_batch)
+        """
+
+    async def start_delivery_stream_encryption(
+        self,
+        *,
+        DeliveryStreamName: str,
+        DeliveryStreamEncryptionConfigurationInput: DeliveryStreamEncryptionConfigurationInputTypeDef = ...
+    ) -> Dict[str, Any]:
+        """
+        Enables server-side encryption (SSE) for the delivery stream.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose.Client.start_delivery_stream_encryption)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/client/#start_delivery_stream_encryption)
+        """
+
+    async def stop_delivery_stream_encryption(self, *, DeliveryStreamName: str) -> Dict[str, Any]:
+        """
+        Disables server-side encryption (SSE) for the delivery stream.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose.Client.stop_delivery_stream_encryption)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/client/#stop_delivery_stream_encryption)
+        """
+
+    async def tag_delivery_stream(
+        self, *, DeliveryStreamName: str, Tags: Sequence[TagTypeDef]
+    ) -> Dict[str, Any]:
+        """
+        Adds or updates tags for the specified delivery stream.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose.Client.tag_delivery_stream)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/client/#tag_delivery_stream)
+        """
+
+    async def untag_delivery_stream(
+        self, *, DeliveryStreamName: str, TagKeys: Sequence[str]
+    ) -> Dict[str, Any]:
+        """
+        Removes tags from the specified delivery stream.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose.Client.untag_delivery_stream)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/client/#untag_delivery_stream)
+        """
+
+    async def update_destination(
+        self,
+        *,
+        DeliveryStreamName: str,
+        CurrentDeliveryStreamVersionId: str,
+        DestinationId: str,
+        S3DestinationUpdate: S3DestinationUpdateTypeDef = ...,
+        ExtendedS3DestinationUpdate: ExtendedS3DestinationUpdateTypeDef = ...,
+        RedshiftDestinationUpdate: RedshiftDestinationUpdateTypeDef = ...,
+        ElasticsearchDestinationUpdate: ElasticsearchDestinationUpdateTypeDef = ...,
+        AmazonopensearchserviceDestinationUpdate: AmazonopensearchserviceDestinationUpdateTypeDef = ...,
+        SplunkDestinationUpdate: SplunkDestinationUpdateTypeDef = ...,
+        HttpEndpointDestinationUpdate: HttpEndpointDestinationUpdateTypeDef = ...,
+        AmazonOpenSearchServerlessDestinationUpdate: AmazonOpenSearchServerlessDestinationUpdateTypeDef = ...
+    ) -> Dict[str, Any]:
+        """
+        Updates the specified destination of the specified delivery stream.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose.Client.update_destination)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/client/#update_destination)
+        """
+
+    async def __aenter__(self) -> "FirehoseClient":
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose.Client)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/client/)
+        """
+
+    async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose.Client)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/client/)
+        """
```

### Comparing `types-aiobotocore-firehose-2.5.2.post1/setup.py` & `types-aiobotocore-firehose-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-firehose",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_firehose"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Firehose 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-firehose-2.5.2.post1/types_aiobotocore_firehose/__main__.py` & `types-aiobotocore-firehose-2.5.2.post2/types_aiobotocore_firehose/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Firehose 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.Firehose 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose\nOther"
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

### Comparing `types-aiobotocore-firehose-2.5.2.post1/types_aiobotocore_firehose/client.py` & `types-aiobotocore-firehose-2.5.2.post2/types_aiobotocore_firehose/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -47,34 +47,31 @@
     SplunkDestinationConfigurationTypeDef,
     SplunkDestinationUpdateTypeDef,
     TagTypeDef,
 )
 
 __all__ = ("FirehoseClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     ConcurrentModificationException: Type[BotocoreClientError]
     InvalidArgumentException: Type[BotocoreClientError]
     InvalidKMSResourceException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     ResourceInUseException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceUnavailableException: Type[BotocoreClientError]
 
-
 class FirehoseClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/client/)
     """
 
     meta: ClientMeta
@@ -83,31 +80,28 @@
     def exceptions(self) -> Exceptions:
         """
         FirehoseClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/client/#exceptions)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/client/#can_paginate)
         """
-
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/client/#close)
         """
-
     async def create_delivery_stream(
         self,
         *,
         DeliveryStreamName: str,
         DeliveryStreamType: DeliveryStreamTypeType = ...,
         KinesisStreamSourceConfiguration: KinesisStreamSourceConfigurationTypeDef = ...,
         DeliveryStreamEncryptionConfigurationInput: DeliveryStreamEncryptionConfigurationInputTypeDef = ...,
@@ -123,136 +117,124 @@
     ) -> CreateDeliveryStreamOutputTypeDef:
         """
         Creates a Kinesis Data Firehose delivery stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose.Client.create_delivery_stream)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/client/#create_delivery_stream)
         """
-
     async def delete_delivery_stream(
         self, *, DeliveryStreamName: str, AllowForceDelete: bool = ...
     ) -> Dict[str, Any]:
         """
         Deletes a delivery stream and its data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose.Client.delete_delivery_stream)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/client/#delete_delivery_stream)
         """
-
     async def describe_delivery_stream(
         self, *, DeliveryStreamName: str, Limit: int = ..., ExclusiveStartDestinationId: str = ...
     ) -> DescribeDeliveryStreamOutputTypeDef:
         """
         Describes the specified delivery stream and its status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose.Client.describe_delivery_stream)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/client/#describe_delivery_stream)
         """
-
     async def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/client/#generate_presigned_url)
         """
-
     async def list_delivery_streams(
         self,
         *,
         Limit: int = ...,
         DeliveryStreamType: DeliveryStreamTypeType = ...,
         ExclusiveStartDeliveryStreamName: str = ...
     ) -> ListDeliveryStreamsOutputTypeDef:
         """
         Lists your delivery streams in alphabetical order of their names.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose.Client.list_delivery_streams)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/client/#list_delivery_streams)
         """
-
     async def list_tags_for_delivery_stream(
         self, *, DeliveryStreamName: str, ExclusiveStartTagKey: str = ..., Limit: int = ...
     ) -> ListTagsForDeliveryStreamOutputTypeDef:
         """
         Lists the tags for the specified delivery stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose.Client.list_tags_for_delivery_stream)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/client/#list_tags_for_delivery_stream)
         """
-
     async def put_record(
         self, *, DeliveryStreamName: str, Record: RecordTypeDef
     ) -> PutRecordOutputTypeDef:
         """
         Writes a single data record into an Amazon Kinesis Data Firehose delivery
         stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose.Client.put_record)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/client/#put_record)
         """
-
     async def put_record_batch(
         self, *, DeliveryStreamName: str, Records: Sequence[RecordTypeDef]
     ) -> PutRecordBatchOutputTypeDef:
         """
         Writes multiple data records into a delivery stream in a single call, which can
         achieve higher throughput per producer than when writing single records.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose.Client.put_record_batch)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/client/#put_record_batch)
         """
-
     async def start_delivery_stream_encryption(
         self,
         *,
         DeliveryStreamName: str,
         DeliveryStreamEncryptionConfigurationInput: DeliveryStreamEncryptionConfigurationInputTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Enables server-side encryption (SSE) for the delivery stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose.Client.start_delivery_stream_encryption)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/client/#start_delivery_stream_encryption)
         """
-
     async def stop_delivery_stream_encryption(self, *, DeliveryStreamName: str) -> Dict[str, Any]:
         """
         Disables server-side encryption (SSE) for the delivery stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose.Client.stop_delivery_stream_encryption)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/client/#stop_delivery_stream_encryption)
         """
-
     async def tag_delivery_stream(
         self, *, DeliveryStreamName: str, Tags: Sequence[TagTypeDef]
     ) -> Dict[str, Any]:
         """
         Adds or updates tags for the specified delivery stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose.Client.tag_delivery_stream)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/client/#tag_delivery_stream)
         """
-
     async def untag_delivery_stream(
         self, *, DeliveryStreamName: str, TagKeys: Sequence[str]
     ) -> Dict[str, Any]:
         """
         Removes tags from the specified delivery stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose.Client.untag_delivery_stream)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/client/#untag_delivery_stream)
         """
-
     async def update_destination(
         self,
         *,
         DeliveryStreamName: str,
         CurrentDeliveryStreamVersionId: str,
         DestinationId: str,
         S3DestinationUpdate: S3DestinationUpdateTypeDef = ...,
@@ -266,19 +248,17 @@
     ) -> Dict[str, Any]:
         """
         Updates the specified destination of the specified delivery stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose.Client.update_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/client/#update_destination)
         """
-
     async def __aenter__(self) -> "FirehoseClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/client/)
         """
-
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_firehose/client/)
         """
```

### Comparing `types-aiobotocore-firehose-2.5.2.post1/types_aiobotocore_firehose/literals.py` & `types-aiobotocore-firehose-2.5.2.post2/types_aiobotocore_firehose/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-firehose-2.5.2.post1/types_aiobotocore_firehose/literals.pyi` & `types-aiobotocore-firehose-2.5.2.post2/types_aiobotocore_firehose/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-firehose-2.5.2.post1/types_aiobotocore_firehose/type_defs.py` & `types-aiobotocore-firehose-2.5.2.post2/types_aiobotocore_firehose/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,31 +68,28 @@
     "KinesisStreamSourceConfigurationTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "SchemaConfigurationTypeDef",
     "DeleteDeliveryStreamInputRequestTypeDef",
     "FailureDescriptionTypeDef",
     "DescribeDeliveryStreamInputRequestTypeDef",
-    "HiveJsonSerDeOutputTypeDef",
-    "OpenXJsonSerDeOutputTypeDef",
     "HiveJsonSerDeTypeDef",
     "OpenXJsonSerDeTypeDef",
     "RetryOptionsTypeDef",
     "ElasticsearchBufferingHintsTypeDef",
     "ElasticsearchRetryOptionsTypeDef",
     "KMSEncryptionConfigTypeDef",
     "HttpEndpointBufferingHintsTypeDef",
     "HttpEndpointCommonAttributeTypeDef",
     "HttpEndpointConfigurationTypeDef",
     "HttpEndpointDescriptionTypeDef",
     "HttpEndpointRetryOptionsTypeDef",
     "KinesisStreamSourceDescriptionTypeDef",
     "ListDeliveryStreamsInputRequestTypeDef",
     "ListTagsForDeliveryStreamInputRequestTypeDef",
-    "OrcSerDeOutputTypeDef",
     "OrcSerDeTypeDef",
     "ParquetSerDeTypeDef",
     "ProcessorParameterTypeDef",
     "PutRecordBatchResponseEntryTypeDef",
     "RedshiftRetryOptionsTypeDef",
     "SplunkRetryOptionsTypeDef",
     "StopDeliveryStreamEncryptionInputRequestTypeDef",
@@ -101,62 +98,54 @@
     "StartDeliveryStreamEncryptionInputRequestTypeDef",
     "TagDeliveryStreamInputRequestTypeDef",
     "CreateDeliveryStreamOutputTypeDef",
     "ListDeliveryStreamsOutputTypeDef",
     "ListTagsForDeliveryStreamOutputTypeDef",
     "PutRecordOutputTypeDef",
     "DeliveryStreamEncryptionConfigurationTypeDef",
-    "DeserializerOutputTypeDef",
     "DeserializerTypeDef",
     "DynamicPartitioningConfigurationTypeDef",
     "EncryptionConfigurationTypeDef",
-    "HttpEndpointRequestConfigurationOutputTypeDef",
     "HttpEndpointRequestConfigurationTypeDef",
     "SourceDescriptionTypeDef",
-    "SerializerOutputTypeDef",
     "SerializerTypeDef",
-    "ProcessorOutputTypeDef",
     "ProcessorTypeDef",
     "PutRecordBatchOutputTypeDef",
     "PutRecordBatchInputRequestTypeDef",
     "PutRecordInputRequestTypeDef",
-    "InputFormatConfigurationOutputTypeDef",
     "InputFormatConfigurationTypeDef",
     "S3DestinationConfigurationTypeDef",
     "S3DestinationDescriptionTypeDef",
     "S3DestinationUpdateTypeDef",
-    "OutputFormatConfigurationOutputTypeDef",
     "OutputFormatConfigurationTypeDef",
-    "ProcessingConfigurationOutputTypeDef",
     "ProcessingConfigurationTypeDef",
-    "DataFormatConversionConfigurationOutputTypeDef",
     "DataFormatConversionConfigurationTypeDef",
-    "AmazonOpenSearchServerlessDestinationDescriptionTypeDef",
-    "AmazonopensearchserviceDestinationDescriptionTypeDef",
-    "ElasticsearchDestinationDescriptionTypeDef",
-    "HttpEndpointDestinationDescriptionTypeDef",
-    "RedshiftDestinationDescriptionTypeDef",
-    "SplunkDestinationDescriptionTypeDef",
     "AmazonOpenSearchServerlessDestinationConfigurationTypeDef",
+    "AmazonOpenSearchServerlessDestinationDescriptionTypeDef",
     "AmazonOpenSearchServerlessDestinationUpdateTypeDef",
     "AmazonopensearchserviceDestinationConfigurationTypeDef",
+    "AmazonopensearchserviceDestinationDescriptionTypeDef",
     "AmazonopensearchserviceDestinationUpdateTypeDef",
     "ElasticsearchDestinationConfigurationTypeDef",
+    "ElasticsearchDestinationDescriptionTypeDef",
     "ElasticsearchDestinationUpdateTypeDef",
     "HttpEndpointDestinationConfigurationTypeDef",
+    "HttpEndpointDestinationDescriptionTypeDef",
     "HttpEndpointDestinationUpdateTypeDef",
     "RedshiftDestinationConfigurationTypeDef",
+    "RedshiftDestinationDescriptionTypeDef",
     "RedshiftDestinationUpdateTypeDef",
     "SplunkDestinationConfigurationTypeDef",
+    "SplunkDestinationDescriptionTypeDef",
     "SplunkDestinationUpdateTypeDef",
-    "ExtendedS3DestinationDescriptionTypeDef",
     "ExtendedS3DestinationConfigurationTypeDef",
+    "ExtendedS3DestinationDescriptionTypeDef",
     "ExtendedS3DestinationUpdateTypeDef",
-    "DestinationDescriptionTypeDef",
     "CreateDeliveryStreamInputRequestTypeDef",
+    "DestinationDescriptionTypeDef",
     "UpdateDestinationInputRequestTypeDef",
     "DeliveryStreamDescriptionTypeDef",
     "DescribeDeliveryStreamOutputTypeDef",
 )
 
 AmazonOpenSearchServerlessBufferingHintsTypeDef = TypedDict(
     "AmazonOpenSearchServerlessBufferingHintsTypeDef",
@@ -373,32 +362,14 @@
 class DescribeDeliveryStreamInputRequestTypeDef(
     _RequiredDescribeDeliveryStreamInputRequestTypeDef,
     _OptionalDescribeDeliveryStreamInputRequestTypeDef,
 ):
     pass
 
 
-HiveJsonSerDeOutputTypeDef = TypedDict(
-    "HiveJsonSerDeOutputTypeDef",
-    {
-        "TimestampFormats": List[str],
-    },
-    total=False,
-)
-
-OpenXJsonSerDeOutputTypeDef = TypedDict(
-    "OpenXJsonSerDeOutputTypeDef",
-    {
-        "ConvertDotsInJsonKeysToUnderscores": bool,
-        "CaseInsensitive": bool,
-        "ColumnToJsonKeyMappings": Dict[str, str],
-    },
-    total=False,
-)
-
 HiveJsonSerDeTypeDef = TypedDict(
     "HiveJsonSerDeTypeDef",
     {
         "TimestampFormats": Sequence[str],
     },
     total=False,
 )
@@ -540,31 +511,14 @@
 class ListTagsForDeliveryStreamInputRequestTypeDef(
     _RequiredListTagsForDeliveryStreamInputRequestTypeDef,
     _OptionalListTagsForDeliveryStreamInputRequestTypeDef,
 ):
     pass
 
 
-OrcSerDeOutputTypeDef = TypedDict(
-    "OrcSerDeOutputTypeDef",
-    {
-        "StripeSizeBytes": int,
-        "BlockSizeBytes": int,
-        "RowIndexStride": int,
-        "EnablePadding": bool,
-        "PaddingTolerance": float,
-        "Compression": OrcCompressionType,
-        "BloomFilterColumns": List[str],
-        "BloomFilterFalsePositiveProbability": float,
-        "DictionaryKeyThreshold": float,
-        "FormatVersion": OrcFormatVersionType,
-    },
-    total=False,
-)
-
 OrcSerDeTypeDef = TypedDict(
     "OrcSerDeTypeDef",
     {
         "StripeSizeBytes": int,
         "BlockSizeBytes": int,
         "RowIndexStride": int,
         "EnablePadding": bool,
@@ -721,23 +675,14 @@
         "KeyType": KeyTypeType,
         "Status": DeliveryStreamEncryptionStatusType,
         "FailureDescription": FailureDescriptionTypeDef,
     },
     total=False,
 )
 
-DeserializerOutputTypeDef = TypedDict(
-    "DeserializerOutputTypeDef",
-    {
-        "OpenXJsonSerDe": OpenXJsonSerDeOutputTypeDef,
-        "HiveJsonSerDe": HiveJsonSerDeOutputTypeDef,
-    },
-    total=False,
-)
-
 DeserializerTypeDef = TypedDict(
     "DeserializerTypeDef",
     {
         "OpenXJsonSerDe": OpenXJsonSerDeTypeDef,
         "HiveJsonSerDe": HiveJsonSerDeTypeDef,
     },
     total=False,
@@ -757,23 +702,14 @@
     {
         "NoEncryptionConfig": Literal["NoEncryption"],
         "KMSEncryptionConfig": KMSEncryptionConfigTypeDef,
     },
     total=False,
 )
 
-HttpEndpointRequestConfigurationOutputTypeDef = TypedDict(
-    "HttpEndpointRequestConfigurationOutputTypeDef",
-    {
-        "ContentEncoding": ContentEncodingType,
-        "CommonAttributes": List[HttpEndpointCommonAttributeTypeDef],
-    },
-    total=False,
-)
-
 HttpEndpointRequestConfigurationTypeDef = TypedDict(
     "HttpEndpointRequestConfigurationTypeDef",
     {
         "ContentEncoding": ContentEncodingType,
         "CommonAttributes": Sequence[HttpEndpointCommonAttributeTypeDef],
     },
     total=False,
@@ -783,51 +719,23 @@
     "SourceDescriptionTypeDef",
     {
         "KinesisStreamSourceDescription": KinesisStreamSourceDescriptionTypeDef,
     },
     total=False,
 )
 
-SerializerOutputTypeDef = TypedDict(
-    "SerializerOutputTypeDef",
-    {
-        "ParquetSerDe": ParquetSerDeTypeDef,
-        "OrcSerDe": OrcSerDeOutputTypeDef,
-    },
-    total=False,
-)
-
 SerializerTypeDef = TypedDict(
     "SerializerTypeDef",
     {
         "ParquetSerDe": ParquetSerDeTypeDef,
         "OrcSerDe": OrcSerDeTypeDef,
     },
     total=False,
 )
 
-_RequiredProcessorOutputTypeDef = TypedDict(
-    "_RequiredProcessorOutputTypeDef",
-    {
-        "Type": ProcessorTypeType,
-    },
-)
-_OptionalProcessorOutputTypeDef = TypedDict(
-    "_OptionalProcessorOutputTypeDef",
-    {
-        "Parameters": List[ProcessorParameterTypeDef],
-    },
-    total=False,
-)
-
-
-class ProcessorOutputTypeDef(_RequiredProcessorOutputTypeDef, _OptionalProcessorOutputTypeDef):
-    pass
-
-
 _RequiredProcessorTypeDef = TypedDict(
     "_RequiredProcessorTypeDef",
     {
         "Type": ProcessorTypeType,
     },
 )
 _OptionalProcessorTypeDef = TypedDict(
@@ -865,22 +773,14 @@
     "PutRecordInputRequestTypeDef",
     {
         "DeliveryStreamName": str,
         "Record": RecordTypeDef,
     },
 )
 
-InputFormatConfigurationOutputTypeDef = TypedDict(
-    "InputFormatConfigurationOutputTypeDef",
-    {
-        "Deserializer": DeserializerOutputTypeDef,
-    },
-    total=False,
-)
-
 InputFormatConfigurationTypeDef = TypedDict(
     "InputFormatConfigurationTypeDef",
     {
         "Deserializer": DeserializerTypeDef,
     },
     total=False,
 )
@@ -950,188 +850,42 @@
         "CompressionFormat": CompressionFormatType,
         "EncryptionConfiguration": EncryptionConfigurationTypeDef,
         "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
     },
     total=False,
 )
 
-OutputFormatConfigurationOutputTypeDef = TypedDict(
-    "OutputFormatConfigurationOutputTypeDef",
-    {
-        "Serializer": SerializerOutputTypeDef,
-    },
-    total=False,
-)
-
 OutputFormatConfigurationTypeDef = TypedDict(
     "OutputFormatConfigurationTypeDef",
     {
         "Serializer": SerializerTypeDef,
     },
     total=False,
 )
 
-ProcessingConfigurationOutputTypeDef = TypedDict(
-    "ProcessingConfigurationOutputTypeDef",
-    {
-        "Enabled": bool,
-        "Processors": List[ProcessorOutputTypeDef],
-    },
-    total=False,
-)
-
 ProcessingConfigurationTypeDef = TypedDict(
     "ProcessingConfigurationTypeDef",
     {
         "Enabled": bool,
         "Processors": Sequence[ProcessorTypeDef],
     },
     total=False,
 )
 
-DataFormatConversionConfigurationOutputTypeDef = TypedDict(
-    "DataFormatConversionConfigurationOutputTypeDef",
-    {
-        "SchemaConfiguration": SchemaConfigurationTypeDef,
-        "InputFormatConfiguration": InputFormatConfigurationOutputTypeDef,
-        "OutputFormatConfiguration": OutputFormatConfigurationOutputTypeDef,
-        "Enabled": bool,
-    },
-    total=False,
-)
-
 DataFormatConversionConfigurationTypeDef = TypedDict(
     "DataFormatConversionConfigurationTypeDef",
     {
         "SchemaConfiguration": SchemaConfigurationTypeDef,
         "InputFormatConfiguration": InputFormatConfigurationTypeDef,
         "OutputFormatConfiguration": OutputFormatConfigurationTypeDef,
         "Enabled": bool,
     },
     total=False,
 )
 
-AmazonOpenSearchServerlessDestinationDescriptionTypeDef = TypedDict(
-    "AmazonOpenSearchServerlessDestinationDescriptionTypeDef",
-    {
-        "RoleARN": str,
-        "CollectionEndpoint": str,
-        "IndexName": str,
-        "BufferingHints": AmazonOpenSearchServerlessBufferingHintsTypeDef,
-        "RetryOptions": AmazonOpenSearchServerlessRetryOptionsTypeDef,
-        "S3BackupMode": AmazonOpenSearchServerlessS3BackupModeType,
-        "S3DestinationDescription": S3DestinationDescriptionTypeDef,
-        "ProcessingConfiguration": ProcessingConfigurationOutputTypeDef,
-        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
-        "VpcConfigurationDescription": VpcConfigurationDescriptionTypeDef,
-    },
-    total=False,
-)
-
-AmazonopensearchserviceDestinationDescriptionTypeDef = TypedDict(
-    "AmazonopensearchserviceDestinationDescriptionTypeDef",
-    {
-        "RoleARN": str,
-        "DomainARN": str,
-        "ClusterEndpoint": str,
-        "IndexName": str,
-        "TypeName": str,
-        "IndexRotationPeriod": AmazonopensearchserviceIndexRotationPeriodType,
-        "BufferingHints": AmazonopensearchserviceBufferingHintsTypeDef,
-        "RetryOptions": AmazonopensearchserviceRetryOptionsTypeDef,
-        "S3BackupMode": AmazonopensearchserviceS3BackupModeType,
-        "S3DestinationDescription": S3DestinationDescriptionTypeDef,
-        "ProcessingConfiguration": ProcessingConfigurationOutputTypeDef,
-        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
-        "VpcConfigurationDescription": VpcConfigurationDescriptionTypeDef,
-    },
-    total=False,
-)
-
-ElasticsearchDestinationDescriptionTypeDef = TypedDict(
-    "ElasticsearchDestinationDescriptionTypeDef",
-    {
-        "RoleARN": str,
-        "DomainARN": str,
-        "ClusterEndpoint": str,
-        "IndexName": str,
-        "TypeName": str,
-        "IndexRotationPeriod": ElasticsearchIndexRotationPeriodType,
-        "BufferingHints": ElasticsearchBufferingHintsTypeDef,
-        "RetryOptions": ElasticsearchRetryOptionsTypeDef,
-        "S3BackupMode": ElasticsearchS3BackupModeType,
-        "S3DestinationDescription": S3DestinationDescriptionTypeDef,
-        "ProcessingConfiguration": ProcessingConfigurationOutputTypeDef,
-        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
-        "VpcConfigurationDescription": VpcConfigurationDescriptionTypeDef,
-    },
-    total=False,
-)
-
-HttpEndpointDestinationDescriptionTypeDef = TypedDict(
-    "HttpEndpointDestinationDescriptionTypeDef",
-    {
-        "EndpointConfiguration": HttpEndpointDescriptionTypeDef,
-        "BufferingHints": HttpEndpointBufferingHintsTypeDef,
-        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
-        "RequestConfiguration": HttpEndpointRequestConfigurationOutputTypeDef,
-        "ProcessingConfiguration": ProcessingConfigurationOutputTypeDef,
-        "RoleARN": str,
-        "RetryOptions": HttpEndpointRetryOptionsTypeDef,
-        "S3BackupMode": HttpEndpointS3BackupModeType,
-        "S3DestinationDescription": S3DestinationDescriptionTypeDef,
-    },
-    total=False,
-)
-
-_RequiredRedshiftDestinationDescriptionTypeDef = TypedDict(
-    "_RequiredRedshiftDestinationDescriptionTypeDef",
-    {
-        "RoleARN": str,
-        "ClusterJDBCURL": str,
-        "CopyCommand": CopyCommandTypeDef,
-        "Username": str,
-        "S3DestinationDescription": S3DestinationDescriptionTypeDef,
-    },
-)
-_OptionalRedshiftDestinationDescriptionTypeDef = TypedDict(
-    "_OptionalRedshiftDestinationDescriptionTypeDef",
-    {
-        "RetryOptions": RedshiftRetryOptionsTypeDef,
-        "ProcessingConfiguration": ProcessingConfigurationOutputTypeDef,
-        "S3BackupMode": RedshiftS3BackupModeType,
-        "S3BackupDescription": S3DestinationDescriptionTypeDef,
-        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
-    },
-    total=False,
-)
-
-
-class RedshiftDestinationDescriptionTypeDef(
-    _RequiredRedshiftDestinationDescriptionTypeDef, _OptionalRedshiftDestinationDescriptionTypeDef
-):
-    pass
-
-
-SplunkDestinationDescriptionTypeDef = TypedDict(
-    "SplunkDestinationDescriptionTypeDef",
-    {
-        "HECEndpoint": str,
-        "HECEndpointType": HECEndpointTypeType,
-        "HECToken": str,
-        "HECAcknowledgmentTimeoutInSeconds": int,
-        "RetryOptions": SplunkRetryOptionsTypeDef,
-        "S3BackupMode": SplunkS3BackupModeType,
-        "S3DestinationDescription": S3DestinationDescriptionTypeDef,
-        "ProcessingConfiguration": ProcessingConfigurationOutputTypeDef,
-        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
-    },
-    total=False,
-)
-
 _RequiredAmazonOpenSearchServerlessDestinationConfigurationTypeDef = TypedDict(
     "_RequiredAmazonOpenSearchServerlessDestinationConfigurationTypeDef",
     {
         "RoleARN": str,
         "IndexName": str,
         "S3Configuration": S3DestinationConfigurationTypeDef,
     },
@@ -1154,14 +908,31 @@
 class AmazonOpenSearchServerlessDestinationConfigurationTypeDef(
     _RequiredAmazonOpenSearchServerlessDestinationConfigurationTypeDef,
     _OptionalAmazonOpenSearchServerlessDestinationConfigurationTypeDef,
 ):
     pass
 
 
+AmazonOpenSearchServerlessDestinationDescriptionTypeDef = TypedDict(
+    "AmazonOpenSearchServerlessDestinationDescriptionTypeDef",
+    {
+        "RoleARN": str,
+        "CollectionEndpoint": str,
+        "IndexName": str,
+        "BufferingHints": AmazonOpenSearchServerlessBufferingHintsTypeDef,
+        "RetryOptions": AmazonOpenSearchServerlessRetryOptionsTypeDef,
+        "S3BackupMode": AmazonOpenSearchServerlessS3BackupModeType,
+        "S3DestinationDescription": S3DestinationDescriptionTypeDef,
+        "ProcessingConfiguration": ProcessingConfigurationTypeDef,
+        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
+        "VpcConfigurationDescription": VpcConfigurationDescriptionTypeDef,
+    },
+    total=False,
+)
+
 AmazonOpenSearchServerlessDestinationUpdateTypeDef = TypedDict(
     "AmazonOpenSearchServerlessDestinationUpdateTypeDef",
     {
         "RoleARN": str,
         "CollectionEndpoint": str,
         "IndexName": str,
         "BufferingHints": AmazonOpenSearchServerlessBufferingHintsTypeDef,
@@ -1202,14 +973,34 @@
 class AmazonopensearchserviceDestinationConfigurationTypeDef(
     _RequiredAmazonopensearchserviceDestinationConfigurationTypeDef,
     _OptionalAmazonopensearchserviceDestinationConfigurationTypeDef,
 ):
     pass
 
 
+AmazonopensearchserviceDestinationDescriptionTypeDef = TypedDict(
+    "AmazonopensearchserviceDestinationDescriptionTypeDef",
+    {
+        "RoleARN": str,
+        "DomainARN": str,
+        "ClusterEndpoint": str,
+        "IndexName": str,
+        "TypeName": str,
+        "IndexRotationPeriod": AmazonopensearchserviceIndexRotationPeriodType,
+        "BufferingHints": AmazonopensearchserviceBufferingHintsTypeDef,
+        "RetryOptions": AmazonopensearchserviceRetryOptionsTypeDef,
+        "S3BackupMode": AmazonopensearchserviceS3BackupModeType,
+        "S3DestinationDescription": S3DestinationDescriptionTypeDef,
+        "ProcessingConfiguration": ProcessingConfigurationTypeDef,
+        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
+        "VpcConfigurationDescription": VpcConfigurationDescriptionTypeDef,
+    },
+    total=False,
+)
+
 AmazonopensearchserviceDestinationUpdateTypeDef = TypedDict(
     "AmazonopensearchserviceDestinationUpdateTypeDef",
     {
         "RoleARN": str,
         "DomainARN": str,
         "ClusterEndpoint": str,
         "IndexName": str,
@@ -1253,14 +1044,34 @@
 class ElasticsearchDestinationConfigurationTypeDef(
     _RequiredElasticsearchDestinationConfigurationTypeDef,
     _OptionalElasticsearchDestinationConfigurationTypeDef,
 ):
     pass
 
 
+ElasticsearchDestinationDescriptionTypeDef = TypedDict(
+    "ElasticsearchDestinationDescriptionTypeDef",
+    {
+        "RoleARN": str,
+        "DomainARN": str,
+        "ClusterEndpoint": str,
+        "IndexName": str,
+        "TypeName": str,
+        "IndexRotationPeriod": ElasticsearchIndexRotationPeriodType,
+        "BufferingHints": ElasticsearchBufferingHintsTypeDef,
+        "RetryOptions": ElasticsearchRetryOptionsTypeDef,
+        "S3BackupMode": ElasticsearchS3BackupModeType,
+        "S3DestinationDescription": S3DestinationDescriptionTypeDef,
+        "ProcessingConfiguration": ProcessingConfigurationTypeDef,
+        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
+        "VpcConfigurationDescription": VpcConfigurationDescriptionTypeDef,
+    },
+    total=False,
+)
+
 ElasticsearchDestinationUpdateTypeDef = TypedDict(
     "ElasticsearchDestinationUpdateTypeDef",
     {
         "RoleARN": str,
         "DomainARN": str,
         "ClusterEndpoint": str,
         "IndexName": str,
@@ -1300,14 +1111,30 @@
 class HttpEndpointDestinationConfigurationTypeDef(
     _RequiredHttpEndpointDestinationConfigurationTypeDef,
     _OptionalHttpEndpointDestinationConfigurationTypeDef,
 ):
     pass
 
 
+HttpEndpointDestinationDescriptionTypeDef = TypedDict(
+    "HttpEndpointDestinationDescriptionTypeDef",
+    {
+        "EndpointConfiguration": HttpEndpointDescriptionTypeDef,
+        "BufferingHints": HttpEndpointBufferingHintsTypeDef,
+        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
+        "RequestConfiguration": HttpEndpointRequestConfigurationTypeDef,
+        "ProcessingConfiguration": ProcessingConfigurationTypeDef,
+        "RoleARN": str,
+        "RetryOptions": HttpEndpointRetryOptionsTypeDef,
+        "S3BackupMode": HttpEndpointS3BackupModeType,
+        "S3DestinationDescription": S3DestinationDescriptionTypeDef,
+    },
+    total=False,
+)
+
 HttpEndpointDestinationUpdateTypeDef = TypedDict(
     "HttpEndpointDestinationUpdateTypeDef",
     {
         "EndpointConfiguration": HttpEndpointConfigurationTypeDef,
         "BufferingHints": HttpEndpointBufferingHintsTypeDef,
         "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
         "RequestConfiguration": HttpEndpointRequestConfigurationTypeDef,
@@ -1347,14 +1174,43 @@
 class RedshiftDestinationConfigurationTypeDef(
     _RequiredRedshiftDestinationConfigurationTypeDef,
     _OptionalRedshiftDestinationConfigurationTypeDef,
 ):
     pass
 
 
+_RequiredRedshiftDestinationDescriptionTypeDef = TypedDict(
+    "_RequiredRedshiftDestinationDescriptionTypeDef",
+    {
+        "RoleARN": str,
+        "ClusterJDBCURL": str,
+        "CopyCommand": CopyCommandTypeDef,
+        "Username": str,
+        "S3DestinationDescription": S3DestinationDescriptionTypeDef,
+    },
+)
+_OptionalRedshiftDestinationDescriptionTypeDef = TypedDict(
+    "_OptionalRedshiftDestinationDescriptionTypeDef",
+    {
+        "RetryOptions": RedshiftRetryOptionsTypeDef,
+        "ProcessingConfiguration": ProcessingConfigurationTypeDef,
+        "S3BackupMode": RedshiftS3BackupModeType,
+        "S3BackupDescription": S3DestinationDescriptionTypeDef,
+        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
+    },
+    total=False,
+)
+
+
+class RedshiftDestinationDescriptionTypeDef(
+    _RequiredRedshiftDestinationDescriptionTypeDef, _OptionalRedshiftDestinationDescriptionTypeDef
+):
+    pass
+
+
 RedshiftDestinationUpdateTypeDef = TypedDict(
     "RedshiftDestinationUpdateTypeDef",
     {
         "RoleARN": str,
         "ClusterJDBCURL": str,
         "CopyCommand": CopyCommandTypeDef,
         "Username": str,
@@ -1393,14 +1249,30 @@
 
 class SplunkDestinationConfigurationTypeDef(
     _RequiredSplunkDestinationConfigurationTypeDef, _OptionalSplunkDestinationConfigurationTypeDef
 ):
     pass
 
 
+SplunkDestinationDescriptionTypeDef = TypedDict(
+    "SplunkDestinationDescriptionTypeDef",
+    {
+        "HECEndpoint": str,
+        "HECEndpointType": HECEndpointTypeType,
+        "HECToken": str,
+        "HECAcknowledgmentTimeoutInSeconds": int,
+        "RetryOptions": SplunkRetryOptionsTypeDef,
+        "S3BackupMode": SplunkS3BackupModeType,
+        "S3DestinationDescription": S3DestinationDescriptionTypeDef,
+        "ProcessingConfiguration": ProcessingConfigurationTypeDef,
+        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
+    },
+    total=False,
+)
+
 SplunkDestinationUpdateTypeDef = TypedDict(
     "SplunkDestinationUpdateTypeDef",
     {
         "HECEndpoint": str,
         "HECEndpointType": HECEndpointTypeType,
         "HECToken": str,
         "HECAcknowledgmentTimeoutInSeconds": int,
@@ -1409,76 +1281,76 @@
         "S3Update": S3DestinationUpdateTypeDef,
         "ProcessingConfiguration": ProcessingConfigurationTypeDef,
         "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
     },
     total=False,
 )
 
-_RequiredExtendedS3DestinationDescriptionTypeDef = TypedDict(
-    "_RequiredExtendedS3DestinationDescriptionTypeDef",
+_RequiredExtendedS3DestinationConfigurationTypeDef = TypedDict(
+    "_RequiredExtendedS3DestinationConfigurationTypeDef",
     {
         "RoleARN": str,
         "BucketARN": str,
-        "BufferingHints": BufferingHintsTypeDef,
-        "CompressionFormat": CompressionFormatType,
-        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
     },
 )
-_OptionalExtendedS3DestinationDescriptionTypeDef = TypedDict(
-    "_OptionalExtendedS3DestinationDescriptionTypeDef",
+_OptionalExtendedS3DestinationConfigurationTypeDef = TypedDict(
+    "_OptionalExtendedS3DestinationConfigurationTypeDef",
     {
         "Prefix": str,
         "ErrorOutputPrefix": str,
+        "BufferingHints": BufferingHintsTypeDef,
+        "CompressionFormat": CompressionFormatType,
+        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
         "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
-        "ProcessingConfiguration": ProcessingConfigurationOutputTypeDef,
+        "ProcessingConfiguration": ProcessingConfigurationTypeDef,
         "S3BackupMode": S3BackupModeType,
-        "S3BackupDescription": S3DestinationDescriptionTypeDef,
-        "DataFormatConversionConfiguration": DataFormatConversionConfigurationOutputTypeDef,
+        "S3BackupConfiguration": S3DestinationConfigurationTypeDef,
+        "DataFormatConversionConfiguration": DataFormatConversionConfigurationTypeDef,
         "DynamicPartitioningConfiguration": DynamicPartitioningConfigurationTypeDef,
     },
     total=False,
 )
 
 
-class ExtendedS3DestinationDescriptionTypeDef(
-    _RequiredExtendedS3DestinationDescriptionTypeDef,
-    _OptionalExtendedS3DestinationDescriptionTypeDef,
+class ExtendedS3DestinationConfigurationTypeDef(
+    _RequiredExtendedS3DestinationConfigurationTypeDef,
+    _OptionalExtendedS3DestinationConfigurationTypeDef,
 ):
     pass
 
 
-_RequiredExtendedS3DestinationConfigurationTypeDef = TypedDict(
-    "_RequiredExtendedS3DestinationConfigurationTypeDef",
+_RequiredExtendedS3DestinationDescriptionTypeDef = TypedDict(
+    "_RequiredExtendedS3DestinationDescriptionTypeDef",
     {
         "RoleARN": str,
         "BucketARN": str,
+        "BufferingHints": BufferingHintsTypeDef,
+        "CompressionFormat": CompressionFormatType,
+        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
     },
 )
-_OptionalExtendedS3DestinationConfigurationTypeDef = TypedDict(
-    "_OptionalExtendedS3DestinationConfigurationTypeDef",
+_OptionalExtendedS3DestinationDescriptionTypeDef = TypedDict(
+    "_OptionalExtendedS3DestinationDescriptionTypeDef",
     {
         "Prefix": str,
         "ErrorOutputPrefix": str,
-        "BufferingHints": BufferingHintsTypeDef,
-        "CompressionFormat": CompressionFormatType,
-        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
         "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
         "ProcessingConfiguration": ProcessingConfigurationTypeDef,
         "S3BackupMode": S3BackupModeType,
-        "S3BackupConfiguration": S3DestinationConfigurationTypeDef,
+        "S3BackupDescription": S3DestinationDescriptionTypeDef,
         "DataFormatConversionConfiguration": DataFormatConversionConfigurationTypeDef,
         "DynamicPartitioningConfiguration": DynamicPartitioningConfigurationTypeDef,
     },
     total=False,
 )
 
 
-class ExtendedS3DestinationConfigurationTypeDef(
-    _RequiredExtendedS3DestinationConfigurationTypeDef,
-    _OptionalExtendedS3DestinationConfigurationTypeDef,
+class ExtendedS3DestinationDescriptionTypeDef(
+    _RequiredExtendedS3DestinationDescriptionTypeDef,
+    _OptionalExtendedS3DestinationDescriptionTypeDef,
 ):
     pass
 
 
 ExtendedS3DestinationUpdateTypeDef = TypedDict(
     "ExtendedS3DestinationUpdateTypeDef",
     {
@@ -1495,46 +1367,14 @@
         "S3BackupUpdate": S3DestinationUpdateTypeDef,
         "DataFormatConversionConfiguration": DataFormatConversionConfigurationTypeDef,
         "DynamicPartitioningConfiguration": DynamicPartitioningConfigurationTypeDef,
     },
     total=False,
 )
 
-_RequiredDestinationDescriptionTypeDef = TypedDict(
-    "_RequiredDestinationDescriptionTypeDef",
-    {
-        "DestinationId": str,
-    },
-)
-_OptionalDestinationDescriptionTypeDef = TypedDict(
-    "_OptionalDestinationDescriptionTypeDef",
-    {
-        "S3DestinationDescription": S3DestinationDescriptionTypeDef,
-        "ExtendedS3DestinationDescription": ExtendedS3DestinationDescriptionTypeDef,
-        "RedshiftDestinationDescription": RedshiftDestinationDescriptionTypeDef,
-        "ElasticsearchDestinationDescription": ElasticsearchDestinationDescriptionTypeDef,
-        "AmazonopensearchserviceDestinationDescription": (
-            AmazonopensearchserviceDestinationDescriptionTypeDef
-        ),
-        "SplunkDestinationDescription": SplunkDestinationDescriptionTypeDef,
-        "HttpEndpointDestinationDescription": HttpEndpointDestinationDescriptionTypeDef,
-        "AmazonOpenSearchServerlessDestinationDescription": (
-            AmazonOpenSearchServerlessDestinationDescriptionTypeDef
-        ),
-    },
-    total=False,
-)
-
-
-class DestinationDescriptionTypeDef(
-    _RequiredDestinationDescriptionTypeDef, _OptionalDestinationDescriptionTypeDef
-):
-    pass
-
-
 _RequiredCreateDeliveryStreamInputRequestTypeDef = TypedDict(
     "_RequiredCreateDeliveryStreamInputRequestTypeDef",
     {
         "DeliveryStreamName": str,
     },
 )
 _OptionalCreateDeliveryStreamInputRequestTypeDef = TypedDict(
@@ -1566,14 +1406,46 @@
 class CreateDeliveryStreamInputRequestTypeDef(
     _RequiredCreateDeliveryStreamInputRequestTypeDef,
     _OptionalCreateDeliveryStreamInputRequestTypeDef,
 ):
     pass
 
 
+_RequiredDestinationDescriptionTypeDef = TypedDict(
+    "_RequiredDestinationDescriptionTypeDef",
+    {
+        "DestinationId": str,
+    },
+)
+_OptionalDestinationDescriptionTypeDef = TypedDict(
+    "_OptionalDestinationDescriptionTypeDef",
+    {
+        "S3DestinationDescription": S3DestinationDescriptionTypeDef,
+        "ExtendedS3DestinationDescription": ExtendedS3DestinationDescriptionTypeDef,
+        "RedshiftDestinationDescription": RedshiftDestinationDescriptionTypeDef,
+        "ElasticsearchDestinationDescription": ElasticsearchDestinationDescriptionTypeDef,
+        "AmazonopensearchserviceDestinationDescription": (
+            AmazonopensearchserviceDestinationDescriptionTypeDef
+        ),
+        "SplunkDestinationDescription": SplunkDestinationDescriptionTypeDef,
+        "HttpEndpointDestinationDescription": HttpEndpointDestinationDescriptionTypeDef,
+        "AmazonOpenSearchServerlessDestinationDescription": (
+            AmazonOpenSearchServerlessDestinationDescriptionTypeDef
+        ),
+    },
+    total=False,
+)
+
+
+class DestinationDescriptionTypeDef(
+    _RequiredDestinationDescriptionTypeDef, _OptionalDestinationDescriptionTypeDef
+):
+    pass
+
+
 _RequiredUpdateDestinationInputRequestTypeDef = TypedDict(
     "_RequiredUpdateDestinationInputRequestTypeDef",
     {
         "DeliveryStreamName": str,
         "CurrentDeliveryStreamVersionId": str,
         "DestinationId": str,
     },
```

### Comparing `types-aiobotocore-firehose-2.5.2.post1/types_aiobotocore_firehose/type_defs.pyi` & `types-aiobotocore-firehose-2.5.2.post2/types_aiobotocore_firehose/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -67,31 +67,28 @@
     "KinesisStreamSourceConfigurationTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "SchemaConfigurationTypeDef",
     "DeleteDeliveryStreamInputRequestTypeDef",
     "FailureDescriptionTypeDef",
     "DescribeDeliveryStreamInputRequestTypeDef",
-    "HiveJsonSerDeOutputTypeDef",
-    "OpenXJsonSerDeOutputTypeDef",
     "HiveJsonSerDeTypeDef",
     "OpenXJsonSerDeTypeDef",
     "RetryOptionsTypeDef",
     "ElasticsearchBufferingHintsTypeDef",
     "ElasticsearchRetryOptionsTypeDef",
     "KMSEncryptionConfigTypeDef",
     "HttpEndpointBufferingHintsTypeDef",
     "HttpEndpointCommonAttributeTypeDef",
     "HttpEndpointConfigurationTypeDef",
     "HttpEndpointDescriptionTypeDef",
     "HttpEndpointRetryOptionsTypeDef",
     "KinesisStreamSourceDescriptionTypeDef",
     "ListDeliveryStreamsInputRequestTypeDef",
     "ListTagsForDeliveryStreamInputRequestTypeDef",
-    "OrcSerDeOutputTypeDef",
     "OrcSerDeTypeDef",
     "ParquetSerDeTypeDef",
     "ProcessorParameterTypeDef",
     "PutRecordBatchResponseEntryTypeDef",
     "RedshiftRetryOptionsTypeDef",
     "SplunkRetryOptionsTypeDef",
     "StopDeliveryStreamEncryptionInputRequestTypeDef",
@@ -100,62 +97,54 @@
     "StartDeliveryStreamEncryptionInputRequestTypeDef",
     "TagDeliveryStreamInputRequestTypeDef",
     "CreateDeliveryStreamOutputTypeDef",
     "ListDeliveryStreamsOutputTypeDef",
     "ListTagsForDeliveryStreamOutputTypeDef",
     "PutRecordOutputTypeDef",
     "DeliveryStreamEncryptionConfigurationTypeDef",
-    "DeserializerOutputTypeDef",
     "DeserializerTypeDef",
     "DynamicPartitioningConfigurationTypeDef",
     "EncryptionConfigurationTypeDef",
-    "HttpEndpointRequestConfigurationOutputTypeDef",
     "HttpEndpointRequestConfigurationTypeDef",
     "SourceDescriptionTypeDef",
-    "SerializerOutputTypeDef",
     "SerializerTypeDef",
-    "ProcessorOutputTypeDef",
     "ProcessorTypeDef",
     "PutRecordBatchOutputTypeDef",
     "PutRecordBatchInputRequestTypeDef",
     "PutRecordInputRequestTypeDef",
-    "InputFormatConfigurationOutputTypeDef",
     "InputFormatConfigurationTypeDef",
     "S3DestinationConfigurationTypeDef",
     "S3DestinationDescriptionTypeDef",
     "S3DestinationUpdateTypeDef",
-    "OutputFormatConfigurationOutputTypeDef",
     "OutputFormatConfigurationTypeDef",
-    "ProcessingConfigurationOutputTypeDef",
     "ProcessingConfigurationTypeDef",
-    "DataFormatConversionConfigurationOutputTypeDef",
     "DataFormatConversionConfigurationTypeDef",
-    "AmazonOpenSearchServerlessDestinationDescriptionTypeDef",
-    "AmazonopensearchserviceDestinationDescriptionTypeDef",
-    "ElasticsearchDestinationDescriptionTypeDef",
-    "HttpEndpointDestinationDescriptionTypeDef",
-    "RedshiftDestinationDescriptionTypeDef",
-    "SplunkDestinationDescriptionTypeDef",
     "AmazonOpenSearchServerlessDestinationConfigurationTypeDef",
+    "AmazonOpenSearchServerlessDestinationDescriptionTypeDef",
     "AmazonOpenSearchServerlessDestinationUpdateTypeDef",
     "AmazonopensearchserviceDestinationConfigurationTypeDef",
+    "AmazonopensearchserviceDestinationDescriptionTypeDef",
     "AmazonopensearchserviceDestinationUpdateTypeDef",
     "ElasticsearchDestinationConfigurationTypeDef",
+    "ElasticsearchDestinationDescriptionTypeDef",
     "ElasticsearchDestinationUpdateTypeDef",
     "HttpEndpointDestinationConfigurationTypeDef",
+    "HttpEndpointDestinationDescriptionTypeDef",
     "HttpEndpointDestinationUpdateTypeDef",
     "RedshiftDestinationConfigurationTypeDef",
+    "RedshiftDestinationDescriptionTypeDef",
     "RedshiftDestinationUpdateTypeDef",
     "SplunkDestinationConfigurationTypeDef",
+    "SplunkDestinationDescriptionTypeDef",
     "SplunkDestinationUpdateTypeDef",
-    "ExtendedS3DestinationDescriptionTypeDef",
     "ExtendedS3DestinationConfigurationTypeDef",
+    "ExtendedS3DestinationDescriptionTypeDef",
     "ExtendedS3DestinationUpdateTypeDef",
-    "DestinationDescriptionTypeDef",
     "CreateDeliveryStreamInputRequestTypeDef",
+    "DestinationDescriptionTypeDef",
     "UpdateDestinationInputRequestTypeDef",
     "DeliveryStreamDescriptionTypeDef",
     "DescribeDeliveryStreamOutputTypeDef",
 )
 
 AmazonOpenSearchServerlessBufferingHintsTypeDef = TypedDict(
     "AmazonOpenSearchServerlessBufferingHintsTypeDef",
@@ -362,32 +351,14 @@
 
 class DescribeDeliveryStreamInputRequestTypeDef(
     _RequiredDescribeDeliveryStreamInputRequestTypeDef,
     _OptionalDescribeDeliveryStreamInputRequestTypeDef,
 ):
     pass
 
-HiveJsonSerDeOutputTypeDef = TypedDict(
-    "HiveJsonSerDeOutputTypeDef",
-    {
-        "TimestampFormats": List[str],
-    },
-    total=False,
-)
-
-OpenXJsonSerDeOutputTypeDef = TypedDict(
-    "OpenXJsonSerDeOutputTypeDef",
-    {
-        "ConvertDotsInJsonKeysToUnderscores": bool,
-        "CaseInsensitive": bool,
-        "ColumnToJsonKeyMappings": Dict[str, str],
-    },
-    total=False,
-)
-
 HiveJsonSerDeTypeDef = TypedDict(
     "HiveJsonSerDeTypeDef",
     {
         "TimestampFormats": Sequence[str],
     },
     total=False,
 )
@@ -525,31 +496,14 @@
 
 class ListTagsForDeliveryStreamInputRequestTypeDef(
     _RequiredListTagsForDeliveryStreamInputRequestTypeDef,
     _OptionalListTagsForDeliveryStreamInputRequestTypeDef,
 ):
     pass
 
-OrcSerDeOutputTypeDef = TypedDict(
-    "OrcSerDeOutputTypeDef",
-    {
-        "StripeSizeBytes": int,
-        "BlockSizeBytes": int,
-        "RowIndexStride": int,
-        "EnablePadding": bool,
-        "PaddingTolerance": float,
-        "Compression": OrcCompressionType,
-        "BloomFilterColumns": List[str],
-        "BloomFilterFalsePositiveProbability": float,
-        "DictionaryKeyThreshold": float,
-        "FormatVersion": OrcFormatVersionType,
-    },
-    total=False,
-)
-
 OrcSerDeTypeDef = TypedDict(
     "OrcSerDeTypeDef",
     {
         "StripeSizeBytes": int,
         "BlockSizeBytes": int,
         "RowIndexStride": int,
         "EnablePadding": bool,
@@ -704,23 +658,14 @@
         "KeyType": KeyTypeType,
         "Status": DeliveryStreamEncryptionStatusType,
         "FailureDescription": FailureDescriptionTypeDef,
     },
     total=False,
 )
 
-DeserializerOutputTypeDef = TypedDict(
-    "DeserializerOutputTypeDef",
-    {
-        "OpenXJsonSerDe": OpenXJsonSerDeOutputTypeDef,
-        "HiveJsonSerDe": HiveJsonSerDeOutputTypeDef,
-    },
-    total=False,
-)
-
 DeserializerTypeDef = TypedDict(
     "DeserializerTypeDef",
     {
         "OpenXJsonSerDe": OpenXJsonSerDeTypeDef,
         "HiveJsonSerDe": HiveJsonSerDeTypeDef,
     },
     total=False,
@@ -740,23 +685,14 @@
     {
         "NoEncryptionConfig": Literal["NoEncryption"],
         "KMSEncryptionConfig": KMSEncryptionConfigTypeDef,
     },
     total=False,
 )
 
-HttpEndpointRequestConfigurationOutputTypeDef = TypedDict(
-    "HttpEndpointRequestConfigurationOutputTypeDef",
-    {
-        "ContentEncoding": ContentEncodingType,
-        "CommonAttributes": List[HttpEndpointCommonAttributeTypeDef],
-    },
-    total=False,
-)
-
 HttpEndpointRequestConfigurationTypeDef = TypedDict(
     "HttpEndpointRequestConfigurationTypeDef",
     {
         "ContentEncoding": ContentEncodingType,
         "CommonAttributes": Sequence[HttpEndpointCommonAttributeTypeDef],
     },
     total=False,
@@ -766,49 +702,23 @@
     "SourceDescriptionTypeDef",
     {
         "KinesisStreamSourceDescription": KinesisStreamSourceDescriptionTypeDef,
     },
     total=False,
 )
 
-SerializerOutputTypeDef = TypedDict(
-    "SerializerOutputTypeDef",
-    {
-        "ParquetSerDe": ParquetSerDeTypeDef,
-        "OrcSerDe": OrcSerDeOutputTypeDef,
-    },
-    total=False,
-)
-
 SerializerTypeDef = TypedDict(
     "SerializerTypeDef",
     {
         "ParquetSerDe": ParquetSerDeTypeDef,
         "OrcSerDe": OrcSerDeTypeDef,
     },
     total=False,
 )
 
-_RequiredProcessorOutputTypeDef = TypedDict(
-    "_RequiredProcessorOutputTypeDef",
-    {
-        "Type": ProcessorTypeType,
-    },
-)
-_OptionalProcessorOutputTypeDef = TypedDict(
-    "_OptionalProcessorOutputTypeDef",
-    {
-        "Parameters": List[ProcessorParameterTypeDef],
-    },
-    total=False,
-)
-
-class ProcessorOutputTypeDef(_RequiredProcessorOutputTypeDef, _OptionalProcessorOutputTypeDef):
-    pass
-
 _RequiredProcessorTypeDef = TypedDict(
     "_RequiredProcessorTypeDef",
     {
         "Type": ProcessorTypeType,
     },
 )
 _OptionalProcessorTypeDef = TypedDict(
@@ -844,22 +754,14 @@
     "PutRecordInputRequestTypeDef",
     {
         "DeliveryStreamName": str,
         "Record": RecordTypeDef,
     },
 )
 
-InputFormatConfigurationOutputTypeDef = TypedDict(
-    "InputFormatConfigurationOutputTypeDef",
-    {
-        "Deserializer": DeserializerOutputTypeDef,
-    },
-    total=False,
-)
-
 InputFormatConfigurationTypeDef = TypedDict(
     "InputFormatConfigurationTypeDef",
     {
         "Deserializer": DeserializerTypeDef,
     },
     total=False,
 )
@@ -925,186 +827,42 @@
         "CompressionFormat": CompressionFormatType,
         "EncryptionConfiguration": EncryptionConfigurationTypeDef,
         "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
     },
     total=False,
 )
 
-OutputFormatConfigurationOutputTypeDef = TypedDict(
-    "OutputFormatConfigurationOutputTypeDef",
-    {
-        "Serializer": SerializerOutputTypeDef,
-    },
-    total=False,
-)
-
 OutputFormatConfigurationTypeDef = TypedDict(
     "OutputFormatConfigurationTypeDef",
     {
         "Serializer": SerializerTypeDef,
     },
     total=False,
 )
 
-ProcessingConfigurationOutputTypeDef = TypedDict(
-    "ProcessingConfigurationOutputTypeDef",
-    {
-        "Enabled": bool,
-        "Processors": List[ProcessorOutputTypeDef],
-    },
-    total=False,
-)
-
 ProcessingConfigurationTypeDef = TypedDict(
     "ProcessingConfigurationTypeDef",
     {
         "Enabled": bool,
         "Processors": Sequence[ProcessorTypeDef],
     },
     total=False,
 )
 
-DataFormatConversionConfigurationOutputTypeDef = TypedDict(
-    "DataFormatConversionConfigurationOutputTypeDef",
-    {
-        "SchemaConfiguration": SchemaConfigurationTypeDef,
-        "InputFormatConfiguration": InputFormatConfigurationOutputTypeDef,
-        "OutputFormatConfiguration": OutputFormatConfigurationOutputTypeDef,
-        "Enabled": bool,
-    },
-    total=False,
-)
-
 DataFormatConversionConfigurationTypeDef = TypedDict(
     "DataFormatConversionConfigurationTypeDef",
     {
         "SchemaConfiguration": SchemaConfigurationTypeDef,
         "InputFormatConfiguration": InputFormatConfigurationTypeDef,
         "OutputFormatConfiguration": OutputFormatConfigurationTypeDef,
         "Enabled": bool,
     },
     total=False,
 )
 
-AmazonOpenSearchServerlessDestinationDescriptionTypeDef = TypedDict(
-    "AmazonOpenSearchServerlessDestinationDescriptionTypeDef",
-    {
-        "RoleARN": str,
-        "CollectionEndpoint": str,
-        "IndexName": str,
-        "BufferingHints": AmazonOpenSearchServerlessBufferingHintsTypeDef,
-        "RetryOptions": AmazonOpenSearchServerlessRetryOptionsTypeDef,
-        "S3BackupMode": AmazonOpenSearchServerlessS3BackupModeType,
-        "S3DestinationDescription": S3DestinationDescriptionTypeDef,
-        "ProcessingConfiguration": ProcessingConfigurationOutputTypeDef,
-        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
-        "VpcConfigurationDescription": VpcConfigurationDescriptionTypeDef,
-    },
-    total=False,
-)
-
-AmazonopensearchserviceDestinationDescriptionTypeDef = TypedDict(
-    "AmazonopensearchserviceDestinationDescriptionTypeDef",
-    {
-        "RoleARN": str,
-        "DomainARN": str,
-        "ClusterEndpoint": str,
-        "IndexName": str,
-        "TypeName": str,
-        "IndexRotationPeriod": AmazonopensearchserviceIndexRotationPeriodType,
-        "BufferingHints": AmazonopensearchserviceBufferingHintsTypeDef,
-        "RetryOptions": AmazonopensearchserviceRetryOptionsTypeDef,
-        "S3BackupMode": AmazonopensearchserviceS3BackupModeType,
-        "S3DestinationDescription": S3DestinationDescriptionTypeDef,
-        "ProcessingConfiguration": ProcessingConfigurationOutputTypeDef,
-        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
-        "VpcConfigurationDescription": VpcConfigurationDescriptionTypeDef,
-    },
-    total=False,
-)
-
-ElasticsearchDestinationDescriptionTypeDef = TypedDict(
-    "ElasticsearchDestinationDescriptionTypeDef",
-    {
-        "RoleARN": str,
-        "DomainARN": str,
-        "ClusterEndpoint": str,
-        "IndexName": str,
-        "TypeName": str,
-        "IndexRotationPeriod": ElasticsearchIndexRotationPeriodType,
-        "BufferingHints": ElasticsearchBufferingHintsTypeDef,
-        "RetryOptions": ElasticsearchRetryOptionsTypeDef,
-        "S3BackupMode": ElasticsearchS3BackupModeType,
-        "S3DestinationDescription": S3DestinationDescriptionTypeDef,
-        "ProcessingConfiguration": ProcessingConfigurationOutputTypeDef,
-        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
-        "VpcConfigurationDescription": VpcConfigurationDescriptionTypeDef,
-    },
-    total=False,
-)
-
-HttpEndpointDestinationDescriptionTypeDef = TypedDict(
-    "HttpEndpointDestinationDescriptionTypeDef",
-    {
-        "EndpointConfiguration": HttpEndpointDescriptionTypeDef,
-        "BufferingHints": HttpEndpointBufferingHintsTypeDef,
-        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
-        "RequestConfiguration": HttpEndpointRequestConfigurationOutputTypeDef,
-        "ProcessingConfiguration": ProcessingConfigurationOutputTypeDef,
-        "RoleARN": str,
-        "RetryOptions": HttpEndpointRetryOptionsTypeDef,
-        "S3BackupMode": HttpEndpointS3BackupModeType,
-        "S3DestinationDescription": S3DestinationDescriptionTypeDef,
-    },
-    total=False,
-)
-
-_RequiredRedshiftDestinationDescriptionTypeDef = TypedDict(
-    "_RequiredRedshiftDestinationDescriptionTypeDef",
-    {
-        "RoleARN": str,
-        "ClusterJDBCURL": str,
-        "CopyCommand": CopyCommandTypeDef,
-        "Username": str,
-        "S3DestinationDescription": S3DestinationDescriptionTypeDef,
-    },
-)
-_OptionalRedshiftDestinationDescriptionTypeDef = TypedDict(
-    "_OptionalRedshiftDestinationDescriptionTypeDef",
-    {
-        "RetryOptions": RedshiftRetryOptionsTypeDef,
-        "ProcessingConfiguration": ProcessingConfigurationOutputTypeDef,
-        "S3BackupMode": RedshiftS3BackupModeType,
-        "S3BackupDescription": S3DestinationDescriptionTypeDef,
-        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
-    },
-    total=False,
-)
-
-class RedshiftDestinationDescriptionTypeDef(
-    _RequiredRedshiftDestinationDescriptionTypeDef, _OptionalRedshiftDestinationDescriptionTypeDef
-):
-    pass
-
-SplunkDestinationDescriptionTypeDef = TypedDict(
-    "SplunkDestinationDescriptionTypeDef",
-    {
-        "HECEndpoint": str,
-        "HECEndpointType": HECEndpointTypeType,
-        "HECToken": str,
-        "HECAcknowledgmentTimeoutInSeconds": int,
-        "RetryOptions": SplunkRetryOptionsTypeDef,
-        "S3BackupMode": SplunkS3BackupModeType,
-        "S3DestinationDescription": S3DestinationDescriptionTypeDef,
-        "ProcessingConfiguration": ProcessingConfigurationOutputTypeDef,
-        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
-    },
-    total=False,
-)
-
 _RequiredAmazonOpenSearchServerlessDestinationConfigurationTypeDef = TypedDict(
     "_RequiredAmazonOpenSearchServerlessDestinationConfigurationTypeDef",
     {
         "RoleARN": str,
         "IndexName": str,
         "S3Configuration": S3DestinationConfigurationTypeDef,
     },
@@ -1125,14 +883,31 @@
 
 class AmazonOpenSearchServerlessDestinationConfigurationTypeDef(
     _RequiredAmazonOpenSearchServerlessDestinationConfigurationTypeDef,
     _OptionalAmazonOpenSearchServerlessDestinationConfigurationTypeDef,
 ):
     pass
 
+AmazonOpenSearchServerlessDestinationDescriptionTypeDef = TypedDict(
+    "AmazonOpenSearchServerlessDestinationDescriptionTypeDef",
+    {
+        "RoleARN": str,
+        "CollectionEndpoint": str,
+        "IndexName": str,
+        "BufferingHints": AmazonOpenSearchServerlessBufferingHintsTypeDef,
+        "RetryOptions": AmazonOpenSearchServerlessRetryOptionsTypeDef,
+        "S3BackupMode": AmazonOpenSearchServerlessS3BackupModeType,
+        "S3DestinationDescription": S3DestinationDescriptionTypeDef,
+        "ProcessingConfiguration": ProcessingConfigurationTypeDef,
+        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
+        "VpcConfigurationDescription": VpcConfigurationDescriptionTypeDef,
+    },
+    total=False,
+)
+
 AmazonOpenSearchServerlessDestinationUpdateTypeDef = TypedDict(
     "AmazonOpenSearchServerlessDestinationUpdateTypeDef",
     {
         "RoleARN": str,
         "CollectionEndpoint": str,
         "IndexName": str,
         "BufferingHints": AmazonOpenSearchServerlessBufferingHintsTypeDef,
@@ -1171,14 +946,34 @@
 
 class AmazonopensearchserviceDestinationConfigurationTypeDef(
     _RequiredAmazonopensearchserviceDestinationConfigurationTypeDef,
     _OptionalAmazonopensearchserviceDestinationConfigurationTypeDef,
 ):
     pass
 
+AmazonopensearchserviceDestinationDescriptionTypeDef = TypedDict(
+    "AmazonopensearchserviceDestinationDescriptionTypeDef",
+    {
+        "RoleARN": str,
+        "DomainARN": str,
+        "ClusterEndpoint": str,
+        "IndexName": str,
+        "TypeName": str,
+        "IndexRotationPeriod": AmazonopensearchserviceIndexRotationPeriodType,
+        "BufferingHints": AmazonopensearchserviceBufferingHintsTypeDef,
+        "RetryOptions": AmazonopensearchserviceRetryOptionsTypeDef,
+        "S3BackupMode": AmazonopensearchserviceS3BackupModeType,
+        "S3DestinationDescription": S3DestinationDescriptionTypeDef,
+        "ProcessingConfiguration": ProcessingConfigurationTypeDef,
+        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
+        "VpcConfigurationDescription": VpcConfigurationDescriptionTypeDef,
+    },
+    total=False,
+)
+
 AmazonopensearchserviceDestinationUpdateTypeDef = TypedDict(
     "AmazonopensearchserviceDestinationUpdateTypeDef",
     {
         "RoleARN": str,
         "DomainARN": str,
         "ClusterEndpoint": str,
         "IndexName": str,
@@ -1220,14 +1015,34 @@
 
 class ElasticsearchDestinationConfigurationTypeDef(
     _RequiredElasticsearchDestinationConfigurationTypeDef,
     _OptionalElasticsearchDestinationConfigurationTypeDef,
 ):
     pass
 
+ElasticsearchDestinationDescriptionTypeDef = TypedDict(
+    "ElasticsearchDestinationDescriptionTypeDef",
+    {
+        "RoleARN": str,
+        "DomainARN": str,
+        "ClusterEndpoint": str,
+        "IndexName": str,
+        "TypeName": str,
+        "IndexRotationPeriod": ElasticsearchIndexRotationPeriodType,
+        "BufferingHints": ElasticsearchBufferingHintsTypeDef,
+        "RetryOptions": ElasticsearchRetryOptionsTypeDef,
+        "S3BackupMode": ElasticsearchS3BackupModeType,
+        "S3DestinationDescription": S3DestinationDescriptionTypeDef,
+        "ProcessingConfiguration": ProcessingConfigurationTypeDef,
+        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
+        "VpcConfigurationDescription": VpcConfigurationDescriptionTypeDef,
+    },
+    total=False,
+)
+
 ElasticsearchDestinationUpdateTypeDef = TypedDict(
     "ElasticsearchDestinationUpdateTypeDef",
     {
         "RoleARN": str,
         "DomainARN": str,
         "ClusterEndpoint": str,
         "IndexName": str,
@@ -1265,14 +1080,30 @@
 
 class HttpEndpointDestinationConfigurationTypeDef(
     _RequiredHttpEndpointDestinationConfigurationTypeDef,
     _OptionalHttpEndpointDestinationConfigurationTypeDef,
 ):
     pass
 
+HttpEndpointDestinationDescriptionTypeDef = TypedDict(
+    "HttpEndpointDestinationDescriptionTypeDef",
+    {
+        "EndpointConfiguration": HttpEndpointDescriptionTypeDef,
+        "BufferingHints": HttpEndpointBufferingHintsTypeDef,
+        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
+        "RequestConfiguration": HttpEndpointRequestConfigurationTypeDef,
+        "ProcessingConfiguration": ProcessingConfigurationTypeDef,
+        "RoleARN": str,
+        "RetryOptions": HttpEndpointRetryOptionsTypeDef,
+        "S3BackupMode": HttpEndpointS3BackupModeType,
+        "S3DestinationDescription": S3DestinationDescriptionTypeDef,
+    },
+    total=False,
+)
+
 HttpEndpointDestinationUpdateTypeDef = TypedDict(
     "HttpEndpointDestinationUpdateTypeDef",
     {
         "EndpointConfiguration": HttpEndpointConfigurationTypeDef,
         "BufferingHints": HttpEndpointBufferingHintsTypeDef,
         "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
         "RequestConfiguration": HttpEndpointRequestConfigurationTypeDef,
@@ -1310,14 +1141,41 @@
 
 class RedshiftDestinationConfigurationTypeDef(
     _RequiredRedshiftDestinationConfigurationTypeDef,
     _OptionalRedshiftDestinationConfigurationTypeDef,
 ):
     pass
 
+_RequiredRedshiftDestinationDescriptionTypeDef = TypedDict(
+    "_RequiredRedshiftDestinationDescriptionTypeDef",
+    {
+        "RoleARN": str,
+        "ClusterJDBCURL": str,
+        "CopyCommand": CopyCommandTypeDef,
+        "Username": str,
+        "S3DestinationDescription": S3DestinationDescriptionTypeDef,
+    },
+)
+_OptionalRedshiftDestinationDescriptionTypeDef = TypedDict(
+    "_OptionalRedshiftDestinationDescriptionTypeDef",
+    {
+        "RetryOptions": RedshiftRetryOptionsTypeDef,
+        "ProcessingConfiguration": ProcessingConfigurationTypeDef,
+        "S3BackupMode": RedshiftS3BackupModeType,
+        "S3BackupDescription": S3DestinationDescriptionTypeDef,
+        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
+    },
+    total=False,
+)
+
+class RedshiftDestinationDescriptionTypeDef(
+    _RequiredRedshiftDestinationDescriptionTypeDef, _OptionalRedshiftDestinationDescriptionTypeDef
+):
+    pass
+
 RedshiftDestinationUpdateTypeDef = TypedDict(
     "RedshiftDestinationUpdateTypeDef",
     {
         "RoleARN": str,
         "ClusterJDBCURL": str,
         "CopyCommand": CopyCommandTypeDef,
         "Username": str,
@@ -1354,14 +1212,30 @@
 )
 
 class SplunkDestinationConfigurationTypeDef(
     _RequiredSplunkDestinationConfigurationTypeDef, _OptionalSplunkDestinationConfigurationTypeDef
 ):
     pass
 
+SplunkDestinationDescriptionTypeDef = TypedDict(
+    "SplunkDestinationDescriptionTypeDef",
+    {
+        "HECEndpoint": str,
+        "HECEndpointType": HECEndpointTypeType,
+        "HECToken": str,
+        "HECAcknowledgmentTimeoutInSeconds": int,
+        "RetryOptions": SplunkRetryOptionsTypeDef,
+        "S3BackupMode": SplunkS3BackupModeType,
+        "S3DestinationDescription": S3DestinationDescriptionTypeDef,
+        "ProcessingConfiguration": ProcessingConfigurationTypeDef,
+        "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
+    },
+    total=False,
+)
+
 SplunkDestinationUpdateTypeDef = TypedDict(
     "SplunkDestinationUpdateTypeDef",
     {
         "HECEndpoint": str,
         "HECEndpointType": HECEndpointTypeType,
         "HECToken": str,
         "HECAcknowledgmentTimeoutInSeconds": int,
@@ -1370,73 +1244,73 @@
         "S3Update": S3DestinationUpdateTypeDef,
         "ProcessingConfiguration": ProcessingConfigurationTypeDef,
         "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
     },
     total=False,
 )
 
-_RequiredExtendedS3DestinationDescriptionTypeDef = TypedDict(
-    "_RequiredExtendedS3DestinationDescriptionTypeDef",
+_RequiredExtendedS3DestinationConfigurationTypeDef = TypedDict(
+    "_RequiredExtendedS3DestinationConfigurationTypeDef",
     {
         "RoleARN": str,
         "BucketARN": str,
-        "BufferingHints": BufferingHintsTypeDef,
-        "CompressionFormat": CompressionFormatType,
-        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
     },
 )
-_OptionalExtendedS3DestinationDescriptionTypeDef = TypedDict(
-    "_OptionalExtendedS3DestinationDescriptionTypeDef",
+_OptionalExtendedS3DestinationConfigurationTypeDef = TypedDict(
+    "_OptionalExtendedS3DestinationConfigurationTypeDef",
     {
         "Prefix": str,
         "ErrorOutputPrefix": str,
+        "BufferingHints": BufferingHintsTypeDef,
+        "CompressionFormat": CompressionFormatType,
+        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
         "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
-        "ProcessingConfiguration": ProcessingConfigurationOutputTypeDef,
+        "ProcessingConfiguration": ProcessingConfigurationTypeDef,
         "S3BackupMode": S3BackupModeType,
-        "S3BackupDescription": S3DestinationDescriptionTypeDef,
-        "DataFormatConversionConfiguration": DataFormatConversionConfigurationOutputTypeDef,
+        "S3BackupConfiguration": S3DestinationConfigurationTypeDef,
+        "DataFormatConversionConfiguration": DataFormatConversionConfigurationTypeDef,
         "DynamicPartitioningConfiguration": DynamicPartitioningConfigurationTypeDef,
     },
     total=False,
 )
 
-class ExtendedS3DestinationDescriptionTypeDef(
-    _RequiredExtendedS3DestinationDescriptionTypeDef,
-    _OptionalExtendedS3DestinationDescriptionTypeDef,
+class ExtendedS3DestinationConfigurationTypeDef(
+    _RequiredExtendedS3DestinationConfigurationTypeDef,
+    _OptionalExtendedS3DestinationConfigurationTypeDef,
 ):
     pass
 
-_RequiredExtendedS3DestinationConfigurationTypeDef = TypedDict(
-    "_RequiredExtendedS3DestinationConfigurationTypeDef",
+_RequiredExtendedS3DestinationDescriptionTypeDef = TypedDict(
+    "_RequiredExtendedS3DestinationDescriptionTypeDef",
     {
         "RoleARN": str,
         "BucketARN": str,
+        "BufferingHints": BufferingHintsTypeDef,
+        "CompressionFormat": CompressionFormatType,
+        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
     },
 )
-_OptionalExtendedS3DestinationConfigurationTypeDef = TypedDict(
-    "_OptionalExtendedS3DestinationConfigurationTypeDef",
+_OptionalExtendedS3DestinationDescriptionTypeDef = TypedDict(
+    "_OptionalExtendedS3DestinationDescriptionTypeDef",
     {
         "Prefix": str,
         "ErrorOutputPrefix": str,
-        "BufferingHints": BufferingHintsTypeDef,
-        "CompressionFormat": CompressionFormatType,
-        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
         "CloudWatchLoggingOptions": CloudWatchLoggingOptionsTypeDef,
         "ProcessingConfiguration": ProcessingConfigurationTypeDef,
         "S3BackupMode": S3BackupModeType,
-        "S3BackupConfiguration": S3DestinationConfigurationTypeDef,
+        "S3BackupDescription": S3DestinationDescriptionTypeDef,
         "DataFormatConversionConfiguration": DataFormatConversionConfigurationTypeDef,
         "DynamicPartitioningConfiguration": DynamicPartitioningConfigurationTypeDef,
     },
     total=False,
 )
 
-class ExtendedS3DestinationConfigurationTypeDef(
-    _RequiredExtendedS3DestinationConfigurationTypeDef,
-    _OptionalExtendedS3DestinationConfigurationTypeDef,
+class ExtendedS3DestinationDescriptionTypeDef(
+    _RequiredExtendedS3DestinationDescriptionTypeDef,
+    _OptionalExtendedS3DestinationDescriptionTypeDef,
 ):
     pass
 
 ExtendedS3DestinationUpdateTypeDef = TypedDict(
     "ExtendedS3DestinationUpdateTypeDef",
     {
         "RoleARN": str,
@@ -1452,44 +1326,14 @@
         "S3BackupUpdate": S3DestinationUpdateTypeDef,
         "DataFormatConversionConfiguration": DataFormatConversionConfigurationTypeDef,
         "DynamicPartitioningConfiguration": DynamicPartitioningConfigurationTypeDef,
     },
     total=False,
 )
 
-_RequiredDestinationDescriptionTypeDef = TypedDict(
-    "_RequiredDestinationDescriptionTypeDef",
-    {
-        "DestinationId": str,
-    },
-)
-_OptionalDestinationDescriptionTypeDef = TypedDict(
-    "_OptionalDestinationDescriptionTypeDef",
-    {
-        "S3DestinationDescription": S3DestinationDescriptionTypeDef,
-        "ExtendedS3DestinationDescription": ExtendedS3DestinationDescriptionTypeDef,
-        "RedshiftDestinationDescription": RedshiftDestinationDescriptionTypeDef,
-        "ElasticsearchDestinationDescription": ElasticsearchDestinationDescriptionTypeDef,
-        "AmazonopensearchserviceDestinationDescription": (
-            AmazonopensearchserviceDestinationDescriptionTypeDef
-        ),
-        "SplunkDestinationDescription": SplunkDestinationDescriptionTypeDef,
-        "HttpEndpointDestinationDescription": HttpEndpointDestinationDescriptionTypeDef,
-        "AmazonOpenSearchServerlessDestinationDescription": (
-            AmazonOpenSearchServerlessDestinationDescriptionTypeDef
-        ),
-    },
-    total=False,
-)
-
-class DestinationDescriptionTypeDef(
-    _RequiredDestinationDescriptionTypeDef, _OptionalDestinationDescriptionTypeDef
-):
-    pass
-
 _RequiredCreateDeliveryStreamInputRequestTypeDef = TypedDict(
     "_RequiredCreateDeliveryStreamInputRequestTypeDef",
     {
         "DeliveryStreamName": str,
     },
 )
 _OptionalCreateDeliveryStreamInputRequestTypeDef = TypedDict(
@@ -1519,14 +1363,44 @@
 
 class CreateDeliveryStreamInputRequestTypeDef(
     _RequiredCreateDeliveryStreamInputRequestTypeDef,
     _OptionalCreateDeliveryStreamInputRequestTypeDef,
 ):
     pass
 
+_RequiredDestinationDescriptionTypeDef = TypedDict(
+    "_RequiredDestinationDescriptionTypeDef",
+    {
+        "DestinationId": str,
+    },
+)
+_OptionalDestinationDescriptionTypeDef = TypedDict(
+    "_OptionalDestinationDescriptionTypeDef",
+    {
+        "S3DestinationDescription": S3DestinationDescriptionTypeDef,
+        "ExtendedS3DestinationDescription": ExtendedS3DestinationDescriptionTypeDef,
+        "RedshiftDestinationDescription": RedshiftDestinationDescriptionTypeDef,
+        "ElasticsearchDestinationDescription": ElasticsearchDestinationDescriptionTypeDef,
+        "AmazonopensearchserviceDestinationDescription": (
+            AmazonopensearchserviceDestinationDescriptionTypeDef
+        ),
+        "SplunkDestinationDescription": SplunkDestinationDescriptionTypeDef,
+        "HttpEndpointDestinationDescription": HttpEndpointDestinationDescriptionTypeDef,
+        "AmazonOpenSearchServerlessDestinationDescription": (
+            AmazonOpenSearchServerlessDestinationDescriptionTypeDef
+        ),
+    },
+    total=False,
+)
+
+class DestinationDescriptionTypeDef(
+    _RequiredDestinationDescriptionTypeDef, _OptionalDestinationDescriptionTypeDef
+):
+    pass
+
 _RequiredUpdateDestinationInputRequestTypeDef = TypedDict(
     "_RequiredUpdateDestinationInputRequestTypeDef",
     {
         "DeliveryStreamName": str,
         "CurrentDeliveryStreamVersionId": str,
         "DestinationId": str,
     },
```

### Comparing `types-aiobotocore-firehose-2.5.2.post1/types_aiobotocore_firehose.egg-info/SOURCES.txt` & `types-aiobotocore-firehose-2.5.2.post2/types_aiobotocore_firehose.egg-info/SOURCES.txt`

 * *Files identical despite different names*

