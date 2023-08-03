# Comparing `tmp/satori_ci-1.3.4.tar.gz` & `tmp/satori_ci-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satori_ci-1.3.4.tar", last modified: Thu Aug  3 11:56:21 2023, max compression
+gzip compressed data, was "satori_ci-1.3.5.tar", last modified: Thu Aug  3 16:39:07 2023, max compression
```

## Comparing `satori_ci-1.3.4.tar` & `satori_ci-1.3.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    35149 2023-08-03 11:56:06.359856 satori_ci-1.3.4/LICENSE
--rw-r--r--   0        0        0     7140 2023-08-03 11:56:06.359856 satori_ci-1.3.4/README.md
--rw-r--r--   0        0        0      755 2023-08-03 11:56:21.688043 satori_ci-1.3.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-03 11:56:06.359856 satori_ci-1.3.4/src/satoricli/__init__.py
--rw-r--r--   0        0        0       37 2023-08-03 11:56:06.359856 satori_ci-1.3.4/src/satoricli/__main__.py
--rw-r--r--   0        0        0     4551 2023-08-03 11:56:06.359856 satori_ci-1.3.4/src/satoricli/classes/api.py
--rw-r--r--   0        0        0     1633 2023-08-03 11:56:06.359856 satori_ci-1.3.4/src/satoricli/classes/bundler.py
--rw-r--r--   0        0        0      484 2023-08-03 11:56:06.359856 satori_ci-1.3.4/src/satoricli/classes/models.py
--rw-r--r--   0        0        0     3345 2023-08-03 11:56:06.359856 satori_ci-1.3.4/src/satoricli/classes/playbooks.py
--rw-r--r--   0        0        0    27448 2023-08-03 11:56:06.359856 satori_ci-1.3.4/src/satoricli/classes/satori.py
--rw-r--r--   0        0        0    13678 2023-08-03 11:56:06.359856 satori_ci-1.3.4/src/satoricli/classes/utils.py
--rw-r--r--   0        0        0     1194 2023-08-03 11:56:06.359856 satori_ci-1.3.4/src/satoricli/classes/validations.py
--rwxr-xr-x   0        0        0     9827 2023-08-03 11:56:06.359856 satori_ci-1.3.4/src/satoricli/cli/parser.py
--rw-r--r--   0        0        0    48305 1970-01-01 00:00:00.000000 satori_ci-1.3.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-08-03 16:38:50.129828 satori_ci-1.3.5/LICENSE
+-rw-r--r--   0        0        0     7140 2023-08-03 16:38:50.129828 satori_ci-1.3.5/README.md
+-rw-r--r--   0        0        0      755 2023-08-03 16:39:07.749973 satori_ci-1.3.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-03 16:38:50.129828 satori_ci-1.3.5/src/satoricli/__init__.py
+-rw-r--r--   0        0        0       37 2023-08-03 16:38:50.129828 satori_ci-1.3.5/src/satoricli/__main__.py
+-rw-r--r--   0        0        0     4551 2023-08-03 16:38:50.129828 satori_ci-1.3.5/src/satoricli/classes/api.py
+-rw-r--r--   0        0        0     1633 2023-08-03 16:38:50.129828 satori_ci-1.3.5/src/satoricli/classes/bundler.py
+-rw-r--r--   0        0        0      484 2023-08-03 16:38:50.129828 satori_ci-1.3.5/src/satoricli/classes/models.py
+-rw-r--r--   0        0        0     3345 2023-08-03 16:38:50.129828 satori_ci-1.3.5/src/satoricli/classes/playbooks.py
+-rw-r--r--   0        0        0    27448 2023-08-03 16:38:50.129828 satori_ci-1.3.5/src/satoricli/classes/satori.py
+-rw-r--r--   0        0        0    13678 2023-08-03 16:38:50.129828 satori_ci-1.3.5/src/satoricli/classes/utils.py
+-rw-r--r--   0        0        0     1194 2023-08-03 16:38:50.129828 satori_ci-1.3.5/src/satoricli/classes/validations.py
+-rwxr-xr-x   0        0        0     9884 2023-08-03 16:38:50.129828 satori_ci-1.3.5/src/satoricli/cli/parser.py
+-rw-r--r--   0        0        0    48305 1970-01-01 00:00:00.000000 satori_ci-1.3.5/PKG-INFO
```

### Comparing `satori_ci-1.3.4/LICENSE` & `satori_ci-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `satori_ci-1.3.4/README.md` & `satori_ci-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `satori_ci-1.3.4/pyproject.toml` & `satori_ci-1.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "satori-ci"
-version = "1.3.4"
+version = "1.3.5"
 description = "Satori CI - Automated Software Testing Platform"
 authors = [
     { name = "Satori CI CLI", email = "info@satori-ci.com" },
 ]
 dependencies = [
     "requests>=2.27.1",
     "pyyaml>=6.0",
```

### Comparing `satori_ci-1.3.4/src/satoricli/classes/api.py` & `satori_ci-1.3.5/src/satoricli/classes/api.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.3.4/src/satoricli/classes/bundler.py` & `satori_ci-1.3.5/src/satoricli/classes/bundler.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.3.4/src/satoricli/classes/playbooks.py` & `satori_ci-1.3.5/src/satoricli/classes/playbooks.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.3.4/src/satoricli/classes/satori.py` & `satori_ci-1.3.5/src/satoricli/classes/satori.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.3.4/src/satoricli/classes/utils.py` & `satori_ci-1.3.5/src/satoricli/classes/utils.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.3.4/src/satoricli/classes/validations.py` & `satori_ci-1.3.5/src/satoricli/classes/validations.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.3.4/src/satoricli/cli/parser.py` & `satori_ci-1.3.5/src/satoricli/cli/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,17 +56,20 @@
         if (
             current_version
             and latest_version
             and version.parse(current_version) < version.parse(latest_version)
         ):
             upgrade_required += package_name + " "
     if upgrade_required:
-        console.print(
-            "[warning]WARNING:[/] Newer version found, upgrade with: "
-            "[b]pip install -U " + upgrade_required
+        print(
+            (
+                "[yellow]WARNING:[/] Newer version found, upgrade with: "
+                f"[b]pip install -U {upgrade_required}"
+            ),
+            file=sys.stderr,
         )
 
 
 def main():
     timestamp = (datetime.now()).strftime("%Y-%m-%d %H:%M:%S")
     print(
         f"[dim]Satori CI {VERSION} - Automated Software Testing Platform - Started on {timestamp}",
```

### Comparing `satori_ci-1.3.4/PKG-INFO` & `satori_ci-1.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satori-ci
-Version: 1.3.4
+Version: 1.3.5
 Summary: Satori CI - Automated Software Testing Platform
 Author-Email: Satori CI CLI <info@satori-ci.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

