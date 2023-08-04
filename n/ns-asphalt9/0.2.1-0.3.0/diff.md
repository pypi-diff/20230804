# Comparing `tmp/ns_asphalt9-0.2.1.tar.gz` & `tmp/ns_asphalt9-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ns_asphalt9-0.2.1.tar", last modified: Sun Jul 30 02:13:23 2023, max compression
+gzip compressed data, was "ns_asphalt9-0.3.0.tar", last modified: Fri Aug  4 15:23:37 2023, max compression
```

## Comparing `ns_asphalt9-0.2.1.tar` & `ns_asphalt9-0.3.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:13:23.419531 ns_asphalt9-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-30 02:13:11.000000 ns_asphalt9-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-30 02:13:11.000000 ns_asphalt9-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-30 02:13:23.419531 ns_asphalt9-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-30 02:13:11.000000 ns_asphalt9-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:13:23.415531 ns_asphalt9-0.2.1/ns_asphalt9/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:13:23.415531 ns_asphalt9-0.2.1/ns_asphalt9/core/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-30 02:13:11.000000 ns_asphalt9-0.2.1/ns_asphalt9/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:13:23.415531 ns_asphalt9-0.2.1/ns_asphalt9/core/actions/
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-30 02:13:11.000000 ns_asphalt9-0.2.1/ns_asphalt9/core/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-30 02:13:11.000000 ns_asphalt9-0.2.1/ns_asphalt9/core/actions/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-07-30 02:13:11.000000 ns_asphalt9-0.2.1/ns_asphalt9/core/actions/enter_page.py
--rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-07-30 02:13:11.000000 ns_asphalt9-0.2.1/ns_asphalt9/core/actions/process_race.py
--rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-07-30 02:13:11.000000 ns_asphalt9-0.2.1/ns_asphalt9/core/actions/select_car.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-30 02:13:11.000000 ns_asphalt9-0.2.1/ns_asphalt9/core/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-07-30 02:13:11.000000 ns_asphalt9-0.2.1/ns_asphalt9/core/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-30 02:13:11.000000 ns_asphalt9-0.2.1/ns_asphalt9/core/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-30 02:13:11.000000 ns_asphalt9-0.2.1/ns_asphalt9/core/globals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:13:23.415531 ns_asphalt9-0.2.1/ns_asphalt9/core/gui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 02:13:11.000000 ns_asphalt9-0.2.1/ns_asphalt9/core/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27238 2023-07-30 02:13:11.000000 ns_asphalt9-0.2.1/ns_asphalt9/core/gui/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:13:23.419531 ns_asphalt9-0.2.1/ns_asphalt9/core/gui/images/
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-07-30 02:13:11.000000 ns_asphalt9-0.2.1/ns_asphalt9/core/gui/images/help.png
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-07-30 02:13:11.000000 ns_asphalt9-0.2.1/ns_asphalt9/core/gui/images/home.png
--rw-r--r--   0 runner    (1001) docker     (123)   202347 2023-07-30 02:13:11.000000 ns_asphalt9-0.2.1/ns_asphalt9/core/gui/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-07-30 02:13:11.000000 ns_asphalt9-0.2.1/ns_asphalt9/core/gui/images/settings.png
--rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-07-30 02:13:11.000000 ns_asphalt9-0.2.1/ns_asphalt9/core/ocr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-30 02:13:11.000000 ns_asphalt9-0.2.1/ns_asphalt9/core/page_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    14129 2023-07-30 02:13:11.000000 ns_asphalt9-0.2.1/ns_asphalt9/core/pages.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-30 02:13:11.000000 ns_asphalt9-0.2.1/ns_asphalt9/core/screenshot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-07-30 02:13:11.000000 ns_asphalt9-0.2.1/ns_asphalt9/core/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:13:23.419531 ns_asphalt9-0.2.1/ns_asphalt9/core/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 02:13:11.000000 ns_asphalt9-0.2.1/ns_asphalt9/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-30 02:13:11.000000 ns_asphalt9-0.2.1/ns_asphalt9/core/utils/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-30 02:13:11.000000 ns_asphalt9-0.2.1/ns_asphalt9/core/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-30 02:13:11.000000 ns_asphalt9-0.2.1/ns_asphalt9/core/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)    41726 2023-07-30 02:13:11.000000 ns_asphalt9-0.2.1/ns_asphalt9/core/utils/track_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    25358 2023-07-30 02:13:11.000000 ns_asphalt9-0.2.1/ns_asphalt9/core/utils/track_navi_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-07-30 02:13:11.000000 ns_asphalt9-0.2.1/ns_asphalt9/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:13:23.415531 ns_asphalt9-0.2.1/ns_asphalt9.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-30 02:13:23.000000 ns_asphalt9-0.2.1/ns_asphalt9.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-30 02:13:23.000000 ns_asphalt9-0.2.1/ns_asphalt9.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 02:13:23.000000 ns_asphalt9-0.2.1/ns_asphalt9.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-30 02:13:23.000000 ns_asphalt9-0.2.1/ns_asphalt9.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 02:13:23.000000 ns_asphalt9-0.2.1/ns_asphalt9.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-30 02:13:23.000000 ns_asphalt9-0.2.1/ns_asphalt9.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-30 02:13:23.000000 ns_asphalt9-0.2.1/ns_asphalt9.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-30 02:13:23.419531 ns_asphalt9-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-30 02:13:11.000000 ns_asphalt9-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:13:23.419531 ns_asphalt9-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-30 02:13:11.000000 ns_asphalt9-0.2.1/tests/test_pages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:23:37.733069 ns_asphalt9-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-04 15:23:21.000000 ns_asphalt9-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-08-04 15:23:21.000000 ns_asphalt9-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-04 15:23:37.733069 ns_asphalt9-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-08-04 15:23:21.000000 ns_asphalt9-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:23:37.725069 ns_asphalt9-0.3.0/ns_asphalt9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:23:37.729069 ns_asphalt9-0.3.0/ns_asphalt9/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-04 15:23:21.000000 ns_asphalt9-0.3.0/ns_asphalt9/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:23:37.729069 ns_asphalt9-0.3.0/ns_asphalt9/core/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-08-04 15:23:21.000000 ns_asphalt9-0.3.0/ns_asphalt9/core/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-08-04 15:23:21.000000 ns_asphalt9-0.3.0/ns_asphalt9/core/actions/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-08-04 15:23:21.000000 ns_asphalt9-0.3.0/ns_asphalt9/core/actions/enter_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-08-04 15:23:21.000000 ns_asphalt9-0.3.0/ns_asphalt9/core/actions/process_race.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-08-04 15:23:21.000000 ns_asphalt9-0.3.0/ns_asphalt9/core/actions/select_car.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-08-04 15:23:21.000000 ns_asphalt9-0.3.0/ns_asphalt9/core/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-08-04 15:23:21.000000 ns_asphalt9-0.3.0/ns_asphalt9/core/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-08-04 15:23:21.000000 ns_asphalt9-0.3.0/ns_asphalt9/core/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-08-04 15:23:21.000000 ns_asphalt9-0.3.0/ns_asphalt9/core/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:23:37.729069 ns_asphalt9-0.3.0/ns_asphalt9/core/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 15:23:21.000000 ns_asphalt9-0.3.0/ns_asphalt9/core/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17716 2023-08-04 15:23:21.000000 ns_asphalt9-0.3.0/ns_asphalt9/core/gui/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:23:37.729069 ns_asphalt9-0.3.0/ns_asphalt9/core/gui/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-08-04 15:23:21.000000 ns_asphalt9-0.3.0/ns_asphalt9/core/gui/images/help.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-08-04 15:23:21.000000 ns_asphalt9-0.3.0/ns_asphalt9/core/gui/images/home.png
+-rw-r--r--   0 runner    (1001) docker     (123)   202347 2023-08-04 15:23:21.000000 ns_asphalt9-0.3.0/ns_asphalt9/core/gui/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-08-04 15:23:21.000000 ns_asphalt9-0.3.0/ns_asphalt9/core/gui/images/settings.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-08-04 15:23:21.000000 ns_asphalt9-0.3.0/ns_asphalt9/core/ocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-08-04 15:23:21.000000 ns_asphalt9-0.3.0/ns_asphalt9/core/page_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14129 2023-08-04 15:23:21.000000 ns_asphalt9-0.3.0/ns_asphalt9/core/pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-08-04 15:23:21.000000 ns_asphalt9-0.3.0/ns_asphalt9/core/screenshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-08-04 15:23:21.000000 ns_asphalt9-0.3.0/ns_asphalt9/core/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:23:37.733069 ns_asphalt9-0.3.0/ns_asphalt9/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 15:23:21.000000 ns_asphalt9-0.3.0/ns_asphalt9/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-08-04 15:23:21.000000 ns_asphalt9-0.3.0/ns_asphalt9/core/utils/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-08-04 15:23:21.000000 ns_asphalt9-0.3.0/ns_asphalt9/core/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-08-04 15:23:21.000000 ns_asphalt9-0.3.0/ns_asphalt9/core/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41726 2023-08-04 15:23:21.000000 ns_asphalt9-0.3.0/ns_asphalt9/core/utils/track_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25358 2023-08-04 15:23:21.000000 ns_asphalt9-0.3.0/ns_asphalt9/core/utils/track_navi_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-08-04 15:23:21.000000 ns_asphalt9-0.3.0/ns_asphalt9/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:23:37.725069 ns_asphalt9-0.3.0/ns_asphalt9.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-04 15:23:37.000000 ns_asphalt9-0.3.0/ns_asphalt9.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-08-04 15:23:37.000000 ns_asphalt9-0.3.0/ns_asphalt9.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 15:23:37.000000 ns_asphalt9-0.3.0/ns_asphalt9.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-04 15:23:37.000000 ns_asphalt9-0.3.0/ns_asphalt9.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 15:23:37.000000 ns_asphalt9-0.3.0/ns_asphalt9.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-04 15:23:37.000000 ns_asphalt9-0.3.0/ns_asphalt9.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-04 15:23:37.000000 ns_asphalt9-0.3.0/ns_asphalt9.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-08-04 15:23:37.733069 ns_asphalt9-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-08-04 15:23:21.000000 ns_asphalt9-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:23:37.733069 ns_asphalt9-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-08-04 15:23:21.000000 ns_asphalt9-0.3.0/tests/test_pages.py
```

### Comparing `ns_asphalt9-0.2.1/LICENSE` & `ns_asphalt9-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.2.1/PKG-INFO` & `ns_asphalt9-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ns_asphalt9
-Version: 0.2.1
+Version: 0.3.0
 Summary: Asphalt 9 daily task handling tool based on NXBT and V4L2.
 Home-page: https://pypi.python.org/pypi/ns_asphalt9
 Author: codehai
 Author-email: wmpksb@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Code, https://github.com/codehai/ns_asphalt9
 Project-URL: Issue tracker, https://github.com/codehai/ns_asphalt9/issues
```

### Comparing `ns_asphalt9-0.2.1/README.md` & `ns_asphalt9-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.2.1/ns_asphalt9/core/actions/common.py` & `ns_asphalt9-0.3.0/ns_asphalt9/core/actions/common.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,23 +10,18 @@
     pro.press_buttons([Buttons.A], down=0.5)
 
 
 def restart():
     """重启游戏"""
     # 回到主页
     pro.press_button(Buttons.HOME, 3)
-    # 切到第二个游戏
-    pro.press_button(Buttons.DPAD_RIGHT, 1)
-    # 按一下确认打开，再按一下确认关闭
-    pro.press_group([Buttons.A] * 2, 1)
-    pro.press_button(Buttons.B, 1)
-    # 回到A9
-    pro.press_button(Buttons.DPAD_LEFT, 1)
-    # 进入游戏
-    pro.press_group([Buttons.A] * 2, 2)
+    # 关闭
+    pro.press_button(Buttons.X, 1)
+    # 按一下确认关闭，再打开
+    pro.press_group([Buttons.A] * 3, 2)
 
 
 def demoted():
     """降级"""
     globals.DIVISION = ""
     pro.press_button(Buttons.B, 3)
```

### Comparing `ns_asphalt9-0.2.1/ns_asphalt9/core/actions/enter_page.py` & `ns_asphalt9-0.3.0/ns_asphalt9/core/actions/enter_page.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.2.1/ns_asphalt9/core/actions/process_race.py` & `ns_asphalt9-0.3.0/ns_asphalt9/core/actions/process_race.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.2.1/ns_asphalt9/core/actions/select_car.py` & `ns_asphalt9-0.3.0/ns_asphalt9/core/actions/select_car.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.2.1/ns_asphalt9/core/cache.py` & `ns_asphalt9-0.3.0/ns_asphalt9/core/cache.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.2.1/ns_asphalt9/core/consts.py` & `ns_asphalt9-0.3.0/ns_asphalt9/core/consts.py`

 * *Files 4% similar despite different names*

```diff
@@ -111,14 +111,15 @@
 mp1_zh = "多人一"
 mp2_zh = "多人二"
 mp3_zh = "多人三"
 mp_zh = "多人"
 free_pack_zh = "免费抽卡"
 prix_pack_zh = "大奖赛抽卡"
 legendary_hunt_zh = "传奇寻车"
+restart = "重启"
 
 
 class Mode:
     car_hunt = "CAR HUNT"
     legendary_hunt = "LEGENDARY HUNT"
     world_series = "WORLD SERIES"
     limited_series = "LIMITED SERIES"
```

### Comparing `ns_asphalt9-0.2.1/ns_asphalt9/core/controller.py` & `ns_asphalt9-0.3.0/ns_asphalt9/core/controller.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.2.1/ns_asphalt9/core/globals.py` & `ns_asphalt9-0.3.0/ns_asphalt9/core/globals.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.2.1/ns_asphalt9/core/gui/images/help.png` & `ns_asphalt9-0.3.0/ns_asphalt9/core/gui/images/help.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.2.1/ns_asphalt9/core/gui/images/home.png` & `ns_asphalt9-0.3.0/ns_asphalt9/core/gui/images/home.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.2.1/ns_asphalt9/core/gui/images/logo.png` & `ns_asphalt9-0.3.0/ns_asphalt9/core/gui/images/logo.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.2.1/ns_asphalt9/core/gui/images/settings.png` & `ns_asphalt9-0.3.0/ns_asphalt9/core/gui/images/settings.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.2.1/ns_asphalt9/core/ocr.py` & `ns_asphalt9-0.3.0/ns_asphalt9/core/ocr.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,12 +168,13 @@
             img = img.filter(filter)
         if convert:
             img = img.convert(convert)
         text: str = pytesseract.image_to_string(img, lang="eng", config=config)
         img.close()
         if replace:
             text = text.replace("\n", " ")
+        logger.info(f"Get text from page, text = text")
         return text
 
 
 if __name__ == "__main__":
     OCR.get_text()
```

### Comparing `ns_asphalt9-0.2.1/ns_asphalt9/core/page_factory.py` & `ns_asphalt9-0.3.0/ns_asphalt9/core/page_factory.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.2.1/ns_asphalt9/core/pages.py` & `ns_asphalt9-0.3.0/ns_asphalt9/core/pages.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.2.1/ns_asphalt9/core/tasks.py` & `ns_asphalt9-0.3.0/ns_asphalt9/core/tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,13 +77,15 @@
             actions.enter_carhunt(page=page)
         if task == consts.free_pack_zh:
             actions.free_pack()
         if task == consts.prix_pack_zh:
             actions.prix_pack()
         if task == consts.legendary_hunt_zh:
             actions.enter_legend_carhunt()
+        if task == consts.restart:
+            actions.restart()
 
     @classmethod
     def set_done(cls) -> None:
         if cls.status == consts.TaskStatus.start:
             cls.status = consts.TaskStatus.done
             cls.current_task = ""
```

### Comparing `ns_asphalt9-0.2.1/ns_asphalt9/core/utils/decorator.py` & `ns_asphalt9-0.3.0/ns_asphalt9/core/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.2.1/ns_asphalt9/core/utils/log.py` & `ns_asphalt9-0.3.0/ns_asphalt9/core/utils/log.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.2.1/ns_asphalt9/core/utils/timer.py` & `ns_asphalt9-0.3.0/ns_asphalt9/core/utils/timer.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.2.1/ns_asphalt9/core/utils/track_data.py` & `ns_asphalt9-0.3.0/ns_asphalt9/core/utils/track_data.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.2.1/ns_asphalt9/core/utils/track_navi_data.py` & `ns_asphalt9-0.3.0/ns_asphalt9/core/utils/track_navi_data.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.2.1/ns_asphalt9/main.py` & `ns_asphalt9-0.3.0/ns_asphalt9/main.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.2.1/ns_asphalt9.egg-info/PKG-INFO` & `ns_asphalt9-0.3.0/ns_asphalt9.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ns-asphalt9
-Version: 0.2.1
+Version: 0.3.0
 Summary: Asphalt 9 daily task handling tool based on NXBT and V4L2.
 Home-page: https://pypi.python.org/pypi/ns_asphalt9
 Author: codehai
 Author-email: wmpksb@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Code, https://github.com/codehai/ns_asphalt9
 Project-URL: Issue tracker, https://github.com/codehai/ns_asphalt9/issues
```

### Comparing `ns_asphalt9-0.2.1/ns_asphalt9.egg-info/SOURCES.txt` & `ns_asphalt9-0.3.0/ns_asphalt9.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.2.1/setup.cfg` & `ns_asphalt9-0.3.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nxbt
-version = 0.2.1
+version = 0.3.0
 author = codehai
 author-email = wmpksb@gmail.com
 project_urls = 
 	Code = https://github.com/codehai/ns_asphalt9
 	Issue tracker = https://github.com/codehai/ns_asphalt9/issues
 license = GNU General Public License v3 (GPLv3)
 license-file = LICENSE
```

### Comparing `ns_asphalt9-0.2.1/tests/test_pages.py` & `ns_asphalt9-0.3.0/tests/test_pages.py`

 * *Files identical despite different names*

