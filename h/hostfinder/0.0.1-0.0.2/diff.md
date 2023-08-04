# Comparing `tmp/hostfinder-0.0.1.tar.gz` & `tmp/hostfinder-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hostfinder-0.0.1.tar", last modified: Thu Aug  3 14:00:22 2023, max compression
+gzip compressed data, was "hostfinder-0.0.2.tar", last modified: Fri Aug  4 21:55:06 2023, max compression
```

## Comparing `hostfinder-0.0.1.tar` & `hostfinder-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:00:22.204354 hostfinder-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-03 14:00:08.000000 hostfinder-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-08-03 14:00:22.204354 hostfinder-0.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:00:22.204354 hostfinder-0.0.1/hostfinder/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-08-03 14:00:08.000000 hostfinder-0.0.1/hostfinder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-08-03 14:00:08.000000 hostfinder-0.0.1/hostfinder/hostfinder.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-08-03 14:00:08.000000 hostfinder-0.0.1/hostfinder/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:00:22.204354 hostfinder-0.0.1/hostfinder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-08-03 14:00:22.000000 hostfinder-0.0.1/hostfinder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-08-03 14:00:22.000000 hostfinder-0.0.1/hostfinder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 14:00:22.000000 hostfinder-0.0.1/hostfinder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-03 14:00:22.000000 hostfinder-0.0.1/hostfinder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-03 14:00:22.000000 hostfinder-0.0.1/hostfinder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-03 14:00:22.000000 hostfinder-0.0.1/hostfinder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-08-03 14:00:08.000000 hostfinder-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 14:00:22.204354 hostfinder-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:00:22.204354 hostfinder-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-08-03 14:00:08.000000 hostfinder-0.0.1/tests/test_finder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:55:06.085339 hostfinder-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 21:54:55.000000 hostfinder-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-08-04 21:55:06.085339 hostfinder-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-08-04 21:54:55.000000 hostfinder-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:55:06.081339 hostfinder-0.0.2/hostfinder/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-08-04 21:54:55.000000 hostfinder-0.0.2/hostfinder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-08-04 21:54:55.000000 hostfinder-0.0.2/hostfinder/hostfinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-08-04 21:54:55.000000 hostfinder-0.0.2/hostfinder/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:55:06.081339 hostfinder-0.0.2/hostfinder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-08-04 21:55:06.000000 hostfinder-0.0.2/hostfinder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-08-04 21:55:06.000000 hostfinder-0.0.2/hostfinder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 21:55:06.000000 hostfinder-0.0.2/hostfinder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-04 21:55:06.000000 hostfinder-0.0.2/hostfinder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-04 21:55:06.000000 hostfinder-0.0.2/hostfinder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-04 21:55:06.000000 hostfinder-0.0.2/hostfinder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-08-04 21:54:55.000000 hostfinder-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 21:55:06.085339 hostfinder-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:55:06.081339 hostfinder-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-08-04 21:54:55.000000 hostfinder-0.0.2/tests/test_finder.py
```

### Comparing `hostfinder-0.0.1/LICENSE` & `hostfinder-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hostfinder-0.0.1/hostfinder/hostfinder.py` & `hostfinder-0.0.2/hostfinder/hostfinder.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import psutil
 
 
 @dataclass
 class HostFinder:
     port: int = 22
-    loopback_address: str = "127.0.0.1"
+    loopback_name: str = "lo"
     timeout: int = 10
 
     def __post_init__(self):
         socket.setdefaulttimeout(self.timeout)
 
     def generate_hosts(self):
         possible_hosts = self.local_subnet_addresses()
@@ -22,26 +22,26 @@
         executor = concurrent.futures.ThreadPoolExecutor(max_workers=num_possible_hosts)
         with executor:
             results = executor.map(self.is_listening, possible_hosts)
             for result in results:
                 if result is not None:
                     yield result
 
-    def local_subnet_addresses(self):
+    def local_subnets(self):
         local_interfaces = psutil.net_if_addrs()
-        for subnets in local_interfaces.values():
-            for subnet in subnets:
-                is_valid = (
-                    subnet.family == socket.AF_INET
-                    and subnet.address != self.loopback_address
-                )
-                if is_valid:
-                    network_string = f"{subnet.address}/{subnet.netmask}"
-                    network = ipaddress.IPv4Network(network_string, strict=False)
-                    for address in network.hosts():
-                        yield str(address)
+        for interface_name, subnets in local_interfaces.items():
+            if interface_name != self.loopback_name:
+                yield from subnets
+
+    def local_subnet_addresses(self):
+        for subnet in self.local_subnets():
+            if subnet.family == socket.AF_INET:
+                network_string = f"{subnet.address}/{subnet.netmask}"
+                network = ipaddress.IPv4Network(network_string, strict=False)
+                for address in network.hosts():
+                    yield str(address)
 
     def is_listening(self, address: str):
         with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as sock:
             connection_result = sock.connect_ex((address, self.port))
         result = address if connection_result == 0 else None
         return result
```

### Comparing `hostfinder-0.0.1/hostfinder/main.py` & `hostfinder-0.0.2/hostfinder/main.py`

 * *Files identical despite different names*

### Comparing `hostfinder-0.0.1/pyproject.toml` & `hostfinder-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "hostfinder"
-version = "0.0.1"
+version = "0.0.2"
 description = "Find host in local subnet listening to specified port"
 authors = [{ name = "Quinten Roets", email = "qdr2104@columbia.edu" }]
 license = { text = "MIT" }
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = []
```

