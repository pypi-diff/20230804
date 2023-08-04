# Comparing `tmp/evque-1.3.0.tar.gz` & `tmp/evque-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evque-1.3.0.tar", last modified: Sat Jul 29 23:16:31 2023, max compression
+gzip compressed data, was "evque-1.4.0.tar", last modified: Fri Aug  4 12:07:16 2023, max compression
```

## Comparing `evque-1.3.0.tar` & `evque-1.4.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 23:16:31.381135 evque-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-07-29 23:16:12.000000 evque-1.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-07-29 23:16:31.381135 evque-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-07-29 23:16:12.000000 evque-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 23:16:31.381135 evque-1.3.0/evque/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-29 23:16:12.000000 evque-1.3.0/evque/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-07-29 23:16:12.000000 evque-1.3.0/evque/evque.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 23:16:31.381135 evque-1.3.0/evque.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-07-29 23:16:31.000000 evque-1.3.0/evque.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-29 23:16:31.000000 evque-1.3.0/evque.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 23:16:31.000000 evque-1.3.0/evque.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-29 23:16:31.000000 evque-1.3.0/evque.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 23:16:31.381135 evque-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-29 23:16:12.000000 evque-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:07:16.944875 evque-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-08-04 12:07:04.000000 evque-1.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-08-04 12:07:16.944875 evque-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-08-04 12:07:04.000000 evque-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:07:16.944875 evque-1.4.0/evque/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-08-04 12:07:04.000000 evque-1.4.0/evque/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-08-04 12:07:04.000000 evque-1.4.0/evque/evque.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:07:16.944875 evque-1.4.0/evque.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-08-04 12:07:16.000000 evque-1.4.0/evque.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-08-04 12:07:16.000000 evque-1.4.0/evque.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:07:16.000000 evque-1.4.0/evque.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-04 12:07:16.000000 evque-1.4.0/evque.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:07:16.948875 evque-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-08-04 12:07:04.000000 evque-1.4.0/setup.py
```

### Comparing `evque-1.3.0/LICENSE.txt` & `evque-1.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `evque-1.3.0/PKG-INFO` & `evque-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evque
-Version: 1.3.0
+Version: 1.4.0
 Summary: A simple event queue library with support for topics.
 Home-page: UNKNOWN
 Author: Ahmad Siavashi
 Author-email: siavashi@aut.ac.ir
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `evque-1.3.0/README.md` & `evque-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `evque-1.3.0/evque/evque.py` & `evque-1.4.0/evque/evque.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,16 +14,16 @@
     _events : list[tuple[int, str, tuple, dict], ...]
         The list of events in the queue, ordered by their delivery time.
     _topics : dict[str, list[Callable, ...]]
         A dictionary containing topics as keys and lists of event handler functions as values.
 
     Methods
     -------
-    subscribe(topic: str, handler: Callable):
-        Subscribe a handler function to a topic.
+    subscribe(topic: str, *handlers: tuple[Callable, ...]):
+        Subscribe handler functions to a topic.
 
     unsubscribe(topic: str, handler: Callable):
         Unsubscribe a handler function from a topic.
 
     publish(topic: str, delivery_time: int, *args):
         Publish an event to a topic with a specific delivery time.
 
@@ -65,42 +65,43 @@
     def __new__(cls):
         if cls._instance is None:
             cls._instance = super().__new__(cls)
             cls._instance._events = []
             cls._instance._topics = {}
         return cls._instance
 
-    def subscribe(self, topic: str, handler: Callable):
+    def subscribe(self, topic: str, *handlers: tuple[Callable, ...]):
         """
-        Subscribe a handler function to a topic.
+        Subscribe handler functions to a topic.
 
         Parameters
         ----------
         topic : str
             The topic to subscribe to.
-        handler : Callable
-            The handler function to be called when events are published to the topic.
+        *handlers : tuple[Callable, ...]
+            The handler functions to be called when events are published to the topic.
         """
         if topic not in self._topics:
             self._topics[topic] = []
-        self._topics[topic].append(handler)
+        self._topics[topic] += handlers
 
-    def unsubscribe(self, topic: str, handler: Callable):
+    def unsubscribe(self, topic: str, *handlers: tuple[Callable, ...]):
         """
-        Unsubscribe a handler function from a topic.
+        Unsubscribe handler functions from a topic.
 
         Parameters
         ----------
         topic :str
             The topic to unsubscribe from.
-        handler : Callable
-            The handler function to be removed from the topic.
+        handlers : tuple[Callable, ...]
+            The handler functions to be removed from the topic.
         """
         if topic in self._topics:
-            self._topics[topic].remove(handler)
+            for handler in handlers:
+                self._topics[topic].remove(handler)
 
     def publish(self, topic: str, delivery_time: int, *args):
         """
         Publish an event to a topic with a specific delivery time.
 
         Parameters
         ----------
```

### Comparing `evque-1.3.0/evque.egg-info/PKG-INFO` & `evque-1.4.0/evque.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evque
-Version: 1.3.0
+Version: 1.4.0
 Summary: A simple event queue library with support for topics.
 Home-page: UNKNOWN
 Author: Ahmad Siavashi
 Author-email: siavashi@aut.ac.ir
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `evque-1.3.0/setup.py` & `evque-1.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='evque',
-    version='1.3.0',
+    version='1.4.0',
     description='A simple event queue library with support for topics.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Ahmad Siavashi',
     author_email='siavashi@aut.ac.ir',
     packages=find_packages(),
     install_requires=[],
```

