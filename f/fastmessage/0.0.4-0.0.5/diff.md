# Comparing `tmp/fastmessage-0.0.4.tar.gz` & `tmp/fastmessage-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastmessage-0.0.4.tar", last modified: Fri Aug  4 07:57:15 2023, max compression
+gzip compressed data, was "fastmessage-0.0.5.tar", last modified: Fri Aug  4 15:29:29 2023, max compression
```

## Comparing `fastmessage-0.0.4.tar` & `fastmessage-0.0.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:57:15.243010 fastmessage-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-04 07:57:03.000000 fastmessage-0.0.4/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-04 07:57:03.000000 fastmessage-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-08-04 07:57:03.000000 fastmessage-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-08-04 07:57:15.243010 fastmessage-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-08-04 07:57:03.000000 fastmessage-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-04 07:57:04.000000 fastmessage-0.0.4/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:57:15.243010 fastmessage-0.0.4/_custom_build/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:57:03.000000 fastmessage-0.0.4/_custom_build/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-08-04 07:57:03.000000 fastmessage-0.0.4/_custom_build/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-04 07:57:03.000000 fastmessage-0.0.4/_custom_build/make_all_extra_requirements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:57:15.243010 fastmessage-0.0.4/fastmessage/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-08-04 07:57:03.000000 fastmessage-0.0.4/fastmessage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-08-04 07:57:03.000000 fastmessage-0.0.4/fastmessage/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12444 2023-08-04 07:57:03.000000 fastmessage-0.0.4/fastmessage/fastmessage_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:57:03.000000 fastmessage-0.0.4/fastmessage/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:57:15.243010 fastmessage-0.0.4/fastmessage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-08-04 07:57:15.000000 fastmessage-0.0.4/fastmessage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-08-04 07:57:15.000000 fastmessage-0.0.4/fastmessage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 07:57:15.000000 fastmessage-0.0.4/fastmessage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-08-04 07:57:15.000000 fastmessage-0.0.4/fastmessage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-04 07:57:15.000000 fastmessage-0.0.4/fastmessage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-08-04 07:57:03.000000 fastmessage-0.0.4/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-08-04 07:57:03.000000 fastmessage-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-04 07:57:03.000000 fastmessage-0.0.4/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-04 07:57:15.000000 fastmessage-0.0.4/requirements-all.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-04 07:57:03.000000 fastmessage-0.0.4/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-04 07:57:03.000000 fastmessage-0.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 07:57:15.243010 fastmessage-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:29:29.570018 fastmessage-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-04 15:29:16.000000 fastmessage-0.0.5/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-04 15:29:16.000000 fastmessage-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-08-04 15:29:16.000000 fastmessage-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-08-04 15:29:29.570018 fastmessage-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-08-04 15:29:16.000000 fastmessage-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-04 15:29:17.000000 fastmessage-0.0.5/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:29:29.570018 fastmessage-0.0.5/_custom_build/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 15:29:16.000000 fastmessage-0.0.5/_custom_build/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-08-04 15:29:16.000000 fastmessage-0.0.5/_custom_build/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-04 15:29:16.000000 fastmessage-0.0.5/_custom_build/make_all_extra_requirements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:29:29.570018 fastmessage-0.0.5/fastmessage/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-08-04 15:29:16.000000 fastmessage-0.0.5/fastmessage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-08-04 15:29:16.000000 fastmessage-0.0.5/fastmessage/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12591 2023-08-04 15:29:16.000000 fastmessage-0.0.5/fastmessage/fastmessage_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 15:29:16.000000 fastmessage-0.0.5/fastmessage/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:29:29.570018 fastmessage-0.0.5/fastmessage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-08-04 15:29:29.000000 fastmessage-0.0.5/fastmessage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-08-04 15:29:29.000000 fastmessage-0.0.5/fastmessage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 15:29:29.000000 fastmessage-0.0.5/fastmessage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-08-04 15:29:29.000000 fastmessage-0.0.5/fastmessage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-04 15:29:29.000000 fastmessage-0.0.5/fastmessage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-08-04 15:29:16.000000 fastmessage-0.0.5/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-08-04 15:29:16.000000 fastmessage-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-04 15:29:16.000000 fastmessage-0.0.5/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-04 15:29:29.000000 fastmessage-0.0.5/requirements-all.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-04 15:29:16.000000 fastmessage-0.0.5/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-04 15:29:16.000000 fastmessage-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 15:29:29.570018 fastmessage-0.0.5/setup.cfg
```

### Comparing `fastmessage-0.0.4/LICENSE` & `fastmessage-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fastmessage-0.0.4/PKG-INFO` & `fastmessage-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastmessage
-Version: 0.0.4
+Version: 0.0.5
 Author-email: Aviv Salem <avivsalem@gmail.com>
 Maintainer-email: Aviv Salem <avivsalem@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Avivsalem/FastMessage/
 Project-URL: Documentation, https://fastmessage.readthedocs.io/
 Platform: win32
 Platform: linux
@@ -24,15 +24,15 @@
 # FastMessage
 
 [![stars](https://badgen.net/github/stars/Avivsalem/FastMessage)](https://github.com/Avivsalem/FastMessage/stargazers)
 [![license](https://badgen.net/github/license/Avivsalem/FastMessage/)](https://github.com/Avivsalem/FastMessage/blob/main/LICENSE)
 [![last commit](https://badgen.net/github/last-commit/Avivsalem/FastMessage/main)](https://github.com/Avivsalem/FastMessage/commit/main)
 [![tests](https://github.com/AvivSalem/FastMessage/actions/workflows/tests.yml/badge.svg)](https://github.com/AvivSalem/FastMessage/actions/workflows/tests.yml?query=branch%3Amain)
 [![Documentation Status](https://readthedocs.org/projects/fastmessage/badge/?version=latest)](https://fastmessage.readthedocs.io/en/latest/?badge=latest)
-[![pypi version](https://badgen.net/pypi/v/FastMessage)](https://pypi.org/project/fastmessage/)
+[![pypi version](https://badgen.net/pypi/v/fastmessage)](https://pypi.org/project/fastmessage/)
 [![python compatibility](https://badgen.net/pypi/python/FastMessage)](https://pypi.org/project/fastmessage/)
 [![downloads](https://img.shields.io/pypi/dm/fastmessage)](https://pypi.org/project/fastmessage/)
 
 FastMessage is an easy framework to create PipelineHandlers for [MessageFlux](https://messageflux.readthedocs.io)
 
 You can find the full documentation [here](https://fastmessage.readthedocs.io/)
```

### Comparing `fastmessage-0.0.4/README.md` & `fastmessage-0.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # FastMessage
 
 [![stars](https://badgen.net/github/stars/Avivsalem/FastMessage)](https://github.com/Avivsalem/FastMessage/stargazers)
 [![license](https://badgen.net/github/license/Avivsalem/FastMessage/)](https://github.com/Avivsalem/FastMessage/blob/main/LICENSE)
 [![last commit](https://badgen.net/github/last-commit/Avivsalem/FastMessage/main)](https://github.com/Avivsalem/FastMessage/commit/main)
 [![tests](https://github.com/AvivSalem/FastMessage/actions/workflows/tests.yml/badge.svg)](https://github.com/AvivSalem/FastMessage/actions/workflows/tests.yml?query=branch%3Amain)
 [![Documentation Status](https://readthedocs.org/projects/fastmessage/badge/?version=latest)](https://fastmessage.readthedocs.io/en/latest/?badge=latest)
-[![pypi version](https://badgen.net/pypi/v/FastMessage)](https://pypi.org/project/fastmessage/)
+[![pypi version](https://badgen.net/pypi/v/fastmessage)](https://pypi.org/project/fastmessage/)
 [![python compatibility](https://badgen.net/pypi/python/FastMessage)](https://pypi.org/project/fastmessage/)
 [![downloads](https://img.shields.io/pypi/dm/fastmessage)](https://pypi.org/project/fastmessage/)
 
 FastMessage is an easy framework to create PipelineHandlers for [MessageFlux](https://messageflux.readthedocs.io)
 
 You can find the full documentation [here](https://fastmessage.readthedocs.io/)
```

### Comparing `fastmessage-0.0.4/_custom_build/make_all_extra_requirements.py` & `fastmessage-0.0.5/_custom_build/make_all_extra_requirements.py`

 * *Files identical despite different names*

### Comparing `fastmessage-0.0.4/fastmessage/fastmessage_handler.py` & `fastmessage-0.0.5/fastmessage/fastmessage_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import inspect
 import json
 import logging
 from dataclasses import dataclass
-from typing import Optional, Callable, Dict, List, Any, TypeVar, Union
+from typing import Optional, Callable, Dict, List, Any, TypeVar, Union, Iterable, Generator
 
+import itertools
 from pydantic import BaseModel, parse_raw_as, create_model, ValidationError, Extra
 from pydantic.config import get_config
 from pydantic.typing import get_all_type_hints
 
 from fastmessage import NotAllowedParamKindException, SpecialDefaultValueException, UnnamedCallableException, \
     DuplicateCallbackException, MissingCallbackException
 from messageflux import InputDevice
@@ -103,15 +104,15 @@
                                        **model_params)
 
     def _get_model_name(self) -> str:
         return f"model_{self._callback.__name__}_{self._input_device}"
 
     def __call__(self,
                  input_device: InputDevice,
-                 message_bundle: MessageBundle) -> Optional[Union[PipelineResult, List[PipelineResult]]]:
+                 message_bundle: MessageBundle) -> Optional[Union[PipelineResult, Iterable[PipelineResult]]]:
         kwargs: Dict[str, Any] = {}
         for param_name, param_info in self._special_params.items():
             if param_info.annotation is InputDeviceName:
                 kwargs[param_name] = input_device.name
             elif param_info.annotation is MessageBundle:
                 kwargs[param_name] = message_bundle
             elif param_info.annotation is Message:
@@ -124,30 +125,33 @@
         callback_return = self._callback(**kwargs)
         if callback_return is None:
             return None
 
         return self._get_pipeline_results(value=callback_return,
                                           default_output_device=self._output_device)
 
-    def _get_pipeline_results(self, value: Any, default_output_device: Optional[str]) -> List[PipelineResult]:
-        results = []
-        if isinstance(value, MultipleReturnValues):
-            for item in value:
-                results.extend(self._get_pipeline_results(value=item,
-                                                          default_output_device=default_output_device))
+    def _get_pipeline_results(self,
+                              value: Any,
+                              default_output_device: Optional[str]) -> Iterable[PipelineResult]:
+
+        if isinstance(value, (MultipleReturnValues, Generator)):
+            return itertools.chain.from_iterable(map(lambda item: self._get_pipeline_results(item,
+                                                                                             default_output_device),
+                                                     value))
+
         elif isinstance(value, FastMessageOutput):
-            results.extend(self._get_pipeline_results(value=value.value,
-                                                      default_output_device=value.output_device))
+            return self._get_pipeline_results(value=value.value,
+                                              default_output_device=value.output_device)
         else:
             pipeline_result = self._get_single_pipeline_result(value=value,
                                                                output_device=default_output_device)
             if pipeline_result is not None:
-                results.append(pipeline_result)
+                return [pipeline_result]
 
-        return results
+        return []
 
     def _get_single_pipeline_result(self, value: Any, output_device: Optional[str]) -> Optional[PipelineResult]:
         if output_device is None:
             _logger.warning(f"callback for input device '{self._input_device}' returned value, "
                             f"but is not mapped to output device")
             return None
 
@@ -248,15 +252,15 @@
                                    output_device=output_device)
             return callback
 
         return _register_callback_decorator
 
     def handle_message(self,
                        input_device: InputDevice,
-                       message_bundle: MessageBundle) -> Optional[Union[PipelineResult, List[PipelineResult]]]:
+                       message_bundle: MessageBundle) -> Optional[Union[PipelineResult, Iterable[PipelineResult]]]:
         callback_wrapper = self._wrappers.get(input_device.name)
         if callback_wrapper is None:
             raise MissingCallbackException(f"No callback registered for device '{input_device.name}'")
         try:
             return callback_wrapper(input_device=input_device, message_bundle=message_bundle)
         except ValidationError as ve:
             if self._validation_error_handler is None:
```

### Comparing `fastmessage-0.0.4/fastmessage.egg-info/PKG-INFO` & `fastmessage-0.0.5/fastmessage.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastmessage
-Version: 0.0.4
+Version: 0.0.5
 Author-email: Aviv Salem <avivsalem@gmail.com>
 Maintainer-email: Aviv Salem <avivsalem@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Avivsalem/FastMessage/
 Project-URL: Documentation, https://fastmessage.readthedocs.io/
 Platform: win32
 Platform: linux
@@ -24,15 +24,15 @@
 # FastMessage
 
 [![stars](https://badgen.net/github/stars/Avivsalem/FastMessage)](https://github.com/Avivsalem/FastMessage/stargazers)
 [![license](https://badgen.net/github/license/Avivsalem/FastMessage/)](https://github.com/Avivsalem/FastMessage/blob/main/LICENSE)
 [![last commit](https://badgen.net/github/last-commit/Avivsalem/FastMessage/main)](https://github.com/Avivsalem/FastMessage/commit/main)
 [![tests](https://github.com/AvivSalem/FastMessage/actions/workflows/tests.yml/badge.svg)](https://github.com/AvivSalem/FastMessage/actions/workflows/tests.yml?query=branch%3Amain)
 [![Documentation Status](https://readthedocs.org/projects/fastmessage/badge/?version=latest)](https://fastmessage.readthedocs.io/en/latest/?badge=latest)
-[![pypi version](https://badgen.net/pypi/v/FastMessage)](https://pypi.org/project/fastmessage/)
+[![pypi version](https://badgen.net/pypi/v/fastmessage)](https://pypi.org/project/fastmessage/)
 [![python compatibility](https://badgen.net/pypi/python/FastMessage)](https://pypi.org/project/fastmessage/)
 [![downloads](https://img.shields.io/pypi/dm/fastmessage)](https://pypi.org/project/fastmessage/)
 
 FastMessage is an easy framework to create PipelineHandlers for [MessageFlux](https://messageflux.readthedocs.io)
 
 You can find the full documentation [here](https://fastmessage.readthedocs.io/)
```

### Comparing `fastmessage-0.0.4/fastmessage.egg-info/SOURCES.txt` & `fastmessage-0.0.5/fastmessage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastmessage-0.0.4/pyproject.toml` & `fastmessage-0.0.5/pyproject.toml`

 * *Files identical despite different names*

