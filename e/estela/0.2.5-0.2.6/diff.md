# Comparing `tmp/estela-0.2.5.tar.gz` & `tmp/estela-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "estela-0.2.5.tar", last modified: Wed Jul 19 17:41:26 2023, max compression
+gzip compressed data, was "estela-0.2.6.tar", last modified: Fri Aug  4 20:31:20 2023, max compression
```

## Comparing `estela-0.2.5.tar` & `estela-0.2.6.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 17:41:26.203639 estela-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-19 17:41:26.203639 estela-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-07-19 17:41:20.000000 estela-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 17:41:26.199639 estela-0.2.5/estela.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-19 17:41:26.000000 estela-0.2.5/estela.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-19 17:41:26.000000 estela-0.2.5/estela.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 17:41:26.000000 estela-0.2.5/estela.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-19 17:41:26.000000 estela-0.2.5/estela.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 17:41:26.000000 estela-0.2.5/estela.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-19 17:41:26.000000 estela-0.2.5/estela.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 17:41:26.199639 estela-0.2.5/estela_cli/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-19 17:41:20.000000 estela-0.2.5/estela_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-19 17:41:20.000000 estela-0.2.5/estela_cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-07-19 17:41:20.000000 estela-0.2.5/estela_cli/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 17:41:26.199639 estela-0.2.5/estela_cli/create/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-19 17:41:20.000000 estela-0.2.5/estela_cli/create/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-19 17:41:20.000000 estela-0.2.5/estela_cli/create/cronjob.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-19 17:41:20.000000 estela-0.2.5/estela_cli/create/job.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-19 17:41:20.000000 estela-0.2.5/estela_cli/create/project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 17:41:26.199639 estela-0.2.5/estela_cli/data/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-19 17:41:20.000000 estela-0.2.5/estela_cli/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-07-19 17:41:20.000000 estela-0.2.5/estela_cli/data/job.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 17:41:26.199639 estela-0.2.5/estela_cli/delete/
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-19 17:41:20.000000 estela-0.2.5/estela_cli/delete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-19 17:41:20.000000 estela-0.2.5/estela_cli/delete/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-07-19 17:41:20.000000 estela-0.2.5/estela_cli/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-07-19 17:41:20.000000 estela-0.2.5/estela_cli/estela_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-07-19 17:41:20.000000 estela-0.2.5/estela_cli/init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 17:41:26.203639 estela-0.2.5/estela_cli/list/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-19 17:41:20.000000 estela-0.2.5/estela_cli/list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-07-19 17:41:20.000000 estela-0.2.5/estela_cli/list/cronjob.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-07-19 17:41:20.000000 estela-0.2.5/estela_cli/list/job.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-19 17:41:20.000000 estela-0.2.5/estela_cli/list/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-19 17:41:20.000000 estela-0.2.5/estela_cli/list/spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-07-19 17:41:20.000000 estela-0.2.5/estela_cli/login.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-19 17:41:20.000000 estela-0.2.5/estela_cli/logout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 17:41:26.203639 estela-0.2.5/estela_cli/stop/
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-19 17:41:20.000000 estela-0.2.5/estela_cli/stop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-07-19 17:41:20.000000 estela-0.2.5/estela_cli/stop/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-19 17:41:20.000000 estela-0.2.5/estela_cli/templates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 17:41:26.203639 estela-0.2.5/estela_cli/update/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-19 17:41:20.000000 estela-0.2.5/estela_cli/update/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-19 17:41:20.000000 estela-0.2.5/estela_cli/update/cronjob.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-07-19 17:41:20.000000 estela-0.2.5/estela_cli/update/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-07-19 17:41:20.000000 estela-0.2.5/estela_cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 17:41:26.203639 estela-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-19 17:41:20.000000 estela-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 20:31:20.947227 estela-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-08-04 20:31:20.947227 estela-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-08-04 20:31:14.000000 estela-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 20:31:20.947227 estela-0.2.6/estela.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-08-04 20:31:20.000000 estela-0.2.6/estela.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-08-04 20:31:20.000000 estela-0.2.6/estela.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 20:31:20.000000 estela-0.2.6/estela.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 20:31:20.000000 estela-0.2.6/estela.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 20:31:20.000000 estela-0.2.6/estela.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-04 20:31:20.000000 estela-0.2.6/estela.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 20:31:20.947227 estela-0.2.6/estela_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-04 20:31:14.000000 estela-0.2.6/estela_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-08-04 20:31:14.000000 estela-0.2.6/estela_cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-08-04 20:31:14.000000 estela-0.2.6/estela_cli/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 20:31:20.947227 estela-0.2.6/estela_cli/create/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-08-04 20:31:14.000000 estela-0.2.6/estela_cli/create/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-08-04 20:31:14.000000 estela-0.2.6/estela_cli/create/cronjob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-08-04 20:31:14.000000 estela-0.2.6/estela_cli/create/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-08-04 20:31:14.000000 estela-0.2.6/estela_cli/create/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 20:31:20.947227 estela-0.2.6/estela_cli/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-08-04 20:31:14.000000 estela-0.2.6/estela_cli/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-08-04 20:31:14.000000 estela-0.2.6/estela_cli/data/job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 20:31:20.947227 estela-0.2.6/estela_cli/delete/
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-08-04 20:31:14.000000 estela-0.2.6/estela_cli/delete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-08-04 20:31:14.000000 estela-0.2.6/estela_cli/delete/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-08-04 20:31:14.000000 estela-0.2.6/estela_cli/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-08-04 20:31:14.000000 estela-0.2.6/estela_cli/estela_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-08-04 20:31:14.000000 estela-0.2.6/estela_cli/init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 20:31:20.947227 estela-0.2.6/estela_cli/list/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-08-04 20:31:14.000000 estela-0.2.6/estela_cli/list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-08-04 20:31:14.000000 estela-0.2.6/estela_cli/list/cronjob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-08-04 20:31:14.000000 estela-0.2.6/estela_cli/list/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-08-04 20:31:14.000000 estela-0.2.6/estela_cli/list/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-08-04 20:31:14.000000 estela-0.2.6/estela_cli/list/spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-08-04 20:31:14.000000 estela-0.2.6/estela_cli/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-08-04 20:31:14.000000 estela-0.2.6/estela_cli/logout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 20:31:20.947227 estela-0.2.6/estela_cli/stop/
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-08-04 20:31:14.000000 estela-0.2.6/estela_cli/stop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-08-04 20:31:14.000000 estela-0.2.6/estela_cli/stop/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-08-04 20:31:14.000000 estela-0.2.6/estela_cli/templates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 20:31:20.947227 estela-0.2.6/estela_cli/update/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-08-04 20:31:14.000000 estela-0.2.6/estela_cli/update/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-08-04 20:31:14.000000 estela-0.2.6/estela_cli/update/cronjob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-08-04 20:31:14.000000 estela-0.2.6/estela_cli/update/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-08-04 20:31:14.000000 estela-0.2.6/estela_cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 20:31:20.947227 estela-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-08-04 20:31:14.000000 estela-0.2.6/setup.py
```

### Comparing `estela-0.2.5/README.md` & `estela-0.2.6/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <h1 align="center"> estela CLI </h1>
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![version](https://img.shields.io/badge/version-0.2.5-blue)](https://github.com/bitmakerla/estela-cli)
+[![version](https://img.shields.io/badge/version-0.2.6-blue)](https://github.com/bitmakerla/estela-cli)
 [![python-version](https://img.shields.io/badge/python-v3.10-orange)](https://www.python.org)
 
 
 estela CLI is a command line client to interact with the estela API. It allows the user to perform the following actions:
 - Link a Scrapy project with a project in estela.
 - Create projects, jobs, and cronjobs in estela.
 - Get the data of a job.
```

### Comparing `estela-0.2.5/estela.egg-info/SOURCES.txt` & `estela-0.2.6/estela.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `estela-0.2.5/estela_cli/__main__.py` & `estela-0.2.6/estela_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.5/estela_cli/context.py` & `estela-0.2.6/estela_cli/context.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.5/estela_cli/create/cronjob.py` & `estela-0.2.6/estela_cli/create/cronjob.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.5/estela_cli/create/job.py` & `estela-0.2.6/estela_cli/create/job.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.5/estela_cli/create/project.py` & `estela-0.2.6/estela_cli/create/project.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.5/estela_cli/data/job.py` & `estela-0.2.6/estela_cli/data/job.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.5/estela_cli/delete/project.py` & `estela-0.2.6/estela_cli/delete/project.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.5/estela_cli/deploy.py` & `estela-0.2.6/estela_cli/deploy.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 import os
 import click
 
-from string import Template
 from zipfile import ZipFile, ZIP_DEFLATED
 from estela_cli.utils import (
     get_project_path,
     get_estela_settings,
     _in,
-    get_estela_dockerfile_path,
 )
 from estela_cli.login import login
 from estela_cli.templates import (
     OK_EMOJI,
     ESTELA_DIR,
     ESTELA_YAML_NAME,
-    DOCKERFILE,
-    DOCKERFILE_NAME,
 )
 import logging
 
 
 SHORT_HELP = "Deploy Scrapy project to estela API"
 
 
@@ -36,43 +32,23 @@
             zip.write(root, os.path.relpath(root, relroot))
             for file in files:
                 filename = os.path.join(root, file)
                 arcname = os.path.join(os.path.relpath(root, relroot), file)
                 zip.write(filename, arcname)
 
 
-def update_dockerfile(requirements_path, python_version, entrypoint):
-    dockerfile_path = get_estela_dockerfile_path()
-
+def verify_requrements(requirements_path):
     project_path = get_project_path()
     requirements_local_path = os.path.join(project_path, requirements_path)
     if not os.path.exists(requirements_local_path):
         raise click.ClickException("The requirements file does not exist.")
 
-    template = Template(DOCKERFILE)
-    values = {
-        "python_version": python_version,
-        "requirements_path": requirements_path,
-        "entrypoint": entrypoint,
-    }
-    result = template.substitute(values)
-    with open(dockerfile_path, "r") as dock:
-        if result == dock.read():
-            click.echo(
-                "{}/{} not changes to update.".format(ESTELA_DIR, DOCKERFILE_NAME)
-            )
-            return
-
-    with open(dockerfile_path, "w+") as dockerfile:
-        dockerfile.write(result)
-        click.echo("{}/{} updated successfully.".format(ESTELA_DIR, DOCKERFILE_NAME))
-
 
 @click.command(short_help=SHORT_HELP)
-@click.option('--verbose', is_flag=True, help='Show debug logs.')
+@click.option("--verbose", is_flag=True, help="Show debug logs.")
 def estela_command(verbose):
     if verbose:
         logging.basicConfig(level=logging.DEBUG)
 
     estela_client = login()
     logging.debug(f"Successfully logged in to {estela_client.host}")
     estela_settings = get_estela_settings()
@@ -87,21 +63,17 @@
         estela_client.get_project(pid)
         logging.debug(f"Verified project exists.")
     except:
         raise click.ClickException(
             "Invalid project at {}/{}.".format(ESTELA_DIR, ESTELA_YAML_NAME)
         )
 
-    logging.debug(f"Updating Dockerfile...")
-    update_dockerfile(
-        p_settings["requirements"],
-        p_settings["python"],
-        p_settings["entrypoint"],
-    )
-    logging.debug(f"Successfully updated Dockerfile.")
+    logging.debug(f"Verifying requirements...")
+    verify_requrements(p_settings["requirements"])
+    logging.debug(f"Successfully verified requirements.")
 
     logging.debug(f"Zipping project for upload to estela...")
     zip_project(pid, project_path, estela_settings)
     logging.debug(f"Successfully zipped the project.")
 
     response = {}
     try:
```

### Comparing `estela-0.2.5/estela_cli/estela_client.py` & `estela-0.2.6/estela_cli/estela_client.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.5/estela_cli/init.py` & `estela-0.2.6/estela_cli/init.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.5/estela_cli/list/cronjob.py` & `estela-0.2.6/estela_cli/list/cronjob.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.5/estela_cli/list/job.py` & `estela-0.2.6/estela_cli/list/job.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.5/estela_cli/list/spider.py` & `estela-0.2.6/estela_cli/list/spider.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.5/estela_cli/login.py` & `estela-0.2.6/estela_cli/login.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.5/estela_cli/logout.py` & `estela-0.2.6/estela_cli/logout.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.5/estela_cli/stop/job.py` & `estela-0.2.6/estela_cli/stop/job.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.5/estela_cli/templates.py` & `estela-0.2.6/estela_cli/templates.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.5/estela_cli/update/cronjob.py` & `estela-0.2.6/estela_cli/update/cronjob.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.5/estela_cli/update/job.py` & `estela-0.2.6/estela_cli/update/job.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.5/estela_cli/utils.py` & `estela-0.2.6/estela_cli/utils.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.5/setup.py` & `estela-0.2.6/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="estela",
-    version="0.2.5",
+    version="0.2.6",
     description="Estela Command Line Interface",
     packages=find_packages(),
     entry_points={
         "console_scripts": [
             "estela = estela_cli.__main__:cli",
         ],
     },
```

