# Comparing `tmp/TwitterHandler-1.1.0.tar.gz` & `tmp/TwitterHandler-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TwitterHandler-1.1.0.tar", last modified: Tue Jul 26 11:11:31 2022, max compression
+gzip compressed data, was "TwitterHandler-1.1.1.tar", last modified: Fri Aug  4 08:37:25 2023, max compression
```

## Comparing `TwitterHandler-1.1.0.tar` & `TwitterHandler-1.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 hassan    (1000) hassan    (1000)        0 2022-07-26 11:11:31.531937 TwitterHandler-1.1.0/
--rw-rw-r--   0 hassan    (1000) hassan    (1000)      103 2022-07-26 08:54:20.000000 TwitterHandler-1.1.0/MANIFEST.in
--rw-rw-r--   0 hassan    (1000) hassan    (1000)     1375 2022-07-26 11:11:31.531937 TwitterHandler-1.1.0/PKG-INFO
--rw-rw-r--   0 hassan    (1000) hassan    (1000)      658 2022-07-26 11:04:07.000000 TwitterHandler-1.1.0/README.md
-drwxrwxr-x   0 hassan    (1000) hassan    (1000)        0 2022-07-26 11:11:31.515937 TwitterHandler-1.1.0/TwitterHandler/
-drwxrwxr-x   0 hassan    (1000) hassan    (1000)        0 2022-07-26 11:11:31.531937 TwitterHandler-1.1.0/TwitterHandler/Kafka/
--rw-rw-r--   0 hassan    (1000) hassan    (1000)        0 2022-07-17 11:21:01.000000 TwitterHandler-1.1.0/TwitterHandler/Kafka/__init__.py
--rwxrwxr-x   0 hassan    (1000) hassan    (1000)     1665 2022-07-26 08:59:28.000000 TwitterHandler-1.1.0/TwitterHandler/Kafka/stream.py
--rw-rw-r--   0 hassan    (1000) hassan    (1000)        5 2022-07-26 11:10:25.000000 TwitterHandler-1.1.0/TwitterHandler/VERSION
--rw-rw-r--   0 hassan    (1000) hassan    (1000)        0 2022-07-17 11:21:01.000000 TwitterHandler-1.1.0/TwitterHandler/__init__.py
-drwxrwxr-x   0 hassan    (1000) hassan    (1000)        0 2022-07-26 11:11:31.531937 TwitterHandler-1.1.0/TwitterHandler.egg-info/
--rw-rw-r--   0 hassan    (1000) hassan    (1000)     1375 2022-07-26 11:11:31.000000 TwitterHandler-1.1.0/TwitterHandler.egg-info/PKG-INFO
--rw-rw-r--   0 hassan    (1000) hassan    (1000)      402 2022-07-26 11:11:31.000000 TwitterHandler-1.1.0/TwitterHandler.egg-info/SOURCES.txt
--rw-rw-r--   0 hassan    (1000) hassan    (1000)        1 2022-07-26 11:11:31.000000 TwitterHandler-1.1.0/TwitterHandler.egg-info/dependency_links.txt
--rw-rw-r--   0 hassan    (1000) hassan    (1000)        1 2022-07-21 12:38:52.000000 TwitterHandler-1.1.0/TwitterHandler.egg-info/not-zip-safe
--rw-rw-r--   0 hassan    (1000) hassan    (1000)       57 2022-07-26 11:11:31.000000 TwitterHandler-1.1.0/TwitterHandler.egg-info/requires.txt
--rw-rw-r--   0 hassan    (1000) hassan    (1000)       15 2022-07-26 11:11:31.000000 TwitterHandler-1.1.0/TwitterHandler.egg-info/top_level.txt
--rwxrwxr-x   0 hassan    (1000) hassan    (1000)      104 2022-07-17 11:21:01.000000 TwitterHandler-1.1.0/pyproject.toml
--rw-rw-r--   0 hassan    (1000) hassan    (1000)       57 2022-07-26 11:09:52.000000 TwitterHandler-1.1.0/requirements.txt
--rw-rw-r--   0 hassan    (1000) hassan    (1000)       38 2022-07-26 11:11:31.531937 TwitterHandler-1.1.0/setup.cfg
--rw-rw-r--   0 hassan    (1000) hassan    (1000)     1835 2022-07-17 11:21:01.000000 TwitterHandler-1.1.0/setup.py
+drwxrwxr-x   0 hassan    (1000) hassan    (1000)        0 2023-08-04 08:37:25.394587 TwitterHandler-1.1.1/
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)      103 2022-07-26 08:54:20.000000 TwitterHandler-1.1.1/MANIFEST.in
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)     1375 2023-08-04 08:37:25.394587 TwitterHandler-1.1.1/PKG-INFO
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)      658 2022-07-26 11:04:07.000000 TwitterHandler-1.1.1/README.md
+drwxrwxr-x   0 hassan    (1000) hassan    (1000)        0 2023-08-04 08:37:25.390587 TwitterHandler-1.1.1/TwitterHandler/
+drwxrwxr-x   0 hassan    (1000) hassan    (1000)        0 2023-08-04 08:37:25.394587 TwitterHandler-1.1.1/TwitterHandler/Kafka/
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)        0 2022-07-17 11:21:01.000000 TwitterHandler-1.1.1/TwitterHandler/Kafka/__init__.py
+-rwxrwxr-x   0 hassan    (1000) hassan    (1000)     1677 2023-08-04 08:32:08.000000 TwitterHandler-1.1.1/TwitterHandler/Kafka/stream.py
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)        5 2023-08-04 08:36:52.000000 TwitterHandler-1.1.1/TwitterHandler/VERSION
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)        0 2022-07-17 11:21:01.000000 TwitterHandler-1.1.1/TwitterHandler/__init__.py
+drwxrwxr-x   0 hassan    (1000) hassan    (1000)        0 2023-08-04 08:37:25.394587 TwitterHandler-1.1.1/TwitterHandler.egg-info/
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)     1375 2023-08-04 08:37:25.000000 TwitterHandler-1.1.1/TwitterHandler.egg-info/PKG-INFO
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)      402 2023-08-04 08:37:25.000000 TwitterHandler-1.1.1/TwitterHandler.egg-info/SOURCES.txt
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)        1 2023-08-04 08:37:25.000000 TwitterHandler-1.1.1/TwitterHandler.egg-info/dependency_links.txt
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)        1 2022-07-21 12:38:52.000000 TwitterHandler-1.1.1/TwitterHandler.egg-info/not-zip-safe
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)       57 2023-08-04 08:37:25.000000 TwitterHandler-1.1.1/TwitterHandler.egg-info/requires.txt
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)       15 2023-08-04 08:37:25.000000 TwitterHandler-1.1.1/TwitterHandler.egg-info/top_level.txt
+-rwxrwxr-x   0 hassan    (1000) hassan    (1000)      104 2022-07-17 11:21:01.000000 TwitterHandler-1.1.1/pyproject.toml
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)       57 2022-07-26 11:09:52.000000 TwitterHandler-1.1.1/requirements.txt
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)       38 2023-08-04 08:37:25.394587 TwitterHandler-1.1.1/setup.cfg
+-rw-rw-r--   0 hassan    (1000) hassan    (1000)     1835 2022-07-17 11:21:01.000000 TwitterHandler-1.1.1/setup.py
```

### Comparing `TwitterHandler-1.1.0/PKG-INFO` & `TwitterHandler-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TwitterHandler
-Version: 1.1.0
+Version: 1.1.1
 Summary: A simple Twitter handler for the Twitter API.
 Home-page: https://github.com/HassanRady/TwitterHandler
 Author: Hassan Rady
 Author-email: hassan.khaled.rady@gmail.com
 License: MIT license
 Keywords: Tweets
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: TwitterHandler Version: 1.1.0 Summary: A simple
+Metadata-Version: 2.1 Name: TwitterHandler Version: 1.1.1 Summary: A simple
 Twitter handler for the Twitter API. Home-page: https://github.com/HassanRady/
 TwitterHandler Author: Hassan Rady Author-email: hassan.khaled.rady@gmail.com
 License: MIT license Keywords: Tweets Classifier: Development Status :: 2 -
 Pre-Alpha Classifier: Intended Audience :: Developers Classifier: License ::
 OSI Approved :: MIT License Classifier: Natural Language :: English Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
```

### Comparing `TwitterHandler-1.1.0/README.md` & `TwitterHandler-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `TwitterHandler-1.1.0/TwitterHandler/Kafka/stream.py` & `TwitterHandler-1.1.1/TwitterHandler/Kafka/stream.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         # self.thread.join()
         pass
 
     def on_error(self, status_code):
         print(status_code)
 
 class Streamer:
-    def __init__(self, ):
+    def __init__(self, BEARER_TOKEN):
         producer = KafkaProducer(bootstrap_servers=f"{KAFKA_HOST}:{KAFKA_PORT}")
         self.streamer = TweetsStreamer(producer, bearer_token=BEARER_TOKEN)
         self.thread = None
 
     def delete_rules(self):
         rules = self.streamer.get_rules().data
         rules_list = []
```

### Comparing `TwitterHandler-1.1.0/TwitterHandler.egg-info/PKG-INFO` & `TwitterHandler-1.1.1/TwitterHandler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TwitterHandler
-Version: 1.1.0
+Version: 1.1.1
 Summary: A simple Twitter handler for the Twitter API.
 Home-page: https://github.com/HassanRady/TwitterHandler
 Author: Hassan Rady
 Author-email: hassan.khaled.rady@gmail.com
 License: MIT license
 Keywords: Tweets
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: TwitterHandler Version: 1.1.0 Summary: A simple
+Metadata-Version: 2.1 Name: TwitterHandler Version: 1.1.1 Summary: A simple
 Twitter handler for the Twitter API. Home-page: https://github.com/HassanRady/
 TwitterHandler Author: Hassan Rady Author-email: hassan.khaled.rady@gmail.com
 License: MIT license Keywords: Tweets Classifier: Development Status :: 2 -
 Pre-Alpha Classifier: Intended Audience :: Developers Classifier: License ::
 OSI Approved :: MIT License Classifier: Natural Language :: English Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
```

### Comparing `TwitterHandler-1.1.0/setup.py` & `TwitterHandler-1.1.1/setup.py`

 * *Files identical despite different names*

