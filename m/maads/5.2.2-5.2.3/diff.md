# Comparing `tmp/maads-5.2.2.tar.gz` & `tmp/maads-5.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\maads-5.2.2.tar", last modified: Sat Jul 10 18:05:41 2021, max compression
+gzip compressed data, was "maads-5.2.3.tar", last modified: Fri Aug  4 19:17:43 2023, max compression
```

## Comparing `maads-5.2.2.tar` & `maads-5.2.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2021-07-10 18:05:41.000000 maads-5.2.2/
--rw-rw-rw-   0        0        0     1067 2021-04-28 21:31:09.000000 maads-5.2.2/LICENSE.txt
--rw-rw-rw-   0        0        0       65 2021-01-25 23:03:44.000000 maads-5.2.2/MANIFEST.in
--rw-rw-rw-   0        0        0   116029 2021-07-10 18:05:41.000000 maads-5.2.2/PKG-INFO
--rw-rw-rw-   0        0        0    94527 2021-07-10 18:01:07.000000 maads-5.2.2/README.md
-drwxrwxrwx   0        0        0        0 2021-07-10 18:05:41.000000 maads-5.2.2/maads/
--rw-rw-rw-   0        0        0     2089 2020-12-21 23:10:17.000000 maads-5.2.2/maads/__init__.py
--rw-rw-rw-   0        0        0     8841 2020-10-18 21:34:32.000000 maads-5.2.2/maads/balancedata.py
--rw-rw-rw-   0        0        0     5395 2020-06-27 20:48:48.000000 maads-5.2.2/maads/callmas.py
--rw-rw-rw-   0        0        0    65036 2021-03-10 20:43:11.000000 maads-5.2.2/maads/sendfiles.py
-drwxrwxrwx   0        0        0        0 2021-07-10 18:05:41.000000 maads-5.2.2/maads.egg-info/
--rw-rw-rw-   0        0        0   116029 2021-07-10 18:05:41.000000 maads-5.2.2/maads.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2021-07-10 18:05:41.000000 maads-5.2.2/maads.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-07-10 18:05:41.000000 maads-5.2.2/maads.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      115 2021-07-10 18:05:41.000000 maads-5.2.2/maads.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2021-07-10 18:05:41.000000 maads-5.2.2/maads.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      122 2021-02-05 16:13:30.000000 maads-5.2.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2021-07-10 18:05:41.000000 maads-5.2.2/setup.cfg
--rw-rw-rw-   0        0        0      993 2021-07-10 17:59:22.000000 maads-5.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 19:17:43.195812 maads-5.2.3/
+-rw-rw-rw-   0        0        0     1067 2021-04-28 21:31:09.000000 maads-5.2.3/LICENSE.txt
+-rw-rw-rw-   0        0        0       65 2021-01-25 23:03:44.000000 maads-5.2.3/MANIFEST.in
+-rw-rw-rw-   0        0        0    37272 2023-08-04 19:17:43.194116 maads-5.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0    36767 2023-08-04 19:12:05.000000 maads-5.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-08-04 19:17:43.162243 maads-5.2.3/maads/
+-rw-rw-rw-   0        0        0     2089 2020-12-21 23:10:17.000000 maads-5.2.3/maads/__init__.py
+-rw-rw-rw-   0        0        0     8841 2020-10-18 21:34:32.000000 maads-5.2.3/maads/balancedata.py
+-rw-rw-rw-   0        0        0     5395 2020-06-27 20:48:48.000000 maads-5.2.3/maads/callmas.py
+-rw-rw-rw-   0        0        0    46299 2022-02-06 19:22:46.000000 maads-5.2.3/maads/sendfiles.py
+drwxrwxrwx   0        0        0        0 2023-08-04 19:17:43.193606 maads-5.2.3/maads.egg-info/
+-rw-rw-rw-   0        0        0    37272 2023-08-04 19:17:42.000000 maads-5.2.3/maads.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2023-08-04 19:17:43.000000 maads-5.2.3/maads.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 19:17:42.000000 maads-5.2.3/maads.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      115 2023-08-04 19:17:42.000000 maads-5.2.3/maads.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-08-04 19:17:42.000000 maads-5.2.3/maads.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      122 2021-02-05 16:13:30.000000 maads-5.2.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-08-04 19:17:43.195812 maads-5.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      993 2023-08-04 18:34:36.000000 maads-5.2.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `maads-5.2.2/LICENSE.txt` & `maads-5.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `maads-5.2.2/maads/__init__.py` & `maads-5.2.3/maads/__init__.py`

 * *Files identical despite different names*

### Comparing `maads-5.2.2/maads/balancedata.py` & `maads-5.2.3/maads/balancedata.py`

 * *Files identical despite different names*

### Comparing `maads-5.2.2/maads/callmas.py` & `maads-5.2.3/maads/callmas.py`

 * *Files identical despite different names*

### Comparing `maads-5.2.2/setup.py` & `maads-5.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 	
 
 with open("requirements.txt","r") as f:
     required = f.read().splitlines()
     
 setuptools.setup(
     name='maads',
-    version='5.2.2',
+    version='5.2.3',
     description='Multi-Agent Accelerator for Data Science (MAADS)',
     license='MIT License',
     packages=['maads'],
     author='Sebastian Maurice',
     author_email='sebastian.maurice@otics.ca',
     keywords=['multi-agent, data science, optimization, prescriptive analytics, machine learning, automl,auto-ml,artificial intelligence', 'predictive analytics', 'advanced analytics'],
     long_description=long_description,
```

