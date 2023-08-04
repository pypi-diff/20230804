# Comparing `tmp/devvio_util-1.6.1.tar.gz` & `tmp/devvio_util-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devvio_util-1.6.1.tar", last modified: Thu Jul 20 15:18:06 2023, max compression
+gzip compressed data, was "devvio_util-1.6.2.tar", last modified: Fri Aug  4 19:27:44 2023, max compression
```

## Comparing `devvio_util-1.6.1.tar` & `devvio_util-1.6.2.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:18:06.029855 devvio_util-1.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-20 15:18:06.029855 devvio_util-1.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 15:17:58.000000 devvio_util-1.6.1/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:18:06.029855 devvio_util-1.6.1/devvio_util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 15:17:58.000000 devvio_util-1.6.1/devvio_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-20 15:17:58.000000 devvio_util-1.6.1/devvio_util/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-07-20 15:17:58.000000 devvio_util-1.6.1/devvio_util/lib_creds.py
--rw-r--r--   0 runner    (1001) docker     (123)     9232 2023-07-20 15:17:58.000000 devvio_util-1.6.1/devvio_util/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:18:06.029855 devvio_util-1.6.1/devvio_util/primitives/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 15:17:58.000000 devvio_util-1.6.1/devvio_util/primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-07-20 15:17:58.000000 devvio_util-1.6.1/devvio_util/primitives/address.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-20 15:17:58.000000 devvio_util-1.6.1/devvio_util/primitives/atomic_transaction_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-07-20 15:17:58.000000 devvio_util-1.6.1/devvio_util/primitives/chainstate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-20 15:17:58.000000 devvio_util-1.6.1/devvio_util/primitives/devv_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     8976 2023-07-20 15:17:58.000000 devvio_util-1.6.1/devvio_util/primitives/devv_sign.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-20 15:17:58.000000 devvio_util-1.6.1/devvio_util/primitives/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-07-20 15:17:58.000000 devvio_util-1.6.1/devvio_util/primitives/final_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-07-20 15:17:58.000000 devvio_util-1.6.1/devvio_util/primitives/signature.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-20 15:17:58.000000 devvio_util-1.6.1/devvio_util/primitives/smart_coin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-07-20 15:17:58.000000 devvio_util-1.6.1/devvio_util/primitives/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)    14658 2023-07-20 15:17:58.000000 devvio_util-1.6.1/devvio_util/primitives/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-07-20 15:17:58.000000 devvio_util-1.6.1/devvio_util/primitives/transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-07-20 15:17:58.000000 devvio_util-1.6.1/devvio_util/primitives/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-07-20 15:17:58.000000 devvio_util-1.6.1/devvio_util/primitives/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-07-20 15:17:58.000000 devvio_util-1.6.1/devvio_util/psql_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:18:06.029855 devvio_util-1.6.1/devvio_util.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-20 15:18:06.000000 devvio_util-1.6.1/devvio_util.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-20 15:18:06.000000 devvio_util-1.6.1/devvio_util.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:18:06.000000 devvio_util-1.6.1/devvio_util.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:18:05.000000 devvio_util-1.6.1/devvio_util.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-20 15:18:06.000000 devvio_util-1.6.1/devvio_util.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-20 15:18:06.000000 devvio_util-1.6.1/devvio_util.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-20 15:18:06.029855 devvio_util-1.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-20 15:17:58.000000 devvio_util-1.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:27:44.880449 devvio_util-1.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-08-04 19:27:44.880449 devvio_util-1.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 19:27:36.000000 devvio_util-1.6.2/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:27:44.876449 devvio_util-1.6.2/devvio_util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 19:27:36.000000 devvio_util-1.6.2/devvio_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-08-04 19:27:36.000000 devvio_util-1.6.2/devvio_util/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-08-04 19:27:36.000000 devvio_util-1.6.2/devvio_util/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-08-04 19:27:36.000000 devvio_util-1.6.2/devvio_util/lib_creds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9223 2023-08-04 19:27:36.000000 devvio_util-1.6.2/devvio_util/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:27:44.880449 devvio_util-1.6.2/devvio_util/primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 19:27:36.000000 devvio_util-1.6.2/devvio_util/primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-08-04 19:27:36.000000 devvio_util-1.6.2/devvio_util/primitives/address.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-04 19:27:36.000000 devvio_util-1.6.2/devvio_util/primitives/atomic_transaction_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-08-04 19:27:36.000000 devvio_util-1.6.2/devvio_util/primitives/chainstate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-08-04 19:27:36.000000 devvio_util-1.6.2/devvio_util/primitives/devv_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8976 2023-08-04 19:27:36.000000 devvio_util-1.6.2/devvio_util/primitives/devv_sign.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-04 19:27:36.000000 devvio_util-1.6.2/devvio_util/primitives/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-08-04 19:27:36.000000 devvio_util-1.6.2/devvio_util/primitives/final_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-08-04 19:27:36.000000 devvio_util-1.6.2/devvio_util/primitives/signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-08-04 19:27:36.000000 devvio_util-1.6.2/devvio_util/primitives/smart_coin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-08-04 19:27:36.000000 devvio_util-1.6.2/devvio_util/primitives/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14658 2023-08-04 19:27:36.000000 devvio_util-1.6.2/devvio_util/primitives/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-08-04 19:27:36.000000 devvio_util-1.6.2/devvio_util/primitives/transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-08-04 19:27:36.000000 devvio_util-1.6.2/devvio_util/primitives/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-08-04 19:27:36.000000 devvio_util-1.6.2/devvio_util/primitives/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-08-04 19:27:36.000000 devvio_util-1.6.2/devvio_util/psql_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:27:44.876449 devvio_util-1.6.2/devvio_util.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-08-04 19:27:44.000000 devvio_util-1.6.2/devvio_util.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-08-04 19:27:44.000000 devvio_util-1.6.2/devvio_util.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 19:27:44.000000 devvio_util-1.6.2/devvio_util.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 19:27:44.000000 devvio_util-1.6.2/devvio_util.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-04 19:27:44.000000 devvio_util-1.6.2/devvio_util.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-04 19:27:44.000000 devvio_util-1.6.2/devvio_util.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-04 19:27:44.880449 devvio_util-1.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-08-04 19:27:36.000000 devvio_util-1.6.2/setup.py
```

### Comparing `devvio_util-1.6.1/devvio_util/config.py` & `devvio_util-1.6.2/devvio_util/config.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.6.1/devvio_util/lib_creds.py` & `devvio_util-1.6.2/devvio_util/lib_creds.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.6.1/devvio_util/logging.py` & `devvio_util-1.6.2/devvio_util/logging.py`

 * *Files 0% similar despite different names*

```diff
@@ -224,31 +224,30 @@
     if len(logging.root.handlers) == 0:
         logging.basicConfig()
 
     logging.root.trace(msg, *args, **kwargs)
 
 
 logging.trace = trace
+logging.setLoggerClass(DevvLogger)
+logging.root = DevvLogger("global")
 
 
 if __name__ == '__main__':
 
     class A_Class():
         def __init__(self, logger):
             self.logger = logger
             logging.debug("a global message")
             logger.trace("a module logger")
 
     def logger2_test():
         logger2 = logging.getLogger()
         logger2.notice("from logger2")
 
-    logging.setLoggerClass(DevvLogger)
-    logging.root = DevvLogger("global")
-
     # Tests
     logger = DevvLogger("logtest")
     logger.trace("Trace message")
     logger.debug("Debug message")
     logger.info("Info message")
     logger.notice("Notice message")
     logger.warning("Warning message")
```

### Comparing `devvio_util-1.6.1/devvio_util/primitives/address.py` & `devvio_util-1.6.2/devvio_util/primitives/address.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.6.1/devvio_util/primitives/chainstate.py` & `devvio_util-1.6.2/devvio_util/primitives/chainstate.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.6.1/devvio_util/primitives/devv_constants.py` & `devvio_util-1.6.2/devvio_util/primitives/devv_constants.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.6.1/devvio_util/primitives/devv_sign.py` & `devvio_util-1.6.2/devvio_util/primitives/devv_sign.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.6.1/devvio_util/primitives/final_block.py` & `devvio_util-1.6.2/devvio_util/primitives/final_block.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.6.1/devvio_util/primitives/signature.py` & `devvio_util-1.6.2/devvio_util/primitives/signature.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.6.1/devvio_util/primitives/smart_coin.py` & `devvio_util-1.6.2/devvio_util/primitives/smart_coin.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.6.1/devvio_util/primitives/summary.py` & `devvio_util-1.6.2/devvio_util/primitives/summary.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.6.1/devvio_util/primitives/transaction.py` & `devvio_util-1.6.2/devvio_util/primitives/transaction.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.6.1/devvio_util/primitives/transfer.py` & `devvio_util-1.6.2/devvio_util/primitives/transfer.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.6.1/devvio_util/primitives/utils.py` & `devvio_util-1.6.2/devvio_util/primitives/utils.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.6.1/devvio_util/primitives/validation.py` & `devvio_util-1.6.2/devvio_util/primitives/validation.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.6.1/devvio_util/psql_mixin.py` & `devvio_util-1.6.2/devvio_util/psql_mixin.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.6.1/devvio_util.egg-info/SOURCES.txt` & `devvio_util-1.6.2/devvio_util.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 README.txt
 setup.cfg
 setup.py
 devvio_util/__init__.py
 devvio_util/config.py
+devvio_util/decorators.py
 devvio_util/lib_creds.py
 devvio_util/logging.py
 devvio_util/psql_mixin.py
 devvio_util.egg-info/PKG-INFO
 devvio_util.egg-info/SOURCES.txt
 devvio_util.egg-info/dependency_links.txt
 devvio_util.egg-info/not-zip-safe
```

### Comparing `devvio_util-1.6.1/setup.py` & `devvio_util-1.6.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from setuptools import setup
-VERSION = 'v1.6.1'
+VERSION = 'v1.6.2'
 
 setup(name='devvio_util',
       version=VERSION,
       long_description=open('README.txt').read(),
       long_description_content_type='text/markdown',
       description='Utility to be used inside Devvio projects',
       author='Devvio Team',
```

