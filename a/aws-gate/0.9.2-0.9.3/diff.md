# Comparing `tmp/aws-gate-0.9.2.tar.gz` & `tmp/aws-gate-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aws-gate-0.9.2.tar", last modified: Sat Oct 17 10:20:30 2020, max compression
+gzip compressed data, was "aws-gate-0.9.3.tar", last modified: Wed Dec 23 09:33:05 2020, max compression
```

## Comparing `aws-gate-0.9.2.tar` & `aws-gate-0.9.3.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-17 10:20:30.764107 aws-gate-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (116)       52 2020-10-17 10:20:23.000000 aws-gate-0.9.2/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (116)     2982 2020-10-17 10:20:23.000000 aws-gate-0.9.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)      333 2020-10-17 10:20:23.000000 aws-gate-0.9.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (116)    17239 2020-10-17 10:20:23.000000 aws-gate-0.9.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (116)      284 2020-10-17 10:20:23.000000 aws-gate-0.9.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (116)      356 2020-10-17 10:20:23.000000 aws-gate-0.9.2/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (116)     4705 2020-10-17 10:20:23.000000 aws-gate-0.9.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (116)      498 2020-10-17 10:20:23.000000 aws-gate-0.9.2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (116)     1528 2020-10-17 10:20:23.000000 aws-gate-0.9.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (116)      124 2020-10-17 10:20:23.000000 aws-gate-0.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)    10825 2020-10-17 10:20:30.764107 aws-gate-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     8393 2020-10-17 10:20:23.000000 aws-gate-0.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-17 10:20:30.760107 aws-gate-0.9.2/aws_gate/
--rw-r--r--   0 runner    (1001) docker     (116)      204 2020-10-17 10:20:23.000000 aws-gate-0.9.2/aws_gate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3919 2020-10-17 10:20:23.000000 aws-gate-0.9.2/aws_gate/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (116)     9767 2020-10-17 10:20:23.000000 aws-gate-0.9.2/aws_gate/cli.py
--rw-r--r--   0 runner    (1001) docker     (116)     4491 2020-10-17 10:20:23.000000 aws-gate-0.9.2/aws_gate/config.py
--rw-r--r--   0 runner    (1001) docker     (116)     1670 2020-10-17 10:20:23.000000 aws-gate-0.9.2/aws_gate/constants.py
--rw-r--r--   0 runner    (1001) docker     (116)     2102 2020-10-17 10:20:23.000000 aws-gate-0.9.2/aws_gate/decorators.py
--rw-r--r--   0 runner    (1001) docker     (116)      168 2020-10-17 10:20:23.000000 aws-gate-0.9.2/aws_gate/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (116)     2099 2020-10-17 10:20:23.000000 aws-gate-0.9.2/aws_gate/exec.py
--rw-r--r--   0 runner    (1001) docker     (116)     2865 2020-10-17 10:20:23.000000 aws-gate-0.9.2/aws_gate/list.py
--rw-r--r--   0 runner    (1001) docker     (116)     4020 2020-10-17 10:20:23.000000 aws-gate-0.9.2/aws_gate/query.py
--rw-r--r--   0 runner    (1001) docker     (116)     1779 2020-10-17 10:20:23.000000 aws-gate-0.9.2/aws_gate/session.py
--rw-r--r--   0 runner    (1001) docker     (116)     1518 2020-10-17 10:20:23.000000 aws-gate-0.9.2/aws_gate/session_common.py
--rw-r--r--   0 runner    (1001) docker     (116)     4467 2020-10-17 10:20:23.000000 aws-gate-0.9.2/aws_gate/ssh.py
--rw-r--r--   0 runner    (1001) docker     (116)     3972 2020-10-17 10:20:23.000000 aws-gate-0.9.2/aws_gate/ssh_common.py
--rw-r--r--   0 runner    (1001) docker     (116)     1124 2020-10-17 10:20:23.000000 aws-gate-0.9.2/aws_gate/ssh_config.py
--rw-r--r--   0 runner    (1001) docker     (116)     2939 2020-10-17 10:20:23.000000 aws-gate-0.9.2/aws_gate/ssh_proxy.py
--rw-r--r--   0 runner    (1001) docker     (116)     6784 2020-10-17 10:20:23.000000 aws-gate-0.9.2/aws_gate/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-17 10:20:30.760107 aws-gate-0.9.2/aws_gate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)    10825 2020-10-17 10:20:30.000000 aws-gate-0.9.2/aws_gate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1341 2020-10-17 10:20:30.000000 aws-gate-0.9.2/aws_gate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-10-17 10:20:30.000000 aws-gate-0.9.2/aws_gate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      133 2020-10-17 10:20:30.000000 aws-gate-0.9.2/aws_gate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       15 2020-10-17 10:20:30.000000 aws-gate-0.9.2/aws_gate.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-17 10:20:30.760107 aws-gate-0.9.2/bin/
--rwxr-xr-x   0 runner    (1001) docker     (116)      122 2020-10-17 10:20:23.000000 aws-gate-0.9.2/bin/aws-gate
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-17 10:20:30.760107 aws-gate-0.9.2/docs/
--rw-r--r--   0 runner    (1001) docker     (116)     4705 2020-10-17 10:20:23.000000 aws-gate-0.9.2/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (116)     3151 2020-10-17 10:20:23.000000 aws-gate-0.9.2/docs/command-line.md
--rw-r--r--   0 runner    (1001) docker     (116)     1239 2020-10-17 10:20:23.000000 aws-gate-0.9.2/docs/configuration.md
--rw-r--r--   0 runner    (1001) docker     (116)     1888 2020-10-17 10:20:23.000000 aws-gate-0.9.2/docs/development.md
--rw-r--r--   0 runner    (1001) docker     (116)     2276 2020-10-17 10:20:23.000000 aws-gate-0.9.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (116)     1528 2020-10-17 10:20:23.000000 aws-gate-0.9.2/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (116)     4256 2020-10-17 10:20:23.000000 aws-gate-0.9.2/docs/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (116)      401 2020-10-17 10:20:23.000000 aws-gate-0.9.2/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-17 10:20:30.760107 aws-gate-0.9.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (116)      133 2020-10-17 10:20:23.000000 aws-gate-0.9.2/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)      379 2020-10-17 10:20:23.000000 aws-gate-0.9.2/requirements/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (116)       14 2020-10-17 10:20:23.000000 aws-gate-0.9.2/requirements/requirements_doc.txt
--rw-r--r--   0 runner    (1001) docker     (116)      218 2020-10-17 10:20:30.764107 aws-gate-0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1509 2020-10-17 10:20:23.000000 aws-gate-0.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-17 10:20:30.760107 aws-gate-0.9.2/tests/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-10-17 10:20:23.000000 aws-gate-0.9.2/tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     1457 2020-10-17 10:20:23.000000 aws-gate-0.9.2/tests/run.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-17 10:20:30.764107 aws-gate-0.9.2/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-10-17 10:20:23.000000 aws-gate-0.9.2/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2633 2020-10-17 10:20:23.000000 aws-gate-0.9.2/tests/unit/conftest.py
--rw-r--r--   0 runner    (1001) docker     (116)     3599 2020-10-17 10:20:23.000000 aws-gate-0.9.2/tests/unit/test_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (116)     5188 2020-10-17 10:20:23.000000 aws-gate-0.9.2/tests/unit/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (116)     6965 2020-10-17 10:20:23.000000 aws-gate-0.9.2/tests/unit/test_config.py
--rw-r--r--   0 runner    (1001) docker     (116)     2746 2020-10-17 10:20:23.000000 aws-gate-0.9.2/tests/unit/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (116)     4423 2020-10-17 10:20:23.000000 aws-gate-0.9.2/tests/unit/test_exec.py
--rw-r--r--   0 runner    (1001) docker     (116)     2639 2020-10-17 10:20:23.000000 aws-gate-0.9.2/tests/unit/test_list.py
--rw-r--r--   0 runner    (1001) docker     (116)     2097 2020-10-17 10:20:23.000000 aws-gate-0.9.2/tests/unit/test_query.py
--rw-r--r--   0 runner    (1001) docker     (116)     4198 2020-10-17 10:20:23.000000 aws-gate-0.9.2/tests/unit/test_session.py
--rw-r--r--   0 runner    (1001) docker     (116)     5795 2020-10-17 10:20:23.000000 aws-gate-0.9.2/tests/unit/test_ssh.py
--rw-r--r--   0 runner    (1001) docker     (116)     3425 2020-10-17 10:20:23.000000 aws-gate-0.9.2/tests/unit/test_ssh_common.py
--rw-r--r--   0 runner    (1001) docker     (116)     1283 2020-10-17 10:20:23.000000 aws-gate-0.9.2/tests/unit/test_ssh_config.py
--rw-r--r--   0 runner    (1001) docker     (116)     5196 2020-10-17 10:20:23.000000 aws-gate-0.9.2/tests/unit/test_ssh_proxy.py
--rw-r--r--   0 runner    (1001) docker     (116)     7436 2020-10-17 10:20:23.000000 aws-gate-0.9.2/tests/unit/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-23 09:33:05.501291 aws-gate-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (116)       52 2020-12-23 09:32:52.000000 aws-gate-0.9.3/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (116)     2982 2020-12-23 09:32:52.000000 aws-gate-0.9.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (116)      333 2020-12-23 09:32:52.000000 aws-gate-0.9.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)    17239 2020-12-23 09:32:52.000000 aws-gate-0.9.3/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (116)      284 2020-12-23 09:32:52.000000 aws-gate-0.9.3/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      356 2020-12-23 09:32:52.000000 aws-gate-0.9.3/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (116)     4767 2020-12-23 09:32:52.000000 aws-gate-0.9.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (116)      498 2020-12-23 09:32:52.000000 aws-gate-0.9.3/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (116)     1528 2020-12-23 09:32:52.000000 aws-gate-0.9.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (116)      124 2020-12-23 09:32:52.000000 aws-gate-0.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)    10825 2020-12-23 09:33:05.501291 aws-gate-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     8393 2020-12-23 09:32:52.000000 aws-gate-0.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-23 09:33:05.501291 aws-gate-0.9.3/aws_gate/
+-rw-r--r--   0 runner    (1001) docker     (116)      204 2020-12-23 09:32:52.000000 aws-gate-0.9.3/aws_gate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3919 2020-12-23 09:32:52.000000 aws-gate-0.9.3/aws_gate/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9767 2020-12-23 09:32:52.000000 aws-gate-0.9.3/aws_gate/cli.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4491 2020-12-23 09:32:52.000000 aws-gate-0.9.3/aws_gate/config.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1670 2020-12-23 09:32:52.000000 aws-gate-0.9.3/aws_gate/constants.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2102 2020-12-23 09:32:52.000000 aws-gate-0.9.3/aws_gate/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (116)      168 2020-12-23 09:32:52.000000 aws-gate-0.9.3/aws_gate/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2099 2020-12-23 09:32:52.000000 aws-gate-0.9.3/aws_gate/exec.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2865 2020-12-23 09:32:52.000000 aws-gate-0.9.3/aws_gate/list.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4020 2020-12-23 09:32:52.000000 aws-gate-0.9.3/aws_gate/query.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1779 2020-12-23 09:32:52.000000 aws-gate-0.9.3/aws_gate/session.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1518 2020-12-23 09:32:52.000000 aws-gate-0.9.3/aws_gate/session_common.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4467 2020-12-23 09:32:52.000000 aws-gate-0.9.3/aws_gate/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3972 2020-12-23 09:32:52.000000 aws-gate-0.9.3/aws_gate/ssh_common.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1124 2020-12-23 09:32:52.000000 aws-gate-0.9.3/aws_gate/ssh_config.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2939 2020-12-23 09:32:52.000000 aws-gate-0.9.3/aws_gate/ssh_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6923 2020-12-23 09:32:52.000000 aws-gate-0.9.3/aws_gate/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-23 09:33:05.501291 aws-gate-0.9.3/aws_gate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)    10825 2020-12-23 09:33:05.000000 aws-gate-0.9.3/aws_gate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     1341 2020-12-23 09:33:05.000000 aws-gate-0.9.3/aws_gate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-23 09:33:05.000000 aws-gate-0.9.3/aws_gate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      133 2020-12-23 09:33:05.000000 aws-gate-0.9.3/aws_gate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       15 2020-12-23 09:33:05.000000 aws-gate-0.9.3/aws_gate.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-23 09:33:05.501291 aws-gate-0.9.3/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (116)      122 2020-12-23 09:32:52.000000 aws-gate-0.9.3/bin/aws-gate
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-23 09:33:05.501291 aws-gate-0.9.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (116)     4767 2020-12-23 09:32:52.000000 aws-gate-0.9.3/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (116)     3151 2020-12-23 09:32:52.000000 aws-gate-0.9.3/docs/command-line.md
+-rw-r--r--   0 runner    (1001) docker     (116)     1239 2020-12-23 09:32:52.000000 aws-gate-0.9.3/docs/configuration.md
+-rw-r--r--   0 runner    (1001) docker     (116)     1888 2020-12-23 09:32:52.000000 aws-gate-0.9.3/docs/development.md
+-rw-r--r--   0 runner    (1001) docker     (116)     2276 2020-12-23 09:32:52.000000 aws-gate-0.9.3/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (116)     1528 2020-12-23 09:32:52.000000 aws-gate-0.9.3/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (116)     4256 2020-12-23 09:32:52.000000 aws-gate-0.9.3/docs/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (116)      401 2020-12-23 09:32:52.000000 aws-gate-0.9.3/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-23 09:33:05.501291 aws-gate-0.9.3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (116)      133 2020-12-23 09:32:52.000000 aws-gate-0.9.3/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      380 2020-12-23 09:32:52.000000 aws-gate-0.9.3/requirements/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       14 2020-12-23 09:32:52.000000 aws-gate-0.9.3/requirements/requirements_doc.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      218 2020-12-23 09:33:05.505291 aws-gate-0.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     1509 2020-12-23 09:32:52.000000 aws-gate-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-23 09:33:05.501291 aws-gate-0.9.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-12-23 09:32:52.000000 aws-gate-0.9.3/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     1457 2020-12-23 09:32:52.000000 aws-gate-0.9.3/tests/run.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-23 09:33:05.501291 aws-gate-0.9.3/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-12-23 09:32:52.000000 aws-gate-0.9.3/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2633 2020-12-23 09:32:52.000000 aws-gate-0.9.3/tests/unit/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3599 2020-12-23 09:32:52.000000 aws-gate-0.9.3/tests/unit/test_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5188 2020-12-23 09:32:52.000000 aws-gate-0.9.3/tests/unit/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6965 2020-12-23 09:32:52.000000 aws-gate-0.9.3/tests/unit/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2746 2020-12-23 09:32:52.000000 aws-gate-0.9.3/tests/unit/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4423 2020-12-23 09:32:52.000000 aws-gate-0.9.3/tests/unit/test_exec.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2639 2020-12-23 09:32:52.000000 aws-gate-0.9.3/tests/unit/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2097 2020-12-23 09:32:52.000000 aws-gate-0.9.3/tests/unit/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4198 2020-12-23 09:32:52.000000 aws-gate-0.9.3/tests/unit/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5795 2020-12-23 09:32:52.000000 aws-gate-0.9.3/tests/unit/test_ssh.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3425 2020-12-23 09:32:52.000000 aws-gate-0.9.3/tests/unit/test_ssh_common.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1283 2020-12-23 09:32:52.000000 aws-gate-0.9.3/tests/unit/test_ssh_config.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5196 2020-12-23 09:32:52.000000 aws-gate-0.9.3/tests/unit/test_ssh_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7436 2020-12-23 09:32:52.000000 aws-gate-0.9.3/tests/unit/test_utils.py
```

### Comparing `aws-gate-0.9.2/.gitignore` & `aws-gate-0.9.3/.gitignore`

 * *Files identical despite different names*

### Comparing `aws-gate-0.9.2/.pylintrc` & `aws-gate-0.9.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `aws-gate-0.9.2/CHANGELOG.md` & `aws-gate-0.9.3/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,13 @@
-0.9.2 (2020-10-10)
+0.9.3 (2020-12-23)
+------------------
+
+* Add new AWS regions
+
+0.9.2 (2020-10-17)
 ------------------
 
 * Fix regression introduced in #572, which resulted in not being to find bootstrapped plugin
 * Plugin version comparison is using more robust mechanism to determine newer plugin version
 
 0.9.1 (2020-10-06)
 ------------------
```

### Comparing `aws-gate-0.9.2/LICENSE.md` & `aws-gate-0.9.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aws-gate-0.9.2/PKG-INFO` & `aws-gate-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-gate
-Version: 0.9.2
+Version: 0.9.3
 Summary: aws-gate - AWS SSM Session Manager client CLI
 Home-page: https://github.com/xen0l/aws-gate
 Author: Adam Stevko
 Author-email: adam.stevko@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/xen0l/aws-gate/issues
 Project-URL: Source Code, https://github.com/xen0l/aws-gate
```

### Comparing `aws-gate-0.9.2/README.md` & `aws-gate-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `aws-gate-0.9.2/aws_gate/bootstrap.py` & `aws-gate-0.9.3/aws_gate/bootstrap.py`

 * *Files identical despite different names*

### Comparing `aws-gate-0.9.2/aws_gate/cli.py` & `aws-gate-0.9.3/aws_gate/cli.py`

 * *Files identical despite different names*

### Comparing `aws-gate-0.9.2/aws_gate/config.py` & `aws-gate-0.9.3/aws_gate/config.py`

 * *Files identical despite different names*

### Comparing `aws-gate-0.9.2/aws_gate/constants.py` & `aws-gate-0.9.3/aws_gate/constants.py`

 * *Files identical despite different names*

### Comparing `aws-gate-0.9.2/aws_gate/decorators.py` & `aws-gate-0.9.3/aws_gate/decorators.py`

 * *Files identical despite different names*

### Comparing `aws-gate-0.9.2/aws_gate/exec.py` & `aws-gate-0.9.3/aws_gate/exec.py`

 * *Files identical despite different names*

### Comparing `aws-gate-0.9.2/aws_gate/list.py` & `aws-gate-0.9.3/aws_gate/list.py`

 * *Files identical despite different names*

### Comparing `aws-gate-0.9.2/aws_gate/query.py` & `aws-gate-0.9.3/aws_gate/query.py`

 * *Files identical despite different names*

### Comparing `aws-gate-0.9.2/aws_gate/session.py` & `aws-gate-0.9.3/aws_gate/session.py`

 * *Files identical despite different names*

### Comparing `aws-gate-0.9.2/aws_gate/session_common.py` & `aws-gate-0.9.3/aws_gate/session_common.py`

 * *Files identical despite different names*

### Comparing `aws-gate-0.9.2/aws_gate/ssh.py` & `aws-gate-0.9.3/aws_gate/ssh.py`

 * *Files identical despite different names*

### Comparing `aws-gate-0.9.2/aws_gate/ssh_common.py` & `aws-gate-0.9.3/aws_gate/ssh_common.py`

 * *Files identical despite different names*

### Comparing `aws-gate-0.9.2/aws_gate/ssh_config.py` & `aws-gate-0.9.3/aws_gate/ssh_config.py`

 * *Files identical despite different names*

### Comparing `aws-gate-0.9.2/aws_gate/ssh_proxy.py` & `aws-gate-0.9.3/aws_gate/ssh_proxy.py`

 * *Files identical despite different names*

### Comparing `aws-gate-0.9.2/aws_gate/utils.py` & `aws-gate-0.9.3/aws_gate/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,29 +15,36 @@
 
 logger = logging.getLogger(__name__)
 
 # This list is maintained by hand as new regions are not added that often. This should be
 # removed once, we find a better way how to obtain region list without the need to
 # contact AWS EC2 API
 AWS_REGIONS = [
+    "af-south-1",
+    "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
-    "ap-northeast-3",
     "ap-south-1",
     "ap-southeast-1",
     "ap-southeast-2",
     "ca-central-1",
+    "cn-north-1",
+    "cn-northwest-1",
     "eu-central-1",
     "eu-north-1",
+    "eu-south-1",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
+    "us-gov-east-1",
+    "us-gov-west-1",
     "us-west-1",
     "us-west-2",
 ]
 
 
 def _create_aws_session(region_name=None, profile_name=None):
     logger.debug("Obtaining boto3 session object")
@@ -188,16 +195,16 @@
 def get_instance_details(instance_id, ec2=None):
     return get_multiple_instance_details(instance_ids=[instance_id], ec2=ec2)[0]
 
 
 def get_multiple_instance_details(instance_ids, ec2=None):
     try:
         ec2_instances = list(ec2.instances.filter(InstanceIds=instance_ids))
-    except botocore.exceptions.ClientError:
-        raise AWSConnectionError
+    except botocore.exceptions.ClientError as e:
+        raise AWSConnectionError(e)
 
     instance_details = []
     for ec2_instance in ec2_instances:
         instance_name = None
         for tag in ec2_instance.tags:
             if tag["Key"] == "Name":
                 instance_name = tag["Value"]
```

### Comparing `aws-gate-0.9.2/aws_gate.egg-info/PKG-INFO` & `aws-gate-0.9.3/aws_gate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-gate
-Version: 0.9.2
+Version: 0.9.3
 Summary: aws-gate - AWS SSM Session Manager client CLI
 Home-page: https://github.com/xen0l/aws-gate
 Author: Adam Stevko
 Author-email: adam.stevko@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/xen0l/aws-gate/issues
 Project-URL: Source Code, https://github.com/xen0l/aws-gate
```

### Comparing `aws-gate-0.9.2/aws_gate.egg-info/SOURCES.txt` & `aws-gate-0.9.3/aws_gate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aws-gate-0.9.2/docs/changelog.md` & `aws-gate-0.9.3/docs/changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,13 @@
-0.9.2 (2020-10-10)
+0.9.3 (2020-12-23)
+------------------
+
+* Add new AWS regions
+
+0.9.2 (2020-10-17)
 ------------------
 
 * Fix regression introduced in #572, which resulted in not being to find bootstrapped plugin
 * Plugin version comparison is using more robust mechanism to determine newer plugin version
 
 0.9.1 (2020-10-06)
 ------------------
```

### Comparing `aws-gate-0.9.2/docs/command-line.md` & `aws-gate-0.9.3/docs/command-line.md`

 * *Files identical despite different names*

### Comparing `aws-gate-0.9.2/docs/configuration.md` & `aws-gate-0.9.3/docs/configuration.md`

 * *Files identical despite different names*

### Comparing `aws-gate-0.9.2/docs/development.md` & `aws-gate-0.9.3/docs/development.md`

 * *Files identical despite different names*

### Comparing `aws-gate-0.9.2/docs/index.md` & `aws-gate-0.9.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `aws-gate-0.9.2/docs/license.md` & `aws-gate-0.9.3/docs/license.md`

 * *Files identical despite different names*

### Comparing `aws-gate-0.9.2/docs/quickstart.md` & `aws-gate-0.9.3/docs/quickstart.md`

 * *Files identical despite different names*

### Comparing `aws-gate-0.9.2/setup.py` & `aws-gate-0.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `aws-gate-0.9.2/tests/run.py` & `aws-gate-0.9.3/tests/run.py`

 * *Files identical despite different names*

### Comparing `aws-gate-0.9.2/tests/unit/conftest.py` & `aws-gate-0.9.3/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `aws-gate-0.9.2/tests/unit/test_bootstrap.py` & `aws-gate-0.9.3/tests/unit/test_bootstrap.py`

 * *Files identical despite different names*

### Comparing `aws-gate-0.9.2/tests/unit/test_cli.py` & `aws-gate-0.9.3/tests/unit/test_cli.py`

 * *Files identical despite different names*

### Comparing `aws-gate-0.9.2/tests/unit/test_config.py` & `aws-gate-0.9.3/tests/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `aws-gate-0.9.2/tests/unit/test_decorators.py` & `aws-gate-0.9.3/tests/unit/test_decorators.py`

 * *Files identical despite different names*

### Comparing `aws-gate-0.9.2/tests/unit/test_exec.py` & `aws-gate-0.9.3/tests/unit/test_exec.py`

 * *Files identical despite different names*

### Comparing `aws-gate-0.9.2/tests/unit/test_list.py` & `aws-gate-0.9.3/tests/unit/test_list.py`

 * *Files identical despite different names*

### Comparing `aws-gate-0.9.2/tests/unit/test_query.py` & `aws-gate-0.9.3/tests/unit/test_query.py`

 * *Files identical despite different names*

### Comparing `aws-gate-0.9.2/tests/unit/test_session.py` & `aws-gate-0.9.3/tests/unit/test_session.py`

 * *Files identical despite different names*

### Comparing `aws-gate-0.9.2/tests/unit/test_ssh.py` & `aws-gate-0.9.3/tests/unit/test_ssh.py`

 * *Files identical despite different names*

### Comparing `aws-gate-0.9.2/tests/unit/test_ssh_common.py` & `aws-gate-0.9.3/tests/unit/test_ssh_common.py`

 * *Files identical despite different names*

### Comparing `aws-gate-0.9.2/tests/unit/test_ssh_config.py` & `aws-gate-0.9.3/tests/unit/test_ssh_config.py`

 * *Files identical despite different names*

### Comparing `aws-gate-0.9.2/tests/unit/test_ssh_proxy.py` & `aws-gate-0.9.3/tests/unit/test_ssh_proxy.py`

 * *Files identical despite different names*

### Comparing `aws-gate-0.9.2/tests/unit/test_utils.py` & `aws-gate-0.9.3/tests/unit/test_utils.py`

 * *Files identical despite different names*

