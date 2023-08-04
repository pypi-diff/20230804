# Comparing `tmp/stdlb-0.0.1.tar.gz` & `tmp/stdlb-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stdlb-0.0.1.tar", last modified: Thu Aug  3 15:02:14 2023, max compression
+gzip compressed data, was "stdlb-0.0.2.tar", last modified: Thu Aug  3 15:45:38 2023, max compression
```

## Comparing `stdlb-0.0.1.tar` & `stdlb-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:02:14.237052 stdlb-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-08-03 15:02:14.237052 stdlb-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-08-03 15:01:57.000000 stdlb-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 15:02:14.237052 stdlb-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-08-03 15:01:57.000000 stdlb-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:02:14.237052 stdlb-0.0.1/stdlb/
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-08-03 15:01:57.000000 stdlb-0.0.1/stdlb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-08-03 15:01:57.000000 stdlb-0.0.1/stdlb/cached_property.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:02:14.237052 stdlb-0.0.1/stdlb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-08-03 15:02:14.000000 stdlb-0.0.1/stdlb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-08-03 15:02:14.000000 stdlb-0.0.1/stdlb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 15:02:14.000000 stdlb-0.0.1/stdlb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-03 15:02:14.000000 stdlb-0.0.1/stdlb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:45:38.771875 stdlb-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-08-03 15:45:38.771875 stdlb-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-08-03 15:45:26.000000 stdlb-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 15:45:38.771875 stdlb-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-08-03 15:45:26.000000 stdlb-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:45:38.771875 stdlb-0.0.2/stdlb/
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-08-03 15:45:26.000000 stdlb-0.0.2/stdlb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-08-03 15:45:26.000000 stdlb-0.0.2/stdlb/cached_property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:45:38.771875 stdlb-0.0.2/stdlb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-08-03 15:45:38.000000 stdlb-0.0.2/stdlb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-08-03 15:45:38.000000 stdlb-0.0.2/stdlb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 15:45:38.000000 stdlb-0.0.2/stdlb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-03 15:45:38.000000 stdlb-0.0.2/stdlb.egg-info/top_level.txt
```

### Comparing `stdlb-0.0.1/PKG-INFO` & `stdlb-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stdlb
-Version: 0.0.1
+Version: 0.0.2
 Summary: Wildcard-import the Python standard library
 Home-page: UNKNOWN
 Author: Ryan Williams <ryan@runsascoded.com>
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
@@ -33,28 +33,34 @@
 %%time
 from stdlb import *
 # CPU times: user 914 µs, sys: 397 µs, total: 1.31 ms
 # Wall time: 1.6 ms
 ```
 
 ### Collisions / Aliases
-In a few cases, a top-level standard library module also contains a member with the same name (e.g. `datetime`, `shlex`). `stdlb` makes an effort to ensure the module "wins" in this case:
+In a few cases, a top-level standard library module also contains a member with the same name (e.g. `datetime`, `shlex`, `time`). `stdlb` makes an effort to ensure the module "wins" in this case:
 
 ```python
 from stdlb import *
 
-datetime
-# <module 'datetime' from '$PYTHON_HOME/lib/python3.9/datetime.py'>
-shlex
-# <module 'shlex' from '$PYTHON_HOME/lib/python3.9/shlex.py'>
+datetime  # <module 'datetime' from '$PYTHON_HOME/lib/python3.9/datetime.py'>
+shlex     # <module 'shlex' from '$PYTHON_HOME/lib/python3.9/shlex.py'>
+time      # <module 'time' (built-in)>
 ```
 
-For convenience, `datetime.datetime` is also exposed as `dt`:
+A few names are disambiguated with the most sensible-seeming defaults:
 ```python
-dt.now()
-# datetime.datetime(2023, 8, 3, 10, 9, 43, 981458)
+path  # resolves to os.path, not sys.path
+join  # os.path.join, not shlex.join
+```
+
+For convenience, `datetime.datetime` is also exposed as `dt`, and a few of its members are exported directly:
+```python
+dt.now()       # datetime.datetime(2023, 8, 3, 10, 9, 43, 981458)
+fromtimestamp  # datetime.datetime.fromtimestamp
+fromisoformat  # datetime.datetime.fromisoformat
 ```
 
 ### Custom `cached_property`
 One additional bit of functionality is [this custom `cached_property` decorator](stdlb/cached_property.py), which omits an unnecessary/unserializable lock found in `functools.cached_property`. [cpython#87634](https://github.com/python/cpython/issues/87634) has more info, seems like [a fix is coming in Python 3.12](https://github.com/python/cpython/issues/87634#issuecomment-1467140709).
```

### Comparing `stdlb-0.0.1/README.md` & `stdlb-0.0.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -23,26 +23,32 @@
 %%time
 from stdlb import *
 # CPU times: user 914 µs, sys: 397 µs, total: 1.31 ms
 # Wall time: 1.6 ms
 ```
 
 ### Collisions / Aliases
-In a few cases, a top-level standard library module also contains a member with the same name (e.g. `datetime`, `shlex`). `stdlb` makes an effort to ensure the module "wins" in this case:
+In a few cases, a top-level standard library module also contains a member with the same name (e.g. `datetime`, `shlex`, `time`). `stdlb` makes an effort to ensure the module "wins" in this case:
 
 ```python
 from stdlb import *
 
-datetime
-# <module 'datetime' from '$PYTHON_HOME/lib/python3.9/datetime.py'>
-shlex
-# <module 'shlex' from '$PYTHON_HOME/lib/python3.9/shlex.py'>
+datetime  # <module 'datetime' from '$PYTHON_HOME/lib/python3.9/datetime.py'>
+shlex     # <module 'shlex' from '$PYTHON_HOME/lib/python3.9/shlex.py'>
+time      # <module 'time' (built-in)>
 ```
 
-For convenience, `datetime.datetime` is also exposed as `dt`:
+A few names are disambiguated with the most sensible-seeming defaults:
 ```python
-dt.now()
-# datetime.datetime(2023, 8, 3, 10, 9, 43, 981458)
+path  # resolves to os.path, not sys.path
+join  # os.path.join, not shlex.join
+```
+
+For convenience, `datetime.datetime` is also exposed as `dt`, and a few of its members are exported directly:
+```python
+dt.now()       # datetime.datetime(2023, 8, 3, 10, 9, 43, 981458)
+fromtimestamp  # datetime.datetime.fromtimestamp
+fromisoformat  # datetime.datetime.fromisoformat
 ```
 
 ### Custom `cached_property`
 One additional bit of functionality is [this custom `cached_property` decorator](stdlb/cached_property.py), which omits an unnecessary/unserializable lock found in `functools.cached_property`. [cpython#87634](https://github.com/python/cpython/issues/87634) has more info, seems like [a fix is coming in Python 3.12](https://github.com/python/cpython/issues/87634#issuecomment-1467140709).
```

### Comparing `stdlb-0.0.1/stdlb/__init__.py` & `stdlb-0.0.2/stdlb/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -48,20 +48,22 @@
 from re import *
 
 from shlex import *
 import shlex
 
 import shutil
 from shutil import *
+join = os.path.join  # seems like a better default than shlex.join
 
 import subprocess
 from subprocess import *
 
 import sys
 from sys import *
+path = os.path
 
 import tempfile
 from tempfile import *
 
 from time import *
 import time
```

### Comparing `stdlb-0.0.1/stdlb/cached_property.py` & `stdlb-0.0.2/stdlb/cached_property.py`

 * *Files identical despite different names*

### Comparing `stdlb-0.0.1/stdlb.egg-info/PKG-INFO` & `stdlb-0.0.2/stdlb.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stdlb
-Version: 0.0.1
+Version: 0.0.2
 Summary: Wildcard-import the Python standard library
 Home-page: UNKNOWN
 Author: Ryan Williams <ryan@runsascoded.com>
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
@@ -33,28 +33,34 @@
 %%time
 from stdlb import *
 # CPU times: user 914 µs, sys: 397 µs, total: 1.31 ms
 # Wall time: 1.6 ms
 ```
 
 ### Collisions / Aliases
-In a few cases, a top-level standard library module also contains a member with the same name (e.g. `datetime`, `shlex`). `stdlb` makes an effort to ensure the module "wins" in this case:
+In a few cases, a top-level standard library module also contains a member with the same name (e.g. `datetime`, `shlex`, `time`). `stdlb` makes an effort to ensure the module "wins" in this case:
 
 ```python
 from stdlb import *
 
-datetime
-# <module 'datetime' from '$PYTHON_HOME/lib/python3.9/datetime.py'>
-shlex
-# <module 'shlex' from '$PYTHON_HOME/lib/python3.9/shlex.py'>
+datetime  # <module 'datetime' from '$PYTHON_HOME/lib/python3.9/datetime.py'>
+shlex     # <module 'shlex' from '$PYTHON_HOME/lib/python3.9/shlex.py'>
+time      # <module 'time' (built-in)>
 ```
 
-For convenience, `datetime.datetime` is also exposed as `dt`:
+A few names are disambiguated with the most sensible-seeming defaults:
 ```python
-dt.now()
-# datetime.datetime(2023, 8, 3, 10, 9, 43, 981458)
+path  # resolves to os.path, not sys.path
+join  # os.path.join, not shlex.join
+```
+
+For convenience, `datetime.datetime` is also exposed as `dt`, and a few of its members are exported directly:
+```python
+dt.now()       # datetime.datetime(2023, 8, 3, 10, 9, 43, 981458)
+fromtimestamp  # datetime.datetime.fromtimestamp
+fromisoformat  # datetime.datetime.fromisoformat
 ```
 
 ### Custom `cached_property`
 One additional bit of functionality is [this custom `cached_property` decorator](stdlb/cached_property.py), which omits an unnecessary/unserializable lock found in `functools.cached_property`. [cpython#87634](https://github.com/python/cpython/issues/87634) has more info, seems like [a fix is coming in Python 3.12](https://github.com/python/cpython/issues/87634#issuecomment-1467140709).
```

