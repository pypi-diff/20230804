# Comparing `tmp/protool-1.1.2.tar.gz` & `tmp/protool-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protool-1.1.2.tar", max compression
+gzip compressed data, was "protool-2.0.0.tar", max compression
```

## Comparing `protool-1.1.2.tar` & `protool-2.0.0.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1095 2023-02-27 13:41:12.679211 protool-1.1.2/LICENSE
--rw-r--r--   0        0        0     2146 2023-02-27 13:41:12.679389 protool-1.1.2/README.md
--rwxr-xr-x   0        0        0     8042 2023-02-27 13:41:12.680662 protool-1.1.2/protool/__init__.py
--rwxr-xr-x   0        0        0     6238 2023-02-27 13:41:12.680891 protool-1.1.2/protool/command_line.py
--rw-r--r--   0        0        0     1034 2023-02-27 13:41:32.751354 protool-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     2982 1970-01-01 00:00:00.000000 protool-1.1.2/setup.py
--rw-r--r--   0        0        0     3233 1970-01-01 00:00:00.000000 protool-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1095 2023-08-04 06:51:43.461586 protool-2.0.0/LICENSE
+-rw-r--r--   0        0        0     2146 2023-08-04 06:51:43.461586 protool-2.0.0/README.md
+-rwxr-xr-x   0        0        0     8013 2023-08-04 06:51:43.465586 protool-2.0.0/protool/__init__.py
+-rwxr-xr-x   0        0        0     6238 2023-08-04 06:51:43.465586 protool-2.0.0/protool/command_line.py
+-rw-r--r--   0        0        0     1202 2023-08-04 06:51:43.465586 protool-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3139 1970-01-01 00:00:00.000000 protool-2.0.0/PKG-INFO
```

### Comparing `protool-1.1.2/LICENSE` & `protool-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `protool-1.1.2/README.md` & `protool-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `protool-1.1.2/protool/__init__.py` & `protool-2.0.0/protool/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 import datetime
 import os
 import plistlib
 import shutil
 import subprocess
 import sys
 import tempfile
-from typing import Any, cast, Dict, Iterable, List, Optional
-import OpenSSL
+from typing import Any, cast, Dict, List, Optional
+from OpenSSL import crypto
 
 
 class ProvisioningType(Enum):
     """Enum representing the type of provisioning profile."""
 
     IOS_DEVELOPMENT = 1
     APP_STORE_DISTRIBUTION = 3
@@ -62,24 +62,24 @@
             return ProvisioningType.APP_STORE_DISTRIBUTION
 
         if self.entitlements.get("get-task-allow") and self.provisioned_devices:
             return ProvisioningType.IOS_DEVELOPMENT
 
         raise Exception("Unable to determine provisioning profile type")
 
-    def developer_certificates(self) -> List[OpenSSL.crypto.X509]:
+    def developer_certificates(self) -> List[crypto.X509]:
         """Returns developer certificates as a list of PyOpenSSL X509."""
-        dev_certs: List[OpenSSL.crypto.X509] = []
+        dev_certs: List[crypto.X509] = []
         raw_cert_items: List[str] = cast(
             List[str], self._contents.get("DeveloperCertificates", [])
         )
 
         for cert_item in raw_cert_items:
-            loaded_cert: OpenSSL.crypto.X509 = OpenSSL.crypto.load_certificate(
-                OpenSSL.crypto.FILETYPE_ASN1, cert_item
+            loaded_cert: crypto.X509 = crypto.load_certificate(
+                crypto.FILETYPE_ASN1, cert_item.encode()
             )
             dev_certs.append(loaded_cert)
 
         return dev_certs
 
     def __init__(self, file_path: str, *, sort_keys: bool = True) -> None:
         self.file_path = os.path.abspath(file_path)
```

### Comparing `protool-1.1.2/protool/command_line.py` & `protool-2.0.0/protool/command_line.py`

 * *Files identical despite different names*

### Comparing `protool-1.1.2/pyproject.toml` & `protool-2.0.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "protool"
-version = "1.1.2"
+version = "2.0.0"
 description = "A tool for dealing with provisioning profiles"
 
 license = "MIT"
 
 authors = [
     "Dale Myers <dalemy@microsoft.com>"
 ]
@@ -18,29 +18,33 @@
 
 classifiers = [
     'Development Status :: 3 - Alpha',
     'Environment :: Console',
     'Environment :: MacOS X',
     'Intended Audience :: Developers',
     'Programming Language :: Python :: 3',
-    'Programming Language :: Python :: 3.7',
+    'Programming Language :: Python :: 3.8',
+    'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
     'Topic :: Software Development',
     'Topic :: Utilities'
 ]
 
 [tool.poetry.scripts]
 protool = 'protool:command_line.run'
 
 [tool.poetry.dependencies]
-python = "^3.7.2"
-pyOpenSSL =">=21.0.0"
+python = "^3.8"
+pyOpenSSL ="^23.2.0"
 
 [tool.poetry.dev-dependencies]
-black = "=23.1.0"
-mypy = "=1.0.1"
-pylint = "=2.16.2"
-pytest = "=7.2.1"
-pytest-cov = "=4.0.0"
+black = "^23.7.0"
+mypy = "^1.4.1"
+pylint = "^2.17.5"
+pytest = "^7.4.0"
+pytest-cov = "^4.1.0"
+types-pyOpenSSL = "^23.2.0.2"
 
 [build-system]
-requires = ["poetry>=0.12"]
-build-backend = "poetry.masonry.api"
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `protool-1.1.2/setup.py` & `protool-2.0.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,87 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: protool
+Version: 2.0.0
+Summary: A tool for dealing with provisioning profiles
+Home-page: https://github.com/Microsoft/protool
+License: MIT
+Keywords: provisioning,profiles,apple,ios,xcode,mobileprovision
+Author: Dale Myers
+Author-email: dalemy@microsoft.com
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Console
+Classifier: Environment :: MacOS X
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development
+Classifier: Topic :: Utilities
+Requires-Dist: pyOpenSSL (>=23.2.0,<24.0.0)
+Project-URL: Repository, https://github.com/Microsoft/protool
+Description-Content-Type: text/markdown
 
-packages = \
-['protool']
+# protool 
 
-package_data = \
-{'': ['*']}
+[![PyPi Version](https://img.shields.io/pypi/v/protool.svg)](https://pypi.org/project/protool/)
+[![License](https://img.shields.io/pypi/l/protool.svg)](https://github.com/Microsoft/protool/blob/master/LICENSE)
 
-install_requires = \
-['pyOpenSSL>=21.0.0']
-
-entry_points = \
-{'console_scripts': ['protool = protool:command_line.run']}
-
-setup_kwargs = {
-    'name': 'protool',
-    'version': '1.1.2',
-    'description': 'A tool for dealing with provisioning profiles',
-    'long_description': '# protool \n\n[![PyPi Version](https://img.shields.io/pypi/v/protool.svg)](https://pypi.org/project/protool/)\n[![License](https://img.shields.io/pypi/l/protool.svg)](https://github.com/Microsoft/protool/blob/master/LICENSE)\n\nA tool for dealing with provisioning profiles.\n\nWhat can it do? \n\n* Read profiles as XML or as a dictionary\n* Read the values from the profile\n* Diff two profiles to see what has changed\n\n### Installation\n\n    pip install protool\n\n### Examples:\n\n    import protool\n    profile = protool.ProvisioningProfile("/path/to/profile")\n\n    # Get the diff of two profiles\n    diff = protool.diff("/path/to/first", "/path/to/second", tool_override="diff")\n\n    # Get the UUID of a profile\n    print profile.uuid\n\n    # Get the full XML of the profile\n    print profile.xml\n\n    # Get the parsed contents of the profile as a dictionary\n    print profile.contents()\n\n\nAlternatively, from the command line:\n\n    # Get the diff\n    protool diff --profiles /path/to/profile1 /path/to/profile2 --tool diff\n\n    # Get the UUID of a profile\n    protool read --profile /path/to/profile --key UUID\n\n    # Get the raw XML (identical to using `security cms -D -i /path/to/profile`)\n    protool decode --profile /path/to/profile\n\n\n# Contributing\n\nThis project welcomes contributions and suggestions.  Most contributions require you to agree to a\nContributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us\nthe rights to use your contribution. For details, visit https://cla.microsoft.com.\n\nWhen you submit a pull request, a CLA-bot will automatically determine whether you need to provide\na CLA and decorate the PR appropriately (e.g., label, comment). Simply follow the instructions\nprovided by the bot. You will only need to do this once across all repos using our CLA.\n\nThis project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).\nFor more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or\ncontact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.\n',
-    'author': 'Dale Myers',
-    'author_email': 'dalemy@microsoft.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/Microsoft/protool',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7.2,<4.0.0',
-}
+A tool for dealing with provisioning profiles.
 
+What can it do? 
+
+* Read profiles as XML or as a dictionary
+* Read the values from the profile
+* Diff two profiles to see what has changed
+
+### Installation
+
+    pip install protool
+
+### Examples:
+
+    import protool
+    profile = protool.ProvisioningProfile("/path/to/profile")
+
+    # Get the diff of two profiles
+    diff = protool.diff("/path/to/first", "/path/to/second", tool_override="diff")
+
+    # Get the UUID of a profile
+    print profile.uuid
+
+    # Get the full XML of the profile
+    print profile.xml
+
+    # Get the parsed contents of the profile as a dictionary
+    print profile.contents()
+
+
+Alternatively, from the command line:
+
+    # Get the diff
+    protool diff --profiles /path/to/profile1 /path/to/profile2 --tool diff
+
+    # Get the UUID of a profile
+    protool read --profile /path/to/profile --key UUID
+
+    # Get the raw XML (identical to using `security cms -D -i /path/to/profile`)
+    protool decode --profile /path/to/profile
+
+
+# Contributing
+
+This project welcomes contributions and suggestions.  Most contributions require you to agree to a
+Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
+the rights to use your contribution. For details, visit https://cla.microsoft.com.
+
+When you submit a pull request, a CLA-bot will automatically determine whether you need to provide
+a CLA and decorate the PR appropriately (e.g., label, comment). Simply follow the instructions
+provided by the bot. You will only need to do this once across all repos using our CLA.
+
+This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
+For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
+contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.
 
-setup(**setup_kwargs)
```

