# Comparing `tmp/pih-mio-1.48024.tar.gz` & `tmp/pih-mio-1.48025.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-mio-1.48024.tar", last modified: Thu Aug  3 07:33:18 2023, max compression
+gzip compressed data, was "pih-mio-1.48025.tar", last modified: Fri Aug  4 01:22:14 2023, max compression
```

## Comparing `pih-mio-1.48024.tar` & `pih-mio-1.48025.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 07:33:15.604016 pih-mio-1.48024/
-drwxrwxrwx   0        0        0        0 2023-08-03 07:33:17.560090 pih-mio-1.48024/MobileHelperCore/
--rw-rw-rw-   0        0        0        0 2023-03-23 02:22:16.000000 pih-mio-1.48024/MobileHelperCore/__init__.py
--rw-rw-rw-   0        0        0      158 2023-07-28 13:41:38.000000 pih-mio-1.48024/MobileHelperCore/__main__.py
--rw-rw-rw-   0        0        0   165341 2023-08-03 07:32:13.000000 pih-mio-1.48024/MobileHelperCore/api.py
--rw-rw-rw-   0        0        0      718 2023-07-28 13:36:37.000000 pih-mio-1.48024/MobileHelperCore/service.py
--rw-rw-rw-   0        0        0     9434 2023-08-01 00:38:40.000000 pih-mio-1.48024/MobileHelperCore/service_api.py
--rw-rw-rw-   0        0        0      986 2023-06-21 05:38:40.000000 pih-mio-1.48024/MobileHelperCore/tools.py
--rw-rw-rw-   0        0        0      279 2023-08-03 07:33:18.131667 pih-mio-1.48024/PKG-INFO
--rw-rw-rw-   0        0        0     1651 2023-08-03 07:25:38.000000 pih-mio-1.48024/pih-mio_setup.py
-drwxrwxrwx   0        0        0        0 2023-08-03 07:33:18.084794 pih-mio-1.48024/pih_mio.egg-info/
--rw-rw-rw-   0        0        0      279 2023-08-03 07:33:11.000000 pih-mio-1.48024/pih_mio.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      372 2023-08-03 07:33:15.000000 pih-mio-1.48024/pih_mio.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 07:33:12.000000 pih-mio-1.48024/pih_mio.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-08-03 07:33:13.000000 pih-mio-1.48024/pih_mio.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       20 2023-08-03 07:33:14.000000 pih-mio-1.48024/pih_mio.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-08-03 07:33:14.000000 pih-mio-1.48024/pih_mio.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-03 07:33:18.147295 pih-mio-1.48024/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-04 01:22:13.718815 pih-mio-1.48025/
+drwxrwxrwx   0        0        0        0 2023-08-04 01:22:14.172213 pih-mio-1.48025/MobileHelperCore/
+-rw-rw-rw-   0        0        0        0 2023-03-23 02:22:16.000000 pih-mio-1.48025/MobileHelperCore/__init__.py
+-rw-rw-rw-   0        0        0      158 2023-07-28 13:41:38.000000 pih-mio-1.48025/MobileHelperCore/__main__.py
+-rw-rw-rw-   0        0        0   165341 2023-08-04 01:21:02.000000 pih-mio-1.48025/MobileHelperCore/api.py
+-rw-rw-rw-   0        0        0      718 2023-07-28 13:36:37.000000 pih-mio-1.48025/MobileHelperCore/service.py
+-rw-rw-rw-   0        0        0     9431 2023-08-04 01:20:17.000000 pih-mio-1.48025/MobileHelperCore/service_api.py
+-rw-rw-rw-   0        0        0      986 2023-06-21 05:38:40.000000 pih-mio-1.48025/MobileHelperCore/tools.py
+-rw-rw-rw-   0        0        0      279 2023-08-04 01:22:14.406583 pih-mio-1.48025/PKG-INFO
+-rw-rw-rw-   0        0        0     1651 2023-08-03 07:25:38.000000 pih-mio-1.48025/pih-mio_setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 01:22:14.312835 pih-mio-1.48025/pih_mio.egg-info/
+-rw-rw-rw-   0        0        0      279 2023-08-04 01:22:12.000000 pih-mio-1.48025/pih_mio.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      372 2023-08-04 01:22:13.000000 pih-mio-1.48025/pih_mio.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 01:22:12.000000 pih-mio-1.48025/pih_mio.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-08-04 01:22:13.000000 pih-mio-1.48025/pih_mio.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       20 2023-08-04 01:22:13.000000 pih-mio-1.48025/pih_mio.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-08-04 01:22:13.000000 pih-mio-1.48025/pih_mio.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-04 01:22:14.422207 pih-mio-1.48025/setup.cfg
```

### Comparing `pih-mio-1.48024/MobileHelperCore/api.py` & `pih-mio-1.48025/MobileHelperCore/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 from MobileHelperContent.content import MEDIA_CONTENT
 import requests
 from io import BytesIO
 
 class MIO:
 
     NAME: str = "mio"       
-    VERSION: str = "1.48024"  
+    VERSION: str = "1.48025"  
 
 class InternalInterrupt(Exception):
 
     @property
     def type(self) -> int:
         return self.args[0]
```

### Comparing `pih-mio-1.48024/MobileHelperCore/service.py` & `pih-mio-1.48025/MobileHelperCore/service.py`

 * *Files identical despite different names*

### Comparing `pih-mio-1.48024/MobileHelperCore/service_api.py` & `pih-mio-1.48025/MobileHelperCore/service_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 SC = A.CT_SC
 
 ROLE: SR = SR.MOBILE_HELPER
 
 #version 0.8
 
 def as_developer() -> bool:
-    return A.SE.arg(1, "").lower() == "true"
+    return A.SE.named_arg("as_developer")
 
 class MobileHelperService():
 
     INIT: bool = False
     INSTANCE: Any | None = None
     NAME: str = "MobileHelper"
```

### Comparing `pih-mio-1.48024/MobileHelperCore/tools.py` & `pih-mio-1.48025/MobileHelperCore/tools.py`

 * *Files identical despite different names*

### Comparing `pih-mio-1.48024/pih-mio_setup.py` & `pih-mio-1.48025/pih-mio_setup.py`

 * *Files identical despite different names*

