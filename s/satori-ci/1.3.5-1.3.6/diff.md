# Comparing `tmp/satori_ci-1.3.5.tar.gz` & `tmp/satori_ci-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satori_ci-1.3.5.tar", last modified: Thu Aug  3 16:39:07 2023, max compression
+gzip compressed data, was "satori_ci-1.3.6.tar", last modified: Thu Aug  3 22:24:01 2023, max compression
```

## Comparing `satori_ci-1.3.5.tar` & `satori_ci-1.3.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    35149 2023-08-03 16:38:50.129828 satori_ci-1.3.5/LICENSE
--rw-r--r--   0        0        0     7140 2023-08-03 16:38:50.129828 satori_ci-1.3.5/README.md
--rw-r--r--   0        0        0      755 2023-08-03 16:39:07.749973 satori_ci-1.3.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-03 16:38:50.129828 satori_ci-1.3.5/src/satoricli/__init__.py
--rw-r--r--   0        0        0       37 2023-08-03 16:38:50.129828 satori_ci-1.3.5/src/satoricli/__main__.py
--rw-r--r--   0        0        0     4551 2023-08-03 16:38:50.129828 satori_ci-1.3.5/src/satoricli/classes/api.py
--rw-r--r--   0        0        0     1633 2023-08-03 16:38:50.129828 satori_ci-1.3.5/src/satoricli/classes/bundler.py
--rw-r--r--   0        0        0      484 2023-08-03 16:38:50.129828 satori_ci-1.3.5/src/satoricli/classes/models.py
--rw-r--r--   0        0        0     3345 2023-08-03 16:38:50.129828 satori_ci-1.3.5/src/satoricli/classes/playbooks.py
--rw-r--r--   0        0        0    27448 2023-08-03 16:38:50.129828 satori_ci-1.3.5/src/satoricli/classes/satori.py
--rw-r--r--   0        0        0    13678 2023-08-03 16:38:50.129828 satori_ci-1.3.5/src/satoricli/classes/utils.py
--rw-r--r--   0        0        0     1194 2023-08-03 16:38:50.129828 satori_ci-1.3.5/src/satoricli/classes/validations.py
--rwxr-xr-x   0        0        0     9884 2023-08-03 16:38:50.129828 satori_ci-1.3.5/src/satoricli/cli/parser.py
--rw-r--r--   0        0        0    48305 1970-01-01 00:00:00.000000 satori_ci-1.3.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-08-03 22:23:41.134072 satori_ci-1.3.6/LICENSE
+-rw-r--r--   0        0        0     7140 2023-08-03 22:23:41.134072 satori_ci-1.3.6/README.md
+-rw-r--r--   0        0        0      755 2023-08-03 22:24:01.102969 satori_ci-1.3.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-03 22:23:41.134072 satori_ci-1.3.6/src/satoricli/__init__.py
+-rw-r--r--   0        0        0       37 2023-08-03 22:23:41.134072 satori_ci-1.3.6/src/satoricli/__main__.py
+-rw-r--r--   0        0        0     4551 2023-08-03 22:23:41.134072 satori_ci-1.3.6/src/satoricli/classes/api.py
+-rw-r--r--   0        0        0     1633 2023-08-03 22:23:41.134072 satori_ci-1.3.6/src/satoricli/classes/bundler.py
+-rw-r--r--   0        0        0      484 2023-08-03 22:23:41.134072 satori_ci-1.3.6/src/satoricli/classes/models.py
+-rw-r--r--   0        0        0     3345 2023-08-03 22:23:41.134072 satori_ci-1.3.6/src/satoricli/classes/playbooks.py
+-rw-r--r--   0        0        0    27666 2023-08-03 22:23:41.134072 satori_ci-1.3.6/src/satoricli/classes/satori.py
+-rw-r--r--   0        0        0    13678 2023-08-03 22:23:41.134072 satori_ci-1.3.6/src/satoricli/classes/utils.py
+-rw-r--r--   0        0        0     1194 2023-08-03 22:23:41.134072 satori_ci-1.3.6/src/satoricli/classes/validations.py
+-rwxr-xr-x   0        0        0     9990 2023-08-03 22:23:41.134072 satori_ci-1.3.6/src/satoricli/cli/parser.py
+-rw-r--r--   0        0        0    48305 1970-01-01 00:00:00.000000 satori_ci-1.3.6/PKG-INFO
```

### Comparing `satori_ci-1.3.5/LICENSE` & `satori_ci-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `satori_ci-1.3.5/README.md` & `satori_ci-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `satori_ci-1.3.5/pyproject.toml` & `satori_ci-1.3.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "satori-ci"
-version = "1.3.5"
+version = "1.3.6"
 description = "Satori CI - Automated Software Testing Platform"
 authors = [
     { name = "Satori CI CLI", email = "info@satori-ci.com" },
 ]
 dependencies = [
     "requests>=2.27.1",
     "pyyaml>=6.0",
```

### Comparing `satori_ci-1.3.5/src/satoricli/classes/api.py` & `satori_ci-1.3.6/src/satoricli/classes/api.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.3.5/src/satoricli/classes/bundler.py` & `satori_ci-1.3.6/src/satoricli/classes/bundler.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.3.5/src/satoricli/classes/playbooks.py` & `satori_ci-1.3.6/src/satoricli/classes/playbooks.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.3.5/src/satoricli/classes/satori.py` & `satori_ci-1.3.6/src/satoricli/classes/satori.py`

 * *Files 1% similar despite different names*

```diff
@@ -505,14 +505,15 @@
 
     def output(self, report_id: str):
         """Returns commands output"""
         format_outputs(self.api.get_report_output(report_id))
 
     def get_outputs(
         self,
+        raw: bool,
         from_date: Optional[date] = None,
         to_date: Optional[date] = None,
         name: Optional[str] = None,
         failed: Optional[bool] = None,
         **kwargs,
     ):
         res = self.api.request(
@@ -522,23 +523,28 @@
                 "from_date": from_date,
                 "to_date": to_date,
                 "name": name,
                 "failed": failed,
             },
         )
 
-        for item in res.json():
-            output = requests.get(item["url"], stream=True)
-
-            if not output.ok:
-                continue
-
-            console.print(f"Report: {item['report_id']}")
-            format_outputs(output.iter_lines())
-            console.print()
+        with requests.Session() as s:
+            for item in res.json():
+                output = s.get(item["url"], stream=True)
+
+                if not output.ok:
+                    continue
+
+                if raw:
+                    console.rule()
+                    console.print(output.text)
+                else:
+                    console.print(f"Report: {item['report_id']}")
+                    format_outputs(output.iter_lines())
+                    console.print()
 
     def output_files(self, report_id: str):
         r = self.api.get_report_files(report_id)
         total = int(r.headers["Content-Length"])
 
         with Progress() as progress:
             task = progress.add_task("Downloading...", total=total)
```

### Comparing `satori_ci-1.3.5/src/satoricli/classes/utils.py` & `satori_ci-1.3.6/src/satoricli/classes/utils.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.3.5/src/satoricli/classes/validations.py` & `satori_ci-1.3.6/src/satoricli/classes/validations.py`

 * *Files identical despite different names*

### Comparing `satori_ci-1.3.5/src/satoricli/cli/parser.py` & `satori_ci-1.3.6/src/satoricli/cli/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,14 +162,17 @@
         default="",
         help="Filters: from,to,satori_error,status",
     )
     add_satori_arguments(report_cmd)
 
     # outputs
     outputs_cmd = subparsers.add_parser("outputs", parents=[baseparser])
+    outputs_cmd.add_argument(
+        "--raw", action="store_true", help="Print without formatting"
+    )
     output_filters = outputs_cmd.add_argument_group("filters")
     output_filters.add_argument(
         "--from",
         type=date.fromisoformat,
         help="Date in ISO format",
         metavar="DATE",
         dest="from_date",
```

### Comparing `satori_ci-1.3.5/PKG-INFO` & `satori_ci-1.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satori-ci
-Version: 1.3.5
+Version: 1.3.6
 Summary: Satori CI - Automated Software Testing Platform
 Author-Email: Satori CI CLI <info@satori-ci.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

