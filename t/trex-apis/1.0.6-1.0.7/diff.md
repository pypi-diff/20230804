# Comparing `tmp/trex-apis-1.0.6.tar.gz` & `tmp/trex-apis-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trex-apis-1.0.6.tar", last modified: Tue Aug  1 02:33:34 2023, max compression
+gzip compressed data, was "trex-apis-1.0.7.tar", last modified: Fri Aug  4 06:32:54 2023, max compression
```

## Comparing `trex-apis-1.0.6.tar` & `trex-apis-1.0.7.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-01 02:33:34.858237 trex-apis-1.0.6/
--rw-r--r--   0 jacklok    (501) staff       (20)      447 2023-08-01 02:33:34.858375 trex-apis-1.0.6/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)       25 2021-06-30 02:28:26.000000 trex-apis-1.0.6/README.md
--rw-r--r--   0 jacklok    (501) staff       (20)       75 2023-08-01 02:33:34.858830 trex-apis-1.0.6/setup.cfg
--rw-r--r--   0 jacklok    (501) staff       (20)      713 2023-08-01 02:30:49.000000 trex-apis-1.0.6/setup.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-01 02:33:34.819427 trex-apis-1.0.6/trex_apis.egg-info/
--rw-r--r--   0 jacklok    (501) staff       (20)      447 2023-08-01 02:33:34.000000 trex-apis-1.0.6/trex_apis.egg-info/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)     1371 2023-08-01 02:33:34.000000 trex-apis-1.0.6/trex_apis.egg-info/SOURCES.txt
--rw-r--r--   0 jacklok    (501) staff       (20)        1 2023-08-01 02:33:34.000000 trex-apis-1.0.6/trex_apis.egg-info/dependency_links.txt
--rw-r--r--   0 jacklok    (501) staff       (20)       23 2023-08-01 02:33:34.000000 trex-apis-1.0.6/trex_apis.egg-info/requires.txt
--rw-r--r--   0 jacklok    (501) staff       (20)        8 2023-08-01 02:33:34.000000 trex-apis-1.0.6/trex_apis.egg-info/top_level.txt
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-01 02:33:34.819954 trex-apis-1.0.6/trexapi/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-06-30 02:30:07.000000 trex-apis-1.0.6/trexapi/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)      937 2023-07-20 09:41:39.000000 trex-apis-1.0.6/trexapi/conf.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-01 02:33:34.845328 trex-apis-1.0.6/trexapi/controllers/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-06-30 02:45:28.000000 trex-apis-1.0.6/trexapi/controllers/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     4523 2023-05-23 05:00:09.000000 trex-apis-1.0.6/trexapi/controllers/api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     3850 2023-05-25 08:10:20.000000 trex-apis-1.0.6/trexapi/controllers/app_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    35947 2023-05-18 03:00:00.000000 trex-apis-1.0.6/trexapi/controllers/customer_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     6945 2023-04-13 05:36:42.000000 trex-apis-1.0.6/trexapi/controllers/customer_membership_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     4750 2023-01-30 07:03:11.000000 trex-apis-1.0.6/trexapi/controllers/customer_reward_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    13204 2023-05-15 02:06:38.000000 trex-apis-1.0.6/trexapi/controllers/loyalty_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    13485 2023-07-12 07:15:15.000000 trex-apis-1.0.6/trexapi/controllers/lucky_draw_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    15269 2023-07-10 09:47:14.000000 trex-apis-1.0.6/trexapi/controllers/merchant_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    11170 2023-05-16 03:00:59.000000 trex-apis-1.0.6/trexapi/controllers/outlet_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1430 2022-09-26 04:18:01.000000 trex-apis-1.0.6/trexapi/controllers/payment_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    24944 2023-05-23 09:32:47.000000 trex-apis-1.0.6/trexapi/controllers/pos_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    27329 2023-04-18 07:01:48.000000 trex-apis-1.0.6/trexapi/controllers/reward_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    12777 2023-07-25 03:49:49.000000 trex-apis-1.0.6/trexapi/controllers/sales_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)      998 2023-04-18 06:08:18.000000 trex-apis-1.0.6/trexapi/controllers/transaction_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    51442 2023-07-31 15:36:43.000000 trex-apis-1.0.6/trexapi/controllers/user_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2980 2023-01-30 02:56:35.000000 trex-apis-1.0.6/trexapi/controllers/user_reward_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    16314 2023-07-05 09:44:39.000000 trex-apis-1.0.6/trexapi/controllers/voucher_api_routes.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-01 02:33:34.847640 trex-apis-1.0.6/trexapi/decorators/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-01 08:42:13.000000 trex-apis-1.0.6/trexapi/decorators/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     5778 2023-06-30 15:57:30.000000 trex-apis-1.0.6/trexapi/decorators/api_decorators.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-01 02:33:34.852726 trex-apis-1.0.6/trexapi/forms/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-12 06:42:53.000000 trex-apis-1.0.6/trexapi/forms/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     7419 2023-02-08 10:14:32.000000 trex-apis-1.0.6/trexapi/forms/customer_api_forms.py
--rw-r--r--   0 jacklok    (501) staff       (20)     7285 2023-04-18 02:42:03.000000 trex-apis-1.0.6/trexapi/forms/reward_api_forms.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1547 2023-04-18 02:41:54.000000 trex-apis-1.0.6/trexapi/forms/sales_api_forms.py
--rw-r--r--   0 jacklok    (501) staff       (20)     3922 2023-05-29 03:02:06.000000 trex-apis-1.0.6/trexapi/forms/user_api_forms.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-01 02:33:34.854114 trex-apis-1.0.6/trexapi/libs/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-05 10:17:19.000000 trex-apis-1.0.6/trexapi/libs/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1143 2021-07-05 10:57:23.000000 trex-apis-1.0.6/trexapi/libs/flask_auth_wrapper.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-01 02:33:34.856203 trex-apis-1.0.6/trexapi/utils/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-08 10:01:06.000000 trex-apis-1.0.6/trexapi/utils/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1347 2022-12-20 01:23:01.000000 trex-apis-1.0.6/trexapi/utils/api_helpers.py
--rw-r--r--   0 jacklok    (501) staff       (20)    78420 2023-06-30 14:45:12.000000 trex-apis-1.0.6/trexapi/utils/reward_transaction_helper.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-04 06:32:54.427461 trex-apis-1.0.7/
+-rw-r--r--   0 jacklok    (501) staff       (20)      447 2023-08-04 06:32:54.427730 trex-apis-1.0.7/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)       25 2021-06-30 02:28:26.000000 trex-apis-1.0.7/README.md
+-rw-r--r--   0 jacklok    (501) staff       (20)       75 2023-08-04 06:32:54.428414 trex-apis-1.0.7/setup.cfg
+-rw-r--r--   0 jacklok    (501) staff       (20)      713 2023-08-04 06:32:32.000000 trex-apis-1.0.7/setup.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-04 06:32:54.386372 trex-apis-1.0.7/trex_apis.egg-info/
+-rw-r--r--   0 jacklok    (501) staff       (20)      447 2023-08-04 06:32:54.000000 trex-apis-1.0.7/trex_apis.egg-info/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)     1371 2023-08-04 06:32:54.000000 trex-apis-1.0.7/trex_apis.egg-info/SOURCES.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)        1 2023-08-04 06:32:54.000000 trex-apis-1.0.7/trex_apis.egg-info/dependency_links.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)       23 2023-08-04 06:32:54.000000 trex-apis-1.0.7/trex_apis.egg-info/requires.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)        8 2023-08-04 06:32:54.000000 trex-apis-1.0.7/trex_apis.egg-info/top_level.txt
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-04 06:32:54.387356 trex-apis-1.0.7/trexapi/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-06-30 02:30:07.000000 trex-apis-1.0.7/trexapi/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      937 2023-07-20 09:41:39.000000 trex-apis-1.0.7/trexapi/conf.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-04 06:32:54.412939 trex-apis-1.0.7/trexapi/controllers/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-06-30 02:45:28.000000 trex-apis-1.0.7/trexapi/controllers/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     4523 2023-05-23 05:00:09.000000 trex-apis-1.0.7/trexapi/controllers/api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     3850 2023-05-25 08:10:20.000000 trex-apis-1.0.7/trexapi/controllers/app_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    35947 2023-05-18 03:00:00.000000 trex-apis-1.0.7/trexapi/controllers/customer_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     6945 2023-04-13 05:36:42.000000 trex-apis-1.0.7/trexapi/controllers/customer_membership_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     4750 2023-01-30 07:03:11.000000 trex-apis-1.0.7/trexapi/controllers/customer_reward_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    13204 2023-05-15 02:06:38.000000 trex-apis-1.0.7/trexapi/controllers/loyalty_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    13485 2023-07-12 07:15:15.000000 trex-apis-1.0.7/trexapi/controllers/lucky_draw_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    15269 2023-07-10 09:47:14.000000 trex-apis-1.0.7/trexapi/controllers/merchant_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    11170 2023-05-16 03:00:59.000000 trex-apis-1.0.7/trexapi/controllers/outlet_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1430 2022-09-26 04:18:01.000000 trex-apis-1.0.7/trexapi/controllers/payment_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    24944 2023-05-23 09:32:47.000000 trex-apis-1.0.7/trexapi/controllers/pos_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    27329 2023-04-18 07:01:48.000000 trex-apis-1.0.7/trexapi/controllers/reward_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    12777 2023-07-25 03:49:49.000000 trex-apis-1.0.7/trexapi/controllers/sales_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      998 2023-04-18 06:08:18.000000 trex-apis-1.0.7/trexapi/controllers/transaction_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    52259 2023-08-04 05:57:17.000000 trex-apis-1.0.7/trexapi/controllers/user_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2980 2023-01-30 02:56:35.000000 trex-apis-1.0.7/trexapi/controllers/user_reward_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    16314 2023-07-05 09:44:39.000000 trex-apis-1.0.7/trexapi/controllers/voucher_api_routes.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-04 06:32:54.414640 trex-apis-1.0.7/trexapi/decorators/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-01 08:42:13.000000 trex-apis-1.0.7/trexapi/decorators/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     5778 2023-06-30 15:57:30.000000 trex-apis-1.0.7/trexapi/decorators/api_decorators.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-04 06:32:54.420851 trex-apis-1.0.7/trexapi/forms/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-12 06:42:53.000000 trex-apis-1.0.7/trexapi/forms/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     7419 2023-02-08 10:14:32.000000 trex-apis-1.0.7/trexapi/forms/customer_api_forms.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     7285 2023-04-18 02:42:03.000000 trex-apis-1.0.7/trexapi/forms/reward_api_forms.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1547 2023-04-18 02:41:54.000000 trex-apis-1.0.7/trexapi/forms/sales_api_forms.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     3922 2023-05-29 03:02:06.000000 trex-apis-1.0.7/trexapi/forms/user_api_forms.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-04 06:32:54.422275 trex-apis-1.0.7/trexapi/libs/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-05 10:17:19.000000 trex-apis-1.0.7/trexapi/libs/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1143 2021-07-05 10:57:23.000000 trex-apis-1.0.7/trexapi/libs/flask_auth_wrapper.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-04 06:32:54.425588 trex-apis-1.0.7/trexapi/utils/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-08 10:01:06.000000 trex-apis-1.0.7/trexapi/utils/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1347 2022-12-20 01:23:01.000000 trex-apis-1.0.7/trexapi/utils/api_helpers.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    78420 2023-06-30 14:45:12.000000 trex-apis-1.0.7/trexapi/utils/reward_transaction_helper.py
```

### Comparing `trex-apis-1.0.6/setup.py` & `trex-apis-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
      name='trex-apis',  
-     version='1.0.6',
+     version='1.0.7',
      author="Jack Lok",
      author_email="sglok77@gmail.com",
      description="TRex APIs package",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://bitbucket.org/lokjac/trex-apis",
      packages=setuptools.find_packages(),
```

### Comparing `trex-apis-1.0.6/trex_apis.egg-info/SOURCES.txt` & `trex-apis-1.0.7/trex_apis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.6/trexapi/conf.py` & `trex-apis-1.0.7/trexapi/conf.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.6/trexapi/controllers/api_routes.py` & `trex-apis-1.0.7/trexapi/controllers/api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.6/trexapi/controllers/app_api_routes.py` & `trex-apis-1.0.7/trexapi/controllers/app_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.6/trexapi/controllers/customer_api_routes.py` & `trex-apis-1.0.7/trexapi/controllers/customer_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.6/trexapi/controllers/customer_membership_api_routes.py` & `trex-apis-1.0.7/trexapi/controllers/customer_membership_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.6/trexapi/controllers/customer_reward_api_routes.py` & `trex-apis-1.0.7/trexapi/controllers/customer_reward_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.6/trexapi/controllers/loyalty_api_routes.py` & `trex-apis-1.0.7/trexapi/controllers/loyalty_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.6/trexapi/controllers/lucky_draw_api_routes.py` & `trex-apis-1.0.7/trexapi/controllers/lucky_draw_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.6/trexapi/controllers/merchant_api_routes.py` & `trex-apis-1.0.7/trexapi/controllers/merchant_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.6/trexapi/controllers/outlet_api_routes.py` & `trex-apis-1.0.7/trexapi/controllers/outlet_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.6/trexapi/controllers/payment_api_routes.py` & `trex-apis-1.0.7/trexapi/controllers/payment_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.6/trexapi/controllers/pos_api_routes.py` & `trex-apis-1.0.7/trexapi/controllers/pos_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.6/trexapi/controllers/reward_api_routes.py` & `trex-apis-1.0.7/trexapi/controllers/reward_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.6/trexapi/controllers/sales_api_routes.py` & `trex-apis-1.0.7/trexapi/controllers/sales_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.6/trexapi/controllers/transaction_api_routes.py` & `trex-apis-1.0.7/trexapi/controllers/transaction_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.6/trexapi/controllers/user_api_routes.py` & `trex-apis-1.0.7/trexapi/controllers/user_api_routes.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,16 +152,16 @@
                 
                 #send_email_verification_code_email(registered_user_acct)
                 (expiry_datetime, token)    = generate_user_auth_token(registered_user_acct.user_id, registered_user_acct.reference_code)
                 
                 return create_rest_message(status_code=StatusCode.OK, 
                                            auth_token                           = token,
                                            reference_code                       = registered_user_acct.reference_code,
-                                           email_vc_expiry_datetime             = registered_user_acct.email_vc_expiry_datetime.strftime('%d-%m-%Y %H:%M:%S'),
-                                           mobile_phone_vc_expiry_datetime      = registered_user_acct.mobile_phone_vc_expiry_datetime.strftime('%d-%m-%Y %H:%M:%S'),
+                                           email_vc_expiry_datetime             = registered_user_acct.email_vc_expiry_datetime.strftime('%d-%m-%Y %H:%M:%S') if registered_user_acct.email_vc_expiry_datetime is not None else None,
+                                           mobile_phone_vc_expiry_datetime      = registered_user_acct.mobile_phone_vc_expiry_datetime.strftime('%d-%m-%Y %H:%M:%S') if registered_user_acct.mobile_phone_vc_expiry_datetime is not None else None,
                                            )
             else:
                 return create_rest_message(status_code=StatusCode.BAD_REQUEST)
             
         else:
             logger.warn('user_register: user registration input is invalid')
             error_message = register_user_form.create_rest_return_error_message()
@@ -241,14 +241,17 @@
 @user_api_bp.route('/auth', methods=['POST'])
 def auth_user():
     
     user_data_in_json   = request.get_json()
     email               = user_data_in_json.get('email')
     password            = user_data_in_json.get('password')
     
+    logger.debug('email=%s', email)
+    logger.debug('password=%s', password)
+    
     if is_not_empty(email) and is_not_empty(password):
         db_client = create_db_client(caller_info="auth_user")
         user_acct = None
         with db_client.context():
             user_acct = User.get_by_email(email)
         
         if user_acct:
@@ -484,17 +487,17 @@
         #vg_generated_datetime = user_acct.vg_generated_datetime.strftime(user_acct.vg_generated_datetime, '%d/%m/%Y, %H:%M:%S')
         email_vc_expiry_datetime = str(user_acct.email_vc_expiry_datetime)
     else:
         email_verified_datetime = str(user_acct.email_verified_datetime)
             
     if is_mobile_phone_verified == False and is_not_empty(user_acct.mobile_phone_vc_expiry_datetime):
         #vg_generated_datetime = user_acct.vg_generated_datetime.strftime(user_acct.vg_generated_datetime, '%d/%m/%Y, %H:%M:%S')
-        mobile_phone_vc_expiry_datetime = str(user_acct.mobile_phone_vc_expiry_datetime)
+        mobile_phone_vc_expiry_datetime = user_acct.mobile_phone_vc_expiry_datetime.strftime('%d-%m-%Y %H:%M:%S')
     else:
-        mobile_phone_verified_datetime = str(user_acct.mobile_phone_verified_datetime)
+        mobile_phone_verified_datetime = user_acct.mobile_phone_verified_datetime.strftime('%d-%m-%Y %H:%M:%S')
         
     birth_date_str = None
     if is_not_empty(user_acct.birth_date):
         birth_date_str = user_acct.birth_date.strftime('%d-%m-%Y')
          
     
     user_details = {
@@ -620,15 +623,30 @@
             }
     
     return jsonify(result)
     
 @user_api_bp.route('/check-auth-token', methods=['POST'])
 @user_auth_token_required
 def check_auth_token():
-    return create_rest_message(status_code=StatusCode.OK,)
+    
+    reference_code = request.headers.get('x-reference-code')
+    user_acct = None
+    db_client = create_db_client(caller_info="check_auth_token")
+    
+    with db_client.context():
+        user_acct = User.get_by_reference_code(reference_code)
+        user_auth_token     = request.headers.get('x-auth-token')
+        
+        response_data = {
+                        'auth_token'              : user_auth_token,
+                        }
+        
+        response_data.update(user_details_dict(user_acct))
+    
+    return create_rest_message(status_code=StatusCode.OK, **response_data)
 
 
     
 @user_api_bp.route('/<reference_code>', methods=['GET'])
 @user_auth_token_required
 def read_user_acct(reference_code):
```

### Comparing `trex-apis-1.0.6/trexapi/controllers/user_reward_api_routes.py` & `trex-apis-1.0.7/trexapi/controllers/user_reward_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.6/trexapi/controllers/voucher_api_routes.py` & `trex-apis-1.0.7/trexapi/controllers/voucher_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.6/trexapi/decorators/api_decorators.py` & `trex-apis-1.0.7/trexapi/decorators/api_decorators.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.6/trexapi/forms/customer_api_forms.py` & `trex-apis-1.0.7/trexapi/forms/customer_api_forms.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.6/trexapi/forms/reward_api_forms.py` & `trex-apis-1.0.7/trexapi/forms/reward_api_forms.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.6/trexapi/forms/sales_api_forms.py` & `trex-apis-1.0.7/trexapi/forms/sales_api_forms.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.6/trexapi/forms/user_api_forms.py` & `trex-apis-1.0.7/trexapi/forms/user_api_forms.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.6/trexapi/libs/flask_auth_wrapper.py` & `trex-apis-1.0.7/trexapi/libs/flask_auth_wrapper.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.6/trexapi/utils/api_helpers.py` & `trex-apis-1.0.7/trexapi/utils/api_helpers.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.6/trexapi/utils/reward_transaction_helper.py` & `trex-apis-1.0.7/trexapi/utils/reward_transaction_helper.py`

 * *Files identical despite different names*

