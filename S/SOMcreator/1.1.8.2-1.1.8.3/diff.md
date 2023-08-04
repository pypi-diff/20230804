# Comparing `tmp/SOMcreator-1.1.8.2.tar.gz` & `tmp/SOMcreator-1.1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SOMcreator-1.1.8.2.tar", last modified: Wed Aug  2 07:02:08 2023, max compression
+gzip compressed data, was "SOMcreator-1.1.8.3.tar", last modified: Fri Aug  4 09:33:15 2023, max compression
```

## Comparing `SOMcreator-1.1.8.2.tar` & `SOMcreator-1.1.8.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 07:02:08.936198 SOMcreator-1.1.8.2/
--rw-rw-rw-   0        0        0     1095 2022-10-28 12:14:14.000000 SOMcreator-1.1.8.2/LICENSE
--rw-rw-rw-   0        0        0       81 2022-11-01 07:22:32.000000 SOMcreator-1.1.8.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1556 2023-08-02 07:02:08.935963 SOMcreator-1.1.8.2/PKG-INFO
--rw-rw-rw-   0        0        0        9 2022-10-28 11:24:11.000000 SOMcreator-1.1.8.2/README.md
--rw-rw-rw-   0        0        0      876 2023-03-20 13:30:05.000000 SOMcreator-1.1.8.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-02 07:02:08.936198 SOMcreator-1.1.8.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-02 07:02:08.706434 SOMcreator-1.1.8.2/src/
-drwxrwxrwx   0        0        0        0 2023-08-02 07:02:08.740712 SOMcreator-1.1.8.2/src/SOMcreator/
-drwxrwxrwx   0        0        0        0 2023-08-02 07:02:08.814039 SOMcreator-1.1.8.2/src/SOMcreator/Template/
--rw-rw-rw-   0        0        0      375 2023-05-16 05:28:24.000000 SOMcreator-1.1.8.2/src/SOMcreator/Template/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 07:02:08.829525 SOMcreator-1.1.8.2/src/SOMcreator/Template/__pyinstaller/
--rw-rw-rw-   0        0        0       71 2023-04-06 10:29:25.000000 SOMcreator-1.1.8.2/src/SOMcreator/Template/__pyinstaller/__init__.py
--rw-rw-rw-   0        0        0      202 2023-04-06 10:29:25.000000 SOMcreator-1.1.8.2/src/SOMcreator/Template/__pyinstaller/hook-SOMcreator.py
--rw-rw-rw-   0        0        0      331 2023-04-06 10:29:25.000000 SOMcreator-1.1.8.2/src/SOMcreator/Template/bookmark_template.txt
--rw-rw-rw-   0        0        0    25168 2023-04-06 10:29:25.000000 SOMcreator-1.1.8.2/src/SOMcreator/Template/ifc.json
-drwxrwxrwx   0        0        0        0 2023-08-02 07:02:08.873396 SOMcreator-1.1.8.2/src/SOMcreator/Template/js_templates/
--rw-rw-rw-   0        0        0     1001 2023-04-06 10:29:25.000000 SOMcreator-1.1.8.2/src/SOMcreator/Template/js_templates/end_ungetestet.js
--rw-rw-rw-   0        0        0     7071 2023-04-06 10:29:25.000000 SOMcreator-1.1.8.2/src/SOMcreator/Template/js_templates/start_check_start.js
--rw-rw-rw-   0        0        0      598 2023-04-06 10:29:25.000000 SOMcreator-1.1.8.2/src/SOMcreator/Template/js_templates/start_koordinaten.js
--rw-rw-rw-   0        0        0     2938 2023-04-06 10:29:25.000000 SOMcreator-1.1.8.2/src/SOMcreator/Template/mapping_template.txt
--rw-rw-rw-   0        0        0     3121 2023-04-06 10:29:25.000000 SOMcreator-1.1.8.2/src/SOMcreator/Template/template.txt
--rw-rw-rw-   0        0        0      156 2023-08-02 07:01:42.000000 SOMcreator-1.1.8.2/src/SOMcreator/__init__.py
--rw-rw-rw-   0        0        0    24588 2023-08-01 15:38:40.000000 SOMcreator-1.1.8.2/src/SOMcreator/classes.py
--rw-rw-rw-   0        0        0     1898 2023-05-04 10:57:17.000000 SOMcreator-1.1.8.2/src/SOMcreator/constants.py
-drwxrwxrwx   0        0        0        0 2023-08-02 07:02:08.934473 SOMcreator-1.1.8.2/src/SOMcreator/external_software/
--rw-rw-rw-   0        0        0        0 2023-04-06 10:29:25.000000 SOMcreator-1.1.8.2/src/SOMcreator/external_software/__init__.py
--rw-rw-rw-   0        0        0     4311 2023-04-06 10:29:25.000000 SOMcreator-1.1.8.2/src/SOMcreator/external_software/allplan.py
--rw-rw-rw-   0        0        0     1365 2023-04-06 10:29:25.000000 SOMcreator-1.1.8.2/src/SOMcreator/external_software/card1.py
--rw-rw-rw-   0        0        0    22074 2023-08-02 06:22:43.000000 SOMcreator-1.1.8.2/src/SOMcreator/external_software/desite.py
--rw-rw-rw-   0        0        0    21951 2023-06-28 13:16:14.000000 SOMcreator-1.1.8.2/src/SOMcreator/external_software/excel.py
--rw-rw-rw-   0        0        0     3326 2023-05-04 10:57:17.000000 SOMcreator-1.1.8.2/src/SOMcreator/external_software/revit.py
--rw-rw-rw-   0        0        0     3227 2023-04-06 10:29:25.000000 SOMcreator-1.1.8.2/src/SOMcreator/external_software/vestra.py
--rw-rw-rw-   0        0        0     9397 2023-08-01 15:25:56.000000 SOMcreator-1.1.8.2/src/SOMcreator/filehandling.py
--rw-rw-rw-   0        0        0      970 2023-04-06 10:29:25.000000 SOMcreator-1.1.8.2/src/SOMcreator/quality_check.py
-drwxrwxrwx   0        0        0        0 2023-08-02 07:02:08.765737 SOMcreator-1.1.8.2/src/SOMcreator.egg-info/
--rw-rw-rw-   0        0        0     1556 2023-08-02 07:02:08.000000 SOMcreator-1.1.8.2/src/SOMcreator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1194 2023-08-02 07:02:08.000000 SOMcreator-1.1.8.2/src/SOMcreator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 07:02:08.000000 SOMcreator-1.1.8.2/src/SOMcreator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2023-08-02 07:02:08.000000 SOMcreator-1.1.8.2/src/SOMcreator.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2023-08-02 07:02:08.000000 SOMcreator-1.1.8.2/src/SOMcreator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-08-02 07:02:08.000000 SOMcreator-1.1.8.2/src/SOMcreator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-04 09:33:15.664758 SOMcreator-1.1.8.3/
+-rw-rw-rw-   0        0        0     1095 2022-10-28 12:14:14.000000 SOMcreator-1.1.8.3/LICENSE
+-rw-rw-rw-   0        0        0       81 2022-11-01 07:22:32.000000 SOMcreator-1.1.8.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1556 2023-08-04 09:33:15.663717 SOMcreator-1.1.8.3/PKG-INFO
+-rw-rw-rw-   0        0        0        9 2022-10-28 11:24:11.000000 SOMcreator-1.1.8.3/README.md
+-rw-rw-rw-   0        0        0      876 2023-03-20 13:30:05.000000 SOMcreator-1.1.8.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-04 09:33:15.665258 SOMcreator-1.1.8.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-04 09:33:15.441687 SOMcreator-1.1.8.3/src/
+drwxrwxrwx   0        0        0        0 2023-08-04 09:33:15.476686 SOMcreator-1.1.8.3/src/SOMcreator/
+drwxrwxrwx   0        0        0        0 2023-08-04 09:33:15.555880 SOMcreator-1.1.8.3/src/SOMcreator/Template/
+-rw-rw-rw-   0        0        0      375 2023-05-16 05:28:24.000000 SOMcreator-1.1.8.3/src/SOMcreator/Template/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-04 09:33:15.567367 SOMcreator-1.1.8.3/src/SOMcreator/Template/__pyinstaller/
+-rw-rw-rw-   0        0        0       71 2023-04-06 10:29:25.000000 SOMcreator-1.1.8.3/src/SOMcreator/Template/__pyinstaller/__init__.py
+-rw-rw-rw-   0        0        0      202 2023-04-06 10:29:25.000000 SOMcreator-1.1.8.3/src/SOMcreator/Template/__pyinstaller/hook-SOMcreator.py
+-rw-rw-rw-   0        0        0      331 2023-04-06 10:29:25.000000 SOMcreator-1.1.8.3/src/SOMcreator/Template/bookmark_template.txt
+-rw-rw-rw-   0        0        0    25168 2023-04-06 10:29:25.000000 SOMcreator-1.1.8.3/src/SOMcreator/Template/ifc.json
+drwxrwxrwx   0        0        0        0 2023-08-04 09:33:15.605855 SOMcreator-1.1.8.3/src/SOMcreator/Template/js_templates/
+-rw-rw-rw-   0        0        0     1001 2023-04-06 10:29:25.000000 SOMcreator-1.1.8.3/src/SOMcreator/Template/js_templates/end_ungetestet.js
+-rw-rw-rw-   0        0        0     7071 2023-04-06 10:29:25.000000 SOMcreator-1.1.8.3/src/SOMcreator/Template/js_templates/start_check_start.js
+-rw-rw-rw-   0        0        0      598 2023-04-06 10:29:25.000000 SOMcreator-1.1.8.3/src/SOMcreator/Template/js_templates/start_koordinaten.js
+-rw-rw-rw-   0        0        0     2938 2023-04-06 10:29:25.000000 SOMcreator-1.1.8.3/src/SOMcreator/Template/mapping_template.txt
+-rw-rw-rw-   0        0        0     3121 2023-04-06 10:29:25.000000 SOMcreator-1.1.8.3/src/SOMcreator/Template/template.txt
+-rw-rw-rw-   0        0        0      156 2023-08-04 09:32:50.000000 SOMcreator-1.1.8.3/src/SOMcreator/__init__.py
+-rw-rw-rw-   0        0        0    25149 2023-08-04 09:32:50.000000 SOMcreator-1.1.8.3/src/SOMcreator/classes.py
+-rw-rw-rw-   0        0        0     1898 2023-05-04 10:57:17.000000 SOMcreator-1.1.8.3/src/SOMcreator/constants.py
+drwxrwxrwx   0        0        0        0 2023-08-04 09:33:15.662713 SOMcreator-1.1.8.3/src/SOMcreator/external_software/
+-rw-rw-rw-   0        0        0        0 2023-04-06 10:29:25.000000 SOMcreator-1.1.8.3/src/SOMcreator/external_software/__init__.py
+-rw-rw-rw-   0        0        0     4311 2023-04-06 10:29:25.000000 SOMcreator-1.1.8.3/src/SOMcreator/external_software/allplan.py
+-rw-rw-rw-   0        0        0     1365 2023-04-06 10:29:25.000000 SOMcreator-1.1.8.3/src/SOMcreator/external_software/card1.py
+-rw-rw-rw-   0        0        0    22074 2023-08-04 09:32:50.000000 SOMcreator-1.1.8.3/src/SOMcreator/external_software/desite.py
+-rw-rw-rw-   0        0        0    21951 2023-06-28 13:16:14.000000 SOMcreator-1.1.8.3/src/SOMcreator/external_software/excel.py
+-rw-rw-rw-   0        0        0     3326 2023-05-04 10:57:17.000000 SOMcreator-1.1.8.3/src/SOMcreator/external_software/revit.py
+-rw-rw-rw-   0        0        0     3227 2023-04-06 10:29:25.000000 SOMcreator-1.1.8.3/src/SOMcreator/external_software/vestra.py
+-rw-rw-rw-   0        0        0     9397 2023-08-01 15:25:56.000000 SOMcreator-1.1.8.3/src/SOMcreator/filehandling.py
+-rw-rw-rw-   0        0        0      970 2023-04-06 10:29:25.000000 SOMcreator-1.1.8.3/src/SOMcreator/quality_check.py
+drwxrwxrwx   0        0        0        0 2023-08-04 09:33:15.513005 SOMcreator-1.1.8.3/src/SOMcreator.egg-info/
+-rw-rw-rw-   0        0        0     1556 2023-08-04 09:33:15.000000 SOMcreator-1.1.8.3/src/SOMcreator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1194 2023-08-04 09:33:15.000000 SOMcreator-1.1.8.3/src/SOMcreator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 09:33:15.000000 SOMcreator-1.1.8.3/src/SOMcreator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2023-08-04 09:33:15.000000 SOMcreator-1.1.8.3/src/SOMcreator.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2023-08-04 09:33:15.000000 SOMcreator-1.1.8.3/src/SOMcreator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-08-04 09:33:15.000000 SOMcreator-1.1.8.3/src/SOMcreator.egg-info/top_level.txt
```

### Comparing `SOMcreator-1.1.8.2/LICENSE` & `SOMcreator-1.1.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.8.2/PKG-INFO` & `SOMcreator-1.1.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SOMcreator
-Version: 1.1.8.2
+Version: 1.1.8.3
 Summary: create simple Datastructures for BIM Models
 License: MIT License
         
         Copyright (c) 2022 Christoph Mellüh
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `SOMcreator-1.1.8.2/pyproject.toml` & `SOMcreator-1.1.8.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.8.2/src/SOMcreator/Template/ifc.json` & `SOMcreator-1.1.8.3/src/SOMcreator/Template/ifc.json`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.8.2/src/SOMcreator/Template/js_templates/end_ungetestet.js` & `SOMcreator-1.1.8.3/src/SOMcreator/Template/js_templates/end_ungetestet.js`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.8.2/src/SOMcreator/Template/js_templates/start_check_start.js` & `SOMcreator-1.1.8.3/src/SOMcreator/Template/js_templates/start_check_start.js`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.8.2/src/SOMcreator/Template/js_templates/start_koordinaten.js` & `SOMcreator-1.1.8.3/src/SOMcreator/Template/js_templates/start_koordinaten.js`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.8.2/src/SOMcreator/Template/mapping_template.txt` & `SOMcreator-1.1.8.3/src/SOMcreator/Template/mapping_template.txt`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.8.2/src/SOMcreator/Template/template.txt` & `SOMcreator-1.1.8.3/src/SOMcreator/Template/template.txt`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.8.2/src/SOMcreator/classes.py` & `SOMcreator-1.1.8.3/src/SOMcreator/classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -216,15 +216,19 @@
 
     @property
     def parent(self) -> Hirarchy:
         return self._parent
 
     @parent.setter
     def parent(self, parent: Hirarchy) -> None:
+        if self.parent is not None:
+            self.parent._children.remove(self)
         self._parent = parent
+        if parent is not None:
+            self._parent._children.add(self)
         self.changed = True
 
     @property
     def is_parent(self) -> bool:
         if self.children:
             return True
         else:
@@ -802,12 +806,23 @@
     @property
     def is_root(self):
         if self.parent is None:
             return True
         return False
 
     def id_group(self) -> str:
-        own_text = f"{self.object.abbreviation}_xxx"
+        abbrev_list = list()
+
+        def iter_id(element: Aggregation):
+            if element.parent_connection in (constants.AGGREGATION, constants.AGGREGATION + constants.INHERITANCE):
+                abbrev_list.append(element.parent.object.abbreviation)
+            if not element.is_root:
+                iter_id(element.parent)
+
         if self.is_root:
-            return own_text
-        else:
-            return f"{self.parent.id_group()}_{own_text}"
+            return ""
+
+        iter_id(self)
+        return "_xxx_".join(reversed(abbrev_list)) + "_xxx"
+
+    def identity(self) -> str:
+        self.id_group() + "_" + self.object.abbreviation + "_xxx"
```

### Comparing `SOMcreator-1.1.8.2/src/SOMcreator/constants.py` & `SOMcreator-1.1.8.3/src/SOMcreator/constants.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.8.2/src/SOMcreator/external_software/allplan.py` & `SOMcreator-1.1.8.3/src/SOMcreator/external_software/allplan.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.8.2/src/SOMcreator/external_software/card1.py` & `SOMcreator-1.1.8.3/src/SOMcreator/external_software/card1.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.8.2/src/SOMcreator/external_software/desite.py` & `SOMcreator-1.1.8.3/src/SOMcreator/external_software/desite.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.8.2/src/SOMcreator/external_software/excel.py` & `SOMcreator-1.1.8.3/src/SOMcreator/external_software/excel.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.8.2/src/SOMcreator/external_software/revit.py` & `SOMcreator-1.1.8.3/src/SOMcreator/external_software/revit.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.8.2/src/SOMcreator/external_software/vestra.py` & `SOMcreator-1.1.8.3/src/SOMcreator/external_software/vestra.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.8.2/src/SOMcreator/filehandling.py` & `SOMcreator-1.1.8.3/src/SOMcreator/filehandling.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.8.2/src/SOMcreator/quality_check.py` & `SOMcreator-1.1.8.3/src/SOMcreator/quality_check.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.8.2/src/SOMcreator.egg-info/PKG-INFO` & `SOMcreator-1.1.8.3/src/SOMcreator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SOMcreator
-Version: 1.1.8.2
+Version: 1.1.8.3
 Summary: create simple Datastructures for BIM Models
 License: MIT License
         
         Copyright (c) 2022 Christoph Mellüh
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `SOMcreator-1.1.8.2/src/SOMcreator.egg-info/SOURCES.txt` & `SOMcreator-1.1.8.3/src/SOMcreator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

