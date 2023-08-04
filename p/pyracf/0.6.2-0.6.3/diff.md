# Comparing `tmp/pyracf-0.6.2.tar.gz` & `tmp/pyracf-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyracf-0.6.2.tar", last modified: Sat May  6 08:30:34 2023, max compression
+gzip compressed data, was "pyracf-0.6.3.tar", last modified: Fri Aug  4 09:28:20 2023, max compression
```

## Comparing `pyracf-0.6.2.tar` & `pyracf-0.6.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2023-05-06 08:30:34.333418 pyracf-0.6.2/
--rw-rw-r--   0 henri     (1000) henri     (1000)    11357 2023-05-01 20:17:28.000000 pyracf-0.6.2/LICENSE
--rw-rw-r--   0 henri     (1000) henri     (1000)      172 2022-04-04 21:07:37.000000 pyracf-0.6.2/MANIFEST.in
--rw-rw-r--   0 henri     (1000) henri     (1000)     8184 2023-05-06 08:30:34.333418 pyracf-0.6.2/PKG-INFO
--rw-rw-r--   0 henri     (1000) henri     (1000)     7659 2023-05-06 08:24:36.000000 pyracf-0.6.2/README.md
--rw-rw-r--   0 henri     (1000) henri     (1000)       38 2023-05-06 08:30:34.333418 pyracf-0.6.2/setup.cfg
--rw-rw-r--   0 henri     (1000) henri     (1000)      956 2023-05-06 08:22:26.000000 pyracf-0.6.2/setup.py
-drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2023-05-06 08:30:34.329418 pyracf-0.6.2/src/
-drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2023-05-06 08:30:34.329418 pyracf-0.6.2/src/pyracf/
--rw-rw-r--   0 henri     (1000) henri     (1000)    33408 2023-05-06 08:23:06.000000 pyracf-0.6.2/src/pyracf/__init__.py
--rw-rw-r--   0 henri     (1000) henri     (1000)   126403 2023-05-05 19:32:44.000000 pyracf-0.6.2/src/pyracf/offsets.json
-drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2023-05-06 08:30:34.333418 pyracf-0.6.2/src/pyracf.egg-info/
--rw-rw-r--   0 henri     (1000) henri     (1000)     8184 2023-05-06 08:30:34.000000 pyracf-0.6.2/src/pyracf.egg-info/PKG-INFO
--rw-rw-r--   0 henri     (1000) henri     (1000)      254 2023-05-06 08:30:34.000000 pyracf-0.6.2/src/pyracf.egg-info/SOURCES.txt
--rw-rw-r--   0 henri     (1000) henri     (1000)        1 2023-05-06 08:30:34.000000 pyracf-0.6.2/src/pyracf.egg-info/dependency_links.txt
--rw-rw-r--   0 henri     (1000) henri     (1000)       38 2023-05-06 08:30:34.000000 pyracf-0.6.2/src/pyracf.egg-info/requires.txt
--rw-rw-r--   0 henri     (1000) henri     (1000)        7 2023-05-06 08:30:34.000000 pyracf-0.6.2/src/pyracf.egg-info/top_level.txt
+drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2023-08-04 09:28:20.053517 pyracf-0.6.3/
+-rw-rw-r--   0 henri     (1000) henri     (1000)    11357 2023-05-01 20:17:28.000000 pyracf-0.6.3/LICENSE
+-rw-rw-r--   0 henri     (1000) henri     (1000)      172 2022-04-04 21:07:37.000000 pyracf-0.6.3/MANIFEST.in
+-rw-rw-r--   0 henri     (1000) henri     (1000)     8184 2023-08-04 09:28:20.053517 pyracf-0.6.3/PKG-INFO
+-rw-rw-r--   0 henri     (1000) henri     (1000)     7659 2023-05-06 08:24:36.000000 pyracf-0.6.3/README.md
+-rw-rw-r--   0 henri     (1000) henri     (1000)       38 2023-08-04 09:28:20.053517 pyracf-0.6.3/setup.cfg
+-rw-rw-r--   0 henri     (1000) henri     (1000)      956 2023-08-04 09:28:14.000000 pyracf-0.6.3/setup.py
+drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2023-08-04 09:28:20.049517 pyracf-0.6.3/src/
+drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2023-08-04 09:28:20.053517 pyracf-0.6.3/src/pyracf/
+-rw-rw-r--   0 henri     (1000) henri     (1000)    33408 2023-05-06 08:23:06.000000 pyracf-0.6.3/src/pyracf/__init__.py
+-rw-rw-r--   0 henri     (1000) henri     (1000)   127367 2023-08-04 09:26:20.000000 pyracf-0.6.3/src/pyracf/offsets.json
+drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2023-08-04 09:28:20.053517 pyracf-0.6.3/src/pyracf.egg-info/
+-rw-rw-r--   0 henri     (1000) henri     (1000)     8184 2023-08-04 09:28:20.000000 pyracf-0.6.3/src/pyracf.egg-info/PKG-INFO
+-rw-rw-r--   0 henri     (1000) henri     (1000)      254 2023-08-04 09:28:20.000000 pyracf-0.6.3/src/pyracf.egg-info/SOURCES.txt
+-rw-rw-r--   0 henri     (1000) henri     (1000)        1 2023-08-04 09:28:20.000000 pyracf-0.6.3/src/pyracf.egg-info/dependency_links.txt
+-rw-rw-r--   0 henri     (1000) henri     (1000)       38 2023-08-04 09:28:20.000000 pyracf-0.6.3/src/pyracf.egg-info/requires.txt
+-rw-rw-r--   0 henri     (1000) henri     (1000)        7 2023-08-04 09:28:20.000000 pyracf-0.6.3/src/pyracf.egg-info/top_level.txt
```

### Comparing `pyracf-0.6.2/LICENSE` & `pyracf-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyracf-0.6.2/PKG-INFO` & `pyracf-0.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyracf
-Version: 0.6.2
+Version: 0.6.3
 Summary: Parsing IRRDBU00 unloads in panda dataframes.
 Home-page: https://github.com/wizardofzos/pyracf
 Author: Wizard of z/OS
 Author-email: wizard@zdevops.com
 Project-URL: Bug Tracker, https://github.com/wizardofzos/pyracf/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `pyracf-0.6.2/README.md` & `pyracf-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `pyracf-0.6.2/setup.py` & `pyracf-0.6.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyracf",
-    version="0.6.2",
+    version="0.6.3",
     author="Wizard of z/OS",
     author_email="wizard@zdevops.com",
     description="Parsing IRRDBU00 unloads in panda dataframes.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/wizardofzos/pyracf",
     project_urls={
```

### Comparing `pyracf-0.6.2/src/pyracf/__init__.py` & `pyracf-0.6.3/src/pyracf/__init__.py`

 * *Files identical despite different names*

### Comparing `pyracf-0.6.2/src/pyracf/offsets.json` & `pyracf-0.6.3/src/pyracf/offsets.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997665732959851%*

 * *Differences: {"'user-basic-data-record'": "{'offsets': {insert: [(44, OrderedDict([('field-name', "*

 * *                             "'USBD_LEG_PWDHIST_CT'), ('type', 'int'), ('start', '605'), ('end', "*

 * *                             "'607')])), (45, OrderedDict([('field-name', 'USBD_XPW_PWDHIST_CT'), "*

 * *                             "('type', 'int'), ('start', '609'), ('end', '611')])), (46, "*

 * *                             "OrderedDict([('field-name', 'USBD_PHR_ALG'), ('type', 'char'), "*

 * *                             "('start',  […]*

```diff
@@ -1926,14 +1926,56 @@
                 "type": "yes/no"
             },
             {
                 "end": "603",
                 "field-name": "USBD_PWD_ALG",
                 "start": "592",
                 "type": "char"
+            },
+            {
+                "end": "607",
+                "field-name": "USBD_LEG_PWDHIST_CT",
+                "start": "605",
+                "type": "int"
+            },
+            {
+                "end": "611",
+                "field-name": "USBD_XPW_PWDHIST_CT",
+                "start": "609",
+                "type": "int"
+            },
+            {
+                "end": "624",
+                "field-name": "USBD_PHR_ALG",
+                "start": "613",
+                "type": "char"
+            },
+            {
+                "end": "628",
+                "field-name": "USBD_LEG_PHRHIST_CT",
+                "start": "626",
+                "type": "int"
+            },
+            {
+                "end": "632",
+                "field-name": "USBD_XPW_PHRHIST_CT",
+                "start": "630",
+                "type": "int"
+            },
+            {
+                "end": "637",
+                "field-name": "USBD_ROAUDIT",
+                "start": "634",
+                "type": "char"
+            },
+            {
+                "end": "641",
+                "field-name": "USBD_MFA_FALLBACK",
+                "start": "639",
+                "type": "char"
             }
         ],
         "record-type": "0200",
         "ref-url": "https://www-01.ibm.com/support/knowledgecenter/SSLTBW_1.13.0/com.ibm.zos.r13.icha300/usr.htm%23wq1264"
     },
     "user-categories-record": {
         "offsets": [
```

### Comparing `pyracf-0.6.2/src/pyracf.egg-info/PKG-INFO` & `pyracf-0.6.3/src/pyracf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyracf
-Version: 0.6.2
+Version: 0.6.3
 Summary: Parsing IRRDBU00 unloads in panda dataframes.
 Home-page: https://github.com/wizardofzos/pyracf
 Author: Wizard of z/OS
 Author-email: wizard@zdevops.com
 Project-URL: Bug Tracker, https://github.com/wizardofzos/pyracf/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

