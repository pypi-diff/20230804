# Comparing `tmp/bookseek-0.1.2.tar.gz` & `tmp/bookseek-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bookseek-0.1.2.tar", last modified: Fri Aug  4 13:14:44 2023, max compression
+gzip compressed data, was "bookseek-0.1.3.tar", last modified: Fri Aug  4 13:17:41 2023, max compression
```

## Comparing `bookseek-0.1.2.tar` & `bookseek-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 domunshaarvin  (1000) domunshaarvin  (1000)        0 2023-08-04 13:14:44.929648 bookseek-0.1.2/
--rw-rw-r--   0 domunshaarvin  (1000) domunshaarvin  (1000)      378 2023-08-04 13:14:44.929648 bookseek-0.1.2/PKG-INFO
-drwxrwxr-x   0 domunshaarvin  (1000) domunshaarvin  (1000)        0 2023-08-04 13:14:44.929648 bookseek-0.1.2/bookseek.egg-info/
--rw-rw-r--   0 domunshaarvin  (1000) domunshaarvin  (1000)      378 2023-08-04 13:14:44.000000 bookseek-0.1.2/bookseek.egg-info/PKG-INFO
--rw-rw-r--   0 domunshaarvin  (1000) domunshaarvin  (1000)      202 2023-08-04 13:14:44.000000 bookseek-0.1.2/bookseek.egg-info/SOURCES.txt
--rw-rw-r--   0 domunshaarvin  (1000) domunshaarvin  (1000)        1 2023-08-04 13:14:44.000000 bookseek-0.1.2/bookseek.egg-info/dependency_links.txt
--rw-rw-r--   0 domunshaarvin  (1000) domunshaarvin  (1000)       52 2023-08-04 13:14:44.000000 bookseek-0.1.2/bookseek.egg-info/entry_points.txt
--rw-rw-r--   0 domunshaarvin  (1000) domunshaarvin  (1000)       39 2023-08-04 13:14:44.000000 bookseek-0.1.2/bookseek.egg-info/requires.txt
--rw-rw-r--   0 domunshaarvin  (1000) domunshaarvin  (1000)        1 2023-08-04 13:14:44.000000 bookseek-0.1.2/bookseek.egg-info/top_level.txt
--rw-rw-r--   0 domunshaarvin  (1000) domunshaarvin  (1000)       38 2023-08-04 13:14:44.929648 bookseek-0.1.2/setup.cfg
--rw-rw-r--   0 domunshaarvin  (1000) domunshaarvin  (1000)      880 2023-08-04 13:13:47.000000 bookseek-0.1.2/setup.py
+drwxrwxr-x   0 domunshaarvin  (1000) domunshaarvin  (1000)        0 2023-08-04 13:17:41.550215 bookseek-0.1.3/
+-rw-rw-r--   0 domunshaarvin  (1000) domunshaarvin  (1000)      378 2023-08-04 13:17:41.550215 bookseek-0.1.3/PKG-INFO
+drwxrwxr-x   0 domunshaarvin  (1000) domunshaarvin  (1000)        0 2023-08-04 13:17:41.550215 bookseek-0.1.3/bookseek.egg-info/
+-rw-rw-r--   0 domunshaarvin  (1000) domunshaarvin  (1000)      378 2023-08-04 13:17:41.000000 bookseek-0.1.3/bookseek.egg-info/PKG-INFO
+-rw-rw-r--   0 domunshaarvin  (1000) domunshaarvin  (1000)      202 2023-08-04 13:17:41.000000 bookseek-0.1.3/bookseek.egg-info/SOURCES.txt
+-rw-rw-r--   0 domunshaarvin  (1000) domunshaarvin  (1000)        1 2023-08-04 13:17:41.000000 bookseek-0.1.3/bookseek.egg-info/dependency_links.txt
+-rw-rw-r--   0 domunshaarvin  (1000) domunshaarvin  (1000)       43 2023-08-04 13:17:41.000000 bookseek-0.1.3/bookseek.egg-info/entry_points.txt
+-rw-rw-r--   0 domunshaarvin  (1000) domunshaarvin  (1000)       39 2023-08-04 13:17:41.000000 bookseek-0.1.3/bookseek.egg-info/requires.txt
+-rw-rw-r--   0 domunshaarvin  (1000) domunshaarvin  (1000)        1 2023-08-04 13:17:41.000000 bookseek-0.1.3/bookseek.egg-info/top_level.txt
+-rw-rw-r--   0 domunshaarvin  (1000) domunshaarvin  (1000)       38 2023-08-04 13:17:41.550215 bookseek-0.1.3/setup.cfg
+-rw-rw-r--   0 domunshaarvin  (1000) domunshaarvin  (1000)      871 2023-08-04 13:17:10.000000 bookseek-0.1.3/setup.py
```

### Comparing `bookseek-0.1.2/setup.py` & `bookseek-0.1.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, 'readme.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='bookseek',
-    version='0.1.2',
+    version='0.1.3',
     description='A command-line tool to search for books on Goodreads.',
     author='Shaarvin',
     author_email='domunshaarvin@gmail.com',
     url='',
     packages=find_packages(),
     install_requires=[
         'requests==2.26.0',
         'beautifulsoup4==4.9.3'
     ],
     entry_points={
         'console_scripts': [
-            'bookseek=bookseek.bookseek:main',
+            'bookseek=bookseek:main',
         ],
     },
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: End Users/Desktop',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.8',
```

