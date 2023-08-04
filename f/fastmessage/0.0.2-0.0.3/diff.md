# Comparing `tmp/fastmessage-0.0.2.tar.gz` & `tmp/fastmessage-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastmessage-0.0.2.tar", last modified: Thu Aug  3 20:18:27 2023, max compression
+gzip compressed data, was "fastmessage-0.0.3.tar", last modified: Fri Aug  4 04:09:46 2023, max compression
```

## Comparing `fastmessage-0.0.2.tar` & `fastmessage-0.0.3.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:18:27.908064 fastmessage-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-03 20:18:16.000000 fastmessage-0.0.2/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-03 20:18:16.000000 fastmessage-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-08-03 20:18:16.000000 fastmessage-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-08-03 20:18:27.908064 fastmessage-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-08-03 20:18:16.000000 fastmessage-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-03 20:18:17.000000 fastmessage-0.0.2/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:18:27.908064 fastmessage-0.0.2/_custom_build/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:18:16.000000 fastmessage-0.0.2/_custom_build/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-08-03 20:18:16.000000 fastmessage-0.0.2/_custom_build/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-03 20:18:16.000000 fastmessage-0.0.2/_custom_build/make_all_extra_requirements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:18:27.908064 fastmessage-0.0.2/fastmessage/
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-08-03 20:18:16.000000 fastmessage-0.0.2/fastmessage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12660 2023-08-03 20:18:16.000000 fastmessage-0.0.2/fastmessage/fastmessage_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:18:16.000000 fastmessage-0.0.2/fastmessage/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:18:27.908064 fastmessage-0.0.2/fastmessage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-08-03 20:18:27.000000 fastmessage-0.0.2/fastmessage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-08-03 20:18:27.000000 fastmessage-0.0.2/fastmessage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 20:18:27.000000 fastmessage-0.0.2/fastmessage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-08-03 20:18:27.000000 fastmessage-0.0.2/fastmessage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-03 20:18:27.000000 fastmessage-0.0.2/fastmessage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-08-03 20:18:16.000000 fastmessage-0.0.2/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-08-03 20:18:16.000000 fastmessage-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-03 20:18:16.000000 fastmessage-0.0.2/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-03 20:18:27.000000 fastmessage-0.0.2/requirements-all.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-03 20:18:16.000000 fastmessage-0.0.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-03 20:18:16.000000 fastmessage-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 20:18:27.908064 fastmessage-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 04:09:46.130957 fastmessage-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-04 04:09:32.000000 fastmessage-0.0.3/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-04 04:09:32.000000 fastmessage-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-08-04 04:09:32.000000 fastmessage-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-08-04 04:09:46.130957 fastmessage-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-08-04 04:09:32.000000 fastmessage-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-04 04:09:33.000000 fastmessage-0.0.3/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 04:09:46.126958 fastmessage-0.0.3/_custom_build/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 04:09:32.000000 fastmessage-0.0.3/_custom_build/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-08-04 04:09:32.000000 fastmessage-0.0.3/_custom_build/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-04 04:09:32.000000 fastmessage-0.0.3/_custom_build/make_all_extra_requirements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 04:09:46.130957 fastmessage-0.0.3/fastmessage/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-08-04 04:09:32.000000 fastmessage-0.0.3/fastmessage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-08-04 04:09:32.000000 fastmessage-0.0.3/fastmessage/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12444 2023-08-04 04:09:32.000000 fastmessage-0.0.3/fastmessage/fastmessage_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 04:09:32.000000 fastmessage-0.0.3/fastmessage/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 04:09:46.130957 fastmessage-0.0.3/fastmessage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-08-04 04:09:46.000000 fastmessage-0.0.3/fastmessage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-08-04 04:09:46.000000 fastmessage-0.0.3/fastmessage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 04:09:46.000000 fastmessage-0.0.3/fastmessage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-08-04 04:09:46.000000 fastmessage-0.0.3/fastmessage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-04 04:09:46.000000 fastmessage-0.0.3/fastmessage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-08-04 04:09:32.000000 fastmessage-0.0.3/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-08-04 04:09:32.000000 fastmessage-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-04 04:09:32.000000 fastmessage-0.0.3/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-04 04:09:45.000000 fastmessage-0.0.3/requirements-all.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-04 04:09:32.000000 fastmessage-0.0.3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-04 04:09:32.000000 fastmessage-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 04:09:46.130957 fastmessage-0.0.3/setup.cfg
```

### Comparing `fastmessage-0.0.2/LICENSE` & `fastmessage-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fastmessage-0.0.2/PKG-INFO` & `fastmessage-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastmessage
-Version: 0.0.2
+Version: 0.0.3
 Author-email: Aviv Salem <avivsalem@gmail.com>
 Maintainer-email: Aviv Salem <avivsalem@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Avivsalem/FastMessage/
 Project-URL: Documentation, https://fastmessage.readthedocs.io/
 Platform: win32
 Platform: linux
```

### Comparing `fastmessage-0.0.2/README.md` & `fastmessage-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `fastmessage-0.0.2/_custom_build/make_all_extra_requirements.py` & `fastmessage-0.0.3/_custom_build/make_all_extra_requirements.py`

 * *Files identical despite different names*

### Comparing `fastmessage-0.0.2/fastmessage/fastmessage_handler.py` & `fastmessage-0.0.3/fastmessage/fastmessage_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,46 +1,24 @@
 import inspect
 import json
 import logging
 from dataclasses import dataclass
 from typing import Optional, Callable, Dict, List, Any, TypeVar, Union
 
+from pydantic import BaseModel, parse_raw_as, create_model, ValidationError, Extra
+from pydantic.config import get_config
+from pydantic.typing import get_all_type_hints
+
+from fastmessage import NotAllowedParamKindException, SpecialDefaultValueException, UnnamedCallableException, \
+    DuplicateCallbackException, MissingCallbackException
 from messageflux import InputDevice
 from messageflux.iodevices.base import InputDeviceManager, OutputDeviceManager
 from messageflux.iodevices.base.common import MessageBundle, Message
 from messageflux.pipeline_service import PipelineHandlerBase, PipelineResult, PipelineService
 
-from pydantic.typing import get_all_type_hints
-from pydantic import BaseModel, parse_raw_as, create_model, ValidationError, Extra
-from pydantic.config import get_config
-
-
-class FastMessageException(Exception):
-    pass
-
-
-class DuplicateCallbackException(FastMessageException):
-    pass
-
-
-class NotAllowedParamKindException(FastMessageException):
-    pass
-
-
-class MissingCallbackException(FastMessageException):
-    pass
-
-
-class SpecialDefaultValueException(FastMessageException):
-    pass
-
-
-class UnnamedCallableException(FastMessageException):
-    pass
-
 
 class InputDeviceName(str):
     """
     a place holder class for input_device name
     """
     pass
```

### Comparing `fastmessage-0.0.2/fastmessage.egg-info/PKG-INFO` & `fastmessage-0.0.3/fastmessage.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastmessage
-Version: 0.0.2
+Version: 0.0.3
 Author-email: Aviv Salem <avivsalem@gmail.com>
 Maintainer-email: Aviv Salem <avivsalem@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Avivsalem/FastMessage/
 Project-URL: Documentation, https://fastmessage.readthedocs.io/
 Platform: win32
 Platform: linux
```

### Comparing `fastmessage-0.0.2/pyproject.toml` & `fastmessage-0.0.3/pyproject.toml`

 * *Files identical despite different names*

