# Comparing `tmp/alfreds-0.0.2-py3-none-any.whl.zip` & `tmp/alfreds-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 6912 bytes, number of entries: 17
--rwxr-xr-x  2.0 unx     2291 b- defN 23-Aug-04 11:55 alfreds-0.0.2.data/scripts/alfreds
--rwxr-xr-x  2.0 unx       14 b- defN 23-Aug-03 10:35 alfreds-0.0.2.data/scripts/main.py
+Zip file size: 6917 bytes, number of entries: 17
+-rwxr-xr-x  2.0 unx     2291 b- defN 23-Aug-04 11:58 alfreds-0.0.3.data/scripts/alfreds
+-rwxr-xr-x  2.0 unx       14 b- defN 23-Aug-03 10:35 alfreds-0.0.3.data/scripts/main.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Aug-04 11:07 alfreds_init/__init__.py
--rw-r--r--  2.0 unx     5226 b- defN 23-Aug-04 11:07 alfreds_init/init.py
+-rw-r--r--  2.0 unx     5261 b- defN 23-Aug-04 11:58 alfreds_init/init.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Aug-04 11:07 alfreds_seed/__init__.py
 -rw-r--r--  2.0 unx      889 b- defN 23-Aug-04 11:07 alfreds_seed/seed.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Aug-04 11:07 alfreds_start/__init__.py
 -rw-r--r--  2.0 unx      769 b- defN 23-Aug-04 11:07 alfreds_start/start.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Aug-04 11:07 alfreds_stop/__init__.py
 -rw-r--r--  2.0 unx      139 b- defN 23-Aug-04 11:07 alfreds_stop/stop.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Aug-04 11:07 alfreds_update/__init__.py
 -rw-r--r--  2.0 unx     1022 b- defN 23-Aug-04 11:07 alfreds_update/update_agent.py
 -rw-r--r--  2.0 unx      990 b- defN 23-Aug-04 11:07 alfreds_update/update_working_directory.py
--rw-r--r--  2.0 unx      486 b- defN 23-Aug-04 11:55 alfreds-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Aug-04 11:55 alfreds-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       68 b- defN 23-Aug-04 11:55 alfreds-0.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1362 b- defN 23-Aug-04 11:55 alfreds-0.0.2.dist-info/RECORD
-17 files, 13348 bytes uncompressed, 4652 bytes compressed:  65.1%
+-rw-r--r--  2.0 unx      486 b- defN 23-Aug-04 11:58 alfreds-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-04 11:58 alfreds-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       68 b- defN 23-Aug-04 11:58 alfreds-0.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1362 b- defN 23-Aug-04 11:58 alfreds-0.0.3.dist-info/RECORD
+17 files, 13383 bytes uncompressed, 4657 bytes compressed:  65.2%
```

## zipnote {}

```diff
@@ -1,11 +1,11 @@
-Filename: alfreds-0.0.2.data/scripts/alfreds
+Filename: alfreds-0.0.3.data/scripts/alfreds
 Comment: 
 
-Filename: alfreds-0.0.2.data/scripts/main.py
+Filename: alfreds-0.0.3.data/scripts/main.py
 Comment: 
 
 Filename: alfreds_init/__init__.py
 Comment: 
 
 Filename: alfreds_init/init.py
 Comment: 
@@ -33,20 +33,20 @@
 
 Filename: alfreds_update/update_agent.py
 Comment: 
 
 Filename: alfreds_update/update_working_directory.py
 Comment: 
 
-Filename: alfreds-0.0.2.dist-info/METADATA
+Filename: alfreds-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: alfreds-0.0.2.dist-info/WHEEL
+Filename: alfreds-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: alfreds-0.0.2.dist-info/top_level.txt
+Filename: alfreds-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: alfreds-0.0.2.dist-info/RECORD
+Filename: alfreds-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## alfreds_init/init.py

```diff
@@ -121,14 +121,16 @@
             wait_for_backend_and_load(seed_directory_path, sync_seed_data)
 
     print("Running alfreds-ui image...")
     if not run_container("datafacade/alfred-ui", "alfred-ui", 5173):
         print("Failed to run alfreds-ui.")
         return
 
+    print("Alfreds UI is ready.")
+
 
 def load_agents(agent_dir):
     response = requests.post("http://localhost:3737/agent?agent_config_path=" + agent_dir)
     if response.status_code != 200:
         print("Failed to load agent.")
         print(response.text)
         return
```

## Comparing `alfreds-0.0.2.data/scripts/alfreds` & `alfreds-0.0.3.data/scripts/alfreds`

 * *Files identical despite different names*

## Comparing `alfreds-0.0.2.dist-info/RECORD` & `alfreds-0.0.3.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-alfreds-0.0.2.data/scripts/alfreds,sha256=w93pIoyhNdyhAB80yxRPfI5hyxk_rSDcWdAxyebaiMA,2291
-alfreds-0.0.2.data/scripts/main.py,sha256=lX4TwHMuSP1Ulvk1iU3JOp2n3NXrj_6lJkb98XjNodE,14
+alfreds-0.0.3.data/scripts/alfreds,sha256=w93pIoyhNdyhAB80yxRPfI5hyxk_rSDcWdAxyebaiMA,2291
+alfreds-0.0.3.data/scripts/main.py,sha256=lX4TwHMuSP1Ulvk1iU3JOp2n3NXrj_6lJkb98XjNodE,14
 alfreds_init/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-alfreds_init/init.py,sha256=WYG8iTIoOW-2PJKV-ZSHbe-1ASVzLLDn1V-DVkK5XHs,5226
+alfreds_init/init.py,sha256=uokCz1z50cAL2tUEd4hmwl9vwdXn8Err4AqyMBxCMrk,5261
 alfreds_seed/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 alfreds_seed/seed.py,sha256=FLqIgMCJWW8cb6KB7dtstioRW8wdzgKMq_wXiwbO5q4,889
 alfreds_start/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 alfreds_start/start.py,sha256=7pbd2P5E9_bOKKsshR45-yrvkCoZJakV9C7qqw-QCj8,769
 alfreds_stop/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 alfreds_stop/stop.py,sha256=T3klfHF8boqT4HpW_7ARtAg8Lql4GgZaK6O4Cm_8OAs,139
 alfreds_update/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 alfreds_update/update_agent.py,sha256=D3-8uk_cKXmiCAFmd-2ib0n8YwmUSOvxgxqCUrWxXQA,1022
 alfreds_update/update_working_directory.py,sha256=IXQp4NYh-IGsgC2Hnl9mbOFPXhtnOJX1hqfO5Ta6iEo,990
-alfreds-0.0.2.dist-info/METADATA,sha256=xCwHnJBR-KwjEsj5f9yKu2V7Rg1-Rwfia5k-L8ycY0A,486
-alfreds-0.0.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-alfreds-0.0.2.dist-info/top_level.txt,sha256=U8QlYE6eJZyrGAi6mUdY_XggkAM9FdCXhxxeeMemZUI,68
-alfreds-0.0.2.dist-info/RECORD,,
+alfreds-0.0.3.dist-info/METADATA,sha256=b2Jcmr1u8I1OPIIgZHpxPeJEX7KZ_QdUxh5SxdPypcg,486
+alfreds-0.0.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+alfreds-0.0.3.dist-info/top_level.txt,sha256=U8QlYE6eJZyrGAi6mUdY_XggkAM9FdCXhxxeeMemZUI,68
+alfreds-0.0.3.dist-info/RECORD,,
```

