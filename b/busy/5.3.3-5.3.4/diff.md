# Comparing `tmp/busy-5.3.3.tar.gz` & `tmp/busy-5.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "busy-5.3.3.tar", last modified: Fri Aug  4 04:26:12 2023, max compression
+gzip compressed data, was "busy-5.3.4.tar", last modified: Fri Aug  4 05:00:14 2023, max compression
```

## Comparing `busy-5.3.3.tar` & `busy-5.3.4.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 04:26:12.574692 busy-5.3.3/
--rw-r--r--   0 root         (0) root         (0)        5 2023-08-04 04:25:23.000000 busy-5.3.3/.version
--rw-rw-rw-   0 root         (0) root         (0)     1071 2023-08-04 04:26:04.000000 busy-5.3.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)    22714 2023-08-04 04:26:12.573692 busy-5.3.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    22464 2023-08-04 04:26:04.000000 busy-5.3.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 04:26:12.564692 busy-5.3.3/busy/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-04 04:26:04.000000 busy-5.3.3/busy/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-08-04 04:26:04.000000 busy-5.3.3/busy/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 04:26:12.569692 busy-5.3.3/busy/command/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-04 04:26:04.000000 busy-5.3.3/busy/command/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1641 2023-08-04 04:26:04.000000 busy-5.3.3/busy/command/activate_command.py
--rw-rw-rw-   0 root         (0) root         (0)      805 2023-08-04 04:26:04.000000 busy-5.3.3/busy/command/add_command.py
--rw-rw-rw-   0 root         (0) root         (0)      293 2023-08-04 04:26:04.000000 busy-5.3.3/busy/command/base_command.py
--rw-rw-rw-   0 root         (0) root         (0)     6834 2023-08-04 04:26:04.000000 busy-5.3.3/busy/command/command.py
--rw-rw-rw-   0 root         (0) root         (0)      246 2023-08-04 04:26:04.000000 busy-5.3.3/busy/command/curses_command.py
--rw-rw-rw-   0 root         (0) root         (0)     1714 2023-08-04 04:26:04.000000 busy-5.3.3/busy/command/defer_command.py
--rw-rw-rw-   0 root         (0) root         (0)      965 2023-08-04 04:26:04.000000 busy-5.3.3/busy/command/delete_command.py
--rw-rw-rw-   0 root         (0) root         (0)     1245 2023-08-04 04:26:04.000000 busy-5.3.3/busy/command/drop_and_pop_command.py
--rw-rw-rw-   0 root         (0) root         (0)      767 2023-08-04 04:26:04.000000 busy-5.3.3/busy/command/edit_command.py
--rw-rw-rw-   0 root         (0) root         (0)     1973 2023-08-04 04:26:04.000000 busy-5.3.3/busy/command/finish_command.py
--rw-rw-rw-   0 root         (0) root         (0)      758 2023-08-04 04:26:04.000000 busy-5.3.3/busy/command/list_command.py
--rw-rw-rw-   0 root         (0) root         (0)      973 2023-08-04 04:26:04.000000 busy-5.3.3/busy/command/print_command.py
--rw-rw-rw-   0 root         (0) root         (0)      272 2023-08-04 04:26:04.000000 busy-5.3.3/busy/command/queues_command.py
--rw-rw-rw-   0 root         (0) root         (0)      284 2023-08-04 04:26:04.000000 busy-5.3.3/busy/command/resource_command.py
--rw-rw-rw-   0 root         (0) root         (0)      256 2023-08-04 04:26:04.000000 busy-5.3.3/busy/command/show_command.py
--rw-rw-rw-   0 root         (0) root         (0)     1039 2023-08-04 04:26:04.000000 busy-5.3.3/busy/command/switch_command.py
--rw-rw-rw-   0 root         (0) root         (0)      334 2023-08-04 04:26:04.000000 busy-5.3.3/busy/command/tags_command.py
--rw-rw-rw-   0 root         (0) root         (0)     3555 2023-08-04 04:26:04.000000 busy-5.3.3/busy/handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 04:26:12.569692 busy-5.3.3/busy/model/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-04 04:26:04.000000 busy-5.3.3/busy/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 04:26:12.570692 busy-5.3.3/busy/model/collection/
--rw-rw-rw-   0 root         (0) root         (0)     5020 2023-08-04 04:26:04.000000 busy-5.3.3/busy/model/collection/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2023-08-04 04:26:04.000000 busy-5.3.3/busy/model/collection/done_collection.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2023-08-04 04:26:04.000000 busy-5.3.3/busy/model/collection/plan_collection.py
--rw-rw-rw-   0 root         (0) root         (0)       81 2023-08-04 04:26:04.000000 busy-5.3.3/busy/model/collection/skip_collection.py
--rw-rw-rw-   0 root         (0) root         (0)       81 2023-08-04 04:26:04.000000 busy-5.3.3/busy/model/collection/todo_collection.py
--rw-rw-rw-   0 root         (0) root         (0)     3376 2023-08-04 04:26:04.000000 busy-5.3.3/busy/model/item.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 04:26:12.571692 busy-5.3.3/busy/storage/
--rw-rw-rw-   0 root         (0) root         (0)      237 2023-08-04 04:26:04.000000 busy-5.3.3/busy/storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2196 2023-08-04 04:26:04.000000 busy-5.3.3/busy/storage/file_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 04:26:12.571692 busy-5.3.3/busy/ui/
--rw-rw-rw-   0 root         (0) root         (0)      133 2023-08-04 04:26:04.000000 busy-5.3.3/busy/ui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6589 2023-08-04 04:26:04.000000 busy-5.3.3/busy/ui/curses_ui.py
--rw-rw-rw-   0 root         (0) root         (0)     1499 2023-08-04 04:26:04.000000 busy-5.3.3/busy/ui/shell_ui.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 04:26:12.572692 busy-5.3.3/busy/ui/tcl_ui/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-04 04:26:04.000000 busy-5.3.3/busy/ui/tcl_ui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      824 2023-08-04 04:26:04.000000 busy-5.3.3/busy/ui/tcl_ui/edit_task_widget.py
--rw-rw-rw-   0 root         (0) root         (0)      701 2023-08-04 04:26:04.000000 busy-5.3.3/busy/ui/tcl_ui/get_item_widget.py
--rw-rw-rw-   0 root         (0) root         (0)     5588 2023-08-04 04:26:04.000000 busy-5.3.3/busy/ui/ui.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 04:26:12.573692 busy-5.3.3/busy/util/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-04 04:26:04.000000 busy-5.3.3/busy/util/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4443 2023-08-04 04:26:04.000000 busy-5.3.3/busy/util/checklist.py
--rw-rw-rw-   0 root         (0) root         (0)     2844 2023-08-04 04:26:04.000000 busy-5.3.3/busy/util/date_util.py
--rw-rw-rw-   0 root         (0) root         (0)      218 2023-08-04 04:26:04.000000 busy-5.3.3/busy/util/python_version.py
--rw-rw-rw-   0 root         (0) root         (0)     2477 2023-08-04 04:26:04.000000 busy-5.3.3/busy/util/selector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 04:26:12.565692 busy-5.3.3/busy.egg-info/
--rw-r--r--   0 root         (0) root         (0)    22714 2023-08-04 04:26:12.000000 busy-5.3.3/busy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1384 2023-08-04 04:26:12.000000 busy-5.3.3/busy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 04:26:12.000000 busy-5.3.3/busy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2023-08-04 04:26:12.000000 busy-5.3.3/busy.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       99 2023-08-04 04:26:12.000000 busy-5.3.3/busy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-08-04 04:26:12.000000 busy-5.3.3/busy.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      627 2023-08-04 04:26:04.000000 busy-5.3.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-04 04:26:12.574692 busy-5.3.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 05:00:14.775890 busy-5.3.4/
+-rw-r--r--   0 root         (0) root         (0)        5 2023-08-04 04:59:26.000000 busy-5.3.4/.version
+-rw-rw-rw-   0 root         (0) root         (0)     1071 2023-08-04 05:00:06.000000 busy-5.3.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    22714 2023-08-04 05:00:14.774890 busy-5.3.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    22464 2023-08-04 05:00:06.000000 busy-5.3.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 05:00:14.765890 busy-5.3.4/busy/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-04 05:00:06.000000 busy-5.3.4/busy/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-08-04 05:00:06.000000 busy-5.3.4/busy/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 05:00:14.770890 busy-5.3.4/busy/command/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-04 05:00:06.000000 busy-5.3.4/busy/command/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1641 2023-08-04 05:00:06.000000 busy-5.3.4/busy/command/activate_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      805 2023-08-04 05:00:06.000000 busy-5.3.4/busy/command/add_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      293 2023-08-04 05:00:06.000000 busy-5.3.4/busy/command/base_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     6834 2023-08-04 05:00:06.000000 busy-5.3.4/busy/command/command.py
+-rw-rw-rw-   0 root         (0) root         (0)      246 2023-08-04 05:00:06.000000 busy-5.3.4/busy/command/curses_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     1714 2023-08-04 05:00:06.000000 busy-5.3.4/busy/command/defer_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      965 2023-08-04 05:00:06.000000 busy-5.3.4/busy/command/delete_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     1245 2023-08-04 05:00:06.000000 busy-5.3.4/busy/command/drop_and_pop_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      767 2023-08-04 05:00:06.000000 busy-5.3.4/busy/command/edit_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     1973 2023-08-04 05:00:06.000000 busy-5.3.4/busy/command/finish_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      758 2023-08-04 05:00:06.000000 busy-5.3.4/busy/command/list_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      973 2023-08-04 05:00:06.000000 busy-5.3.4/busy/command/print_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      272 2023-08-04 05:00:06.000000 busy-5.3.4/busy/command/queues_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      284 2023-08-04 05:00:06.000000 busy-5.3.4/busy/command/resource_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      256 2023-08-04 05:00:06.000000 busy-5.3.4/busy/command/show_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     1039 2023-08-04 05:00:06.000000 busy-5.3.4/busy/command/switch_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      334 2023-08-04 05:00:06.000000 busy-5.3.4/busy/command/tags_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     3555 2023-08-04 05:00:06.000000 busy-5.3.4/busy/handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 05:00:14.770890 busy-5.3.4/busy/model/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-04 05:00:06.000000 busy-5.3.4/busy/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 05:00:14.771890 busy-5.3.4/busy/model/collection/
+-rw-rw-rw-   0 root         (0) root         (0)     5020 2023-08-04 05:00:06.000000 busy-5.3.4/busy/model/collection/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2023-08-04 05:00:06.000000 busy-5.3.4/busy/model/collection/done_collection.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2023-08-04 05:00:06.000000 busy-5.3.4/busy/model/collection/plan_collection.py
+-rw-rw-rw-   0 root         (0) root         (0)       81 2023-08-04 05:00:06.000000 busy-5.3.4/busy/model/collection/skip_collection.py
+-rw-rw-rw-   0 root         (0) root         (0)       81 2023-08-04 05:00:06.000000 busy-5.3.4/busy/model/collection/todo_collection.py
+-rw-rw-rw-   0 root         (0) root         (0)     3376 2023-08-04 05:00:06.000000 busy-5.3.4/busy/model/item.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 05:00:14.772890 busy-5.3.4/busy/storage/
+-rw-rw-rw-   0 root         (0) root         (0)      237 2023-08-04 05:00:06.000000 busy-5.3.4/busy/storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2196 2023-08-04 05:00:06.000000 busy-5.3.4/busy/storage/file_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 05:00:14.773890 busy-5.3.4/busy/ui/
+-rw-rw-rw-   0 root         (0) root         (0)      133 2023-08-04 05:00:06.000000 busy-5.3.4/busy/ui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6690 2023-08-04 05:00:06.000000 busy-5.3.4/busy/ui/curses_ui.py
+-rw-rw-rw-   0 root         (0) root         (0)     1499 2023-08-04 05:00:06.000000 busy-5.3.4/busy/ui/shell_ui.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 05:00:14.773890 busy-5.3.4/busy/ui/tcl_ui/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-04 05:00:06.000000 busy-5.3.4/busy/ui/tcl_ui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      824 2023-08-04 05:00:06.000000 busy-5.3.4/busy/ui/tcl_ui/edit_task_widget.py
+-rw-rw-rw-   0 root         (0) root         (0)      701 2023-08-04 05:00:06.000000 busy-5.3.4/busy/ui/tcl_ui/get_item_widget.py
+-rw-rw-rw-   0 root         (0) root         (0)     5588 2023-08-04 05:00:06.000000 busy-5.3.4/busy/ui/ui.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 05:00:14.774890 busy-5.3.4/busy/util/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-04 05:00:06.000000 busy-5.3.4/busy/util/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4443 2023-08-04 05:00:06.000000 busy-5.3.4/busy/util/checklist.py
+-rw-rw-rw-   0 root         (0) root         (0)     2844 2023-08-04 05:00:06.000000 busy-5.3.4/busy/util/date_util.py
+-rw-rw-rw-   0 root         (0) root         (0)      218 2023-08-04 05:00:06.000000 busy-5.3.4/busy/util/python_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     2477 2023-08-04 05:00:06.000000 busy-5.3.4/busy/util/selector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 05:00:14.767890 busy-5.3.4/busy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    22714 2023-08-04 05:00:14.000000 busy-5.3.4/busy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1384 2023-08-04 05:00:14.000000 busy-5.3.4/busy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 05:00:14.000000 busy-5.3.4/busy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2023-08-04 05:00:14.000000 busy-5.3.4/busy.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       99 2023-08-04 05:00:14.000000 busy-5.3.4/busy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-08-04 05:00:14.000000 busy-5.3.4/busy.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      627 2023-08-04 05:00:06.000000 busy-5.3.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-04 05:00:14.775890 busy-5.3.4/setup.cfg
```

### Comparing `busy-5.3.3/LICENSE` & `busy-5.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `busy-5.3.3/PKG-INFO` & `busy-5.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: busy
-Version: 5.3.3
+Version: 5.3.4
 Summary: Personal time management for techies
 Author-email: Francis Potter <busy@steampunkwizard.ca>
 License: MIT
 Requires-Python: >=3.6.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `busy-5.3.3/README.md` & `busy-5.3.4/README.md`

 * *Files identical despite different names*

### Comparing `busy-5.3.3/busy/command/activate_command.py` & `busy-5.3.4/busy/command/activate_command.py`

 * *Files identical despite different names*

### Comparing `busy-5.3.3/busy/command/add_command.py` & `busy-5.3.4/busy/command/add_command.py`

 * *Files identical despite different names*

### Comparing `busy-5.3.3/busy/command/command.py` & `busy-5.3.4/busy/command/command.py`

 * *Files identical despite different names*

### Comparing `busy-5.3.3/busy/command/defer_command.py` & `busy-5.3.4/busy/command/defer_command.py`

 * *Files identical despite different names*

### Comparing `busy-5.3.3/busy/command/delete_command.py` & `busy-5.3.4/busy/command/delete_command.py`

 * *Files identical despite different names*

### Comparing `busy-5.3.3/busy/command/drop_and_pop_command.py` & `busy-5.3.4/busy/command/drop_and_pop_command.py`

 * *Files identical despite different names*

### Comparing `busy-5.3.3/busy/command/edit_command.py` & `busy-5.3.4/busy/command/edit_command.py`

 * *Files identical despite different names*

### Comparing `busy-5.3.3/busy/command/finish_command.py` & `busy-5.3.4/busy/command/finish_command.py`

 * *Files identical despite different names*

### Comparing `busy-5.3.3/busy/command/list_command.py` & `busy-5.3.4/busy/command/list_command.py`

 * *Files identical despite different names*

### Comparing `busy-5.3.3/busy/command/print_command.py` & `busy-5.3.4/busy/command/print_command.py`

 * *Files identical despite different names*

### Comparing `busy-5.3.3/busy/command/switch_command.py` & `busy-5.3.4/busy/command/switch_command.py`

 * *Files identical despite different names*

### Comparing `busy-5.3.3/busy/handler.py` & `busy-5.3.4/busy/handler.py`

 * *Files identical despite different names*

### Comparing `busy-5.3.3/busy/model/collection/__init__.py` & `busy-5.3.4/busy/model/collection/__init__.py`

 * *Files identical despite different names*

### Comparing `busy-5.3.3/busy/model/item.py` & `busy-5.3.4/busy/model/item.py`

 * *Files identical despite different names*

### Comparing `busy-5.3.3/busy/storage/file_storage.py` & `busy-5.3.4/busy/storage/file_storage.py`

 * *Files identical despite different names*

### Comparing `busy-5.3.3/busy/ui/curses_ui.py` & `busy-5.3.4/busy/ui/curses_ui.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,15 +47,17 @@
         chooser.add_choice(keys=['q'], words=['quit'])
         self._command_prompt = chooser
 
         curses.wrapper(self.term_loop)
 
     def output(self, intro=""):
         self._descwin.clear()
-        self._descwin.addstr(intro)
+        maxy, maxx = self._descwin.getmaxyx()
+        lines = intro.split("\n")
+        self._descwin.addstr('\n'.join(lines[0:maxy-1]))
         self._descwin.refresh()
 
     def write_prompt(self, prompt):
         """
         Output the prompt with underlines to the window.
         """
         window = self._statuswin
```

### Comparing `busy-5.3.3/busy/ui/shell_ui.py` & `busy-5.3.4/busy/ui/shell_ui.py`

 * *Files identical despite different names*

### Comparing `busy-5.3.3/busy/ui/tcl_ui/edit_task_widget.py` & `busy-5.3.4/busy/ui/tcl_ui/edit_task_widget.py`

 * *Files identical despite different names*

### Comparing `busy-5.3.3/busy/ui/tcl_ui/get_item_widget.py` & `busy-5.3.4/busy/ui/tcl_ui/get_item_widget.py`

 * *Files identical despite different names*

### Comparing `busy-5.3.3/busy/ui/ui.py` & `busy-5.3.4/busy/ui/ui.py`

 * *Files identical despite different names*

### Comparing `busy-5.3.3/busy/util/checklist.py` & `busy-5.3.4/busy/util/checklist.py`

 * *Files identical despite different names*

### Comparing `busy-5.3.3/busy/util/date_util.py` & `busy-5.3.4/busy/util/date_util.py`

 * *Files identical despite different names*

### Comparing `busy-5.3.3/busy/util/selector.py` & `busy-5.3.4/busy/util/selector.py`

 * *Files identical despite different names*

### Comparing `busy-5.3.3/busy.egg-info/PKG-INFO` & `busy-5.3.4/busy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: busy
-Version: 5.3.3
+Version: 5.3.4
 Summary: Personal time management for techies
 Author-email: Francis Potter <busy@steampunkwizard.ca>
 License: MIT
 Requires-Python: >=3.6.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `busy-5.3.3/busy.egg-info/SOURCES.txt` & `busy-5.3.4/busy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `busy-5.3.3/pyproject.toml` & `busy-5.3.4/pyproject.toml`

 * *Files identical despite different names*

