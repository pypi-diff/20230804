# Comparing `tmp/pytoniq-0.0.9.tar.gz` & `tmp/pytoniq-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytoniq-0.0.9.tar", last modified: Tue Aug  1 12:48:58 2023, max compression
+gzip compressed data, was "dist/pytoniq-0.1.0.tar", last modified: Fri Aug  4 06:42:42 2023, max compression
```

## Comparing `pytoniq-0.0.9.tar` & `pytoniq-0.1.0.tar`

### file list

```diff
@@ -1,77 +1,30 @@
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-08-01 12:48:58.693693 pytoniq-0.0.9/
--rw-r--r--   0 maxankurb   (501) staff       (20)       29 2023-07-27 17:44:46.000000 pytoniq-0.0.9/MANIFEST.in
--rw-r--r--   0 maxankurb   (501) staff       (20)    13983 2023-08-01 12:48:58.693343 pytoniq-0.0.9/PKG-INFO
--rw-r--r--   0 maxankurb   (501) staff       (20)    13577 2023-07-30 15:08:36.000000 pytoniq-0.0.9/README.md
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-08-01 12:48:58.649725 pytoniq-0.0.9/pytoniq/
--rw-r--r--   0 maxankurb   (501) staff       (20)      149 2023-07-23 15:42:41.000000 pytoniq-0.0.9/pytoniq/__init__.py
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-08-01 12:48:58.659578 pytoniq-0.0.9/pytoniq/boc/
--rw-r--r--   0 maxankurb   (501) staff       (20)      222 2023-07-23 15:42:41.000000 pytoniq-0.0.9/pytoniq/boc/__init__.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     3700 2023-07-27 16:08:51.000000 pytoniq-0.0.9/pytoniq/boc/address.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     4204 2023-07-21 09:13:36.000000 pytoniq-0.0.9/pytoniq/boc/builder.py
--rw-r--r--   0 maxankurb   (501) staff       (20)    11007 2023-07-23 16:49:28.000000 pytoniq-0.0.9/pytoniq/boc/cell.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     9079 2023-07-28 16:29:36.000000 pytoniq-0.0.9/pytoniq/boc/deserialize.py
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-08-01 12:48:58.662565 pytoniq-0.0.9/pytoniq/boc/dict/
--rw-r--r--   0 maxankurb   (501) staff       (20)       41 2023-07-23 15:42:41.000000 pytoniq-0.0.9/pytoniq/boc/dict/__init__.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     5060 2023-07-23 15:16:15.000000 pytoniq-0.0.9/pytoniq/boc/dict/dict.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     3919 2023-07-23 17:27:59.000000 pytoniq-0.0.9/pytoniq/boc/dict/parse.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     4989 2023-06-19 11:55:15.000000 pytoniq-0.0.9/pytoniq/boc/dict/utils.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     1026 2023-07-23 13:47:12.000000 pytoniq-0.0.9/pytoniq/boc/exotic.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     7521 2023-07-11 20:09:21.000000 pytoniq-0.0.9/pytoniq/boc/slice.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     1866 2023-07-05 13:08:40.000000 pytoniq-0.0.9/pytoniq/boc/tvm_bitarray.py
--rw-r--r--   0 maxankurb   (501) staff       (20)      298 2023-07-13 12:16:46.000000 pytoniq-0.0.9/pytoniq/boc/utils.py
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-08-01 12:48:58.664424 pytoniq-0.0.9/pytoniq/contract/
--rw-r--r--   0 maxankurb   (501) staff       (20)       69 2023-07-23 15:42:41.000000 pytoniq-0.0.9/pytoniq/contract/__init__.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     6750 2023-07-28 19:24:43.000000 pytoniq-0.0.9/pytoniq/contract/contract.py
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-08-01 12:48:58.665769 pytoniq-0.0.9/pytoniq/contract/nft/
--rw-r--r--   0 maxankurb   (501) staff       (20)       25 2023-07-27 17:13:15.000000 pytoniq-0.0.9/pytoniq/contract/nft/__init__.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     3643 2023-07-27 17:10:31.000000 pytoniq-0.0.9/pytoniq/contract/nft/nft.py
--rw-r--r--   0 maxankurb   (501) staff       (20)      102 2023-07-22 17:41:04.000000 pytoniq-0.0.9/pytoniq/contract/utils.py
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-08-01 12:48:58.667798 pytoniq-0.0.9/pytoniq/contract/wallets/
--rw-r--r--   0 maxankurb   (501) staff       (20)      151 2023-07-23 15:42:41.000000 pytoniq-0.0.9/pytoniq/contract/wallets/__init__.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     7615 2023-07-23 07:51:49.000000 pytoniq-0.0.9/pytoniq/contract/wallets/highload.py
--rw-r--r--   0 maxankurb   (501) staff       (20)    18779 2023-07-23 07:41:58.000000 pytoniq-0.0.9/pytoniq/contract/wallets/wallet.py
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-08-01 12:48:58.671758 pytoniq-0.0.9/pytoniq/crypto/
--rw-r--r--   0 maxankurb   (501) staff       (20)        0 2023-06-17 12:05:39.000000 pytoniq-0.0.9/pytoniq/crypto/__init__.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     2087 2023-05-27 14:21:05.000000 pytoniq-0.0.9/pytoniq/crypto/ciphers.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     6558 2023-06-17 13:10:44.000000 pytoniq-0.0.9/pytoniq/crypto/crc.py
--rw-r--r--   0 maxankurb   (501) staff       (20)    22014 2023-07-22 13:35:04.000000 pytoniq-0.0.9/pytoniq/crypto/keys.py
--rw-r--r--   0 maxankurb   (501) staff       (20)      820 2023-07-27 14:32:52.000000 pytoniq-0.0.9/pytoniq/crypto/signature.py
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-08-01 12:48:58.674874 pytoniq-0.0.9/pytoniq/liteclient/
--rw-r--r--   0 maxankurb   (501) staff       (20)       88 2023-07-23 15:42:41.000000 pytoniq-0.0.9/pytoniq/liteclient/__init__.py
--rw-r--r--   0 maxankurb   (501) staff       (20)    39220 2023-08-01 12:48:54.000000 pytoniq-0.0.9/pytoniq/liteclient/client.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     5409 2023-07-30 14:31:13.000000 pytoniq-0.0.9/pytoniq/liteclient/sync.py
--rw-r--r--   0 maxankurb   (501) staff       (20)      625 2023-07-24 15:34:43.000000 pytoniq-0.0.9/pytoniq/liteclient/utils.py
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-08-01 12:48:58.676136 pytoniq-0.0.9/pytoniq/proof/
--rw-r--r--   0 maxankurb   (501) staff       (20)      186 2023-07-23 15:42:41.000000 pytoniq-0.0.9/pytoniq/proof/__init__.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     6193 2023-07-21 11:26:13.000000 pytoniq-0.0.9/pytoniq/proof/check_proof.py
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-08-01 12:48:58.678911 pytoniq-0.0.9/pytoniq/tl/
--rw-r--r--   0 maxankurb   (501) staff       (20)      118 2023-07-23 15:42:41.000000 pytoniq-0.0.9/pytoniq/tl/__init__.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     2990 2023-07-23 08:44:15.000000 pytoniq-0.0.9/pytoniq/tl/block.py
--rw-r--r--   0 maxankurb   (501) staff       (20)    14400 2023-07-30 15:03:21.000000 pytoniq-0.0.9/pytoniq/tl/generator.py
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-08-01 12:48:58.681006 pytoniq-0.0.9/pytoniq/tl/schemas/
--rw-r--r--   0 maxankurb   (501) staff       (20)     7204 2023-07-30 12:46:41.000000 pytoniq-0.0.9/pytoniq/tl/schemas/lite_api.tl
--rw-r--r--   0 maxankurb   (501) staff       (20)    45439 2023-06-17 21:53:59.000000 pytoniq-0.0.9/pytoniq/tl/schemas/ton_api.tl
--rw-r--r--   0 maxankurb   (501) staff       (20)    18697 2023-05-29 07:39:43.000000 pytoniq-0.0.9/pytoniq/tl/schemas/tonlib_api.tl
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-08-01 12:48:58.690747 pytoniq-0.0.9/pytoniq/tlb/
--rw-r--r--   0 maxankurb   (501) staff       (20)      924 2023-07-24 08:29:16.000000 pytoniq-0.0.9/pytoniq/tlb/__init__.py
--rw-r--r--   0 maxankurb   (501) staff       (20)    11853 2023-07-23 13:10:19.000000 pytoniq-0.0.9/pytoniq/tlb/account.py
--rw-r--r--   0 maxankurb   (501) staff       (20)    34959 2023-07-24 08:25:46.000000 pytoniq-0.0.9/pytoniq/tlb/block.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     5137 2023-06-30 16:07:22.000000 pytoniq-0.0.9/pytoniq/tlb/code_generator.py
--rw-r--r--   0 maxankurb   (501) staff       (20)    56951 2023-07-13 14:13:51.000000 pytoniq-0.0.9/pytoniq/tlb/config.py
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-08-01 12:48:58.692585 pytoniq-0.0.9/pytoniq/tlb/custom/
--rw-r--r--   0 maxankurb   (501) staff       (20)       91 2023-07-27 17:13:15.000000 pytoniq-0.0.9/pytoniq/tlb/custom/__init__.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     1436 2023-07-27 17:07:58.000000 pytoniq-0.0.9/pytoniq/tlb/custom/nft.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     4584 2023-07-23 14:27:13.000000 pytoniq-0.0.9/pytoniq/tlb/custom/wallet.py
--rw-r--r--   0 maxankurb   (501) staff       (20)    12530 2023-07-27 17:28:35.000000 pytoniq-0.0.9/pytoniq/tlb/generator.py
--rw-r--r--   0 maxankurb   (501) staff       (20)      382 2023-07-23 14:10:34.000000 pytoniq-0.0.9/pytoniq/tlb/tlb.py
--rw-r--r--   0 maxankurb   (501) staff       (20)    44289 2023-07-28 18:49:05.000000 pytoniq-0.0.9/pytoniq/tlb/transaction.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     2292 2023-07-12 11:03:41.000000 pytoniq-0.0.9/pytoniq/tlb/utils.py
--rw-r--r--   0 maxankurb   (501) staff       (20)    15591 2023-08-01 07:42:26.000000 pytoniq-0.0.9/pytoniq/tlb/vm_stack.py
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-08-01 12:48:58.651881 pytoniq-0.0.9/pytoniq.egg-info/
--rw-r--r--   0 maxankurb   (501) staff       (20)    13983 2023-08-01 12:48:58.000000 pytoniq-0.0.9/pytoniq.egg-info/PKG-INFO
--rw-r--r--   0 maxankurb   (501) staff       (20)     1552 2023-08-01 12:48:58.000000 pytoniq-0.0.9/pytoniq.egg-info/SOURCES.txt
--rw-r--r--   0 maxankurb   (501) staff       (20)        1 2023-08-01 12:48:58.000000 pytoniq-0.0.9/pytoniq.egg-info/dependency_links.txt
--rw-r--r--   0 maxankurb   (501) staff       (20)      101 2023-08-01 12:48:58.000000 pytoniq-0.0.9/pytoniq.egg-info/requires.txt
--rw-r--r--   0 maxankurb   (501) staff       (20)        8 2023-08-01 12:48:58.000000 pytoniq-0.0.9/pytoniq.egg-info/top_level.txt
--rw-r--r--   0 maxankurb   (501) staff       (20)       38 2023-08-01 12:48:58.693794 pytoniq-0.0.9/setup.cfg
--rw-r--r--   0 maxankurb   (501) staff       (20)      948 2023-08-01 12:48:54.000000 pytoniq-0.0.9/setup.py
+drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-08-04 06:42:42.996296 pytoniq-0.1.0/
+-rw-r--r--   0 maxankurb   (501) staff       (20)    13984 2023-08-04 06:42:42.995871 pytoniq-0.1.0/PKG-INFO
+-rw-r--r--   0 maxankurb   (501) staff       (20)    13578 2023-08-04 06:41:49.000000 pytoniq-0.1.0/README.md
+drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-08-04 06:42:42.984453 pytoniq-0.1.0/pytoniq/
+-rw-r--r--   0 maxankurb   (501) staff       (20)      209 2023-08-04 06:37:21.000000 pytoniq-0.1.0/pytoniq/__init__.py
+drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-08-04 06:42:42.987787 pytoniq-0.1.0/pytoniq/contract/
+-rw-r--r--   0 maxankurb   (501) staff       (20)       88 2023-08-04 06:37:21.000000 pytoniq-0.1.0/pytoniq/contract/__init__.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     6805 2023-08-04 06:37:21.000000 pytoniq-0.1.0/pytoniq/contract/contract.py
+drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-08-04 06:42:42.989339 pytoniq-0.1.0/pytoniq/contract/nft/
+-rw-r--r--   0 maxankurb   (501) staff       (20)       25 2023-07-27 17:13:15.000000 pytoniq-0.1.0/pytoniq/contract/nft/__init__.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     3415 2023-08-04 06:37:21.000000 pytoniq-0.1.0/pytoniq/contract/nft/nft.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     5929 2023-08-04 06:37:20.000000 pytoniq-0.1.0/pytoniq/contract/nft/nft_sale.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)      102 2023-07-22 17:41:04.000000 pytoniq-0.1.0/pytoniq/contract/utils.py
+drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-08-04 06:42:42.991237 pytoniq-0.1.0/pytoniq/contract/wallets/
+-rw-r--r--   0 maxankurb   (501) staff       (20)      151 2023-07-23 15:42:41.000000 pytoniq-0.1.0/pytoniq/contract/wallets/__init__.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     7675 2023-08-04 06:37:21.000000 pytoniq-0.1.0/pytoniq/contract/wallets/highload.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)    18839 2023-08-04 06:37:21.000000 pytoniq-0.1.0/pytoniq/contract/wallets/wallet.py
+drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-08-04 06:42:42.994983 pytoniq-0.1.0/pytoniq/liteclient/
+-rw-r--r--   0 maxankurb   (501) staff       (20)       88 2023-07-23 15:42:41.000000 pytoniq-0.1.0/pytoniq/liteclient/__init__.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)    39278 2023-08-04 06:37:21.000000 pytoniq-0.1.0/pytoniq/liteclient/client.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     5420 2023-08-04 06:37:21.000000 pytoniq-0.1.0/pytoniq/liteclient/sync.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)      636 2023-08-04 06:37:21.000000 pytoniq-0.1.0/pytoniq/liteclient/utils.py
+drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-08-04 06:42:42.986280 pytoniq-0.1.0/pytoniq.egg-info/
+-rw-r--r--   0 maxankurb   (501) staff       (20)    13984 2023-08-04 06:42:42.000000 pytoniq-0.1.0/pytoniq.egg-info/PKG-INFO
+-rw-r--r--   0 maxankurb   (501) staff       (20)      594 2023-08-04 06:42:42.000000 pytoniq-0.1.0/pytoniq.egg-info/SOURCES.txt
+-rw-r--r--   0 maxankurb   (501) staff       (20)        1 2023-08-04 06:42:42.000000 pytoniq-0.1.0/pytoniq.egg-info/dependency_links.txt
+-rw-r--r--   0 maxankurb   (501) staff       (20)       56 2023-08-04 06:42:42.000000 pytoniq-0.1.0/pytoniq.egg-info/requires.txt
+-rw-r--r--   0 maxankurb   (501) staff       (20)        8 2023-08-04 06:42:42.000000 pytoniq-0.1.0/pytoniq.egg-info/top_level.txt
+-rw-r--r--   0 maxankurb   (501) staff       (20)       38 2023-08-04 06:42:42.996397 pytoniq-0.1.0/setup.cfg
+-rw-r--r--   0 maxankurb   (501) staff       (20)      840 2023-08-04 06:41:49.000000 pytoniq-0.1.0/setup.py
```

### Comparing `pytoniq-0.0.9/PKG-INFO` & `pytoniq-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 Metadata-Version: 2.1
 Name: pytoniq
-Version: 0.0.9
+Version: 0.1.0
 Summary: TON Blockchain SDK
 Home-page: https://github.com/yungwine/pytoniq
 Author: Maksim Kurbatov
 Author-email: cyrbatoff@gmail.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # pytoniq
 
-[![PyPI version](https://badge.fury.io/py/pytoniq.svg)](https://badge.fury.io/py/pytoniq) ![](https://pepy.tech/badge/pytoniq) [![Downloads](https://static.pepy.tech/badge/pytoniq/month)](https://pepy.tech/project/pytoniq) [![](https://img.shields.io/badge/%F0%9F%92%8E-TON-grey)](https://ton.org)
+[![PyPI version](https://badge.fury.io/py/pytoniq.svg)](https://badge.fury.io/py/pytoniq) 
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pytoniq)](https://pypi.org/project/tonsdk/)
+![](https://pepy.tech/badge/pytoniq) 
+[![Downloads](https://static.pepy.tech/badge/pytoniq/month)](https://pepy.tech/project/pytoniq) 
+[![](https://img.shields.io/badge/%F0%9F%92%8E-TON-grey)](https://ton.org)
 
-Pytoniq is a Python SDK for the TON Blockchain. 
-Currently, it has native ADNL over TCP connection to Liteservers,
-boc types implementation, wrappers for almost all TLB schemes from block.tlb,
-automaic TL schemes serialization/deserialization,
-some popular contracts wrappers.
-
-* Work in progress
+Pytoniq is a Python SDK for the TON Blockchain. This library extends [pytoniq-core](https://github.com/yungwine/pytoniq-core) with native `LiteClient` and `ADNL` over `udp` (in future).
 
 ## Documentation
 [GitBook](https://yungwine.gitbook.io/pytoniq-doc/)
 
 ## Installation
 
 ```commandline
```

### Comparing `pytoniq-0.0.9/README.md` & `pytoniq-0.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 # pytoniq
 
-[![PyPI version](https://badge.fury.io/py/pytoniq.svg)](https://badge.fury.io/py/pytoniq) ![](https://pepy.tech/badge/pytoniq) [![Downloads](https://static.pepy.tech/badge/pytoniq/month)](https://pepy.tech/project/pytoniq) [![](https://img.shields.io/badge/%F0%9F%92%8E-TON-grey)](https://ton.org)
+[![PyPI version](https://badge.fury.io/py/pytoniq.svg)](https://badge.fury.io/py/pytoniq) 
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pytoniq)](https://pypi.org/project/tonsdk/)
+![](https://pepy.tech/badge/pytoniq) 
+[![Downloads](https://static.pepy.tech/badge/pytoniq/month)](https://pepy.tech/project/pytoniq) 
+[![](https://img.shields.io/badge/%F0%9F%92%8E-TON-grey)](https://ton.org)
 
-Pytoniq is a Python SDK for the TON Blockchain. 
-Currently, it has native ADNL over TCP connection to Liteservers,
-boc types implementation, wrappers for almost all TLB schemes from block.tlb,
-automaic TL schemes serialization/deserialization,
-some popular contracts wrappers.
-
-* Work in progress
+Pytoniq is a Python SDK for the TON Blockchain. This library extends [pytoniq-core](https://github.com/yungwine/pytoniq-core) with native `LiteClient` and `ADNL` over `udp` (in future).
 
 ## Documentation
 [GitBook](https://yungwine.gitbook.io/pytoniq-doc/)
 
 ## Installation
 
 ```commandline
```

### Comparing `pytoniq-0.0.9/pytoniq/contract/contract.py` & `pytoniq-0.1.0/pytoniq/contract/contract.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import typing
 
 from ..liteclient.client import LiteClient
-from ..boc.cell import Cell
-from ..boc.address import Address
-from ..tlb.account import StateInit, Account, SimpleAccount, ShardAccount
-from ..tlb.block import CurrencyCollection
-from ..tlb.transaction import ExternalMsgInfo, MessageAny, InternalMsgInfo
+from pytoniq_core.boc.cell import Cell
+from pytoniq_core.boc.address import Address
+from pytoniq_core.tlb.account import StateInit, Account, SimpleAccount, ShardAccount
+from pytoniq_core.tlb.block import CurrencyCollection
+from pytoniq_core.tlb.transaction import ExternalMsgInfo, MessageAny, InternalMsgInfo
 
 
 class ContractError(BaseException):
     pass
 
 
 class Contract:
```

### Comparing `pytoniq-0.0.9/pytoniq/contract/nft/nft.py` & `pytoniq-0.1.0/pytoniq/contract/nft/nft.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,12 @@
-import time
-import typing
-
-from ..utils import generate_query_id
 from ..contract import Contract, ContractError
 from ...liteclient.client import LiteClient
-from ...crypto.keys import private_key_to_public_key, mnemonic_to_private_key, mnemonic_is_valid, mnemonic_new
-from ...crypto.signature import sign_message
-from ...boc import Cell, Builder, HashMap
-from ...boc.address import Address
-from ...tlb.account import StateInit
-from ...tlb.custom.nft import NftItemData
+from pytoniq_core.boc import Cell, Builder, HashMap
+from pytoniq_core.boc.address import Address
+from pytoniq_core.tlb.custom.nft import NftItemData
 
 NFT_CODE = Cell.one_from_boc(b'\xb5\xee\x9crA\x02\r\x01\x00\x01\xd0\x00\x01\x14\xff\x00\xf4\xa4\x13\xf4\xbc\xf2\xc8\x0b\x01\x02\x01b\x02\x03\x02\x02\xce\x04\x05\x00\t\xa1\x1f\x9f\xe0\x05\x02\x01 \x06\x07\x02\x01 \x0b\x0c\x02\xd7\x0c\x88q\xc0$\x97\xc0\xf844\xc0\xc0\\l$\x97\xc0\xf8>\x90>\x90\x0c~\x80\x0c\\u\xc8~\x80\x0c~\x80\x0c<\x00\x81,\xe3\x85\x0c\x1b\x08\x8d\x14\x8c\xb1\xc1|\xb8e@~\x905\x0c\x04\x08\xfc\x00\xf8\x01\xb4\xc7\xf4\xcf\xe0\x84\x17\xf3\x0fE\x14\x8c.\xa3\xa1\xcc\x84\r\xd7\x8c\x90\x04\xf8\x0c\r\r\rM`\x84\x0b\xf2\xc9\xa8\x84\xae\xb8\xc0\x97\xc1!\x03\xfc\xbc \x08\t\x00\x11>\x91\x0c\x1c.\xbc\xb8S`\x01\xf6Q5\xc7\x05\xf2\xe1\x91\xfa@!\xf0\x01\xfa@\xd2\x001\xfa\x00\x82\n\xfa\xf0\x80\x1b\xa1!\x94S\x15\xa0\xa1\xde"\xd7\x0b\x01\xc3\x00 \x92\x06\xa1\x916\xe2 \xc2\xff\xf2\xe1\x92!\x8e>\x82\x10\x05\x13\x8d\x91\xc8P\t\xcf\x16P\x0b\xcf\x16q$I\x14TF\xa0p\x80\x10\xc8\xcb\x05P\x07\xcf\x16P\x05\xfa\x02\x15\xcbj\x12\xcb\x1f\xcb?"n\xb3\x94X\xcf\x17\x01\x912\xe2\x01\xc9\x01\xfb\x00\x10G\x94\x10*7[\xe2\n\x00rp\x82\x10\x8bw\x175\x05\xc8\xcb\xffP\x04\xcf\x16\x10$\x80@p\x80\x10\xc8\xcb\x05P\x07\xcf\x16P\x05\xfa\x02\x15\xcbj\x12\xcb\x1f\xcb?"n\xb3\x94X\xcf\x17\x01\x912\xe2\x01\xc9\x01\xfb\x00\x00\x82\x02\x8e5&\xf0\x01\x82\x10\xd52v\xdb\x107D\x00mqp\x80\x10\xc8\xcb\x05P\x07\xcf\x16P\x05\xfa\x02\x15\xcbj\x12\xcb\x1f\xcb?"n\xb3\x94X\xcf\x17\x01\x912\xe2\x01\xc9\x01\xfb\x00\x93024\xe2U\x02\xf0\x03\x00;;Q44\xcf\xfe\x90\x085\xd2p\x80&\x9f\xc0~\x905\x0c\x04\t\x04\x08\xf8\x0c\x1c\x16[[`\x00\x1d\x00\xf22\xcf\xd63\xc5\x80s\xc5\xb32{U \xbfu\x04\x1b')
 
 
 class NftItem(Contract):
 
     @classmethod
```

### Comparing `pytoniq-0.0.9/pytoniq/contract/wallets/highload.py` & `pytoniq-0.1.0/pytoniq/contract/wallets/highload.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import time
 import typing
 
 from .wallet import Wallet, WalletError
 from ..utils import generate_query_id
 from ..contract import Contract, ContractError
 from ...liteclient.client import LiteClient
-from ...crypto.keys import private_key_to_public_key, mnemonic_to_private_key, mnemonic_is_valid, mnemonic_new
-from ...crypto.signature import sign_message
-from ...boc import Cell, Builder, HashMap
-from ...boc.address import Address
-from ...tlb.account import StateInit
-from ...tlb.custom.wallet import HighloadWalletData, WalletMessage
+from pytoniq_core.crypto.keys import private_key_to_public_key, mnemonic_to_private_key, mnemonic_is_valid, mnemonic_new
+from pytoniq_core.crypto.signature import sign_message
+from pytoniq_core.boc import Cell, Builder, HashMap
+from pytoniq_core.boc.address import Address
+from pytoniq_core.tlb.account import StateInit
+from pytoniq_core.tlb.custom.wallet import HighloadWalletData, WalletMessage
 
 HIGHLOAD_WALLET_CODE = Cell.one_from_boc(
     b'\xb5\xee\x9cr\x01\x01\t\x01\x00\xe5\x00\x01\x14\xff\x00\xf4\xa4\x13\xf4\xbc\xf2\xc8\x0b\x01\x02\x01 \x02\x03\x02\x01H\x04\x05\x01\xea\xf2\x83\x08\xd7\x18 \xd3\x1f\xd3?\xf8#\xaa\x1fS \xb9\xf2c\xedD\xd0\xd3\x1f\xd3?\xd3\xff\xf4\x04\xd1S`\x80@\xf4\x0eo\xa11\xf2`Qs\xba\xf2\xa2\x07\xf9\x01T\x10\x87\xf9\x10\xf2\xa3\x02\xf4\x04\xd1\xf8\x00\x7f\x8e\x16!\x80\x10\xf4xo\xa5 \x98\x02\xd3\x07\xd40\x01\xfb\x00\x912\xe2\x01\xb3\xe6[\x83%\xa1\xc8@4\x80@\xf4C\x8a\xe61\x01\xc8\xcb\x1f\x13\xcb?\xcb\xff\xf4\x00\xc9\xedT\x08\x00\x04\xd00\x02\x01 \x06\x07\x00\x17\xbd\x9c\xe7j&\x86\x9a\xf9\x8e\xb8_\xfc\x00A\xbe_\x97j&\x86\x98\xf9\x8e\x99\xfe\x9f\xf9\x8f\xa0&\x8a\x91\x04\x02\x07\xa0s}\t\x8c\x92\xdb\xfc\x95\xdd\x1f\x14\x004 \x80@\xf4\x96o\xa5l\x12 \x940S\x03\xb9\xde \x9336\x01\x92l!\xe2\xb3')
 
 
 class HighloadWallet(Wallet):
```

### Comparing `pytoniq-0.0.9/pytoniq/contract/wallets/wallet.py` & `pytoniq-0.1.0/pytoniq/contract/wallets/wallet.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import time
 import typing
 
 from ...liteclient.client import LiteClient
 from ..contract import Contract, ContractError
-from ...crypto.keys import private_key_to_public_key, mnemonic_to_private_key, mnemonic_is_valid, mnemonic_new
-from ...crypto.signature import sign_message
-from ...boc import Cell, Builder
-from ...boc.address import Address
-from ...tlb.account import StateInit
-from ...tlb.custom.wallet import WalletV3Data, WalletV4Data, WalletMessage
+from pytoniq_core.crypto.keys import private_key_to_public_key, mnemonic_to_private_key, mnemonic_is_valid, mnemonic_new
+from pytoniq_core.crypto.signature import sign_message
+from pytoniq_core.boc import Cell, Builder
+from pytoniq_core.boc.address import Address
+from pytoniq_core.tlb.account import StateInit
+from pytoniq_core.tlb.custom.wallet import WalletV3Data, WalletV4Data, WalletMessage
 
 WALLET_V3_R2_CODE = Cell.one_from_boc(
     b'\xb5\xee\x9crA\x01\x01\x01\x00q\x00\x00\xde\xff\x00 \xdd \x82\x01L\x97\xba!\x82\x013\x9c\xba\xb1\x9fq\xb0\xedD\xd0\xd3\x1f\xd3\x1f1\xd7\x0b\xff\xe3\x04\xe0\xa4\xf2`\x83\x08\xd7\x18 \xd3\x1f\xd3\x1f\xd3\x1f\xf8#\x13\xbb\xf2c\xedD\xd0\xd3\x1f\xd3\x1f\xd3\xff\xd1Q2\xba\xf2\xa1QD\xba\xf2\xa2\x04\xf9\x01T\x10U\xf9\x10\xf2\xa3\xf8\x00\x93 \xd7J\x96\xd3\x07\xd4\x02\xfb\x00\xe8\xd1\x01\xa4\xc8\xcb\x1f\xcb\x1f\xcb\xff\xc9\xedT\x10\xbdm\xad')
 WALLET_V3_R1_CODE = Cell.one_from_boc(
     b'\xb5\xee\x9crA\x01\x01\x01\x00b\x00\x00\xc0\xff\x00 \xdd \x82\x01L\x97\xba\x970\xedD\xd0\xd7\x0b\x1f\xe0\xa4\xf2`\x83\x08\xd7\x18 \xd3\x1f\xd3\x1f\xd3\x1f\xf8#\x13\xbb\xf2c\xedD\xd0\xd3\x1f\xd3\x1f\xd3\xff\xd1Q2\xba\xf2\xa1QD\xba\xf2\xa2\x04\xf9\x01T\x10U\xf9\x10\xf2\xa3\xf8\x00\x93 \xd7J\x96\xd3\x07\xd4\x02\xfb\x00\xe8\xd1\x01\xa4\xc8\xcb\x1f\xcb\x1f\xcb\xff\xc9\xedT?\xben\xe0')
 WALLET_V4_R2_CODE = Cell.one_from_boc(
     b'\xb5\xee\x9crA\x02\x14\x01\x00\x02\xd4\x00\x01\x14\xff\x00\xf4\xa4\x13\xf4\xbc\xf2\xc8\x0b\x01\x02\x01 \x02\x03\x02\x01H\x04\x05\x04\xf8\xf2\x83\x08\xd7\x18 \xd3\x1f\xd3\x1f\xd3\x1f\x02\xf8#\xbb\xf2d\xedD\xd0\xd3\x1f\xd3\x1f\xd3\xff\xf4\x04\xd1QC\xba\xf2\xa1QQ\xba\xf2\xa2\x05\xf9\x01T\x10d\xf9\x10\xf2\xa3\xf8\x00$\xa4\xc8\xcb\x1fR@\xcb\x1fR0\xcb\xffR\x10\xf4\x00\xc9\xedT\xf8\x0f\x01\xd3\x07!\xc0\x00\x9flQ\x93 \xd7J\x96\xd3\x07\xd4\x02\xfb\x00\xe80\xe0!\xc0\x01\xe3\x00!\xc0\x02\xe3\x00\x01\xc0\x03\x910\xe3\r\x03\xa4\xc8\xcb\x1f\x12\xcb\x1f\xcb\xff\x10\x11\x12\x13\x02\xe6\xd0\x01\xd0\xd3\x03!q\xb0\x92_\x04\xe0"\xd7I\xc1 \x92_\x04\xe0\x02\xd3\x1f!\x82\x10plug\xbd"\x82\x10dstr\xbd\xb0\x92_\x05\xe0\x03\xfa@0 \xfaD\x01\xc8\xca\x07\xcb\xff\xc9\xd0\xedD\xd0\x81\x01@\xd7!\xf4\x040\\\x81\x01\x08\xf4\no\xa11\xb3\x92_\x07\xe0\x05\xd3?\xc8%\x82\x10plug\xba\x9280\xe3\r\x03\x82\x10dstr\xba\x92_\x06\xe3\r\x06\x07\x02\x01 \x08\t\x00x\x01\xfa\x00\xf4\x040\xf8\'o"0P\n\xa1!\xbe\xf2\xe0P\x82\x10plug\x83\x1e\xb1p\x80\x18P\x04\xcb\x05&\xcf\x16X\xfa\x02\x19\xf4\x00\xcbi\x17\xcb\x1fR`\xcb? \xc9\x80@\xfb\x00\x06\x00\x8aP\x04\x81\x01\x08\xf4Y0\xedD\xd0\x81\x01@\xd7 \xc8\x01\xcf\x16\xf4\x00\xc9\xedT\x01r\xb0\x8e#\x82\x10dstr\x83\x1e\xb1p\x80\x18P\x05\xcb\x05P\x03\xcf\x16#\xfa\x02\x13\xcbj\xcb\x1f\xcb?\xc9\x80@\xfb\x00\x92_\x03\xe2\x02\x01 \n\x0b\x00Y\xbd$+oj&\x84\x08\n\x06\xb9\x0f\xa0!\x84p\xd4\x08\x08G\xa4\x93})\x91\x0c\xe6\x90>\x9f\xf9\x83x\x12\x80\x1bx\x10\x14\x89\x87\x15\x9f1\x84\x02\x01X\x0c\r\x00\x11\xb8\xc9~\xd4M\rp\xb1\xf8\x00=\xb2\x9d\xfbQ4 @P5\xc8}\x01\x0c\x00\xb22\x81\xf2\xff\xf2t\x00`@B=\x02\x9b\xe8L`\x02\x01 \x0e\x0f\x00\x19\xad\xcev\xa2h@ k\x90\xeb\x85\xff\xc0\x00\x19\xaf\x1d\xf6\xa2h@\x10k\x90\xeb\x85\x8f\xc0\x00n\xd2\x07\xfa\x00\xd4\xd4"\xf9\x00\x05\xc8\xca\x07\x15\xcb\xff\xc9\xd0wt\x80\x18\xc8\xcb\x05\xcb\x02"\xcf\x16P\x05\xfa\x02\x14\xcbk\x12\xcc\xcc\xc9s\xfb\x00\xc8@\x14\x81\x01\x08\xf4Q\xf2\xa7\x02\x00p\x81\x01\x08\xd7\x18\xfa\x00\xd3?\xc8T G\x81\x01\x08\xf4Q\xf2\xa7\x82\x10notept\x80\x18\xc8\xcb\x05\xcb\x02P\x06\xcf\x16P\x04\xfa\x02\x14\xcbj\x12\xcb\x1f\xcb?\xc9s\xfb\x00\x02\x00l\x81\x01\x08\xd7\x18\xfa\x00\xd3?0R$\x81\x01\x08\xf4Y\xf2\xa7\x82\x10dstrpt\x80\x18\xc8\xcb\x05\xcb\x02P\x05\xcf\x16P\x03\xfa\x02\x13\xcbj\xcb\x1f\x12\xcb?\xc9s\xfb\x00\x00\n\xf4\x00\xc9\xedTib%\xe5')
```

### Comparing `pytoniq-0.0.9/pytoniq/liteclient/client.py` & `pytoniq-0.1.0/pytoniq/liteclient/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,32 +8,31 @@
 import time
 import typing
 
 import requests
 
 from .sync import persistent_state_ttl, choose_key_block, sync
 from .utils import init_mainnet_block, init_testnet_block
-from ..boc import Slice, Cell, Builder
-from ..proof.check_proof import check_block_header_proof, check_shard_proof, check_account_proof, check_proof, \
+from pytoniq_core.boc import Slice, Cell, Builder
+from pytoniq_core.proof.check_proof import check_block_header_proof, check_shard_proof, check_account_proof, check_proof, \
     check_block_signatures, compute_validator_set
-from ..boc.address import Address
+from pytoniq_core.boc.address import Address
 
-# from .crypto import ed25519Public, ed25519Private, x25519Public, x25519Private
-from ..crypto.ciphers import Server, Client, get_random, create_aes_ctr_cipher, aes_ctr_encrypt, aes_ctr_decrypt, get_shared_key
-from ..crypto.crc import crc16
-
-from ..tl.generator import TlGenerator, TlSchema
-from ..tl.block import BlockId, BlockIdExt
-from ..tlb.config import ConfigParam34, ConfigParam28, ConfigParam
-from ..tlb.transaction import Transaction
-from ..tlb.utils import deserialize_shard_hashes
-
-from ..tlb.vm_stack import VmStack
-from ..tlb.block import Block, ShardDescr, BinTree, ShardStateUnsplit, KeyExtBlkRef
-from ..tlb.account import Account, SimpleAccount, ShardAccount, AccountBlock
+from pytoniq_core.crypto.ciphers import Server, Client, get_random, create_aes_ctr_cipher, aes_ctr_encrypt, aes_ctr_decrypt, get_shared_key
+from pytoniq_core.crypto.crc import crc16
+
+from pytoniq_core.tl.generator import TlGenerator, TlSchema
+from pytoniq_core.tl.block import BlockId, BlockIdExt
+from pytoniq_core.tlb.config import ConfigParam34, ConfigParam28, ConfigParam
+from pytoniq_core.tlb.transaction import Transaction
+from pytoniq_core.tlb.utils import deserialize_shard_hashes
+
+from pytoniq_core.tlb.vm_stack import VmStack
+from pytoniq_core.tlb.block import Block, ShardDescr, BinTree, ShardStateUnsplit, KeyExtBlkRef
+from pytoniq_core.tlb.account import Account, SimpleAccount, ShardAccount, AccountBlock
 
 
 class LiteClientError(BaseException):
     pass
 
 
 class RunGetMethodError(LiteClientError):
@@ -78,16 +77,17 @@
         self.pinger: asyncio.Task = None
         self.updater: asyncio.Task = None
         self.loop: asyncio.AbstractEventLoop = None
         self.delta = 0.02  # listen delay
 
         """########### TL ###########"""
         if tl_schemas_path is None:
-            tl_schemas_path = os.path.join(os.path.dirname(__file__), os.pardir, 'tl/schemas')
-        self.schemas = TlGenerator(tl_schemas_path).generate()
+            self.schemas = TlGenerator.with_default_schemas().generate()
+        else:
+            self.schemas = TlGenerator(tl_schemas_path).generate()
         # for better performance:
         self.ping_sch = self.schemas.get_by_name('tcp.ping')
         self.pong_sch = self.schemas.get_by_name('tcp.pong')
         self.adnl_query_sch = self.schemas.get_by_name('adnl.message.query')
         self.ls_query_sch = self.schemas.get_by_name('liteServer.query')
 
     def encrypt(self, data: bytes) -> bytes:
```

### Comparing `pytoniq-0.0.9/pytoniq/liteclient/sync.py` & `pytoniq-0.1.0/pytoniq/liteclient/sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 import os
 import time
 import typing
 
-from ..tl.block import BlockIdExt
+from pytoniq_core.tl.block import BlockIdExt
 
 
 logger = logging.getLogger('sync')
 
 
 async def sync(client: "LiteClient", to_block: BlockIdExt, init_block: BlockIdExt):
     logger.info(msg=f'syncing to {to_block}')
```

### Comparing `pytoniq-0.0.9/pytoniq/liteclient/utils.py` & `pytoniq-0.1.0/pytoniq/liteclient/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ..tl.block import BlockIdExt
+from pytoniq_core.tl.block import BlockIdExt
 
 init_mainnet_block = BlockIdExt.from_dict({
     "root_hash": "61192b72664cbcb06f8da9f0282c8bdf0e2871e18fb457e0c7cca6d502822bfe",
     "seqno": 27747086,
     "file_hash": "378db1ccf9c98c3944de1c4f5ce6fea4dcd7a26811b695f9019ccc3e7200e35b",
     "workchain": -1,
     "shard": -9223372036854775808
```

### Comparing `pytoniq-0.0.9/pytoniq.egg-info/PKG-INFO` & `pytoniq-0.1.0/pytoniq.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 Metadata-Version: 2.1
 Name: pytoniq
-Version: 0.0.9
+Version: 0.1.0
 Summary: TON Blockchain SDK
 Home-page: https://github.com/yungwine/pytoniq
 Author: Maksim Kurbatov
 Author-email: cyrbatoff@gmail.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # pytoniq
 
-[![PyPI version](https://badge.fury.io/py/pytoniq.svg)](https://badge.fury.io/py/pytoniq) ![](https://pepy.tech/badge/pytoniq) [![Downloads](https://static.pepy.tech/badge/pytoniq/month)](https://pepy.tech/project/pytoniq) [![](https://img.shields.io/badge/%F0%9F%92%8E-TON-grey)](https://ton.org)
+[![PyPI version](https://badge.fury.io/py/pytoniq.svg)](https://badge.fury.io/py/pytoniq) 
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pytoniq)](https://pypi.org/project/tonsdk/)
+![](https://pepy.tech/badge/pytoniq) 
+[![Downloads](https://static.pepy.tech/badge/pytoniq/month)](https://pepy.tech/project/pytoniq) 
+[![](https://img.shields.io/badge/%F0%9F%92%8E-TON-grey)](https://ton.org)
 
-Pytoniq is a Python SDK for the TON Blockchain. 
-Currently, it has native ADNL over TCP connection to Liteservers,
-boc types implementation, wrappers for almost all TLB schemes from block.tlb,
-automaic TL schemes serialization/deserialization,
-some popular contracts wrappers.
-
-* Work in progress
+Pytoniq is a Python SDK for the TON Blockchain. This library extends [pytoniq-core](https://github.com/yungwine/pytoniq-core) with native `LiteClient` and `ADNL` over `udp` (in future).
 
 ## Documentation
 [GitBook](https://yungwine.gitbook.io/pytoniq-doc/)
 
 ## Installation
 
 ```commandline
```

### Comparing `pytoniq-0.0.9/setup.py` & `pytoniq-0.1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,28 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pytoniq",
-    version="0.0.9",
+    version="0.1.0",
     author="Maksim Kurbatov",
     author_email="cyrbatoff@gmail.com",
     description="TON Blockchain SDK",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages('.', exclude=['tests', 'examples', 'pytoniq/adnl']),
-    include_package_data=True,
     classifiers=[
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Topic :: Software Development :: Libraries",
     ],
     url="https://github.com/yungwine/pytoniq",
     python_requires='>=3.10',
     py_modules=["pytoniq"],
     install_requires=[
-        "cryptography>=40.0.2",
-        "bitarray>=2.6.0",
+        "pytoniq-core>=0.1.0",
         "requests>=2.31.0",
-        "x25519>=0.0.2",
         "setuptools>=65.5.1",
-        "PyNaCl>=1.5.0"
     ]
 )
```

