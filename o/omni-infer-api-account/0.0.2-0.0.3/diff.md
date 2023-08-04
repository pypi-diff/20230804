# Comparing `tmp/omni_infer_api_account-0.0.2-py3-none-any.whl.zip` & `tmp/omni_infer_api_account-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 8701 bytes, number of entries: 10
+Zip file size: 8739 bytes, number of entries: 10
 -rw-rw-rw-  2.0 fat       81 b- defN 23-Aug-01 13:09 omniinfer_account/__init__.py
--rw-rw-rw-  2.0 fat    14108 b- defN 23-Aug-02 11:51 omniinfer_account/account.py
+-rw-rw-rw-  2.0 fat    14109 b- defN 23-Aug-03 11:30 omniinfer_account/account.py
 -rw-rw-rw-  2.0 fat      365 b- defN 23-Aug-02 11:58 omniinfer_account/config.py
 -rw-rw-rw-  2.0 fat     3266 b- defN 23-Aug-01 08:30 omniinfer_account/data.py
 -rw-rw-rw-  2.0 fat      184 b- defN 23-Jul-31 09:25 omniinfer_account/error.py
--rw-rw-rw-  2.0 fat    14803 b- defN 23-Aug-02 12:50 omniinfer_account/system.py
--rw-rw-rw-  2.0 fat      239 b- defN 23-Aug-02 13:29 omni_infer_api_account-0.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-02 13:29 omni_infer_api_account-0.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       18 b- defN 23-Aug-02 13:29 omni_infer_api_account-0.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      859 b- defN 23-Aug-02 13:29 omni_infer_api_account-0.0.2.dist-info/RECORD
-10 files, 34015 bytes uncompressed, 7219 bytes compressed:  78.8%
+-rw-rw-rw-  2.0 fat    14928 b- defN 23-Aug-03 11:30 omniinfer_account/system.py
+-rw-rw-rw-  2.0 fat      239 b- defN 23-Aug-03 11:30 omni_infer_api_account-0.0.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-03 11:30 omni_infer_api_account-0.0.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       18 b- defN 23-Aug-03 11:30 omni_infer_api_account-0.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      859 b- defN 23-Aug-03 11:30 omni_infer_api_account-0.0.3.dist-info/RECORD
+10 files, 34141 bytes uncompressed, 7257 bytes compressed:  78.7%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: omniinfer_account/error.py
 Comment: 
 
 Filename: omniinfer_account/system.py
 Comment: 
 
-Filename: omni_infer_api_account-0.0.2.dist-info/METADATA
+Filename: omni_infer_api_account-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: omni_infer_api_account-0.0.2.dist-info/WHEEL
+Filename: omni_infer_api_account-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: omni_infer_api_account-0.0.2.dist-info/top_level.txt
+Filename: omni_infer_api_account-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: omni_infer_api_account-0.0.2.dist-info/RECORD
+Filename: omni_infer_api_account-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## omniinfer_account/account.py

```diff
@@ -100,15 +100,15 @@
             raise error.OmniInferAccountError("Key " + key + " is not str or be null")
         elif (key == "batch_size" or key == "n_iter") and (not isinstance(value, int) or not 1 <= value <= 8):
             raise error.OmniInferAccountError("Key " + key + " is not int or out of range")
         elif key == "steps" and (not isinstance(value, int) or not 1 <= value <= 50):
             raise error.OmniInferAccountError("Key steps is not int or out of range")
         elif key == "cfg_scale" and (not isinstance(value, int) or not 0 <= value <= 30):
             raise error.OmniInferAccountError("Key cfg_scale is not int or out of range")
-        elif key == "seed" and (not isinstance(value, int) or not -1 <= value <= 2 ^ 32):
+        elif key == "seed" and (not isinstance(value, int) or not -1 <= value <= 2 ** 32):
             raise error.OmniInferAccountError("Key seed is not int or out of range")
         elif (key == "width" or key == "height") and (not isinstance(value, int) or not 1 <= value <= 2048
                                                       or not value % 8 == 0):
             raise error.OmniInferAccountError("Key " + key + " is not int or out of range")
         elif (key == "restore_faces" or key == "using_controlnet" or key == "controlnet_lowvram"
               or key == "controlnet_pixel_perfect") and not isinstance(value, bool):
             raise error.OmniInferAccountError("Key " + key + " is not bool")
```

## omniinfer_account/system.py

```diff
@@ -152,15 +152,16 @@
         try:
             result = self.account_list[str(account_id)].last_result
             if self.account_list[str(account_id)].status == 0:
                 self.account_list[str(account_id)].last_result = {}
                 if result is None:
                     return {"code": 1, "msg": "No task"}
                 if result["status"] == 2:
-                    return {"code": 0, "msg": "", "imgs": result["imgs"], "seed": json.loads(result["info"])}
+                    return {"code": 0, "msg": "", "imgs": result["imgs"], "seed": json.loads(result["info"])["seed"]
+                            , "time": result["debug_info"]["submit_time_ms"] - result["debug_info"]["finish_time_ms"]}
                 elif result["status"] == 2 or result["status"] == 3:
                     return {"code": 1, "msg": result["failed reason"]}
                 else:
                     return {"code": 1, "msg": "UnException status"}
             elif self.account_list[str(account_id)].status == 1:
                 return {"code": 2, "msg": "Waiting in queue."}
             elif self.account_list[str(account_id)].status == 2:
@@ -312,8 +313,7 @@
             return {"code": 0, "msg": ""}
         except KeyError:
             logging.warning("AddN: Unknown account {}".format(str(account_id)))
             return {"code": 1, "msg": "Unknown account id"}
         except OmniInferAccountError as e:
             logging.warning("AddN: " + str(e))
             return {"code": 1, "msg": str(e)}
-
```

