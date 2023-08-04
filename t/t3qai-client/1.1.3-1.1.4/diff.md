# Comparing `tmp/t3qai_client-1.1.3-py3-none-any.whl.zip` & `tmp/t3qai_client-1.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 15106 bytes, number of entries: 8
+Zip file size: 15017 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat     1639 b- defN 23-Aug-03 08:00 t3qai_client/__init__.py
--rw-rw-rw-  2.0 fat    23600 b- defN 23-Aug-03 08:00 t3qai_client/t3qai_helper.py
+-rw-rw-rw-  2.0 fat    23318 b- defN 23-Aug-04 08:20 t3qai_client/t3qai_helper.py
 -rw-rw-rw-  2.0 fat     6328 b- defN 23-Aug-03 08:00 t3qai_client/t3qai_serving.py
--rw-rw-rw-  2.0 fat    11533 b- defN 23-Aug-03 08:01 t3qai_client-1.1.3.dist-info/LICENSE-2.0.txt
--rw-rw-rw-  2.0 fat     2850 b- defN 23-Aug-03 08:01 t3qai_client-1.1.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-03 08:01 t3qai_client-1.1.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       13 b- defN 23-Aug-03 08:01 t3qai_client-1.1.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      673 b- defN 23-Aug-03 08:01 t3qai_client-1.1.3.dist-info/RECORD
-8 files, 46728 bytes uncompressed, 13930 bytes compressed:  70.2%
+-rw-rw-rw-  2.0 fat    11533 b- defN 23-Aug-04 08:20 t3qai_client-1.1.4.dist-info/LICENSE-2.0.txt
+-rw-rw-rw-  2.0 fat     2850 b- defN 23-Aug-04 08:20 t3qai_client-1.1.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-04 08:20 t3qai_client-1.1.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       13 b- defN 23-Aug-04 08:20 t3qai_client-1.1.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      673 b- defN 23-Aug-04 08:20 t3qai_client-1.1.4.dist-info/RECORD
+8 files, 46446 bytes uncompressed, 13841 bytes compressed:  70.2%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: t3qai_client/t3qai_helper.py
 Comment: 
 
 Filename: t3qai_client/t3qai_serving.py
 Comment: 
 
-Filename: t3qai_client-1.1.3.dist-info/LICENSE-2.0.txt
+Filename: t3qai_client-1.1.4.dist-info/LICENSE-2.0.txt
 Comment: 
 
-Filename: t3qai_client-1.1.3.dist-info/METADATA
+Filename: t3qai_client-1.1.4.dist-info/METADATA
 Comment: 
 
-Filename: t3qai_client-1.1.3.dist-info/WHEEL
+Filename: t3qai_client-1.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: t3qai_client-1.1.3.dist-info/top_level.txt
+Filename: t3qai_client-1.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: t3qai_client-1.1.3.dist-info/RECORD
+Filename: t3qai_client-1.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## t3qai_client/t3qai_helper.py

```diff
@@ -547,36 +547,29 @@
             _configure_logger(logger, train_log_path, log_filename=_log_filename, log_level=_log_level)
     
     
 def inference_set_logger():
     """
     Inference logger setup
     """
-    _log_filename = 'oper.log'
-    #_log_level = 'DEBUG'
-    _log_level = 'INFO'
+    _log_directory = 'logs'
+    _log_filename =  'oper.log'
+    _log_level = 'DEBUG'
     
     logger = logging.getLogger()
-    logger.setLevel(_log_level)
+    logger_path = inference_load_path().get("logger_path")
     
-    #logging.getLogger("werkzeug").setLevel(logging.WARNING)
-    logging.getLogger("werkzeug").setLevel(logging.INFO)
+    pathlib.Path(logger_path).mkdir(parents=True, exist_ok=True)
     
-    logger_path = inference_load_path().get("logger_path")
-    if logger_path and  os.path.exists(logger_path):
-        log_name = os.path.join(logger_path, _log_filename)
-        pathlib.Path(logger_path).mkdir(parents=True, exist_ok=True)
-        
-        #_add_console_handler(logger, log_level=_log_level)
-        
-        handler = RotatingFileHandler(log_name, mode="w", maxBytes=10 * 1024 * 1024, backupCount=10)
-        handler.setLevel(_log_level)
-        handler.setFormatter(logging.Formatter(LOG_FORMAT))
-        
-        logger.addHandler(handler)
+    if logger_path and os.path.exists(logger_path):
+        log_file_path = os.path.join(logger_path, _log_filename)
+        if os.path.exists(log_file_path):
+            os.remove(os.path.join(log_file_path))
+        _configure_logger(logger, logger_path, log_filename=_log_filename, log_level=_log_level)
+
 
 
 class DownloadFile():
     """
     Inference file obj setup
     """
     def __init__(self, file_name=None, file_obj=None, file_path=None):
```

## Comparing `t3qai_client-1.1.3.dist-info/LICENSE-2.0.txt` & `t3qai_client-1.1.4.dist-info/LICENSE-2.0.txt`

 * *Files identical despite different names*

## Comparing `t3qai_client-1.1.3.dist-info/METADATA` & `t3qai_client-1.1.4.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t3qai-client
-Version: 1.1.3
+Version: 1.1.4
 Summary: t3qai client module
 Home-page: UNKNOWN
 Author: t3q
 Author-email: lab@t3q.com
 License: UNKNOWN
 Keywords: t3q,t3qai,t3qai client,t3qai_client
 Platform: UNKNOWN
```

