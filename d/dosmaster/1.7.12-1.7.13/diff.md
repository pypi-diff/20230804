# Comparing `tmp/dosmaster-1.7.12.tar.gz` & `tmp/dosmaster-1.7.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dosmaster-1.7.12.tar", last modified: Fri Aug  4 00:17:10 2023, max compression
+gzip compressed data, was "dist/dosmaster-1.7.13.tar", last modified: Fri Aug  4 08:49:20 2023, max compression
```

## Comparing `dosmaster-1.7.12.tar` & `dosmaster-1.7.13.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-04 00:17:10.000000 dosmaster-1.7.12/
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       40 2023-08-03 06:58:46.000000 dosmaster-1.7.12/MANIFEST.in
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      640 2023-08-04 00:17:10.000000 dosmaster-1.7.12/PKG-INFO
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     1635 2023-08-04 00:14:12.000000 dosmaster-1.7.12/README.md
-drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-04 00:17:10.000000 dosmaster-1.7.12/dosmaster/
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      130 2023-08-04 00:11:02.000000 dosmaster-1.7.12/dosmaster/__init__.py
-drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-04 00:17:10.000000 dosmaster-1.7.12/dosmaster/base/
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       39 2023-08-04 00:11:02.000000 dosmaster-1.7.12/dosmaster/base/__init__.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     3491 2023-08-04 00:11:02.000000 dosmaster-1.7.12/dosmaster/base/data_generation.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     4463 2023-08-04 00:11:02.000000 dosmaster-1.7.12/dosmaster/base/printer.py
-drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-04 00:17:10.000000 dosmaster-1.7.12/dosmaster/features/
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       55 2023-08-04 00:11:02.000000 dosmaster-1.7.12/dosmaster/features/__init__.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     2512 2023-08-04 00:11:02.000000 dosmaster-1.7.12/dosmaster/features/a_add_atom_dos.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     8658 2023-08-04 00:11:02.000000 dosmaster-1.7.12/dosmaster/features/b_dos_projection.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     1427 2023-08-04 00:13:58.000000 dosmaster-1.7.12/dosmaster/features/c_dos_sum.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     2032 2023-08-04 00:11:02.000000 dosmaster-1.7.12/dosmaster/features/d_avergae_dos.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     1314 2023-08-04 00:11:02.000000 dosmaster-1.7.12/dosmaster/features/e_remove_dos.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     1350 2023-08-04 00:11:02.000000 dosmaster-1.7.12/dosmaster/features/f_change_sign.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     9873 2023-08-04 00:11:02.000000 dosmaster-1.7.12/dosmaster/features/g_graph_editor.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     5897 2023-08-04 00:11:02.000000 dosmaster-1.7.12/dosmaster/features/h_axis_optimization.py
-drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-04 00:17:10.000000 dosmaster-1.7.12/dosmaster/fileparser/
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       61 2023-08-04 00:11:02.000000 dosmaster-1.7.12/dosmaster/fileparser/__init__.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     4062 2023-08-04 00:11:02.000000 dosmaster-1.7.12/dosmaster/fileparser/doscar_split.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      221 2023-08-04 00:11:02.000000 dosmaster-1.7.12/dosmaster/fileparser/procar_parser.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     6742 2023-08-04 00:11:02.000000 dosmaster-1.7.12/dosmaster/fileparser/structure_parser.py
-drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-04 00:17:10.000000 dosmaster-1.7.12/dosmaster/main/
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      154 2023-08-04 00:14:35.000000 dosmaster-1.7.12/dosmaster/main/__init__.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     6372 2023-08-04 00:14:46.000000 dosmaster-1.7.12/dosmaster/main/dosmaster.py
-drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-04 00:17:10.000000 dosmaster-1.7.12/dosmaster/mainplotter/
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       36 2023-08-04 00:11:02.000000 dosmaster-1.7.12/dosmaster/mainplotter/__init__.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     9843 2023-08-04 00:11:02.000000 dosmaster-1.7.12/dosmaster/mainplotter/dosplot.py
-drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-04 00:17:10.000000 dosmaster-1.7.12/dosmaster/subplotter/
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       40 2023-08-04 00:11:02.000000 dosmaster-1.7.12/dosmaster/subplotter/__init__.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     1180 2023-08-04 00:11:02.000000 dosmaster-1.7.12/dosmaster/subplotter/colors.csv
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     3361 2023-08-04 00:11:02.000000 dosmaster-1.7.12/dosmaster/subplotter/colortable.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     6330 2023-08-04 00:11:02.000000 dosmaster-1.7.12/dosmaster/subplotter/dosplot_manager.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     1947 2023-08-04 00:11:02.000000 dosmaster-1.7.12/dosmaster/subplotter/make_color_list.py
-drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-04 00:17:10.000000 dosmaster-1.7.12/dosmaster.egg-info/
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      640 2023-08-04 00:17:10.000000 dosmaster-1.7.12/dosmaster.egg-info/PKG-INFO
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     1115 2023-08-04 00:17:10.000000 dosmaster-1.7.12/dosmaster.egg-info/SOURCES.txt
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)        1 2023-08-04 00:17:10.000000 dosmaster-1.7.12/dosmaster.egg-info/dependency_links.txt
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       60 2023-08-04 00:17:10.000000 dosmaster-1.7.12/dosmaster.egg-info/entry_points.txt
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       59 2023-08-04 00:17:10.000000 dosmaster-1.7.12/dosmaster.egg-info/requires.txt
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       10 2023-08-04 00:17:10.000000 dosmaster-1.7.12/dosmaster.egg-info/top_level.txt
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       38 2023-08-04 00:17:10.000000 dosmaster-1.7.12/setup.cfg
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1328 2023-08-03 07:00:57.000000 dosmaster-1.7.12/setup.py
+drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-04 08:49:20.000000 dosmaster-1.7.13/
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       40 2023-08-03 06:58:46.000000 dosmaster-1.7.13/MANIFEST.in
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      640 2023-08-04 08:49:20.000000 dosmaster-1.7.13/PKG-INFO
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     1635 2023-08-04 08:47:26.000000 dosmaster-1.7.13/README.md
+drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-04 08:49:20.000000 dosmaster-1.7.13/dosmaster/
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      130 2023-08-04 00:11:02.000000 dosmaster-1.7.13/dosmaster/__init__.py
+drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-04 08:49:20.000000 dosmaster-1.7.13/dosmaster/base/
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       39 2023-08-04 00:11:02.000000 dosmaster-1.7.13/dosmaster/base/__init__.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     3491 2023-08-04 00:11:02.000000 dosmaster-1.7.13/dosmaster/base/data_generation.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     4463 2023-08-04 00:11:02.000000 dosmaster-1.7.13/dosmaster/base/printer.py
+drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-04 08:49:20.000000 dosmaster-1.7.13/dosmaster/features/
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       55 2023-08-04 00:11:02.000000 dosmaster-1.7.13/dosmaster/features/__init__.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     2512 2023-08-04 00:11:02.000000 dosmaster-1.7.13/dosmaster/features/a_add_atom_dos.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     8640 2023-08-04 08:46:00.000000 dosmaster-1.7.13/dosmaster/features/b_dos_projection.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     1427 2023-08-04 00:13:58.000000 dosmaster-1.7.13/dosmaster/features/c_dos_sum.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     2032 2023-08-04 00:11:02.000000 dosmaster-1.7.13/dosmaster/features/d_avergae_dos.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     1314 2023-08-04 00:11:02.000000 dosmaster-1.7.13/dosmaster/features/e_remove_dos.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     1350 2023-08-04 00:11:02.000000 dosmaster-1.7.13/dosmaster/features/f_change_sign.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     9873 2023-08-04 00:11:02.000000 dosmaster-1.7.13/dosmaster/features/g_graph_editor.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     5897 2023-08-04 00:11:02.000000 dosmaster-1.7.13/dosmaster/features/h_axis_optimization.py
+drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-04 08:49:20.000000 dosmaster-1.7.13/dosmaster/fileparser/
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       61 2023-08-04 00:11:02.000000 dosmaster-1.7.13/dosmaster/fileparser/__init__.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     4062 2023-08-04 00:11:02.000000 dosmaster-1.7.13/dosmaster/fileparser/doscar_split.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      221 2023-08-04 00:11:02.000000 dosmaster-1.7.13/dosmaster/fileparser/procar_parser.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     6742 2023-08-04 00:11:02.000000 dosmaster-1.7.13/dosmaster/fileparser/structure_parser.py
+drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-04 08:49:20.000000 dosmaster-1.7.13/dosmaster/main/
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      154 2023-08-04 08:47:43.000000 dosmaster-1.7.13/dosmaster/main/__init__.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     6372 2023-08-04 08:47:35.000000 dosmaster-1.7.13/dosmaster/main/dosmaster.py
+drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-04 08:49:20.000000 dosmaster-1.7.13/dosmaster/mainplotter/
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       36 2023-08-04 00:11:02.000000 dosmaster-1.7.13/dosmaster/mainplotter/__init__.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     9843 2023-08-04 00:11:02.000000 dosmaster-1.7.13/dosmaster/mainplotter/dosplot.py
+drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-04 08:49:20.000000 dosmaster-1.7.13/dosmaster/subplotter/
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       40 2023-08-04 00:11:02.000000 dosmaster-1.7.13/dosmaster/subplotter/__init__.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     1180 2023-08-04 00:11:02.000000 dosmaster-1.7.13/dosmaster/subplotter/colors.csv
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     3361 2023-08-04 00:11:02.000000 dosmaster-1.7.13/dosmaster/subplotter/colortable.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     6330 2023-08-04 00:11:02.000000 dosmaster-1.7.13/dosmaster/subplotter/dosplot_manager.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     1947 2023-08-04 00:11:02.000000 dosmaster-1.7.13/dosmaster/subplotter/make_color_list.py
+drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-04 08:49:20.000000 dosmaster-1.7.13/dosmaster.egg-info/
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      640 2023-08-04 08:49:20.000000 dosmaster-1.7.13/dosmaster.egg-info/PKG-INFO
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     1115 2023-08-04 08:49:20.000000 dosmaster-1.7.13/dosmaster.egg-info/SOURCES.txt
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)        1 2023-08-04 08:49:20.000000 dosmaster-1.7.13/dosmaster.egg-info/dependency_links.txt
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       60 2023-08-04 08:49:20.000000 dosmaster-1.7.13/dosmaster.egg-info/entry_points.txt
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       59 2023-08-04 08:49:20.000000 dosmaster-1.7.13/dosmaster.egg-info/requires.txt
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       10 2023-08-04 08:49:20.000000 dosmaster-1.7.13/dosmaster.egg-info/top_level.txt
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       38 2023-08-04 08:49:20.000000 dosmaster-1.7.13/setup.cfg
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1328 2023-08-03 07:00:57.000000 dosmaster-1.7.13/setup.py
```

### Comparing `dosmaster-1.7.12/README.md` & `dosmaster-1.7.13/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 ver.1.2 : 최종 data 파일 저장 기능 추가
 
 ver.1.3 : 버그 수정
 
 ver.1.4.2 : PyPI에 올릴 수 있도록 수정
 
-ver 1.7.12 : Packaging 진행, DOS_Sum, Average_DOS, Axis_Optimization 추가 및 각종 성능 향상 (Old DOS를 남길 때 Label 오류 존재)
+ver 1.7.13 : Packaging 진행, DOS_Sum, Average_DOS, Axis_Optimization 추가 및 각종 성능 향상 (Old DOS를 남길 때 Label 오류 존재)
 
 
 ## Features
 1) Add Atom DOS
 2) DOS Projection
 3) Sum DOS
 4) Average DOS
```

### Comparing `dosmaster-1.7.12/dosmaster/base/data_generation.py` & `dosmaster-1.7.13/dosmaster/base/data_generation.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.7.12/dosmaster/base/printer.py` & `dosmaster-1.7.13/dosmaster/base/printer.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.7.12/dosmaster/features/a_add_atom_dos.py` & `dosmaster-1.7.13/dosmaster/features/a_add_atom_dos.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.7.12/dosmaster/features/b_dos_projection.py` & `dosmaster-1.7.13/dosmaster/features/b_dos_projection.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,26 +19,26 @@
     
 def Projected_DOS(data_dict, graph_config):
     DOS_list = data_dict['DOS_list']
     orbital_list = data_dict['orbital_list']
     Labellist = data_dict['Labellist']
     
     print_current_DOS(DOS_list, Labellist, graph_config)
-    while True:
-        group_select = input('Please select the DOS for projection (enter index) : ')
-    
-        if group_select == 'q':
-            return DOS_list, graph_config
+    group_select = input('Please select the DOS for projection (enter index) : ')
 
-        elif group_select.isdigit() == True:
-            group_select = int(group_select)
-            group_select = group_select - 1
-    
-        else:
-            print('Please enter again.')
+    if group_select == 'q':
+        return DOS_list, graph_config
+
+    elif group_select.isdigit() == True:
+        group_select = int(group_select)
+        group_select = group_select - 1
+
+    else:
+        print('Please enter again.')
+        return DOS_list, graph_config
     
     if isinstance(DOS_list[group_select], list) == False:
         if DOS_list[group_select] == 'Total DOS_all':
             user_orbital_list = Get_User_Projection_Orbital_list(orbital_list)
             issum=input('Should these be combined? (Combine(1)/Keep separate(2[default])): ')
             for u in reversed(user_orbital_list):
                 DOS_list.insert(group_select+1, 'Total DOS_'+u)
```

### Comparing `dosmaster-1.7.12/dosmaster/features/c_dos_sum.py` & `dosmaster-1.7.13/dosmaster/features/c_dos_sum.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.7.12/dosmaster/features/d_avergae_dos.py` & `dosmaster-1.7.13/dosmaster/features/d_avergae_dos.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.7.12/dosmaster/features/e_remove_dos.py` & `dosmaster-1.7.13/dosmaster/features/e_remove_dos.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.7.12/dosmaster/features/f_change_sign.py` & `dosmaster-1.7.13/dosmaster/features/f_change_sign.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.7.12/dosmaster/features/g_graph_editor.py` & `dosmaster-1.7.13/dosmaster/features/g_graph_editor.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.7.12/dosmaster/features/h_axis_optimization.py` & `dosmaster-1.7.13/dosmaster/features/h_axis_optimization.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.7.12/dosmaster/fileparser/doscar_split.py` & `dosmaster-1.7.13/dosmaster/fileparser/doscar_split.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.7.12/dosmaster/fileparser/structure_parser.py` & `dosmaster-1.7.13/dosmaster/fileparser/structure_parser.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.7.12/dosmaster/main/dosmaster.py` & `dosmaster-1.7.13/dosmaster/main/dosmaster.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 #======================================================================================================
-#Script Name : dosmaster Program(ver.1.7.12)
+#Script Name : dosmaster Program(ver.1.7.13)
 #Made by Youngjun Park (yjpark29@postech.ac.kr)
 #Inspired by Jaesun Kim
 #Edit Date : 23/08/02
 #======================================================================================================
 #Description : DOS Plot Smartly in Terminal Environment
 #======================================================================================================
 #: 1) Add Atom DOS
```

### Comparing `dosmaster-1.7.12/dosmaster/mainplotter/dosplot.py` & `dosmaster-1.7.13/dosmaster/mainplotter/dosplot.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.7.12/dosmaster/subplotter/colors.csv` & `dosmaster-1.7.13/dosmaster/subplotter/colors.csv`

 * *Files identical despite different names*

### Comparing `dosmaster-1.7.12/dosmaster/subplotter/colortable.py` & `dosmaster-1.7.13/dosmaster/subplotter/colortable.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.7.12/dosmaster/subplotter/dosplot_manager.py` & `dosmaster-1.7.13/dosmaster/subplotter/dosplot_manager.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.7.12/dosmaster/subplotter/make_color_list.py` & `dosmaster-1.7.13/dosmaster/subplotter/make_color_list.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.7.12/dosmaster.egg-info/SOURCES.txt` & `dosmaster-1.7.13/dosmaster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dosmaster-1.7.12/setup.py` & `dosmaster-1.7.13/setup.py`

 * *Files identical despite different names*

