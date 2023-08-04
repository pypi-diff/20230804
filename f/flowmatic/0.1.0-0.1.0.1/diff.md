# Comparing `tmp/flowmatic-0.1.0.tar.gz` & `tmp/flowmatic-0.1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flowmatic-0.1.0.tar", max compression
+gzip compressed data, was "flowmatic-0.1.0.1.tar", max compression
```

## Comparing `flowmatic-0.1.0.tar` & `flowmatic-0.1.0.1.tar`

### file list

```diff
@@ -1,33 +1,34 @@
--rw-r--r--   0        0        0       45 2023-07-21 16:14:29.790328 flowmatic-0.1.0/README.md
--rw-r--r--   0        0        0     1018 2023-08-03 19:12:09.055231 flowmatic-0.1.0/flowmatic/__init__.py
--rw-r--r--   0        0        0     1369 2023-08-03 19:12:25.618022 flowmatic-0.1.0/flowmatic/flowmatic.py
--rw-r--r--   0        0        0       23 2023-08-03 17:19:06.570805 flowmatic-0.1.0/flowmatic/flows/__init__.py
--rw-r--r--   0        0        0      911 2023-08-03 19:13:35.680948 flowmatic-0.1.0/flowmatic/flows/flow.py
--rw-r--r--   0        0        0       61 2023-08-03 18:26:50.079008 flowmatic-0.1.0/flowmatic/forms/__init__.py
--rw-r--r--   0        0        0      129 2023-07-24 17:53:30.077799 flowmatic-0.1.0/flowmatic/forms/fields/__init__.py
--rw-r--r--   0        0        0      632 2023-08-03 18:24:49.723342 flowmatic-0.1.0/flowmatic/forms/fields/field.py
--rw-r--r--   0        0        0     4856 2023-08-03 19:13:38.342628 flowmatic-0.1.0/flowmatic/forms/fields/file_field.py
--rw-r--r--   0        0        0     1381 2023-08-03 19:13:44.569066 flowmatic-0.1.0/flowmatic/forms/fields/radio_group.py
--rw-r--r--   0        0        0     1575 2023-08-03 18:25:43.937900 flowmatic-0.1.0/flowmatic/forms/fields/text_field.py
--rw-r--r--   0        0        0      665 2023-08-03 18:26:01.647054 flowmatic-0.1.0/flowmatic/forms/validation.py
--rw-r--r--   0        0        0      230 2023-07-25 18:00:22.957457 flowmatic-0.1.0/flowmatic/gui/__init__.py
--rw-r--r--   0        0        0       34 2023-08-03 18:04:14.349035 flowmatic-0.1.0/flowmatic/gui/elements/__init__.py
--rw-r--r--   0        0        0      114 2023-08-03 18:04:14.776051 flowmatic-0.1.0/flowmatic/gui/elements/element_infos.py
--rw-r--r--   0        0        0      620 2023-08-03 17:26:16.133827 flowmatic-0.1.0/flowmatic/gui/gui.py
--rw-r--r--   0        0        0      141 2023-08-03 16:43:19.056726 flowmatic-0.1.0/flowmatic/gui/screens/__init__.py
--rw-r--r--   0        0        0     3549 2023-08-03 19:13:48.229952 flowmatic-0.1.0/flowmatic/gui/screens/form_screen.py
--rw-r--r--   0        0        0      773 2023-08-03 19:13:49.139651 flowmatic-0.1.0/flowmatic/gui/screens/menu_screen.py
--rw-r--r--   0        0        0      830 2023-08-03 18:26:50.012027 flowmatic-0.1.0/flowmatic/gui/screens/screen.py
--rw-r--r--   0        0        0      690 2023-08-03 19:13:53.030208 flowmatic-0.1.0/flowmatic/gui/screens/title_screen.py
--rw-r--r--   0        0        0       99 2023-08-03 18:26:50.045750 flowmatic-0.1.0/flowmatic/gui/style/__init__.py
--rw-r--r--   0        0        0     1856 2023-08-03 19:13:47.426758 flowmatic-0.1.0/flowmatic/gui/tkgui.py
--rw-r--r--   0        0        0       56 2023-08-03 19:12:09.064638 flowmatic-0.1.0/flowmatic/server.py
--rw-r--r--   0        0        0      209 2023-08-02 17:38:37.416214 flowmatic-0.1.0/flowmatic/util/__init__.py
--rw-r--r--   0        0        0      568 2023-08-03 18:26:50.045768 flowmatic-0.1.0/flowmatic/util/exceptions.py
--rw-r--r--   0        0        0     1135 2023-07-28 08:15:57.031850 flowmatic-0.1.0/flowmatic/util/icons.py
--rw-r--r--   0        0        0     1442 2023-08-03 19:13:52.392401 flowmatic-0.1.0/flowmatic/util/saved_class.py
--rw-r--r--   0        0        0       77 2023-08-03 19:13:55.246023 flowmatic-0.1.0/flowmatic/util/settings.py
--rw-r--r--   0        0        0      225 2023-08-03 18:26:50.045780 flowmatic-0.1.0/flowmatic/util/singleton.py
--rw-r--r--   0        0        0       73 2023-08-03 19:13:56.642042 flowmatic-0.1.0/flowmatic/util/user.py
--rw-r--r--   0        0        0      364 2023-08-03 19:11:05.906075 flowmatic-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      492 1970-01-01 00:00:00.000000 flowmatic-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       46 2023-08-04 13:30:55.255141 flowmatic-0.1.0.1/README.md
+-rw-r--r--   0        0        0       51 2023-08-04 13:30:55.255141 flowmatic-0.1.0.1/flowmatic/README.md
+-rw-r--r--   0        0        0     1068 2023-08-04 13:30:55.255141 flowmatic-0.1.0.1/flowmatic/__init__.py
+-rw-r--r--   0        0        0     1375 2023-08-04 13:30:55.255141 flowmatic-0.1.0.1/flowmatic/flowmatic.py
+-rw-r--r--   0        0        0       23 2023-08-04 13:30:55.255141 flowmatic-0.1.0.1/flowmatic/flows/__init__.py
+-rw-r--r--   0        0        0      911 2023-08-04 13:30:55.255141 flowmatic-0.1.0.1/flowmatic/flows/flow.py
+-rw-r--r--   0        0        0       61 2023-08-04 13:30:55.255141 flowmatic-0.1.0.1/flowmatic/forms/__init__.py
+-rw-r--r--   0        0        0      129 2023-08-04 13:30:55.255141 flowmatic-0.1.0.1/flowmatic/forms/fields/__init__.py
+-rw-r--r--   0        0        0      632 2023-08-04 13:30:55.255141 flowmatic-0.1.0.1/flowmatic/forms/fields/field.py
+-rw-r--r--   0        0        0     4856 2023-08-04 13:30:55.255141 flowmatic-0.1.0.1/flowmatic/forms/fields/file_field.py
+-rw-r--r--   0        0        0     1381 2023-08-04 13:30:55.255141 flowmatic-0.1.0.1/flowmatic/forms/fields/radio_group.py
+-rw-r--r--   0        0        0     1575 2023-08-04 13:30:55.255141 flowmatic-0.1.0.1/flowmatic/forms/fields/text_field.py
+-rw-r--r--   0        0        0      665 2023-08-04 13:30:55.255141 flowmatic-0.1.0.1/flowmatic/forms/validation.py
+-rw-r--r--   0        0        0      230 2023-08-04 13:30:55.255141 flowmatic-0.1.0.1/flowmatic/gui/__init__.py
+-rw-r--r--   0        0        0       34 2023-08-04 13:30:55.255141 flowmatic-0.1.0.1/flowmatic/gui/elements/__init__.py
+-rw-r--r--   0        0        0      114 2023-08-04 13:30:55.255141 flowmatic-0.1.0.1/flowmatic/gui/elements/element_infos.py
+-rw-r--r--   0        0        0      620 2023-08-04 13:30:55.255141 flowmatic-0.1.0.1/flowmatic/gui/gui.py
+-rw-r--r--   0        0        0      141 2023-08-04 13:30:55.255141 flowmatic-0.1.0.1/flowmatic/gui/screens/__init__.py
+-rw-r--r--   0        0        0     3549 2023-08-04 13:30:55.255141 flowmatic-0.1.0.1/flowmatic/gui/screens/form_screen.py
+-rw-r--r--   0        0        0      773 2023-08-04 13:30:55.255141 flowmatic-0.1.0.1/flowmatic/gui/screens/menu_screen.py
+-rw-r--r--   0        0        0      830 2023-08-04 13:30:55.259141 flowmatic-0.1.0.1/flowmatic/gui/screens/screen.py
+-rw-r--r--   0        0        0      690 2023-08-04 13:30:55.259141 flowmatic-0.1.0.1/flowmatic/gui/screens/title_screen.py
+-rw-r--r--   0        0        0       99 2023-08-04 13:30:55.259141 flowmatic-0.1.0.1/flowmatic/gui/style/__init__.py
+-rw-r--r--   0        0        0     1856 2023-08-04 13:30:55.259141 flowmatic-0.1.0.1/flowmatic/gui/tkgui.py
+-rw-r--r--   0        0        0       56 2023-08-04 13:30:55.259141 flowmatic-0.1.0.1/flowmatic/server.py
+-rw-r--r--   0        0        0      209 2023-08-04 13:30:55.259141 flowmatic-0.1.0.1/flowmatic/util/__init__.py
+-rw-r--r--   0        0        0      568 2023-08-04 13:30:55.259141 flowmatic-0.1.0.1/flowmatic/util/exceptions.py
+-rw-r--r--   0        0        0     1135 2023-08-04 13:30:55.259141 flowmatic-0.1.0.1/flowmatic/util/icons.py
+-rw-r--r--   0        0        0     1442 2023-08-04 13:30:55.259141 flowmatic-0.1.0.1/flowmatic/util/saved_class.py
+-rw-r--r--   0        0        0       77 2023-08-04 13:30:55.259141 flowmatic-0.1.0.1/flowmatic/util/settings.py
+-rw-r--r--   0        0        0      225 2023-08-04 13:30:55.259141 flowmatic-0.1.0.1/flowmatic/util/singleton.py
+-rw-r--r--   0        0        0       73 2023-08-04 13:30:55.259141 flowmatic-0.1.0.1/flowmatic/util/user.py
+-rw-r--r--   0        0        0      366 2023-08-04 13:30:55.259141 flowmatic-0.1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      495 1970-01-01 00:00:00.000000 flowmatic-0.1.0.1/PKG-INFO
```

### Comparing `flowmatic-0.1.0/flowmatic/__init__.py` & `flowmatic-0.1.0.1/flowmatic/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from .gui.screens.screen import Screen
+from .gui.screens import *
+from .gui.screens.screen import *
+from .gui.elements import *
 from .flows.flow import Flow
 from .server import Server
 from .util import Settings
 from .flowmatic import App
 
 
 server = Server()
```

### Comparing `flowmatic-0.1.0/flowmatic/flowmatic.py` & `flowmatic-0.1.0.1/flowmatic/flowmatic.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         settings (Settings): Settings.
         user (User): User.
 
     Args:
         title (str, optional): Title of the app. Defaults to "Appy".
     """
 
-    title: str = "App"
+    title: str = "FlowMatic"
     gui: GUI = None  # type: ignore
     settings: Settings
     user: User
 
     start_screen: Screen
 
     def __init__(self):
```

### Comparing `flowmatic-0.1.0/flowmatic/flows/flow.py` & `flowmatic-0.1.0.1/flowmatic/flows/flow.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.0/flowmatic/forms/fields/field.py` & `flowmatic-0.1.0.1/flowmatic/forms/fields/field.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.0/flowmatic/forms/fields/file_field.py` & `flowmatic-0.1.0.1/flowmatic/forms/fields/file_field.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.0/flowmatic/forms/fields/radio_group.py` & `flowmatic-0.1.0.1/flowmatic/forms/fields/radio_group.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.0/flowmatic/forms/fields/text_field.py` & `flowmatic-0.1.0.1/flowmatic/forms/fields/text_field.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.0/flowmatic/forms/validation.py` & `flowmatic-0.1.0.1/flowmatic/forms/validation.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.0/flowmatic/gui/gui.py` & `flowmatic-0.1.0.1/flowmatic/gui/gui.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.0/flowmatic/gui/screens/form_screen.py` & `flowmatic-0.1.0.1/flowmatic/gui/screens/form_screen.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.0/flowmatic/gui/screens/menu_screen.py` & `flowmatic-0.1.0.1/flowmatic/gui/screens/menu_screen.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.0/flowmatic/gui/screens/screen.py` & `flowmatic-0.1.0.1/flowmatic/gui/screens/screen.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.0/flowmatic/gui/screens/title_screen.py` & `flowmatic-0.1.0.1/flowmatic/gui/screens/title_screen.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.0/flowmatic/gui/tkgui.py` & `flowmatic-0.1.0.1/flowmatic/gui/tkgui.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.0/flowmatic/util/exceptions.py` & `flowmatic-0.1.0.1/flowmatic/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.0/flowmatic/util/icons.py` & `flowmatic-0.1.0.1/flowmatic/util/icons.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.0/flowmatic/util/saved_class.py` & `flowmatic-0.1.0.1/flowmatic/util/saved_class.py`

 * *Files identical despite different names*

