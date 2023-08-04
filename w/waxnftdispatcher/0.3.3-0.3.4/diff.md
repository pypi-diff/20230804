# Comparing `tmp/waxnftdispatcher-0.3.3.tar.gz` & `tmp/waxnftdispatcher-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waxnftdispatcher-0.3.3.tar", max compression
+gzip compressed data, was "waxnftdispatcher-0.3.4.tar", max compression
```

## Comparing `waxnftdispatcher-0.3.3.tar` & `waxnftdispatcher-0.3.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1068 2023-05-02 20:37:23.918020 waxnftdispatcher-0.3.3/LICENSE
--rw-r--r--   0        0        0     2052 2023-05-02 20:37:23.918020 waxnftdispatcher-0.3.3/README.md
--rw-r--r--   0        0        0      589 2023-07-13 17:43:25.555941 waxnftdispatcher-0.3.3/pyproject.toml
--rw-r--r--   0        0        0       41 2023-05-02 20:37:23.918020 waxnftdispatcher-0.3.3/waxnftdispatcher/__init__.py
--rw-r--r--   0        0        0    19689 2023-07-13 17:42:47.380956 waxnftdispatcher-0.3.3/waxnftdispatcher/waxNFTdispatcher.py
--rw-r--r--   0        0        0     2885 1970-01-01 00:00:00.000000 waxnftdispatcher-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-05-02 20:37:23.918020 waxnftdispatcher-0.3.4/LICENSE
+-rw-r--r--   0        0        0     2135 2023-08-04 09:34:02.462553 waxnftdispatcher-0.3.4/README.md
+-rw-r--r--   0        0        0      588 2023-08-04 09:32:39.142207 waxnftdispatcher-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0       41 2023-05-02 20:37:23.918020 waxnftdispatcher-0.3.4/waxnftdispatcher/__init__.py
+-rw-r--r--   0        0        0    19681 2023-08-04 09:32:03.562748 waxnftdispatcher-0.3.4/waxnftdispatcher/waxNFTdispatcher.py
+-rw-r--r--   0        0        0     2968 1970-01-01 00:00:00.000000 waxnftdispatcher-0.3.4/PKG-INFO
```

### Comparing `waxnftdispatcher-0.3.3/LICENSE` & `waxnftdispatcher-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `waxnftdispatcher-0.3.3/README.md` & `waxnftdispatcher-0.3.4/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # waxNFTdispatcher
 
-This library will help you to transfer or to mint NFTs on the WAX blockchain. It relies on the library 
+This library will help you to transfer or to mint NFTs on the WAX blockchain. It relies on the library
 pyntelope for blockchain interaction and on the library loguru for beautiful logs.
 
 By default, the [EOSUSA](https://eosusa.io/) WAX API is used to post transactions to blockchain.
 It can be changed while creating an object.
 Due to some limitations only EOSUSA API can be used to get transaction info from blockchain.
 
 
@@ -40,18 +40,21 @@
 # Mint given number of same assets
 assetsender.mint_assets("rawmaterials", "318738", "recipient.wam", 5)
 
 # Mint given number of same assets and then try to fetch their IDs
 assetsender.mint_assets_and_get_ids("rawmaterials", "318738", "recipient.wam", 5)
 ```
 
-The methods return tuple or list of tuples where on the first place is the asset ID or id-schema-template tuple, and 
+The methods return tuple or list of tuples where on the first place is the asset ID or id-schema-template tuple, and
 on the second place either hash of successful transaction or 'False' if transaction failed for some reason. For example:
 
 ```
 [(('1099511811820', 'rawmaterials', '318738'), False),
 (('1099511811819',), '6b80b145aa261736941583ed17802a8be0254cd21a78b6bb415c923ec64ad32c')]
 ```
 
 ## Contribution
-Contribution is highly welcome. Please send your pull requests or create issues with found bugs and suggestions. 
+Contribution is highly welcome. Please send your pull requests or create issues with found bugs and suggestions.
 In your pull requests please use Black formatting.
+
+## Donation
+If you feel like you can send any amount of WAX to the WAX address 24.gm
```

### Comparing `waxnftdispatcher-0.3.3/pyproject.toml` & `waxnftdispatcher-0.3.4/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "waxNFTdispatcher"
-version = "0.3.03"
+version = "0.3.4"
 description = "This library will help you to transfer or to mint NFTs on the WAX blockchain"
 authors = ["Amparo Dios <amparo.dios@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/alparo/waxNFTdispatcher"
 repository = "https://github.com/alparo/waxNFTdispatcher"
```

### Comparing `waxnftdispatcher-0.3.3/waxnftdispatcher/waxNFTdispatcher.py` & `waxnftdispatcher-0.3.4/waxnftdispatcher/waxNFTdispatcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -266,15 +266,15 @@
 
     def _send_transaction(self, action):
         """
         Sends transaction into blockchain.
         :param action: Action object.
         :return: Tuple with asset ID(s) and TX ID/False(if TX failed).
         """
-        raw_transaction = pyntelope.Transaction(actions=[action, action])
+        raw_transaction = pyntelope.Transaction(actions=[action])
         logger.debug("Linking transaction to the network...")
         if self.testnet:
             net = pyntelope.WaxTestnet()  # this is an alias for WAX testnet node
         else:
             net = pyntelope.WaxMainnet()  # this is an alias for WAX mainnet node
         linked_transaction = raw_transaction.link(net=net)
         logger.debug("Signing transaction...")
```

### Comparing `waxnftdispatcher-0.3.3/PKG-INFO` & `waxnftdispatcher-0.3.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waxnftdispatcher
-Version: 0.3.3
+Version: 0.3.4
 Summary: This library will help you to transfer or to mint NFTs on the WAX blockchain
 Home-page: https://github.com/alparo/waxNFTdispatcher
 License: MIT
 Author: Amparo Dios
 Author-email: amparo.dios@gmail.com
 Requires-Python: >=3.8.0,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -17,15 +17,15 @@
 Requires-Dist: pyntelope (>=0.8.0,<0.9.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Project-URL: Repository, https://github.com/alparo/waxNFTdispatcher
 Description-Content-Type: text/markdown
 
 # waxNFTdispatcher
 
-This library will help you to transfer or to mint NFTs on the WAX blockchain. It relies on the library 
+This library will help you to transfer or to mint NFTs on the WAX blockchain. It relies on the library
 pyntelope for blockchain interaction and on the library loguru for beautiful logs.
 
 By default, the [EOSUSA](https://eosusa.io/) WAX API is used to post transactions to blockchain.
 It can be changed while creating an object.
 Due to some limitations only EOSUSA API can be used to get transaction info from blockchain.
 
 
@@ -61,19 +61,22 @@
 # Mint given number of same assets
 assetsender.mint_assets("rawmaterials", "318738", "recipient.wam", 5)
 
 # Mint given number of same assets and then try to fetch their IDs
 assetsender.mint_assets_and_get_ids("rawmaterials", "318738", "recipient.wam", 5)
 ```
 
-The methods return tuple or list of tuples where on the first place is the asset ID or id-schema-template tuple, and 
+The methods return tuple or list of tuples where on the first place is the asset ID or id-schema-template tuple, and
 on the second place either hash of successful transaction or 'False' if transaction failed for some reason. For example:
 
 ```
 [(('1099511811820', 'rawmaterials', '318738'), False),
 (('1099511811819',), '6b80b145aa261736941583ed17802a8be0254cd21a78b6bb415c923ec64ad32c')]
 ```
 
 ## Contribution
-Contribution is highly welcome. Please send your pull requests or create issues with found bugs and suggestions. 
+Contribution is highly welcome. Please send your pull requests or create issues with found bugs and suggestions.
 In your pull requests please use Black formatting.
 
+## Donation
+If you feel like you can send any amount of WAX to the WAX address 24.gm
+
```

