# Comparing `tmp/yog-2.2.4.tar.gz` & `tmp/yog-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yog-2.2.4.tar", max compression
+gzip compressed data, was "yog-2.2.5.tar", max compression
```

## Comparing `yog-2.2.4.tar` & `yog-2.2.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    10174 2023-02-25 02:02:07.903436 yog-2.2.4/README.md
--rw-r--r--   0        0        0      541 2023-06-07 04:40:28.802373 yog-2.2.4/pyproject.toml
--rw-r--r--   0        0        0        0 2021-07-16 04:35:58.316463 yog-2.2.4/yog/__init__.py
--rw-r--r--   0        0        0      465 2023-02-22 20:50:59.508191 yog-2.2.4/yog/command.py
--rw-r--r--   0        0        0      636 2021-11-19 21:53:36.530661 yog-2.2.4/yog/git_utils.py
--rw-r--r--   0        0        0        0 2021-11-19 21:18:00.056940 yog-2.2.4/yog/host/__init__.py
--rw-r--r--   0        0        0    12156 2023-04-17 17:51:32.509096 yog-2.2.4/yog/host/docker_attrs.py
--rw-r--r--   0        0        0      499 2023-02-22 04:11:12.414451 yog-2.2.4/yog/host/main.py
--rw-r--r--   0        0        0     7573 2023-06-07 04:40:13.632348 yog-2.2.4/yog/host/manage.py
--rw-r--r--   0        0        0     9656 2023-06-07 04:40:13.632348 yog-2.2.4/yog/host/necronomicon.py
--rw-r--r--   0        0        0     1050 2023-05-30 01:28:33.283278 yog-2.2.4/yog/host/os_utils.py
--rw-r--r--   0        0        0    12672 2023-05-30 01:53:37.105511 yog-2.2.4/yog/host/pki.py
--rw-r--r--   0        0        0      752 2023-05-30 01:36:44.675981 yog-2.2.4/yog/host/pki_model.py
--rw-r--r--   0        0        0     1516 2023-06-07 04:40:13.632348 yog-2.2.4/yog/host/systemd.py
--rw-r--r--   0        0        0    11039 2023-02-01 20:50:54.524689 yog-2.2.4/yog/host/test_docker_attrs.py
--rw-r--r--   0        0        0      936 2023-02-22 04:11:12.414451 yog-2.2.4/yog/logging_utils.py
--rw-r--r--   0        0        0      389 2023-02-22 04:11:12.414451 yog-2.2.4/yog/model_utils.py
--rw-r--r--   0        0        0        0 2021-11-19 21:17:46.640293 yog-2.2.4/yog/repo/__init__.py
--rw-r--r--   0        0        0     4580 2022-12-28 04:50:30.284835 yog-2.2.4/yog/repo/main.py
--rw-r--r--   0        0        0      120 2021-07-25 01:26:53.898074 yog-2.2.4/yog/res/__init__.py
--rw-r--r--   0        0        0       80 2023-02-22 04:11:12.414451 yog-2.2.4/yog/res/cas.yml
--rw-r--r--   0        0        0      707 2023-02-01 20:50:54.524689 yog-2.2.4/yog/res/docker_test.yml
--rw-r--r--   0        0        0      434 2023-02-01 20:50:54.524689 yog-2.2.4/yog/res/sample_necronomicon.yml
--rw-r--r--   0        0        0      426 2021-07-30 04:19:50.436971 yog-2.2.4/yog/res/sample_needs_tunnel_back.yml
--rw-r--r--   0        0        0      195 2023-05-30 01:31:38.821403 yog-2.2.4/yog/res/sample_pki_necronomicon.yml
--rw-r--r--   0        0        0       50 2021-07-25 01:26:25.424796 yog-2.2.4/yog/res/sample_site_necronomicon.yml
--rw-r--r--   0        0        0    11032 2023-05-30 01:53:37.125512 yog-2.2.4/yog/ssh_utils.py
--rw-r--r--   0        0        0    10804 1970-01-01 00:00:00.000000 yog-2.2.4/PKG-INFO
+-rw-r--r--   0        0        0    10174 2023-02-25 02:02:07.000000 yog-2.2.5/README.md
+-rw-r--r--   0        0        0      541 2023-08-04 00:45:01.073337 yog-2.2.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2021-07-16 04:35:58.000000 yog-2.2.5/yog/__init__.py
+-rw-r--r--   0        0        0      465 2023-02-22 20:50:59.000000 yog-2.2.5/yog/command.py
+-rw-r--r--   0        0        0      636 2021-11-19 21:53:36.000000 yog-2.2.5/yog/git_utils.py
+-rw-r--r--   0        0        0        0 2021-11-19 21:18:00.000000 yog-2.2.5/yog/host/__init__.py
+-rw-r--r--   0        0        0    12156 2023-04-17 17:51:32.000000 yog-2.2.5/yog/host/docker_attrs.py
+-rw-r--r--   0        0        0      499 2023-02-22 04:11:12.000000 yog-2.2.5/yog/host/main.py
+-rw-r--r--   0        0        0     7573 2023-06-07 04:40:13.000000 yog-2.2.5/yog/host/manage.py
+-rw-r--r--   0        0        0     9656 2023-06-07 04:40:13.000000 yog-2.2.5/yog/host/necronomicon.py
+-rw-r--r--   0        0        0     1050 2023-05-30 01:28:33.000000 yog-2.2.5/yog/host/os_utils.py
+-rw-r--r--   0        0        0    12672 2023-05-30 01:53:37.000000 yog-2.2.5/yog/host/pki.py
+-rw-r--r--   0        0        0      752 2023-05-30 01:36:44.000000 yog-2.2.5/yog/host/pki_model.py
+-rw-r--r--   0        0        0     1516 2023-06-07 04:40:13.000000 yog-2.2.5/yog/host/systemd.py
+-rw-r--r--   0        0        0    11039 2023-02-01 20:50:54.000000 yog-2.2.5/yog/host/test_docker_attrs.py
+-rw-r--r--   0        0        0      936 2023-02-22 04:11:12.000000 yog-2.2.5/yog/logging_utils.py
+-rw-r--r--   0        0        0      389 2023-02-22 04:11:12.000000 yog-2.2.5/yog/model_utils.py
+-rw-r--r--   0        0        0        0 2021-11-19 21:17:46.000000 yog-2.2.5/yog/repo/__init__.py
+-rw-r--r--   0        0        0     4580 2022-12-28 04:50:30.000000 yog-2.2.5/yog/repo/main.py
+-rw-r--r--   0        0        0      120 2021-07-25 01:26:53.000000 yog-2.2.5/yog/res/__init__.py
+-rw-r--r--   0        0        0       80 2023-02-22 04:11:12.000000 yog-2.2.5/yog/res/cas.yml
+-rw-r--r--   0        0        0      707 2023-02-01 20:50:54.000000 yog-2.2.5/yog/res/docker_test.yml
+-rw-r--r--   0        0        0      434 2023-02-01 20:50:54.000000 yog-2.2.5/yog/res/sample_necronomicon.yml
+-rw-r--r--   0        0        0      426 2021-07-30 04:19:50.000000 yog-2.2.5/yog/res/sample_needs_tunnel_back.yml
+-rw-r--r--   0        0        0      195 2023-05-30 01:31:38.000000 yog-2.2.5/yog/res/sample_pki_necronomicon.yml
+-rw-r--r--   0        0        0       50 2021-07-25 01:26:25.000000 yog-2.2.5/yog/res/sample_site_necronomicon.yml
+-rw-r--r--   0        0        0    11032 2023-05-30 01:53:37.000000 yog-2.2.5/yog/ssh_utils.py
+-rw-r--r--   0        0        0    10804 1970-01-01 00:00:00.000000 yog-2.2.5/PKG-INFO
```

### Comparing `yog-2.2.4/README.md` & `yog-2.2.5/README.md`

 * *Files identical despite different names*

### Comparing `yog-2.2.4/pyproject.toml` & `yog-2.2.5/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yog"
-version = "2.2.4"
+version = "2.2.5"
 description = "The Gate and Key"
 authors = ["Josh Hertlein <jmhertlein@gmail.com>"]
 license = "AGPLv3"
 readme = "README.md"
 
 [tool.poetry.scripts]
 yog = "yog.host.main:main"
@@ -12,15 +12,15 @@
 yog-pki = "yog.command:ca_main"
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
 paramiko = "^2.8.0"
 PyYAML = "^6.0"
-docker = "^5.0.3"
+docker = "^6.1.3"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2.1"
 twine = "^3.6.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `yog-2.2.4/yog/git_utils.py` & `yog-2.2.5/yog/git_utils.py`

 * *Files identical despite different names*

### Comparing `yog-2.2.4/yog/host/docker_attrs.py` & `yog-2.2.5/yog/host/docker_attrs.py`

 * *Files identical despite different names*

### Comparing `yog-2.2.4/yog/host/manage.py` & `yog-2.2.5/yog/host/manage.py`

 * *Files identical despite different names*

### Comparing `yog-2.2.4/yog/host/necronomicon.py` & `yog-2.2.5/yog/host/necronomicon.py`

 * *Files identical despite different names*

### Comparing `yog-2.2.4/yog/host/os_utils.py` & `yog-2.2.5/yog/host/os_utils.py`

 * *Files identical despite different names*

### Comparing `yog-2.2.4/yog/host/pki.py` & `yog-2.2.5/yog/host/pki.py`

 * *Files identical despite different names*

### Comparing `yog-2.2.4/yog/host/pki_model.py` & `yog-2.2.5/yog/host/pki_model.py`

 * *Files identical despite different names*

### Comparing `yog-2.2.4/yog/host/systemd.py` & `yog-2.2.5/yog/host/systemd.py`

 * *Files identical despite different names*

### Comparing `yog-2.2.4/yog/host/test_docker_attrs.py` & `yog-2.2.5/yog/host/test_docker_attrs.py`

 * *Files identical despite different names*

### Comparing `yog-2.2.4/yog/logging_utils.py` & `yog-2.2.5/yog/logging_utils.py`

 * *Files identical despite different names*

### Comparing `yog-2.2.4/yog/repo/main.py` & `yog-2.2.5/yog/repo/main.py`

 * *Files identical despite different names*

### Comparing `yog-2.2.4/yog/res/docker_test.yml` & `yog-2.2.5/yog/res/docker_test.yml`

 * *Files identical despite different names*

### Comparing `yog-2.2.4/yog/ssh_utils.py` & `yog-2.2.5/yog/ssh_utils.py`

 * *Files identical despite different names*

### Comparing `yog-2.2.4/PKG-INFO` & `yog-2.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: yog
-Version: 2.2.4
+Version: 2.2.5
 Summary: The Gate and Key
 License: AGPLv3
 Author: Josh Hertlein
 Author-email: jmhertlein@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyYAML (>=6.0,<7.0)
-Requires-Dist: docker (>=5.0.3,<6.0.0)
+Requires-Dist: docker (>=6.1.3,<7.0.0)
 Requires-Dist: paramiko (>=2.8.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Overview
 
 An opinionated docker-and-ssh-centric declarative system management tool.
```

