# Comparing `tmp/ashcrypt-3.1.7.tar.gz` & `tmp/ashcrypt-3.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ashcrypt-3.1.7.tar", last modified: Thu Aug  3 14:12:23 2023, max compression
+gzip compressed data, was "dist/ashcrypt-3.1.8.tar", last modified: Thu Aug  3 14:23:25 2023, max compression
```

## Comparing `ashcrypt-3.1.7.tar` & `ashcrypt-3.1.8.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:12:23.000000 ashcrypt-3.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-03 14:12:23.000000 ashcrypt-3.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17424 2023-08-03 14:12:09.000000 ashcrypt-3.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:12:23.000000 ashcrypt-3.1.7/ashcrypt/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-03 14:12:09.000000 ashcrypt-3.1.7/ashcrypt/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-03 14:12:09.000000 ashcrypt-3.1.7/ashcrypt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-08-03 14:12:09.000000 ashcrypt-3.1.7/ashcrypt/crypt.py
--rw-r--r--   0 runner    (1001) docker     (123)    10523 2023-08-03 14:12:09.000000 ashcrypt-3.1.7/ashcrypt/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-08-03 14:12:09.000000 ashcrypt-3.1.7/ashcrypt/filecrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)    39578 2023-08-03 14:12:09.000000 ashcrypt-3.1.7/ashcrypt/gui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:12:23.000000 ashcrypt-3.1.7/ashcrypt/sandbox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 14:12:09.000000 ashcrypt-3.1.7/ashcrypt/sandbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-08-03 14:12:09.000000 ashcrypt-3.1.7/ashcrypt/sandbox/clicrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-08-03 14:12:09.000000 ashcrypt-3.1.7/ashcrypt/textcrypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:12:23.000000 ashcrypt-3.1.7/ashcrypt/unittests/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-03 14:12:09.000000 ashcrypt-3.1.7/ashcrypt/unittests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-08-03 14:12:09.000000 ashcrypt-3.1.7/ashcrypt/unittests/unittest_crypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:12:23.000000 ashcrypt-3.1.7/ashcrypt/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 14:12:09.000000 ashcrypt-3.1.7/ashcrypt/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:12:23.000000 ashcrypt-3.1.7/ashcrypt/utils/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-03 14:12:09.000000 ashcrypt-3.1.7/ashcrypt/utils/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-08-03 14:12:09.000000 ashcrypt-3.1.7/ashcrypt/utils/exceptions/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:12:23.000000 ashcrypt-3.1.7/ashcrypt/utils/safepack/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 14:12:09.000000 ashcrypt-3.1.7/ashcrypt/utils/safepack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-08-03 14:12:09.000000 ashcrypt-3.1.7/ashcrypt/utils/safepack/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-03 14:12:09.000000 ashcrypt-3.1.7/ashcrypt/utils/safepack/qr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-08-03 14:12:09.000000 ashcrypt-3.1.7/ashcrypt/utils/safepack/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:12:23.000000 ashcrypt-3.1.7/ashcrypt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-03 14:12:23.000000 ashcrypt-3.1.7/ashcrypt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-08-03 14:12:23.000000 ashcrypt-3.1.7/ashcrypt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 14:12:23.000000 ashcrypt-3.1.7/ashcrypt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-03 14:12:23.000000 ashcrypt-3.1.7/ashcrypt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-03 14:12:23.000000 ashcrypt-3.1.7/ashcrypt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 14:12:23.000000 ashcrypt-3.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-08-03 14:12:09.000000 ashcrypt-3.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:23:25.000000 ashcrypt-3.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-03 14:23:25.000000 ashcrypt-3.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17424 2023-08-03 14:23:10.000000 ashcrypt-3.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:23:25.000000 ashcrypt-3.1.8/ashcrypt/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-03 14:23:10.000000 ashcrypt-3.1.8/ashcrypt/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-03 14:23:10.000000 ashcrypt-3.1.8/ashcrypt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7251 2023-08-03 14:23:10.000000 ashcrypt-3.1.8/ashcrypt/crypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10523 2023-08-03 14:23:10.000000 ashcrypt-3.1.8/ashcrypt/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-08-03 14:23:10.000000 ashcrypt-3.1.8/ashcrypt/filecrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39578 2023-08-03 14:23:10.000000 ashcrypt-3.1.8/ashcrypt/gui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:23:25.000000 ashcrypt-3.1.8/ashcrypt/sandbox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 14:23:10.000000 ashcrypt-3.1.8/ashcrypt/sandbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-08-03 14:23:10.000000 ashcrypt-3.1.8/ashcrypt/sandbox/clicrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-08-03 14:23:10.000000 ashcrypt-3.1.8/ashcrypt/textcrypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:23:25.000000 ashcrypt-3.1.8/ashcrypt/unittests/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-03 14:23:10.000000 ashcrypt-3.1.8/ashcrypt/unittests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-08-03 14:23:10.000000 ashcrypt-3.1.8/ashcrypt/unittests/unittest_crypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:23:25.000000 ashcrypt-3.1.8/ashcrypt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 14:23:10.000000 ashcrypt-3.1.8/ashcrypt/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:23:25.000000 ashcrypt-3.1.8/ashcrypt/utils/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-03 14:23:10.000000 ashcrypt-3.1.8/ashcrypt/utils/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-08-03 14:23:10.000000 ashcrypt-3.1.8/ashcrypt/utils/exceptions/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:23:25.000000 ashcrypt-3.1.8/ashcrypt/utils/safepack/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 14:23:10.000000 ashcrypt-3.1.8/ashcrypt/utils/safepack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-08-03 14:23:10.000000 ashcrypt-3.1.8/ashcrypt/utils/safepack/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-03 14:23:10.000000 ashcrypt-3.1.8/ashcrypt/utils/safepack/qr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-08-03 14:23:10.000000 ashcrypt-3.1.8/ashcrypt/utils/safepack/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:23:25.000000 ashcrypt-3.1.8/ashcrypt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-03 14:23:25.000000 ashcrypt-3.1.8/ashcrypt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-08-03 14:23:25.000000 ashcrypt-3.1.8/ashcrypt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 14:23:25.000000 ashcrypt-3.1.8/ashcrypt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-03 14:23:25.000000 ashcrypt-3.1.8/ashcrypt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-03 14:23:25.000000 ashcrypt-3.1.8/ashcrypt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 14:23:25.000000 ashcrypt-3.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-08-03 14:23:10.000000 ashcrypt-3.1.8/setup.py
```

### Comparing `ashcrypt-3.1.7/PKG-INFO` & `ashcrypt-3.1.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ashcrypt
-Version: 3.1.7
+Version: 3.1.8
 Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 License: UNKNOWN
 Description: # Cryptography App & Library For AES-256
         ## Docs ##
```

### Comparing `ashcrypt-3.1.7/README.md` & `ashcrypt-3.1.8/README.md`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.7/ashcrypt/crypt.py` & `ashcrypt-3.1.8/ashcrypt/crypt.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,29 +9,33 @@
 import bcrypt
 from ashcrypt.utils import exceptions
 from cryptography.hazmat.primitives.ciphers import Cipher, algorithms, modes
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import hashes, hmac
 from cryptography.hazmat.primitives import padding
 
+IV_SIZE = 16
+SALT_SIZE = 16
+PEPPER_SIZE = 16
+
 
 class Enc:
     """Class to encrypt data of either type bytes or str"""
 
     def __init__(self, message: Union[str, bytes], mainkey: str,
                  iterations: Optional[int] = 50) -> None:
         if isinstance(message, str):
             self.message = message.encode()
         elif isinstance(message, bytes):
             self.message = message
 
         self.mainkey = mainkey
-        self._iv = os.urandom(16)
-        self.salt = os.urandom(16)
-        self.pepper = os.urandom(16)
+        self._iv = os.urandom(IV_SIZE)
+        self.salt = os.urandom(SALT_SIZE)
+        self.pepper = os.urandom(PEPPER_SIZE)
         self.iterations = iterations
         if self.iterations < 50 or self.iterations > 100000:
             raise exceptions.IterationsOutofRangeError(self.iterations)
         self.enc_key = self.derkey(self.mainkey, self.salt, self.iterations)
         self.hmac_key = self.derkey(self.mainkey, self.pepper, self.iterations)
 
     @staticmethod
```

### Comparing `ashcrypt-3.1.7/ashcrypt/database.py` & `ashcrypt-3.1.8/ashcrypt/database.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.7/ashcrypt/filecrypt.py` & `ashcrypt-3.1.8/ashcrypt/filecrypt.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.7/ashcrypt/gui.py` & `ashcrypt-3.1.8/ashcrypt/gui.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.7/ashcrypt/sandbox/clicrypt.py` & `ashcrypt-3.1.8/ashcrypt/sandbox/clicrypt.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.7/ashcrypt/textcrypt.py` & `ashcrypt-3.1.8/ashcrypt/textcrypt.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.7/ashcrypt/unittests/unittest_crypt.py` & `ashcrypt-3.1.8/ashcrypt/unittests/unittest_crypt.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.7/ashcrypt/utils/exceptions/main.py` & `ashcrypt-3.1.8/ashcrypt/utils/exceptions/main.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.7/ashcrypt/utils/safepack/file.py` & `ashcrypt-3.1.8/ashcrypt/utils/safepack/file.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.7/ashcrypt/utils/safepack/text.py` & `ashcrypt-3.1.8/ashcrypt/utils/safepack/text.py`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.7/ashcrypt.egg-info/PKG-INFO` & `ashcrypt-3.1.8/ashcrypt.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ashcrypt
-Version: 3.1.7
+Version: 3.1.8
 Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 License: UNKNOWN
 Description: # Cryptography App & Library For AES-256
         ## Docs ##
```

### Comparing `ashcrypt-3.1.7/ashcrypt.egg-info/SOURCES.txt` & `ashcrypt-3.1.8/ashcrypt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ashcrypt-3.1.7/setup.py` & `ashcrypt-3.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('ashcrypt/README.md', 'r') as f:
     readme = f.read()
 
 setup(
     name='ashcrypt',
-    version='3.1.7',
+    version='3.1.8',
     author='Ashref Gwader',
     author_email='AshrefGw@proton.me',
     python_requires='>=3.7',
     description="Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along"
                 " with a database module to store encrypted content.",
     long_description_content_type='text/markdown',
     long_description=readme,
```

