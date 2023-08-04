# Comparing `tmp/nemusicapi-0.1.1a5.tar.gz` & `tmp/nemusicapi-0.1.1a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nemusicapi-0.1.1a5.tar", max compression
+gzip compressed data, was "nemusicapi-0.1.1a6.tar", max compression
```

## Comparing `nemusicapi-0.1.1a5.tar` & `nemusicapi-0.1.1a6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11558 2023-08-01 07:21:02.527622 nemusicapi-0.1.1a5/LICENSE
--rw-r--r--   0        0        0      372 2023-08-04 04:15:15.239106 nemusicapi-0.1.1a5/nemusicapi/__init__.py
--rw-r--r--   0        0        0     1828 2023-08-04 04:14:01.769971 nemusicapi-0.1.1a5/nemusicapi/api.py
--rw-r--r--   0        0        0     3244 2023-08-04 04:13:14.028049 nemusicapi-0.1.1a5/nemusicapi/base_api.py
--rw-r--r--   0        0        0      113 2023-08-03 06:48:17.625541 nemusicapi-0.1.1a5/nemusicapi/exception.py
--rw-r--r--   0        0        0      363 2023-08-03 11:15:34.699086 nemusicapi-0.1.1a5/nemusicapi/type.py
--rw-r--r--   0        0        0      466 2023-08-04 04:16:10.930270 nemusicapi-0.1.1a5/pyproject.toml
--rw-r--r--   0        0        0     1291 2023-08-04 04:08:02.476322 nemusicapi-0.1.1a5/README.md
--rw-r--r--   0        0        0     1912 1970-01-01 00:00:00.000000 nemusicapi-0.1.1a5/PKG-INFO
+-rw-r--r--   0        0        0    11558 2023-08-01 07:21:02.527622 nemusicapi-0.1.1a6/LICENSE
+-rw-r--r--   0        0        0      372 2023-08-04 04:41:37.772467 nemusicapi-0.1.1a6/nemusicapi/__init__.py
+-rw-r--r--   0        0        0     1921 2023-08-04 04:44:28.216009 nemusicapi-0.1.1a6/nemusicapi/api.py
+-rw-r--r--   0        0        0     3265 2023-08-04 04:38:15.035228 nemusicapi-0.1.1a6/nemusicapi/base_api.py
+-rw-r--r--   0        0        0      113 2023-08-03 06:48:17.625541 nemusicapi-0.1.1a6/nemusicapi/exception.py
+-rw-r--r--   0        0        0      363 2023-08-03 11:15:34.699086 nemusicapi-0.1.1a6/nemusicapi/type.py
+-rw-r--r--   0        0        0      466 2023-08-04 04:41:46.602723 nemusicapi-0.1.1a6/pyproject.toml
+-rw-r--r--   0        0        0     1291 2023-08-04 04:08:02.476322 nemusicapi-0.1.1a6/README.md
+-rw-r--r--   0        0        0     1912 1970-01-01 00:00:00.000000 nemusicapi-0.1.1a6/PKG-INFO
```

### Comparing `nemusicapi-0.1.1a5/LICENSE` & `nemusicapi-0.1.1a6/LICENSE`

 * *Files identical despite different names*

### Comparing `nemusicapi-0.1.1a5/nemusicapi/api.py` & `nemusicapi-0.1.1a6/nemusicapi/api.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 
 import requests
 import urllib3
 
-from nemusicapi.exception import NoDownloadDirException
 from nemusicapi.type import QualityLevel, EncodeType
 from nemusicapi.base_api import BaseApi
+from nemusicapi.exception import NoDownloadDirException
 
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
 
 class Api(BaseApi):
     def __init__(self, *, 
                  cookie='',
@@ -19,21 +19,24 @@
         self.download_dir = download_dir
         
         if download_dir:
             if not os.path.exists(download_dir):
                 os.makedirs(download_dir)
 
 
-    def get_song_data(self, raw_song_name: str) -> tuple[int, str] | None:
-        res = self.search_music(raw_song_name)
+    def get_song_data(self, raw_song_name: str, *, limit: int = 10) -> dict[int, str] | None:
+        res = self.search_music(raw_song_name, limit=limit)
         if res['result']['songCount'] == 0:
             return
-        song_id = res['result']['songs'][0]['id']
-        song_name = res['result']['songs'][0]['name']
-        return song_id, song_name
+        song_data = {}
+        for j in res['result']['songs']:
+            song_id = j['id']
+            song_name = j['name']
+            song_data[song_id] = song_name
+        return song_data
 
 
     def get_song_download_data(self, song_id: int, *,
                                level=QualityLevel.standard,
                                encodeType=EncodeType.flac
                                ) -> tuple[str, EncodeType] | None:
         res = self.get_song_file_data(song_id, level=level, encodeType=encodeType)
```

### Comparing `nemusicapi-0.1.1a5/nemusicapi/base_api.py` & `nemusicapi-0.1.1a6/nemusicapi/base_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import random
 import base64
 import codecs
 import json
 
 import requests
+import urllib3
 from Crypto.Cipher import AES
 
 from nemusicapi.type import QualityLevel, EncodeType
 
+urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
+
 
 def aes_encrypt(raw_text: str, raw_key: str):
-    key = raw_key.encode('utf-8')  # 将密钥转换为utf-8格式
+    key = raw_key.encode('utf-8')
+    _text = raw_text.encode('utf-8')
     iv = '0102030405060708'.encode('utf-8')  # iv偏移量
     encryptor = AES.new(key, AES.MODE_CBC, iv)  # 创建一个AES对象
-    _text = raw_text.encode('utf-8')  # 将明文转换为utf-8格式
     pad = 16 - len(_text) % 16
     text = _text + (pad * chr(pad)).encode('utf-8')  # 明文需要转成二进制，且可以被16整除
     _encrypt_text = encryptor.encrypt(text)  # 加密
     encrypt_text = base64.b64encode(_encrypt_text)  # base64编码转换为byte字符串
     return encrypt_text.decode('utf-8')
```

### Comparing `nemusicapi-0.1.1a5/README.md` & `nemusicapi-0.1.1a6/README.md`

 * *Files identical despite different names*

### Comparing `nemusicapi-0.1.1a5/PKG-INFO` & `nemusicapi-0.1.1a6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nemusicapi
-Version: 0.1.1a5
+Version: 0.1.1a6
 Summary: A Netsase music api
 Home-page: https://github.com/yuyi2439/NeteaseMusicApi
 License: Apache-2.0
 Author: yuyi2439
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

