# Comparing `tmp/lendsmart_api-2.4.tar.gz` & `tmp/lendsmart_api-2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lendsmart_api-2.4.tar", last modified: Thu Mar 16 15:46:33 2023, max compression
+gzip compressed data, was "lendsmart_api-2.5.tar", last modified: Fri Aug  4 06:27:10 2023, max compression
```

## Comparing `lendsmart_api-2.4.tar` & `lendsmart_api-2.5.tar`

### file list

```diff
@@ -1,60 +1,61 @@
-drwxr-x---   0 root         (0) root         (0)        0 2023-03-16 15:46:33.000000 lendsmart_api-2.4/
-drwxr-x---   0 root         (0) root         (0)        0 2023-03-16 15:46:33.000000 lendsmart_api-2.4/test/
-drwxr-x---   0 root         (0) root         (0)        0 2023-03-16 15:46:33.000000 lendsmart_api-2.4/test/objects/
--rw-r-----   0 root         (0) root         (0)      523 2023-03-16 15:36:04.000000 lendsmart_api-2.4/test/objects/prediction_test.py
--rw-r-----   0 root         (0) root         (0)        0 2023-03-16 15:36:04.000000 lendsmart_api-2.4/test/objects/__init__.py
--rw-r-----   0 root         (0) root         (0)     1335 2023-03-16 15:36:04.000000 lendsmart_api-2.4/test/objects/test_access_token.py
--rw-r-----   0 root         (0) root         (0)      487 2023-03-16 15:36:04.000000 lendsmart_api-2.4/test/objects/document_test.py
--rw-r-----   0 root         (0) root         (0)     5267 2023-03-16 15:36:04.000000 lendsmart_api-2.4/test/base.py
--rw-r-----   0 root         (0) root         (0)     1156 2023-03-16 15:36:04.000000 lendsmart_api-2.4/test/task_test.py
--rw-r-----   0 root         (0) root         (0)     3164 2023-03-16 15:36:04.000000 lendsmart_api-2.4/test/team_member_test.py
--rw-r-----   0 root         (0) root         (0)        0 2023-03-16 15:36:04.000000 lendsmart_api-2.4/test/__init__.py
--rw-r-----   0 root         (0) root         (0)     2435 2023-03-16 15:36:04.000000 lendsmart_api-2.4/test/originating_loan_permission_test.py
--rw-r-----   0 root         (0) root         (0)     2651 2023-03-16 15:36:04.000000 lendsmart_api-2.4/test/loan_status_test.py
--rw-r-----   0 root         (0) root         (0)     1613 2023-03-16 15:36:04.000000 lendsmart_api-2.4/test/letter_of_explanations_test.py
--rw-r-----   0 root         (0) root         (0)     2050 2023-03-16 15:36:04.000000 lendsmart_api-2.4/test/lendsmart_client_test.py
--rw-r-----   0 root         (0) root         (0)     2759 2023-03-16 15:36:04.000000 lendsmart_api-2.4/test/advisor_profiles_test.py
--rw-r-----   0 root         (0) root         (0)     2521 2023-03-16 15:36:04.000000 lendsmart_api-2.4/test/openid_test.py
--rw-r-----   0 root         (0) root         (0)     1253 2023-03-16 15:36:04.000000 lendsmart_api-2.4/test/fixtures.py
--rw-r-----   0 root         (0) root         (0)      583 2023-03-16 15:36:04.000000 lendsmart_api-2.4/test/freddie_mac_test.py
--rw-r-----   0 root         (0) root         (0)     2686 2023-03-16 15:36:04.000000 lendsmart_api-2.4/README.md
--rwxr-x---   0 root         (0) root         (0)     2833 2023-03-16 15:46:05.000000 lendsmart_api-2.4/setup.py
--rw-r-----   0 root         (0) root         (0)     4510 2023-03-16 15:46:33.000000 lendsmart_api-2.4/PKG-INFO
-drwxr-x---   0 root         (0) root         (0)        0 2023-03-16 15:46:33.000000 lendsmart_api-2.4/lendsmart_api/
-drwxr-x---   0 root         (0) root         (0)        0 2023-03-16 15:46:33.000000 lendsmart_api-2.4/lendsmart_api/objects/
--rw-r-----   0 root         (0) root         (0)      646 2023-03-16 15:36:04.000000 lendsmart_api-2.4/lendsmart_api/objects/document_pointer.py
--rw-r-----   0 root         (0) root         (0)    12444 2023-03-16 15:36:04.000000 lendsmart_api-2.4/lendsmart_api/objects/base.py
--rw-r-----   0 root         (0) root         (0)      516 2023-03-16 15:36:04.000000 lendsmart_api-2.4/lendsmart_api/objects/namespace.py
--rw-r-----   0 root         (0) root         (0)      916 2023-03-16 15:36:04.000000 lendsmart_api-2.4/lendsmart_api/objects/dbase.py
--rw-r-----   0 root         (0) root         (0)      613 2023-03-16 15:36:04.000000 lendsmart_api-2.4/lendsmart_api/objects/__init__.py
--rw-r-----   0 root         (0) root         (0)      482 2023-03-16 15:36:04.000000 lendsmart_api-2.4/lendsmart_api/objects/letter_of_explanations.py
--rw-r-----   0 root         (0) root         (0)      636 2023-03-16 15:36:04.000000 lendsmart_api-2.4/lendsmart_api/objects/task.py
--rw-r-----   0 root         (0) root         (0)     7742 2023-03-16 15:36:04.000000 lendsmart_api-2.4/lendsmart_api/objects/filtering.py
--rw-r-----   0 root         (0) root         (0)     1032 2023-03-16 15:36:04.000000 lendsmart_api-2.4/lendsmart_api/objects/advisors.py
--rw-r-----   0 root         (0) root         (0)      595 2023-03-16 15:36:04.000000 lendsmart_api-2.4/lendsmart_api/objects/notifier.py
--rw-r-----   0 root         (0) root         (0)      821 2023-03-16 15:36:04.000000 lendsmart_api-2.4/lendsmart_api/objects/lending_term.py
--rw-r-----   0 root         (0) root         (0)     1495 2023-03-16 15:36:04.000000 lendsmart_api-2.4/lendsmart_api/objects/prediction.py
--rw-r-----   0 root         (0) root         (0)      734 2023-03-16 15:36:04.000000 lendsmart_api-2.4/lendsmart_api/objects/account.py
--rw-r-----   0 root         (0) root         (0)      589 2023-03-16 15:36:04.000000 lendsmart_api-2.4/lendsmart_api/objects/signature.py
--rw-r-----   0 root         (0) root         (0)      735 2023-03-16 15:36:04.000000 lendsmart_api-2.4/lendsmart_api/objects/document.py
--rw-r-----   0 root         (0) root         (0)      424 2023-03-16 15:36:04.000000 lendsmart_api-2.4/lendsmart_api/objects/finicity.py
--rw-r-----   0 root         (0) root         (0)      437 2023-03-16 15:36:04.000000 lendsmart_api-2.4/lendsmart_api/objects/openids.py
--rw-r-----   0 root         (0) root         (0)      366 2023-03-16 15:36:04.000000 lendsmart_api-2.4/lendsmart_api/__init__.py
--rw-r-----   0 root         (0) root         (0)     1162 2023-03-16 15:36:04.000000 lendsmart_api-2.4/lendsmart_api/errors.py
-drwxr-x---   0 root         (0) root         (0)        0 2023-03-16 15:46:33.000000 lendsmart_api-2.4/lendsmart_api/jwt/
-drwxr-x---   0 root         (0) root         (0)        0 2023-03-16 15:46:33.000000 lendsmart_api-2.4/lendsmart_api/jwt/access_token/
--rw-r-----   0 root         (0) root         (0)      722 2023-03-16 15:36:04.000000 lendsmart_api-2.4/lendsmart_api/jwt/access_token/service_account.py
--rw-r-----   0 root         (0) root         (0)     1215 2023-03-16 15:36:04.000000 lendsmart_api-2.4/lendsmart_api/jwt/access_token/__init__.py
--rw-r-----   0 root         (0) root         (0)     6279 2023-03-16 15:36:04.000000 lendsmart_api-2.4/lendsmart_api/jwt/__init__.py
--rw-r-----   0 root         (0) root         (0)     1118 2023-03-16 15:36:04.000000 lendsmart_api-2.4/lendsmart_api/jwt/compat.py
--rw-r-----   0 root         (0) root         (0)    45085 2023-03-16 15:36:04.000000 lendsmart_api-2.4/lendsmart_api/lendsmart_client.py
--rw-r-----   0 root         (0) root         (0)     1079 2023-03-16 15:36:04.000000 lendsmart_api-2.4/lendsmart_api/constants.py
--rw-r-----   0 root         (0) root         (0)     1551 2023-03-16 15:36:04.000000 lendsmart_api-2.4/lendsmart_api/common.py
--rw-r-----   0 root         (0) root         (0)     7775 2023-03-16 15:36:04.000000 lendsmart_api-2.4/lendsmart_api/paginated_list.py
-drwxr-x---   0 root         (0) root         (0)        0 2023-03-16 15:46:33.000000 lendsmart_api-2.4/lendsmart_api.egg-info/
--rw-r-----   0 root         (0) root         (0)        1 2023-03-16 15:46:33.000000 lendsmart_api-2.4/lendsmart_api.egg-info/dependency_links.txt
--rw-r-----   0 root         (0) root         (0)     4510 2023-03-16 15:46:33.000000 lendsmart_api-2.4/lendsmart_api.egg-info/PKG-INFO
--rw-r-----   0 root         (0) root         (0)       19 2023-03-16 15:46:33.000000 lendsmart_api-2.4/lendsmart_api.egg-info/top_level.txt
--rw-r-----   0 root         (0) root         (0)       29 2023-03-16 15:46:33.000000 lendsmart_api-2.4/lendsmart_api.egg-info/requires.txt
--rw-r-----   0 root         (0) root         (0)     1534 2023-03-16 15:46:33.000000 lendsmart_api-2.4/lendsmart_api.egg-info/SOURCES.txt
--rw-r-----   0 root         (0) root         (0)       38 2023-03-16 15:46:33.000000 lendsmart_api-2.4/setup.cfg
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-04 06:27:10.912759 lendsmart_api-2.5/
+-rw-rw-r--   0 user      (1000) user      (1000)     1486 2023-08-04 06:26:09.000000 lendsmart_api-2.5/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)     3405 2023-08-04 06:27:10.912759 lendsmart_api-2.5/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     2686 2023-08-04 06:26:09.000000 lendsmart_api-2.5/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-04 06:27:10.908759 lendsmart_api-2.5/lendsmart_api/
+-rw-rw-r--   0 user      (1000) user      (1000)      366 2023-08-04 06:26:09.000000 lendsmart_api-2.5/lendsmart_api/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1551 2023-08-04 06:26:09.000000 lendsmart_api-2.5/lendsmart_api/common.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1079 2023-08-04 06:26:09.000000 lendsmart_api-2.5/lendsmart_api/constants.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1162 2023-08-04 06:26:09.000000 lendsmart_api-2.5/lendsmart_api/errors.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-04 06:27:10.908759 lendsmart_api-2.5/lendsmart_api/jwt/
+-rw-rw-r--   0 user      (1000) user      (1000)     6279 2023-08-04 06:26:09.000000 lendsmart_api-2.5/lendsmart_api/jwt/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-04 06:27:10.908759 lendsmart_api-2.5/lendsmart_api/jwt/access_token/
+-rw-rw-r--   0 user      (1000) user      (1000)     1215 2023-08-04 06:26:09.000000 lendsmart_api-2.5/lendsmart_api/jwt/access_token/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      722 2023-08-04 06:26:09.000000 lendsmart_api-2.5/lendsmart_api/jwt/access_token/service_account.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1118 2023-08-04 06:26:09.000000 lendsmart_api-2.5/lendsmart_api/jwt/compat.py
+-rw-rw-r--   0 user      (1000) user      (1000)    45085 2023-08-04 06:26:09.000000 lendsmart_api-2.5/lendsmart_api/lendsmart_client.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-04 06:27:10.908759 lendsmart_api-2.5/lendsmart_api/objects/
+-rw-rw-r--   0 user      (1000) user      (1000)      613 2023-08-04 06:26:09.000000 lendsmart_api-2.5/lendsmart_api/objects/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      734 2023-08-04 06:26:09.000000 lendsmart_api-2.5/lendsmart_api/objects/account.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1032 2023-08-04 06:26:09.000000 lendsmart_api-2.5/lendsmart_api/objects/advisors.py
+-rw-rw-r--   0 user      (1000) user      (1000)    12444 2023-08-04 06:26:09.000000 lendsmart_api-2.5/lendsmart_api/objects/base.py
+-rw-rw-r--   0 user      (1000) user      (1000)      916 2023-08-04 06:26:09.000000 lendsmart_api-2.5/lendsmart_api/objects/dbase.py
+-rw-rw-r--   0 user      (1000) user      (1000)      735 2023-08-04 06:26:09.000000 lendsmart_api-2.5/lendsmart_api/objects/document.py
+-rw-rw-r--   0 user      (1000) user      (1000)      646 2023-08-04 06:26:09.000000 lendsmart_api-2.5/lendsmart_api/objects/document_pointer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7742 2023-08-04 06:26:09.000000 lendsmart_api-2.5/lendsmart_api/objects/filtering.py
+-rw-rw-r--   0 user      (1000) user      (1000)      424 2023-08-04 06:26:09.000000 lendsmart_api-2.5/lendsmart_api/objects/finicity.py
+-rw-rw-r--   0 user      (1000) user      (1000)      821 2023-08-04 06:26:09.000000 lendsmart_api-2.5/lendsmart_api/objects/lending_term.py
+-rw-rw-r--   0 user      (1000) user      (1000)      482 2023-08-04 06:26:09.000000 lendsmart_api-2.5/lendsmart_api/objects/letter_of_explanations.py
+-rw-rw-r--   0 user      (1000) user      (1000)      516 2023-08-04 06:26:09.000000 lendsmart_api-2.5/lendsmart_api/objects/namespace.py
+-rw-rw-r--   0 user      (1000) user      (1000)      595 2023-08-04 06:26:09.000000 lendsmart_api-2.5/lendsmart_api/objects/notifier.py
+-rw-rw-r--   0 user      (1000) user      (1000)      437 2023-08-04 06:26:09.000000 lendsmart_api-2.5/lendsmart_api/objects/openids.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1495 2023-08-04 06:26:09.000000 lendsmart_api-2.5/lendsmart_api/objects/prediction.py
+-rw-rw-r--   0 user      (1000) user      (1000)      589 2023-08-04 06:26:09.000000 lendsmart_api-2.5/lendsmart_api/objects/signature.py
+-rw-rw-r--   0 user      (1000) user      (1000)      636 2023-08-04 06:26:09.000000 lendsmart_api-2.5/lendsmart_api/objects/task.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7775 2023-08-04 06:26:09.000000 lendsmart_api-2.5/lendsmart_api/paginated_list.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-04 06:27:10.908759 lendsmart_api-2.5/lendsmart_api.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)     3405 2023-08-04 06:27:10.000000 lendsmart_api-2.5/lendsmart_api.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1542 2023-08-04 06:27:10.000000 lendsmart_api-2.5/lendsmart_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      184 2023-08-04 06:27:10.000000 lendsmart_api-2.5/lendsmart_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       22 2023-08-04 06:27:10.000000 lendsmart_api-2.5/lendsmart_api.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       19 2023-08-04 06:27:10.000000 lendsmart_api-2.5/lendsmart_api.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-08-04 06:27:10.912759 lendsmart_api-2.5/setup.cfg
+-rwxrwxr-x   0 user      (1000) user      (1000)     3134 2023-08-04 06:26:09.000000 lendsmart_api-2.5/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-04 06:27:10.912759 lendsmart_api-2.5/test/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-08-04 06:26:09.000000 lendsmart_api-2.5/test/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2759 2023-08-04 06:26:09.000000 lendsmart_api-2.5/test/advisor_profiles_test.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5267 2023-08-04 06:26:09.000000 lendsmart_api-2.5/test/base.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1253 2023-08-04 06:26:09.000000 lendsmart_api-2.5/test/fixtures.py
+-rw-rw-r--   0 user      (1000) user      (1000)      583 2023-08-04 06:26:09.000000 lendsmart_api-2.5/test/freddie_mac_test.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2050 2023-08-04 06:26:09.000000 lendsmart_api-2.5/test/lendsmart_client_test.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1613 2023-08-04 06:26:09.000000 lendsmart_api-2.5/test/letter_of_explanations_test.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2651 2023-08-04 06:26:09.000000 lendsmart_api-2.5/test/loan_status_test.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-04 06:27:10.912759 lendsmart_api-2.5/test/objects/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-08-04 06:26:09.000000 lendsmart_api-2.5/test/objects/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      487 2023-08-04 06:26:09.000000 lendsmart_api-2.5/test/objects/document_test.py
+-rw-rw-r--   0 user      (1000) user      (1000)      523 2023-08-04 06:26:09.000000 lendsmart_api-2.5/test/objects/prediction_test.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1335 2023-08-04 06:26:09.000000 lendsmart_api-2.5/test/objects/test_access_token.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2521 2023-08-04 06:26:09.000000 lendsmart_api-2.5/test/openid_test.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2435 2023-08-04 06:26:09.000000 lendsmart_api-2.5/test/originating_loan_permission_test.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1156 2023-08-04 06:26:09.000000 lendsmart_api-2.5/test/task_test.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3164 2023-08-04 06:26:09.000000 lendsmart_api-2.5/test/team_member_test.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `lendsmart_api-2.4/test/objects/prediction_test.py` & `lendsmart_api-2.5/test/objects/prediction_test.py`

 * *Files identical despite different names*

### Comparing `lendsmart_api-2.4/test/objects/test_access_token.py` & `lendsmart_api-2.5/test/objects/test_access_token.py`

 * *Files identical despite different names*

### Comparing `lendsmart_api-2.4/test/base.py` & `lendsmart_api-2.5/test/base.py`

 * *Files identical despite different names*

### Comparing `lendsmart_api-2.4/test/task_test.py` & `lendsmart_api-2.5/test/task_test.py`

 * *Files identical despite different names*

### Comparing `lendsmart_api-2.4/test/team_member_test.py` & `lendsmart_api-2.5/test/team_member_test.py`

 * *Files identical despite different names*

### Comparing `lendsmart_api-2.4/test/originating_loan_permission_test.py` & `lendsmart_api-2.5/test/originating_loan_permission_test.py`

 * *Files identical despite different names*

### Comparing `lendsmart_api-2.4/test/loan_status_test.py` & `lendsmart_api-2.5/test/loan_status_test.py`

 * *Files identical despite different names*

### Comparing `lendsmart_api-2.4/test/letter_of_explanations_test.py` & `lendsmart_api-2.5/test/letter_of_explanations_test.py`

 * *Files identical despite different names*

### Comparing `lendsmart_api-2.4/test/lendsmart_client_test.py` & `lendsmart_api-2.5/test/lendsmart_client_test.py`

 * *Files identical despite different names*

### Comparing `lendsmart_api-2.4/test/advisor_profiles_test.py` & `lendsmart_api-2.5/test/advisor_profiles_test.py`

 * *Files identical despite different names*

### Comparing `lendsmart_api-2.4/test/openid_test.py` & `lendsmart_api-2.5/test/openid_test.py`

 * *Files identical despite different names*

### Comparing `lendsmart_api-2.4/test/fixtures.py` & `lendsmart_api-2.5/test/fixtures.py`

 * *Files identical despite different names*

### Comparing `lendsmart_api-2.4/test/freddie_mac_test.py` & `lendsmart_api-2.5/test/freddie_mac_test.py`

 * *Files identical despite different names*

### Comparing `lendsmart_api-2.4/README.md` & `lendsmart_api-2.5/README.md`

 * *Files identical despite different names*

### Comparing `lendsmart_api-2.4/setup.py` & `lendsmart_api-2.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/env python3
+# pylint: disable=W0622, C0116, C0301
 """
 A setuptools based setup module
 
 Based on a template here:
 https://github.com/pypa/sampleproject/blob/master/setup.py
 """
 
@@ -27,15 +28,15 @@
 
 setup(
     name='lendsmart_api',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='2.4',
+    version='2.5',
 
     description='The official python SDK for LendSmart API v1',
     long_description=long_description,
     long_description_content_type="text/markdown",
 
     # The project's main homepage.
     url='https://bitbucket.org/lendsmartlabs/lendsmart_py/',
@@ -85,13 +86,16 @@
         "retry",
     ] if sys.version_info >= (3, 4) else [
         "future",
         "requests",
         "enum34",
         "retry",
     ],
-
+    dependency_links=[
+        # this is cryptography package
+        "https://files.pythonhosted.org/packages/fe/ee/aa40ae0f8cfb5988736b3a93adba13421dbfe318211d48a2da138a3a346e/cryptography-41.0.2-cp37-abi3-manylinux_2_17_x86_64.manylinux2014_x86_64.whl",
+    ],
     tests_require=[
         "mock",
     ],
     test_suite= 'setup.get_test_suite'
 )
```

### Comparing `lendsmart_api-2.4/lendsmart_api/objects/document_pointer.py` & `lendsmart_api-2.5/lendsmart_api/objects/document_pointer.py`

 * *Files identical despite different names*

### Comparing `lendsmart_api-2.4/lendsmart_api/objects/base.py` & `lendsmart_api-2.5/lendsmart_api/objects/base.py`

 * *Files identical despite different names*

### Comparing `lendsmart_api-2.4/lendsmart_api/objects/namespace.py` & `lendsmart_api-2.5/lendsmart_api/objects/namespace.py`

 * *Files identical despite different names*

### Comparing `lendsmart_api-2.4/lendsmart_api/objects/dbase.py` & `lendsmart_api-2.5/lendsmart_api/objects/dbase.py`

 * *Files identical despite different names*

### Comparing `lendsmart_api-2.4/lendsmart_api/objects/__init__.py` & `lendsmart_api-2.5/lendsmart_api/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `lendsmart_api-2.4/lendsmart_api/objects/task.py` & `lendsmart_api-2.5/lendsmart_api/objects/task.py`

 * *Files identical despite different names*

### Comparing `lendsmart_api-2.4/lendsmart_api/objects/filtering.py` & `lendsmart_api-2.5/lendsmart_api/objects/filtering.py`

 * *Files identical despite different names*

### Comparing `lendsmart_api-2.4/lendsmart_api/objects/advisors.py` & `lendsmart_api-2.5/lendsmart_api/objects/advisors.py`

 * *Files identical despite different names*

### Comparing `lendsmart_api-2.4/lendsmart_api/objects/notifier.py` & `lendsmart_api-2.5/lendsmart_api/objects/notifier.py`

 * *Files identical despite different names*

### Comparing `lendsmart_api-2.4/lendsmart_api/objects/lending_term.py` & `lendsmart_api-2.5/lendsmart_api/objects/lending_term.py`

 * *Files identical despite different names*

### Comparing `lendsmart_api-2.4/lendsmart_api/objects/prediction.py` & `lendsmart_api-2.5/lendsmart_api/objects/prediction.py`

 * *Files identical despite different names*

### Comparing `lendsmart_api-2.4/lendsmart_api/objects/account.py` & `lendsmart_api-2.5/lendsmart_api/objects/account.py`

 * *Files identical despite different names*

### Comparing `lendsmart_api-2.4/lendsmart_api/objects/signature.py` & `lendsmart_api-2.5/lendsmart_api/objects/signature.py`

 * *Files identical despite different names*

### Comparing `lendsmart_api-2.4/lendsmart_api/objects/document.py` & `lendsmart_api-2.5/lendsmart_api/objects/document.py`

 * *Files identical despite different names*

### Comparing `lendsmart_api-2.4/lendsmart_api/errors.py` & `lendsmart_api-2.5/lendsmart_api/errors.py`

 * *Files identical despite different names*

### Comparing `lendsmart_api-2.4/lendsmart_api/jwt/access_token/service_account.py` & `lendsmart_api-2.5/lendsmart_api/jwt/access_token/service_account.py`

 * *Files identical despite different names*

### Comparing `lendsmart_api-2.4/lendsmart_api/jwt/access_token/__init__.py` & `lendsmart_api-2.5/lendsmart_api/jwt/access_token/__init__.py`

 * *Files identical despite different names*

### Comparing `lendsmart_api-2.4/lendsmart_api/jwt/__init__.py` & `lendsmart_api-2.5/lendsmart_api/jwt/__init__.py`

 * *Files identical despite different names*

### Comparing `lendsmart_api-2.4/lendsmart_api/jwt/compat.py` & `lendsmart_api-2.5/lendsmart_api/jwt/compat.py`

 * *Files identical despite different names*

### Comparing `lendsmart_api-2.4/lendsmart_api/lendsmart_client.py` & `lendsmart_api-2.5/lendsmart_api/lendsmart_client.py`

 * *Files identical despite different names*

### Comparing `lendsmart_api-2.4/lendsmart_api/constants.py` & `lendsmart_api-2.5/lendsmart_api/constants.py`

 * *Files identical despite different names*

### Comparing `lendsmart_api-2.4/lendsmart_api/common.py` & `lendsmart_api-2.5/lendsmart_api/common.py`

 * *Files identical despite different names*

### Comparing `lendsmart_api-2.4/lendsmart_api/paginated_list.py` & `lendsmart_api-2.5/lendsmart_api/paginated_list.py`

 * *Files identical despite different names*

### Comparing `lendsmart_api-2.4/lendsmart_api.egg-info/PKG-INFO` & `lendsmart_api-2.5/lendsmart_api.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,157 +1,157 @@
 Metadata-Version: 2.1
 Name: lendsmart-api
-Version: 2.4
+Version: 2.5
 Summary: The official python SDK for LendSmart API v1
 Home-page: https://bitbucket.org/lendsmartlabs/lendsmart_py/
 Author: Smart Labs
 Author-email: infos@lendsmart.ai
 License: MIT
-Description: # lendsmart_api
-        
-        *python*
-        
-        The official python library for the [Lendsmart API v1](https://lendsmartlabs.postman.co)` in python.
-        
-        **This library is currently in beta.**
-        
-        [![PyPI](https://img.shields.io/pypi/v/lendsmart-api.svg)](https://pypi.python.org/pypi/lendsmart-api)
-        [![PyPI](https://img.shields.io/pypi/pyversions/lendsmart-api.svg)](https://pypi.python.org/pypi/lendsmart-api)
-        
-        [https://badge.fury.io/py/lendsmart-api.svg](https://badge.fury.io/py/lendsmart-api)
-        
-        
-        
-        ## Pre reqs
-        
-        - python 3
-        
-        - install virtualenv using below command
-        
-        ```
-            pip install virtualenv
-        ```
-        
-        ## Activate virtual environment
-        
-        ```
-            . ./venv/bin/activate
-        ```
-        
-        ## Installation
-        
-        ```
-            pip install lendsmart_api
-        ```
-        
-        # Usage
-        
-        You will need the service account private key files to access Lendsmart.
-        
-        Only a limited set of API is supported.
-        
-        ## Client
-        
-        ### Create client
-        
-        ```
-        
-        ```
-        
-        ### Update Document
-        
-        
-        ```
-        
-        
-        ```
-        
-        
-        
-        # Building from Source
-        
-        
-        To build and install this package:
-        
-        - Clone this repository
-        
-        ```
-        
-            cd core_api
-        
-            virtualenv venv
-        
-            ./setup.py install
-        ```
-        
-        # Testing individually
-        
-        Make sure the `prereqs`, and `building from source` are complete
-        
-        ```
-        
-            cd lendsmart_python
-        
-            . venv/bin/activate
-        
-            python3 get_documents_test.py
-        ```
-        # Local testing with lendsmart_api package
-        # Set environment path to your local file path in your python file
-        
-        ```
-        import sys
-        sys.path.append('/home/lendsmart/code/lendsmart/workspace/py_lscommon/core_api/')
-        ```
-        # remove old package which is in virtual environment
-        ```
-        rm -r /venv/lib/python3.8/site-packages/lendsmart_api
-        ```
-        # Auto tests
-        
-        Tests live in the ``tests`` directory.  When invoking tests, make sure you are
-        in the root directory of this project.  To run the full suite across all
-        supported python versions, use tox_:
-        
-        ```
-        
-           tox
-        
-        ```
-        
-        Running tox also runs pylint and coverage reports.
-        
-        The test suite uses fixtures stored as JSON in `test/fixtures`.  These files
-        contain sanitized JSON responses from the API - the file name is the URL called
-        to produce the response, replacing any slashes with underscores.
-        
-        Test classes should extend `test.base.ClientBaseCase`.  This provides them
-        with `self.client`, a `LendsmartClient` object that is set up to work with
-        tests.  Importantly, any GET request made by this object will be mocked to
-        retrieve data from the test fixtures.  This includes lazy-loaded objects using
-        this client (and by extension related models).
-        
-        When testing against requests other than GET requests, `self.mock_post` (and
-        equivalent methods for other HTTP verbs) can be used in a ``with`` block to
-        mock out the intended request type.  
-        
-        [tox](http://tox.readthedocs.io)
-        
-        # License
-        
-        MIT
-        
-        # Author
-        
-        Lendsmart Inc, USA
-        
 Keywords: prediction ai lendsmart
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# lendsmart_api
+
+*python*
+
+The official python library for the [Lendsmart API v1](https://lendsmartlabs.postman.co)` in python.
+
+**This library is currently in beta.**
+
+[![PyPI](https://img.shields.io/pypi/v/lendsmart-api.svg)](https://pypi.python.org/pypi/lendsmart-api)
+[![PyPI](https://img.shields.io/pypi/pyversions/lendsmart-api.svg)](https://pypi.python.org/pypi/lendsmart-api)
+
+[https://badge.fury.io/py/lendsmart-api.svg](https://badge.fury.io/py/lendsmart-api)
+
+
+
+## Pre reqs
+
+- python 3
+
+- install virtualenv using below command
+
+```
+    pip install virtualenv
+```
+
+## Activate virtual environment
+
+```
+    . ./venv/bin/activate
+```
+
+## Installation
+
+```
+    pip install lendsmart_api
+```
+
+# Usage
+
+You will need the service account private key files to access Lendsmart.
+
+Only a limited set of API is supported.
+
+## Client
+
+### Create client
+
+```
+
+```
+
+### Update Document
+
+
+```
+
+
+```
+
+
+
+# Building from Source
+
+
+To build and install this package:
+
+- Clone this repository
+
+```
+
+    cd core_api
+
+    virtualenv venv
+
+    ./setup.py install
+```
+
+# Testing individually
+
+Make sure the `prereqs`, and `building from source` are complete
+
+```
+
+    cd lendsmart_python
+
+    . venv/bin/activate
+
+    python3 get_documents_test.py
+```
+# Local testing with lendsmart_api package
+# Set environment path to your local file path in your python file
+
+```
+import sys
+sys.path.append('/home/lendsmart/code/lendsmart/workspace/py_lscommon/core_api/')
+```
+# remove old package which is in virtual environment
+```
+rm -r /venv/lib/python3.8/site-packages/lendsmart_api
+```
+# Auto tests
+
+Tests live in the ``tests`` directory.  When invoking tests, make sure you are
+in the root directory of this project.  To run the full suite across all
+supported python versions, use tox_:
+
+```
+
+   tox
+
+```
+
+Running tox also runs pylint and coverage reports.
+
+The test suite uses fixtures stored as JSON in `test/fixtures`.  These files
+contain sanitized JSON responses from the API - the file name is the URL called
+to produce the response, replacing any slashes with underscores.
+
+Test classes should extend `test.base.ClientBaseCase`.  This provides them
+with `self.client`, a `LendsmartClient` object that is set up to work with
+tests.  Importantly, any GET request made by this object will be mocked to
+retrieve data from the test fixtures.  This includes lazy-loaded objects using
+this client (and by extension related models).
+
+When testing against requests other than GET requests, `self.mock_post` (and
+equivalent methods for other HTTP verbs) can be used in a ``with`` block to
+mock out the intended request type.  
+
+[tox](http://tox.readthedocs.io)
+
+# License
+
+MIT
+
+# Author
+
+Lendsmart Inc, USA
```

### Comparing `lendsmart_api-2.4/lendsmart_api.egg-info/SOURCES.txt` & `lendsmart_api-2.5/lendsmart_api.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 lendsmart_api/__init__.py
 lendsmart_api/common.py
 lendsmart_api/constants.py
 lendsmart_api/errors.py
 lendsmart_api/lendsmart_client.py
```

