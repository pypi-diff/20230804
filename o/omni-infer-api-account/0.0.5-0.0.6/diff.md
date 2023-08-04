# Comparing `tmp/omni_infer_api_account-0.0.5-py3-none-any.whl.zip` & `tmp/omni_infer_api_account-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 8763 bytes, number of entries: 10
+Zip file size: 8801 bytes, number of entries: 10
 -rw-rw-rw-  2.0 fat       81 b- defN 23-Aug-01 13:09 omniinfer_account/__init__.py
 -rw-rw-rw-  2.0 fat    14213 b- defN 23-Aug-04 09:54 omniinfer_account/account.py
 -rw-rw-rw-  2.0 fat      365 b- defN 23-Aug-02 11:58 omniinfer_account/config.py
 -rw-rw-rw-  2.0 fat     3310 b- defN 23-Aug-04 09:47 omniinfer_account/data.py
 -rw-rw-rw-  2.0 fat      184 b- defN 23-Jul-31 09:25 omniinfer_account/error.py
--rw-rw-rw-  2.0 fat    14928 b- defN 23-Aug-03 11:30 omniinfer_account/system.py
--rw-rw-rw-  2.0 fat      239 b- defN 23-Aug-04 09:54 omni_infer_api_account-0.0.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-04 09:54 omni_infer_api_account-0.0.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       18 b- defN 23-Aug-04 09:54 omni_infer_api_account-0.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      859 b- defN 23-Aug-04 09:54 omni_infer_api_account-0.0.5.dist-info/RECORD
-10 files, 34289 bytes uncompressed, 7281 bytes compressed:  78.8%
+-rw-rw-rw-  2.0 fat    15110 b- defN 23-Aug-04 10:07 omniinfer_account/system.py
+-rw-rw-rw-  2.0 fat      239 b- defN 23-Aug-04 10:07 omni_infer_api_account-0.0.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-04 10:07 omni_infer_api_account-0.0.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       18 b- defN 23-Aug-04 10:07 omni_infer_api_account-0.0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      859 b- defN 23-Aug-04 10:07 omni_infer_api_account-0.0.6.dist-info/RECORD
+10 files, 34471 bytes uncompressed, 7319 bytes compressed:  78.8%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: omniinfer_account/error.py
 Comment: 
 
 Filename: omniinfer_account/system.py
 Comment: 
 
-Filename: omni_infer_api_account-0.0.5.dist-info/METADATA
+Filename: omni_infer_api_account-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: omni_infer_api_account-0.0.5.dist-info/WHEEL
+Filename: omni_infer_api_account-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: omni_infer_api_account-0.0.5.dist-info/top_level.txt
+Filename: omni_infer_api_account-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: omni_infer_api_account-0.0.5.dist-info/RECORD
+Filename: omni_infer_api_account-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## omniinfer_account/system.py

```diff
@@ -178,15 +178,18 @@
         self.account_list[str(account_id)] = account(account_id)
         logging.info("CreateAccount: {} created".format(str(account_id)))
         return {"code": 0, "msg": ""}
 
     def set(self, account_id: int, mode: str, key: str, value):
         try:
             self.account_list[str(account_id)].set(mode, key, value)
-            logging.info("Set: {} set {}.{} as {}".format(str(account_id), mode, key, str(value)))
+            if key != "init_image" and key != "controlnet_input_image":
+                logging.info("Set: {} set {}.{} as {}".format(str(account_id), mode, key, str(value)))
+            else:
+                logging.info("Set: {} set {}.{}".format(str(account_id), mode, key))
             return {"code": 0, "msg": ""}
         except KeyError:
             logging.warning("Set: Unknown account id {}".format(str(account_id)))
             return {"code": 1, "msg": "Unknown account id {}".format(str(account_id))}
         except OmniInferAccountError as e:
             logging.warning("Set: {}".format(str(e)))
             return {"code": 1, "msg": str(e)}
```

## Comparing `omni_infer_api_account-0.0.5.dist-info/RECORD` & `omni_infer_api_account-0.0.6.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 omniinfer_account/__init__.py,sha256=8xVBC5zKvhEXnKS-yvAICUvJoUgdJbScMAuK4SDlYJ8,81
 omniinfer_account/account.py,sha256=ZihteRhLmCwsphI2clhF78m2u26yyx0w0f9WJvhWs-Q,14213
 omniinfer_account/config.py,sha256=XBxhdj5B8-TxcaZhUdAe3xu8Ruxzb64O20WE_kZKupw,365
 omniinfer_account/data.py,sha256=oDdzps3N4hCSICb11tzC6ToDsJ3VlRm04bvWVYdwI48,3310
 omniinfer_account/error.py,sha256=SN5KyCv7ekz0aatzSMfq5tF60SEUckt2-7uyyl4VdW0,184
-omniinfer_account/system.py,sha256=D903vptUKvCRObWcn_pabF1VQVH-5knzQbMKtDWm2jM,14928
-omni_infer_api_account-0.0.5.dist-info/METADATA,sha256=L0z6ado86BE59U3Izv6Rt1hrkGJTG_J-Rs1RWOB0ocY,239
-omni_infer_api_account-0.0.5.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-omni_infer_api_account-0.0.5.dist-info/top_level.txt,sha256=VYfZEk7HEk2argDpUHIImB1bxq7PaIdrKN9yKXDTOVQ,18
-omni_infer_api_account-0.0.5.dist-info/RECORD,,
+omniinfer_account/system.py,sha256=VNGXCqgvhHzkO19svQVUATQDlldb1R1F4gnw4WpQx44,15110
+omni_infer_api_account-0.0.6.dist-info/METADATA,sha256=CS4dWBJgaJ7gVRsx3uqsIzae8xcWkTeOR4KBUf2BcSY,239
+omni_infer_api_account-0.0.6.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+omni_infer_api_account-0.0.6.dist-info/top_level.txt,sha256=VYfZEk7HEk2argDpUHIImB1bxq7PaIdrKN9yKXDTOVQ,18
+omni_infer_api_account-0.0.6.dist-info/RECORD,,
```

