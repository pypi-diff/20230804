# Comparing `tmp/DmxOscServer-1.0.2.tar.gz` & `tmp/DmxOscServer-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/pi/Documents/DmxOscServer/dist/.tmp-k_s_joz3/DmxOscServer-1.0.2.tar", last modified: Wed Aug  2 17:06:11 2023, max compression
+gzip compressed data, was "/home/pi/Documents/DmxOscServer/dist/.tmp-oezfajnj/DmxOscServer-1.0.3.tar", last modified: Fri Aug  4 11:43:46 2023, max compression
```

## Comparing `DmxOscServer-1.0.2.tar` & `DmxOscServer-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-08-02 17:06:11.000000 DmxOscServer-1.0.2/
--rw-r--r--   0 pi        (1000) pi        (1000)     2266 2023-08-02 17:06:11.000000 DmxOscServer-1.0.2/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)     1830 2023-08-02 17:03:56.000000 DmxOscServer-1.0.2/README.md
--rw-r--r--   0 pi        (1000) pi        (1000)       78 2023-08-02 17:06:11.000000 DmxOscServer-1.0.2/setup.cfg
--rw-r--r--   0 pi        (1000) pi        (1000)      865 2023-08-02 16:30:11.000000 DmxOscServer-1.0.2/setup.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-08-02 17:06:11.000000 DmxOscServer-1.0.2/src/
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-08-02 17:06:11.000000 DmxOscServer-1.0.2/src/DmxOscServer/
--rw-r--r--   0 pi        (1000) pi        (1000)     4162 2023-08-02 16:47:34.000000 DmxOscServer-1.0.2/src/DmxOscServer/DmxOscServer.py
--rw-r--r--   0 pi        (1000) pi        (1000)     1609 2023-07-31 17:31:17.000000 DmxOscServer-1.0.2/src/DmxOscServer/Fixture.py
--rw-r--r--   0 pi        (1000) pi        (1000)       68 2023-07-30 18:25:02.000000 DmxOscServer-1.0.2/src/DmxOscServer/__init__.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-08-02 17:06:11.000000 DmxOscServer-1.0.2/src/DmxOscServer.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)     2266 2023-08-02 17:06:11.000000 DmxOscServer-1.0.2/src/DmxOscServer.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      317 2023-08-02 17:06:11.000000 DmxOscServer-1.0.2/src/DmxOscServer.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-08-02 17:06:11.000000 DmxOscServer-1.0.2/src/DmxOscServer.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       11 2023-08-02 17:06:11.000000 DmxOscServer-1.0.2/src/DmxOscServer.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       13 2023-08-02 17:06:11.000000 DmxOscServer-1.0.2/src/DmxOscServer.egg-info/top_level.txt
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-08-04 11:43:46.000000 DmxOscServer-1.0.3/
+-rw-r--r--   0 pi        (1000) pi        (1000)     3375 2023-08-04 11:43:46.000000 DmxOscServer-1.0.3/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)     2939 2023-08-04 11:08:49.000000 DmxOscServer-1.0.3/README.md
+-rw-r--r--   0 pi        (1000) pi        (1000)       78 2023-08-04 11:43:46.000000 DmxOscServer-1.0.3/setup.cfg
+-rw-r--r--   0 pi        (1000) pi        (1000)      865 2023-08-04 11:31:21.000000 DmxOscServer-1.0.3/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-08-04 11:43:46.000000 DmxOscServer-1.0.3/src/
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-08-04 11:43:46.000000 DmxOscServer-1.0.3/src/DmxOscServer/
+-rw-r--r--   0 pi        (1000) pi        (1000)     5154 2023-08-04 11:39:51.000000 DmxOscServer-1.0.3/src/DmxOscServer/DmxOscServer.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     2206 2023-08-04 11:28:22.000000 DmxOscServer-1.0.3/src/DmxOscServer/Fixture.py
+-rw-r--r--   0 pi        (1000) pi        (1000)       68 2023-07-30 18:25:02.000000 DmxOscServer-1.0.3/src/DmxOscServer/__init__.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-08-04 11:43:46.000000 DmxOscServer-1.0.3/src/DmxOscServer.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)     3375 2023-08-04 11:43:46.000000 DmxOscServer-1.0.3/src/DmxOscServer.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      317 2023-08-04 11:43:46.000000 DmxOscServer-1.0.3/src/DmxOscServer.egg-info/SOURCES.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-08-04 11:43:46.000000 DmxOscServer-1.0.3/src/DmxOscServer.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       11 2023-08-04 11:43:46.000000 DmxOscServer-1.0.3/src/DmxOscServer.egg-info/requires.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       13 2023-08-04 11:43:46.000000 DmxOscServer-1.0.3/src/DmxOscServer.egg-info/top_level.txt
```

### Comparing `DmxOscServer-1.0.2/PKG-INFO` & `DmxOscServer-1.0.3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: DmxOscServer
-Version: 1.0.2
-Summary: A Python Lib to create a DMX compatible OSC server with handlers
-Home-page: https://dmxoscserver.readthedocs.io/en/latest/
-Author: Miniontoby
-Project-URL: Bug Reports, https://github.com/Miniontoby/DmxOscServer/issues
-Project-URL: Source, https://github.com/Miniontoby/DmxOscServer
-Keywords: dmx,osc,server
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
-
 # DMX OSC Server
 
 DMX OSC Server is a python lib to make it easier to create OSC Servers for the DMX Protocol.
 
 It allows you to register fixtures are the wanted universe, starting address and channels.
 You will also be able to add an handler which will be called when a message is received for that fixture.
 
@@ -32,36 +20,43 @@
 from DmxOscServer import DmxOscServer
 
 server = DmxOscServer()
 
 # Define a 3 channel Fixture at address 0 at universe 0 which will execute my_rgb_handler when called
 @server.define_fixture(0, 0, 3)
 def my_rgb_handler(fixture, address, *args):
-    fixture.values[address] = args[0]
-    print (fixture.values)
+    print ("{} got {}".format(address, args))
 
 server.run()
 ```
 
+To make the define more readable, you can use the argument names
+
+```py
+# Define a 3 channel Fixture at address 0 at universe 0 which will execute my_rgb_handler when called
+@server.define_fixture(universe=0, starting_addr=0, channels=3)
+def my_rgb_handler(fixture, address, *args):
+    print ("{} has been set to {}".format(address, args))
+```
+
 
 To change the IP and/or port, you can specify that at the `.run()` method
 
 ```py
 server.run("10.10.123.5", 1234) # Will listen on 10.10.123.5:1234
 ```
 
 
 It is also possible to use the `Fixture` class and the `add_fixture` method
 
 ```py
 from DmxOscServer import DmxOscServer, Fixture
 
 def my_rgb_handler(fixture, address, *args):
-    fixture.values[address] = args[0]
-    print (fixture.values)
+    print ("{} has been set to {}".format(address, args))
 
 server = DmxOscServer()
 server.add_fixture(Fixture(0, 0, 3, my_rgb_handler)) # Register a 3 channel Fixture at address 0 at universe 0
 ```
 
 
 And for the `add_fixture` method, you can also add multiple fixtures at once using:
@@ -72,10 +67,29 @@
 server.add_fixtures(
     Fixture(0, 0, 3, my_rgb_handler), # Register a 3 channel Fixture at address 0 of universe 0
     Fixture(0, 3, 3, my_rgb_handler), # Register a 3 channel Fixture at address 3 of universe 0
 )
 ```
 
 
+You can use the `fixture.values` property to see all the current values
+
+```py
+@server.define_fixture(0, 0, 3)
+def my_rgb_handler(fixture, address, *args):
+    print (fixture.values)
+```
+
+
+# The handler
+
+The handler receives a call when a message is received for that fixture
+Arguments: `(fixture, address, *args)`
+- `fixture` is the fixture, so you have a reference
+- `address` is the message address (it starts at the starting_address, so use `address - fixture.starting_addr` if you want to have the internal address)
+- `*args` are the args of the message. It is almost always 1 int going from 0 to 1, so you can just use `args[0]` in your code and multiply it by your max value
+
+The handler should never receive an address out of its address range, if the fixture is called correctly
+
 # More Documentation
 
 More Documentation can be found at https://dmxoscserver.readthedocs.io/en/latest/
```

### Comparing `DmxOscServer-1.0.2/setup.py` & `DmxOscServer-1.0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="DmxOscServer",
-    version="1.0.2",
+    version="1.0.3",
     description="A Python Lib to create a DMX compatible OSC server with handlers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://dmxoscserver.readthedocs.io/en/latest/",
     author="Miniontoby",
     keywords="dmx, osc, server",
     package_dir={"": "src"},
```

### Comparing `DmxOscServer-1.0.2/src/DmxOscServer/Fixture.py` & `DmxOscServer-1.0.3/src/DmxOscServer/Fixture.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,63 @@
 # Fixture Default Class
 
 class Fixture():
   """
   Instantiate a Fixture
 
-  :param universe: The universe for this Fixture
-  :type universe: int
-  :param starting_addr: The starting address for this Fixture
-  :type starting_addr: int
-  :param channels: The amount of channel that this Fixture should have
-  :type channels: int
+  :param int universe: The universe for this Fixture
+  :param int starting_addr: The starting address for this Fixture
+  :param int channels: The amount of channel that this Fixture should have
   :param handler: The callback function be to called when a message is received for this address
   :type handler: function
   """
   def __init__(self, universe, starting_addr, channels, handler):
     self.universe = universe
     self.starting_addr = starting_addr
     self.channels = channels
     self.end_addr = starting_addr + channels
-    self.handler = handler
+    self.address_range = range(self.starting_addr, self.end_addr)
+    self._handler = handler
     self.values = [0] * channels
 
   def __call__(self, address: int, *args):
     """
     Makes the Fixture callable for the server
 
-    :param address: The address of this Fixture that was called
-    :type address: int
+    :param int address: The address of this Fixture that was called
     :param *args: The arguments sent by the OSC Client
+    :raises ValueError: If the address is not within range
+
+    :returns: The result from the handler function
     """
-    return self.handler(self, address, *args)
+    # Set the values property
+    if address in self:
+      self.values[address - self.starting_addr] = args[0]
+      return self._handler(self, address, *args)
+    else:
+      raise ValueError("Address {} is not within the address range!".format(address))
 
   def __contains__(self, addr: int):
     """
     Checks if the address is in this Fixture's address range
 
-    :param addr: The address to look for
-    :type addr: int
+    :param int addr: The address to look for
 
     :returns: True if the address is within this Fixture's address
+    :rtype: bool
     """
-    return addr in range(self.starting_addr, self.end_addr)
+    return addr in self.address_range
 
   def __str__(self):
     """
     This will be used as the template when printing the Fixture object
 
     :returns: The Fixture class as a string
+    :rtype: str
     """
     return 'Fixture(universe={0.universe}, starting_addr={0.starting_addr}, channels={0.channels}, values={0.values})'.format(self)
+
+  def __setattr__(self, name, value):
+    if name not in ["universe","starting_addr","channels","end_addr","address_range","handler","values"]: pass
+    elif name not in self.__dict__: pass
+    else: raise AttributeError("Can't modify {}".format(name))
+    super().__setattr__(name, value)
```

### Comparing `DmxOscServer-1.0.2/src/DmxOscServer.egg-info/PKG-INFO` & `DmxOscServer-1.0.3/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DmxOscServer
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Python Lib to create a DMX compatible OSC server with handlers
 Home-page: https://dmxoscserver.readthedocs.io/en/latest/
 Author: Miniontoby
 Project-URL: Bug Reports, https://github.com/Miniontoby/DmxOscServer/issues
 Project-URL: Source, https://github.com/Miniontoby/DmxOscServer
 Keywords: dmx,osc,server
 Requires-Python: >=3.5
@@ -32,36 +32,43 @@
 from DmxOscServer import DmxOscServer
 
 server = DmxOscServer()
 
 # Define a 3 channel Fixture at address 0 at universe 0 which will execute my_rgb_handler when called
 @server.define_fixture(0, 0, 3)
 def my_rgb_handler(fixture, address, *args):
-    fixture.values[address] = args[0]
-    print (fixture.values)
+    print ("{} got {}".format(address, args))
 
 server.run()
 ```
 
+To make the define more readable, you can use the argument names
+
+```py
+# Define a 3 channel Fixture at address 0 at universe 0 which will execute my_rgb_handler when called
+@server.define_fixture(universe=0, starting_addr=0, channels=3)
+def my_rgb_handler(fixture, address, *args):
+    print ("{} has been set to {}".format(address, args))
+```
+
 
 To change the IP and/or port, you can specify that at the `.run()` method
 
 ```py
 server.run("10.10.123.5", 1234) # Will listen on 10.10.123.5:1234
 ```
 
 
 It is also possible to use the `Fixture` class and the `add_fixture` method
 
 ```py
 from DmxOscServer import DmxOscServer, Fixture
 
 def my_rgb_handler(fixture, address, *args):
-    fixture.values[address] = args[0]
-    print (fixture.values)
+    print ("{} has been set to {}".format(address, args))
 
 server = DmxOscServer()
 server.add_fixture(Fixture(0, 0, 3, my_rgb_handler)) # Register a 3 channel Fixture at address 0 at universe 0
 ```
 
 
 And for the `add_fixture` method, you can also add multiple fixtures at once using:
@@ -72,10 +79,29 @@
 server.add_fixtures(
     Fixture(0, 0, 3, my_rgb_handler), # Register a 3 channel Fixture at address 0 of universe 0
     Fixture(0, 3, 3, my_rgb_handler), # Register a 3 channel Fixture at address 3 of universe 0
 )
 ```
 
 
+You can use the `fixture.values` property to see all the current values
+
+```py
+@server.define_fixture(0, 0, 3)
+def my_rgb_handler(fixture, address, *args):
+    print (fixture.values)
+```
+
+
+# The handler
+
+The handler receives a call when a message is received for that fixture
+Arguments: `(fixture, address, *args)`
+- `fixture` is the fixture, so you have a reference
+- `address` is the message address (it starts at the starting_address, so use `address - fixture.starting_addr` if you want to have the internal address)
+- `*args` are the args of the message. It is almost always 1 int going from 0 to 1, so you can just use `args[0]` in your code and multiply it by your max value
+
+The handler should never receive an address out of its address range, if the fixture is called correctly
+
 # More Documentation
 
 More Documentation can be found at https://dmxoscserver.readthedocs.io/en/latest/
```

