# Comparing `tmp/timedctl-5.0.6.tar.gz` & `tmp/timedctl-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timedctl-5.0.6.tar", max compression
+gzip compressed data, was "timedctl-5.1.0.tar", max compression
```

## Comparing `timedctl-5.0.6.tar` & `timedctl-5.1.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    34454 2023-07-28 14:19:52.199210 timedctl-5.0.6/LICENSE
--rw-r--r--   0        0        0      774 2023-07-28 14:19:52.199210 timedctl-5.0.6/README.md
--rw-r--r--   0        0        0      858 2023-07-28 14:20:17.111347 timedctl-5.0.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-28 14:19:52.199210 timedctl-5.0.6/timedctl/__init__.py
--rw-r--r--   0        0        0     1831 2023-07-28 14:19:52.199210 timedctl-5.0.6/timedctl/helpers.py
--rwxr-xr-x   0        0        0    19859 2023-07-28 14:19:52.199210 timedctl-5.0.6/timedctl/timedctl.py
--rw-r--r--   0        0        0     1529 1970-01-01 00:00:00.000000 timedctl-5.0.6/PKG-INFO
+-rw-r--r--   0        0        0    34454 2023-08-04 20:02:24.177902 timedctl-5.1.0/LICENSE
+-rw-r--r--   0        0        0     1764 2023-08-04 20:02:24.177902 timedctl-5.1.0/README.md
+-rw-r--r--   0        0        0      858 2023-08-04 20:02:50.974334 timedctl-5.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-04 20:02:24.177902 timedctl-5.1.0/timedctl/__init__.py
+-rw-r--r--   0        0        0     2449 2023-08-04 20:02:24.177902 timedctl-5.1.0/timedctl/helpers.py
+-rwxr-xr-x   0        0        0    23046 2023-08-04 20:02:24.177902 timedctl-5.1.0/timedctl/timedctl.py
+-rw-r--r--   0        0        0     2519 1970-01-01 00:00:00.000000 timedctl-5.1.0/PKG-INFO
```

### Comparing `timedctl-5.0.6/LICENSE` & `timedctl-5.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `timedctl-5.0.6/pyproject.toml` & `timedctl-5.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "timedctl"
-version = "5.0.6"
+version = "5.1.0"
 description = "CLI for timed"
 authors = ["Arthur Deierlein <arthur.deierlein@adfinis.com>", "Gian Klug <gian.klug@adfinis.com>"]
 readme = "README.md"
 license = "AGPL-3.0-only"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `timedctl-5.0.6/timedctl/helpers.py` & `timedctl-5.1.0/timedctl/helpers.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,20 @@
+import json
 import rich
 import re
 import pyfzf
 import click
 import datetime
 import sys
+
 """
 API unrelated helper functions.
 """
 
+
 def msg(message, nonl=False):
     """Print a message in bold green."""
     rich.print(f"[bold green]{message}[/bold green]", end="" if nonl else "\n")
 
 
 def error_handler(error):
     """Handle errors."""
@@ -61,7 +64,27 @@
     """Sum up an array of time strings."""
     total = datetime.timedelta()
     for line in arr[1:]:
         val = line[-1]
         total += val
     # format as HH:MM:SS
     return str(total)
+
+
+def output_formatted(data, format):
+    """Output data in a specified format."""
+    match format:
+        case "json":
+            print(json.dumps(data, indent=4))
+        case "csv":
+            keys = data[0].keys()
+            output = ",".join(keys) + "\n"
+            for obj in data:
+                output += ",".join(obj.values()) + "\n"
+            print(output)
+        case "text":
+            for obj in data:
+                for key, val in obj.items():
+                    print(f"[{key}]: {val}, ", end="")
+                print("")
+        case _:
+            print("Invalid format")
```

### Comparing `timedctl-5.0.6/timedctl/timedctl.py` & `timedctl-5.1.0/timedctl/timedctl.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,22 @@
 import terminaltables
 import tomllib
 from click_aliases import ClickAliasedGroup
 from libtimed import TimedAPIClient
 from libtimed.oidc import OIDCClient
 from tomlkit import dump
 
-from timedctl.helpers import msg, error_handler, fzf_wrapper, time_picker, time_sum
+from timedctl.helpers import (
+    msg,
+    error_handler,
+    fzf_wrapper,
+    time_picker,
+    time_sum,
+    output_formatted,
+)
 
 
 def load_config():
     """Load the timedctl config."""
     cfg = {
         "username": "test",
         "timed_url": "https://timed.example.com",
@@ -164,14 +171,90 @@
 
 @timedctl.group(cls=ClickAliasedGroup, aliases=["g", "show", "describe"])
 def get():
     """Get different things."""
     pass  # pylint: disable=W0107
 
 
+@get.group(cls=ClickAliasedGroup)
+def data():
+    """Get raw data for building custom scripts."""
+    pass  # pylint: disable=W0107
+
+
+@data.command("customers")
+@click.option("--format", default="json", type=click.Choice(["json", "csv", "text"]))
+def get_customers(format):
+    """Get customers."""
+    customers = timed.customers.get(cached=True)
+    data = []
+    for customer in customers:
+        data.append({"id": customer["id"], "name": customer["attributes"]["name"]})
+    output_formatted(data, format)
+
+
+@data.command("projects")
+@click.option("--format", default="json", type=click.Choice(["json", "csv", "text"]))
+@click.option("--customer-id", default=None, type=int)
+@click.option("--customer-name", default=None, type=str)
+def get_projects(format, customer_id, customer_name):
+    """Get projects."""
+    if not (customer_id or customer_name):
+        error_handler("ERR_MISSING_ARGUMENTS")
+    # Get customer ID if name is specified
+    if not customer_id:
+        customers = timed.customers.get(cached=True)
+        customer = [c for c in customers if c["attributes"]["name"] == customer_name]
+        if len(customer) == 0:
+            error_handler("ERR_CUSTOMER_NOT_FOUND")
+        customer_id = customer[0]["id"]
+    projects = timed.projects.get(cached=True, filters={"customer": customer_id})
+    data = []
+    for project in projects:
+        data.append({"id": project["id"], "name": project["attributes"]["name"]})
+    output_formatted(data, format)
+
+
+@data.command("tasks")
+@click.option("--format", default="json", type=click.Choice(["json", "csv", "text"]))
+@click.option("--customer-id", default=None, type=int)
+@click.option("--customer-name", default=None, type=str)
+@click.option("--project-id", default=None, type=int)
+@click.option("--project-name", default=None, type=str)
+def get_tasks(format, customer_id, customer_name, project_id, project_name):
+    """Get tasks."""
+    if project_name and not (customer_id or customer_name):
+        error_handler("ERR_CUSTOMER_INFO_MISSING")
+    if not (project_id or project_name):
+        error_handler("ERR_MISSING_ARGUMENTS")
+    # Get project ID if name is specified
+    if not project_id:
+        # we need an id for the customer
+        if not customer_id:
+            customers = timed.customers.get(cached=True)
+            customer = [
+                c for c in customers if c["attributes"]["name"] == customer_name
+            ]
+            if len(customer) == 0:
+                error_handler("ERR_CUSTOMER_NOT_FOUND")
+            customer_id = customer[0]["id"]
+        # get the project id
+        projects = timed.projects.get(cached=True, filters={"customer": customer_id})
+        project = [c for c in projects if c["attributes"]["name"] == project_name]
+        if len(project) == 0:
+            error_handler("ERR_PROJECT_NOT_FOUND")
+        project_id = project[0]["id"]
+    # get the tasks for the specified project
+    tasks = timed.tasks.get(cached=True, filters={"project": project_id})
+    data = []
+    for task in tasks:
+        data.append({"id": task["id"], "name": task["attributes"]["name"]})
+    output_formatted(data, format)
+
+
 @get.command("overtime", aliases=["t", "ot", "undertime"])
 @click.option("--date", default=None)
 def get_overtime(date):
     """Get overtime of user."""
     user = timed.users.me["id"]
     overtime = timed.overtime.get({"user": user, "date": date})
     msg(f"Currrent overtime is: {overtime}")
```

