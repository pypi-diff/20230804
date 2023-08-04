# Comparing `tmp/salure_helpers_task_scheduler-1.1.4.tar.gz` & `tmp/salure_helpers_task_scheduler-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/salure_helpers_task_scheduler-1.1.4.tar", last modified: Fri Jul 28 12:21:58 2023, max compression
+gzip compressed data, was "dist/salure_helpers_task_scheduler-1.1.5.tar", last modified: Fri Aug  4 07:39:32 2023, max compression
```

## Comparing `salure_helpers_task_scheduler-1.1.4.tar` & `salure_helpers_task_scheduler-1.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 12:21:58.000000 salure_helpers_task_scheduler-1.1.4/
--rw-r--r--   0 root         (0) root         (0)      269 2023-07-28 12:21:58.000000 salure_helpers_task_scheduler-1.1.4/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 12:21:58.000000 salure_helpers_task_scheduler-1.1.4/salure_helpers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 12:21:58.000000 salure_helpers_task_scheduler-1.1.4/salure_helpers/task_scheduler/
--rw-rw-rw-   0 root         (0) root         (0)       70 2023-07-28 12:21:45.000000 salure_helpers_task_scheduler-1.1.4/salure_helpers/task_scheduler/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    39919 2023-07-28 12:21:45.000000 salure_helpers_task_scheduler-1.1.4/salure_helpers/task_scheduler/task_scheduler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 12:21:58.000000 salure_helpers_task_scheduler-1.1.4/salure_helpers_task_scheduler.egg-info/
--rw-r--r--   0 root         (0) root         (0)      269 2023-07-28 12:21:58.000000 salure_helpers_task_scheduler-1.1.4/salure_helpers_task_scheduler.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      414 2023-07-28 12:21:58.000000 salure_helpers_task_scheduler-1.1.4/salure_helpers_task_scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 12:21:58.000000 salure_helpers_task_scheduler-1.1.4/salure_helpers_task_scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 12:21:58.000000 salure_helpers_task_scheduler-1.1.4/salure_helpers_task_scheduler.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      177 2023-07-28 12:21:58.000000 salure_helpers_task_scheduler-1.1.4/salure_helpers_task_scheduler.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-07-28 12:21:58.000000 salure_helpers_task_scheduler-1.1.4/salure_helpers_task_scheduler.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-28 12:21:58.000000 salure_helpers_task_scheduler-1.1.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      651 2023-07-28 12:21:45.000000 salure_helpers_task_scheduler-1.1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 07:39:32.000000 salure_helpers_task_scheduler-1.1.5/
+-rw-r--r--   0 root         (0) root         (0)      269 2023-08-04 07:39:32.000000 salure_helpers_task_scheduler-1.1.5/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 07:39:32.000000 salure_helpers_task_scheduler-1.1.5/salure_helpers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 07:39:32.000000 salure_helpers_task_scheduler-1.1.5/salure_helpers/task_scheduler/
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-08-04 07:39:18.000000 salure_helpers_task_scheduler-1.1.5/salure_helpers/task_scheduler/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    39927 2023-08-04 07:39:18.000000 salure_helpers_task_scheduler-1.1.5/salure_helpers/task_scheduler/task_scheduler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 07:39:32.000000 salure_helpers_task_scheduler-1.1.5/salure_helpers_task_scheduler.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      269 2023-08-04 07:39:31.000000 salure_helpers_task_scheduler-1.1.5/salure_helpers_task_scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      414 2023-08-04 07:39:31.000000 salure_helpers_task_scheduler-1.1.5/salure_helpers_task_scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 07:39:31.000000 salure_helpers_task_scheduler-1.1.5/salure_helpers_task_scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 07:39:31.000000 salure_helpers_task_scheduler-1.1.5/salure_helpers_task_scheduler.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      177 2023-08-04 07:39:31.000000 salure_helpers_task_scheduler-1.1.5/salure_helpers_task_scheduler.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-08-04 07:39:31.000000 salure_helpers_task_scheduler-1.1.5/salure_helpers_task_scheduler.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-04 07:39:32.000000 salure_helpers_task_scheduler-1.1.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      651 2023-08-04 07:39:18.000000 salure_helpers_task_scheduler-1.1.5/setup.py
```

### Comparing `salure_helpers_task_scheduler-1.1.4/salure_helpers/task_scheduler/task_scheduler.py` & `salure_helpers_task_scheduler-1.1.5/salure_helpers/task_scheduler/task_scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -243,15 +243,15 @@
             if isinstance(data, dict):
                 data = pd.DataFrame([data])
 
             payload = {
                 'reload_id': self.run_id,
                 'task_id': self.task_id,
                 'customer_id': os.getenv('SALURECONNECT_CUSTOMER_NAME').lower().replace(' ', '_'),
-                'started_at': self.started_at.isoformat(),
+                'started_at': datetime.datetime.now().isoformat(),
                 'records': len(data),
                 'columns': len(data.columns),
                 'cells': len(data) * len(data.columns),
                 'data': data.to_csv(sep='|', index=False),
                 'loglevel': loglevel,
                 'message': message
             }
```

### Comparing `salure_helpers_task_scheduler-1.1.4/setup.py` & `salure_helpers_task_scheduler-1.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name='salure_helpers_task_scheduler',
-    version='1.1.4',
+    version='1.1.5',
     description='Task Scheduler from Salure',
     long_description='Task Schedule from Salure',
     author='D&A Salure',
     author_email='support@salureconnnect.com',
     packages=["salure_helpers.task_scheduler"],
     license='Salure License',
     install_requires=[
```

