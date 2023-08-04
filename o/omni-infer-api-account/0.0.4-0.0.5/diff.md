# Comparing `tmp/omni_infer_api_account-0.0.4-py3-none-any.whl.zip` & `tmp/omni_infer_api_account-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 8740 bytes, number of entries: 10
+Zip file size: 8763 bytes, number of entries: 10
 -rw-rw-rw-  2.0 fat       81 b- defN 23-Aug-01 13:09 omniinfer_account/__init__.py
--rw-rw-rw-  2.0 fat    14121 b- defN 23-Aug-04 04:22 omniinfer_account/account.py
+-rw-rw-rw-  2.0 fat    14213 b- defN 23-Aug-04 09:54 omniinfer_account/account.py
 -rw-rw-rw-  2.0 fat      365 b- defN 23-Aug-02 11:58 omniinfer_account/config.py
--rw-rw-rw-  2.0 fat     3266 b- defN 23-Aug-01 08:30 omniinfer_account/data.py
+-rw-rw-rw-  2.0 fat     3310 b- defN 23-Aug-04 09:47 omniinfer_account/data.py
 -rw-rw-rw-  2.0 fat      184 b- defN 23-Jul-31 09:25 omniinfer_account/error.py
 -rw-rw-rw-  2.0 fat    14928 b- defN 23-Aug-03 11:30 omniinfer_account/system.py
--rw-rw-rw-  2.0 fat      239 b- defN 23-Aug-04 04:42 omni_infer_api_account-0.0.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-04 04:42 omni_infer_api_account-0.0.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       18 b- defN 23-Aug-04 04:42 omni_infer_api_account-0.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      859 b- defN 23-Aug-04 04:42 omni_infer_api_account-0.0.4.dist-info/RECORD
-10 files, 34153 bytes uncompressed, 7258 bytes compressed:  78.7%
+-rw-rw-rw-  2.0 fat      239 b- defN 23-Aug-04 09:54 omni_infer_api_account-0.0.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-04 09:54 omni_infer_api_account-0.0.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       18 b- defN 23-Aug-04 09:54 omni_infer_api_account-0.0.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      859 b- defN 23-Aug-04 09:54 omni_infer_api_account-0.0.5.dist-info/RECORD
+10 files, 34289 bytes uncompressed, 7281 bytes compressed:  78.8%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: omniinfer_account/error.py
 Comment: 
 
 Filename: omniinfer_account/system.py
 Comment: 
 
-Filename: omni_infer_api_account-0.0.4.dist-info/METADATA
+Filename: omni_infer_api_account-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: omni_infer_api_account-0.0.4.dist-info/WHEEL
+Filename: omni_infer_api_account-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: omni_infer_api_account-0.0.4.dist-info/top_level.txt
+Filename: omni_infer_api_account-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: omni_infer_api_account-0.0.4.dist-info/RECORD
+Filename: omni_infer_api_account-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## omniinfer_account/account.py

```diff
@@ -193,14 +193,15 @@
                 steps=self.t2i_data.steps,
                 cfg_scale=self.t2i_data.cfg_scale,
                 seed=self.t2i_data.seed,
                 height=self.t2i_data.height,
                 width=self.t2i_data.width,
                 restore_faces=self.t2i_data.restore_faces,
                 clip_skip=self.t2i_data.clip_skip,
+                sd_vae=self.t2i_data.sd_vae,
                 using_controlnet=self.t2i_data.using_controlnet,
                 controlnet_model=self.t2i_data.controlnet_model,
                 controlnet_module=self.t2i_data.controlnet_module,
                 controlnet_weight=self.t2i_data.controlnet_weight,
                 controlnet_input_image=self.t2i_data.controlnet_input_image,
                 control_mode=self.t2i_data.control_mode,
                 controlnet_mask=self.t2i_data.controlnet_mask,
@@ -249,14 +250,15 @@
                 cfg_scale=self.i2i_data.cfg_scale,
                 seed=self.i2i_data.seed,
                 height=self.i2i_data.height,
                 width=self.i2i_data.width,
                 denoising_strength=self.i2i_data.denoising_strength,
                 restore_faces=self.i2i_data.restore_faces,
                 clip_skip=self.i2i_data.clip_skip,
+                sd_vae=self.i2i_data.sd_vae,
                 api_key=self.self_api_key if self.using_self_api_key else ""
             )
             if not self.using_self_api_key:
                 self.remain_credit -= cost
                 self.used_credit += cost
             return task_id
         except omniifer_api.OMNI_INFER_API_ERROR as e:
```

## omniinfer_account/data.py

```diff
@@ -13,14 +13,15 @@
     steps: int = 20
     cfg_scale: int = 7
     seed: int = -1
     height: int = 512
     width: int = 512
     restore_faces: bool = False
     clip_skip: int = 2
+    sd_vae: str = ""
     using_controlnet: bool = False
     controlnet_model: str = "control_v11p_sd15_openpose"
     controlnet_module: str = "none"
     controlnet_weight: float = 1.0
     controlnet_input_image: str = ""
     control_mode: int = 0
     controlnet_mask: int = -1
@@ -53,14 +54,15 @@
     cfg_scale: int = 7
     seed: int = -1
     height: int = 512
     width: int = 512
     denoising_strength: float = 0.75
     restore_faces: bool = False
     clip_skip: int = 2
+    sd_vae: str = ""
 
     def __getitem__(self, key):
         return getattr(self, key)
 
     def __setitem__(self, key, value):
         setattr(self, key, value)
```

## Comparing `omni_infer_api_account-0.0.4.dist-info/RECORD` & `omni_infer_api_account-0.0.5.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 omniinfer_account/__init__.py,sha256=8xVBC5zKvhEXnKS-yvAICUvJoUgdJbScMAuK4SDlYJ8,81
-omniinfer_account/account.py,sha256=jsbLZABFu1mF6nG4KSGq0sWVLvY082G5izQiHSqvwX0,14121
+omniinfer_account/account.py,sha256=ZihteRhLmCwsphI2clhF78m2u26yyx0w0f9WJvhWs-Q,14213
 omniinfer_account/config.py,sha256=XBxhdj5B8-TxcaZhUdAe3xu8Ruxzb64O20WE_kZKupw,365
-omniinfer_account/data.py,sha256=T4EJ3ltamEa4tOVPz9phVH0GD5DEQYNg9KVJdwv9-DI,3266
+omniinfer_account/data.py,sha256=oDdzps3N4hCSICb11tzC6ToDsJ3VlRm04bvWVYdwI48,3310
 omniinfer_account/error.py,sha256=SN5KyCv7ekz0aatzSMfq5tF60SEUckt2-7uyyl4VdW0,184
 omniinfer_account/system.py,sha256=D903vptUKvCRObWcn_pabF1VQVH-5knzQbMKtDWm2jM,14928
-omni_infer_api_account-0.0.4.dist-info/METADATA,sha256=S5HJMLyW9zYzquGmB44kbFqGt7uxuuGKVJ3cDI4kB68,239
-omni_infer_api_account-0.0.4.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-omni_infer_api_account-0.0.4.dist-info/top_level.txt,sha256=VYfZEk7HEk2argDpUHIImB1bxq7PaIdrKN9yKXDTOVQ,18
-omni_infer_api_account-0.0.4.dist-info/RECORD,,
+omni_infer_api_account-0.0.5.dist-info/METADATA,sha256=L0z6ado86BE59U3Izv6Rt1hrkGJTG_J-Rs1RWOB0ocY,239
+omni_infer_api_account-0.0.5.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+omni_infer_api_account-0.0.5.dist-info/top_level.txt,sha256=VYfZEk7HEk2argDpUHIImB1bxq7PaIdrKN9yKXDTOVQ,18
+omni_infer_api_account-0.0.5.dist-info/RECORD,,
```

