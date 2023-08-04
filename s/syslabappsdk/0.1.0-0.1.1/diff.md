# Comparing `tmp/syslabappsdk-0.1.0.tar.gz` & `tmp/syslabappsdk-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syslabappsdk-0.1.0.tar", last modified: Tue Jun 20 03:07:50 2023, max compression
+gzip compressed data, was "syslabappsdk-0.1.1.tar", last modified: Fri Aug  4 07:10:38 2023, max compression
```

## Comparing `syslabappsdk-0.1.0.tar` & `syslabappsdk-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 03:07:50.561140 syslabappsdk-0.1.0/
--rw-rw-rw-   0        0        0     1123 2023-06-13 11:46:07.000000 syslabappsdk-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     4871 2023-06-20 03:07:50.560141 syslabappsdk-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2665 2023-06-19 05:45:00.000000 syslabappsdk-0.1.0/README.md
--rw-rw-rw-   0        0        0      923 2023-06-20 02:35:44.000000 syslabappsdk-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-20 03:07:50.561140 syslabappsdk-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-20 03:07:50.545131 syslabappsdk-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-20 03:07:50.557141 syslabappsdk-0.1.0/src/py_syslab_app_sdk/
--rw-rw-rw-   0        0        0       91 2023-04-13 08:12:57.000000 syslabappsdk-0.1.0/src/py_syslab_app_sdk/__init__.py
--rw-rw-rw-   0        0        0     2991 2023-05-31 04:57:25.000000 syslabappsdk-0.1.0/src/py_syslab_app_sdk/connect_client.py
--rw-rw-rw-   0        0        0     7905 2023-06-12 07:47:28.000000 syslabappsdk-0.1.0/src/py_syslab_app_sdk/syslab_app_sdk.py
--rw-rw-rw-   0        0        0      230 2023-05-16 07:49:12.000000 syslabappsdk-0.1.0/src/py_syslab_app_sdk/variable_info.py
-drwxrwxrwx   0        0        0        0 2023-06-20 03:07:50.560141 syslabappsdk-0.1.0/src/syslabappsdk.egg-info/
--rw-rw-rw-   0        0        0     4871 2023-06-20 03:07:50.000000 syslabappsdk-0.1.0/src/syslabappsdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      345 2023-06-20 03:07:50.000000 syslabappsdk-0.1.0/src/syslabappsdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 03:07:50.000000 syslabappsdk-0.1.0/src/syslabappsdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-06-20 03:07:50.000000 syslabappsdk-0.1.0/src/syslabappsdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-04 07:10:38.648393 syslabappsdk-0.1.1/
+-rw-rw-rw-   0        0        0     1123 2023-06-13 11:46:07.000000 syslabappsdk-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     4871 2023-08-04 07:10:38.647397 syslabappsdk-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2665 2023-06-19 05:45:00.000000 syslabappsdk-0.1.1/README.md
+-rw-rw-rw-   0        0        0      923 2023-08-04 06:49:35.000000 syslabappsdk-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-04 07:10:38.648393 syslabappsdk-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-04 07:10:38.631456 syslabappsdk-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-08-04 07:10:38.643410 syslabappsdk-0.1.1/src/py_syslab_app_sdk/
+-rw-rw-rw-   0        0        0       91 2023-04-13 08:12:57.000000 syslabappsdk-0.1.1/src/py_syslab_app_sdk/__init__.py
+-rw-rw-rw-   0        0        0     2991 2023-05-31 04:57:25.000000 syslabappsdk-0.1.1/src/py_syslab_app_sdk/connect_client.py
+-rw-rw-rw-   0        0        0     7975 2023-08-04 06:30:43.000000 syslabappsdk-0.1.1/src/py_syslab_app_sdk/syslab_app_sdk.py
+-rw-rw-rw-   0        0        0      230 2023-05-16 07:49:12.000000 syslabappsdk-0.1.1/src/py_syslab_app_sdk/variable_info.py
+drwxrwxrwx   0        0        0        0 2023-08-04 07:10:38.647397 syslabappsdk-0.1.1/src/syslabappsdk.egg-info/
+-rw-rw-rw-   0        0        0     4871 2023-08-04 07:10:38.000000 syslabappsdk-0.1.1/src/syslabappsdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      345 2023-08-04 07:10:38.000000 syslabappsdk-0.1.1/src/syslabappsdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 07:10:38.000000 syslabappsdk-0.1.1/src/syslabappsdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-08-04 07:10:38.000000 syslabappsdk-0.1.1/src/syslabappsdk.egg-info/top_level.txt
```

### Comparing `syslabappsdk-0.1.0/LICENSE` & `syslabappsdk-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `syslabappsdk-0.1.0/PKG-INFO` & `syslabappsdk-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syslabappsdk
-Version: 0.1.0
+Version: 0.1.1
 Summary: SDK for data interaction and function calls between Python APP and Syslab platform
 Author-email: Suzhou-tongyuan <support@tongyuan.cc>
 License: The MIT License (MIT)
         Copyright (c) 2023 Suzhou-Tongyuan (support@tongyuan.cc)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `syslabappsdk-0.1.0/README.md` & `syslabappsdk-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `syslabappsdk-0.1.0/pyproject.toml` & `syslabappsdk-0.1.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "syslabappsdk"
-version = "0.1.0"
+version = "0.1.1"
 description = "SDK for data interaction and function calls between Python APP and Syslab platform"
 authors = [
   { name="Suzhou-tongyuan", email="support@tongyuan.cc" },
 ]
 license = {file = "LICENSE"}
 readme = "README.md"
 requires-python = ">=3.7, <4"
```

### Comparing `syslabappsdk-0.1.0/src/py_syslab_app_sdk/connect_client.py` & `syslabappsdk-0.1.1/src/py_syslab_app_sdk/connect_client.py`

 * *Files identical despite different names*

### Comparing `syslabappsdk-0.1.0/src/py_syslab_app_sdk/syslab_app_sdk.py` & `syslabappsdk-0.1.1/src/py_syslab_app_sdk/syslab_app_sdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,24 +72,26 @@
         if self.__conn == None:
             return False
         return self.__conn.send_bytes(request.encode("utf-8"))
 
     def _consume_respond_msg(self):
         respond = ""
         respond_length = 0
+        byte_length = 0
         while True:
             temp_respond = self.__conn.recv_bytes()
+            byte_length += len(temp_respond)
             temp_respond = temp_respond.decode("utf-8")
             if temp_respond.find("Content-Length: ") == 0:
                 cl_str = "Content-Length: "
                 rn_place = temp_respond.find("\r\n")
                 sub_str = temp_respond[len(cl_str):rn_place]
                 respond_length = int(sub_str) + 4 + rn_place
             respond += temp_respond
-            if len(respond) >= respond_length:
+            if byte_length >= respond_length:
                 return respond
 
     def _unpack_json_get_variables(self, text, request_id):
         start_pos = text.find('{')
         if start_pos == -1:
             return False
```

### Comparing `syslabappsdk-0.1.0/src/syslabappsdk.egg-info/PKG-INFO` & `syslabappsdk-0.1.1/src/syslabappsdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syslabappsdk
-Version: 0.1.0
+Version: 0.1.1
 Summary: SDK for data interaction and function calls between Python APP and Syslab platform
 Author-email: Suzhou-tongyuan <support@tongyuan.cc>
 License: The MIT License (MIT)
         Copyright (c) 2023 Suzhou-Tongyuan (support@tongyuan.cc)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

