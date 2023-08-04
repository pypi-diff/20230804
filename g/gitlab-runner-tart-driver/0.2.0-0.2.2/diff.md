# Comparing `tmp/gitlab-runner-tart-driver-0.2.0.tar.gz` & `tmp/gitlab-runner-tart-driver-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitlab-runner-tart-driver-0.2.0.tar", last modified: Mon Jul  3 12:51:24 2023, max compression
+gzip compressed data, was "gitlab-runner-tart-driver-0.2.2.tar", last modified: Fri Aug  4 10:36:57 2023, max compression
```

## Comparing `gitlab-runner-tart-driver-0.2.0.tar` & `gitlab-runner-tart-driver-0.2.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 12:51:24.679694 gitlab-runner-tart-driver-0.2.0/
--rw-rw-rw-   0 root         (0) root         (0)     3303 2023-07-03 12:51:16.000000 gitlab-runner-tart-driver-0.2.0/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)       48 2023-07-03 12:51:16.000000 gitlab-runner-tart-driver-0.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    20528 2023-07-03 12:51:24.679694 gitlab-runner-tart-driver-0.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    20007 2023-07-03 12:51:16.000000 gitlab-runner-tart-driver-0.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 12:51:24.675694 gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-07-03 12:51:16.000000 gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      107 2023-07-03 12:51:16.000000 gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)      596 2023-07-03 12:51:16.000000 gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 12:51:24.678694 gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 12:51:16.000000 gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1321 2023-07-03 12:51:16.000000 gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver/commands/cleanup.py
--rw-rw-rw-   0 root         (0) root         (0)      760 2023-07-03 12:51:16.000000 gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver/commands/config.py
--rw-rw-rw-   0 root         (0) root         (0)    10415 2023-07-03 12:51:16.000000 gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver/commands/prepare.py
--rw-rw-rw-   0 root         (0) root         (0)     2235 2023-07-03 12:51:16.000000 gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver/commands/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 12:51:24.678694 gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver/modules/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 12:51:16.000000 gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver/modules/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3234 2023-07-03 12:51:16.000000 gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver/modules/gitlab_custom_command_config.py
--rw-rw-rw-   0 root         (0) root         (0)      405 2023-07-03 12:51:16.000000 gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver/modules/gitlab_custom_driver_config.py
--rw-rw-rw-   0 root         (0) root         (0)     8937 2023-07-03 12:51:16.000000 gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver/modules/tart.py
--rw-rw-rw-   0 root         (0) root         (0)      923 2023-07-03 12:51:16.000000 gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver/modules/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 12:51:24.679694 gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver/scripts/
--rwxrwxrwx   0 root         (0) root         (0)     2533 2023-07-03 12:51:16.000000 gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver/scripts/install-gitlab-runner.sh.j2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 12:51:24.677694 gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver.egg-info/
--rw-r--r--   0 root         (0) root         (0)    20528 2023-07-03 12:51:24.000000 gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1060 2023-07-03 12:51:24.000000 gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 12:51:24.000000 gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       82 2023-07-03 12:51:24.000000 gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 12:51:24.000000 gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       47 2023-07-03 12:51:24.000000 gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-07-03 12:51:24.000000 gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       31 2023-07-03 12:51:16.000000 gitlab-runner-tart-driver-0.2.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 12:51:24.679694 gitlab-runner-tart-driver-0.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1461 2023-07-03 12:51:16.000000 gitlab-runner-tart-driver-0.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 10:36:57.993769 gitlab-runner-tart-driver-0.2.2/
+-rw-rw-rw-   0 root         (0) root         (0)     3303 2023-08-04 10:36:50.000000 gitlab-runner-tart-driver-0.2.2/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       48 2023-08-04 10:36:50.000000 gitlab-runner-tart-driver-0.2.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    20528 2023-08-04 10:36:57.992769 gitlab-runner-tart-driver-0.2.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    20007 2023-08-04 10:36:50.000000 gitlab-runner-tart-driver-0.2.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 10:36:57.988769 gitlab-runner-tart-driver-0.2.2/gitlab_runner_tart_driver/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-08-04 10:36:50.000000 gitlab-runner-tart-driver-0.2.2/gitlab_runner_tart_driver/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      107 2023-08-04 10:36:50.000000 gitlab-runner-tart-driver-0.2.2/gitlab_runner_tart_driver/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)      596 2023-08-04 10:36:50.000000 gitlab-runner-tart-driver-0.2.2/gitlab_runner_tart_driver/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 10:36:57.991769 gitlab-runner-tart-driver-0.2.2/gitlab_runner_tart_driver/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-04 10:36:50.000000 gitlab-runner-tart-driver-0.2.2/gitlab_runner_tart_driver/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1321 2023-08-04 10:36:50.000000 gitlab-runner-tart-driver-0.2.2/gitlab_runner_tart_driver/commands/cleanup.py
+-rw-rw-rw-   0 root         (0) root         (0)      760 2023-08-04 10:36:50.000000 gitlab-runner-tart-driver-0.2.2/gitlab_runner_tart_driver/commands/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    10487 2023-08-04 10:36:50.000000 gitlab-runner-tart-driver-0.2.2/gitlab_runner_tart_driver/commands/prepare.py
+-rw-rw-rw-   0 root         (0) root         (0)     2235 2023-08-04 10:36:50.000000 gitlab-runner-tart-driver-0.2.2/gitlab_runner_tart_driver/commands/run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 10:36:57.992769 gitlab-runner-tart-driver-0.2.2/gitlab_runner_tart_driver/modules/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-04 10:36:50.000000 gitlab-runner-tart-driver-0.2.2/gitlab_runner_tart_driver/modules/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3234 2023-08-04 10:36:50.000000 gitlab-runner-tart-driver-0.2.2/gitlab_runner_tart_driver/modules/gitlab_custom_command_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      405 2023-08-04 10:36:50.000000 gitlab-runner-tart-driver-0.2.2/gitlab_runner_tart_driver/modules/gitlab_custom_driver_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     8965 2023-08-04 10:36:50.000000 gitlab-runner-tart-driver-0.2.2/gitlab_runner_tart_driver/modules/tart.py
+-rw-rw-rw-   0 root         (0) root         (0)      923 2023-08-04 10:36:50.000000 gitlab-runner-tart-driver-0.2.2/gitlab_runner_tart_driver/modules/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 10:36:57.992769 gitlab-runner-tart-driver-0.2.2/gitlab_runner_tart_driver/scripts/
+-rwxrwxrwx   0 root         (0) root         (0)     2533 2023-08-04 10:36:50.000000 gitlab-runner-tart-driver-0.2.2/gitlab_runner_tart_driver/scripts/install-gitlab-runner.sh.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 10:36:57.990769 gitlab-runner-tart-driver-0.2.2/gitlab_runner_tart_driver.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    20528 2023-08-04 10:36:57.000000 gitlab-runner-tart-driver-0.2.2/gitlab_runner_tart_driver.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1060 2023-08-04 10:36:57.000000 gitlab-runner-tart-driver-0.2.2/gitlab_runner_tart_driver.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 10:36:57.000000 gitlab-runner-tart-driver-0.2.2/gitlab_runner_tart_driver.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       82 2023-08-04 10:36:57.000000 gitlab-runner-tart-driver-0.2.2/gitlab_runner_tart_driver.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 10:36:57.000000 gitlab-runner-tart-driver-0.2.2/gitlab_runner_tart_driver.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       47 2023-08-04 10:36:57.000000 gitlab-runner-tart-driver-0.2.2/gitlab_runner_tart_driver.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-08-04 10:36:57.000000 gitlab-runner-tart-driver-0.2.2/gitlab_runner_tart_driver.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       31 2023-08-04 10:36:50.000000 gitlab-runner-tart-driver-0.2.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-04 10:36:57.993769 gitlab-runner-tart-driver-0.2.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1461 2023-08-04 10:36:50.000000 gitlab-runner-tart-driver-0.2.2/setup.py
```

### Comparing `gitlab-runner-tart-driver-0.2.0/LICENSE.txt` & `gitlab-runner-tart-driver-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.2.0/PKG-INFO` & `gitlab-runner-tart-driver-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlab-runner-tart-driver
-Version: 0.2.0
+Version: 0.2.2
 Home-page: https://gitlab.com/schmieder.matthias/gitlab-runner-tart-driver
 Author: Matthias Schmieder
 Author-email: schmieder.matthias@gmail.com
 License: BSD
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Developers
```

### Comparing `gitlab-runner-tart-driver-0.2.0/README.md` & `gitlab-runner-tart-driver-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver/cli.py` & `gitlab-runner-tart-driver-0.2.2/gitlab_runner_tart_driver/cli.py`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver/commands/cleanup.py` & `gitlab-runner-tart-driver-0.2.2/gitlab_runner_tart_driver/commands/cleanup.py`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver/commands/config.py` & `gitlab-runner-tart-driver-0.2.2/gitlab_runner_tart_driver/commands/config.py`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver/commands/prepare.py` & `gitlab-runner-tart-driver-0.2.2/gitlab_runner_tart_driver/commands/prepare.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,16 +174,18 @@
 
     # verfiy that the limit of running VMs is not exceeded
     list_running_vms = []
     for vm in tart.list():
         if vm.running:
             list_running_vms.append(vm)
 
-    if len(list_running_vms) >= p.tart_max_vm_count:
-        click.secho("[ERROR] The limit of running VMs is exceeded.", fg="red")
+    if len(list_running_vms) > p.tart_max_vm_count:
+        click.secho(
+            f"[ERROR] The limit of running VMs [{p.tart_max_vm_count}] is exceeded [{len(list_running_vms)}].", fg="red"
+        )
         sys.exit(1)
 
     click.echo(f"[INFO] Cloning VM instance '{tart_vm_name}' from '{p.ci_job_image}'")
     try:
         tart.clone(p.ci_job_image, tart_vm_name)
     except:
         click.secho(f"[ERROR] failed to clone image f'{p.ci_job_image}'", fg="red")
```

### Comparing `gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver/commands/run.py` & `gitlab-runner-tart-driver-0.2.2/gitlab_runner_tart_driver/commands/run.py`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver/modules/gitlab_custom_command_config.py` & `gitlab-runner-tart-driver-0.2.2/gitlab_runner_tart_driver/modules/gitlab_custom_command_config.py`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver/modules/tart.py` & `gitlab-runner-tart-driver-0.2.2/gitlab_runner_tart_driver/modules/tart.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,17 +62,17 @@
         self.ssh_client = SSHClient()
         self.ssh_client.set_missing_host_key_policy(MissingHostKeyPolicy())
         self.ssh_client.connect(ip, username=username, password=password)
 
     def exec_ssh_command(self, command, get_pty=True):
         """Executes an ssh command and prints it's output continously to stdout/stderr"""
         _, stdout, stderr = self.ssh_client.exec_command(command, get_pty=get_pty)
-        for line in iter(stdout.readline, ""):
+        for line in iter(lambda: stdout.readline(2048), ""):
             click.echo(line, nl=False)
-        for line in iter(stderr.readline, ""):
+        for line in iter(lambda: stderr.readline(2048), ""):
             click.echo(line, nl=False, err=True)
         return stdout.channel.recv_exit_status()
 
 
 class Tart(object):
     def __init__(self, exec_path="tart"):
         self.tart_executable = exec_path
```

### Comparing `gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver/modules/utils.py` & `gitlab-runner-tart-driver-0.2.2/gitlab_runner_tart_driver/modules/utils.py`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver/scripts/install-gitlab-runner.sh.j2` & `gitlab-runner-tart-driver-0.2.2/gitlab_runner_tart_driver/scripts/install-gitlab-runner.sh.j2`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver.egg-info/PKG-INFO` & `gitlab-runner-tart-driver-0.2.2/gitlab_runner_tart_driver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlab-runner-tart-driver
-Version: 0.2.0
+Version: 0.2.2
 Home-page: https://gitlab.com/schmieder.matthias/gitlab-runner-tart-driver
 Author: Matthias Schmieder
 Author-email: schmieder.matthias@gmail.com
 License: BSD
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Developers
```

### Comparing `gitlab-runner-tart-driver-0.2.0/gitlab_runner_tart_driver.egg-info/SOURCES.txt` & `gitlab-runner-tart-driver-0.2.2/gitlab_runner_tart_driver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.2.0/setup.py` & `gitlab-runner-tart-driver-0.2.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 # read the long description from README.md
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
-version = "0.2.0"
+version = "0.2.2"
 
 version = f"{version}{os.environ.get('PIP_VERSION_POSTFIX','')}"
 
 # read the requirements from requirements.txt
 requirements = []
 with pathlib.Path("requirements.txt").open() as requirements_txt:
     requirements = [str(requirement) for requirement in pkg_resources.parse_requirements(requirements_txt)]
```

