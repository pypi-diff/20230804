# Comparing `tmp/catenae_stopover-3.2308.2-py3-none-any.whl.zip` & `tmp/catenae_stopover-3.2308.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 9337 bytes, number of entries: 12
--rw-r--r--  2.0 unx     2088 b- defN 23-Aug-02 18:22 catenae/__init__.py
--rw-r--r--  2.0 unx    18047 b- defN 23-Aug-02 18:22 catenae/catenae.py
+Zip file size: 9370 bytes, number of entries: 12
+-rw-r--r--  2.0 unx     2088 b- defN 23-Aug-04 14:20 catenae/__init__.py
+-rw-r--r--  2.0 unx    18088 b- defN 23-Aug-04 13:51 catenae/catenae.py
 -rw-r--r--  2.0 unx      390 b- defN 23-Aug-02 17:07 catenae/errors.py
 -rw-r--r--  2.0 unx      636 b- defN 23-Aug-02 17:00 catenae/health.py
--rw-r--r--  2.0 unx      568 b- defN 23-Aug-02 17:19 catenae/logger.py
+-rw-r--r--  2.0 unx      707 b- defN 23-Aug-04 14:17 catenae/logger.py
 -rw-r--r--  2.0 unx     2096 b- defN 23-Aug-02 17:02 catenae/queue.py
 -rw-r--r--  2.0 unx     2027 b- defN 23-Aug-02 17:08 catenae/threading.py
 -rw-r--r--  2.0 unx     1060 b- defN 23-Aug-02 17:06 catenae/utils.py
--rw-r--r--  2.0 unx      824 b- defN 23-Aug-02 18:23 catenae_stopover-3.2308.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Aug-02 18:23 catenae_stopover-3.2308.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Aug-02 18:23 catenae_stopover-3.2308.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      938 b- defN 23-Aug-02 18:23 catenae_stopover-3.2308.2.dist-info/RECORD
-12 files, 28774 bytes uncompressed, 7771 bytes compressed:  73.0%
+-rw-r--r--  2.0 unx      824 b- defN 23-Aug-04 14:21 catenae_stopover-3.2308.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-04 14:21 catenae_stopover-3.2308.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Aug-04 14:21 catenae_stopover-3.2308.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      938 b- defN 23-Aug-04 14:21 catenae_stopover-3.2308.3.dist-info/RECORD
+12 files, 28954 bytes uncompressed, 7804 bytes compressed:  73.0%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: catenae/threading.py
 Comment: 
 
 Filename: catenae/utils.py
 Comment: 
 
-Filename: catenae_stopover-3.2308.2.dist-info/METADATA
+Filename: catenae_stopover-3.2308.3.dist-info/METADATA
 Comment: 
 
-Filename: catenae_stopover-3.2308.2.dist-info/WHEEL
+Filename: catenae_stopover-3.2308.3.dist-info/WHEEL
 Comment: 
 
-Filename: catenae_stopover-3.2308.2.dist-info/top_level.txt
+Filename: catenae_stopover-3.2308.3.dist-info/top_level.txt
 Comment: 
 
-Filename: catenae_stopover-3.2308.2.dist-info/RECORD
+Filename: catenae_stopover-3.2308.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## catenae/__init__.py

```diff
@@ -12,8 +12,8 @@
     '    ◼◼◼              ◼◼◼    ◼◼◼         ◼◼       ◼◼◼               ◼◼◼ ◼◼◼   ◼◼◼       ◼◼◼    ◼◼◼      ◼◼◼             \n'  # noqa: E501
     '  ◼◼◼               ◼◼◼      ◼◼◼        ◼◼     ◼◼◼◼◼◼◼◼◼◼◼◼◼◼◼◼◼◼  ◼◼◼  ◼◼◼  ◼◼◼      ◼◼◼      ◼◼◼   ◼◼◼◼◼◼◼◼◼◼◼◼◼◼◼◼◼◼\n'  # noqa: E501
     '    ◼◼◼            ◼◼◼        ◼◼◼       ◼◼       ◼◼◼               ◼◼◼    ◼◼ ◼◼◼     ◼◼◼        ◼◼◼    ◼◼◼             \n'  # noqa: E501
     '      ◼◼◼         ◼◼◼          ◼◼◼      ◼◼         ◼◼◼             ◼◼◼     ◼◼◼◼◼    ◼◼◼          ◼◼◼     ◼◼◼           \n'  # noqa: E501
     '        ◼◼◼      ◼◼◼            ◼◼◼     ◼◼           ◼◼◼           ◼◼◼      ◼◼◼◼   ◼◼◼            ◼◼◼      ◼◼◼         \n'  # noqa: E501
     '          ◼◼◼   ◼◼◼              ◼◼◼    ◼◼             ◼◼◼         ◼◼◼       ◼◼◼  ◼◼◼              ◼◼◼       ◼◼◼       \n'  # noqa: E501
 )
-__version__ = '3.2308.2'
+__version__ = '3.2308.3'
```

## catenae/catenae.py

```diff
@@ -82,17 +82,22 @@
         receiver_group: str = None,
         rpc_enabled: bool = None,
         rpc_by_uid: bool = None,
         enable_health: bool = None,
         health_port: int = None,
         log_level: str = None,
         progress_without_commit: bool = None,
+        binnakle_config: Dict = None,
         **ignored_kwargs,
     ):
-        self.logger = Logger(self, level=log_level)
+        self.logger = Logger(
+            self,
+            level=log_level,
+            config=binnakle_config,
+        )
 
         if endpoint is not None:
             endpoints = [endpoint]
         if not endpoints:
             endpoints = []
 
         if input_stream is not None:
@@ -268,18 +273,15 @@
         if not startup_text:
             print(catenae.text_logo)
         else:
             print(startup_text)
 
         self.logger.log(f'catenae  v{catenae.__version__}')
         self.logger.log(f'stopover v{stopover.__version__}')
-
-        self.logger.log(
-            f'configuration:\n{utils.dump_dict_pretty(self._config)}'
-        )
+        self.logger.log(self._config)
 
         with self._locks['start_stop']:
             self._started = True
 
         if setup_kwargs is None:
             setup_kwargs = {}
         self.setup(**setup_kwargs)
```

## catenae/logger.py

```diff
@@ -1,23 +1,32 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 from binnakle import Binnakle
 
 
 class Logger:
-    def __init__(self, instance, level=None):
+    def __init__(
+        self,
+        instance,
+        level=None,
+        config=None,
+    ):
         self.level = level.lower() if level else 'info'
         self.instance = instance
-        self._logger = Binnakle()
+
+        if config is None:
+            config = {}
+        self._logger = Binnakle(**config)
 
     def log(
         self,
         message='',
         level=None,
     ):
         level = level.lower() if level else self.level
         getattr(self._logger, level.lower())(
             message,
+            stack_depth=2,
             instance=self.instance.uid,
             microservice=self.instance.__class__.__name__,
         )
```

## Comparing `catenae_stopover-3.2308.2.dist-info/METADATA` & `catenae_stopover-3.2308.3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catenae-stopover
-Version: 3.2308.2
+Version: 3.2308.3
 Summary: Catenae 3 – Microservices Framework for Stopover
 Home-page: https://github.com/catenae
 Author: Rodrigo Martínez
 Author-email: dev@brunneis.com
 License: GNU General Public License v3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

## Comparing `catenae_stopover-3.2308.2.dist-info/RECORD` & `catenae_stopover-3.2308.3.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-catenae/__init__.py,sha256=fw8V1uXUiZsWxkIdhw6qtDUP0raTdsOcyKCrMXY0t6U,2088
-catenae/catenae.py,sha256=MwhnPCWGRXnQH1F6yEDbA8ARI9NVxWYkY2FQV-jOCK8,18047
+catenae/__init__.py,sha256=ERDJhnlq9luPQmhBjLM-APvezBEvEGddopszWWEYDeY,2088
+catenae/catenae.py,sha256=a-p_3fVxTA_aZz_n-VGG6ZDVBzpvfqJvlKTx6TzY4o0,18088
 catenae/errors.py,sha256=FvbeToyM4f07ZgJe0rRsuNBs-TR5O7V0bh-qCL29BSs,390
 catenae/health.py,sha256=EznwORvPvG-HXXgCXDkC57wydpkwNgZdvjs5557le6I,636
-catenae/logger.py,sha256=ik9q4oslzt8DZzHUSj1rPGMiKVHjFslJ7W0WigdhgaQ,568
+catenae/logger.py,sha256=1UpLDOE8M-5Q4SrN8ac8HQ-p3SFqDsDwpzwquMnPJQQ,707
 catenae/queue.py,sha256=qpEP2wy2icStRdKqHmN9fQxxLDRNcVpybHLXmFKGZ1k,2096
 catenae/threading.py,sha256=4HW-WyCL4H5gCNWSErn7gqdeRSW337i8989S6nfzVGs,2027
 catenae/utils.py,sha256=HYSNgDxx8WEAomYSjizutAZIyvi5do6XUYoivyAPVJk,1060
-catenae_stopover-3.2308.2.dist-info/METADATA,sha256=Ahi2cwmV3m1dOshfAx7yLkzkfnuFViVXF1vzn7ystEY,824
-catenae_stopover-3.2308.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-catenae_stopover-3.2308.2.dist-info/top_level.txt,sha256=8E6E0SqL9fHRQOOIaHVm5xJyTIBR5BqQiu04oOmV2YQ,8
-catenae_stopover-3.2308.2.dist-info/RECORD,,
+catenae_stopover-3.2308.3.dist-info/METADATA,sha256=ErTG8IB2Z09ikcQbfZeUJF2UBPrTp_k5KCBcrlsaFN4,824
+catenae_stopover-3.2308.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+catenae_stopover-3.2308.3.dist-info/top_level.txt,sha256=8E6E0SqL9fHRQOOIaHVm5xJyTIBR5BqQiu04oOmV2YQ,8
+catenae_stopover-3.2308.3.dist-info/RECORD,,
```

