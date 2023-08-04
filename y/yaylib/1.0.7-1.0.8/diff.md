# Comparing `tmp/yaylib-1.0.7.tar.gz` & `tmp/yaylib-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaylib-1.0.7.tar", last modified: Wed Aug  2 23:10:28 2023, max compression
+gzip compressed data, was "yaylib-1.0.8.tar", last modified: Fri Aug  4 11:48:25 2023, max compression
```

## Comparing `yaylib-1.0.7.tar` & `yaylib-1.0.8.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 23:10:28.635736 yaylib-1.0.7/
--rw-rw-rw-   0        0        0     1096 2023-07-09 07:25:01.000000 yaylib-1.0.7/LICENSE
--rw-rw-rw-   0        0        0    12901 2023-08-02 23:10:28.634728 yaylib-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0    11986 2023-08-01 05:26:45.000000 yaylib-1.0.7/README.md
--rw-rw-rw-   0        0        0       42 2023-08-02 23:10:28.635736 yaylib-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1646 2023-07-30 14:47:09.000000 yaylib-1.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-02 23:10:28.586065 yaylib-1.0.7/tests/
--rw-rw-rw-   0        0        0        0 2023-07-28 03:22:00.000000 yaylib-1.0.7/tests/__init__.py
--rw-rw-rw-   0        0        0     2205 2023-07-28 03:15:02.000000 yaylib-1.0.7/tests/config.py
--rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.7/tests/test_call.py
--rw-rw-rw-   0        0        0     1935 2023-07-09 07:25:01.000000 yaylib-1.0.7/tests/test_cassandra.py
--rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.7/tests/test_chat.py
--rw-rw-rw-   0        0        0     1337 2023-07-09 07:25:01.000000 yaylib-1.0.7/tests/test_group.py
--rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.7/tests/test_misc.py
--rw-rw-rw-   0        0        0     3723 2023-07-09 07:25:01.000000 yaylib-1.0.7/tests/test_post.py
--rw-rw-rw-   0        0        0     2028 2023-07-09 07:25:01.000000 yaylib-1.0.7/tests/test_review.py
--rw-rw-rw-   0        0        0     1339 2023-07-09 07:25:01.000000 yaylib-1.0.7/tests/test_thread.py
--rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.7/tests/test_user.py
--rw-rw-rw-   0        0        0     1908 2023-07-28 03:21:48.000000 yaylib-1.0.7/tests/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-08-02 23:10:28.595564 yaylib-1.0.7/yaylib/
--rw-rw-rw-   0        0        0      668 2023-07-25 06:44:17.000000 yaylib-1.0.7/yaylib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 23:10:28.633723 yaylib-1.0.7/yaylib/api/
--rw-rw-rw-   0        0        0      715 2023-07-25 06:44:11.000000 yaylib-1.0.7/yaylib/api/__init__.py
--rw-rw-rw-   0        0        0    14771 2023-07-31 09:13:51.000000 yaylib-1.0.7/yaylib/api/api.py
--rw-rw-rw-   0        0        0     9429 2023-07-23 06:18:02.000000 yaylib-1.0.7/yaylib/api/call.py
--rw-rw-rw-   0        0        0     2713 2023-07-28 02:06:00.000000 yaylib-1.0.7/yaylib/api/cassandra.py
--rw-rw-rw-   0        0        0    14964 2023-07-29 04:53:58.000000 yaylib-1.0.7/yaylib/api/chat.py
--rw-rw-rw-   0        0        0    23494 2023-07-30 13:58:08.000000 yaylib-1.0.7/yaylib/api/group.py
--rw-rw-rw-   0        0        0     8253 2023-07-31 09:13:58.000000 yaylib-1.0.7/yaylib/api/login.py
--rw-rw-rw-   0        0        0     7417 2023-07-18 08:52:45.000000 yaylib-1.0.7/yaylib/api/misc.py
--rw-rw-rw-   0        0        0    33647 2023-07-30 13:59:19.000000 yaylib-1.0.7/yaylib/api/post.py
--rw-rw-rw-   0        0        0     4445 2023-07-30 13:59:56.000000 yaylib-1.0.7/yaylib/api/review.py
--rw-rw-rw-   0        0        0     5945 2023-07-18 08:52:45.000000 yaylib-1.0.7/yaylib/api/thread.py
--rw-rw-rw-   0        0        0    23685 2023-07-30 14:01:24.000000 yaylib-1.0.7/yaylib/api/user.py
--rw-rw-rw-   0        0        0     9409 2023-07-28 13:12:41.000000 yaylib-1.0.7/yaylib/api/websocket.py
--rw-rw-rw-   0        0        0    86744 2023-08-01 05:27:28.000000 yaylib-1.0.7/yaylib/client.py
--rw-rw-rw-   0        0        0    18880 2023-07-31 07:48:17.000000 yaylib-1.0.7/yaylib/config.py
--rw-rw-rw-   0        0        0     2131 2023-07-18 08:52:45.000000 yaylib-1.0.7/yaylib/errors.py
--rw-rw-rw-   0        0        0    56113 2023-07-21 11:49:21.000000 yaylib-1.0.7/yaylib/models.py
--rw-rw-rw-   0        0        0    34292 2023-07-21 11:34:08.000000 yaylib-1.0.7/yaylib/responses.py
--rw-rw-rw-   0        0        0     1643 2023-07-31 07:40:14.000000 yaylib-1.0.7/yaylib/utils.py
-drwxrwxrwx   0        0        0        0 2023-08-02 23:10:28.619004 yaylib-1.0.7/yaylib.egg-info/
--rw-rw-rw-   0        0        0    12901 2023-08-02 23:10:28.000000 yaylib-1.0.7/yaylib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      799 2023-08-02 23:10:28.000000 yaylib-1.0.7/yaylib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 23:10:28.000000 yaylib-1.0.7/yaylib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-08-02 23:10:28.000000 yaylib-1.0.7/yaylib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-08-02 23:10:28.000000 yaylib-1.0.7/yaylib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-04 11:48:25.264502 yaylib-1.0.8/
+-rw-rw-rw-   0        0        0     1096 2023-07-09 07:25:01.000000 yaylib-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0    12901 2023-08-04 11:48:25.264502 yaylib-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0    11986 2023-08-03 05:52:33.000000 yaylib-1.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-04 11:48:25.264502 yaylib-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1646 2023-08-03 05:52:33.000000 yaylib-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 11:48:25.213107 yaylib-1.0.8/tests/
+-rw-rw-rw-   0        0        0        0 2023-08-03 05:52:33.000000 yaylib-1.0.8/tests/__init__.py
+-rw-rw-rw-   0        0        0     2205 2023-08-03 05:52:33.000000 yaylib-1.0.8/tests/config.py
+-rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.8/tests/test_call.py
+-rw-rw-rw-   0        0        0     1935 2023-07-09 07:25:01.000000 yaylib-1.0.8/tests/test_cassandra.py
+-rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.8/tests/test_chat.py
+-rw-rw-rw-   0        0        0     1337 2023-07-09 07:25:01.000000 yaylib-1.0.8/tests/test_group.py
+-rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.8/tests/test_misc.py
+-rw-rw-rw-   0        0        0     3723 2023-07-09 07:25:01.000000 yaylib-1.0.8/tests/test_post.py
+-rw-rw-rw-   0        0        0     2028 2023-07-09 07:25:01.000000 yaylib-1.0.8/tests/test_review.py
+-rw-rw-rw-   0        0        0     1339 2023-07-09 07:25:01.000000 yaylib-1.0.8/tests/test_thread.py
+-rw-rw-rw-   0        0        0     1335 2023-07-09 07:25:01.000000 yaylib-1.0.8/tests/test_user.py
+-rw-rw-rw-   0        0        0     1908 2023-08-03 05:52:33.000000 yaylib-1.0.8/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-08-04 11:48:25.222441 yaylib-1.0.8/yaylib/
+-rw-rw-rw-   0        0        0      668 2023-08-04 08:28:13.000000 yaylib-1.0.8/yaylib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-04 11:48:25.263292 yaylib-1.0.8/yaylib/api/
+-rw-rw-rw-   0        0        0      715 2023-08-03 05:52:33.000000 yaylib-1.0.8/yaylib/api/__init__.py
+-rw-rw-rw-   0        0        0    14777 2023-08-04 08:22:26.000000 yaylib-1.0.8/yaylib/api/api.py
+-rw-rw-rw-   0        0        0     9429 2023-08-03 05:52:33.000000 yaylib-1.0.8/yaylib/api/call.py
+-rw-rw-rw-   0        0        0     2713 2023-08-03 05:52:33.000000 yaylib-1.0.8/yaylib/api/cassandra.py
+-rw-rw-rw-   0        0        0    14964 2023-08-03 05:52:33.000000 yaylib-1.0.8/yaylib/api/chat.py
+-rw-rw-rw-   0        0        0    23520 2023-08-04 11:39:54.000000 yaylib-1.0.8/yaylib/api/group.py
+-rw-rw-rw-   0        0        0     8253 2023-08-03 05:52:33.000000 yaylib-1.0.8/yaylib/api/login.py
+-rw-rw-rw-   0        0        0     7417 2023-07-18 08:52:45.000000 yaylib-1.0.8/yaylib/api/misc.py
+-rw-rw-rw-   0        0        0    33647 2023-08-03 05:52:33.000000 yaylib-1.0.8/yaylib/api/post.py
+-rw-rw-rw-   0        0        0     4445 2023-08-03 05:52:33.000000 yaylib-1.0.8/yaylib/api/review.py
+-rw-rw-rw-   0        0        0     5945 2023-07-18 08:52:45.000000 yaylib-1.0.8/yaylib/api/thread.py
+-rw-rw-rw-   0        0        0    23685 2023-08-03 05:52:33.000000 yaylib-1.0.8/yaylib/api/user.py
+-rw-rw-rw-   0        0        0     9409 2023-08-03 05:52:33.000000 yaylib-1.0.8/yaylib/api/websocket.py
+-rw-rw-rw-   0        0        0    86748 2023-08-04 11:40:27.000000 yaylib-1.0.8/yaylib/client.py
+-rw-rw-rw-   0        0        0    18880 2023-08-04 11:46:28.000000 yaylib-1.0.8/yaylib/config.py
+-rw-rw-rw-   0        0        0     2131 2023-07-18 08:52:45.000000 yaylib-1.0.8/yaylib/errors.py
+-rw-rw-rw-   0        0        0    56916 2023-08-04 11:41:18.000000 yaylib-1.0.8/yaylib/models.py
+-rw-rw-rw-   0        0        0    34292 2023-08-03 05:52:33.000000 yaylib-1.0.8/yaylib/responses.py
+-rw-rw-rw-   0        0        0     1643 2023-08-03 05:52:33.000000 yaylib-1.0.8/yaylib/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-04 11:48:25.246967 yaylib-1.0.8/yaylib.egg-info/
+-rw-rw-rw-   0        0        0    12901 2023-08-04 11:48:25.000000 yaylib-1.0.8/yaylib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      799 2023-08-04 11:48:25.000000 yaylib-1.0.8/yaylib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 11:48:25.000000 yaylib-1.0.8/yaylib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-08-04 11:48:25.000000 yaylib-1.0.8/yaylib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-08-04 11:48:25.000000 yaylib-1.0.8/yaylib.egg-info/top_level.txt
```

### Comparing `yaylib-1.0.7/LICENSE` & `yaylib-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.7/PKG-INFO` & `yaylib-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaylib
-Version: 1.0.7
+Version: 1.0.8
 Summary: 同世代と趣味の通話コミュニティ - Yay! (イェイ) で、投稿やタイムラインの取得、リツイートやいいねの実行、フォローや投稿の検索など様々な機能を利用可能なAPIクライアントツールです。
 Home-page: https://github.com/qvco/yaylib
 Download-URL: https://github.com/qvco/yaylib
 Author: Qvco, Konn
 Author-email: nikola.desuga@gmail.com
 Maintainer: Qvco, Konn
 Maintainer-email: nikola.desuga@gmail.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: yaylib Version: 1.0.7 Summary:
+Metadata-Version: 2.1 Name: yaylib Version: 1.0.8 Summary:
 åä¸ä»£ã¨è¶£å³ã®éè©±ã³ãã¥ããã£ - Yay! (ã¤ã§ã¤)
 ã§ãæç¨¿ãã¿ã¤ã ã©ã¤ã³ã®åå¾ããªãã¤ã¼ããããã­ã®å®è¡ããã©ã­ã¼ãæç¨¿ã®æ¤ç´¢ãªã©æ§ããªæ©è½ãå©ç¨å¯è½ãªAPIã¯ã©ã¤ã¢ã³ããã¼ã«ã§ãã
 Home-page: https://github.com/qvco/yaylib Download-URL: https://github.com/
 qvco/yaylib Author: Qvco, Konn Author-email: nikola.desuga@gmail.com
 Maintainer: Qvco, Konn Maintainer-email: nikola.desuga@gmail.com License: MIT
 Keywords:
 yay,yaylib,api,bot,tool,client,library,wrapper,ããã,ã©ã¤ãã©ãª,ãã¼ã«
```

### Comparing `yaylib-1.0.7/README.md` & `yaylib-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.7/setup.py` & `yaylib-1.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.7/tests/config.py` & `yaylib-1.0.8/tests/config.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.7/tests/test_call.py` & `yaylib-1.0.8/tests/test_call.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.7/tests/test_cassandra.py` & `yaylib-1.0.8/tests/test_cassandra.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.7/tests/test_chat.py` & `yaylib-1.0.8/tests/test_chat.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.7/tests/test_group.py` & `yaylib-1.0.8/tests/test_group.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.7/tests/test_misc.py` & `yaylib-1.0.8/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.7/tests/test_post.py` & `yaylib-1.0.8/tests/test_post.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.7/tests/test_review.py` & `yaylib-1.0.8/tests/test_review.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.7/tests/test_thread.py` & `yaylib-1.0.8/tests/test_thread.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.7/tests/test_user.py` & `yaylib-1.0.8/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.7/tests/test_utils.py` & `yaylib-1.0.8/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.7/yaylib/__init__.py` & `yaylib-1.0.8/yaylib/__init__.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.7/yaylib/api/__init__.py` & `yaylib-1.0.8/yaylib/api/__init__.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.7/yaylib/api/api.py` & `yaylib-1.0.8/yaylib/api/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,17 +157,18 @@
             if self.save_cookie_file is True and response.status_code == 401:
                 if "/api/v1/oauth/token" in endpoint:
                     os.remove(self.base_path + self.cookie_filename + ".json")
                     message = "Refresh token expired. Try logging in again."
                     raise AuthenticationError(message)
 
                 auth_retry_count += 1
-                self.logger.debug("Access token expired. Refreshing tokens...")
 
                 if auth_retry_count < max_auth_retries:
+                    self.logger.debug("Access token expired. Refreshing tokens...")
+
                     cookies = self.load_cookies()
 
                     if cookies is not None and self.fernet is not None:
                         cookies = self.decrypt_cookies(self.fernet, cookies)
                         response = get_token(
                             self,
                             grant_type="refresh_token",
```

### Comparing `yaylib-1.0.7/yaylib/api/call.py` & `yaylib-1.0.8/yaylib/api/call.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.7/yaylib/api/cassandra.py` & `yaylib-1.0.8/yaylib/api/cassandra.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.7/yaylib/api/chat.py` & `yaylib-1.0.8/yaylib/api/chat.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.7/yaylib/api/group.py` & `yaylib-1.0.8/yaylib/api/group.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 """
 
 from datetime import datetime
 from typing import List
 
 from ..config import Endpoints
 from ..models import CreateGroupQuota
+from ..models import Group
 from ..responses import (
     CreateGroupResponse,
     GroupCategoriesResponse,
     GroupResponse,
     GroupsRelatedResponse,
     GroupsResponse,
     GroupUserResponse,
@@ -283,21 +284,21 @@
         "GET",
         endpoint=f"{Endpoints.GROUPS_V1}/created_quota",
         data_type=CreateGroupQuota,
         access_token=access_token,
     ).create
 
 
-def get_group(self, group_id: int, access_token: str = None) -> GroupResponse:
+def get_group(self, group_id: int, access_token: str = None) -> Group:
     return self._make_request(
         "GET",
         endpoint=f"{Endpoints.GROUPS_V1}/{group_id}",
         data_type=GroupResponse,
         access_token=access_token,
-    )
+    ).group
 
 
 def get_groups(self, access_token: str = None, **params) -> GroupsResponse:
     """
 
     Parameters:
     ----------
```

### Comparing `yaylib-1.0.7/yaylib/api/login.py` & `yaylib-1.0.8/yaylib/api/login.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.7/yaylib/api/misc.py` & `yaylib-1.0.8/yaylib/api/misc.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.7/yaylib/api/post.py` & `yaylib-1.0.8/yaylib/api/post.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.7/yaylib/api/review.py` & `yaylib-1.0.8/yaylib/api/review.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.7/yaylib/api/thread.py` & `yaylib-1.0.8/yaylib/api/thread.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.7/yaylib/api/user.py` & `yaylib-1.0.8/yaylib/api/user.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.7/yaylib/api/websocket.py` & `yaylib-1.0.8/yaylib/api/websocket.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.7/yaylib/client.py` & `yaylib-1.0.8/yaylib/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -265,14 +265,15 @@
 from .models import (
     Bgm,
     ChatRoom,
     ConferenceCall,
     CreateGroupQuota,
     Footprint,
     GifImageCategory,
+    Group,
     Message,
     Post,
     PresignedUrl,
     SharedUrl,
     StickerPack,
     Survey,
     ThreadInfo,
@@ -1167,15 +1168,15 @@
         """
 
         サークル作成可能な割当量を取得します
 
         """
         return get_create_group_quota(self, access_token)
 
-    def get_group(self, group_id: int, access_token: str = None) -> GroupResponse:
+    def get_group(self, group_id: int, access_token: str = None) -> Group:
         """
 
         サークルの詳細を取得します
 
         """
         return get_group(self, group_id, access_token)
```

### Comparing `yaylib-1.0.7/yaylib/config.py` & `yaylib-1.0.8/yaylib/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,18 +22,18 @@
 SOFTWARE.
 """
 
 from enum import Enum
 
 
 class Configs:
-    YAYLIB_VERSION = "1.0.7"
-    YAY_API_VERSION = "3.20"
-    YAY_VERSION_NAME = "3.20.1"
-    YAY_API_VERSION_KEY = "d4420f4943bebe2831c20b2b4cb4a8c1"
+    YAYLIB_VERSION = "1.0.8"
+    YAY_API_VERSION = "3.21"
+    YAY_VERSION_NAME = "3.21.0"
+    YAY_API_VERSION_KEY = "c687e24f6a454896891acd68868c7979"
     YAY_API_KEY = "ccd59ee269c01511ba763467045c115779fcae3050238a252f1bd1a4b65cfec6"
     YAY_SHARED_KEY = "yayZ1"
     YAY_STORE_KEY = "yayZ1payment"
     AGORA_APP_ID = "79046b8c9be54945b7f10a4d128d5395"
     ID_CARD_CHECK_SECRET_KEY = "4aa6d1c301a97154bc1098c2"
     YAY_REVIEW_HOST_1 = "review.yay.space"
     YAY_REVIEW_HOST_2 = "cas-stg.yay.space"
```

### Comparing `yaylib-1.0.7/yaylib/errors.py` & `yaylib-1.0.8/yaylib/errors.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.7/yaylib/models.py` & `yaylib-1.0.8/yaylib/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,31 +26,36 @@
 
 
 class Activity:
     __slots__ = (
         "data",
         "id",
         "created_at",
-        "created_at_parsed",
         "type",
         "user",
         "from_post",
         "to_post",
         "group",
         "followers",
+        "followers_count",
         "from_post_ids",
         "vip_reward",
         "is_bulk_invitation",
+        "content_preview",
+        "title",
+        "body",
+        "url",
+        "birthday_users",
+        "birthday_users_count",
     )
 
     def __init__(self, data):
         self.data = data
         self.id = data.get("id")
         self.created_at = data.get("created_at")
-        self.created_at_parsed = parse_datetime(data.get("created_at"))
         self.type = data.get("type")
 
         self.user = data.get("user")
         if self.user is not None:
             self.user = User(self.user)
 
         self.from_post = data.get("from_post")
@@ -65,17 +70,30 @@
         if self.group is not None:
             self.group = Group(self.group)
 
         self.followers = data.get("followers")
         if self.followers is not None:
             self.followers = [User(follower) for follower in self.followers]
 
+        self.followers_count = data.get("followers_count")
         self.from_post_ids = data.get("from_post_ids")
         self.vip_reward = data.get("vip_reward")
         self.is_bulk_invitation = data.get("is_bulk_invitation")
+        self.content_preview = data.get("content_preview")
+        self.title = data.get("title")
+        self.body = data.get("body")
+        self.url = data.get("url")
+
+        self.birthday_users = data.get("birthday_users")
+        if self.birthday_users is not None:
+            self.birthday_users = [
+                User(birthday_user) for birthday_user in self.birthday_users
+            ]
+
+        self.birthday_users_count = data.get("birthday_users_count")
 
     def __repr__(self):
         return f"Activity(data={self.data})"
 
 
 class BanWord:
     __slots__ = ("data", "id", "type", "word")
@@ -593,38 +611,41 @@
 
 class Group:
     __slots__ = (
         "data",
         "id",
         "topic",
         "description",
-        "user_id",
         "groups_users_count",
         "posts_count",
+        "user_id",
         "threads_count",
         "highlighted_count",
         "views_count",
         "related_count",
         "secret",
         "gender",
+        "place",
         "hide_reported_posts",
         "hide_conference_call",
         "is_private",
         "only_verified_age",
         "only_mobile_verified",
         "call_timeline_display",
         "updated_at",
-        "updated_at_parsed",
+        "group_icon",
+        "group_icon_thumbnail",
         "cover_image",
         "cover_image_thumbnail",
         "generation_groups_limit",
         "owner",
         "is_joined",
         "is_pending",
         "group_category_id",
+        "homepage",
         "unread_counts",
         "moderator_ids",
         "seizable",
         "seizable_before",
         "pending_count",
         "pending_transfer_id",
         "pending_deputize_ids",
@@ -653,33 +674,36 @@
         self.posts_count = data.get("posts_count")
         self.threads_count = data.get("threads_count")
         self.highlighted_count = data.get("highlighted_count")
         self.views_count = data.get("views_count")
         self.related_count = data.get("related_count")
         self.secret = data.get("secret")
         self.gender = data.get("gender")
+        self.place = data.get("place")
         self.hide_reported_posts = data.get("hide_reported_posts")
         self.hide_conference_call = data.get("hide_conference_call")
         self.is_private = data.get("is_private")
         self.only_verified_age = data.get("only_verified_age")
         self.only_mobile_verified = data.get("only_mobile_verified")
         self.call_timeline_display = data.get("call_timeline_display")
         self.updated_at = data.get("updated_at")
-        self.updated_at_parsed = parse_datetime(data.get("updated_at"))
+        self.group_icon = data.get("group_icon")
+        self.group_icon_thumbnail = data.get("group_icon_thumbnail")
         self.cover_image = data.get("cover_image")
         self.cover_image_thumbnail = data.get("cover_image_thumbnail")
         self.generation_groups_limit = data.get("generation_groups_limit")
 
         self.owner = data.get("owner")
         if self.owner is not None:
             self.owner = User(self.owner)
 
         self.is_joined = data.get("is_joined")
         self.is_pending = data.get("is_pending")
         self.group_category_id = data.get("group_category_id")
+        self.homepage = data.get("homepage")
         self.unread_counts = data.get("unread_counts")
         self.moderator_ids = data.get("moderator_ids")
         self.seizable = data.get("seizable")
         self.seizable_before = data.get("seizable_before")
         self.pending_count = data.get("pending_count")
         self.pending_transfer_id = data.get("pending_transfer_id")
         self.pending_deputize_ids = data.get("pending_deputize_ids")
```

### Comparing `yaylib-1.0.7/yaylib/responses.py` & `yaylib-1.0.8/yaylib/responses.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.7/yaylib/utils.py` & `yaylib-1.0.8/yaylib/utils.py`

 * *Files identical despite different names*

### Comparing `yaylib-1.0.7/yaylib.egg-info/PKG-INFO` & `yaylib-1.0.8/yaylib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaylib
-Version: 1.0.7
+Version: 1.0.8
 Summary: 同世代と趣味の通話コミュニティ - Yay! (イェイ) で、投稿やタイムラインの取得、リツイートやいいねの実行、フォローや投稿の検索など様々な機能を利用可能なAPIクライアントツールです。
 Home-page: https://github.com/qvco/yaylib
 Download-URL: https://github.com/qvco/yaylib
 Author: Qvco, Konn
 Author-email: nikola.desuga@gmail.com
 Maintainer: Qvco, Konn
 Maintainer-email: nikola.desuga@gmail.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: yaylib Version: 1.0.7 Summary:
+Metadata-Version: 2.1 Name: yaylib Version: 1.0.8 Summary:
 åä¸ä»£ã¨è¶£å³ã®éè©±ã³ãã¥ããã£ - Yay! (ã¤ã§ã¤)
 ã§ãæç¨¿ãã¿ã¤ã ã©ã¤ã³ã®åå¾ããªãã¤ã¼ããããã­ã®å®è¡ããã©ã­ã¼ãæç¨¿ã®æ¤ç´¢ãªã©æ§ããªæ©è½ãå©ç¨å¯è½ãªAPIã¯ã©ã¤ã¢ã³ããã¼ã«ã§ãã
 Home-page: https://github.com/qvco/yaylib Download-URL: https://github.com/
 qvco/yaylib Author: Qvco, Konn Author-email: nikola.desuga@gmail.com
 Maintainer: Qvco, Konn Maintainer-email: nikola.desuga@gmail.com License: MIT
 Keywords:
 yay,yaylib,api,bot,tool,client,library,wrapper,ããã,ã©ã¤ãã©ãª,ãã¼ã«
```

### Comparing `yaylib-1.0.7/yaylib.egg-info/SOURCES.txt` & `yaylib-1.0.8/yaylib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

