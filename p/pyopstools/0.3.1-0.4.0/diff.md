# Comparing `tmp/pyopstools-0.3.1.tar.gz` & `tmp/pyopstools-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyopstools-0.3.1.tar", last modified: Thu Mar  9 19:53:08 2023, max compression
+gzip compressed data, was "pyopstools-0.4.0.tar", last modified: Fri Aug  4 11:47:20 2023, max compression
```

## Comparing `pyopstools-0.3.1.tar` & `pyopstools-0.4.0.tar`

### file list

```diff
@@ -1,29 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-03-09 19:53:08.622785 pyopstools-0.3.1/
--rw-rw-rw-   0        0        0     1105 2023-01-21 11:35:27.000000 pyopstools-0.3.1/LICENSE
--rw-rw-rw-   0        0        0      119 2023-01-21 21:11:00.000000 pyopstools-0.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2172 2023-03-09 19:53:08.622785 pyopstools-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     1091 2023-01-22 12:34:15.000000 pyopstools-0.3.1/README.md
--rw-rw-rw-   0        0        0      348 2023-01-21 22:24:25.000000 pyopstools-0.3.1/configuration.sample.json
--rw-rw-rw-   0        0        0       98 2023-01-21 20:50:37.000000 pyopstools-0.3.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-09 19:53:08.622785 pyopstools-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1617 2023-03-09 19:06:49.000000 pyopstools-0.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-09 19:53:08.592720 pyopstools-0.3.1/src/
-drwxrwxrwx   0        0        0        0 2023-03-09 19:53:08.610805 pyopstools-0.3.1/src/apitester/
--rw-rw-rw-   0        0        0        0 2023-01-22 15:03:39.000000 pyopstools-0.3.1/src/apitester/__init__.py
--rw-rw-rw-   0        0        0     4138 2023-03-08 18:16:17.000000 pyopstools-0.3.1/src/apitester/api_request.py
--rw-rw-rw-   0        0        0     3542 2023-03-09 19:50:33.000000 pyopstools-0.3.1/src/apitester/api_tester.py
--rw-rw-rw-   0        0        0     1484 2023-03-08 18:16:17.000000 pyopstools-0.3.1/src/apitester/app_logger.py
--rw-rw-rw-   0        0        0     1435 2023-03-08 18:16:17.000000 pyopstools-0.3.1/src/apitester/custom_auth_token.py
-drwxrwxrwx   0        0        0        0 2023-03-09 19:53:08.615784 pyopstools-0.3.1/src/pyopstools.egg-info/
--rw-rw-rw-   0        0        0     2172 2023-03-09 19:53:08.000000 pyopstools-0.3.1/src/pyopstools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      558 2023-03-09 19:53:08.000000 pyopstools-0.3.1/src/pyopstools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-09 19:53:08.000000 pyopstools-0.3.1/src/pyopstools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-03-09 19:53:08.000000 pyopstools-0.3.1/src/pyopstools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       56 2023-03-09 19:53:08.000000 pyopstools-0.3.1/src/pyopstools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-03-09 19:53:08.000000 pyopstools-0.3.1/src/pyopstools.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-09 19:53:08.617785 pyopstools-0.3.1/src/tools/
--rw-rw-rw-   0        0        0       47 2023-03-09 19:26:42.000000 pyopstools-0.3.1/src/tools/__init__.py
--rw-rw-rw-   0        0        0      281 2023-03-09 19:46:05.000000 pyopstools-0.3.1/src/tools/custom_decorators.py
--rw-rw-rw-   0        0        0     2964 2023-03-09 19:51:42.000000 pyopstools-0.3.1/src/tools/main.py
-drwxrwxrwx   0        0        0        0 2023-03-09 19:53:08.621805 pyopstools-0.3.1/tests/
--rw-rw-rw-   0        0        0     4174 2023-01-21 21:14:52.000000 pyopstools-0.3.1/tests/test_custom_auth_token.py
+drwxrwxrwx   0        0        0        0 2023-08-04 11:47:20.847558 pyopstools-0.4.0/
+-rw-rw-rw-   0        0        0     1105 2023-01-23 09:18:35.000000 pyopstools-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0      124 2023-01-23 09:18:35.000000 pyopstools-0.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2213 2023-08-04 11:47:20.845650 pyopstools-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1222 2023-08-03 10:45:45.000000 pyopstools-0.4.0/README.md
+-rw-rw-rw-   0        0        0      364 2023-01-23 09:18:35.000000 pyopstools-0.4.0/configuration.sample.json
+-rw-rw-rw-   0        0        0      101 2023-08-03 15:47:48.000000 pyopstools-0.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-04 11:47:20.848605 pyopstools-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1700 2023-08-03 15:47:56.000000 pyopstools-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 11:47:20.594600 pyopstools-0.4.0/src/
+drwxrwxrwx   0        0        0        0 2023-08-04 11:47:20.648042 pyopstools-0.4.0/src/apitester/
+-rw-rw-rw-   0        0        0        0 2023-01-23 09:18:35.000000 pyopstools-0.4.0/src/apitester/__init__.py
+-rw-rw-rw-   0        0        0     4000 2023-08-04 08:37:07.000000 pyopstools-0.4.0/src/apitester/api_request.py
+-rw-rw-rw-   0        0        0     3377 2023-08-04 08:21:59.000000 pyopstools-0.4.0/src/apitester/api_tester.py
+-rw-rw-rw-   0        0        0     1405 2023-03-01 10:55:33.000000 pyopstools-0.4.0/src/apitester/custom_auth_token.py
+drwxrwxrwx   0        0        0        0 2023-08-04 11:47:20.663251 pyopstools-0.4.0/src/fileencoding/
+-rw-rw-rw-   0        0        0        0 2023-01-23 09:18:35.000000 pyopstools-0.4.0/src/fileencoding/__init__.py
+-rw-rw-rw-   0        0        0     3739 2023-08-04 11:45:58.000000 pyopstools-0.4.0/src/fileencoding/file_encoding.py
+drwxrwxrwx   0        0        0        0 2023-08-04 11:47:20.715835 pyopstools-0.4.0/src/helpers/
+-rw-rw-rw-   0        0        0        0 2023-08-04 08:12:45.000000 pyopstools-0.4.0/src/helpers/__init__.py
+-rw-rw-rw-   0        0        0     1494 2023-08-04 08:12:52.000000 pyopstools-0.4.0/src/helpers/app_logger.py
+-rw-rw-rw-   0        0        0      557 2023-08-04 08:30:59.000000 pyopstools-0.4.0/src/helpers/dict_helpers.py
+-rw-rw-rw-   0        0        0      178 2023-08-04 08:17:29.000000 pyopstools-0.4.0/src/helpers/path_helpers.py
+drwxrwxrwx   0        0        0        0 2023-08-04 11:47:20.777913 pyopstools-0.4.0/src/pyopstools.egg-info/
+-rw-rw-rw-   0        0        0     2213 2023-08-04 11:47:20.000000 pyopstools-0.4.0/src/pyopstools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      699 2023-08-04 11:47:20.000000 pyopstools-0.4.0/src/pyopstools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 11:47:20.000000 pyopstools-0.4.0/src/pyopstools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-08-04 11:47:20.000000 pyopstools-0.4.0/src/pyopstools.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       75 2023-08-04 11:47:20.000000 pyopstools-0.4.0/src/pyopstools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       37 2023-08-04 11:47:20.000000 pyopstools-0.4.0/src/pyopstools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-04 11:47:20.821894 pyopstools-0.4.0/src/tools/
+-rw-rw-rw-   0        0        0       49 2023-08-03 15:48:56.000000 pyopstools-0.4.0/src/tools/__init__.py
+-rw-rw-rw-   0        0        0      293 2023-08-03 10:26:24.000000 pyopstools-0.4.0/src/tools/custom_decorators.py
+-rw-rw-rw-   0        0        0     4874 2023-08-04 11:44:15.000000 pyopstools-0.4.0/src/tools/main.py
+drwxrwxrwx   0        0        0        0 2023-08-04 11:47:20.837784 pyopstools-0.4.0/tests/
+-rw-rw-rw-   0        0        0     4174 2023-01-23 09:18:35.000000 pyopstools-0.4.0/tests/test_custom_auth_token.py
```

### Comparing `pyopstools-0.3.1/LICENSE` & `pyopstools-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyopstools-0.3.1/PKG-INFO` & `pyopstools-0.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyopstools
-Version: 0.3.1
+Version: 0.4.0
 Summary: DevOps CLI tools
 Home-page: https://github.com/adeotek/pyopstools
 Author: George Benjamin-Schonberger
 Author-email: <george.benjamin@gmail.com>
 Keywords: ops,api,tester,tools
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -29,14 +29,15 @@
 ## Description
 
 A collection of DevOps CLI tools written in Python
 
 ## Available tools
 
 - `apitester` - A simple API tester where the requests are configured in a JSON file (see `configuration.sample.json` sample configuration)
+- `encodings` - File encoding converter
 
 ## Setup
 
 ### Install `venv` module
 
 ```powershell
 pip3.9 install virtualenv
```

### Comparing `pyopstools-0.3.1/README.md` & `pyopstools-0.4.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,90 +1,91 @@
-# Python DevOps Tools
-
-## Description
-
-A collection of DevOps CLI tools written in Python
-
-## Available tools
-
-- `apitester` - A simple API tester where the requests are configured in a JSON file (see `configuration.sample.json` sample configuration)
-
-## Setup
-
-### Install `venv` module
-
-```powershell
-pip3.9 install virtualenv
-```
-
-### Create environment
-
-```powershell
-# cd project_path
-python3.9 -m venv env
-```
-
-### Activate environment
-
-#### Windows
-
-```powershell
-.\env\Scripts\Activate.ps1
-```
-
-#### Linux
-
-```bash
-source env/bin/activate
-```
-
-### Upgrade `pip`
-
-```powershell
-python -m pip install --upgrade pip
-```
-
-### Deactivate environment
-
-```powershell
-deactivate
-```
-
-## Install tool from source
-
-### For development
-
-```powershell
-python -m pip install --editable .
-```
-
-### For usage only
-
-```powershell
-python -m pip install .
-```
-
-## Publish to PyPi.org
-
-### Prerequisite
-
-```powershell
-python -m pip install build twine
-```
-
-### Build
-
-```powershell
-python -m build
-```
-
-### Check
-
-```powershell
-twine check dist/*
-```
-
-### Upload
-
-```powershell
-twine upload dist/*
-```
+# Python DevOps Tools
+
+## Description
+
+A collection of DevOps CLI tools written in Python
+
+## Available tools
+
+- `apitester` - A simple API tester where the requests are configured in a JSON file (see `configuration.sample.json` sample configuration)
+- `encodings` - File encoding converter
+
+## Setup
+
+### Install `venv` module
+
+```powershell
+pip3.9 install virtualenv
+```
+
+### Create environment
+
+```powershell
+# cd project_path
+python3.9 -m venv env
+```
+
+### Activate environment
+
+#### Windows
+
+```powershell
+.\env\Scripts\Activate.ps1
+```
+
+#### Linux
+
+```bash
+source env/bin/activate
+```
+
+### Upgrade `pip`
+
+```powershell
+python -m pip install --upgrade pip
+```
+
+### Deactivate environment
+
+```powershell
+deactivate
+```
+
+## Install tool from source
+
+### For development
+
+```powershell
+python -m pip install --editable .
+```
+
+### For usage only
+
+```powershell
+python -m pip install .
+```
+
+## Publish to PyPi.org
+
+### Prerequisite
+
+```powershell
+python -m pip install build twine
+```
+
+### Build
+
+```powershell
+python -m build
+```
+
+### Check
+
+```powershell
+twine check dist/*
+```
+
+### Upload
+
+```powershell
+twine upload dist/*
+```
```

### Comparing `pyopstools-0.3.1/setup.py` & `pyopstools-0.4.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,52 +1,53 @@
-#!/usr/bin/env python
-import os
-
-from setuptools import setup, find_packages
-
-this_directory = os.path.abspath(os.path.dirname(__file__))
-with open(os.path.join(this_directory, 'README.md'), encoding='utf-8') as f:
-    long_description = f.read()
-
-setup(
-    name='pyopstools',
-    version="0.3.1",
-    author='George Benjamin-Schonberger',
-    author_email='<george.benjamin@gmail.com>',
-    description='DevOps CLI tools',
-    keywords=['ops', 'api', 'tester', 'tools'],
-    long_description_content_type='text/markdown',
-    long_description=long_description,
-    url='https://github.com/adeotek/pyopstools',
-    package_dir={'': 'src'},
-    packages=find_packages(where='src'),
-    python_requires='>=3.7',
-    install_requires=[
-        'colorama',
-        'termcolor',
-        'requests',
-        'click'
-    ],
-    extras_require={
-        'dev': ['check-manifest'],
-    },
-    entry_points={
-        'console_scripts': [
-            'pyopstools=tools:cli',
-        ],
-    },
-    classifiers=[
-        'Environment :: Console',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
-        'Development Status :: 3 - Alpha',
-        'Programming Language :: Python :: 3 :: Only',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
-        'Operating System :: Unix',
-        'Operating System :: MacOS :: MacOS X',
-        'Operating System :: Microsoft :: Windows',
-    ]
-)
+#!/usr/bin/env python
+import os
+
+from setuptools import setup, find_packages
+
+this_directory = os.path.abspath(os.path.dirname(__file__))
+with open(os.path.join(this_directory, 'README.md'), encoding='utf-8') as f:
+    long_description = f.read()
+
+setup(
+    name='pyopstools',
+    version="0.4.0",
+    author='George Benjamin-Schonberger',
+    author_email='<george.benjamin@gmail.com>',
+    description='DevOps CLI tools',
+    keywords=['ops', 'api', 'tester', 'tools'],
+    long_description_content_type='text/markdown',
+    long_description=long_description,
+    url='https://github.com/adeotek/pyopstools',
+    package_dir={'': 'src'},
+    packages=find_packages(where='src'),
+    python_requires='>=3.7',
+    install_requires=[
+        'colorama',
+        'termcolor',
+        'requests',
+        'click',
+        'charset-normalizer'
+    ],
+    extras_require={
+        'dev': ['check-manifest'],
+    },
+    entry_points={
+        'console_scripts': [
+            'pyopstools=tools:cli',
+        ],
+    },
+    classifiers=[
+        'Environment :: Console',
+        'Intended Audience :: Developers',
+        'License :: OSI Approved :: MIT License',
+        'Development Status :: 3 - Alpha',
+        'Programming Language :: Python :: 3 :: Only',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Operating System :: Unix',
+        'Operating System :: MacOS :: MacOS X',
+        'Operating System :: Microsoft :: Windows',
+    ]
+)
```

### Comparing `pyopstools-0.3.1/src/apitester/api_request.py` & `pyopstools-0.4.0/src/apitester/api_request.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,101 +1,101 @@
-import json
-from typing import Optional
-
-from urllib3 import disable_warnings
-from urllib3.exceptions import InsecureRequestWarning
-from requests import request as requests_request
-from requests.exceptions import ConnectionError
-import apitester.app_logger as app_logger
-
-disable_warnings(InsecureRequestWarning)
-
-
-class ApiRequest:
-    __logger: app_logger.Logger
-    verb: str
-    url: str
-    headers: dict
-    sslVerify: bool
-    payload = None
-    response = None
-    output = None
-
-    def __init__(self, verb: str, url: str, payload=None, headers=None, output=None, ssl_verify: bool = True,
-                 logger=None) -> None:
-        if headers is None:
-            headers = {}
-        if isinstance(logger, app_logger.Logger):
-            self.__logger = logger
-        else:
-            self.__logger = app_logger.Logger(False)
-        self.verb = verb
-        self.url = url
-        self.headers = headers
-        self.output = output
-        self.sslVerify = ssl_verify
-        if 'Content-Type' not in self.headers.keys():
-            self.set_header('Content-Type', 'application/json')
-        if 'User-Agent' not in self.headers.keys():
-            self.set_header('User-Agent', 'Python-API-Tester')
-        self.payload = payload
-
-    def set_header(self, key, value):
-        self.headers[key] = value
-        return self
-
-    def print_response(self) -> None:
-        if self.response is None:
-            self.__logger.clog(('No response!', 'red'))
-            if isinstance(self.output, str) and self.output != '':
-                output_file = open(self.output, "w")
-                output_file.write('')
-                output_file.close()
-        else:
-            try:
-                json_output = self.response.json()
-                output = json.dumps(json_output, indent=4)
-            except (ValueError, json.decoder.JSONDecodeError):
-                output = self.response.text
-            if isinstance(self.output, str) and self.output != '':
-                output_file = open(self.output, "w")
-                output_file.write(output)
-                output_file.close()
-            else:
-                self.__logger.log(output)
-
-    def execute(self, print_response: bool = True):
-        self.__logger.cdebug(('Request ', 'yellow'), (self.verb, 'cyan'), ('(', 'yellow'), (self.url, 'cyan'),
-                             (')...', 'yellow'))
-        self.__logger.cdebug(('Headers:', 'yellow'), (json.dumps(self.headers, indent=4), 'cyan'))
-        if self.verb == "GET":
-            body = None
-        else:
-            if isinstance(self.payload, str):
-                body = self.payload
-                self.__logger.cdebug(('Body:', 'yellow'), (self.payload, 'cyan'))
-            else:
-                body = json.dumps(self.payload)
-                self.__logger.cdebug(('Body:', 'yellow'), (json.dumps(self.payload, indent=4), 'cyan'))
-        try:
-            self.response = requests_request(self.verb, self.url, headers=self.headers, verify=self.sslVerify,
-                                             data=body)
-            if self.response.status_code == 200:
-                self.__logger.clog(('Response: ', 'green'), (self.verb, 'cyan'), '(', (self.url, 'cyan'),
-                                   ') Status code: [', (self.response.status_code, 'green'), ']')
-            else:
-                self.__logger.clog(('Response: ', 'red'), (self.verb, 'cyan'), '(', (self.url, 'cyan'),
-                                   ') Status code: [', (self.response.status_code, 'magenta'), ']')
-        except (ValueError, ConnectionError) as err:
-            self.response = None
-            self.__logger.clog(('ERROR: [', 'red'), (str(err.errno), 'magenta'), ('] ' + str(err), 'red'))
-        if print_response:
-            self.print_response()
-        return self
-
-    def __get_response_code(self) -> Optional[int]:
-        if self.response is None:
-            return None
-        else:
-            return self.response.status_code
-
-    response_code = property(__get_response_code)
+import json
+from typing import Optional
+
+from urllib3 import disable_warnings
+from urllib3.exceptions import InsecureRequestWarning
+from requests import request as requests_request
+from requests.exceptions import ConnectionError
+from helpers.app_logger import Logger
+
+disable_warnings(InsecureRequestWarning)
+
+
+class ApiRequest:
+    __logger: Logger
+    verb: str
+    url: str
+    headers: dict
+    sslVerify: bool
+    payload = None
+    response = None
+    output = None
+
+    def __init__(self, verb: str, url: str, payload=None, headers=None, output=None, ssl_verify: bool = True,
+                 logger=None) -> None:
+        if headers is None:
+            headers = {}
+        if isinstance(logger, Logger):
+            self.__logger = logger
+        else:
+            self.__logger = Logger(False)
+        self.verb = verb
+        self.url = url
+        self.headers = headers
+        self.output = output
+        self.sslVerify = ssl_verify
+        if 'Content-Type' not in self.headers.keys():
+            self.set_header('Content-Type', 'application/json')
+        if 'User-Agent' not in self.headers.keys():
+            self.set_header('User-Agent', 'Python-API-Tester')
+        self.payload = payload
+
+    def set_header(self, key, value):
+        self.headers[key] = value
+        return self
+
+    def print_response(self) -> None:
+        if self.response is None:
+            self.__logger.clog(('No response!', 'red'))
+            if isinstance(self.output, str) and self.output != '':
+                output_file = open(self.output, "w")
+                output_file.write('')
+                output_file.close()
+        else:
+            try:
+                json_output = self.response.json()
+                output = json.dumps(json_output, indent=4)
+            except (ValueError, json.decoder.JSONDecodeError):
+                output = self.response.text
+            if isinstance(self.output, str) and self.output != '':
+                output_file = open(self.output, "w")
+                output_file.write(output)
+                output_file.close()
+            else:
+                self.__logger.log(output)
+
+    def execute(self, print_response: bool = True):
+        self.__logger.cdebug(('Request ', 'yellow'), (self.verb, 'cyan'), ('(', 'yellow'), (self.url, 'cyan'),
+                             (')...', 'yellow'))
+        self.__logger.cdebug(('Headers:', 'yellow'), (json.dumps(self.headers, indent=4), 'cyan'))
+        if self.verb == "GET":
+            body = None
+        else:
+            if isinstance(self.payload, str):
+                body = self.payload
+                self.__logger.cdebug(('Body:', 'yellow'), (self.payload, 'cyan'))
+            else:
+                body = json.dumps(self.payload)
+                self.__logger.cdebug(('Body:', 'yellow'), (json.dumps(self.payload, indent=4), 'cyan'))
+        try:
+            self.response = requests_request(self.verb, self.url, headers=self.headers, verify=self.sslVerify,
+                                             data=body)
+            if self.response.status_code == 200:
+                self.__logger.clog(('Response: ', 'green'), (self.verb, 'cyan'), '(', (self.url, 'cyan'),
+                                   ') Status code: [', (self.response.status_code, 'green'), ']')
+            else:
+                self.__logger.clog(('Response: ', 'red'), (self.verb, 'cyan'), '(', (self.url, 'cyan'),
+                                   ') Status code: [', (self.response.status_code, 'magenta'), ']')
+        except (ValueError, ConnectionError) as err:
+            self.response = None
+            self.__logger.clog(('ERROR: [', 'red'), (str(err.errno), 'magenta'), ('] ' + str(err), 'red'))
+        if print_response:
+            self.print_response()
+        return self
+
+    def __get_response_code(self) -> Optional[int]:
+        if self.response is None:
+            return None
+        else:
+            return self.response.status_code
+
+    response_code = property(__get_response_code)
```

### Comparing `pyopstools-0.3.1/src/apitester/api_tester.py` & `pyopstools-0.4.0/src/apitester/api_tester.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,104 +1,92 @@
-import os
-import json
-import apitester.custom_auth_token as custom_auth_token
-import apitester.app_logger as app_logger
-import apitester.api_request as api_request
-
-logger: app_logger.Logger
-configuration: dict
-
-
-def get_dict_attr(data: dict, key: str, default=None):
-    if key in data.keys():
-        return data[key]
-    else:
-        return default
-
-
-def get_full_path(input_path: str) -> str:
-    if os.path.isabs(input_path):
-        return input_path
-    else:
-        return os.path.join(os.getcwd(), input_path)
-
-
-def get_request_title(req: dict) -> tuple:
-    title = ['-']
-    group = get_dict_attr(req, 'Group', '')
-    if group != '':
-        title.append(' [')
-        title.append((group, 'blue'))
-        title.append('] ')
-    name = get_dict_attr(req, 'Name', '')
-    if name != '':
-        title.append((' ' + name, 'magenta'))
-    else:
-        title.append(('----', 'magenta'))
-    return tuple(title)
-
-
-def execute_request(req: dict) -> None:
-    global logger
-    if req['Verb'] not in ['GET', 'POST', 'PUT', 'PATCH', 'DELETE']:
-        logger.new_line() \
-            .clog(('Invalid verb `', 'red'), (req['Verb'], 'magenta'), ('` provided!', 'red')).new_line()
-        return
-    if 'Output' in req.keys() and isinstance(req['Output'], str) and req['Output'] != '':
-        output_file_name = get_full_path(req['Output'])
-    else:
-        output_file_name = None
-    request = api_request.ApiRequest(
-        verb=req['Verb'],
-        url=req['URL'],
-        headers=get_dict_attr(req, 'Headers', {}),
-        output=output_file_name,
-        ssl_verify=get_dict_attr(req, 'SSLVerify', True),
-        payload=get_dict_attr(req, 'Payload'),
-        logger=logger)
-    if get_dict_attr(req, 'UseCustomAuthToken', False):
-        token, expires_at = custom_auth_token.generate_token(req['CustomAuthToken']['SecretKey'],
-                                                             req['CustomAuthToken']['ClientId'],
-                                                             req['CustomAuthToken']['ServerId'])
-        logger.cdebug('Generated Auth Token will expire at: ', (str(expires_at), 'cyan'))
-        request.set_header('Authorization', 'Bearer ' + str(token))
-    request.execute(True)
-
-
-def init(config) -> bool:
-    global logger, configuration
-    # load configuration
-    config_file_name = get_full_path(config)
-    if not os.path.exists(config_file_name):
-        logger = app_logger.Logger()
-        logger.new_line()\
-            .clog(('No `', 'red'), ('configuration.json', 'magenta'), ('` file provided!', 'red')).new_line()
-        return False
-    config_file = open(config_file_name)
-    configuration = json.load(config_file)
-    config_file.close()
-    # initialize logger
-    logger = app_logger.Logger(configuration['Verbose'])
-    return True
-
-
-def run(config, version: str) -> None:
-    global logger, configuration
-    if not init(config):
-        return
-    logger.clog(('Starting API tester ', 'white'), ('v' + version, 'green'), (' ...', 'white')).new_line()
-    for req in configuration['Requests']:
-        if get_dict_attr(req, 'IsActive', True):
-            logger.new_line().clog(*get_request_title(req))
-            execute_request(req)
-    logger.new_line().clog(('DONE!', 'green'))
-
-
-def direct_run(req: dict, version: str) -> None:
-    global logger
-    logger = app_logger.Logger()
-    logger.clog(('Starting API tester ', 'white'), ('v' + version, 'green'), (' ...', 'white')).new_line()
-    execute_request(req)
-
-
-if __name__ == '__main__':
-    run('configuration.json')
+import os
+import json
+from helpers.app_logger import Logger
+from helpers.path_helpers import get_full_path
+from helpers.dict_helpers import get_dict_attr
+import apitester.custom_auth_token as custom_auth_token
+import apitester.api_request as api_request
+
+logger: Logger
+configuration: dict
+
+
+def get_request_title(req: dict) -> tuple:
+    title = ['-']
+    group = get_dict_attr(req, 'Group', '')
+    if group != '':
+        title.append(' [')
+        title.append((group, 'blue'))
+        title.append('] ')
+    name = get_dict_attr(req, 'Name', '')
+    if name != '':
+        title.append((' ' + name, 'magenta'))
+    else:
+        title.append(('----', 'magenta'))
+    return tuple(title)
+
+
+def execute_request(req: dict) -> None:
+    global logger
+    if req['Verb'] not in ['GET', 'POST', 'PUT', 'PATCH', 'DELETE']:
+        logger.new_line() \
+            .clog(('Invalid verb `', 'red'), (req['Verb'], 'magenta'), ('` provided!', 'red')).new_line()
+        return
+    if 'Output' in req.keys() and isinstance(req['Output'], str) and req['Output'] != '':
+        output_file_name = get_full_path(req['Output'])
+    else:
+        output_file_name = None
+    request = api_request.ApiRequest(
+        verb=req['Verb'],
+        url=req['URL'],
+        headers=get_dict_attr(req, 'Headers', {}),
+        output=output_file_name,
+        ssl_verify=get_dict_attr(req, 'SSLVerify', True),
+        payload=get_dict_attr(req, 'Payload'),
+        logger=logger)
+    if get_dict_attr(req, 'UseCustomAuthToken', False):
+        token, expires_at = custom_auth_token.generate_token(req['CustomAuthToken']['SecretKey'],
+                                                             req['CustomAuthToken']['ClientId'],
+                                                             req['CustomAuthToken']['ServerId'])
+        logger.cdebug('Generated Auth Token will expire at: ', (str(expires_at), 'cyan'))
+        request.set_header('Authorization', 'Bearer ' + str(token))
+    request.execute(True)
+
+
+def init(config) -> bool:
+    global logger, configuration
+    # load configuration
+    config_file_name = get_full_path(config)
+    if not os.path.exists(config_file_name):
+        logger = Logger()
+        logger.new_line()\
+            .clog(('No `', 'red'), ('configuration.json', 'magenta'), ('` file provided!', 'red')).new_line()
+        return False
+    config_file = open(config_file_name)
+    configuration = json.load(config_file)
+    config_file.close()
+    # initialize logger
+    logger = Logger(configuration['Verbose'])
+    return True
+
+
+def run(config, version: str) -> None:
+    global logger, configuration
+    if not init(config):
+        return
+    logger.clog(('Starting API tester ', 'white'), ('v' + version, 'green'), (' ...', 'white')).new_line()
+    for req in configuration['Requests']:
+        if get_dict_attr(req, 'IsActive', True):
+            logger.new_line().clog(*get_request_title(req))
+            execute_request(req)
+    logger.new_line().clog(('DONE!', 'green'))
+
+
+def direct_run(req: dict, version: str) -> None:
+    global logger
+    logger = Logger()
+    logger.clog(('Starting API tester ', 'white'), ('v' + version, 'green'), (' ...', 'white')).new_line()
+    execute_request(req)
+
+
+if __name__ == '__main__':
+    run('configuration.json', 'N/A')
```

### Comparing `pyopstools-0.3.1/src/apitester/app_logger.py` & `pyopstools-0.4.0/src/helpers/app_logger.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,55 +1,58 @@
-from colorama import just_fix_windows_console
-from typing import Any
-from termcolor import colored, cprint, COLORS
-
-just_fix_windows_console()
-
-
-class Logger:
-    __verbose = False
-
-    def __init__(self, verbose: bool = False) -> None:
-        self.__verbose = verbose
-
-    def set_verbose(self, value: bool):
-        self.__verbose = value
-        return self
-
-    def new_line(self):
-        print()
-        return self
-
-    def log(self, *values: object, **kwargs: Any):
-        print(*values, sep='', **kwargs)
-        return self
-
-    def debug(self, *values: object, **kwargs: Any):
-        if self.__verbose:
-            self.log(*values, **kwargs)
-        return self
-
-    def clog(self, *values: object, **kwargs: Any):
-        cvalues = []
-        for v in values:
-            if isinstance(v, tuple) and len(v) == 2 and isinstance(v[1], str) and v[1] in COLORS:
-                cvalues.append(colored(v[0], v[1]))
-            else:
-                cvalues.append(v)
-        self.log(*tuple(cvalues), **kwargs)
-        return self
-
-    def cdebug(self, *values: object, **kwargs: Any):
-        if self.__verbose:
-            self.clog(*values, **kwargs)
-        return self
-
-    def cprint(
-        self,
-        text: str,
-        color=None,
-        on_color=None,
-        attrs=None,
-        **kwargs: Any,
-    ):
-        cprint(text=text, color=color, on_color=on_color, attrs=attrs, **kwargs)
-        return self
+from colorama import just_fix_windows_console
+from typing import Any
+from termcolor import colored, cprint, COLORS
+
+just_fix_windows_console()
+
+
+class Logger:
+    __verbose = False
+
+    def __init__(self, verbose: bool = False) -> None:
+        self.__verbose = verbose
+
+    def set_verbose(self, value: bool):
+        self.__verbose = value
+        return self
+
+    def is_verbose(self) -> bool:
+        return self.__verbose
+
+    def new_line(self):
+        print()
+        return self
+
+    def log(self, *values: object, **kwargs: Any):
+        print(*values, sep='', **kwargs)
+        return self
+
+    def debug(self, *values: object, **kwargs: Any):
+        if self.__verbose:
+            self.log(*values, **kwargs)
+        return self
+
+    def clog(self, *values: object, **kwargs: Any):
+        cvalues = []
+        for v in values:
+            if isinstance(v, tuple) and len(v) == 2 and isinstance(v[1], str) and v[1] in COLORS:
+                cvalues.append(colored(v[0], v[1]))
+            else:
+                cvalues.append(v)
+        self.log(*tuple(cvalues), **kwargs)
+        return self
+
+    def cdebug(self, *values: object, **kwargs: Any):
+        if self.__verbose:
+            self.clog(*values, **kwargs)
+        return self
+
+    def cprint(
+        self,
+        text: str,
+        color=None,
+        on_color=None,
+        attrs=None,
+        **kwargs: Any,
+    ):
+        cprint(text=text, color=color, on_color=on_color, attrs=attrs, **kwargs)
+        return self
```

### Comparing `pyopstools-0.3.1/src/apitester/custom_auth_token.py` & `pyopstools-0.4.0/src/apitester/custom_auth_token.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-import hashlib
-from datetime import datetime, timedelta
-
-
-def generate_token(secret_key: str, client_id: str = '', server_id: str = '', validity: int = 10):
-    if secret_key == '':
-        raise ValueError('Invalid `secretKey`')
-    token_source = 'Sk:' + secret_key + '-Iss:' + server_id
-    token = hashlib.sha256(token_source.encode('ascii')).hexdigest()
-    expires_at = datetime.now() + timedelta(minutes=validity)
-    expires_at_token = expires_at.strftime('%Y-%m-%dT%H:%M:%S').encode('ascii').hex().lower()
-    return client_id + token + expires_at_token, expires_at
-
-
-def validate_token(token, secret_key: str, server_id: str = ''):
-    if not isinstance(token, str) or token == '' or len(token) < 102:
-        return False, None, 'Invalid token value/size!'
-    if not isinstance(secret_key, str) or secret_key == '':
-        return False, None, 'Invalid `secretKey` value!'
-    client_id = token[0:-102]
-    token_source = 'Sk:' + secret_key + '-Iss:' + server_id
-    check_hash = hashlib.sha256(token_source.encode('ascii')).hexdigest()
-    token_hash = token[-102:-38]
-    if check_hash.lower() != token_hash.lower():
-        return False, client_id, 'Invalid token!'
-    exp_date = datetime.strptime(bytes.fromhex(token[-38:]).decode(), '%Y-%m-%dT%H:%M:%S')
-    if exp_date > datetime.now():
-        return True, client_id, ''
-    else:
-        return False, client_id, 'Token has expired!'
+import hashlib
+from datetime import datetime, timedelta
+
+
+def generate_token(secret_key: str, client_id: str = '', server_id: str = '', validity: int = 10):
+    if secret_key == '':
+        raise ValueError('Invalid `secretKey`')
+    token_source = 'Sk:' + secret_key + '-Iss:' + server_id
+    token = hashlib.sha256(token_source.encode('ascii')).hexdigest()
+    expires_at = datetime.now() + timedelta(minutes=validity)
+    expires_at_token = expires_at.strftime('%Y-%m-%dT%H:%M:%S').encode('ascii').hex().lower()
+    return client_id + token + expires_at_token, expires_at
+
+
+def validate_token(token, secret_key: str, server_id: str = ''):
+    if not isinstance(token, str) or token == '' or len(token) < 102:
+        return False, None, 'Invalid token value/size!'
+    if not isinstance(secret_key, str) or secret_key == '':
+        return False, None, 'Invalid `secretKey` value!'
+    client_id = token[0:-102]
+    token_source = 'Sk:' + secret_key + '-Iss:' + server_id
+    check_hash = hashlib.sha256(token_source.encode('ascii')).hexdigest()
+    token_hash = token[-102:-38]
+    if check_hash.lower() != token_hash.lower():
+        return False, client_id, 'Invalid token!'
+    exp_date = datetime.strptime(bytes.fromhex(token[-38:]).decode(), '%Y-%m-%dT%H:%M:%S')
+    if exp_date > datetime.now():
+        return True, client_id, ''
+    else:
+        return False, client_id, 'Token has expired!'
```

### Comparing `pyopstools-0.3.1/src/pyopstools.egg-info/PKG-INFO` & `pyopstools-0.4.0/src/pyopstools.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyopstools
-Version: 0.3.1
+Version: 0.4.0
 Summary: DevOps CLI tools
 Home-page: https://github.com/adeotek/pyopstools
 Author: George Benjamin-Schonberger
 Author-email: <george.benjamin@gmail.com>
 Keywords: ops,api,tester,tools
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -29,14 +29,15 @@
 ## Description
 
 A collection of DevOps CLI tools written in Python
 
 ## Available tools
 
 - `apitester` - A simple API tester where the requests are configured in a JSON file (see `configuration.sample.json` sample configuration)
+- `encodings` - File encoding converter
 
 ## Setup
 
 ### Install `venv` module
 
 ```powershell
 pip3.9 install virtualenv
```

### Comparing `pyopstools-0.3.1/tests/test_custom_auth_token.py` & `pyopstools-0.4.0/tests/test_custom_auth_token.py`

 * *Files identical despite different names*

