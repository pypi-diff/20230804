# Comparing `tmp/tts-gen-1.2.4.tar.gz` & `tmp/tts-gen-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tts-gen-1.2.4.tar", last modified: Wed Apr 12 11:16:10 2023, max compression
+gzip compressed data, was "dist/tts-gen-1.3.0.tar", last modified: Fri Aug  4 07:15:04 2023, max compression
```

## Comparing `tts-gen-1.2.4.tar` & `tts-gen-1.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 zhengdi   (1007) zhengdi   (1007)        0 2023-04-12 11:16:10.000000 tts-gen-1.2.4/
-drwxrwxr-x   0 zhengdi   (1007) zhengdi   (1007)        0 2023-04-12 11:16:10.000000 tts-gen-1.2.4/tts_gen.egg-info/
--rw-rw-r--   0 zhengdi   (1007) zhengdi   (1007)      263 2023-04-12 11:16:10.000000 tts-gen-1.2.4/tts_gen.egg-info/SOURCES.txt
--rw-rw-r--   0 zhengdi   (1007) zhengdi   (1007)        1 2023-04-12 11:16:09.000000 tts-gen-1.2.4/tts_gen.egg-info/dependency_links.txt
--rw-rw-r--   0 zhengdi   (1007) zhengdi   (1007)      555 2023-04-12 11:16:09.000000 tts-gen-1.2.4/tts_gen.egg-info/PKG-INFO
--rw-rw-r--   0 zhengdi   (1007) zhengdi   (1007)       14 2023-04-12 11:16:09.000000 tts-gen-1.2.4/tts_gen.egg-info/requires.txt
--rw-rw-r--   0 zhengdi   (1007) zhengdi   (1007)       14 2023-04-12 11:16:09.000000 tts-gen-1.2.4/tts_gen.egg-info/top_level.txt
--rw-rw-r--   0 zhengdi   (1007) zhengdi   (1007)     1617 2022-08-10 02:41:51.000000 tts-gen-1.2.4/setup.py
--rw-rw-r--   0 zhengdi   (1007) zhengdi   (1007)      555 2023-04-12 11:16:10.000000 tts-gen-1.2.4/PKG-INFO
--rw-rw-r--   0 zhengdi   (1007) zhengdi   (1007)       38 2023-04-12 11:16:10.000000 tts-gen-1.2.4/setup.cfg
-drwxrwxr-x   0 zhengdi   (1007) zhengdi   (1007)        0 2023-04-12 11:16:10.000000 tts-gen-1.2.4/tts_generator/
--rw-rw-r--   0 zhengdi   (1007) zhengdi   (1007)     1995 2022-11-30 11:17:17.000000 tts-gen-1.2.4/tts_generator/tts-gen
--rw-rw-r--   0 zhengdi   (1007) zhengdi   (1007)     1995 2022-11-30 10:36:27.000000 tts-gen-1.2.4/tts_generator/__main__.py
--rw-rw-r--   0 zhengdi   (1007) zhengdi   (1007)     8510 2023-04-12 11:15:15.000000 tts-gen-1.2.4/tts_generator/gen_voice.py
--rw-rw-r--   0 zhengdi   (1007) zhengdi   (1007)      254 2023-04-12 09:00:21.000000 tts-gen-1.2.4/tts_generator/__init__.py
+drwxrwxr-x   0 zhengdi   (1007) zhengdi   (1007)        0 2023-08-04 07:15:04.176122 tts-gen-1.3.0/
+-rw-rw-r--   0 zhengdi   (1007) zhengdi   (1007)      499 2023-08-04 07:15:04.176122 tts-gen-1.3.0/PKG-INFO
+-rw-rw-r--   0 zhengdi   (1007) zhengdi   (1007)       38 2023-08-04 07:15:04.176122 tts-gen-1.3.0/setup.cfg
+-rw-rw-r--   0 zhengdi   (1007) zhengdi   (1007)     1617 2022-08-10 02:41:51.000000 tts-gen-1.3.0/setup.py
+drwxrwxr-x   0 zhengdi   (1007) zhengdi   (1007)        0 2023-08-04 07:15:04.176122 tts-gen-1.3.0/tts_gen.egg-info/
+-rw-rw-r--   0 zhengdi   (1007) zhengdi   (1007)      499 2023-08-04 07:15:04.000000 tts-gen-1.3.0/tts_gen.egg-info/PKG-INFO
+-rw-rw-r--   0 zhengdi   (1007) zhengdi   (1007)      263 2023-08-04 07:15:04.000000 tts-gen-1.3.0/tts_gen.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhengdi   (1007) zhengdi   (1007)        1 2023-08-04 07:15:04.000000 tts-gen-1.3.0/tts_gen.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhengdi   (1007) zhengdi   (1007)       14 2023-08-04 07:15:04.000000 tts-gen-1.3.0/tts_gen.egg-info/requires.txt
+-rw-rw-r--   0 zhengdi   (1007) zhengdi   (1007)       14 2023-08-04 07:15:04.000000 tts-gen-1.3.0/tts_gen.egg-info/top_level.txt
+drwxrwxr-x   0 zhengdi   (1007) zhengdi   (1007)        0 2023-08-04 07:15:04.176122 tts-gen-1.3.0/tts_generator/
+-rw-rw-r--   0 zhengdi   (1007) zhengdi   (1007)      307 2023-08-04 06:48:27.000000 tts-gen-1.3.0/tts_generator/__init__.py
+-rw-rw-r--   0 zhengdi   (1007) zhengdi   (1007)     2160 2023-08-04 02:21:50.000000 tts-gen-1.3.0/tts_generator/__main__.py
+-rw-rw-r--   0 zhengdi   (1007) zhengdi   (1007)    11884 2023-08-04 07:14:31.000000 tts-gen-1.3.0/tts_generator/gen_voice.py
+-rw-rw-r--   0 zhengdi   (1007) zhengdi   (1007)     2160 2023-08-04 07:09:16.000000 tts-gen-1.3.0/tts_generator/tts-gen
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tts-gen-1.2.4/setup.py` & `tts-gen-1.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `tts-gen-1.2.4/tts_generator/tts-gen` & `tts-gen-1.3.0/tts_generator/__main__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 #!/usr/bin/env python
 
 import sys
 import argparse
-from tts_generator import __version__, __server_url__, __server_bridge_url__
+from tts_generator import __version__, __server_url__, __server_valle_url__, __server_bridge_url__
 from tts_generator.gen_voice import gen_voice
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser(prog='tts-gen', description='TTS Generator')
     parser.add_argument('-V', '--version', action='version', version='tts-gen %s' % __version__)
     parser.add_argument('-f', '--file', help='tts keywords file, one keyword per line')
     parser.add_argument('-o', '--output', help='output wavs directory')
     parser.add_argument('-n', '--num', type=int, help='number of wavs to be generated per keyword (default: max)')
-    parser.add_argument('-u', '--url', help='url of tts server (default: %s)' % __server_url__)
-    parser.add_argument('-b', '--bridge_url', help='url of tts server (default: %s)' % __server_bridge_url__)
+    parser.add_argument('-u', '--url', help='url of tts server (default: gx: %s, valle: %s, aliyun/mobvoi: %s)'
+            % (__server_url__, __server_valle_url__, __server_bridge_url__))
+    parser.add_argument('-b', '--bridge_url', help='(LEGACY) url of aliyun/mobvoi tts server (default: %s)' % __server_bridge_url__)
     parser.add_argument('-t', '--type', choices=['all', 'train', 'test'], default='all',
-                        help='generate train, test, or all wavs (default: all) (only valid when gx tts selected)')
-    parser.add_argument('-i', '--infer', choices=['gx', 'aliyun', 'mobvoi'], default='gx',
+                        help='generate train, test, or all wavs (default: all) (only valid when gx or valle tts selected)')
+    parser.add_argument('-i', '--infer', choices=['gx', 'valle', 'aliyun', 'mobvoi'], default='gx',
                         help='tts server (default: gx)')
-    parser.add_argument('-p', '--process', type=int, default=3, help='multiply process num (default/max: mobvoi 3, aliyun 2, gx 1)')
+    parser.add_argument('-p', '--process', type=int, default=3, help='multiply process num (default/max: mobvoi 3, aliyun 2, gx 1, valle 1)')
     parser.add_argument('-s', '--style', action="store_true", help='generate wavs with speaker style')
     args = parser.parse_args()
     if args.file and args.output:
         texts = []
         for line in open(args.file, 'r'):
             line = line.strip(' ').strip('\t').strip('\n')
             if line:
```

### Comparing `tts-gen-1.2.4/tts_generator/__main__.py` & `tts-gen-1.3.0/tts_generator/tts-gen`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 #!/usr/bin/env python
 
 import sys
 import argparse
-from tts_generator import __version__, __server_url__, __server_bridge_url__
+from tts_generator import __version__, __server_url__, __server_valle_url__, __server_bridge_url__
 from tts_generator.gen_voice import gen_voice
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser(prog='tts-gen', description='TTS Generator')
     parser.add_argument('-V', '--version', action='version', version='tts-gen %s' % __version__)
     parser.add_argument('-f', '--file', help='tts keywords file, one keyword per line')
     parser.add_argument('-o', '--output', help='output wavs directory')
     parser.add_argument('-n', '--num', type=int, help='number of wavs to be generated per keyword (default: max)')
-    parser.add_argument('-u', '--url', help='url of tts server (default: %s)' % __server_url__)
-    parser.add_argument('-b', '--bridge_url', help='url of tts server (default: %s)' % __server_bridge_url__)
+    parser.add_argument('-u', '--url', help='url of tts server (default: gx: %s, valle: %s, aliyun/mobvoi: %s)'
+            % (__server_url__, __server_valle_url__, __server_bridge_url__))
+    parser.add_argument('-b', '--bridge_url', help='(LEGACY) url of aliyun/mobvoi tts server (default: %s)' % __server_bridge_url__)
     parser.add_argument('-t', '--type', choices=['all', 'train', 'test'], default='all',
-                        help='generate train, test, or all wavs (default: all) (only valid when gx tts selected)')
-    parser.add_argument('-i', '--infer', choices=['gx', 'aliyun', 'mobvoi'], default='gx',
+                        help='generate train, test, or all wavs (default: all) (only valid when gx or valle tts selected)')
+    parser.add_argument('-i', '--infer', choices=['gx', 'valle', 'aliyun', 'mobvoi'], default='gx',
                         help='tts server (default: gx)')
-    parser.add_argument('-p', '--process', type=int, default=3, help='multiply process num (default/max: mobvoi 3, aliyun 2, gx 1)')
+    parser.add_argument('-p', '--process', type=int, default=3, help='multiply process num (default/max: mobvoi 3, aliyun 2, gx 1, valle 1)')
     parser.add_argument('-s', '--style', action="store_true", help='generate wavs with speaker style')
     args = parser.parse_args()
     if args.file and args.output:
         texts = []
         for line in open(args.file, 'r'):
             line = line.strip(' ').strip('\t').strip('\n')
             if line:
```

### Comparing `tts-gen-1.2.4/tts_generator/gen_voice.py` & `tts-gen-1.3.0/tts_generator/gen_voice.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import os.path
 import requests
 import json
 import string
 import multiprocessing
 from tqdm import tqdm
-from tts_generator import __server_url__, __server_bridge_url__
+from tts_generator import __server_url__, __server_valle_url__, __server_bridge_url__
 
 headers = {
         'User-Agent'         : 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/94.0.4606.61 Safari/537.36',
         'Accept-Language'    : 'zh-CN,zh;q=0.9',
         }
 
 def gen_wav_dir_str(s):
@@ -31,20 +31,93 @@
         if wav_type == 'train':
             max_voice_num = info['max_train_voice_num']
         elif wav_type == 'test':
             max_voice_num = info['max_test_voice_num']
         else:
             max_voice_num = info['max_voice_num']
         if not voice_num:
-            voice_num = max_voice_num
-        total_voice_num = min(max_voice_num, voice_num)
+            total_voice_num = max_voice_num
+        else:
+            total_voice_num = min(max_voice_num, voice_num)
+
+        for text in texts:
+            print('generate %s wavs ...' % text)
+
+            wav_dir_str = gen_wav_dir_str(text)
+            text_dir = os.path.join(output_dir, wav_dir_str)
+            if not os.path.exists(text_dir):
+                os.mkdir(text_dir)
+
+            if wav_type in ('train', 'test'):
+                text_dir = os.path.join(text_dir, wav_type)
+                if not os.path.exists(text_dir):
+                    os.mkdir(text_dir)
+                list_f_name = '%s_%s.list' % (wav_dir_str, wav_type)
+                wav_dir = '%s/%s' % (wav_dir_str, wav_type)
+            else:
+                list_f_name = '%s.list' % wav_dir_str
+                wav_dir = '%s' % wav_dir_str
+
+            list_f_path = os.path.join(output_dir, list_f_name)
+            list_f = open(list_f_path, "w")
+            blk_voice_num = 10 # 分块传输
+            for voice_index in tqdm(range(0, total_voice_num, blk_voice_num)):
+                data = {
+                    'text': text,
+                    'voice_index': voice_index,
+                    'voice_num': min(blk_voice_num, total_voice_num - voice_index),
+                    'wav_type': wav_type,
+                    }
+                r = session.post(url=server_synthesize_url, data=data, headers=headers, verify=False)
+                wav_split_map = json.loads(r.headers['Content-Type'])
+                for k, v in wav_split_map.items():
+                    begin, end = v[0], v[1]
+                    with open('%s' % os.path.join(text_dir, k), 'wb') as f:
+                        f.write(r.content[begin:end])
+                    list_f.write('%s,%s\n' % (os.path.join(wav_dir, k), text))
+            list_f.close()
+
+
+def gen_valle_voice(texts, output_dir, server_url=None, voice_num=None, wav_type='all', tts_server_name='valle'):
+    if not server_url:
+        server_url = __server_valle_url__
+    server_synthesize_url = server_url + '/api/synthesize_multi'
+    server_info_url = server_url + '/api/info'
+
+    if not os.path.exists(output_dir):
+        os.mkdir(output_dir)
+
+    with requests.Session() as session:
+        r = session.get(url=server_info_url, headers=headers, verify=False)
+        info = json.loads(r.text)
 
         for text in texts:
             print('generate %s wavs ...' % text)
 
+            if is_english_text(text):
+                language = 'en'
+                if wav_type == 'train':
+                    max_voice_num = info['max_en_train_voice_num']
+                elif wav_type == 'test':
+                    max_voice_num = info['max_en_test_voice_num']
+                else:
+                    max_voice_num = info['max_en_voice_num']
+            else:
+                language = 'zh'
+                if wav_type == 'train':
+                    max_voice_num = info['max_zh_train_voice_num']
+                elif wav_type == 'test':
+                    max_voice_num = info['max_zh_test_voice_num']
+                else:
+                    max_voice_num = info['max_zh_voice_num']
+            if not voice_num:
+                total_voice_num = max_voice_num
+            else:
+                total_voice_num = min(max_voice_num, voice_num)
+
             wav_dir_str = gen_wav_dir_str(text)
             text_dir = os.path.join(output_dir, wav_dir_str)
             if not os.path.exists(text_dir):
                 os.mkdir(text_dir)
 
             if wav_type in ('train', 'test'):
                 text_dir = os.path.join(text_dir, wav_type)
@@ -60,14 +133,15 @@
             list_f = open(list_f_path, "w")
             blk_voice_num = 10 # 分块传输
             for voice_index in tqdm(range(0, total_voice_num, blk_voice_num)):
                 data = {
                     'text': text,
                     'voice_index': voice_index,
                     'voice_num': min(blk_voice_num, total_voice_num - voice_index),
+                    'language': language,
                     'wav_type': wav_type,
                     }
                 r = session.post(url=server_synthesize_url, data=data, headers=headers, verify=False)
                 wav_split_map = json.loads(r.headers['Content-Type'])
                 for k, v in wav_split_map.items():
                     begin, end = v[0], v[1]
                     with open('%s' % os.path.join(text_dir, k), 'wb') as f:
@@ -187,22 +261,26 @@
             pool.join()
 
 
 def gen_voice(texts, output_dir, server_url=None, bridge_server_url=None, voice_num=None, wav_type='all',
         tts_server_name='gx', process_num=3, with_style=False):
     if tts_server_name == 'gx':
         return gen_gx_voice(texts, output_dir, server_url, voice_num, wav_type)
+    elif tts_server_name == 'valle':
+        return gen_valle_voice(texts, output_dir, server_url, voice_num, wav_type)
     else:
         max_process_num = 1
         if tts_server_name == 'aliyun':
             max_process_num = 2
         elif tts_server_name == 'mobvoi':
             max_process_num = 3
         if process_num > max_process_num:
             process_num = max_process_num
+        if server_url is not None:
+            bridge_server_url = server_url
         return gen_other_voice(texts, output_dir, bridge_server_url, voice_num, wav_type,
                 tts_server_name, process_num, with_style)
 
 
 if __name__ == '__main__':
     texts = []
     texts.append('你好小爱')
```

