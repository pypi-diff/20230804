# Comparing `tmp/pytest-sosu-0.3.0.tar.gz` & `tmp/pytest-sosu-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/andrzejpragacz/projects/github.com/apragacz/pytest-sosu/dist/.tmp-04odsykv/pytest-sosu-0.3.0.tar", last modified: Wed Aug  2 22:43:48 2023, max compression
+gzip compressed data, was "/Users/andrzejpragacz/projects/github.com/apragacz/pytest-sosu/dist/.tmp-nejd7kct/pytest-sosu-0.3.1.tar", last modified: Fri Aug  4 08:45:02 2023, max compression
```

## Comparing `pytest-sosu-0.3.0.tar` & `pytest-sosu-0.3.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-08-02 22:43:48.360939 pytest-sosu-0.3.0/
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     1072 2020-02-24 11:36:45.000000 pytest-sosu-0.3.0/LICENSE
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)       49 2021-06-29 11:09:48.000000 pytest-sosu-0.3.0/MANIFEST.in
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     3642 2023-08-02 22:43:48.360218 pytest-sosu-0.3.0/PKG-INFO
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     1296 2023-08-02 22:29:12.000000 pytest-sosu-0.3.0/README.md
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     3001 2023-08-02 21:23:45.000000 pytest-sosu-0.3.0/pyproject.toml
-drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-08-02 22:43:48.337503 pytest-sosu-0.3.0/pytest_sosu/
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)       59 2021-06-29 11:53:51.000000 pytest-sosu-0.3.0/pytest_sosu/__init__.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)       22 2023-08-02 22:43:26.000000 pytest-sosu-0.3.0/pytest_sosu/_version.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     2215 2023-07-04 21:50:23.000000 pytest-sosu-0.3.0/pytest_sosu/config.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)      329 2022-02-19 00:17:09.000000 pytest-sosu-0.3.0/pytest_sosu/exceptions.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     3647 2023-02-13 23:47:50.000000 pytest-sosu-0.3.0/pytest_sosu/logging.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     5684 2023-08-02 21:27:18.000000 pytest-sosu-0.3.0/pytest_sosu/plugin.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     2278 2022-02-18 23:32:06.000000 pytest-sosu-0.3.0/pytest_sosu/plugin_helpers.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)      530 2022-01-18 13:38:52.000000 pytest-sosu-0.3.0/pytest_sosu/typing.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     3016 2023-02-13 12:03:21.000000 pytest-sosu-0.3.0/pytest_sosu/utils.py
-drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-08-02 22:43:48.358505 pytest-sosu-0.3.0/pytest_sosu/webdriver/
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)      517 2023-08-02 21:25:56.000000 pytest-sosu-0.3.0/pytest_sosu/webdriver/__init__.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     7728 2023-07-04 21:48:57.000000 pytest-sosu-0.3.0/pytest_sosu/webdriver/capabilities.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)      184 2023-08-02 21:25:04.000000 pytest-sosu-0.3.0/pytest_sosu/webdriver/compat.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     1975 2022-11-17 00:56:32.000000 pytest-sosu-0.3.0/pytest_sosu/webdriver/platforms.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     3089 2023-08-02 22:27:39.000000 pytest-sosu-0.3.0/pytest_sosu/webdriver/selenium.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     2048 2022-11-17 00:48:08.000000 pytest-sosu-0.3.0/pytest_sosu/webdriver/url.py
-drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-08-02 22:43:48.344941 pytest-sosu-0.3.0/pytest_sosu.egg-info/
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     3642 2023-08-02 22:43:48.000000 pytest-sosu-0.3.0/pytest_sosu.egg-info/PKG-INFO
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)      681 2023-08-02 22:43:48.000000 pytest-sosu-0.3.0/pytest_sosu.egg-info/SOURCES.txt
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)        1 2023-08-02 22:43:48.000000 pytest-sosu-0.3.0/pytest_sosu.egg-info/dependency_links.txt
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)       37 2023-08-02 22:43:48.000000 pytest-sosu-0.3.0/pytest_sosu.egg-info/entry_points.txt
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)       22 2023-08-02 22:43:48.000000 pytest-sosu-0.3.0/pytest_sosu.egg-info/requires.txt
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)       12 2023-08-02 22:43:48.000000 pytest-sosu-0.3.0/pytest_sosu.egg-info/top_level.txt
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)       38 2023-08-02 22:43:48.361263 pytest-sosu-0.3.0/setup.cfg
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)      102 2023-02-13 23:47:50.000000 pytest-sosu-0.3.0/setup.py
+drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-08-04 08:45:02.900148 pytest-sosu-0.3.1/
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)     1072 2020-02-24 11:36:45.000000 pytest-sosu-0.3.1/LICENSE
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)       49 2021-06-29 11:09:48.000000 pytest-sosu-0.3.1/MANIFEST.in
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)     3651 2023-08-04 08:45:02.895039 pytest-sosu-0.3.1/PKG-INFO
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)     1305 2023-08-02 22:45:38.000000 pytest-sosu-0.3.1/README.md
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)     3001 2023-08-02 21:23:45.000000 pytest-sosu-0.3.1/pyproject.toml
+drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-08-04 08:45:02.835771 pytest-sosu-0.3.1/pytest_sosu/
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)       59 2021-06-29 11:53:51.000000 pytest-sosu-0.3.1/pytest_sosu/__init__.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)       22 2023-08-04 08:44:32.000000 pytest-sosu-0.3.1/pytest_sosu/_version.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)     2894 2023-08-04 08:41:35.000000 pytest-sosu-0.3.1/pytest_sosu/config.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)      329 2022-02-19 00:17:09.000000 pytest-sosu-0.3.1/pytest_sosu/exceptions.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)     3647 2023-02-13 23:47:50.000000 pytest-sosu-0.3.1/pytest_sosu/logging.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)     6939 2023-08-04 08:40:30.000000 pytest-sosu-0.3.1/pytest_sosu/plugin.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)     2752 2023-08-04 08:40:18.000000 pytest-sosu-0.3.1/pytest_sosu/plugin_helpers.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)      530 2022-01-18 13:38:52.000000 pytest-sosu-0.3.1/pytest_sosu/typing.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)     3016 2023-02-13 12:03:21.000000 pytest-sosu-0.3.1/pytest_sosu/utils.py
+drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-08-04 08:45:02.892637 pytest-sosu-0.3.1/pytest_sosu/webdriver/
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)      517 2023-08-02 21:25:56.000000 pytest-sosu-0.3.1/pytest_sosu/webdriver/__init__.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)     7676 2023-08-02 22:57:59.000000 pytest-sosu-0.3.1/pytest_sosu/webdriver/capabilities.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)      184 2023-08-02 21:25:04.000000 pytest-sosu-0.3.1/pytest_sosu/webdriver/compat.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)     1975 2022-11-17 00:56:32.000000 pytest-sosu-0.3.1/pytest_sosu/webdriver/platforms.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)     3089 2023-08-02 22:27:39.000000 pytest-sosu-0.3.1/pytest_sosu/webdriver/selenium.py
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)     2048 2022-11-17 00:48:08.000000 pytest-sosu-0.3.1/pytest_sosu/webdriver/url.py
+drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-08-04 08:45:02.880243 pytest-sosu-0.3.1/pytest_sosu.egg-info/
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)     3651 2023-08-04 08:45:02.000000 pytest-sosu-0.3.1/pytest_sosu.egg-info/PKG-INFO
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)      681 2023-08-04 08:45:02.000000 pytest-sosu-0.3.1/pytest_sosu.egg-info/SOURCES.txt
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)        1 2023-08-04 08:45:02.000000 pytest-sosu-0.3.1/pytest_sosu.egg-info/dependency_links.txt
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)       37 2023-08-04 08:45:02.000000 pytest-sosu-0.3.1/pytest_sosu.egg-info/entry_points.txt
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)       22 2023-08-04 08:45:02.000000 pytest-sosu-0.3.1/pytest_sosu.egg-info/requires.txt
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)       12 2023-08-04 08:45:02.000000 pytest-sosu-0.3.1/pytest_sosu.egg-info/top_level.txt
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)       38 2023-08-04 08:45:02.900383 pytest-sosu-0.3.1/setup.cfg
+-rw-r--r--   0 andrzejpragacz   (502) staff       (20)      102 2023-02-13 23:47:50.000000 pytest-sosu-0.3.1/setup.py
```

### Comparing `pytest-sosu-0.3.0/LICENSE` & `pytest-sosu-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-sosu-0.3.0/PKG-INFO` & `pytest-sosu-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-sosu
-Version: 0.3.0
+Version: 0.3.1
 Summary: Unofficial PyTest plugin for Sauce Labs
 Author-email: Andrzej Pragacz <apragacz@o2.pl>
 License: MIT License
         
         Copyright (c) 2020 Andrzej Pragacz
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -88,12 +88,12 @@
 # when build basename is set, tests running in given pytest session
 # have a build assigned
 @pytest.fixture(scope="session")
 def sosu_build_basename():
     return 'my-project-name'
 
 
-# alias for sosu_webdriver
+# alias for sosu_selenium_webdriver
 @pytest.fixture
 def driver(sosu_selenium_webdriver):
     yield sosu_selenium_webdriver
 ```
```

### Comparing `pytest-sosu-0.3.0/README.md` & `pytest-sosu-0.3.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -41,12 +41,12 @@
 # when build basename is set, tests running in given pytest session
 # have a build assigned
 @pytest.fixture(scope="session")
 def sosu_build_basename():
     return 'my-project-name'
 
 
-# alias for sosu_webdriver
+# alias for sosu_selenium_webdriver
 @pytest.fixture
 def driver(sosu_selenium_webdriver):
     yield sosu_selenium_webdriver
 ```
```

### Comparing `pytest-sosu-0.3.0/pyproject.toml` & `pytest-sosu-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytest-sosu-0.3.0/pytest_sosu/config.py` & `pytest-sosu-0.3.1/pytest_sosu/config.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,37 +4,52 @@
 from typing import Optional
 
 from _pytest.config import UsageError
 
 from pytest_sosu.logging import get_struct_logger
 from pytest_sosu.webdriver import WebDriverUrlData
 
+DEFAULT_SAUCE_BUILD_FORMAT = "${build_basename}_${build_version}"
+
 logger = get_struct_logger(__name__)
 
 
+# pylint: disable=too-many-instance-attributes
 @dataclass
 class SosuConfig:
     username: str
     access_key: str
     region: Optional[str]
     webdriver_url_data: WebDriverUrlData
+    build_name: Optional[str]
+    build_basename: Optional[str]
+    build_version: Optional[str]
+    build_format: str
 
     @property
     def webdriver_url_data_with_credentials(self) -> WebDriverUrlData:
         if not self.webdriver_url_data.has_credentials:
             return self.webdriver_url_data.with_credentials(
                 self.username, self.access_key
             )
         return self.webdriver_url_data
 
 
 def build_sosu_config(args: argparse.Namespace, env: os._Environ) -> SosuConfig:
     logger.debug("build_sosu_config", args=args, env=env)
     username = args.sosu_username or env.get("SAUCE_USERNAME")
     access_key = args.sosu_access_key or env.get("SAUCE_ACCESS_KEY")
+    build_name = args.sosu_build_name or env.get("SAUCE_BUILD_NAME")
+    build_basename = args.sosu_build_basename or env.get("SAUCE_BUILD_BASENAME")
+    build_version = args.sosu_build_version or env.get("SAUCE_BUILD_VERSION")
+    build_format = (
+        args.sosu_build_format
+        or env.get("SAUCE_BUILD_FORMAT")
+        or DEFAULT_SAUCE_BUILD_FORMAT
+    )
 
     if not username:
         raise UsageError("--sosu-username or SAUCE_USERNAME are not provided")
 
     if not access_key:
         raise UsageError("--sosu-access-key or SAUCE_ACCESS_KEY are not provided")
 
@@ -51,14 +66,18 @@
             raise UsageError("Invalid WebDriver URL") from None
 
     return SosuConfig(
         username=username,
         access_key=access_key,
         region=region,
         webdriver_url_data=webdriver_url_data,
+        build_name=build_name,
+        build_basename=build_basename,
+        build_version=build_version,
+        build_format=build_format,
     )
 
 
 def get_host_by_region(region: Optional[str]) -> str:
     if not region:
         region = "us"
     if region in ["global", "legacy"]:
@@ -66,10 +85,8 @@
     host_region = REGION_MAP.get(region, region)
     return f"ondemand.{host_region}.saucelabs.com"
 
 
 REGION_MAP = {
     "us": "us-west-1",
     "eu": "eu-central-1",
-    "apac": "apac-southeast-1",
-    "headless": "us-east-1",
 }
```

### Comparing `pytest-sosu-0.3.0/pytest_sosu/logging.py` & `pytest-sosu-0.3.1/pytest_sosu/logging.py`

 * *Files identical despite different names*

### Comparing `pytest-sosu-0.3.0/pytest_sosu/plugin.py` & `pytest-sosu-0.3.1/pytest_sosu/plugin.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Any, Callable, Optional
 
 import pytest
 from _pytest.config import Config
 
 from pytest_sosu.config import SosuConfig, build_sosu_config
 from pytest_sosu.logging import get_struct_logger
-from pytest_sosu.plugin_helpers import parametrize_capabilities
+from pytest_sosu.plugin_helpers import build_sosu_build_name, parametrize_capabilities
 from pytest_sosu.webdriver import (
     Browser,
     Capabilities,
     Platform,
     SauceOptions,
     WebDriverTestFailed,
     WebDriverTestInterrupted,
@@ -46,14 +46,38 @@
     )
     group.addoption(
         "--sosu-webdriver-url",
         action="store",
         metavar="SAUCE_WEBDRIVER_URL",
         help="Sauce Labs WebDriver URL",
     )
+    group.addoption(
+        "--sosu-build-basename",
+        action="store",
+        metavar="SAUCE_BUILD_BASENAME",
+        help="Sauce Labs build basename",
+    )
+    group.addoption(
+        "--sosu-build-version",
+        action="store",
+        metavar="SAUCE_BUILD_VERSION",
+        help="Sauce Labs build version",
+    )
+    group.addoption(
+        "--sosu-build-format",
+        action="store",
+        metavar="SAUCE_BUILD_FORMAT",
+        help="Sauce Labs build format",
+    )
+    group.addoption(
+        "--sosu-build-name",
+        action="store",
+        metavar="SAUCE_BUILD_NAME",
+        help="Sauce Labs build name",
+    )
 
 
 def pytest_configure(config: Config):
     logger.debug("pytest_configure", config=config)
     # register an additional marker
     config.addinivalue_line("markers", "sosu(type): mark test to run with Sauce Labs")
 
@@ -90,38 +114,56 @@
 
     # Set a report attribute for each phase of a call, which can
     # be "setup", "call", "teardown"
     setattr(item, "report_when_" + report.when, report)
 
 
 @pytest.fixture(scope="session")
-def sosu_build_basename() -> Optional[str]:
-    return None
+def sosu_build_basename(pytestconfig: Config) -> Optional[str]:
+    sosu_config = _get_sosu_config(pytestconfig)
+    return sosu_config.region
 
 
 @pytest.fixture(scope="session")
 def sosu_build_time_tag() -> str:
     now = datetime.datetime.now()
     date_str = f"{now.year}{now.month:02d}{now.day:02d}"
     time_str = f"{now.hour:02d}{now.minute:02d}"
     return f"{date_str}_{time_str}"
 
 
 @pytest.fixture(scope="session")
-def sosu_build_version(sosu_build_time_tag: str) -> str:
+def sosu_build_format(pytestconfig: Config) -> str:
+    sosu_config = _get_sosu_config(pytestconfig)
+    return sosu_config.build_format
+
+
+@pytest.fixture(scope="session")
+def sosu_build_version(pytestconfig: Config, sosu_build_time_tag: str) -> str:
+    sosu_config = _get_sosu_config(pytestconfig)
+    if sosu_config.build_version:
+        return sosu_config.build_version
     return sosu_build_time_tag
 
 
 @pytest.fixture(scope="session")
 def sosu_build_name(
-    sosu_build_basename: Optional[str], sosu_build_version: str
+    pytestconfig: Config,
+    sosu_build_basename: Optional[str],
+    sosu_build_version: str,
+    sosu_build_format: str,
 ) -> Optional[str]:
-    if sosu_build_basename is None:
-        return None
-    return f"{sosu_build_basename}_{sosu_build_version}"
+    sosu_config = _get_sosu_config(pytestconfig)
+    if sosu_config.build_name:
+        return sosu_config.build_name
+    return build_sosu_build_name(
+        sosu_build_basename,
+        sosu_build_version,
+        sosu_build_format,
+    )
 
 
 @pytest.fixture
 def sosu_webdriver_url_data(pytestconfig: Config) -> WebDriverUrlData:
     sosu_config = _get_sosu_config(pytestconfig)
     return sosu_config.webdriver_url_data_with_credentials
```

### Comparing `pytest-sosu-0.3.0/pytest_sosu/plugin_helpers.py` & `pytest-sosu-0.3.1/pytest_sosu/plugin_helpers.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import string
 from typing import Any, List, Optional
 
 import pytest
 from _pytest.mark.structures import Mark
 from _pytest.python import Metafunc
 
 from pytest_sosu.exceptions import (
@@ -76,7 +77,25 @@
     if len(values) > 1:
         raise MultipleMarkerParametersFound()
 
     if not values:
         return None
 
     return values[0]
+
+
+def build_sosu_build_name(
+    sosu_build_basename: Optional[str],
+    sosu_build_version: str,
+    sosu_build_format: str,
+) -> Optional[str]:
+    if sosu_build_basename is None:
+        return None
+    if not sosu_build_format:
+        return None
+    template = string.Template(sosu_build_format)
+    return template.substitute(
+        {
+            "build_basename": sosu_build_basename,
+            "build_version": sosu_build_version,
+        }
+    )
```

### Comparing `pytest-sosu-0.3.0/pytest_sosu/typing.py` & `pytest-sosu-0.3.1/pytest_sosu/typing.py`

 * *Files identical despite different names*

### Comparing `pytest-sosu-0.3.0/pytest_sosu/utils.py` & `pytest-sosu-0.3.1/pytest_sosu/utils.py`

 * *Files identical despite different names*

### Comparing `pytest-sosu-0.3.0/pytest_sosu/webdriver/__init__.py` & `pytest-sosu-0.3.1/pytest_sosu/webdriver/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest-sosu-0.3.0/pytest_sosu/webdriver/capabilities.py` & `pytest-sosu-0.3.1/pytest_sosu/webdriver/capabilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 from __future__ import annotations
 
 import dataclasses
 import enum
 from dataclasses import dataclass
 from typing import Any, Dict, Iterator, List, Optional, Sequence, Union
 
-import selenium  # type: ignore
-import selenium.webdriver  # type: ignore
-import selenium.webdriver.common.by  # type: ignore
-
 from pytest_sosu.logging import get_struct_logger
 from pytest_sosu.utils import (
     ImmutableDict,
     convert_snake_case_to_camel_case,
     try_one_of,
     try_one_of_or_none,
 )
+from pytest_sosu.webdriver.compat import selenium_version
 from pytest_sosu.webdriver.platforms import Browser, Platform
 
 logger = get_struct_logger(__name__)
 
 
 class SauceTestResultsVisibility(enum.Enum):
     PUBLIC = "public"
@@ -94,16 +91,16 @@
         auto_include_selenium_version = try_one_of(
             auto_include_selenium_version,
             lambda: self.auto_include_selenium_version,
             default=False,
         )
 
         data: Dict[str, Any] = {}
-        if auto_include_selenium_version:
-            data["seleniumVersion"] = selenium.__version__
+        if auto_include_selenium_version and selenium_version:
+            data["seleniumVersion"] = selenium_version
         for field in dataclasses.fields(self):
             name = field.name
             if name in self.TO_DICT_AUTO_EXCLUDES:
                 continue
             value = getattr(self, name)
             if value is None:
                 continue
```

### Comparing `pytest-sosu-0.3.0/pytest_sosu/webdriver/platforms.py` & `pytest-sosu-0.3.1/pytest_sosu/webdriver/platforms.py`

 * *Files identical despite different names*

### Comparing `pytest-sosu-0.3.0/pytest_sosu/webdriver/selenium.py` & `pytest-sosu-0.3.1/pytest_sosu/webdriver/selenium.py`

 * *Files identical despite different names*

### Comparing `pytest-sosu-0.3.0/pytest_sosu/webdriver/url.py` & `pytest-sosu-0.3.1/pytest_sosu/webdriver/url.py`

 * *Files identical despite different names*

### Comparing `pytest-sosu-0.3.0/pytest_sosu.egg-info/PKG-INFO` & `pytest-sosu-0.3.1/pytest_sosu.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-sosu
-Version: 0.3.0
+Version: 0.3.1
 Summary: Unofficial PyTest plugin for Sauce Labs
 Author-email: Andrzej Pragacz <apragacz@o2.pl>
 License: MIT License
         
         Copyright (c) 2020 Andrzej Pragacz
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -88,12 +88,12 @@
 # when build basename is set, tests running in given pytest session
 # have a build assigned
 @pytest.fixture(scope="session")
 def sosu_build_basename():
     return 'my-project-name'
 
 
-# alias for sosu_webdriver
+# alias for sosu_selenium_webdriver
 @pytest.fixture
 def driver(sosu_selenium_webdriver):
     yield sosu_selenium_webdriver
 ```
```

### Comparing `pytest-sosu-0.3.0/pytest_sosu.egg-info/SOURCES.txt` & `pytest-sosu-0.3.1/pytest_sosu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

