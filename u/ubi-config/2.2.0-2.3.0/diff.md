# Comparing `tmp/ubi-config-2.2.0.tar.gz` & `tmp/ubi-config-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ubi-config-2.2.0.tar", last modified: Thu Oct 24 14:23:27 2019, max compression
+gzip compressed data, was "ubi-config-2.3.0.tar", last modified: Fri Aug  4 14:06:04 2023, max compression
```

## Comparing `ubi-config-2.2.0.tar` & `ubi-config-2.3.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-24 14:23:27.000000 ubi-config-2.2.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)       80 2019-10-24 14:22:51.000000 ubi-config-2.2.0/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)      249 2019-10-24 14:22:51.000000 ubi-config-2.2.0/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     3216 2019-10-24 14:23:27.000000 ubi-config-2.2.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1896 2019-10-24 14:22:51.000000 ubi-config-2.2.0/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-24 14:23:27.000000 ubi-config-2.2.0/ubiconfig/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1984 2019-10-24 14:22:51.000000 ubi-config-2.2.0/ubiconfig/ubi.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-24 14:23:27.000000 ubi-config-2.2.0/ubiconfig/_impl/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-24 14:23:27.000000 ubi-config-2.2.0/ubiconfig/_impl/loaders/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4656 2019-10-24 14:22:51.000000 ubi-config-2.2.0/ubiconfig/_impl/loaders/gitlab.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3687 2019-10-24 14:22:51.000000 ubi-config-2.2.0/ubiconfig/_impl/loaders/local.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      990 2019-10-24 14:22:51.000000 ubi-config-2.2.0/ubiconfig/_impl/loaders/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      142 2019-10-24 14:22:51.000000 ubi-config-2.2.0/ubiconfig/_impl/loaders/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-24 14:22:51.000000 ubi-config-2.2.0/ubiconfig/_impl/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-24 14:23:27.000000 ubi-config-2.2.0/ubiconfig/utils/
--rw-rw-r--   0 travis    (2000) travis    (2000)      496 2019-10-24 14:22:51.000000 ubi-config-2.2.0/ubiconfig/utils/config_validation.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-24 14:23:27.000000 ubi-config-2.2.0/ubiconfig/utils/api/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2323 2019-10-24 14:22:51.000000 ubi-config-2.2.0/ubiconfig/utils/api/gitlab.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-24 14:22:51.000000 ubi-config-2.2.0/ubiconfig/utils/api/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-10-24 14:22:51.000000 ubi-config-2.2.0/ubiconfig/utils/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2156 2019-10-24 14:22:51.000000 ubi-config-2.2.0/ubiconfig/utils/config_schema.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      260 2019-10-24 14:22:51.000000 ubi-config-2.2.0/ubiconfig/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-24 14:23:27.000000 ubi-config-2.2.0/ubiconfig/config_types/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2308 2019-10-24 14:22:51.000000 ubi-config-2.2.0/ubiconfig/config_types/content_sets.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1285 2019-10-24 14:22:51.000000 ubi-config-2.2.0/ubiconfig/config_types/modules.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2235 2019-10-24 14:22:51.000000 ubi-config-2.2.0/ubiconfig/config_types/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1331 2019-10-24 14:22:51.000000 ubi-config-2.2.0/ubiconfig/config_types/packages.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-24 14:23:27.000000 ubi-config-2.2.0/ubi_config.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3216 2019-10-24 14:23:27.000000 ubi-config-2.2.0/ubi_config.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-10-24 14:23:27.000000 ubi-config-2.2.0/ubi_config.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       10 2019-10-24 14:23:27.000000 ubi-config-2.2.0/ubi_config.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      744 2019-10-24 14:23:27.000000 ubi-config-2.2.0/ubi_config.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      116 2019-10-24 14:23:27.000000 ubi-config-2.2.0/ubi_config.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2019-10-24 14:23:27.000000 ubi-config-2.2.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)    35069 2019-10-24 14:22:51.000000 ubi-config-2.2.0/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     1519 2019-10-24 14:22:51.000000 ubi-config-2.2.0/CHANGELOG.md
--rw-rw-r--   0 travis    (2000) travis    (2000)     1492 2019-10-24 14:22:51.000000 ubi-config-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:06:04.277322 ubi-config-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-08-04 14:05:53.000000 ubi-config-2.3.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35069 2023-08-04 14:05:53.000000 ubi-config-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-04 14:05:53.000000 ubi-config-2.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-08-04 14:06:04.277322 ubi-config-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-08-04 14:05:53.000000 ubi-config-2.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-04 14:05:53.000000 ubi-config-2.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 14:06:04.277322 ubi-config-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-08-04 14:05:53.000000 ubi-config-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:06:04.273322 ubi-config-2.3.0/ubi_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-08-04 14:06:04.000000 ubi-config-2.3.0/ubi_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-08-04 14:06:04.000000 ubi-config-2.3.0/ubi_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 14:06:04.000000 ubi-config-2.3.0/ubi_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-04 14:06:04.000000 ubi-config-2.3.0/ubi_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-04 14:06:04.000000 ubi-config-2.3.0/ubi_config.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:06:04.273322 ubi-config-2.3.0/ubiconfig/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-08-04 14:05:53.000000 ubi-config-2.3.0/ubiconfig/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:06:04.273322 ubi-config-2.3.0/ubiconfig/_impl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 14:05:53.000000 ubi-config-2.3.0/ubiconfig/_impl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:06:04.277322 ubi-config-2.3.0/ubiconfig/_impl/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-08-04 14:05:53.000000 ubi-config-2.3.0/ubiconfig/_impl/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-08-04 14:05:53.000000 ubi-config-2.3.0/ubiconfig/_impl/loaders/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-08-04 14:05:53.000000 ubi-config-2.3.0/ubiconfig/_impl/loaders/gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-08-04 14:05:53.000000 ubi-config-2.3.0/ubiconfig/_impl/loaders/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:06:04.277322 ubi-config-2.3.0/ubiconfig/config_types/
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-08-04 14:05:53.000000 ubi-config-2.3.0/ubiconfig/config_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-08-04 14:05:53.000000 ubi-config-2.3.0/ubiconfig/config_types/content_sets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-08-04 14:05:53.000000 ubi-config-2.3.0/ubiconfig/config_types/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-08-04 14:05:53.000000 ubi-config-2.3.0/ubiconfig/config_types/packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-08-04 14:05:53.000000 ubi-config-2.3.0/ubiconfig/ubi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:06:04.277322 ubi-config-2.3.0/ubiconfig/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 14:05:53.000000 ubi-config-2.3.0/ubiconfig/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:06:04.277322 ubi-config-2.3.0/ubiconfig/utils/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 14:05:53.000000 ubi-config-2.3.0/ubiconfig/utils/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-08-04 14:05:53.000000 ubi-config-2.3.0/ubiconfig/utils/api/gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-08-04 14:05:53.000000 ubi-config-2.3.0/ubiconfig/utils/config_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-08-04 14:05:53.000000 ubi-config-2.3.0/ubiconfig/utils/config_validation.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ubi-config-2.2.0/PKG-INFO` & `ubi-config-2.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: ubi-config
-Version: 2.2.0
+Version: 2.3.0
 Summary: A Python Library for accessing Universal Base Image configuration
 Home-page: https://github.com/release-engineering/ubi-config
 Author: 
 Author-email: 
 License: GNU General Public License
 Project-URL: Documentation, https://release-engineering.github.io/ubi-config/
 Description: 
         
         A Python library for accessing Universal Base Image configuration
         
-        [![Build Status](https://travis-ci.org/release-engineering/ubi-config.svg?branch=master)](https://travis-ci.org/release-engineering/ubi-config)
-        [![Coverage Status](https://coveralls.io/repos/github/release-engineering/ubi-config/badge.svg?branch=master)](https://coveralls.io/github/release-engineering/ubi-config?branch=master)
+        [![Build Status](https://github.com/release-engineering/ubi-config/actions/workflows/tox-test.yml/badge.svg)](https://github.com/release-engineering/ubi-config/actions/workflows/tox-test.yml))
+        [![codecov](https://codecov.io/gh/release-engineering/ubi-config/branch/master/graph/badge.svg?token=fPG7EINR9O)](https://codecov.io/gh/release-engineering/ubi-config)
         [![Maintainability](https://api.codeclimate.com/v1/badges/c62407f84ad66135fa8d/maintainability)](https://codeclimate.com/github/release-engineering/ubi-config/maintainability)
         
         - [Source](https://github.com/release-engineering/ubi-config)
         - [Documentation](https://release-engineering.github.io/ubi-config/)
         - [PyPI](https://pypi.org/project/ubi-config)
         
         Installation
@@ -70,13 +70,11 @@
         (at your option) any later version.
         
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.6
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `ubi-config-2.2.0/README.md` & `ubi-config-2.3.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ubiconfig
 =========
 
 A Python library for accessing Universal Base Image configuration
 
-[![Build Status](https://travis-ci.org/release-engineering/ubi-config.svg?branch=master)](https://travis-ci.org/release-engineering/ubi-config)
-[![Coverage Status](https://coveralls.io/repos/github/release-engineering/ubi-config/badge.svg?branch=master)](https://coveralls.io/github/release-engineering/ubi-config?branch=master)
+[![Build Status](https://github.com/release-engineering/ubi-config/actions/workflows/tox-test.yml/badge.svg)](https://github.com/release-engineering/ubi-config/actions/workflows/tox-test.yml))
+[![codecov](https://codecov.io/gh/release-engineering/ubi-config/branch/master/graph/badge.svg?token=fPG7EINR9O)](https://codecov.io/gh/release-engineering/ubi-config)
 [![Maintainability](https://api.codeclimate.com/v1/badges/c62407f84ad66135fa8d/maintainability)](https://codeclimate.com/github/release-engineering/ubi-config/maintainability)
 
 - [Source](https://github.com/release-engineering/ubi-config)
 - [Documentation](https://release-engineering.github.io/ubi-config/)
 - [PyPI](https://pypi.org/project/ubi-config)
 
 Installation
```

### Comparing `ubi-config-2.2.0/ubiconfig/ubi.py` & `ubi-config-2.3.0/ubiconfig/ubi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import logging
 
-from six.moves.urllib.parse import urlparse
+from urllib.parse import urlparse
 
 from ._impl.loaders import _LocalLoader, _GitlabLoader
 
 
 DEFAULT_UBI_REPO = os.getenv("DEFAULT_UBI_REPO", "")
 
 LOG = logging.getLogger("ubiconfig")
```

### Comparing `ubi-config-2.2.0/ubiconfig/_impl/loaders/gitlab.py` & `ubi-config-2.3.0/ubiconfig/_impl/loaders/gitlab.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import logging
+import re
 import yaml
 import requests
 
 from jsonschema.exceptions import ValidationError
 
 from ubiconfig.utils.api.gitlab import RepoApi
 from ubiconfig.utils.config_validation import validate_config
 from ubiconfig.config_types import UbiConfig
 
 from .base import Loader
 
 LOG = logging.getLogger("ubiconfig")
 
+BRANCH_RE = re.compile(r"^(?P<prefix>[\w-]{1,25})(?P<default_version>[\d]{1,2})")
+
 
 class GitlabLoader(Loader):
     """Load configuration from a remote repo on gitlab."""
 
     def __init__(self, url):
         """
         :param url: gitlab repo url in form of `https://<host>/<repo>`
@@ -23,52 +26,62 @@
         self._url = url
         self._session = requests.Session()
         self._repo_api = RepoApi(self._url.rstrip("/"))
         self._branches = self._get_branches()
         self._files_branch_map = self._pre_load()
 
     def load(self, file_name, version=None):
-        """ Load file from remote repository.
+        """Load file from remote repository.
         :param file_name: filename that is on remote repository in any branch
+        :param version: name of remote branch
         """
+        if version is None:
+            raise ValueError(
+                "Provide valid name of remote branch, provided %s" % version
+            )
+
         if file_name not in self._files_branch_map:
             raise ValueError(
                 "Couldn't find file %s from remote repo %s" % (file_name, self._url)
             )
 
-        sha1 = self._branches.get(version)
-        if version and not sha1:
-            LOG.warning(
-                "Couldn't find version %s from %s, will try to find %s in default",
-                version,
-                self._url,
-                file_name,
-            )
+        match = re.match(BRANCH_RE, version)
+        if not match:
+            raise ValueError("Invalid version (branch name) %s" % version)
+
+        prefix = match.group("prefix")
+        default_version = match.group("default_version")
 
-        if not version or not sha1:
-            # branch is not available from the wanted version or not specified,
-            # use the default version.
-            for branch_sha1 in self._files_branch_map[file_name]:
-                if branch_sha1[0] == "ubi7":
-                    version = "ubi7"
-                    break
-            else:
-                version = "ubi8"
-            sha1 = self._branches[version]
+        default_branch = f"{prefix}{default_version}"
+
+        sha1 = None
+        loaded_version = None
+
+        for branch_name in (version, default_branch):
+            sha1 = self._branches.get(branch_name)
+            if sha1:
+                loaded_version = branch_name.lstrip(prefix)
+                break
+
+        if sha1 is None:
+            raise ValueError(
+                "Couldn't find version %s and default branch %s from %s for %s"
+                % (version, default_branch, self._url, file_name)
+            )
 
         LOG.info("Loading config file %s from branch %s", file_name, version)
         config_file_url = self._repo_api.get_file_content_api(file_name, sha1)
         response = self._session.get(config_file_url)
         response.raise_for_status()
 
         config_dict = yaml.load(response.content, Loader=yaml.BaseLoader)
         # validate input data
         validate_config(config_dict)
 
-        return UbiConfig.load_from_dict(config_dict, file_name, version[3:])
+        return UbiConfig.load_from_dict(config_dict, file_name, loaded_version)
 
     def load_all(self):
         ubi_configs = []
         for f in self._files_branch_map:
             for branch_sha1 in self._files_branch_map[f]:
                 LOG.debug("Now loading %s from branch %s", f, branch_sha1[0])
                 try:
@@ -81,16 +94,15 @@
                 except ValidationError as e:
                     LOG.error("%s FAILED schema validation:\n%s\nSkip for now", f, e)
                     continue
 
         return ubi_configs
 
     def _pre_load(self):
-        """Iterate all branches to get a mapping of {file_path: (branch, sha1)...}
-        """
+        """Iterate all branches to get a mapping of {file_path: (branch, sha1)...}"""
         files_branch_map = {}
 
         LOG.debug("Loading config files from all branches")
 
         for branch, sha1 in self._branches.items():
             page = 1
             while True:
```

### Comparing `ubi-config-2.2.0/ubiconfig/_impl/loaders/local.py` & `ubi-config-2.3.0/ubiconfig/_impl/loaders/local.py`

 * *Files identical despite different names*

### Comparing `ubi-config-2.2.0/ubiconfig/_impl/loaders/base.py` & `ubi-config-2.3.0/ubiconfig/_impl/loaders/base.py`

 * *Files identical despite different names*

### Comparing `ubi-config-2.2.0/ubiconfig/utils/api/gitlab.py` & `ubi-config-2.3.0/ubiconfig/utils/api/gitlab.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """provide gitlab api used to read repositories"""
 import os
 import re
 
-from six.moves.urllib.parse import urljoin
+from urllib.parse import urljoin
 
 
 DEFAULT_GIT_LAB_URL_FMT = re.compile(r"(?P<host>.+com|org|net)/(?P<project>.+)")
 
 API_FORMAT = "%s/api/v%s/projects/%s/"  # hostname/api/:apiversion/projects/:id/
 
 GIT_LAB_URL_FMT = re.compile(os.getenv("GIT_LAB_URL_FMT", DEFAULT_GIT_LAB_URL_FMT))
```

### Comparing `ubi-config-2.2.0/ubiconfig/utils/config_schema.json` & `ubi-config-2.3.0/ubiconfig/utils/config_schema.json`

 * *Files identical despite different names*

### Comparing `ubi-config-2.2.0/ubiconfig/config_types/content_sets.py` & `ubi-config-2.3.0/ubiconfig/config_types/content_sets.py`

 * *Files identical despite different names*

### Comparing `ubi-config-2.2.0/ubiconfig/config_types/modules.py` & `ubi-config-2.3.0/ubiconfig/config_types/modules.py`

 * *Files identical despite different names*

### Comparing `ubi-config-2.2.0/ubiconfig/config_types/__init__.py` & `ubi-config-2.3.0/ubiconfig/config_types/__init__.py`

 * *Files identical despite different names*

### Comparing `ubi-config-2.2.0/ubiconfig/config_types/packages.py` & `ubi-config-2.3.0/ubiconfig/config_types/packages.py`

 * *Files identical despite different names*

### Comparing `ubi-config-2.2.0/ubi_config.egg-info/PKG-INFO` & `ubi-config-2.3.0/ubi_config.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: ubi-config
-Version: 2.2.0
+Version: 2.3.0
 Summary: A Python Library for accessing Universal Base Image configuration
 Home-page: https://github.com/release-engineering/ubi-config
 Author: 
 Author-email: 
 License: GNU General Public License
 Project-URL: Documentation, https://release-engineering.github.io/ubi-config/
 Description: 
         
         A Python library for accessing Universal Base Image configuration
         
-        [![Build Status](https://travis-ci.org/release-engineering/ubi-config.svg?branch=master)](https://travis-ci.org/release-engineering/ubi-config)
-        [![Coverage Status](https://coveralls.io/repos/github/release-engineering/ubi-config/badge.svg?branch=master)](https://coveralls.io/github/release-engineering/ubi-config?branch=master)
+        [![Build Status](https://github.com/release-engineering/ubi-config/actions/workflows/tox-test.yml/badge.svg)](https://github.com/release-engineering/ubi-config/actions/workflows/tox-test.yml))
+        [![codecov](https://codecov.io/gh/release-engineering/ubi-config/branch/master/graph/badge.svg?token=fPG7EINR9O)](https://codecov.io/gh/release-engineering/ubi-config)
         [![Maintainability](https://api.codeclimate.com/v1/badges/c62407f84ad66135fa8d/maintainability)](https://codeclimate.com/github/release-engineering/ubi-config/maintainability)
         
         - [Source](https://github.com/release-engineering/ubi-config)
         - [Documentation](https://release-engineering.github.io/ubi-config/)
         - [PyPI](https://pypi.org/project/ubi-config)
         
         Installation
@@ -70,13 +70,11 @@
         (at your option) any later version.
         
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.6
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `ubi-config-2.2.0/ubi_config.egg-info/SOURCES.txt` & `ubi-config-2.3.0/ubi_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ubi-config-2.2.0/LICENSE` & `ubi-config-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ubi-config-2.2.0/CHANGELOG.md` & `ubi-config-2.3.0/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [v2.3.0] - 2023-08-04
+
+### Added
+- `GitlabLoader` is now more generic and supports custom branch names
+
 ## [v2.2.0] - 2019-10-24
 
 ### Added
 - Make ubiconfig.utils.config_validation.validate_config publicly available via
   ubiconfig.validate_config
 
 ### Fixed
```

### Comparing `ubi-config-2.2.0/setup.py` & `ubi-config-2.3.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,30 +17,28 @@
 def get_requirements():
     with open("requirements.txt") as f:
         return f.read().splitlines()
 
 
 setup(
     name="ubi-config",
-    version="2.2.0",
+    version="2.3.0",
     author="",
     author_email="",
     packages=find_packages(exclude=["tests", "tests.*"]),
     package_data={"ubiconfig": ["utils/config_schema.json"]},
     url="https://github.com/release-engineering/ubi-config",
     license="GNU General Public License",
     description=get_description(),
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
-        "Programming Language :: Python :: 2",
-        "Programming Language :: Python :: 2.6",
-        "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     install_requires=get_requirements(),
+    python_requires=">=3.6",
     project_urls={"Documentation": "https://release-engineering.github.io/ubi-config/"},
 )
```

