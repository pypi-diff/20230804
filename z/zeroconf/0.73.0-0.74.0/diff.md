# Comparing `tmp/zeroconf-0.73.0.tar.gz` & `tmp/zeroconf-0.74.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeroconf-0.73.0.tar", max compression
+gzip compressed data, was "zeroconf-0.74.0.tar", max compression
```

## Comparing `zeroconf-0.73.0.tar` & `zeroconf-0.74.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0    57738 2023-08-03 23:49:30.895270 zeroconf-0.73.0/CHANGELOG.md
--rw-r--r--   0        0        0    24380 2023-08-03 23:49:30.011251 zeroconf-0.73.0/COPYING
--rw-r--r--   0        0        0     4407 2023-08-03 23:49:30.011251 zeroconf-0.73.0/README.rst
--rw-r--r--   0        0        0     1060 2023-08-03 23:49:30.011251 zeroconf-0.73.0/build_ext.py
--rw-r--r--   0        0        0     6770 2023-08-03 23:49:30.011251 zeroconf-0.73.0/docs/Makefile
--rw-r--r--   0        0        0      234 2023-08-03 23:49:30.011251 zeroconf-0.73.0/docs/api.rst
--rw-r--r--   0        0        0     8145 2023-08-03 23:49:30.011251 zeroconf-0.73.0/docs/conf.py
--rw-r--r--   0        0        0      991 2023-08-03 23:49:30.011251 zeroconf-0.73.0/docs/index.rst
--rw-r--r--   0        0        0     3995 2023-08-03 23:49:30.983272 zeroconf-0.73.0/pyproject.toml
--rw-r--r--   0        0        0     3868 2023-08-03 23:49:30.915271 zeroconf-0.73.0/src/zeroconf/__init__.py
--rw-r--r--   0        0        0      897 2023-08-03 23:49:30.015251 zeroconf-0.73.0/src/zeroconf/_cache.pxd
--rw-r--r--   0        0        0    10040 2023-08-03 23:49:30.015251 zeroconf-0.73.0/src/zeroconf/_cache.py
--rw-r--r--   0        0        0    39600 2023-08-03 23:49:30.015251 zeroconf-0.73.0/src/zeroconf/_core.py
--rw-r--r--   0        0        0     2480 2023-08-03 23:49:30.015251 zeroconf-0.73.0/src/zeroconf/_dns.pxd
--rw-r--r--   0        0        0    18381 2023-08-03 23:49:30.015251 zeroconf-0.73.0/src/zeroconf/_dns.py
--rw-r--r--   0        0        0     2167 2023-08-03 23:49:30.015251 zeroconf-0.73.0/src/zeroconf/_exceptions.py
--rw-r--r--   0        0        0    24697 2023-08-03 23:49:30.015251 zeroconf-0.73.0/src/zeroconf/_handlers.py
--rw-r--r--   0        0        0     2916 2023-08-03 23:49:30.015251 zeroconf-0.73.0/src/zeroconf/_history.py
--rw-r--r--   0        0        0     2980 2023-08-03 23:49:30.015251 zeroconf-0.73.0/src/zeroconf/_logger.py
--rw-r--r--   0        0        0      971 2023-08-03 23:49:30.015251 zeroconf-0.73.0/src/zeroconf/_protocol/__init__.py
--rw-r--r--   0        0        0     2661 2023-08-03 23:49:30.015251 zeroconf-0.73.0/src/zeroconf/_protocol/incoming.pxd
--rw-r--r--   0        0        0    14353 2023-08-03 23:49:30.015251 zeroconf-0.73.0/src/zeroconf/_protocol/incoming.py
--rw-r--r--   0        0        0     2317 2023-08-03 23:49:30.015251 zeroconf-0.73.0/src/zeroconf/_protocol/outgoing.pxd
--rw-r--r--   0        0        0    17896 2023-08-03 23:49:30.015251 zeroconf-0.73.0/src/zeroconf/_protocol/outgoing.py
--rw-r--r--   0        0        0     2419 2023-08-03 23:49:30.015251 zeroconf-0.73.0/src/zeroconf/_services/__init__.py
--rw-r--r--   0        0        0    23045 2023-08-03 23:49:30.015251 zeroconf-0.73.0/src/zeroconf/_services/browser.py
--rw-r--r--   0        0        0    28331 2023-08-03 23:49:30.015251 zeroconf-0.73.0/src/zeroconf/_services/info.py
--rw-r--r--   0        0        0     3999 2023-08-03 23:49:30.015251 zeroconf-0.73.0/src/zeroconf/_services/registry.py
--rw-r--r--   0        0        0     3003 2023-08-03 23:49:30.015251 zeroconf-0.73.0/src/zeroconf/_services/types.py
--rw-r--r--   0        0        0     2909 2023-08-03 23:49:30.015251 zeroconf-0.73.0/src/zeroconf/_updates.py
--rw-r--r--   0        0        0      971 2023-08-03 23:49:30.015251 zeroconf-0.73.0/src/zeroconf/_utils/__init__.py
--rw-r--r--   0        0        0     4144 2023-08-03 23:49:30.015251 zeroconf-0.73.0/src/zeroconf/_utils/asyncio.py
--rw-r--r--   0        0        0     6928 2023-08-03 23:49:30.015251 zeroconf-0.73.0/src/zeroconf/_utils/name.py
--rw-r--r--   0        0        0    15252 2023-08-03 23:49:30.015251 zeroconf-0.73.0/src/zeroconf/_utils/net.py
--rw-r--r--   0        0        0     1308 2023-08-03 23:49:30.015251 zeroconf-0.73.0/src/zeroconf/_utils/time.py
--rw-r--r--   0        0        0    11084 2023-08-03 23:49:30.015251 zeroconf-0.73.0/src/zeroconf/asyncio.py
--rw-r--r--   0        0        0     4515 2023-08-03 23:49:30.015251 zeroconf-0.73.0/src/zeroconf/const.py
--rw-r--r--   0        0        0        0 2023-08-03 23:49:30.015251 zeroconf-0.73.0/src/zeroconf/py.typed
--rw-r--r--   0        0        0     2416 2023-08-03 23:49:30.015251 zeroconf-0.73.0/tests/__init__.py
--rw-r--r--   0        0        0     1057 2023-08-03 23:49:30.015251 zeroconf-0.73.0/tests/conftest.py
--rw-r--r--   0        0        0      971 2023-08-03 23:49:30.015251 zeroconf-0.73.0/tests/services/__init__.py
--rw-r--r--   0        0        0    42949 2023-08-03 23:49:30.019251 zeroconf-0.73.0/tests/services/test_browser.py
--rw-r--r--   0        0        0    49788 2023-08-03 23:49:30.019251 zeroconf-0.73.0/tests/services/test_info.py
--rw-r--r--   0        0        0     4157 2023-08-03 23:49:30.019251 zeroconf-0.73.0/tests/services/test_registry.py
--rw-r--r--   0        0        0     4677 2023-08-03 23:49:30.019251 zeroconf-0.73.0/tests/services/test_types.py
--rw-r--r--   0        0        0    44525 2023-08-03 23:49:30.019251 zeroconf-0.73.0/tests/test_asyncio.py
--rw-r--r--   0        0        0     8830 2023-08-03 23:49:30.019251 zeroconf-0.73.0/tests/test_cache.py
--rw-r--r--   0        0        0    32599 2023-08-03 23:49:30.019251 zeroconf-0.73.0/tests/test_core.py
--rw-r--r--   0        0        0    14686 2023-08-03 23:49:30.019251 zeroconf-0.73.0/tests/test_dns.py
--rw-r--r--   0        0        0     5021 2023-08-03 23:49:30.019251 zeroconf-0.73.0/tests/test_exceptions.py
--rw-r--r--   0        0        0    67411 2023-08-03 23:49:30.019251 zeroconf-0.73.0/tests/test_handlers.py
--rw-r--r--   0        0        0     2580 2023-08-03 23:49:30.019251 zeroconf-0.73.0/tests/test_history.py
--rw-r--r--   0        0        0     6640 2023-08-03 23:49:30.019251 zeroconf-0.73.0/tests/test_init.py
--rw-r--r--   0        0        0     3396 2023-08-03 23:49:30.019251 zeroconf-0.73.0/tests/test_logger.py
--rw-r--r--   0        0        0    41672 2023-08-03 23:49:30.019251 zeroconf-0.73.0/tests/test_protocol.py
--rw-r--r--   0        0        0     8849 2023-08-03 23:49:30.019251 zeroconf-0.73.0/tests/test_services.py
--rw-r--r--   0        0        0     2240 2023-08-03 23:49:30.019251 zeroconf-0.73.0/tests/test_updates.py
--rw-r--r--   0        0        0      971 2023-08-03 23:49:30.019251 zeroconf-0.73.0/tests/utils/__init__.py
--rw-r--r--   0        0        0     5101 2023-08-03 23:49:30.019251 zeroconf-0.73.0/tests/utils/test_asyncio.py
--rw-r--r--   0        0        0     2045 2023-08-03 23:49:30.019251 zeroconf-0.73.0/tests/utils/test_name.py
--rw-r--r--   0        0        0     9413 2023-08-03 23:49:30.019251 zeroconf-0.73.0/tests/utils/test_net.py
--rw-r--r--   0        0        0     5527 1970-01-01 00:00:00.000000 zeroconf-0.73.0/setup.py
--rw-r--r--   0        0        0     6045 1970-01-01 00:00:00.000000 zeroconf-0.73.0/PKG-INFO
+-rw-r--r--   0        0        0    58259 2023-08-04 00:45:26.473501 zeroconf-0.74.0/CHANGELOG.md
+-rw-r--r--   0        0        0    24380 2023-08-04 00:45:25.393493 zeroconf-0.74.0/COPYING
+-rw-r--r--   0        0        0     4407 2023-08-04 00:45:25.393493 zeroconf-0.74.0/README.rst
+-rw-r--r--   0        0        0     1060 2023-08-04 00:45:25.393493 zeroconf-0.74.0/build_ext.py
+-rw-r--r--   0        0        0     6770 2023-08-04 00:45:25.393493 zeroconf-0.74.0/docs/Makefile
+-rw-r--r--   0        0        0      234 2023-08-04 00:45:25.393493 zeroconf-0.74.0/docs/api.rst
+-rw-r--r--   0        0        0     8145 2023-08-04 00:45:25.393493 zeroconf-0.74.0/docs/conf.py
+-rw-r--r--   0        0        0      991 2023-08-04 00:45:25.393493 zeroconf-0.74.0/docs/index.rst
+-rw-r--r--   0        0        0     3995 2023-08-04 00:45:26.553502 zeroconf-0.74.0/pyproject.toml
+-rw-r--r--   0        0        0     3868 2023-08-04 00:45:26.485501 zeroconf-0.74.0/src/zeroconf/__init__.py
+-rw-r--r--   0        0        0      897 2023-08-04 00:45:25.393493 zeroconf-0.74.0/src/zeroconf/_cache.pxd
+-rw-r--r--   0        0        0    10040 2023-08-04 00:45:25.393493 zeroconf-0.74.0/src/zeroconf/_cache.py
+-rw-r--r--   0        0        0    39600 2023-08-04 00:45:25.393493 zeroconf-0.74.0/src/zeroconf/_core.py
+-rw-r--r--   0        0        0     2480 2023-08-04 00:45:25.393493 zeroconf-0.74.0/src/zeroconf/_dns.pxd
+-rw-r--r--   0        0        0    18400 2023-08-04 00:45:25.393493 zeroconf-0.74.0/src/zeroconf/_dns.py
+-rw-r--r--   0        0        0     2167 2023-08-04 00:45:25.393493 zeroconf-0.74.0/src/zeroconf/_exceptions.py
+-rw-r--r--   0        0        0    24697 2023-08-04 00:45:25.393493 zeroconf-0.74.0/src/zeroconf/_handlers.py
+-rw-r--r--   0        0        0     2916 2023-08-04 00:45:25.393493 zeroconf-0.74.0/src/zeroconf/_history.py
+-rw-r--r--   0        0        0     2980 2023-08-04 00:45:25.393493 zeroconf-0.74.0/src/zeroconf/_logger.py
+-rw-r--r--   0        0        0      971 2023-08-04 00:45:25.393493 zeroconf-0.74.0/src/zeroconf/_protocol/__init__.py
+-rw-r--r--   0        0        0     2661 2023-08-04 00:45:25.393493 zeroconf-0.74.0/src/zeroconf/_protocol/incoming.pxd
+-rw-r--r--   0        0        0    14353 2023-08-04 00:45:25.397493 zeroconf-0.74.0/src/zeroconf/_protocol/incoming.py
+-rw-r--r--   0        0        0     2317 2023-08-04 00:45:25.397493 zeroconf-0.74.0/src/zeroconf/_protocol/outgoing.pxd
+-rw-r--r--   0        0        0    17896 2023-08-04 00:45:25.397493 zeroconf-0.74.0/src/zeroconf/_protocol/outgoing.py
+-rw-r--r--   0        0        0     2419 2023-08-04 00:45:25.397493 zeroconf-0.74.0/src/zeroconf/_services/__init__.py
+-rw-r--r--   0        0        0    23045 2023-08-04 00:45:25.397493 zeroconf-0.74.0/src/zeroconf/_services/browser.py
+-rw-r--r--   0        0        0    29106 2023-08-04 00:45:25.397493 zeroconf-0.74.0/src/zeroconf/_services/info.py
+-rw-r--r--   0        0        0     3999 2023-08-04 00:45:25.397493 zeroconf-0.74.0/src/zeroconf/_services/registry.py
+-rw-r--r--   0        0        0     3003 2023-08-04 00:45:25.397493 zeroconf-0.74.0/src/zeroconf/_services/types.py
+-rw-r--r--   0        0        0     2909 2023-08-04 00:45:25.397493 zeroconf-0.74.0/src/zeroconf/_updates.py
+-rw-r--r--   0        0        0      971 2023-08-04 00:45:25.397493 zeroconf-0.74.0/src/zeroconf/_utils/__init__.py
+-rw-r--r--   0        0        0     4144 2023-08-04 00:45:25.397493 zeroconf-0.74.0/src/zeroconf/_utils/asyncio.py
+-rw-r--r--   0        0        0     6928 2023-08-04 00:45:25.397493 zeroconf-0.74.0/src/zeroconf/_utils/name.py
+-rw-r--r--   0        0        0    15252 2023-08-04 00:45:25.397493 zeroconf-0.74.0/src/zeroconf/_utils/net.py
+-rw-r--r--   0        0        0     1308 2023-08-04 00:45:25.397493 zeroconf-0.74.0/src/zeroconf/_utils/time.py
+-rw-r--r--   0        0        0    11084 2023-08-04 00:45:25.397493 zeroconf-0.74.0/src/zeroconf/asyncio.py
+-rw-r--r--   0        0        0     4515 2023-08-04 00:45:25.397493 zeroconf-0.74.0/src/zeroconf/const.py
+-rw-r--r--   0        0        0        0 2023-08-04 00:45:25.397493 zeroconf-0.74.0/src/zeroconf/py.typed
+-rw-r--r--   0        0        0     2416 2023-08-04 00:45:25.397493 zeroconf-0.74.0/tests/__init__.py
+-rw-r--r--   0        0        0     1057 2023-08-04 00:45:25.397493 zeroconf-0.74.0/tests/conftest.py
+-rw-r--r--   0        0        0      971 2023-08-04 00:45:25.397493 zeroconf-0.74.0/tests/services/__init__.py
+-rw-r--r--   0        0        0    42949 2023-08-04 00:45:25.397493 zeroconf-0.74.0/tests/services/test_browser.py
+-rw-r--r--   0        0        0    49788 2023-08-04 00:45:25.397493 zeroconf-0.74.0/tests/services/test_info.py
+-rw-r--r--   0        0        0     4157 2023-08-04 00:45:25.397493 zeroconf-0.74.0/tests/services/test_registry.py
+-rw-r--r--   0        0        0     4677 2023-08-04 00:45:25.397493 zeroconf-0.74.0/tests/services/test_types.py
+-rw-r--r--   0        0        0    44525 2023-08-04 00:45:25.397493 zeroconf-0.74.0/tests/test_asyncio.py
+-rw-r--r--   0        0        0     8830 2023-08-04 00:45:25.397493 zeroconf-0.74.0/tests/test_cache.py
+-rw-r--r--   0        0        0    32599 2023-08-04 00:45:25.397493 zeroconf-0.74.0/tests/test_core.py
+-rw-r--r--   0        0        0    14686 2023-08-04 00:45:25.397493 zeroconf-0.74.0/tests/test_dns.py
+-rw-r--r--   0        0        0     5021 2023-08-04 00:45:25.397493 zeroconf-0.74.0/tests/test_exceptions.py
+-rw-r--r--   0        0        0    67411 2023-08-04 00:45:25.397493 zeroconf-0.74.0/tests/test_handlers.py
+-rw-r--r--   0        0        0     2580 2023-08-04 00:45:25.397493 zeroconf-0.74.0/tests/test_history.py
+-rw-r--r--   0        0        0     6640 2023-08-04 00:45:25.397493 zeroconf-0.74.0/tests/test_init.py
+-rw-r--r--   0        0        0     3396 2023-08-04 00:45:25.397493 zeroconf-0.74.0/tests/test_logger.py
+-rw-r--r--   0        0        0    41672 2023-08-04 00:45:25.397493 zeroconf-0.74.0/tests/test_protocol.py
+-rw-r--r--   0        0        0     8849 2023-08-04 00:45:25.397493 zeroconf-0.74.0/tests/test_services.py
+-rw-r--r--   0        0        0     2240 2023-08-04 00:45:25.397493 zeroconf-0.74.0/tests/test_updates.py
+-rw-r--r--   0        0        0      971 2023-08-04 00:45:25.397493 zeroconf-0.74.0/tests/utils/__init__.py
+-rw-r--r--   0        0        0     5101 2023-08-04 00:45:25.397493 zeroconf-0.74.0/tests/utils/test_asyncio.py
+-rw-r--r--   0        0        0     2045 2023-08-04 00:45:25.397493 zeroconf-0.74.0/tests/utils/test_name.py
+-rw-r--r--   0        0        0     9413 2023-08-04 00:45:25.397493 zeroconf-0.74.0/tests/utils/test_net.py
+-rw-r--r--   0        0        0     5527 1970-01-01 00:00:00.000000 zeroconf-0.74.0/setup.py
+-rw-r--r--   0        0        0     6045 1970-01-01 00:00:00.000000 zeroconf-0.74.0/PKG-INFO
```

### Comparing `zeroconf-0.73.0/CHANGELOG.md` & `zeroconf-0.74.0/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.74.0 (2023-08-04)
+
+### Feature
+
+* Speed up unpacking text records in ServiceInfo ([#1212](https://github.com/python-zeroconf/python-zeroconf/issues/1212)) ([`99a6f98`](https://github.com/python-zeroconf/python-zeroconf/commit/99a6f98e44a1287ba537eabb852b1b69923402f0))
+
+### Fix
+
+* Remove typing on reset_ttl for cython compat ([#1213](https://github.com/python-zeroconf/python-zeroconf/issues/1213)) ([`0094e26`](https://github.com/python-zeroconf/python-zeroconf/commit/0094e2684344c6b7edd7948924f093f1b4c19901))
+
 ## v0.73.0 (2023-08-03)
 
 ### Feature
 
 * Add a cache to service_type_name ([#1211](https://github.com/python-zeroconf/python-zeroconf/issues/1211)) ([`53a694f`](https://github.com/python-zeroconf/python-zeroconf/commit/53a694f60e675ae0560e727be6b721b401c2b68f))
 
 ## v0.72.3 (2023-08-03)
```

### Comparing `zeroconf-0.73.0/COPYING` & `zeroconf-0.74.0/COPYING`

 * *Files identical despite different names*

### Comparing `zeroconf-0.73.0/README.rst` & `zeroconf-0.74.0/README.rst`

 * *Files identical despite different names*

### Comparing `zeroconf-0.73.0/build_ext.py` & `zeroconf-0.74.0/build_ext.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.73.0/docs/Makefile` & `zeroconf-0.74.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `zeroconf-0.73.0/docs/conf.py` & `zeroconf-0.74.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.73.0/docs/index.rst` & `zeroconf-0.74.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `zeroconf-0.73.0/pyproject.toml` & `zeroconf-0.74.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zeroconf"
-version = "0.73.0"
+version = "0.74.0"
 description = "A pure python implementation of multicast DNS service discovery"
 authors = ["Paul Scott-Murphy", "William McBrine", "Jakub Stasiak", "J. Nick Koston"]
 license = "LGPL"
 readme = "README.rst"
 repository = "https://github.com/python-zeroconf/python-zeroconf"
 documentation = "https://python-zeroconf.readthedocs.io"
 classifiers=[
```

### Comparing `zeroconf-0.73.0/src/zeroconf/__init__.py` & `zeroconf-0.74.0/src/zeroconf/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 from ._utils.time import (  # noqa # import needed for backwards compat
     current_time_millis,
     millis_to_seconds,
 )
 
 __author__ = 'Paul Scott-Murphy, William McBrine'
 __maintainer__ = 'Jakub Stasiak <jakub@stasiak.at>'
-__version__ = '0.73.0'
+__version__ = '0.74.0'
 __license__ = 'LGPL'
 
 
 __all__ = [
     "__version__",
     "Zeroconf",
     "ServiceInfo",
```

### Comparing `zeroconf-0.73.0/src/zeroconf/_cache.pxd` & `zeroconf-0.74.0/src/zeroconf/_cache.pxd`

 * *Files identical despite different names*

### Comparing `zeroconf-0.73.0/src/zeroconf/_cache.py` & `zeroconf-0.74.0/src/zeroconf/_cache.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.73.0/src/zeroconf/_core.py` & `zeroconf-0.74.0/src/zeroconf/_core.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.73.0/src/zeroconf/_dns.pxd` & `zeroconf-0.74.0/src/zeroconf/_dns.pxd`

 * *Files identical despite different names*

### Comparing `zeroconf-0.73.0/src/zeroconf/_dns.py` & `zeroconf-0.74.0/src/zeroconf/_dns.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,15 +203,15 @@
         """Returns true if this record is at least half way expired."""
         return self.created + (_EXPIRE_STALE_TIME_MS * self.ttl) <= now
 
     def is_recent(self, now: _float) -> bool:
         """Returns true if the record more than one quarter of its TTL remaining."""
         return self.created + (_RECENT_TIME_MS * self.ttl) > now
 
-    def reset_ttl(self, other: 'DNSRecord') -> None:
+    def reset_ttl(self, other) -> None:  # type: ignore[no-untyped-def]
         """Sets this record's TTL and created time to that of
         another record."""
         self.set_created_ttl(other.created, other.ttl)
 
     def set_created_ttl(self, created: float, ttl: Union[float, int]) -> None:
         """Set the created and ttl of a record."""
         self.created = created
```

### Comparing `zeroconf-0.73.0/src/zeroconf/_exceptions.py` & `zeroconf-0.74.0/src/zeroconf/_exceptions.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.73.0/src/zeroconf/_handlers.py` & `zeroconf-0.74.0/src/zeroconf/_handlers.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.73.0/src/zeroconf/_history.py` & `zeroconf-0.74.0/src/zeroconf/_history.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.73.0/src/zeroconf/_logger.py` & `zeroconf-0.74.0/src/zeroconf/_logger.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.73.0/src/zeroconf/_protocol/__init__.py` & `zeroconf-0.74.0/src/zeroconf/_protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.73.0/src/zeroconf/_protocol/incoming.pxd` & `zeroconf-0.74.0/src/zeroconf/_protocol/incoming.pxd`

 * *Files identical despite different names*

### Comparing `zeroconf-0.73.0/src/zeroconf/_protocol/incoming.py` & `zeroconf-0.74.0/src/zeroconf/_protocol/incoming.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.73.0/src/zeroconf/_protocol/outgoing.pxd` & `zeroconf-0.74.0/src/zeroconf/_protocol/outgoing.pxd`

 * *Files identical despite different names*

### Comparing `zeroconf-0.73.0/src/zeroconf/_protocol/outgoing.py` & `zeroconf-0.74.0/src/zeroconf/_protocol/outgoing.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.73.0/src/zeroconf/_services/__init__.py` & `zeroconf-0.74.0/src/zeroconf/_services/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.73.0/src/zeroconf/_services/browser.py` & `zeroconf-0.74.0/src/zeroconf/_services/browser.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.73.0/src/zeroconf/_services/info.py` & `zeroconf-0.74.0/src/zeroconf/_services/info.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,15 +168,15 @@
         elif parsed_addresses is not None:
             self.addresses = [_encode_address(a) for a in parsed_addresses]
         self.port = port
         self.weight = weight
         self.priority = priority
         self.server = server if server else None
         self.server_key = server.lower() if server else None
-        self._properties: Dict[Union[str, bytes], Optional[Union[str, bytes]]] = {}
+        self._properties: Optional[Dict[Union[str, bytes], Optional[Union[str, bytes]]]] = None
         if isinstance(properties, bytes):
             self._set_text(properties)
         else:
             self._set_properties(properties)
         self.host_ttl = host_ttl
         self.other_ttl = other_ttl
         self.interface_index = interface_index
@@ -222,22 +222,26 @@
                 )
             if addr.version == 4:
                 self._ipv4_addresses.append(addr)
             else:
                 self._ipv6_addresses.append(addr)
 
     @property
-    def properties(self) -> Dict:
+    def properties(self) -> Dict[Union[str, bytes], Optional[Union[str, bytes]]]:
         """If properties were set in the constructor this property returns the original dictionary
         of type `Dict[Union[bytes, str], Any]`.
 
         If properties are coming from the network, after decoding a TXT record, the keys are always
         bytes and the values are either bytes, if there was a value, even empty, or `None`, if there
         was none. No further decoding is attempted. The type returned is `Dict[bytes, Optional[bytes]]`.
         """
+        if self._properties is None:
+            self._unpack_text_into_properties()
+        if TYPE_CHECKING:
+            assert self._properties is not None
         return self._properties
 
     async def async_wait(self, timeout: float) -> None:
         """Calling task waits for a given number of milliseconds or until notified."""
         loop = asyncio.get_running_loop()
         future = loop.create_future()
         self._new_records_futures.append(future)
@@ -313,18 +317,18 @@
         if self.interface_index is None:
             return self.parsed_addresses(version)
         return [
             f"{addr}%{self.interface_index}" if addr.version == 6 and addr.is_link_local else str(addr)
             for addr in self._ip_addresses_by_version_value(version.value)
         ]
 
-    def _set_properties(self, properties: Dict) -> None:
+    def _set_properties(self, properties: Dict[Union[str, bytes], Optional[Union[str, bytes]]]) -> None:
         """Sets properties and text of this info from a dictionary"""
         self._properties = properties
-        list_ = []
+        list_: List[bytes] = []
         result = b''
         for key, value in properties.items():
             if isinstance(key, str):
                 key = key.encode('utf-8')
 
             record = key
             if value is not None:
@@ -334,42 +338,56 @@
             list_.append(record)
         for item in list_:
             result = b''.join((result, bytes((len(item),)), item))
         self.text = result
 
     def _set_text(self, text: bytes) -> None:
         """Sets properties and text given a text field"""
+        if text == self.text:
+            return
         self.text = text
+        # Clear the properties cache
+        self._properties = None
+
+    def _unpack_text_into_properties(self) -> None:
+        """Unpacks the text field into properties"""
+        text = self.text
         end = len(text)
         if end == 0:
+            # Properties should be set atomically
+            # in case another thread is reading them
             self._properties = {}
             return
+
         result: Dict[Union[str, bytes], Optional[Union[str, bytes]]] = {}
         index = 0
-        strs = []
+        strs: List[bytes] = []
         while index < end:
             length = text[index]
             index += 1
             strs.append(text[index : index + length])
             index += length
 
         key: bytes
         value: Optional[bytes]
         for s in strs:
-            try:
-                key, value = s.split(b'=', 1)
-            except ValueError:
+            key_value = s.split(b'=', 1)
+            if len(key_value) == 2:
+                key, value = key_value
+            else:
                 # No equals sign at all
                 key = s
                 value = None
 
             # Only update non-existent properties
-            if key and result.get(key) is None:
+            if key and key not in result:
                 result[key] = value
 
+        # Properties should be set atomically
+        # in case another thread is reading them
         self._properties = result
 
     def get_name(self) -> str:
         """Name accessor"""
         return self.name[: len(self.name) - len(self.type) - 1]
 
     def _get_ip_addresses_from_cache_lifo(
```

### Comparing `zeroconf-0.73.0/src/zeroconf/_services/registry.py` & `zeroconf-0.74.0/src/zeroconf/_services/registry.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.73.0/src/zeroconf/_services/types.py` & `zeroconf-0.74.0/src/zeroconf/_services/types.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.73.0/src/zeroconf/_updates.py` & `zeroconf-0.74.0/src/zeroconf/_updates.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.73.0/src/zeroconf/_utils/__init__.py` & `zeroconf-0.74.0/src/zeroconf/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.73.0/src/zeroconf/_utils/asyncio.py` & `zeroconf-0.74.0/src/zeroconf/_utils/asyncio.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.73.0/src/zeroconf/_utils/name.py` & `zeroconf-0.74.0/src/zeroconf/_utils/name.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.73.0/src/zeroconf/_utils/net.py` & `zeroconf-0.74.0/src/zeroconf/_utils/net.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.73.0/src/zeroconf/_utils/time.py` & `zeroconf-0.74.0/src/zeroconf/_utils/time.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.73.0/src/zeroconf/asyncio.py` & `zeroconf-0.74.0/src/zeroconf/asyncio.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.73.0/src/zeroconf/const.py` & `zeroconf-0.74.0/src/zeroconf/const.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.73.0/tests/__init__.py` & `zeroconf-0.74.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.73.0/tests/conftest.py` & `zeroconf-0.74.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.73.0/tests/services/__init__.py` & `zeroconf-0.74.0/tests/services/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.73.0/tests/services/test_browser.py` & `zeroconf-0.74.0/tests/services/test_browser.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.73.0/tests/services/test_info.py` & `zeroconf-0.74.0/tests/services/test_info.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.73.0/tests/services/test_registry.py` & `zeroconf-0.74.0/tests/services/test_registry.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.73.0/tests/services/test_types.py` & `zeroconf-0.74.0/tests/services/test_types.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.73.0/tests/test_asyncio.py` & `zeroconf-0.74.0/tests/test_asyncio.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.73.0/tests/test_cache.py` & `zeroconf-0.74.0/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.73.0/tests/test_core.py` & `zeroconf-0.74.0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.73.0/tests/test_dns.py` & `zeroconf-0.74.0/tests/test_dns.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.73.0/tests/test_exceptions.py` & `zeroconf-0.74.0/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.73.0/tests/test_handlers.py` & `zeroconf-0.74.0/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.73.0/tests/test_history.py` & `zeroconf-0.74.0/tests/test_history.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.73.0/tests/test_init.py` & `zeroconf-0.74.0/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.73.0/tests/test_logger.py` & `zeroconf-0.74.0/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.73.0/tests/test_protocol.py` & `zeroconf-0.74.0/tests/test_protocol.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.73.0/tests/test_services.py` & `zeroconf-0.74.0/tests/test_services.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.73.0/tests/test_updates.py` & `zeroconf-0.74.0/tests/test_updates.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.73.0/tests/utils/__init__.py` & `zeroconf-0.74.0/tests/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.73.0/tests/utils/test_asyncio.py` & `zeroconf-0.74.0/tests/utils/test_asyncio.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.73.0/tests/utils/test_name.py` & `zeroconf-0.74.0/tests/utils/test_name.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.73.0/tests/utils/test_net.py` & `zeroconf-0.74.0/tests/utils/test_net.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.73.0/setup.py` & `zeroconf-0.74.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ['ifaddr>=0.1.7']
 
 extras_require = \
 {':python_version < "3.11"': ['async-timeout>=3.0.0']}
 
 setup_kwargs = {
     'name': 'zeroconf',
-    'version': '0.73.0',
+    'version': '0.74.0',
     'description': 'A pure python implementation of multicast DNS service discovery',
     'long_description': 'python-zeroconf\n===============\n\n.. image:: https://github.com/python-zeroconf/python-zeroconf/workflows/CI/badge.svg\n   :target: https://github.com/python-zeroconf/python-zeroconf?query=workflow%3ACI+branch%3Amaster\n\n.. image:: https://img.shields.io/pypi/v/zeroconf.svg\n    :target: https://pypi.python.org/pypi/zeroconf\n\n.. image:: https://codecov.io/gh/python-zeroconf/python-zeroconf/branch/master/graph/badge.svg\n   :target: https://codecov.io/gh/python-zeroconf/python-zeroconf\n\n`Documentation <https://python-zeroconf.readthedocs.io/en/latest/>`_.\n\nThis is fork of pyzeroconf, Multicast DNS Service Discovery for Python,\noriginally by Paul Scott-Murphy (https://github.com/paulsm/pyzeroconf),\nmodified by William McBrine (https://github.com/wmcbrine/pyzeroconf).\n\nThe original William McBrine\'s fork note::\n\n    This fork is used in all of my TiVo-related projects: HME for Python\n    (and therefore HME/VLC), Network Remote, Remote Proxy, and pyTivo.\n    Before this, I was tracking the changes for zeroconf.py in three\n    separate repos. I figured I should have an authoritative source.\n\n    Although I make changes based on my experience with TiVos, I expect that\n    they\'re generally applicable. This version also includes patches found\n    on the now-defunct (?) Launchpad repo of pyzeroconf, and elsewhere\n    around the net -- not always well-documented, sorry.\n\nCompatible with:\n\n* Bonjour\n* Avahi\n\nCompared to some other Zeroconf/Bonjour/Avahi Python packages, python-zeroconf:\n\n* isn\'t tied to Bonjour or Avahi\n* doesn\'t use D-Bus\n* doesn\'t force you to use particular event loop or Twisted (asyncio is used under the hood but not required)\n* is pip-installable\n* has PyPI distribution\n* has an optional cython extension for performance (pure python is supported as well)\n\nPython compatibility\n--------------------\n\n* CPython 3.7+\n* PyPy3.7 7.3+\n\nVersioning\n----------\n\nThis project uses semantic versioning.\n\nStatus\n------\n\nThis project is actively maintained.\n\nTraffic Reduction\n-----------------\n\nBefore version 0.32, most traffic reduction techniques described in https://datatracker.ietf.org/doc/html/rfc6762#section-7\nwhere not implemented which could lead to excessive network traffic.  It is highly recommended that version 0.32 or later\nis used if this is a concern.\n\nIPv6 support\n------------\n\nIPv6 support is relatively new and currently limited, specifically:\n\n* `InterfaceChoice.All` is an alias for `InterfaceChoice.Default` on non-POSIX\n  systems.\n* Dual-stack IPv6 sockets are used, which may not be supported everywhere (some\n  BSD variants do not have them).\n* Listening on localhost (`::1`) does not work. Help with understanding why is\n  appreciated.\n\nHow to get python-zeroconf?\n===========================\n\n* PyPI page https://pypi.org/project/zeroconf/\n* GitHub project https://github.com/python-zeroconf/python-zeroconf\n\nThe easiest way to install python-zeroconf is using pip::\n\n    pip install zeroconf\n\n\n\nHow do I use it?\n================\n\nHere\'s an example of browsing for a service:\n\n.. code-block:: python\n\n    from zeroconf import ServiceBrowser, ServiceListener, Zeroconf\n\n\n    class MyListener(ServiceListener):\n\n        def update_service(self, zc: Zeroconf, type_: str, name: str) -> None:\n            print(f"Service {name} updated")\n\n        def remove_service(self, zc: Zeroconf, type_: str, name: str) -> None:\n            print(f"Service {name} removed")\n\n        def add_service(self, zc: Zeroconf, type_: str, name: str) -> None:\n            info = zc.get_service_info(type_, name)\n            print(f"Service {name} added, service info: {info}")\n\n\n    zeroconf = Zeroconf()\n    listener = MyListener()\n    browser = ServiceBrowser(zeroconf, "_http._tcp.local.", listener)\n    try:\n        input("Press enter to exit...\\n\\n")\n    finally:\n        zeroconf.close()\n\n.. note::\n\n    Discovery and service registration use *all* available network interfaces by default.\n    If you want to customize that you need to specify ``interfaces`` argument when\n    constructing ``Zeroconf`` object (see the code for details).\n\nIf you don\'t know the name of the service you need to browse for, try:\n\n.. code-block:: python\n\n    from zeroconf import ZeroconfServiceTypes\n    print(\'\\n\'.join(ZeroconfServiceTypes.find()))\n\nSee examples directory for more.\n\nChangelog\n=========\n\n`Changelog <CHANGELOG.md>`_\n\nLicense\n=======\n\nLGPL, see COPYING file for details.\n',
     'author': 'Paul Scott-Murphy',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/python-zeroconf/python-zeroconf',
```

### Comparing `zeroconf-0.73.0/PKG-INFO` & `zeroconf-0.74.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeroconf
-Version: 0.73.0
+Version: 0.74.0
 Summary: A pure python implementation of multicast DNS service discovery
 Home-page: https://github.com/python-zeroconf/python-zeroconf
 License: LGPL
 Author: Paul Scott-Murphy
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

