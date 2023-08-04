# Comparing `tmp/adafri-0.0.72.tar.gz` & `tmp/adafri-0.0.73.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafri-0.0.72.tar", last modified: Tue Aug  1 01:31:39 2023, max compression
+gzip compressed data, was "adafri-0.0.73.tar", last modified: Fri Aug  4 05:19:50 2023, max compression
```

## Comparing `adafri-0.0.72.tar` & `adafri-0.0.73.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-01 01:31:39.349430 adafri-0.0.72/
--rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-08-01 01:31:39.349062 adafri-0.0.72/PKG-INFO
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-01 01:31:39.314703 adafri-0.0.72/adafri/
--rw-r--r--   0 ibrahima   (502) staff       (20)       80 2023-08-01 01:31:32.000000 adafri-0.0.72/adafri/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-01 01:31:39.322450 adafri-0.0.72/adafri/utils/
--rw-r--r--   0 ibrahima   (502) staff       (20)      101 2023-07-21 05:44:28.000000 adafri-0.0.72/adafri/utils/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1252 2023-07-21 06:19:41.000000 adafri-0.0.72/adafri/utils/country.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     2519 2023-07-22 08:32:21.000000 adafri-0.0.72/adafri/utils/phone_number.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1356 2023-07-31 01:55:04.000000 adafri-0.0.72/adafri/utils/response.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    19150 2023-07-31 02:21:52.000000 adafri-0.0.72/adafri/utils/utils.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-01 01:31:39.323683 adafri-0.0.72/adafri/v1/
--rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-16 06:12:23.000000 adafri-0.0.72/adafri/v1/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-01 01:31:39.324649 adafri-0.0.72/adafri/v1/account/
--rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.72/adafri/v1/account/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-01 01:31:39.327269 adafri-0.0.72/adafri/v1/account/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.72/adafri/v1/account/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4514 2023-07-20 05:14:32.000000 adafri-0.0.72/adafri/v1/account/models/account.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3852 2023-07-28 08:14:22.000000 adafri-0.0.72/adafri/v1/account/models/account_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-01 01:31:39.328086 adafri-0.0.72/adafri/v1/auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      249 2023-07-16 05:40:34.000000 adafri-0.0.72/adafri/v1/auth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-01 01:31:39.329692 adafri-0.0.72/adafri/v1/auth/firebase_auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      316 2023-07-25 19:22:35.000000 adafri-0.0.72/adafri/v1/auth/firebase_auth/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     5059 2023-07-26 04:56:41.000000 adafri-0.0.72/adafri/v1/auth/firebase_auth/firebase_auth.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-01 01:31:39.330675 adafri-0.0.72/adafri/v1/auth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.72/adafri/v1/auth/models/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-01 01:31:39.331102 adafri-0.0.72/adafri/v1/auth/oauth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      965 2023-07-28 08:17:28.000000 adafri-0.0.72/adafri/v1/auth/oauth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-01 01:31:39.339090 adafri-0.0.72/adafri/v1/auth/oauth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.72/adafri/v1/auth/oauth/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     6979 2023-07-31 01:04:15.000000 adafri-0.0.72/adafri/v1/auth/oauth/models/client.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     5478 2023-07-28 08:09:48.000000 adafri-0.0.72/adafri/v1/auth/oauth/models/client_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     6529 2023-07-31 01:47:56.000000 adafri-0.0.72/adafri/v1/auth/oauth/models/code.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     2505 2023-07-31 01:28:33.000000 adafri-0.0.72/adafri/v1/auth/oauth/models/code_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    16147 2023-07-31 01:04:27.000000 adafri-0.0.72/adafri/v1/auth/oauth/models/grant.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3653 2023-07-28 08:10:56.000000 adafri-0.0.72/adafri/v1/auth/oauth/models/grant_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     9468 2023-07-31 01:04:45.000000 adafri-0.0.72/adafri/v1/auth/oauth/models/token.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3728 2023-07-28 08:11:40.000000 adafri-0.0.72/adafri/v1/auth/oauth/models/token_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-01 01:31:39.341751 adafri-0.0.72/adafri/v1/auth/oauth/server/
--rw-r--r--   0 ibrahima   (502) staff       (20)      163 2023-07-16 05:39:01.000000 adafri-0.0.72/adafri/v1/auth/oauth/server/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1574 2023-07-20 05:43:11.000000 adafri-0.0.72/adafri/v1/auth/oauth/server/oidc_server.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     2685 2023-07-19 19:45:35.000000 adafri-0.0.72/adafri/v1/auth/oauth/server/server.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-01 01:31:39.343325 adafri-0.0.72/adafri/v1/base/
--rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.72/adafri/v1/base/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-25 06:31:47.000000 adafri-0.0.72/adafri/v1/base/firebase_collection.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-01 01:31:39.344190 adafri-0.0.72/adafri/v1/mailing/
--rw-r--r--   0 ibrahima   (502) staff       (20)    11325 2023-08-01 01:31:24.000000 adafri-0.0.72/adafri/v1/mailing/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-01 01:31:39.344977 adafri-0.0.72/adafri/v1/user/
--rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.72/adafri/v1/user/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-01 01:31:39.348039 adafri-0.0.72/adafri/v1/user/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.72/adafri/v1/user/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    11624 2023-07-26 07:42:34.000000 adafri-0.0.72/adafri/v1/user/models/user.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     7382 2023-07-28 08:13:51.000000 adafri-0.0.72/adafri/v1/user/models/user_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-01 01:31:39.317885 adafri-0.0.72/adafri.egg-info/
--rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-08-01 01:31:39.000000 adafri-0.0.72/adafri.egg-info/PKG-INFO
--rw-r--r--   0 ibrahima   (502) staff       (20)     1329 2023-08-01 01:31:39.000000 adafri-0.0.72/adafri.egg-info/SOURCES.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-08-01 01:31:39.000000 adafri-0.0.72/adafri.egg-info/dependency_links.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-08-01 01:31:39.000000 adafri-0.0.72/adafri.egg-info/top_level.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-08-01 01:31:39.349674 adafri-0.0.72/setup.cfg
--rw-r--r--   0 ibrahima   (502) staff       (20)      684 2023-07-16 01:48:05.000000 adafri-0.0.72/setup.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-04 05:19:50.391644 adafri-0.0.73/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-08-04 05:19:50.377756 adafri-0.0.73/PKG-INFO
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-04 05:19:50.321887 adafri-0.0.73/adafri/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       80 2023-08-04 05:19:44.000000 adafri-0.0.73/adafri/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-04 05:19:50.337229 adafri-0.0.73/adafri/utils/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      101 2023-07-21 05:44:28.000000 adafri-0.0.73/adafri/utils/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1252 2023-07-21 06:19:41.000000 adafri-0.0.73/adafri/utils/country.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     2519 2023-07-22 08:32:21.000000 adafri-0.0.73/adafri/utils/phone_number.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1356 2023-07-31 01:55:04.000000 adafri-0.0.73/adafri/utils/response.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    19150 2023-07-31 02:21:52.000000 adafri-0.0.73/adafri/utils/utils.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-04 05:19:50.338350 adafri-0.0.73/adafri/v1/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-16 06:12:23.000000 adafri-0.0.73/adafri/v1/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-04 05:19:50.340407 adafri-0.0.73/adafri/v1/account/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.73/adafri/v1/account/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-04 05:19:50.347726 adafri-0.0.73/adafri/v1/account/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.73/adafri/v1/account/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4514 2023-07-20 05:14:32.000000 adafri-0.0.73/adafri/v1/account/models/account.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3852 2023-07-28 08:14:22.000000 adafri-0.0.73/adafri/v1/account/models/account_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-04 05:19:50.349487 adafri-0.0.73/adafri/v1/auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      249 2023-07-16 05:40:34.000000 adafri-0.0.73/adafri/v1/auth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-04 05:19:50.353434 adafri-0.0.73/adafri/v1/auth/firebase_auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      316 2023-07-25 19:22:35.000000 adafri-0.0.73/adafri/v1/auth/firebase_auth/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     5059 2023-07-26 04:56:41.000000 adafri-0.0.73/adafri/v1/auth/firebase_auth/firebase_auth.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-04 05:19:50.355788 adafri-0.0.73/adafri/v1/auth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.73/adafri/v1/auth/models/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-04 05:19:50.356358 adafri-0.0.73/adafri/v1/auth/oauth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      965 2023-07-28 08:17:28.000000 adafri-0.0.73/adafri/v1/auth/oauth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-04 05:19:50.368792 adafri-0.0.73/adafri/v1/auth/oauth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.73/adafri/v1/auth/oauth/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     7034 2023-08-04 05:19:39.000000 adafri-0.0.73/adafri/v1/auth/oauth/models/client.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     5478 2023-07-28 08:09:48.000000 adafri-0.0.73/adafri/v1/auth/oauth/models/client_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     6529 2023-07-31 01:47:56.000000 adafri-0.0.73/adafri/v1/auth/oauth/models/code.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     2505 2023-07-31 01:28:33.000000 adafri-0.0.73/adafri/v1/auth/oauth/models/code_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    16147 2023-07-31 01:04:27.000000 adafri-0.0.73/adafri/v1/auth/oauth/models/grant.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3653 2023-07-28 08:10:56.000000 adafri-0.0.73/adafri/v1/auth/oauth/models/grant_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     9468 2023-07-31 01:04:45.000000 adafri-0.0.73/adafri/v1/auth/oauth/models/token.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3728 2023-07-28 08:11:40.000000 adafri-0.0.73/adafri/v1/auth/oauth/models/token_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-04 05:19:50.370865 adafri-0.0.73/adafri/v1/auth/oauth/server/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      163 2023-07-16 05:39:01.000000 adafri-0.0.73/adafri/v1/auth/oauth/server/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1574 2023-07-20 05:43:11.000000 adafri-0.0.73/adafri/v1/auth/oauth/server/oidc_server.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     2685 2023-07-19 19:45:35.000000 adafri-0.0.73/adafri/v1/auth/oauth/server/server.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-04 05:19:50.372583 adafri-0.0.73/adafri/v1/base/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.73/adafri/v1/base/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-25 06:31:47.000000 adafri-0.0.73/adafri/v1/base/firebase_collection.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-04 05:19:50.373185 adafri-0.0.73/adafri/v1/mailing/
+-rw-r--r--   0 ibrahima   (502) staff       (20)    11325 2023-08-01 01:31:24.000000 adafri-0.0.73/adafri/v1/mailing/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-04 05:19:50.374433 adafri-0.0.73/adafri/v1/user/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.73/adafri/v1/user/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-04 05:19:50.376660 adafri-0.0.73/adafri/v1/user/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.73/adafri/v1/user/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    11624 2023-07-26 07:42:34.000000 adafri-0.0.73/adafri/v1/user/models/user.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     7382 2023-07-28 08:13:51.000000 adafri-0.0.73/adafri/v1/user/models/user_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-04 05:19:50.324938 adafri-0.0.73/adafri.egg-info/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-08-04 05:19:50.000000 adafri-0.0.73/adafri.egg-info/PKG-INFO
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1329 2023-08-04 05:19:50.000000 adafri-0.0.73/adafri.egg-info/SOURCES.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-08-04 05:19:50.000000 adafri-0.0.73/adafri.egg-info/dependency_links.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-08-04 05:19:50.000000 adafri-0.0.73/adafri.egg-info/top_level.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-08-04 05:19:50.391973 adafri-0.0.73/setup.cfg
+-rw-r--r--   0 ibrahima   (502) staff       (20)      684 2023-07-16 01:48:05.000000 adafri-0.0.73/setup.py
```

### Comparing `adafri-0.0.72/adafri/utils/country.py` & `adafri-0.0.73/adafri/utils/country.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.72/adafri/utils/phone_number.py` & `adafri-0.0.73/adafri/utils/phone_number.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.72/adafri/utils/response.py` & `adafri-0.0.73/adafri/utils/response.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.72/adafri/utils/utils.py` & `adafri-0.0.73/adafri/utils/utils.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.72/adafri/v1/account/models/account.py` & `adafri-0.0.73/adafri/v1/account/models/account.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.72/adafri/v1/account/models/account_fields.py` & `adafri-0.0.73/adafri/v1/account/models/account_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.72/adafri/v1/auth/firebase_auth/firebase_auth.py` & `adafri-0.0.73/adafri/v1/auth/firebase_auth/firebase_auth.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.72/adafri/v1/auth/oauth/__init__.py` & `adafri-0.0.73/adafri/v1/auth/oauth/__init__.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.72/adafri/v1/auth/oauth/models/client.py` & `adafri-0.0.73/adafri/v1/auth/oauth/models/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     def __init__(self, client=None, default_redirect_uri=None, **kwargs):
         if type(client) is str:
             client = {"client_id": client} 
         (cls_object, keys, data_args) = init_class_kwargs(self, client, STANDARD_FIELDS, ClientFieldProps, CLIENT_COLLECTION, ['id'], **kwargs)
         super().__init__(**data_args);
         for key in keys:
             setattr(self, key, cls_object[key])
-        if bool(self.allowed_redirect_uris) is False:
+        if getattr(self, 'allowed_redirect_uris',None) is None or bool(self.allowed_redirect_uris) is False:
             self.allowed_redirect_uris = self.redirect_uris
         #self.default_redirect_uri = default_redirect_uri
 
 
     @staticmethod
     def generate_model(_key_="default_value"):
         user = {};
```

### Comparing `adafri-0.0.72/adafri/v1/auth/oauth/models/client_fields.py` & `adafri-0.0.73/adafri/v1/auth/oauth/models/client_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.72/adafri/v1/auth/oauth/models/code.py` & `adafri-0.0.73/adafri/v1/auth/oauth/models/code.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.72/adafri/v1/auth/oauth/models/code_fields.py` & `adafri-0.0.73/adafri/v1/auth/oauth/models/code_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.72/adafri/v1/auth/oauth/models/grant.py` & `adafri-0.0.73/adafri/v1/auth/oauth/models/grant.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.72/adafri/v1/auth/oauth/models/grant_fields.py` & `adafri-0.0.73/adafri/v1/auth/oauth/models/grant_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.72/adafri/v1/auth/oauth/models/token.py` & `adafri-0.0.73/adafri/v1/auth/oauth/models/token.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.72/adafri/v1/auth/oauth/models/token_fields.py` & `adafri-0.0.73/adafri/v1/auth/oauth/models/token_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.72/adafri/v1/auth/oauth/server/oidc_server.py` & `adafri-0.0.73/adafri/v1/auth/oauth/server/oidc_server.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.72/adafri/v1/auth/oauth/server/server.py` & `adafri-0.0.73/adafri/v1/auth/oauth/server/server.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.72/adafri/v1/base/firebase_collection.py` & `adafri-0.0.73/adafri/v1/base/firebase_collection.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.72/adafri/v1/mailing/__init__.py` & `adafri-0.0.73/adafri/v1/mailing/__init__.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.72/adafri/v1/user/models/user.py` & `adafri-0.0.73/adafri/v1/user/models/user.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.72/adafri/v1/user/models/user_fields.py` & `adafri-0.0.73/adafri/v1/user/models/user_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.72/adafri.egg-info/SOURCES.txt` & `adafri-0.0.73/adafri.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafri-0.0.72/setup.py` & `adafri-0.0.73/setup.py`

 * *Files identical despite different names*

