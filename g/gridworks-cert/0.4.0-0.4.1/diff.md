# Comparing `tmp/gridworks_cert-0.4.0.tar.gz` & `tmp/gridworks_cert-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridworks_cert-0.4.0.tar", max compression
+gzip compressed data, was "gridworks_cert-0.4.1.tar", max compression
```

## Comparing `gridworks_cert-0.4.0.tar` & `gridworks_cert-0.4.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1073 2023-08-03 00:13:35.035691 gridworks_cert-0.4.0/LICENSE
--rw-r--r--   0        0        0     4088 2023-08-03 00:13:35.035691 gridworks_cert-0.4.0/README.md
--rw-r--r--   0        0        0     2165 2023-08-03 00:13:56.732980 gridworks_cert-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      101 2023-08-03 00:13:35.039692 gridworks_cert-0.4.0/src/gwcert/__init__.py
--rw-r--r--   0        0        0      658 2023-08-03 00:13:35.039692 gridworks_cert-0.4.0/src/gwcert/__main__.py
--rw-r--r--   0        0        0       99 2023-08-03 00:13:35.039692 gridworks_cert-0.4.0/src/gwcert/ca/__init__.py
--rw-r--r--   0        0        0     7416 2023-08-03 00:13:35.039692 gridworks_cert-0.4.0/src/gwcert/ca/__main__.py
--rw-r--r--   0        0        0      172 2023-08-03 00:13:35.039692 gridworks_cert-0.4.0/src/gwcert/key/__init__.py
--rw-r--r--   0        0        0    22025 2023-08-03 00:13:56.732980 gridworks_cert-0.4.0/src/gwcert/key/__main__.py
--rw-r--r--   0        0        0      196 2023-08-03 00:13:35.039692 gridworks_cert-0.4.0/src/gwcert/paths.py
--rw-r--r--   0        0        0        0 2023-08-03 00:13:35.039692 gridworks_cert-0.4.0/src/gwcert/py.typed
--rw-r--r--   0        0        0     5080 1970-01-01 00:00:00.000000 gridworks_cert-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-08-04 14:19:55.058749 gridworks_cert-0.4.1/LICENSE
+-rw-r--r--   0        0        0     4088 2023-08-04 14:19:55.058749 gridworks_cert-0.4.1/README.md
+-rw-r--r--   0        0        0     2165 2023-08-04 14:20:13.586999 gridworks_cert-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      101 2023-08-04 14:19:55.062749 gridworks_cert-0.4.1/src/gwcert/__init__.py
+-rw-r--r--   0        0        0     1187 2023-08-04 14:20:13.586999 gridworks_cert-0.4.1/src/gwcert/__main__.py
+-rw-r--r--   0        0        0       99 2023-08-04 14:19:55.062749 gridworks_cert-0.4.1/src/gwcert/ca/__init__.py
+-rw-r--r--   0        0        0     7479 2023-08-04 14:20:13.586999 gridworks_cert-0.4.1/src/gwcert/ca/__main__.py
+-rw-r--r--   0        0        0      172 2023-08-04 14:19:55.062749 gridworks_cert-0.4.1/src/gwcert/key/__init__.py
+-rw-r--r--   0        0        0    22025 2023-08-04 14:19:55.062749 gridworks_cert-0.4.1/src/gwcert/key/__main__.py
+-rw-r--r--   0        0        0      196 2023-08-04 14:19:55.062749 gridworks_cert-0.4.1/src/gwcert/paths.py
+-rw-r--r--   0        0        0        0 2023-08-04 14:19:55.062749 gridworks_cert-0.4.1/src/gwcert/py.typed
+-rw-r--r--   0        0        0     5080 1970-01-01 00:00:00.000000 gridworks_cert-0.4.1/PKG-INFO
```

### Comparing `gridworks_cert-0.4.0/LICENSE` & `gridworks_cert-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gridworks_cert-0.4.0/README.md` & `gridworks_cert-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `gridworks_cert-0.4.0/pyproject.toml` & `gridworks_cert-0.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gridworks-cert"
-version = "0.4.0"
+version = "0.4.1"
 description = "TLS certificate management tools for GridWorks"
 authors = ["Andrew Schweitzer <schweitz72@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/thegridelectric/gridworks-cert"
 repository = "https://github.com/thegridelectric/gridworks-cert"
 documentation = "https://gridworks-cert.readthedocs.io"
```

### Comparing `gridworks_cert-0.4.0/src/gwcert/ca/__main__.py` & `gridworks_cert-0.4.1/src/gwcert/ca/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,14 +104,16 @@
         typer.Option(
             help="Passed to cryptography.hazmat.primitives.asymmetric.rsa.generate_private_key()"
         ),
     ] = 2048,
 ) -> None:
     """Create files necessary for a simple, self-signed Certificate Authority."""
     ca_dir = Path(ca_dir)
+    if not ca_dir.exists():
+        ca_dir.mkdir(parents=True)
     ca_status = ownca_directory(str(ca_dir))
     if ca_status.certificate or ca_status.key or ca_status.public_key or ca_status.crl:
         print(
             f"[yellow][bold]WARNING: [/yellow][/bold] CA directory <{ca_dir}> is not empty. "
         )
         print("[yellow][bold]WARNING: [/yellow][/bold] NOT creating CA.")
     else:
```

### Comparing `gridworks_cert-0.4.0/src/gwcert/key/__main__.py` & `gridworks_cert-0.4.1/src/gwcert/key/__main__.py`

 * *Files identical despite different names*

### Comparing `gridworks_cert-0.4.0/PKG-INFO` & `gridworks_cert-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gridworks-cert
-Version: 0.4.0
+Version: 0.4.1
 Summary: TLS certificate management tools for GridWorks
 Home-page: https://github.com/thegridelectric/gridworks-cert
 License: MIT
 Author: Andrew Schweitzer
 Author-email: schweitz72@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
```

