# Comparing `tmp/ez0th-0.1.5.tar.gz` & `tmp/ez0th-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ez0th-0.1.5.tar", last modified: Sun Jul 16 02:47:17 2023, max compression
+gzip compressed data, was "ez0th-0.1.6.tar", last modified: Fri Aug  4 04:40:46 2023, max compression
```

## Comparing `ez0th-0.1.5.tar` & `ez0th-0.1.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 02:47:17.565664 ez0th-0.1.5/
--rw-rw-rw-   0        0        0    14838 2023-07-16 02:47:17.564651 ez0th-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0    12168 2023-07-16 02:46:44.000000 ez0th-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-16 02:47:17.548444 ez0th-0.1.5/ez0th/
--rw-rw-rw-   0        0        0    10983 2023-07-07 05:41:40.000000 ez0th-0.1.5/ez0th/__init__.py
--rw-rw-rw-   0        0        0     3687 2023-07-16 02:42:45.000000 ez0th-0.1.5/ez0th/test.py
-drwxrwxrwx   0        0        0        0 2023-07-16 02:47:17.563686 ez0th-0.1.5/ez0th.egg-info/
--rw-rw-rw-   0        0        0    14838 2023-07-16 02:47:17.000000 ez0th-0.1.5/ez0th.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      194 2023-07-16 02:47:17.000000 ez0th-0.1.5/ez0th.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 02:47:17.000000 ez0th-0.1.5/ez0th.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-07-16 02:47:17.000000 ez0th-0.1.5/ez0th.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-16 02:47:17.000000 ez0th-0.1.5/ez0th.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-16 02:47:17.565664 ez0th-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      801 2023-07-16 02:47:13.000000 ez0th-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 04:40:46.083548 ez0th-0.1.6/
+-rw-rw-rw-   0        0        0    14838 2023-08-04 04:40:46.083548 ez0th-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0    12168 2023-07-16 02:46:44.000000 ez0th-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-08-04 04:40:46.069288 ez0th-0.1.6/ez0th/
+-rw-rw-rw-   0        0        0    11055 2023-08-04 04:33:25.000000 ez0th-0.1.6/ez0th/__init__.py
+-rw-rw-rw-   0        0        0     3687 2023-08-04 04:34:23.000000 ez0th-0.1.6/ez0th/test.py
+drwxrwxrwx   0        0        0        0 2023-08-04 04:40:46.081545 ez0th-0.1.6/ez0th.egg-info/
+-rw-rw-rw-   0        0        0    14838 2023-08-04 04:40:45.000000 ez0th-0.1.6/ez0th.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      194 2023-08-04 04:40:45.000000 ez0th-0.1.6/ez0th.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 04:40:45.000000 ez0th-0.1.6/ez0th.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-08-04 04:40:45.000000 ez0th-0.1.6/ez0th.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-08-04 04:40:45.000000 ez0th-0.1.6/ez0th.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-04 04:40:46.083548 ez0th-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      801 2023-08-04 04:40:34.000000 ez0th-0.1.6/setup.py
```

### Comparing `ez0th-0.1.5/PKG-INFO` & `ez0th-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ez0th
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python Library for Easy Authentication and Authorization
 Home-page: https://github.co.jp/
 Author: bib_inf
 Author-email: contact.bibinf@gmail.com
 License: CC0 v1.0
 Description: # ez0th - Python Library for Easy Authentication and Authorization
```

### Comparing `ez0th-0.1.5/README.md` & `ez0th-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `ez0th-0.1.5/ez0th/__init__.py` & `ez0th-0.1.6/ez0th/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,15 +181,17 @@
 	# セッショントークンの発行
 	inner_id = db["read"]("id_" + u_id)
 	sess_token = gen_sess_token(inner_id, timeout, db)
 	# メール送信等
 	try:
 		send_func(sess_token)
 		return True
-	except:
+	except Exception as e:
+		# エラーメッセージの表示
+		print(repr(e))
 		return False
 
 # ログアウト [ez0th]
 def logout(
 	sess_token,	# セッショントークン
 	db = "auto"	# データベース
 ):
```

### Comparing `ez0th-0.1.5/ez0th/test.py` & `ez0th-0.1.6/ez0th/test.py`

 * *Files identical despite different names*

### Comparing `ez0th-0.1.5/ez0th.egg-info/PKG-INFO` & `ez0th-0.1.6/ez0th.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ez0th
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python Library for Easy Authentication and Authorization
 Home-page: https://github.co.jp/
 Author: bib_inf
 Author-email: contact.bibinf@gmail.com
 License: CC0 v1.0
 Description: # ez0th - Python Library for Easy Authentication and Authorization
```

### Comparing `ez0th-0.1.5/setup.py` & `ez0th-0.1.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 00000080: 205b 657a 7069 705d 0d0a 7769 7468 2065   [ezpip]..with e
 00000090: 7a70 6970 2e70 6163 6b61 6765 7228 6465  zpip.packager(de
 000000a0: 7665 6c6f 705f 6469 7220 3d20 222e 2f5f  velop_dir = "./_
 000000b0: 6465 7665 6c6f 705f 657a 3074 682f 2229  develop_ez0th/")
 000000c0: 2061 7320 703a 0d0a 0973 6574 7570 280d   as p:...setup(.
 000000d0: 0a09 096e 616d 6520 3d20 2265 7a30 7468  ...name = "ez0th
 000000e0: 222c 0d0a 0909 7665 7273 696f 6e20 3d20  ",....version = 
-000000f0: 2230 2e31 2e35 222c 0d0a 0909 6465 7363  "0.1.5",....desc
+000000f0: 2230 2e31 2e36 222c 0d0a 0909 6465 7363  "0.1.6",....desc
 00000100: 7269 7074 696f 6e20 3d20 2250 7974 686f  ription = "Pytho
 00000110: 6e20 4c69 6272 6172 7920 666f 7220 4561  n Library for Ea
 00000120: 7379 2041 7574 6865 6e74 6963 6174 696f  sy Authenticatio
 00000130: 6e20 616e 6420 4175 7468 6f72 697a 6174  n and Authorizat
 00000140: 696f 6e22 2c0d 0a09 0961 7574 686f 7220  ion",....author 
 00000150: 3d20 2262 6962 5f69 6e66 222c 0d0a 0909  = "bib_inf",....
 00000160: 6175 7468 6f72 5f65 6d61 696c 203d 2022  author_email = "
```

