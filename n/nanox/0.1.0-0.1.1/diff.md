# Comparing `tmp/nanox-0.1.0.tar.gz` & `tmp/nanox-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanox-0.1.0.tar", max compression
+gzip compressed data, was "nanox-0.1.1.tar", max compression
```

## Comparing `nanox-0.1.0.tar` & `nanox-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0     1074 2023-08-04 14:22:45.509913 nanox-0.1.0/LICENSE
--rw-r--r--   0        0        0     5690 2023-08-04 17:19:05.233515 nanox-0.1.0/nanox/model/encoder.py
--rw-r--r--   0        0        0     1710 2023-08-04 15:53:12.742226 nanox-0.1.0/nanox/model/encoder_layer.py
--rw-r--r--   0        0        0     5697 2023-08-04 16:01:16.391132 nanox-0.1.0/nanox/model/layers.py
--rw-r--r--   0        0        0     8951 2023-08-04 15:46:44.525602 nanox-0.1.0/nanox/model/multihead_attention.py
--rw-r--r--   0        0        0     1187 2023-08-04 16:27:52.259604 nanox-0.1.0/nanox/model/pretained.py
--rw-r--r--   0        0        0     3045 2023-08-04 17:19:29.233445 nanox-0.1.0/nanox/nanox.py
--rw-r--r--   0        0        0      315 2023-08-04 18:01:51.778144 nanox-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      651 1970-01-01 00:00:00.000000 nanox-0.1.0/setup.py
--rw-r--r--   0        0        0      480 1970-01-01 00:00:00.000000 nanox-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-08-04 14:22:45.509913 nanox-0.1.1/LICENSE
+-rw-r--r--   0        0        0       92 2023-08-04 18:04:03.731407 nanox-0.1.1/nanox/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-04 18:02:32.219192 nanox-0.1.1/nanox/model/__init__.py
+-rw-r--r--   0        0        0     5690 2023-08-04 17:19:05.233515 nanox-0.1.1/nanox/model/encoder.py
+-rw-r--r--   0        0        0     1710 2023-08-04 15:53:12.742226 nanox-0.1.1/nanox/model/encoder_layer.py
+-rw-r--r--   0        0        0     5697 2023-08-04 16:01:16.391132 nanox-0.1.1/nanox/model/layers.py
+-rw-r--r--   0        0        0     8951 2023-08-04 15:46:44.525602 nanox-0.1.1/nanox/model/multihead_attention.py
+-rw-r--r--   0        0        0     1187 2023-08-04 16:27:52.259604 nanox-0.1.1/nanox/model/pretained.py
+-rw-r--r--   0        0        0     3045 2023-08-04 17:19:29.233445 nanox-0.1.1/nanox/nanox.py
+-rw-r--r--   0        0        0      315 2023-08-04 18:04:10.608581 nanox-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      651 1970-01-01 00:00:00.000000 nanox-0.1.1/setup.py
+-rw-r--r--   0        0        0      480 1970-01-01 00:00:00.000000 nanox-0.1.1/PKG-INFO
```

### Comparing `nanox-0.1.0/LICENSE` & `nanox-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nanox-0.1.0/nanox/model/encoder.py` & `nanox-0.1.1/nanox/model/encoder.py`

 * *Files identical despite different names*

### Comparing `nanox-0.1.0/nanox/model/encoder_layer.py` & `nanox-0.1.1/nanox/model/encoder_layer.py`

 * *Files identical despite different names*

### Comparing `nanox-0.1.0/nanox/model/layers.py` & `nanox-0.1.1/nanox/model/layers.py`

 * *Files identical despite different names*

### Comparing `nanox-0.1.0/nanox/model/multihead_attention.py` & `nanox-0.1.1/nanox/model/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `nanox-0.1.0/nanox/model/pretained.py` & `nanox-0.1.1/nanox/model/pretained.py`

 * *Files identical despite different names*

### Comparing `nanox-0.1.0/nanox/nanox.py` & `nanox-0.1.1/nanox/nanox.py`

 * *Files identical despite different names*

### Comparing `nanox-0.1.0/setup.py` & `nanox-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['torch>=1.10.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'nanox',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'A transformer model for creating bio-compatible nanomachines',
     'long_description': 'None',
     'author': 'Kye Gomez',
     'author_email': 'kye@apac.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

