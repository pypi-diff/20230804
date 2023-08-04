# Comparing `tmp/flowmatic-0.1.0.1.tar.gz` & `tmp/flowmatic-0.1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flowmatic-0.1.0.1.tar", max compression
+gzip compressed data, was "flowmatic-0.1.0.2.tar", max compression
```

## Comparing `flowmatic-0.1.0.1.tar` & `flowmatic-0.1.0.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0       46 2023-08-04 13:30:55.255141 flowmatic-0.1.0.1/README.md
--rw-r--r--   0        0        0       51 2023-08-04 13:30:55.255141 flowmatic-0.1.0.1/flowmatic/README.md
--rw-r--r--   0        0        0     1068 2023-08-04 13:30:55.255141 flowmatic-0.1.0.1/flowmatic/__init__.py
--rw-r--r--   0        0        0     1375 2023-08-04 13:30:55.255141 flowmatic-0.1.0.1/flowmatic/flowmatic.py
--rw-r--r--   0        0        0       23 2023-08-04 13:30:55.255141 flowmatic-0.1.0.1/flowmatic/flows/__init__.py
--rw-r--r--   0        0        0      911 2023-08-04 13:30:55.255141 flowmatic-0.1.0.1/flowmatic/flows/flow.py
--rw-r--r--   0        0        0       61 2023-08-04 13:30:55.255141 flowmatic-0.1.0.1/flowmatic/forms/__init__.py
--rw-r--r--   0        0        0      129 2023-08-04 13:30:55.255141 flowmatic-0.1.0.1/flowmatic/forms/fields/__init__.py
--rw-r--r--   0        0        0      632 2023-08-04 13:30:55.255141 flowmatic-0.1.0.1/flowmatic/forms/fields/field.py
--rw-r--r--   0        0        0     4856 2023-08-04 13:30:55.255141 flowmatic-0.1.0.1/flowmatic/forms/fields/file_field.py
--rw-r--r--   0        0        0     1381 2023-08-04 13:30:55.255141 flowmatic-0.1.0.1/flowmatic/forms/fields/radio_group.py
--rw-r--r--   0        0        0     1575 2023-08-04 13:30:55.255141 flowmatic-0.1.0.1/flowmatic/forms/fields/text_field.py
--rw-r--r--   0        0        0      665 2023-08-04 13:30:55.255141 flowmatic-0.1.0.1/flowmatic/forms/validation.py
--rw-r--r--   0        0        0      230 2023-08-04 13:30:55.255141 flowmatic-0.1.0.1/flowmatic/gui/__init__.py
--rw-r--r--   0        0        0       34 2023-08-04 13:30:55.255141 flowmatic-0.1.0.1/flowmatic/gui/elements/__init__.py
--rw-r--r--   0        0        0      114 2023-08-04 13:30:55.255141 flowmatic-0.1.0.1/flowmatic/gui/elements/element_infos.py
--rw-r--r--   0        0        0      620 2023-08-04 13:30:55.255141 flowmatic-0.1.0.1/flowmatic/gui/gui.py
--rw-r--r--   0        0        0      141 2023-08-04 13:30:55.255141 flowmatic-0.1.0.1/flowmatic/gui/screens/__init__.py
--rw-r--r--   0        0        0     3549 2023-08-04 13:30:55.255141 flowmatic-0.1.0.1/flowmatic/gui/screens/form_screen.py
--rw-r--r--   0        0        0      773 2023-08-04 13:30:55.255141 flowmatic-0.1.0.1/flowmatic/gui/screens/menu_screen.py
--rw-r--r--   0        0        0      830 2023-08-04 13:30:55.259141 flowmatic-0.1.0.1/flowmatic/gui/screens/screen.py
--rw-r--r--   0        0        0      690 2023-08-04 13:30:55.259141 flowmatic-0.1.0.1/flowmatic/gui/screens/title_screen.py
--rw-r--r--   0        0        0       99 2023-08-04 13:30:55.259141 flowmatic-0.1.0.1/flowmatic/gui/style/__init__.py
--rw-r--r--   0        0        0     1856 2023-08-04 13:30:55.259141 flowmatic-0.1.0.1/flowmatic/gui/tkgui.py
--rw-r--r--   0        0        0       56 2023-08-04 13:30:55.259141 flowmatic-0.1.0.1/flowmatic/server.py
--rw-r--r--   0        0        0      209 2023-08-04 13:30:55.259141 flowmatic-0.1.0.1/flowmatic/util/__init__.py
--rw-r--r--   0        0        0      568 2023-08-04 13:30:55.259141 flowmatic-0.1.0.1/flowmatic/util/exceptions.py
--rw-r--r--   0        0        0     1135 2023-08-04 13:30:55.259141 flowmatic-0.1.0.1/flowmatic/util/icons.py
--rw-r--r--   0        0        0     1442 2023-08-04 13:30:55.259141 flowmatic-0.1.0.1/flowmatic/util/saved_class.py
--rw-r--r--   0        0        0       77 2023-08-04 13:30:55.259141 flowmatic-0.1.0.1/flowmatic/util/settings.py
--rw-r--r--   0        0        0      225 2023-08-04 13:30:55.259141 flowmatic-0.1.0.1/flowmatic/util/singleton.py
--rw-r--r--   0        0        0       73 2023-08-04 13:30:55.259141 flowmatic-0.1.0.1/flowmatic/util/user.py
--rw-r--r--   0        0        0      366 2023-08-04 13:30:55.259141 flowmatic-0.1.0.1/pyproject.toml
--rw-r--r--   0        0        0      495 1970-01-01 00:00:00.000000 flowmatic-0.1.0.1/PKG-INFO
+-rw-r--r--   0        0        0       46 2023-08-04 13:41:36.940938 flowmatic-0.1.0.2/README.md
+-rw-r--r--   0        0        0       51 2023-08-04 13:41:36.940938 flowmatic-0.1.0.2/flowmatic/README.md
+-rw-r--r--   0        0        0     1068 2023-08-04 13:41:36.940938 flowmatic-0.1.0.2/flowmatic/__init__.py
+-rw-r--r--   0        0        0     1438 2023-08-04 13:41:36.940938 flowmatic-0.1.0.2/flowmatic/flowmatic.py
+-rw-r--r--   0        0        0       23 2023-08-04 13:41:36.940938 flowmatic-0.1.0.2/flowmatic/flows/__init__.py
+-rw-r--r--   0        0        0      911 2023-08-04 13:41:36.940938 flowmatic-0.1.0.2/flowmatic/flows/flow.py
+-rw-r--r--   0        0        0       61 2023-08-04 13:41:36.940938 flowmatic-0.1.0.2/flowmatic/forms/__init__.py
+-rw-r--r--   0        0        0      129 2023-08-04 13:41:36.940938 flowmatic-0.1.0.2/flowmatic/forms/fields/__init__.py
+-rw-r--r--   0        0        0      632 2023-08-04 13:41:36.940938 flowmatic-0.1.0.2/flowmatic/forms/fields/field.py
+-rw-r--r--   0        0        0     4856 2023-08-04 13:41:36.940938 flowmatic-0.1.0.2/flowmatic/forms/fields/file_field.py
+-rw-r--r--   0        0        0     1381 2023-08-04 13:41:36.940938 flowmatic-0.1.0.2/flowmatic/forms/fields/radio_group.py
+-rw-r--r--   0        0        0     1575 2023-08-04 13:41:36.940938 flowmatic-0.1.0.2/flowmatic/forms/fields/text_field.py
+-rw-r--r--   0        0        0      665 2023-08-04 13:41:36.940938 flowmatic-0.1.0.2/flowmatic/forms/validation.py
+-rw-r--r--   0        0        0      230 2023-08-04 13:41:36.940938 flowmatic-0.1.0.2/flowmatic/gui/__init__.py
+-rw-r--r--   0        0        0       34 2023-08-04 13:41:36.940938 flowmatic-0.1.0.2/flowmatic/gui/elements/__init__.py
+-rw-r--r--   0        0        0      114 2023-08-04 13:41:36.940938 flowmatic-0.1.0.2/flowmatic/gui/elements/element_infos.py
+-rw-r--r--   0        0        0      620 2023-08-04 13:41:36.940938 flowmatic-0.1.0.2/flowmatic/gui/gui.py
+-rw-r--r--   0        0        0      141 2023-08-04 13:41:36.940938 flowmatic-0.1.0.2/flowmatic/gui/screens/__init__.py
+-rw-r--r--   0        0        0     3549 2023-08-04 13:41:36.940938 flowmatic-0.1.0.2/flowmatic/gui/screens/form_screen.py
+-rw-r--r--   0        0        0      773 2023-08-04 13:41:36.940938 flowmatic-0.1.0.2/flowmatic/gui/screens/menu_screen.py
+-rw-r--r--   0        0        0      830 2023-08-04 13:41:36.940938 flowmatic-0.1.0.2/flowmatic/gui/screens/screen.py
+-rw-r--r--   0        0        0      690 2023-08-04 13:41:36.940938 flowmatic-0.1.0.2/flowmatic/gui/screens/title_screen.py
+-rw-r--r--   0        0        0       99 2023-08-04 13:41:36.940938 flowmatic-0.1.0.2/flowmatic/gui/style/__init__.py
+-rw-r--r--   0        0        0     1856 2023-08-04 13:41:36.940938 flowmatic-0.1.0.2/flowmatic/gui/tkgui.py
+-rw-r--r--   0        0        0       56 2023-08-04 13:41:36.940938 flowmatic-0.1.0.2/flowmatic/server.py
+-rw-r--r--   0        0        0      209 2023-08-04 13:41:36.940938 flowmatic-0.1.0.2/flowmatic/util/__init__.py
+-rw-r--r--   0        0        0      568 2023-08-04 13:41:36.940938 flowmatic-0.1.0.2/flowmatic/util/exceptions.py
+-rw-r--r--   0        0        0     1135 2023-08-04 13:41:36.940938 flowmatic-0.1.0.2/flowmatic/util/icons.py
+-rw-r--r--   0        0        0     1442 2023-08-04 13:41:36.940938 flowmatic-0.1.0.2/flowmatic/util/saved_class.py
+-rw-r--r--   0        0        0       77 2023-08-04 13:41:36.940938 flowmatic-0.1.0.2/flowmatic/util/settings.py
+-rw-r--r--   0        0        0      225 2023-08-04 13:41:36.940938 flowmatic-0.1.0.2/flowmatic/util/singleton.py
+-rw-r--r--   0        0        0       73 2023-08-04 13:41:36.940938 flowmatic-0.1.0.2/flowmatic/util/user.py
+-rw-r--r--   0        0        0      366 2023-08-04 13:41:36.940938 flowmatic-0.1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      495 1970-01-01 00:00:00.000000 flowmatic-0.1.0.2/PKG-INFO
```

### Comparing `flowmatic-0.1.0.1/flowmatic/__init__.py` & `flowmatic-0.1.0.2/flowmatic/__init__.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.0.1/flowmatic/flowmatic.py` & `flowmatic-0.1.0.2/flowmatic/flowmatic.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,15 +20,16 @@
     title: str = "FlowMatic"
     gui: GUI = None  # type: ignore
     settings: Settings
     user: User
 
     start_screen: Screen
 
-    def __init__(self):
+    def __init__(self, start_screen: Screen):
+        self.start_screen = start_screen
         self.gui = self.gui or TKGUI(
             title=self.title, start_screen=self.start_screen, geometry="1280x720"
         )
         self.settings = Settings.load("files/settings.json")
         self.user = User("")
 
     def start(
```

### Comparing `flowmatic-0.1.0.1/flowmatic/flows/flow.py` & `flowmatic-0.1.0.2/flowmatic/flows/flow.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.0.1/flowmatic/forms/fields/field.py` & `flowmatic-0.1.0.2/flowmatic/forms/fields/field.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.0.1/flowmatic/forms/fields/file_field.py` & `flowmatic-0.1.0.2/flowmatic/forms/fields/file_field.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.0.1/flowmatic/forms/fields/radio_group.py` & `flowmatic-0.1.0.2/flowmatic/forms/fields/radio_group.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.0.1/flowmatic/forms/fields/text_field.py` & `flowmatic-0.1.0.2/flowmatic/forms/fields/text_field.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.0.1/flowmatic/forms/validation.py` & `flowmatic-0.1.0.2/flowmatic/forms/validation.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.0.1/flowmatic/gui/gui.py` & `flowmatic-0.1.0.2/flowmatic/gui/gui.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.0.1/flowmatic/gui/screens/form_screen.py` & `flowmatic-0.1.0.2/flowmatic/gui/screens/form_screen.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.0.1/flowmatic/gui/screens/menu_screen.py` & `flowmatic-0.1.0.2/flowmatic/gui/screens/menu_screen.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.0.1/flowmatic/gui/screens/screen.py` & `flowmatic-0.1.0.2/flowmatic/gui/screens/screen.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.0.1/flowmatic/gui/screens/title_screen.py` & `flowmatic-0.1.0.2/flowmatic/gui/screens/title_screen.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.0.1/flowmatic/gui/tkgui.py` & `flowmatic-0.1.0.2/flowmatic/gui/tkgui.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.0.1/flowmatic/util/exceptions.py` & `flowmatic-0.1.0.2/flowmatic/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.0.1/flowmatic/util/icons.py` & `flowmatic-0.1.0.2/flowmatic/util/icons.py`

 * *Files identical despite different names*

### Comparing `flowmatic-0.1.0.1/flowmatic/util/saved_class.py` & `flowmatic-0.1.0.2/flowmatic/util/saved_class.py`

 * *Files identical despite different names*

