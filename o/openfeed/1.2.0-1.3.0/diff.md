# Comparing `tmp/openfeed-1.2.0.tar.gz` & `tmp/openfeed-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/tmp/tmpm514ljpl/tmp8eupmvd9/openfeed-1.2.0.tar", last modified: Wed Jun  8 17:19:33 2022, max compression
+gzip compressed data, was "/tmp/tmpzo5u7lyk/.tmp-ihf59094/openfeed-1.3.0.tar", last modified: Fri Aug  4 15:57:20 2023, max compression
```

## Comparing `openfeed-1.2.0.tar` & `openfeed-1.3.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-08 17:19:33.000000 openfeed-1.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-08 17:19:33.000000 openfeed-1.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-08 17:19:33.000000 openfeed-1.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)     1073 2022-06-08 17:19:21.000000 openfeed-1.2.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (116)     2253 2022-06-08 17:19:21.000000 openfeed-1.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)     1090 2022-06-08 17:19:21.000000 openfeed-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     2212 2022-06-08 17:19:33.000000 openfeed-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1831 2022-06-08 17:19:21.000000 openfeed-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (116)      341 2022-06-08 17:19:21.000000 openfeed-1.2.0/build.sh
--rw-r--r--   0 runner    (1001) docker     (116)     1551 2022-06-08 17:19:21.000000 openfeed-1.2.0/example.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-08 17:19:33.000000 openfeed-1.2.0/openfeed/
--rw-r--r--   0 runner    (1001) docker     (116)      247 2022-06-08 17:19:21.000000 openfeed-1.2.0/openfeed/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-08 17:19:33.000000 openfeed-1.2.0/openfeed/generated/
--rw-r--r--   0 runner    (1001) docker     (116)    80980 2022-06-08 17:19:21.000000 openfeed-1.2.0/openfeed/generated/openfeed_api_pb2.py
--rw-r--r--   0 runner    (1001) docker     (116)    61064 2022-06-08 17:19:21.000000 openfeed-1.2.0/openfeed/generated/openfeed_instrument_pb2.py
--rw-r--r--   0 runner    (1001) docker     (116)   320600 2022-06-08 17:19:21.000000 openfeed-1.2.0/openfeed/generated/openfeed_pb2.py
--rw-r--r--   0 runner    (1001) docker     (116)    24765 2022-06-08 17:19:21.000000 openfeed-1.2.0/openfeed/openfeed_client.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-08 17:19:33.000000 openfeed-1.2.0/openfeed.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     2212 2022-06-08 17:19:32.000000 openfeed-1.2.0/openfeed.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      455 2022-06-08 17:19:33.000000 openfeed-1.2.0/openfeed.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-06-08 17:19:32.000000 openfeed-1.2.0/openfeed.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       72 2022-06-08 17:19:33.000000 openfeed-1.2.0/openfeed.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        9 2022-06-08 17:19:33.000000 openfeed-1.2.0/openfeed.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-08 17:19:33.000000 openfeed-1.2.0/protos/
--rw-r--r--   0 runner    (1001) docker     (116)       75 2022-06-08 17:19:21.000000 openfeed-1.2.0/protos/README.md
--rw-r--r--   0 runner    (1001) docker     (116)      415 2022-06-08 17:19:21.000000 openfeed-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-06-08 17:19:33.000000 openfeed-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      900 2022-06-08 17:19:21.000000 openfeed-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:57:20.000000 openfeed-1.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:57:20.000000 openfeed-1.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:57:20.000000 openfeed-1.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-08-04 15:57:14.000000 openfeed-1.3.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-08-04 15:57:14.000000 openfeed-1.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-04 15:57:14.000000 openfeed-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-08-04 15:57:20.000000 openfeed-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-08-04 15:57:14.000000 openfeed-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-08-04 15:57:14.000000 openfeed-1.3.0/build.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-08-04 15:57:14.000000 openfeed-1.3.0/example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:57:20.000000 openfeed-1.3.0/openfeed/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-08-04 15:57:14.000000 openfeed-1.3.0/openfeed/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:57:20.000000 openfeed-1.3.0/openfeed/generated/
+-rw-r--r--   0 runner    (1001) docker     (123)    85067 2023-08-04 15:57:14.000000 openfeed-1.3.0/openfeed/generated/openfeed_api_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63876 2023-08-04 15:57:14.000000 openfeed-1.3.0/openfeed/generated/openfeed_instrument_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   321078 2023-08-04 15:57:14.000000 openfeed-1.3.0/openfeed/generated/openfeed_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27549 2023-08-04 15:57:14.000000 openfeed-1.3.0/openfeed/openfeed_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-04 15:57:14.000000 openfeed-1.3.0/openfeed/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:57:20.000000 openfeed-1.3.0/openfeed.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-08-04 15:57:20.000000 openfeed-1.3.0/openfeed.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-08-04 15:57:20.000000 openfeed-1.3.0/openfeed.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 15:57:20.000000 openfeed-1.3.0/openfeed.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-04 15:57:20.000000 openfeed-1.3.0/openfeed.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-04 15:57:20.000000 openfeed-1.3.0/openfeed.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:57:20.000000 openfeed-1.3.0/protos/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-08-04 15:57:14.000000 openfeed-1.3.0/protos/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-08-04 15:57:14.000000 openfeed-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 15:57:20.000000 openfeed-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-08-04 15:57:14.000000 openfeed-1.3.0/setup.py
```

### Comparing `openfeed-1.2.0/.github/workflows/publish-to-pypi.yml` & `openfeed-1.3.0/.github/workflows/publish-to-pypi.yml`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 name: PyPI and TestPyPI
 
 on: push
 
 jobs:
   build-n-publish:
     name: Build and publish package to PyPI and TestPyPI
-    runs-on: ubuntu-18.04
+    runs-on: ubuntu-22.04
     steps:
     - uses: actions/checkout@master
     - name: Set up Python 3.7
       uses: actions/setup-python@v1
       with:
         python-version: 3.7
     - name: Install pep517
@@ -23,19 +23,19 @@
         python -m
         pep517.build
         --source
         --binary
         --out-dir dist/
         .
     - name: Publish package to Test PyPI
-      uses: pypa/gh-action-pypi-publish@master
+      uses: pypa/gh-action-pypi-publish@release/v1
       with:
         password: ${{ secrets.test_pypi_token }}
         repository_url: https://test.pypi.org/legacy/
         skip_existing: true 
     - name: Publish package to PyPI
       if: startsWith(github.ref, 'refs/tags')
-      uses: pypa/gh-action-pypi-publish@master
+      uses: pypa/gh-action-pypi-publish@release/v1
       with:
         password: ${{ secrets.pypi_token }}
         skip_existing: true
```

### Comparing `openfeed-1.2.0/.gitignore` & `openfeed-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `openfeed-1.2.0/LICENSE` & `openfeed-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openfeed-1.2.0/PKG-INFO` & `openfeed-1.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openfeed
-Version: 1.2.0
+Version: 1.3.0
 Summary: Barchart Openfeed Example Client for Python
 Home-page: https://github.com/openfeed-org/sdk-python
 Download-URL: https://github.com/openfeed-org/sdk-python/archive/master.zip
 Author: Barchart
 Author-email: mike@barchart.com
 License: MIT
 Description-Content-Type: text/markdown
@@ -56,17 +56,21 @@
 of-client: Connected
 of-client: Market Data:  subscriptionResponse
 of-client: Market Data:  marketSnapshot
 of-client: Market Data:  marketUpdate
 of-client: Market Data:  marketUpdate
 ```
 
+### Openfeed Documentation
+
+* [https://docs.barchart.com/openfeed](https://docs.barchart.com/openfeed)
+
 ## Subscription Types
 
-Openfeed supports many levels of [subscription types](https://openfeed-org.github.io/documentation/Message%20Specification/#org.openfeed.SubscriptionType).
+Openfeed supports many levels of [subscription types](https://docs.barchart.com/openfeed/#/proto?id=subscriptiontype).
 
 ### OHLC
 
 ```python
 of_client.add_exchange_subscription(["NYSE"], callback=on_message, subscription_type=["OHLC"])
 ```
```

### Comparing `openfeed-1.2.0/README.md` & `openfeed-1.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -43,17 +43,21 @@
 of-client: Connected
 of-client: Market Data:  subscriptionResponse
 of-client: Market Data:  marketSnapshot
 of-client: Market Data:  marketUpdate
 of-client: Market Data:  marketUpdate
 ```
 
+### Openfeed Documentation
+
+* [https://docs.barchart.com/openfeed](https://docs.barchart.com/openfeed)
+
 ## Subscription Types
 
-Openfeed supports many levels of [subscription types](https://openfeed-org.github.io/documentation/Message%20Specification/#org.openfeed.SubscriptionType).
+Openfeed supports many levels of [subscription types](https://docs.barchart.com/openfeed/#/proto?id=subscriptiontype).
 
 ### OHLC
 
 ```python
 of_client.add_exchange_subscription(["NYSE"], callback=on_message, subscription_type=["OHLC"])
 ```
```

### Comparing `openfeed-1.2.0/example.py` & `openfeed-1.3.0/example.py`

 * *Files identical despite different names*

### Comparing `openfeed-1.2.0/openfeed/generated/openfeed_api_pb2.py` & `openfeed-1.3.0/openfeed/generated/openfeed_api_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='openfeed_api.proto',
   package='org.openfeed',
   syntax='proto3',
   serialized_options=b'H\001P\001\240\001\001',
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n\x12openfeed_api.proto\x12\x0corg.openfeed\x1a\x19openfeed_instrument.proto\x1a\x0eopenfeed.proto\"\x94\x03\n\x16OpenfeedGatewayRequest\x12\x32\n\x0cloginRequest\x18\x01 \x01(\x0b\x32\x1a.org.openfeed.LoginRequestH\x00\x12\x34\n\rlogoutRequest\x18\x02 \x01(\x0b\x32\x1b.org.openfeed.LogoutRequestH\x00\x12@\n\x13subscriptionRequest\x18\x03 \x01(\x0b\x32!.org.openfeed.SubscriptionRequestH\x00\x12<\n\x11instrumentRequest\x18\x04 \x01(\x0b\x32\x1f.org.openfeed.InstrumentRequestH\x00\x12N\n\x1ainstrumentReferenceRequest\x18\x05 \x01(\x0b\x32(.org.openfeed.InstrumentReferenceRequestH\x00\x12\x38\n\x0f\x65xchangeRequest\x18\x06 \x01(\x0b\x32\x1d.org.openfeed.ExchangeRequestH\x00\x42\x06\n\x04\x64\x61ta\"\xc8\x06\n\x16OpenfeedGatewayMessage\x12\x34\n\rloginResponse\x18\x01 \x01(\x0b\x32\x1b.org.openfeed.LoginResponseH\x00\x12\x36\n\x0elogoutResponse\x18\x02 \x01(\x0b\x32\x1c.org.openfeed.LogoutResponseH\x00\x12>\n\x12instrumentResponse\x18\x03 \x01(\x0b\x32 .org.openfeed.InstrumentResponseH\x00\x12P\n\x1binstrumentReferenceResponse\x18\x04 \x01(\x0b\x32).org.openfeed.InstrumentReferenceResponseH\x00\x12\x42\n\x14subscriptionResponse\x18\x05 \x01(\x0b\x32\".org.openfeed.SubscriptionResponseH\x00\x12\x32\n\x0cmarketStatus\x18\x06 \x01(\x0b\x32\x1a.org.openfeed.MarketStatusH\x00\x12,\n\theartBeat\x18\x07 \x01(\x0b\x32\x17.org.openfeed.HeartBeatH\x00\x12\x42\n\x14instrumentDefinition\x18\x08 \x01(\x0b\x32\".org.openfeed.InstrumentDefinitionH\x00\x12\x36\n\x0emarketSnapshot\x18\t \x01(\x0b\x32\x1c.org.openfeed.MarketSnapshotH\x00\x12\x32\n\x0cmarketUpdate\x18\n \x01(\x0b\x32\x1a.org.openfeed.MarketUpdateH\x00\x12\x34\n\rvolumeAtPrice\x18\x0b \x01(\x0b\x32\x1b.org.openfeed.VolumeAtPriceH\x00\x12\"\n\x04ohlc\x18\x0c \x01(\x0b\x32\x12.org.openfeed.OhlcH\x00\x12:\n\x10\x65xchangeResponse\x18\r \x01(\x0b\x32\x1e.org.openfeed.ExchangeResponseH\x00\x12:\n\x10instrumentAction\x18\x0e \x01(\x0b\x32\x1e.org.openfeed.InstrumentActionH\x00\x42\x06\n\x04\x64\x61ta\"g\n\x06Status\x12$\n\x06result\x18\x01 \x01(\x0e\x32\x14.org.openfeed.Result\x12\x0f\n\x07message\x18\x02 \x01(\t\x12&\n\x07service\x18\x03 \x01(\x0e\x32\x15.org.openfeed.Service\"y\n\x0cLoginRequest\x12\x15\n\rcorrelationId\x18\x01 \x01(\x12\x12\x10\n\x08username\x18\x02 \x01(\t\x12\x10\n\x08password\x18\x03 \x01(\t\x12\x15\n\rclientVersion\x18\x04 \x01(\t\x12\x17\n\x0fprotocolVersion\x18\x05 \x01(\x11\"[\n\rLoginResponse\x12\x15\n\rcorrelationId\x18\x01 \x01(\x12\x12$\n\x06status\x18\x02 \x01(\x0b\x32\x14.org.openfeed.Status\x12\r\n\x05token\x18\x03 \x01(\t\"5\n\rLogoutRequest\x12\x15\n\rcorrelationId\x18\x01 \x01(\x12\x12\r\n\x05token\x18\x03 \x01(\t\"M\n\x0eLogoutResponse\x12\x15\n\rcorrelationId\x18\x01 \x01(\x12\x12$\n\x06status\x18\x02 \x01(\x0b\x32\x14.org.openfeed.Status\"\x93\x01\n\x11InstrumentRequest\x12\x15\n\rcorrelationId\x18\x01 \x01(\x12\x12\r\n\x05token\x18\x02 \x01(\t\x12\x10\n\x06symbol\x18\n \x01(\tH\x00\x12\x12\n\x08marketId\x18\x0b \x01(\x12H\x00\x12\x12\n\x08\x65xchange\x18\x0c \x01(\tH\x00\x12\x13\n\tchannelId\x18\r \x01(\x11H\x00\x42\t\n\x07request\"\xb5\x01\n\x12InstrumentResponse\x12\x15\n\rcorrelationId\x18\x01 \x01(\x12\x12$\n\x06status\x18\x02 \x01(\x0b\x32\x14.org.openfeed.Status\x12\x1b\n\x13numberOfDefinitions\x18\x03 \x01(\x11\x12\x0e\n\x06symbol\x18\x04 \x01(\t\x12\x10\n\x08marketId\x18\x05 \x01(\x12\x12\x10\n\x08\x65xchange\x18\x06 \x01(\t\x12\x11\n\tchannelId\x18\x07 \x01(\x11\"\x9c\x01\n\x1aInstrumentReferenceRequest\x12\x15\n\rcorrelationId\x18\x01 \x01(\x12\x12\r\n\x05token\x18\x02 \x01(\t\x12\x10\n\x06symbol\x18\n \x01(\tH\x00\x12\x12\n\x08marketId\x18\x0b \x01(\x12H\x00\x12\x12\n\x08\x65xchange\x18\x0c \x01(\tH\x00\x12\x13\n\tchannelId\x18\r \x01(\x11H\x00\x42\t\n\x07request\"\x93\x02\n\x1bInstrumentReferenceResponse\x12\x15\n\rcorrelationId\x18\x01 \x01(\x12\x12$\n\x06status\x18\x02 \x01(\x0b\x32\x14.org.openfeed.Status\x12\x1b\n\x13numberOfDefinitions\x18\x03 \x01(\x11\x12\x11\n\tchannelId\x18\x04 \x01(\x11\x12\x10\n\x08marketId\x18\x05 \x01(\x12\x12\x0e\n\x06symbol\x18\x06 \x01(\t\x12\x10\n\x08\x65xchange\x18\x07 \x01(\t\x12\x11\n\tddfSymbol\x18\x08 \x01(\t\x12\x13\n\x0b\x64\x64\x66\x45xchange\x18\t \x01(\t\x12\x13\n\x0b\x64\x64\x66\x42\x61seCode\x18\n \x01(\t\x12\x16\n\x0e\x65xchangeSymbol\x18\x0b \x01(\t\"7\n\x0f\x45xchangeRequest\x12\x15\n\rcorrelationId\x18\x01 \x01(\x12\x12\r\n\x05token\x18\x02 \x01(\t\"\xcb\x01\n\x10\x45xchangeResponse\x12\x15\n\rcorrelationId\x18\x01 \x01(\x12\x12$\n\x06status\x18\x02 \x01(\x0b\x32\x14.org.openfeed.Status\x12:\n\texchanges\x18\x03 \x03(\x0b\x32\'.org.openfeed.ExchangeResponse.Exchange\x1a>\n\x08\x45xchange\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0f\n\x07\x61liases\x18\x03 \x03(\t\"\xbe\x03\n\x13SubscriptionRequest\x12\x15\n\rcorrelationId\x18\x01 \x01(\x12\x12\r\n\x05token\x18\x02 \x01(\t\x12&\n\x07service\x18\x03 \x01(\x0e\x32\x15.org.openfeed.Service\x12\x13\n\x0bunsubscribe\x18\x04 \x01(\x08\x12;\n\x08requests\x18\x05 \x03(\x0b\x32).org.openfeed.SubscriptionRequest.Request\x1a\x86\x02\n\x07Request\x12\x10\n\x06symbol\x18\x01 \x01(\tH\x00\x12\x12\n\x08marketId\x18\x02 \x01(\x12H\x00\x12\x12\n\x08\x65xchange\x18\x03 \x01(\tH\x00\x12\x13\n\tchannelId\x18\x04 \x01(\x11H\x00\x12\x38\n\x10subscriptionType\x18\n \x03(\x0e\x32\x1e.org.openfeed.SubscriptionType\x12\x1f\n\x17snapshotIntervalSeconds\x18\x0b \x01(\x11\x12I\n\x0einstrumentType\x18\x0c \x03(\x0e\x32\x31.org.openfeed.InstrumentDefinition.InstrumentTypeB\x06\n\x04\x64\x61ta\"\x86\x02\n\x14SubscriptionResponse\x12\x15\n\rcorrelationId\x18\x01 \x01(\x12\x12$\n\x06status\x18\x02 \x01(\x0b\x32\x14.org.openfeed.Status\x12\x0e\n\x06symbol\x18\x03 \x01(\t\x12\x10\n\x08marketId\x18\x04 \x01(\x12\x12\x10\n\x08\x65xchange\x18\x05 \x01(\t\x12\x11\n\tchannelId\x18\x06 \x01(\x11\x12\x1b\n\x13numberOfDefinitions\x18\x07 \x01(\x11\x12\x38\n\x10subscriptionType\x18\x08 \x01(\x0e\x32\x1e.org.openfeed.SubscriptionType\x12\x13\n\x0bunsubscribe\x18\t \x01(\x08*\xde\x02\n\x06Result\x12\x12\n\x0eUNKNOWN_RESULT\x10\x00\x12\x0b\n\x07SUCCESS\x10\x01\x12\x13\n\x0f\x44UPLICATE_LOGIN\x10s\x12\x12\n\x0eINVALID_SYMBOL\x10t\x12\x15\n\x11INVALID_MARKET_ID\x10u\x12\x14\n\x10INVALID_EXCHANGE\x10v\x12\x16\n\x12INVALID_CHANNEL_ID\x10w\x12\x15\n\x11MALFORMED_MESSAGE\x10x\x12\x16\n\x12UNEXPECTED_MESSAGE\x10y\x12\x12\n\x0eNOT_SUBSCRIBED\x10z\x12\x1a\n\x16\x44UPLICATE_SUBSCRIPTION\x10{\x12\x17\n\x13INVALID_CREDENTIALS\x10|\x12\x1b\n\x17INSUFFICIENT_PRIVILEGES\x10}\x12\x1b\n\x17\x41UTHENTICATION_REQUIRED\x10~\x12\x13\n\x0fGENERIC_FAILURE\x10\x7f*\xa1\x01\n\x10SubscriptionType\x12\x07\n\x03\x41LL\x10\x00\x12\t\n\x05QUOTE\x10\x01\x12\x15\n\x11QUOTE_PARTICIPANT\x10\x02\x12\x0f\n\x0b\x44\x45PTH_PRICE\x10\x03\x12\x0f\n\x0b\x44\x45PTH_ORDER\x10\x04\x12\n\n\x06TRADES\x10\x05\x12\x14\n\x10\x43UMLATIVE_VOLUME\x10\x06\x12\x08\n\x04OHLC\x10\x07\x12\x14\n\x10OHLC_NON_REGULAR\x10\x08\x42\x07H\x01P\x01\xa0\x01\x01\x62\x06proto3'
+  serialized_pb=b'\n\x12openfeed_api.proto\x12\x0corg.openfeed\x1a\x19openfeed_instrument.proto\x1a\x0eopenfeed.proto\"\x94\x03\n\x16OpenfeedGatewayRequest\x12\x32\n\x0cloginRequest\x18\x01 \x01(\x0b\x32\x1a.org.openfeed.LoginRequestH\x00\x12\x34\n\rlogoutRequest\x18\x02 \x01(\x0b\x32\x1b.org.openfeed.LogoutRequestH\x00\x12@\n\x13subscriptionRequest\x18\x03 \x01(\x0b\x32!.org.openfeed.SubscriptionRequestH\x00\x12<\n\x11instrumentRequest\x18\x04 \x01(\x0b\x32\x1f.org.openfeed.InstrumentRequestH\x00\x12N\n\x1ainstrumentReferenceRequest\x18\x05 \x01(\x0b\x32(.org.openfeed.InstrumentReferenceRequestH\x00\x12\x38\n\x0f\x65xchangeRequest\x18\x06 \x01(\x0b\x32\x1d.org.openfeed.ExchangeRequestH\x00\x42\x06\n\x04\x64\x61ta\"\xc8\x06\n\x16OpenfeedGatewayMessage\x12\x34\n\rloginResponse\x18\x01 \x01(\x0b\x32\x1b.org.openfeed.LoginResponseH\x00\x12\x36\n\x0elogoutResponse\x18\x02 \x01(\x0b\x32\x1c.org.openfeed.LogoutResponseH\x00\x12>\n\x12instrumentResponse\x18\x03 \x01(\x0b\x32 .org.openfeed.InstrumentResponseH\x00\x12P\n\x1binstrumentReferenceResponse\x18\x04 \x01(\x0b\x32).org.openfeed.InstrumentReferenceResponseH\x00\x12\x42\n\x14subscriptionResponse\x18\x05 \x01(\x0b\x32\".org.openfeed.SubscriptionResponseH\x00\x12\x32\n\x0cmarketStatus\x18\x06 \x01(\x0b\x32\x1a.org.openfeed.MarketStatusH\x00\x12,\n\theartBeat\x18\x07 \x01(\x0b\x32\x17.org.openfeed.HeartBeatH\x00\x12\x42\n\x14instrumentDefinition\x18\x08 \x01(\x0b\x32\".org.openfeed.InstrumentDefinitionH\x00\x12\x36\n\x0emarketSnapshot\x18\t \x01(\x0b\x32\x1c.org.openfeed.MarketSnapshotH\x00\x12\x32\n\x0cmarketUpdate\x18\n \x01(\x0b\x32\x1a.org.openfeed.MarketUpdateH\x00\x12\x34\n\rvolumeAtPrice\x18\x0b \x01(\x0b\x32\x1b.org.openfeed.VolumeAtPriceH\x00\x12\"\n\x04ohlc\x18\x0c \x01(\x0b\x32\x12.org.openfeed.OhlcH\x00\x12:\n\x10\x65xchangeResponse\x18\r \x01(\x0b\x32\x1e.org.openfeed.ExchangeResponseH\x00\x12:\n\x10instrumentAction\x18\x0e \x01(\x0b\x32\x1e.org.openfeed.InstrumentActionH\x00\x42\x06\n\x04\x64\x61ta\"g\n\x06Status\x12$\n\x06result\x18\x01 \x01(\x0e\x32\x14.org.openfeed.Result\x12\x0f\n\x07message\x18\x02 \x01(\t\x12&\n\x07service\x18\x03 \x01(\x0e\x32\x15.org.openfeed.Service\"y\n\x0cLoginRequest\x12\x15\n\rcorrelationId\x18\x01 \x01(\x12\x12\x10\n\x08username\x18\x02 \x01(\t\x12\x10\n\x08password\x18\x03 \x01(\t\x12\x15\n\rclientVersion\x18\x04 \x01(\t\x12\x17\n\x0fprotocolVersion\x18\x05 \x01(\x11\"[\n\rLoginResponse\x12\x15\n\rcorrelationId\x18\x01 \x01(\x12\x12$\n\x06status\x18\x02 \x01(\x0b\x32\x14.org.openfeed.Status\x12\r\n\x05token\x18\x03 \x01(\t\"5\n\rLogoutRequest\x12\x15\n\rcorrelationId\x18\x01 \x01(\x12\x12\r\n\x05token\x18\x03 \x01(\t\"M\n\x0eLogoutResponse\x12\x15\n\rcorrelationId\x18\x01 \x01(\x12\x12$\n\x06status\x18\x02 \x01(\x0b\x32\x14.org.openfeed.Status\"\x93\x01\n\x11InstrumentRequest\x12\x15\n\rcorrelationId\x18\x01 \x01(\x12\x12\r\n\x05token\x18\x02 \x01(\t\x12\x10\n\x06symbol\x18\n \x01(\tH\x00\x12\x12\n\x08marketId\x18\x0b \x01(\x12H\x00\x12\x12\n\x08\x65xchange\x18\x0c \x01(\tH\x00\x12\x13\n\tchannelId\x18\r \x01(\x11H\x00\x42\t\n\x07request\"\xb5\x01\n\x12InstrumentResponse\x12\x15\n\rcorrelationId\x18\x01 \x01(\x12\x12$\n\x06status\x18\x02 \x01(\x0b\x32\x14.org.openfeed.Status\x12\x1b\n\x13numberOfDefinitions\x18\x03 \x01(\x11\x12\x0e\n\x06symbol\x18\x04 \x01(\t\x12\x10\n\x08marketId\x18\x05 \x01(\x12\x12\x10\n\x08\x65xchange\x18\x06 \x01(\t\x12\x11\n\tchannelId\x18\x07 \x01(\x11\"\x9c\x01\n\x1aInstrumentReferenceRequest\x12\x15\n\rcorrelationId\x18\x01 \x01(\x12\x12\r\n\x05token\x18\x02 \x01(\t\x12\x10\n\x06symbol\x18\n \x01(\tH\x00\x12\x12\n\x08marketId\x18\x0b \x01(\x12H\x00\x12\x12\n\x08\x65xchange\x18\x0c \x01(\tH\x00\x12\x13\n\tchannelId\x18\r \x01(\x11H\x00\x42\t\n\x07request\"\x93\x02\n\x1bInstrumentReferenceResponse\x12\x15\n\rcorrelationId\x18\x01 \x01(\x12\x12$\n\x06status\x18\x02 \x01(\x0b\x32\x14.org.openfeed.Status\x12\x1b\n\x13numberOfDefinitions\x18\x03 \x01(\x11\x12\x11\n\tchannelId\x18\x04 \x01(\x11\x12\x10\n\x08marketId\x18\x05 \x01(\x12\x12\x0e\n\x06symbol\x18\x06 \x01(\t\x12\x10\n\x08\x65xchange\x18\x07 \x01(\t\x12\x11\n\tddfSymbol\x18\x08 \x01(\t\x12\x13\n\x0b\x64\x64\x66\x45xchange\x18\t \x01(\t\x12\x13\n\x0b\x64\x64\x66\x42\x61seCode\x18\n \x01(\t\x12\x16\n\x0e\x65xchangeSymbol\x18\x0b \x01(\t\"7\n\x0f\x45xchangeRequest\x12\x15\n\rcorrelationId\x18\x01 \x01(\x12\x12\r\n\x05token\x18\x02 \x01(\t\"\xcb\x01\n\x10\x45xchangeResponse\x12\x15\n\rcorrelationId\x18\x01 \x01(\x12\x12$\n\x06status\x18\x02 \x01(\x0b\x32\x14.org.openfeed.Status\x12:\n\texchanges\x18\x03 \x03(\x0b\x32\'.org.openfeed.ExchangeResponse.Exchange\x1a>\n\x08\x45xchange\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0f\n\x07\x61liases\x18\x03 \x03(\t\"]\n\x16\x42ulkSubscriptionFilter\x12,\n\nsymbolType\x18\x01 \x01(\x0e\x32\x18.org.openfeed.SymbolType\x12\x15\n\rsymbolPattern\x18\x02 \x01(\t\"\x84\x04\n\x13SubscriptionRequest\x12\x15\n\rcorrelationId\x18\x01 \x01(\x12\x12\r\n\x05token\x18\x02 \x01(\t\x12&\n\x07service\x18\x03 \x01(\x0e\x32\x15.org.openfeed.Service\x12\x13\n\x0bunsubscribe\x18\x04 \x01(\x08\x12;\n\x08requests\x18\x05 \x03(\x0b\x32).org.openfeed.SubscriptionRequest.Request\x1a\xcc\x02\n\x07Request\x12\x10\n\x06symbol\x18\x01 \x01(\tH\x00\x12\x12\n\x08marketId\x18\x02 \x01(\x12H\x00\x12\x12\n\x08\x65xchange\x18\x03 \x01(\tH\x00\x12\x13\n\tchannelId\x18\x04 \x01(\x11H\x00\x12\x38\n\x10subscriptionType\x18\n \x03(\x0e\x32\x1e.org.openfeed.SubscriptionType\x12\x1f\n\x17snapshotIntervalSeconds\x18\x0b \x01(\x11\x12I\n\x0einstrumentType\x18\x0c \x03(\x0e\x32\x31.org.openfeed.InstrumentDefinition.InstrumentType\x12\x44\n\x16\x62ulkSubscriptionFilter\x18\r \x03(\x0b\x32$.org.openfeed.BulkSubscriptionFilterB\x06\n\x04\x64\x61ta\"\xa7\x02\n\x14SubscriptionResponse\x12\x15\n\rcorrelationId\x18\x01 \x01(\x12\x12$\n\x06status\x18\x02 \x01(\x0b\x32\x14.org.openfeed.Status\x12\x0e\n\x06symbol\x18\x03 \x01(\t\x12\x10\n\x08marketId\x18\x04 \x01(\x12\x12\x10\n\x08\x65xchange\x18\x05 \x01(\t\x12\x11\n\tchannelId\x18\x06 \x01(\x11\x12\x1b\n\x13numberOfDefinitions\x18\x07 \x01(\x11\x12\x38\n\x10subscriptionType\x18\x08 \x01(\x0e\x32\x1e.org.openfeed.SubscriptionType\x12\x13\n\x0bunsubscribe\x18\t \x01(\x08\x12\x1f\n\x17snapshotIntervalSeconds\x18\n \x01(\x11*\xde\x02\n\x06Result\x12\x12\n\x0eUNKNOWN_RESULT\x10\x00\x12\x0b\n\x07SUCCESS\x10\x01\x12\x13\n\x0f\x44UPLICATE_LOGIN\x10s\x12\x12\n\x0eINVALID_SYMBOL\x10t\x12\x15\n\x11INVALID_MARKET_ID\x10u\x12\x14\n\x10INVALID_EXCHANGE\x10v\x12\x16\n\x12INVALID_CHANNEL_ID\x10w\x12\x15\n\x11MALFORMED_MESSAGE\x10x\x12\x16\n\x12UNEXPECTED_MESSAGE\x10y\x12\x12\n\x0eNOT_SUBSCRIBED\x10z\x12\x1a\n\x16\x44UPLICATE_SUBSCRIPTION\x10{\x12\x17\n\x13INVALID_CREDENTIALS\x10|\x12\x1b\n\x17INSUFFICIENT_PRIVILEGES\x10}\x12\x1b\n\x17\x41UTHENTICATION_REQUIRED\x10~\x12\x13\n\x0fGENERIC_FAILURE\x10\x7f*\xa1\x01\n\x10SubscriptionType\x12\x07\n\x03\x41LL\x10\x00\x12\t\n\x05QUOTE\x10\x01\x12\x15\n\x11QUOTE_PARTICIPANT\x10\x02\x12\x0f\n\x0b\x44\x45PTH_PRICE\x10\x03\x12\x0f\n\x0b\x44\x45PTH_ORDER\x10\x04\x12\n\n\x06TRADES\x10\x05\x12\x14\n\x10\x43UMLATIVE_VOLUME\x10\x06\x12\x08\n\x04OHLC\x10\x07\x12\x14\n\x10OHLC_NON_REGULAR\x10\x08*(\n\nSymbolType\x12\x0c\n\x08\x42\x41RCHART\x10\x00\x12\x0c\n\x08\x45XCHANGE\x10\x01\x42\x07H\x01P\x01\xa0\x01\x01\x62\x06proto3'
   ,
   dependencies=[openfeed__instrument__pb2.DESCRIPTOR,openfeed__pb2.DESCRIPTOR,])
 
 _RESULT = _descriptor.EnumDescriptor(
   name='Result',
   full_name='org.openfeed.Result',
   filename=None,
@@ -107,16 +107,16 @@
       name='GENERIC_FAILURE', index=14, number=127,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=3533,
-  serialized_end=3883,
+  serialized_start=3731,
+  serialized_end=4081,
 )
 _sym_db.RegisterEnumDescriptor(_RESULT)
 
 Result = enum_type_wrapper.EnumTypeWrapper(_RESULT)
 _SUBSCRIPTIONTYPE = _descriptor.EnumDescriptor(
   name='SubscriptionType',
   full_name='org.openfeed.SubscriptionType',
@@ -168,20 +168,46 @@
       name='OHLC_NON_REGULAR', index=8, number=8,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=3886,
-  serialized_end=4047,
+  serialized_start=4084,
+  serialized_end=4245,
 )
 _sym_db.RegisterEnumDescriptor(_SUBSCRIPTIONTYPE)
 
 SubscriptionType = enum_type_wrapper.EnumTypeWrapper(_SUBSCRIPTIONTYPE)
+_SYMBOLTYPE = _descriptor.EnumDescriptor(
+  name='SymbolType',
+  full_name='org.openfeed.SymbolType',
+  filename=None,
+  file=DESCRIPTOR,
+  create_key=_descriptor._internal_create_key,
+  values=[
+    _descriptor.EnumValueDescriptor(
+      name='BARCHART', index=0, number=0,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='EXCHANGE', index=1, number=1,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+  ],
+  containing_type=None,
+  serialized_options=None,
+  serialized_start=4247,
+  serialized_end=4287,
+)
+_sym_db.RegisterEnumDescriptor(_SYMBOLTYPE)
+
+SymbolType = enum_type_wrapper.EnumTypeWrapper(_SYMBOLTYPE)
 UNKNOWN_RESULT = 0
 SUCCESS = 1
 DUPLICATE_LOGIN = 115
 INVALID_SYMBOL = 116
 INVALID_MARKET_ID = 117
 INVALID_EXCHANGE = 118
 INVALID_CHANNEL_ID = 119
@@ -198,14 +224,16 @@
 QUOTE_PARTICIPANT = 2
 DEPTH_PRICE = 3
 DEPTH_ORDER = 4
 TRADES = 5
 CUMLATIVE_VOLUME = 6
 OHLC = 7
 OHLC_NON_REGULAR = 8
+BARCHART = 0
+EXCHANGE = 1
 
 
 
 _OPENFEEDGATEWAYREQUEST = _descriptor.Descriptor(
   name='OpenfeedGatewayRequest',
   full_name='org.openfeed.OpenfeedGatewayRequest',
   filename=None,
@@ -1081,14 +1109,53 @@
   oneofs=[
   ],
   serialized_start=2613,
   serialized_end=2816,
 )
 
 
+_BULKSUBSCRIPTIONFILTER = _descriptor.Descriptor(
+  name='BulkSubscriptionFilter',
+  full_name='org.openfeed.BulkSubscriptionFilter',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='symbolType', full_name='org.openfeed.BulkSubscriptionFilter.symbolType', index=0,
+      number=1, type=14, cpp_type=8, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='symbolPattern', full_name='org.openfeed.BulkSubscriptionFilter.symbolPattern', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=2818,
+  serialized_end=2911,
+)
+
+
 _SUBSCRIPTIONREQUEST_REQUEST = _descriptor.Descriptor(
   name='Request',
   full_name='org.openfeed.SubscriptionRequest.Request',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
@@ -1138,14 +1205,21 @@
     _descriptor.FieldDescriptor(
       name='instrumentType', full_name='org.openfeed.SubscriptionRequest.Request.instrumentType', index=6,
       number=12, type=14, cpp_type=8, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='bulkSubscriptionFilter', full_name='org.openfeed.SubscriptionRequest.Request.bulkSubscriptionFilter', index=7,
+      number=13, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
@@ -1155,16 +1229,16 @@
   oneofs=[
     _descriptor.OneofDescriptor(
       name='data', full_name='org.openfeed.SubscriptionRequest.Request.data',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
-  serialized_start=3003,
-  serialized_end=3265,
+  serialized_start=3098,
+  serialized_end=3430,
 )
 
 _SUBSCRIPTIONREQUEST = _descriptor.Descriptor(
   name='SubscriptionRequest',
   full_name='org.openfeed.SubscriptionRequest',
   filename=None,
   file=DESCRIPTOR,
@@ -1214,16 +1288,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2819,
-  serialized_end=3265,
+  serialized_start=2914,
+  serialized_end=3430,
 )
 
 
 _SUBSCRIPTIONRESPONSE = _descriptor.Descriptor(
   name='SubscriptionResponse',
   full_name='org.openfeed.SubscriptionResponse',
   filename=None,
@@ -1290,28 +1364,35 @@
     _descriptor.FieldDescriptor(
       name='unsubscribe', full_name='org.openfeed.SubscriptionResponse.unsubscribe', index=8,
       number=9, type=8, cpp_type=7, label=1,
       has_default_value=False, default_value=False,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='snapshotIntervalSeconds', full_name='org.openfeed.SubscriptionResponse.snapshotIntervalSeconds', index=9,
+      number=10, type=17, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3268,
-  serialized_end=3530,
+  serialized_start=3433,
+  serialized_end=3728,
 )
 
 _OPENFEEDGATEWAYREQUEST.fields_by_name['loginRequest'].message_type = _LOGINREQUEST
 _OPENFEEDGATEWAYREQUEST.fields_by_name['logoutRequest'].message_type = _LOGOUTREQUEST
 _OPENFEEDGATEWAYREQUEST.fields_by_name['subscriptionRequest'].message_type = _SUBSCRIPTIONREQUEST
 _OPENFEEDGATEWAYREQUEST.fields_by_name['instrumentRequest'].message_type = _INSTRUMENTREQUEST
 _OPENFEEDGATEWAYREQUEST.fields_by_name['instrumentReferenceRequest'].message_type = _INSTRUMENTREFERENCEREQUEST
@@ -1419,16 +1500,18 @@
 _INSTRUMENTREFERENCEREQUEST.oneofs_by_name['request'].fields.append(
   _INSTRUMENTREFERENCEREQUEST.fields_by_name['channelId'])
 _INSTRUMENTREFERENCEREQUEST.fields_by_name['channelId'].containing_oneof = _INSTRUMENTREFERENCEREQUEST.oneofs_by_name['request']
 _INSTRUMENTREFERENCERESPONSE.fields_by_name['status'].message_type = _STATUS
 _EXCHANGERESPONSE_EXCHANGE.containing_type = _EXCHANGERESPONSE
 _EXCHANGERESPONSE.fields_by_name['status'].message_type = _STATUS
 _EXCHANGERESPONSE.fields_by_name['exchanges'].message_type = _EXCHANGERESPONSE_EXCHANGE
+_BULKSUBSCRIPTIONFILTER.fields_by_name['symbolType'].enum_type = _SYMBOLTYPE
 _SUBSCRIPTIONREQUEST_REQUEST.fields_by_name['subscriptionType'].enum_type = _SUBSCRIPTIONTYPE
 _SUBSCRIPTIONREQUEST_REQUEST.fields_by_name['instrumentType'].enum_type = openfeed__instrument__pb2._INSTRUMENTDEFINITION_INSTRUMENTTYPE
+_SUBSCRIPTIONREQUEST_REQUEST.fields_by_name['bulkSubscriptionFilter'].message_type = _BULKSUBSCRIPTIONFILTER
 _SUBSCRIPTIONREQUEST_REQUEST.containing_type = _SUBSCRIPTIONREQUEST
 _SUBSCRIPTIONREQUEST_REQUEST.oneofs_by_name['data'].fields.append(
   _SUBSCRIPTIONREQUEST_REQUEST.fields_by_name['symbol'])
 _SUBSCRIPTIONREQUEST_REQUEST.fields_by_name['symbol'].containing_oneof = _SUBSCRIPTIONREQUEST_REQUEST.oneofs_by_name['data']
 _SUBSCRIPTIONREQUEST_REQUEST.oneofs_by_name['data'].fields.append(
   _SUBSCRIPTIONREQUEST_REQUEST.fields_by_name['marketId'])
 _SUBSCRIPTIONREQUEST_REQUEST.fields_by_name['marketId'].containing_oneof = _SUBSCRIPTIONREQUEST_REQUEST.oneofs_by_name['data']
@@ -1451,18 +1534,20 @@
 DESCRIPTOR.message_types_by_name['LogoutResponse'] = _LOGOUTRESPONSE
 DESCRIPTOR.message_types_by_name['InstrumentRequest'] = _INSTRUMENTREQUEST
 DESCRIPTOR.message_types_by_name['InstrumentResponse'] = _INSTRUMENTRESPONSE
 DESCRIPTOR.message_types_by_name['InstrumentReferenceRequest'] = _INSTRUMENTREFERENCEREQUEST
 DESCRIPTOR.message_types_by_name['InstrumentReferenceResponse'] = _INSTRUMENTREFERENCERESPONSE
 DESCRIPTOR.message_types_by_name['ExchangeRequest'] = _EXCHANGEREQUEST
 DESCRIPTOR.message_types_by_name['ExchangeResponse'] = _EXCHANGERESPONSE
+DESCRIPTOR.message_types_by_name['BulkSubscriptionFilter'] = _BULKSUBSCRIPTIONFILTER
 DESCRIPTOR.message_types_by_name['SubscriptionRequest'] = _SUBSCRIPTIONREQUEST
 DESCRIPTOR.message_types_by_name['SubscriptionResponse'] = _SUBSCRIPTIONRESPONSE
 DESCRIPTOR.enum_types_by_name['Result'] = _RESULT
 DESCRIPTOR.enum_types_by_name['SubscriptionType'] = _SUBSCRIPTIONTYPE
+DESCRIPTOR.enum_types_by_name['SymbolType'] = _SYMBOLTYPE
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
 
 OpenfeedGatewayRequest = _reflection.GeneratedProtocolMessageType('OpenfeedGatewayRequest', (_message.Message,), {
   'DESCRIPTOR' : _OPENFEEDGATEWAYREQUEST,
   '__module__' : 'openfeed_api_pb2'
   # @@protoc_insertion_point(class_scope:org.openfeed.OpenfeedGatewayRequest)
   })
@@ -1556,14 +1641,21 @@
   'DESCRIPTOR' : _EXCHANGERESPONSE,
   '__module__' : 'openfeed_api_pb2'
   # @@protoc_insertion_point(class_scope:org.openfeed.ExchangeResponse)
   })
 _sym_db.RegisterMessage(ExchangeResponse)
 _sym_db.RegisterMessage(ExchangeResponse.Exchange)
 
+BulkSubscriptionFilter = _reflection.GeneratedProtocolMessageType('BulkSubscriptionFilter', (_message.Message,), {
+  'DESCRIPTOR' : _BULKSUBSCRIPTIONFILTER,
+  '__module__' : 'openfeed_api_pb2'
+  # @@protoc_insertion_point(class_scope:org.openfeed.BulkSubscriptionFilter)
+  })
+_sym_db.RegisterMessage(BulkSubscriptionFilter)
+
 SubscriptionRequest = _reflection.GeneratedProtocolMessageType('SubscriptionRequest', (_message.Message,), {
 
   'Request' : _reflection.GeneratedProtocolMessageType('Request', (_message.Message,), {
     'DESCRIPTOR' : _SUBSCRIPTIONREQUEST_REQUEST,
     '__module__' : 'openfeed_api_pb2'
     # @@protoc_insertion_point(class_scope:org.openfeed.SubscriptionRequest.Request)
     })
```

### Comparing `openfeed-1.2.0/openfeed/generated/openfeed_instrument_pb2.py` & `openfeed-1.3.0/openfeed/generated/openfeed_instrument_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='openfeed_instrument.proto',
   package='org.openfeed',
   syntax='proto3',
   serialized_options=b'H\001P\001\240\001\001',
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n\x19openfeed_instrument.proto\x12\x0corg.openfeed\"\xef\x1a\n\x14InstrumentDefinition\x12\x10\n\x08marketId\x18\x01 \x01(\x12\x12I\n\x0einstrumentType\x18\x02 \x01(\x0e\x32\x31.org.openfeed.InstrumentDefinition.InstrumentType\x12\x45\n\x10supportBookTypes\x18\x03 \x03(\x0e\x32+.org.openfeed.InstrumentDefinition.BookType\x12\x11\n\tbookDepth\x18\x04 \x01(\x11\x12\x10\n\x08vendorId\x18\x05 \x01(\t\x12\x0e\n\x06symbol\x18\x06 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x07 \x01(\t\x12\x0f\n\x07\x63\x66iCode\x18\x08 \x01(\t\x12\x14\n\x0c\x63urrencyCode\x18\t \x01(\t\x12\x14\n\x0c\x65xchangeCode\x18\n \x01(\t\x12\x1d\n\x15minimumPriceIncrement\x18\x0b \x01(\x02\x12\x1a\n\x12\x63ontractPointValue\x18\x0c \x01(\x02\x12=\n\x08schedule\x18\r \x01(\x0b\x32+.org.openfeed.InstrumentDefinition.Schedule\x12=\n\x08\x63\x61lendar\x18\x0e \x01(\x0b\x32+.org.openfeed.InstrumentDefinition.Calendar\x12\x18\n\x10recordCreateTime\x18\x0f \x01(\x12\x12\x18\n\x10recordUpdateTime\x18\x10 \x01(\x12\x12\x14\n\x0ctimeZoneName\x18\x11 \x01(\t\x12\x17\n\x0finstrumentGroup\x18\x12 \x01(\t\x12I\n\x10symbolExpiration\x18\x13 \x01(\x0b\x32/.org.openfeed.InstrumentDefinition.MaturityDate\x12\x37\n\x05state\x18\x14 \x01(\x0e\x32(.org.openfeed.InstrumentDefinition.State\x12\x0f\n\x07\x63hannel\x18\x15 \x01(\x11\x12\x1a\n\x12underlyingMarketId\x18\x16 \x01(\x12\x12\x43\n\x0bpriceFormat\x18\x17 \x01(\x0b\x32..org.openfeed.InstrumentDefinition.PriceFormat\x12O\n\x17optionStrikePriceFormat\x18\x18 \x01(\x0b\x32..org.openfeed.InstrumentDefinition.PriceFormat\x12\x18\n\x10priceDenominator\x18\x1c \x01(\x11\x12\x1b\n\x13quantityDenominator\x18\x1d \x01(\x11\x12\x12\n\nisTradable\x18\x1e \x01(\x08\x12\x17\n\x0ftransactionTime\x18\x32 \x01(\x12\x12\x15\n\rauxiliaryData\x18\x63 \x01(\x0c\x12:\n\x07symbols\x18\x64 \x03(\x0b\x32).org.openfeed.InstrumentDefinition.Symbol\x12\x15\n\x0coptionStrike\x18\xc8\x01 \x01(\x12\x12\x42\n\noptionType\x18\xca\x01 \x01(\x0e\x32-.org.openfeed.InstrumentDefinition.OptionType\x12\x44\n\x0boptionStyle\x18\xcb\x01 \x01(\x0e\x32..org.openfeed.InstrumentDefinition.OptionStyle\x12 \n\x17optionStrikeDenominator\x18\xcc\x01 \x01(\x11\x12\x13\n\nspreadCode\x18\xd2\x01 \x01(\t\x12@\n\tspreadLeg\x18\xd3\x01 \x03(\x0b\x32,.org.openfeed.InstrumentDefinition.SpreadLeg\x12\x1a\n\x11userDefinedSpread\x18\xd4\x01 \x01(\x08\x12\x13\n\nmarketTier\x18\xd5\x01 \x01(\t\x12!\n\x18\x66inancialStatusIndicator\x18\xd6\x01 \x01(\t\x12\r\n\x04isin\x18\xd7\x01 \x01(\t\x12\x46\n\x0c\x63urrencyPair\x18\xd8\x01 \x01(\x0b\x32/.org.openfeed.InstrumentDefinition.CurrencyPair\x12\x1c\n\x13\x65xchangeSendsVolume\x18\xd9\x01 \x01(\x08\x12\x1a\n\x11\x65xchangeSendsHigh\x18\xda\x01 \x01(\x08\x12\x19\n\x10\x65xchangeSendsLow\x18\xdb\x01 \x01(\x08\x12\x1a\n\x11\x65xchangeSendsOpen\x18\xdc\x01 \x01(\x08\x12#\n\x1a\x63onsolidatedFeedInstrument\x18\xdd\x01 \x01(\x08\x12\x1d\n\x14openOutcryInstrument\x18\xde\x01 \x01(\x08\x12*\n!syntheticAmericanOptionInstrument\x18\xdf\x01 \x01(\x08\x12\x1d\n\x14\x62\x61rchartExchangeCode\x18\xe0\x01 \x01(\t\x12\x19\n\x10\x62\x61rchartBaseCode\x18\xe1\x01 \x01(\t\x12\x1a\n\x11volumeDenominator\x18\xe2\x01 \x01(\x11\x12$\n\x1b\x62idOfferQuantityDenominator\x18\xe3\x01 \x01(\x11\x12*\n!primaryListingMarketParticipantId\x18\xe4\x01 \x01(\t\x12\x1b\n\x12subscriptionSymbol\x18\xe5\x01 \x01(\t\x1aI\n\x08Schedule\x12=\n\x08sessions\x18\x01 \x03(\x0b\x32+.org.openfeed.InstrumentDefinition.TimeSpan\x1a\x31\n\x08TimeSpan\x12\x11\n\ttimeStart\x18\x01 \x01(\x12\x12\x12\n\ntimeFinish\x18\x02 \x01(\x12\x1a\x44\n\x08\x43\x61lendar\x12\x38\n\x06\x65vents\x18\x01 \x03(\x0b\x32(.org.openfeed.InstrumentDefinition.Event\x1aQ\n\x05\x45vent\x12:\n\x04type\x18\x01 \x01(\x0e\x32,.org.openfeed.InstrumentDefinition.EventType\x12\x0c\n\x04\x64\x61te\x18\x02 \x01(\x12\x1a<\n\tSpreadLeg\x12\x10\n\x08marketId\x18\x01 \x01(\x12\x12\r\n\x05ratio\x18\x02 \x01(\x11\x12\x0e\n\x06symbol\x18\x03 \x01(\t\x1a\x38\n\x0cMaturityDate\x12\x0c\n\x04year\x18\x01 \x01(\x11\x12\r\n\x05month\x18\x02 \x01(\x11\x12\x0b\n\x03\x64\x61y\x18\x03 \x01(\x11\x1a(\n\x06Symbol\x12\x0e\n\x06vendor\x18\x01 \x01(\t\x12\x0e\n\x06symbol\x18\x02 \x01(\t\x1a\xd1\x01\n\x0bPriceFormat\x12\x14\n\x0cisFractional\x18\x01 \x01(\x08\x12\x13\n\x0b\x64\x65nominator\x18\x02 \x01(\x11\x12\x16\n\x0esubDenominator\x18\x04 \x01(\x11\x12K\n\tsubFormat\x18\x06 \x01(\x0e\x32\x38.org.openfeed.InstrumentDefinition.PriceFormat.SubFormat\"2\n\tSubFormat\x12\x08\n\x04\x46LAT\x10\x00\x12\x0e\n\nFRACTIONAL\x10\x01\x12\x0b\n\x07\x44\x45\x43IMAL\x10\x02\x1a\x34\n\x0c\x43urrencyPair\x12\x11\n\tcurrency1\x18\x01 \x01(\t\x12\x11\n\tcurrency2\x18\x02 \x01(\t\"\x9b\x01\n\x0eInstrumentType\x12\x1b\n\x17UNKNOWN_INSTRUMENT_TYPE\x10\x00\x12\t\n\x05\x46OREX\x10\x01\x12\t\n\x05INDEX\x10\x02\x12\n\n\x06\x45QUITY\x10\x03\x12\n\n\x06\x46UTURE\x10\x04\x12\n\n\x06OPTION\x10\x05\x12\n\n\x06SPREAD\x10\x06\x12\x0f\n\x0bMUTUAL_FUND\x10\x07\x12\x15\n\x11MONEY_MARKET_FUND\x10\x08\"Z\n\x08\x42ookType\x12\x15\n\x11UNKNOWN_BOOK_TYPE\x10\x00\x12\x0f\n\x0bTOP_OF_BOOK\x10\x01\x12\x15\n\x11PRICE_LEVEL_DEPTH\x10\x02\x12\x0f\n\x0bORDER_DEPTH\x10\x03\"8\n\nOptionType\x12\x17\n\x13UNKNOWN_OPTION_TYPE\x10\x00\x12\x08\n\x04\x43\x41LL\x10\x01\x12\x07\n\x03PUT\x10\x02\"Q\n\x0bOptionStyle\x12\x19\n\x15UNKNOWN_OPTIONS_STYLE\x10\x00\x12\x0b\n\x07\x44\x45\x46\x41ULT\x10\x01\x12\x0c\n\x08\x41MERICAN\x10\x02\x12\x0c\n\x08\x45UROPEAN\x10\x03\"3\n\x05State\x12\x11\n\rUNKNOWN_STATE\x10\x00\x12\n\n\x06\x41\x43TIVE\x10\x01\x12\x0b\n\x07PASSIVE\x10\x02\"\xa7\x02\n\tEventType\x12\x16\n\x12UNKNOWN_EVENT_TYPE\x10\x00\x12\x14\n\x10\x46IRST_TRADE_DATE\x10\x01\x12\x13\n\x0fLAST_TRADE_DATE\x10\x02\x12\x19\n\x15\x46INAL_SETTLEMENT_DATE\x10\n\x12\x17\n\x13\x46IRST_DELIVERY_DATE\x10\x0b\x12\x16\n\x12LAST_DELIVERY_DATE\x10\x0c\x12\x15\n\x11\x46IRST_NOTICE_DATE\x10\r\x12\x14\n\x10LAST_NOTICE_DATE\x10\x0e\x12\x16\n\x12\x46IRST_HOLDING_DATE\x10\x0f\x12\x15\n\x11LAST_HOLDING_DATE\x10\x10\x12\x17\n\x13\x46IRST_POSITION_DATE\x10\x11\x12\x16\n\x12LAST_POSITION_DATE\x10\x12\x42\x07H\x01P\x01\xa0\x01\x01\x62\x06proto3'
+  serialized_pb=b'\n\x19openfeed_instrument.proto\x12\x0corg.openfeed\"\x9e\x1c\n\x14InstrumentDefinition\x12\x10\n\x08marketId\x18\x01 \x01(\x12\x12I\n\x0einstrumentType\x18\x02 \x01(\x0e\x32\x31.org.openfeed.InstrumentDefinition.InstrumentType\x12\x45\n\x10supportBookTypes\x18\x03 \x03(\x0e\x32+.org.openfeed.InstrumentDefinition.BookType\x12\x11\n\tbookDepth\x18\x04 \x01(\x11\x12\x10\n\x08vendorId\x18\x05 \x01(\t\x12\x0e\n\x06symbol\x18\x06 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x07 \x01(\t\x12\x0f\n\x07\x63\x66iCode\x18\x08 \x01(\t\x12\x14\n\x0c\x63urrencyCode\x18\t \x01(\t\x12\x14\n\x0c\x65xchangeCode\x18\n \x01(\t\x12\x1d\n\x15minimumPriceIncrement\x18\x0b \x01(\x02\x12\x1a\n\x12\x63ontractPointValue\x18\x0c \x01(\x02\x12=\n\x08schedule\x18\r \x01(\x0b\x32+.org.openfeed.InstrumentDefinition.Schedule\x12=\n\x08\x63\x61lendar\x18\x0e \x01(\x0b\x32+.org.openfeed.InstrumentDefinition.Calendar\x12\x18\n\x10recordCreateTime\x18\x0f \x01(\x12\x12\x18\n\x10recordUpdateTime\x18\x10 \x01(\x12\x12\x14\n\x0ctimeZoneName\x18\x11 \x01(\t\x12\x17\n\x0finstrumentGroup\x18\x12 \x01(\t\x12I\n\x10symbolExpiration\x18\x13 \x01(\x0b\x32/.org.openfeed.InstrumentDefinition.MaturityDate\x12\x37\n\x05state\x18\x14 \x01(\x0e\x32(.org.openfeed.InstrumentDefinition.State\x12\x0f\n\x07\x63hannel\x18\x15 \x01(\x11\x12\x1a\n\x12underlyingMarketId\x18\x16 \x01(\x12\x12\x43\n\x0bpriceFormat\x18\x17 \x01(\x0b\x32..org.openfeed.InstrumentDefinition.PriceFormat\x12O\n\x17optionStrikePriceFormat\x18\x18 \x01(\x0b\x32..org.openfeed.InstrumentDefinition.PriceFormat\x12\x18\n\x10priceDenominator\x18\x1c \x01(\x11\x12\x1b\n\x13quantityDenominator\x18\x1d \x01(\x11\x12\x12\n\nisTradable\x18\x1e \x01(\x08\x12\x17\n\x0ftransactionTime\x18\x32 \x01(\x12\x12\x15\n\rauxiliaryData\x18\x63 \x01(\x0c\x12:\n\x07symbols\x18\x64 \x03(\x0b\x32).org.openfeed.InstrumentDefinition.Symbol\x12\x15\n\x0coptionStrike\x18\xc8\x01 \x01(\x12\x12\x42\n\noptionType\x18\xca\x01 \x01(\x0e\x32-.org.openfeed.InstrumentDefinition.OptionType\x12\x44\n\x0boptionStyle\x18\xcb\x01 \x01(\x0e\x32..org.openfeed.InstrumentDefinition.OptionStyle\x12 \n\x17optionStrikeDenominator\x18\xcc\x01 \x01(\x11\x12\x13\n\nspreadCode\x18\xd2\x01 \x01(\t\x12@\n\tspreadLeg\x18\xd3\x01 \x03(\x0b\x32,.org.openfeed.InstrumentDefinition.SpreadLeg\x12\x1a\n\x11userDefinedSpread\x18\xd4\x01 \x01(\x08\x12\x13\n\nmarketTier\x18\xd5\x01 \x01(\t\x12!\n\x18\x66inancialStatusIndicator\x18\xd6\x01 \x01(\t\x12\r\n\x04isin\x18\xd7\x01 \x01(\t\x12\x46\n\x0c\x63urrencyPair\x18\xd8\x01 \x01(\x0b\x32/.org.openfeed.InstrumentDefinition.CurrencyPair\x12\x1c\n\x13\x65xchangeSendsVolume\x18\xd9\x01 \x01(\x08\x12\x1a\n\x11\x65xchangeSendsHigh\x18\xda\x01 \x01(\x08\x12\x19\n\x10\x65xchangeSendsLow\x18\xdb\x01 \x01(\x08\x12\x1a\n\x11\x65xchangeSendsOpen\x18\xdc\x01 \x01(\x08\x12#\n\x1a\x63onsolidatedFeedInstrument\x18\xdd\x01 \x01(\x08\x12\x1d\n\x14openOutcryInstrument\x18\xde\x01 \x01(\x08\x12*\n!syntheticAmericanOptionInstrument\x18\xdf\x01 \x01(\x08\x12\x1d\n\x14\x62\x61rchartExchangeCode\x18\xe0\x01 \x01(\t\x12\x19\n\x10\x62\x61rchartBaseCode\x18\xe1\x01 \x01(\t\x12\x1a\n\x11volumeDenominator\x18\xe2\x01 \x01(\x11\x12$\n\x1b\x62idOfferQuantityDenominator\x18\xe3\x01 \x01(\x11\x12*\n!primaryListingMarketParticipantId\x18\xe4\x01 \x01(\t\x12\x1b\n\x12subscriptionSymbol\x18\xe5\x01 \x01(\t\x12J\n\x10\x63ontractMaturity\x18\xe6\x01 \x01(\x0b\x32/.org.openfeed.InstrumentDefinition.MaturityDate\x1aI\n\x08Schedule\x12=\n\x08sessions\x18\x01 \x03(\x0b\x32+.org.openfeed.InstrumentDefinition.TimeSpan\x1a\x31\n\x08TimeSpan\x12\x11\n\ttimeStart\x18\x01 \x01(\x12\x12\x12\n\ntimeFinish\x18\x02 \x01(\x12\x1a\x44\n\x08\x43\x61lendar\x12\x38\n\x06\x65vents\x18\x01 \x03(\x0b\x32(.org.openfeed.InstrumentDefinition.Event\x1aQ\n\x05\x45vent\x12:\n\x04type\x18\x01 \x01(\x0e\x32,.org.openfeed.InstrumentDefinition.EventType\x12\x0c\n\x04\x64\x61te\x18\x02 \x01(\x12\x1az\n\tSpreadLeg\x12\x10\n\x08marketId\x18\x01 \x01(\x12\x12\r\n\x05ratio\x18\x02 \x01(\x11\x12\x0e\n\x06symbol\x18\x03 \x01(\t\x12\x12\n\nlongSymbol\x18\x04 \x01(\t\x12\x16\n\x0elegOptionDelta\x18\x05 \x01(\x02\x12\x10\n\x08legPrice\x18\x06 \x01(\x02\x1a\x38\n\x0cMaturityDate\x12\x0c\n\x04year\x18\x01 \x01(\x11\x12\r\n\x05month\x18\x02 \x01(\x11\x12\x0b\n\x03\x64\x61y\x18\x03 \x01(\x11\x1a<\n\x06Symbol\x12\x0e\n\x06vendor\x18\x01 \x01(\t\x12\x0e\n\x06symbol\x18\x02 \x01(\t\x12\x12\n\nlongSymbol\x18\x03 \x01(\t\x1a\xd1\x01\n\x0bPriceFormat\x12\x14\n\x0cisFractional\x18\x01 \x01(\x08\x12\x13\n\x0b\x64\x65nominator\x18\x02 \x01(\x11\x12\x16\n\x0esubDenominator\x18\x04 \x01(\x11\x12K\n\tsubFormat\x18\x06 \x01(\x0e\x32\x38.org.openfeed.InstrumentDefinition.PriceFormat.SubFormat\"2\n\tSubFormat\x12\x08\n\x04\x46LAT\x10\x00\x12\x0e\n\nFRACTIONAL\x10\x01\x12\x0b\n\x07\x44\x45\x43IMAL\x10\x02\x1a\x34\n\x0c\x43urrencyPair\x12\x11\n\tcurrency1\x18\x01 \x01(\t\x12\x11\n\tcurrency2\x18\x02 \x01(\t\"\xb4\x01\n\x0eInstrumentType\x12\x1b\n\x17UNKNOWN_INSTRUMENT_TYPE\x10\x00\x12\t\n\x05\x46OREX\x10\x01\x12\t\n\x05INDEX\x10\x02\x12\n\n\x06\x45QUITY\x10\x03\x12\n\n\x06\x46UTURE\x10\x04\x12\n\n\x06OPTION\x10\x05\x12\n\n\x06SPREAD\x10\x06\x12\x0f\n\x0bMUTUAL_FUND\x10\x07\x12\x15\n\x11MONEY_MARKET_FUND\x10\x08\x12\x17\n\x13USER_DEFINED_SPREAD\x10\t\"Z\n\x08\x42ookType\x12\x15\n\x11UNKNOWN_BOOK_TYPE\x10\x00\x12\x0f\n\x0bTOP_OF_BOOK\x10\x01\x12\x15\n\x11PRICE_LEVEL_DEPTH\x10\x02\x12\x0f\n\x0bORDER_DEPTH\x10\x03\"8\n\nOptionType\x12\x17\n\x13UNKNOWN_OPTION_TYPE\x10\x00\x12\x08\n\x04\x43\x41LL\x10\x01\x12\x07\n\x03PUT\x10\x02\"Q\n\x0bOptionStyle\x12\x19\n\x15UNKNOWN_OPTIONS_STYLE\x10\x00\x12\x0b\n\x07\x44\x45\x46\x41ULT\x10\x01\x12\x0c\n\x08\x41MERICAN\x10\x02\x12\x0c\n\x08\x45UROPEAN\x10\x03\"3\n\x05State\x12\x11\n\rUNKNOWN_STATE\x10\x00\x12\n\n\x06\x41\x43TIVE\x10\x01\x12\x0b\n\x07PASSIVE\x10\x02\"\x9f\x02\n\tEventType\x12\x16\n\x12UNKNOWN_EVENT_TYPE\x10\x00\x12\x14\n\x10\x46IRST_TRADE_DATE\x10\x01\x12\x13\n\x0fLAST_TRADE_DATE\x10\x02\x12\x11\n\rMATURITY_DATE\x10\n\x12\x17\n\x13\x46IRST_DELIVERY_DATE\x10\x0b\x12\x16\n\x12LAST_DELIVERY_DATE\x10\x0c\x12\x15\n\x11\x46IRST_NOTICE_DATE\x10\r\x12\x14\n\x10LAST_NOTICE_DATE\x10\x0e\x12\x16\n\x12\x46IRST_HOLDING_DATE\x10\x0f\x12\x15\n\x11LAST_HOLDING_DATE\x10\x10\x12\x17\n\x13\x46IRST_POSITION_DATE\x10\x11\x12\x16\n\x12LAST_POSITION_DATE\x10\x12\x42\x07H\x01P\x01\xa0\x01\x01\x62\x06proto3'
 )
 
 
 
 _INSTRUMENTDEFINITION_PRICEFORMAT_SUBFORMAT = _descriptor.EnumDescriptor(
   name='SubFormat',
   full_name='org.openfeed.InstrumentDefinition.PriceFormat.SubFormat',
@@ -45,16 +45,16 @@
       name='DECIMAL', index=2, number=2,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=2637,
-  serialized_end=2687,
+  serialized_start=2795,
+  serialized_end=2845,
 )
 _sym_db.RegisterEnumDescriptor(_INSTRUMENTDEFINITION_PRICEFORMAT_SUBFORMAT)
 
 _INSTRUMENTDEFINITION_INSTRUMENTTYPE = _descriptor.EnumDescriptor(
   name='InstrumentType',
   full_name='org.openfeed.InstrumentDefinition.InstrumentType',
   filename=None,
@@ -102,19 +102,24 @@
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
       name='MONEY_MARKET_FUND', index=8, number=8,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='USER_DEFINED_SPREAD', index=9, number=9,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=2744,
-  serialized_end=2899,
+  serialized_start=2902,
+  serialized_end=3082,
 )
 _sym_db.RegisterEnumDescriptor(_INSTRUMENTDEFINITION_INSTRUMENTTYPE)
 
 _INSTRUMENTDEFINITION_BOOKTYPE = _descriptor.EnumDescriptor(
   name='BookType',
   full_name='org.openfeed.InstrumentDefinition.BookType',
   filename=None,
@@ -140,16 +145,16 @@
       name='ORDER_DEPTH', index=3, number=3,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=2901,
-  serialized_end=2991,
+  serialized_start=3084,
+  serialized_end=3174,
 )
 _sym_db.RegisterEnumDescriptor(_INSTRUMENTDEFINITION_BOOKTYPE)
 
 _INSTRUMENTDEFINITION_OPTIONTYPE = _descriptor.EnumDescriptor(
   name='OptionType',
   full_name='org.openfeed.InstrumentDefinition.OptionType',
   filename=None,
@@ -170,16 +175,16 @@
       name='PUT', index=2, number=2,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=2993,
-  serialized_end=3049,
+  serialized_start=3176,
+  serialized_end=3232,
 )
 _sym_db.RegisterEnumDescriptor(_INSTRUMENTDEFINITION_OPTIONTYPE)
 
 _INSTRUMENTDEFINITION_OPTIONSTYLE = _descriptor.EnumDescriptor(
   name='OptionStyle',
   full_name='org.openfeed.InstrumentDefinition.OptionStyle',
   filename=None,
@@ -205,16 +210,16 @@
       name='EUROPEAN', index=3, number=3,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=3051,
-  serialized_end=3132,
+  serialized_start=3234,
+  serialized_end=3315,
 )
 _sym_db.RegisterEnumDescriptor(_INSTRUMENTDEFINITION_OPTIONSTYLE)
 
 _INSTRUMENTDEFINITION_STATE = _descriptor.EnumDescriptor(
   name='State',
   full_name='org.openfeed.InstrumentDefinition.State',
   filename=None,
@@ -235,16 +240,16 @@
       name='PASSIVE', index=2, number=2,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=3134,
-  serialized_end=3185,
+  serialized_start=3317,
+  serialized_end=3368,
 )
 _sym_db.RegisterEnumDescriptor(_INSTRUMENTDEFINITION_STATE)
 
 _INSTRUMENTDEFINITION_EVENTTYPE = _descriptor.EnumDescriptor(
   name='EventType',
   full_name='org.openfeed.InstrumentDefinition.EventType',
   filename=None,
@@ -263,15 +268,15 @@
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
       name='LAST_TRADE_DATE', index=2, number=2,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='FINAL_SETTLEMENT_DATE', index=3, number=10,
+      name='MATURITY_DATE', index=3, number=10,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
       name='FIRST_DELIVERY_DATE', index=4, number=11,
       serialized_options=None,
       type=None,
@@ -310,16 +315,16 @@
       name='LAST_POSITION_DATE', index=11, number=18,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=3188,
-  serialized_end=3483,
+  serialized_start=3371,
+  serialized_end=3658,
 )
 _sym_db.RegisterEnumDescriptor(_INSTRUMENTDEFINITION_EVENTTYPE)
 
 
 _INSTRUMENTDEFINITION_SCHEDULE = _descriptor.Descriptor(
   name='Schedule',
   full_name='org.openfeed.InstrumentDefinition.Schedule',
@@ -343,16 +348,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2036,
-  serialized_end=2109,
+  serialized_start=2112,
+  serialized_end=2185,
 )
 
 _INSTRUMENTDEFINITION_TIMESPAN = _descriptor.Descriptor(
   name='TimeSpan',
   full_name='org.openfeed.InstrumentDefinition.TimeSpan',
   filename=None,
   file=DESCRIPTOR,
@@ -381,16 +386,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2111,
-  serialized_end=2160,
+  serialized_start=2187,
+  serialized_end=2236,
 )
 
 _INSTRUMENTDEFINITION_CALENDAR = _descriptor.Descriptor(
   name='Calendar',
   full_name='org.openfeed.InstrumentDefinition.Calendar',
   filename=None,
   file=DESCRIPTOR,
@@ -412,16 +417,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2162,
-  serialized_end=2230,
+  serialized_start=2238,
+  serialized_end=2306,
 )
 
 _INSTRUMENTDEFINITION_EVENT = _descriptor.Descriptor(
   name='Event',
   full_name='org.openfeed.InstrumentDefinition.Event',
   filename=None,
   file=DESCRIPTOR,
@@ -450,16 +455,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2232,
-  serialized_end=2313,
+  serialized_start=2308,
+  serialized_end=2389,
 )
 
 _INSTRUMENTDEFINITION_SPREADLEG = _descriptor.Descriptor(
   name='SpreadLeg',
   full_name='org.openfeed.InstrumentDefinition.SpreadLeg',
   filename=None,
   file=DESCRIPTOR,
@@ -483,28 +488,49 @@
     _descriptor.FieldDescriptor(
       name='symbol', full_name='org.openfeed.InstrumentDefinition.SpreadLeg.symbol', index=2,
       number=3, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='longSymbol', full_name='org.openfeed.InstrumentDefinition.SpreadLeg.longSymbol', index=3,
+      number=4, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='legOptionDelta', full_name='org.openfeed.InstrumentDefinition.SpreadLeg.legOptionDelta', index=4,
+      number=5, type=2, cpp_type=6, label=1,
+      has_default_value=False, default_value=float(0),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='legPrice', full_name='org.openfeed.InstrumentDefinition.SpreadLeg.legPrice', index=5,
+      number=6, type=2, cpp_type=6, label=1,
+      has_default_value=False, default_value=float(0),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2315,
-  serialized_end=2375,
+  serialized_start=2391,
+  serialized_end=2513,
 )
 
 _INSTRUMENTDEFINITION_MATURITYDATE = _descriptor.Descriptor(
   name='MaturityDate',
   full_name='org.openfeed.InstrumentDefinition.MaturityDate',
   filename=None,
   file=DESCRIPTOR,
@@ -540,16 +566,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2377,
-  serialized_end=2433,
+  serialized_start=2515,
+  serialized_end=2571,
 )
 
 _INSTRUMENTDEFINITION_SYMBOL = _descriptor.Descriptor(
   name='Symbol',
   full_name='org.openfeed.InstrumentDefinition.Symbol',
   filename=None,
   file=DESCRIPTOR,
@@ -566,28 +592,35 @@
     _descriptor.FieldDescriptor(
       name='symbol', full_name='org.openfeed.InstrumentDefinition.Symbol.symbol', index=1,
       number=2, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='longSymbol', full_name='org.openfeed.InstrumentDefinition.Symbol.longSymbol', index=2,
+      number=3, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2435,
-  serialized_end=2475,
+  serialized_start=2573,
+  serialized_end=2633,
 )
 
 _INSTRUMENTDEFINITION_PRICEFORMAT = _descriptor.Descriptor(
   name='PriceFormat',
   full_name='org.openfeed.InstrumentDefinition.PriceFormat',
   filename=None,
   file=DESCRIPTOR,
@@ -631,16 +664,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2478,
-  serialized_end=2687,
+  serialized_start=2636,
+  serialized_end=2845,
 )
 
 _INSTRUMENTDEFINITION_CURRENCYPAIR = _descriptor.Descriptor(
   name='CurrencyPair',
   full_name='org.openfeed.InstrumentDefinition.CurrencyPair',
   filename=None,
   file=DESCRIPTOR,
@@ -669,16 +702,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2689,
-  serialized_end=2741,
+  serialized_start=2847,
+  serialized_end=2899,
 )
 
 _INSTRUMENTDEFINITION = _descriptor.Descriptor(
   name='InstrumentDefinition',
   full_name='org.openfeed.InstrumentDefinition',
   filename=None,
   file=DESCRIPTOR,
@@ -1059,14 +1092,21 @@
     _descriptor.FieldDescriptor(
       name='subscriptionSymbol', full_name='org.openfeed.InstrumentDefinition.subscriptionSymbol', index=53,
       number=229, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='contractMaturity', full_name='org.openfeed.InstrumentDefinition.contractMaturity', index=54,
+      number=230, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[_INSTRUMENTDEFINITION_SCHEDULE, _INSTRUMENTDEFINITION_TIMESPAN, _INSTRUMENTDEFINITION_CALENDAR, _INSTRUMENTDEFINITION_EVENT, _INSTRUMENTDEFINITION_SPREADLEG, _INSTRUMENTDEFINITION_MATURITYDATE, _INSTRUMENTDEFINITION_SYMBOL, _INSTRUMENTDEFINITION_PRICEFORMAT, _INSTRUMENTDEFINITION_CURRENCYPAIR, ],
   enum_types=[
     _INSTRUMENTDEFINITION_INSTRUMENTTYPE,
     _INSTRUMENTDEFINITION_BOOKTYPE,
@@ -1078,15 +1118,15 @@
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=44,
-  serialized_end=3483,
+  serialized_end=3658,
 )
 
 _INSTRUMENTDEFINITION_SCHEDULE.fields_by_name['sessions'].message_type = _INSTRUMENTDEFINITION_TIMESPAN
 _INSTRUMENTDEFINITION_SCHEDULE.containing_type = _INSTRUMENTDEFINITION
 _INSTRUMENTDEFINITION_TIMESPAN.containing_type = _INSTRUMENTDEFINITION
 _INSTRUMENTDEFINITION_CALENDAR.fields_by_name['events'].message_type = _INSTRUMENTDEFINITION_EVENT
 _INSTRUMENTDEFINITION_CALENDAR.containing_type = _INSTRUMENTDEFINITION
@@ -1108,14 +1148,15 @@
 _INSTRUMENTDEFINITION.fields_by_name['priceFormat'].message_type = _INSTRUMENTDEFINITION_PRICEFORMAT
 _INSTRUMENTDEFINITION.fields_by_name['optionStrikePriceFormat'].message_type = _INSTRUMENTDEFINITION_PRICEFORMAT
 _INSTRUMENTDEFINITION.fields_by_name['symbols'].message_type = _INSTRUMENTDEFINITION_SYMBOL
 _INSTRUMENTDEFINITION.fields_by_name['optionType'].enum_type = _INSTRUMENTDEFINITION_OPTIONTYPE
 _INSTRUMENTDEFINITION.fields_by_name['optionStyle'].enum_type = _INSTRUMENTDEFINITION_OPTIONSTYLE
 _INSTRUMENTDEFINITION.fields_by_name['spreadLeg'].message_type = _INSTRUMENTDEFINITION_SPREADLEG
 _INSTRUMENTDEFINITION.fields_by_name['currencyPair'].message_type = _INSTRUMENTDEFINITION_CURRENCYPAIR
+_INSTRUMENTDEFINITION.fields_by_name['contractMaturity'].message_type = _INSTRUMENTDEFINITION_MATURITYDATE
 _INSTRUMENTDEFINITION_INSTRUMENTTYPE.containing_type = _INSTRUMENTDEFINITION
 _INSTRUMENTDEFINITION_BOOKTYPE.containing_type = _INSTRUMENTDEFINITION
 _INSTRUMENTDEFINITION_OPTIONTYPE.containing_type = _INSTRUMENTDEFINITION
 _INSTRUMENTDEFINITION_OPTIONSTYLE.containing_type = _INSTRUMENTDEFINITION
 _INSTRUMENTDEFINITION_STATE.containing_type = _INSTRUMENTDEFINITION
 _INSTRUMENTDEFINITION_EVENTTYPE.containing_type = _INSTRUMENTDEFINITION
 DESCRIPTOR.message_types_by_name['InstrumentDefinition'] = _INSTRUMENTDEFINITION
```

### Comparing `openfeed-1.2.0/openfeed/generated/openfeed_pb2.py` & `openfeed-1.3.0/openfeed/generated/openfeed_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='openfeed.proto',
   package='org.openfeed',
   syntax='proto3',
   serialized_options=b'H\001P\001\240\001\001',
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n\x0eopenfeed.proto\x12\x0corg.openfeed\x1a\x19openfeed_instrument.proto\"\xbe\x05\n\x0fOpenfeedMessage\x12\x13\n\x0bsendingTime\x18\x01 \x01(\x12\x12\x12\n\ntotalCount\x18\x02 \x01(\x11\x12\x14\n\x0csyncSequence\x18\x03 \x01(\x03\x12&\n\x07\x63ontext\x18\x04 \x01(\x0b\x32\x15.org.openfeed.Context\x12\x32\n\x0c\x63hannelReset\x18\n \x01(\x0b\x32\x1a.org.openfeed.ChannelResetH\x00\x12,\n\theartBeat\x18\x0b \x01(\x0b\x32\x17.org.openfeed.HeartBeatH\x00\x12\x32\n\x0c\x61\x64minMessage\x18\x0c \x01(\x0b\x32\x1a.org.openfeed.AdminMessageH\x00\x12\x42\n\x14instrumentDefinition\x18\r \x01(\x0b\x32\".org.openfeed.InstrumentDefinitionH\x00\x12\x44\n\x15instrumentGroupStatus\x18\x0e \x01(\x0b\x32#.org.openfeed.InstrumentGroupStatusH\x00\x12\x36\n\x0emarketSnapshot\x18\x0f \x01(\x0b\x32\x1c.org.openfeed.MarketSnapshotH\x00\x12\x32\n\x0cmarketUpdate\x18\x10 \x01(\x0b\x32\x1a.org.openfeed.MarketUpdateH\x00\x12\x32\n\x0cmarketStatus\x18\x11 \x01(\x0b\x32\x1a.org.openfeed.MarketStatusH\x00\x12@\n\x13\x65odCommoditySummary\x18\x12 \x01(\x0b\x32!.org.openfeed.EODCommoditySummaryH\x00\x12:\n\x10instrumentAction\x18\x13 \x01(\x0b\x32\x1e.org.openfeed.InstrumentActionH\x00\x42\x06\n\x04\x64\x61ta\"8\n\x0c\x43hannelReset\x12\x0f\n\x07\x63hannel\x18\x01 \x01(\x11\x12\x17\n\x0ftransactionTime\x18\x02 \x01(\x12\"W\n\tHeartBeat\x12\x17\n\x0ftransactionTime\x18\x01 \x01(\x12\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x10\n\x08\x65xchange\x18\x03 \x01(\x08\x12\x0f\n\x07\x63hannel\x18\x04 \x01(\x11\"\xc3\x01\n\x0c\x41\x64minMessage\x12\x17\n\x0foriginationTime\x18\x01 \x01(\x12\x12\x0e\n\x06source\x18\x02 \x01(\t\x12\x14\n\x0clanguageCode\x18\x03 \x01(\t\x12\x10\n\x08headLine\x18\x04 \x01(\t\x12\x0c\n\x04text\x18\x05 \x01(\t\x12\x31\n\x06status\x18\x06 \x01(\x0e\x32!.org.openfeed.AdminMessage.Status\x12\x0f\n\x07\x63hannel\x18\x07 \x01(\x11\"\x10\n\x06Status\x12\x06\n\x02OK\x10\x00\"\xad\x01\n\x15InstrumentGroupStatus\x12\x17\n\x0ftransactionTime\x18\x01 \x01(\x12\x12\x19\n\x11instrumentGroupId\x18\x02 \x01(\t\x12<\n\rtradingStatus\x18\x03 \x01(\x0e\x32%.org.openfeed.InstrumentTradingStatus\x12\x11\n\ttradeDate\x18\x04 \x01(\x11\x12\x0f\n\x07\x63hannel\x18\x05 \x01(\x11\"r\n\x0cMarketStatus\x12\x17\n\x0ftransactionTime\x18\x01 \x01(\x12\x12\x0f\n\x07\x63hannel\x18\x02 \x01(\x11\x12\x38\n\x10marketWideStatus\x18\x03 \x01(\x0e\x32\x1e.org.openfeed.MarketWideStatus\"\x93\x01\n\x13\x45ODCommoditySummary\x12\x11\n\ttradeDate\x18\x01 \x01(\x11\x12\x14\n\x0c\x63ontractRoot\x18\x02 \x01(\t\x12\x1a\n\x12\x63onsolidatedVolume\x18\x03 \x01(\x12\x12 \n\x18\x63onsolidatedOpenInterest\x18\x04 \x01(\x12\x12\x15\n\rauxiliaryData\x18\x63 \x01(\x0c\"\xe3\x03\n\rMarketSession\x12\x11\n\ttradeDate\x18\x04 \x01(\x11\x12 \n\x04open\x18\x1e \x01(\x0b\x32\x12.org.openfeed.Open\x12 \n\x04high\x18\x1f \x01(\x0b\x32\x12.org.openfeed.High\x12\x1e\n\x03low\x18  \x01(\x0b\x32\x11.org.openfeed.Low\x12 \n\x04last\x18# \x01(\x0b\x32\x12.org.openfeed.Last\x12$\n\x06volume\x18& \x01(\x0b\x32\x14.org.openfeed.Volume\x12,\n\nsettlement\x18\' \x01(\x0b\x32\x18.org.openfeed.Settlement\x12\x30\n\x0eprevSettlement\x18, \x01(\x0b\x32\x18.org.openfeed.Settlement\x12\x30\n\x0copenInterest\x18( \x01(\x0b\x32\x1a.org.openfeed.OpenInterest\x12\x34\n\x0enumberOfTrades\x18) \x01(\x0b\x32\x1c.org.openfeed.NumberOfTrades\x12\x32\n\rmonetaryValue\x18* \x01(\x0b\x32\x1b.org.openfeed.MonetaryValue\x12\x17\n\x0ftransactionTime\x18+ \x01(\x12\"\xcf\x0c\n\x0eMarketSnapshot\x12\x10\n\x08marketId\x18\x01 \x01(\x12\x12\x17\n\x0ftransactionTime\x18\x02 \x01(\x12\x12\x16\n\x0emarketSequence\x18\x03 \x01(\x03\x12\x11\n\ttradeDate\x18\x04 \x01(\x11\x12\x13\n\x0btotalChunks\x18\x05 \x01(\x11\x12\x14\n\x0c\x63urrentChunk\x18\x06 \x01(\x11\x12\x0e\n\x06symbol\x18\x07 \x01(\t\x12\x18\n\x10priceDenominator\x18\x08 \x01(\x11\x12&\n\x07service\x18\t \x01(\x0e\x32\x15.org.openfeed.Service\x12\x38\n\x10instrumentStatus\x18\n \x01(\x0b\x32\x1e.org.openfeed.InstrumentStatus\x12\'\n\x03\x62\x62o\x18\x0b \x01(\x0b\x32\x1a.org.openfeed.BestBidOffer\x12\'\n\x05index\x18\x0c \x01(\x0b\x32\x18.org.openfeed.IndexValue\x12\x30\n\x0bpriceLevels\x18\r \x03(\x0b\x32\x1b.org.openfeed.AddPriceLevel\x12&\n\x06orders\x18\x0e \x03(\x0b\x32\x16.org.openfeed.AddOrder\x12 \n\x04news\x18\x0f \x01(\x0b\x32\x12.org.openfeed.News\x12 \n\x04open\x18\x1e \x01(\x0b\x32\x12.org.openfeed.Open\x12 \n\x04high\x18\x1f \x01(\x0b\x32\x12.org.openfeed.High\x12\x1e\n\x03low\x18  \x01(\x0b\x32\x11.org.openfeed.Low\x12\"\n\x05\x63lose\x18! \x01(\x0b\x32\x13.org.openfeed.Close\x12*\n\tprevClose\x18\" \x01(\x0b\x32\x17.org.openfeed.PrevClose\x12 \n\x04last\x18# \x01(\x0b\x32\x12.org.openfeed.Last\x12(\n\x08yearHigh\x18$ \x01(\x0b\x32\x16.org.openfeed.YearHigh\x12&\n\x07yearLow\x18% \x01(\x0b\x32\x15.org.openfeed.YearLow\x12$\n\x06volume\x18& \x01(\x0b\x32\x14.org.openfeed.Volume\x12,\n\nsettlement\x18\' \x01(\x0b\x32\x18.org.openfeed.Settlement\x12\x30\n\x0copenInterest\x18( \x01(\x0b\x32\x1a.org.openfeed.OpenInterest\x12 \n\x04vwap\x18) \x01(\x0b\x32\x12.org.openfeed.Vwap\x12P\n\x1c\x64ividendsIncomeDistributions\x18* \x01(\x0b\x32*.org.openfeed.DividendsIncomeDistributions\x12\x34\n\x0enumberOfTrades\x18+ \x01(\x0b\x32\x1c.org.openfeed.NumberOfTrades\x12\x32\n\rmonetaryValue\x18, \x01(\x0b\x32\x1b.org.openfeed.MonetaryValue\x12@\n\x14\x63\x61pitalDistributions\x18- \x01(\x0b\x32\".org.openfeed.CapitalDistributions\x12:\n\x11sharesOutstanding\x18. \x01(\x0b\x32\x1f.org.openfeed.SharesOutstanding\x12\x32\n\rnetAssetValue\x18/ \x01(\x0b\x32\x1b.org.openfeed.NetAssetValue\x12\x34\n\x0fpreviousSession\x18\x30 \x01(\x0b\x32\x1b.org.openfeed.MarketSession\x12-\n\x08tSession\x18\x31 \x01(\x0b\x32\x1b.org.openfeed.MarketSession\x12\x32\n\rvolumeAtPrice\x18\x32 \x01(\x0b\x32\x1b.org.openfeed.VolumeAtPrice\x12.\n\x0bhighRolling\x18\x33 \x01(\x0b\x32\x19.org.openfeed.HighRolling\x12,\n\nlowRolling\x18\x34 \x01(\x0b\x32\x18.org.openfeed.LowRolling\x12-\n\x08zSession\x18\x35 \x01(\x0b\x32\x1b.org.openfeed.MarketSession\"\x94\x01\n\x16MarketSnapshotResponse\x12\x33\n\x06result\x18\x01 \x01(\x0e\x32#.org.openfeed.SnapshotRequestResult\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x34\n\x0emarketSnapshot\x18\x03 \x01(\x0b\x32\x1c.org.openfeed.MarketSnapshot\"\xbd\x0e\n\x0cMarketUpdate\x12\x10\n\x08marketId\x18\x01 \x01(\x12\x12\x0e\n\x06symbol\x18\x02 \x01(\t\x12\x17\n\x0ftransactionTime\x18\x03 \x01(\x12\x12\x18\n\x10\x64istributionTime\x18\x04 \x01(\x12\x12\x16\n\x0emarketSequence\x18\x05 \x01(\x12\x12\x16\n\x0esourceSequence\x18\x06 \x01(\x12\x12\x14\n\x0coriginatorId\x18\x07 \x01(\x0c\x12\x18\n\x10priceDenominator\x18\t \x01(\x11\x12&\n\x07\x63ontext\x18\n \x01(\x0b\x32\x15.org.openfeed.Context\x12,\n\x07session\x18\x0b \x01(\x0b\x32\x1b.org.openfeed.MarketSession\x12-\n\x08tSession\x18\x0c \x01(\x0b\x32\x1b.org.openfeed.MarketSession\x12\x34\n\x0fpreviousSession\x18\r \x01(\x0b\x32\x1b.org.openfeed.MarketSession\x12\x10\n\x08regional\x18\x0e \x01(\x08\x12-\n\x08zSession\x18\x0f \x01(\x0b\x32\x1b.org.openfeed.MarketSession\x12\"\n\x04news\x18\x14 \x01(\x0b\x32\x12.org.openfeed.NewsH\x00\x12,\n\tclearBook\x18\x15 \x01(\x0b\x32\x17.org.openfeed.ClearBookH\x00\x12:\n\x10instrumentStatus\x18\x16 \x01(\x0b\x32\x1e.org.openfeed.InstrumentStatusH\x00\x12)\n\x03\x62\x62o\x18\x17 \x01(\x0b\x32\x1a.org.openfeed.BestBidOfferH\x00\x12\x38\n\x0f\x64\x65pthPriceLevel\x18\x18 \x01(\x0b\x32\x1d.org.openfeed.DepthPriceLevelH\x00\x12.\n\ndepthOrder\x18\x19 \x01(\x0b\x32\x18.org.openfeed.DepthOrderH\x00\x12)\n\x05index\x18\x1a \x01(\x0b\x32\x18.org.openfeed.IndexValueH\x00\x12&\n\x06trades\x18\x1b \x01(\x0b\x32\x14.org.openfeed.TradesH\x00\x12\"\n\x04open\x18\x1c \x01(\x0b\x32\x12.org.openfeed.OpenH\x00\x12\"\n\x04high\x18\x1d \x01(\x0b\x32\x12.org.openfeed.HighH\x00\x12 \n\x03low\x18\x1e \x01(\x0b\x32\x11.org.openfeed.LowH\x00\x12$\n\x05\x63lose\x18\x1f \x01(\x0b\x32\x13.org.openfeed.CloseH\x00\x12,\n\tprevClose\x18  \x01(\x0b\x32\x17.org.openfeed.PrevCloseH\x00\x12\"\n\x04last\x18! \x01(\x0b\x32\x12.org.openfeed.LastH\x00\x12*\n\x08yearHigh\x18\" \x01(\x0b\x32\x16.org.openfeed.YearHighH\x00\x12(\n\x07yearLow\x18# \x01(\x0b\x32\x15.org.openfeed.YearLowH\x00\x12&\n\x06volume\x18$ \x01(\x0b\x32\x14.org.openfeed.VolumeH\x00\x12.\n\nsettlement\x18% \x01(\x0b\x32\x18.org.openfeed.SettlementH\x00\x12\x32\n\x0copenInterest\x18& \x01(\x0b\x32\x1a.org.openfeed.OpenInterestH\x00\x12\"\n\x04vwap\x18\' \x01(\x0b\x32\x12.org.openfeed.VwapH\x00\x12R\n\x1c\x64ividendsIncomeDistributions\x18( \x01(\x0b\x32*.org.openfeed.DividendsIncomeDistributionsH\x00\x12\x36\n\x0enumberOfTrades\x18) \x01(\x0b\x32\x1c.org.openfeed.NumberOfTradesH\x00\x12\x34\n\rmonetaryValue\x18* \x01(\x0b\x32\x1b.org.openfeed.MonetaryValueH\x00\x12\x42\n\x14\x63\x61pitalDistributions\x18+ \x01(\x0b\x32\".org.openfeed.CapitalDistributionsH\x00\x12<\n\x11sharesOutstanding\x18, \x01(\x0b\x32\x1f.org.openfeed.SharesOutstandingH\x00\x12\x34\n\rnetAssetValue\x18- \x01(\x0b\x32\x1b.org.openfeed.NetAssetValueH\x00\x12\x34\n\rmarketSummary\x18. \x01(\x0b\x32\x1b.org.openfeed.MarketSummaryH\x00\x12\x30\n\x0bhighRolling\x18/ \x01(\x0b\x32\x19.org.openfeed.HighRollingH\x00\x12.\n\nlowRolling\x18\x30 \x01(\x0b\x32\x18.org.openfeed.LowRollingH\x00\x42\x06\n\x04\x64\x61taJ\x04\x08\x08\x10\t\"\x86\x02\n\x0f\x44\x65pthPriceLevel\x12\x33\n\x06levels\x18\x01 \x03(\x0b\x32#.org.openfeed.DepthPriceLevel.Entry\x1a\xbd\x01\n\x05\x45ntry\x12\x34\n\raddPriceLevel\x18\x01 \x01(\x0b\x32\x1b.org.openfeed.AddPriceLevelH\x00\x12:\n\x10\x64\x65letePriceLevel\x18\x02 \x01(\x0b\x32\x1e.org.openfeed.DeletePriceLevelH\x00\x12:\n\x10modifyPriceLevel\x18\x03 \x01(\x0b\x32\x1e.org.openfeed.ModifyPriceLevelH\x00\x42\x06\n\x04\x64\x61ta\"\xde\x01\n\nDepthOrder\x12.\n\x06orders\x18\x01 \x03(\x0b\x32\x1e.org.openfeed.DepthOrder.Entry\x1a\x9f\x01\n\x05\x45ntry\x12*\n\x08\x61\x64\x64Order\x18\x01 \x01(\x0b\x32\x16.org.openfeed.AddOrderH\x00\x12\x30\n\x0b\x64\x65leteOrder\x18\x02 \x01(\x0b\x32\x19.org.openfeed.DeleteOrderH\x00\x12\x30\n\x0bmodifyOrder\x18\x03 \x01(\x0b\x32\x19.org.openfeed.ModifyOrderH\x00\x42\x06\n\x04\x64\x61ta\"v\n\x04News\x12\x17\n\x0foriginationTime\x18\x01 \x01(\x12\x12\x0e\n\x06source\x18\x02 \x01(\t\x12\x14\n\x0clanguageCode\x18\x03 \x01(\t\x12\x10\n\x08headLine\x18\x04 \x01(\t\x12\x0c\n\x04text\x18\x05 \x01(\t\x12\x0f\n\x07symbols\x18\x06 \x03(\t\"6\n\tClearBook\x12\x10\n\x08reserved\x18\x01 \x01(\x11\x12\x17\n\x0ftransactionTime\x18\x02 \x01(\x12\"\xf7\x01\n\x10InstrumentStatus\x12\x17\n\x0ftransactionTime\x18\t \x01(\x12\x12<\n\rtradingStatus\x18\n \x01(\x0e\x32%.org.openfeed.InstrumentTradingStatus\x12\x13\n\x0bopeningTime\x18\x0b \x01(\x12\x12\x0c\n\x04note\x18\x0c \x01(\t\x12\x11\n\ttradeDate\x18\r \x01(\x11\x12V\n\x1fregulationSHOShortSalePriceTest\x18\x0e \x01(\x0e\x32-.org.openfeed.RegulationSHOShortSalePriceTest\"\xd4\x02\n\x0c\x42\x65stBidOffer\x12\x17\n\x0ftransactionTime\x18\t \x01(\x12\x12\x10\n\x08\x62idPrice\x18\n \x01(\x12\x12\x13\n\x0b\x62idQuantity\x18\x0b \x01(\x12\x12\x15\n\rbidOrderCount\x18\x0c \x01(\x11\x12\x15\n\rbidOriginator\x18\r \x01(\x0c\x12\x19\n\x11\x62idQuoteCondition\x18\x0e \x01(\x0c\x12\x12\n\nofferPrice\x18\x14 \x01(\x12\x12\x15\n\rofferQuantity\x18\x15 \x01(\x12\x12\x17\n\x0fofferOrderCount\x18\x16 \x01(\x11\x12\x17\n\x0fofferOriginator\x18\x17 \x01(\x0c\x12\x1b\n\x13offerQuoteCondition\x18\x18 \x01(\x0c\x12\x16\n\x0equoteCondition\x18\x1e \x01(\x0c\x12\x10\n\x08regional\x18  \x01(\x08\x12\x11\n\ttransient\x18! \x01(\x08J\x04\x08\x1f\x10 \"\xab\x01\n\rAddPriceLevel\x12\x17\n\x0ftransactionTime\x18\t \x01(\x12\x12\r\n\x05level\x18\n \x01(\x11\x12$\n\x04side\x18\x0b \x01(\x0e\x32\x16.org.openfeed.BookSide\x12\r\n\x05price\x18\x0c \x01(\x12\x12\x10\n\x08quantity\x18\r \x01(\x12\x12\x12\n\norderCount\x18\x0e \x01(\x11\x12\x17\n\x0fimpliedQuantity\x18\x0f \x01(\x12\"`\n\x10\x44\x65letePriceLevel\x12\x17\n\x0ftransactionTime\x18\t \x01(\x12\x12\r\n\x05level\x18\n \x01(\x11\x12$\n\x04side\x18\x0b \x01(\x0e\x32\x16.org.openfeed.BookSide\"\xae\x01\n\x10ModifyPriceLevel\x12\x17\n\x0ftransactionTime\x18\t \x01(\x12\x12\r\n\x05level\x18\n \x01(\x11\x12$\n\x04side\x18\x0b \x01(\x0e\x32\x16.org.openfeed.BookSide\x12\r\n\x05price\x18\x0c \x01(\x12\x12\x10\n\x08quantity\x18\r \x01(\x12\x12\x12\n\norderCount\x18\x0e \x01(\x11\x12\x17\n\x0fimpliedQuantity\x18\x0f \x01(\x12\"\xa0\x01\n\x08\x41\x64\x64Order\x12\x17\n\x0ftransactionTime\x18\t \x01(\x12\x12\x0f\n\x07orderId\x18\n \x01(\x12\x12$\n\x04side\x18\x0b \x01(\x0e\x32\x16.org.openfeed.BookSide\x12\r\n\x05price\x18\x0c \x01(\x12\x12\x10\n\x08quantity\x18\r \x01(\x12\x12\x11\n\tisImplied\x18\x0e \x01(\x08\x12\x10\n\x08priority\x18\x0f \x01(\x12\"]\n\x0b\x44\x65leteOrder\x12\x17\n\x0ftransactionTime\x18\t \x01(\x12\x12\x0f\n\x07orderId\x18\n \x01(\x12\x12$\n\x04side\x18\x0b \x01(\x0e\x32\x16.org.openfeed.BookSide\"\xa3\x01\n\x0bModifyOrder\x12\x17\n\x0ftransactionTime\x18\t \x01(\x12\x12\x0f\n\x07orderId\x18\n \x01(\x12\x12$\n\x04side\x18\x0b \x01(\x0e\x32\x16.org.openfeed.BookSide\x12\r\n\x05price\x18\x0c \x01(\x12\x12\x10\n\x08quantity\x18\r \x01(\x12\x12\x11\n\tisImplied\x18\x0e \x01(\x08\x12\x10\n\x08priority\x18\x0f \x01(\x12\"\xd7\x01\n\nIndexValue\x12\x17\n\x0ftransactionTime\x18\t \x01(\x12\x12\x11\n\ttradeDate\x18\n \x01(\x11\x12\x0c\n\x04last\x18\x0b \x01(\x12\x12\x0e\n\x06volume\x18\x0c \x01(\x12\x12\x0c\n\x04open\x18\r \x01(\x12\x12\x16\n\x0esettlementOpen\x18\x0e \x01(\x12\x12\x13\n\x0bspecialOpen\x18\x0f \x01(\x12\x12\x0c\n\x04high\x18\x10 \x01(\x12\x12\x0b\n\x03low\x18\x11 \x01(\x12\x12\r\n\x05\x63lose\x18\x12 \x01(\x12\x12\x0b\n\x03\x62id\x18\x13 \x01(\x12\x12\r\n\x05offer\x18\x14 \x01(\x12\"\xd8\x01\n\x06Trades\x12*\n\x06trades\x18\x01 \x03(\x0b\x32\x1a.org.openfeed.Trades.Entry\x1a\xa1\x01\n\x05\x45ntry\x12$\n\x05trade\x18\x01 \x01(\x0b\x32\x13.org.openfeed.TradeH\x00\x12\x38\n\x0ftradeCorrection\x18\x02 \x01(\x0b\x32\x1d.org.openfeed.TradeCorrectionH\x00\x12\x30\n\x0btradeCancel\x18\x03 \x01(\x0b\x32\x19.org.openfeed.TradeCancelH\x00\x42\x06\n\x04\x64\x61ta\"\x8f\x05\n\x05Trade\x12\x14\n\x0coriginatorId\x18\x08 \x01(\x0c\x12\x17\n\x0ftransactionTime\x18\t \x01(\x12\x12\r\n\x05price\x18\n \x01(\x12\x12\x10\n\x08quantity\x18\x0b \x01(\x12\x12\x0f\n\x07tradeId\x18\x0c \x01(\x0c\x12$\n\x04side\x18\r \x01(\x0e\x32\x16.org.openfeed.BookSide\x12\x11\n\ttradeDate\x18\x0e \x01(\x11\x12\x0f\n\x07\x62uyerId\x18\x0f \x01(\x0c\x12\x10\n\x08sellerId\x18\x10 \x01(\x0c\x12\x14\n\x0copeningTrade\x18\x11 \x01(\x08\x12\x14\n\x0csystemPriced\x18\x12 \x01(\x08\x12\x15\n\rmarketOnClose\x18\x13 \x01(\x08\x12\x0e\n\x06oddLot\x18\x14 \x01(\x08\x12\x36\n\x0fsettlementTerms\x18\x15 \x01(\x0e\x32\x1d.org.openfeed.SettlementTerms\x12*\n\tcrossType\x18\x16 \x01(\x0e\x32\x17.org.openfeed.CrossType\x12\x0e\n\x06\x62yPass\x18\x17 \x01(\x08\x12\x11\n\tlastPrice\x18\x18 \x01(\x12\x12\x15\n\rsaleCondition\x18\x19 \x01(\x0c\x12\x10\n\x08\x63urrency\x18\x1a \x01(\t\x12\x19\n\x11\x64oesNotUpdateLast\x18\x1b \x01(\x08\x12\x1b\n\x13\x64oesNotUpdateVolume\x18\x1c \x01(\x08\x12\x0f\n\x07session\x18\x1e \x01(\t\x12\x12\n\nblockTrade\x18\x1f \x01(\x08\x12\x18\n\x10\x64istributionTime\x18  \x01(\x12\x12\x18\n\x10transactionTime2\x18! \x01(\x12\x12\"\n\x1a\x63onsolidatedPriceIndicator\x18\" \x01(\t\x12\x11\n\ttransient\x18# \x01(\x08\"\xc6\x04\n\x0fTradeCorrection\x12\x14\n\x0coriginatorId\x18\x08 \x01(\x0c\x12\x17\n\x0ftransactionTime\x18\t \x01(\x12\x12\r\n\x05price\x18\n \x01(\x12\x12\x10\n\x08quantity\x18\x0b \x01(\x12\x12\x0f\n\x07tradeId\x18\x0c \x01(\x0c\x12$\n\x04side\x18\r \x01(\x0e\x32\x16.org.openfeed.BookSide\x12\x11\n\ttradeDate\x18\x0e \x01(\x11\x12\x0f\n\x07\x62uyerId\x18\x0f \x01(\x0c\x12\x10\n\x08sellerId\x18\x10 \x01(\x0c\x12\x14\n\x0copeningTrade\x18\x11 \x01(\x08\x12\x14\n\x0csystemPriced\x18\x12 \x01(\x08\x12\x15\n\rmarketOnClose\x18\x13 \x01(\x08\x12\x0e\n\x06oddLot\x18\x14 \x01(\x08\x12\x36\n\x0fsettlementTerms\x18\x15 \x01(\x0e\x32\x1d.org.openfeed.SettlementTerms\x12*\n\tcrossType\x18\x16 \x01(\x0e\x32\x17.org.openfeed.CrossType\x12\x0e\n\x06\x62yPass\x18\x17 \x01(\x08\x12\x17\n\x0foriginalTradeId\x18\x18 \x01(\x0c\x12\x15\n\rsaleCondition\x18\x19 \x01(\x0c\x12\x10\n\x08\x63urrency\x18\x1a \x01(\t\x12\x18\n\x10\x64istributionTime\x18\x1b \x01(\x12\x12\x18\n\x10transactionTime2\x18\x1c \x01(\x12\x12\x1a\n\x12originalTradePrice\x18\x1d \x01(\x12\x12\x1d\n\x15originalTradeQuantity\x18\x1e \x01(\x12\"\xe7\x01\n\x0bTradeCancel\x12\x14\n\x0coriginatorId\x18\x08 \x01(\x0c\x12\x17\n\x0ftransactionTime\x18\t \x01(\x12\x12\x1b\n\x13\x63orrectedTradePrice\x18\n \x01(\x12\x12\x1e\n\x16\x63orrectedTradeQuantity\x18\x0b \x01(\x12\x12\x0f\n\x07tradeId\x18\x0c \x01(\x0c\x12\x15\n\rsaleCondition\x18\r \x01(\x0c\x12\x10\n\x08\x63urrency\x18\x0e \x01(\t\x12\x18\n\x10\x64istributionTime\x18\x0f \x01(\x12\x12\x18\n\x10transactionTime2\x18\x10 \x01(\x12\"\x9b\x01\n\x04Open\x12\x17\n\x0ftransactionTime\x18\t \x01(\x12\x12\x11\n\ttradeDate\x18\n \x01(\x11\x12\r\n\x05price\x18\x0b \x01(\x12\x12\x46\n\x17OpenCloseSettlementFlag\x18\x0c \x01(\x0e\x32%.org.openfeed.OpenCloseSettlementFlag\x12\x10\n\x08\x63urrency\x18\r \x01(\t\"S\n\x04High\x12\x17\n\x0ftransactionTime\x18\t \x01(\x12\x12\x11\n\ttradeDate\x18\n \x01(\x11\x12\r\n\x05price\x18\x0b \x01(\x12\x12\x10\n\x08\x63urrency\x18\x0c \x01(\t\"Z\n\x0bHighRolling\x12\x17\n\x0ftransactionTime\x18\t \x01(\x12\x12\x11\n\ttradeDate\x18\n \x01(\x11\x12\r\n\x05price\x18\x0b \x01(\x12\x12\x10\n\x08\x63urrency\x18\x0c \x01(\t\"R\n\x03Low\x12\x17\n\x0ftransactionTime\x18\t \x01(\x12\x12\x11\n\ttradeDate\x18\n \x01(\x11\x12\r\n\x05price\x18\x0b \x01(\x12\x12\x10\n\x08\x63urrency\x18\x0c \x01(\t\"Y\n\nLowRolling\x12\x17\n\x0ftransactionTime\x18\t \x01(\x12\x12\x11\n\ttradeDate\x18\n \x01(\x11\x12\r\n\x05price\x18\x0b \x01(\x12\x12\x10\n\x08\x63urrency\x18\x0c \x01(\t\"T\n\x05\x43lose\x12\x17\n\x0ftransactionTime\x18\t \x01(\x12\x12\x11\n\ttradeDate\x18\n \x01(\x11\x12\r\n\x05price\x18\x0b \x01(\x12\x12\x10\n\x08\x63urrency\x18\x0c \x01(\t\"X\n\tPrevClose\x12\x17\n\x0ftransactionTime\x18\t \x01(\x12\x12\x11\n\ttradeDate\x18\n \x01(\x11\x12\r\n\x05price\x18\x0b \x01(\x12\x12\x10\n\x08\x63urrency\x18\x0c \x01(\t\"v\n\x04Last\x12\x17\n\x0ftransactionTime\x18\t \x01(\x12\x12\x11\n\ttradeDate\x18\n \x01(\x11\x12\r\n\x05price\x18\x0b \x01(\x12\x12\x10\n\x08quantity\x18\x0c \x01(\x12\x12\x10\n\x08\x63urrency\x18\r \x01(\t\x12\x0f\n\x07session\x18\x1e \x01(\t\"D\n\x08YearHigh\x12\x17\n\x0ftransactionTime\x18\t \x01(\x12\x12\r\n\x05price\x18\n \x01(\x12\x12\x10\n\x08\x63urrency\x18\x0b \x01(\t\"C\n\x07YearLow\x12\x17\n\x0ftransactionTime\x18\t \x01(\x12\x12\r\n\x05price\x18\n \x01(\x12\x12\x10\n\x08\x63urrency\x18\x0b \x01(\t\"D\n\x06Volume\x12\x17\n\x0ftransactionTime\x18\t \x01(\x12\x12\x11\n\ttradeDate\x18\n \x01(\x11\x12\x0e\n\x06volume\x18\x0b \x01(\x12\"R\n\x0eNumberOfTrades\x12\x17\n\x0ftransactionTime\x18\t \x01(\x12\x12\x11\n\ttradeDate\x18\n \x01(\x11\x12\x14\n\x0cnumberTrades\x18\x0b \x01(\x12\"e\n\rMonetaryValue\x12\x17\n\x0ftransactionTime\x18\t \x01(\x12\x12\x11\n\ttradeDate\x18\n \x01(\x11\x12\r\n\x05value\x18\x0b \x01(\x12\x12\x19\n\x11valueCurrencyCode\x18\x0c \x01(\t\"\xe4\x01\n\nSettlement\x12\x17\n\x0ftransactionTime\x18\t \x01(\x12\x12\x11\n\ttradeDate\x18\n \x01(\x11\x12\r\n\x05price\x18\x0b \x01(\x12\x12\x19\n\x11preliminarySettle\x18\x0c \x01(\x08\x12\x10\n\x08\x63urrency\x18\r \x01(\t\x12\x38\n\x10settlementSource\x18\x0e \x01(\x0e\x32\x1e.org.openfeed.SettlementSource\x12\x0f\n\x07session\x18\x0f \x01(\t\x12\x11\n\ttransient\x18\x10 \x01(\x08\x12\x10\n\x08reserved\x18\x7f \x01(\x08\"J\n\x0cOpenInterest\x12\x17\n\x0ftransactionTime\x18\t \x01(\x12\x12\x11\n\ttradeDate\x18\n \x01(\x11\x12\x0e\n\x06volume\x18\x0b \x01(\x12\"@\n\x04Vwap\x12\x17\n\x0ftransactionTime\x18\t \x01(\x12\x12\x11\n\ttradeDate\x18\n \x01(\x11\x12\x0c\n\x04vwap\x18\x0b \x01(\x12\"\xf8\x03\n\x1c\x44ividendsIncomeDistributions\x12\x17\n\x0ftransactionTime\x18\x06 \x01(\x12\x12\x16\n\x0einstrumentType\x18\x07 \x01(\t\x12\x17\n\x0f\x63orporateAction\x18\x08 \x01(\t\x12\x18\n\x10\x64istributionType\x18\t \x01(\t\x12\x13\n\x0bpayableDate\x18\n \x01(\x11\x12\x12\n\nrecordDate\x18\x0b \x01(\x11\x12\x16\n\x0e\x65xDividendDate\x18\x0c \x01(\x11\x12\x0e\n\x06\x61mount\x18\r \x01(\x12\x12\x14\n\x0c\x63urrencyCode\x18\x0e \x01(\t\x12\r\n\x05notes\x18\x0f \x03(\t\x12\x1d\n\x15totalCashDistribution\x18\x10 \x01(\x12\x12$\n\x1cnonQualifiedCashDistribution\x18\x11 \x01(\x12\x12!\n\x19qualifiedCashDistribution\x18\x12 \x01(\x12\x12\x1f\n\x17taxFreeCashDistribution\x18\x13 \x01(\x12\x12 \n\x18ordinaryForeignTaxCredit\x18\x14 \x01(\x12\x12!\n\x19qualifiedForeignTaxCredit\x18\x15 \x01(\x12\x12\x1a\n\x12stockDividendRatio\x18\x16 \x01(\x12\x12\x14\n\x0creinvestDate\x18\x17 \x01(\x11\"\xca\x02\n\x14\x43\x61pitalDistributions\x12\x17\n\x0ftransactionTime\x18\x08 \x01(\x12\x12\x16\n\x0einstrumentType\x18\t \x01(\t\x12\x17\n\x0f\x63orporateAction\x18\n \x01(\t\x12\x13\n\x0bpayableDate\x18\x0b \x01(\x11\x12\x12\n\nrecordDate\x18\x0c \x01(\x11\x12\x0e\n\x06\x65xDate\x18\r \x01(\x11\x12\x1c\n\x14shortTermCapitalGain\x18\x0e \x01(\x12\x12\x1b\n\x13longTermCapitalGain\x18\x0f \x01(\x12\x12 \n\x18unallocatedDistributions\x18\x10 \x01(\x12\x12\x17\n\x0freturnOfCapital\x18\x11 \x01(\x12\x12\x14\n\x0c\x63urrencyCode\x18\x12 \x01(\t\x12\r\n\x05notes\x18\x13 \x03(\t\x12\x14\n\x0creinvestDate\x18\x14 \x01(\x11\"G\n\x11SharesOutstanding\x12\x19\n\x11sharesOutstanding\x18\x01 \x01(\x12\x12\x17\n\x0ftransactionTime\x18\x02 \x01(\x12\"?\n\rNetAssetValue\x12\x15\n\rnetAssetValue\x18\x01 \x01(\x12\x12\x17\n\x0ftransactionTime\x18\x02 \x01(\x12\"\xc7\x07\n\rMarketSummary\x12\x17\n\x0ftransactionTime\x18\x01 \x01(\x12\x12\x13\n\x0btradingDate\x18\x02 \x01(\x11\x12\x12\n\nstartOfDay\x18\x03 \x01(\x08\x12\x10\n\x08\x65ndOfDay\x18\x04 \x01(\x08\x12\x33\n\x05\x63lear\x18\x05 \x01(\x0e\x32$.org.openfeed.MarketSummary.ClearSet\x12\x38\n\x10instrumentStatus\x18\t \x01(\x0b\x32\x1e.org.openfeed.InstrumentStatus\x12\'\n\x03\x62\x62o\x18\n \x01(\x0b\x32\x1a.org.openfeed.BestBidOffer\x12 \n\x04open\x18\x0b \x01(\x0b\x32\x12.org.openfeed.Open\x12 \n\x04high\x18\x0c \x01(\x0b\x32\x12.org.openfeed.High\x12\x1e\n\x03low\x18\r \x01(\x0b\x32\x11.org.openfeed.Low\x12\"\n\x05\x63lose\x18\x0e \x01(\x0b\x32\x13.org.openfeed.Close\x12*\n\tprevClose\x18\x0f \x01(\x0b\x32\x17.org.openfeed.PrevClose\x12 \n\x04last\x18\x10 \x01(\x0b\x32\x12.org.openfeed.Last\x12$\n\x06volume\x18\x11 \x01(\x0b\x32\x14.org.openfeed.Volume\x12,\n\nsettlement\x18\x12 \x01(\x0b\x32\x18.org.openfeed.Settlement\x12\x30\n\x0copenInterest\x18\x13 \x01(\x0b\x32\x1a.org.openfeed.OpenInterest\x12 \n\x04vwap\x18\x14 \x01(\x0b\x32\x12.org.openfeed.Vwap\x12\x0f\n\x07session\x18\x15 \x01(\t\x12<\n\x0bsummaryType\x18\x16 \x01(\x0e\x32\'.org.openfeed.MarketSummary.SummaryType\x12(\n\nprevVolume\x18\x17 \x01(\x0b\x32\x14.org.openfeed.Volume\x12\x11\n\ttransient\x18\x18 \x01(\x08\"3\n\x08\x43learSet\x12\x08\n\x04NONE\x10\x00\x12\x07\n\x03\x41LL\x10\x01\x12\x06\n\x02\x42\x41\x10\x02\x12\x0c\n\x08\x43USTOM_1\x10\x03\"\x8a\x01\n\x0bSummaryType\x12\x14\n\x10\x45XCHANGE_REFRESH\x10\x00\x12\x16\n\x12REFRESH_LIVE_PRICE\x10\x01\x12\x18\n\x14\x45OD_COMMODITY_PRICES\x10\x02\x12\x1a\n\x16\x45OD_STOCK_FOREX_PRICES\x10\x03\x12\x17\n\x13\x45OD_COMMODITY_STATS\x10\x04\"a\n\x07\x43ontext\x12\'\n\x04\x64\x61ta\x18\x01 \x03(\x0b\x32\x19.org.openfeed.ContextData\x12-\n\x0btracePoints\x18\x02 \x03(\x0b\x32\x18.org.openfeed.TracePoint\"\xa2\x01\n\x0b\x43ontextData\x12\n\n\x02id\x18\x01 \x01(\t\x12\x11\n\x07vstring\x18\x05 \x01(\tH\x00\x12\x10\n\x06vbytes\x18\x06 \x01(\x0cH\x00\x12\x0f\n\x05vbool\x18\x07 \x01(\x08H\x00\x12\x11\n\x07vsint32\x18\x08 \x01(\x11H\x00\x12\x11\n\x07vsint64\x18\t \x01(\x12H\x00\x12\x10\n\x06vfloat\x18\n \x01(\x02H\x00\x12\x11\n\x07vdouble\x18\x0b \x01(\x01H\x00\x42\x06\n\x04\x64\x61ta\"^\n\nTracePoint\x12\n\n\x02id\x18\x01 \x01(\t\x12\x13\n\x0b\x63omponentId\x18\x02 \x01(\t\x12\x13\n\x0btimestampNs\x18\x03 \x01(\x12\x12\x1a\n\x12\x63omponentLatencyNs\x18\x04 \x01(\x05\"v\n\x1aTCPHistoricalReplayRequest\x12\x0f\n\x07\x63hannel\x18\x01 \x01(\x05\x12\x13\n\x0bresetNumber\x18\x02 \x01(\x05\x12\x10\n\x08sequence\x18\x03 \x01(\x03\x12\r\n\x05\x63ount\x18\x04 \x01(\x05\x12\x11\n\trequestId\x18\x05 \x01(\t\"\xe6\x01\n\x0fSnapshotRequest\x12\x0f\n\x07\x63hannel\x18\x01 \x01(\x05\x12\x13\n\x0bresetNumber\x18\x02 \x01(\x05\x12\x11\n\trequestId\x18\x03 \x01(\t\x12O\n\x14snapshotRequestTypes\x18\x04 \x03(\x0e\x32\x31.org.openfeed.SnapshotRequest.SnapshotRequestType\"I\n\x13SnapshotRequestType\x12\x07\n\x03\x41LL\x10\x00\x12\t\n\x05QUOTE\x10\x01\x12\t\n\x05\x44\x45PTH\x10\x02\x12\x13\n\x0fVOLUME_AT_PRICE\x10\x03\"\x9b\x02\n\rVolumeAtPrice\x12\x10\n\x08marketId\x18\x01 \x01(\x12\x12\x0e\n\x06symbol\x18\x02 \x01(\t\x12\x17\n\x0ftransactionTime\x18\x03 \x01(\x12\x12\x11\n\tlastPrice\x18\x04 \x01(\x12\x12\x14\n\x0clastQuantity\x18\x05 \x01(\x12\x12\x1c\n\x14lastCumulativeVolume\x18\x06 \x01(\x12\x12\x11\n\ttradeDate\x18\x07 \x01(\x11\x12\x42\n\x0cpriceVolumes\x18\x08 \x03(\x0b\x32,.org.openfeed.VolumeAtPrice.PriceLevelVolume\x1a\x31\n\x10PriceLevelVolume\x12\r\n\x05price\x18\x01 \x01(\x12\x12\x0e\n\x06volume\x18\x02 \x01(\x12\"\xd6\x02\n\x04Ohlc\x12\x10\n\x08marketId\x18\x01 \x01(\x12\x12\x0e\n\x06symbol\x18\x02 \x01(\t\x12 \n\x04open\x18\x03 \x01(\x0b\x32\x12.org.openfeed.Open\x12 \n\x04high\x18\x04 \x01(\x0b\x32\x12.org.openfeed.High\x12\x1e\n\x03low\x18\x05 \x01(\x0b\x32\x11.org.openfeed.Low\x12\"\n\x05\x63lose\x18\x06 \x01(\x0b\x32\x13.org.openfeed.Close\x12\x0e\n\x06volume\x18\x07 \x01(\x12\x12\x13\n\x0bpriceVolume\x18\x08 \x01(\x01\x12\x14\n\x0cnumberTrades\x18\t \x01(\x12\x12\x11\n\ttradeDate\x18\n \x01(\x11\x12\x17\n\x0ftransactionTime\x18\x0b \x01(\x12\x12\x10\n\x08tradeIds\x18\x0c \x03(\t\x12\x15\n\ropenStartTime\x18\r \x01(\x12\x12\x14\n\x0c\x63loseEndTime\x18\x0e \x01(\x12\"\xec\x01\n\x10InstrumentAction\x12\x17\n\x0ftransactionTime\x18\x01 \x01(\x12\x12\x11\n\ttradeDate\x18\x02 \x01(\x11\x12(\n\x06\x61\x63tion\x18\x03 \x01(\x0e\x32\x18.org.openfeed.ActionType\x12\x0f\n\x07message\x18\x04 \x01(\t\x12\x36\n\ninstrument\x18\n \x01(\x0b\x32\".org.openfeed.InstrumentDefinition\x12\x39\n\rnewInstrument\x18\x0b \x01(\x0b\x32\".org.openfeed.InstrumentDefinition*5\n\x08\x42ookSide\x12\x15\n\x11UNKNOWN_BOOK_SIDE\x10\x00\x12\x07\n\x03\x42ID\x10\x01\x12\t\n\x05OFFER\x10\x02*\xa0\x05\n\x17InstrumentTradingStatus\x12\x1a\n\x16UNKNOWN_TRADING_STATUS\x10\x00\x12\x12\n\x0eTRADING_RESUME\x10\x01\x12\x0c\n\x08PRE_OPEN\x10\x02\x12\x08\n\x04OPEN\x10\x03\x12\r\n\tPRE_CLOSE\x10\x04\x12\t\n\x05\x43LOSE\x10\x05\x12\x10\n\x0cTRADING_HALT\x10\x06\x12\x14\n\x10QUOTATION_RESUME\x10\x07\x12\x0e\n\nOPEN_DELAY\x10\x08\x12\x15\n\x11NO_OPEN_NO_RESUME\x10\t\x12\x0f\n\x0b\x46\x41ST_MARKET\x10\n\x12\x13\n\x0f\x46\x41ST_MARKET_END\x10\x0b\x12\x0f\n\x0bLATE_MARKET\x10\x0c\x12\x13\n\x0fLATE_MARKET_END\x10\r\x12\x10\n\x0cPOST_SESSION\x10\x0e\x12\x14\n\x10POST_SESSION_END\x10\x0f\x12\x18\n\x14NEW_PRICE_INDICATION\x10\x10\x12\x1d\n\x19NOT_AVAILABLE_FOR_TRADING\x10\x11\x12\r\n\tPRE_CROSS\x10\x12\x12\t\n\x05\x43ROSS\x10\x13\x12\x0e\n\nPOST_CLOSE\x10\x14\x12\r\n\tNO_CHANGE\x10\x15\x12\x08\n\x04NAFT\x10\x16\x12\x1c\n\x18TRADING_RANGE_INDICATION\x10\x17\x12\x18\n\x14MARKET_IMBALANCE_BUY\x10\x18\x12\x19\n\x15MARKET_IMBALANCE_SELL\x10\x19\x12\x15\n\x11MOC_IMBALANCE_BUY\x10\x1a\x12\x16\n\x12MOC_IMBALANCE_SELL\x10\x1b\x12\x17\n\x13NO_MARKET_IMBALANCE\x10\x1c\x12\x14\n\x10NO_MOC_IMBALANCE\x10\x1d\x12\x1a\n\x16SHORT_SELL_RESTRICTION\x10\x1e\x12\x17\n\x13LIMIT_UP_LIMIT_DOWN\x10\x1f*\x8a\x01\n\x1fRegulationSHOShortSalePriceTest\x12\x16\n\x12UNKNOWN_PRICE_TEST\x10\x00\x12\x13\n\x0fPRICE_TEST_NONE\x10\x01\x12\x18\n\x14PRICE_TEST_IN_EFFECT\x10\x02\x12 \n\x1cPRICE_TEST_REMAINS_IN_EFFECT\x10\x03*v\n\x0fSettlementTerms\x12\x1c\n\x18UNKNOWN_SETTLEMENT_TERMS\x10\x00\x12\x08\n\x04\x43\x41SH\x10\x01\x12\x0b\n\x07NON_NET\x10\x02\x12\x14\n\x10\x43ONTINGENT_TRADE\x10\x03\x12\x0e\n\nCASH_TODAY\x10\x04\x12\x08\n\x04\x44\x41TE\x10\x05*}\n\tCrossType\x12\x16\n\x12UNKNOWN_CROSS_TYPE\x10\x00\x12\x0b\n\x07\x44\x45\x46\x41ULT\x10\x01\x12\x0c\n\x08INTERNAL\x10\x02\x12\t\n\x05\x42\x41SIS\x10\x03\x12\x0e\n\nCONTINGENT\x10\x04\x12\x0b\n\x07SPECIAL\x10\x05\x12\x08\n\x04VWAP\x10\x06\x12\x0b\n\x07REGULAR\x10\x07*Q\n\x17OpenCloseSettlementFlag\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0e\n\nDAILY_OPEN\x10\x01\x12\x19\n\x15INDICATIVE_OPEN_PRICE\x10\x02*R\n\x10SettlementSource\x12\x1d\n\x19UNKNOWN_SETTLEMENT_SOURCE\x10\x00\x12\n\n\x06GLOBEX\x10\x01\x12\x07\n\x03ITC\x10\x02\x12\n\n\x06MANUAL\x10\x03*x\n\x07Service\x12\x13\n\x0fUNKNOWN_SERVICE\x10\x00\x12\r\n\tREAL_TIME\x10\x01\x12\x0b\n\x07\x44\x45LAYED\x10\x02\x12\x16\n\x12REAL_TIME_SNAPSHOT\x10\x03\x12\x14\n\x10\x44\x45LAYED_SNAPSHOT\x10\x04\x12\x0e\n\nEND_OF_DAY\x10\x05*y\n\x10MarketWideStatus\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x17\n\x13STATUS_START_OF_DAY\x10\x01\x12\x15\n\x11STATUS_END_OF_DAY\x10\x02\x12\x0f\n\x0bSTATUS_OPEN\x10\x03\x12\x10\n\x0cSTATUS_CLOSE\x10\x04*\xcc\x01\n\x15SnapshotRequestResult\x12#\n\x1fSNAPSHOT_REQUEST_UNKNOWN_RESULT\x10\x00\x12\x1c\n\x18SNAPSHOT_REQUEST_SUCCESS\x10\x01\x12\x1e\n\x1aSNAPSHOT_REQUEST_NOT_FOUND\x10\x02\x12*\n&SNAPSHOT_REQUEST_SERVICE_NOT_AVAILABLE\x10\x03\x12$\n SNAPSHOT_REQUEST_GENERIC_FAILURE\x10\x04*O\n\nActionType\x12\x12\n\x0eUNKNOWN_ACTION\x10\x00\x12\x0b\n\x07LISTING\x10\x01\x12\r\n\tDELISTING\x10\x02\x12\x11\n\rEXCHANGE_MOVE\x10\x03\x42\x07H\x01P\x01\xa0\x01\x01\x62\x06proto3'
+  serialized_pb=b'\n\x0eopenfeed.proto\x12\x0corg.openfeed\x1a\x19openfeed_instrument.proto\"\xbe\x05\n\x0fOpenfeedMessage\x12\x13\n\x0bsendingTime\x18\x01 \x01(\x12\x12\x12\n\ntotalCount\x18\x02 \x01(\x11\x12\x14\n\x0csyncSequence\x18\x03 \x01(\x03\x12&\n\x07\x63ontext\x18\x04 \x01(\x0b\x32\x15.org.openfeed.Context\x12\x32\n\x0c\x63hannelReset\x18\n \x01(\x0b\x32\x1a.org.openfeed.ChannelResetH\x00\x12,\n\theartBeat\x18\x0b \x01(\x0b\x32\x17.org.openfeed.HeartBeatH\x00\x12\x32\n\x0c\x61\x64minMessage\x18\x0c \x01(\x0b\x32\x1a.org.openfeed.AdminMessageH\x00\x12\x42\n\x14instrumentDefinition\x18\r \x01(\x0b\x32\".org.openfeed.InstrumentDefinitionH\x00\x12\x44\n\x15instrumentGroupStatus\x18\x0e \x01(\x0b\x32#.org.openfeed.InstrumentGroupStatusH\x00\x12\x36\n\x0emarketSnapshot\x18\x0f \x01(\x0b\x32\x1c.org.openfeed.MarketSnapshotH\x00\x12\x32\n\x0cmarketUpdate\x18\x10 \x01(\x0b\x32\x1a.org.openfeed.MarketUpdateH\x00\x12\x32\n\x0cmarketStatus\x18\x11 \x01(\x0b\x32\x1a.org.openfeed.MarketStatusH\x00\x12@\n\x13\x65odCommoditySummary\x18\x12 \x01(\x0b\x32!.org.openfeed.EODCommoditySummaryH\x00\x12:\n\x10instrumentAction\x18\x13 \x01(\x0b\x32\x1e.org.openfeed.InstrumentActionH\x00\x42\x06\n\x04\x64\x61ta\"8\n\x0c\x43hannelReset\x12\x0f\n\x07\x63hannel\x18\x01 \x01(\x11\x12\x17\n\x0ftransactionTime\x18\x02 \x01(\x12\"W\n\tHeartBeat\x12\x17\n\x0ftransactionTime\x18\x01 \x01(\x12\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x10\n\x08\x65xchange\x18\x03 \x01(\x08\x12\x0f\n\x07\x63hannel\x18\x04 \x01(\x11\"\xc3\x01\n\x0c\x41\x64minMessage\x12\x17\n\x0foriginationTime\x18\x01 \x01(\x12\x12\x0e\n\x06source\x18\x02 \x01(\t\x12\x14\n\x0clanguageCode\x18\x03 \x01(\t\x12\x10\n\x08headLine\x18\x04 \x01(\t\x12\x0c\n\x04text\x18\x05 \x01(\t\x12\x31\n\x06status\x18\x06 \x01(\x0e\x32!.org.openfeed.AdminMessage.Status\x12\x0f\n\x07\x63hannel\x18\x07 \x01(\x11\"\x10\n\x06Status\x12\x06\n\x02OK\x10\x00\"\xad\x01\n\x15InstrumentGroupStatus\x12\x17\n\x0ftransactionTime\x18\x01 \x01(\x12\x12\x19\n\x11instrumentGroupId\x18\x02 \x01(\t\x12<\n\rtradingStatus\x18\x03 \x01(\x0e\x32%.org.openfeed.InstrumentTradingStatus\x12\x11\n\ttradeDate\x18\x04 \x01(\x11\x12\x0f\n\x07\x63hannel\x18\x05 \x01(\x11\"r\n\x0cMarketStatus\x12\x17\n\x0ftransactionTime\x18\x01 \x01(\x12\x12\x0f\n\x07\x63hannel\x18\x02 \x01(\x11\x12\x38\n\x10marketWideStatus\x18\x03 \x01(\x0e\x32\x1e.org.openfeed.MarketWideStatus\"\x93\x01\n\x13\x45ODCommoditySummary\x12\x11\n\ttradeDate\x18\x01 \x01(\x11\x12\x14\n\x0c\x63ontractRoot\x18\x02 \x01(\t\x12\x1a\n\x12\x63onsolidatedVolume\x18\x03 \x01(\x12\x12 \n\x18\x63onsolidatedOpenInterest\x18\x04 \x01(\x12\x12\x15\n\rauxiliaryData\x18\x63 \x01(\x0c\"\xe3\x03\n\rMarketSession\x12\x11\n\ttradeDate\x18\x04 \x01(\x11\x12 \n\x04open\x18\x1e \x01(\x0b\x32\x12.org.openfeed.Open\x12 \n\x04high\x18\x1f \x01(\x0b\x32\x12.org.openfeed.High\x12\x1e\n\x03low\x18  \x01(\x0b\x32\x11.org.openfeed.Low\x12 \n\x04last\x18# \x01(\x0b\x32\x12.org.openfeed.Last\x12$\n\x06volume\x18& \x01(\x0b\x32\x14.org.openfeed.Volume\x12,\n\nsettlement\x18\' \x01(\x0b\x32\x18.org.openfeed.Settlement\x12\x30\n\x0eprevSettlement\x18, \x01(\x0b\x32\x18.org.openfeed.Settlement\x12\x30\n\x0copenInterest\x18( \x01(\x0b\x32\x1a.org.openfeed.OpenInterest\x12\x34\n\x0enumberOfTrades\x18) \x01(\x0b\x32\x1c.org.openfeed.NumberOfTrades\x12\x32\n\rmonetaryValue\x18* \x01(\x0b\x32\x1b.org.openfeed.MonetaryValue\x12\x17\n\x0ftransactionTime\x18+ \x01(\x12\"\xcf\x0c\n\x0eMarketSnapshot\x12\x10\n\x08marketId\x18\x01 \x01(\x12\x12\x17\n\x0ftransactionTime\x18\x02 \x01(\x12\x12\x16\n\x0emarketSequence\x18\x03 \x01(\x03\x12\x11\n\ttradeDate\x18\x04 \x01(\x11\x12\x13\n\x0btotalChunks\x18\x05 \x01(\x11\x12\x14\n\x0c\x63urrentChunk\x18\x06 \x01(\x11\x12\x0e\n\x06symbol\x18\x07 \x01(\t\x12\x18\n\x10priceDenominator\x18\x08 \x01(\x11\x12&\n\x07service\x18\t \x01(\x0e\x32\x15.org.openfeed.Service\x12\x38\n\x10instrumentStatus\x18\n \x01(\x0b\x32\x1e.org.openfeed.InstrumentStatus\x12\'\n\x03\x62\x62o\x18\x0b \x01(\x0b\x32\x1a.org.openfeed.BestBidOffer\x12\'\n\x05index\x18\x0c \x01(\x0b\x32\x18.org.openfeed.IndexValue\x12\x30\n\x0bpriceLevels\x18\r \x03(\x0b\x32\x1b.org.openfeed.AddPriceLevel\x12&\n\x06orders\x18\x0e \x03(\x0b\x32\x16.org.openfeed.AddOrder\x12 \n\x04news\x18\x0f \x01(\x0b\x32\x12.org.openfeed.News\x12 \n\x04open\x18\x1e \x01(\x0b\x32\x12.org.openfeed.Open\x12 \n\x04high\x18\x1f \x01(\x0b\x32\x12.org.openfeed.High\x12\x1e\n\x03low\x18  \x01(\x0b\x32\x11.org.openfeed.Low\x12\"\n\x05\x63lose\x18! \x01(\x0b\x32\x13.org.openfeed.Close\x12*\n\tprevClose\x18\" \x01(\x0b\x32\x17.org.openfeed.PrevClose\x12 \n\x04last\x18# \x01(\x0b\x32\x12.org.openfeed.Last\x12(\n\x08yearHigh\x18$ \x01(\x0b\x32\x16.org.openfeed.YearHigh\x12&\n\x07yearLow\x18% \x01(\x0b\x32\x15.org.openfeed.YearLow\x12$\n\x06volume\x18& \x01(\x0b\x32\x14.org.openfeed.Volume\x12,\n\nsettlement\x18\' \x01(\x0b\x32\x18.org.openfeed.Settlement\x12\x30\n\x0copenInterest\x18( \x01(\x0b\x32\x1a.org.openfeed.OpenInterest\x12 \n\x04vwap\x18) \x01(\x0b\x32\x12.org.openfeed.Vwap\x12P\n\x1c\x64ividendsIncomeDistributions\x18* \x01(\x0b\x32*.org.openfeed.DividendsIncomeDistributions\x12\x34\n\x0enumberOfTrades\x18+ \x01(\x0b\x32\x1c.org.openfeed.NumberOfTrades\x12\x32\n\rmonetaryValue\x18, \x01(\x0b\x32\x1b.org.openfeed.MonetaryValue\x12@\n\x14\x63\x61pitalDistributions\x18- \x01(\x0b\x32\".org.openfeed.CapitalDistributions\x12:\n\x11sharesOutstanding\x18. \x01(\x0b\x32\x1f.org.openfeed.SharesOutstanding\x12\x32\n\rnetAssetValue\x18/ \x01(\x0b\x32\x1b.org.openfeed.NetAssetValue\x12\x34\n\x0fpreviousSession\x18\x30 \x01(\x0b\x32\x1b.org.openfeed.MarketSession\x12-\n\x08tSession\x18\x31 \x01(\x0b\x32\x1b.org.openfeed.MarketSession\x12\x32\n\rvolumeAtPrice\x18\x32 \x01(\x0b\x32\x1b.org.openfeed.VolumeAtPrice\x12.\n\x0bhighRolling\x18\x33 \x01(\x0b\x32\x19.org.openfeed.HighRolling\x12,\n\nlowRolling\x18\x34 \x01(\x0b\x32\x18.org.openfeed.LowRolling\x12-\n\x08zSession\x18\x35 \x01(\x0b\x32\x1b.org.openfeed.MarketSession\"\x94\x01\n\x16MarketSnapshotResponse\x12\x33\n\x06result\x18\x01 \x01(\x0e\x32#.org.openfeed.SnapshotRequestResult\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x34\n\x0emarketSnapshot\x18\x03 \x01(\x0b\x32\x1c.org.openfeed.MarketSnapshot\"\xbd\x0e\n\x0cMarketUpdate\x12\x10\n\x08marketId\x18\x01 \x01(\x12\x12\x0e\n\x06symbol\x18\x02 \x01(\t\x12\x17\n\x0ftransactionTime\x18\x03 \x01(\x12\x12\x18\n\x10\x64istributionTime\x18\x04 \x01(\x12\x12\x16\n\x0emarketSequence\x18\x05 \x01(\x12\x12\x16\n\x0esourceSequence\x18\x06 \x01(\x12\x12\x14\n\x0coriginatorId\x18\x07 \x01(\x0c\x12\x18\n\x10priceDenominator\x18\t \x01(\x11\x12&\n\x07\x63ontext\x18\n \x01(\x0b\x32\x15.org.openfeed.Context\x12,\n\x07session\x18\x0b \x01(\x0b\x32\x1b.org.openfeed.MarketSession\x12-\n\x08tSession\x18\x0c \x01(\x0b\x32\x1b.org.openfeed.MarketSession\x12\x34\n\x0fpreviousSession\x18\r \x01(\x0b\x32\x1b.org.openfeed.MarketSession\x12\x10\n\x08regional\x18\x0e \x01(\x08\x12-\n\x08zSession\x18\x0f \x01(\x0b\x32\x1b.org.openfeed.MarketSession\x12\"\n\x04news\x18\x14 \x01(\x0b\x32\x12.org.openfeed.NewsH\x00\x12,\n\tclearBook\x18\x15 \x01(\x0b\x32\x17.org.openfeed.ClearBookH\x00\x12:\n\x10instrumentStatus\x18\x16 \x01(\x0b\x32\x1e.org.openfeed.InstrumentStatusH\x00\x12)\n\x03\x62\x62o\x18\x17 \x01(\x0b\x32\x1a.org.openfeed.BestBidOfferH\x00\x12\x38\n\x0f\x64\x65pthPriceLevel\x18\x18 \x01(\x0b\x32\x1d.org.openfeed.DepthPriceLevelH\x00\x12.\n\ndepthOrder\x18\x19 \x01(\x0b\x32\x18.org.openfeed.DepthOrderH\x00\x12)\n\x05index\x18\x1a \x01(\x0b\x32\x18.org.openfeed.IndexValueH\x00\x12&\n\x06trades\x18\x1b \x01(\x0b\x32\x14.org.openfeed.TradesH\x00\x12\"\n\x04open\x18\x1c \x01(\x0b\x32\x12.org.openfeed.OpenH\x00\x12\"\n\x04high\x18\x1d \x01(\x0b\x32\x12.org.openfeed.HighH\x00\x12 \n\x03low\x18\x1e \x01(\x0b\x32\x11.org.openfeed.LowH\x00\x12$\n\x05\x63lose\x18\x1f \x01(\x0b\x32\x13.org.openfeed.CloseH\x00\x12,\n\tprevClose\x18  \x01(\x0b\x32\x17.org.openfeed.PrevCloseH\x00\x12\"\n\x04last\x18! \x01(\x0b\x32\x12.org.openfeed.LastH\x00\x12*\n\x08yearHigh\x18\" \x01(\x0b\x32\x16.org.openfeed.YearHighH\x00\x12(\n\x07yearLow\x18# \x01(\x0b\x32\x15.org.openfeed.YearLowH\x00\x12&\n\x06volume\x18$ \x01(\x0b\x32\x14.org.openfeed.VolumeH\x00\x12.\n\nsettlement\x18% \x01(\x0b\x32\x18.org.openfeed.SettlementH\x00\x12\x32\n\x0copenInterest\x18& \x01(\x0b\x32\x1a.org.openfeed.OpenInterestH\x00\x12\"\n\x04vwap\x18\' \x01(\x0b\x32\x12.org.openfeed.VwapH\x00\x12R\n\x1c\x64ividendsIncomeDistributions\x18( \x01(\x0b\x32*.org.openfeed.DividendsIncomeDistributionsH\x00\x12\x36\n\x0enumberOfTrades\x18) \x01(\x0b\x32\x1c.org.openfeed.NumberOfTradesH\x00\x12\x34\n\rmonetaryValue\x18* \x01(\x0b\x32\x1b.org.openfeed.MonetaryValueH\x00\x12\x42\n\x14\x63\x61pitalDistributions\x18+ \x01(\x0b\x32\".org.openfeed.CapitalDistributionsH\x00\x12<\n\x11sharesOutstanding\x18, \x01(\x0b\x32\x1f.org.openfeed.SharesOutstandingH\x00\x12\x34\n\rnetAssetValue\x18- \x01(\x0b\x32\x1b.org.openfeed.NetAssetValueH\x00\x12\x34\n\rmarketSummary\x18. \x01(\x0b\x32\x1b.org.openfeed.MarketSummaryH\x00\x12\x30\n\x0bhighRolling\x18/ \x01(\x0b\x32\x19.org.openfeed.HighRollingH\x00\x12.\n\nlowRolling\x18\x30 \x01(\x0b\x32\x18.org.openfeed.LowRollingH\x00\x42\x06\n\x04\x64\x61taJ\x04\x08\x08\x10\t\"\x86\x02\n\x0f\x44\x65pthPriceLevel\x12\x33\n\x06levels\x18\x01 \x03(\x0b\x32#.org.openfeed.DepthPriceLevel.Entry\x1a\xbd\x01\n\x05\x45ntry\x12\x34\n\raddPriceLevel\x18\x01 \x01(\x0b\x32\x1b.org.openfeed.AddPriceLevelH\x00\x12:\n\x10\x64\x65letePriceLevel\x18\x02 \x01(\x0b\x32\x1e.org.openfeed.DeletePriceLevelH\x00\x12:\n\x10modifyPriceLevel\x18\x03 \x01(\x0b\x32\x1e.org.openfeed.ModifyPriceLevelH\x00\x42\x06\n\x04\x64\x61ta\"\xde\x01\n\nDepthOrder\x12.\n\x06orders\x18\x01 \x03(\x0b\x32\x1e.org.openfeed.DepthOrder.Entry\x1a\x9f\x01\n\x05\x45ntry\x12*\n\x08\x61\x64\x64Order\x18\x01 \x01(\x0b\x32\x16.org.openfeed.AddOrderH\x00\x12\x30\n\x0b\x64\x65leteOrder\x18\x02 \x01(\x0b\x32\x19.org.openfeed.DeleteOrderH\x00\x12\x30\n\x0bmodifyOrder\x18\x03 \x01(\x0b\x32\x19.org.openfeed.ModifyOrderH\x00\x42\x06\n\x04\x64\x61ta\"v\n\x04News\x12\x17\n\x0foriginationTime\x18\x01 \x01(\x12\x12\x0e\n\x06source\x18\x02 \x01(\t\x12\x14\n\x0clanguageCode\x18\x03 \x01(\t\x12\x10\n\x08headLine\x18\x04 \x01(\t\x12\x0c\n\x04text\x18\x05 \x01(\t\x12\x0f\n\x07symbols\x18\x06 \x03(\t\"6\n\tClearBook\x12\x10\n\x08reserved\x18\x01 \x01(\x11\x12\x17\n\x0ftransactionTime\x18\x02 \x01(\x12\"\xf7\x01\n\x10InstrumentStatus\x12\x17\n\x0ftransactionTime\x18\t \x01(\x12\x12<\n\rtradingStatus\x18\n \x01(\x0e\x32%.org.openfeed.InstrumentTradingStatus\x12\x13\n\x0bopeningTime\x18\x0b \x01(\x12\x12\x0c\n\x04note\x18\x0c \x01(\t\x12\x11\n\ttradeDate\x18\r \x01(\x11\x12V\n\x1fregulationSHOShortSalePriceTest\x18\x0e \x01(\x0e\x32-.org.openfeed.RegulationSHOShortSalePriceTest\"\xd4\x02\n\x0c\x42\x65stBidOffer\x12\x17\n\x0ftransactionTime\x18\t \x01(\x12\x12\x10\n\x08\x62idPrice\x18\n \x01(\x12\x12\x13\n\x0b\x62idQuantity\x18\x0b \x01(\x12\x12\x15\n\rbidOrderCount\x18\x0c \x01(\x11\x12\x15\n\rbidOriginator\x18\r \x01(\x0c\x12\x19\n\x11\x62idQuoteCondition\x18\x0e \x01(\x0c\x12\x12\n\nofferPrice\x18\x14 \x01(\x12\x12\x15\n\rofferQuantity\x18\x15 \x01(\x12\x12\x17\n\x0fofferOrderCount\x18\x16 \x01(\x11\x12\x17\n\x0fofferOriginator\x18\x17 \x01(\x0c\x12\x1b\n\x13offerQuoteCondition\x18\x18 \x01(\x0c\x12\x16\n\x0equoteCondition\x18\x1e \x01(\x0c\x12\x10\n\x08regional\x18  \x01(\x08\x12\x11\n\ttransient\x18! \x01(\x08J\x04\x08\x1f\x10 \"\xab\x01\n\rAddPriceLevel\x12\x17\n\x0ftransactionTime\x18\t \x01(\x12\x12\r\n\x05level\x18\n \x01(\x11\x12$\n\x04side\x18\x0b \x01(\x0e\x32\x16.org.openfeed.BookSide\x12\r\n\x05price\x18\x0c \x01(\x12\x12\x10\n\x08quantity\x18\r \x01(\x12\x12\x12\n\norderCount\x18\x0e \x01(\x11\x12\x17\n\x0fimpliedQuantity\x18\x0f \x01(\x12\"`\n\x10\x44\x65letePriceLevel\x12\x17\n\x0ftransactionTime\x18\t \x01(\x12\x12\r\n\x05level\x18\n \x01(\x11\x12$\n\x04side\x18\x0b \x01(\x0e\x32\x16.org.openfeed.BookSide\"\xae\x01\n\x10ModifyPriceLevel\x12\x17\n\x0ftransactionTime\x18\t \x01(\x12\x12\r\n\x05level\x18\n \x01(\x11\x12$\n\x04side\x18\x0b \x01(\x0e\x32\x16.org.openfeed.BookSide\x12\r\n\x05price\x18\x0c \x01(\x12\x12\x10\n\x08quantity\x18\r \x01(\x12\x12\x12\n\norderCount\x18\x0e \x01(\x11\x12\x17\n\x0fimpliedQuantity\x18\x0f \x01(\x12\"\xa0\x01\n\x08\x41\x64\x64Order\x12\x17\n\x0ftransactionTime\x18\t \x01(\x12\x12\x0f\n\x07orderId\x18\n \x01(\x12\x12$\n\x04side\x18\x0b \x01(\x0e\x32\x16.org.openfeed.BookSide\x12\r\n\x05price\x18\x0c \x01(\x12\x12\x10\n\x08quantity\x18\r \x01(\x12\x12\x11\n\tisImplied\x18\x0e \x01(\x08\x12\x10\n\x08priority\x18\x0f \x01(\x12\"]\n\x0b\x44\x65leteOrder\x12\x17\n\x0ftransactionTime\x18\t \x01(\x12\x12\x0f\n\x07orderId\x18\n \x01(\x12\x12$\n\x04side\x18\x0b \x01(\x0e\x32\x16.org.openfeed.BookSide\"\xa3\x01\n\x0bModifyOrder\x12\x17\n\x0ftransactionTime\x18\t \x01(\x12\x12\x0f\n\x07orderId\x18\n \x01(\x12\x12$\n\x04side\x18\x0b \x01(\x0e\x32\x16.org.openfeed.BookSide\x12\r\n\x05price\x18\x0c \x01(\x12\x12\x10\n\x08quantity\x18\r \x01(\x12\x12\x11\n\tisImplied\x18\x0e \x01(\x08\x12\x10\n\x08priority\x18\x0f \x01(\x12\"\xd7\x01\n\nIndexValue\x12\x17\n\x0ftransactionTime\x18\t \x01(\x12\x12\x11\n\ttradeDate\x18\n \x01(\x11\x12\x0c\n\x04last\x18\x0b \x01(\x12\x12\x0e\n\x06volume\x18\x0c \x01(\x12\x12\x0c\n\x04open\x18\r \x01(\x12\x12\x16\n\x0esettlementOpen\x18\x0e \x01(\x12\x12\x13\n\x0bspecialOpen\x18\x0f \x01(\x12\x12\x0c\n\x04high\x18\x10 \x01(\x12\x12\x0b\n\x03low\x18\x11 \x01(\x12\x12\r\n\x05\x63lose\x18\x12 \x01(\x12\x12\x0b\n\x03\x62id\x18\x13 \x01(\x12\x12\r\n\x05offer\x18\x14 \x01(\x12\"\xd8\x01\n\x06Trades\x12*\n\x06trades\x18\x01 \x03(\x0b\x32\x1a.org.openfeed.Trades.Entry\x1a\xa1\x01\n\x05\x45ntry\x12$\n\x05trade\x18\x01 \x01(\x0b\x32\x13.org.openfeed.TradeH\x00\x12\x38\n\x0ftradeCorrection\x18\x02 \x01(\x0b\x32\x1d.org.openfeed.TradeCorrectionH\x00\x12\x30\n\x0btradeCancel\x18\x03 \x01(\x0b\x32\x19.org.openfeed.TradeCancelH\x00\x42\x06\n\x04\x64\x61ta\"\xa7\x05\n\x05Trade\x12\x14\n\x0coriginatorId\x18\x08 \x01(\x0c\x12\x17\n\x0ftransactionTime\x18\t \x01(\x12\x12\r\n\x05price\x18\n \x01(\x12\x12\x10\n\x08quantity\x18\x0b \x01(\x12\x12\x0f\n\x07tradeId\x18\x0c \x01(\x0c\x12$\n\x04side\x18\r \x01(\x0e\x32\x16.org.openfeed.BookSide\x12\x11\n\ttradeDate\x18\x0e \x01(\x11\x12\x0f\n\x07\x62uyerId\x18\x0f \x01(\x0c\x12\x10\n\x08sellerId\x18\x10 \x01(\x0c\x12\x14\n\x0copeningTrade\x18\x11 \x01(\x08\x12\x14\n\x0csystemPriced\x18\x12 \x01(\x08\x12\x15\n\rmarketOnClose\x18\x13 \x01(\x08\x12\x0e\n\x06oddLot\x18\x14 \x01(\x08\x12\x36\n\x0fsettlementTerms\x18\x15 \x01(\x0e\x32\x1d.org.openfeed.SettlementTerms\x12*\n\tcrossType\x18\x16 \x01(\x0e\x32\x17.org.openfeed.CrossType\x12\x0e\n\x06\x62yPass\x18\x17 \x01(\x08\x12\x11\n\tlastPrice\x18\x18 \x01(\x12\x12\x15\n\rsaleCondition\x18\x19 \x01(\x0c\x12\x10\n\x08\x63urrency\x18\x1a \x01(\t\x12\x19\n\x11\x64oesNotUpdateLast\x18\x1b \x01(\x08\x12\x1b\n\x13\x64oesNotUpdateVolume\x18\x1c \x01(\x08\x12\x0f\n\x07session\x18\x1e \x01(\t\x12\x12\n\nblockTrade\x18\x1f \x01(\x08\x12\x18\n\x10\x64istributionTime\x18  \x01(\x12\x12\x18\n\x10transactionTime2\x18! \x01(\x12\x12\"\n\x1a\x63onsolidatedPriceIndicator\x18\" \x01(\t\x12\x11\n\ttransient\x18# \x01(\x08\x12\x16\n\x0eindexShortName\x18$ \x01(\t\"\xc6\x04\n\x0fTradeCorrection\x12\x14\n\x0coriginatorId\x18\x08 \x01(\x0c\x12\x17\n\x0ftransactionTime\x18\t \x01(\x12\x12\r\n\x05price\x18\n \x01(\x12\x12\x10\n\x08quantity\x18\x0b \x01(\x12\x12\x0f\n\x07tradeId\x18\x0c \x01(\x0c\x12$\n\x04side\x18\r \x01(\x0e\x32\x16.org.openfeed.BookSide\x12\x11\n\ttradeDate\x18\x0e \x01(\x11\x12\x0f\n\x07\x62uyerId\x18\x0f \x01(\x0c\x12\x10\n\x08sellerId\x18\x10 \x01(\x0c\x12\x14\n\x0copeningTrade\x18\x11 \x01(\x08\x12\x14\n\x0csystemPriced\x18\x12 \x01(\x08\x12\x15\n\rmarketOnClose\x18\x13 \x01(\x08\x12\x0e\n\x06oddLot\x18\x14 \x01(\x08\x12\x36\n\x0fsettlementTerms\x18\x15 \x01(\x0e\x32\x1d.org.openfeed.SettlementTerms\x12*\n\tcrossType\x18\x16 \x01(\x0e\x32\x17.org.openfeed.CrossType\x12\x0e\n\x06\x62yPass\x18\x17 \x01(\x08\x12\x17\n\x0foriginalTradeId\x18\x18 \x01(\x0c\x12\x15\n\rsaleCondition\x18\x19 \x01(\x0c\x12\x10\n\x08\x63urrency\x18\x1a \x01(\t\x12\x18\n\x10\x64istributionTime\x18\x1b \x01(\x12\x12\x18\n\x10transactionTime2\x18\x1c \x01(\x12\x12\x1a\n\x12originalTradePrice\x18\x1d \x01(\x12\x12\x1d\n\x15originalTradeQuantity\x18\x1e \x01(\x12\"\xe7\x01\n\x0bTradeCancel\x12\x14\n\x0coriginatorId\x18\x08 \x01(\x0c\x12\x17\n\x0ftransactionTime\x18\t \x01(\x12\x12\x1b\n\x13\x63orrectedTradePrice\x18\n \x01(\x12\x12\x1e\n\x16\x63orrectedTradeQuantity\x18\x0b \x01(\x12\x12\x0f\n\x07tradeId\x18\x0c \x01(\x0c\x12\x15\n\rsaleCondition\x18\r \x01(\x0c\x12\x10\n\x08\x63urrency\x18\x0e \x01(\t\x12\x18\n\x10\x64istributionTime\x18\x0f \x01(\x12\x12\x18\n\x10transactionTime2\x18\x10 \x01(\x12\"\x9b\x01\n\x04Open\x12\x17\n\x0ftransactionTime\x18\t \x01(\x12\x12\x11\n\ttradeDate\x18\n \x01(\x11\x12\r\n\x05price\x18\x0b \x01(\x12\x12\x46\n\x17OpenCloseSettlementFlag\x18\x0c \x01(\x0e\x32%.org.openfeed.OpenCloseSettlementFlag\x12\x10\n\x08\x63urrency\x18\r \x01(\t\"S\n\x04High\x12\x17\n\x0ftransactionTime\x18\t \x01(\x12\x12\x11\n\ttradeDate\x18\n \x01(\x11\x12\r\n\x05price\x18\x0b \x01(\x12\x12\x10\n\x08\x63urrency\x18\x0c \x01(\t\"Z\n\x0bHighRolling\x12\x17\n\x0ftransactionTime\x18\t \x01(\x12\x12\x11\n\ttradeDate\x18\n \x01(\x11\x12\r\n\x05price\x18\x0b \x01(\x12\x12\x10\n\x08\x63urrency\x18\x0c \x01(\t\"R\n\x03Low\x12\x17\n\x0ftransactionTime\x18\t \x01(\x12\x12\x11\n\ttradeDate\x18\n \x01(\x11\x12\r\n\x05price\x18\x0b \x01(\x12\x12\x10\n\x08\x63urrency\x18\x0c \x01(\t\"Y\n\nLowRolling\x12\x17\n\x0ftransactionTime\x18\t \x01(\x12\x12\x11\n\ttradeDate\x18\n \x01(\x11\x12\r\n\x05price\x18\x0b \x01(\x12\x12\x10\n\x08\x63urrency\x18\x0c \x01(\t\"T\n\x05\x43lose\x12\x17\n\x0ftransactionTime\x18\t \x01(\x12\x12\x11\n\ttradeDate\x18\n \x01(\x11\x12\r\n\x05price\x18\x0b \x01(\x12\x12\x10\n\x08\x63urrency\x18\x0c \x01(\t\"X\n\tPrevClose\x12\x17\n\x0ftransactionTime\x18\t \x01(\x12\x12\x11\n\ttradeDate\x18\n \x01(\x11\x12\r\n\x05price\x18\x0b \x01(\x12\x12\x10\n\x08\x63urrency\x18\x0c \x01(\t\"v\n\x04Last\x12\x17\n\x0ftransactionTime\x18\t \x01(\x12\x12\x11\n\ttradeDate\x18\n \x01(\x11\x12\r\n\x05price\x18\x0b \x01(\x12\x12\x10\n\x08quantity\x18\x0c \x01(\x12\x12\x10\n\x08\x63urrency\x18\r \x01(\t\x12\x0f\n\x07session\x18\x1e \x01(\t\"D\n\x08YearHigh\x12\x17\n\x0ftransactionTime\x18\t \x01(\x12\x12\r\n\x05price\x18\n \x01(\x12\x12\x10\n\x08\x63urrency\x18\x0b \x01(\t\"C\n\x07YearLow\x12\x17\n\x0ftransactionTime\x18\t \x01(\x12\x12\r\n\x05price\x18\n \x01(\x12\x12\x10\n\x08\x63urrency\x18\x0b \x01(\t\"D\n\x06Volume\x12\x17\n\x0ftransactionTime\x18\t \x01(\x12\x12\x11\n\ttradeDate\x18\n \x01(\x11\x12\x0e\n\x06volume\x18\x0b \x01(\x12\"R\n\x0eNumberOfTrades\x12\x17\n\x0ftransactionTime\x18\t \x01(\x12\x12\x11\n\ttradeDate\x18\n \x01(\x11\x12\x14\n\x0cnumberTrades\x18\x0b \x01(\x12\"e\n\rMonetaryValue\x12\x17\n\x0ftransactionTime\x18\t \x01(\x12\x12\x11\n\ttradeDate\x18\n \x01(\x11\x12\r\n\x05value\x18\x0b \x01(\x12\x12\x19\n\x11valueCurrencyCode\x18\x0c \x01(\t\"\xe4\x01\n\nSettlement\x12\x17\n\x0ftransactionTime\x18\t \x01(\x12\x12\x11\n\ttradeDate\x18\n \x01(\x11\x12\r\n\x05price\x18\x0b \x01(\x12\x12\x19\n\x11preliminarySettle\x18\x0c \x01(\x08\x12\x10\n\x08\x63urrency\x18\r \x01(\t\x12\x38\n\x10settlementSource\x18\x0e \x01(\x0e\x32\x1e.org.openfeed.SettlementSource\x12\x0f\n\x07session\x18\x0f \x01(\t\x12\x11\n\ttransient\x18\x10 \x01(\x08\x12\x10\n\x08reserved\x18\x7f \x01(\x08\"J\n\x0cOpenInterest\x12\x17\n\x0ftransactionTime\x18\t \x01(\x12\x12\x11\n\ttradeDate\x18\n \x01(\x11\x12\x0e\n\x06volume\x18\x0b \x01(\x12\"@\n\x04Vwap\x12\x17\n\x0ftransactionTime\x18\t \x01(\x12\x12\x11\n\ttradeDate\x18\n \x01(\x11\x12\x0c\n\x04vwap\x18\x0b \x01(\x12\"\xf8\x03\n\x1c\x44ividendsIncomeDistributions\x12\x17\n\x0ftransactionTime\x18\x06 \x01(\x12\x12\x16\n\x0einstrumentType\x18\x07 \x01(\t\x12\x17\n\x0f\x63orporateAction\x18\x08 \x01(\t\x12\x18\n\x10\x64istributionType\x18\t \x01(\t\x12\x13\n\x0bpayableDate\x18\n \x01(\x11\x12\x12\n\nrecordDate\x18\x0b \x01(\x11\x12\x16\n\x0e\x65xDividendDate\x18\x0c \x01(\x11\x12\x0e\n\x06\x61mount\x18\r \x01(\x12\x12\x14\n\x0c\x63urrencyCode\x18\x0e \x01(\t\x12\r\n\x05notes\x18\x0f \x03(\t\x12\x1d\n\x15totalCashDistribution\x18\x10 \x01(\x12\x12$\n\x1cnonQualifiedCashDistribution\x18\x11 \x01(\x12\x12!\n\x19qualifiedCashDistribution\x18\x12 \x01(\x12\x12\x1f\n\x17taxFreeCashDistribution\x18\x13 \x01(\x12\x12 \n\x18ordinaryForeignTaxCredit\x18\x14 \x01(\x12\x12!\n\x19qualifiedForeignTaxCredit\x18\x15 \x01(\x12\x12\x1a\n\x12stockDividendRatio\x18\x16 \x01(\x12\x12\x14\n\x0creinvestDate\x18\x17 \x01(\x11\"\xca\x02\n\x14\x43\x61pitalDistributions\x12\x17\n\x0ftransactionTime\x18\x08 \x01(\x12\x12\x16\n\x0einstrumentType\x18\t \x01(\t\x12\x17\n\x0f\x63orporateAction\x18\n \x01(\t\x12\x13\n\x0bpayableDate\x18\x0b \x01(\x11\x12\x12\n\nrecordDate\x18\x0c \x01(\x11\x12\x0e\n\x06\x65xDate\x18\r \x01(\x11\x12\x1c\n\x14shortTermCapitalGain\x18\x0e \x01(\x12\x12\x1b\n\x13longTermCapitalGain\x18\x0f \x01(\x12\x12 \n\x18unallocatedDistributions\x18\x10 \x01(\x12\x12\x17\n\x0freturnOfCapital\x18\x11 \x01(\x12\x12\x14\n\x0c\x63urrencyCode\x18\x12 \x01(\t\x12\r\n\x05notes\x18\x13 \x03(\t\x12\x14\n\x0creinvestDate\x18\x14 \x01(\x11\"G\n\x11SharesOutstanding\x12\x19\n\x11sharesOutstanding\x18\x01 \x01(\x12\x12\x17\n\x0ftransactionTime\x18\x02 \x01(\x12\"?\n\rNetAssetValue\x12\x15\n\rnetAssetValue\x18\x01 \x01(\x12\x12\x17\n\x0ftransactionTime\x18\x02 \x01(\x12\"\xc7\x07\n\rMarketSummary\x12\x17\n\x0ftransactionTime\x18\x01 \x01(\x12\x12\x13\n\x0btradingDate\x18\x02 \x01(\x11\x12\x12\n\nstartOfDay\x18\x03 \x01(\x08\x12\x10\n\x08\x65ndOfDay\x18\x04 \x01(\x08\x12\x33\n\x05\x63lear\x18\x05 \x01(\x0e\x32$.org.openfeed.MarketSummary.ClearSet\x12\x38\n\x10instrumentStatus\x18\t \x01(\x0b\x32\x1e.org.openfeed.InstrumentStatus\x12\'\n\x03\x62\x62o\x18\n \x01(\x0b\x32\x1a.org.openfeed.BestBidOffer\x12 \n\x04open\x18\x0b \x01(\x0b\x32\x12.org.openfeed.Open\x12 \n\x04high\x18\x0c \x01(\x0b\x32\x12.org.openfeed.High\x12\x1e\n\x03low\x18\r \x01(\x0b\x32\x11.org.openfeed.Low\x12\"\n\x05\x63lose\x18\x0e \x01(\x0b\x32\x13.org.openfeed.Close\x12*\n\tprevClose\x18\x0f \x01(\x0b\x32\x17.org.openfeed.PrevClose\x12 \n\x04last\x18\x10 \x01(\x0b\x32\x12.org.openfeed.Last\x12$\n\x06volume\x18\x11 \x01(\x0b\x32\x14.org.openfeed.Volume\x12,\n\nsettlement\x18\x12 \x01(\x0b\x32\x18.org.openfeed.Settlement\x12\x30\n\x0copenInterest\x18\x13 \x01(\x0b\x32\x1a.org.openfeed.OpenInterest\x12 \n\x04vwap\x18\x14 \x01(\x0b\x32\x12.org.openfeed.Vwap\x12\x0f\n\x07session\x18\x15 \x01(\t\x12<\n\x0bsummaryType\x18\x16 \x01(\x0e\x32\'.org.openfeed.MarketSummary.SummaryType\x12(\n\nprevVolume\x18\x17 \x01(\x0b\x32\x14.org.openfeed.Volume\x12\x11\n\ttransient\x18\x18 \x01(\x08\"3\n\x08\x43learSet\x12\x08\n\x04NONE\x10\x00\x12\x07\n\x03\x41LL\x10\x01\x12\x06\n\x02\x42\x41\x10\x02\x12\x0c\n\x08\x43USTOM_1\x10\x03\"\x8a\x01\n\x0bSummaryType\x12\x14\n\x10\x45XCHANGE_REFRESH\x10\x00\x12\x16\n\x12REFRESH_LIVE_PRICE\x10\x01\x12\x18\n\x14\x45OD_COMMODITY_PRICES\x10\x02\x12\x1a\n\x16\x45OD_STOCK_FOREX_PRICES\x10\x03\x12\x17\n\x13\x45OD_COMMODITY_STATS\x10\x04\"a\n\x07\x43ontext\x12\'\n\x04\x64\x61ta\x18\x01 \x03(\x0b\x32\x19.org.openfeed.ContextData\x12-\n\x0btracePoints\x18\x02 \x03(\x0b\x32\x18.org.openfeed.TracePoint\"\xa2\x01\n\x0b\x43ontextData\x12\n\n\x02id\x18\x01 \x01(\t\x12\x11\n\x07vstring\x18\x05 \x01(\tH\x00\x12\x10\n\x06vbytes\x18\x06 \x01(\x0cH\x00\x12\x0f\n\x05vbool\x18\x07 \x01(\x08H\x00\x12\x11\n\x07vsint32\x18\x08 \x01(\x11H\x00\x12\x11\n\x07vsint64\x18\t \x01(\x12H\x00\x12\x10\n\x06vfloat\x18\n \x01(\x02H\x00\x12\x11\n\x07vdouble\x18\x0b \x01(\x01H\x00\x42\x06\n\x04\x64\x61ta\"^\n\nTracePoint\x12\n\n\x02id\x18\x01 \x01(\t\x12\x13\n\x0b\x63omponentId\x18\x02 \x01(\t\x12\x13\n\x0btimestampNs\x18\x03 \x01(\x12\x12\x1a\n\x12\x63omponentLatencyNs\x18\x04 \x01(\x05\"v\n\x1aTCPHistoricalReplayRequest\x12\x0f\n\x07\x63hannel\x18\x01 \x01(\x05\x12\x13\n\x0bresetNumber\x18\x02 \x01(\x05\x12\x10\n\x08sequence\x18\x03 \x01(\x03\x12\r\n\x05\x63ount\x18\x04 \x01(\x05\x12\x11\n\trequestId\x18\x05 \x01(\t\"\xe6\x01\n\x0fSnapshotRequest\x12\x0f\n\x07\x63hannel\x18\x01 \x01(\x05\x12\x13\n\x0bresetNumber\x18\x02 \x01(\x05\x12\x11\n\trequestId\x18\x03 \x01(\t\x12O\n\x14snapshotRequestTypes\x18\x04 \x03(\x0e\x32\x31.org.openfeed.SnapshotRequest.SnapshotRequestType\"I\n\x13SnapshotRequestType\x12\x07\n\x03\x41LL\x10\x00\x12\t\n\x05QUOTE\x10\x01\x12\t\n\x05\x44\x45PTH\x10\x02\x12\x13\n\x0fVOLUME_AT_PRICE\x10\x03\"\x9b\x02\n\rVolumeAtPrice\x12\x10\n\x08marketId\x18\x01 \x01(\x12\x12\x0e\n\x06symbol\x18\x02 \x01(\t\x12\x17\n\x0ftransactionTime\x18\x03 \x01(\x12\x12\x11\n\tlastPrice\x18\x04 \x01(\x12\x12\x14\n\x0clastQuantity\x18\x05 \x01(\x12\x12\x1c\n\x14lastCumulativeVolume\x18\x06 \x01(\x12\x12\x11\n\ttradeDate\x18\x07 \x01(\x11\x12\x42\n\x0cpriceVolumes\x18\x08 \x03(\x0b\x32,.org.openfeed.VolumeAtPrice.PriceLevelVolume\x1a\x31\n\x10PriceLevelVolume\x12\r\n\x05price\x18\x01 \x01(\x12\x12\x0e\n\x06volume\x18\x02 \x01(\x12\"\xd6\x02\n\x04Ohlc\x12\x10\n\x08marketId\x18\x01 \x01(\x12\x12\x0e\n\x06symbol\x18\x02 \x01(\t\x12 \n\x04open\x18\x03 \x01(\x0b\x32\x12.org.openfeed.Open\x12 \n\x04high\x18\x04 \x01(\x0b\x32\x12.org.openfeed.High\x12\x1e\n\x03low\x18\x05 \x01(\x0b\x32\x11.org.openfeed.Low\x12\"\n\x05\x63lose\x18\x06 \x01(\x0b\x32\x13.org.openfeed.Close\x12\x0e\n\x06volume\x18\x07 \x01(\x12\x12\x13\n\x0bpriceVolume\x18\x08 \x01(\x01\x12\x14\n\x0cnumberTrades\x18\t \x01(\x12\x12\x11\n\ttradeDate\x18\n \x01(\x11\x12\x17\n\x0ftransactionTime\x18\x0b \x01(\x12\x12\x10\n\x08tradeIds\x18\x0c \x03(\t\x12\x15\n\ropenStartTime\x18\r \x01(\x12\x12\x14\n\x0c\x63loseEndTime\x18\x0e \x01(\x12\"\xec\x01\n\x10InstrumentAction\x12\x17\n\x0ftransactionTime\x18\x01 \x01(\x12\x12\x11\n\ttradeDate\x18\x02 \x01(\x11\x12(\n\x06\x61\x63tion\x18\x03 \x01(\x0e\x32\x18.org.openfeed.ActionType\x12\x0f\n\x07message\x18\x04 \x01(\t\x12\x36\n\ninstrument\x18\n \x01(\x0b\x32\".org.openfeed.InstrumentDefinition\x12\x39\n\rnewInstrument\x18\x0b \x01(\x0b\x32\".org.openfeed.InstrumentDefinition*5\n\x08\x42ookSide\x12\x15\n\x11UNKNOWN_BOOK_SIDE\x10\x00\x12\x07\n\x03\x42ID\x10\x01\x12\t\n\x05OFFER\x10\x02*\xa0\x05\n\x17InstrumentTradingStatus\x12\x1a\n\x16UNKNOWN_TRADING_STATUS\x10\x00\x12\x12\n\x0eTRADING_RESUME\x10\x01\x12\x0c\n\x08PRE_OPEN\x10\x02\x12\x08\n\x04OPEN\x10\x03\x12\r\n\tPRE_CLOSE\x10\x04\x12\t\n\x05\x43LOSE\x10\x05\x12\x10\n\x0cTRADING_HALT\x10\x06\x12\x14\n\x10QUOTATION_RESUME\x10\x07\x12\x0e\n\nOPEN_DELAY\x10\x08\x12\x15\n\x11NO_OPEN_NO_RESUME\x10\t\x12\x0f\n\x0b\x46\x41ST_MARKET\x10\n\x12\x13\n\x0f\x46\x41ST_MARKET_END\x10\x0b\x12\x0f\n\x0bLATE_MARKET\x10\x0c\x12\x13\n\x0fLATE_MARKET_END\x10\r\x12\x10\n\x0cPOST_SESSION\x10\x0e\x12\x14\n\x10POST_SESSION_END\x10\x0f\x12\x18\n\x14NEW_PRICE_INDICATION\x10\x10\x12\x1d\n\x19NOT_AVAILABLE_FOR_TRADING\x10\x11\x12\r\n\tPRE_CROSS\x10\x12\x12\t\n\x05\x43ROSS\x10\x13\x12\x0e\n\nPOST_CLOSE\x10\x14\x12\r\n\tNO_CHANGE\x10\x15\x12\x08\n\x04NAFT\x10\x16\x12\x1c\n\x18TRADING_RANGE_INDICATION\x10\x17\x12\x18\n\x14MARKET_IMBALANCE_BUY\x10\x18\x12\x19\n\x15MARKET_IMBALANCE_SELL\x10\x19\x12\x15\n\x11MOC_IMBALANCE_BUY\x10\x1a\x12\x16\n\x12MOC_IMBALANCE_SELL\x10\x1b\x12\x17\n\x13NO_MARKET_IMBALANCE\x10\x1c\x12\x14\n\x10NO_MOC_IMBALANCE\x10\x1d\x12\x1a\n\x16SHORT_SELL_RESTRICTION\x10\x1e\x12\x17\n\x13LIMIT_UP_LIMIT_DOWN\x10\x1f*\x8a\x01\n\x1fRegulationSHOShortSalePriceTest\x12\x16\n\x12UNKNOWN_PRICE_TEST\x10\x00\x12\x13\n\x0fPRICE_TEST_NONE\x10\x01\x12\x18\n\x14PRICE_TEST_IN_EFFECT\x10\x02\x12 \n\x1cPRICE_TEST_REMAINS_IN_EFFECT\x10\x03*v\n\x0fSettlementTerms\x12\x1c\n\x18UNKNOWN_SETTLEMENT_TERMS\x10\x00\x12\x08\n\x04\x43\x41SH\x10\x01\x12\x0b\n\x07NON_NET\x10\x02\x12\x14\n\x10\x43ONTINGENT_TRADE\x10\x03\x12\x0e\n\nCASH_TODAY\x10\x04\x12\x08\n\x04\x44\x41TE\x10\x05*}\n\tCrossType\x12\x16\n\x12UNKNOWN_CROSS_TYPE\x10\x00\x12\x0b\n\x07\x44\x45\x46\x41ULT\x10\x01\x12\x0c\n\x08INTERNAL\x10\x02\x12\t\n\x05\x42\x41SIS\x10\x03\x12\x0e\n\nCONTINGENT\x10\x04\x12\x0b\n\x07SPECIAL\x10\x05\x12\x08\n\x04VWAP\x10\x06\x12\x0b\n\x07REGULAR\x10\x07*Q\n\x17OpenCloseSettlementFlag\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0e\n\nDAILY_OPEN\x10\x01\x12\x19\n\x15INDICATIVE_OPEN_PRICE\x10\x02*R\n\x10SettlementSource\x12\x1d\n\x19UNKNOWN_SETTLEMENT_SOURCE\x10\x00\x12\n\n\x06GLOBEX\x10\x01\x12\x07\n\x03ITC\x10\x02\x12\n\n\x06MANUAL\x10\x03*x\n\x07Service\x12\x13\n\x0fUNKNOWN_SERVICE\x10\x00\x12\r\n\tREAL_TIME\x10\x01\x12\x0b\n\x07\x44\x45LAYED\x10\x02\x12\x16\n\x12REAL_TIME_SNAPSHOT\x10\x03\x12\x14\n\x10\x44\x45LAYED_SNAPSHOT\x10\x04\x12\x0e\n\nEND_OF_DAY\x10\x05*y\n\x10MarketWideStatus\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x17\n\x13STATUS_START_OF_DAY\x10\x01\x12\x15\n\x11STATUS_END_OF_DAY\x10\x02\x12\x0f\n\x0bSTATUS_OPEN\x10\x03\x12\x10\n\x0cSTATUS_CLOSE\x10\x04*\xcc\x01\n\x15SnapshotRequestResult\x12#\n\x1fSNAPSHOT_REQUEST_UNKNOWN_RESULT\x10\x00\x12\x1c\n\x18SNAPSHOT_REQUEST_SUCCESS\x10\x01\x12\x1e\n\x1aSNAPSHOT_REQUEST_NOT_FOUND\x10\x02\x12*\n&SNAPSHOT_REQUEST_SERVICE_NOT_AVAILABLE\x10\x03\x12$\n SNAPSHOT_REQUEST_GENERIC_FAILURE\x10\x04*O\n\nActionType\x12\x12\n\x0eUNKNOWN_ACTION\x10\x00\x12\x0b\n\x07LISTING\x10\x01\x12\r\n\tDELISTING\x10\x02\x12\x11\n\rEXCHANGE_MOVE\x10\x03\x42\x07H\x01P\x01\xa0\x01\x01\x62\x06proto3'
   ,
   dependencies=[openfeed__instrument__pb2.DESCRIPTOR,])
 
 _BOOKSIDE = _descriptor.EnumDescriptor(
   name='BookSide',
   full_name='org.openfeed.BookSide',
   filename=None,
@@ -46,16 +46,16 @@
       name='OFFER', index=2, number=2,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=14814,
-  serialized_end=14867,
+  serialized_start=14838,
+  serialized_end=14891,
 )
 _sym_db.RegisterEnumDescriptor(_BOOKSIDE)
 
 BookSide = enum_type_wrapper.EnumTypeWrapper(_BOOKSIDE)
 _INSTRUMENTTRADINGSTATUS = _descriptor.EnumDescriptor(
   name='InstrumentTradingStatus',
   full_name='org.openfeed.InstrumentTradingStatus',
@@ -222,16 +222,16 @@
       name='LIMIT_UP_LIMIT_DOWN', index=31, number=31,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=14870,
-  serialized_end=15542,
+  serialized_start=14894,
+  serialized_end=15566,
 )
 _sym_db.RegisterEnumDescriptor(_INSTRUMENTTRADINGSTATUS)
 
 InstrumentTradingStatus = enum_type_wrapper.EnumTypeWrapper(_INSTRUMENTTRADINGSTATUS)
 _REGULATIONSHOSHORTSALEPRICETEST = _descriptor.EnumDescriptor(
   name='RegulationSHOShortSalePriceTest',
   full_name='org.openfeed.RegulationSHOShortSalePriceTest',
@@ -258,16 +258,16 @@
       name='PRICE_TEST_REMAINS_IN_EFFECT', index=3, number=3,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=15545,
-  serialized_end=15683,
+  serialized_start=15569,
+  serialized_end=15707,
 )
 _sym_db.RegisterEnumDescriptor(_REGULATIONSHOSHORTSALEPRICETEST)
 
 RegulationSHOShortSalePriceTest = enum_type_wrapper.EnumTypeWrapper(_REGULATIONSHOSHORTSALEPRICETEST)
 _SETTLEMENTTERMS = _descriptor.EnumDescriptor(
   name='SettlementTerms',
   full_name='org.openfeed.SettlementTerms',
@@ -304,16 +304,16 @@
       name='DATE', index=5, number=5,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=15685,
-  serialized_end=15803,
+  serialized_start=15709,
+  serialized_end=15827,
 )
 _sym_db.RegisterEnumDescriptor(_SETTLEMENTTERMS)
 
 SettlementTerms = enum_type_wrapper.EnumTypeWrapper(_SETTLEMENTTERMS)
 _CROSSTYPE = _descriptor.EnumDescriptor(
   name='CrossType',
   full_name='org.openfeed.CrossType',
@@ -360,16 +360,16 @@
       name='REGULAR', index=7, number=7,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=15805,
-  serialized_end=15930,
+  serialized_start=15829,
+  serialized_end=15954,
 )
 _sym_db.RegisterEnumDescriptor(_CROSSTYPE)
 
 CrossType = enum_type_wrapper.EnumTypeWrapper(_CROSSTYPE)
 _OPENCLOSESETTLEMENTFLAG = _descriptor.EnumDescriptor(
   name='OpenCloseSettlementFlag',
   full_name='org.openfeed.OpenCloseSettlementFlag',
@@ -391,16 +391,16 @@
       name='INDICATIVE_OPEN_PRICE', index=2, number=2,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=15932,
-  serialized_end=16013,
+  serialized_start=15956,
+  serialized_end=16037,
 )
 _sym_db.RegisterEnumDescriptor(_OPENCLOSESETTLEMENTFLAG)
 
 OpenCloseSettlementFlag = enum_type_wrapper.EnumTypeWrapper(_OPENCLOSESETTLEMENTFLAG)
 _SETTLEMENTSOURCE = _descriptor.EnumDescriptor(
   name='SettlementSource',
   full_name='org.openfeed.SettlementSource',
@@ -427,16 +427,16 @@
       name='MANUAL', index=3, number=3,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=16015,
-  serialized_end=16097,
+  serialized_start=16039,
+  serialized_end=16121,
 )
 _sym_db.RegisterEnumDescriptor(_SETTLEMENTSOURCE)
 
 SettlementSource = enum_type_wrapper.EnumTypeWrapper(_SETTLEMENTSOURCE)
 _SERVICE = _descriptor.EnumDescriptor(
   name='Service',
   full_name='org.openfeed.Service',
@@ -473,16 +473,16 @@
       name='END_OF_DAY', index=5, number=5,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=16099,
-  serialized_end=16219,
+  serialized_start=16123,
+  serialized_end=16243,
 )
 _sym_db.RegisterEnumDescriptor(_SERVICE)
 
 Service = enum_type_wrapper.EnumTypeWrapper(_SERVICE)
 _MARKETWIDESTATUS = _descriptor.EnumDescriptor(
   name='MarketWideStatus',
   full_name='org.openfeed.MarketWideStatus',
@@ -514,16 +514,16 @@
       name='STATUS_CLOSE', index=4, number=4,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=16221,
-  serialized_end=16342,
+  serialized_start=16245,
+  serialized_end=16366,
 )
 _sym_db.RegisterEnumDescriptor(_MARKETWIDESTATUS)
 
 MarketWideStatus = enum_type_wrapper.EnumTypeWrapper(_MARKETWIDESTATUS)
 _SNAPSHOTREQUESTRESULT = _descriptor.EnumDescriptor(
   name='SnapshotRequestResult',
   full_name='org.openfeed.SnapshotRequestResult',
@@ -555,16 +555,16 @@
       name='SNAPSHOT_REQUEST_GENERIC_FAILURE', index=4, number=4,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=16345,
-  serialized_end=16549,
+  serialized_start=16369,
+  serialized_end=16573,
 )
 _sym_db.RegisterEnumDescriptor(_SNAPSHOTREQUESTRESULT)
 
 SnapshotRequestResult = enum_type_wrapper.EnumTypeWrapper(_SNAPSHOTREQUESTRESULT)
 _ACTIONTYPE = _descriptor.EnumDescriptor(
   name='ActionType',
   full_name='org.openfeed.ActionType',
@@ -591,16 +591,16 @@
       name='EXCHANGE_MOVE', index=3, number=3,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=16551,
-  serialized_end=16630,
+  serialized_start=16575,
+  serialized_end=16654,
 )
 _sym_db.RegisterEnumDescriptor(_ACTIONTYPE)
 
 ActionType = enum_type_wrapper.EnumTypeWrapper(_ACTIONTYPE)
 UNKNOWN_BOOK_SIDE = 0
 BID = 1
 OFFER = 2
@@ -729,16 +729,16 @@
       name='CUSTOM_1', index=3, number=3,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=13037,
-  serialized_end=13088,
+  serialized_start=13061,
+  serialized_end=13112,
 )
 _sym_db.RegisterEnumDescriptor(_MARKETSUMMARY_CLEARSET)
 
 _MARKETSUMMARY_SUMMARYTYPE = _descriptor.EnumDescriptor(
   name='SummaryType',
   full_name='org.openfeed.MarketSummary.SummaryType',
   filename=None,
@@ -769,16 +769,16 @@
       name='EOD_COMMODITY_STATS', index=4, number=4,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=13091,
-  serialized_end=13229,
+  serialized_start=13115,
+  serialized_end=13253,
 )
 _sym_db.RegisterEnumDescriptor(_MARKETSUMMARY_SUMMARYTYPE)
 
 _SNAPSHOTREQUEST_SNAPSHOTREQUESTTYPE = _descriptor.EnumDescriptor(
   name='SnapshotRequestType',
   full_name='org.openfeed.SnapshotRequest.SnapshotRequestType',
   filename=None,
@@ -804,16 +804,16 @@
       name='VOLUME_AT_PRICE', index=3, number=3,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=13869,
-  serialized_end=13942,
+  serialized_start=13893,
+  serialized_end=13966,
 )
 _sym_db.RegisterEnumDescriptor(_SNAPSHOTREQUEST_SNAPSHOTREQUESTTYPE)
 
 
 _OPENFEEDMESSAGE = _descriptor.Descriptor(
   name='OpenfeedMessage',
   full_name='org.openfeed.OpenfeedMessage',
@@ -3291,28 +3291,35 @@
     _descriptor.FieldDescriptor(
       name='transient', full_name='org.openfeed.Trade.transient', index=26,
       number=35, type=8, cpp_type=7, label=1,
       has_default_value=False, default_value=False,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='indexShortName', full_name='org.openfeed.Trade.indexShortName', index=27,
+      number=36, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=8232,
-  serialized_end=8887,
+  serialized_end=8911,
 )
 
 
 _TRADECORRECTION = _descriptor.Descriptor(
   name='TradeCorrection',
   full_name='org.openfeed.TradeCorrection',
   filename=None,
@@ -3489,16 +3496,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=8890,
-  serialized_end=9472,
+  serialized_start=8914,
+  serialized_end=9496,
 )
 
 
 _TRADECANCEL = _descriptor.Descriptor(
   name='TradeCancel',
   full_name='org.openfeed.TradeCancel',
   filename=None,
@@ -3577,16 +3584,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=9475,
-  serialized_end=9706,
+  serialized_start=9499,
+  serialized_end=9730,
 )
 
 
 _OPEN = _descriptor.Descriptor(
   name='Open',
   full_name='org.openfeed.Open',
   filename=None,
@@ -3637,16 +3644,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=9709,
-  serialized_end=9864,
+  serialized_start=9733,
+  serialized_end=9888,
 )
 
 
 _HIGH = _descriptor.Descriptor(
   name='High',
   full_name='org.openfeed.High',
   filename=None,
@@ -3690,16 +3697,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=9866,
-  serialized_end=9949,
+  serialized_start=9890,
+  serialized_end=9973,
 )
 
 
 _HIGHROLLING = _descriptor.Descriptor(
   name='HighRolling',
   full_name='org.openfeed.HighRolling',
   filename=None,
@@ -3743,16 +3750,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=9951,
-  serialized_end=10041,
+  serialized_start=9975,
+  serialized_end=10065,
 )
 
 
 _LOW = _descriptor.Descriptor(
   name='Low',
   full_name='org.openfeed.Low',
   filename=None,
@@ -3796,16 +3803,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=10043,
-  serialized_end=10125,
+  serialized_start=10067,
+  serialized_end=10149,
 )
 
 
 _LOWROLLING = _descriptor.Descriptor(
   name='LowRolling',
   full_name='org.openfeed.LowRolling',
   filename=None,
@@ -3849,16 +3856,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=10127,
-  serialized_end=10216,
+  serialized_start=10151,
+  serialized_end=10240,
 )
 
 
 _CLOSE = _descriptor.Descriptor(
   name='Close',
   full_name='org.openfeed.Close',
   filename=None,
@@ -3902,16 +3909,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=10218,
-  serialized_end=10302,
+  serialized_start=10242,
+  serialized_end=10326,
 )
 
 
 _PREVCLOSE = _descriptor.Descriptor(
   name='PrevClose',
   full_name='org.openfeed.PrevClose',
   filename=None,
@@ -3955,16 +3962,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=10304,
-  serialized_end=10392,
+  serialized_start=10328,
+  serialized_end=10416,
 )
 
 
 _LAST = _descriptor.Descriptor(
   name='Last',
   full_name='org.openfeed.Last',
   filename=None,
@@ -4022,16 +4029,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=10394,
-  serialized_end=10512,
+  serialized_start=10418,
+  serialized_end=10536,
 )
 
 
 _YEARHIGH = _descriptor.Descriptor(
   name='YearHigh',
   full_name='org.openfeed.YearHigh',
   filename=None,
@@ -4068,16 +4075,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=10514,
-  serialized_end=10582,
+  serialized_start=10538,
+  serialized_end=10606,
 )
 
 
 _YEARLOW = _descriptor.Descriptor(
   name='YearLow',
   full_name='org.openfeed.YearLow',
   filename=None,
@@ -4114,16 +4121,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=10584,
-  serialized_end=10651,
+  serialized_start=10608,
+  serialized_end=10675,
 )
 
 
 _VOLUME = _descriptor.Descriptor(
   name='Volume',
   full_name='org.openfeed.Volume',
   filename=None,
@@ -4160,16 +4167,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=10653,
-  serialized_end=10721,
+  serialized_start=10677,
+  serialized_end=10745,
 )
 
 
 _NUMBEROFTRADES = _descriptor.Descriptor(
   name='NumberOfTrades',
   full_name='org.openfeed.NumberOfTrades',
   filename=None,
@@ -4206,16 +4213,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=10723,
-  serialized_end=10805,
+  serialized_start=10747,
+  serialized_end=10829,
 )
 
 
 _MONETARYVALUE = _descriptor.Descriptor(
   name='MonetaryValue',
   full_name='org.openfeed.MonetaryValue',
   filename=None,
@@ -4259,16 +4266,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=10807,
-  serialized_end=10908,
+  serialized_start=10831,
+  serialized_end=10932,
 )
 
 
 _SETTLEMENT = _descriptor.Descriptor(
   name='Settlement',
   full_name='org.openfeed.Settlement',
   filename=None,
@@ -4347,16 +4354,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=10911,
-  serialized_end=11139,
+  serialized_start=10935,
+  serialized_end=11163,
 )
 
 
 _OPENINTEREST = _descriptor.Descriptor(
   name='OpenInterest',
   full_name='org.openfeed.OpenInterest',
   filename=None,
@@ -4393,16 +4400,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=11141,
-  serialized_end=11215,
+  serialized_start=11165,
+  serialized_end=11239,
 )
 
 
 _VWAP = _descriptor.Descriptor(
   name='Vwap',
   full_name='org.openfeed.Vwap',
   filename=None,
@@ -4439,16 +4446,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=11217,
-  serialized_end=11281,
+  serialized_start=11241,
+  serialized_end=11305,
 )
 
 
 _DIVIDENDSINCOMEDISTRIBUTIONS = _descriptor.Descriptor(
   name='DividendsIncomeDistributions',
   full_name='org.openfeed.DividendsIncomeDistributions',
   filename=None,
@@ -4590,16 +4597,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=11284,
-  serialized_end=11788,
+  serialized_start=11308,
+  serialized_end=11812,
 )
 
 
 _CAPITALDISTRIBUTIONS = _descriptor.Descriptor(
   name='CapitalDistributions',
   full_name='org.openfeed.CapitalDistributions',
   filename=None,
@@ -4706,16 +4713,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=11791,
-  serialized_end=12121,
+  serialized_start=11815,
+  serialized_end=12145,
 )
 
 
 _SHARESOUTSTANDING = _descriptor.Descriptor(
   name='SharesOutstanding',
   full_name='org.openfeed.SharesOutstanding',
   filename=None,
@@ -4745,16 +4752,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=12123,
-  serialized_end=12194,
+  serialized_start=12147,
+  serialized_end=12218,
 )
 
 
 _NETASSETVALUE = _descriptor.Descriptor(
   name='NetAssetValue',
   full_name='org.openfeed.NetAssetValue',
   filename=None,
@@ -4784,16 +4791,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=12196,
-  serialized_end=12259,
+  serialized_start=12220,
+  serialized_end=12283,
 )
 
 
 _MARKETSUMMARY = _descriptor.Descriptor(
   name='MarketSummary',
   full_name='org.openfeed.MarketSummary',
   filename=None,
@@ -4958,16 +4965,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=12262,
-  serialized_end=13229,
+  serialized_start=12286,
+  serialized_end=13253,
 )
 
 
 _CONTEXT = _descriptor.Descriptor(
   name='Context',
   full_name='org.openfeed.Context',
   filename=None,
@@ -4997,16 +5004,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=13231,
-  serialized_end=13328,
+  serialized_start=13255,
+  serialized_end=13352,
 )
 
 
 _CONTEXTDATA = _descriptor.Descriptor(
   name='ContextData',
   full_name='org.openfeed.ContextData',
   filename=None,
@@ -5083,16 +5090,16 @@
   oneofs=[
     _descriptor.OneofDescriptor(
       name='data', full_name='org.openfeed.ContextData.data',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
-  serialized_start=13331,
-  serialized_end=13493,
+  serialized_start=13355,
+  serialized_end=13517,
 )
 
 
 _TRACEPOINT = _descriptor.Descriptor(
   name='TracePoint',
   full_name='org.openfeed.TracePoint',
   filename=None,
@@ -5136,16 +5143,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=13495,
-  serialized_end=13589,
+  serialized_start=13519,
+  serialized_end=13613,
 )
 
 
 _TCPHISTORICALREPLAYREQUEST = _descriptor.Descriptor(
   name='TCPHistoricalReplayRequest',
   full_name='org.openfeed.TCPHistoricalReplayRequest',
   filename=None,
@@ -5196,16 +5203,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=13591,
-  serialized_end=13709,
+  serialized_start=13615,
+  serialized_end=13733,
 )
 
 
 _SNAPSHOTREQUEST = _descriptor.Descriptor(
   name='SnapshotRequest',
   full_name='org.openfeed.SnapshotRequest',
   filename=None,
@@ -5250,16 +5257,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=13712,
-  serialized_end=13942,
+  serialized_start=13736,
+  serialized_end=13966,
 )
 
 
 _VOLUMEATPRICE_PRICELEVELVOLUME = _descriptor.Descriptor(
   name='PriceLevelVolume',
   full_name='org.openfeed.VolumeAtPrice.PriceLevelVolume',
   filename=None,
@@ -5289,16 +5296,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=14179,
-  serialized_end=14228,
+  serialized_start=14203,
+  serialized_end=14252,
 )
 
 _VOLUMEATPRICE = _descriptor.Descriptor(
   name='VolumeAtPrice',
   full_name='org.openfeed.VolumeAtPrice',
   filename=None,
   file=DESCRIPTOR,
@@ -5369,16 +5376,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=13945,
-  serialized_end=14228,
+  serialized_start=13969,
+  serialized_end=14252,
 )
 
 
 _OHLC = _descriptor.Descriptor(
   name='Ohlc',
   full_name='org.openfeed.Ohlc',
   filename=None,
@@ -5492,16 +5499,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=14231,
-  serialized_end=14573,
+  serialized_start=14255,
+  serialized_end=14597,
 )
 
 
 _INSTRUMENTACTION = _descriptor.Descriptor(
   name='InstrumentAction',
   full_name='org.openfeed.InstrumentAction',
   filename=None,
@@ -5559,16 +5566,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=14576,
-  serialized_end=14812,
+  serialized_start=14600,
+  serialized_end=14836,
 )
 
 _OPENFEEDMESSAGE.fields_by_name['context'].message_type = _CONTEXT
 _OPENFEEDMESSAGE.fields_by_name['channelReset'].message_type = _CHANNELRESET
 _OPENFEEDMESSAGE.fields_by_name['heartBeat'].message_type = _HEARTBEAT
 _OPENFEEDMESSAGE.fields_by_name['adminMessage'].message_type = _ADMINMESSAGE
 _OPENFEEDMESSAGE.fields_by_name['instrumentDefinition'].message_type = openfeed__instrument__pb2._INSTRUMENTDEFINITION
```

### Comparing `openfeed-1.2.0/openfeed/openfeed_client.py` & `openfeed-1.3.0/openfeed/openfeed_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 from typing import Union
 from generated import openfeed_api_pb2
 from generated import openfeed_pb2
 from generated import openfeed_instrument_pb2
+from struct import unpack
+from io import BytesIO
+import platform
 import time
 import traceback
 import sys
 import inspect
 import collections
 import websocket
 import random
+from .version import VERSION
 try:
     import thread
 except ImportError:
     import _thread as thread
 
 
 class OpenfeedClient(object):
@@ -80,21 +84,18 @@
         ----------
         service: str, optional
             Default is `REAL_TIME` for delayed market data, set it to `DELAYED`, or for snapshots set it as one of `REAL_TIME_SNAPSHOT` or `DELAYED_SNAPSHOT'
         callback: Callable
             Your callback function for Market Data messages
         subscription_type: list, optional
             Default is ['QUOTE']. Can contain any of: 'ALL', 'QUOTE', 'QUOTE_PARTICIPANT', 'DEPTH_PRICE', 'DEPTH_ORDER', 'TRADES', 'OHLC'
-        instrument_type: list, optional
-            Spreads and Options must be explicitly requested. Can contain any of: 'SPREAD', 'OPTION', 'FUTURE', 'FOREX', 'EQUITY', 'INDEX', 'MUTUAL_FUND', 'MONEY_MARKET', 'MONEY_MARKET_FUND'
 
         [Market Data]: https://docs.barchart.com/openfeed/#/proto?id=marketupdate
         [SubscriptionTypes]: https://docs.barchart.com/openfeed/#/proto?id=subscriptiontype
         [Service]: https://docs.barchart.com/openfeed/#/proto?id=service
-        [InstrumentTypes]: https://docs.barchart.com/openfeed/#/proto?id=instrumentdefinitioninstrumenttype
         """
         symbols = []
 
         if isinstance(symbol, list) == False:
             symbols = [symbol]
         else:
             symbols = symbol
@@ -108,42 +109,59 @@
 
         if self.token is not None:
             self._send_message(
                 self.__create_subscription_request(symbols=symbols, service=service, subscription_type=subscription_type, snapshot_interval_seconds=snapshot_interval_seconds))
 
         return self
 
-    def add_exchange_subscription(self, exchange: Union[str, list], callback, service="REAL_TIME", subscription_type=["QUOTE"], instrument_type=[], snapshot_interval_seconds=60):
+    def add_exchange_subscription(self, exchange: Union[str, list], callback, service="REAL_TIME", subscription_type=["QUOTE"], instrument_type=[], snapshot_interval_seconds=60, bulk_subscription_filters=[]):
         """Subscribe to [Market Data] by Barchart Exchange code(s).
 
         Complete list of [SubscriptionTypes]. List of [Service] types.
 
         Note: your credentials must have the correct service level (FEED) for this operation.
 
+        Parameters
+        ----------
+        exchange: str, list
+            Barchart Exchange code(s)
+        service: str, optional
+            [ServiceType]. Default is `REAL_TIME` for delayed market data, set it to `DELAYED`, or for snapshots set it as one of `REAL_TIME_SNAPSHOT` or `DELAYED_SNAPSHOT'
+        callback: Callable
+            Your callback function for Market Data messages
+        subscription_type: list, optional
+            [SubscriptionTypes]. Default is ['QUOTE']. Can contain any of: 'ALL', 'QUOTE', 'QUOTE_PARTICIPANT', 'DEPTH_PRICE', 'DEPTH_ORDER', 'TRADES', 'OHLC'
+        instrument_type: list, optional
+            [InstrumentTypes]. Spreads and Options must be explicitly requested. Can contain any of: 'SPREAD', 'OPTION', 'FUTURE', 'FOREX', 'EQUITY', 'INDEX', 'MUTUAL_FUND', 'MONEY_MARKET', 'MONEY_MARKET_FUND'
+        bulk_subscription_filters: list of BulkSubscriptionFilter, optional
+            List of [BulkSubscriptionFilter]
+
         [Market Data]: https://docs.barchart.com/openfeed/#/proto?id=marketupdate
         [SubscriptionTypes]: https://docs.barchart.com/openfeed/#/proto?id=subscriptiontype
-        [Service]: https://docs.barchart.com/openfeed/#/proto?id=service
+        [ServiceType]: https://docs.barchart.com/openfeed/#/proto?id=service
+        [InstrumentTypes]: https://docs.barchart.com/openfeed/#/proto?id=instrumentdefinitioninstrumenttype
+        [BulkSubscriptionFilter]: https://docs.barchart.com/openfeed/#/proto?id=bulksubscriptionfilter
         """
         exchanges = []
 
         if isinstance(exchange, list) == False:
             exchanges = [exchange]
         else:
             exchanges = exchange
 
         for exch in exchanges:
             if exch not in self.exchange_handlers:
                 self.exchange_handlers[exch] = []
 
             self.exchange_handlers[exch].append(Listener(
-                exchange=exch, callback=callback, service=service, subscription_type=subscription_type, instrument_type=instrument_type, snapshot_interval_seconds=snapshot_interval_seconds))
+                exchange=exch, callback=callback, service=service, subscription_type=subscription_type, instrument_type=instrument_type, snapshot_interval_seconds=snapshot_interval_seconds, bulk_subscription_filters=bulk_subscription_filters))
 
         if self.token is not None:
-            self._send_message(
-                self.__create_subscription_request(exchanges=exchanges, service=service, subscription_type=subscription_type, instrument_type=instrument_type, snapshot_interval_seconds=snapshot_interval_seconds))
+             self._send_message(
+                self.__create_subscription_request(exchanges=exchanges, service=service, subscription_type=subscription_type, instrument_type=instrument_type, snapshot_interval_seconds=snapshot_interval_seconds, bulk_subscription_filters=bulk_subscription_filters))
 
         return self
 
     def request_available_exchanges(self, callback):
         """Request a list of available [Exchanges] for subscription.
 
         [Exchanges]: https://docs.barchart.com/openfeed/#/openfeed_streaming?id=requesting-exchanges
@@ -356,30 +374,42 @@
             "instrumentDefinition": handleInstrumentDefinition,
             "marketSnapshot": handleMarketSnapshot,
             "marketUpdate": handleMarketUpdate,
             "ohlc": handleOHLC
         }
 
         def on_message(ws: websocket.WebSocketApp, message):
+            byte_buffer = BytesIO(message)
+            total = byte_buffer.getbuffer().nbytes
 
-            msg = openfeed_api_pb2.OpenfeedGatewayMessage()
-            msg.ParseFromString(message)
+            msg_count = 0
 
-            msg_type = msg.WhichOneof("data")
+            while byte_buffer.tell() != total:
+                msg_len = int.from_bytes(byte_buffer.read(
+                    2), byteorder='big', signed=True)
 
-            handler = handlers.get(
-                msg_type, lambda x: print("Unhandled Message:", x))
+                msg = openfeed_api_pb2.OpenfeedGatewayMessage()
+                msg.ParseFromString(byte_buffer.read(msg_len))
 
-            try:
-                handler(msg)
-            except Exception as e:
                 if self.debug:
-                    print("Failed handling incoming message:", msg_type, e)
-                    traceback.print_exc()
-                self.__callback(self.on_error, e)
+                    msg_count = msg_count+1
+                    print("msg len:", msg_len, "number of messages:", msg_count)
+
+                msg_type = msg.WhichOneof("data")
+
+                handler = handlers.get(
+                    msg_type, lambda x: print("Unhandled Message:", x))
+
+                try:
+                    handler(msg)
+                except Exception as e:
+                    if self.debug:
+                        print("Failed handling incoming message:", msg_type, e)
+                        traceback.print_exc()
+                    self.__callback(self.on_error, e)
 
         def on_error(ws, error):
             if self.debug:
                 print("WebSocket Error: ", error)
                 traceback.print_exc()
             self.__callback(self.on_error, error)
 
@@ -458,42 +488,50 @@
         for listeners in all_listeners:
             for l in listeners:
                 if l.service not in interest:
                     interest[l.service] = {}
                 listeners_by_service = interest[l.service]
                 if l.key() not in listeners_by_service:
                     listeners_by_service[l.key()] = Listener(
-                        symbol=l.symbol, exchange=l.exchange, service=l.service, subscription_type=l.subscription_type, instrument_type=l.instrument_type, snapshot_interval_seconds=l.snapshot_interval_seconds)
+                        symbol=l.symbol, exchange=l.exchange, service=l.service, subscription_type=l.subscription_type, instrument_type=l.instrument_type, snapshot_interval_seconds=l.snapshot_interval_seconds, bulk_subscription_filters=l.bulk_subscription_filters)
                 else:
                     existing = listeners_by_service[l.key()]
                     existing.subscription_type = list(set(
                         existing.subscription_type + l.subscription_type))
 
         # send subscriptions
         for service in interest.keys():
             for i in interest[service].values():
                 self._send_message(
-                    self.__create_subscription_request(exchanges=i.exchanges(), symbols=i.symbols(), service=service, subscription_type=i.subscription_type, instrument_type=i.get_instrument_types(), snapshot_interval_seconds=i.snapshot_interval_seconds))
+                    self.__create_subscription_request(exchanges=i.exchanges(),
+                                                       symbols=i.symbols(),
+                                                       service=service,
+                                                       subscription_type=i.subscription_type,
+                                                       instrument_type=i.get_instrument_types(),
+                                                       snapshot_interval_seconds=i.snapshot_interval_seconds,
+                                                       bulk_subscription_filters=i.bulk_subscription_filters))
 
         # send other rpc requests
         for req in self.request_id_handlers.values():
             req.send(self)
 
-    def __create_subscription_request(self, exchanges=[], symbols=[], service="REAL_TIME", subscription_type=["QUOTE"], instrument_type=[], snapshot_interval_seconds=60):
+    def __create_subscription_request(self, exchanges=[], symbols=[], service="REAL_TIME", subscription_type=["QUOTE"], instrument_type=[], snapshot_interval_seconds=60, bulk_subscription_filters=[]):
         requests = []
 
         if len(exchanges) > 0:
             for exch in exchanges:
                 requests.append(openfeed_api_pb2.SubscriptionRequest.Request(
                     exchange=exch,
                     subscriptionType=[openfeed_api_pb2.SubscriptionType.Value(
                         t) for t in subscription_type],
                     snapshotIntervalSeconds=snapshot_interval_seconds,
                     instrumentType=[openfeed_instrument_pb2.InstrumentDefinition.InstrumentType.Value(
-                        t) for t in instrument_type]
+                        t) for t in instrument_type],
+                    bulkSubscriptionFilter=[openfeed_api_pb2.BulkSubscriptionFilter(
+                        symbolType=f.symbolType, symbolPattern=f.symbolPattern) for f in bulk_subscription_filters]
                 ))
 
         if len(symbols) > 0:
             for sym in symbols:
                 requests.append(openfeed_api_pb2.SubscriptionRequest.Request(
                     symbol=sym,
                     subscriptionType=[openfeed_api_pb2.SubscriptionType.Value(
@@ -553,35 +591,39 @@
                     vendor="Barchart",
                     symbol=symbol
                 )
             ]
         )
 
     def __create_login_request(self):
+        client_version = "sdk_python_version={}:python_version={}:sys_version:{}".format(
+            VERSION, platform.python_version(), sys.version)
         return openfeed_api_pb2.OpenfeedGatewayRequest(
             loginRequest=openfeed_api_pb2.LoginRequest(
+                protocolVersion=1, clientVersion=client_version,
                 username=self.username, password=self.password))
 
     def __callback(self, callback, *args):
         try:
             if callback is not None:
                 callback(*args)
         except Exception as e:
             print("Failed to call callback", e)
 
 
 class Listener(object):
-    def __init__(self, symbol="", exchange="", callback=None, service="REAL_TIME", subscription_type=["QUOTE"], instrument_type=[], snapshot_interval_seconds=60):
+    def __init__(self, symbol="", exchange="", callback=None, service="REAL_TIME", subscription_type=["QUOTE"], instrument_type=[], snapshot_interval_seconds=60, bulk_subscription_filters=[]):
         self.symbol = symbol
         self.exchange = exchange
         self.callback = callback
         self.service = service
         self.subscription_type = subscription_type
         self.instrument_type = instrument_type
         self.snapshot_interval_seconds = snapshot_interval_seconds
+        self.bulk_subscription_filters = bulk_subscription_filters
 
     def key(self):
         if len(self.exchange) > 0:
             return self.exchange
         return self.symbol
 
     def symbols(self):
@@ -623,14 +665,20 @@
 
         of_client._send_message(self.request)
 
     def is_type(self, request_type):
         return request_type == self.request.WhichOneof("data")
 
 
+class BulkSubscriptionFilter(object):
+    def __init__(self, symbolType, symbolPattern):
+        self.symbolType = symbolType
+        self.symbolPattern = symbolPattern
+
+
 if __name__ == "__main__":
 
     def handle_message(msg):
         print("of-client: Market Data: ", msg.WhichOneof("data"))
 
     def handle_heartbeat(msg):
         print("of-client: Heartbeat: ", msg)
```

### Comparing `openfeed-1.2.0/openfeed.egg-info/PKG-INFO` & `openfeed-1.3.0/openfeed.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openfeed
-Version: 1.2.0
+Version: 1.3.0
 Summary: Barchart Openfeed Example Client for Python
 Home-page: https://github.com/openfeed-org/sdk-python
 Download-URL: https://github.com/openfeed-org/sdk-python/archive/master.zip
 Author: Barchart
 Author-email: mike@barchart.com
 License: MIT
 Description-Content-Type: text/markdown
@@ -56,17 +56,21 @@
 of-client: Connected
 of-client: Market Data:  subscriptionResponse
 of-client: Market Data:  marketSnapshot
 of-client: Market Data:  marketUpdate
 of-client: Market Data:  marketUpdate
 ```
 
+### Openfeed Documentation
+
+* [https://docs.barchart.com/openfeed](https://docs.barchart.com/openfeed)
+
 ## Subscription Types
 
-Openfeed supports many levels of [subscription types](https://openfeed-org.github.io/documentation/Message%20Specification/#org.openfeed.SubscriptionType).
+Openfeed supports many levels of [subscription types](https://docs.barchart.com/openfeed/#/proto?id=subscriptiontype).
 
 ### OHLC
 
 ```python
 of_client.add_exchange_subscription(["NYSE"], callback=on_message, subscription_type=["OHLC"])
 ```
```

### Comparing `openfeed-1.2.0/setup.py` & `openfeed-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ]
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='openfeed',
-    version='1.2.0',
+    version='1.3.0',
     author='Barchart',
     author_email='mike@barchart.com',
     license='MIT',
     url='https://github.com/openfeed-org/sdk-python',
     include_package_data=True,
     packages=find_packages(),
     install_requires=install_requires,
```

