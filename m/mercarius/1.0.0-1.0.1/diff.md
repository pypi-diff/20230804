# Comparing `tmp/mercarius-1.0.0.tar.gz` & `tmp/mercarius-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mercarius-1.0.0.tar", last modified: Sat Feb 25 20:50:23 2023, max compression
+gzip compressed data, was "mercarius-1.0.1.tar", last modified: Fri Aug  4 08:04:43 2023, max compression
```

## Comparing `mercarius-1.0.0.tar` & `mercarius-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 batmanuel   (501) staff       (20)        0 2023-02-25 20:50:23.378803 mercarius-1.0.0/
--rw-r--r--   0 batmanuel   (501) staff       (20)       43 2023-02-25 01:23:38.000000 mercarius-1.0.0/MANIFEST.in
--rw-r--r--   0 batmanuel   (501) staff       (20)     2999 2023-02-25 20:50:23.378700 mercarius-1.0.0/PKG-INFO
--rw-r--r--   0 batmanuel   (501) staff       (20)     2673 2023-02-25 20:47:28.000000 mercarius-1.0.0/README.md
-drwxr-xr-x   0 batmanuel   (501) staff       (20)        0 2023-02-25 20:50:23.377802 mercarius-1.0.0/mercarius/
--rw-r--r--   0 batmanuel   (501) staff       (20)       46 2023-02-25 20:08:27.000000 mercarius-1.0.0/mercarius/__init__.py
--rw-r--r--   0 batmanuel   (501) staff       (20)     3599 2023-02-25 20:14:02.000000 mercarius-1.0.0/mercarius/mercari.py
-drwxr-xr-x   0 batmanuel   (501) staff       (20)        0 2023-02-25 20:50:23.378552 mercarius-1.0.0/mercarius.egg-info/
--rw-r--r--   0 batmanuel   (501) staff       (20)     2999 2023-02-25 20:50:23.000000 mercarius-1.0.0/mercarius.egg-info/PKG-INFO
--rw-r--r--   0 batmanuel   (501) staff       (20)      254 2023-02-25 20:50:23.000000 mercarius-1.0.0/mercarius.egg-info/SOURCES.txt
--rw-r--r--   0 batmanuel   (501) staff       (20)        1 2023-02-25 20:50:23.000000 mercarius-1.0.0/mercarius.egg-info/dependency_links.txt
--rw-r--r--   0 batmanuel   (501) staff       (20)       89 2023-02-25 20:50:23.000000 mercarius-1.0.0/mercarius.egg-info/requires.txt
--rw-r--r--   0 batmanuel   (501) staff       (20)       10 2023-02-25 20:50:23.000000 mercarius-1.0.0/mercarius.egg-info/top_level.txt
--rw-r--r--   0 batmanuel   (501) staff       (20)       89 2023-02-25 01:25:01.000000 mercarius-1.0.0/requirements.txt
--rw-r--r--   0 batmanuel   (501) staff       (20)       38 2023-02-25 20:50:23.378835 mercarius-1.0.0/setup.cfg
--rw-r--r--   0 batmanuel   (501) staff       (20)      676 2023-02-25 20:47:40.000000 mercarius-1.0.0/setup.py
+drwxr-xr-x   0 batmanuel   (501) staff       (20)        0 2023-08-04 08:04:43.459177 mercarius-1.0.1/
+-rw-r--r--   0 batmanuel   (501) staff       (20)       43 2023-02-25 01:23:38.000000 mercarius-1.0.1/MANIFEST.in
+-rw-r--r--   0 batmanuel   (501) staff       (20)     3198 2023-08-04 08:04:43.459061 mercarius-1.0.1/PKG-INFO
+-rw-r--r--   0 batmanuel   (501) staff       (20)     2872 2023-08-04 08:03:32.000000 mercarius-1.0.1/README.md
+drwxr-xr-x   0 batmanuel   (501) staff       (20)        0 2023-08-04 08:04:43.458271 mercarius-1.0.1/mercarius/
+-rw-r--r--   0 batmanuel   (501) staff       (20)       46 2023-02-25 20:54:21.000000 mercarius-1.0.1/mercarius/__init__.py
+-rw-r--r--   0 batmanuel   (501) staff       (20)     4863 2023-08-04 08:02:39.000000 mercarius-1.0.1/mercarius/mercari.py
+drwxr-xr-x   0 batmanuel   (501) staff       (20)        0 2023-08-04 08:04:43.458912 mercarius-1.0.1/mercarius.egg-info/
+-rw-r--r--   0 batmanuel   (501) staff       (20)     3198 2023-08-04 08:04:43.000000 mercarius-1.0.1/mercarius.egg-info/PKG-INFO
+-rw-r--r--   0 batmanuel   (501) staff       (20)      254 2023-08-04 08:04:43.000000 mercarius-1.0.1/mercarius.egg-info/SOURCES.txt
+-rw-r--r--   0 batmanuel   (501) staff       (20)        1 2023-08-04 08:04:43.000000 mercarius-1.0.1/mercarius.egg-info/dependency_links.txt
+-rw-r--r--   0 batmanuel   (501) staff       (20)       89 2023-08-04 08:04:43.000000 mercarius-1.0.1/mercarius.egg-info/requires.txt
+-rw-r--r--   0 batmanuel   (501) staff       (20)       10 2023-08-04 08:04:43.000000 mercarius-1.0.1/mercarius.egg-info/top_level.txt
+-rw-r--r--   0 batmanuel   (501) staff       (20)       89 2023-02-25 01:25:01.000000 mercarius-1.0.1/requirements.txt
+-rw-r--r--   0 batmanuel   (501) staff       (20)       38 2023-08-04 08:04:43.459216 mercarius-1.0.1/setup.cfg
+-rw-r--r--   0 batmanuel   (501) staff       (20)      676 2023-08-04 08:04:28.000000 mercarius-1.0.1/setup.py
```

### Comparing `mercarius-1.0.0/PKG-INFO` & `mercarius-1.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercarius
-Version: 1.0.0
+Version: 1.0.1
 Summary: mercari-us api-like wrapper
 Home-page: https://github.com/marvinody/mercari-us/
 Author: marvinody
 Author-email: manny@pypi.sadpanda.moe
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
@@ -47,7 +47,19 @@
 
 ```
 
 It'll print out a blob of JSON so you can see all the available properties on the item object.
 
 **Note, you're not guaranteed to have all unique items and may see duplicates.** I recommend to run the final list through a duplicate checker using the id property just to be safe. During my testing it was pretty random.
 
+
+
+# Development
+
+Clone this repo, install the dependencies in `requirement.txt` and off you go.
+
+## Deploying / Publishing
+
+- `python setup.py sdist`
+
+- `twine upload dist/mercari-<version>.tar.gz`
+
```

### Comparing `mercarius-1.0.0/README.md` & `mercarius-1.0.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -33,8 +33,20 @@
 print('All keys in a single item:')
 print(json.dumps(merch[0], indent=2))
 
 ```
 
 It'll print out a blob of JSON so you can see all the available properties on the item object.
 
-**Note, you're not guaranteed to have all unique items and may see duplicates.** I recommend to run the final list through a duplicate checker using the id property just to be safe. During my testing it was pretty random.
+**Note, you're not guaranteed to have all unique items and may see duplicates.** I recommend to run the final list through a duplicate checker using the id property just to be safe. During my testing it was pretty random.
+
+
+
+# Development
+
+Clone this repo, install the dependencies in `requirement.txt` and off you go.
+
+## Deploying / Publishing
+
+- `python setup.py sdist`
+
+- `twine upload dist/mercari-<version>.tar.gz`
```

### Comparing `mercarius-1.0.0/mercarius.egg-info/PKG-INFO` & `mercarius-1.0.1/mercarius.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercarius
-Version: 1.0.0
+Version: 1.0.1
 Summary: mercari-us api-like wrapper
 Home-page: https://github.com/marvinody/mercari-us/
 Author: marvinody
 Author-email: manny@pypi.sadpanda.moe
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
@@ -47,7 +47,19 @@
 
 ```
 
 It'll print out a blob of JSON so you can see all the available properties on the item object.
 
 **Note, you're not guaranteed to have all unique items and may see duplicates.** I recommend to run the final list through a duplicate checker using the id property just to be safe. During my testing it was pretty random.
 
+
+
+# Development
+
+Clone this repo, install the dependencies in `requirement.txt` and off you go.
+
+## Deploying / Publishing
+
+- `python setup.py sdist`
+
+- `twine upload dist/mercari-<version>.tar.gz`
+
```

### Comparing `mercarius-1.0.0/setup.py` & `mercarius-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = f.read().splitlines()
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='mercarius',
-    version='1.0.0',
+    version='1.0.1',
     author='marvinody',
     author_email='manny@pypi.sadpanda.moe',
     description='mercari-us api-like wrapper',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/marvinody/mercari-us/',
     packages=setuptools.find_packages(),
```

