# Comparing `tmp/nemusicapi-0.1.1a6.tar.gz` & `tmp/nemusicapi-0.1.1a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nemusicapi-0.1.1a6.tar", max compression
+gzip compressed data, was "nemusicapi-0.1.1a7.tar", max compression
```

## Comparing `nemusicapi-0.1.1a6.tar` & `nemusicapi-0.1.1a7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11558 2023-08-01 07:21:02.527622 nemusicapi-0.1.1a6/LICENSE
--rw-r--r--   0        0        0      372 2023-08-04 04:41:37.772467 nemusicapi-0.1.1a6/nemusicapi/__init__.py
--rw-r--r--   0        0        0     1921 2023-08-04 04:44:28.216009 nemusicapi-0.1.1a6/nemusicapi/api.py
--rw-r--r--   0        0        0     3265 2023-08-04 04:38:15.035228 nemusicapi-0.1.1a6/nemusicapi/base_api.py
--rw-r--r--   0        0        0      113 2023-08-03 06:48:17.625541 nemusicapi-0.1.1a6/nemusicapi/exception.py
--rw-r--r--   0        0        0      363 2023-08-03 11:15:34.699086 nemusicapi-0.1.1a6/nemusicapi/type.py
--rw-r--r--   0        0        0      466 2023-08-04 04:41:46.602723 nemusicapi-0.1.1a6/pyproject.toml
--rw-r--r--   0        0        0     1291 2023-08-04 04:08:02.476322 nemusicapi-0.1.1a6/README.md
--rw-r--r--   0        0        0     1912 1970-01-01 00:00:00.000000 nemusicapi-0.1.1a6/PKG-INFO
+-rw-r--r--   0        0        0    11558 2023-08-01 07:21:02.527622 nemusicapi-0.1.1a7/LICENSE
+-rw-r--r--   0        0        0      372 2023-08-04 04:41:37.772467 nemusicapi-0.1.1a7/nemusicapi/__init__.py
+-rw-r--r--   0        0        0     1921 2023-08-04 05:33:24.653663 nemusicapi-0.1.1a7/nemusicapi/api.py
+-rw-r--r--   0        0        0     3387 2023-08-04 05:34:42.298502 nemusicapi-0.1.1a7/nemusicapi/base_api.py
+-rw-r--r--   0        0        0      103 2023-08-04 05:34:09.580970 nemusicapi-0.1.1a7/nemusicapi/exception.py
+-rw-r--r--   0        0        0      363 2023-08-03 11:15:34.699086 nemusicapi-0.1.1a7/nemusicapi/type.py
+-rw-r--r--   0        0        0      466 2023-08-04 05:37:37.375511 nemusicapi-0.1.1a7/pyproject.toml
+-rw-r--r--   0        0        0     1340 2023-08-04 04:55:04.520489 nemusicapi-0.1.1a7/README.md
+-rw-r--r--   0        0        0     1960 1970-01-01 00:00:00.000000 nemusicapi-0.1.1a7/PKG-INFO
```

### Comparing `nemusicapi-0.1.1a6/LICENSE` & `nemusicapi-0.1.1a7/LICENSE`

 * *Files identical despite different names*

### Comparing `nemusicapi-0.1.1a6/nemusicapi/api.py` & `nemusicapi-0.1.1a7/nemusicapi/api.py`

 * *Files identical despite different names*

### Comparing `nemusicapi-0.1.1a6/nemusicapi/base_api.py` & `nemusicapi-0.1.1a7/nemusicapi/base_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import json
 
 import requests
 import urllib3
 from Crypto.Cipher import AES
 
 from nemusicapi.type import QualityLevel, EncodeType
+from nemusicapi.exception import NoSongNameException
 
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
 
 def aes_encrypt(raw_text: str, raw_key: str):
     key = raw_key.encode('utf-8')
     _text = raw_text.encode('utf-8')
@@ -56,14 +57,16 @@
             'Cookie': self.cookie
         }
         res = requests.post(url=url, params=params, headers=headers, verify=False)
         return res.json()
 
 
     def search_music(self, song_name: str, *, type=1, offset=0, total='true', limit=20):
+        if song_name == '':
+            raise NoSongNameException
         params = {
             'hlpretag': '<span class=\'s-fc7\'>',
             'hlposttag': '</span>',
             's': song_name,
             'type': type,
             'offset': offset,
             'total': total,
```

### Comparing `nemusicapi-0.1.1a6/README.md` & `nemusicapi-0.1.1a7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -18,18 +18,19 @@
 download_dir = './download'
 cookie = '这里输入cookie'
 
 api = Api(cookie=cookie, download_dir=download_dir)
 
 
 def main(raw_song_name: str):
-    res = api.refresh_song_data(raw_song_name)
+    res = api.get_song_data(raw_song_name, limit=1)
     if res is None:
         return
-    song_id, song_name = res
+    song_id = list(res.keys())[0]
+    song_name = list(res.values())[0]
     
     level = QualityLevel.hires
     res = api.get_song_download_data(song_id, level=level)
     if res is None:
         return
     song_url, song_type = res
```

### Comparing `nemusicapi-0.1.1a6/PKG-INFO` & `nemusicapi-0.1.1a7/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nemusicapi
-Version: 0.1.1a6
+Version: 0.1.1a7
 Summary: A Netsase music api
 Home-page: https://github.com/yuyi2439/NeteaseMusicApi
 License: Apache-2.0
 Author: yuyi2439
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -36,18 +36,19 @@
 download_dir = './download'
 cookie = '这里输入cookie'
 
 api = Api(cookie=cookie, download_dir=download_dir)
 
 
 def main(raw_song_name: str):
-    res = api.refresh_song_data(raw_song_name)
+    res = api.get_song_data(raw_song_name, limit=1)
     if res is None:
         return
-    song_id, song_name = res
+    song_id = list(res.keys())[0]
+    song_name = list(res.values())[0]
     
     level = QualityLevel.hires
     res = api.get_song_download_data(song_id, level=level)
     if res is None:
         return
     song_url, song_type = res
```

