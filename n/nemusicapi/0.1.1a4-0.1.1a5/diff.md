# Comparing `tmp/nemusicapi-0.1.1a4.tar.gz` & `tmp/nemusicapi-0.1.1a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nemusicapi-0.1.1a4.tar", max compression
+gzip compressed data, was "nemusicapi-0.1.1a5.tar", max compression
```

## Comparing `nemusicapi-0.1.1a4.tar` & `nemusicapi-0.1.1a5.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0    11558 2023-08-01 07:21:02.527622 nemusicapi-0.1.1a4/LICENSE
--rw-r--r--   0        0        0      311 2023-08-03 09:11:40.318932 nemusicapi-0.1.1a4/nemusicapi/__init__.py
--rw-r--r--   0        0        0     4958 2023-08-03 11:17:30.186582 nemusicapi-0.1.1a4/nemusicapi/api.py
--rw-r--r--   0        0        0      113 2023-08-03 06:48:17.625541 nemusicapi-0.1.1a4/nemusicapi/exception.py
--rw-r--r--   0        0        0      363 2023-08-03 11:15:34.699086 nemusicapi-0.1.1a4/nemusicapi/type.py
--rw-r--r--   0        0        0      466 2023-08-03 11:17:10.491986 nemusicapi-0.1.1a4/pyproject.toml
--rw-r--r--   0        0        0     1291 2023-08-03 11:15:05.073832 nemusicapi-0.1.1a4/README.md
--rw-r--r--   0        0        0     1912 1970-01-01 00:00:00.000000 nemusicapi-0.1.1a4/PKG-INFO
+-rw-r--r--   0        0        0    11558 2023-08-01 07:21:02.527622 nemusicapi-0.1.1a5/LICENSE
+-rw-r--r--   0        0        0      372 2023-08-04 04:15:15.239106 nemusicapi-0.1.1a5/nemusicapi/__init__.py
+-rw-r--r--   0        0        0     1828 2023-08-04 04:14:01.769971 nemusicapi-0.1.1a5/nemusicapi/api.py
+-rw-r--r--   0        0        0     3244 2023-08-04 04:13:14.028049 nemusicapi-0.1.1a5/nemusicapi/base_api.py
+-rw-r--r--   0        0        0      113 2023-08-03 06:48:17.625541 nemusicapi-0.1.1a5/nemusicapi/exception.py
+-rw-r--r--   0        0        0      363 2023-08-03 11:15:34.699086 nemusicapi-0.1.1a5/nemusicapi/type.py
+-rw-r--r--   0        0        0      466 2023-08-04 04:16:10.930270 nemusicapi-0.1.1a5/pyproject.toml
+-rw-r--r--   0        0        0     1291 2023-08-04 04:08:02.476322 nemusicapi-0.1.1a5/README.md
+-rw-r--r--   0        0        0     1912 1970-01-01 00:00:00.000000 nemusicapi-0.1.1a5/PKG-INFO
```

### Comparing `nemusicapi-0.1.1a4/LICENSE` & `nemusicapi-0.1.1a5/LICENSE`

 * *Files identical despite different names*

### Comparing `nemusicapi-0.1.1a4/nemusicapi/api.py` & `nemusicapi-0.1.1a5/nemusicapi/base_api.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,18 @@
-import json
-import os
 import random
 import base64
 import codecs
+import json
 
 import requests
 from Crypto.Cipher import AES
-import urllib3
 
-from nemusicapi.exception import NoDownloadDirException
 from nemusicapi.type import QualityLevel, EncodeType
 
 
-urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
-
-
 def aes_encrypt(raw_text: str, raw_key: str):
     key = raw_key.encode('utf-8')  # 将密钥转换为utf-8格式
     iv = '0102030405060708'.encode('utf-8')  # iv偏移量
     encryptor = AES.new(key, AES.MODE_CBC, iv)  # 创建一个AES对象
     _text = raw_text.encode('utf-8')  # 将明文转换为utf-8格式
     pad = 16 - len(_text) % 16
     text = _text + (pad * chr(pad)).encode('utf-8')  # 明文需要转成二进制，且可以被16整除
@@ -38,15 +32,15 @@
     random_str = ''.join(random.sample('abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789', 16))
     encText = aes_encrypt(raw_params, '0CoJUm6Qyw8W8jud')
     params = aes_encrypt(encText, random_str)
     encSecKey = rsa_encrypt(random_str, '010001', '00e0b509f6259df8642dbc35662901477df22677ec152b5ff68ace615bb7b725152b3ab17a876aea8a5aa76d2e417629ec4ee341f56135fccf695280104e0312ecbda92557c93870114af6c9d05c4f7f0c3685b7a46bee255932575cce10b424d813cfe4875d3e82047b97ddef52741d546b8e289dc6935b3ece0462db0a22b8e7')  # RSA加密后获得encSecKey
     return params, encSecKey
 
 
-class RawApi:
+class BaseApi:
     def __init__(self, *,
                  cookie=''
                  ):
         self.cookie = cookie
 
 
     def _get_data(self, url: str, raw_params) -> dict:
@@ -81,53 +75,8 @@
         url = f'https://music.163.com/weapi/song/enhance/player/url/v1'
         params = {
             'ids': '["' + str(song_id) + '"]',
             'level': level.value,
             'encodeType': encodeType.value
         }
         res = self._get_data(url, params)
-        return res
-
-
-class Api(RawApi):
-    def __init__(self, *, 
-                 cookie='',
-                 download_dir=None
-                 ):
-        super().__init__(cookie=cookie)
-        self.download_dir = download_dir
-        
-        if download_dir:
-            if not os.path.exists(download_dir):
-                os.makedirs(download_dir)
-
-
-    def get_song_data(self, raw_song_name: str) -> tuple[int, str] | None:
-        res = self.search_music(raw_song_name)
-        if res['result']['songCount'] == 0:
-            return
-        song_id = res['result']['songs'][0]['id']
-        song_name = res['result']['songs'][0]['name']
-        return song_id, song_name
-
-
-    def get_song_download_data(self, song_id: int, *,
-                               level=QualityLevel.standard,
-                               encodeType=EncodeType.flac
-                               ) -> tuple[str, EncodeType] | None:
-        res = self.get_song_file_data(song_id, level=level, encodeType=encodeType)
-        if res['data'][0]['url'] is None:
-            return
-        song_url = res['data'][0]['url']
-        song_type = res['data'][0]['type']
-        return song_url, EncodeType(song_type)
-
-
-    def download_song(self, song_url: str, file_name: str):
-        if self.download_dir == None:
-            raise NoDownloadDirException
-        
-        file_path = os.path.join(self.download_dir, file_name)
-        
-        with open(file_path, 'wb') as f:
-            f.write(requests.get(song_url).content)
-        return True
+        return res
```

### Comparing `nemusicapi-0.1.1a4/README.md` & `nemusicapi-0.1.1a5/README.md`

 * *Files identical despite different names*

### Comparing `nemusicapi-0.1.1a4/PKG-INFO` & `nemusicapi-0.1.1a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nemusicapi
-Version: 0.1.1a4
+Version: 0.1.1a5
 Summary: A Netsase music api
 Home-page: https://github.com/yuyi2439/NeteaseMusicApi
 License: Apache-2.0
 Author: yuyi2439
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

