# Comparing `tmp/pyfluids-2.4.0.tar.gz` & `tmp/pyfluids-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfluids-2.4.0.tar", max compression
+gzip compressed data, was "pyfluids-2.5.0.tar", max compression
```

## Comparing `pyfluids-2.4.0.tar` & `pyfluids-2.5.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1078 2023-07-04 13:52:39.912248 pyfluids-2.4.0/LICENSE
--rw-r--r--   0        0        0     1203 2023-07-04 13:52:39.912248 pyfluids-2.4.0/PyPI.md
--rw-r--r--   0        0        0      208 2023-07-04 13:52:39.920248 pyfluids-2.4.0/pyfluids/__init__.py
--rw-r--r--   0        0        0      265 2023-07-04 13:52:39.920248 pyfluids-2.4.0/pyfluids/config/__init__.py
--rw-r--r--   0        0        0      242 2023-07-04 13:52:39.920248 pyfluids-2.4.0/pyfluids/config/pyfluids_config.py
--rw-r--r--   0        0        0     3638 2023-07-04 13:52:39.920248 pyfluids-2.4.0/pyfluids/config/pyfluids_config_builder.py
--rw-r--r--   0        0        0      239 2023-07-04 13:52:39.920248 pyfluids-2.4.0/pyfluids/config/singleton.py
--rw-r--r--   0        0        0     1886 2023-07-04 13:52:39.920248 pyfluids-2.4.0/pyfluids/config/unit_converter.py
--rw-r--r--   0        0        0      341 2023-07-04 13:52:39.920248 pyfluids-2.4.0/pyfluids/config/units_system.py
--rw-r--r--   0        0        0      130 2023-07-04 13:52:39.920248 pyfluids-2.4.0/pyfluids/enums/__init__.py
--rw-r--r--   0        0        0    12938 2023-07-04 13:52:39.920248 pyfluids-2.4.0/pyfluids/enums/fluids_list.py
--rw-r--r--   0        0        0      267 2023-07-04 13:52:39.920248 pyfluids-2.4.0/pyfluids/enums/mix.py
--rw-r--r--   0        0        0      654 2023-07-04 13:52:39.920248 pyfluids-2.4.0/pyfluids/enums/phases.py
--rw-r--r--   0        0        0       87 2023-07-04 13:52:39.920248 pyfluids-2.4.0/pyfluids/fluids/__init__.py
--rw-r--r--   0        0        0    25819 2023-07-04 13:52:39.920248 pyfluids-2.4.0/pyfluids/fluids/abstract_fluid.py
--rw-r--r--   0        0        0     3665 2023-07-04 13:52:39.920248 pyfluids-2.4.0/pyfluids/fluids/fluid.py
--rw-r--r--   0        0        0     3419 2023-07-04 13:52:39.920248 pyfluids-2.4.0/pyfluids/fluids/mixture.py
--rw-r--r--   0        0        0       54 2023-07-04 13:52:39.920248 pyfluids-2.4.0/pyfluids/humid_air/__init__.py
--rw-r--r--   0        0        0    24476 2023-07-04 13:52:39.920248 pyfluids-2.4.0/pyfluids/humid_air/humid_air.py
--rw-r--r--   0        0        0      164 2023-07-04 13:52:39.920248 pyfluids-2.4.0/pyfluids/io/__init__.py
--rw-r--r--   0        0        0      999 2023-07-04 13:52:39.920248 pyfluids-2.4.0/pyfluids/io/abstract_input.py
--rw-r--r--   0        0        0     2886 2023-07-04 13:52:39.920248 pyfluids-2.4.0/pyfluids/io/input.py
--rw-r--r--   0        0        0     4758 2023-07-04 13:52:39.920248 pyfluids-2.4.0/pyfluids/io/input_humid_air.py
--rw-r--r--   0        0        0      481 2023-07-04 13:52:39.920248 pyfluids-2.4.0/pyfluids/io/outputs_validator.py
--rw-r--r--   0        0        0     2050 2023-07-04 13:52:39.920248 pyfluids-2.4.0/pyproject.toml
--rw-r--r--   0        0        0     3111 1970-01-01 00:00:00.000000 pyfluids-2.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-08-04 21:41:37.934060 pyfluids-2.5.0/LICENSE
+-rw-r--r--   0        0        0     1203 2023-08-04 21:41:37.934060 pyfluids-2.5.0/PyPI.md
+-rw-r--r--   0        0        0      208 2023-08-04 21:41:37.942060 pyfluids-2.5.0/pyfluids/__init__.py
+-rw-r--r--   0        0        0      265 2023-08-04 21:41:37.942060 pyfluids-2.5.0/pyfluids/config/__init__.py
+-rw-r--r--   0        0        0      242 2023-08-04 21:41:37.942060 pyfluids-2.5.0/pyfluids/config/pyfluids_config.py
+-rw-r--r--   0        0        0     3638 2023-08-04 21:41:37.942060 pyfluids-2.5.0/pyfluids/config/pyfluids_config_builder.py
+-rw-r--r--   0        0        0      239 2023-08-04 21:41:37.942060 pyfluids-2.5.0/pyfluids/config/singleton.py
+-rw-r--r--   0        0        0     1886 2023-08-04 21:41:37.942060 pyfluids-2.5.0/pyfluids/config/unit_converter.py
+-rw-r--r--   0        0        0      341 2023-08-04 21:41:37.942060 pyfluids-2.5.0/pyfluids/config/units_system.py
+-rw-r--r--   0        0        0      130 2023-08-04 21:41:37.942060 pyfluids-2.5.0/pyfluids/enums/__init__.py
+-rw-r--r--   0        0        0    12938 2023-08-04 21:41:37.942060 pyfluids-2.5.0/pyfluids/enums/fluids_list.py
+-rw-r--r--   0        0        0      267 2023-08-04 21:41:37.942060 pyfluids-2.5.0/pyfluids/enums/mix.py
+-rw-r--r--   0        0        0      654 2023-08-04 21:41:37.942060 pyfluids-2.5.0/pyfluids/enums/phases.py
+-rw-r--r--   0        0        0       87 2023-08-04 21:41:37.942060 pyfluids-2.5.0/pyfluids/fluids/__init__.py
+-rw-r--r--   0        0        0    26224 2023-08-04 21:41:37.942060 pyfluids-2.5.0/pyfluids/fluids/abstract_fluid.py
+-rw-r--r--   0        0        0     3665 2023-08-04 21:41:37.942060 pyfluids-2.5.0/pyfluids/fluids/fluid.py
+-rw-r--r--   0        0        0     3419 2023-08-04 21:41:37.942060 pyfluids-2.5.0/pyfluids/fluids/mixture.py
+-rw-r--r--   0        0        0       54 2023-08-04 21:41:37.942060 pyfluids-2.5.0/pyfluids/humid_air/__init__.py
+-rw-r--r--   0        0        0    24476 2023-08-04 21:41:37.942060 pyfluids-2.5.0/pyfluids/humid_air/humid_air.py
+-rw-r--r--   0        0        0      164 2023-08-04 21:41:37.942060 pyfluids-2.5.0/pyfluids/io/__init__.py
+-rw-r--r--   0        0        0      999 2023-08-04 21:41:37.942060 pyfluids-2.5.0/pyfluids/io/abstract_input.py
+-rw-r--r--   0        0        0     2886 2023-08-04 21:41:37.942060 pyfluids-2.5.0/pyfluids/io/input.py
+-rw-r--r--   0        0        0     4758 2023-08-04 21:41:37.942060 pyfluids-2.5.0/pyfluids/io/input_humid_air.py
+-rw-r--r--   0        0        0      481 2023-08-04 21:41:37.942060 pyfluids-2.5.0/pyfluids/io/outputs_validator.py
+-rw-r--r--   0        0        0     2050 2023-08-04 21:41:37.942060 pyfluids-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3111 1970-01-01 00:00:00.000000 pyfluids-2.5.0/PKG-INFO
```

### Comparing `pyfluids-2.4.0/LICENSE` & `pyfluids-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfluids-2.4.0/PyPI.md` & `pyfluids-2.5.0/PyPI.md`

 * *Files identical despite different names*

### Comparing `pyfluids-2.4.0/pyfluids/config/pyfluids_config_builder.py` & `pyfluids-2.5.0/pyfluids/config/pyfluids_config_builder.py`

 * *Files identical despite different names*

### Comparing `pyfluids-2.4.0/pyfluids/config/unit_converter.py` & `pyfluids-2.5.0/pyfluids/config/unit_converter.py`

 * *Files identical despite different names*

### Comparing `pyfluids-2.4.0/pyfluids/enums/fluids_list.py` & `pyfluids-2.5.0/pyfluids/enums/fluids_list.py`

 * *Files identical despite different names*

### Comparing `pyfluids-2.4.0/pyfluids/enums/phases.py` & `pyfluids-2.5.0/pyfluids/enums/phases.py`

 * *Files identical despite different names*

### Comparing `pyfluids-2.4.0/pyfluids/fluids/abstract_fluid.py` & `pyfluids-2.5.0/pyfluids/fluids/abstract_fluid.py`

 * *Files 1% similar despite different names*

```diff
@@ -361,14 +361,29 @@
         self.__pressure = None
         self.__quality = None
         self.__sound_speed = None
         self.__specific_heat = None
         self.__surface_tension = None
         self.__temperature = None
 
+    def specify_phase(self, phase: Phases):
+        """
+        Specify the phase state for all further calculations.
+
+        :param phase: Phase state.
+        """
+        self._backend.specify_phase(phase.value)
+
+    def unspecify_phase(self):
+        """
+        Unspecify the phase state and
+        go back to calculating it based on the inputs.
+        """
+        self._backend.unspecify_phase()
+
     def isentropic_compression_to_pressure(self, pressure: float) -> AbstractFluid:
         """
         The process of isentropic compression to a given pressure.
 
         :param pressure: Absolute pressure [Pa].
         :return: The state of the fluid at the end of the process.
         :raises ValueError: If pressure is invalid.
```

### Comparing `pyfluids-2.4.0/pyfluids/fluids/fluid.py` & `pyfluids-2.5.0/pyfluids/fluids/fluid.py`

 * *Files identical despite different names*

### Comparing `pyfluids-2.4.0/pyfluids/fluids/mixture.py` & `pyfluids-2.5.0/pyfluids/fluids/mixture.py`

 * *Files identical despite different names*

### Comparing `pyfluids-2.4.0/pyfluids/humid_air/humid_air.py` & `pyfluids-2.5.0/pyfluids/humid_air/humid_air.py`

 * *Files identical despite different names*

### Comparing `pyfluids-2.4.0/pyfluids/io/abstract_input.py` & `pyfluids-2.5.0/pyfluids/io/abstract_input.py`

 * *Files identical despite different names*

### Comparing `pyfluids-2.4.0/pyfluids/io/input.py` & `pyfluids-2.5.0/pyfluids/io/input.py`

 * *Files identical despite different names*

### Comparing `pyfluids-2.4.0/pyfluids/io/input_humid_air.py` & `pyfluids-2.5.0/pyfluids/io/input_humid_air.py`

 * *Files identical despite different names*

### Comparing `pyfluids-2.4.0/pyproject.toml` & `pyfluids-2.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyfluids"
-version = "2.4.0"
+version = "2.5.0"
 description = "A simple, full-featured, lightweight CoolProp wrapper for Python"
 authors = [
     "Vladimir Portyanikhin <v.portyanikhin@ya.ru>",
 ]
 license = "MIT"
 readme = "PyPI.md"
 homepage = "https://github.com/portyanikhin/PyFluids"
@@ -55,13 +55,13 @@
 [tool.poetry.dependencies]
 python = ">=3.7, <3.12"
 CoolProp = "6.4.3.post1"
 tomli = "2.0.1"
 
 [tool.poetry.group.test.dependencies]
 pytest = "7.4.0"
-pytest-asyncio = "0.21.0"
+pytest-asyncio = "0.21.1"
 pytest-cov = "4.1.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pyfluids-2.4.0/PKG-INFO` & `pyfluids-2.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfluids
-Version: 2.4.0
+Version: 2.5.0
 Summary: A simple, full-featured, lightweight CoolProp wrapper for Python
 Home-page: https://github.com/portyanikhin/PyFluids
 License: MIT
 Keywords: CoolProp,fluids,mixtures,humid,air,thermophysical,properties,thermodynamics
 Author: Vladimir Portyanikhin
 Author-email: v.portyanikhin@ya.ru
 Requires-Python: >=3.7,<3.12
```

