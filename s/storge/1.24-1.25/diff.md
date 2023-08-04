# Comparing `tmp/storge-1.24.tar.gz` & `tmp/storge-1.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "storge-1.24.tar", last modified: Wed Jan 11 16:18:53 2023, max compression
+gzip compressed data, was "storge-1.25.tar", last modified: Fri Aug  4 20:09:14 2023, max compression
```

## Comparing `storge-1.24.tar` & `storge-1.25.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 gwyn      (1000) gwyn      (1000)        0 2023-01-11 16:18:53.092217 storge-1.24/
--rw-rw-r--   0 gwyn      (1000) gwyn      (1000)    35147 2021-08-16 15:15:12.000000 storge-1.24/LICENSE.txt
--rw-r--r--   0 gwyn      (1000) gwyn      (1000)      535 2023-01-11 16:18:53.092217 storge-1.24/PKG-INFO
--rw-r--r--   0 gwyn      (1000) gwyn      (1000)      104 2023-01-10 19:21:41.000000 storge-1.24/pyproject.toml
-drwxr-xr-x   0 gwyn      (1000) gwyn      (1000)        0 2023-01-11 16:18:53.090217 storge-1.24/pystorge/
--rw-rw-r--   0 gwyn      (1000) gwyn      (1000)     9035 2021-12-29 21:41:33.000000 storge-1.24/pystorge/__init__.py
--rw-rw-r--   0 gwyn      (1000) gwyn      (1000)     1398 2021-08-16 15:15:12.000000 storge-1.24/pystorge/favicon.ico
--rw-rw-r--   0 gwyn      (1000) gwyn      (1000)      873 2023-01-11 16:18:53.093217 storge-1.24/setup.cfg
--rwxrwxr-x   0 gwyn      (1000) gwyn      (1000)    15356 2023-01-10 18:10:52.000000 storge-1.24/storge
-drwxr-xr-x   0 gwyn      (1000) gwyn      (1000)        0 2023-01-11 16:18:53.091217 storge-1.24/storge.egg-info/
--rw-r--r--   0 gwyn      (1000) gwyn      (1000)      535 2023-01-11 16:18:53.000000 storge-1.24/storge.egg-info/PKG-INFO
--rw-r--r--   0 gwyn      (1000) gwyn      (1000)      248 2023-01-11 16:18:53.000000 storge-1.24/storge.egg-info/SOURCES.txt
--rw-r--r--   0 gwyn      (1000) gwyn      (1000)        1 2023-01-11 16:18:53.000000 storge-1.24/storge.egg-info/dependency_links.txt
--rw-r--r--   0 gwyn      (1000) gwyn      (1000)       54 2023-01-11 16:18:53.000000 storge-1.24/storge.egg-info/requires.txt
--rw-r--r--   0 gwyn      (1000) gwyn      (1000)        9 2023-01-11 16:18:53.000000 storge-1.24/storge.egg-info/top_level.txt
--rwxrwxr-x   0 gwyn      (1000) gwyn      (1000)    14230 2023-01-10 22:49:36.000000 storge-1.24/storged
--rwxrwxr-x   0 gwyn      (1000) gwyn      (1000)      840 2019-10-30 23:12:00.000000 storge-1.24/torge
+drwxr-xr-x   0 gwyn      (1000) gwyn      (1000)        0 2023-08-04 20:09:14.058685 storge-1.25/
+-rw-rw-r--   0 gwyn      (1000) gwyn      (1000)    35147 2021-08-16 15:15:12.000000 storge-1.25/LICENSE.txt
+-rw-r--r--   0 gwyn      (1000) gwyn      (1000)      535 2023-08-04 20:09:14.058685 storge-1.25/PKG-INFO
+-rw-r--r--   0 gwyn      (1000) gwyn      (1000)      104 2023-01-10 19:21:41.000000 storge-1.25/pyproject.toml
+drwxr-xr-x   0 gwyn      (1000) gwyn      (1000)        0 2023-08-04 20:09:14.056686 storge-1.25/pystorge/
+-rw-rw-r--   0 gwyn      (1000) gwyn      (1000)     9265 2023-08-04 19:46:37.000000 storge-1.25/pystorge/__init__.py
+-rw-rw-r--   0 gwyn      (1000) gwyn      (1000)     1398 2021-08-16 15:15:12.000000 storge-1.25/pystorge/favicon.ico
+-rw-rw-r--   0 gwyn      (1000) gwyn      (1000)      892 2023-08-04 20:09:14.059685 storge-1.25/setup.cfg
+-rwxrwxr-x   0 gwyn      (1000) gwyn      (1000)    15727 2023-08-04 20:04:26.000000 storge-1.25/storge
+drwxr-xr-x   0 gwyn      (1000) gwyn      (1000)        0 2023-08-04 20:09:14.057685 storge-1.25/storge.egg-info/
+-rw-r--r--   0 gwyn      (1000) gwyn      (1000)      535 2023-08-04 20:09:14.000000 storge-1.25/storge.egg-info/PKG-INFO
+-rw-r--r--   0 gwyn      (1000) gwyn      (1000)      269 2023-08-04 20:09:14.000000 storge-1.25/storge.egg-info/SOURCES.txt
+-rw-r--r--   0 gwyn      (1000) gwyn      (1000)        1 2023-08-04 20:09:14.000000 storge-1.25/storge.egg-info/dependency_links.txt
+-rw-r--r--   0 gwyn      (1000) gwyn      (1000)       54 2023-08-04 20:09:14.000000 storge-1.25/storge.egg-info/requires.txt
+-rw-r--r--   0 gwyn      (1000) gwyn      (1000)        9 2023-08-04 20:09:14.000000 storge-1.25/storge.egg-info/top_level.txt
+-rwxrwxr-x   0 gwyn      (1000) gwyn      (1000)    14230 2023-08-04 20:04:38.000000 storge-1.25/storged
+drwxr-xr-x   0 gwyn      (1000) gwyn      (1000)        0 2023-08-04 20:09:14.057685 storge-1.25/tests/
+-rw-rw-r--   0 gwyn      (1000) gwyn      (1000)     3813 2022-01-12 17:54:50.000000 storge-1.25/tests/test_storge.py
+-rwxrwxr-x   0 gwyn      (1000) gwyn      (1000)      840 2019-10-30 23:12:00.000000 storge-1.25/torge
```

### Comparing `storge-1.24/LICENSE.txt` & `storge-1.25/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `storge-1.24/PKG-INFO` & `storge-1.25/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: storge
-Version: 1.24
+Version: 1.25
 Summary: Web file storage
 Home-page: https://codeberg.org/gwync/storge
 Author: Gwyn Ciesla
 Author-email: gwync@protonmail.com
 License: GPLv3+
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
 Storge uses CherryPy and MySQL to allow quick storage and sharing of files
```

### Comparing `storge-1.24/pystorge/__init__.py` & `storge-1.25/pystorge/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,15 +199,19 @@
     else:
         with open(keyf, 'r', encoding='utf-8') as keyfile:
             keycontent = keyfile.read()
         key = crypto.load_privatekey(crypto.FILETYPE_PEM, keycontent)
 
     # If cert exists, return, otherwise create.
     if os.path.isfile(certf):
-        return 0
+        certfile = open(certf, 'rt', encoding='utf-8').read() # pylint: disable=consider-using-with
+        ctx = crypto
+        certobj = ctx.load_certificate(ctx.FILETYPE_PEM, certfile)
+        if not certobj.has_expired():
+            return 0
 
     req = crypto.X509Req()
     req.get_subject().C = 'US'
     req.get_subject().ST = 'None'
     req.get_subject().L = 'None'
     req.get_subject().O = 'None'
     req.get_subject().CN = 'localhost'
```

### Comparing `storge-1.24/pystorge/favicon.ico` & `storge-1.25/pystorge/favicon.ico`

 * *Files identical despite different names*

### Comparing `storge-1.24/setup.cfg` & `storge-1.25/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [metadata]
 name = storge
-version = 1.24
+version = 1.25
 license = GPLv3+
 author = Gwyn Ciesla
 author_email = gwync@protonmail.com
 description = Web file storage
 long_description = Storge uses CherryPy and MySQL to allow quick storage and sharing of files
 long_description_content_type = text/x-rst
 url = https://codeberg.org/gwync/storge
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 	Operating System :: OS Independent
 packages = pystorge
 
 [options]
-python_requires = >=3.7
+python_requires = >=3.8
 packages = pystorge
 install_requires = 
 	requests
 	cherrypy
 	pyOpenSSL
 	sqlalchemy
 	pymysql
@@ -30,20 +30,21 @@
 	torge
 
 [options.package_data]
 pystorge = *.ico
 
 [tox:tox]
 skipsdist = True
-envlist = py37,py38,py39,py310
+envlist = py38,py39,py310,py311,py312
 
 [testenv]
 deps = 
 	pytest
 	pyOpenSSL
+	sqlalchemy
 commands = 
 	pytest
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `storge-1.24/storge` & `storge-1.25/storge`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/python3
 """ CherryPy application for file storage"""
 
-# Copyright (C) 2021 Gwyn Ciesla
+# Copyright (C) 2023 Gwyn Ciesla
 
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 # This program is distributed in the hope that it will be useful,
@@ -34,16 +34,18 @@
 def dehtml(text):
     """ Strip HTML tags """
     return ''.join(xml.etree.ElementTree.fromstring(text).itertext())
 
 URL = 'https://127.0.0.1:8080'
 PASSWORD = 'storge'
 
+TIMEOUT = 30
+
 PARSER = argparse.ArgumentParser(description="Send a file to a Storge server")
-PARSER.add_argument("-v", "--version", action="version", version="1.24")
+PARSER.add_argument("-v", "--version", action="version", version="1.25")
 PARSER.add_argument("-l", "--list", action="store_true", dest="lst", \
     help="List stored files")
 PARSER.add_argument("-r", "--remote", action="store", dest="remote", \
     help="URL to sync files from")
 PARSER.add_argument("-d", "--download", action="store", dest="download", \
     help="Download file by ID; N for newest, O for oldest, A for all")
 PARSER.add_argument("-u", "--url", action="store", dest="url", \
@@ -74,15 +76,15 @@
 
 if ARGS.url:
     URL = ARGS.url.rstrip('/')
 
 if ARGS.lst:
     try:
         OUTPUT = requests.post(URL + '/api', files={'flag': 'list'}, \
-            auth=HTTPDigestAuth('storge', PASSWORD), verify=False)
+            auth=HTTPDigestAuth('storge', PASSWORD), verify=False, timeout=TIMEOUT)
     except OSError:
         print("Unable to connect")
         sys.exit(1)
     if OUTPUT.status_code == 401:
         print("Invalid password")
         sys.exit(1)
 
@@ -92,26 +94,26 @@
         print(OUTPUT.text.replace('|||', '\n'))
 
     sys.exit(0)
 
 if ARGS.remote:
     try:
         OUTPUT = requests.post(URL + '/api', files={'flag': 'sync'}, \
-            auth=HTTPDigestAuth('storge', PASSWORD), verify=False)
+            auth=HTTPDigestAuth('storge', PASSWORD), verify=False, timeout=TIMEOUT)
     except OSError:
         print("Unable to connect")
         sys.exit(1)
 
     if OUTPUT.status_code == 401:
         print("Invalid password")
         sys.exit(1)
     LOCALHASHES = OUTPUT.text.split('|||')
     try:
         OUTPUT = requests.post(ARGS.remote + '/api', files={'flag': 'sync'}, \
-            auth=HTTPDigestAuth('storge', PASSWORD), verify=False)
+            auth=HTTPDigestAuth('storge', PASSWORD), verify=False, timeout=TIMEOUT)
     except OSError:
         print("Unable to connect")
         sys.exit(1)
 
     if OUTPUT.status_code == 401:
         print("Invalid password")
         sys.exit(1)
@@ -126,54 +128,54 @@
                     if int(len(tar_fields)) > 0:
                         if tar_fields[1] == fields[1]:
                             TRANSFER = 0
             if TRANSFER == 1:
                 try:
                     OUTPUT = requests.post(ARGS.remote + '/download', \
                         files={'fileid': fields[0]}, \
-                        auth=HTTPDigestAuth('storge', PASSWORD), verify=False)
+                        auth=HTTPDigestAuth('storge', PASSWORD), verify=False, timeout=TIMEOUT)
                 except OSError:
                     print("Unable to connect")
                     sys.exit(1)
 
                 if OUTPUT.status_code == 401:
                     print("Invalid password")
                     sys.exit(1)
                 FNAME = re.findall('"([^"]*)"', \
                     OUTPUT.headers.get('Content-Disposition').split('filename=')[1])[0]
                 try:
                     UPLOAD = requests.post(URL + '/upload', \
                         files={'userfile' : (FNAME, OUTPUT.content)}, \
-                            auth=HTTPDigestAuth('storge', PASSWORD), verify=False)
+                            auth=HTTPDigestAuth('storge', PASSWORD), verify=False, timeout=TIMEOUT)
                 except OSError:
                     print("Unable to connect")
                     sys.exit(1)
 
                 if UPLOAD.status_code == 401:
                     print("Invalid password")
                     sys.exit(1)
 
     sys.exit(0)
 
 if ARGS.pop:
     TARGETS = []
     try:
         OUTPUT = requests.post(URL + '/api', files={'flag': 'pop'}, \
-            auth=HTTPDigestAuth('storge', PASSWORD), verify=False)
+            auth=HTTPDigestAuth('storge', PASSWORD), verify=False, timeout=TIMEOUT)
     except OSError:
         print("Unable to connect")
         sys.exit(1)
     if OUTPUT.status_code == 401:
         print("Invalid password")
         sys.exit(1)
     TARGETS.append(OUTPUT.text.split('|||')[0].split(' ')[0])
     for target in TARGETS:
         try:
             OUTPUT = requests.post(URL + '/download', files={'fileid': target}, \
-                auth=HTTPDigestAuth('storge', PASSWORD), verify=False)
+                auth=HTTPDigestAuth('storge', PASSWORD), verify=False, timeout=TIMEOUT)
         except OSError:
             print("Unable to connect")
             sys.exit(1)
 
         if OUTPUT.status_code == 401:
             print("Invalid password")
             sys.exit(1)
@@ -187,15 +189,15 @@
 
         hashthing = hashlib.new('sha3_512')
         hashthing.update(OUTPUT.content)
         filehash = hashthing.hexdigest()
 
         try:
             SOUTPUT = requests.post(URL + '/api', files={'flag': 'sync'}, \
-                auth=HTTPDigestAuth('storge', PASSWORD), verify=False)
+                auth=HTTPDigestAuth('storge', PASSWORD), verify=False, timeout=TIMEOUT)
         except OSError:
             print("Unable to connect")
             sys.exit(1)
 
         if SOUTPUT.status_code == 401:
             print("Invalid password")
             sys.exit(1)
@@ -211,15 +213,15 @@
             print(FNAME + " exists, aborting.")
 
         if filehash != serverhash:
             print('Download issue;\nlocal hash: ' + filehash + '\nremote hash: ' + serverhash)
         else:
             try:
                 OUTPUT = requests.post(URL + '/delete', files={'fileid': target}, \
-                    auth=HTTPDigestAuth('storge', PASSWORD), verify=False)
+                    auth=HTTPDigestAuth('storge', PASSWORD), verify=False, timeout=TIMEOUT)
             except OSError:
                 print("Unable to connect")
                 sys.exit(1)
 
         if OUTPUT.status_code == 401:
             print("Invalid password")
             sys.exit(1)
@@ -228,52 +230,52 @@
 
 
 if ARGS.download:
     TARGETS = []
     if ARGS.download == 'N':
         try:
             OUTPUT = requests.post(URL + '/api', files={'flag': 'list'}, \
-                auth=HTTPDigestAuth('storge', PASSWORD), verify=False)
+                auth=HTTPDigestAuth('storge', PASSWORD), verify=False, timeout=TIMEOUT)
         except OSError:
             print("Unable to connect")
             sys.exit(1)
         if OUTPUT.status_code == 401:
             print("Invalid password")
             sys.exit(1)
         TARGETS.append(OUTPUT.text.split('|||')[0].split(' ')[0])
     elif ARGS.download == 'O':
         try:
             OUTPUT = requests.post(URL + '/api', files={'flag': 'list'}, \
-                auth=HTTPDigestAuth('storge', PASSWORD), verify=False)
+                auth=HTTPDigestAuth('storge', PASSWORD), verify=False, timeout=TIMEOUT)
         except OSError:
             print("Unable to connect")
             sys.exit(1)
         if OUTPUT.status_code == 401:
             print("Invalid password")
             sys.exit(1)
         TARGETS.append(OUTPUT.text.split('|||')[-1].split(' ')[0])
     elif ARGS.download == 'A':
         try:
             OUTPUT = requests.post(URL + '/api', files={'flag': 'list'}, \
-                auth=HTTPDigestAuth('storge', PASSWORD), verify=False)
+                auth=HTTPDigestAuth('storge', PASSWORD), verify=False, timeout=TIMEOUT)
         except OSError:
             print("Unable to connect")
             sys.exit(1)
         if OUTPUT.status_code == 401:
             print("Invalid password")
             sys.exit(1)
         for line in OUTPUT.text.split('|||'):
             TARGETS.append(line.split(' ')[0])
     else:
         TARGETS.append(ARGS.download)
 
     for target in TARGETS:
         try:
             OUTPUT = requests.post(URL + '/download', files={'fileid': target}, \
-                auth=HTTPDigestAuth('storge', PASSWORD), verify=False)
+                auth=HTTPDigestAuth('storge', PASSWORD), verify=False, timeout=TIMEOUT)
         except OSError:
             print("Unable to connect")
             sys.exit(1)
 
         if OUTPUT.status_code == 401:
             print("Invalid password")
             sys.exit(1)
@@ -287,15 +289,15 @@
 
         hashthing = hashlib.new('sha3_512')
         hashthing.update(OUTPUT.content)
         filehash = hashthing.hexdigest()
 
         try:
             SOUTPUT = requests.post(URL + '/api', files={'flag': 'sync'}, \
-                auth=HTTPDigestAuth('storge', PASSWORD), verify=False)
+                auth=HTTPDigestAuth('storge', PASSWORD), verify=False, timeout=TIMEOUT)
         except OSError:
             print("Unable to connect")
             sys.exit(1)
 
         if SOUTPUT.status_code == 401:
             print("Invalid password")
             sys.exit(1)
@@ -315,52 +317,52 @@
 
     sys.exit(0)
 
 if ARGS.delete:
     if ARGS.delete == 'N':
         try:
             OUTPUT = requests.post(URL + '/api', files={'flag': 'list'}, \
-                auth=HTTPDigestAuth('storge', PASSWORD), verify=False)
+                auth=HTTPDigestAuth('storge', PASSWORD), verify=False, timeout=TIMEOUT)
         except OSError:
             print("Unable to connect")
             sys.exit(1)
         if OUTPUT.status_code == 401:
             print("Invalid password")
             sys.exit(1)
         TARGET = OUTPUT.text.split('|||')[0].split(' ')[0]
     elif ARGS.delete == 'O':
         try:
             OUTPUT = requests.post(URL + '/api', files={'flag': 'list'}, \
-                auth=HTTPDigestAuth('storge', PASSWORD), verify=False)
+                auth=HTTPDigestAuth('storge', PASSWORD), verify=False, timeout=TIMEOUT)
         except OSError:
             print("Unable to connect")
             sys.exit(1)
         if OUTPUT.status_code == 401:
             print("Invalid password")
             sys.exit(1)
         TARGET = OUTPUT.text.split('|||')[-1].split(' ')[0]
     else:
         TARGET = ARGS.delete
 
     try:
         OUTPUT = requests.post(URL + '/delete', files={'fileid': TARGET}, \
-            auth=HTTPDigestAuth('storge', PASSWORD), verify=False)
+            auth=HTTPDigestAuth('storge', PASSWORD), verify=False, timeout=TIMEOUT)
     except OSError:
         print("Unable to connect")
         sys.exit(1)
 
     if OUTPUT.status_code == 401:
         print("Invalid password")
         sys.exit(1)
     sys.exit(0)
 
 if ARGS.vacuum:
     try:
         OUTPUT = requests.post(URL + '/vacuum', \
-            auth=HTTPDigestAuth('storge', PASSWORD), verify=False)
+            auth=HTTPDigestAuth('storge', PASSWORD), verify=False, timeout=TIMEOUT)
         SAVINGS = OUTPUT.text.split('>')[1]
         print(SAVINGS + " saved.")
     except OSError:
         print("Unable to connect")
         sys.exit(1)
 
     if OUTPUT.status_code == 401:
@@ -389,15 +391,15 @@
 
         hashthing = hashlib.new('sha3_512')
         hashthing.update(CONTENT)
         filehash = hashthing.hexdigest()
 
         try:
             OUTPUT = requests.post(URL + '/api', files={'flag': 'sync'}, \
-                auth=HTTPDigestAuth('storge', PASSWORD), verify=False)
+                auth=HTTPDigestAuth('storge', PASSWORD), verify=False, timeout=TIMEOUT)
         except OSError:
             print("Unable to connect")
             sys.exit(1)
 
         if OUTPUT.status_code == 401:
             print("Invalid password")
             sys.exit(1)
@@ -411,30 +413,30 @@
                     print("File " + file + " already uploaded, aborting.")
                     UPLOADED = 1
             if UPLOADED == 1:
                 break
         if UPLOADED == 0:
             try:
                 OUTPUT = requests.post(URL + '/upload', files={'userfile': open(file, 'rb')}, \
-                    auth=HTTPDigestAuth('storge', PASSWORD), verify=False) # pylint: disable=consider-using-with
+                    auth=HTTPDigestAuth('storge', PASSWORD), verify=False, timeout=TIMEOUT) # pylint: disable=consider-using-with
             except OSError:
                 print("Unable to connect")
                 sys.exit(1)
 
             if OUTPUT.status_code == 401:
                 print("Invalid password")
                 sys.exit(1)
 
             if OUTPUT.status_code != 200:
                 print(dehtml(OUTPUT))
 
             NEWUPLOADED = 0
             try:
                 OUTPUT = requests.post(URL + '/api', files={'flag': 'sync'}, \
-                    auth=HTTPDigestAuth('storge', PASSWORD), verify=False)
+                    auth=HTTPDigestAuth('storge', PASSWORD), verify=False, timeout=TIMEOUT)
             except OSError:
                 print("Unable to connect")
                 sys.exit(1)
 
             if OUTPUT.status_code == 401:
                 print("Invalid password")
                 sys.exit(1)
```

### Comparing `storge-1.24/storge.egg-info/PKG-INFO` & `storge-1.25/storge.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: storge
-Version: 1.24
+Version: 1.25
 Summary: Web file storage
 Home-page: https://codeberg.org/gwync/storge
 Author: Gwyn Ciesla
 Author-email: gwync@protonmail.com
 License: GPLv3+
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
 Storge uses CherryPy and MySQL to allow quick storage and sharing of files
```

### Comparing `storge-1.24/storged` & `storge-1.25/storged`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 import cherrypy
 from cherrypy.lib import auth_digest
 import sqlalchemy
 from sqlalchemy.sql import text
 import psutil
 import pystorge
 
-VERSION = "1.24"
-FOOTER = "<h6 align=center>Storge " + VERSION + " © Gwyn Ciesla 2021</h6>"
+VERSION = "1.25"
+FOOTER = "<h6 align=center>Storge " + VERSION + " © Gwyn Ciesla 2023</h6>"
 
 DATABASE = os.path.join(os.path.expanduser('~' +  getpass.getuser()), '.storge.db')
 DBHOST = "127.0.0.1"
 DBPASS = "storge"
 IPADDR = "127.0.0.1"
 PORT = 8080
 REFRESH = "15"
```

### Comparing `storge-1.24/torge` & `storge-1.25/torge`

 * *Files identical despite different names*

