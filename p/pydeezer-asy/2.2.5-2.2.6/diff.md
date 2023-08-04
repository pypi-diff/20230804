# Comparing `tmp/pydeezer_asy-2.2.5.tar.gz` & `tmp/pydeezer_asy-2.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydeezer_asy-2.2.5.tar", last modified: Fri Jul 28 17:51:39 2023, max compression
+gzip compressed data, was "pydeezer_asy-2.2.6.tar", last modified: Fri Aug  4 15:38:41 2023, max compression
```

## Comparing `pydeezer_asy-2.2.5.tar` & `pydeezer_asy-2.2.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 17:51:39.213268 pydeezer_asy-2.2.5/
--rw-rw-rw-   0        0        0     3743 2023-07-28 17:51:39.211954 pydeezer_asy-2.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     3379 2023-07-28 17:51:13.000000 pydeezer_asy-2.2.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-28 17:51:39.123712 pydeezer_asy-2.2.5/deezer_asy/
--rw-rw-rw-   0        0        0    31843 2023-07-28 17:21:24.000000 pydeezer_asy-2.2.5/deezer_asy/DeezerAsy.py
--rw-rw-rw-   0        0        0      168 2023-07-28 16:45:52.000000 pydeezer_asy-2.2.5/deezer_asy/__init__.py
--rw-rw-rw-   0        0        0    29344 2023-07-28 17:21:32.000000 pydeezer_asy-2.2.5/deezer_asy/aiodeezer.py
-drwxrwxrwx   0        0        0        0 2023-07-28 17:51:39.150225 pydeezer_asy-2.2.5/deezer_asy/constants/
--rw-rw-rw-   0        0        0      193 2023-05-22 20:25:26.000000 pydeezer_asy-2.2.5/deezer_asy/constants/__init__.py
--rw-rw-rw-   0        0        0      789 2023-05-22 20:25:26.000000 pydeezer_asy-2.2.5/deezer_asy/constants/api_methods.py
--rw-rw-rw-   0        0        0      191 2023-05-22 20:25:26.000000 pydeezer_asy-2.2.5/deezer_asy/constants/api_urls.py
--rw-rw-rw-   0        0        0      124 2023-05-22 20:25:26.000000 pydeezer_asy-2.2.5/deezer_asy/constants/image_hosts.py
--rw-rw-rw-   0        0        0      392 2023-05-22 20:25:26.000000 pydeezer_asy-2.2.5/deezer_asy/constants/networking_settings.py
--rw-rw-rw-   0        0        0       72 2023-05-22 20:25:26.000000 pydeezer_asy-2.2.5/deezer_asy/constants/search_types.py
--rw-rw-rw-   0        0        0      694 2023-05-22 20:25:26.000000 pydeezer_asy-2.2.5/deezer_asy/constants/track_formats.py
--rw-rw-rw-   0        0        0      140 2023-05-22 20:25:26.000000 pydeezer_asy-2.2.5/deezer_asy/exceptions.py
--rw-rw-rw-   0        0        0     2004 2023-07-07 16:54:00.000000 pydeezer_asy-2.2.5/deezer_asy/util.py
-drwxrwxrwx   0        0        0        0 2023-07-28 17:51:39.207831 pydeezer_asy-2.2.5/pydeezer_asy.egg-info/
--rw-rw-rw-   0        0        0     3743 2023-07-28 17:51:38.000000 pydeezer_asy-2.2.5/pydeezer_asy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      569 2023-07-28 17:51:38.000000 pydeezer_asy-2.2.5/pydeezer_asy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 17:51:38.000000 pydeezer_asy-2.2.5/pydeezer_asy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-07-28 17:51:38.000000 pydeezer_asy-2.2.5/pydeezer_asy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-28 17:51:38.000000 pydeezer_asy-2.2.5/pydeezer_asy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-28 17:51:39.213268 pydeezer_asy-2.2.5/setup.cfg
--rw-rw-rw-   0        0        0      774 2023-07-28 17:51:30.000000 pydeezer_asy-2.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 15:38:41.225470 pydeezer_asy-2.2.6/
+-rw-rw-rw-   0        0        0     3743 2023-08-04 15:38:41.224469 pydeezer_asy-2.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3379 2023-07-28 17:53:01.000000 pydeezer_asy-2.2.6/README.md
+drwxrwxrwx   0        0        0        0 2023-08-04 15:38:41.143128 pydeezer_asy-2.2.6/deezer_asy/
+-rw-rw-rw-   0        0        0    31911 2023-08-04 15:38:23.000000 pydeezer_asy-2.2.6/deezer_asy/DeezerAsy.py
+-rw-rw-rw-   0        0        0      168 2023-07-28 16:45:52.000000 pydeezer_asy-2.2.6/deezer_asy/__init__.py
+-rw-rw-rw-   0        0        0    29418 2023-08-04 15:38:19.000000 pydeezer_asy-2.2.6/deezer_asy/aiodeezer.py
+drwxrwxrwx   0        0        0        0 2023-08-04 15:38:41.166024 pydeezer_asy-2.2.6/deezer_asy/constants/
+-rw-rw-rw-   0        0        0      193 2023-05-22 20:25:26.000000 pydeezer_asy-2.2.6/deezer_asy/constants/__init__.py
+-rw-rw-rw-   0        0        0      789 2023-05-22 20:25:26.000000 pydeezer_asy-2.2.6/deezer_asy/constants/api_methods.py
+-rw-rw-rw-   0        0        0      191 2023-05-22 20:25:26.000000 pydeezer_asy-2.2.6/deezer_asy/constants/api_urls.py
+-rw-rw-rw-   0        0        0      124 2023-05-22 20:25:26.000000 pydeezer_asy-2.2.6/deezer_asy/constants/image_hosts.py
+-rw-rw-rw-   0        0        0      392 2023-05-22 20:25:26.000000 pydeezer_asy-2.2.6/deezer_asy/constants/networking_settings.py
+-rw-rw-rw-   0        0        0       72 2023-05-22 20:25:26.000000 pydeezer_asy-2.2.6/deezer_asy/constants/search_types.py
+-rw-rw-rw-   0        0        0      694 2023-05-22 20:25:26.000000 pydeezer_asy-2.2.6/deezer_asy/constants/track_formats.py
+-rw-rw-rw-   0        0        0      140 2023-05-22 20:25:26.000000 pydeezer_asy-2.2.6/deezer_asy/exceptions.py
+-rw-rw-rw-   0        0        0     2004 2023-07-07 16:54:00.000000 pydeezer_asy-2.2.6/deezer_asy/util.py
+drwxrwxrwx   0        0        0        0 2023-08-04 15:38:41.220923 pydeezer_asy-2.2.6/pydeezer_asy.egg-info/
+-rw-rw-rw-   0        0        0     3743 2023-08-04 15:38:40.000000 pydeezer_asy-2.2.6/pydeezer_asy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      569 2023-08-04 15:38:40.000000 pydeezer_asy-2.2.6/pydeezer_asy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 15:38:40.000000 pydeezer_asy-2.2.6/pydeezer_asy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-08-04 15:38:40.000000 pydeezer_asy-2.2.6/pydeezer_asy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-08-04 15:38:40.000000 pydeezer_asy-2.2.6/pydeezer_asy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-04 15:38:41.225470 pydeezer_asy-2.2.6/setup.cfg
+-rw-rw-rw-   0        0        0      774 2023-08-04 15:38:28.000000 pydeezer_asy-2.2.6/setup.py
```

### Comparing `pydeezer_asy-2.2.5/PKG-INFO` & `pydeezer_asy-2.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydeezer_asy
-Version: 2.2.5
+Version: 2.2.6
 Summary: Asynchronous version of the `py-deezer` module
 Home-page: https://github.com/drhspfn/deezer-asy
 Author: drhspfn
 Author-email: drhspfn@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -78,15 +78,15 @@
 if __name__ == "__main__":
     loop.run_until_complete(main())
 ```
 
 
 ### Usage aioDeezer
 ```python
-from deezer_asy import DeezerAsy
+from deezer_asy import aioDeezer
 import logging
 import asyncio
 
 
 ARL = "edit this"
 loop = asyncio.get_event_loop()
 aio_session = aiohttp.ClientSession()
```

### Comparing `pydeezer_asy-2.2.5/README.md` & `pydeezer_asy-2.2.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 if __name__ == "__main__":
     loop.run_until_complete(main())
 ```
 
 
 ### Usage aioDeezer
 ```python
-from deezer_asy import DeezerAsy
+from deezer_asy import aioDeezer
 import logging
 import asyncio
 
 
 ARL = "edit this"
 loop = asyncio.get_event_loop()
 aio_session = aiohttp.ClientSession()
```

### Comparing `pydeezer_asy-2.2.5/deezer_asy/DeezerAsy.py` & `pydeezer_asy-2.2.6/deezer_asy/DeezerAsy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Standard Library
 import hashlib
 from os import path, remove
 import logging
 
+from threading import Thread
 # External Libraries
 import aiohttp
 import asyncio
 import aiofiles
 import httpx
 from yarl import URL
 from cryptography.hazmat.backends import default_backend
@@ -871,10 +872,13 @@
             cover_handle.save(_path)
     async def _write_mp3_tags(self, path, track, tags=None):
         track = track["DATA"] if "DATA" in track else track
 
         if not tags:
             tags = await self.get_track_tags(track)
 
-        _ = await self.loop.run_in_executor(None, self.__update_mp3, path, tags)
 
+        thread = Thread(target=self.__update_mp3, args=(path, tags,))
+
+        thread.start()
+        thread.join()
         return True
```

### Comparing `pydeezer_asy-2.2.5/deezer_asy/aiodeezer.py` & `pydeezer_asy-2.2.6/deezer_asy/aiodeezer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Standard Library
 import hashlib
 from os import path, remove
 import logging
 
+from threading import Thread
 # External Libraries
 import aiohttp
 import asyncio
 import aiofiles
 import httpx
 from yarl import URL
 from cryptography.hazmat.backends import default_backend
@@ -819,16 +820,20 @@
             cover_handle.save(_path)
     async def _write_mp3_tags(self, path, track, tags=None):
         track = track["DATA"] if "DATA" in track else track
 
         if not tags:
             tags = await self.get_track_tags(track)
 
-        _ = await self.loop.run_in_executor(None, self.__update_mp3, path, tags)
 
+    
+        thread = Thread(target=self.__update_mp3, args=(path, tags,))
+
+        thread.start()
+        thread.join()
         return True
```

### Comparing `pydeezer_asy-2.2.5/deezer_asy/constants/api_methods.py` & `pydeezer_asy-2.2.6/deezer_asy/constants/api_methods.py`

 * *Files identical despite different names*

### Comparing `pydeezer_asy-2.2.5/deezer_asy/constants/track_formats.py` & `pydeezer_asy-2.2.6/deezer_asy/constants/track_formats.py`

 * *Files identical despite different names*

### Comparing `pydeezer_asy-2.2.5/deezer_asy/util.py` & `pydeezer_asy-2.2.6/deezer_asy/util.py`

 * *Files identical despite different names*

### Comparing `pydeezer_asy-2.2.5/pydeezer_asy.egg-info/PKG-INFO` & `pydeezer_asy-2.2.6/pydeezer_asy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydeezer-asy
-Version: 2.2.5
+Version: 2.2.6
 Summary: Asynchronous version of the `py-deezer` module
 Home-page: https://github.com/drhspfn/deezer-asy
 Author: drhspfn
 Author-email: drhspfn@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -78,15 +78,15 @@
 if __name__ == "__main__":
     loop.run_until_complete(main())
 ```
 
 
 ### Usage aioDeezer
 ```python
-from deezer_asy import DeezerAsy
+from deezer_asy import aioDeezer
 import logging
 import asyncio
 
 
 ARL = "edit this"
 loop = asyncio.get_event_loop()
 aio_session = aiohttp.ClientSession()
```

### Comparing `pydeezer_asy-2.2.5/pydeezer_asy.egg-info/SOURCES.txt` & `pydeezer_asy-2.2.6/pydeezer_asy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydeezer_asy-2.2.5/setup.py` & `pydeezer_asy-2.2.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name='pydeezer_asy',
-    version='2.2.5',
+    version='2.2.6',
     description='Asynchronous version of the `py-deezer` module',
     author='drhspfn',
     author_email="drhspfn@gmail.com",
     packages=setuptools.find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/drhspfn/deezer-asy",
```

