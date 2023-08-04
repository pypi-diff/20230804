# Comparing `tmp/RUTTS-0.1.1.tar.gz` & `tmp/RUTTS-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RUTTS-0.1.1.tar", last modified: Fri Aug  4 17:48:39 2023, max compression
+gzip compressed data, was "RUTTS-0.1.2.tar", last modified: Fri Aug  4 17:53:05 2023, max compression
```

## Comparing `RUTTS-0.1.1.tar` & `RUTTS-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0 teraspace  (1000) teraspace  (1000)        0 2023-08-04 17:48:39.701094 RUTTS-0.1.1/
--rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)     1057 2023-07-27 22:12:45.000000 RUTTS-0.1.1/LICENSE.txt
--rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)      561 2023-08-04 17:48:39.700920 RUTTS-0.1.1/PKG-INFO
-drwxrwxrwx   0 teraspace  (1000) teraspace  (1000)        0 2023-08-04 17:48:39.698718 RUTTS-0.1.1/RUTTS/
--rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)       27 2023-07-27 21:39:42.000000 RUTTS-0.1.1/RUTTS/__init__.py
--rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)     3732 2023-08-04 17:45:47.000000 RUTTS-0.1.1/RUTTS/infer_onnx.py
-drwxrwxrwx   0 teraspace  (1000) teraspace  (1000)        0 2023-08-04 17:48:39.700590 RUTTS-0.1.1/RUTTS.egg-info/
--rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)      561 2023-08-04 17:48:39.000000 RUTTS-0.1.1/RUTTS.egg-info/PKG-INFO
--rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)      202 2023-08-04 17:48:39.000000 RUTTS-0.1.1/RUTTS.egg-info/SOURCES.txt
--rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)        1 2023-08-04 17:48:39.000000 RUTTS-0.1.1/RUTTS.egg-info/dependency_links.txt
--rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)       66 2023-08-04 17:48:39.000000 RUTTS-0.1.1/RUTTS.egg-info/requires.txt
--rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)        6 2023-08-04 17:48:39.000000 RUTTS-0.1.1/RUTTS.egg-info/top_level.txt
--rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)       38 2023-08-04 17:48:39.701155 RUTTS-0.1.1/setup.cfg
--rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)      731 2023-08-04 17:46:39.000000 RUTTS-0.1.1/setup.py
+drwxrwxrwx   0 teraspace  (1000) teraspace  (1000)        0 2023-08-04 17:53:05.505162 RUTTS-0.1.2/
+-rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)     1057 2023-07-27 22:12:45.000000 RUTTS-0.1.2/LICENSE.txt
+-rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)      561 2023-08-04 17:53:05.504953 RUTTS-0.1.2/PKG-INFO
+drwxrwxrwx   0 teraspace  (1000) teraspace  (1000)        0 2023-08-04 17:53:05.502303 RUTTS-0.1.2/RUTTS/
+-rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)       27 2023-07-27 21:39:42.000000 RUTTS-0.1.2/RUTTS/__init__.py
+-rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)     3732 2023-08-04 17:52:23.000000 RUTTS-0.1.2/RUTTS/infer_onnx.py
+drwxrwxrwx   0 teraspace  (1000) teraspace  (1000)        0 2023-08-04 17:53:05.504509 RUTTS-0.1.2/RUTTS.egg-info/
+-rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)      561 2023-08-04 17:53:05.000000 RUTTS-0.1.2/RUTTS.egg-info/PKG-INFO
+-rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)      202 2023-08-04 17:53:05.000000 RUTTS-0.1.2/RUTTS.egg-info/SOURCES.txt
+-rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)        1 2023-08-04 17:53:05.000000 RUTTS-0.1.2/RUTTS.egg-info/dependency_links.txt
+-rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)       66 2023-08-04 17:53:05.000000 RUTTS-0.1.2/RUTTS.egg-info/requires.txt
+-rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)        6 2023-08-04 17:53:05.000000 RUTTS-0.1.2/RUTTS.egg-info/top_level.txt
+-rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)       38 2023-08-04 17:53:05.505231 RUTTS-0.1.2/setup.cfg
+-rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)      731 2023-08-04 17:52:46.000000 RUTTS-0.1.2/setup.py
```

### Comparing `RUTTS-0.1.1/LICENSE.txt` & `RUTTS-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `RUTTS-0.1.1/PKG-INFO` & `RUTTS-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RUTTS
-Version: 0.1.1
+Version: 0.1.2
 Summary: russian text to speech
 Home-page: https://github.com/Tera2Space/RUTTS
 Author: Tera Space
 Author-email: tera2space@gmail.com
 License: MIT
 Keywords: tts
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `RUTTS-0.1.1/RUTTS/infer_onnx.py` & `RUTTS-0.1.2/RUTTS/infer_onnx.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     
     
     def _get_text(self, text: str) -> list[int]:
         text_norm = self._text_to_sequence(text)
         text_norm = self._intersperse(text_norm, 0)
         return text_norm
     
-    def _add_silent(self, audio, silence_duration: float = 0.5, sample_rate: int = 22050):
+    def _add_silent(self, audio, silence_duration: float = 1.0, sample_rate: int = 22050):
         num_samples_silence = int(sample_rate * silence_duration)
         silence_array = np.zeros(num_samples_silence, dtype=np.float32)
         audio_with_silence = np.concatenate((audio, silence_array), axis=0)
         return audio_with_silence
     
     def save_wav(self, audio, path:str):
         '''save audio to wav'''
```

### Comparing `RUTTS-0.1.1/RUTTS.egg-info/PKG-INFO` & `RUTTS-0.1.2/RUTTS.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RUTTS
-Version: 0.1.1
+Version: 0.1.2
 Summary: russian text to speech
 Home-page: https://github.com/Tera2Space/RUTTS
 Author: Tera Space
 Author-email: tera2space@gmail.com
 License: MIT
 Keywords: tts
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `RUTTS-0.1.1/setup.py` & `RUTTS-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
   'Operating System :: MacOS',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='RUTTS',
-  version='0.1.1',
+  version='0.1.2',
   description='russian text to speech',
   url='https://github.com/Tera2Space/RUTTS',  
   author='Tera Space',
   author_email='tera2space@gmail.com',
   license='MIT', 
   classifiers=classifiers,
   keywords='tts',
```

