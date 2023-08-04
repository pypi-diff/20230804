# Comparing `tmp/STEP.py-2.3.tar.gz` & `tmp/STEP.py-2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "STEP.py-2.3.tar", last modified: Wed Jul 26 01:14:29 2023, max compression
+gzip compressed data, was "STEP.py-2.4.tar", last modified: Fri Aug  4 02:10:22 2023, max compression
```

## Comparing `STEP.py-2.3.tar` & `STEP.py-2.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 eddo8    (197610) eddo8    (197610)        0 2023-07-26 01:14:29.890567 STEP.py-2.3/
--rw-r--r--   0 eddo8    (197610) eddo8    (197610)     1068 2022-09-28 02:37:16.000000 STEP.py-2.3/LICENSE.txt
--rw-r--r--   0 eddo8    (197610) eddo8    (197610)     6647 2023-07-26 01:14:29.891567 STEP.py-2.3/PKG-INFO
--rw-r--r--   0 eddo8    (197610) eddo8    (197610)     6314 2022-09-28 02:37:16.000000 STEP.py-2.3/README.md
-drwxr-xr-x   0 eddo8    (197610) eddo8    (197610)        0 2023-07-26 01:14:29.873567 STEP.py-2.3/STEP/
--rwxr--r--   0 eddo8    (197610) eddo8    (197610)     1317 2022-04-21 05:05:19.000000 STEP.py-2.3/STEP/Cleaner.py
--rwxr--r--   0 eddo8    (197610) eddo8    (197610)    40711 2023-07-26 01:10:41.000000 STEP.py-2.3/STEP/REST.py
--rwxr--r--   0 eddo8    (197610) eddo8    (197610)    14931 2022-12-01 04:21:29.000000 STEP.py-2.3/STEP/SOAP.py
--rwxr--r--   0 eddo8    (197610) eddo8    (197610)    11053 2022-04-21 05:05:19.000000 STEP.py-2.3/STEP/XML.py
--rwxr--r--   0 eddo8    (197610) eddo8    (197610)  3190632 2022-07-29 00:09:13.000000 STEP.py-2.3/STEP/XSD.py
--rwxr--r--   0 eddo8    (197610) eddo8    (197610)        0 2022-09-28 02:37:16.000000 STEP.py-2.3/STEP/__init__.py
-drwxr-xr-x   0 eddo8    (197610) eddo8    (197610)        0 2023-07-26 01:14:29.880567 STEP.py-2.3/STEP.py.egg-info/
--rw-r--r--   0 eddo8    (197610) eddo8    (197610)     6647 2023-07-26 01:14:29.000000 STEP.py-2.3/STEP.py.egg-info/PKG-INFO
--rw-r--r--   0 eddo8    (197610) eddo8    (197610)      379 2023-07-26 01:14:29.000000 STEP.py-2.3/STEP.py.egg-info/SOURCES.txt
--rw-r--r--   0 eddo8    (197610) eddo8    (197610)        1 2023-07-26 01:14:29.000000 STEP.py-2.3/STEP.py.egg-info/dependency_links.txt
--rw-r--r--   0 eddo8    (197610) eddo8    (197610)      117 2023-07-26 01:14:29.000000 STEP.py-2.3/STEP.py.egg-info/requires.txt
--rw-r--r--   0 eddo8    (197610) eddo8    (197610)        5 2023-07-26 01:14:29.000000 STEP.py-2.3/STEP.py.egg-info/top_level.txt
-drwxr-xr-x   0 eddo8    (197610) eddo8    (197610)        0 2023-07-26 01:14:29.887567 STEP.py-2.3/bin/
--rwxr--r--   0 eddo8    (197610) eddo8    (197610)      178 2022-04-21 05:05:19.000000 STEP.py-2.3/bin/excel2step.py
--rwxr--r--   0 eddo8    (197610) eddo8    (197610)      287 2022-07-26 22:14:49.000000 STEP.py-2.3/bin/step.rest.py
--rwxr--r--   0 eddo8    (197610) eddo8    (197610)      716 2022-07-26 22:16:51.000000 STEP.py-2.3/bin/step.soap.py
--rwxr--r--   0 eddo8    (197610) eddo8    (197610)    19193 2023-03-22 04:38:13.000000 STEP.py-2.3/bin/step2uml.py
--rwxr--r--   0 eddo8    (197610) eddo8    (197610)    16469 2022-07-19 06:08:05.000000 STEP.py-2.3/bin/uml2step.py
--rw-r--r--   0 eddo8    (197610) eddo8    (197610)       79 2023-07-26 01:14:29.891567 STEP.py-2.3/setup.cfg
--rwxr--r--   0 eddo8    (197610) eddo8    (197610)      980 2023-07-26 01:09:25.000000 STEP.py-2.3/setup.py
-drwxr-xr-x   0 eddo8    (197610) eddo8    (197610)        0 2023-07-26 01:14:29.889567 STEP.py-2.3/test/
--rwxr--r--   0 eddo8    (197610) eddo8    (197610)    10118 2022-09-01 05:43:58.000000 STEP.py-2.3/test/test_rest.py
+drwxr-xr-x   0 eddo8    (197610) eddo8    (197610)        0 2023-08-04 02:10:22.474113 STEP.py-2.4/
+-rw-r--r--   0 eddo8    (197610) eddo8    (197610)     1068 2022-09-28 02:37:16.000000 STEP.py-2.4/LICENSE.txt
+-rw-r--r--   0 eddo8    (197610) eddo8    (197610)     6610 2023-08-04 02:10:22.474113 STEP.py-2.4/PKG-INFO
+-rw-r--r--   0 eddo8    (197610) eddo8    (197610)     6314 2022-09-28 02:37:16.000000 STEP.py-2.4/README.md
+drwxr-xr-x   0 eddo8    (197610) eddo8    (197610)        0 2023-08-04 02:10:22.456113 STEP.py-2.4/STEP/
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)     1317 2022-04-21 05:05:19.000000 STEP.py-2.4/STEP/Cleaner.py
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)    41839 2023-08-04 02:09:43.000000 STEP.py-2.4/STEP/REST.py
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)    14931 2022-12-01 04:21:29.000000 STEP.py-2.4/STEP/SOAP.py
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)    11053 2022-04-21 05:05:19.000000 STEP.py-2.4/STEP/XML.py
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)  3190632 2022-07-29 00:09:13.000000 STEP.py-2.4/STEP/XSD.py
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)        0 2022-09-28 02:37:16.000000 STEP.py-2.4/STEP/__init__.py
+drwxr-xr-x   0 eddo8    (197610) eddo8    (197610)        0 2023-08-04 02:10:22.463115 STEP.py-2.4/STEP.py.egg-info/
+-rw-r--r--   0 eddo8    (197610) eddo8    (197610)     6610 2023-08-04 02:10:22.000000 STEP.py-2.4/STEP.py.egg-info/PKG-INFO
+-rw-r--r--   0 eddo8    (197610) eddo8    (197610)      379 2023-08-04 02:10:22.000000 STEP.py-2.4/STEP.py.egg-info/SOURCES.txt
+-rw-r--r--   0 eddo8    (197610) eddo8    (197610)        1 2023-08-04 02:10:22.000000 STEP.py-2.4/STEP.py.egg-info/dependency_links.txt
+-rw-r--r--   0 eddo8    (197610) eddo8    (197610)      117 2023-08-04 02:10:22.000000 STEP.py-2.4/STEP.py.egg-info/requires.txt
+-rw-r--r--   0 eddo8    (197610) eddo8    (197610)        5 2023-08-04 02:10:22.000000 STEP.py-2.4/STEP.py.egg-info/top_level.txt
+drwxr-xr-x   0 eddo8    (197610) eddo8    (197610)        0 2023-08-04 02:10:22.470114 STEP.py-2.4/bin/
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)      178 2022-04-21 05:05:19.000000 STEP.py-2.4/bin/excel2step.py
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)      287 2022-07-26 22:14:49.000000 STEP.py-2.4/bin/step.rest.py
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)      716 2022-07-26 22:16:51.000000 STEP.py-2.4/bin/step.soap.py
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)    19193 2023-03-22 04:38:13.000000 STEP.py-2.4/bin/step2uml.py
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)    16469 2022-07-19 06:08:05.000000 STEP.py-2.4/bin/uml2step.py
+-rw-r--r--   0 eddo8    (197610) eddo8    (197610)       79 2023-08-04 02:10:22.475113 STEP.py-2.4/setup.cfg
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)      980 2023-08-04 01:57:28.000000 STEP.py-2.4/setup.py
+drwxr-xr-x   0 eddo8    (197610) eddo8    (197610)        0 2023-08-04 02:10:22.472113 STEP.py-2.4/test/
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)    10118 2022-09-01 05:43:58.000000 STEP.py-2.4/test/test_rest.py
```

### Comparing `STEP.py-2.3/LICENSE.txt` & `STEP.py-2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `STEP.py-2.3/PKG-INFO` & `STEP.py-2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: STEP.py
-Version: 2.3
-Summary: UNKNOWN
+Version: 2.4
 Home-page: https://github.com/eddo888/STEP.py
+Download-URL: https://github.com/eddo888/STEP.py/archive/2.4.tar.gz
 Author: David Edson
 Author-email: eddo888@tpg.com.au
 License: MIT
-Download-URL: https://github.com/eddo888/STEP.py/archive/2.3.tar.gz
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # STEP.py
 
 python libraries to support Stibo STEP MDM APIs
 
@@ -174,9 +172,7 @@
 ["UML-Reference-Stereotypes.sparxea.xml" Sparx->Configure->Model->Transfer->Import Reference Data, then select file and choose specifications](https://github.com/eddo888/STEP.py/raw/master/UML/UML-Reference-Stereotypes.sparxea.xml)
 
 
 
 
 
 
-
-
```

### Comparing `STEP.py-2.3/README.md` & `STEP.py-2.4/README.md`

 * *Files identical despite different names*

### Comparing `STEP.py-2.3/STEP/Cleaner.py` & `STEP.py-2.4/STEP/Cleaner.py`

 * *Files identical despite different names*

### Comparing `STEP.py-2.3/STEP/REST.py` & `STEP.py-2.4/STEP/REST.py`

 * *Files 2% similar despite different names*

```diff
@@ -247,14 +247,21 @@
 		'''
 		get the asset by ID
 		'''
 		return super().get('%s/%s'%(self.base,id))
 
 
 	#________________________________________________________________________________________________
+	@args.operation(help='approve asset by id')
+	@args.parameter(name='id', help='the ID of asset')
+	def approve(self, id):
+		return super().post('%s/%s/approve'%(self.base,id))
+
+
+	#________________________________________________________________________________________________
 	@args.operation
 	@args.parameter(name='output', short='o', help='where to store the content, defautls to stdout')
 	def content(self, id, output=None):
 		'''
 		downlaod the asset to a local directory
 		'''
 		path='%s/%s/content'%(self.base, id)
@@ -442,14 +449,21 @@
 		if save:
 			with open('/restapi/products/%s'%id,'w') as output:
 				output.write(result)
 		return result
 
 	
 	#________________________________________________________________________________________________
+	@args.operation(help='approve product by id')
+	@args.parameter(name='id', help='the ID of product')
+	def approve(self, id):
+		return super().post('%s/%s/approve'%(self.base,id))
+
+
+	#________________________________________________________________________________________________
 	@args.operation(help='create a new product')
 	@args.parameter(name='name', short='n')
 	@args.parameter(name='values', short='a', nargs='*', metavar='attr=value')
 	def create(self, parent, objectType, name=None, values=[]):
 		body=dict(
 			parent=parent,
 			objectType=objectType,
@@ -609,14 +623,21 @@
 	@args.operation(help='get entity by id')
 	@args.parameter(name='id', help='the ID of entity')
 	def get(self, id):
 		return super().get('%s/%s'%(self.base,id))
 
 
 	#________________________________________________________________________________________________
+	@args.operation(help='approve entity by id')
+	@args.parameter(name='id', help='the ID of entity')
+	def approve(self, id):
+		return super().post('%s/%s/approve'%(self.base,id))
+
+
+	#________________________________________________________________________________________________
 	@args.operation(help='get children of entity by id')
 	@args.parameter(name='id', help='the ID of entity')
 	def children(self, id):
 		return super().get('%s/%s/children'%(self.base,id))
 
 
 	#________________________________________________________________________________________________
@@ -690,14 +711,21 @@
 	@args.operation(help='get classification by id')
 	@args.parameter(name='id', help='the ID of classification')
 	def get(self, id):
 		return super().get('%s/%s'%(self.base,id))
 
 
 	#________________________________________________________________________________________________
+	@args.operation(help='approve classification by id')
+	@args.parameter(name='id', help='the ID of classification')
+	def approve(self, id):
+		return super().post('%s/%s/approve'%(self.base,id))
+
+
+	#________________________________________________________________________________________________
 	@args.operation(help='create a new classification')
 	@args.parameter(name='name', short='n')
 	@args.parameter(name='values', short='a', nargs='*', metavar='attr=value')
 	def create(self, parent, objectType, name=None, values=[]):
 		body=dict(
 			parent=parent,
 			objectType=objectType,
```

### Comparing `STEP.py-2.3/STEP/SOAP.py` & `STEP.py-2.4/STEP/SOAP.py`

 * *Files identical despite different names*

### Comparing `STEP.py-2.3/STEP/XML.py` & `STEP.py-2.4/STEP/XML.py`

 * *Files identical despite different names*

### Comparing `STEP.py-2.3/STEP/XSD.py` & `STEP.py-2.4/STEP/XSD.py`

 * *Files identical despite different names*

### Comparing `STEP.py-2.3/STEP.py.egg-info/PKG-INFO` & `STEP.py-2.4/STEP.py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: STEP.py
-Version: 2.3
-Summary: UNKNOWN
+Version: 2.4
 Home-page: https://github.com/eddo888/STEP.py
+Download-URL: https://github.com/eddo888/STEP.py/archive/2.4.tar.gz
 Author: David Edson
 Author-email: eddo888@tpg.com.au
 License: MIT
-Download-URL: https://github.com/eddo888/STEP.py/archive/2.3.tar.gz
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # STEP.py
 
 python libraries to support Stibo STEP MDM APIs
 
@@ -174,9 +172,7 @@
 ["UML-Reference-Stereotypes.sparxea.xml" Sparx->Configure->Model->Transfer->Import Reference Data, then select file and choose specifications](https://github.com/eddo888/STEP.py/raw/master/UML/UML-Reference-Stereotypes.sparxea.xml)
 
 
 
 
 
 
-
-
```

### Comparing `STEP.py-2.3/bin/step.soap.py` & `STEP.py-2.4/bin/step.soap.py`

 * *Files identical despite different names*

### Comparing `STEP.py-2.3/bin/step2uml.py` & `STEP.py-2.4/bin/step2uml.py`

 * *Files identical despite different names*

### Comparing `STEP.py-2.3/bin/uml2step.py` & `STEP.py-2.4/bin/uml2step.py`

 * *Files identical despite different names*

### Comparing `STEP.py-2.3/setup.py` & `STEP.py-2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 pwd = path.abspath(path.dirname(__file__))
 with codecs.open(path.join(pwd, 'README.md'), 'r', encoding='utf8') as input:
 	long_description = input.read()
 
 name='STEP.py'
 user='eddo888'
-version='2.3'
+version='2.4'
 
 setup(
 	name=name,
 	version=version,
 	license='MIT',
 	long_description=long_description,
 	long_description_content_type="text/markdown",
```

### Comparing `STEP.py-2.3/test/test_rest.py` & `STEP.py-2.4/test/test_rest.py`

 * *Files identical despite different names*

