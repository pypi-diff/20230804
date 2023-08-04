# Comparing `tmp/DmxOscServer-1.0.3.tar.gz` & `tmp/DmxOscServer-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/pi/Documents/DmxOscServer/dist/.tmp-oezfajnj/DmxOscServer-1.0.3.tar", last modified: Fri Aug  4 11:43:46 2023, max compression
+gzip compressed data, was "/home/pi/Documents/DmxOscServer/dist/.tmp-1h1xirwo/DmxOscServer-1.0.4.tar", last modified: Fri Aug  4 14:31:46 2023, max compression
```

## Comparing `DmxOscServer-1.0.3.tar` & `DmxOscServer-1.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-08-04 11:43:46.000000 DmxOscServer-1.0.3/
--rw-r--r--   0 pi        (1000) pi        (1000)     3375 2023-08-04 11:43:46.000000 DmxOscServer-1.0.3/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)     2939 2023-08-04 11:08:49.000000 DmxOscServer-1.0.3/README.md
--rw-r--r--   0 pi        (1000) pi        (1000)       78 2023-08-04 11:43:46.000000 DmxOscServer-1.0.3/setup.cfg
--rw-r--r--   0 pi        (1000) pi        (1000)      865 2023-08-04 11:31:21.000000 DmxOscServer-1.0.3/setup.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-08-04 11:43:46.000000 DmxOscServer-1.0.3/src/
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-08-04 11:43:46.000000 DmxOscServer-1.0.3/src/DmxOscServer/
--rw-r--r--   0 pi        (1000) pi        (1000)     5154 2023-08-04 11:39:51.000000 DmxOscServer-1.0.3/src/DmxOscServer/DmxOscServer.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2206 2023-08-04 11:28:22.000000 DmxOscServer-1.0.3/src/DmxOscServer/Fixture.py
--rw-r--r--   0 pi        (1000) pi        (1000)       68 2023-07-30 18:25:02.000000 DmxOscServer-1.0.3/src/DmxOscServer/__init__.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-08-04 11:43:46.000000 DmxOscServer-1.0.3/src/DmxOscServer.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)     3375 2023-08-04 11:43:46.000000 DmxOscServer-1.0.3/src/DmxOscServer.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      317 2023-08-04 11:43:46.000000 DmxOscServer-1.0.3/src/DmxOscServer.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-08-04 11:43:46.000000 DmxOscServer-1.0.3/src/DmxOscServer.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       11 2023-08-04 11:43:46.000000 DmxOscServer-1.0.3/src/DmxOscServer.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       13 2023-08-04 11:43:46.000000 DmxOscServer-1.0.3/src/DmxOscServer.egg-info/top_level.txt
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-08-04 14:31:46.000000 DmxOscServer-1.0.4/
+-rw-r--r--   0 pi        (1000) pi        (1000)     3375 2023-08-04 14:31:46.000000 DmxOscServer-1.0.4/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)     2939 2023-08-04 11:08:49.000000 DmxOscServer-1.0.4/README.md
+-rw-r--r--   0 pi        (1000) pi        (1000)       78 2023-08-04 14:31:46.000000 DmxOscServer-1.0.4/setup.cfg
+-rw-r--r--   0 pi        (1000) pi        (1000)      865 2023-08-04 14:31:16.000000 DmxOscServer-1.0.4/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-08-04 14:31:46.000000 DmxOscServer-1.0.4/src/
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-08-04 14:31:46.000000 DmxOscServer-1.0.4/src/DmxOscServer/
+-rw-r--r--   0 pi        (1000) pi        (1000)     5152 2023-08-04 14:29:12.000000 DmxOscServer-1.0.4/src/DmxOscServer/DmxOscServer.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     2206 2023-08-04 11:28:22.000000 DmxOscServer-1.0.4/src/DmxOscServer/Fixture.py
+-rw-r--r--   0 pi        (1000) pi        (1000)       68 2023-07-30 18:25:02.000000 DmxOscServer-1.0.4/src/DmxOscServer/__init__.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-08-04 14:31:46.000000 DmxOscServer-1.0.4/src/DmxOscServer.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)     3375 2023-08-04 14:31:46.000000 DmxOscServer-1.0.4/src/DmxOscServer.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      317 2023-08-04 14:31:46.000000 DmxOscServer-1.0.4/src/DmxOscServer.egg-info/SOURCES.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-08-04 14:31:46.000000 DmxOscServer-1.0.4/src/DmxOscServer.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       11 2023-08-04 14:31:46.000000 DmxOscServer-1.0.4/src/DmxOscServer.egg-info/requires.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       13 2023-08-04 14:31:46.000000 DmxOscServer-1.0.4/src/DmxOscServer.egg-info/top_level.txt
```

### Comparing `DmxOscServer-1.0.3/PKG-INFO` & `DmxOscServer-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DmxOscServer
-Version: 1.0.3
+Version: 1.0.4
 Summary: A Python Lib to create a DMX compatible OSC server with handlers
 Home-page: https://dmxoscserver.readthedocs.io/en/latest/
 Author: Miniontoby
 Project-URL: Bug Reports, https://github.com/Miniontoby/DmxOscServer/issues
 Project-URL: Source, https://github.com/Miniontoby/DmxOscServer
 Keywords: dmx,osc,server
 Requires-Python: >=3.5
```

### Comparing `DmxOscServer-1.0.3/README.md` & `DmxOscServer-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `DmxOscServer-1.0.3/setup.py` & `DmxOscServer-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="DmxOscServer",
-    version="1.0.3",
+    version="1.0.4",
     description="A Python Lib to create a DMX compatible OSC server with handlers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://dmxoscserver.readthedocs.io/en/latest/",
     author="Miniontoby",
     keywords="dmx, osc, server",
     package_dir={"": "src"},
```

### Comparing `DmxOscServer-1.0.3/src/DmxOscServer/DmxOscServer.py` & `DmxOscServer-1.0.4/src/DmxOscServer/DmxOscServer.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,16 +153,16 @@
     Start the server run
 
     Should be called always AFTER all fixtures are added
 
     :param str ip: The IP address to listen on
     :param int port: The Port to listen on
     """
-    self.__osc_server = ThreadingOSCUDPServer((ip, port), self.__dispatcher)
+    self.__osc_server = ThreadingOSCUDPServer((ip, port), self._dispatcher)
     print ("Serving on {}".format(self.__osc_server.server_address))
     self.__osc_server.serve_forever()
 
   def __setattr__(self, name, value):
-    if name not in ["__fixtures","__dispatcher","__osc_server"]: pass
+    if name not in ["__fixtures","_dispatcher","__osc_server"]: pass
     elif name not in self.__dict__: pass
     else: raise AttributeError("Can't modify {}".format(name))
     super().__setattr__(name, value)
```

### Comparing `DmxOscServer-1.0.3/src/DmxOscServer/Fixture.py` & `DmxOscServer-1.0.4/src/DmxOscServer/Fixture.py`

 * *Files identical despite different names*

### Comparing `DmxOscServer-1.0.3/src/DmxOscServer.egg-info/PKG-INFO` & `DmxOscServer-1.0.4/src/DmxOscServer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DmxOscServer
-Version: 1.0.3
+Version: 1.0.4
 Summary: A Python Lib to create a DMX compatible OSC server with handlers
 Home-page: https://dmxoscserver.readthedocs.io/en/latest/
 Author: Miniontoby
 Project-URL: Bug Reports, https://github.com/Miniontoby/DmxOscServer/issues
 Project-URL: Source, https://github.com/Miniontoby/DmxOscServer
 Keywords: dmx,osc,server
 Requires-Python: >=3.5
```

