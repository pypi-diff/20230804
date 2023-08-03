# Comparing `tmp/dagster_cloud_examples-1.4.3.tar.gz` & `tmp/dagster_cloud_examples-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster_cloud_examples-1.4.3.tar", last modified: Mon Jul 31 23:08:52 2023, max compression
+gzip compressed data, was "dagster_cloud_examples-1.4.4.tar", last modified: Thu Aug  3 22:02:11 2023, max compression
```

## Comparing `dagster_cloud_examples-1.4.3.tar` & `dagster_cloud_examples-1.4.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:08:52.242392 dagster_cloud_examples-1.4.3/
--rw-r--r--   0 root         (0) root         (0)      319 2023-07-31 23:08:52.242392 dagster_cloud_examples-1.4.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-07-31 22:58:37.000000 dagster_cloud_examples-1.4.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:08:52.238392 dagster_cloud_examples-1.4.3/dagster_cloud_examples/
--rw-r--r--   0 root         (0) root         (0)       60 2023-07-31 22:58:37.000000 dagster_cloud_examples-1.4.3/dagster_cloud_examples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:08:52.238392 dagster_cloud_examples-1.4.3/dagster_cloud_examples/cereals/
--rw-r--r--   0 root         (0) root         (0)       63 2023-07-31 22:58:37.000000 dagster_cloud_examples-1.4.3/dagster_cloud_examples/cereals/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:08:52.238392 dagster_cloud_examples-1.4.3/dagster_cloud_examples/cereals/jobs/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 22:58:37.000000 dagster_cloud_examples-1.4.3/dagster_cloud_examples/cereals/jobs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:08:52.238392 dagster_cloud_examples-1.4.3/dagster_cloud_examples/cereals/jobs/compute_cereal_properties/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 22:58:37.000000 dagster_cloud_examples-1.4.3/dagster_cloud_examples/cereals/jobs/compute_cereal_properties/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:08:52.242392 dagster_cloud_examples-1.4.3/dagster_cloud_examples/cereals/jobs/compute_cereal_properties/ops/
--rw-r--r--   0 root         (0) root         (0)      770 2023-07-31 22:58:37.000000 dagster_cloud_examples-1.4.3/dagster_cloud_examples/cereals/jobs/compute_cereal_properties/ops/__init__.py
--rw-r--r--   0 root         (0) root         (0)      374 2023-07-31 22:58:37.000000 dagster_cloud_examples-1.4.3/dagster_cloud_examples/cereals/jobs/compute_cereal_properties/process_cereals.py
--rw-r--r--   0 root         (0) root         (0)      306 2023-07-31 22:58:37.000000 dagster_cloud_examples-1.4.3/dagster_cloud_examples/cereals/repository.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:08:52.242392 dagster_cloud_examples-1.4.3/dagster_cloud_examples/cereals/schedules/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 22:58:37.000000 dagster_cloud_examples-1.4.3/dagster_cloud_examples/cereals/schedules/__init__.py
--rw-r--r--   0 root         (0) root         (0)      367 2023-07-31 22:58:37.000000 dagster_cloud_examples-1.4.3/dagster_cloud_examples/cereals/schedules/daily_process_cereals.py
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-31 22:58:37.000000 dagster_cloud_examples-1.4.3/dagster_cloud_examples/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 23:08:52.238392 dagster_cloud_examples-1.4.3/dagster_cloud_examples.egg-info/
--rw-r--r--   0 root         (0) root         (0)      319 2023-07-31 23:08:52.000000 dagster_cloud_examples-1.4.3/dagster_cloud_examples.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      804 2023-07-31 23:08:52.000000 dagster_cloud_examples-1.4.3/dagster_cloud_examples.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 23:08:52.000000 dagster_cloud_examples-1.4.3/dagster_cloud_examples.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-07-31 23:08:52.000000 dagster_cloud_examples-1.4.3/dagster_cloud_examples.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-07-31 23:08:52.000000 dagster_cloud_examples-1.4.3/dagster_cloud_examples.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-31 23:08:52.242392 dagster_cloud_examples-1.4.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      956 2023-07-31 22:58:37.000000 dagster_cloud_examples-1.4.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 22:02:11.964361 dagster_cloud_examples-1.4.4/
+-rw-r--r--   0 root         (0) root         (0)      319 2023-08-03 22:02:11.964361 dagster_cloud_examples-1.4.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-08-03 21:50:30.000000 dagster_cloud_examples-1.4.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 22:02:11.960361 dagster_cloud_examples-1.4.4/dagster_cloud_examples/
+-rw-r--r--   0 root         (0) root         (0)       60 2023-08-03 21:50:30.000000 dagster_cloud_examples-1.4.4/dagster_cloud_examples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 22:02:11.960361 dagster_cloud_examples-1.4.4/dagster_cloud_examples/cereals/
+-rw-r--r--   0 root         (0) root         (0)       63 2023-08-03 21:50:30.000000 dagster_cloud_examples-1.4.4/dagster_cloud_examples/cereals/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 22:02:11.960361 dagster_cloud_examples-1.4.4/dagster_cloud_examples/cereals/jobs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 21:50:30.000000 dagster_cloud_examples-1.4.4/dagster_cloud_examples/cereals/jobs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 22:02:11.960361 dagster_cloud_examples-1.4.4/dagster_cloud_examples/cereals/jobs/compute_cereal_properties/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 21:50:30.000000 dagster_cloud_examples-1.4.4/dagster_cloud_examples/cereals/jobs/compute_cereal_properties/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 22:02:11.960361 dagster_cloud_examples-1.4.4/dagster_cloud_examples/cereals/jobs/compute_cereal_properties/ops/
+-rw-r--r--   0 root         (0) root         (0)      770 2023-08-03 21:50:30.000000 dagster_cloud_examples-1.4.4/dagster_cloud_examples/cereals/jobs/compute_cereal_properties/ops/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      374 2023-08-03 21:50:30.000000 dagster_cloud_examples-1.4.4/dagster_cloud_examples/cereals/jobs/compute_cereal_properties/process_cereals.py
+-rw-r--r--   0 root         (0) root         (0)      306 2023-08-03 21:50:30.000000 dagster_cloud_examples-1.4.4/dagster_cloud_examples/cereals/repository.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 22:02:11.964361 dagster_cloud_examples-1.4.4/dagster_cloud_examples/cereals/schedules/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 21:50:30.000000 dagster_cloud_examples-1.4.4/dagster_cloud_examples/cereals/schedules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      367 2023-08-03 21:50:30.000000 dagster_cloud_examples-1.4.4/dagster_cloud_examples/cereals/schedules/daily_process_cereals.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-08-03 21:50:30.000000 dagster_cloud_examples-1.4.4/dagster_cloud_examples/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 22:02:11.960361 dagster_cloud_examples-1.4.4/dagster_cloud_examples.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      319 2023-08-03 22:02:11.000000 dagster_cloud_examples-1.4.4/dagster_cloud_examples.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      804 2023-08-03 22:02:11.000000 dagster_cloud_examples-1.4.4/dagster_cloud_examples.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 22:02:11.000000 dagster_cloud_examples-1.4.4/dagster_cloud_examples.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-08-03 22:02:11.000000 dagster_cloud_examples-1.4.4/dagster_cloud_examples.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-08-03 22:02:11.000000 dagster_cloud_examples-1.4.4/dagster_cloud_examples.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-03 22:02:11.964361 dagster_cloud_examples-1.4.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      956 2023-08-03 21:50:30.000000 dagster_cloud_examples-1.4.4/setup.py
```

### Comparing `dagster_cloud_examples-1.4.3/README.md` & `dagster_cloud_examples-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `dagster_cloud_examples-1.4.3/dagster_cloud_examples/cereals/jobs/compute_cereal_properties/ops/__init__.py` & `dagster_cloud_examples-1.4.4/dagster_cloud_examples/cereals/jobs/compute_cereal_properties/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_examples-1.4.3/dagster_cloud_examples.egg-info/SOURCES.txt` & `dagster_cloud_examples-1.4.4/dagster_cloud_examples.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster_cloud_examples-1.4.3/setup.py` & `dagster_cloud_examples-1.4.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 ver = get_version()
 # dont pin dev installs to avoid pip dep resolver issues
 pin = "" if ver == "1!0+dev" else f"=={ver}"
 setup(
     name="dagster_cloud_examples",
     version=ver,
     packages=find_packages(exclude=["dagster_cloud_examples_tests*"]),
-    install_requires=["dagster_cloud==1.4.3"],
+    install_requires=["dagster_cloud==1.4.4"],
     extras_require={"tests": ["mypy", "pylint", "pytest"]},
     author="Elementl",
     author_email="hello@elementl.com",
     license="Apache-2.0",
     classifiers=[
         "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: Apache Software License",
```

