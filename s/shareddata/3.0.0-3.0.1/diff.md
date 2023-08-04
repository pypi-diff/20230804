# Comparing `tmp/shareddata-3.0.0.tar.gz` & `tmp/shareddata-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shareddata-3.0.0.tar", last modified: Thu Aug  3 11:08:10 2023, max compression
+gzip compressed data, was "shareddata-3.0.1.tar", last modified: Thu Aug  3 12:31:00 2023, max compression
```

## Comparing `shareddata-3.0.0.tar` & `shareddata-3.0.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-03 11:08:10.943004 shareddata-3.0.0/
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    35149 2023-06-24 22:46:48.000000 shareddata-3.0.0/LICENSE
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1166 2023-08-03 11:08:10.943004 shareddata-3.0.0/PKG-INFO
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      611 2023-06-25 11:52:46.000000 shareddata-3.0.0/README.md
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      103 2023-06-24 22:46:48.000000 shareddata-3.0.0/pyproject.toml
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      894 2023-08-03 11:08:10.943004 shareddata-3.0.0/setup.cfg
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-03 11:08:10.943004 shareddata-3.0.0/src/
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-03 11:08:10.943004 shareddata-3.0.0/src/SharedData/
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    14294 2023-08-01 11:14:58.000000 shareddata-3.0.0/src/SharedData/AWSKinesis.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     5533 2023-08-01 11:14:58.000000 shareddata-3.0.0/src/SharedData/AWSS3.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    10577 2023-08-03 10:07:54.000000 shareddata-3.0.0/src/SharedData/DataFrame.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1514 2023-08-01 11:14:58.000000 shareddata-3.0.0/src/SharedData/Defaults.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     4284 2023-08-01 11:14:58.000000 shareddata-3.0.0/src/SharedData/Logger.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1272 2023-08-01 11:14:58.000000 shareddata-3.0.0/src/SharedData/LoggerConsumerProcess.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    11236 2023-08-01 11:14:58.000000 shareddata-3.0.0/src/SharedData/Metadata.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     4251 2023-08-02 08:56:01.000000 shareddata-3.0.0/src/SharedData/MultiProc.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     8428 2023-08-03 11:07:23.000000 shareddata-3.0.0/src/SharedData/RealTime.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     7485 2023-08-03 10:08:20.000000 shareddata-3.0.0/src/SharedData/SharedData.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     9244 2023-08-03 10:09:20.000000 shareddata-3.0.0/src/SharedData/SharedNumpy.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    30749 2023-08-03 10:04:28.000000 shareddata-3.0.0/src/SharedData/Table.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     8672 2023-08-02 13:49:16.000000 shareddata-3.0.0/src/SharedData/TableIndex.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    18035 2023-08-01 11:14:58.000000 shareddata-3.0.0/src/SharedData/TableIndexJit.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    13186 2023-08-03 10:08:05.000000 shareddata-3.0.0/src/SharedData/TimeSeries.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    16371 2023-08-01 11:14:58.000000 shareddata-3.0.0/src/SharedData/TimeseriesContainer.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1391 2023-07-29 18:49:47.000000 shareddata-3.0.0/src/SharedData/Utils.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        0 2023-06-24 22:46:48.000000 shareddata-3.0.0/src/SharedData/__init__.py
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-03 11:08:10.943004 shareddata-3.0.0/src/shareddata.egg-info/
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1166 2023-08-03 11:08:10.000000 shareddata-3.0.0/src/shareddata.egg-info/PKG-INFO
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      748 2023-08-03 11:08:10.000000 shareddata-3.0.0/src/shareddata.egg-info/SOURCES.txt
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        1 2023-08-03 11:08:10.000000 shareddata-3.0.0/src/shareddata.egg-info/dependency_links.txt
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      183 2023-08-03 11:08:10.000000 shareddata-3.0.0/src/shareddata.egg-info/requires.txt
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)       11 2023-08-03 11:08:10.000000 shareddata-3.0.0/src/shareddata.egg-info/top_level.txt
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-03 12:31:00.846447 shareddata-3.0.1/
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    35149 2023-06-24 22:46:48.000000 shareddata-3.0.1/LICENSE
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1166 2023-08-03 12:31:00.846447 shareddata-3.0.1/PKG-INFO
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      611 2023-06-25 11:52:46.000000 shareddata-3.0.1/README.md
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      103 2023-06-24 22:46:48.000000 shareddata-3.0.1/pyproject.toml
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      894 2023-08-03 12:31:00.846447 shareddata-3.0.1/setup.cfg
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-03 12:31:00.846447 shareddata-3.0.1/src/
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-03 12:31:00.846447 shareddata-3.0.1/src/SharedData/
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    14294 2023-08-01 11:14:58.000000 shareddata-3.0.1/src/SharedData/AWSKinesis.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     5533 2023-08-01 11:14:58.000000 shareddata-3.0.1/src/SharedData/AWSS3.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    10577 2023-08-03 11:10:47.000000 shareddata-3.0.1/src/SharedData/DataFrame.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1514 2023-08-01 11:14:58.000000 shareddata-3.0.1/src/SharedData/Defaults.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     4284 2023-08-01 11:14:58.000000 shareddata-3.0.1/src/SharedData/Logger.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1272 2023-08-01 11:14:58.000000 shareddata-3.0.1/src/SharedData/LoggerConsumerProcess.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    11236 2023-08-01 11:14:58.000000 shareddata-3.0.1/src/SharedData/Metadata.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     4251 2023-08-03 11:10:47.000000 shareddata-3.0.1/src/SharedData/MultiProc.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     8297 2023-08-03 12:30:32.000000 shareddata-3.0.1/src/SharedData/RealTime.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     7485 2023-08-03 11:10:47.000000 shareddata-3.0.1/src/SharedData/SharedData.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     9244 2023-08-03 11:10:47.000000 shareddata-3.0.1/src/SharedData/SharedNumpy.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    30749 2023-08-03 11:10:47.000000 shareddata-3.0.1/src/SharedData/Table.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     8672 2023-08-02 13:49:16.000000 shareddata-3.0.1/src/SharedData/TableIndex.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    18035 2023-08-01 11:14:58.000000 shareddata-3.0.1/src/SharedData/TableIndexJit.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    13186 2023-08-03 11:10:47.000000 shareddata-3.0.1/src/SharedData/TimeSeries.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    16371 2023-08-01 11:14:58.000000 shareddata-3.0.1/src/SharedData/TimeseriesContainer.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1391 2023-07-29 18:49:47.000000 shareddata-3.0.1/src/SharedData/Utils.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        0 2023-06-24 22:46:48.000000 shareddata-3.0.1/src/SharedData/__init__.py
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-03 12:31:00.846447 shareddata-3.0.1/src/shareddata.egg-info/
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1166 2023-08-03 12:31:00.000000 shareddata-3.0.1/src/shareddata.egg-info/PKG-INFO
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      748 2023-08-03 12:31:00.000000 shareddata-3.0.1/src/shareddata.egg-info/SOURCES.txt
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        1 2023-08-03 12:31:00.000000 shareddata-3.0.1/src/shareddata.egg-info/dependency_links.txt
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      183 2023-08-03 12:31:00.000000 shareddata-3.0.1/src/shareddata.egg-info/requires.txt
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)       11 2023-08-03 12:31:00.000000 shareddata-3.0.1/src/shareddata.egg-info/top_level.txt
```

### Comparing `shareddata-3.0.0/LICENSE` & `shareddata-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `shareddata-3.0.0/PKG-INFO` & `shareddata-3.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shareddata
-Version: 3.0.0
+Version: 3.0.1
 Summary: Shared Memory Database with S3 repository
 Home-page: https://github.com/jcarlitooliveira/SharedData
 Author: Jose Carlito de Oliveira Filho
 Author-email: jcarlitooliveira@gmail.com
 Project-URL: Bug Tracker, https://github.com/jcarlitooliveira/SharedData/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shareddata-3.0.0/README.md` & `shareddata-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `shareddata-3.0.0/setup.cfg` & `shareddata-3.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = shareddata
-version = 3.0.0
+version = 3.0.1
 author = Jose Carlito de Oliveira Filho
 author_email = jcarlitooliveira@gmail.com
 description = Shared Memory Database with S3 repository
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/jcarlitooliveira/SharedData
 project_urls =
```

### Comparing `shareddata-3.0.0/src/SharedData/AWSKinesis.py` & `shareddata-3.0.1/src/SharedData/AWSKinesis.py`

 * *Files identical despite different names*

### Comparing `shareddata-3.0.0/src/SharedData/AWSS3.py` & `shareddata-3.0.1/src/SharedData/AWSS3.py`

 * *Files identical despite different names*

### Comparing `shareddata-3.0.0/src/SharedData/DataFrame.py` & `shareddata-3.0.1/src/SharedData/DataFrame.py`

 * *Files identical despite different names*

### Comparing `shareddata-3.0.0/src/SharedData/Defaults.py` & `shareddata-3.0.1/src/SharedData/Defaults.py`

 * *Files identical despite different names*

### Comparing `shareddata-3.0.0/src/SharedData/Logger.py` & `shareddata-3.0.1/src/SharedData/Logger.py`

 * *Files identical despite different names*

### Comparing `shareddata-3.0.0/src/SharedData/LoggerConsumerProcess.py` & `shareddata-3.0.1/src/SharedData/LoggerConsumerProcess.py`

 * *Files identical despite different names*

### Comparing `shareddata-3.0.0/src/SharedData/Metadata.py` & `shareddata-3.0.1/src/SharedData/Metadata.py`

 * *Files identical despite different names*

### Comparing `shareddata-3.0.0/src/SharedData/MultiProc.py` & `shareddata-3.0.1/src/SharedData/MultiProc.py`

 * *Files identical despite different names*

### Comparing `shareddata-3.0.0/src/SharedData/RealTime.py` & `shareddata-3.0.1/src/SharedData/RealTime.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,15 +110,15 @@
                             ids2send = np.unique(ids2send)
                             ids2send = np.sort(ids2send)
                             maxrows = sockdata['maxrows']
                             rows2send = len(ids2send)
                             sentrows = 0
                             while sentrows<rows2send:
                                 msgsize = min(maxrows,rows2send)
-                                msg = table[ids2send[sentrows:msgsize]].tobytes()
+                                msg = table[ids2send[sentrows:sentrows+msgsize]].tobytes()
                                 conn.sendall(msg)
                                 sentrows+=msgsize
                             sockdata['watchdog']=time.time_ns() # clear watchdog
                                 
                     time.sleep(0.0001)
                 except Exception as e:
                     Logger.log.error('Client {addr} disconnected with error:%s' % (e))
@@ -128,18 +128,14 @@
                 RealTime.clients.pop(conn)
             Logger.log.info(f"Client {addr} disconnected.")
             conn.close()
 
     @staticmethod
     def table_subscribe_thread(table,host,port):
 
-        # host = '18.205.153.215'
-        # port = 10150
-        # table = shdata.table('MarketData','S5','IBKR','20230803',size=10000000)
-
         shnumpy = table.records
         buffsize = int(np.floor(1024/shnumpy.itemsize))*shnumpy.itemsize
         bytes_buffer = bytearray()
 
         while True:
             try:
                 client_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
```

### Comparing `shareddata-3.0.0/src/SharedData/SharedData.py` & `shareddata-3.0.1/src/SharedData/SharedData.py`

 * *Files identical despite different names*

### Comparing `shareddata-3.0.0/src/SharedData/SharedNumpy.py` & `shareddata-3.0.1/src/SharedData/SharedNumpy.py`

 * *Files identical despite different names*

### Comparing `shareddata-3.0.0/src/SharedData/Table.py` & `shareddata-3.0.1/src/SharedData/Table.py`

 * *Files identical despite different names*

### Comparing `shareddata-3.0.0/src/SharedData/TableIndex.py` & `shareddata-3.0.1/src/SharedData/TableIndex.py`

 * *Files identical despite different names*

### Comparing `shareddata-3.0.0/src/SharedData/TableIndexJit.py` & `shareddata-3.0.1/src/SharedData/TableIndexJit.py`

 * *Files identical despite different names*

### Comparing `shareddata-3.0.0/src/SharedData/TimeSeries.py` & `shareddata-3.0.1/src/SharedData/TimeSeries.py`

 * *Files identical despite different names*

### Comparing `shareddata-3.0.0/src/SharedData/TimeseriesContainer.py` & `shareddata-3.0.1/src/SharedData/TimeseriesContainer.py`

 * *Files identical despite different names*

### Comparing `shareddata-3.0.0/src/SharedData/Utils.py` & `shareddata-3.0.1/src/SharedData/Utils.py`

 * *Files identical despite different names*

### Comparing `shareddata-3.0.0/src/shareddata.egg-info/PKG-INFO` & `shareddata-3.0.1/src/shareddata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shareddata
-Version: 3.0.0
+Version: 3.0.1
 Summary: Shared Memory Database with S3 repository
 Home-page: https://github.com/jcarlitooliveira/SharedData
 Author: Jose Carlito de Oliveira Filho
 Author-email: jcarlitooliveira@gmail.com
 Project-URL: Bug Tracker, https://github.com/jcarlitooliveira/SharedData/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shareddata-3.0.0/src/shareddata.egg-info/SOURCES.txt` & `shareddata-3.0.1/src/shareddata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

