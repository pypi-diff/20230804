# Comparing `tmp/pxuploaderapi-1.1.6.tar.gz` & `tmp/pxuploaderapi-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pxuploaderapi-1.1.6.tar", last modified: Thu Aug  3 21:50:01 2023, max compression
+gzip compressed data, was "pxuploaderapi-1.1.7.tar", last modified: Thu Aug  3 21:55:01 2023, max compression
```

## Comparing `pxuploaderapi-1.1.6.tar` & `pxuploaderapi-1.1.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 21:50:01.357784 pxuploaderapi-1.1.6/
--rw-rw-rw-   0        0        0      333 2023-08-03 21:50:01.357784 pxuploaderapi-1.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      108 2023-07-06 23:26:11.000000 pxuploaderapi-1.1.6/pyproject.toml
--rw-rw-rw-   0        0        0      523 2023-08-03 21:50:01.357784 pxuploaderapi-1.1.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-03 21:50:01.342162 pxuploaderapi-1.1.6/src/
-drwxrwxrwx   0        0        0        0 2023-08-03 21:50:01.342162 pxuploaderapi-1.1.6/src/pxuploaderapi/
--rw-rw-rw-   0        0        0     3473 2023-08-03 21:49:44.000000 pxuploaderapi-1.1.6/src/pxuploaderapi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-03 21:50:01.357784 pxuploaderapi-1.1.6/src/pxuploaderapi.egg-info/
--rw-rw-rw-   0        0        0      333 2023-08-03 21:50:01.000000 pxuploaderapi-1.1.6/src/pxuploaderapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2023-08-03 21:50:01.000000 pxuploaderapi-1.1.6/src/pxuploaderapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 21:50:01.000000 pxuploaderapi-1.1.6/src/pxuploaderapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-08-03 21:50:01.000000 pxuploaderapi-1.1.6/src/pxuploaderapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-03 21:55:01.930878 pxuploaderapi-1.1.7/
+-rw-rw-rw-   0        0        0      333 2023-08-03 21:55:01.930878 pxuploaderapi-1.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      108 2023-07-06 23:26:11.000000 pxuploaderapi-1.1.7/pyproject.toml
+-rw-rw-rw-   0        0        0      523 2023-08-03 21:55:01.930878 pxuploaderapi-1.1.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-03 21:55:01.893125 pxuploaderapi-1.1.7/src/
+drwxrwxrwx   0        0        0        0 2023-08-03 21:55:01.908746 pxuploaderapi-1.1.7/src/pxuploaderapi/
+-rw-rw-rw-   0        0        0     3707 2023-08-03 21:54:36.000000 pxuploaderapi-1.1.7/src/pxuploaderapi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 21:55:01.908746 pxuploaderapi-1.1.7/src/pxuploaderapi.egg-info/
+-rw-rw-rw-   0        0        0      333 2023-08-03 21:55:01.000000 pxuploaderapi-1.1.7/src/pxuploaderapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2023-08-03 21:55:01.000000 pxuploaderapi-1.1.7/src/pxuploaderapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 21:55:01.000000 pxuploaderapi-1.1.7/src/pxuploaderapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-08-03 21:55:01.000000 pxuploaderapi-1.1.7/src/pxuploaderapi.egg-info/top_level.txt
```

### Comparing `pxuploaderapi-1.1.6/setup.cfg` & `pxuploaderapi-1.1.7/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7875 706c 6f61 6465 7261 7069   = pxuploaderapi
 00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 312e  ..version = 1.1.
-00000030: 360d 0a61 7574 686f 7220 3d20 506f 756e  6..author = Poun
+00000030: 370d 0a61 7574 686f 7220 3d20 506f 756e  7..author = Poun
 00000040: 6465 7820 4173 736f 6369 6174 6573 2043  dex Associates C
 00000050: 6f72 706f 7261 7469 6f6e 0d0a 6175 7468  orporation..auth
 00000060: 6f72 5f65 6d61 696c 203d 2069 7440 706f  or_email = it@po
 00000070: 756e 6465 782e 636f 6d0d 0a64 6573 6372  undex.com..descr
 00000080: 6970 7469 6f6e 203d 200d 0a6c 6f6e 675f  iption = ..long_
 00000090: 6465 7363 7269 7074 696f 6e20 3d20 0d0a  description = ..
 000000a0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
```

### Comparing `pxuploaderapi-1.1.6/src/pxuploaderapi/__init__.py` & `pxuploaderapi-1.1.7/src/pxuploaderapi/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -53,47 +53,56 @@
     def writeToFile(self, score_dict):
         with open(self.score_file, "wb") as f:
             pickle.dump(score_dict, f) 
 
     def setUpScore(self, uuid):
         # If it's a new day, or if the uuid hasn't existed, reset the score.
         score_dict = self.getScores()
+        uuid = str(uuid)
         if uuid not in score_dict or score_dict[uuid][3] != datetime.datetime.now().date():
             score_dict[uuid] = (0, 0, 0, datetime.datetime.now().date())
             self.writeToFile(score_dict)
     
     def getScore(self, uuid) -> (int, int, int, datetime.date):
+        uuid = str(uuid)
         self.setUpScore(uuid)
         return self.getScores()[uuid]
     
     def getSuccesses(self, uuid) -> int:
+        uuid = str(uuid)
         return self.getScore(uuid)[0]
     
     def getPartial(self, uuid) -> int:
+        uuid = str(uuid)
         return self.getScore(uuid)[1]
     
     def getFailures(self, uuid) -> int:
+        uuid = str(uuid)
         return self.getScore(uuid)[2]
     
     def getDate(self, uuid) -> datetime.date:
+        uuid = str(uuid)
         return self.getScore(uuid)[3]
     
     def scoreSuccess(self, uuid):
+        uuid = str(uuid)
         self.setUpScore(uuid)
         score_dict = self.getScores()
         score_dict[uuid] = (self.getSuccesses(uuid) + 1, self.getPartial(uuid), self.getFailures(uuid), self.getDate(uuid))
         self.writeToFile(score_dict)
 
     def scorePartial(self, uuid):
+        uuid = str(uuid)
         self.setUpScore(uuid)
         score_dict = self.getScores()
         score_dict[uuid] = (self.getSuccesses(uuid), self.getPartial(uuid) + 1, self.getFailures(uuid), self.getDate(uuid))
         self.writeToFile(score_dict)
 
     def scoreFailed(self, uuid):
+        uuid = str(uuid)
         self.setUpScore(uuid)
         score_dict = self.getScores()
         score_dict[uuid] = (self.getSuccesses(uuid), self.getPartial(uuid), self.getFailures(uuid) + 1, self.getDate(uuid))
         self.writeToFile(score_dict)
```

