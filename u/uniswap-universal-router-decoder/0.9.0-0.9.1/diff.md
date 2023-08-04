# Comparing `tmp/uniswap-universal-router-decoder-0.9.0.tar.gz` & `tmp/uniswap-universal-router-decoder-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uniswap-universal-router-decoder-0.9.0.tar", last modified: Tue Jul  4 17:21:02 2023, max compression
+gzip compressed data, was "uniswap-universal-router-decoder-0.9.1.tar", last modified: Fri Aug  4 13:37:29 2023, max compression
```

## Comparing `uniswap-universal-router-decoder-0.9.0.tar` & `uniswap-universal-router-decoder-0.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 elnaril   (1000) elnaril   (1000)        0 2023-07-04 17:21:02.951264 uniswap-universal-router-decoder-0.9.0/
--rw-rw-r--   0 elnaril   (1000) elnaril   (1000)     1064 2023-02-10 14:36:58.000000 uniswap-universal-router-decoder-0.9.0/LICENSE
--rw-rw-r--   0 elnaril   (1000) elnaril   (1000)    15747 2023-07-04 17:21:02.951264 uniswap-universal-router-decoder-0.9.0/PKG-INFO
--rw-rw-r--   0 elnaril   (1000) elnaril   (1000)    14647 2023-07-04 17:12:01.000000 uniswap-universal-router-decoder-0.9.0/README.md
--rw-rw-r--   0 elnaril   (1000) elnaril   (1000)     1279 2023-07-04 17:12:21.000000 uniswap-universal-router-decoder-0.9.0/pyproject.toml
--rw-rw-r--   0 elnaril   (1000) elnaril   (1000)       38 2023-07-04 17:21:02.951264 uniswap-universal-router-decoder-0.9.0/setup.cfg
-drwxrwxr-x   0 elnaril   (1000) elnaril   (1000)        0 2023-07-04 17:21:02.951264 uniswap-universal-router-decoder-0.9.0/tests/
--rw-rw-r--   0 elnaril   (1000) elnaril   (1000)     1311 2023-03-18 12:57:32.000000 uniswap-universal-router-decoder-0.9.0/tests/test_abi_builder.py
--rw-rw-r--   0 elnaril   (1000) elnaril   (1000)     4750 2023-03-18 12:57:32.000000 uniswap-universal-router-decoder-0.9.0/tests/test_decoder.py
--rw-rw-r--   0 elnaril   (1000) elnaril   (1000)    20784 2023-07-04 17:12:01.000000 uniswap-universal-router-decoder-0.9.0/tests/test_encoder.py
--rw-rw-r--   0 elnaril   (1000) elnaril   (1000)      347 2023-03-18 12:57:32.000000 uniswap-universal-router-decoder-0.9.0/tests/test_router_codec.py
-drwxrwxr-x   0 elnaril   (1000) elnaril   (1000)        0 2023-07-04 17:21:02.951264 uniswap-universal-router-decoder-0.9.0/uniswap_universal_router_decoder/
--rw-rw-r--   0 elnaril   (1000) elnaril   (1000)      189 2023-03-18 12:57:32.000000 uniswap-universal-router-decoder-0.9.0/uniswap_universal_router_decoder/__init__.py
--rw-rw-r--   0 elnaril   (1000) elnaril   (1000)     5517 2023-03-18 12:57:32.000000 uniswap-universal-router-decoder-0.9.0/uniswap_universal_router_decoder/_abi_builder.py
--rw-rw-r--   0 elnaril   (1000) elnaril   (1000)     7003 2023-03-18 12:57:32.000000 uniswap-universal-router-decoder-0.9.0/uniswap_universal_router_decoder/_constants.py
--rw-rw-r--   0 elnaril   (1000) elnaril   (1000)     4273 2023-03-18 12:57:32.000000 uniswap-universal-router-decoder-0.9.0/uniswap_universal_router_decoder/_decoder.py
--rw-rw-r--   0 elnaril   (1000) elnaril   (1000)    22088 2023-07-04 17:12:01.000000 uniswap-universal-router-decoder-0.9.0/uniswap_universal_router_decoder/_encoder.py
--rw-rw-r--   0 elnaril   (1000) elnaril   (1000)     1073 2023-07-04 17:12:01.000000 uniswap-universal-router-decoder-0.9.0/uniswap_universal_router_decoder/_enums.py
--rw-rw-r--   0 elnaril   (1000) elnaril   (1000)     4309 2023-03-18 12:57:32.000000 uniswap-universal-router-decoder-0.9.0/uniswap_universal_router_decoder/router_codec.py
-drwxrwxr-x   0 elnaril   (1000) elnaril   (1000)        0 2023-07-04 17:21:02.951264 uniswap-universal-router-decoder-0.9.0/uniswap_universal_router_decoder.egg-info/
--rw-rw-r--   0 elnaril   (1000) elnaril   (1000)    15747 2023-07-04 17:21:02.000000 uniswap-universal-router-decoder-0.9.0/uniswap_universal_router_decoder.egg-info/PKG-INFO
--rw-rw-r--   0 elnaril   (1000) elnaril   (1000)      731 2023-07-04 17:21:02.000000 uniswap-universal-router-decoder-0.9.0/uniswap_universal_router_decoder.egg-info/SOURCES.txt
--rw-rw-r--   0 elnaril   (1000) elnaril   (1000)        1 2023-07-04 17:21:02.000000 uniswap-universal-router-decoder-0.9.0/uniswap_universal_router_decoder.egg-info/dependency_links.txt
--rw-rw-r--   0 elnaril   (1000) elnaril   (1000)       19 2023-07-04 17:21:02.000000 uniswap-universal-router-decoder-0.9.0/uniswap_universal_router_decoder.egg-info/requires.txt
--rw-rw-r--   0 elnaril   (1000) elnaril   (1000)       33 2023-07-04 17:21:02.000000 uniswap-universal-router-decoder-0.9.0/uniswap_universal_router_decoder.egg-info/top_level.txt
+drwxrwxr-x   0 elnaril   (1000) elnaril   (1000)        0 2023-08-04 13:37:29.380735 uniswap-universal-router-decoder-0.9.1/
+-rw-rw-r--   0 elnaril   (1000) elnaril   (1000)     1064 2023-02-10 14:36:58.000000 uniswap-universal-router-decoder-0.9.1/LICENSE
+-rw-rw-r--   0 elnaril   (1000) elnaril   (1000)    15928 2023-08-04 13:37:29.380735 uniswap-universal-router-decoder-0.9.1/PKG-INFO
+-rw-rw-r--   0 elnaril   (1000) elnaril   (1000)    14828 2023-08-04 13:34:55.000000 uniswap-universal-router-decoder-0.9.1/README.md
+-rw-rw-r--   0 elnaril   (1000) elnaril   (1000)     1279 2023-08-04 13:36:16.000000 uniswap-universal-router-decoder-0.9.1/pyproject.toml
+-rw-rw-r--   0 elnaril   (1000) elnaril   (1000)       38 2023-08-04 13:37:29.380735 uniswap-universal-router-decoder-0.9.1/setup.cfg
+drwxrwxr-x   0 elnaril   (1000) elnaril   (1000)        0 2023-08-04 13:37:29.376735 uniswap-universal-router-decoder-0.9.1/tests/
+-rw-rw-r--   0 elnaril   (1000) elnaril   (1000)     1311 2023-03-18 12:57:32.000000 uniswap-universal-router-decoder-0.9.1/tests/test_abi_builder.py
+-rw-rw-r--   0 elnaril   (1000) elnaril   (1000)     4754 2023-08-04 13:34:55.000000 uniswap-universal-router-decoder-0.9.1/tests/test_decoder.py
+-rw-rw-r--   0 elnaril   (1000) elnaril   (1000)    20786 2023-08-04 13:34:55.000000 uniswap-universal-router-decoder-0.9.1/tests/test_encoder.py
+-rw-rw-r--   0 elnaril   (1000) elnaril   (1000)      347 2023-03-18 12:57:32.000000 uniswap-universal-router-decoder-0.9.1/tests/test_router_codec.py
+drwxrwxr-x   0 elnaril   (1000) elnaril   (1000)        0 2023-08-04 13:37:29.376735 uniswap-universal-router-decoder-0.9.1/uniswap_universal_router_decoder/
+-rw-rw-r--   0 elnaril   (1000) elnaril   (1000)      189 2023-03-18 12:57:32.000000 uniswap-universal-router-decoder-0.9.1/uniswap_universal_router_decoder/__init__.py
+-rw-rw-r--   0 elnaril   (1000) elnaril   (1000)     5517 2023-03-18 12:57:32.000000 uniswap-universal-router-decoder-0.9.1/uniswap_universal_router_decoder/_abi_builder.py
+-rw-rw-r--   0 elnaril   (1000) elnaril   (1000)     7003 2023-03-18 12:57:32.000000 uniswap-universal-router-decoder-0.9.1/uniswap_universal_router_decoder/_constants.py
+-rw-rw-r--   0 elnaril   (1000) elnaril   (1000)     4277 2023-08-04 13:34:55.000000 uniswap-universal-router-decoder-0.9.1/uniswap_universal_router_decoder/_decoder.py
+-rw-rw-r--   0 elnaril   (1000) elnaril   (1000)    22014 2023-08-04 13:34:55.000000 uniswap-universal-router-decoder-0.9.1/uniswap_universal_router_decoder/_encoder.py
+-rw-rw-r--   0 elnaril   (1000) elnaril   (1000)     1073 2023-07-04 17:12:01.000000 uniswap-universal-router-decoder-0.9.1/uniswap_universal_router_decoder/_enums.py
+-rw-rw-r--   0 elnaril   (1000) elnaril   (1000)     4309 2023-03-18 12:57:32.000000 uniswap-universal-router-decoder-0.9.1/uniswap_universal_router_decoder/router_codec.py
+drwxrwxr-x   0 elnaril   (1000) elnaril   (1000)        0 2023-08-04 13:37:29.380735 uniswap-universal-router-decoder-0.9.1/uniswap_universal_router_decoder.egg-info/
+-rw-rw-r--   0 elnaril   (1000) elnaril   (1000)    15928 2023-08-04 13:37:29.000000 uniswap-universal-router-decoder-0.9.1/uniswap_universal_router_decoder.egg-info/PKG-INFO
+-rw-rw-r--   0 elnaril   (1000) elnaril   (1000)      731 2023-08-04 13:37:29.000000 uniswap-universal-router-decoder-0.9.1/uniswap_universal_router_decoder.egg-info/SOURCES.txt
+-rw-rw-r--   0 elnaril   (1000) elnaril   (1000)        1 2023-08-04 13:37:29.000000 uniswap-universal-router-decoder-0.9.1/uniswap_universal_router_decoder.egg-info/dependency_links.txt
+-rw-rw-r--   0 elnaril   (1000) elnaril   (1000)       19 2023-08-04 13:37:29.000000 uniswap-universal-router-decoder-0.9.1/uniswap_universal_router_decoder.egg-info/requires.txt
+-rw-rw-r--   0 elnaril   (1000) elnaril   (1000)       33 2023-08-04 13:37:29.000000 uniswap-universal-router-decoder-0.9.1/uniswap_universal_router_decoder.egg-info/top_level.txt
```

### Comparing `uniswap-universal-router-decoder-0.9.0/LICENSE` & `uniswap-universal-router-decoder-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `uniswap-universal-router-decoder-0.9.0/PKG-INFO` & `uniswap-universal-router-decoder-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uniswap-universal-router-decoder
-Version: 0.9.0
+Version: 0.9.1
 Summary: Decode & Encode transaction data sent to Uniswap Universal Router
 Author-email: Elnaril <elnaril_dev@caramail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/Elnaril/uniswap-universal-router-decoder
 Project-URL: Bug Tracker, https://github.com/Elnaril/uniswap-universal-router-decoder/issues
 Project-URL: Fiverr, https://www.fiverr.com/elnaril
 Keywords: blockchain,ethereum,uniswap,universal router,decoder,encoder,codec,wrapper
@@ -39,27 +39,30 @@
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![Type Checker: mypy](https://img.shields.io/badge/%20type%20checker-mypy-%231674b1?style=flat&labelColor=ef8336)](https://mypy-lang.org/)
 [![Linter: flake8](https://img.shields.io/badge/%20linter-flake8-%231674b1?style=flat&labelColor=ef8336)](https://flake8.pycqa.org/en/latest/)
 
 ---
 
 ## Release Notes
+### V0.9.1
+ - Fix lint error
+ - Change v*_swap_exact_in_from_balance payer_is_sender default to False. This parameter will be removed in the next version.
 ### V0.9.0
  - Add support for UNWRAP_WETH encoding
  - Add v2_swap_exact_in_from_balance() and v3_swap_exact_in_from_balance(): 2 convenient methods which are used when the exact in_amount is not known when the transaction is built, typically chained after a V*_SWAP_EXACT_IN.
 ### V0.8.0
  - Breaking changes because of refactoring
  - Command chaining extension: all supported UR functions can now be chained in a single transaction
 
 ---
 
 ## Overview and Points of Attention
 
 The object of this library is to decode & encode the transaction input sent to the Uniswap universal router (UR)
-(address [`0x3fC91A3afd70395Cd496C647d5a6CC9D4B2b7FAD`](https://etherscan.io/address/0xEf1c6E67703c7BD7107eed8303Fbe6EC2554BF6B) 
+(address [`0x3fC91A3afd70395Cd496C647d5a6CC9D4B2b7FAD`](https://etherscan.io/address/0x3fC91A3afd70395Cd496C647d5a6CC9D4B2b7FAD) 
 on Ethereum Mainnet). It is based on, and is intended to be used with [web3.py](https://github.com/ethereum/web3.py)
 
 ⚠ This library has not been audited, so use at your own risk !
 
 ⚠ This project is a work in progress so not all commands are decoded yet. Below the list of the already implemented ones.
 
 | Command Id | Function Name | Decode | Encode
@@ -165,15 +168,15 @@
 And then the decoder will get the transaction from the blockchain and decode it, along with its input data:
 ```python
 trx_hash = "0x52e63b7 ... 11b979dd9"
 decoded_transaction = codec.decode.transaction(trx_hash)
 ```
 
 ### How to decode an Uniswap V3 swap path
-The `RouterCodec` class exposes also the method `decode.v3_path` which can be used to decode a given Uniswap V3 path.
+The `RouterCodec` class exposes also the method `decode.v3_path()` which can be used to decode a given Uniswap V3 path.
 
 ```python
 from uniswap_universal_router_decoder import RouterCodec
 
 uniswap_v3_path = b"\xc0*\xaa9\xb2#\xfe\x8d\n\x0e ... \xd7\x89"  # bytes or str hex
 fn_name = "V3_SWAP_EXACT_IN"  # Or V3_SWAP_EXACT_OUT
 codec = RouterCodec()
@@ -211,15 +214,15 @@
 # then in your transaction dict:
 transaction["data"] = encoded_data
 
 # you can now sign and send the transaction to the UR
 ```
 
 ### How to encode a call to the function V2_SWAP_EXACT_IN
-This function can be used to swap tokens on a V2 pool. Correct allowances must have been set before using sending such transaction.
+This function can be used to swap tokens on a V2 pool. Correct allowances must have been set before sending such transaction.
 ```python
 from uniswap_universal_router_decoder import FunctionRecipient, RouterCodec
 
 codec = RouterCodec()
 encoded_data = codec.encode.chain().v2_swap_exact_in(
         FunctionRecipient.SENDER,  # the output tokens are sent to the transaction sender
         amount_in,  # in Wei
@@ -233,15 +236,15 @@
 # then in your transaction dict:
 transaction["data"] = encoded_data
 
 # you can now sign and send the transaction to the UR
 ```
 
 ### How to encode a call to the function V2_SWAP_EXACT_OUT
-This function can be used to swap tokens on a V2 pool. Correct allowances must have been set before using sending such transaction.
+This function can be used to swap tokens on a V2 pool. Correct allowances must have been set before sending such transaction.
 ```python
 from uniswap_universal_router_decoder import FunctionRecipient, RouterCodec
 
 codec = RouterCodec()
 encoded_data = codec.encode.chain().v2_swap_exact_out(
         FunctionRecipient.SENDER,
         amount_out,  # in Wei
@@ -277,15 +280,15 @@
 # then in your transaction dict:
 transaction["data"] = encoded_data
 
 # you can now sign and send the transaction to the UR
 ```
 
 ### How to encode a call to the function V3_SWAP_EXACT_OUT
-This function can be used to swap tokens on a V3 pool. Correct allowances must have been set before using sending such transaction.
+This function can be used to swap tokens on a V3 pool. Correct allowances must have been set before sending such transaction.
 ```python
 from uniswap_universal_router_decoder import FunctionRecipient, RouterCodec
 
 codec = RouterCodec()
 encoded_data = codec.encode.chain().v3_swap_exact_out(
         FunctionRecipient.SENDER,
         amount_out,  # in Wei
@@ -310,15 +313,15 @@
 
 codec = RouterCodec()
 data, signable_message = codec.create_permit2_signable_message(
     token_address,
     amount,  # max = 2**160 - 1
     expiration,
     nonce,  # Permit2 nonce
-    spender,  # UR
+    spender,  # The UR checksum address
     deadline,
     1,  # chain id
 )
 
 # Then you need to sign the message:
 signed_message = acc.sign_message(signable_message)  # where acc is your LocalAccount
 
@@ -342,15 +345,15 @@
 
 # Permit signature
 data, signable_message = codec.create_permit2_signable_message(
     token_address,
     amount,  # max = 2**160 - 1
     expiration,
     nonce,  # Permit2 nonce
-    spender,  # UR
+    spender,  # The UR checksum address
     deadline,
     1,  # chain id
 )
 
 # Then you need to sign the message:
 signed_message = acc.sign_message(signable_message)  # where acc is your LocalAccount
```

### Comparing `uniswap-universal-router-decoder-0.9.0/README.md` & `uniswap-universal-router-decoder-0.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -15,27 +15,30 @@
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![Type Checker: mypy](https://img.shields.io/badge/%20type%20checker-mypy-%231674b1?style=flat&labelColor=ef8336)](https://mypy-lang.org/)
 [![Linter: flake8](https://img.shields.io/badge/%20linter-flake8-%231674b1?style=flat&labelColor=ef8336)](https://flake8.pycqa.org/en/latest/)
 
 ---
 
 ## Release Notes
+### V0.9.1
+ - Fix lint error
+ - Change v*_swap_exact_in_from_balance payer_is_sender default to False. This parameter will be removed in the next version.
 ### V0.9.0
  - Add support for UNWRAP_WETH encoding
  - Add v2_swap_exact_in_from_balance() and v3_swap_exact_in_from_balance(): 2 convenient methods which are used when the exact in_amount is not known when the transaction is built, typically chained after a V*_SWAP_EXACT_IN.
 ### V0.8.0
  - Breaking changes because of refactoring
  - Command chaining extension: all supported UR functions can now be chained in a single transaction
 
 ---
 
 ## Overview and Points of Attention
 
 The object of this library is to decode & encode the transaction input sent to the Uniswap universal router (UR)
-(address [`0x3fC91A3afd70395Cd496C647d5a6CC9D4B2b7FAD`](https://etherscan.io/address/0xEf1c6E67703c7BD7107eed8303Fbe6EC2554BF6B) 
+(address [`0x3fC91A3afd70395Cd496C647d5a6CC9D4B2b7FAD`](https://etherscan.io/address/0x3fC91A3afd70395Cd496C647d5a6CC9D4B2b7FAD) 
 on Ethereum Mainnet). It is based on, and is intended to be used with [web3.py](https://github.com/ethereum/web3.py)
 
 ⚠ This library has not been audited, so use at your own risk !
 
 ⚠ This project is a work in progress so not all commands are decoded yet. Below the list of the already implemented ones.
 
 | Command Id | Function Name | Decode | Encode
@@ -141,15 +144,15 @@
 And then the decoder will get the transaction from the blockchain and decode it, along with its input data:
 ```python
 trx_hash = "0x52e63b7 ... 11b979dd9"
 decoded_transaction = codec.decode.transaction(trx_hash)
 ```
 
 ### How to decode an Uniswap V3 swap path
-The `RouterCodec` class exposes also the method `decode.v3_path` which can be used to decode a given Uniswap V3 path.
+The `RouterCodec` class exposes also the method `decode.v3_path()` which can be used to decode a given Uniswap V3 path.
 
 ```python
 from uniswap_universal_router_decoder import RouterCodec
 
 uniswap_v3_path = b"\xc0*\xaa9\xb2#\xfe\x8d\n\x0e ... \xd7\x89"  # bytes or str hex
 fn_name = "V3_SWAP_EXACT_IN"  # Or V3_SWAP_EXACT_OUT
 codec = RouterCodec()
@@ -187,15 +190,15 @@
 # then in your transaction dict:
 transaction["data"] = encoded_data
 
 # you can now sign and send the transaction to the UR
 ```
 
 ### How to encode a call to the function V2_SWAP_EXACT_IN
-This function can be used to swap tokens on a V2 pool. Correct allowances must have been set before using sending such transaction.
+This function can be used to swap tokens on a V2 pool. Correct allowances must have been set before sending such transaction.
 ```python
 from uniswap_universal_router_decoder import FunctionRecipient, RouterCodec
 
 codec = RouterCodec()
 encoded_data = codec.encode.chain().v2_swap_exact_in(
         FunctionRecipient.SENDER,  # the output tokens are sent to the transaction sender
         amount_in,  # in Wei
@@ -209,15 +212,15 @@
 # then in your transaction dict:
 transaction["data"] = encoded_data
 
 # you can now sign and send the transaction to the UR
 ```
 
 ### How to encode a call to the function V2_SWAP_EXACT_OUT
-This function can be used to swap tokens on a V2 pool. Correct allowances must have been set before using sending such transaction.
+This function can be used to swap tokens on a V2 pool. Correct allowances must have been set before sending such transaction.
 ```python
 from uniswap_universal_router_decoder import FunctionRecipient, RouterCodec
 
 codec = RouterCodec()
 encoded_data = codec.encode.chain().v2_swap_exact_out(
         FunctionRecipient.SENDER,
         amount_out,  # in Wei
@@ -253,15 +256,15 @@
 # then in your transaction dict:
 transaction["data"] = encoded_data
 
 # you can now sign and send the transaction to the UR
 ```
 
 ### How to encode a call to the function V3_SWAP_EXACT_OUT
-This function can be used to swap tokens on a V3 pool. Correct allowances must have been set before using sending such transaction.
+This function can be used to swap tokens on a V3 pool. Correct allowances must have been set before sending such transaction.
 ```python
 from uniswap_universal_router_decoder import FunctionRecipient, RouterCodec
 
 codec = RouterCodec()
 encoded_data = codec.encode.chain().v3_swap_exact_out(
         FunctionRecipient.SENDER,
         amount_out,  # in Wei
@@ -286,15 +289,15 @@
 
 codec = RouterCodec()
 data, signable_message = codec.create_permit2_signable_message(
     token_address,
     amount,  # max = 2**160 - 1
     expiration,
     nonce,  # Permit2 nonce
-    spender,  # UR
+    spender,  # The UR checksum address
     deadline,
     1,  # chain id
 )
 
 # Then you need to sign the message:
 signed_message = acc.sign_message(signable_message)  # where acc is your LocalAccount
 
@@ -318,15 +321,15 @@
 
 # Permit signature
 data, signable_message = codec.create_permit2_signable_message(
     token_address,
     amount,  # max = 2**160 - 1
     expiration,
     nonce,  # Permit2 nonce
-    spender,  # UR
+    spender,  # The UR checksum address
     deadline,
     1,  # chain id
 )
 
 # Then you need to sign the message:
 signed_message = acc.sign_message(signable_message)  # where acc is your LocalAccount
```

### Comparing `uniswap-universal-router-decoder-0.9.0/pyproject.toml` & `uniswap-universal-router-decoder-0.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "uniswap-universal-router-decoder"
-version = "0.9.0"
+version = "0.9.1"
 authors = [
   { name="Elnaril", email="elnaril_dev@caramail.com" },
 ]
 description = "Decode & Encode transaction data sent to Uniswap Universal Router"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `uniswap-universal-router-decoder-0.9.0/tests/test_abi_builder.py` & `uniswap-universal-router-decoder-0.9.1/tests/test_abi_builder.py`

 * *Files identical despite different names*

### Comparing `uniswap-universal-router-decoder-0.9.0/tests/test_decoder.py` & `uniswap-universal-router-decoder-0.9.1/tests/test_decoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     decoded_trx = codec_w3.decode.transaction(trx_hash)
     command_inputs = decoded_trx["decoded_input"]["inputs"]
     assert len(command_inputs) == len(expected_fct_names)
     for i, expected_name in enumerate(expected_fct_names):
         if expected_name:
             assert expected_name == command_inputs[i][0].fn_name
         else:
-            assert type(command_inputs[i]) == str
+            assert isinstance(command_inputs[i], str)
             int(command_inputs[i], 16)  # check the str is actually a hex
 
 
 # Test Decode V3 Path
 
 expected_parsed_path_02 = (
     Web3.to_checksum_address("0x4d224452801ACEd8B2F0aebE155379bb5D594381"),
```

### Comparing `uniswap-universal-router-decoder-0.9.0/tests/test_encoder.py` & `uniswap-universal-router-decoder-0.9.1/tests/test_encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,17 +61,17 @@
     encoded_input = codec.encode.chain().v2_swap_exact_in_from_balance(
         FunctionRecipient.SENDER,
         Wei(0),
         [
             Web3.to_checksum_address("0xB4FBF271143F4FBf7B91A5ded31805e42b2208d6"),
             Web3.to_checksum_address("0x326C977E6efc84E512bB9C30f76E30c160eD06FB"),
         ],
-        payer_is_sender=True,
+        payer_is_sender=False,
     ).build(1676919287)
-    assert encoded_input == HexStr("0x3593564c000000000000000000000000000000000000000000000000000000000000006000000000000000000000000000000000000000000000000000000000000000a00000000000000000000000000000000000000000000000000000000063f3c1f70000000000000000000000000000000000000000000000000000000000000001080000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000010000000000000000000000000000000000000000000000000000000000000020000000000000000000000000000000000000000000000000000000000000010000000000000000000000000000000000000000000000000000000000000000018000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000a000000000000000000000000000000000000000000000000000000000000000010000000000000000000000000000000000000000000000000000000000000002000000000000000000000000b4fbf271143f4fbf7b91a5ded31805e42b2208d6000000000000000000000000326c977e6efc84e512bb9c30f76e30c160ed06fb")  # noqa E501
+    assert encoded_input == HexStr("0x3593564c000000000000000000000000000000000000000000000000000000000000006000000000000000000000000000000000000000000000000000000000000000a00000000000000000000000000000000000000000000000000000000063f3c1f70000000000000000000000000000000000000000000000000000000000000001080000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000010000000000000000000000000000000000000000000000000000000000000020000000000000000000000000000000000000000000000000000000000000010000000000000000000000000000000000000000000000000000000000000000018000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000a000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000002000000000000000000000000b4fbf271143f4fbf7b91a5ded31805e42b2208d6000000000000000000000000326c977e6efc84e512bb9c30f76e30c160ed06fb")  # noqa E501
 
 
 def test_chain_v2_swap_exact_out(codec):
     # https://etherscan.io/tx/0xd3abc2fe01376ebaff699a944ae3fb94b00ab899e8ed845a5e22ae120e83cb9e
     encoded_input = codec.encode.chain().v2_swap_exact_out(
         FunctionRecipient.SENDER,
         Wei(5000000000000000000000000),
@@ -144,17 +144,17 @@
         [
             Web3.to_checksum_address("0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48"),
             500,
             Web3.to_checksum_address("0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2"),
             500,
             Web3.to_checksum_address("0x2260FAC5E5542a773Aa44fBCfeDf7C193bc2C599"),
         ],
-        payer_is_sender=True,
+        payer_is_sender=False,
     ).build(1677080627)
-    assert encoded_input == HexStr("0x3593564c000000000000000000000000000000000000000000000000000000000000006000000000000000000000000000000000000000000000000000000000000000a00000000000000000000000000000000000000000000000000000000063f63833000000000000000000000000000000000000000000000000000000000000000100000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001000000000000000000000000000000000000000000000000000000000000002000000000000000000000000000000000000000000000000000000000000001200000000000000000000000000000000000000000000000000000000000000001800000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000383747ae00000000000000000000000000000000000000000000000000000000000000a000000000000000000000000000000000000000000000000000000000000000010000000000000000000000000000000000000000000000000000000000000042a0b86991c6218b36c1d19d4a2e9eb0ce3606eb480001f4c02aaa39b223fe8d0a0e5c4f27ead9083c756cc20001f42260fac5e5542a773aa44fbcfedf7c193bc2c599000000000000000000000000000000000000000000000000000000000000")  # noqa E501
+    assert encoded_input == HexStr("0x3593564c000000000000000000000000000000000000000000000000000000000000006000000000000000000000000000000000000000000000000000000000000000a00000000000000000000000000000000000000000000000000000000063f63833000000000000000000000000000000000000000000000000000000000000000100000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001000000000000000000000000000000000000000000000000000000000000002000000000000000000000000000000000000000000000000000000000000001200000000000000000000000000000000000000000000000000000000000000001800000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000383747ae00000000000000000000000000000000000000000000000000000000000000a000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000042a0b86991c6218b36c1d19d4a2e9eb0ce3606eb480001f4c02aaa39b223fe8d0a0e5c4f27ead9083c756cc20001f42260fac5e5542a773aa44fbcfedf7c193bc2c599000000000000000000000000000000000000000000000000000000000000")  # noqa E501
 
 
 def test_chain_v3_swap_exact_out(codec):
     # https://etherscan.io/tx/0x6aa16d2af66a8d960ce459abdd0a9018e35b2338cd3d2eb52b1280cc5a5f93ff
     encoded_input = codec.encode.chain().v3_swap_exact_out(
         FunctionRecipient.SENDER,
         Wei(40_000 * 10**18),
```

### Comparing `uniswap-universal-router-decoder-0.9.0/uniswap_universal_router_decoder/_abi_builder.py` & `uniswap-universal-router-decoder-0.9.1/uniswap_universal_router_decoder/_abi_builder.py`

 * *Files identical despite different names*

### Comparing `uniswap-universal-router-decoder-0.9.0/uniswap_universal_router_decoder/_constants.py` & `uniswap-universal-router-decoder-0.9.1/uniswap_universal_router_decoder/_constants.py`

 * *Files identical despite different names*

### Comparing `uniswap-universal-router-decoder-0.9.0/uniswap_universal_router_decoder/_decoder.py` & `uniswap-universal-router-decoder-0.9.1/uniswap_universal_router_decoder/_decoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         :param path: the V3 path as returned by decode_function_input() or decode_transaction()
         :return: a tuple of token addresses separated by the corresponding pool fees, first token being the 'in-token',
         last token being the 'out-token'
         """
         valid_fn_names = ("V3_SWAP_EXACT_IN", "V3_SWAP_EXACT_OUT")
         if v3_fn_name.upper() not in valid_fn_names:
             raise ValueError(f"v3_fn_name must be in {valid_fn_names}")
-        path_str = path.hex() if type(path) == bytes else str(path)
+        path_str = path.hex() if isinstance(path, bytes) else str(path)
         path_str = path_str[2:] if path_str.startswith("0x") else path_str
         path_list: List[Union[int, ChecksumAddress]] = [Web3.to_checksum_address(path_str[0:40]), ]
         parsed_remaining_path: List[List[Union[int, ChecksumAddress]]] = [
             [
                 int(path_str[40:][i:i + 6], 16),
                 Web3.to_checksum_address(path_str[40:][i + 6:i + 46]),
             ]
```

### Comparing `uniswap-universal-router-decoder-0.9.0/uniswap_universal_router_decoder/_encoder.py` & `uniswap-universal-router-decoder-0.9.1/uniswap_universal_router_decoder/_encoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,26 +211,26 @@
 
     def v2_swap_exact_in_from_balance(
             self,
             function_recipient: FunctionRecipient,
             amount_out_min: Wei,
             path: Sequence[ChecksumAddress],
             custom_recipient: Optional[ChecksumAddress] = None,
-            payer_is_sender: bool = True) -> _ChainedFunctionBuilder:
+            payer_is_sender: bool = False) -> _ChainedFunctionBuilder:
         """
         Encode the call to the function V2_SWAP_EXACT_IN, using the router balance as amount_in,
         which swaps tokens on Uniswap V2.
         Typically used when the amount_in is unknown because it comes from a V*_SWAP_EXACT_IN output.
         Correct allowances must have been set before sending such transaction.
 
         :param function_recipient: A FunctionRecipient which defines the recipient of this function output.
         :param amount_out_min: The minimum accepted bought token (token_out)
         :param path: The V2 path: a list of 2 or 3 tokens where the first is token_in and the last is token_out
         :param custom_recipient: If function_recipient is CUSTOM, must be the actual recipient, otherwise None.
-        :param payer_is_sender: True if the in tokens come from the sender, False if they already are in the router
+        :param payer_is_sender: Always False. Will be removed in next version
         :return: The chain link corresponding to this function call.
         """
         return self.v2_swap_exact_in(
             function_recipient,
             _RouterConstant.ROUTER_BALANCE.value,
             amount_out_min,
             path,
@@ -338,27 +338,27 @@
 
     def v3_swap_exact_in_from_balance(
             self,
             function_recipient: FunctionRecipient,
             amount_out_min: Wei,
             path: Sequence[Union[int, ChecksumAddress]],
             custom_recipient: Optional[ChecksumAddress] = None,
-            payer_is_sender: bool = True) -> _ChainedFunctionBuilder:
+            payer_is_sender: bool = False) -> _ChainedFunctionBuilder:
         """
         Encode the call to the function V3_SWAP_EXACT_IN, using the router balance as amount_in,
         which swaps tokens on Uniswap V3.
         Typically used when the amount_in is unknown because it comes from a V*_SWAP_EXACT_IN output.
         Correct allowances must have been set before sending such transaction.
 
         :param function_recipient: A FunctionRecipient which defines the recipient of this function output.
         :param amount_out_min: The minimum accepted bought token (token_out) in Wei
         :param path: The V3 path: a list of tokens where the first is the token_in, the last one is the token_out, and
         with the pool fee between each token in basis points (ex: 3000 for 0.3%)
         :param custom_recipient: If function_recipient is CUSTOM, must be the actual recipient, otherwise None.
-        :param payer_is_sender: True if the in tokens come from the sender, False if they already are in the router
+        :param payer_is_sender: Always False. Will be removed in next version
         :return: The chain link corresponding to this function call.
         """
         return self.v3_swap_exact_in(
             function_recipient,
             _RouterConstant.ROUTER_BALANCE.value,
             amount_out_min,
             path,
```

### Comparing `uniswap-universal-router-decoder-0.9.0/uniswap_universal_router_decoder/_enums.py` & `uniswap-universal-router-decoder-0.9.1/uniswap_universal_router_decoder/_enums.py`

 * *Files identical despite different names*

### Comparing `uniswap-universal-router-decoder-0.9.0/uniswap_universal_router_decoder/router_codec.py` & `uniswap-universal-router-decoder-0.9.1/uniswap_universal_router_decoder/router_codec.py`

 * *Files identical despite different names*

### Comparing `uniswap-universal-router-decoder-0.9.0/uniswap_universal_router_decoder.egg-info/PKG-INFO` & `uniswap-universal-router-decoder-0.9.1/uniswap_universal_router_decoder.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uniswap-universal-router-decoder
-Version: 0.9.0
+Version: 0.9.1
 Summary: Decode & Encode transaction data sent to Uniswap Universal Router
 Author-email: Elnaril <elnaril_dev@caramail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/Elnaril/uniswap-universal-router-decoder
 Project-URL: Bug Tracker, https://github.com/Elnaril/uniswap-universal-router-decoder/issues
 Project-URL: Fiverr, https://www.fiverr.com/elnaril
 Keywords: blockchain,ethereum,uniswap,universal router,decoder,encoder,codec,wrapper
@@ -39,27 +39,30 @@
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![Type Checker: mypy](https://img.shields.io/badge/%20type%20checker-mypy-%231674b1?style=flat&labelColor=ef8336)](https://mypy-lang.org/)
 [![Linter: flake8](https://img.shields.io/badge/%20linter-flake8-%231674b1?style=flat&labelColor=ef8336)](https://flake8.pycqa.org/en/latest/)
 
 ---
 
 ## Release Notes
+### V0.9.1
+ - Fix lint error
+ - Change v*_swap_exact_in_from_balance payer_is_sender default to False. This parameter will be removed in the next version.
 ### V0.9.0
  - Add support for UNWRAP_WETH encoding
  - Add v2_swap_exact_in_from_balance() and v3_swap_exact_in_from_balance(): 2 convenient methods which are used when the exact in_amount is not known when the transaction is built, typically chained after a V*_SWAP_EXACT_IN.
 ### V0.8.0
  - Breaking changes because of refactoring
  - Command chaining extension: all supported UR functions can now be chained in a single transaction
 
 ---
 
 ## Overview and Points of Attention
 
 The object of this library is to decode & encode the transaction input sent to the Uniswap universal router (UR)
-(address [`0x3fC91A3afd70395Cd496C647d5a6CC9D4B2b7FAD`](https://etherscan.io/address/0xEf1c6E67703c7BD7107eed8303Fbe6EC2554BF6B) 
+(address [`0x3fC91A3afd70395Cd496C647d5a6CC9D4B2b7FAD`](https://etherscan.io/address/0x3fC91A3afd70395Cd496C647d5a6CC9D4B2b7FAD) 
 on Ethereum Mainnet). It is based on, and is intended to be used with [web3.py](https://github.com/ethereum/web3.py)
 
 ⚠ This library has not been audited, so use at your own risk !
 
 ⚠ This project is a work in progress so not all commands are decoded yet. Below the list of the already implemented ones.
 
 | Command Id | Function Name | Decode | Encode
@@ -165,15 +168,15 @@
 And then the decoder will get the transaction from the blockchain and decode it, along with its input data:
 ```python
 trx_hash = "0x52e63b7 ... 11b979dd9"
 decoded_transaction = codec.decode.transaction(trx_hash)
 ```
 
 ### How to decode an Uniswap V3 swap path
-The `RouterCodec` class exposes also the method `decode.v3_path` which can be used to decode a given Uniswap V3 path.
+The `RouterCodec` class exposes also the method `decode.v3_path()` which can be used to decode a given Uniswap V3 path.
 
 ```python
 from uniswap_universal_router_decoder import RouterCodec
 
 uniswap_v3_path = b"\xc0*\xaa9\xb2#\xfe\x8d\n\x0e ... \xd7\x89"  # bytes or str hex
 fn_name = "V3_SWAP_EXACT_IN"  # Or V3_SWAP_EXACT_OUT
 codec = RouterCodec()
@@ -211,15 +214,15 @@
 # then in your transaction dict:
 transaction["data"] = encoded_data
 
 # you can now sign and send the transaction to the UR
 ```
 
 ### How to encode a call to the function V2_SWAP_EXACT_IN
-This function can be used to swap tokens on a V2 pool. Correct allowances must have been set before using sending such transaction.
+This function can be used to swap tokens on a V2 pool. Correct allowances must have been set before sending such transaction.
 ```python
 from uniswap_universal_router_decoder import FunctionRecipient, RouterCodec
 
 codec = RouterCodec()
 encoded_data = codec.encode.chain().v2_swap_exact_in(
         FunctionRecipient.SENDER,  # the output tokens are sent to the transaction sender
         amount_in,  # in Wei
@@ -233,15 +236,15 @@
 # then in your transaction dict:
 transaction["data"] = encoded_data
 
 # you can now sign and send the transaction to the UR
 ```
 
 ### How to encode a call to the function V2_SWAP_EXACT_OUT
-This function can be used to swap tokens on a V2 pool. Correct allowances must have been set before using sending such transaction.
+This function can be used to swap tokens on a V2 pool. Correct allowances must have been set before sending such transaction.
 ```python
 from uniswap_universal_router_decoder import FunctionRecipient, RouterCodec
 
 codec = RouterCodec()
 encoded_data = codec.encode.chain().v2_swap_exact_out(
         FunctionRecipient.SENDER,
         amount_out,  # in Wei
@@ -277,15 +280,15 @@
 # then in your transaction dict:
 transaction["data"] = encoded_data
 
 # you can now sign and send the transaction to the UR
 ```
 
 ### How to encode a call to the function V3_SWAP_EXACT_OUT
-This function can be used to swap tokens on a V3 pool. Correct allowances must have been set before using sending such transaction.
+This function can be used to swap tokens on a V3 pool. Correct allowances must have been set before sending such transaction.
 ```python
 from uniswap_universal_router_decoder import FunctionRecipient, RouterCodec
 
 codec = RouterCodec()
 encoded_data = codec.encode.chain().v3_swap_exact_out(
         FunctionRecipient.SENDER,
         amount_out,  # in Wei
@@ -310,15 +313,15 @@
 
 codec = RouterCodec()
 data, signable_message = codec.create_permit2_signable_message(
     token_address,
     amount,  # max = 2**160 - 1
     expiration,
     nonce,  # Permit2 nonce
-    spender,  # UR
+    spender,  # The UR checksum address
     deadline,
     1,  # chain id
 )
 
 # Then you need to sign the message:
 signed_message = acc.sign_message(signable_message)  # where acc is your LocalAccount
 
@@ -342,15 +345,15 @@
 
 # Permit signature
 data, signable_message = codec.create_permit2_signable_message(
     token_address,
     amount,  # max = 2**160 - 1
     expiration,
     nonce,  # Permit2 nonce
-    spender,  # UR
+    spender,  # The UR checksum address
     deadline,
     1,  # chain id
 )
 
 # Then you need to sign the message:
 signed_message = acc.sign_message(signable_message)  # where acc is your LocalAccount
```

### Comparing `uniswap-universal-router-decoder-0.9.0/uniswap_universal_router_decoder.egg-info/SOURCES.txt` & `uniswap-universal-router-decoder-0.9.1/uniswap_universal_router_decoder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

