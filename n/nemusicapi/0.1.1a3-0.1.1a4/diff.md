# Comparing `tmp/nemusicapi-0.1.1a3.tar.gz` & `tmp/nemusicapi-0.1.1a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nemusicapi-0.1.1a3.tar", max compression
+gzip compressed data, was "nemusicapi-0.1.1a4.tar", max compression
```

## Comparing `nemusicapi-0.1.1a3.tar` & `nemusicapi-0.1.1a4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11558 2023-08-01 07:21:02.527622 nemusicapi-0.1.1a3/LICENSE
--rw-r--r--   0        0        0      311 2023-08-03 09:11:40.318932 nemusicapi-0.1.1a3/nemusicapi/__init__.py
--rw-r--r--   0        0        0     4883 2023-08-03 09:44:38.640178 nemusicapi-0.1.1a3/nemusicapi/api.py
--rw-r--r--   0        0        0      113 2023-08-03 06:48:17.625541 nemusicapi-0.1.1a3/nemusicapi/exception.py
--rw-r--r--   0        0        0      355 2023-08-03 09:37:41.904391 nemusicapi-0.1.1a3/nemusicapi/type.py
--rw-r--r--   0        0        0      466 2023-08-03 09:44:53.732438 nemusicapi-0.1.1a3/pyproject.toml
--rw-r--r--   0        0        0     1285 2023-08-03 09:34:57.662330 nemusicapi-0.1.1a3/README.md
--rw-r--r--   0        0        0     1906 1970-01-01 00:00:00.000000 nemusicapi-0.1.1a3/PKG-INFO
+-rw-r--r--   0        0        0    11558 2023-08-01 07:21:02.527622 nemusicapi-0.1.1a4/LICENSE
+-rw-r--r--   0        0        0      311 2023-08-03 09:11:40.318932 nemusicapi-0.1.1a4/nemusicapi/__init__.py
+-rw-r--r--   0        0        0     4958 2023-08-03 11:17:30.186582 nemusicapi-0.1.1a4/nemusicapi/api.py
+-rw-r--r--   0        0        0      113 2023-08-03 06:48:17.625541 nemusicapi-0.1.1a4/nemusicapi/exception.py
+-rw-r--r--   0        0        0      363 2023-08-03 11:15:34.699086 nemusicapi-0.1.1a4/nemusicapi/type.py
+-rw-r--r--   0        0        0      466 2023-08-03 11:17:10.491986 nemusicapi-0.1.1a4/pyproject.toml
+-rw-r--r--   0        0        0     1291 2023-08-03 11:15:05.073832 nemusicapi-0.1.1a4/README.md
+-rw-r--r--   0        0        0     1912 1970-01-01 00:00:00.000000 nemusicapi-0.1.1a4/PKG-INFO
```

### Comparing `nemusicapi-0.1.1a3/LICENSE` & `nemusicapi-0.1.1a4/LICENSE`

 * *Files identical despite different names*

### Comparing `nemusicapi-0.1.1a3/nemusicapi/api.py` & `nemusicapi-0.1.1a4/nemusicapi/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 
 class RawApi:
     def __init__(self, *,
                  cookie=''
                  ):
         self.cookie = cookie
-        
+
 
     def _get_data(self, url: str, raw_params) -> dict:
         _params, encSecKey = get_params(json.dumps(raw_params))
         params = {
             "params": _params,
             "encSecKey": encSecKey
         }
@@ -71,15 +71,16 @@
             'offset': offset,
             'total': total,
             'limit': limit
         }
         url = 'https://music.163.com/weapi/cloudsearch/get/web'
         res = self._get_data(url, params)
         return res
-    
+
+
     def get_song_file_data(self, song_id: int, *, level: QualityLevel, encodeType: EncodeType):
         url = f'https://music.163.com/weapi/song/enhance/player/url/v1'
         params = {
             'ids': '["' + str(song_id) + '"]',
             'level': level.value,
             'encodeType': encodeType.value
         }
@@ -94,26 +95,29 @@
                  ):
         super().__init__(cookie=cookie)
         self.download_dir = download_dir
         
         if download_dir:
             if not os.path.exists(download_dir):
                 os.makedirs(download_dir)
-    
-    
-    def refresh_song_data(self, raw_song_name: str) -> tuple[int, str] | None:
+
+
+    def get_song_data(self, raw_song_name: str) -> tuple[int, str] | None:
         res = self.search_music(raw_song_name)
         if res['result']['songCount'] == 0:
             return
         song_id = res['result']['songs'][0]['id']
         song_name = res['result']['songs'][0]['name']
         return song_id, song_name
 
 
-    def get_song_download_data(self, song_id: int, *, level=QualityLevel.standard, encodeType=EncodeType.flac) -> tuple[str, EncodeType] | None:
+    def get_song_download_data(self, song_id: int, *,
+                               level=QualityLevel.standard,
+                               encodeType=EncodeType.flac
+                               ) -> tuple[str, EncodeType] | None:
         res = self.get_song_file_data(song_id, level=level, encodeType=encodeType)
         if res['data'][0]['url'] is None:
             return
         song_url = res['data'][0]['url']
         song_type = res['data'][0]['type']
         return song_url, EncodeType(song_type)
```

### Comparing `nemusicapi-0.1.1a3/README.md` & `nemusicapi-0.1.1a4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     
     level = QualityLevel.hires
     res = api.get_song_download_data(song_id, level=level)
     if res is None:
         return
     song_url, song_type = res
     
-    file_name = f'{song_name}_{level.value}.{song_type}'
+    file_name = f'{song_name}_{level.value}.{song_type.value}'
     if not os.path.exists(os.path.join(download_dir, file_name)):
         api.download_song(song_url, file_name)
 
 
 if __name__ == '__main__':
     main('这里输入歌曲名')
 ```
```

### Comparing `nemusicapi-0.1.1a3/PKG-INFO` & `nemusicapi-0.1.1a4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nemusicapi
-Version: 0.1.1a3
+Version: 0.1.1a4
 Summary: A Netsase music api
 Home-page: https://github.com/yuyi2439/NeteaseMusicApi
 License: Apache-2.0
 Author: yuyi2439
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -47,15 +47,15 @@
     
     level = QualityLevel.hires
     res = api.get_song_download_data(song_id, level=level)
     if res is None:
         return
     song_url, song_type = res
     
-    file_name = f'{song_name}_{level.value}.{song_type}'
+    file_name = f'{song_name}_{level.value}.{song_type.value}'
     if not os.path.exists(os.path.join(download_dir, file_name)):
         api.download_song(song_url, file_name)
 
 
 if __name__ == '__main__':
     main('这里输入歌曲名')
 ```
```

