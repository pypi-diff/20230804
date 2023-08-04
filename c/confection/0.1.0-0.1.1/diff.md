# Comparing `tmp/confection-0.1.0.tar.gz` & `tmp/confection-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "confection-0.1.0.tar", last modified: Thu Jun 29 08:12:12 2023, max compression
+gzip compressed data, was "confection-0.1.1.tar", last modified: Fri Aug  4 09:52:03 2023, max compression
```

## Comparing `confection-0.1.0.tar` & `confection-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-29 08:12:12.103952 confection-0.1.0/
--rw-r--r--   0 vsts      (1001) docker     (122)     1073 2023-06-29 08:12:00.000000 confection-0.1.0/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)       44 2023-06-29 08:12:00.000000 confection-0.1.0/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)    18832 2023-06-29 08:12:12.103952 confection-0.1.0/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)    17749 2023-06-29 08:12:00.000000 confection-0.1.0/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-29 08:12:12.103952 confection-0.1.0/confection/
--rw-r--r--   0 vsts      (1001) docker     (122)    46489 2023-06-29 08:12:00.000000 confection-0.1.0/confection/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-29 08:12:00.000000 confection-0.1.0/confection/py.typed
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-29 08:12:12.103952 confection-0.1.0/confection/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-29 08:12:00.000000 confection-0.1.0/confection/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      488 2023-06-29 08:12:00.000000 confection-0.1.0/confection/tests/conftest.py
--rw-r--r--   0 vsts      (1001) docker     (122)    53132 2023-06-29 08:12:00.000000 confection-0.1.0/confection/tests/test_config.py
--rw-r--r--   0 vsts      (1001) docker     (122)      774 2023-06-29 08:12:00.000000 confection-0.1.0/confection/tests/test_frozen_structures.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3627 2023-06-29 08:12:00.000000 confection-0.1.0/confection/tests/util.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4074 2023-06-29 08:12:00.000000 confection-0.1.0/confection/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-29 08:12:12.103952 confection-0.1.0/confection.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)    18832 2023-06-29 08:12:12.000000 confection-0.1.0/confection.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      481 2023-06-29 08:12:12.000000 confection-0.1.0/confection.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-29 08:12:12.000000 confection-0.1.0/confection.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      119 2023-06-29 08:12:12.000000 confection-0.1.0/confection.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       11 2023-06-29 08:12:12.000000 confection-0.1.0/confection.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-29 08:12:11.000000 confection-0.1.0/confection.egg-info/zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)       86 2023-06-29 08:12:00.000000 confection-0.1.0/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (122)     1374 2023-06-29 08:12:12.103952 confection-0.1.0/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)      154 2023-06-29 08:12:00.000000 confection-0.1.0/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-04 09:52:03.376389 confection-0.1.1/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1073 2023-08-04 09:51:50.000000 confection-0.1.1/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)       44 2023-08-04 09:51:50.000000 confection-0.1.1/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)    18936 2023-08-04 09:52:03.376389 confection-0.1.1/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)    17853 2023-08-04 09:51:50.000000 confection-0.1.1/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-04 09:52:03.376389 confection-0.1.1/confection/
+-rw-r--r--   0 vsts      (1001) docker     (122)    46687 2023-08-04 09:51:50.000000 confection-0.1.1/confection/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-08-04 09:51:50.000000 confection-0.1.1/confection/py.typed
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-04 09:52:03.376389 confection-0.1.1/confection/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-08-04 09:51:50.000000 confection-0.1.1/confection/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      489 2023-08-04 09:51:50.000000 confection-0.1.1/confection/tests/conftest.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    53301 2023-08-04 09:51:50.000000 confection-0.1.1/confection/tests/test_config.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      774 2023-08-04 09:51:50.000000 confection-0.1.1/confection/tests/test_frozen_structures.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3686 2023-08-04 09:51:50.000000 confection-0.1.1/confection/tests/util.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4074 2023-08-04 09:51:50.000000 confection-0.1.1/confection/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-04 09:52:03.376389 confection-0.1.1/confection.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)    18936 2023-08-04 09:52:03.000000 confection-0.1.1/confection.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      481 2023-08-04 09:52:03.000000 confection-0.1.1/confection.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-08-04 09:52:03.000000 confection-0.1.1/confection.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      118 2023-08-04 09:52:03.000000 confection-0.1.1/confection.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       11 2023-08-04 09:52:03.000000 confection-0.1.1/confection.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-08-04 09:52:03.000000 confection-0.1.1/confection.egg-info/zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)      118 2023-08-04 09:51:50.000000 confection-0.1.1/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (122)     1373 2023-08-04 09:52:03.376389 confection-0.1.1/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)      154 2023-08-04 09:51:50.000000 confection-0.1.1/setup.py
```

### Comparing `confection-0.1.0/LICENSE` & `confection-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `confection-0.1.0/PKG-INFO` & `confection-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: confection
-Version: 0.1.0
+Version: 0.1.1
 Summary: The sweetest config system for Python
 Home-page: https://github.com/explosion/confection
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -140,15 +140,16 @@
 ```ini
 [optimizer]
 @optimizers = "my_cool_optimizer.v1"
 learn_rate = 0.001
 gamma = 1e-8
 ```
 
-To load and parse this configuration:
+To load and parse this configuration using a `catalogue` registry (install
+[`catalogue`](https://github.com/explosion/catalogue) separately):
 
 ```python
 import dataclasses
 from typing import Union, Iterable
 import catalogue
 from confection import registry, Config
```

### Comparing `confection-0.1.0/README.md` & `confection-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -112,15 +112,16 @@
 ```ini
 [optimizer]
 @optimizers = "my_cool_optimizer.v1"
 learn_rate = 0.001
 gamma = 1e-8
 ```
 
-To load and parse this configuration:
+To load and parse this configuration using a `catalogue` registry (install
+[`catalogue`](https://github.com/explosion/catalogue) separately):
 
 ```python
 import dataclasses
 from typing import Union, Iterable
 import catalogue
 from confection import registry, Config
```

### Comparing `confection-0.1.0/confection/__init__.py` & `confection-0.1.1/confection/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,53 @@
-from typing import Union, Dict, Any, Optional, List, Tuple, Callable, Type, Mapping
-from typing import Iterable, Sequence, cast
-from types import GeneratorType
-from dataclasses import dataclass
-from configparser import ConfigParser, ExtendedInterpolation, MAX_INTERPOLATION_DEPTH
-from configparser import InterpolationMissingOptionError, InterpolationSyntaxError
-from configparser import NoSectionError, NoOptionError, InterpolationDepthError
-from configparser import ParsingError
-from pathlib import Path
-from pydantic import BaseModel, create_model, ValidationError, Extra
-from pydantic.main import ModelMetaclass
-from pydantic.fields import ModelField
-import srsly
-import catalogue
+import copy
 import inspect
 import io
-import copy
 import re
 import warnings
+from configparser import (
+    MAX_INTERPOLATION_DEPTH,
+    ConfigParser,
+    ExtendedInterpolation,
+    InterpolationDepthError,
+    InterpolationMissingOptionError,
+    InterpolationSyntaxError,
+    NoOptionError,
+    NoSectionError,
+    ParsingError,
+)
+from dataclasses import dataclass
+from pathlib import Path
+from types import GeneratorType
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    Iterable,
+    List,
+    Mapping,
+    Optional,
+    Sequence,
+    Tuple,
+    Type,
+    Union,
+    cast,
+)
+
+import srsly
+
+try:
+    from pydantic.v1 import BaseModel, Extra, ValidationError, create_model
+    from pydantic.v1.fields import ModelField
+    from pydantic.v1.main import ModelMetaclass
+except ImportError:
+    from pydantic import BaseModel, create_model, ValidationError, Extra  # type: ignore
+    from pydantic.main import ModelMetaclass  # type: ignore
+    from pydantic.fields import ModelField  # type: ignore
 
-from .util import Decorator, SimpleFrozenDict, SimpleFrozenList
+from .util import SimpleFrozenDict, SimpleFrozenList  # noqa: F401
 
 # Field used for positional arguments, e.g. [section.*.xyz]. The alias is
 # required for the schema (shouldn't clash with user-defined arg names)
 ARGS_FIELD = "*"
 ARGS_FIELD_ALIAS = "VARIABLE_POSITIONAL_ARGS"
 # Aliases for fields that would otherwise shadow pydantic attributes. Can be any
 # string, so we're using name + space so it looks the same in error messages etc.
@@ -216,15 +241,17 @@
                 continue
             parts = section.split(".")
             node = self
             for part in parts[:-1]:
                 if part == "*":
                     node = node.setdefault(part, {})
                 elif part not in node:
-                    err_title = f"Error parsing config section. Perhaps a section name is wrong?"
+                    err_title = (
+                        "Error parsing config section. Perhaps a section name is wrong?"
+                    )
                     err = [{"loc": parts, "msg": f"Section '{part}' is not defined"}]
                     raise ConfigValidationError(
                         config=self, errors=err, title=err_title
                     )
                 else:
                     node = node[part]
             if not isinstance(node, dict):
@@ -408,19 +435,15 @@
                 # they have leaf entries, as we don't want to expand
                 # blocks that are undefined
                 flattened.add_section(section_name)
             for key, value in node.items():
                 if hasattr(value, "items"):
                     # Reference to a function with no arguments, serialize
                     # inline as a dict and don't create new section
-                    if (
-                        registry.is_promise(value)
-                        and len(value) == 1
-                        and is_kwarg
-                    ):
+                    if registry.is_promise(value) and len(value) == 1 and is_kwarg:
                         flattened.set(section_name, key, try_dump_json(value, node))
                     else:
                         queue.append((path + (key,), value))
                 else:
                     flattened.set(section_name, key, try_dump_json(value, node))
         # Order so subsection follow parent (not all sections, then all subs etc.)
         flattened._sections = self._sort(flattened._sections)
```

### Comparing `confection-0.1.0/confection/tests/test_config.py` & `confection-0.1.1/confection/tests/test_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import inspect
+import pickle
 import platform
+from types import GeneratorType
+from typing import Any, Callable, Dict, Iterable, List, Optional, Tuple, Union
 
 import catalogue
 import pytest
-from typing import Dict, Optional, Iterable, Callable, Any, Union, List, Tuple
-from types import GeneratorType
-import pickle
 
-from pydantic import BaseModel, StrictFloat, PositiveInt, constr
-from pydantic.types import StrictBool
+try:
+    from pydantic.v1 import BaseModel, PositiveInt, StrictFloat, constr
+    from pydantic.v1.types import StrictBool
+except ImportError:
+    from pydantic import BaseModel, StrictFloat, PositiveInt, constr  # type: ignore
+    from pydantic.types import StrictBool  # type: ignore
 
-from confection import ConfigValidationError, Config
+from confection import Config, ConfigValidationError
+from confection.tests.util import Cat, make_tempdir, my_registry
 from confection.util import Generator, partial
-from confection.tests.util import Cat, my_registry, make_tempdir
-
 
 EXAMPLE_CONFIG = """
 [optimizer]
 @optimizers = "Adam.v1"
 beta1 = 0.9
 beta2 = 0.999
 use_averages = true
@@ -324,15 +327,15 @@
         Config().from_str(config_str)
 
 
 def test_validation_custom_types():
     def complex_args(
         rate: StrictFloat,
         steps: PositiveInt = 10,  # type: ignore
-        log_level: constr(regex="(DEBUG|INFO|WARNING|ERROR)") = "ERROR",
+        log_level: constr(regex="(DEBUG|INFO|WARNING|ERROR)") = "ERROR",  # noqa: F821
     ):
         return None
 
     my_registry.complex = catalogue.create(
         my_registry.namespace, "complex", entry_points=False
     )
     my_registry.complex("complex.v1")(complex_args)
@@ -766,15 +769,14 @@
     assert result["evil"] is False
     assert "not_evil" not in result
     result = my_registry.resolve({"cfg": config}, validate=True)["cfg"]["test"]
     assert result["not_evil"] is True
 
 
 def test_deepcopy_config():
-    numpy = pytest.importorskip("numpy")
     config = Config({"a": 1, "b": {"c": 2, "d": 3}})
     copied = config.copy()
     # Same values but not same object
     assert config == copied
     assert config is not copied
 
 
@@ -1283,14 +1285,15 @@
     assert filled["catsie"]["cute"] is True
     with pytest.raises(ConfigValidationError):
         my_registry.resolve(config, schema=BaseSchema)
     filled2 = my_registry.fill(config, schema=BaseSchema)
     assert filled2["catsie"]["cute"] is True
     resolved = my_registry.resolve(filled2)
     assert resolved["catsie"] == "meow"
+
     # With unavailable function
     class BaseSchema2(BaseModel):
         catsie: Any
         other: int = 12
 
     config = {"catsie": {"@cats": "dog", "evil": False}}
     filled3 = my_registry.fill(config, schema=BaseSchema2)
@@ -1378,28 +1381,30 @@
     overrides = {"vars.a": greeting}
     assert "${vars.a}" in str_cfg
     cfg = Config().from_str(str_cfg, overrides=overrides)
     assert expected in str(cfg)
 
 
 def test_warn_single_quotes():
-    str_cfg = f"""
+    str_cfg = """
     [project]
     commands = 'do stuff'
     """
 
     with pytest.warns(UserWarning, match="single-quoted"):
-        cfg = Config().from_str(str_cfg)
+        Config().from_str(str_cfg)
 
     # should not warn if single quotes are in the middle
-    str_cfg = f"""
+    str_cfg = """
     [project]
     commands = some'thing
     """
-    cfg = Config().from_str(str_cfg)
+    Config().from_str(str_cfg)
 
 
 def test_parse_strings_interpretable_as_ints():
     """Test whether strings interpretable as integers are parsed correctly (i. e. as strings)."""
-    cfg = Config().from_str(f"""[a]\nfoo = [${{b.bar}}, "00${{b.bar}}", "y"]\n\n[b]\nbar = 3""")
+    cfg = Config().from_str(
+        f"""[a]\nfoo = [${{b.bar}}, "00${{b.bar}}", "y"]\n\n[b]\nbar = 3"""  # noqa: F541
+    )
     assert cfg["a"]["foo"] == [3, "003", "y"]
     assert cfg["b"]["bar"] == 3
```

### Comparing `confection-0.1.0/confection/tests/test_frozen_structures.py` & `confection-0.1.1/confection/tests/test_frozen_structures.py`

 * *Files identical despite different names*

### Comparing `confection-0.1.0/confection/tests/util.py` & `confection-0.1.1/confection/tests/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,26 +2,23 @@
 Registered functions used for config tests.
 """
 import contextlib
 import dataclasses
 import shutil
 import tempfile
 from pathlib import Path
-from typing import (
-    Iterable,
-    List,
-    Union,
-    Generator,
-    Generic,
-    TypeVar,
-    Optional,
-)
-from pydantic.types import StrictBool
+from typing import Generator, Generic, Iterable, List, Optional, TypeVar, Union
 
 import catalogue
+
+try:
+    from pydantic.v1.types import StrictBool
+except ImportError:
+    from pydantic.types import StrictBool  # type: ignore
+
 import confection
 
 FloatOrSeq = Union[float, List[float], Generator]
 InT = TypeVar("InT")
 OutT = TypeVar("OutT")
```

### Comparing `confection-0.1.0/confection/util.py` & `confection-0.1.1/confection/util.py`

 * *Files identical despite different names*

### Comparing `confection-0.1.0/confection.egg-info/PKG-INFO` & `confection-0.1.1/confection.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: confection
-Version: 0.1.0
+Version: 0.1.1
 Summary: The sweetest config system for Python
 Home-page: https://github.com/explosion/confection
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -140,15 +140,16 @@
 ```ini
 [optimizer]
 @optimizers = "my_cool_optimizer.v1"
 learn_rate = 0.001
 gamma = 1e-8
 ```
 
-To load and parse this configuration:
+To load and parse this configuration using a `catalogue` registry (install
+[`catalogue`](https://github.com/explosion/catalogue) separately):
 
 ```python
 import dataclasses
 from typing import Union, Iterable
 import catalogue
 from confection import registry, Config
```

### Comparing `confection-0.1.0/setup.cfg` & `confection-0.1.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 0.1.0
+version = 0.1.1
 description = The sweetest config system for Python
 url = https://github.com/explosion/confection
 author = Explosion
 author_email = contact@explosion.ai
 license = MIT
 long_description = file: README.md
 long_description_content_type = text/markdown
@@ -26,15 +26,15 @@
 	Topic :: Scientific/Engineering
 
 [options]
 zip_safe = true
 include_package_data = true
 python_requires = >=3.6
 install_requires = 
-	pydantic>=1.7.4,!=1.8,!=1.8.1,<1.11.0
+	pydantic>=1.7.4,!=1.8,!=1.8.1,<3.0.0
 	typing_extensions>=3.7.4.1,<4.5.0; python_version < "3.8"
 	srsly>=2.4.0,<3.0.0
 
 [sdist]
 formats = gztar
 
 [flake8]
```

