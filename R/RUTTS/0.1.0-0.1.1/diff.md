# Comparing `tmp/RUTTS-0.1.0.tar.gz` & `tmp/RUTTS-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RUTTS-0.1.0.tar", last modified: Wed Aug  2 22:33:50 2023, max compression
+gzip compressed data, was "RUTTS-0.1.1.tar", last modified: Fri Aug  4 17:48:39 2023, max compression
```

## Comparing `RUTTS-0.1.0.tar` & `RUTTS-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0 teraspace  (1000) teraspace  (1000)        0 2023-08-02 22:33:50.601159 RUTTS-0.1.0/
--rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)     1057 2023-07-27 22:12:45.000000 RUTTS-0.1.0/LICENSE.txt
--rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)      561 2023-08-02 22:33:50.600914 RUTTS-0.1.0/PKG-INFO
-drwxrwxrwx   0 teraspace  (1000) teraspace  (1000)        0 2023-08-02 22:33:50.597908 RUTTS-0.1.0/RUTTS/
--rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)       27 2023-07-27 21:39:42.000000 RUTTS-0.1.0/RUTTS/__init__.py
--rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)     3383 2023-08-02 22:30:58.000000 RUTTS-0.1.0/RUTTS/infer_onnx.py
-drwxrwxrwx   0 teraspace  (1000) teraspace  (1000)        0 2023-08-02 22:33:50.600427 RUTTS-0.1.0/RUTTS.egg-info/
--rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)      561 2023-08-02 22:33:50.000000 RUTTS-0.1.0/RUTTS.egg-info/PKG-INFO
--rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)      202 2023-08-02 22:33:50.000000 RUTTS-0.1.0/RUTTS.egg-info/SOURCES.txt
--rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)        1 2023-08-02 22:33:50.000000 RUTTS-0.1.0/RUTTS.egg-info/dependency_links.txt
--rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)       66 2023-08-02 22:33:50.000000 RUTTS-0.1.0/RUTTS.egg-info/requires.txt
--rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)        6 2023-08-02 22:33:50.000000 RUTTS-0.1.0/RUTTS.egg-info/top_level.txt
--rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)       38 2023-08-02 22:33:50.601245 RUTTS-0.1.0/setup.cfg
--rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)      731 2023-08-02 22:33:44.000000 RUTTS-0.1.0/setup.py
+drwxrwxrwx   0 teraspace  (1000) teraspace  (1000)        0 2023-08-04 17:48:39.701094 RUTTS-0.1.1/
+-rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)     1057 2023-07-27 22:12:45.000000 RUTTS-0.1.1/LICENSE.txt
+-rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)      561 2023-08-04 17:48:39.700920 RUTTS-0.1.1/PKG-INFO
+drwxrwxrwx   0 teraspace  (1000) teraspace  (1000)        0 2023-08-04 17:48:39.698718 RUTTS-0.1.1/RUTTS/
+-rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)       27 2023-07-27 21:39:42.000000 RUTTS-0.1.1/RUTTS/__init__.py
+-rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)     3732 2023-08-04 17:45:47.000000 RUTTS-0.1.1/RUTTS/infer_onnx.py
+drwxrwxrwx   0 teraspace  (1000) teraspace  (1000)        0 2023-08-04 17:48:39.700590 RUTTS-0.1.1/RUTTS.egg-info/
+-rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)      561 2023-08-04 17:48:39.000000 RUTTS-0.1.1/RUTTS.egg-info/PKG-INFO
+-rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)      202 2023-08-04 17:48:39.000000 RUTTS-0.1.1/RUTTS.egg-info/SOURCES.txt
+-rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)        1 2023-08-04 17:48:39.000000 RUTTS-0.1.1/RUTTS.egg-info/dependency_links.txt
+-rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)       66 2023-08-04 17:48:39.000000 RUTTS-0.1.1/RUTTS.egg-info/requires.txt
+-rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)        6 2023-08-04 17:48:39.000000 RUTTS-0.1.1/RUTTS.egg-info/top_level.txt
+-rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)       38 2023-08-04 17:48:39.701155 RUTTS-0.1.1/setup.cfg
+-rwxrwxrwx   0 teraspace  (1000) teraspace  (1000)      731 2023-08-04 17:46:39.000000 RUTTS-0.1.1/setup.py
```

### Comparing `RUTTS-0.1.0/LICENSE.txt` & `RUTTS-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `RUTTS-0.1.0/PKG-INFO` & `RUTTS-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RUTTS
-Version: 0.1.0
+Version: 0.1.1
 Summary: russian text to speech
 Home-page: https://github.com/Tera2Space/RUTTS
 Author: Tera Space
 Author-email: tera2space@gmail.com
 License: MIT
 Keywords: tts
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `RUTTS-0.1.0/RUTTS/infer_onnx.py` & `RUTTS-0.1.1/RUTTS/infer_onnx.py`

 * *Files 22% similar despite different names*

```diff
@@ -61,28 +61,33 @@
     
     
     def _get_text(self, text: str) -> list[int]:
         text_norm = self._text_to_sequence(text)
         text_norm = self._intersperse(text_norm, 0)
         return text_norm
     
+    def _add_silent(self, audio, silence_duration: float = 0.5, sample_rate: int = 22050):
+        num_samples_silence = int(sample_rate * silence_duration)
+        silence_array = np.zeros(num_samples_silence, dtype=np.float32)
+        audio_with_silence = np.concatenate((audio, silence_array), axis=0)
+        return audio_with_silence
     
     def save_wav(self, audio, path:str):
         '''save audio to wav'''
         scipy.io.wavfile.write(path, 22050, audio)
     
     
     def play_audio(self, audio):
-        # sd.play(audio, 22050, blocking=True) # GOOD FOR LINUX but not for Windows :(
-        sd.play(audio, 22050)
-        time.sleep(
-            (len(audio)/22050) 
-            +
-            self.add_time_to_end
-            )
+        sd.play(audio, 22050, blocking=True)
+        # sd.play(audio, 22050)
+        # time.sleep(
+        #     (len(audio)/22050) 
+        #     +
+        #     self.add_time_to_end
+        #     )
     
     
     def __call__(self, text: str, play = False):
         phoneme_ids = self._get_text(text)
         text = np.expand_dims(np.array(phoneme_ids, dtype=np.int64), 0)
         text_lengths = np.array([text.shape[1]], dtype=np.int64)
         scales = np.array(
@@ -94,10 +99,11 @@
             {
                 "input": text,
                 "input_lengths": text_lengths,
                 "scales": scales,
                 "sid": None,
             },
         )[0][0,0][0]
+        audio = self._add_silent(audio)
         if play:
             self.play_audio(audio)
         return audio
```

### Comparing `RUTTS-0.1.0/RUTTS.egg-info/PKG-INFO` & `RUTTS-0.1.1/RUTTS.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RUTTS
-Version: 0.1.0
+Version: 0.1.1
 Summary: russian text to speech
 Home-page: https://github.com/Tera2Space/RUTTS
 Author: Tera Space
 Author-email: tera2space@gmail.com
 License: MIT
 Keywords: tts
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `RUTTS-0.1.0/setup.py` & `RUTTS-0.1.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,15 @@
   'Operating System :: MacOS',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='RUTTS',
-  version='0.1.0',
+  version='0.1.1',
   description='russian text to speech',
   url='https://github.com/Tera2Space/RUTTS',  
   author='Tera Space',
   author_email='tera2space@gmail.com',
   license='MIT', 
   classifiers=classifiers,
   keywords='tts',
```

