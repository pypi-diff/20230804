# Comparing `tmp/grpc-accesslog-0.1.1.tar.gz` & `tmp/grpc_accesslog-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grpc-accesslog-0.1.1.tar", max compression
+gzip compressed data, was "grpc_accesslog-0.2.0.tar", max compression
```

## Comparing `grpc-accesslog-0.1.1.tar` & `grpc_accesslog-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     1086 2022-08-15 20:51:16.881666 grpc-accesslog-0.1.1/LICENSE.rst
--rw-r--r--   0        0        0     3009 2022-08-15 20:51:16.881666 grpc-accesslog-0.1.1/README.rst
--rw-r--r--   0        0        0     1828 2022-08-15 20:51:28.457724 grpc-accesslog-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      161 2022-08-15 20:51:16.881666 grpc-accesslog-0.1.1/src/grpc_accesslog/__init__.py
--rw-r--r--   0        0        0      339 2022-08-15 20:51:16.881666 grpc-accesslog-0.1.1/src/grpc_accesslog/_context.py
--rw-r--r--   0        0        0     3222 2022-08-15 20:51:16.881666 grpc-accesslog-0.1.1/src/grpc_accesslog/_server.py
--rw-r--r--   0        0        0     3357 2022-08-15 20:51:16.881666 grpc-accesslog-0.1.1/src/grpc_accesslog/handlers.py
--rw-r--r--   0        0        0        0 2022-08-15 20:51:16.881666 grpc-accesslog-0.1.1/src/grpc_accesslog/py.typed
--rw-r--r--   0        0        0     3972 2022-08-15 20:51:31.056908 grpc-accesslog-0.1.1/setup.py
--rw-r--r--   0        0        0     3913 2022-08-15 20:51:31.057360 grpc-accesslog-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-08-04 02:36:45.299019 grpc_accesslog-0.2.0/LICENSE.rst
+-rw-r--r--   0        0        0     3009 2023-08-04 02:36:45.299019 grpc_accesslog-0.2.0/README.rst
+-rw-r--r--   0        0        0     1973 2023-08-04 02:37:00.635139 grpc_accesslog-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      161 2023-08-04 02:36:45.299019 grpc_accesslog-0.2.0/src/grpc_accesslog/__init__.py
+-rw-r--r--   0        0        0      339 2023-08-04 02:36:45.299019 grpc_accesslog-0.2.0/src/grpc_accesslog/_context.py
+-rw-r--r--   0        0        0     6379 2023-08-04 02:36:45.299019 grpc_accesslog-0.2.0/src/grpc_accesslog/_server.py
+-rw-r--r--   0        0        0     3357 2023-08-04 02:36:45.299019 grpc_accesslog-0.2.0/src/grpc_accesslog/handlers.py
+-rw-r--r--   0        0        0        0 2023-08-04 02:36:45.299019 grpc_accesslog-0.2.0/src/grpc_accesslog/py.typed
+-rw-r--r--   0        0        0     3874 1970-01-01 00:00:00.000000 grpc_accesslog-0.2.0/PKG-INFO
```

### Comparing `grpc-accesslog-0.1.1/LICENSE.rst` & `grpc_accesslog-0.2.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `grpc-accesslog-0.1.1/README.rst` & `grpc_accesslog-0.2.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 * Write stdout logs for every RPC request
 * Log messages built with customizable callback handlers
 
 
 Requirements
 ------------
 
-* Python 3.7+
+* Python 3.8+
 * grpc-interceptors 0.13+
 
 
 Installation
 ------------
 
 You can install *gRPC Access Log* via pip_ from PyPI_:
```

### Comparing `grpc-accesslog-0.1.1/src/grpc_accesslog/handlers.py` & `grpc_accesslog-0.2.0/src/grpc_accesslog/handlers.py`

 * *Files identical despite different names*

### Comparing `grpc-accesslog-0.1.1/setup.py` & `grpc_accesslog-0.2.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,127 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: grpc-accesslog
+Version: 0.2.0
+Summary: gRPC Access Log
+Home-page: https://github.com/villainy/grpc-accesslog
+License: MIT
+Author: Michael Morgan
+Author-email: git@morgan83.com
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: grpcio (>=1.56.2,<2.0.0)
+Project-URL: Changelog, https://github.com/villainy/grpc-accesslog/releases
+Project-URL: Documentation, https://grpc-accesslog.readthedocs.io
+Project-URL: Repository, https://github.com/villainy/grpc-accesslog
+Description-Content-Type: text/x-rst
 
-package_dir = \
-{'': 'src'}
+gRPC Access Log
+===============
 
-packages = \
-['grpc_accesslog']
+|PyPI| |Status| |Python Version| |License|
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['grpc-interceptor>=0.13.0', 'grpc-stubs>=1.24.5']
-
-entry_points = \
-{'console_scripts': ['grpc-accesslog = grpc_accesslog.__main__:main']}
-
-setup_kwargs = {
-    'name': 'grpc-accesslog',
-    'version': '0.1.1',
-    'description': 'gRPC Access Log',
-    'long_description': "gRPC Access Log\n===============\n\n|PyPI| |Status| |Python Version| |License|\n\n|Read the Docs| |Tests| |Codecov|\n\n|pre-commit| |Black|\n\n.. |PyPI| image:: https://img.shields.io/pypi/v/grpc-accesslog.svg\n   :target: https://pypi.org/project/grpc-accesslog/\n   :alt: PyPI\n.. |Status| image:: https://img.shields.io/pypi/status/grpc-accesslog.svg\n   :target: https://pypi.org/project/grpc-accesslog/\n   :alt: Status\n.. |Python Version| image:: https://img.shields.io/pypi/pyversions/grpc-accesslog\n   :target: https://pypi.org/project/grpc-accesslog\n   :alt: Python Version\n.. |License| image:: https://img.shields.io/pypi/l/grpc-accesslog\n   :target: https://opensource.org/licenses/MIT\n   :alt: License\n.. |Read the Docs| image:: https://img.shields.io/readthedocs/grpc-accesslog/latest.svg?label=Read%20the%20Docs\n   :target: https://grpc-accesslog.readthedocs.io/\n   :alt: Read the documentation at https://grpc-accesslog.readthedocs.io/\n.. |Tests| image:: https://github.com/villainy/grpc-accesslog/workflows/Tests/badge.svg\n   :target: https://github.com/villainy/grpc-accesslog/actions?workflow=Tests\n   :alt: Tests\n.. |Codecov| image:: https://codecov.io/gh/villainy/grpc-accesslog/branch/main/graph/badge.svg\n   :target: https://app.codecov.io/gh/villainy/grpc-accesslog\n   :alt: Codecov\n.. |pre-commit| image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white\n   :target: https://github.com/pre-commit/pre-commit\n   :alt: pre-commit\n.. |Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg\n   :target: https://github.com/psf/black\n   :alt: Black\n\n\nFeatures\n--------\n\n* Write stdout logs for every RPC request\n* Log messages built with customizable callback handlers\n\n\nRequirements\n------------\n\n* Python 3.7+\n* grpc-interceptors 0.13+\n\n\nInstallation\n------------\n\nYou can install *gRPC Access Log* via pip_ from PyPI_:\n\n.. code:: console\n\n   $ pip install grpc-accesslog\n\n\nUsage\n-----\n\nPlease see the `Reference <Usage_>`_ for details.\n\n\nContributing\n------------\n\nContributions are very welcome.\nTo learn more, see the `Contributor Guide`_.\n\n\nLicense\n-------\n\nDistributed under the terms of the `MIT license`_,\n*gRPC Access Log* is free and open source software.\n\n\nIssues\n------\n\nIf you encounter any problems,\nplease `file an issue`_ along with a detailed description.\n\n\nCredits\n-------\n\nThis project was generated from `@cjolowicz`_'s `Hypermodern Python Cookiecutter`_ template.\n\n.. _@cjolowicz: https://github.com/cjolowicz\n.. _Cookiecutter: https://github.com/audreyr/cookiecutter\n.. _MIT license: https://opensource.org/licenses/MIT\n.. _PyPI: https://pypi.org/\n.. _Hypermodern Python Cookiecutter: https://github.com/cjolowicz/cookiecutter-hypermodern-python\n.. _file an issue: https://github.com/villainy/grpc-accesslog/issues\n.. _pip: https://pip.pypa.io/\n.. github-only\n.. _Contributor Guide: https://grpc-accesslog.readthedocs.io/en/latest/contributing.html\n.. _Usage: https://grpc-accesslog.readthedocs.io/en/latest/usage.html\n",
-    'author': 'Michael Morgan',
-    'author_email': 'git@morgan83.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/villainy/grpc-accesslog',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
+|Read the Docs| |Tests| |Codecov|
 
+|pre-commit| |Black|
+
+.. |PyPI| image:: https://img.shields.io/pypi/v/grpc-accesslog.svg
+   :target: https://pypi.org/project/grpc-accesslog/
+   :alt: PyPI
+.. |Status| image:: https://img.shields.io/pypi/status/grpc-accesslog.svg
+   :target: https://pypi.org/project/grpc-accesslog/
+   :alt: Status
+.. |Python Version| image:: https://img.shields.io/pypi/pyversions/grpc-accesslog
+   :target: https://pypi.org/project/grpc-accesslog
+   :alt: Python Version
+.. |License| image:: https://img.shields.io/pypi/l/grpc-accesslog
+   :target: https://opensource.org/licenses/MIT
+   :alt: License
+.. |Read the Docs| image:: https://img.shields.io/readthedocs/grpc-accesslog/latest.svg?label=Read%20the%20Docs
+   :target: https://grpc-accesslog.readthedocs.io/
+   :alt: Read the documentation at https://grpc-accesslog.readthedocs.io/
+.. |Tests| image:: https://github.com/villainy/grpc-accesslog/workflows/Tests/badge.svg
+   :target: https://github.com/villainy/grpc-accesslog/actions?workflow=Tests
+   :alt: Tests
+.. |Codecov| image:: https://codecov.io/gh/villainy/grpc-accesslog/branch/main/graph/badge.svg
+   :target: https://app.codecov.io/gh/villainy/grpc-accesslog
+   :alt: Codecov
+.. |pre-commit| image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
+   :target: https://github.com/pre-commit/pre-commit
+   :alt: pre-commit
+.. |Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
+   :target: https://github.com/psf/black
+   :alt: Black
+
+
+Features
+--------
+
+* Write stdout logs for every RPC request
+* Log messages built with customizable callback handlers
+
+
+Requirements
+------------
+
+* Python 3.8+
+* grpc-interceptors 0.13+
+
+
+Installation
+------------
+
+You can install *gRPC Access Log* via pip_ from PyPI_:
+
+.. code:: console
+
+   $ pip install grpc-accesslog
+
+
+Usage
+-----
+
+Please see the `Reference <Usage_>`_ for details.
+
+
+Contributing
+------------
+
+Contributions are very welcome.
+To learn more, see the `Contributor Guide`_.
+
+
+License
+-------
+
+Distributed under the terms of the `MIT license`_,
+*gRPC Access Log* is free and open source software.
+
+
+Issues
+------
+
+If you encounter any problems,
+please `file an issue`_ along with a detailed description.
+
+
+Credits
+-------
+
+This project was generated from `@cjolowicz`_'s `Hypermodern Python Cookiecutter`_ template.
+
+.. _@cjolowicz: https://github.com/cjolowicz
+.. _Cookiecutter: https://github.com/audreyr/cookiecutter
+.. _MIT license: https://opensource.org/licenses/MIT
+.. _PyPI: https://pypi.org/
+.. _Hypermodern Python Cookiecutter: https://github.com/cjolowicz/cookiecutter-hypermodern-python
+.. _file an issue: https://github.com/villainy/grpc-accesslog/issues
+.. _pip: https://pip.pypa.io/
+.. github-only
+.. _Contributor Guide: https://grpc-accesslog.readthedocs.io/en/latest/contributing.html
+.. _Usage: https://grpc-accesslog.readthedocs.io/en/latest/usage.html
 
-setup(**setup_kwargs)
```

