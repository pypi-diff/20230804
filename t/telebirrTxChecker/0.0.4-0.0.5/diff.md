# Comparing `tmp/telebirrTxChecker-0.0.4.tar.gz` & `tmp/telebirrTxChecker-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telebirrTxChecker-0.0.4.tar", last modified: Fri Aug  4 08:27:23 2023, max compression
+gzip compressed data, was "telebirrTxChecker-0.0.5.tar", last modified: Fri Aug  4 15:05:23 2023, max compression
```

## Comparing `telebirrTxChecker-0.0.4.tar` & `telebirrTxChecker-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:27:23.564737 telebirrTxChecker-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-08-04 08:27:23.564737 telebirrTxChecker-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-08-04 08:27:11.000000 telebirrTxChecker-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 08:27:23.564737 telebirrTxChecker-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-08-04 08:27:11.000000 telebirrTxChecker-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:27:23.564737 telebirrTxChecker-0.0.4/telebirrTxChecker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-08-04 08:27:23.000000 telebirrTxChecker-0.0.4/telebirrTxChecker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-08-04 08:27:23.000000 telebirrTxChecker-0.0.4/telebirrTxChecker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 08:27:23.000000 telebirrTxChecker-0.0.4/telebirrTxChecker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-04 08:27:23.000000 telebirrTxChecker-0.0.4/telebirrTxChecker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-04 08:27:23.000000 telebirrTxChecker-0.0.4/telebirrTxChecker.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:27:23.564737 telebirrTxChecker-0.0.4/ttxc/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-04 08:27:11.000000 telebirrTxChecker-0.0.4/ttxc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-08-04 08:27:11.000000 telebirrTxChecker-0.0.4/ttxc/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:27:23.564737 telebirrTxChecker-0.0.4/ttxc/errors/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-04 08:27:11.000000 telebirrTxChecker-0.0.4/ttxc/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-08-04 08:27:11.000000 telebirrTxChecker-0.0.4/ttxc/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:27:23.564737 telebirrTxChecker-0.0.4/ttxc/types/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-08-04 08:27:11.000000 telebirrTxChecker-0.0.4/ttxc/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-08-04 08:27:11.000000 telebirrTxChecker-0.0.4/ttxc/types/payer.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-04 08:27:11.000000 telebirrTxChecker-0.0.4/ttxc/types/receiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-08-04 08:27:11.000000 telebirrTxChecker-0.0.4/ttxc/types/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-08-04 08:27:11.000000 telebirrTxChecker-0.0.4/ttxc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:05:23.296934 telebirrTxChecker-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-08-04 15:05:23.296934 telebirrTxChecker-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-08-04 15:05:07.000000 telebirrTxChecker-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 15:05:23.296934 telebirrTxChecker-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-08-04 15:05:07.000000 telebirrTxChecker-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:05:23.292934 telebirrTxChecker-0.0.5/telebirrTxChecker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-08-04 15:05:23.000000 telebirrTxChecker-0.0.5/telebirrTxChecker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-08-04 15:05:23.000000 telebirrTxChecker-0.0.5/telebirrTxChecker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 15:05:23.000000 telebirrTxChecker-0.0.5/telebirrTxChecker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-04 15:05:23.000000 telebirrTxChecker-0.0.5/telebirrTxChecker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-04 15:05:23.000000 telebirrTxChecker-0.0.5/telebirrTxChecker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:05:23.292934 telebirrTxChecker-0.0.5/ttxc/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-04 15:05:07.000000 telebirrTxChecker-0.0.5/ttxc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-08-04 15:05:07.000000 telebirrTxChecker-0.0.5/ttxc/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:05:23.292934 telebirrTxChecker-0.0.5/ttxc/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-04 15:05:07.000000 telebirrTxChecker-0.0.5/ttxc/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-08-04 15:05:07.000000 telebirrTxChecker-0.0.5/ttxc/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:05:23.296934 telebirrTxChecker-0.0.5/ttxc/types/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-08-04 15:05:07.000000 telebirrTxChecker-0.0.5/ttxc/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-08-04 15:05:07.000000 telebirrTxChecker-0.0.5/ttxc/types/payer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-04 15:05:07.000000 telebirrTxChecker-0.0.5/ttxc/types/receiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-08-04 15:05:07.000000 telebirrTxChecker-0.0.5/ttxc/types/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-08-04 15:05:07.000000 telebirrTxChecker-0.0.5/ttxc/utils.py
```

### Comparing `telebirrTxChecker-0.0.4/PKG-INFO` & `telebirrTxChecker-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telebirrTxChecker
-Version: 0.0.4
+Version: 0.0.5
 Summary: asynchronous telebirr transaction checker
 Home-page: https://github.com/wizkiye/TelebirrPaymentProcessor
 Author: Kidus
 Author-email: wizkiye@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `telebirrTxChecker-0.0.4/README.md` & `telebirrTxChecker-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `telebirrTxChecker-0.0.4/setup.py` & `telebirrTxChecker-0.0.5/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pathlib import Path
 
 from setuptools import setup, find_packages
 
 setup(
     name="telebirrTxChecker",
-    version="0.0.4",
+    version="0.0.5",
     packages=find_packages(),
     url="https://github.com/wizkiye/TelebirrPaymentProcessor",
     license="MIT",
     author="Kidus",
     author_email="wizkiye@gmail.com",
     description="asynchronous telebirr transaction checker",
     long_description=Path("README.md").read_text(),
```

### Comparing `telebirrTxChecker-0.0.4/telebirrTxChecker.egg-info/PKG-INFO` & `telebirrTxChecker-0.0.5/telebirrTxChecker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telebirrTxChecker
-Version: 0.0.4
+Version: 0.0.5
 Summary: asynchronous telebirr transaction checker
 Home-page: https://github.com/wizkiye/TelebirrPaymentProcessor
 Author: Kidus
 Author-email: wizkiye@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `telebirrTxChecker-0.0.4/ttxc/main.py` & `telebirrTxChecker-0.0.5/ttxc/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from datetime import datetime
 from typing import Union, Optional
 
 import httpx
-import pdfkit
 
 from ttxc import constants, utils
 from ttxc.errors import TransactionNotFound
 from ttxc.types import Transaction, Payer, Receiver
 
 
 def r_birr(text: str):
@@ -60,10 +59,10 @@
             date=datetime.strptime(data["date"], "%d-%m-%Y %H:%M:%S"),
             mode=data["mode"],
             reason=data["reason"],
             channel=data["channel"],
             base=self,
         )
 
-    @staticmethod
-    async def save_pdf(tx_id: str, path: str) -> bool:
-        return pdfkit.from_url(constants.BASE_URL.format(tx_id), path)
+    # @staticmethod
+    # async def save_pdf(tx_id: str, path: str) -> bool:
+    #     return pdfkit.from_url(constants.BASE_URL.format(tx_id), path)
```

### Comparing `telebirrTxChecker-0.0.4/ttxc/types/transaction.py` & `telebirrTxChecker-0.0.5/ttxc/types/transaction.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,16 +34,16 @@
             and self.receiver.name.lower() == name.lower()
         )
 
     @property
     def is_paid(self):
         return self.status.lower() == "completed"
 
-    async def save_pdf(self, path: str) -> bool:
-        return await self.base.save_pdf(self.id, path)
+    # async def save_pdf(self, path: str) -> bool:
+    #     return await self.base.save_pdf(self.id, path)
 
     def dict(self):
         return {
             "id": self.id,
             "payer": self.payer.__dict__,
             "receiver": self.receiver.__dict__,
             "status": self.status,
```

### Comparing `telebirrTxChecker-0.0.4/ttxc/utils.py` & `telebirrTxChecker-0.0.5/ttxc/utils.py`

 * *Files identical despite different names*

