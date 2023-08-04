# Comparing `tmp/garth-0.3.5.tar.gz` & `tmp/garth-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garth-0.3.5.tar", last modified: Sun Jul 30 02:37:07 2023, max compression
+gzip compressed data, was "garth-0.4.0.tar", last modified: Fri Aug  4 04:47:08 2023, max compression
```

## Comparing `garth-0.3.5.tar` & `garth-0.4.0.tar`

### file list

```diff
@@ -1,53 +1,51 @@
--rw-r--r--   0        0        0     1071 2023-07-20 12:44:00.130760 garth-0.3.5/LICENSE
--rw-r--r--   0        0        0    13326 2023-07-30 01:22:39.496857 garth-0.3.5/README.md
--rw-r--r--   0        0        0      683 2023-07-30 01:10:44.332019 garth-0.3.5/garth/__init__.py
--rw-r--r--   0        0        0      931 2023-07-28 12:08:41.094670 garth-0.3.5/garth/auth_token.py
--rw-r--r--   0        0        0      145 2023-07-18 22:32:58.010661 garth-0.3.5/garth/exc.py
--rw-r--r--   0        0        0     4678 2023-07-30 02:35:49.039173 garth-0.3.5/garth/http.py
--rw-r--r--   0        0        0        0 2023-07-27 13:16:10.642595 garth-0.3.5/garth/py.typed
--rw-r--r--   0        0        0      434 2023-07-30 01:10:27.575730 garth-0.3.5/garth/resources/__init__.py
--rw-r--r--   0        0        0     1167 2023-07-30 01:22:51.576888 garth-0.3.5/garth/resources/hrv.py
--rw-r--r--   0        0        0      612 2023-07-29 23:28:46.923483 garth-0.3.5/garth/resources/intensity_minutes.py
--rw-r--r--   0        0        0     3524 2023-07-30 01:09:43.261424 garth-0.3.5/garth/resources/sleep.py
--rw-r--r--   0        0        0      654 2023-07-29 23:30:44.232250 garth-0.3.5/garth/resources/steps.py
--rw-r--r--   0        0        0      653 2023-07-29 23:30:50.433149 garth-0.3.5/garth/resources/stress.py
--rw-r--r--   0        0        0     3767 2023-07-28 12:13:50.747670 garth-0.3.5/garth/sso.py
--rw-r--r--   0        0        0     1529 2023-07-29 23:29:30.202390 garth-0.3.5/garth/stats.py
--rw-r--r--   0        0        0     1319 2023-07-30 01:09:15.596865 garth-0.3.5/garth/utils.py
--rw-r--r--   0        0        0       22 2023-07-30 02:36:35.896096 garth-0.3.5/garth/version.py
--rw-r--r--   0        0        0     1146 2023-07-30 02:37:07.146077 garth-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     2386 2023-07-22 11:39:14.617674 garth-0.3.5/tests/cassettes/test_client_get.yaml
--rw-r--r--   0        0        0     2425 2023-07-22 11:39:14.746057 garth-0.3.5/tests/cassettes/test_client_post.yaml
--rw-r--r--   0        0        0   100962 2023-07-22 11:22:15.428262 garth-0.3.5/tests/cassettes/test_client_request.yaml
--rw-r--r--   0        0        0     2331 2023-07-28 03:35:21.644342 garth-0.3.5/tests/cassettes/test_connectapi.yaml
--rw-r--r--   0        0        0     4564 2023-07-28 03:35:21.644997 garth-0.3.5/tests/cassettes/test_connectapi_refresh.yaml
--rw-r--r--   0        0        0     3231 2023-07-28 03:35:21.645581 garth-0.3.5/tests/cassettes/test_exchange.yaml
--rw-r--r--   0        0        0    10962 2023-07-23 13:53:16.232082 garth-0.3.5/tests/cassettes/test_get_username.yaml
--rw-r--r--   0        0        0    50551 2023-07-22 15:27:42.274531 garth-0.3.5/tests/cassettes/test_login_email_password_fail.yaml
--rw-r--r--   0        0        0    91847 2023-07-23 13:50:32.012417 garth-0.3.5/tests/cassettes/test_login_success.yaml
--rw-r--r--   0        0        0     2270 2023-07-28 03:35:21.646057 garth-0.3.5/tests/cassettes/test_refresh.yaml
--rw-r--r--   0        0        0     2963 2023-07-28 03:35:21.646600 garth-0.3.5/tests/cassettes/test_refresh_expired.yaml
--rw-r--r--   0        0        0     3080 2023-07-28 12:57:32.501754 garth-0.3.5/tests/conftest.py
--rw-r--r--   0        0        0     8524 2023-07-30 01:16:56.595924 garth-0.3.5/tests/resources/cassettes/test_daily_hrv.yaml
--rw-r--r--   0        0        0     4197 2023-07-29 23:34:06.394173 garth-0.3.5/tests/resources/cassettes/test_daily_intensity_minutes.yaml
--rw-r--r--   0        0        0     3098 2023-07-28 03:35:40.317256 garth-0.3.5/tests/resources/cassettes/test_daily_sleep.yaml
--rw-r--r--   0        0        0     4179 2023-07-29 17:52:20.398786 garth-0.3.5/tests/resources/cassettes/test_daily_steps.yaml
--rw-r--r--   0        0        0     6252 2023-07-28 03:35:40.317752 garth-0.3.5/tests/resources/cassettes/test_daily_stress.yaml
--rw-r--r--   0        0        0    44427 2023-07-28 03:35:40.318411 garth-0.3.5/tests/resources/cassettes/test_daily_stress_pagination.yaml
--rw-r--r--   0        0        0     3652 2023-07-28 12:21:13.363000 garth-0.3.5/tests/resources/cassettes/test_sleep_data_get.yaml
--rw-r--r--   0        0        0    77468 2023-07-28 12:22:31.103002 garth-0.3.5/tests/resources/cassettes/test_sleep_data_list.yaml
--rw-r--r--   0        0        0     3349 2023-07-29 23:35:28.845204 garth-0.3.5/tests/resources/cassettes/test_weekly_intensity_minutes.yaml
--rw-r--r--   0        0        0    13052 2023-07-29 17:52:45.776274 garth-0.3.5/tests/resources/cassettes/test_weekly_steps.yaml
--rw-r--r--   0        0        0     4717 2023-07-28 03:35:40.318832 garth-0.3.5/tests/resources/cassettes/test_weekly_stress.yaml
--rw-r--r--   0        0        0    16221 2023-07-28 03:35:40.319518 garth-0.3.5/tests/resources/cassettes/test_weekly_stress_beyond_data.yaml
--rw-r--r--   0        0        0     7522 2023-07-28 03:35:40.320026 garth-0.3.5/tests/resources/cassettes/test_weekly_stress_pagination.yaml
--rw-r--r--   0        0        0      346 2023-07-30 01:22:47.002975 garth-0.3.5/tests/resources/test_hrv.py
--rw-r--r--   0        0        0      748 2023-07-29 23:40:27.912636 garth-0.3.5/tests/resources/test_intensity_minutes.py
--rw-r--r--   0        0        0      849 2023-07-28 12:22:22.098284 garth-0.3.5/tests/resources/test_sleep.py
--rw-r--r--   0        0        0      667 2023-07-29 17:53:35.423973 garth-0.3.5/tests/resources/test_steps.py
--rw-r--r--   0        0        0     1437 2023-07-27 13:31:20.424008 garth-0.3.5/tests/resources/test_stress.py
--rw-r--r--   0        0        0     1808 2023-07-23 13:40:52.098938 garth-0.3.5/tests/test_auth_token.py
--rw-r--r--   0        0        0     4102 2023-07-30 02:36:22.827788 garth-0.3.5/tests/test_http.py
--rw-r--r--   0        0        0     2570 2023-07-28 12:10:36.895963 garth-0.3.5/tests/test_sso.py
--rw-r--r--   0        0        0      531 2023-07-27 13:16:10.645234 garth-0.3.5/tests/test_utils.py
--rw-r--r--   0        0        0    13738 1970-01-01 00:00:00.000000 garth-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-20 12:44:00.130760 garth-0.4.0/LICENSE
+-rw-r--r--   0        0        0    13332 2023-08-01 00:53:50.423067 garth-0.4.0/README.md
+-rw-r--r--   0        0        0      679 2023-08-01 00:53:18.694307 garth-0.4.0/garth/__init__.py
+-rw-r--r--   0        0        0      734 2023-08-04 01:10:15.046660 garth-0.4.0/garth/auth_tokens.py
+-rw-r--r--   0        0        0      145 2023-07-18 22:32:58.010661 garth-0.4.0/garth/exc.py
+-rw-r--r--   0        0        0     4922 2023-08-04 04:12:36.576282 garth-0.4.0/garth/http.py
+-rw-r--r--   0        0        0        0 2023-07-27 13:16:10.642595 garth-0.4.0/garth/py.typed
+-rw-r--r--   0        0        0     4656 2023-08-04 04:07:53.677094 garth-0.4.0/garth/sso.py
+-rw-r--r--   0        0        0      434 2023-07-30 01:10:27.575730 garth-0.4.0/garth/stats/__init__.py
+-rw-r--r--   0        0        0     1531 2023-08-01 00:53:16.612824 garth-0.4.0/garth/stats/_base.py
+-rw-r--r--   0        0        0     1726 2023-07-30 04:26:19.317148 garth-0.4.0/garth/stats/hrv.py
+-rw-r--r--   0        0        0      611 2023-08-01 00:53:21.402342 garth-0.4.0/garth/stats/intensity_minutes.py
+-rw-r--r--   0        0        0     3523 2023-08-01 01:10:51.104099 garth-0.4.0/garth/stats/sleep.py
+-rw-r--r--   0        0        0      653 2023-08-01 00:53:20.538257 garth-0.4.0/garth/stats/steps.py
+-rw-r--r--   0        0        0      652 2023-08-01 00:53:19.922467 garth-0.4.0/garth/stats/stress.py
+-rw-r--r--   0        0        0     1767 2023-08-04 01:10:15.047656 garth-0.4.0/garth/utils.py
+-rw-r--r--   0        0        0       22 2023-08-04 04:47:02.589550 garth-0.4.0/garth/version.py
+-rw-r--r--   0        0        0     1221 2023-08-04 04:47:08.260255 garth-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0   100792 2023-08-04 01:10:15.050440 garth-0.4.0/tests/cassettes/test_client_request.yaml
+-rw-r--r--   0        0        0     2602 2023-08-04 01:10:15.050693 garth-0.4.0/tests/cassettes/test_connectapi.yaml
+-rw-r--r--   0        0        0     3102 2023-08-04 03:43:23.879883 garth-0.4.0/tests/cassettes/test_exchange.yaml
+-rw-r--r--   0        0        0    50571 2023-08-04 01:10:15.051257 garth-0.4.0/tests/cassettes/test_login_email_password_fail.yaml
+-rw-r--r--   0        0        0    71668 2023-08-04 01:10:15.052079 garth-0.4.0/tests/cassettes/test_login_success.yaml
+-rw-r--r--   0        0        0     4883 2023-08-04 01:10:15.052284 garth-0.4.0/tests/cassettes/test_username.yaml
+-rw-r--r--   0        0        0     3692 2023-08-04 01:10:15.052523 garth-0.4.0/tests/conftest.py
+-rw-r--r--   0        0        0     8412 2023-08-04 01:10:15.052774 garth-0.4.0/tests/stats/cassettes/test_daily_hrv.yaml
+-rw-r--r--   0        0        0     1893 2023-08-04 01:10:15.052978 garth-0.4.0/tests/stats/cassettes/test_daily_hrv_no_results.yaml
+-rw-r--r--   0        0        0    16982 2023-08-04 01:10:15.053232 garth-0.4.0/tests/stats/cassettes/test_daily_hrv_paginate.yaml
+-rw-r--r--   0        0        0     1897 2023-08-04 01:10:15.053481 garth-0.4.0/tests/stats/cassettes/test_daily_hrv_paginate_no_results.yaml
+-rw-r--r--   0        0        0     3926 2023-08-04 01:10:15.053705 garth-0.4.0/tests/stats/cassettes/test_daily_intensity_minutes.yaml
+-rw-r--r--   0        0        0     2759 2023-08-04 01:10:15.053918 garth-0.4.0/tests/stats/cassettes/test_daily_sleep.yaml
+-rw-r--r--   0        0        0     4067 2023-08-04 01:10:15.054145 garth-0.4.0/tests/stats/cassettes/test_daily_steps.yaml
+-rw-r--r--   0        0        0     6085 2023-08-04 01:10:15.054397 garth-0.4.0/tests/stats/cassettes/test_daily_stress.yaml
+-rw-r--r--   0        0        0    18594 2023-08-04 01:10:15.054680 garth-0.4.0/tests/stats/cassettes/test_daily_stress_pagination.yaml
+-rw-r--r--   0        0        0     8588 2023-08-04 01:10:15.054936 garth-0.4.0/tests/stats/cassettes/test_sleep_data_get.yaml
+-rw-r--r--   0        0        0    78725 2023-08-04 01:10:15.055303 garth-0.4.0/tests/stats/cassettes/test_sleep_data_list.yaml
+-rw-r--r--   0        0        0     3259 2023-08-04 01:10:15.055564 garth-0.4.0/tests/stats/cassettes/test_weekly_intensity_minutes.yaml
+-rw-r--r--   0        0        0    12946 2023-08-04 01:10:15.055800 garth-0.4.0/tests/stats/cassettes/test_weekly_steps.yaml
+-rw-r--r--   0        0        0     4552 2023-08-04 01:10:15.056039 garth-0.4.0/tests/stats/cassettes/test_weekly_stress.yaml
+-rw-r--r--   0        0        0    15357 2023-08-04 01:10:15.056262 garth-0.4.0/tests/stats/cassettes/test_weekly_stress_beyond_data.yaml
+-rw-r--r--   0        0        0     7120 2023-08-04 01:10:15.056491 garth-0.4.0/tests/stats/cassettes/test_weekly_stress_pagination.yaml
+-rw-r--r--   0        0        0     1001 2023-07-30 04:28:17.698327 garth-0.4.0/tests/stats/test_hrv.py
+-rw-r--r--   0        0        0      748 2023-07-29 23:40:27.912636 garth-0.4.0/tests/stats/test_intensity_minutes.py
+-rw-r--r--   0        0        0      849 2023-07-28 12:22:22.098284 garth-0.4.0/tests/stats/test_sleep.py
+-rw-r--r--   0        0        0      667 2023-07-29 17:53:35.423973 garth-0.4.0/tests/stats/test_steps.py
+-rw-r--r--   0        0        0     1437 2023-07-27 13:31:20.424008 garth-0.4.0/tests/stats/test_stress.py
+-rw-r--r--   0        0        0      455 2023-08-04 01:10:15.056632 garth-0.4.0/tests/test_auth_tokens.py
+-rw-r--r--   0        0        0     3331 2023-08-04 04:13:58.627319 garth-0.4.0/tests/test_http.py
+-rw-r--r--   0        0        0     2397 2023-08-04 04:07:40.517972 garth-0.4.0/tests/test_sso.py
+-rw-r--r--   0        0        0     1655 2023-08-04 04:10:40.202147 garth-0.4.0/tests/test_utils.py
+-rw-r--r--   0        0        0    13784 1970-01-01 00:00:00.000000 garth-0.4.0/PKG-INFO
```

### Comparing `garth-0.3.5/LICENSE` & `garth-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `garth-0.3.5/README.md` & `garth-0.4.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -159,15 +159,15 @@
         "overallStressLevel": 33,
         "restStressDuration": 30960,
         "mediumStressDuration": 8760
     }
 }
 ```
 
-## Resources
+## Stats resources
 
 ### Stress
 
 Daily stress levels
 
 ```python
 DailyStress.list("2023-07-23", 2)
```

### Comparing `garth-0.3.5/garth/__init__.py` & `garth-0.4.0/garth/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from .http import client
-from .resources import (
+from .stats import (
     DailyHRV,
     DailyIntensityMinutes,
     DailySleep,
     DailySteps,
     DailyStress,
     SleepData,
     WeeklyIntensityMinutes,
```

### Comparing `garth-0.3.5/garth/auth_token.py` & `garth-0.4.0/garth/auth_tokens.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,32 @@
 import time
-from dataclasses import dataclass
+from datetime import datetime
 
-from . import sso
+from pydantic.dataclasses import dataclass
 
 
 @dataclass
-class AuthToken:
+class OAuth1Token:
+    oauth_token: str
+    oauth_token_secret: str
+    mfa_token: str
+    mfa_expiration_timestamp: datetime
+
+
+@dataclass
+class OAuth2Token:
     scope: str
     jti: str
     token_type: str
     access_token: str
     refresh_token: str
     expires_in: int
     expires_at: int
     refresh_token_expires_in: int
     refresh_token_expires_at: int
-    username: str
-
-    @classmethod
-    def login(cls, *args, **kwargs) -> "AuthToken":
-        return cls(**sso.login(*args, **kwargs))
-
-    def refresh(self, **kwargs):
-        if self.refresh_expired:
-            token = sso.exchange(**kwargs)
-        else:
-            token = sso.refresh(self.refresh_token, **kwargs)
-        self.__dict__.update(token)
 
     @property
     def expired(self):
         return self.expires_at < time.time()
 
     @property
     def refresh_expired(self):
```

### Comparing `garth-0.3.5/garth/http.py` & `garth-0.4.0/garth/http.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import json
 import os
-import pickle
-from dataclasses import asdict
 
 from requests import Response, Session
 from requests.adapters import HTTPAdapter, Retry
-from requests.cookies import RequestsCookieJar
 
-from .auth_token import AuthToken
+from . import sso
+from .auth_tokens import OAuth1Token, OAuth2Token
+from .utils import asdict
 
 USER_AGENT = {
     "User-Agent": (
         "Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X) "
         "AppleWebKit/605.1.15 (KHTML, like Gecko) Mobile/15E148"
     ),
 }
 
 
 class Client:
     sess: Session
     last_resp: Response
     domain: str = "garmin.com"
-    auth_token: AuthToken | None = None
+    oauth1_token: OAuth1Token | None = None
+    oauth2_token: OAuth2Token | None = None
     timeout: int = 10
     retries: int = 3
     status_forcelist: tuple[int, ...] = (408, 429, 500, 502, 503, 504)
     backoff_factor: float = 0.5
     _username: str | None = None
 
     def __init__(self, session: Session | None = None, **kwargs):
@@ -38,28 +38,28 @@
             backoff_factor=self.backoff_factor,
             **kwargs,
         )
 
     def configure(
         self,
         /,
-        auth_token: AuthToken | None = None,
-        cookies: RequestsCookieJar | None = None,
+        oauth1_token: OAuth1Token | None = None,
+        oauth2_token: OAuth2Token | None = None,
         domain: str | None = None,
         proxies: dict | None = None,
         ssl_verify: bool | None = None,
         timeout: int | None = None,
         retries: int | None = None,
         status_forcelist: tuple[int, ...] | None = None,
         backoff_factor: float | None = None,
     ):
-        if auth_token is not None:
-            self.auth_token = auth_token
-        if cookies is not None:
-            self.sess.cookies = cookies
+        if oauth1_token is not None:
+            self.oauth1_token = oauth1_token
+        if oauth2_token is not None:
+            self.oauth2_token = oauth2_token
         if domain:
             self.domain = domain
         if proxies is not None:
             self.sess.proxies.update(proxies)
         if ssl_verify is not None:
             self.sess.verify = ssl_verify
         if timeout is not None:
@@ -77,15 +77,19 @@
             backoff_factor=self.backoff_factor,
         )
         adapter = HTTPAdapter(max_retries=retry)
         self.sess.mount("https://", adapter)
 
     @property
     def username(self) -> str | None:
-        return self.auth_token.username if self.auth_token else None
+        if not self._username:
+            self._username = self.connectapi(
+                "/userprofile-service/socialProfile"
+            )["userName"]
+        return self._username
 
     def request(
         self,
         method: str,
         subdomain: str,
         path: str,
         /,
@@ -96,18 +100,15 @@
     ):
         url = f"https://{subdomain}.{self.domain}{path}"
         if referrer is True and self.last_resp:
             headers["referer"] = self.last_resp.url
         elif referrer:
             headers["referer"] = referrer
         if api:
-            if self.auth_token and self.auth_token.expired:
-                self.auth_token.refresh(client=self)
-            headers["Authorization"] = str(self.auth_token)
-            headers["di-backend"] = f"connectapi.{self.domain}"
+            headers["Authorization"] = str(self.oauth2_token)
         self.last_resp = self.sess.request(
             method,
             url,
             headers=headers,
             timeout=self.timeout,
             **kwargs,
         )
@@ -117,29 +118,37 @@
     def get(self, *args, **kwargs):
         return self.request("GET", *args, **kwargs)
 
     def post(self, *args, **kwargs):
         return self.request("POST", *args, **kwargs)
 
     def login(self, *args):
-        self.auth_token = AuthToken.login(*args, client=self)
+        self.oauth1_token, self.oauth2_token = sso.login(*args, client=self)
 
     def connectapi(self, path: str, **kwargs):
-        return self.get("connect", path, api=True, **kwargs).json()
+        resp = self.get("connectapi", path, api=True, **kwargs)
+        if resp.status_code == 204:
+            rv = None
+        else:
+            rv = resp.json()
+        return rv
 
     def dump(self, dir_path: str):
         dir_path = os.path.expanduser(dir_path)
-        with open(os.path.join(dir_path, "cookies.pickle"), "wb") as f:
-            pickle.dump(self.sess.cookies, f)
-        with open(os.path.join(dir_path, "auth_token.json"), "w") as f:
-            json.dump(asdict(self.auth_token) if self.auth_token else {}, f)
+        os.makedirs(dir_path, exist_ok=True)
+        with open(os.path.join(dir_path, "oauth1_token.json"), "w") as f:
+            if self.oauth1_token:
+                json.dump(asdict(self.oauth1_token), f, indent=4)
+        with open(os.path.join(dir_path, "oauth2_token.json"), "w") as f:
+            if self.oauth2_token:
+                json.dump(asdict(self.oauth2_token), f, indent=4)
 
     def load(self, dir_path: str):
         dir_path = os.path.expanduser(dir_path)
-        with open(os.path.join(dir_path, "cookies.pickle"), "rb") as f:
-            cookies = pickle.load(f)
-        with open(os.path.join(dir_path, "auth_token.json")) as f:
-            auth_token = AuthToken(**json.load(f))
-        self.configure(auth_token=auth_token, cookies=cookies)
+        with open(os.path.join(dir_path, "oauth1_token.json")) as f:
+            oauth1 = OAuth1Token(**json.load(f))
+        with open(os.path.join(dir_path, "oauth2_token.json")) as f:
+            oauth2 = OAuth2Token(**json.load(f))
+        self.configure(oauth1_token=oauth1, oauth2_token=oauth2)
 
 
 client = Client()
```

### Comparing `garth-0.3.5/garth/resources/hrv.py` & `garth-0.4.0/garth/stats/hrv.py`

 * *Files 27% similar despite different names*

```diff
@@ -23,23 +23,42 @@
     last_night_5_min_high: int
     baseline: HRVBaseline
     status: str
     feedback_phrase: str
     create_time_stamp: datetime
 
     _path: ClassVar[str] = "/hrv-service/hrv/daily/{start}/{end}"
+    _page_size: ClassVar[int] = 28
 
     @classmethod
     def list(
         cls,
         end: date | str | None = None,
         period: int = 28,
         *,
         client: http.Client | None = None,
     ) -> list["DailyHRV"]:
         client = client or http.client
         end = format_end_date(end)
+
+        # Paginate if period is greater than page size
+        if period > cls._page_size:
+            page = cls.list(end, cls._page_size, client=client)
+            if not page:
+                return []
+            page = (
+                cls.list(
+                    end - timedelta(days=cls._page_size),
+                    period - cls._page_size,
+                    client=client,
+                )
+                + page
+            )
+            return page
+
         start = end - timedelta(days=period - 1)
         path = cls._path.format(start=start, end=end)
         daily_hrv = client.connectapi(path)
+        if daily_hrv is None:
+            return []
         daily_hrv = camel_to_snake_dict(daily_hrv)["hrv_summaries"]
         return [cls(**hrv) for hrv in daily_hrv]
```

### Comparing `garth-0.3.5/garth/resources/intensity_minutes.py` & `garth-0.4.0/garth/stats/intensity_minutes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import ClassVar
 
 from pydantic.dataclasses import dataclass
 
-from ..stats import Stats
+from ._base import Stats
 
 BASE_PATH = "/usersummary-service/stats/im"
 
 
 @dataclass(frozen=True)
 class DailyIntensityMinutes(Stats):
     weekly_goal: int
```

### Comparing `garth-0.3.5/garth/resources/sleep.py` & `garth-0.4.0/garth/stats/sleep.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from datetime import date, datetime
 from typing import ClassVar, Optional
 
 from pydantic.dataclasses import dataclass
 
 from .. import http
-from ..stats import Stats
 from ..utils import camel_to_snake_dict, date_range, format_end_date
+from ._base import Stats
 
 
 @dataclass(frozen=True)
 class DailySleep(Stats):
     value: int
 
     _path: ClassVar[
```

### Comparing `garth-0.3.5/garth/resources/steps.py` & `garth-0.4.0/garth/stats/steps.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import ClassVar
 
 from pydantic.dataclasses import dataclass
 
-from ..stats import Stats
+from ._base import Stats
 
 BASE_PATH = "/usersummary-service/stats/steps"
 
 
 @dataclass(frozen=True)
 class DailySteps(Stats):
     total_steps: int
```

### Comparing `garth-0.3.5/garth/resources/stress.py` & `garth-0.4.0/garth/stats/stress.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import ClassVar
 
 from pydantic.dataclasses import dataclass
 
-from ..stats import Stats
+from ._base import Stats
 
 BASE_PATH = "/usersummary-service/stats/stress"
 
 
 @dataclass(frozen=True)
 class DailyStress(Stats):
     overall_stress_level: int
```

### Comparing `garth-0.3.5/garth/stats.py` & `garth-0.4.0/garth/stats/_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from datetime import date, timedelta
 from typing import ClassVar
 
 from pydantic.dataclasses import dataclass
 
-from . import http
-from .utils import camel_to_snake_dict, format_end_date
+from .. import http
+from ..utils import camel_to_snake_dict, format_end_date
 
 BASE_PATH = "/usersummary-service/stats/stress"
 
 
 @dataclass(frozen=True)
 class Stats:
     calendar_date: date
```

### Comparing `garth-0.3.5/garth/utils.py` & `garth-0.4.0/garth/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+import dataclasses
 import re
-from datetime import date, timedelta
+import typing
+from datetime import date, datetime, timedelta
 from typing import Any
 
 CAMEL_TO_SNAKE = re.compile(
     r"((?<=[a-z0-9])[A-Z]|(?!^)[A-Z](?=[a-z])|(?<=[a-zA-Z])[0-9])"
 )
 
 
@@ -39,7 +41,24 @@
     return end
 
 
 def date_range(date_: date | str, days: int):
     date_ = date_ if isinstance(date_, date) else date.fromisoformat(date_)
     for day in range(days):
         yield date_ - timedelta(days=day)
+
+
+def asdict(obj):
+    if dataclasses.is_dataclass(obj):
+        result = {}
+        for field in dataclasses.fields(obj):
+            value = getattr(obj, field.name)
+            result[field.name] = asdict(value)
+        return result
+
+    if isinstance(obj, typing.List):
+        return [asdict(v) for v in obj]
+
+    if isinstance(obj, (datetime, date)):
+        return obj.isoformat()
+
+    return obj
```

### Comparing `garth-0.3.5/pyproject.toml` & `garth-0.4.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -4,39 +4,43 @@
 description = "Garmin SSO auth + Connect client"
 authors = [
     { name = "Matin Tamizi", email = "mtamizi@duck.com" },
 ]
 dependencies = [
     "requests",
     "pydantic",
+    "requests-oauthlib>=1.3.1",
 ]
 requires-python = ">=3.10"
 readme = "README.md"
 classifiers = [
     "Operating System :: MacOS :: MacOS X",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: POSIX :: Linux",
 ]
 packages = [
     { include = "garth" },
 ]
-version = "0.3.5"
+version = "0.4.0"
 
 [project.license]
 text = "MIT"
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [tool.pytest.ini_options]
 addopts = "--ignore=__pypackages__ --ignore-glob=*.yaml"
 
+[tool.mypy]
+ignore_missing_imports = true
+
 [tool.isort]
 multi_line_output = 3
 include_trailing_comma = true
 force_grid_wrap = 0
 use_parentheses = true
 line_length = 79
 known_first_party = "garth"
```

### Comparing `garth-0.3.5/tests/cassettes/test_client_request.yaml` & `garth-0.4.0/tests/cassettes/test_client_request.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -296,15 +296,15 @@
         title=\"Connect\" href=\"/\"></a></h1><div class=\"c0123\"></div></header><main
         class=\"c0113 c0115\"><div class=\"c011\"><div class=\"c012\"><div></div><div></div><div
         class=\"c013\"><div><a class=\"c0133 c0132\" href=\"https://play.google.com/store/apps/details?id=com.garmin.android.apps.connectmobile\"
         title=\"Garmin Connect Mobile\" target=\"play_store\"></a></div><div><a class=\"c0135
         c0132\" href=\"https://itunes.apple.com/us/app/garmin-connect-mobile/id583446403?mt=8&amp;amp;uo=4\"
         title=\"Garmin Connect Mobile\" target=\"itunes_store\"></a></div></div></div><div
         class=\"c014\"><script type=\"text/javascript\" style=\"display:none\">\n//<![CDATA[\nwindow.__mirage2
-        = {petok:\"V9h.0isjHs2kr_LmLrW.hUFt5mTB3VynL.2ppatrpEU-1800-0\"};\n//]]>\n</script>\n<script
+        = {petok:\"y6pOYB4GoEuWpWlDYMol.kVrhYUDaf6dHn8FxaoQHM8-1800-0\"};\n//]]>\n</script>\n<script
         type=\"text/javascript\" src=\"https://ajax.cloudflare.com/cdn-cgi/scripts/04b3eb47/cloudflare-static/mirage2.min.js\"></script>\n<img
         data-cfsrc=\"/static/screen-phone-myday-717fec02a4d8eea2690241774363b357.png\"
         class=\"c017\" alt=\"\" style=\"display:none;visibility:hidden;\" /><noscript><img
         src=\"/static/screen-phone-myday-717fec02a4d8eea2690241774363b357.png\" class=\"c017\"
         alt=\"\"/></noscript></div><div class=\"c015\"><div><a href=\"#exploreSection\"><p></p><div
         class=\"c016\"></div></a></div></div></div></main><aside><div id=\"exploreSection\"
         class=\"c018\"><div> </div><div><img src=\"data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0iVVRGLTgiPz4KPHN2ZyB3aWR0aD0iNDJweCIgaGVpZ2h0PSI3NHB4IiB2aWV3Qm94PSIwIDAgNDIgNzQiIHZlcnNpb249IjEuMSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIiB4bWxuczp4bGluaz0iaHR0cDovL3d3dy53My5vcmcvMTk5OS94bGluayI+CiAgICA8IS0tIEdlbmVyYXRvcjogU2tldGNoIDUzLjEgKDcyNjMxKSAtIGh0dHBzOi8vc2tldGNoYXBwLmNvbSAtLT4KICAgIDx0aXRsZT5pY29uLXBob25lPC90aXRsZT4KICAgIDxkZXNjPkNyZWF0ZWQgd2l0aCBTa2V0Y2guPC9kZXNjPgogICAgPGcgaWQ9Imljb24tcGhvbmUiIHN0cm9rZT0ibm9uZSIgc3Ryb2tlLXdpZHRoPSIxIiBmaWxsPSJub25lIiBmaWxsLXJ1bGU9ImV2ZW5vZGQiPgogICAgICAgIDxwYXRoIGQ9Ik0yLjA1ODgyMzUzLDYuNTE1OTU1MTEgTDM5Ljk0MTE3NjUsNi41MTU5NTUxMSBMMzkuOTQxMTc2NSwzLjAzMjc4Njg5IEMzOS45NDExNzY1LDIuNDc1NTYyODQgMzkuNDc5NTg4MiwyLjAyMTg1NzkyIDM4LjkxMTc2NDcsMi4wMjE4NTc5MiBMMy4wODgyMzUyOSwyLjAyMTg1NzkyIEMyLjUyMDQxMTc2LDIuMDIxODU3OTIgMi4wNTg4MjM1MywyLjQ3NTU2Mjg0IDIuMDU4ODIzNTMsMy4wMzI3ODY4OSBMMi4wNTg4MjM1Myw2LjUxNTk1NTExIFogTTIuMDU4ODIzNTMsNjcuNzgwOTYxNCBMMi4wNTg4MjM1Myw3MC45NjcyMTMxIEMyLjA1ODgyMzUzLDcxLjUyNDQzNzIgMi41MjA0MTE3Niw3MS45NzgxNDIxIDMuMDg4MjM1MjksNzEuOTc4MTQyMSBMMzguOTExNzY0Nyw3MS45NzgxNDIxIEMzOS40Nzk1ODgyLDcxLjk3ODE0MjEgMzkuOTQxMTc2NSw3MS41MjQ0MzcyIDM5Ljk0MTE3NjUsNzAuOTY3MjEzMSBMMzkuOTQxMTc2NSw2Ny43ODA5NjE0IEwyLjA1ODgyMzUzLDY3Ljc4MDk2MTQgWiBNMzguOTExNzY0Nyw3NCBMMy4wODgyMzUyOSw3NCBDMS4zODUxNzY0Nyw3NCAwLDcyLjYzOTY5NCAwLDcwLjk2NzIxMzEgTDAsMy4wMzI3ODY4OSBDMCwxLjM2MDMwNjAxIDEuMzg1MTc2NDcsMCAzLjA4ODIzNTI5LDAgTDM4LjkxMTc2NDcsMCBDNDAuNjE0ODIzNSwwIDQyLDEuMzYwMzA2MDEgNDIsMy4wMzI3ODY4OSBMNDIsNzAuOTY3MjEzMSBDNDIsNzIuNjM5Njk0IDQwLjYxNDgyMzUsNzQgMzguOTExNzY0Nyw3NCBaIE04LjA1NTk1NjIzLDEzLjc4OTY4NDUgQzcuNDg5Mjk0NzYsMTMuNzg5Njg0NSA3LjAyODY1MTE3LDE0LjI0MzA4MDMgNy4wMjg2NTExNywxNC43OTk5MjQ3IEw3LjAyODY1MTE3LDE2Ljk3ODAwMjYgQzcuMDI4NjUxMTcsMTcuNTM1MjUxIDcuNDg5Mjk0NzYsMTcuOTg4MjQyNyA4LjA1NTk1NjIzLDE3Ljk4ODI0MjcgTDEwLjI3MTIzNjksMTcuOTg4MjQyNyBDMTAuODM3ODk4MywxNy45ODgyNDI3IDExLjI5ODU0MTksMTcuNTM1MjUxIDExLjI5ODU0MTksMTYuOTc4MDAyNiBMMTEuMjk4NTQxOSwxNC43OTk5MjQ3IEMxMS4yOTg1NDE5LDE0LjI0MzA4MDMgMTAuODM3ODk4MywxMy43ODk2ODQ1IDEwLjI3MTIzNjksMTMuNzg5Njg0NSBMOC4wNTU5NTYyMywxMy43ODk2ODQ1IFogTTEwLjI3MTIzNjksMjAuMDA4NzIzMSBMOC4wNTU5NTYyMywyMC4wMDg3MjMxIEM2LjM1NjM4Mjc0LDIwLjAwODcyMzEgNC45NzQwNDEwNSwxOC42NDkzNDM5IDQuOTc0MDQxMDUsMTYuOTc4MDAyNiBMNC45NzQwNDEwNSwxNC43OTk5MjQ3IEM0Ljk3NDA0MTA1LDEzLjEyODU4MzMgNi4zNTYzODI3NCwxMS43NjkyMDQxIDguMDU1OTU2MjMsMTEuNzY5MjA0MSBMMTAuMjcxMjM2OSwxMS43NjkyMDQxIEMxMS45NzAzOTk0LDExLjc2OTIwNDEgMTMuMzUzMTUyLDEzLjEyODU4MzMgMTMuMzUzMTUyLDE0Ljc5OTkyNDcgTDEzLjM1MzE1MiwxNi45NzgwMDI2IEMxMy4zNTMxNTIsMTguNjQ5MzQzOSAxMS45NzAzOTk0LDIwLjAwODcyMzEgMTAuMjcxMjM2OSwyMC4wMDg3MjMxIFogTTE5Ljk3MjY5NDksMTMuNzg5Njg0NSBDMTkuNDA2MDMzNSwxMy43ODk2ODQ1IDE4Ljk0NTM4OTksMTQuMjQzMDgwMyAxOC45NDUzODk5LDE0Ljc5OTkyNDcgTDE4Ljk0NTM4OTksMTYuOTc4MDAyNiBDMTguOTQ1Mzg5OSwxNy41MzUyNTEgMTkuNDA2MDMzNSwxNy45ODgyNDI3IDE5Ljk3MjY5NDksMTcuOTg4MjQyNyBMMjIuMTg3NTY0NywxNy45ODgyNDI3IEMyMi43NTQyMjYxLDE3Ljk4ODI0MjcgMjMuMjE0ODY5NywxNy41MzUyNTEgMjMuMjE0ODY5NywxNi45NzgwMDI2IEwyMy4yMTQ4Njk3LDE0Ljc5OTkyNDcgQzIzLjIxNDg2OTcsMTQuMjQzMDgwMyAyMi43NTQyMjYxLDEzLjc4OTY4NDUgMjIuMTg3NTY0NywxMy43ODk2ODQ1IEwxOS45NzI2OTQ5LDEzLjc4OTY4NDUgWiBNMjIuMTg3NTY0NywyMC4wMDg3MjMxIEwxOS45NzI2OTQ5LDIwLjAwODcyMzEgQzE4LjI3MzEyMTQsMjAuMDA4NzIzMSAxNi44OTA3Nzk4LDE4LjY0OTM0MzkgMTYuODkwNzc5OCwxNi45NzgwMDI2IEwxNi44OTA3Nzk4LDE0Ljc5OTkyNDcgQzE2Ljg5MDc3OTgsMTMuMTI4NTgzMyAxOC4yNzMxMjE0LDExLjc2OTIwNDEgMTkuOTcyNjk0OSwxMS43NjkyMDQxIEwyMi4xODc1NjQ3LDExLjc2OTIwNDEgQzIzLjg4NjcyNzIsMTEuNzY5MjA0MSAyNS4yNjk0Nzk4LDEzLjEyODU4MzMgMjUuMjY5NDc5OCwxNC43OTk5MjQ3IEwyNS4yNjk0Nzk4LDE2Ljk3ODAwMjYgQzI1LjI2OTQ3OTgsMTguNjQ5MzQzOSAyMy44ODY3MjcyLDIwLjAwODcyMzEgMjIuMTg3NTY0NywyMC4wMDg3MjMxIFogTTMxLjQ3ODUxMTYsMTMuNzg5Njg0NSBDMzAuOTExODUwMiwxMy43ODk2ODQ1IDMwLjQ1MTIwNjYsMTQuMjQzMDgwMyAzMC40NTEyMDY2LDE0Ljc5OTkyNDcgTDMwLjQ1MTIwNjYsMTYuOTc4MDAyNiBDMzAuNDUxMjA2NiwxNy41MzUyNTEgMzAuOTExODUwMiwxNy45ODgyNDI3IDMxLjQ3ODUxMTYsMTcuOTg4MjQyNyBMMzMuNjkzMzgxMywxNy45ODgyNDI3IEMzNC4yNjAwNDI4LDE3Ljk4ODI0MjcgMzQuNzIwNjg2NCwxNy41MzUyNTEgMzQuNzIwNjg2NCwxNi45NzgwMDI2IEwzNC43MjA2ODY0LDE0Ljc5OTkyNDcgQzM0LjcyMDY4NjQsMTQuMjQzMDgwMyAzNC4yNjAwNDI4LDEzLjc4OTY4NDUgMzMuNjkzMzgxMywxMy43ODk2ODQ1IEwzMS40Nzg1MTE2LDEzLjc4OTY4NDUgWiBNMzMuNjkzMzgxMywyMC4wMDg3MjMxIEwzMS40Nzg1MTE2LDIwLjAwODcyMzEgQzI5Ljc3ODkzODEsMjAuMDA4NzIzMSAyOC4zOTY1OTY0LDE4LjY0OTM0MzkgMjguMzk2NTk2NCwxNi45NzgwMDI2IEwyOC4zOTY1OTY0LDE0Ljc5OTkyNDcgQzI4LjM5NjU5NjQsMTMuMTI4NTgzMyAyOS43Nzg5MzgxLDExLjc2OTIwNDEgMzEuNDc4NTExNiwxMS43NjkyMDQxIEwzMy42OTMzODEzLDExLjc2OTIwNDEgQzM1LjM5MjU0MzksMTEuNzY5MjA0MSAzNi43NzUyOTY1LDEzLjEyODU4MzMgMzYuNzc1Mjk2NSwxNC43OTk5MjQ3IEwzNi43NzUyOTY1LDE2Ljk3ODAwMjYgQzM2Ljc3NTI5NjUsMTguNjQ5MzQzOSAzNS4zOTI1NDM5LDIwLjAwODcyMzEgMzMuNjkzMzgxMywyMC4wMDg3MjMxIFogTTguMDU1OTU2MjMsMjUuMTA0Mzc0NyBDNy40ODkyOTQ3NiwyNS4xMDQzNzQ3IDcuMDI4NjUxMTcsMjUuNTU3NzcwNSA3LjAyODY1MTE3LDI2LjExNDYxNDkgTDcuMDI4NjUxMTcsMjguMjkyNjkyNyBDNy4wMjg2NTExNywyOC44NDk5NDEyIDcuNDg5Mjk0NzYsMjkuMzAyOTMyOSA4LjA1NTk1NjIzLDI5LjMwMjkzMjkgTDEwLjI3MTIzNjksMjkuMzAyOTMyOSBDMTAuODM3ODk4MywyOS4zMDI5MzI5IDExLjI5ODU0MTksMjguODQ5OTQxMiAxMS4yOTg1NDE5LDI4LjI5MjY5MjcgTDExLjI5ODU0MTksMjYuMTE0NjE0OSBDMTEuMjk4NTQxOSwyNS41NTc3NzA1IDEwLjgzNzg5ODMsMjUuMTA0Mzc0NyAxMC4yNzEyMzY5LDI1LjEwNDM3NDcgTDguMDU1OTU2MjMsMjUuMTA0Mzc0NyBaIE0xMC4yNzEyMzY5LDMxLjMyMzQxMzMgTDguMDU1OTU2MjMsMzEuMzIzNDEzMyBDNi4zNTYzODI3NCwzMS4zMjM0MTMzIDQuOTc0MDQxMDUsMjkuOTY0MDM0MSA0Ljk3NDA0MTA1LDI4LjI5MjY5MjcgTDQuOTc0MDQxMDUsMjYuMTE0NjE0OSBDNC45NzQwNDEwNSwyNC40NDMyNzM1IDYuMzU2MzgyNzQsMjMuMDgzODk0MyA4LjA1NTk1NjIzLDIzLjA4Mzg5NDMgTDEwLjI3MTIzNjksMjMuMDgzODk0MyBDMTEuOTcwMzk5NCwyMy4wODM4OTQzIDEzLjM1MzE1MiwyNC40NDMyNzM1IDEzLjM1MzE1MiwyNi4xMTQ2MTQ5IEwxMy4zNTMxNTIsMjguMjkyNjkyNyBDMTMuMzUzMTUyLDI5Ljk2NDAzNDEgMTEuOTcwMzk5NCwzMS4zMjM0MTMzIDEwLjI3MTIzNjksMzEuMzIzNDEzMyBaIE0xOS45NzI2OTQ5LDI1LjEwNDM3NDcgQzE5LjQwNjAzMzUsMjUuMTA0Mzc0NyAxOC45NDUzODk5LDI1LjU1Nzc3MDUgMTguOTQ1Mzg5OSwyNi4xMTQ2MTQ5IEwxOC45NDUzODk5LDI4LjI5MjY5MjcgQzE4Ljk0NTM4OTksMjguODQ5OTQxMiAxOS40MDYwMzM1LDI5LjMwMjkzMjkgMTkuOTcyNjk0OSwyOS4zMDI5MzI5IEwyMi4xODc1NjQ3LDI5LjMwMjkzMjkgQzIyLjc1NDIyNjEsMjkuMzAyOTMyOSAyMy4yMTQ4Njk3LDI4Ljg0OTk0MTIgMjMuMjE0ODY5NywyOC4yOTI2OTI3IEwyMy4yMTQ4Njk3LDI2LjExNDYxNDkgQzIzLjIxNDg2OTcsMjUuNTU3NzcwNSAyMi43NTQyMjYxLDI1LjEwNDM3NDcgMjIuMTg3NTY0NywyNS4xMDQzNzQ3IEwxOS45NzI2OTQ5LDI1LjEwNDM3NDcgWiBNMjIuMTg3NTY0NywzMS4zMjM0MTMzIEwxOS45NzI2OTQ5LDMxLjMyMzQxMzMgQzE4LjI3MzEyMTQsMzEuMzIzNDEzMyAxNi44OTA3Nzk4LDI5Ljk2NDAzNDEgMTYuODkwNzc5OCwyOC4yOTI2OTI3IEwxNi44OTA3Nzk4LDI2LjExNDYxNDkgQzE2Ljg5MDc3OTgsMjQuNDQzMjczNSAxOC4yNzMxMjE0LDIzLjA4Mzg5NDMgMTkuOTcyNjk0OSwyMy4wODM4OTQzIEwyMi4xODc1NjQ3LDIzLjA4Mzg5NDMgQzIzLjg4NjcyNzIsMjMuMDgzODk0MyAyNS4yNjk0Nzk4LDI0LjQ0MzI3MzUgMjUuMjY5NDc5OCwyNi4xMTQ2MTQ5IEwyNS4yNjk0Nzk4LDI4LjI5MjY5MjcgQzI1LjI2OTQ3OTgsMjkuOTY0MDM0MSAyMy44ODY3MjcyLDMxLjMyMzQxMzMgMjIuMTg3NTY0NywzMS4zMjM0MTMzIFogTTMxLjQ3ODUxMTYsMjUuMTA0Mzc0NyBDMzAuOTExODUwMiwyNS4xMDQzNzQ3IDMwLjQ1MTIwNjYsMjUuNTU3NzcwNSAzMC40NTEyMDY2LDI2LjExNDYxNDkgTDMwLjQ1MTIwNjYsMjguMjkyNjkyNyBDMzAuNDUxMjA2NiwyOC44NDk5NDEyIDMwLjkxMTg1MDIsMjkuMzAyOTMyOSAzMS40Nzg1MTE2LDI5LjMwMjkzMjkgTDMzLjY5MzM4MTMsMjkuMzAyOTMyOSBDMzQuMjYwMDQyOCwyOS4zMDI5MzI5IDM0LjcyMDY4NjQsMjguODQ5OTQxMiAzNC43MjA2ODY0LDI4LjI5MjY5MjcgTDM0LjcyMDY4NjQsMjYuMTE0NjE0OSBDMzQuNzIwNjg2NCwyNS41NTc3NzA1IDM0LjI2MDA0MjgsMjUuMTA0Mzc0NyAzMy42OTMzODEzLDI1LjEwNDM3NDcgTDMxLjQ3ODUxMTYsMjUuMTA0Mzc0NyBaIE0zMy42OTMzODEzLDMxLjMyMzQxMzMgTDMxLjQ3ODUxMTYsMzEuMzIzNDEzMyBDMjkuNzc4OTM4MSwzMS4zMjM0MTMzIDI4LjM5NjU5NjQsMjkuOTY0MDM0MSAyOC4zOTY1OTY0LDI4LjI5MjY5MjcgTDI4LjM5NjU5NjQsMjYuMTE0NjE0OSBDMjguMzk2NTk2NCwyNC40NDMyNzM1IDI5Ljc3ODkzODEsMjMuMDgzODk0MyAzMS40Nzg1MTE2LDIzLjA4Mzg5NDMgTDMzLjY5MzM4MTMsMjMuMDgzODk0MyBDMzUuMzkyNTQzOSwyMy4wODM4OTQzIDM2Ljc3NTI5NjUsMjQuNDQzMjczNSAzNi43NzUyOTY1LDI2LjExNDYxNDkgTDM2Ljc3NTI5NjUsMjguMjkyNjkyNyBDMzYuNzc1Mjk2NSwyOS45NjQwMzQxIDM1LjM5MjU0MzksMzEuMzIzNDEzMyAzMy42OTMzODEzLDMxLjMyMzQxMzMgWiBNOC4wNTU5NTYyMywzNi40MTkwNjQ4IEM3LjQ4OTI5NDc2LDM2LjQxOTA2NDggNy4wMjg2NTExNywzNi44NzI0NjA2IDcuMDI4NjUxMTcsMzcuNDI5MzA1IEw3LjAyODY1MTE3LDM5LjYwNzM4MjkgQzcuMDI4NjUxMTcsNDAuMTY0NjMxNCA3LjQ4OTI5NDc2LDQwLjYxNzYyMzEgOC4wNTU5NTYyMyw0MC42MTc2MjMxIEwxMC4yNzEyMzY5LDQwLjYxNzYyMzEgQzEwLjgzNzg5ODMsNDAuNjE3NjIzMSAxMS4yOTg1NDE5LDQwLjE2NDYzMTQgMTEuMjk4NTQxOSwzOS42MDczODI5IEwxMS4yOTg1NDE5LDM3LjQyOTMwNSBDMTEuMjk4NTQxOSwzNi44NzI0NjA2IDEwLjgzNzg5ODMsMzYuNDE5MDY0OCAxMC4yNzEyMzY5LDM2LjQxOTA2NDggTDguMDU1OTU2MjMsMzYuNDE5MDY0OCBaIE0xMC4yNzEyMzY5LDQyLjYzODEwMzUgTDguMDU1OTU2MjMsNDIuNjM4MTAzNSBDNi4zNTYzODI3NCw0Mi42MzgxMDM1IDQuOTc0MDQxMDUsNDEuMjc4NzI0MiA0Ljk3NDA0MTA1LDM5LjYwNzM4MjkgTDQuOTc0MDQxMDUsMzcuNDI5MzA1IEM0Ljk3NDA0MTA1LDM1Ljc1Nzk2MzYgNi4zNTYzODI3NCwzNC4zOTg1ODQ0IDguMDU1OTU2MjMsMzQuMzk4NTg0NCBMMTAuMjcxMjM2OSwzNC4zOTg1ODQ0IEMxMS45NzAzOTk0LDM0LjM5ODU4NDQgMTMuMzUzMTUyLDM1Ljc1Nzk2MzYgMTMuMzUzMTUyLDM3LjQyOTMwNSBMMTMuMzUzMTUyLDM5LjYwNzM4MjkgQzEzLjM1MzE1Miw0MS4yNzg3MjQyIDExLjk3MDM5OTQsNDIuNjM4MTAzNSAxMC4yNzEyMzY5LDQyLjYzODEwMzUgWiBNMTkuOTcyNjk0OSwzNi40MTkwNjQ4IEMxOS40MDYwMzM1LDM2LjQxOTA2NDggMTguOTQ1Mzg5OSwzNi44NzI0NjA2IDE4Ljk0NTM4OTksMzcuNDI5MzA1IEwxOC45NDUzODk5LDM5LjYwNzM4MjkgQzE4Ljk0NTM4OTksNDAuMTY0NjMxNCAxOS40MDYwMzM1LDQwLjYxNzYyMzEgMTkuOTcyNjk0OSw0MC42MTc2MjMxIEwyMi4xODc1NjQ3LDQwLjYxNzYyMzEgQzIyLjc1NDIyNjEsNDAuNjE3NjIzMSAyMy4yMTQ4Njk3LDQwLjE2NDYzMTQgMjMuMjE0ODY5NywzOS42MDczODI5IEwyMy4yMTQ4Njk3LDM3LjQyOTMwNSBDMjMuMjE0ODY5NywzNi44NzI0NjA2IDIyLjc1NDIyNjEsMzYuNDE5MDY0OCAyMi4xODc1NjQ3LDM2LjQxOTA2NDggTDE5Ljk3MjY5NDksMzYuNDE5MDY0OCBaIE0yMi4xODc1NjQ3LDQyLjYzODEwMzUgTDE5Ljk3MjY5NDksNDIuNjM4MTAzNSBDMTguMjczMTIxNCw0Mi42MzgxMDM1IDE2Ljg5MDc3OTgsNDEuMjc4NzI0MiAxNi44OTA3Nzk4LDM5LjYwNzM4MjkgTDE2Ljg5MDc3OTgsMzcuNDI5MzA1IEMxNi44OTA3Nzk4LDM1Ljc1Nzk2MzYgMTguMjczMTIxNCwzNC4zOTg1ODQ0IDE5Ljk3MjY5NDksMzQuMzk4NTg0NCBMMjIuMTg3NTY0NywzNC4zOTg1ODQ0IEMyMy44ODY3MjcyLDM0LjM5ODU4NDQgMjUuMjY5NDc5OCwzNS43NTc5NjM2IDI1LjI2OTQ3OTgsMzcuNDI5MzA1IEwyNS4yNjk0Nzk4LDM5LjYwNzM4MjkgQzI1LjI2OTQ3OTgsNDEuMjc4NzI0MiAyMy44ODY3MjcyLDQyLjYzODEwMzUgMjIuMTg3NTY0Nyw0Mi42MzgxMDM1IFogTTIuMDk3NTg2ODgsNjUuNzYwNDgxIEwzOS45MDI0MTMxLDY1Ljc2MDQ4MSBMMzkuOTAyNDEzMSw4LjUzNjgzOTU5IEwyLjA5NzU4Njg4LDguNTM2ODM5NTkgTDIuMDk3NTg2ODgsNjUuNzYwNDgxIFoiIGlkPSJDb21iaW5lZC1TaGFwZSIgZmlsbD0iI0ZGRiI+PC9wYXRoPgogICAgPC9nPgo8L3N2Zz4K\"
@@ -366,104 +366,100 @@
         src=\"/polyfill-9a6e2095c8f8c9aa1c78.js\" nomodule=\"\"></script><script src=\"/component---src-pages-index-js-848563019fe90b815f1a.js\"
         async=\"\"></script><script src=\"/c4c2febd23cefcadacb2723a138c781d9ee72589-5cefab089cea48bc2c5e.js\"
         async=\"\"></script><script src=\"/efb7dbcb2f9f0ef36ee1da515773e35807028e0c-76f1f376d84e0b0467fc.js\"
         async=\"\"></script><script src=\"/eaeed06d504ae546165ee91c3dc1e07947955f13-6dcd5ab7da14191eae89.js\"
         async=\"\"></script><script src=\"/app-949317601b74f8af13e9.js\" async=\"\"></script><script
         src=\"/styles-2ed6c2e7b748a8320e46.js\" async=\"\"></script><script src=\"/framework-f3ec01444cccc4b4057e.js\"
         async=\"\"></script><script src=\"/webpack-runtime-5df688dd07b59ccf541d.js\"
-        async=\"\"></script><script defer src=\"https://static.cloudflareinsights.com/beacon.min.js/v2cb3a2ab87c5498db5ce7e6608cf55231689030342039\"
-        integrity=\"sha512-DI3rPuZDcpH/mSGyN22erN5QFnhl760f50/te7FTIYxodEF8jJnSFnfnmG/c+osmIQemvUrnBtxnMpNdzvx1/g==\"
-        data-cf-beacon='{\"rayId\":\"7eab42d69a97b6e8\",\"version\":\"2023.4.0\",\"b\":1,\"token\":\"1bd18b8f69214e379ef7bd34509191ae\",\"si\":100}'
+        async=\"\"></script><script defer src=\"https://static.cloudflareinsights.com/beacon.min.js/v8b253dfea2ab4077af8c6f58422dfbfd1689876627854\"
+        integrity=\"sha512-bjgnUKX4azu3dLTVtie9u6TKqgx29RBwfj3QXYt5EKfWM/9hPSAI/4qcV5NACjwAo8UtTeWefx6Zq5PHcMm7Tg==\"
+        data-cf-beacon='{\"rayId\":\"7f0ee80fca96154a\",\"version\":\"2023.7.0\",\"b\":1,\"token\":\"1bd18b8f69214e379ef7bd34509191ae\",\"si\":100}'
         crossorigin=\"anonymous\"></script>\n</body></html>"
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7eab42d69a97b6e8-QRO
+      - 7f0ee80fca96154a-QRO
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - text/html; charset=UTF-8
       Date:
-      - Sat, 22 Jul 2023 11:14:37 GMT
+      - Thu, 03 Aug 2023 13:28:55 GMT
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=eGdZ5FmBzpES0Ej3Cn%2BpAGuid6j1UJnMvFUHc0Gb3heNOLv0wG5jHC2XRfiiip9S0iIjyWBh48qZCOwIXuGQud9K69y2Up4qcjjo7yV0YM0hXlZ2iXLxMsVWEmlogCD1upIPVQ%3D%3D"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=pBhM%2FFYBcODg%2FPIna39iyE9lAG%2BDKwwlec%2FLBrLJv6uI1Oh03efBEQDeNQPAgyjUSUPf96sdG75o2goOlnGkTY8%2FQpPnO5quPWlTXL9DuQP%2F2W8Yn3uECo5%2FAsbsupzUx0pbXA%3D%3D"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Set-Cookie:
-      - __cflb=02DiuJLbVZHipNWxN8xk76RcdLU1TyEEwicRTP4G4S9tY; SameSite=None; Secure;
-        path=/; expires=Sun, 23-Jul-23 10:14:37 GMT; HttpOnly
-      - _cfuvid=.KxliIcXLtxacMxq2J79PSNV1LjufvpEeDoWeyeFYKg-1690024477284-0-604800000;
-        path=/; domain=.connect.garmin.com; HttpOnly; Secure; SameSite=None
+      - __cflb=SANITIZED; SameSite=SANITIZED; Secure; path=SANITIZED; expires=SANITIZED;
+        HttpOnly
+      - _cfuvid=SANITIZED; path=SANITIZED; domain=SANITIZED; HttpOnly; Secure; SameSite=SANITIZED
       Transfer-Encoding:
       - chunked
       cache-control:
       - no-cache
       last-modified:
-      - Wed, 24 May 2023 14:23:16 GMT
+      - Wed, 24 May 2023 14:26:45 GMT
       x-frame-options:
       - deny
     status:
       code: 200
       message: OK
 - request:
     body: null
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
-      Authorization:
-      - None
       Connection:
       - keep-alive
-      Cookie:
-      - _cfuvid=.KxliIcXLtxacMxq2J79PSNV1LjufvpEeDoWeyeFYKg-1690024477284-0-604800000;
-        __cflb=02DiuJLbVZHipNWxN8xk76RcdLU1TyEEwicRTP4G4S9tY
       User-Agent:
       - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X) AppleWebKit/605.1.15
         (KHTML, like Gecko) Mobile/15E148
-      di-backend:
-      - connectapi.garmin.com
     method: GET
-    uri: https://connect.garmin.com/
+    uri: https://connectapi.garmin.com/
   response:
     body:
       string: "<html><head><meta http-equiv=\"Content-Type\" content=\"text/html;
         charset=UTF-8\"><title>Not Found</title></head>\n<body>\n    <div class=\"headerContainer\">\n
         \       <h2 class=\"page-title\">Page Not Found</h2>\n\n        <p>We're sorry.
         The page you're looking for does not exist.</p>\n    </div>\n<script defer
-        src=\"https://static.cloudflareinsights.com/beacon.min.js/v2cb3a2ab87c5498db5ce7e6608cf55231689030342039\"
-        integrity=\"sha512-DI3rPuZDcpH/mSGyN22erN5QFnhl760f50/te7FTIYxodEF8jJnSFnfnmG/c+osmIQemvUrnBtxnMpNdzvx1/g==\"
-        data-cf-beacon='{\"rayId\":\"7eab42d7ccb61556\",\"version\":\"2023.4.0\",\"b\":1,\"token\":\"1bd18b8f69214e379ef7bd34509191ae\",\"si\":100}'
+        src=\"https://static.cloudflareinsights.com/beacon.min.js/v8b253dfea2ab4077af8c6f58422dfbfd1689876627854\"
+        integrity=\"sha512-bjgnUKX4azu3dLTVtie9u6TKqgx29RBwfj3QXYt5EKfWM/9hPSAI/4qcV5NACjwAo8UtTeWefx6Zq5PHcMm7Tg==\"
+        data-cf-beacon='{\"rayId\":\"7f0ee8119bcb155f\",\"version\":\"2023.7.0\",\"b\":1,\"token\":\"dfcba71ff1d44ca3956104d931b99217\",\"si\":100}'
         crossorigin=\"anonymous\"></script>\n</body>\n</html>"
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7eab42d7ccb61556-QRO
+      - 7f0ee8119bcb155f-QRO
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - text/html
       Date:
-      - Sat, 22 Jul 2023 11:14:37 GMT
+      - Thu, 03 Aug 2023 13:28:55 GMT
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=quZV5JXfabHTtSYAxGoVYmutTxWgWC7JWUdSrp6VQ%2FSRlJE6mrw1IdalKQisPuyO7ID6xwqbvgu1jcUAqwYgFns%2BJ7IUuGAz4GTF6QD5SSa%2FQf27rWcFf5b4sznm5yBmDatwtQ%3D%3D"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=QIDnUWv2zs9Snb92gU%2BaTTvPJVmZifjxFWfJbPr3Ua7lsSIF3HLhgED53f7VE7jV9ucgR6Z9e41tBz6gqv%2Fmc4IMZ7fEvhPpMJ%2B1kz1AKfl4Ey0Gis1E5D2umJ0UbLSGo7gQ%2BjPxaw%3D%3D"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
+      Set-Cookie:
+      - _cfuvid=SANITIZED; path=SANITIZED; domain=SANITIZED; HttpOnly; Secure; SameSite=SANITIZED
       Transfer-Encoding:
       - chunked
+      alt-svc:
+      - h3=":443"; ma=86400
       cache-control:
       - no-cache
     status:
       code: 404
       message: Not Found
 version: 1
```

#### html2text {}

```diff
@@ -76,45 +76,43 @@
 Garmin Jr.
 ">
 ">
 ">
 , 0, 0);white-space:nowrap;border:0\" aria-live=\"assertive\" aria-
 atomic=\"true\">
 \n
-" headers: CF-Cache-Status: - DYNAMIC CF-RAY: - 7eab42d69a97b6e8-QRO
+" headers: CF-Cache-Status: - DYNAMIC CF-RAY: - 7f0ee80fca96154a-QRO
 Connection: - keep-alive Content-Encoding: - gzip Content-Type: - text/html;
-charset=UTF-8 Date: - Sat, 22 Jul 2023 11:14:37 GMT NEL: - '
+charset=UTF-8 Date: - Thu, 03 Aug 2023 13:28:55 GMT NEL: - '
 {"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}' Report-To: - '
 {"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/
-v3?s=eGdZ5FmBzpES0Ej3Cn%2BpAGuid6j1UJnMvFUHc0Gb3heNOLv0wG5jHC2XRfiiip9S0iIjyWBh48qZCOwIXuGQud9K69y2Up4qcjjo7yV0YM0hXlZ2iXLxMsVWEmlogCD1upIPVQ%3D%3D"}],"group":
+v3?s=pBhM%2FFYBcODg%2FPIna39iyE9lAG%2BDKwwlec%2FLBrLJv6uI1Oh03efBEQDeNQPAgyjUSUPf96sdG75o2goOlnGkTY8%2FQpPnO5quPWlTXL9DuQP%2F2W8Yn3uECo5%2FAsbsupzUx0pbXA%3D%3D"}],"group":
 "cf-nel","max_age":604800}' Server: - cloudflare Set-Cookie: -
-__cflb=02DiuJLbVZHipNWxN8xk76RcdLU1TyEEwicRTP4G4S9tY; SameSite=None; Secure;
-path=/; expires=Sun, 23-Jul-23 10:14:37 GMT; HttpOnly -
-_cfuvid=.KxliIcXLtxacMxq2J79PSNV1LjufvpEeDoWeyeFYKg-1690024477284-0-604800000;
-path=/; domain=.connect.garmin.com; HttpOnly; Secure; SameSite=None Transfer-
-Encoding: - chunked cache-control: - no-cache last-modified: - Wed, 24 May 2023
-14:23:16 GMT x-frame-options: - deny status: code: 200 message: OK - request:
-body: null headers: Accept: - '*/*' Accept-Encoding: - gzip, deflate
-Authorization: - None Connection: - keep-alive Cookie: -
-_cfuvid=.KxliIcXLtxacMxq2J79PSNV1LjufvpEeDoWeyeFYKg-1690024477284-0-604800000;
-__cflb=02DiuJLbVZHipNWxN8xk76RcdLU1TyEEwicRTP4G4S9tY User-Agent: - Mozilla/5.0
-(iPhone; CPU iPhone OS 16_5 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like
-Gecko) Mobile/15E148 di-backend: - connectapi.garmin.com method: GET uri:
-https://connect.garmin.com/ response: body: string: "
+__cflb=SANITIZED; SameSite=SANITIZED; Secure; path=SANITIZED;
+expires=SANITIZED; HttpOnly - _cfuvid=SANITIZED; path=SANITIZED;
+domain=SANITIZED; HttpOnly; Secure; SameSite=SANITIZED Transfer-Encoding: -
+chunked cache-control: - no-cache last-modified: - Wed, 24 May 2023 14:26:45
+GMT x-frame-options: - deny status: code: 200 message: OK - request: body: null
+headers: Accept: - '*/*' Accept-Encoding: - gzip, deflate Connection: - keep-
+alive User-Agent: - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X)
+AppleWebKit/605.1.15 (KHTML, like Gecko) Mobile/15E148 method: GET uri: https:/
+/connectapi.garmin.com/ response: body: string: "
 \n
 \n
 \n \
 ***** Page Not Found *****
 \n\n
 We're sorry. The page you're looking for does not exist.
 \n
 \n
 \n
 \n
-" headers: CF-Cache-Status: - DYNAMIC CF-RAY: - 7eab42d7ccb61556-QRO
+" headers: CF-Cache-Status: - DYNAMIC CF-RAY: - 7f0ee8119bcb155f-QRO
 Connection: - keep-alive Content-Encoding: - gzip Content-Type: - text/html
-Date: - Sat, 22 Jul 2023 11:14:37 GMT NEL: - '{"success_fraction":
+Date: - Thu, 03 Aug 2023 13:28:55 GMT NEL: - '{"success_fraction":
 0.01,"report_to":"cf-nel","max_age":604800}' Report-To: - '{"endpoints":[
 {"url":"https:\/\/a.nel.cloudflare.com\/report\/
-v3?s=quZV5JXfabHTtSYAxGoVYmutTxWgWC7JWUdSrp6VQ%2FSRlJE6mrw1IdalKQisPuyO7ID6xwqbvgu1jcUAqwYgFns%2BJ7IUuGAz4GTF6QD5SSa%2FQf27rWcFf5b4sznm5yBmDatwtQ%3D%3D"}],"group":
-"cf-nel","max_age":604800}' Server: - cloudflare Transfer-Encoding: - chunked
+v3?s=QIDnUWv2zs9Snb92gU%2BaTTvPJVmZifjxFWfJbPr3Ua7lsSIF3HLhgED53f7VE7jV9ucgR6Z9e41tBz6gqv%2Fmc4IMZ7fEvhPpMJ%2B1kz1AKfl4Ey0Gis1E5D2umJ0UbLSGo7gQ%2BjPxaw%3D%3D"}],"group":
+"cf-nel","max_age":604800}' Server: - cloudflare Set-Cookie: -
+_cfuvid=SANITIZED; path=SANITIZED; domain=SANITIZED; HttpOnly; Secure;
+SameSite=SANITIZED Transfer-Encoding: - chunked alt-svc: - h3=":443"; ma=86400
 cache-control: - no-cache status: code: 404 message: Not Found version: 1
```

### Comparing `garth-0.3.5/tests/cassettes/test_connectapi.yaml` & `garth-0.4.0/tests/cassettes/test_connectapi.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -6,50 +6,49 @@
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Authorization:
       - Bearer SANITIZED
       Connection:
       - keep-alive
-      Cookie:
-      - JWT_FGP=SANITIZED; _cfuvid=SANITIZED; GARMIN-SSO=SANITIZED; GARMIN-SSO-CUST-GUID=SANITIZED;
-        GARMIN-SSO-GUID=SANITIZED; GarminNoCache=SANITIZED; SESSIONID=SANITIZED; __cflb=SANITIZED
       User-Agent:
       - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X) AppleWebKit/605.1.15
         (KHTML, like Gecko) Mobile/15E148
-      di-backend:
-      - connectapi.garmin.com
+      referer:
+      - https://sso.garmin.com/sso/verifyMFA/loginEnterMfaCode?id=gauth-widget&service=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&source=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountLoginUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountCreationUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&gauthHost=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed
     method: GET
-    uri: https://connect.garmin.com/usersummary-service/stats/stress/daily/2023-07-21/2023-07-21
+    uri: https://connectapi.garmin.com/usersummary-service/stats/stress/daily/2023-07-21/2023-07-21
   response:
     body:
       string: '[{"calendarDate": "2023-07-21", "values": {"highStressDuration": 3240,
         "lowStressDuration": 20280, "overallStressLevel": 35, "restStressDuration":
         31020, "mediumStressDuration": 11640}}]'
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7eb52339ccc3b6ee-QRO
+      - 7f12d932aa00b6ee-QRO
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json
       Date:
-      - Sun, 23 Jul 2023 16:00:40 GMT
+      - Fri, 04 Aug 2023 00:57:49 GMT
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=sxGOHJpePpkk6jijH3Zgi0prd6bcRuVK08b%2Bp52sMeq%2FaJ%2FNCrU2vz%2BCwky1LR06ppa7ymWdGBLb9Uv5VDwxFrrGRJz%2BfAhPXiZTyYu2AW4%2BKX03ZUIy%2Bimf%2FKVeKNoishuwgQ%3D%3D"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=FuGLLTTuU8CV4eTRQnQ7XY0oTrHoXEaIYrPbxrkK1vRVT4yAr2Zv0YIj4D%2BZ0eQTeYgycpuCP1gSE4yk0bZE2Aj2p29AIZ2Ce%2BuOUJqB9Mp54VyHR9uEC5AAcVLUYqtzpE4YIK0Fgw%3D%3D"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Transfer-Encoding:
       - chunked
+      alt-svc:
+      - h3=":443"; ma=86400
       cache-control:
       - no-cache, no-store, private
       pragma:
       - no-cache
       set-cookie:
       - ADRUM_BTa=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
@@ -57,11 +56,12 @@
         Secure
       - SameSite=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
       - ADRUM_BT1=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
       - ADRUM_BT1=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
+      - _cfuvid=SANITIZED; path=SANITIZED; domain=SANITIZED; HttpOnly; Secure; SameSite=SANITIZED
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `garth-0.3.5/tests/cassettes/test_exchange.yaml` & `garth-0.4.0/tests/stats/cassettes/test_weekly_intensity_minutes.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -2,86 +2,76 @@
 - request:
     body: null
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
+      Authorization:
+      - Bearer SANITIZED
       Connection:
       - keep-alive
-      Content-Length:
-      - '0'
-      Cookie:
-      - JWT_FGP=SANITIZED; _cfuvid=SANITIZED; GARMIN-SSO=SANITIZED; GARMIN-SSO-CUST-GUID=SANITIZED;
-        GARMIN-SSO-GUID=SANITIZED; GarminNoCache=SANITIZED; ADRUM_BT1=SANITIZED; ADRUM_BTa=SANITIZED;
-        SESSIONID=SANITIZED; SameSite=SANITIZED; __cflb=SANITIZED
       User-Agent:
       - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X) AppleWebKit/605.1.15
         (KHTML, like Gecko) Mobile/15E148
-      referer:
-      - https://connect.garmin.com/modern
-    method: POST
-    uri: https://connect.garmin.com/modern/di-oauth/exchange
+    method: GET
+    uri: https://connectapi.garmin.com/usersummary-service/stats/im/weekly/2023-05-04/2023-07-20
   response:
     body:
-      string: '{"scope": "COMMUNITY_COURSE_READ GOLF_API_READ GHS_HID ATP_READ GHS_SAMD
-        INSIGHTS_READ COMMUNITY_COURSE_WRITE CONNECT_WRITE DIVE_SHARED_READ GHS_REGISTRATION
-        GOLF_API_WRITE INSIGHTS_WRITE PRODUCT_SEARCH_READ GOLF_SHARED_READ CONNECT_NON_SOCIAL_SHARED_READ
-        CONNECT_READ ATP_WRITE", "jti": "SANITIZED", "access_token": "SANITIZED",
-        "token_type": "Bearer", "refresh_token": "SANITIZED", "expires_in": 3599,
-        "refresh_token_expires_in": 7199}'
+      string: '[{"calendarDate": "2023-05-01", "weeklyGoal": 150, "moderateValue":
+        79, "vigorousValue": 172}, {"calendarDate": "2023-05-08", "weeklyGoal": 150,
+        "moderateValue": 94, "vigorousValue": 206}, {"calendarDate": "2023-05-15",
+        "weeklyGoal": 150, "moderateValue": 86, "vigorousValue": 120}, {"calendarDate":
+        "2023-05-22", "weeklyGoal": 150, "moderateValue": 99, "vigorousValue": 190},
+        {"calendarDate": "2023-05-29", "weeklyGoal": 150, "moderateValue": 94, "vigorousValue":
+        221}, {"calendarDate": "2023-06-05", "weeklyGoal": 150, "moderateValue": 195,
+        "vigorousValue": 103}, {"calendarDate": "2023-06-12", "weeklyGoal": 150, "moderateValue":
+        40, "vigorousValue": 73}, {"calendarDate": "2023-06-19", "weeklyGoal": 150,
+        "moderateValue": 216, "vigorousValue": 70}, {"calendarDate": "2023-06-26",
+        "weeklyGoal": 150, "moderateValue": 158, "vigorousValue": 77}, {"calendarDate":
+        "2023-07-03", "weeklyGoal": 150, "moderateValue": 177, "vigorousValue": 48},
+        {"calendarDate": "2023-07-10", "weeklyGoal": 150, "moderateValue": 185, "vigorousValue":
+        58}, {"calendarDate": "2023-07-17", "weeklyGoal": 150, "moderateValue": 103,
+        "vigorousValue": 9}]'
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7eb423c6adebb6eb-QRO
+      - 7f12d0043855b6e5-QRO
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json
       Date:
-      - Sun, 23 Jul 2023 13:06:17 GMT
+      - Fri, 04 Aug 2023 00:51:33 GMT
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=l%2FP8nOP%2BWHqKJyHI4cr2dVlIX%2BshJk8CSjTXX1NZtGk3rBbLHQY3Jo3MT32UqyZ4jB2sT04fi2CgJJfzZshZPrP7nJ%2Bz7C3d8TKU4%2FGMgaBCe8YbmYb9BuHIqIwFw%2FXQYLQGhA%3D%3D"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=%2Fd8SWt8jTX1j%2ByBa8lT%2FhYdFgj%2FLL%2Fh%2FHF%2BAAv9naauecx6nX7D0atI97wTq0Te%2FxapUS9%2FsMCkQcHZqXXfkxIlB1RCC5DO4GQjIklHkn%2Bezz4%2FRNqjC0vsX7l7Is8wrpoJDoR9gug%3D%3D"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Transfer-Encoding:
       - chunked
+      alt-svc:
+      - h3=":443"; ma=86400
       cache-control:
       - no-cache, no-store, private
       pragma:
       - no-cache
       set-cookie:
-      - ADRUM_BT1=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
-        Secure
-      - ADRUM_BTa=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
-        Secure
       - ADRUM_BTa=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
       - ADRUM_BTa=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
       - SameSite=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
       - ADRUM_BT1=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
       - ADRUM_BT1=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
-      - JWT_FGP=SANITIZED; SameSite=SANITIZED; HttpOnly; Secure; Max-Age=SANITIZED;
-        Domain=SANITIZED; Path=SANITIZED
-      strict-transport-security:
-      - max-age=31536000 ; includeSubDomains
-      x-content-type-options:
-      - nosniff
-      x-frame-options:
-      - DENY
-      x-vcap-request-id:
-      - b3da260b-a319-4682-54b1-2eb0401bb301
-      x-xss-protection:
-      - 1; mode=block
+      - _cfuvid=SANITIZED; path=SANITIZED; domain=SANITIZED; HttpOnly; Secure; SameSite=SANITIZED
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `garth-0.3.5/tests/cassettes/test_login_email_password_fail.yaml` & `garth-0.4.0/tests/cassettes/test_login_email_password_fail.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     method: GET
     uri: https://sso.garmin.com/sso/embed?id=gauth-widget&embedWidget=true&gauthHost=https%3A%2F%2Fsso.garmin.com%2Fsso
   response:
     body:
       string: "<html>\n\t<head>\n\t    <title>GAuth Embedded Version</title>\n\t    <meta
         http-equiv=\"X-UA-Compatible\" content=\"IE=edge;\" />\n\t    <style type=\"text/css\">\n\t
         \   \t#gauth-widget {border: none !important;}\n\t    </style>\n\t</head>\n\t<body>\n\t\t<script
-        type=\"text/javascript\" src=\"/sso/js/jquery/3.1.1/jquery.min.js?20210319\"></script>\n\n<div>\n\t<pre>\t<span>ERROR:
+        type=\"text/javascript\" src=\"/sso/js/jquery/3.1.1/jquery.min.js?20210319\"></script>\n\n<div>\n\t<pre>\n\t<span>ERROR:
         clientId parameter must be specified!!!</span>\n\n\t<span >Usage: https://sso.garmin.com/sso/embed?clientId=&lt;clientId&gt;&amp;locale=&lt;locale&gt;...</span>\n\n\tRequest
         parameter configuration options:\n\n\tNAME                           REQ  VALUES
         \                                                  DESCRIPTION\n\t------------------
         \            ---  -------------------------------------------------------
         \ ---------------------------------------------------------------------------------------------------\n\tclientId
         \                      Yes  \"MY_GARMIN\"/\"BUY_GARMIN\"/\"FLY_GARMIN\"/                   Client
         identifier for your web application\n\t                                    \"RMA\"/\"GarminConnect\"/\"OpenCaching\"/etc\n\tlocale
@@ -131,15 +131,15 @@
         a multi factor authentication check. (Only valid for an already logged in
         user.)\n\trememberMyBrowserShown          No  true/false (Default value is
         false)                      Whether the \"Remember My Browser\" check box
         is shown in the GAuth login widget MFA verification screen.\n\trememberMyBrowserChecked
         \       No  true/false (Default value is false)                      Whether
         the \"Remember My Browser\" check box feature is checked by default.\n\tconsentTypeIds\t\t\t\t\tNo\tconsent_types
         ids\t\t \t\t\t\t\t\t\t\t multiple consent types ids can be passed as consentTypeIds=type1&consentTypeIds=type2\n\t</pre>\n</div>\n\n\n\t<script>(function(){var
-        js = \"window['__CF$cv$params']={r:'7eabf9c8bcc61557'};_cpo=document.createElement('script');_cpo.nonce='',_cpo.src='/cdn-cgi/challenge-platform/scripts/invisible.js',document.getElementsByTagName('head')[0].appendChild(_cpo);\";var
+        js = \"window['__CF$cv$params']={r:'7f0ebee0b84eb6eb'};_cpo=document.createElement('script');_cpo.nonce='',_cpo.src='/cdn-cgi/challenge-platform/scripts/invisible.js',document.getElementsByTagName('head')[0].appendChild(_cpo);\";var
         _0xh = document.createElement('iframe');_0xh.height = 1;_0xh.width = 1;_0xh.style.position
         = 'absolute';_0xh.style.top = 0;_0xh.style.left = 0;_0xh.style.border = 'none';_0xh.style.visibility
         = 'hidden';document.body.appendChild(_0xh);function handler() {var _0xi =
         _0xh.contentDocument || _0xh.contentWindow.document;if (_0xi) {var _0xj =
         _0xi.createElement('script');_0xj.innerHTML = js;_0xi.getElementsByTagName('head')[0].appendChild(_0xj);}}if
         (document.readyState !== 'loading') {handler();} else if (window.addEventListener)
         {document.addEventListener('DOMContentLoaded', handler);} else {var prev =
@@ -155,49 +155,49 @@
       Access-Control-Allow-Methods:
       - GET,POST,OPTIONS
       Access-Control-Allow-Origin:
       - https://www.garmin.com
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7eabf9c8bcc61557-QRO
+      - 7f0ebee0b84eb6eb-QRO
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Language:
       - en
       Content-Type:
       - text/html;charset=UTF-8
       Date:
-      - Sat, 22 Jul 2023 13:19:30 GMT
+      - Thu, 03 Aug 2023 13:00:48 GMT
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=8FJAjRj7psNVxrFe0TaX%2BbEsRpVmUwS74VIBuDj9U7CW%2FjL15qkAb%2FNCGL1OFr80ZMj18Rq3ebDf3PdjOCHvcnCYN9wxZ748p5jZ3d3Jtil64mhG4VCjTxtMWuhz9Xyl"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=FYg8CIY7syHu7HGTCCZYHHCLE0JMzvFpi1TZYZ5GOc%2FtOFCtIx6lx%2B9bROv%2ByIhhGU%2BchQQgsyI%2Be5jSTj5PO8M%2B7%2Btep4vUVASUzdJhaPl2aiLOR%2BiQ58DJEvUOh872"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Set-Cookie:
       - org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED;
         Path=SANITIZED
       - __cf_bm=SANITIZED; path=SANITIZED; expires=SANITIZED; domain=SANITIZED; HttpOnly;
         Secure; SameSite=SANITIZED
       - __cflb=SANITIZED; SameSite=SANITIZED; Secure; path=SANITIZED; expires=SANITIZED;
         HttpOnly
       - _cfuvid=SANITIZED; path=SANITIZED; domain=SANITIZED; HttpOnly; Secure; SameSite=SANITIZED
       Transfer-Encoding:
       - chunked
       X-Application-Context:
-      - casServer:cloud,prod,prod-US_1102:7
+      - casServer:cloud,prod,prod-US_1102:3
       X-B3-Traceid:
-      - 3e4871c26292e7ea058dc919952a7591
+      - 539e4929d7e5643e5b31d17315b85ee7
       X-Robots-Tag:
       - noindex
       X-Vcap-Request-Id:
-      - 6ecfd42e-066f-4776-485b-387ec1f8f242
+      - df714043-a936-4659-6d80-bcdf2f3ea41d
     status:
       code: 200
       message: OK
 - request:
     body: null
     headers:
       Accept:
@@ -307,15 +307,15 @@
         \                           <label for=\"password\">Password</label>\n                            <a
         id=\"loginforgotpassword\" class=\"login-forgot-password\" style=\"cursor:pointer\">(Forgot?)</a>\n
         \                           <input type=\"password\" name=\"password\" id=\"password\"
         spellcheck=\"false\" autocorrect=\"off\" autocapitalize=\"off\" />\n                             <strong
         id=\"capslock-warning\" class=\"information\" title=\"Caps lock is on.\" style=\"display:
         none;\">Caps lock is on.</strong>\n\t\t\t\t\t    </div>\n                        <input
         type=\"hidden\" name=\"embed\" value=\"false\"/>\n                        <input
-        type=\"hidden\" name=\"_csrf\" value=\"4DE82AE827B18092410064FD04FB49A3B0667FF16BC6235CDFFCE575DE6620E9D52DCD853F8E08E0F351EFB8CFB736904772\"
+        type=\"hidden\" name=\"_csrf\" value=\"6E091072C8E5EF936879CC80F8E7E0D3A93E4D5CAD2D44240C60584EAE969BDE27C686E2A8A391B44C246D41F16CFDF9BD0A\"
         />\n                        <button type=\"submit\" id=\"login-btn-signin\"
         class=\"btn1\" accesskey=\"l\">Sign In</button>\n                        \n\n\n
         \                       <!-- The existence of the \"rememberme\" parameter
         at all will remember the user! -->\n                        \n\n                    </form>\n
         \               </div>\n                <!-- end login form -->\n\n                <!--
         begin Create Account message -->\n\t            <div id=\"login-create-account\">\n\t
         \               \n\t            </div>\n\t            <!-- end Create Account
@@ -333,15 +333,15 @@
         Otherwise focus them in the username field of the login dialog.\n                    jQuery(\"#username\").focus();\n
         \               }\n\n                // Scroll to top of iframe to fix problem
         where Firefox 3.0-3.6 browsers initially show top of iframe cutoff.\n                location.href=\"#\";\n\n
         \               if(!embedWidget){\n                \tjQuery('.createAccountLink').click(function(){\n\t
         \                   send({'openLiteBox':'createAccountLink', 'popupUrl': createAccountConfigURL,
         'popupTitle':'Create An Account', 'clientId':clientId});\n\t                });\n
         \               }\n            });\n        </script>\n    <script>(function(){var
-        js = \"window['__CF$cv$params']={r:'7eabf9c98cb0b6e8'};_cpo=document.createElement('script');_cpo.nonce='',_cpo.src='/cdn-cgi/challenge-platform/scripts/invisible.js',document.getElementsByTagName('head')[0].appendChild(_cpo);\";var
+        js = \"window['__CF$cv$params']={r:'7f0ebee1f96fb6e1'};_cpo=document.createElement('script');_cpo.nonce='',_cpo.src='/cdn-cgi/challenge-platform/scripts/invisible.js',document.getElementsByTagName('head')[0].appendChild(_cpo);\";var
         _0xh = document.createElement('iframe');_0xh.height = 1;_0xh.width = 1;_0xh.style.position
         = 'absolute';_0xh.style.top = 0;_0xh.style.left = 0;_0xh.style.border = 'none';_0xh.style.visibility
         = 'hidden';document.body.appendChild(_0xh);function handler() {var _0xi =
         _0xh.contentDocument || _0xh.contentWindow.document;if (_0xi) {var _0xj =
         _0xi.createElement('script');_0xj.innerHTML = js;_0xi.getElementsByTagName('head')[0].appendChild(_0xj);}}if
         (document.readyState !== 'loading') {handler();} else if (window.addEventListener)
         {document.addEventListener('DOMContentLoaded', handler);} else {var prev =
@@ -357,53 +357,53 @@
       Access-Control-Allow-Methods:
       - GET,POST,OPTIONS
       Access-Control-Allow-Origin:
       - https://www.garmin.com
       CF-Cache-Status:
       - DYNAMIC
       CF-Ray:
-      - 7eabf9c98cb0b6e8-QRO
+      - 7f0ebee1f96fb6e1-QRO
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Language:
       - en
       Content-Type:
       - text/html;charset=UTF-8
       Date:
-      - Sat, 22 Jul 2023 13:19:30 GMT
+      - Thu, 03 Aug 2023 13:00:48 GMT
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=tS9s5M6jGcoNaF8%2BHyacWq1ARZl51RPgATIMTQ0Ke5HvlNC5ob9jBr2OuLjDmcjlrC09s42OpMZc5xt19bdKiR6%2BTWwFQfH%2BBDCgCzLzJt9GwoDuIC%2FjzURsSSEWcIe7"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=efV6W2ZN6%2Fr0zRCn0VGftLsZ03ALs%2Be9qskgTgLh3m8%2FtlL3vmz6DefY7dixm0jmW5GaBh6fEV%2Bcqov2z6HbmfSzsjQqIUtB%2FycgXjxpVAyU0sDCY3fAYQnYuSFs5PS%2F"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Set-Cookie:
       - org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED;
         Path=SANITIZED
       - SESSION=SANITIZED; Path=SANITIZED; Secure; HttpOnly
       - __VCAP_ID__=SANITIZED; Path=SANITIZED; HttpOnly; Secure
       Transfer-Encoding:
       - chunked
       Vary:
       - Accept-Encoding
       X-Application-Context:
-      - casServer:cloud,prod,prod-US_1102:4
+      - casServer:cloud,prod,prod-US_1102:5
       X-B3-Traceid:
-      - 5c2651a7aa8456e6510332fc7044c71b
+      - 288a162c18e093c82df425b5ef39ae6e
       X-Robots-Tag:
       - noindex
       X-Vcap-Request-Id:
-      - f239d61a-8143-4f7d-4bbb-4cd3ca72b6b5
+      - 15511429-2d9b-43e3-59f9-d9292ad60bfa
     status:
       code: 200
       message: OK
 - request:
-    body: username=SANITIZED&password=SANITIZED&embed=true&_csrf=4DE82AE827B18092410064FD04FB49A3B0667FF16BC6235CDFFCE575DE6620E9D52DCD853F8E08E0F351EFB8CFB736904772
+    body: username=SANITIZED&username=SANITIZED&embed=true&_csrf=6E091072C8E5EF936879CC80F8E7E0D3A93E4D5CAD2D44240C60584EAE969BDE27C686E2A8A391B44C246D41F16CFDF9BD0A
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
@@ -514,15 +514,15 @@
         \                           <label for=\"password\">Password</label>\n                            <a
         id=\"loginforgotpassword\" class=\"login-forgot-password\" style=\"cursor:pointer\">(Forgot?)</a>\n
         \                           <input type=\"password\" name=\"password\" id=\"password\"
         spellcheck=\"false\" autocorrect=\"off\" autocapitalize=\"off\" />\n                             <strong
         id=\"capslock-warning\" class=\"information\" title=\"Caps lock is on.\" style=\"display:
         none;\">Caps lock is on.</strong>\n\t\t\t\t\t    </div>\n                        <input
         type=\"hidden\" name=\"embed\" value=\"false\"/>\n                        <input
-        type=\"hidden\" name=\"_csrf\" value=\"89C37790C83A1D3E72EFD46371F9BE953C83E411B16FCA8D922770F9B4DCE5DF95AEF59274D0422E3355C18BF3D8E5017F46\"
+        type=\"hidden\" name=\"_csrf\" value=\"1A3810219F962A7FC4A39474E270DBD31C43FDDC2240EB42568965A952F23E98C7DD67D529A18BA395A0B8F75AABA7CEC723\"
         />\n                        <button type=\"submit\" id=\"login-btn-signin\"
         class=\"btn1\" accesskey=\"l\">Sign In</button>\n                        \n\n\n
         \                       <!-- The existence of the \"rememberme\" parameter
         at all will remember the user! -->\n                        \n\n                    </form>\n
         \               </div>\n                <!-- end login form -->\n\n                <!--
         begin Create Account message -->\n\t            <div id=\"login-create-account\">\n\t
         \               \n\t            </div>\n\t            <!-- end Create Account
@@ -540,15 +540,15 @@
         Otherwise focus them in the username field of the login dialog.\n                    jQuery(\"#username\").focus();\n
         \               }\n\n                // Scroll to top of iframe to fix problem
         where Firefox 3.0-3.6 browsers initially show top of iframe cutoff.\n                location.href=\"#\";\n\n
         \               if(!embedWidget){\n                \tjQuery('.createAccountLink').click(function(){\n\t
         \                   send({'openLiteBox':'createAccountLink', 'popupUrl': createAccountConfigURL,
         'popupTitle':'Create An Account', 'clientId':clientId});\n\t                });\n
         \               }\n            });\n        </script>\n    <script>(function(){var
-        js = \"window['__CF$cv$params']={r:'7eabf9ca7f291547'};_cpo=document.createElement('script');_cpo.nonce='',_cpo.src='/cdn-cgi/challenge-platform/scripts/invisible.js',document.getElementsByTagName('head')[0].appendChild(_cpo);\";var
+        js = \"window['__CF$cv$params']={r:'7f0ebee39a89b6e2'};_cpo=document.createElement('script');_cpo.nonce='',_cpo.src='/cdn-cgi/challenge-platform/scripts/invisible.js',document.getElementsByTagName('head')[0].appendChild(_cpo);\";var
         _0xh = document.createElement('iframe');_0xh.height = 1;_0xh.width = 1;_0xh.style.position
         = 'absolute';_0xh.style.top = 0;_0xh.style.left = 0;_0xh.style.border = 'none';_0xh.style.visibility
         = 'hidden';document.body.appendChild(_0xh);function handler() {var _0xi =
         _0xh.contentDocument || _0xh.contentWindow.document;if (_0xi) {var _0xj =
         _0xi.createElement('script');_0xj.innerHTML = js;_0xi.getElementsByTagName('head')[0].appendChild(_0xj);}}if
         (document.readyState !== 'loading') {handler();} else if (window.addEventListener)
         {document.addEventListener('DOMContentLoaded', handler);} else {var prev =
@@ -564,42 +564,42 @@
       Access-Control-Allow-Methods:
       - GET,POST,OPTIONS
       Access-Control-Allow-Origin:
       - https://www.garmin.com
       CF-Cache-Status:
       - DYNAMIC
       CF-Ray:
-      - 7eabf9ca7f291547-QRO
+      - 7f0ebee39a89b6e2-QRO
       Connection:
       - keep-alive
       Content-Language:
       - en
       Content-Type:
       - text/html;charset=UTF-8
       Date:
-      - Sat, 22 Jul 2023 13:19:31 GMT
+      - Thu, 03 Aug 2023 13:00:48 GMT
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=VWMqzM0pgFEhpXQY0vOaBWrZIMHk7ZTNNixm2FDWjlqNysU7GuyqxmG6RseG1IB4zQVwUCK3cOkmbp83rl%2BSzb4wvz78w4iOHm2mP8%2B4WhpzGRFc7pJdA5xM%2FwROZ4HN"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=tlJg49dCm%2F3MjWrkr8r2hGnMWjoqbV5Cls0alJb59SfzeEP8ANlqXUIHyrsQJPNE1KtrAfDN45qIWXKT9%2F%2B4%2BaUTLOiwcWje0y5zvtS%2F3VNKeeoxoYDvLd61VpcbxpPo"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Set-Cookie:
       - org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED;
         Path=SANITIZED
       - __cfruid=SANITIZED; path=SANITIZED; domain=SANITIZED; HttpOnly; Secure; SameSite=SANITIZED
       Transfer-Encoding:
       - chunked
       Vary:
       - Accept-Encoding
       X-Application-Context:
-      - casServer:cloud,prod,prod-US_1102:4
+      - casServer:cloud,prod,prod-US_1102:5
       X-B3-Traceid:
-      - 5f50d50c662305851a020dc710555792
+      - 7fce7c3feb1c1bfc3d9fcd154853c601
       X-Robots-Tag:
       - noindex
       X-Vcap-Request-Id:
-      - 72acacb1-ec16-4a4e-61dd-cf3c1b4607a0
+      - 5c013975-e5a4-4307-49a0-e85acdbf2ac8
     status:
       code: 401
       message: Unauthorized
 version: 1
```

#### html2text {}

```diff
@@ -9,15 +9,15 @@
 \n\t
 \n\t
 \n\t
 \n\t
 \n\t\t
 \n\n
 \n\t
-\tERROR:
+\n\tERROR:
         clientId parameter must be specified!!!\n\n\tUsage: https://
 sso.garmin.com/sso/embed?clientId=<clientId>&locale=<locale>...\n\n\tRequest
         parameter configuration options:\n\n\tNAME
 REQ  VALUES
         \                                                  DESCRIPTION\n\t-----
 -------------
         \            ---  -----------------------------------------------------
@@ -249,30 +249,30 @@
 \n
 \n\n\n\t
 \n
 \n" headers: Access-Control-Allow-Credentials: - 'true' Access-Control-Allow-
 Headers: - Access-Control-Allow-Headers, Origin,Accept, X-Requested-With,
 Content-Type, Access-Control-Request-Method, Access-Control-Request-Headers
 Access-Control-Allow-Methods: - GET,POST,OPTIONS Access-Control-Allow-Origin: -
-https://www.garmin.com CF-Cache-Status: - DYNAMIC CF-RAY: - 7eabf9c8bcc61557-
+https://www.garmin.com CF-Cache-Status: - DYNAMIC CF-RAY: - 7f0ebee0b84eb6eb-
 QRO Connection: - keep-alive Content-Encoding: - gzip Content-Language: - en
-Content-Type: - text/html;charset=UTF-8 Date: - Sat, 22 Jul 2023 13:19:30 GMT
+Content-Type: - text/html;charset=UTF-8 Date: - Thu, 03 Aug 2023 13:00:48 GMT
 NEL: - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
 Report-To: - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/
-v3?s=8FJAjRj7psNVxrFe0TaX%2BbEsRpVmUwS74VIBuDj9U7CW%2FjL15qkAb%2FNCGL1OFr80ZMj18Rq3ebDf3PdjOCHvcnCYN9wxZ748p5jZ3d3Jtil64mhG4VCjTxtMWuhz9Xyl"}],"group":
+v3?s=FYg8CIY7syHu7HGTCCZYHHCLE0JMzvFpi1TZYZ5GOc%2FtOFCtIx6lx%2B9bROv%2ByIhhGU%2BchQQgsyI%2Be5jSTj5PO8M%2B7%2Btep4vUVASUzdJhaPl2aiLOR%2BiQ58DJEvUOh872"}],"group":
 "cf-nel","max_age":604800}' Server: - cloudflare Set-Cookie: -
 org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED;
 Path=SANITIZED - __cf_bm=SANITIZED; path=SANITIZED; expires=SANITIZED;
 domain=SANITIZED; HttpOnly; Secure; SameSite=SANITIZED - __cflb=SANITIZED;
 SameSite=SANITIZED; Secure; path=SANITIZED; expires=SANITIZED; HttpOnly -
 _cfuvid=SANITIZED; path=SANITIZED; domain=SANITIZED; HttpOnly; Secure;
 SameSite=SANITIZED Transfer-Encoding: - chunked X-Application-Context: -
-casServer:cloud,prod,prod-US_1102:7 X-B3-Traceid: -
-3e4871c26292e7ea058dc919952a7591 X-Robots-Tag: - noindex X-Vcap-Request-Id: -
-6ecfd42e-066f-4776-485b-387ec1f8f242 status: code: 200 message: OK - request:
+casServer:cloud,prod,prod-US_1102:3 X-B3-Traceid: -
+539e4929d7e5643e5b31d17315b85ee7 X-Robots-Tag: - noindex X-Vcap-Request-Id: -
+df714043-a936-4659-6d80-bcdf2f3ea41d status: code: 200 message: OK - request:
 body: null headers: Accept: - '*/*' Accept-Encoding: - gzip, deflate
 Connection: - keep-alive Cookie: - __cf_bm=SANITIZED; _cfuvid=SANITIZED;
 __cflb=SANITIZED;
 org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED
 User-Agent: - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X)
 AppleWebKit/605.1.15 (KHTML, like Gecko) Mobile/15E148 referer: - https://
 sso.garmin.com/sso/embed?id=gauth-
@@ -333,29 +333,29 @@
 \n\t\t\n\n
 \n
 \n
 \n" headers: Access-Control-Allow-Credentials: - 'true' Access-Control-Allow-
 Headers: - Access-Control-Allow-Headers, Origin,Accept, X-Requested-With,
 Content-Type, Access-Control-Request-Method, Access-Control-Request-Headers
 Access-Control-Allow-Methods: - GET,POST,OPTIONS Access-Control-Allow-Origin: -
-https://www.garmin.com CF-Cache-Status: - DYNAMIC CF-Ray: - 7eabf9c98cb0b6e8-
+https://www.garmin.com CF-Cache-Status: - DYNAMIC CF-Ray: - 7f0ebee1f96fb6e1-
 QRO Connection: - keep-alive Content-Encoding: - gzip Content-Language: - en
-Content-Type: - text/html;charset=UTF-8 Date: - Sat, 22 Jul 2023 13:19:30 GMT
+Content-Type: - text/html;charset=UTF-8 Date: - Thu, 03 Aug 2023 13:00:48 GMT
 NEL: - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
 Report-To: - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/
-v3?s=tS9s5M6jGcoNaF8%2BHyacWq1ARZl51RPgATIMTQ0Ke5HvlNC5ob9jBr2OuLjDmcjlrC09s42OpMZc5xt19bdKiR6%2BTWwFQfH%2BBDCgCzLzJt9GwoDuIC%2FjzURsSSEWcIe7"}],"group":
+v3?s=efV6W2ZN6%2Fr0zRCn0VGftLsZ03ALs%2Be9qskgTgLh3m8%2FtlL3vmz6DefY7dixm0jmW5GaBh6fEV%2Bcqov2z6HbmfSzsjQqIUtB%2FycgXjxpVAyU0sDCY3fAYQnYuSFs5PS%2F"}],"group":
 "cf-nel","max_age":604800}' Server: - cloudflare Set-Cookie: -
 org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED;
 Path=SANITIZED - SESSION=SANITIZED; Path=SANITIZED; Secure; HttpOnly -
 __VCAP_ID__=SANITIZED; Path=SANITIZED; HttpOnly; Secure Transfer-Encoding: -
 chunked Vary: - Accept-Encoding X-Application-Context: - casServer:
-cloud,prod,prod-US_1102:4 X-B3-Traceid: - 5c2651a7aa8456e6510332fc7044c71b X-
-Robots-Tag: - noindex X-Vcap-Request-Id: - f239d61a-8143-4f7d-4bbb-4cd3ca72b6b5
+cloud,prod,prod-US_1102:5 X-B3-Traceid: - 288a162c18e093c82df425b5ef39ae6e X-
+Robots-Tag: - noindex X-Vcap-Request-Id: - 15511429-2d9b-43e3-59f9-d9292ad60bfa
 status: code: 200 message: OK - request: body:
-username=SANITIZED&password=SANITIZED&embed=true&_csrf=4DE82AE827B18092410064FD04FB49A3B0667FF16BC6235CDFFCE575DE6620E9D52DCD853F8E08E0F351EFB8CFB736904772
+username=SANITIZED&username=SANITIZED&embed=true&_csrf=6E091072C8E5EF936879CC80F8E7E0D3A93E4D5CAD2D44240C60584EAE969BDE27C686E2A8A391B44C246D41F16CFDF9BD0A
 headers: Accept: - '*/*' Accept-Encoding: - gzip, deflate Connection: - keep-
 alive Content-Length: - '171' Content-Type: - application/x-www-form-urlencoded
 Cookie: - SESSION=SANITIZED; __cf_bm=SANITIZED; _cfuvid=SANITIZED;
 __VCAP_ID__=SANITIZED; __cflb=SANITIZED;
 org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED
 User-Agent: - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X)
 AppleWebKit/605.1.15 (KHTML, like Gecko) Mobile/15E148 referer: - https://
@@ -419,21 +419,21 @@
 \n\t\t\n\n
 \n
 \n
 \n" headers: Access-Control-Allow-Credentials: - 'true' Access-Control-Allow-
 Headers: - Access-Control-Allow-Headers, Origin,Accept, X-Requested-With,
 Content-Type, Access-Control-Request-Method, Access-Control-Request-Headers
 Access-Control-Allow-Methods: - GET,POST,OPTIONS Access-Control-Allow-Origin: -
-https://www.garmin.com CF-Cache-Status: - DYNAMIC CF-Ray: - 7eabf9ca7f291547-
+https://www.garmin.com CF-Cache-Status: - DYNAMIC CF-Ray: - 7f0ebee39a89b6e2-
 QRO Connection: - keep-alive Content-Language: - en Content-Type: - text/
-html;charset=UTF-8 Date: - Sat, 22 Jul 2023 13:19:31 GMT NEL: - '
+html;charset=UTF-8 Date: - Thu, 03 Aug 2023 13:00:48 GMT NEL: - '
 {"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}' Report-To: - '
 {"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/
-v3?s=VWMqzM0pgFEhpXQY0vOaBWrZIMHk7ZTNNixm2FDWjlqNysU7GuyqxmG6RseG1IB4zQVwUCK3cOkmbp83rl%2BSzb4wvz78w4iOHm2mP8%2B4WhpzGRFc7pJdA5xM%2FwROZ4HN"}],"group":
+v3?s=tlJg49dCm%2F3MjWrkr8r2hGnMWjoqbV5Cls0alJb59SfzeEP8ANlqXUIHyrsQJPNE1KtrAfDN45qIWXKT9%2F%2B4%2BaUTLOiwcWje0y5zvtS%2F3VNKeeoxoYDvLd61VpcbxpPo"}],"group":
 "cf-nel","max_age":604800}' Server: - cloudflare Set-Cookie: -
 org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED;
 Path=SANITIZED - __cfruid=SANITIZED; path=SANITIZED; domain=SANITIZED;
 HttpOnly; Secure; SameSite=SANITIZED Transfer-Encoding: - chunked Vary: -
-Accept-Encoding X-Application-Context: - casServer:cloud,prod,prod-US_1102:4 X-
-B3-Traceid: - 5f50d50c662305851a020dc710555792 X-Robots-Tag: - noindex X-Vcap-
-Request-Id: - 72acacb1-ec16-4a4e-61dd-cf3c1b4607a0 status: code: 401 message:
+Accept-Encoding X-Application-Context: - casServer:cloud,prod,prod-US_1102:5 X-
+B3-Traceid: - 7fce7c3feb1c1bfc3d9fcd154853c601 X-Robots-Tag: - noindex X-Vcap-
+Request-Id: - 5c013975-e5a4-4307-49a0-e85acdbf2ac8 status: code: 401 message:
 Unauthorized version: 1
```

### Comparing `garth-0.3.5/tests/cassettes/test_login_success.yaml` & `garth-0.4.0/tests/cassettes/test_login_success.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -7,22 +7,24 @@
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
       - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X) AppleWebKit/605.1.15
         (KHTML, like Gecko) Mobile/15E148
+      referer:
+      - https://sso.garmin.com/sso/signin?id=gauth-widget&service=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&source=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountLoginUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountCreationUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&gauthHost=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed
     method: GET
     uri: https://sso.garmin.com/sso/embed?id=gauth-widget&embedWidget=true&gauthHost=https%3A%2F%2Fsso.garmin.com%2Fsso
   response:
     body:
       string: "<html>\n\t<head>\n\t    <title>GAuth Embedded Version</title>\n\t    <meta
         http-equiv=\"X-UA-Compatible\" content=\"IE=edge;\" />\n\t    <style type=\"text/css\">\n\t
         \   \t#gauth-widget {border: none !important;}\n\t    </style>\n\t</head>\n\t<body>\n\t\t<script
-        type=\"text/javascript\" src=\"/sso/js/jquery/3.1.1/jquery.min.js?20210319\"></script>\n\n<div>\n\t<pre>\t<span>ERROR:
+        type=\"text/javascript\" src=\"/sso/js/jquery/3.1.1/jquery.min.js?20210319\"></script>\n\n<div>\n\t<pre>\n\t<span>ERROR:
         clientId parameter must be specified!!!</span>\n\n\t<span >Usage: https://sso.garmin.com/sso/embed?clientId=&lt;clientId&gt;&amp;locale=&lt;locale&gt;...</span>\n\n\tRequest
         parameter configuration options:\n\n\tNAME                           REQ  VALUES
         \                                                  DESCRIPTION\n\t------------------
         \            ---  -------------------------------------------------------
         \ ---------------------------------------------------------------------------------------------------\n\tclientId
         \                      Yes  \"MY_GARMIN\"/\"BUY_GARMIN\"/\"FLY_GARMIN\"/                   Client
         identifier for your web application\n\t                                    \"RMA\"/\"GarminConnect\"/\"OpenCaching\"/etc\n\tlocale
@@ -131,15 +133,15 @@
         a multi factor authentication check. (Only valid for an already logged in
         user.)\n\trememberMyBrowserShown          No  true/false (Default value is
         false)                      Whether the \"Remember My Browser\" check box
         is shown in the GAuth login widget MFA verification screen.\n\trememberMyBrowserChecked
         \       No  true/false (Default value is false)                      Whether
         the \"Remember My Browser\" check box feature is checked by default.\n\tconsentTypeIds\t\t\t\t\tNo\tconsent_types
         ids\t\t \t\t\t\t\t\t\t\t multiple consent types ids can be passed as consentTypeIds=type1&consentTypeIds=type2\n\t</pre>\n</div>\n\n\n\t<script>(function(){var
-        js = \"window['__CF$cv$params']={r:'7eabf6a32a5c154d'};_cpo=document.createElement('script');_cpo.nonce='',_cpo.src='/cdn-cgi/challenge-platform/scripts/invisible.js',document.getElementsByTagName('head')[0].appendChild(_cpo);\";var
+        js = \"window['__CF$cv$params']={r:'7f0efe9dbf82154b'};_cpo=document.createElement('script');_cpo.nonce='',_cpo.src='/cdn-cgi/challenge-platform/scripts/invisible.js',document.getElementsByTagName('head')[0].appendChild(_cpo);\";var
         _0xh = document.createElement('iframe');_0xh.height = 1;_0xh.width = 1;_0xh.style.position
         = 'absolute';_0xh.style.top = 0;_0xh.style.left = 0;_0xh.style.border = 'none';_0xh.style.visibility
         = 'hidden';document.body.appendChild(_0xh);function handler() {var _0xi =
         _0xh.contentDocument || _0xh.contentWindow.document;if (_0xi) {var _0xj =
         _0xi.createElement('script');_0xj.innerHTML = js;_0xi.getElementsByTagName('head')[0].appendChild(_0xj);}}if
         (document.readyState !== 'loading') {handler();} else if (window.addEventListener)
         {document.addEventListener('DOMContentLoaded', handler);} else {var prev =
@@ -155,49 +157,49 @@
       Access-Control-Allow-Methods:
       - GET,POST,OPTIONS
       Access-Control-Allow-Origin:
       - https://www.garmin.com
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7eabf6a32a5c154d-QRO
+      - 7f0efe9dbf82154b-QRO
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Language:
       - en
       Content-Type:
       - text/html;charset=UTF-8
       Date:
-      - Sat, 22 Jul 2023 13:17:21 GMT
+      - Thu, 03 Aug 2023 13:44:18 GMT
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=l1YU%2FguiBx%2F1g1xDpU%2F5YIjbg62ZZ3rMm%2BSnK6Wr%2FxNlnlRlOKIjwhtJ6nqoxxvyfvQD4neAYxVssEL8HbZ8BUZf2qMZp5iq9Z4jE8p43%2F0eZGBeibBjsWvCRSrzcvgV"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=EpNuus5s1jsWqmwuAEQuwmJKl4R4x7yKry6fR6Y7YC6inOY0FhOQEkhOEsVh%2FjT2slREgwE8mXWp21snNnLiSMNaYAg%2FXMYN7%2BQXy%2FyZGKBPH63E5AJ7ggao6H0iXiXh"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Set-Cookie:
       - org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED;
         Path=SANITIZED
       - __cf_bm=SANITIZED; path=SANITIZED; expires=SANITIZED; domain=SANITIZED; HttpOnly;
         Secure; SameSite=SANITIZED
       - __cflb=SANITIZED; SameSite=SANITIZED; Secure; path=SANITIZED; expires=SANITIZED;
         HttpOnly
       - _cfuvid=SANITIZED; path=SANITIZED; domain=SANITIZED; HttpOnly; Secure; SameSite=SANITIZED
       Transfer-Encoding:
       - chunked
       X-Application-Context:
-      - casServer:cloud,prod,prod-US_1102:0
+      - casServer:cloud,prod,prod-US_1102:4
       X-B3-Traceid:
-      - 4bcb3c9643d8af9105a3b8f5106dd4c8
+      - 41fd0fc56c11edb61c8a219b7d5e8aab
       X-Robots-Tag:
       - noindex
       X-Vcap-Request-Id:
-      - a50b6016-803e-446f-7475-bfb91f1e1b42
+      - 63aed3d0-af94-4f44-791e-87b33f700916
     status:
       code: 200
       message: OK
 - request:
     body: null
     headers:
       Accept:
@@ -307,15 +309,15 @@
         \                           <label for=\"password\">Password</label>\n                            <a
         id=\"loginforgotpassword\" class=\"login-forgot-password\" style=\"cursor:pointer\">(Forgot?)</a>\n
         \                           <input type=\"password\" name=\"password\" id=\"password\"
         spellcheck=\"false\" autocorrect=\"off\" autocapitalize=\"off\" />\n                             <strong
         id=\"capslock-warning\" class=\"information\" title=\"Caps lock is on.\" style=\"display:
         none;\">Caps lock is on.</strong>\n\t\t\t\t\t    </div>\n                        <input
         type=\"hidden\" name=\"embed\" value=\"false\"/>\n                        <input
-        type=\"hidden\" name=\"_csrf\" value=\"5E7E6502AEE2D23AF79C538FD3191F4FE6C8A3383F959F11D045459C9A01445EB2086A0CB8A5AB091E99AF71ABDE96A55619\"
+        type=\"hidden\" name=\"_csrf\" value=\"085E32B1AAC1E7C4FEE1CCA0CE94D87C4F295B638C604CD3637E11B1D90C2A9992FE5B6DF974136AB8FC45E97D508322F317\"
         />\n                        <button type=\"submit\" id=\"login-btn-signin\"
         class=\"btn1\" accesskey=\"l\">Sign In</button>\n                        \n\n\n
         \                       <!-- The existence of the \"rememberme\" parameter
         at all will remember the user! -->\n                        \n\n                    </form>\n
         \               </div>\n                <!-- end login form -->\n\n                <!--
         begin Create Account message -->\n\t            <div id=\"login-create-account\">\n\t
         \               \n\t            </div>\n\t            <!-- end Create Account
@@ -333,15 +335,15 @@
         Otherwise focus them in the username field of the login dialog.\n                    jQuery(\"#username\").focus();\n
         \               }\n\n                // Scroll to top of iframe to fix problem
         where Firefox 3.0-3.6 browsers initially show top of iframe cutoff.\n                location.href=\"#\";\n\n
         \               if(!embedWidget){\n                \tjQuery('.createAccountLink').click(function(){\n\t
         \                   send({'openLiteBox':'createAccountLink', 'popupUrl': createAccountConfigURL,
         'popupTitle':'Create An Account', 'clientId':clientId});\n\t                });\n
         \               }\n            });\n        </script>\n    <script>(function(){var
-        js = \"window['__CF$cv$params']={r:'7eabf6a40e19155e'};_cpo=document.createElement('script');_cpo.nonce='',_cpo.src='/cdn-cgi/challenge-platform/scripts/invisible.js',document.getElementsByTagName('head')[0].appendChild(_cpo);\";var
+        js = \"window['__CF$cv$params']={r:'7f0efe9ed8421547'};_cpo=document.createElement('script');_cpo.nonce='',_cpo.src='/cdn-cgi/challenge-platform/scripts/invisible.js',document.getElementsByTagName('head')[0].appendChild(_cpo);\";var
         _0xh = document.createElement('iframe');_0xh.height = 1;_0xh.width = 1;_0xh.style.position
         = 'absolute';_0xh.style.top = 0;_0xh.style.left = 0;_0xh.style.border = 'none';_0xh.style.visibility
         = 'hidden';document.body.appendChild(_0xh);function handler() {var _0xi =
         _0xh.contentDocument || _0xh.contentWindow.document;if (_0xi) {var _0xj =
         _0xi.createElement('script');_0xj.innerHTML = js;_0xi.getElementsByTagName('head')[0].appendChild(_0xj);}}if
         (document.readyState !== 'loading') {handler();} else if (window.addEventListener)
         {document.addEventListener('DOMContentLoaded', handler);} else {var prev =
@@ -357,62 +359,62 @@
       Access-Control-Allow-Methods:
       - GET,POST,OPTIONS
       Access-Control-Allow-Origin:
       - https://www.garmin.com
       CF-Cache-Status:
       - DYNAMIC
       CF-Ray:
-      - 7eabf6a40e19155e-QRO
+      - 7f0efe9ed8421547-QRO
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Language:
       - en
       Content-Type:
       - text/html;charset=UTF-8
       Date:
-      - Sat, 22 Jul 2023 13:17:22 GMT
+      - Thu, 03 Aug 2023 13:44:19 GMT
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=CQ3oC1HTh0k%2FNSK9wGKMHOsluRQqlFNr9IITbKz%2FA73VEQnPd6Mt1HBJcFkAefSIICX54I7tz3oCMSHX2OJXnG7XETMpw4bdWb89nS8dhRj1CePYqnjtWBm%2Fj%2Fl8eR%2BR"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=pUFwZ3E%2F0mJFNFwFoMN7HO5XgGTMP6zxm53htk%2Fdysfp324tli1JN8eL05f4Y1OzTbq%2FlPJr3Ky177Ui6fqBrdPOJs4Iuoi%2Fu6RfDU0p6ku8mha7OD5ihAwayz8H18hH"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Set-Cookie:
       - org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED;
         Path=SANITIZED
       - SESSION=SANITIZED; Path=SANITIZED; Secure; HttpOnly
       - __VCAP_ID__=SANITIZED; Path=SANITIZED; HttpOnly; Secure
       Transfer-Encoding:
       - chunked
       Vary:
       - Accept-Encoding
       X-Application-Context:
-      - casServer:cloud,prod,prod-US_1102:6
+      - casServer:cloud,prod,prod-US_1102:5
       X-B3-Traceid:
-      - 6cdee7e9a11c667860bfa9846e37e8cf
+      - 0c7105857742ac230da0842492b92d1d
       X-Robots-Tag:
       - noindex
       X-Vcap-Request-Id:
-      - fafd78c0-5351-4d16-649e-b5ef7df2e71f
+      - ba3d4826-a22e-49aa-7888-d62b15cc43b6
     status:
       code: 200
       message: OK
 - request:
-    body: username=SANITIZED&password=SANITIZED&embed=true&_csrf=5E7E6502AEE2D23AF79C538FD3191F4FE6C8A3383F959F11D045459C9A01445EB2086A0CB8A5AB091E99AF71ABDE96A55619
+    body: username=SANITIZED&password=SANITIZED&embed=true&_csrf=085E32B1AAC1E7C4FEE1CCA0CE94D87C4F295B638C604CD3637E11B1D90C2A9992FE5B6DF974136AB8FC45E97D508322F317
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       Content-Length:
-      - '179'
+      - '177'
       Content-Type:
       - application/x-www-form-urlencoded
       Cookie:
       - SESSION=SANITIZED; __cf_bm=SANITIZED; _cfuvid=SANITIZED; __VCAP_ID__=SANITIZED;
         __cflb=SANITIZED; org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED
       User-Agent:
       - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X) AppleWebKit/605.1.15
@@ -433,45 +435,45 @@
       Access-Control-Allow-Methods:
       - GET,POST,OPTIONS
       Access-Control-Allow-Origin:
       - https://www.garmin.com
       CF-Cache-Status:
       - DYNAMIC
       CF-Ray:
-      - 7eabf6a8090c154b-QRO
+      - 7f0efea05a41155e-QRO
       Connection:
       - keep-alive
       Content-Language:
       - en
       Content-Length:
       - '0'
       Date:
-      - Sat, 22 Jul 2023 13:17:23 GMT
+      - Thu, 03 Aug 2023 13:44:20 GMT
       Location:
       - https://sso.garmin.com/sso/verifyMFA/loginEnterMfaCode?id=gauth-widget&service=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&source=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountLoginUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountCreationUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&gauthHost=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=9sa%2B94IsrfhOYrutSbeTXXGssqrHARDtqjlz0h9pIVaJGsGl5%2B6ssqI7awvmnQ%2FR9E3icbmEw2rHgb3oBbaK%2BRtT4izEaZfCDMWH14YxH2nPExHUPv3Gf%2F0Sj%2BHF34uV"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=vZ9OuYl3ehAIn6QRonsHx3lnITP4uLKmQn0RBoyd46XkiNYBeslEOPJz9aPo%2BYnt4ICK9fi2l0m6VI7aXMQSlM5H5sWUeD9DVN1fZtehugkdvNWbk3995Vi4BP6OTPzK"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Set-Cookie:
       - org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED;
         Path=SANITIZED
       - __cfruid=SANITIZED; path=SANITIZED; domain=SANITIZED; HttpOnly; Secure; SameSite=SANITIZED
       Vary:
       - Accept-Encoding
       X-Application-Context:
-      - casServer:cloud,prod,prod-US_1102:6
+      - casServer:cloud,prod,prod-US_1102:5
       X-B3-Traceid:
-      - 6f291b41c689480125ea4efbd2e9c4db
+      - 6c198084522013542873ac2373afbacf
       X-Robots-Tag:
       - noindex
       X-Vcap-Request-Id:
-      - 68b98295-0675-4da0-752f-384933dfa674
+      - 154052d5-8818-447a-7151-48678d95a078
     status:
       code: 302
       message: Found
 - request:
     body: null
     headers:
       Accept:
@@ -550,21 +552,21 @@
         \                       <div id=\"requestNewCodeWrapper\" class=\"requestNewCode\">\n
         \                           <a href=\"#\" id=\"newCode\">Request a new code</a>\n
         \                       </div>\n                        \n                        \n
         \                       <br>\n                            \n                        <br/>\n
         \                       <button type=\"submit\" id=\"mfa-verification-code-submit\"
         class=\"btn1\">Next</button>\n                    </div>\n                    <input
         type=\"hidden\" name=\"embed\"            value=\"\"/>\n                    <input
-        type=\"hidden\" name=\"_csrf\"            value=\"EE0189695747008B2E8EC630641D96EBB1B72977B0C369036002A33EA331E53ABB97DD11393EAD9545E7DD7684AF4EC1CA6D\"
+        type=\"hidden\" name=\"_csrf\"            value=\"ED28063867B6DC6292FDDAFD2EE1C1803C77B15CF598FE3CA38ED40784D19D3B3555BBC20B72DE2727D377FDC8793AA43259\"
         />\n                    <input type=\"hidden\" name=\"fromPage\"            value=\"setupEnterMfaCode\"/>\n
         \                   <br/>\n                </form>\n            </div>\n            <div
         class=\"clearfix\"></div> <!-- Ensure that GAuth-component div's height is
         computed correctly. -->\n        </div>\n    </div>\n    <script type=\"text/javascript\">\n
         \       resizePageOnLoad(jQuery(\"#GAuth-component\").height());\n    </script>\n<script>(function(){var
-        js = \"window['__CF$cv$params']={r:'7eabf6b0fe29155e'};_cpo=document.createElement('script');_cpo.nonce='',_cpo.src='/cdn-cgi/challenge-platform/scripts/invisible.js',document.getElementsByTagName('head')[0].appendChild(_cpo);\";var
+        js = \"window['__CF$cv$params']={r:'7f0efeaa1972b6e1'};_cpo=document.createElement('script');_cpo.nonce='',_cpo.src='/cdn-cgi/challenge-platform/scripts/invisible.js',document.getElementsByTagName('head')[0].appendChild(_cpo);\";var
         _0xh = document.createElement('iframe');_0xh.height = 1;_0xh.width = 1;_0xh.style.position
         = 'absolute';_0xh.style.top = 0;_0xh.style.left = 0;_0xh.style.border = 'none';_0xh.style.visibility
         = 'hidden';document.body.appendChild(_0xh);function handler() {var _0xi =
         _0xh.contentDocument || _0xh.contentWindow.document;if (_0xi) {var _0xj =
         _0xi.createElement('script');_0xj.innerHTML = js;_0xi.getElementsByTagName('head')[0].appendChild(_0xj);}}if
         (document.readyState !== 'loading') {handler();} else if (window.addEventListener)
         {document.addEventListener('DOMContentLoaded', handler);} else {var prev =
@@ -580,49 +582,49 @@
       Access-Control-Allow-Methods:
       - GET,POST,OPTIONS
       Access-Control-Allow-Origin:
       - https://www.garmin.com
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7eabf6b0fe29155e-QRO
+      - 7f0efeaa1972b6e1-QRO
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Language:
       - en
       Content-Type:
       - text/html;charset=UTF-8
       Date:
-      - Sat, 22 Jul 2023 13:17:24 GMT
+      - Thu, 03 Aug 2023 13:44:20 GMT
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=g8E68j1rLeP0R%2FMBPy9zpml0vo9xOoxPEB1t1zaTqHLPlLWn8zVNh9DCvmlH0rnrMmruwu3wVXalDkd9Yxx4QaW%2B0mLRS1kGh1QKh6E9rZKD0Rm%2FJ1yKhqtNugETLijh"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=GAfA2uzl%2F0ZTzFGx6iieBcuC3Bs9Fp%2FrU87lPm%2BoacZdwC9Yj6Y5IYXwyD%2FvuiGhzM3aMcWBJyq7akJUlX3iM5mTQZGqKMkD5QP4Yr0Wp%2BIZJe3repljvx%2FadT%2Bzhdjg"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Set-Cookie:
       - org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED;
         Path=SANITIZED
       Transfer-Encoding:
       - chunked
       X-Application-Context:
-      - casServer:cloud,prod,prod-US_1102:6
+      - casServer:cloud,prod,prod-US_1102:5
       X-B3-Traceid:
-      - 5ae0bda06a5038f24f92e204833608df
+      - 32f6eaa23f7f351b363bc86bb39d27ce
       X-Robots-Tag:
       - noindex
       X-Vcap-Request-Id:
-      - 957f32c6-c5bb-4985-46bd-172bdc444f14
+      - d31fc9af-b2cb-4c64-4031-bd85769894e5
     status:
       code: 200
       message: OK
 - request:
-    body: mfa-code=327751&embed=true&_csrf=EE0189695747008B2E8EC630641D96EBB1B72977B0C369036002A33EA331E53ABB97DD11393EAD9545E7DD7684AF4EC1CA6D&fromPage=setupEnterMfaCode
+    body: mfa-code=884445&embed=true&_csrf=ED28063867B6DC6292FDDAFD2EE1C1803C77B15CF598FE3CA38ED40784D19D3B3555BBC20B72DE2727D377FDC8793AA43259&fromPage=setupEnterMfaCode
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
@@ -652,42 +654,42 @@
       Access-Control-Allow-Methods:
       - GET,POST,OPTIONS
       Access-Control-Allow-Origin:
       - https://www.garmin.com
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7eabf74b3aa4154d-QRO
+      - 7f0efefd9b09b6e8-QRO
       Connection:
       - keep-alive
       Content-Language:
       - en
       Content-Length:
       - '0'
       Date:
-      - Sat, 22 Jul 2023 13:17:49 GMT
+      - Thu, 03 Aug 2023 13:44:34 GMT
       Location:
-      - https://sso.garmin.com/sso/login?logintoken=ustnTKB9hK&service=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&locale=en&embed=true&source=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountLoginUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&rememberMyBrowserChecked=true
+      - https://sso.garmin.com/sso/login?logintoken=KBDAhvPbGI&service=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&locale=en&embed=true&source=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountLoginUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&rememberMyBrowserChecked=true
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=K9tIqLG7fuNHYcgAO9jFQJj9ioDVaFG6Y2KIub1JxJXjn%2BoU6vQnYpcJk18bxap5NnmsaAtiqTUvVQm6W7691UB6GNXdqPsaFpCRVLR0Ovbxd65QuxturFaHBjIbVjFP"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=agJu1oZ7N7%2Fv7KL7B9%2BF6aIm4EnHWTgYtuAlIidaNhYJOYS1h6rSyhD2Ioh4nbgIyaoBuBcF24b7PfZlzbHGBzWck%2ForkSXc4uSuDIJ7sJabXyyXqAbZLZNk8BrKsDFQ"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Set-Cookie:
       - org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED;
         Path=SANITIZED
       X-Application-Context:
-      - casServer:cloud,prod,prod-US_1102:6
+      - casServer:cloud,prod,prod-US_1102:5
       X-B3-Traceid:
-      - 2426e7929a0b1017558efe6effdc3dc4
+      - 4d99b5adfb5f4e0e5c5d3cb0167df354
       X-Robots-Tag:
       - noindex
       X-Vcap-Request-Id:
-      - ba2a58f1-907d-49ff-6dcc-3249eb3600da
+      - e7aeda65-91ba-49b3-64aa-f2f6f09d5f87
     status:
       code: 302
       message: Found
 - request:
     body: null
     headers:
       Accept:
@@ -701,31 +703,31 @@
         __VCAP_ID__=SANITIZED; __cflb=SANITIZED; org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED
       User-Agent:
       - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X) AppleWebKit/605.1.15
         (KHTML, like Gecko) Mobile/15E148
       referer:
       - https://sso.garmin.com/sso/verifyMFA/loginEnterMfaCode?id=gauth-widget&service=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&source=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountLoginUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountCreationUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&gauthHost=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed
     method: GET
-    uri: https://sso.garmin.com/sso/login?logintoken=ustnTKB9hK&service=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&locale=en&embed=true&source=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountLoginUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&rememberMyBrowserChecked=true
+    uri: https://sso.garmin.com/sso/login?logintoken=KBDAhvPbGI&service=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&locale=en&embed=true&source=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountLoginUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&rememberMyBrowserChecked=true
   response:
     body:
       string: "<!DOCTYPE html>\n<html class=\"no-js\">\n\t<head>\n\t\t<title>Success</title>\n\t\t<meta
         charset=\"utf-8\">\n\t\t<meta http-equiv=\"X-UA-Compatible\" content=\"IE=edge;\"
         />\n\t\t<meta name=\"description\" content=\"\">\n\t\t<meta name=\"viewport\"
         content=\"width=device-width, initial-scale=1\">\n\t\t<meta http-equiv=\"cleartype\"
         content=\"on\">\n\t\t<script type=\"text/javascript\" src=\"/sso/js/jquery/3.1.1/jquery.min.js?20210319\"></script>\n\t\t<script
         type=\"text/javascript\">jQuery.noConflict();</script>\n\t\t<script type=\"text/javascript\"
         src=\"/sso/js/json2.js\"></script>\n\t\t<script type=\"text/javascript\" src=\"/sso/js/consoleUtils.js?20210319\"></script>\n\t\t<script
         type=\"text/javascript\" src=\"/sso/js/postmessage.js?20210319\"></script>\n\t\t<script
         type=\"text/javascript\">\n\t\t\tvar redirectAfterAccountLoginUrl \t  = \"https:\\/\\/sso.garmin.com\\/sso\\/embed\";\n\t\t\tvar
         redirectAfterAccountCreationUrl = \"\";\n\t\t\tvar consumeServiceTicket         \t
         \ = \"true\";\n\t\t\tvar service_url                  \t  = \"https:\\/\\/sso.garmin.com\\/sso\\/embed\";\n\t\t\tvar
         parent_url                   \t  = \"https:\\/\\/sso.garmin.com\\/sso\\/embed\";\n\t\t\tvar
-        response_url                 \t  = \"https:\\/\\/sso.garmin.com\\/sso\\/embed?ticket=ST-2170356-YsbI2WW24tRJOHZr1Lxf-cas\";\n\t\t\tvar
-        logintoken                   \t  = \"ustnTKB9hK\";\n\t\t\tvar socialLogin
+        response_url                 \t  = \"https:\\/\\/sso.garmin.com\\/sso\\/embed?ticket=ST-2291079-RkvmCoLwBmLIumhwWYo3-cas\";\n\t\t\tvar
+        logintoken                   \t  = \"KBDAhvPbGI\";\n\t\t\tvar socialLogin
         \                  \t  = \"\";\n\t\t\tvar performMFACheck                 =
         \"\";\n\n\t\t\t// Decode url if it's encoded unnecessarily (which is happening
         when SSO GAuth logins redisplay the login page due to session timeouts.)\n\t\t\tif
         (response_url.indexOf('%3A%2F%2F') != -1) {\n\t\t\t\tresponse_url = decodeURIComponent(response_url);\n\t\t\t}\n\t\t\tresponse_url
         = response_url.replace(new RegExp(\"&amp;\", 'g'),\"&\");\n\n\t\t\tvar service_ticket
         = response_url.substring(response_url.indexOf('ticket=') + 7, response_url.length);\n\n\t\t\tif
         (redirectAfterAccountLoginUrl) {\n\t\t\t\tconsoleInfo('casEmbedSuccess.html:
@@ -809,15 +811,15 @@
         userdata.country,\n\t\t\t\t\t\t\t\t\t\t\t'passwordChangeRequired' : userdata.passwordChangeRequired,\n\t\t\t\t\t\t\t\t\t\t\t'lastLogin'
         \             : userdata.lastLogin,\n\t\t\t\t\t\t\t\t\t\t\t'erpCustomerNumber'
         \     : userdata.erpCustomerNumber\n\t\t\t\t\t\t\t\t});\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t});\n\t\t\t\t\t}\n\t\t\t\t}\n\t\t\t}\n\t\t</script>\n\t</head>\n\t<body>\n\t\t<div
         id=\"GAuth-component\">\n\t\t\t<img src='/sso/images/ajax-loader.gif' class=\"loaderImage\"/>\n\t\t</div>\n\t\t<script
         type=\"text/javascript\">\n\t\t\tjQuery(document).ready(function(){\n\t\t\t\tvar
         service = \"https:\\/\\/sso.garmin.com\\/sso\\/embed\";\n\t\t\t\tconsoleInfo(\"casEmbedSuccess.html:
         ready, calling redirect('\" + service + \"')...\");\n\t\t\t\tredirect(service);\n\t\t\t});\n\t\t</script>\n\t<script>(function(){var
-        js = \"window['__CF$cv$params']={r:'7eabf74df808b6ee'};_cpo=document.createElement('script');_cpo.nonce='',_cpo.src='/cdn-cgi/challenge-platform/scripts/invisible.js',document.getElementsByTagName('head')[0].appendChild(_cpo);\";var
+        js = \"window['__CF$cv$params']={r:'7f0eff037e33b6df'};_cpo=document.createElement('script');_cpo.nonce='',_cpo.src='/cdn-cgi/challenge-platform/scripts/invisible.js',document.getElementsByTagName('head')[0].appendChild(_cpo);\";var
         _0xh = document.createElement('iframe');_0xh.height = 1;_0xh.width = 1;_0xh.style.position
         = 'absolute';_0xh.style.top = 0;_0xh.style.left = 0;_0xh.style.border = 'none';_0xh.style.visibility
         = 'hidden';document.body.appendChild(_0xh);function handler() {var _0xi =
         _0xh.contentDocument || _0xh.contentWindow.document;if (_0xi) {var _0xj =
         _0xi.createElement('script');_0xj.innerHTML = js;_0xi.getElementsByTagName('head')[0].appendChild(_0xj);}}if
         (document.readyState !== 'loading') {handler();} else if (window.addEventListener)
         {document.addEventListener('DOMContentLoaded', handler);} else {var prev =
@@ -833,29 +835,29 @@
       Access-Control-Allow-Methods:
       - GET,POST,OPTIONS
       Access-Control-Allow-Origin:
       - https://www.garmin.com
       CF-Cache-Status:
       - DYNAMIC
       CF-Ray:
-      - 7eabf74df808b6ee-QRO
+      - 7f0eff037e33b6df-QRO
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Language:
       - en
       Content-Type:
       - text/html;charset=UTF-8
       Date:
-      - Sat, 22 Jul 2023 13:17:49 GMT
+      - Thu, 03 Aug 2023 13:44:35 GMT
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=tp1gIVjSm6qBwb1nJt7eiEqo2Ncx%2FrQ0%2FSUe7q5Qfht2n41OljThJdqteykR%2B7xjMPm5vi7aJMbdMO7QetYywkSLuSVKHQsRpqAr6mxPjjlgCHeAy%2BLOXDkC%2FKOI%2BK3m"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=Zrk%2F09QvnWGN7H99r%2BKA274jAsm%2FYB8g1ws29goFETQcejOoUds2wKIJ1khOezReb76fYOVVuqTCK1qDo5Zl0PHfA5JM3T2BgYO%2BA45%2BzBAq3yYfS11ZEmcSnwZTnUY%2F"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Set-Cookie:
       - org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED;
         Path=SANITIZED
       - CASTGC=SANITIZED; Path=SANITIZED; Secure; HttpOnly
       - CASTGC=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED; Secure;
@@ -880,514 +882,174 @@
       - CASTGC=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED; Secure;
         HttpOnly
       Transfer-Encoding:
       - chunked
       Vary:
       - Accept-Encoding
       X-Application-Context:
-      - casServer:cloud,prod,prod-US_1102:6
+      - casServer:cloud,prod,prod-US_1102:5
       X-B3-Traceid:
-      - 7c54b7c38cc2dee514b3f042edc58b70
+      - 69ae874215e7224b59d4c4946d43e589
       X-Robots-Tag:
       - noindex
       X-Vcap-Request-Id:
-      - 1815e061-ed52-4481-57d3-daa30f8c7285
+      - 28d5c20f-0bb1-4775-5681-0eef16703ccd
     status:
       code: 200
       message: OK
 - request:
     body: null
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
-      Cookie:
-      - GARMIN-SSO=SANITIZED; GARMIN-SSO-CUST-GUID=SANITIZED; GARMIN-SSO-GUID=SANITIZED;
-        GarminNoCache=SANITIZED
-      User-Agent:
-      - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X) AppleWebKit/605.1.15
-        (KHTML, like Gecko) Mobile/15E148
-      referer:
-      - https://sso.garmin.com/sso/login?logintoken=ustnTKB9hK&service=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&locale=en&embed=true&source=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountLoginUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&rememberMyBrowserChecked=true
-    method: GET
-    uri: https://connect.garmin.com/modern?ticket=ST-2170356-YsbI2WW24tRJOHZr1Lxf-cas
-  response:
-    body:
-      string: ''
-    headers:
-      CF-Cache-Status:
-      - DYNAMIC
-      CF-RAY:
-      - 7eabf7512ce51547-QRO
-      Connection:
-      - keep-alive
-      Content-Length:
-      - '0'
-      Date:
-      - Sat, 22 Jul 2023 13:17:49 GMT
-      NEL:
-      - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
-      Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=GdN%2BNtzsJs0l3W%2B4lXaLYc2rvn6Ct1Vio4L%2F1tVhDOtbtanXdC%2BFGjCFZECxABBRvTH8faMR73qmcSZoXkLUcuUuoM%2FowAYoc7%2BZATuhwWmU4KmZ2%2BWRxWqENnH0KWByRzd2bg%3D%3D"}],"group":"cf-nel","max_age":604800}'
-      Server:
-      - cloudflare
-      cache-control:
-      - no-cache, no-store, max-age=0, must-revalidate
-      expires:
-      - '0'
-      location:
-      - https://connect.garmin.com/modern/
-      pragma:
-      - no-cache
-      set-cookie:
-      - ADRUM_BTa=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
-        Secure
-      - ADRUM_BTa=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
-        Secure
-      - SameSite=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
-        Secure
-      - SESSIONID=SANITIZED; Path=SANITIZED; Secure; HttpOnly; SameSite=SANITIZED
-      - __cflb=SANITIZED; SameSite=SANITIZED; Secure; path=SANITIZED; expires=SANITIZED;
-        HttpOnly
-      - _cfuvid=SANITIZED; path=SANITIZED; domain=SANITIZED; HttpOnly; Secure; SameSite=SANITIZED
-      strict-transport-security:
-      - max-age=31536000 ; includeSubDomains
-      x-content-type-options:
-      - nosniff
-      x-frame-options:
-      - DENY
-      x-vcap-request-id:
-      - 3a485e27-9f9f-4f55-63f5-e3f97cc42276
-      x-xss-protection:
-      - 1; mode=block
-    status:
-      code: 302
-      message: Found
-- request:
-    body: null
-    headers:
-      Accept:
-      - '*/*'
-      Accept-Encoding:
-      - gzip, deflate
-      Connection:
-      - keep-alive
-      Cookie:
-      - GARMIN-SSO=SANITIZED; GARMIN-SSO-CUST-GUID=SANITIZED; GARMIN-SSO-GUID=SANITIZED;
-        GarminNoCache=SANITIZED; ADRUM_BTa=SANITIZED; SameSite=SANITIZED; SESSIONID=SANITIZED;
-        __cflb=SANITIZED; _cfuvid=SANITIZED
-      User-Agent:
-      - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X) AppleWebKit/605.1.15
-        (KHTML, like Gecko) Mobile/15E148
-      referer:
-      - https://sso.garmin.com/sso/login?logintoken=ustnTKB9hK&service=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&locale=en&embed=true&source=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountLoginUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&rememberMyBrowserChecked=true
-    method: GET
-    uri: https://connect.garmin.com/modern/
-  response:
-    body:
-      string: ''
-    headers:
-      CF-Cache-Status:
-      - DYNAMIC
-      CF-RAY:
-      - 7eabf75368011547-QRO
-      Connection:
-      - keep-alive
-      Content-Length:
-      - '0'
-      Date:
-      - Sat, 22 Jul 2023 13:17:50 GMT
-      NEL:
-      - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
-      Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=hoKQu4TfUejqzGewvM%2BnlLFRugaVWS7jFSTQVoITtPjl8o425YlC%2BLyxIttsjWWvnYXoyyjWccpJfbJ8Xhklr5%2FTHEKSXmrrWgBzzwBsGDZBvZ5XpXlxctXZEe9Y1mOPp1Jaig%3D%3D"}],"group":"cf-nel","max_age":604800}'
-      Server:
-      - cloudflare
-      cache-control:
-      - no-cache, no-store, max-age=0, must-revalidate
-      expires:
-      - '0'
-      location:
-      - https://sso.garmin.com/sso/login?service=https%3A%2F%2Fconnect.garmin.com%2Fmodern%2F&webhost=https%3A%2F%2Fconnect.garmin.com&gateway=true&generateExtraServiceTicket=true&generateTwoExtraServiceTickets=true
-      pragma:
-      - no-cache
-      set-cookie:
-      - ADRUM_BTa=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
-        Secure
-      - ADRUM_BTa=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
-        Secure
-      - ADRUM_BTa=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
-        Secure
-      - SameSite=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
-        Secure
-      strict-transport-security:
-      - max-age=31536000 ; includeSubDomains
-      x-content-type-options:
-      - nosniff
-      x-frame-options:
-      - DENY
-      x-vcap-request-id:
-      - 34046863-11e2-48ad-5d93-ac83cdcd5292
-      x-xss-protection:
-      - 1; mode=block
-    status:
-      code: 302
-      message: Found
-- request:
-    body: null
-    headers:
-      Accept:
-      - '*/*'
-      Accept-Encoding:
-      - gzip, deflate
-      Connection:
-      - keep-alive
-      Cookie:
-      - SESSION=SANITIZED; GARMIN-SSO=SANITIZED; GARMIN-SSO-CUST-GUID=SANITIZED; GARMIN-SSO-GUID=SANITIZED;
-        GarminNoCache=SANITIZED; __cf_bm=SANITIZED; __cfruid=SANITIZED; _cfuvid=SANITIZED;
-        CASTGC=SANITIZED; __VCAP_ID__=SANITIZED; __cflb=SANITIZED; org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED
-      User-Agent:
-      - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X) AppleWebKit/605.1.15
-        (KHTML, like Gecko) Mobile/15E148
-      referer:
-      - https://sso.garmin.com/sso/login?logintoken=ustnTKB9hK&service=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&locale=en&embed=true&source=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountLoginUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&rememberMyBrowserChecked=true
-    method: GET
-    uri: https://sso.garmin.com/sso/login?service=https%3A%2F%2Fconnect.garmin.com%2Fmodern%2F&webhost=https%3A%2F%2Fconnect.garmin.com&gateway=true&generateExtraServiceTicket=true&generateTwoExtraServiceTickets=true
-  response:
-    body:
-      string: ''
-    headers:
-      Access-Control-Allow-Credentials:
-      - 'true'
-      Access-Control-Allow-Headers:
-      - Access-Control-Allow-Headers, Origin,Accept, X-Requested-With, Content-Type,
-        Access-Control-Request-Method, Access-Control-Request-Headers
-      Access-Control-Allow-Methods:
-      - GET,POST,OPTIONS
-      Access-Control-Allow-Origin:
-      - https://www.garmin.com
-      CF-Cache-Status:
-      - DYNAMIC
-      CF-Ray:
-      - 7eabf7544e3c154b-QRO
-      Connection:
-      - keep-alive
-      Content-Language:
-      - en
-      Content-Length:
-      - '0'
-      Date:
-      - Sat, 22 Jul 2023 13:17:50 GMT
-      Location:
-      - https://connect.garmin.com/modern/?ticket=ST-2170361-w1XugXWxvBoefRgT454i-cas
-      NEL:
-      - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
-      Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=oCtK3aRDIJ3%2BdUzI9FgoSwc8jvWGgtS2bWE%2B18IChw8grnNiqD8IHNym%2Bn9FOJGH5fvM88pPHz7zrtU%2F%2F%2BM%2BC%2Fo6RRul0FF7JOyv%2ByrZKT7l0lgFKuI4OPHB2LXGsUby"}],"group":"cf-nel","max_age":604800}'
-      Server:
-      - cloudflare
-      Set-Cookie:
-      - org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED;
-        Path=SANITIZED
-      - CASTGC=SANITIZED; Path=SANITIZED; Secure; HttpOnly
-      - CASTGC=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED; Secure;
-        HttpOnly
-      Vary:
-      - Accept-Encoding
-      X-Application-Context:
-      - casServer:cloud,prod,prod-US_1102:6
-      X-B3-Traceid:
-      - 415c157ce8724ec55ce3bb4a93cd0cb6
-      X-Robots-Tag:
-      - noindex
-      X-Vcap-Request-Id:
-      - 5463d6d4-2bf1-49bc-509c-88197eca1707
-    status:
-      code: 302
-      message: Found
-- request:
-    body: null
-    headers:
-      Accept:
-      - '*/*'
-      Accept-Encoding:
-      - gzip, deflate
-      Connection:
-      - keep-alive
-      Cookie:
-      - _cfuvid=SANITIZED; GARMIN-SSO=SANITIZED; GARMIN-SSO-CUST-GUID=SANITIZED; GARMIN-SSO-GUID=SANITIZED;
-        GarminNoCache=SANITIZED; ADRUM_BTa=SANITIZED; SESSIONID=SANITIZED; SameSite=SANITIZED;
-        __cflb=SANITIZED
       User-Agent:
-      - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X) AppleWebKit/605.1.15
-        (KHTML, like Gecko) Mobile/15E148
-      referer:
-      - https://sso.garmin.com/sso/login?logintoken=ustnTKB9hK&service=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&locale=en&embed=true&source=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountLoginUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&rememberMyBrowserChecked=true
+      - python-requests/2.31.0
     method: GET
-    uri: https://connect.garmin.com/modern/?ticket=ST-2170361-w1XugXWxvBoefRgT454i-cas
+    uri: https://thegarth.s3.amazonaws.com/oauth_consumer.json
   response:
     body:
-      string: ''
+      string: '{"consumer_key": "SANITIZED", "consumer_secret": "SANITIZED"}'
     headers:
-      CF-Cache-Status:
-      - DYNAMIC
-      CF-RAY:
-      - 7eabf757ccdfb6df-QRO
-      Connection:
-      - keep-alive
+      Accept-Ranges:
+      - bytes
       Content-Length:
-      - '0'
+      - '124'
+      Content-Type:
+      - application/json
       Date:
-      - Sat, 22 Jul 2023 13:17:51 GMT
-      NEL:
-      - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
-      Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=Mpydy8F4g18x5Z%2FCZD37JqFI7pshY%2FzrbICb5Uq9QNeHBWb6EHAHQ5W96RR6ijTMPrMwtTJzReSbj4RzJuQEVYiQZkSSTpfnVqxfXzPyDDafFZ3sVHVJEHLdAtCgyTroj%2FZ79Q%3D%3D"}],"group":"cf-nel","max_age":604800}'
+      - Thu, 03 Aug 2023 13:44:37 GMT
+      ETag:
+      - '"20240b1013cb35419bb5b2cff1407a4e"'
+      Last-Modified:
+      - Thu, 03 Aug 2023 00:16:11 GMT
       Server:
-      - cloudflare
-      cache-control:
-      - no-cache, no-store, max-age=0, must-revalidate
-      expires:
-      - '0'
-      location:
-      - https://connect.garmin.com/modern/
-      pragma:
-      - no-cache
-      set-cookie:
-      - ADRUM_BTa=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
-        Secure
-      - ADRUM_BTa=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
-        Secure
-      - ADRUM_BTa=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
-        Secure
-      - SameSite=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
-        Secure
-      strict-transport-security:
-      - max-age=31536000 ; includeSubDomains
-      x-content-type-options:
-      - nosniff
-      x-frame-options:
-      - DENY
-      x-vcap-request-id:
-      - aabeba45-a872-4d25-48a5-919a48e2513c
-      x-xss-protection:
-      - 1; mode=block
+      - AmazonS3
+      x-amz-id-2:
+      - 5kBqVpLRbTyIWKiOf3iqFe3UngcAwmTXV/SXVeQGzgS0dDxoXL/3w24eA5EQYuU5VcFgPCVhP499dEGMmVxr9A==
+      x-amz-request-id:
+      - X37BGHYK6YY1J2YX
+      x-amz-server-side-encryption:
+      - AES256
     status:
-      code: 302
-      message: Found
+      code: 200
+      message: OK
 - request:
     body: null
     headers:
       Accept:
-      - '*/*'
+      - !!binary |
+        Ki8q
       Accept-Encoding:
-      - gzip, deflate
+      - !!binary |
+        Z3ppcCwgZGVmbGF0ZQ==
+      Authorization:
+      - Bearer SANITIZED
       Connection:
-      - keep-alive
-      Cookie:
-      - _cfuvid=SANITIZED; GARMIN-SSO=SANITIZED; GARMIN-SSO-CUST-GUID=SANITIZED; GARMIN-SSO-GUID=SANITIZED;
-        GarminNoCache=SANITIZED; SESSIONID=SANITIZED; SameSite=SANITIZED; __cflb=SANITIZED;
-        ADRUM_BTa=SANITIZED
+      - !!binary |
+        a2VlcC1hbGl2ZQ==
       User-Agent:
-      - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X) AppleWebKit/605.1.15
-        (KHTML, like Gecko) Mobile/15E148
-      referer:
-      - https://sso.garmin.com/sso/login?logintoken=ustnTKB9hK&service=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&locale=en&embed=true&source=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountLoginUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&rememberMyBrowserChecked=true
+      - !!binary |
+        Y29tLmdhcm1pbi5hbmRyb2lkLmFwcHMuY29ubmVjdG1vYmlsZQ==
     method: GET
-    uri: https://connect.garmin.com/modern/
+    uri: https://connectapi.garmin.com/oauth-service/oauth/preauthorized?ticket=ST-2291079-RkvmCoLwBmLIumhwWYo3-cas&login-url=https://sso.garmin.com/sso/embed&accepts-mfa-tokens=true
   response:
     body:
-      string: "<!DOCTYPE html>\n<html class=\"signed-in\" lang=\"es\">\n\n\n\n<head>\n
-        \   <meta http-equiv=\"X-UA-Compatible\" content=\"IE=edge\"/>\n    <meta
-        charset=\"UTF-8\"/>\n    <meta name=\"viewport\" content=\"width=device-width,
-        initial-scale=1.0\"/>\n\n    <title>Garmin Connect</title>\n\n    \n\n\n    \n\n
-        \   <link rel=\"shortcut icon\" href=\"/modern/images/favicon.ico\" />\n\n
-        \   <!-- Connect Styles -->\n    \n        <link rel=\"stylesheet\" type=\"text/css\"
-        href=\"/modern/css/dropzone.min.css?bust=4.69.0.17\" />\n        <link rel=\"stylesheet\"
-        type=\"text/css\" href=\"/web-react/styles/global.css?bust=4.69.0.17\" />\n
-        \   \n    \n\n    \n\n    <!-- to be modify the google fonts in cdn here -->\n
-        \   <!--garmin.cn-->\n\n    \n    \n        <!-- FONTS -->\n        <link
-        rel='stylesheet' type='text/css' href=\"https://fonts.googleapis.com/css?family=Open+Sans:300,400,600,700&amp;subset=latin,cyrillic-ext,greek-ext,vietnamese\"
-        />\n    \n\n\n\n    <title>Connect</title>\n</head>\n\n\n<body>\n<a href=\"connectagent://launch\"
-        id=\"notify-agent\" style=\"display: none\" tabindex=\"-1\"><!-- dummy comment
-        --></a>\n\n\n\n<div class=\"connect-container\">\n\n    <nav class=\"main-nav
-        hide\"><!-- main navigation --></nav>\n\n    <div class=\"react-global-modal\"><!--
-        react-global-modal --></div>\n\n    <div class=\"main-body\">\n        <!--
-        Header -->\n        \n\n    <header class=\"header hide\">\n        <!-- placeholder
-        -->\n    </header>\n\n    <section class=\"beta-testers-survey-banner takeover-container\">\n
-        \       <!-- placeholder -->\n    </section>\n\n\n<div class=\"main-header\"></div>\n\n\n
-        \       <!-- Content Container -->\n        \n<div class=\"content clearfix\">\n\n
-        \   \n    <script>\n        window.VIEWER_USERPREFERENCES = {\"heartRateFormat\":{\"formatKey\":\"bpm\",\"formatId\":21,\"maxFraction\":0,\"displayFormat\":null,\"groupingUsed\":false,\"minFraction\":0},\"golfSpeedUnit\":null,\"dateFormat\":{\"formatKey\":\"mmddyyyy\",\"formatId\":23,\"maxFraction\":0,\"displayFormat\":\"EEE,
-        MMM d, yyyy\",\"groupingUsed\":false,\"minFraction\":0},\"displayName\":\"acamus\",\"golfDistanceUnit\":\"statute_us\",\"timeZone\":\"America\\/Chicago\",\"hydrationContainers\":[],\"hydrationMeasurementUnit\":\"milliliter\",\"powerFormat\":{\"formatKey\":\"watt\",\"formatId\":30,\"maxFraction\":0,\"displayFormat\":null,\"groupingUsed\":true,\"minFraction\":0},\"numberFormat\":\"decimal_period\",\"firstDayOfWeek\":{\"dayName\":\"sunday\",\"isPossibleFirstDay\":true,\"sortOrder\":2,\"dayId\":2},\"timeFormat\":{\"formatKey\":\"time_twenty_four_hr\",\"formatId\":33,\"maxFraction\":0,\"displayFormat\":\"H:mm\",\"groupingUsed\":false,\"minFraction\":0},\"measurementSystem\":\"metric\",\"golfElevationUnit\":null,\"preferredLocale\":\"es\"};\n
-        \       window.VIEWER_SOCIAL_PROFILE = {\"runningTrainingSpeed\":0,\"swimmingTrainingSpeed\":0,\"showRecentDevice\":false,\"twitterUrl\":null,\"levelIsViewed\":false,\"bio\":null,\"activityStartVisibility\":\"private\",\"cyclingTrainingSpeed\":0,\"showHeight\":false,\"showBadges\":true,\"levelUpdateDate\":\"2020-12-12T15:20:38.0\",\"id\":3154645,\"showRecentFavorites\":false,\"makeGolfScorecardsPrivate\":true,\"activityHeartRateVisibility\":\"public\",\"profileVisibility\":\"private\",\"nameApproved\":true,\"garminGUID\":\"0690cc1d-d23d-4412-b027-80fd4ed1c0f6\",\"otherMotivation\":null,\"showAgeRange\":false,\"showLifetimeTotals\":false,\"favoriteCyclingActivityTypes\":[],\"cyclingClassification\":null,\"otherPrimaryActivity\":null,\"userPointOffset\":0,\"userRoles\":[\"ROLE_OUTDOOR_USER\",\"ROLE_CONNECTUSER\",\"ROLE_FITNESS_USER\",\"ROLE_WELLNESS_USER\",\"ROLE_CONNECT_2_USER\",\"ROLE_TACX_APP_USER\"],\"profileId\":2591602,\"showActivityClass\":false,\"profileImageUrlSmall\":\"https:\\/\\/s3.amazonaws.com\\/garmin-connect-prod\\/profile_images\\/6302f021-0ec7-4dc9-b0c3-d5a19bc5a08c-2591602.png\",\"showRecentGear\":false,\"showLast12Months\":false,\"showGender\":false,\"displayName\":\"acamus\",\"personalWebsite\":null,\"motivation\":null,\"primaryActivity\":null,\"facebookUrl\":null,\"userLevel\":3,\"userPro\":false,\"favoriteActivityTypes\":[],\"courseVisibility\":\"public\",\"profileImageUuid\":\"73240e81-6e4d-43fc-8af8-c8f6c51b3b8f\",\"userPoint\":117,\"badgeVisibility\":\"private\",\"fullName\":\"Albert
-        Camus\",\"showWeightClass\":false,\"allowGolfScoringByConnections\":true,\"levelPointThreshold\":140,\"userName\":\"acamus\",\"showVO2Max\":false,\"allowGolfLiveScoring\":false,\"profileImageUrlMedium\":\"https:\\/\\/s3.amazonaws.com\\/garmin-connect-prod\\/profile_images\\/685a19e9-a7be-4a11-9bf9-faca0c5d1f1a-2591602.png\",\"otherActivity\":null,\"showUpcomingEvents\":false,\"showAge\":false,\"profileImageUrlLarge\":\"https:\\/\\/s3.amazonaws.com\\/garmin-connect-prod\\/profile_images\\/73240e81-6e4d-43fc-8af8-c8f6c51b3b8f-2591602.png\",\"location\":\"Ciudad
-        de M\xE9xico, CDMX\",\"showPersonalRecords\":false,\"activityMapVisibility\":\"public\",\"userProfileFullName\":\"Albert
-        Camus\",\"cyclingMaxAvgPower\":0,\"showWeight\":false,\"activityPowerVisibility\":\"public\"};\n
-        \       window.VIEWER_DASHBOARDS = [{\"dashboardTitle\":\"\",\"dashboardId\":3282008,\"dashboardOrder\":0,\"ownerId\":2591602,\"dashboardTitleKey\":\"fitness_dashboard\"},{\"dashboardTitle\":\"\",\"dashboardId\":55801129,\"dashboardOrder\":1,\"ownerId\":2591602,\"dashboardTitleKey\":\"wellness_dashboard\"},{\"dashboardTitle\":\"\",\"dashboardId\":55801130,\"dashboardOrder\":2,\"ownerId\":2591602,\"dashboardTitleKey\":\"golf_dashboard\"}];\n\n
-        \       window.queueNotificationTimeout = 600000;\n        window.queuePollRate
-        = 600000;\n\n        window.ERROR_VIEW = null;\n        window.USER_PROFILE
-        = null;\n\n        window.viewerIsAuthenticated = true;\n\n        window.SYSTEM_TIME_GMT
-        = 1690031871925;\n        window.SESSION_LENGTH = 2700000;\n        window.GAUTH_HOST
-        = \"https:\\/\\/sso.garmin.com\\/sso\";\n        window.GARMIN_APP_URL = \"https:\\/\\/apps.garmin.com\\/connect?locale={locale}\";\n
-        \       window.WEB_TOKEN = \"\";\n        window.URL_BUST_VALUE = \"4.69.0.17\";\n\n
-        \       window.IS_READONLY = null;\n        window.PRODUCT_SUPPORT_MODE =
-        null;\n\n        window.JS_ERROR = true;\n        window.DI_BACKENDS = {\"golf\":\"golf.garmin.com\",\"ghs\":\"ghs.connect.garmin.com\",\"insights\":\"insights.gcs.garmin.com\",\"gcs\":\"api.gcs.garmin.com\",\"gcapi\":\"connectapi.garmin.com\",\"omt\":\"omt.garmin.com\",\"gcsalt\":\"gcs.garmin.com\",\"atp\":\"atp.gcs.garmin.com\"};\n
-        \       window.PREFERENCES = {\"ce34657d-8a85-4b6e-8bb4-00897590c217\":\"ROLE_DI_TESTER\",\"5c8d3401-e6e7-4354-9095-39526016a47c\":\"ROLE_CONNECTUSER\",\"d3c94498-8962-4a62-bd3a-0d80a08e3386\":\"false\",\"7ae52c9a-1967-46e9-952f-3e40e3770bde\":\"ROLE_DI_TESTER\"};\n
-        \   </script>\n\n    <script src=\"/web-react/static/js/vendor.js?bust=4.69.0.17\"></script>\n
-        \   <script src=\"/web-react/static/js/backbone-lib.js?bust=4.69.0.17\"></script>\n
-        \   <script src=\"/web-react/static/js/bundle.js?bust=4.69.0.17\"></script>\n</div>\n\n
-        \       <!-- END .content -->\n\n        <!-- Footer -->\n        <div class=\"main-footer\"></div>\n
-        \       <!-- END .footer -->\n        <p style=\"display: none;\" id=\"garmin-connect-version\">4.69.0.17</p>\n
-        \   </div>\n\n    <!-- END .container -->\n</div>\n\n<style>\n    .privacy-overlay
-        {\n        position: fixed; /* Sit on top of the page content */\n        width:
-        100%; /* Full width (cover the whole page) */\n        height: 100%; /* Full
-        height (cover the whole page) */\n        top: 0;\n        left: 0;\n        background-color:
-        #fff;\n        z-index: 9999; /* Specify a stack order in case you're using
-        a different order for other elements */\n    }\n</style>\n\n<div id=\"overlay\"
-        class=\"privacy-overlay\">\n</div>\n\n<script defer src=\"https://static.cloudflareinsights.com/beacon.min.js/v2cb3a2ab87c5498db5ce7e6608cf55231689030342039\"
-        integrity=\"sha512-DI3rPuZDcpH/mSGyN22erN5QFnhl760f50/te7FTIYxodEF8jJnSFnfnmG/c+osmIQemvUrnBtxnMpNdzvx1/g==\"
-        data-cf-beacon='{\"rayId\":\"7eabf75a488b1547\",\"version\":\"2023.4.0\",\"b\":1,\"token\":\"1bd18b8f69214e379ef7bd34509191ae\",\"si\":100}'
-        crossorigin=\"anonymous\"></script>\n</body>\n\n\n\n</html>"
+      string: oauth_token=SANITIZED&oauth_token_secret=SANITIZED&mfa_token=SANITIZED&mfa_expiration_timestamp=2023-08-03
+        15:44:35.000
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7eabf75a488b1547-QRO
+      - 7f0eff0a3f4f1557-QRO
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
-      - text/html;charset=UTF-8
+      - text/plain;charset=utf-8
       Date:
-      - Sat, 22 Jul 2023 13:17:51 GMT
+      - Thu, 03 Aug 2023 13:44:36 GMT
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=mHxILkyoUvQ7guqKTqL4aC%2Fx%2BxF0OtAi7wckNzEF%2B7n2aSCf2HaqKRDvNBKgC8erF7S%2FVHBc3e1IJhtHmEupc%2FAWH9ID362jzILvtRdllqO9ocCPsLnPwT9D27SOyPH1Uq8H8Q%3D%3D"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=wx6PD3r3tVRMWclSoxaB3Dm82pfy4XmhSvh7od0%2Fux%2FJHi7FudxJADY%2BICt8sKbMK%2B1ywjlmylnj70wO6I4LEL4btzHWgNKZ9LG5aKSKn00w0ZqqHRQiT93c9DptWX7WY24hqz9V8Q%3D%3D"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
+      Set-Cookie:
+      - _cfuvid=SANITIZED; path=SANITIZED; domain=SANITIZED; HttpOnly; Secure; SameSite=SANITIZED
       Transfer-Encoding:
       - chunked
-      cache-control:
-      - no-cache, no-store, max-age=0, must-revalidate
-      content-language:
-      - en-US
-      expires:
-      - '0'
-      pragma:
-      - no-cache
-      set-cookie:
-      - ADRUM_BTa=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
-        Secure
-      - ADRUM_BTa=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
-        Secure
-      - ADRUM_BTa=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
-        Secure
-      - SameSite=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
-        Secure
-      - ADRUM_BT1=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
-        Secure
-      - ADRUM_BT1=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
-        Secure
-      strict-transport-security:
-      - max-age=31536000 ; includeSubDomains
-      x-content-type-options:
-      - nosniff
-      x-frame-options:
-      - DENY
-      x-vcap-request-id:
-      - 35da0075-f093-4460-5627-51c31a9caf90
-      x-xss-protection:
-      - 1; mode=block
+      alt-svc:
+      - h3=":443"; ma=86400
     status:
       code: 200
       message: OK
 - request:
-    body: null
+    body: ''
     headers:
       Accept:
-      - '*/*'
+      - !!binary |
+        Ki8q
       Accept-Encoding:
-      - gzip, deflate
+      - !!binary |
+        Z3ppcCwgZGVmbGF0ZQ==
+      Authorization:
+      - Bearer SANITIZED
       Connection:
-      - keep-alive
+      - !!binary |
+        a2VlcC1hbGl2ZQ==
       Content-Length:
-      - '0'
-      Cookie:
-      - _cfuvid=SANITIZED; GARMIN-SSO=SANITIZED; GARMIN-SSO-CUST-GUID=SANITIZED; GARMIN-SSO-GUID=SANITIZED;
-        GarminNoCache=SANITIZED; ADRUM_BT1=SANITIZED; ADRUM_BTa=SANITIZED; SESSIONID=SANITIZED;
-        SameSite=SANITIZED; __cflb=SANITIZED
+      - !!binary |
+        MA==
+      Content-Type:
+      - !!binary |
+        YXBwbGljYXRpb24veC13d3ctZm9ybS11cmxlbmNvZGVk
       User-Agent:
-      - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X) AppleWebKit/605.1.15
-        (KHTML, like Gecko) Mobile/15E148
-      referer:
-      - https://connect.garmin.com/modern
+      - !!binary |
+        Y29tLmdhcm1pbi5hbmRyb2lkLmFwcHMuY29ubmVjdG1vYmlsZQ==
     method: POST
-    uri: https://connect.garmin.com/modern/di-oauth/exchange
+    uri: https://connectapi.garmin.com/oauth-service/oauth/exchange/user/2.0
   response:
     body:
-      string: '{"scope": "COMMUNITY_COURSE_READ GOLF_API_READ GHS_HID ATP_READ GHS_SAMD
-        INSIGHTS_READ COMMUNITY_COURSE_WRITE CONNECT_WRITE DIVE_SHARED_READ GHS_REGISTRATION
-        GOLF_API_WRITE INSIGHTS_WRITE PRODUCT_SEARCH_READ GOLF_SHARED_READ CONNECT_NON_SOCIAL_SHARED_READ
-        CONNECT_READ ATP_WRITE", "jti": "SANITIZED", "access_token":
+      string: '{"scope": "COMMUNITY_COURSE_READ GARMINPAY_WRITE GOLF_API_READ ATP_READ
+        GHS_SAMD GHS_UPLOAD INSIGHTS_READ COMMUNITY_COURSE_WRITE CONNECT_WRITE GCOFFER_WRITE
+        GARMINPAY_READ DT_CLIENT_ANALYTICS_WRITE GOLF_API_WRITE INSIGHTS_WRITE PRODUCT_SEARCH_READ
+        GCOFFER_READ CONNECT_READ ATP_WRITE", "jti": "SANITIZED", "access_token":
         "SANITIZED", "token_type": "Bearer", "refresh_token": "SANITIZED", "expires_in":
-        3599, "refresh_token_expires_in": 7199}'
+        95631, "refresh_token_expires_in": 2591999}'
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7eabf7602f9a155e-QRO
+      - 7f0eff0daa741547-QRO
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json
       Date:
-      - Sat, 22 Jul 2023 13:17:52 GMT
+      - Thu, 03 Aug 2023 13:44:37 GMT
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=5Kfbn7%2BM%2FJURIaBxa7p3O8VlzRLjIw9unm4J%2FoM8Gxh9IuGYjDwT9zipvqjh%2BpdrwkoewEYRSCa%2FmwEsYsM5kTjjNPNJvsWgIEi%2FRBTMo1qYfyimlmZ5jNy12mxDoHallpwvDg%3D%3D"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=UWx0LW8l%2Bzswc3LmvfMCaKHSQvKAeBn6tXX2wu0jpjPXnK%2Bvyt9%2FibwHSbLvJa43YjJXG8MWRYH5CcV9M1TCjuDE%2BwQ5kMIO684fQExIQLiGQQLqC7OR%2FBjXjV%2BY4ItI3sYempKLpQ%3D%3D"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
+      Set-Cookie:
+      - _cfuvid=SANITIZED; path=SANITIZED; domain=SANITIZED; HttpOnly; Secure; SameSite=SANITIZED
       Transfer-Encoding:
       - chunked
+      alt-svc:
+      - h3=":443"; ma=86400
       cache-control:
       - no-cache, no-store, private
       pragma:
       - no-cache
-      set-cookie:
-      - ADRUM_BT1=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
-        Secure
-      - ADRUM_BTa=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
-        Secure
-      - ADRUM_BTa=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
-        Secure
-      - ADRUM_BTa=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
-        Secure
-      - SameSite=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
-        Secure
-      - ADRUM_BT1=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
-        Secure
-      - ADRUM_BT1=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
-        Secure
-      - JWT_FGP=SANITIZED; SameSite=SANITIZED; HttpOnly; Secure; Max-Age=SANITIZED;
-        Domain=SANITIZED; Path=SANITIZED
-      strict-transport-security:
-      - max-age=31536000 ; includeSubDomains
-      x-content-type-options:
-      - nosniff
-      x-frame-options:
-      - DENY
-      x-vcap-request-id:
-      - f29cd951-1c6f-461b-73a5-aa1ae2e83a86
-      x-xss-protection:
-      - 1; mode=block
     status:
       code: 200
       message: OK
 version: 1
```

#### html2text {}

```diff
@@ -1,23 +1,25 @@
 interactions: - request: body: null headers: Accept: - '*/*' Accept-Encoding: -
 gzip, deflate Connection: - keep-alive User-Agent: - Mozilla/5.0 (iPhone; CPU
 iPhone OS 16_5 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Mobile/
-15E148 method: GET uri: https://sso.garmin.com/sso/embed?id=gauth-
+15E148 referer: - https://sso.garmin.com/sso/signin?id=gauth-
+widget&service=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&source=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountLoginUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountCreationUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&gauthHost=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed
+method: GET uri: https://sso.garmin.com/sso/embed?id=gauth-
 widget&embedWidget=true&gauthHost=https%3A%2F%2Fsso.garmin.com%2Fsso response:
 body: string: "
 \n\t
 \n\t
 \n\t
 \n\t
 \n\t
 \n\t
 \n\t\t
 \n\n
 \n\t
-\tERROR:
+\n\tERROR:
         clientId parameter must be specified!!!\n\n\tUsage: https://
 sso.garmin.com/sso/embed?clientId=<clientId>&locale=<locale>...\n\n\tRequest
         parameter configuration options:\n\n\tNAME
 REQ  VALUES
         \                                                  DESCRIPTION\n\t-----
 -------------
         \            ---  -----------------------------------------------------
@@ -249,30 +251,30 @@
 \n
 \n\n\n\t
 \n
 \n" headers: Access-Control-Allow-Credentials: - 'true' Access-Control-Allow-
 Headers: - Access-Control-Allow-Headers, Origin,Accept, X-Requested-With,
 Content-Type, Access-Control-Request-Method, Access-Control-Request-Headers
 Access-Control-Allow-Methods: - GET,POST,OPTIONS Access-Control-Allow-Origin: -
-https://www.garmin.com CF-Cache-Status: - DYNAMIC CF-RAY: - 7eabf6a32a5c154d-
+https://www.garmin.com CF-Cache-Status: - DYNAMIC CF-RAY: - 7f0efe9dbf82154b-
 QRO Connection: - keep-alive Content-Encoding: - gzip Content-Language: - en
-Content-Type: - text/html;charset=UTF-8 Date: - Sat, 22 Jul 2023 13:17:21 GMT
+Content-Type: - text/html;charset=UTF-8 Date: - Thu, 03 Aug 2023 13:44:18 GMT
 NEL: - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
 Report-To: - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/
-v3?s=l1YU%2FguiBx%2F1g1xDpU%2F5YIjbg62ZZ3rMm%2BSnK6Wr%2FxNlnlRlOKIjwhtJ6nqoxxvyfvQD4neAYxVssEL8HbZ8BUZf2qMZp5iq9Z4jE8p43%2F0eZGBeibBjsWvCRSrzcvgV"}],"group":
+v3?s=EpNuus5s1jsWqmwuAEQuwmJKl4R4x7yKry6fR6Y7YC6inOY0FhOQEkhOEsVh%2FjT2slREgwE8mXWp21snNnLiSMNaYAg%2FXMYN7%2BQXy%2FyZGKBPH63E5AJ7ggao6H0iXiXh"}],"group":
 "cf-nel","max_age":604800}' Server: - cloudflare Set-Cookie: -
 org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED;
 Path=SANITIZED - __cf_bm=SANITIZED; path=SANITIZED; expires=SANITIZED;
 domain=SANITIZED; HttpOnly; Secure; SameSite=SANITIZED - __cflb=SANITIZED;
 SameSite=SANITIZED; Secure; path=SANITIZED; expires=SANITIZED; HttpOnly -
 _cfuvid=SANITIZED; path=SANITIZED; domain=SANITIZED; HttpOnly; Secure;
 SameSite=SANITIZED Transfer-Encoding: - chunked X-Application-Context: -
-casServer:cloud,prod,prod-US_1102:0 X-B3-Traceid: -
-4bcb3c9643d8af9105a3b8f5106dd4c8 X-Robots-Tag: - noindex X-Vcap-Request-Id: -
-a50b6016-803e-446f-7475-bfb91f1e1b42 status: code: 200 message: OK - request:
+casServer:cloud,prod,prod-US_1102:4 X-B3-Traceid: -
+41fd0fc56c11edb61c8a219b7d5e8aab X-Robots-Tag: - noindex X-Vcap-Request-Id: -
+63aed3d0-af94-4f44-791e-87b33f700916 status: code: 200 message: OK - request:
 body: null headers: Accept: - '*/*' Accept-Encoding: - gzip, deflate
 Connection: - keep-alive Cookie: - __cf_bm=SANITIZED; _cfuvid=SANITIZED;
 __cflb=SANITIZED;
 org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED
 User-Agent: - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X)
 AppleWebKit/605.1.15 (KHTML, like Gecko) Mobile/15E148 referer: - https://
 sso.garmin.com/sso/embed?id=gauth-
@@ -333,59 +335,59 @@
 \n\t\t\n\n
 \n
 \n
 \n" headers: Access-Control-Allow-Credentials: - 'true' Access-Control-Allow-
 Headers: - Access-Control-Allow-Headers, Origin,Accept, X-Requested-With,
 Content-Type, Access-Control-Request-Method, Access-Control-Request-Headers
 Access-Control-Allow-Methods: - GET,POST,OPTIONS Access-Control-Allow-Origin: -
-https://www.garmin.com CF-Cache-Status: - DYNAMIC CF-Ray: - 7eabf6a40e19155e-
+https://www.garmin.com CF-Cache-Status: - DYNAMIC CF-Ray: - 7f0efe9ed8421547-
 QRO Connection: - keep-alive Content-Encoding: - gzip Content-Language: - en
-Content-Type: - text/html;charset=UTF-8 Date: - Sat, 22 Jul 2023 13:17:22 GMT
+Content-Type: - text/html;charset=UTF-8 Date: - Thu, 03 Aug 2023 13:44:19 GMT
 NEL: - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
 Report-To: - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/
-v3?s=CQ3oC1HTh0k%2FNSK9wGKMHOsluRQqlFNr9IITbKz%2FA73VEQnPd6Mt1HBJcFkAefSIICX54I7tz3oCMSHX2OJXnG7XETMpw4bdWb89nS8dhRj1CePYqnjtWBm%2Fj%2Fl8eR%2BR"}],"group":
+v3?s=pUFwZ3E%2F0mJFNFwFoMN7HO5XgGTMP6zxm53htk%2Fdysfp324tli1JN8eL05f4Y1OzTbq%2FlPJr3Ky177Ui6fqBrdPOJs4Iuoi%2Fu6RfDU0p6ku8mha7OD5ihAwayz8H18hH"}],"group":
 "cf-nel","max_age":604800}' Server: - cloudflare Set-Cookie: -
 org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED;
 Path=SANITIZED - SESSION=SANITIZED; Path=SANITIZED; Secure; HttpOnly -
 __VCAP_ID__=SANITIZED; Path=SANITIZED; HttpOnly; Secure Transfer-Encoding: -
 chunked Vary: - Accept-Encoding X-Application-Context: - casServer:
-cloud,prod,prod-US_1102:6 X-B3-Traceid: - 6cdee7e9a11c667860bfa9846e37e8cf X-
-Robots-Tag: - noindex X-Vcap-Request-Id: - fafd78c0-5351-4d16-649e-b5ef7df2e71f
+cloud,prod,prod-US_1102:5 X-B3-Traceid: - 0c7105857742ac230da0842492b92d1d X-
+Robots-Tag: - noindex X-Vcap-Request-Id: - ba3d4826-a22e-49aa-7888-d62b15cc43b6
 status: code: 200 message: OK - request: body:
-username=SANITIZED&password=SANITIZED&embed=true&_csrf=5E7E6502AEE2D23AF79C538FD3191F4FE6C8A3383F959F11D045459C9A01445EB2086A0CB8A5AB091E99AF71ABDE96A55619
+username=SANITIZED&password=SANITIZED&embed=true&_csrf=085E32B1AAC1E7C4FEE1CCA0CE94D87C4F295B638C604CD3637E11B1D90C2A9992FE5B6DF974136AB8FC45E97D508322F317
 headers: Accept: - '*/*' Accept-Encoding: - gzip, deflate Connection: - keep-
-alive Content-Length: - '179' Content-Type: - application/x-www-form-urlencoded
+alive Content-Length: - '177' Content-Type: - application/x-www-form-urlencoded
 Cookie: - SESSION=SANITIZED; __cf_bm=SANITIZED; _cfuvid=SANITIZED;
 __VCAP_ID__=SANITIZED; __cflb=SANITIZED;
 org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED
 User-Agent: - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X)
 AppleWebKit/605.1.15 (KHTML, like Gecko) Mobile/15E148 referer: - https://
 sso.garmin.com/sso/signin?id=gauth-
 widget&service=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&source=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountLoginUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountCreationUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&gauthHost=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed
 method: POST uri: https://sso.garmin.com/sso/signin?id=gauth-
 widget&service=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&source=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountLoginUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountCreationUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&gauthHost=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed
 response: body: string: '' headers: Access-Control-Allow-Credentials: - 'true'
 Access-Control-Allow-Headers: - Access-Control-Allow-Headers, Origin,Accept, X-
 Requested-With, Content-Type, Access-Control-Request-Method, Access-Control-
 Request-Headers Access-Control-Allow-Methods: - GET,POST,OPTIONS Access-
 Control-Allow-Origin: - https://www.garmin.com CF-Cache-Status: - DYNAMIC CF-
-Ray: - 7eabf6a8090c154b-QRO Connection: - keep-alive Content-Language: - en
-Content-Length: - '0' Date: - Sat, 22 Jul 2023 13:17:23 GMT Location: - https:/
+Ray: - 7f0efea05a41155e-QRO Connection: - keep-alive Content-Language: - en
+Content-Length: - '0' Date: - Thu, 03 Aug 2023 13:44:20 GMT Location: - https:/
 /sso.garmin.com/sso/verifyMFA/loginEnterMfaCode?id=gauth-
 widget&service=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&source=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountLoginUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountCreationUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&gauthHost=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed
 NEL: - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
 Report-To: - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/
-v3?s=9sa%2B94IsrfhOYrutSbeTXXGssqrHARDtqjlz0h9pIVaJGsGl5%2B6ssqI7awvmnQ%2FR9E3icbmEw2rHgb3oBbaK%2BRtT4izEaZfCDMWH14YxH2nPExHUPv3Gf%2F0Sj%2BHF34uV"}],"group":
+v3?s=vZ9OuYl3ehAIn6QRonsHx3lnITP4uLKmQn0RBoyd46XkiNYBeslEOPJz9aPo%2BYnt4ICK9fi2l0m6VI7aXMQSlM5H5sWUeD9DVN1fZtehugkdvNWbk3995Vi4BP6OTPzK"}],"group":
 "cf-nel","max_age":604800}' Server: - cloudflare Set-Cookie: -
 org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED;
 Path=SANITIZED - __cfruid=SANITIZED; path=SANITIZED; domain=SANITIZED;
 HttpOnly; Secure; SameSite=SANITIZED Vary: - Accept-Encoding X-Application-
-Context: - casServer:cloud,prod,prod-US_1102:6 X-B3-Traceid: -
-6f291b41c689480125ea4efbd2e9c4db X-Robots-Tag: - noindex X-Vcap-Request-Id: -
-68b98295-0675-4da0-752f-384933dfa674 status: code: 302 message: Found -
+Context: - casServer:cloud,prod,prod-US_1102:5 X-B3-Traceid: -
+6c198084522013542873ac2373afbacf X-Robots-Tag: - noindex X-Vcap-Request-Id: -
+154052d5-8818-447a-7151-48678d95a078 status: code: 302 message: Found -
 request: body: null headers: Accept: - '*/*' Accept-Encoding: - gzip, deflate
 Connection: - keep-alive Cookie: - SESSION=SANITIZED; __cf_bm=SANITIZED;
 _cfuvid=SANITIZED; __cfruid=SANITIZED; __VCAP_ID__=SANITIZED; __cflb=SANITIZED;
 org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED
 User-Agent: - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X)
 AppleWebKit/605.1.15 (KHTML, like Gecko) Mobile/15E148 referer: - https://
 sso.garmin.com/sso/signin?id=gauth-
@@ -459,27 +461,27 @@
 \n
 \n
 \n
 " headers: Access-Control-Allow-Credentials: - 'true' Access-Control-Allow-
 Headers: - Access-Control-Allow-Headers, Origin,Accept, X-Requested-With,
 Content-Type, Access-Control-Request-Method, Access-Control-Request-Headers
 Access-Control-Allow-Methods: - GET,POST,OPTIONS Access-Control-Allow-Origin: -
-https://www.garmin.com CF-Cache-Status: - DYNAMIC CF-RAY: - 7eabf6b0fe29155e-
+https://www.garmin.com CF-Cache-Status: - DYNAMIC CF-RAY: - 7f0efeaa1972b6e1-
 QRO Connection: - keep-alive Content-Encoding: - gzip Content-Language: - en
-Content-Type: - text/html;charset=UTF-8 Date: - Sat, 22 Jul 2023 13:17:24 GMT
+Content-Type: - text/html;charset=UTF-8 Date: - Thu, 03 Aug 2023 13:44:20 GMT
 NEL: - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
 Report-To: - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/
-v3?s=g8E68j1rLeP0R%2FMBPy9zpml0vo9xOoxPEB1t1zaTqHLPlLWn8zVNh9DCvmlH0rnrMmruwu3wVXalDkd9Yxx4QaW%2B0mLRS1kGh1QKh6E9rZKD0Rm%2FJ1yKhqtNugETLijh"}],"group":
+v3?s=GAfA2uzl%2F0ZTzFGx6iieBcuC3Bs9Fp%2FrU87lPm%2BoacZdwC9Yj6Y5IYXwyD%2FvuiGhzM3aMcWBJyq7akJUlX3iM5mTQZGqKMkD5QP4Yr0Wp%2BIZJe3repljvx%2FadT%2Bzhdjg"}],"group":
 "cf-nel","max_age":604800}' Server: - cloudflare Set-Cookie: -
 org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED;
 Path=SANITIZED Transfer-Encoding: - chunked X-Application-Context: - casServer:
-cloud,prod,prod-US_1102:6 X-B3-Traceid: - 5ae0bda06a5038f24f92e204833608df X-
-Robots-Tag: - noindex X-Vcap-Request-Id: - 957f32c6-c5bb-4985-46bd-172bdc444f14
+cloud,prod,prod-US_1102:5 X-B3-Traceid: - 32f6eaa23f7f351b363bc86bb39d27ce X-
+Robots-Tag: - noindex X-Vcap-Request-Id: - d31fc9af-b2cb-4c64-4031-bd85769894e5
 status: code: 200 message: OK - request: body: mfa-
-code=327751&embed=true&_csrf=EE0189695747008B2E8EC630641D96EBB1B72977B0C369036002A33EA331E53ABB97DD11393EAD9545E7DD7684AF4EC1CA6D&fromPage=setupEnterMfaCode
+code=884445&embed=true&_csrf=ED28063867B6DC6292FDDAFD2EE1C1803C77B15CF598FE3CA38ED40784D19D3B3555BBC20B72DE2727D377FDC8793AA43259&fromPage=setupEnterMfaCode
 headers: Accept: - '*/*' Accept-Encoding: - gzip, deflate Connection: - keep-
 alive Content-Length: - '160' Content-Type: - application/x-www-form-urlencoded
 Cookie: - SESSION=SANITIZED; __cf_bm=SANITIZED; __cfruid=SANITIZED;
 _cfuvid=SANITIZED; __VCAP_ID__=SANITIZED; __cflb=SANITIZED;
 org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED
 User-Agent: - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X)
 AppleWebKit/605.1.15 (KHTML, like Gecko) Mobile/15E148 referer: - https://
@@ -489,37 +491,37 @@
 loginEnterMfaCode?id=gauth-
 widget&service=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&source=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountLoginUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountCreationUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&gauthHost=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&rememberMyBrowserChecked=true
 response: body: string: '' headers: Access-Control-Allow-Credentials: - 'true'
 Access-Control-Allow-Headers: - Access-Control-Allow-Headers, Origin,Accept, X-
 Requested-With, Content-Type, Access-Control-Request-Method, Access-Control-
 Request-Headers Access-Control-Allow-Methods: - GET,POST,OPTIONS Access-
 Control-Allow-Origin: - https://www.garmin.com CF-Cache-Status: - DYNAMIC CF-
-RAY: - 7eabf74b3aa4154d-QRO Connection: - keep-alive Content-Language: - en
-Content-Length: - '0' Date: - Sat, 22 Jul 2023 13:17:49 GMT Location: - https:/
+RAY: - 7f0efefd9b09b6e8-QRO Connection: - keep-alive Content-Language: - en
+Content-Length: - '0' Date: - Thu, 03 Aug 2023 13:44:34 GMT Location: - https:/
 /sso.garmin.com/sso/
-login?logintoken=ustnTKB9hK&service=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&locale=en&embed=true&source=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountLoginUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&rememberMyBrowserChecked=true
+login?logintoken=KBDAhvPbGI&service=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&locale=en&embed=true&source=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountLoginUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&rememberMyBrowserChecked=true
 NEL: - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
 Report-To: - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/
-v3?s=K9tIqLG7fuNHYcgAO9jFQJj9ioDVaFG6Y2KIub1JxJXjn%2BoU6vQnYpcJk18bxap5NnmsaAtiqTUvVQm6W7691UB6GNXdqPsaFpCRVLR0Ovbxd65QuxturFaHBjIbVjFP"}],"group":
+v3?s=agJu1oZ7N7%2Fv7KL7B9%2BF6aIm4EnHWTgYtuAlIidaNhYJOYS1h6rSyhD2Ioh4nbgIyaoBuBcF24b7PfZlzbHGBzWck%2ForkSXc4uSuDIJ7sJabXyyXqAbZLZNk8BrKsDFQ"}],"group":
 "cf-nel","max_age":604800}' Server: - cloudflare Set-Cookie: -
 org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED;
-Path=SANITIZED X-Application-Context: - casServer:cloud,prod,prod-US_1102:6 X-
-B3-Traceid: - 2426e7929a0b1017558efe6effdc3dc4 X-Robots-Tag: - noindex X-Vcap-
-Request-Id: - ba2a58f1-907d-49ff-6dcc-3249eb3600da status: code: 302 message:
+Path=SANITIZED X-Application-Context: - casServer:cloud,prod,prod-US_1102:5 X-
+B3-Traceid: - 4d99b5adfb5f4e0e5c5d3cb0167df354 X-Robots-Tag: - noindex X-Vcap-
+Request-Id: - e7aeda65-91ba-49b3-64aa-f2f6f09d5f87 status: code: 302 message:
 Found - request: body: null headers: Accept: - '*/*' Accept-Encoding: - gzip,
 deflate Connection: - keep-alive Cookie: - SESSION=SANITIZED;
 __cf_bm=SANITIZED; __cfruid=SANITIZED; _cfuvid=SANITIZED;
 __VCAP_ID__=SANITIZED; __cflb=SANITIZED;
 org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED
 User-Agent: - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X)
 AppleWebKit/605.1.15 (KHTML, like Gecko) Mobile/15E148 referer: - https://
 sso.garmin.com/sso/verifyMFA/loginEnterMfaCode?id=gauth-
 widget&service=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&source=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountLoginUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountCreationUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&gauthHost=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed
 method: GET uri: https://sso.garmin.com/sso/
-login?logintoken=ustnTKB9hK&service=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&locale=en&embed=true&source=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountLoginUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&rememberMyBrowserChecked=true
+login?logintoken=KBDAhvPbGI&service=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&locale=en&embed=true&source=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountLoginUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&rememberMyBrowserChecked=true
 response: body: string: "
 \n
 \n\t
 \n\t\t
 \n\t\t
 \n\t\t
 \n\t\t
@@ -538,20 +540,20 @@
 \n\t\t
 \n\t
 \n
 \n" headers: Access-Control-Allow-Credentials: - 'true' Access-Control-Allow-
 Headers: - Access-Control-Allow-Headers, Origin,Accept, X-Requested-With,
 Content-Type, Access-Control-Request-Method, Access-Control-Request-Headers
 Access-Control-Allow-Methods: - GET,POST,OPTIONS Access-Control-Allow-Origin: -
-https://www.garmin.com CF-Cache-Status: - DYNAMIC CF-Ray: - 7eabf74df808b6ee-
+https://www.garmin.com CF-Cache-Status: - DYNAMIC CF-Ray: - 7f0eff037e33b6df-
 QRO Connection: - keep-alive Content-Encoding: - gzip Content-Language: - en
-Content-Type: - text/html;charset=UTF-8 Date: - Sat, 22 Jul 2023 13:17:49 GMT
+Content-Type: - text/html;charset=UTF-8 Date: - Thu, 03 Aug 2023 13:44:35 GMT
 NEL: - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
 Report-To: - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/
-v3?s=tp1gIVjSm6qBwb1nJt7eiEqo2Ncx%2FrQ0%2FSUe7q5Qfht2n41OljThJdqteykR%2B7xjMPm5vi7aJMbdMO7QetYywkSLuSVKHQsRpqAr6mxPjjlgCHeAy%2BLOXDkC%2FKOI%2BK3m"}],"group":
+v3?s=Zrk%2F09QvnWGN7H99r%2BKA274jAsm%2FYB8g1ws29goFETQcejOoUds2wKIJ1khOezReb76fYOVVuqTCK1qDo5Zl0PHfA5JM3T2BgYO%2BA45%2BzBAq3yYfS11ZEmcSnwZTnUY%2F"}],"group":
 "cf-nel","max_age":604800}' Server: - cloudflare Set-Cookie: -
 org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED;
 Path=SANITIZED - CASTGC=SANITIZED; Path=SANITIZED; Secure; HttpOnly -
 CASTGC=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED; Secure;
 HttpOnly - GARMIN-SSO=SANITIZED; Domain=SANITIZED; Path=SANITIZED - GARMIN-
 SSO=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Domain=SANITIZED;
 Path=SANITIZED - GarminNoCache=SANITIZED; Domain=SANITIZED; Path=SANITIZED -
@@ -563,223 +565,61 @@
 Path=SANITIZED - GARMIN-SSO-GUID=SANITIZED; Max-Age=SANITIZED;
 Expires=SANITIZED; Domain=SANITIZED; Path=SANITIZED - GARMIN-SSO-CUST-
 GUID=SANITIZED; Domain=SANITIZED; Path=SANITIZED - GARMIN-SSO-CUST-
 GUID=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Domain=SANITIZED;
 Path=SANITIZED - CASTGC=SANITIZED; Path=SANITIZED; Secure; HttpOnly -
 CASTGC=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED; Secure;
 HttpOnly Transfer-Encoding: - chunked Vary: - Accept-Encoding X-Application-
-Context: - casServer:cloud,prod,prod-US_1102:6 X-B3-Traceid: -
-7c54b7c38cc2dee514b3f042edc58b70 X-Robots-Tag: - noindex X-Vcap-Request-Id: -
-1815e061-ed52-4481-57d3-daa30f8c7285 status: code: 200 message: OK - request:
+Context: - casServer:cloud,prod,prod-US_1102:5 X-B3-Traceid: -
+69ae874215e7224b59d4c4946d43e589 X-Robots-Tag: - noindex X-Vcap-Request-Id: -
+28d5c20f-0bb1-4775-5681-0eef16703ccd status: code: 200 message: OK - request:
 body: null headers: Accept: - '*/*' Accept-Encoding: - gzip, deflate
-Connection: - keep-alive Cookie: - GARMIN-SSO=SANITIZED; GARMIN-SSO-CUST-
-GUID=SANITIZED; GARMIN-SSO-GUID=SANITIZED; GarminNoCache=SANITIZED User-Agent:
-- Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X) AppleWebKit/605.1.15
-(KHTML, like Gecko) Mobile/15E148 referer: - https://sso.garmin.com/sso/
-login?logintoken=ustnTKB9hK&service=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&locale=en&embed=true&source=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountLoginUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&rememberMyBrowserChecked=true
-method: GET uri: https://connect.garmin.com/modern?ticket=ST-2170356-
-YsbI2WW24tRJOHZr1Lxf-cas response: body: string: '' headers: CF-Cache-Status: -
-DYNAMIC CF-RAY: - 7eabf7512ce51547-QRO Connection: - keep-alive Content-Length:
-- '0' Date: - Sat, 22 Jul 2023 13:17:49 GMT NEL: - '{"success_fraction":
-0.01,"report_to":"cf-nel","max_age":604800}' Report-To: - '{"endpoints":[
-{"url":"https:\/\/a.nel.cloudflare.com\/report\/
-v3?s=GdN%2BNtzsJs0l3W%2B4lXaLYc2rvn6Ct1Vio4L%2F1tVhDOtbtanXdC%2BFGjCFZECxABBRvTH8faMR73qmcSZoXkLUcuUuoM%2FowAYoc7%2BZATuhwWmU4KmZ2%2BWRxWqENnH0KWByRzd2bg%3D%3D"}],"group":
-"cf-nel","max_age":604800}' Server: - cloudflare cache-control: - no-cache, no-
-store, max-age=0, must-revalidate expires: - '0' location: - https://
-connect.garmin.com/modern/ pragma: - no-cache set-cookie: -
-ADRUM_BTa=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
-Secure - ADRUM_BTa=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED;
-Path=SANITIZED; Secure - SameSite=SANITIZED; Max-Age=SANITIZED;
-Expires=SANITIZED; Path=SANITIZED; Secure - SESSIONID=SANITIZED;
-Path=SANITIZED; Secure; HttpOnly; SameSite=SANITIZED - __cflb=SANITIZED;
-SameSite=SANITIZED; Secure; path=SANITIZED; expires=SANITIZED; HttpOnly -
-_cfuvid=SANITIZED; path=SANITIZED; domain=SANITIZED; HttpOnly; Secure;
-SameSite=SANITIZED strict-transport-security: - max-age=31536000 ;
-includeSubDomains x-content-type-options: - nosniff x-frame-options: - DENY x-
-vcap-request-id: - 3a485e27-9f9f-4f55-63f5-e3f97cc42276 x-xss-protection: - 1;
-mode=block status: code: 302 message: Found - request: body: null headers:
-Accept: - '*/*' Accept-Encoding: - gzip, deflate Connection: - keep-alive
-Cookie: - GARMIN-SSO=SANITIZED; GARMIN-SSO-CUST-GUID=SANITIZED; GARMIN-SSO-
-GUID=SANITIZED; GarminNoCache=SANITIZED; ADRUM_BTa=SANITIZED;
-SameSite=SANITIZED; SESSIONID=SANITIZED; __cflb=SANITIZED; _cfuvid=SANITIZED
-User-Agent: - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X)
-AppleWebKit/605.1.15 (KHTML, like Gecko) Mobile/15E148 referer: - https://
-sso.garmin.com/sso/
-login?logintoken=ustnTKB9hK&service=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&locale=en&embed=true&source=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountLoginUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&rememberMyBrowserChecked=true
-method: GET uri: https://connect.garmin.com/modern/ response: body: string: ''
-headers: CF-Cache-Status: - DYNAMIC CF-RAY: - 7eabf75368011547-QRO Connection:
-- keep-alive Content-Length: - '0' Date: - Sat, 22 Jul 2023 13:17:50 GMT NEL: -
-'{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}' Report-To: -
-'{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/
-v3?s=hoKQu4TfUejqzGewvM%2BnlLFRugaVWS7jFSTQVoITtPjl8o425YlC%2BLyxIttsjWWvnYXoyyjWccpJfbJ8Xhklr5%2FTHEKSXmrrWgBzzwBsGDZBvZ5XpXlxctXZEe9Y1mOPp1Jaig%3D%3D"}],"group":
-"cf-nel","max_age":604800}' Server: - cloudflare cache-control: - no-cache, no-
-store, max-age=0, must-revalidate expires: - '0' location: - https://
-sso.garmin.com/sso/
-login?service=https%3A%2F%2Fconnect.garmin.com%2Fmodern%2F&webhost=https%3A%2F%2Fconnect.garmin.com&gateway=true&generateExtraServiceTicket=true&generateTwoExtraServiceTickets=true
-pragma: - no-cache set-cookie: - ADRUM_BTa=SANITIZED; Max-Age=SANITIZED;
-Expires=SANITIZED; Path=SANITIZED; Secure - ADRUM_BTa=SANITIZED; Max-
-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED; Secure - ADRUM_BTa=SANITIZED;
-Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED; Secure -
-SameSite=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
-Secure strict-transport-security: - max-age=31536000 ; includeSubDomains x-
-content-type-options: - nosniff x-frame-options: - DENY x-vcap-request-id: -
-34046863-11e2-48ad-5d93-ac83cdcd5292 x-xss-protection: - 1; mode=block status:
-code: 302 message: Found - request: body: null headers: Accept: - '*/*' Accept-
-Encoding: - gzip, deflate Connection: - keep-alive Cookie: - SESSION=SANITIZED;
-GARMIN-SSO=SANITIZED; GARMIN-SSO-CUST-GUID=SANITIZED; GARMIN-SSO-
-GUID=SANITIZED; GarminNoCache=SANITIZED; __cf_bm=SANITIZED; __cfruid=SANITIZED;
-_cfuvid=SANITIZED; CASTGC=SANITIZED; __VCAP_ID__=SANITIZED; __cflb=SANITIZED;
-org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED
-User-Agent: - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X)
-AppleWebKit/605.1.15 (KHTML, like Gecko) Mobile/15E148 referer: - https://
-sso.garmin.com/sso/
-login?logintoken=ustnTKB9hK&service=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&locale=en&embed=true&source=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountLoginUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&rememberMyBrowserChecked=true
-method: GET uri: https://sso.garmin.com/sso/
-login?service=https%3A%2F%2Fconnect.garmin.com%2Fmodern%2F&webhost=https%3A%2F%2Fconnect.garmin.com&gateway=true&generateExtraServiceTicket=true&generateTwoExtraServiceTickets=true
-response: body: string: '' headers: Access-Control-Allow-Credentials: - 'true'
-Access-Control-Allow-Headers: - Access-Control-Allow-Headers, Origin,Accept, X-
-Requested-With, Content-Type, Access-Control-Request-Method, Access-Control-
-Request-Headers Access-Control-Allow-Methods: - GET,POST,OPTIONS Access-
-Control-Allow-Origin: - https://www.garmin.com CF-Cache-Status: - DYNAMIC CF-
-Ray: - 7eabf7544e3c154b-QRO Connection: - keep-alive Content-Language: - en
-Content-Length: - '0' Date: - Sat, 22 Jul 2023 13:17:50 GMT Location: - https:/
-/connect.garmin.com/modern/?ticket=ST-2170361-w1XugXWxvBoefRgT454i-cas NEL: - '
+Connection: - keep-alive User-Agent: - python-requests/2.31.0 method: GET uri:
+https://thegarth.s3.amazonaws.com/oauth_consumer.json response: body: string: '
+{"consumer_key": "SANITIZED", "consumer_secret": "SANITIZED"}' headers: Accept-
+Ranges: - bytes Content-Length: - '124' Content-Type: - application/json Date:
+- Thu, 03 Aug 2023 13:44:37 GMT ETag: - '"20240b1013cb35419bb5b2cff1407a4e"'
+Last-Modified: - Thu, 03 Aug 2023 00:16:11 GMT Server: - AmazonS3 x-amz-id-2: -
+5kBqVpLRbTyIWKiOf3iqFe3UngcAwmTXV/SXVeQGzgS0dDxoXL/
+3w24eA5EQYuU5VcFgPCVhP499dEGMmVxr9A== x-amz-request-id: - X37BGHYK6YY1J2YX x-
+amz-server-side-encryption: - AES256 status: code: 200 message: OK - request:
+body: null headers: Accept: - !!binary | Ki8q Accept-Encoding: - !!binary |
+Z3ppcCwgZGVmbGF0ZQ== Authorization: - Bearer SANITIZED Connection: - !!binary |
+a2VlcC1hbGl2ZQ== User-Agent: - !!binary |
+Y29tLmdhcm1pbi5hbmRyb2lkLmFwcHMuY29ubmVjdG1vYmlsZQ== method: GET uri: https://
+connectapi.garmin.com/oauth-service/oauth/preauthorized?ticket=ST-2291079-
+RkvmCoLwBmLIumhwWYo3-cas&login-url=https://sso.garmin.com/sso/embed&accepts-
+mfa-tokens=true response: body: string:
+oauth_token=SANITIZED&oauth_token_secret=SANITIZED&mfa_token=SANITIZED&mfa_expiration_timestamp=2023-
+08-03 15:44:35.000 headers: CF-Cache-Status: - DYNAMIC CF-RAY: -
+7f0eff0a3f4f1557-QRO Connection: - keep-alive Content-Encoding: - gzip Content-
+Type: - text/plain;charset=utf-8 Date: - Thu, 03 Aug 2023 13:44:36 GMT NEL: - '
 {"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}' Report-To: - '
 {"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/
-v3?s=oCtK3aRDIJ3%2BdUzI9FgoSwc8jvWGgtS2bWE%2B18IChw8grnNiqD8IHNym%2Bn9FOJGH5fvM88pPHz7zrtU%2F%2F%2BM%2BC%2Fo6RRul0FF7JOyv%2ByrZKT7l0lgFKuI4OPHB2LXGsUby"}],"group":
+v3?s=wx6PD3r3tVRMWclSoxaB3Dm82pfy4XmhSvh7od0%2Fux%2FJHi7FudxJADY%2BICt8sKbMK%2B1ywjlmylnj70wO6I4LEL4btzHWgNKZ9LG5aKSKn00w0ZqqHRQiT93c9DptWX7WY24hqz9V8Q%3D%3D"}],"group":
 "cf-nel","max_age":604800}' Server: - cloudflare Set-Cookie: -
-org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED;
-Path=SANITIZED - CASTGC=SANITIZED; Path=SANITIZED; Secure; HttpOnly -
-CASTGC=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED; Secure;
-HttpOnly Vary: - Accept-Encoding X-Application-Context: - casServer:
-cloud,prod,prod-US_1102:6 X-B3-Traceid: - 415c157ce8724ec55ce3bb4a93cd0cb6 X-
-Robots-Tag: - noindex X-Vcap-Request-Id: - 5463d6d4-2bf1-49bc-509c-88197eca1707
-status: code: 302 message: Found - request: body: null headers: Accept: - '*/*'
-Accept-Encoding: - gzip, deflate Connection: - keep-alive Cookie: -
-_cfuvid=SANITIZED; GARMIN-SSO=SANITIZED; GARMIN-SSO-CUST-GUID=SANITIZED;
-GARMIN-SSO-GUID=SANITIZED; GarminNoCache=SANITIZED; ADRUM_BTa=SANITIZED;
-SESSIONID=SANITIZED; SameSite=SANITIZED; __cflb=SANITIZED User-Agent: -
-Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X) AppleWebKit/605.1.15
-(KHTML, like Gecko) Mobile/15E148 referer: - https://sso.garmin.com/sso/
-login?logintoken=ustnTKB9hK&service=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&locale=en&embed=true&source=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountLoginUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&rememberMyBrowserChecked=true
-method: GET uri: https://connect.garmin.com/modern/?ticket=ST-2170361-
-w1XugXWxvBoefRgT454i-cas response: body: string: '' headers: CF-Cache-Status: -
-DYNAMIC CF-RAY: - 7eabf757ccdfb6df-QRO Connection: - keep-alive Content-Length:
-- '0' Date: - Sat, 22 Jul 2023 13:17:51 GMT NEL: - '{"success_fraction":
-0.01,"report_to":"cf-nel","max_age":604800}' Report-To: - '{"endpoints":[
-{"url":"https:\/\/a.nel.cloudflare.com\/report\/
-v3?s=Mpydy8F4g18x5Z%2FCZD37JqFI7pshY%2FzrbICb5Uq9QNeHBWb6EHAHQ5W96RR6ijTMPrMwtTJzReSbj4RzJuQEVYiQZkSSTpfnVqxfXzPyDDafFZ3sVHVJEHLdAtCgyTroj%2FZ79Q%3D%3D"}],"group":
-"cf-nel","max_age":604800}' Server: - cloudflare cache-control: - no-cache, no-
-store, max-age=0, must-revalidate expires: - '0' location: - https://
-connect.garmin.com/modern/ pragma: - no-cache set-cookie: -
-ADRUM_BTa=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
-Secure - ADRUM_BTa=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED;
-Path=SANITIZED; Secure - ADRUM_BTa=SANITIZED; Max-Age=SANITIZED;
-Expires=SANITIZED; Path=SANITIZED; Secure - SameSite=SANITIZED; Max-
-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED; Secure strict-transport-
-security: - max-age=31536000 ; includeSubDomains x-content-type-options: -
-nosniff x-frame-options: - DENY x-vcap-request-id: - aabeba45-a872-4d25-48a5-
-919a48e2513c x-xss-protection: - 1; mode=block status: code: 302 message: Found
-- request: body: null headers: Accept: - '*/*' Accept-Encoding: - gzip, deflate
-Connection: - keep-alive Cookie: - _cfuvid=SANITIZED; GARMIN-SSO=SANITIZED;
-GARMIN-SSO-CUST-GUID=SANITIZED; GARMIN-SSO-GUID=SANITIZED;
-GarminNoCache=SANITIZED; SESSIONID=SANITIZED; SameSite=SANITIZED;
-__cflb=SANITIZED; ADRUM_BTa=SANITIZED User-Agent: - Mozilla/5.0 (iPhone; CPU
-iPhone OS 16_5 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Mobile/
-15E148 referer: - https://sso.garmin.com/sso/
-login?logintoken=ustnTKB9hK&service=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&locale=en&embed=true&source=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountLoginUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&rememberMyBrowserChecked=true
-method: GET uri: https://connect.garmin.com/modern/ response: body: string: "
-\n
-\n\n\n\n
-\n \
-\n
-\n
-\n\n
-\n\n \n\n\n \n\n \
-" href=\"/modern/images/favicon.ico\" />\n\n \ \n \n
-\n
-\n \ \n \n\n \n\n \n \ \n\n \n \n \n
-\n \n\n\n\n
-\n
-\n\n\n
-\n
-" tabindex=\"-1\">
-\n\n\n\n
-\n\n
-">\n\n
-\n\n
-\n \n \n\n
-">\n \n \n\n
-">\n \ \n \n\n\n
-\n\n\n \ \n \n
-">\n\n \ \n
-\n\n
-\n \
-\n \
-\n
-\n\n \ \n\n \n
-\n \ \n
-\" id=\"garmin-connect-version\">4.69.0.17
-\n \
-\n\n \n
-\n\n
-\n\n
-\n
-\n\n
-\n
-\n\n\n\n
-" headers: CF-Cache-Status: - DYNAMIC CF-RAY: - 7eabf75a488b1547-QRO
-Connection: - keep-alive Content-Encoding: - gzip Content-Type: - text/
-html;charset=UTF-8 Date: - Sat, 22 Jul 2023 13:17:51 GMT NEL: - '
-{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}' Report-To: - '
-{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/
-v3?s=mHxILkyoUvQ7guqKTqL4aC%2Fx%2BxF0OtAi7wckNzEF%2B7n2aSCf2HaqKRDvNBKgC8erF7S%2FVHBc3e1IJhtHmEupc%2FAWH9ID362jzILvtRdllqO9ocCPsLnPwT9D27SOyPH1Uq8H8Q%3D%3D"}],"group":
-"cf-nel","max_age":604800}' Server: - cloudflare Transfer-Encoding: - chunked
-cache-control: - no-cache, no-store, max-age=0, must-revalidate content-
-language: - en-US expires: - '0' pragma: - no-cache set-cookie: -
-ADRUM_BTa=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
-Secure - ADRUM_BTa=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED;
-Path=SANITIZED; Secure - ADRUM_BTa=SANITIZED; Max-Age=SANITIZED;
-Expires=SANITIZED; Path=SANITIZED; Secure - SameSite=SANITIZED; Max-
-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED; Secure - ADRUM_BT1=SANITIZED;
-Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED; Secure -
-ADRUM_BT1=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
-Secure strict-transport-security: - max-age=31536000 ; includeSubDomains x-
-content-type-options: - nosniff x-frame-options: - DENY x-vcap-request-id: -
-35da0075-f093-4460-5627-51c31a9caf90 x-xss-protection: - 1; mode=block status:
-code: 200 message: OK - request: body: null headers: Accept: - '*/*' Accept-
-Encoding: - gzip, deflate Connection: - keep-alive Content-Length: - '0'
-Cookie: - _cfuvid=SANITIZED; GARMIN-SSO=SANITIZED; GARMIN-SSO-CUST-
-GUID=SANITIZED; GARMIN-SSO-GUID=SANITIZED; GarminNoCache=SANITIZED;
-ADRUM_BT1=SANITIZED; ADRUM_BTa=SANITIZED; SESSIONID=SANITIZED;
-SameSite=SANITIZED; __cflb=SANITIZED User-Agent: - Mozilla/5.0 (iPhone; CPU
-iPhone OS 16_5 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Mobile/
-15E148 referer: - https://connect.garmin.com/modern method: POST uri: https://
-connect.garmin.com/modern/di-oauth/exchange response: body: string: '{"scope":
-"COMMUNITY_COURSE_READ GOLF_API_READ GHS_HID ATP_READ GHS_SAMD INSIGHTS_READ
-COMMUNITY_COURSE_WRITE CONNECT_WRITE DIVE_SHARED_READ GHS_REGISTRATION
-GOLF_API_WRITE INSIGHTS_WRITE PRODUCT_SEARCH_READ GOLF_SHARED_READ
-CONNECT_NON_SOCIAL_SHARED_READ CONNECT_READ ATP_WRITE", "jti": "SANITIZED",
-"access_token": "SANITIZED", "token_type": "Bearer", "refresh_token":
-"SANITIZED", "expires_in": 3599, "refresh_token_expires_in": 7199}' headers:
-CF-Cache-Status: - DYNAMIC CF-RAY: - 7eabf7602f9a155e-QRO Connection: - keep-
-alive Content-Encoding: - gzip Content-Type: - application/json Date: - Sat, 22
-Jul 2023 13:17:52 GMT NEL: - '{"success_fraction":0.01,"report_to":"cf-
+_cfuvid=SANITIZED; path=SANITIZED; domain=SANITIZED; HttpOnly; Secure;
+SameSite=SANITIZED Transfer-Encoding: - chunked alt-svc: - h3=":443"; ma=86400
+status: code: 200 message: OK - request: body: '' headers: Accept: - !!binary |
+Ki8q Accept-Encoding: - !!binary | Z3ppcCwgZGVmbGF0ZQ== Authorization: - Bearer
+SANITIZED Connection: - !!binary | a2VlcC1hbGl2ZQ== Content-Length: - !!binary
+| MA== Content-Type: - !!binary | YXBwbGljYXRpb24veC13d3ctZm9ybS11cmxlbmNvZGVk
+User-Agent: - !!binary | Y29tLmdhcm1pbi5hbmRyb2lkLmFwcHMuY29ubmVjdG1vYmlsZQ==
+method: POST uri: https://connectapi.garmin.com/oauth-service/oauth/exchange/
+user/2.0 response: body: string: '{"scope": "COMMUNITY_COURSE_READ
+GARMINPAY_WRITE GOLF_API_READ ATP_READ GHS_SAMD GHS_UPLOAD INSIGHTS_READ
+COMMUNITY_COURSE_WRITE CONNECT_WRITE GCOFFER_WRITE GARMINPAY_READ
+DT_CLIENT_ANALYTICS_WRITE GOLF_API_WRITE INSIGHTS_WRITE PRODUCT_SEARCH_READ
+GCOFFER_READ CONNECT_READ ATP_WRITE", "jti": "SANITIZED", "access_token":
+"SANITIZED", "token_type": "Bearer", "refresh_token": "SANITIZED",
+"expires_in": 95631, "refresh_token_expires_in": 2591999}' headers: CF-Cache-
+Status: - DYNAMIC CF-RAY: - 7f0eff0daa741547-QRO Connection: - keep-alive
+Content-Encoding: - gzip Content-Type: - application/json Date: - Thu, 03 Aug
+2023 13:44:37 GMT NEL: - '{"success_fraction":0.01,"report_to":"cf-
 nel","max_age":604800}' Report-To: - '{"endpoints":[{"url":"https:\/\/
 a.nel.cloudflare.com\/report\/
-v3?s=5Kfbn7%2BM%2FJURIaBxa7p3O8VlzRLjIw9unm4J%2FoM8Gxh9IuGYjDwT9zipvqjh%2BpdrwkoewEYRSCa%2FmwEsYsM5kTjjNPNJvsWgIEi%2FRBTMo1qYfyimlmZ5jNy12mxDoHallpwvDg%3D%3D"}],"group":
-"cf-nel","max_age":604800}' Server: - cloudflare Transfer-Encoding: - chunked
-cache-control: - no-cache, no-store, private pragma: - no-cache set-cookie: -
-ADRUM_BT1=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
-Secure - ADRUM_BTa=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED;
-Path=SANITIZED; Secure - ADRUM_BTa=SANITIZED; Max-Age=SANITIZED;
-Expires=SANITIZED; Path=SANITIZED; Secure - ADRUM_BTa=SANITIZED; Max-
-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED; Secure - SameSite=SANITIZED;
-Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED; Secure -
-ADRUM_BT1=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
-Secure - ADRUM_BT1=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED;
-Path=SANITIZED; Secure - JWT_FGP=SANITIZED; SameSite=SANITIZED; HttpOnly;
-Secure; Max-Age=SANITIZED; Domain=SANITIZED; Path=SANITIZED strict-transport-
-security: - max-age=31536000 ; includeSubDomains x-content-type-options: -
-nosniff x-frame-options: - DENY x-vcap-request-id: - f29cd951-1c6f-461b-73a5-
-aa1ae2e83a86 x-xss-protection: - 1; mode=block status: code: 200 message: OK
-version: 1
+v3?s=UWx0LW8l%2Bzswc3LmvfMCaKHSQvKAeBn6tXX2wu0jpjPXnK%2Bvyt9%2FibwHSbLvJa43YjJXG8MWRYH5CcV9M1TCjuDE%2BwQ5kMIO684fQExIQLiGQQLqC7OR%2FBjXjV%2BY4ItI3sYempKLpQ%3D%3D"}],"group":
+"cf-nel","max_age":604800}' Server: - cloudflare Set-Cookie: -
+_cfuvid=SANITIZED; path=SANITIZED; domain=SANITIZED; HttpOnly; Secure;
+SameSite=SANITIZED Transfer-Encoding: - chunked alt-svc: - h3=":443"; ma=86400
+cache-control: - no-cache, no-store, private pragma: - no-cache status: code:
+200 message: OK version: 1
```

### Comparing `garth-0.3.5/tests/cassettes/test_refresh.yaml` & `garth-0.4.0/tests/cassettes/test_exchange.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,62 +1,107 @@
 interactions:
 - request:
-    body: '{"refresh_token": "SANITIZED"}'
+    body: null
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
+      User-Agent:
+      - python-requests/2.31.0
+    method: GET
+    uri: https://thegarth.s3.amazonaws.com/oauth_consumer.json
+  response:
+    body:
+      string: '{"consumer_key": "SANITIZED", "consumer_secret": "SANITIZED"}'
+    headers:
+      Accept-Ranges:
+      - bytes
       Content-Length:
-      - '57'
+      - '124'
       Content-Type:
       - application/json
-      Cookie:
-      - JWT_FGP=SANITIZED; _cfuvid=SANITIZED; GARMIN-SSO=SANITIZED; GARMIN-SSO-CUST-GUID=SANITIZED;
-        GARMIN-SSO-GUID=SANITIZED; GarminNoCache=SANITIZED; SESSIONID=SANITIZED; __cflb=SANITIZED
+      Date:
+      - Fri, 04 Aug 2023 03:43:24 GMT
+      ETag:
+      - '"20240b1013cb35419bb5b2cff1407a4e"'
+      Last-Modified:
+      - Thu, 03 Aug 2023 00:16:11 GMT
+      Server:
+      - AmazonS3
+      x-amz-id-2:
+      - V8hHVVhXCEX7RD7Vzw8IsKS//xFr7co0468z4G834xsWIJ46GpXAwZKETm68Odczy470cauMZXo=
+      x-amz-request-id:
+      - Z03APPY9GXZFWZ69
+      x-amz-server-side-encryption:
+      - AES256
+    status:
+      code: 200
+      message: OK
+- request:
+    body: ''
+    headers:
+      Accept:
+      - !!binary |
+        Ki8q
+      Accept-Encoding:
+      - !!binary |
+        Z3ppcCwgZGVmbGF0ZQ==
+      Authorization:
+      - Bearer SANITIZED
+      Connection:
+      - !!binary |
+        a2VlcC1hbGl2ZQ==
+      Content-Length:
+      - !!binary |
+        MA==
+      Content-Type:
+      - !!binary |
+        YXBwbGljYXRpb24veC13d3ctZm9ybS11cmxlbmNvZGVk
       User-Agent:
-      - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X) AppleWebKit/605.1.15
-        (KHTML, like Gecko) Mobile/15E148
+      - !!binary |
+        Y29tLmdhcm1pbi5hbmRyb2lkLmFwcHMuY29ubmVjdG1vYmlsZQ==
     method: POST
-    uri: https://connect.garmin.com/services/auth/token/refresh
+    uri: https://connectapi.garmin.com/oauth-service/oauth/exchange/user/2.0
   response:
     body:
-      string: '{"access_token": "SANITIZED", "token_type": "bearer", "refresh_token":
-        "SANITIZED", "expires_in": 3599, "scope": "COMMUNITY_COURSE_READ GOLF_API_READ
-        GHS_HID ATP_READ GHS_SAMD INSIGHTS_READ COMMUNITY_COURSE_WRITE CONNECT_WRITE
-        DIVE_SHARED_READ GHS_REGISTRATION GOLF_API_WRITE INSIGHTS_WRITE PRODUCT_SEARCH_READ
-        GOLF_SHARED_READ CONNECT_NON_SOCIAL_SHARED_READ CONNECT_READ ATP_WRITE", "jti":
-        "SANITIZED", "refresh_token_expires_in": 7199}'
+      string: '{"scope": "COMMUNITY_COURSE_READ GARMINPAY_WRITE GOLF_API_READ ATP_READ
+        GHS_SAMD GHS_UPLOAD INSIGHTS_READ COMMUNITY_COURSE_WRITE CONNECT_WRITE GCOFFER_WRITE
+        GARMINPAY_READ DT_CLIENT_ANALYTICS_WRITE GOLF_API_WRITE INSIGHTS_WRITE PRODUCT_SEARCH_READ
+        GCOFFER_READ CONNECT_READ ATP_WRITE", "jti": "SANITIZED", "access_token":
+        "SANITIZED", "token_type": "Bearer", "refresh_token": "SANITIZED", "expires_in":
+        107182, "refresh_token_expires_in": 2591999}'
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7eb41bb0d8471549-QRO
+      - 7f13cbbc2a754790-DFW
       Connection:
       - keep-alive
-      Content-Length:
-      - '1685'
+      Content-Encoding:
+      - gzip
       Content-Type:
-      - application/json; charset=utf-8
+      - application/json
       Date:
-      - Sun, 23 Jul 2023 13:00:46 GMT
+      - Fri, 04 Aug 2023 03:43:23 GMT
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=qvssb2pR8clCJ9TqmPzrjjTgy2YL5%2F1ZiGv%2F8zmCUgQVf6AJeZTNgTsOCCUdPSWP%2Bm%2FNrTGy2frrbJJ2quWBgK04viYeGeiKqh5KBiYOtkYVq2vCKg2PvZzAXDf0rGIMz%2FVcrA%3D%3D"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=T5EHGPEATgD5SbyAMCZh1mKSEJkUest3sa7l%2FTpQ6dZl3uv3K%2BW7Ng20XTseNh3KPdqYzHdkCCB5d4npBML1ZgAAmVUYdkrYiM2uJhmn7WfvSdrIyme0uCf9p5t7RY6%2BRUxNYfhL8Q%3D%3D"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
-      etag:
-      - W/"695-06sM1EKqILFTnvbNt7w08+ZJ9Rs"
-      set-cookie:
-      - JWT_FGP=SANITIZED; Max-Age=SANITIZED; Domain=SANITIZED; Path=SANITIZED; Expires=SANITIZED;
-        HttpOnly; Secure
-      x-powered-by:
-      - Express
-      x-vcap-request-id:
-      - 7dd8a031-3d6c-46a5-49c9-4d62c693158d
+      Set-Cookie:
+      - _cfuvid=SANITIZED; path=SANITIZED; domain=SANITIZED; HttpOnly; Secure; SameSite=SANITIZED
+      Transfer-Encoding:
+      - chunked
+      alt-svc:
+      - h3=":443"; ma=86400
+      cache-control:
+      - no-cache, no-store, private
+      pragma:
+      - no-cache
     status:
-      code: 201
-      message: Created
+      code: 200
+      message: OK
 version: 1
```

### Comparing `garth-0.3.5/tests/conftest.py` & `garth-0.4.0/tests/conftest.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,78 +2,94 @@
 import os
 import re
 import time
 
 import pytest
 from requests import Session
 
-from garth.auth_token import AuthToken
+from garth.auth_tokens import OAuth1Token, OAuth2Token
 from garth.http import Client
 
 
 @pytest.fixture
 def session():
     return Session()
 
 
 @pytest.fixture
 def client(session) -> Client:
     return Client(session=session)
 
 
 @pytest.fixture
-def auth_token_dict() -> dict:
+def oauth1_token_dict() -> dict:
+    return dict(
+        oauth_token="7fdff19aa9d64dda83e9d7858473aed1",
+        oauth_token_secret="49919d7c4c8241ac93fb4345886fbcea",
+        mfa_token="ab316f8640f3491f999f3298f3d6f1bb",
+        mfa_expiration_timestamp="2023-08-02 05:56:10.000",
+    )
+
+
+@pytest.fixture
+def oauth1_token(oauth1_token_dict) -> OAuth1Token:
+    return OAuth1Token(**oauth1_token_dict)
+
+
+@pytest.fixture
+def oauth2_token_dict() -> dict:
     return dict(
         scope="CONNECT_READ CONNECT_WRITE",
         jti="foo",
         token_type="Bearer",
         access_token="bar",
         refresh_token="baz",
         expires_in=3599,
         refresh_token_expires_in=7199,
-        username="mtamizi",
     )
 
 
 @pytest.fixture
-def auth_token(auth_token_dict: dict) -> AuthToken:
-    token = AuthToken(
+def oauth2_token(oauth2_token_dict: dict) -> OAuth2Token:
+    token = OAuth2Token(
         expires_at=int(time.time() + 3599),
         refresh_token_expires_at=int(time.time() + 7199),
-        **auth_token_dict,
+        **oauth2_token_dict,
     )
     return token
 
 
 @pytest.fixture
-def authed_client(auth_token: AuthToken) -> Client:
+def authed_client(
+    oauth1_token: OAuth1Token, oauth2_token: OAuth2Token
+) -> Client:
     client = Client()
     try:
-        client.load(os.environ["GARTH_SESSION"])
+        client.load(os.environ["GARTH_HOME"])
     except KeyError:
-        client.auth_token = auth_token
+        client.configure(oauth1_token=oauth1_token, oauth2_token=oauth2_token)
     return client
 
 
 @pytest.fixture
 def vcr(vcr):
-    if "GARTH_SESSION" not in os.environ:
+    if "GARTH_HOME" not in os.environ:
         vcr.record_mode = "none"
     return vcr
 
 
 def sanitize_cookie(cookie_value) -> str:
     return re.sub(r"=[^;]*", "=SANITIZED", cookie_value)
 
 
 def sanitize_request(request):
     if request.body:
         body = request.body.decode("utf8")
         for key in ["username", "password", "refresh_token"]:
-            body = re.sub(key + r"=[^&]*", "username=SANITIZED", body)
+            body = re.sub(key + r"=[^&]*", f"{key}=SANITIZED", body)
         request.body = body.encode("utf8")
 
     if "Cookie" in request.headers:
         cookies = request.headers["Cookie"].split("; ")
         sanitized_cookies = [sanitize_cookie(cookie) for cookie in cookies]
         request.headers["Cookie"] = "; ".join(sanitized_cookies)
     return request
@@ -82,31 +98,43 @@
 def sanitize_response(response):
     for key in ["set-cookie", "Set-Cookie"]:
         if key in response["headers"]:
             cookies = response["headers"][key]
             sanitized_cookies = [sanitize_cookie(cookie) for cookie in cookies]
             response["headers"][key] = sanitized_cookies
 
-    if "body" in response and response["body"]["string"]:
-        try:
-            body = response["body"]["string"].decode("utf8")
-            body_json = json.loads(body)
-        except json.JSONDecodeError:
-            pass
-        else:
-            # sanitize access_token and refresh_token
-            if "access_token" in body_json:
-                body_json["access_token"] = "SANITIZED"
-            if "refresh_token" in body_json:
-                body_json["refresh_token"] = "SANITIZED"
-            if "jti" in body_json:
-                body_json["jti"] = "SANITIZED"
+    if "body" not in response and response["body"]["string"]:
+        return response
+
+    body = response["body"]["string"].decode("utf8")
+    patterns = [
+        "oauth_token=[^&]*",
+        "oauth_token_secret=[^&]*",
+        "mfa_token=[^&]*",
+    ]
+    for pattern in patterns:
+        body = re.sub(pattern, pattern.split("=")[0] + "=SANITIZED", body)
+    try:
+        body_json = json.loads(body)
+    except json.JSONDecodeError:
+        pass
+    else:
+        for field in [
+            "access_token",
+            "refresh_token",
+            "jti",
+            "consumer_key",
+            "consumer_secret",
+        ]:
+            if field in body_json:
+                body_json[field] = "SANITIZED"
+
+        body = json.dumps(body_json)
+    response["body"]["string"] = body.encode("utf8")
 
-            body = json.dumps(body_json)
-            response["body"]["string"] = body.encode("utf8")
     return response
 
 
 @pytest.fixture(scope="session")
 def vcr_config():
     return {
         "filter_headers": [("Authorization", "Bearer SANITIZED")],
```

### Comparing `garth-0.3.5/tests/resources/cassettes/test_daily_hrv.yaml` & `garth-0.4.0/tests/stats/cassettes/test_daily_hrv.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -6,24 +6,19 @@
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Authorization:
       - Bearer SANITIZED
       Connection:
       - keep-alive
-      Cookie:
-      - JWT_FGP=SANITIZED; _cfuvid=SANITIZED; GARMIN-SSO=SANITIZED; GARMIN-SSO-CUST-GUID=SANITIZED;
-        GARMIN-SSO-GUID=SANITIZED; GarminNoCache=SANITIZED; SESSIONID=SANITIZED; __cflb=SANITIZED
       User-Agent:
       - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X) AppleWebKit/605.1.15
         (KHTML, like Gecko) Mobile/15E148
-      di-backend:
-      - connectapi.garmin.com
     method: GET
-    uri: https://connect.garmin.com/hrv-service/hrv/daily/2023-07-01/2023-07-20
+    uri: https://connectapi.garmin.com/hrv-service/hrv/daily/2023-07-01/2023-07-20
   response:
     body:
       string: '{"hrvSummaries": [{"calendarDate": "2023-07-01", "weeklyAvg": 43, "lastNightAvg":
         43, "lastNight5MinHigh": 60, "baseline": {"lowUpper": 35, "balancedLow": 38,
         "balancedUpper": 52, "markerValue": 0.42855835}, "status": "BALANCED", "feedbackPhrase":
         "HRV_BALANCED_8", "createTimeStamp": "2023-07-01T12:27:14.85"}, {"calendarDate":
         "2023-07-02", "weeklyAvg": 43, "lastNightAvg": 44, "lastNight5MinHigh": 63,
@@ -94,39 +89,42 @@
         "balancedLow": 39, "balancedUpper": 52, "markerValue": 0.25}, "status": "BALANCED",
         "feedbackPhrase": "HRV_BALANCED_7", "createTimeStamp": "2023-07-20T12:14:11.898"}],
         "userProfilePk": 2591602}'
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7ee9c25508eab6ee-QRO
+      - 7f12cffb1bf04740-DFW
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json
       Date:
-      - Sun, 30 Jul 2023 01:16:56 GMT
+      - Fri, 04 Aug 2023 00:51:31 GMT
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=Ig10n8P3G%2FX4Vp3ul24i1kHttHYtcRm1HiCd6dc%2Fjz1lmoB4AtNDuCVpY54U4ex5q2t13XG5VtXvxr2fofHo1aG0CXozSONIa4yPdKFoWX1NaIdE9QGEgalg46QnrI6w6D9yVA%3D%3D"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=FwXXbkT4TDPL0xwdyj0pemCK5IZtMhJ0cEJStvFh9rhUuwEgA9nPQyW5%2F78guNWU4c0CMB5arBD5aYFCFwrJ0S9cXV%2BHnxbblaMvHkHhr3XZNcHySwLfohsTZBtkWiUT4iZVWVGDgg%3D%3D"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Transfer-Encoding:
       - chunked
+      alt-svc:
+      - h3=":443"; ma=86400
       cache-control:
       - no-cache, no-store, private
       pragma:
       - no-cache
       set-cookie:
       - ADRUM_BTa=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED
       - ADRUM_BTa=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED
       - SameSite=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
       - ADRUM_BT1=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED
       - ADRUM_BT1=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED
+      - _cfuvid=SANITIZED; path=SANITIZED; domain=SANITIZED; HttpOnly; Secure; SameSite=SANITIZED
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `garth-0.3.5/tests/resources/cassettes/test_daily_intensity_minutes.yaml` & `garth-0.4.0/tests/stats/cassettes/test_daily_intensity_minutes.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -6,26 +6,19 @@
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Authorization:
       - Bearer SANITIZED
       Connection:
       - keep-alive
-      Cookie:
-      - JWT_FGP=SANITIZED; _cfuvid=SANITIZED; GARMIN-SSO=SANITIZED; GARMIN-SSO-CUST-GUID=SANITIZED;
-        GARMIN-SSO-GUID=SANITIZED; GarminNoCache=SANITIZED; SESSIONID=SANITIZED; __cflb=SANITIZED
       User-Agent:
       - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X) AppleWebKit/605.1.15
         (KHTML, like Gecko) Mobile/15E148
-      di-backend:
-      - connectapi.garmin.com
-      referer:
-      - https://connect.garmin.com/modern
     method: GET
-    uri: https://connect.garmin.com/usersummary-service/stats/im/daily/2023-07-01/2023-07-20
+    uri: https://connectapi.garmin.com/usersummary-service/stats/im/daily/2023-07-01/2023-07-20
   response:
     body:
       string: '[{"calendarDate": "2023-07-01", "weeklyGoal": 150, "moderateValue":
         0, "vigorousValue": 0}, {"calendarDate": "2023-07-02", "weeklyGoal": 150,
         "moderateValue": 55, "vigorousValue": 6}, {"calendarDate": "2023-07-03", "weeklyGoal":
         150, "moderateValue": 13, "vigorousValue": 0}, {"calendarDate": "2023-07-04",
         "weeklyGoal": 150, "moderateValue": 9, "vigorousValue": 34}, {"calendarDate":
@@ -48,43 +41,44 @@
         "2023-07-19", "weeklyGoal": 150, "moderateValue": 1, "vigorousValue": 0},
         {"calendarDate": "2023-07-20", "weeklyGoal": 150, "moderateValue": 0, "vigorousValue":
         0}]'
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7ee92bb1799b4636-DFW
+      - 7f12d0031b5247fd-DFW
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json
       Date:
-      - Sat, 29 Jul 2023 23:34:06 GMT
+      - Fri, 04 Aug 2023 00:51:33 GMT
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=3bJmnY%2FRk1xU%2BQfwwKbmIo6tmq5qdR%2F%2BRsyvVIFwX6TBo%2FQeE3BW7dSCCc1wS%2BAvMZoLIc9zSdNZIEj9emCIhHlV76RkZ5Z6KwYYXf4qhlv3DyV7qd8TdNUkKv40gnes%2Bs6RpQ%3D%3D"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=9im50IutY9DBaURoxea2zvLVuniHkDcSgeUppPhyVdmW%2FDSA3THWATEIui7XNQQxyQo08JOtLQ5MRRM1%2F6faiOqzehpRUM3EJ3eDtkXNQwLBUlFZ%2B3ldpbg%2FNfHDN%2BXb3rjJU1YjJg%3D%3D"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Transfer-Encoding:
       - chunked
+      alt-svc:
+      - h3=":443"; ma=86400
       cache-control:
       - no-cache, no-store, private
       pragma:
       - no-cache
       set-cookie:
       - ADRUM_BTa=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
       - ADRUM_BTa=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
       - SameSite=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
       - ADRUM_BT1=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
-      - ADRUM_BT1=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
-        Secure
+      - _cfuvid=SANITIZED; path=SANITIZED; domain=SANITIZED; HttpOnly; Secure; SameSite=SANITIZED
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `garth-0.3.5/tests/resources/cassettes/test_daily_sleep.yaml` & `garth-0.4.0/tests/stats/cassettes/test_daily_sleep.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -6,26 +6,19 @@
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Authorization:
       - Bearer SANITIZED
       Connection:
       - keep-alive
-      Cookie:
-      - JWT_FGP=SANITIZED; _cfuvid=SANITIZED; GARMIN-SSO=SANITIZED; GARMIN-SSO-CUST-GUID=SANITIZED;
-        GARMIN-SSO-GUID=SANITIZED; GarminNoCache=SANITIZED; SESSIONID=SANITIZED; __cflb=SANITIZED
       User-Agent:
       - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X) AppleWebKit/605.1.15
         (KHTML, like Gecko) Mobile/15E148
-      di-backend:
-      - connectapi.garmin.com
-      referer:
-      - https://connect.garmin.com/modern
     method: GET
-    uri: https://connect.garmin.com/wellness-service/stats/daily/sleep/score/2023-07-01/2023-07-20
+    uri: https://connectapi.garmin.com/wellness-service/stats/daily/sleep/score/2023-07-01/2023-07-20
   response:
     body:
       string: '[{"calendarDate": "2023-07-01", "value": 60}, {"calendarDate": "2023-07-02",
         "value": 70}, {"calendarDate": "2023-07-03", "value": 82}, {"calendarDate":
         "2023-07-04", "value": 75}, {"calendarDate": "2023-07-05", "value": 70}, {"calendarDate":
         "2023-07-06", "value": 28}, {"calendarDate": "2023-07-07", "value": 79}, {"calendarDate":
         "2023-07-08", "value": 70}, {"calendarDate": "2023-07-09", "value": 77}, {"calendarDate":
@@ -35,39 +28,40 @@
         "2023-07-16", "value": 71}, {"calendarDate": "2023-07-17", "value": 94}, {"calendarDate":
         "2023-07-18", "value": 77}, {"calendarDate": "2023-07-19", "value": 80}, {"calendarDate":
         "2023-07-20", "value": 68}]'
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7ed53bffbdc1b6e7-QRO
+      - 7f12d00638244600-DFW
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json
       Date:
-      - Thu, 27 Jul 2023 13:29:59 GMT
+      - Fri, 04 Aug 2023 00:51:33 GMT
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=mcH9qRTKgVawVzt%2Fwd%2BXH5ToBuUsjCQc1mlRKrUO3HwURn4w27YgL%2F6tVXco3j7glLvrTvKhhoCU91F8lyIwDbg4zFMeetk68vkdeKKn%2BMUClbU83EWQ11WBd6%2FWPEh9ygliqA%3D%3D"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=RyGEQnxnunkvjbgNO5BmWlIHgK45Gi5ICNxJrWUnFSVIYAOexuuvkkAPYzGQCZKluGJewZGrYLSriEsXOrcOcQ3heU9KlvGhE7UD2gY1xn7AECCOV5wWcGb5WLwgJ8%2FDzFs%2FdL3hGg%3D%3D"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Transfer-Encoding:
       - chunked
+      alt-svc:
+      - h3=":443"; ma=86400
       cache-control:
       - no-cache, no-store, private
       pragma:
       - no-cache
       set-cookie:
       - ADRUM_BTa=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED
       - ADRUM_BTa=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED
       - SameSite=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
-      - ADRUM_BT1=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED
-      - ADRUM_BT1=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED
+      - _cfuvid=SANITIZED; path=SANITIZED; domain=SANITIZED; HttpOnly; Secure; SameSite=SANITIZED
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `garth-0.3.5/tests/resources/cassettes/test_daily_steps.yaml` & `garth-0.4.0/tests/stats/cassettes/test_daily_steps.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -6,24 +6,19 @@
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Authorization:
       - Bearer SANITIZED
       Connection:
       - keep-alive
-      Cookie:
-      - JWT_FGP=SANITIZED; _cfuvid=SANITIZED; GARMIN-SSO=SANITIZED; GARMIN-SSO-CUST-GUID=SANITIZED;
-        GARMIN-SSO-GUID=SANITIZED; GarminNoCache=SANITIZED; SESSIONID=SANITIZED; __cflb=SANITIZED
       User-Agent:
       - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X) AppleWebKit/605.1.15
         (KHTML, like Gecko) Mobile/15E148
-      di-backend:
-      - connectapi.garmin.com
     method: GET
-    uri: https://connect.garmin.com/usersummary-service/stats/steps/daily/2023-07-01/2023-07-20
+    uri: https://connectapi.garmin.com/usersummary-service/stats/steps/daily/2023-07-01/2023-07-20
   response:
     body:
       string: '[{"calendarDate": "2023-07-01", "totalSteps": 12413, "totalDistance":
         10368, "stepGoal": 7950}, {"calendarDate": "2023-07-02", "totalSteps": 5719,
         "totalDistance": 5207, "stepGoal": 8400}, {"calendarDate": "2023-07-03", "totalSteps":
         3633, "totalDistance": 3152, "stepGoal": 8140}, {"calendarDate": "2023-07-04",
         "totalSteps": 9593, "totalDistance": 8745, "stepGoal": 8140}, {"calendarDate":
@@ -46,31 +41,33 @@
         3103, "stepGoal": 9160}, {"calendarDate": "2023-07-19", "totalSteps": 3998,
         "totalDistance": 3384, "stepGoal": 8050}, {"calendarDate": "2023-07-20", "totalSteps":
         7322, "totalDistance": 6148, "stepGoal": 7240}]'
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7ee7370f48edb6e7-QRO
+      - 7f12d0361f51b6ee-QRO
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json
       Date:
-      - Sat, 29 Jul 2023 17:52:20 GMT
+      - Fri, 04 Aug 2023 00:51:41 GMT
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=BuaovcAR78Kybq5pFV6t8GIMQCw8fYThEA0qGvQ%2B6yrTkPo%2F7yoBFkmtI1%2B%2BC0qTZ%2Bqp3QwVJFEjRVmktBhZmzRyV5Fd9CpbnOnkBxqnBhdlSDhox1YYGbh9Z0SOzATk%2F80I7w%3D%3D"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=bzh%2FUoGEfIajBdQR5MV3QW0RLYZzm5KVdFbwvpMqO9thm%2FwjZKTcc%2FouaGofuuNQmFoGl%2FTksvg%2BtFeTKq3Nt78N%2BaIJVDV3FIetTmEZlwD083NaVOvpEMEwaB80srEQbZuua1khiw%3D%3D"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Transfer-Encoding:
       - chunked
+      alt-svc:
+      - h3=":443"; ma=86400
       cache-control:
       - no-cache, no-store, private
       pragma:
       - no-cache
       set-cookie:
       - ADRUM_BTa=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
@@ -78,11 +75,12 @@
         Secure
       - SameSite=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
       - ADRUM_BT1=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
       - ADRUM_BT1=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
+      - _cfuvid=SANITIZED; path=SANITIZED; domain=SANITIZED; HttpOnly; Secure; SameSite=SANITIZED
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `garth-0.3.5/tests/resources/cassettes/test_daily_stress.yaml` & `garth-0.4.0/tests/stats/cassettes/test_daily_stress.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -6,26 +6,19 @@
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Authorization:
       - Bearer SANITIZED
       Connection:
       - keep-alive
-      Cookie:
-      - JWT_FGP=SANITIZED; _cfuvid=SANITIZED; GARMIN-SSO=SANITIZED; GARMIN-SSO-CUST-GUID=SANITIZED;
-        GARMIN-SSO-GUID=SANITIZED; GarminNoCache=SANITIZED; SESSIONID=SANITIZED; __cflb=SANITIZED
       User-Agent:
       - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X) AppleWebKit/605.1.15
         (KHTML, like Gecko) Mobile/15E148
-      di-backend:
-      - connectapi.garmin.com
-      referer:
-      - https://connect.garmin.com/modern
     method: GET
-    uri: https://connect.garmin.com/usersummary-service/stats/stress/daily/2023-07-01/2023-07-20
+    uri: https://connectapi.garmin.com/usersummary-service/stats/stress/daily/2023-07-01/2023-07-20
   response:
     body:
       string: '[{"calendarDate": "2023-07-01", "values": {"highStressDuration": 1680,
         "lowStressDuration": 21780, "overallStressLevel": 35, "restStressDuration":
         27780, "mediumStressDuration": 12660}}, {"calendarDate": "2023-07-02", "values":
         {"highStressDuration": 3600, "lowStressDuration": 11580, "overallStressLevel":
         29, "restStressDuration": 39840, "mediumStressDuration": 7740}}, {"calendarDate":
@@ -71,31 +64,33 @@
         32340, "mediumStressDuration": 14100}}, {"calendarDate": "2023-07-20", "values":
         {"highStressDuration": 2880, "lowStressDuration": 21780, "overallStressLevel":
         38, "restStressDuration": 26580, "mediumStressDuration": 18240}}]'
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7eb7a1fedd4b4778-DFW
+      - 7f12d0397ff347ab-DFW
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json
       Date:
-      - Sun, 23 Jul 2023 23:16:44 GMT
+      - Fri, 04 Aug 2023 00:51:41 GMT
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=hRlYF%2BI7aGUYNRhwk9rGpXqYZMMD6JKll%2FmzTJLCu7SU8BqSjHbDPE%2Fe1XzLdUkEzU2Y8XxB7GCL6O6%2BV%2BzPYVrUzZDhBBmHBdXHA39sumDl2Bc3YVwIWQQTiiuanMTmO0Amxg%3D%3D"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=T9CAErSSY%2FFeBvVNVWoa%2FYNy0BI%2BhWzwaRSbOHzHpcYcA8u1JRck31Y044IFAjfPbLAdM1LUfY%2Fkt2eOoD4gMvuh%2B9KKGJ0VefqDsQE15iwlyQ%2FlI2YAHnt7eAhdme6nZHe8saWUvQ%3D%3D"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Transfer-Encoding:
       - chunked
+      alt-svc:
+      - h3=":443"; ma=86400
       cache-control:
       - no-cache, no-store, private
       pragma:
       - no-cache
       set-cookie:
       - ADRUM_BTa=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
@@ -103,11 +98,12 @@
         Secure
       - SameSite=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
       - ADRUM_BT1=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
       - ADRUM_BT1=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
+      - _cfuvid=SANITIZED; path=SANITIZED; domain=SANITIZED; HttpOnly; Secure; SameSite=SANITIZED
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `garth-0.3.5/tests/resources/cassettes/test_sleep_data_list.yaml` & `garth-0.4.0/tests/stats/cassettes/test_sleep_data_list.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -6,24 +6,112 @@
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Authorization:
       - Bearer SANITIZED
       Connection:
       - keep-alive
+      User-Agent:
+      - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X) AppleWebKit/605.1.15
+        (KHTML, like Gecko) Mobile/15E148
+    method: GET
+    uri: https://connectapi.garmin.com/userprofile-service/socialProfile
+  response:
+    body:
+      string: '{"id": 3154645, "profileId": 2591602, "garminGUID": "0690cc1d-d23d-4412-b027-80fd4ed1c0f6",
+        "displayName": "mtamizi", "fullName": "Matin Tamizi", "userName": "mtamizi",
+        "profileImageUuid": "73240e81-6e4d-43fc-8af8-c8f6c51b3b8f", "profileImageUrlLarge":
+        "https://s3.amazonaws.com/garmin-connect-prod/profile_images/73240e81-6e4d-43fc-8af8-c8f6c51b3b8f-2591602.png",
+        "profileImageUrlMedium": "https://s3.amazonaws.com/garmin-connect-prod/profile_images/685a19e9-a7be-4a11-9bf9-faca0c5d1f1a-2591602.png",
+        "profileImageUrlSmall": "https://s3.amazonaws.com/garmin-connect-prod/profile_images/6302f021-0ec7-4dc9-b0c3-d5a19bc5a08c-2591602.png",
+        "location": "Ciudad de M\u00e9xico, CDMX", "facebookUrl": null, "twitterUrl":
+        null, "personalWebsite": null, "motivation": null, "bio": null, "primaryActivity":
+        null, "favoriteActivityTypes": [], "runningTrainingSpeed": 0.0, "cyclingTrainingSpeed":
+        0.0, "favoriteCyclingActivityTypes": [], "cyclingClassification": null, "cyclingMaxAvgPower":
+        0.0, "swimmingTrainingSpeed": 0.0, "profileVisibility": "private", "activityStartVisibility":
+        "private", "activityMapVisibility": "public", "courseVisibility": "public",
+        "activityHeartRateVisibility": "public", "activityPowerVisibility": "public",
+        "badgeVisibility": "private", "showAge": false, "showWeight": false, "showHeight":
+        false, "showWeightClass": false, "showAgeRange": false, "showGender": false,
+        "showActivityClass": false, "showVO2Max": false, "showPersonalRecords": false,
+        "showLast12Months": false, "showLifetimeTotals": false, "showUpcomingEvents":
+        false, "showRecentFavorites": false, "showRecentDevice": false, "showRecentGear":
+        false, "showBadges": true, "otherActivity": null, "otherPrimaryActivity":
+        null, "otherMotivation": null, "userRoles": ["SCOPE_ATP_READ", "SCOPE_ATP_WRITE",
+        "SCOPE_COMMUNITY_COURSE_READ", "SCOPE_COMMUNITY_COURSE_WRITE", "SCOPE_CONNECT_READ",
+        "SCOPE_CONNECT_WRITE", "SCOPE_DT_CLIENT_ANALYTICS_WRITE", "SCOPE_GARMINPAY_READ",
+        "SCOPE_GARMINPAY_WRITE", "SCOPE_GCOFFER_READ", "SCOPE_GCOFFER_WRITE", "SCOPE_GHS_SAMD",
+        "SCOPE_GHS_UPLOAD", "SCOPE_GOLF_API_READ", "SCOPE_GOLF_API_WRITE", "SCOPE_INSIGHTS_READ",
+        "SCOPE_INSIGHTS_WRITE", "SCOPE_PRODUCT_SEARCH_READ", "ROLE_CONNECTUSER", "ROLE_FITNESS_USER",
+        "ROLE_WELLNESS_USER", "ROLE_OUTDOOR_USER", "ROLE_CONNECT_2_USER", "ROLE_TACX_APP_USER"],
+        "nameApproved": true, "userProfileFullName": "Matin Tamizi", "makeGolfScorecardsPrivate":
+        true, "allowGolfLiveScoring": false, "allowGolfScoringByConnections": true,
+        "userLevel": 3, "userPoint": 117, "levelUpdateDate": "2020-12-12T15:20:38.0",
+        "levelIsViewed": false, "levelPointThreshold": 140, "userPointOffset": 0,
+        "userPro": false}'
+    headers:
+      CF-Cache-Status:
+      - DYNAMIC
+      CF-RAY:
+      - 7f12d00c9e4f46c8-DFW
+      Connection:
+      - keep-alive
+      Content-Encoding:
+      - gzip
+      Content-Type:
+      - application/json;charset=UTF-8
+      Date:
+      - Fri, 04 Aug 2023 00:51:34 GMT
+      NEL:
+      - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
+      Report-To:
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=SXM84DDSSI7c2TJJIKh4622LJWgHbCgtQVtcjQc4SQGNDgPqWUJh7vb%2FX%2FdHtnARXtM3%2FXoDj%2FsE0xyvVmQn8pWqyjKc1ZHrpqhNKFluwNgtDZlMCAXkhD%2BMfw0D%2B0%2FAMRlortyIeA%3D%3D"}],"group":"cf-nel","max_age":604800}'
+      Server:
+      - cloudflare
+      Transfer-Encoding:
+      - chunked
+      alt-svc:
+      - h3=":443"; ma=86400
+      cache-control:
+      - no-cache, no-store, private
+      pragma:
+      - no-cache
+      set-cookie:
+      - ADRUM_BTa=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
+        Secure
+      - ADRUM_BTa=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
+        Secure
+      - SameSite=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
+        Secure
+      - ADRUM_BT1=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
+        Secure
+      - ADRUM_BT1=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
+        Secure
+      - _cfuvid=SANITIZED; path=SANITIZED; domain=SANITIZED; HttpOnly; Secure; SameSite=SANITIZED
+    status:
+      code: 200
+      message: OK
+- request:
+    body: null
+    headers:
+      Accept:
+      - '*/*'
+      Accept-Encoding:
+      - gzip, deflate
+      Authorization:
+      - Bearer SANITIZED
+      Connection:
+      - keep-alive
       Cookie:
-      - JWT_FGP=SANITIZED; _cfuvid=SANITIZED; GARMIN-SSO=SANITIZED; GARMIN-SSO-CUST-GUID=SANITIZED;
-        GARMIN-SSO-GUID=SANITIZED; GarminNoCache=SANITIZED; SESSIONID=SANITIZED; __cflb=SANITIZED
+      - _cfuvid=SANITIZED; ADRUM_BT1=SANITIZED; ADRUM_BTa=SANITIZED; SameSite=SANITIZED
       User-Agent:
       - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X) AppleWebKit/605.1.15
         (KHTML, like Gecko) Mobile/15E148
-      di-backend:
-      - connectapi.garmin.com
     method: GET
-    uri: https://connect.garmin.com/wellness-service/wellness/dailySleepData/mtamizi?nonSleepBufferMinutes=60&date=2021-07-20
+    uri: https://connectapi.garmin.com/wellness-service/wellness/dailySleepData/mtamizi?nonSleepBufferMinutes=60&date=2021-07-20
   response:
     body:
       string: '{"dailySleepDTO": {"id": 1626758400000, "userProfilePK": 2591602, "calendarDate":
         "2021-07-20", "sleepTimeSeconds": 25740, "napTimeSeconds": 0, "sleepWindowConfirmed":
         true, "sleepWindowConfirmationType": "enhanced_confirmed_final", "sleepStartTimestampGMT":
         1626758400000, "sleepEndTimestampGMT": 1626785940000, "sleepStartTimestampLocal":
         1626740400000, "sleepEndTimestampLocal": 1626767940000, "autoSleepStartTimestampGMT":
@@ -38,36 +126,42 @@
         "2021-07-20T05:21:00.0", "sleepMeasurementEndGMT": "2021-07-20T12:56:00.0",
         "alertThresholdValue": null, "numberOfEventsBelowThreshold": null, "durationOfEventsBelowThreshold":
         null, "averageSPO2": 92.0, "averageSpO2HR": 51.0, "lowestSPO2": 84}}'
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7edd166f9f9f155e-QRO
+      - 7f12d00e988e478e-DFW
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json;charset=UTF-8
       Date:
-      - Fri, 28 Jul 2023 12:22:26 GMT
+      - Fri, 04 Aug 2023 00:51:34 GMT
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=dD4eO7TmfpPHQF4rU8yUd3aBikbc16LUFpExZmFSBbQLnnRyOSyJRF3M47FWbCQ6mdLZq2kjMZnzKAyyyhsUMum6XHCt6zDdXtttH7rxuoSd6xAJM3jb6qAgYpkAw8s6rK4LcQ%3D%3D"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=qtSiA5VrDrG458hymR1BvS6PbA4aF2F7Zp8gLXC14T8J6biYe7%2F4mCla4JfoukylEE5VCzRscZy8mQr4HsyKhfwgOJJHG6AUz2IFkxK67ubouyhHv%2BklbNorsLXmJNd0U%2F2oJlsUyA%3D%3D"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Transfer-Encoding:
       - chunked
+      alt-svc:
+      - h3=":443"; ma=86400
       cache-control:
       - no-cache, no-store, private
       pragma:
       - no-cache
       set-cookie:
+      - ADRUM_BT1=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
+        Secure
+      - ADRUM_BTa=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
+        Secure
       - ADRUM_BTa=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
       - ADRUM_BTa=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
       - SameSite=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
       - ADRUM_BT1=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
@@ -85,24 +179,20 @@
       Accept-Encoding:
       - gzip, deflate
       Authorization:
       - Bearer SANITIZED
       Connection:
       - keep-alive
       Cookie:
-      - JWT_FGP=SANITIZED; _cfuvid=SANITIZED; GARMIN-SSO=SANITIZED; GARMIN-SSO-CUST-GUID=SANITIZED;
-        GARMIN-SSO-GUID=SANITIZED; GarminNoCache=SANITIZED; ADRUM_BT1=SANITIZED; ADRUM_BTa=SANITIZED;
-        SESSIONID=SANITIZED; SameSite=SANITIZED; __cflb=SANITIZED
+      - _cfuvid=SANITIZED; ADRUM_BT1=SANITIZED; ADRUM_BTa=SANITIZED; SameSite=SANITIZED
       User-Agent:
       - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X) AppleWebKit/605.1.15
         (KHTML, like Gecko) Mobile/15E148
-      di-backend:
-      - connectapi.garmin.com
     method: GET
-    uri: https://connect.garmin.com/wellness-service/wellness/dailySleepData/mtamizi?nonSleepBufferMinutes=60&date=2021-07-19
+    uri: https://connectapi.garmin.com/wellness-service/wellness/dailySleepData/mtamizi?nonSleepBufferMinutes=60&date=2021-07-19
   response:
     body:
       string: '{"dailySleepDTO": {"id": 1626671040000, "userProfilePK": 2591602, "calendarDate":
         "2021-07-19", "sleepTimeSeconds": 22560, "napTimeSeconds": 0, "sleepWindowConfirmed":
         true, "sleepWindowConfirmationType": "enhanced_confirmed_final", "sleepStartTimestampGMT":
         1626671040000, "sleepEndTimestampGMT": 1626695040000, "sleepStartTimestampLocal":
         1626653040000, "sleepEndTimestampLocal": 1626677040000, "autoSleepStartTimestampGMT":
@@ -117,31 +207,33 @@
         "2021-07-19T05:05:00.0", "sleepMeasurementEndGMT": "2021-07-19T11:44:00.0",
         "alertThresholdValue": null, "numberOfEventsBelowThreshold": null, "durationOfEventsBelowThreshold":
         null, "averageSPO2": 90.0, "averageSpO2HR": 50.0, "lowestSPO2": 83}}'
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7edd16712d03b6ee-QRO
+      - 7f12d010fb38475d-DFW
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json;charset=UTF-8
       Date:
-      - Fri, 28 Jul 2023 12:22:26 GMT
+      - Fri, 04 Aug 2023 00:51:35 GMT
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=V32F2QUrmMKnElYCDuDM5nkMXYdpf0PGcSTNowIElKEmoJY%2BvoMJrcJMOy0xuJ3mZnAg0tvyvmU%2ByE7EMD3%2BKniPIQk7LMUqs2kmY6VCOpZwLVIK10Qcu1LdOmitL%2BtF0QaZQA%3D%3D"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=eMCF23SNhpZfXvBbLwLcJ9MqtbFnMA33hH1OpHo5ovJI6rdsD3OtmN%2B5b7hyZkJyp5FX0Ds7lKVwYs3Ud%2Fr%2BYE2WrzgB%2FbGmlicEKi9VCJtbosDTBM06mYeypjMcvhmsg4Fr%2BIb42g%3D%3D"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Transfer-Encoding:
       - chunked
+      alt-svc:
+      - h3=":443"; ma=86400
       cache-control:
       - no-cache, no-store, private
       pragma:
       - no-cache
       set-cookie:
       - ADRUM_BT1=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
@@ -168,24 +260,20 @@
       Accept-Encoding:
       - gzip, deflate
       Authorization:
       - Bearer SANITIZED
       Connection:
       - keep-alive
       Cookie:
-      - JWT_FGP=SANITIZED; _cfuvid=SANITIZED; GARMIN-SSO=SANITIZED; GARMIN-SSO-CUST-GUID=SANITIZED;
-        GARMIN-SSO-GUID=SANITIZED; GarminNoCache=SANITIZED; ADRUM_BT1=SANITIZED; ADRUM_BTa=SANITIZED;
-        SESSIONID=SANITIZED; SameSite=SANITIZED; __cflb=SANITIZED
+      - _cfuvid=SANITIZED; ADRUM_BT1=SANITIZED; ADRUM_BTa=SANITIZED; SameSite=SANITIZED
       User-Agent:
       - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X) AppleWebKit/605.1.15
         (KHTML, like Gecko) Mobile/15E148
-      di-backend:
-      - connectapi.garmin.com
     method: GET
-    uri: https://connect.garmin.com/wellness-service/wellness/dailySleepData/mtamizi?nonSleepBufferMinutes=60&date=2021-07-18
+    uri: https://connectapi.garmin.com/wellness-service/wellness/dailySleepData/mtamizi?nonSleepBufferMinutes=60&date=2021-07-18
   response:
     body:
       string: '{"dailySleepDTO": {"id": 1626588480000, "userProfilePK": 2591602, "calendarDate":
         "2021-07-18", "sleepTimeSeconds": 26100, "napTimeSeconds": 0, "sleepWindowConfirmed":
         true, "sleepWindowConfirmationType": "enhanced_confirmed_final", "sleepStartTimestampGMT":
         1626588480000, "sleepEndTimestampGMT": 1626615420000, "sleepStartTimestampLocal":
         1626570480000, "sleepEndTimestampLocal": 1626597420000, "autoSleepStartTimestampGMT":
@@ -200,31 +288,33 @@
         "2021-07-18T06:09:00.0", "sleepMeasurementEndGMT": "2021-07-18T13:36:00.0",
         "alertThresholdValue": null, "numberOfEventsBelowThreshold": null, "durationOfEventsBelowThreshold":
         null, "averageSPO2": 91.0, "averageSpO2HR": 48.0, "lowestSPO2": 84}}'
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7edd16727c52154a-QRO
+      - 7f12d01359034768-DFW
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json;charset=UTF-8
       Date:
-      - Fri, 28 Jul 2023 12:22:27 GMT
+      - Fri, 04 Aug 2023 00:51:35 GMT
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=gZL4F1vBdhtncBy6BvcPV2TQ5%2BEQ2241ugVEuQgq09qnw21Lv3ECcJms1BkUZO5tLb3rid5ktcMNAtPgA3iafmCZ7%2FhEEX7Q8LP2E90ptvg5MXO3iRaB2mXa%2Fspte%2FO9niJz%2BQ%3D%3D"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=TXemOIhT3MxW7TfPvgRX0yMbVWTXPkmn85pRv1GiXohXOs5Avj6jNNkdiQqvBt2PwcowVugQWUAINg3UGxGJAyBkW6%2FxX3%2BL2aW%2BIeeImK9jqnGw6ESTwT6qEbldai7bo%2FYhBP56bg%3D%3D"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Transfer-Encoding:
       - chunked
+      alt-svc:
+      - h3=":443"; ma=86400
       cache-control:
       - no-cache, no-store, private
       pragma:
       - no-cache
       set-cookie:
       - ADRUM_BT1=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
@@ -251,24 +341,20 @@
       Accept-Encoding:
       - gzip, deflate
       Authorization:
       - Bearer SANITIZED
       Connection:
       - keep-alive
       Cookie:
-      - JWT_FGP=SANITIZED; _cfuvid=SANITIZED; GARMIN-SSO=SANITIZED; GARMIN-SSO-CUST-GUID=SANITIZED;
-        GARMIN-SSO-GUID=SANITIZED; GarminNoCache=SANITIZED; ADRUM_BT1=SANITIZED; ADRUM_BTa=SANITIZED;
-        SESSIONID=SANITIZED; SameSite=SANITIZED; __cflb=SANITIZED
+      - _cfuvid=SANITIZED; ADRUM_BT1=SANITIZED; ADRUM_BTa=SANITIZED; SameSite=SANITIZED
       User-Agent:
       - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X) AppleWebKit/605.1.15
         (KHTML, like Gecko) Mobile/15E148
-      di-backend:
-      - connectapi.garmin.com
     method: GET
-    uri: https://connect.garmin.com/wellness-service/wellness/dailySleepData/mtamizi?nonSleepBufferMinutes=60&date=2021-07-17
+    uri: https://connectapi.garmin.com/wellness-service/wellness/dailySleepData/mtamizi?nonSleepBufferMinutes=60&date=2021-07-17
   response:
     body:
       string: '{"dailySleepDTO": {"id": 1626500220000, "userProfilePK": 2591602, "calendarDate":
         "2021-07-17", "sleepTimeSeconds": 28800, "napTimeSeconds": 0, "sleepWindowConfirmed":
         true, "sleepWindowConfirmationType": "enhanced_confirmed_final", "sleepStartTimestampGMT":
         1626500220000, "sleepEndTimestampGMT": 1626530580000, "sleepStartTimestampLocal":
         1626482220000, "sleepEndTimestampLocal": 1626512580000, "autoSleepStartTimestampGMT":
@@ -283,31 +369,33 @@
         "2021-07-17T05:38:00.0", "sleepMeasurementEndGMT": "2021-07-17T14:01:00.0",
         "alertThresholdValue": null, "numberOfEventsBelowThreshold": null, "durationOfEventsBelowThreshold":
         null, "averageSPO2": 90.0, "averageSpO2HR": 50.0, "lowestSPO2": 83}}'
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7edd1674c9c7b6e8-QRO
+      - 7f12d0159ef14674-DFW
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json;charset=UTF-8
       Date:
-      - Fri, 28 Jul 2023 12:22:27 GMT
+      - Fri, 04 Aug 2023 00:51:36 GMT
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=pjd8iyQKzHmVbze2Qi%2BZWWM3wHOrlpxObEjC62wFrv3DdABNkdu48tuGHQkbZ5KlxG4C1YAFXaLdwT%2F8he2nElODD2verOoYFd5fntxxwqiq2ArVirtaiNeZ8PtTuebYReOsPA%3D%3D"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=pgCdzfoVvNSHnKtFrRCTKSmhU4%2FVIzENX16OwPCShsXegufDPs6hW9OpOIwGlqmP4FyxW7VLkin9TZWyS63O4DmdOWaFTa6etMtM2VNTjPcQOmgmDAF%2Faci1ms5YINMIVZOqBTBf7g%3D%3D"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Transfer-Encoding:
       - chunked
+      alt-svc:
+      - h3=":443"; ma=86400
       cache-control:
       - no-cache, no-store, private
       pragma:
       - no-cache
       set-cookie:
       - ADRUM_BT1=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
@@ -334,24 +422,20 @@
       Accept-Encoding:
       - gzip, deflate
       Authorization:
       - Bearer SANITIZED
       Connection:
       - keep-alive
       Cookie:
-      - JWT_FGP=SANITIZED; _cfuvid=SANITIZED; GARMIN-SSO=SANITIZED; GARMIN-SSO-CUST-GUID=SANITIZED;
-        GARMIN-SSO-GUID=SANITIZED; GarminNoCache=SANITIZED; ADRUM_BT1=SANITIZED; ADRUM_BTa=SANITIZED;
-        SESSIONID=SANITIZED; SameSite=SANITIZED; __cflb=SANITIZED
+      - _cfuvid=SANITIZED; ADRUM_BT1=SANITIZED; ADRUM_BTa=SANITIZED; SameSite=SANITIZED
       User-Agent:
       - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X) AppleWebKit/605.1.15
         (KHTML, like Gecko) Mobile/15E148
-      di-backend:
-      - connectapi.garmin.com
     method: GET
-    uri: https://connect.garmin.com/wellness-service/wellness/dailySleepData/mtamizi?nonSleepBufferMinutes=60&date=2021-07-16
+    uri: https://connectapi.garmin.com/wellness-service/wellness/dailySleepData/mtamizi?nonSleepBufferMinutes=60&date=2021-07-16
   response:
     body:
       string: '{"dailySleepDTO": {"id": 1626411660000, "userProfilePK": 2591602, "calendarDate":
         "2021-07-16", "sleepTimeSeconds": 22740, "napTimeSeconds": 0, "sleepWindowConfirmed":
         true, "sleepWindowConfirmationType": "enhanced_confirmed_final", "sleepStartTimestampGMT":
         1626411660000, "sleepEndTimestampGMT": 1626435360000, "sleepStartTimestampLocal":
         1626393660000, "sleepEndTimestampLocal": 1626417360000, "autoSleepStartTimestampGMT":
@@ -366,31 +450,33 @@
         "2021-07-16T05:02:00.0", "sleepMeasurementEndGMT": "2021-07-16T11:34:00.0",
         "alertThresholdValue": null, "numberOfEventsBelowThreshold": null, "durationOfEventsBelowThreshold":
         null, "averageSPO2": 92.0, "averageSpO2HR": 51.0, "lowestSPO2": 86}}'
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7edd16762e62b6e1-QRO
+      - 7f12d017ccd34781-DFW
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json;charset=UTF-8
       Date:
-      - Fri, 28 Jul 2023 12:22:27 GMT
+      - Fri, 04 Aug 2023 00:51:36 GMT
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=dP%2BK3t%2FrtdWxzxjMbY0us0vjDRPLuHs3jxTk6lbYiA2FwepP6kJZLrBUhUYcrlcHyPG2o%2BQeqMpNwtBmXJH7kPOITCC0EmFlRsosgPeRL%2BFaZewWC6jc5WHSDpnHMOsyV3wWJQ%3D%3D"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=PXKVOL42vgqaWu%2FW6x7DQt2xfGvtmaKmyjWzK0jnNbPqyqaBSDbvQPZBnSZRbCF17pdhhpMq8ddERaKeIqHWpRqiTkbaVfAGAuyiozyYpzYIVA%2BGDq0PDth6ViV6jLYOLQpdMz4Rmw%3D%3D"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Transfer-Encoding:
       - chunked
+      alt-svc:
+      - h3=":443"; ma=86400
       cache-control:
       - no-cache, no-store, private
       pragma:
       - no-cache
       set-cookie:
       - ADRUM_BT1=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
@@ -417,24 +503,20 @@
       Accept-Encoding:
       - gzip, deflate
       Authorization:
       - Bearer SANITIZED
       Connection:
       - keep-alive
       Cookie:
-      - JWT_FGP=SANITIZED; _cfuvid=SANITIZED; GARMIN-SSO=SANITIZED; GARMIN-SSO-CUST-GUID=SANITIZED;
-        GARMIN-SSO-GUID=SANITIZED; GarminNoCache=SANITIZED; ADRUM_BT1=SANITIZED; ADRUM_BTa=SANITIZED;
-        SESSIONID=SANITIZED; SameSite=SANITIZED; __cflb=SANITIZED
+      - _cfuvid=SANITIZED; ADRUM_BT1=SANITIZED; ADRUM_BTa=SANITIZED; SameSite=SANITIZED
       User-Agent:
       - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X) AppleWebKit/605.1.15
         (KHTML, like Gecko) Mobile/15E148
-      di-backend:
-      - connectapi.garmin.com
     method: GET
-    uri: https://connect.garmin.com/wellness-service/wellness/dailySleepData/mtamizi?nonSleepBufferMinutes=60&date=2021-07-15
+    uri: https://connectapi.garmin.com/wellness-service/wellness/dailySleepData/mtamizi?nonSleepBufferMinutes=60&date=2021-07-15
   response:
     body:
       string: '{"dailySleepDTO": {"id": 1626327960000, "userProfilePK": 2591602, "calendarDate":
         "2021-07-15", "sleepTimeSeconds": 21720, "napTimeSeconds": 0, "sleepWindowConfirmed":
         true, "sleepWindowConfirmationType": "enhanced_confirmed_final", "sleepStartTimestampGMT":
         1626327960000, "sleepEndTimestampGMT": 1626350400000, "sleepStartTimestampLocal":
         1626309960000, "sleepEndTimestampLocal": 1626332400000, "autoSleepStartTimestampGMT":
@@ -449,31 +531,33 @@
         "2021-07-15T05:47:00.0", "sleepMeasurementEndGMT": "2021-07-15T12:00:00.0",
         "alertThresholdValue": null, "numberOfEventsBelowThreshold": null, "durationOfEventsBelowThreshold":
         null, "averageSPO2": 92.0, "averageSpO2HR": 51.0, "lowestSPO2": 85}}'
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7edd16776ff1155e-QRO
+      - 7f12d01a1b48474f-DFW
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json;charset=UTF-8
       Date:
-      - Fri, 28 Jul 2023 12:22:27 GMT
+      - Fri, 04 Aug 2023 00:51:36 GMT
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=pa7hKrryiemKn7D0gnR37UEPA5asOQJr1pwzjEna6o1biiFVqJa7RGj9N9oahX2nLhYNGaxgwHntdcbzf5VEBv7tkkyxFZx4rI4%2BlfH0sequK3M4%2FlXYokO6vvuDpNS6lSQjtg%3D%3D"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=7pid3UMIAFp8WbajCLUNaip8agbChk73kXWIofcrPjIMGcGwu0q%2FJ%2BFOWWDHRZy9hO4C23PT21nXDuHclg2GxeNQoUn%2FTyJ6mFnRZ4E7TNXWcz%2FE7q%2FaT%2FU7mz1eaqnjNtrEbOiNwg%3D%3D"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Transfer-Encoding:
       - chunked
+      alt-svc:
+      - h3=":443"; ma=86400
       cache-control:
       - no-cache, no-store, private
       pragma:
       - no-cache
       set-cookie:
       - ADRUM_BT1=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
@@ -500,24 +584,20 @@
       Accept-Encoding:
       - gzip, deflate
       Authorization:
       - Bearer SANITIZED
       Connection:
       - keep-alive
       Cookie:
-      - JWT_FGP=SANITIZED; _cfuvid=SANITIZED; GARMIN-SSO=SANITIZED; GARMIN-SSO-CUST-GUID=SANITIZED;
-        GARMIN-SSO-GUID=SANITIZED; GarminNoCache=SANITIZED; ADRUM_BT1=SANITIZED; ADRUM_BTa=SANITIZED;
-        SESSIONID=SANITIZED; SameSite=SANITIZED; __cflb=SANITIZED
+      - _cfuvid=SANITIZED; ADRUM_BT1=SANITIZED; ADRUM_BTa=SANITIZED; SameSite=SANITIZED
       User-Agent:
       - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X) AppleWebKit/605.1.15
         (KHTML, like Gecko) Mobile/15E148
-      di-backend:
-      - connectapi.garmin.com
     method: GET
-    uri: https://connect.garmin.com/wellness-service/wellness/dailySleepData/mtamizi?nonSleepBufferMinutes=60&date=2021-07-14
+    uri: https://connectapi.garmin.com/wellness-service/wellness/dailySleepData/mtamizi?nonSleepBufferMinutes=60&date=2021-07-14
   response:
     body:
       string: '{"dailySleepDTO": {"id": 1626238140000, "userProfilePK": 2591602, "calendarDate":
         "2021-07-14", "sleepTimeSeconds": 22920, "napTimeSeconds": 0, "sleepWindowConfirmed":
         true, "sleepWindowConfirmationType": "enhanced_confirmed_final", "sleepStartTimestampGMT":
         1626238140000, "sleepEndTimestampGMT": 1626262560000, "sleepStartTimestampLocal":
         1626220140000, "sleepEndTimestampLocal": 1626244560000, "autoSleepStartTimestampGMT":
@@ -532,31 +612,33 @@
         "2021-07-14T04:50:00.0", "sleepMeasurementEndGMT": "2021-07-14T11:36:00.0",
         "alertThresholdValue": null, "numberOfEventsBelowThreshold": null, "durationOfEventsBelowThreshold":
         null, "averageSPO2": 92.0, "averageSpO2HR": 52.0, "lowestSPO2": 83}}'
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7edd16793b3a154d-QRO
+      - 7f12d01b9805b6e2-QRO
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json;charset=UTF-8
       Date:
-      - Fri, 28 Jul 2023 12:22:28 GMT
+      - Fri, 04 Aug 2023 00:51:37 GMT
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=xgtj4kMVeoq28Bgd%2F9XXlV4GhbnqE77BST%2FhdXYvNoRQDzu7RbYVAaFK%2F%2B3UR1ouZgA9itWCWWkqbC9%2FryjgSM1s00ewcAUnmVHcXUUt1xAgJawxdZgG5%2FFCa2WQUuGRKAJl0w%3D%3D"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=Kyp6FBYtZ7PEJETr2dOApNJqD8zsoYXCD6nit72%2BXd%2BD5ByvfeBC7Js6udY8%2BWbmvD7BIRzuGzKP8qIb2wTZnWrM0cRyE8EBj1OXeBqrhqRhCXezZO5WvVUtx%2FnJPz1RxVKMarAyBw%3D%3D"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Transfer-Encoding:
       - chunked
+      alt-svc:
+      - h3=":443"; ma=86400
       cache-control:
       - no-cache, no-store, private
       pragma:
       - no-cache
       set-cookie:
       - ADRUM_BT1=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
@@ -583,24 +665,20 @@
       Accept-Encoding:
       - gzip, deflate
       Authorization:
       - Bearer SANITIZED
       Connection:
       - keep-alive
       Cookie:
-      - JWT_FGP=SANITIZED; _cfuvid=SANITIZED; GARMIN-SSO=SANITIZED; GARMIN-SSO-CUST-GUID=SANITIZED;
-        GARMIN-SSO-GUID=SANITIZED; GarminNoCache=SANITIZED; ADRUM_BT1=SANITIZED; ADRUM_BTa=SANITIZED;
-        SESSIONID=SANITIZED; SameSite=SANITIZED; __cflb=SANITIZED
+      - _cfuvid=SANITIZED; ADRUM_BT1=SANITIZED; ADRUM_BTa=SANITIZED; SameSite=SANITIZED
       User-Agent:
       - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X) AppleWebKit/605.1.15
         (KHTML, like Gecko) Mobile/15E148
-      di-backend:
-      - connectapi.garmin.com
     method: GET
-    uri: https://connect.garmin.com/wellness-service/wellness/dailySleepData/mtamizi?nonSleepBufferMinutes=60&date=2021-07-13
+    uri: https://connectapi.garmin.com/wellness-service/wellness/dailySleepData/mtamizi?nonSleepBufferMinutes=60&date=2021-07-13
   response:
     body:
       string: '{"dailySleepDTO": {"id": 1626148140000, "userProfilePK": 2591602, "calendarDate":
         "2021-07-13", "sleepTimeSeconds": 27060, "napTimeSeconds": 0, "sleepWindowConfirmed":
         true, "sleepWindowConfirmationType": "enhanced_confirmed_final", "sleepStartTimestampGMT":
         1626148140000, "sleepEndTimestampGMT": 1626175920000, "sleepStartTimestampLocal":
         1626130140000, "sleepEndTimestampLocal": 1626157920000, "autoSleepStartTimestampGMT":
@@ -615,31 +693,33 @@
         "2021-07-13T03:51:00.0", "sleepMeasurementEndGMT": "2021-07-13T11:32:00.0",
         "alertThresholdValue": null, "numberOfEventsBelowThreshold": null, "durationOfEventsBelowThreshold":
         null, "averageSPO2": 92.0, "averageSpO2HR": 54.0, "lowestSPO2": 86}}'
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7edd167aabb0154a-QRO
+      - 7f12d01d0a15b6e7-QRO
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json;charset=UTF-8
       Date:
-      - Fri, 28 Jul 2023 12:22:28 GMT
+      - Fri, 04 Aug 2023 00:51:37 GMT
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=tisGfCnIWmSCDBeGYENr%2FGHXQaIU5XwcMxPWhu2vVgWQ9Cc%2FBLjF1Qcp%2B4oqJPkj7htri5N1cxS3JWltS4RHH2%2FUhAuPpzXgk4WrqAgSpZiBGFribmxwkeOHzKjqeUEZtVzmxw%3D%3D"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=y4bDuYdVHk6b%2BsQI8TbaQoTcbx51Nw7VwXcB5iGvCMvSLgBfvJh7qTCBNkidlGE%2F4soACLsKxG4PiEXrU2qtwBS%2BJPrTaN3nfWP3gYHPWEfRkHi8utIwFfKHUhvKUz6mUHHaH7QxGA%3D%3D"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Transfer-Encoding:
       - chunked
+      alt-svc:
+      - h3=":443"; ma=86400
       cache-control:
       - no-cache, no-store, private
       pragma:
       - no-cache
       set-cookie:
       - ADRUM_BT1=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
@@ -666,24 +746,20 @@
       Accept-Encoding:
       - gzip, deflate
       Authorization:
       - Bearer SANITIZED
       Connection:
       - keep-alive
       Cookie:
-      - JWT_FGP=SANITIZED; _cfuvid=SANITIZED; GARMIN-SSO=SANITIZED; GARMIN-SSO-CUST-GUID=SANITIZED;
-        GARMIN-SSO-GUID=SANITIZED; GarminNoCache=SANITIZED; ADRUM_BT1=SANITIZED; ADRUM_BTa=SANITIZED;
-        SESSIONID=SANITIZED; SameSite=SANITIZED; __cflb=SANITIZED
+      - _cfuvid=SANITIZED; ADRUM_BT1=SANITIZED; ADRUM_BTa=SANITIZED; SameSite=SANITIZED
       User-Agent:
       - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X) AppleWebKit/605.1.15
         (KHTML, like Gecko) Mobile/15E148
-      di-backend:
-      - connectapi.garmin.com
     method: GET
-    uri: https://connect.garmin.com/wellness-service/wellness/dailySleepData/mtamizi?nonSleepBufferMinutes=60&date=2021-07-12
+    uri: https://connectapi.garmin.com/wellness-service/wellness/dailySleepData/mtamizi?nonSleepBufferMinutes=60&date=2021-07-12
   response:
     body:
       string: '{"dailySleepDTO": {"id": 1626066900000, "userProfilePK": 2591602, "calendarDate":
         "2021-07-12", "sleepTimeSeconds": 22740, "napTimeSeconds": 0, "sleepWindowConfirmed":
         true, "sleepWindowConfirmationType": "enhanced_confirmed_final", "sleepStartTimestampGMT":
         1626066900000, "sleepEndTimestampGMT": 1626089640000, "sleepStartTimestampLocal":
         1626048900000, "sleepEndTimestampLocal": 1626071640000, "autoSleepStartTimestampGMT":
@@ -698,31 +774,33 @@
         "2021-07-12T05:16:00.0", "sleepMeasurementEndGMT": "2021-07-12T11:34:00.0",
         "alertThresholdValue": null, "numberOfEventsBelowThreshold": null, "durationOfEventsBelowThreshold":
         null, "averageSPO2": 92.0, "averageSpO2HR": 54.0, "lowestSPO2": 85}}'
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7edd167bd81b1547-QRO
+      - 7f12d01f7ba3486f-DFW
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json;charset=UTF-8
       Date:
-      - Fri, 28 Jul 2023 12:22:28 GMT
+      - Fri, 04 Aug 2023 00:51:37 GMT
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=nnhmzIMmMQbjUsBoiHas4%2Bw7wLktd22dg303MfeAHKsgtODydTWZPwNztsXK%2FWvxqNkVeH6J2ji9TchH2LHnBkp7Btc435YfjQMw3QFOTBMwBtNudk0CPamAHl1H65MXEiTcig%3D%3D"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=wOEZYLrzX36T%2FP7LxIeWv3eOi1vIUblM%2FgAatvAZazruO53bb5VxxKqNMb5b%2Ff7yjGyC7ptcMwg2Ofv4VkUbgZf6BfNcb4IVTiB9FO9Epgq9SxCi9yoR66qF86NSRCpg28Bf3pMG0g%3D%3D"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Transfer-Encoding:
       - chunked
+      alt-svc:
+      - h3=":443"; ma=86400
       cache-control:
       - no-cache, no-store, private
       pragma:
       - no-cache
       set-cookie:
       - ADRUM_BT1=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
@@ -749,24 +827,20 @@
       Accept-Encoding:
       - gzip, deflate
       Authorization:
       - Bearer SANITIZED
       Connection:
       - keep-alive
       Cookie:
-      - JWT_FGP=SANITIZED; _cfuvid=SANITIZED; GARMIN-SSO=SANITIZED; GARMIN-SSO-CUST-GUID=SANITIZED;
-        GARMIN-SSO-GUID=SANITIZED; GarminNoCache=SANITIZED; ADRUM_BT1=SANITIZED; ADRUM_BTa=SANITIZED;
-        SESSIONID=SANITIZED; SameSite=SANITIZED; __cflb=SANITIZED
+      - _cfuvid=SANITIZED; ADRUM_BT1=SANITIZED; ADRUM_BTa=SANITIZED; SameSite=SANITIZED
       User-Agent:
       - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X) AppleWebKit/605.1.15
         (KHTML, like Gecko) Mobile/15E148
-      di-backend:
-      - connectapi.garmin.com
     method: GET
-    uri: https://connect.garmin.com/wellness-service/wellness/dailySleepData/mtamizi?nonSleepBufferMinutes=60&date=2021-07-11
+    uri: https://connectapi.garmin.com/wellness-service/wellness/dailySleepData/mtamizi?nonSleepBufferMinutes=60&date=2021-07-11
   response:
     body:
       string: '{"dailySleepDTO": {"id": 1625978160000, "userProfilePK": 2591602, "calendarDate":
         "2021-07-11", "sleepTimeSeconds": 26040, "napTimeSeconds": 0, "sleepWindowConfirmed":
         true, "sleepWindowConfirmationType": "enhanced_confirmed_final", "sleepStartTimestampGMT":
         1625978160000, "sleepEndTimestampGMT": 1626010620000, "sleepStartTimestampLocal":
         1625960160000, "sleepEndTimestampLocal": 1625992620000, "autoSleepStartTimestampGMT":
@@ -781,31 +855,33 @@
         "2021-07-11T04:38:00.0", "sleepMeasurementEndGMT": "2021-07-11T13:36:00.0",
         "alertThresholdValue": null, "numberOfEventsBelowThreshold": null, "durationOfEventsBelowThreshold":
         null, "averageSPO2": 91.0, "averageSpO2HR": 54.0, "lowestSPO2": 78}}'
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7edd167d3f3e154d-QRO
+      - 7f12d0216eee1549-QRO
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json;charset=UTF-8
       Date:
-      - Fri, 28 Jul 2023 12:22:28 GMT
+      - Fri, 04 Aug 2023 00:51:37 GMT
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=130%2FNxYNoZbWxZw%2BbhTpWEF0v%2BPL4jJHPs5iFCeeLdmG%2FiEPfI9xj2W4zpc%2BmpwejTM1PLhuUjB%2Buhc%2FZJMIfe7GK8kjafBs8nbqFg0RpRBL121zdFmFGDfg8JnVFBLrra5y5Q%3D%3D"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=gsvldxh95pVQcbIzp28v%2B00WIXTcbzySNXlBT%2F92sEN77RYrooXBcU8S9v9rBMgG2V57ftUfxVYWnAkJTzJ6wa2CZJcMPcM9%2Bh0ZjLu%2F55iWgwfDvEQayV3F4JKWVVWn%2FjY3JEmcxw%3D%3D"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Transfer-Encoding:
       - chunked
+      alt-svc:
+      - h3=":443"; ma=86400
       cache-control:
       - no-cache, no-store, private
       pragma:
       - no-cache
       set-cookie:
       - ADRUM_BT1=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
@@ -832,24 +908,20 @@
       Accept-Encoding:
       - gzip, deflate
       Authorization:
       - Bearer SANITIZED
       Connection:
       - keep-alive
       Cookie:
-      - JWT_FGP=SANITIZED; _cfuvid=SANITIZED; GARMIN-SSO=SANITIZED; GARMIN-SSO-CUST-GUID=SANITIZED;
-        GARMIN-SSO-GUID=SANITIZED; GarminNoCache=SANITIZED; ADRUM_BT1=SANITIZED; ADRUM_BTa=SANITIZED;
-        SESSIONID=SANITIZED; SameSite=SANITIZED; __cflb=SANITIZED
+      - _cfuvid=SANITIZED; ADRUM_BT1=SANITIZED; ADRUM_BTa=SANITIZED; SameSite=SANITIZED
       User-Agent:
       - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X) AppleWebKit/605.1.15
         (KHTML, like Gecko) Mobile/15E148
-      di-backend:
-      - connectapi.garmin.com
     method: GET
-    uri: https://connect.garmin.com/wellness-service/wellness/dailySleepData/mtamizi?nonSleepBufferMinutes=60&date=2021-07-10
+    uri: https://connectapi.garmin.com/wellness-service/wellness/dailySleepData/mtamizi?nonSleepBufferMinutes=60&date=2021-07-10
   response:
     body:
       string: '{"dailySleepDTO": {"id": 1625903640000, "userProfilePK": 2591602, "calendarDate":
         "2021-07-10", "sleepTimeSeconds": 20160, "napTimeSeconds": 0, "sleepWindowConfirmed":
         true, "sleepWindowConfirmationType": "enhanced_confirmed_final", "sleepStartTimestampGMT":
         1625903640000, "sleepEndTimestampGMT": 1625926500000, "sleepStartTimestampLocal":
         1625885640000, "sleepEndTimestampLocal": 1625908500000, "autoSleepStartTimestampGMT":
@@ -864,31 +936,33 @@
         "2021-07-10T07:55:00.0", "sleepMeasurementEndGMT": "2021-07-10T14:11:00.0",
         "alertThresholdValue": null, "numberOfEventsBelowThreshold": null, "durationOfEventsBelowThreshold":
         null, "averageSPO2": 90.0, "averageSpO2HR": 56.0, "lowestSPO2": 83}}'
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7edd167e9fa3154a-QRO
+      - 7f12d022b923b6e1-QRO
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json;charset=UTF-8
       Date:
-      - Fri, 28 Jul 2023 12:22:28 GMT
+      - Fri, 04 Aug 2023 00:51:38 GMT
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=SRqmaA8aflzo%2B4kFJZYYmmNKk2vWcHtukZ49FDCNdz01QQVi6FNl9exkxXLk8B3jtSynpmdD3%2BByou0Tpd2kJh90UQdsNYRIzoVaA3uSckHSk3KullpvzweDl79IkTDtxGzAjw%3D%3D"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=jwsKC6MCMrJ5RC7h9NCaWM8LwMQI3SpxYgNIg3BRnMXEXPTshhGu2SJHrgtz2ZjNePcrnFqVntqx9x2Cfb4j5h2jJfINkVo4nV9vfPpgBMxL2pxQSBlyvUuxYZs%2BnpQe96jRDbXqqg%3D%3D"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Transfer-Encoding:
       - chunked
+      alt-svc:
+      - h3=":443"; ma=86400
       cache-control:
       - no-cache, no-store, private
       pragma:
       - no-cache
       set-cookie:
       - ADRUM_BT1=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
@@ -915,24 +989,20 @@
       Accept-Encoding:
       - gzip, deflate
       Authorization:
       - Bearer SANITIZED
       Connection:
       - keep-alive
       Cookie:
-      - JWT_FGP=SANITIZED; _cfuvid=SANITIZED; GARMIN-SSO=SANITIZED; GARMIN-SSO-CUST-GUID=SANITIZED;
-        GARMIN-SSO-GUID=SANITIZED; GarminNoCache=SANITIZED; ADRUM_BT1=SANITIZED; ADRUM_BTa=SANITIZED;
-        SESSIONID=SANITIZED; SameSite=SANITIZED; __cflb=SANITIZED
+      - _cfuvid=SANITIZED; ADRUM_BT1=SANITIZED; ADRUM_BTa=SANITIZED; SameSite=SANITIZED
       User-Agent:
       - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X) AppleWebKit/605.1.15
         (KHTML, like Gecko) Mobile/15E148
-      di-backend:
-      - connectapi.garmin.com
     method: GET
-    uri: https://connect.garmin.com/wellness-service/wellness/dailySleepData/mtamizi?nonSleepBufferMinutes=60&date=2021-07-09
+    uri: https://connectapi.garmin.com/wellness-service/wellness/dailySleepData/mtamizi?nonSleepBufferMinutes=60&date=2021-07-09
   response:
     body:
       string: '{"dailySleepDTO": {"id": 1625809560000, "userProfilePK": 2591602, "calendarDate":
         "2021-07-09", "sleepTimeSeconds": 20040, "napTimeSeconds": 0, "sleepWindowConfirmed":
         true, "sleepWindowConfirmationType": "enhanced_confirmed_final", "sleepStartTimestampGMT":
         1625809560000, "sleepEndTimestampGMT": 1625832480000, "sleepStartTimestampLocal":
         1625791560000, "sleepEndTimestampLocal": 1625814480000, "autoSleepStartTimestampGMT":
@@ -947,31 +1017,33 @@
         "2021-07-09T05:47:00.0", "sleepMeasurementEndGMT": "2021-07-09T12:06:00.0",
         "alertThresholdValue": null, "numberOfEventsBelowThreshold": null, "durationOfEventsBelowThreshold":
         null, "averageSPO2": 92.0, "averageSpO2HR": 52.0, "lowestSPO2": 76}}'
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7edd167fdafc1557-QRO
+      - 7f12d0252f7a485c-DFW
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json;charset=UTF-8
       Date:
-      - Fri, 28 Jul 2023 12:22:29 GMT
+      - Fri, 04 Aug 2023 00:51:38 GMT
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=P%2FiLgCqeTSrNi6P%2F8mDMMHdPJaenrfRx4cxHimAzdQlyIqSN1iB47ZgWZ0SQ812uU9NK4lTpFZq6Dbiy0J7KbnU6aUFUOzxnSPZvWrOBgNcaIVxCjsl09sUXneIsWXf43qwoww%3D%3D"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=zJ7oFbt70uWJOtt0%2B55RGhnCh0nOCnaB7qloify9Lx9Akj3hgV6D0dtKKNC%2FQIX6NJk0cbokv2wHKdoDEW%2Bt7Ndw5hRotoDOtPV06jAS6zNdlHsxnr5WMZjC%2FvF0FkwbMxBKhOCqgg%3D%3D"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Transfer-Encoding:
       - chunked
+      alt-svc:
+      - h3=":443"; ma=86400
       cache-control:
       - no-cache, no-store, private
       pragma:
       - no-cache
       set-cookie:
       - ADRUM_BT1=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
@@ -998,24 +1070,20 @@
       Accept-Encoding:
       - gzip, deflate
       Authorization:
       - Bearer SANITIZED
       Connection:
       - keep-alive
       Cookie:
-      - JWT_FGP=SANITIZED; _cfuvid=SANITIZED; GARMIN-SSO=SANITIZED; GARMIN-SSO-CUST-GUID=SANITIZED;
-        GARMIN-SSO-GUID=SANITIZED; GarminNoCache=SANITIZED; ADRUM_BT1=SANITIZED; ADRUM_BTa=SANITIZED;
-        SESSIONID=SANITIZED; SameSite=SANITIZED; __cflb=SANITIZED
+      - _cfuvid=SANITIZED; ADRUM_BT1=SANITIZED; ADRUM_BTa=SANITIZED; SameSite=SANITIZED
       User-Agent:
       - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X) AppleWebKit/605.1.15
         (KHTML, like Gecko) Mobile/15E148
-      di-backend:
-      - connectapi.garmin.com
     method: GET
-    uri: https://connect.garmin.com/wellness-service/wellness/dailySleepData/mtamizi?nonSleepBufferMinutes=60&date=2021-07-08
+    uri: https://connectapi.garmin.com/wellness-service/wellness/dailySleepData/mtamizi?nonSleepBufferMinutes=60&date=2021-07-08
   response:
     body:
       string: '{"dailySleepDTO": {"id": 1625721060000, "userProfilePK": 2591602, "calendarDate":
         "2021-07-08", "sleepTimeSeconds": 14460, "napTimeSeconds": 0, "sleepWindowConfirmed":
         true, "sleepWindowConfirmationType": "enhanced_confirmed_final", "sleepStartTimestampGMT":
         1625721060000, "sleepEndTimestampGMT": 1625736180000, "sleepStartTimestampLocal":
         1625703060000, "sleepEndTimestampLocal": 1625718180000, "autoSleepStartTimestampGMT":
@@ -1030,31 +1098,33 @@
         "2021-07-08T05:12:00.0", "sleepMeasurementEndGMT": "2021-07-08T09:23:00.0",
         "alertThresholdValue": null, "numberOfEventsBelowThreshold": null, "durationOfEventsBelowThreshold":
         null, "averageSPO2": 92.0, "averageSpO2HR": 52.0, "lowestSPO2": 85}}'
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7edd1682c817155f-QRO
+      - 7f12d026af141559-QRO
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json;charset=UTF-8
       Date:
-      - Fri, 28 Jul 2023 12:22:29 GMT
+      - Fri, 04 Aug 2023 00:51:38 GMT
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=OHlhL0xeORPEm9DFLbYhOgU2Zr6rHvf7KxDJf8SZXdkOmJPxnzRKnuDqcZznjoghoZh84bE%2Bby6onATK33UST5YaR7NKgTzTJgPPAV06bZ24rAIQ5qNVLh9%2FyQ6RWJJd%2FCKG1Q%3D%3D"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=iHZXPfdqlhB0eilEpnFUAr3NMskgS%2FSt1zCZBj0L69StSyKWg2e%2BkZ%2FZQ9Gbn3aF0e%2FOTHL0CmzFKHOncpvBcOjQntvUH%2BfiavmAt7aHfn1hLQOw4R9gTtx37%2BsM3Ao0qfsS3Bn8hQ%3D%3D"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Transfer-Encoding:
       - chunked
+      alt-svc:
+      - h3=":443"; ma=86400
       cache-control:
       - no-cache, no-store, private
       pragma:
       - no-cache
       set-cookie:
       - ADRUM_BT1=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
@@ -1081,24 +1151,20 @@
       Accept-Encoding:
       - gzip, deflate
       Authorization:
       - Bearer SANITIZED
       Connection:
       - keep-alive
       Cookie:
-      - JWT_FGP=SANITIZED; _cfuvid=SANITIZED; GARMIN-SSO=SANITIZED; GARMIN-SSO-CUST-GUID=SANITIZED;
-        GARMIN-SSO-GUID=SANITIZED; GarminNoCache=SANITIZED; ADRUM_BT1=SANITIZED; ADRUM_BTa=SANITIZED;
-        SESSIONID=SANITIZED; SameSite=SANITIZED; __cflb=SANITIZED
+      - _cfuvid=SANITIZED; ADRUM_BT1=SANITIZED; ADRUM_BTa=SANITIZED; SameSite=SANITIZED
       User-Agent:
       - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X) AppleWebKit/605.1.15
         (KHTML, like Gecko) Mobile/15E148
-      di-backend:
-      - connectapi.garmin.com
     method: GET
-    uri: https://connect.garmin.com/wellness-service/wellness/dailySleepData/mtamizi?nonSleepBufferMinutes=60&date=2021-07-07
+    uri: https://connectapi.garmin.com/wellness-service/wellness/dailySleepData/mtamizi?nonSleepBufferMinutes=60&date=2021-07-07
   response:
     body:
       string: '{"dailySleepDTO": {"id": 1625633700000, "userProfilePK": 2591602, "calendarDate":
         "2021-07-07", "sleepTimeSeconds": 23340, "napTimeSeconds": 0, "sleepWindowConfirmed":
         true, "sleepWindowConfirmationType": "enhanced_confirmed_final", "sleepStartTimestampGMT":
         1625633700000, "sleepEndTimestampGMT": 1625658420000, "sleepStartTimestampLocal":
         1625615700000, "sleepEndTimestampLocal": 1625640420000, "autoSleepStartTimestampGMT":
@@ -1113,31 +1179,33 @@
         "2021-07-07T04:56:00.0", "sleepMeasurementEndGMT": "2021-07-07T11:47:00.0",
         "alertThresholdValue": null, "numberOfEventsBelowThreshold": null, "durationOfEventsBelowThreshold":
         null, "averageSPO2": 92.0, "averageSpO2HR": 48.0, "lowestSPO2": 83}}'
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7edd16841968155f-QRO
+      - 7f12d027fd801556-QRO
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json;charset=UTF-8
       Date:
-      - Fri, 28 Jul 2023 12:22:29 GMT
+      - Fri, 04 Aug 2023 00:51:39 GMT
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=2pRek2wXAdMBeNVlKjRxXcSMbbeDVfLegzTwPL7FIAwr3rnJhJWbw7dxkbdCZhTZIZHznky%2FExbUf1B2nSSC7naZivBVQQ5oUT%2Bhp1o%2BTUOIW2gp6D4Jc6bcsZwfQDl%2FkHX%2BGg%3D%3D"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=ifg072PLpOiN5JuUhMzuqqfl1ndTjmx9TCZJvjoUZCgjUArPdYpQe4alkOSXspvKFXzekP10ke1p37u0XDB2jcVtpQeo3NfeBhyVUgKIwAG5t5EZOqVWD%2B9xsLMqXJihPoRTnuMdRg%3D%3D"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Transfer-Encoding:
       - chunked
+      alt-svc:
+      - h3=":443"; ma=86400
       cache-control:
       - no-cache, no-store, private
       pragma:
       - no-cache
       set-cookie:
       - ADRUM_BT1=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
@@ -1164,24 +1232,20 @@
       Accept-Encoding:
       - gzip, deflate
       Authorization:
       - Bearer SANITIZED
       Connection:
       - keep-alive
       Cookie:
-      - JWT_FGP=SANITIZED; _cfuvid=SANITIZED; GARMIN-SSO=SANITIZED; GARMIN-SSO-CUST-GUID=SANITIZED;
-        GARMIN-SSO-GUID=SANITIZED; GarminNoCache=SANITIZED; ADRUM_BT1=SANITIZED; ADRUM_BTa=SANITIZED;
-        SESSIONID=SANITIZED; SameSite=SANITIZED; __cflb=SANITIZED
+      - _cfuvid=SANITIZED; ADRUM_BT1=SANITIZED; ADRUM_BTa=SANITIZED; SameSite=SANITIZED
       User-Agent:
       - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X) AppleWebKit/605.1.15
         (KHTML, like Gecko) Mobile/15E148
-      di-backend:
-      - connectapi.garmin.com
     method: GET
-    uri: https://connect.garmin.com/wellness-service/wellness/dailySleepData/mtamizi?nonSleepBufferMinutes=60&date=2021-07-06
+    uri: https://connectapi.garmin.com/wellness-service/wellness/dailySleepData/mtamizi?nonSleepBufferMinutes=60&date=2021-07-06
   response:
     body:
       string: '{"dailySleepDTO": {"id": 1625543220000, "userProfilePK": 2591602, "calendarDate":
         "2021-07-06", "sleepTimeSeconds": 27660, "napTimeSeconds": 0, "sleepWindowConfirmed":
         true, "sleepWindowConfirmationType": "enhanced_confirmed_final", "sleepStartTimestampGMT":
         1625543220000, "sleepEndTimestampGMT": 1625571900000, "sleepStartTimestampLocal":
         1625525220000, "sleepEndTimestampLocal": 1625553900000, "autoSleepStartTimestampGMT":
@@ -1196,31 +1260,33 @@
         "2021-07-06T03:48:00.0", "sleepMeasurementEndGMT": "2021-07-06T11:45:00.0",
         "alertThresholdValue": null, "numberOfEventsBelowThreshold": null, "durationOfEventsBelowThreshold":
         null, "averageSPO2": 93.0, "averageSpO2HR": 52.0, "lowestSPO2": 87}}'
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7edd16855fd1154b-QRO
+      - 7f12d02a7fc2b6e2-QRO
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json;charset=UTF-8
       Date:
-      - Fri, 28 Jul 2023 12:22:30 GMT
+      - Fri, 04 Aug 2023 00:51:39 GMT
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=ISOxj2CL9i8mMf0veqqOK4JwQx2h3RYWhGWvOT1TqJpAI2BIfdf4gKojXmhg6Z%2FfYTy3Feb7uawJHdKzVvLOSEQLDG3N6RKPG66m%2BSVWtpguw8GtbbjE%2B5Mp2EUXNdSfxSvdJw%3D%3D"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=sJt1xIs%2BBX85Utg6JZC%2BvLjLKrO%2F2KUG3p4NU3yPZPDZhTP24CkFrQGvhKLElwF4cZ9lLOMZkB3fCIPi71OCE%2B9hibWbSxdUVUoLhcWKSPqGWALrPm2tLAy8v%2FcNtQy0uZ8VW6aqEg%3D%3D"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Transfer-Encoding:
       - chunked
+      alt-svc:
+      - h3=":443"; ma=86400
       cache-control:
       - no-cache, no-store, private
       pragma:
       - no-cache
       set-cookie:
       - ADRUM_BT1=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
@@ -1228,18 +1294,14 @@
         Secure
       - ADRUM_BTa=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
       - ADRUM_BTa=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
       - SameSite=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
-      - ADRUM_BT1=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
-        Secure
-      - ADRUM_BT1=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
-        Secure
     status:
       code: 200
       message: OK
 - request:
     body: null
     headers:
       Accept:
@@ -1247,24 +1309,20 @@
       Accept-Encoding:
       - gzip, deflate
       Authorization:
       - Bearer SANITIZED
       Connection:
       - keep-alive
       Cookie:
-      - JWT_FGP=SANITIZED; _cfuvid=SANITIZED; GARMIN-SSO=SANITIZED; GARMIN-SSO-CUST-GUID=SANITIZED;
-        GARMIN-SSO-GUID=SANITIZED; GarminNoCache=SANITIZED; ADRUM_BT1=SANITIZED; ADRUM_BTa=SANITIZED;
-        SESSIONID=SANITIZED; SameSite=SANITIZED; __cflb=SANITIZED
+      - _cfuvid=SANITIZED; ADRUM_BTa=SANITIZED; SameSite=SANITIZED
       User-Agent:
       - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X) AppleWebKit/605.1.15
         (KHTML, like Gecko) Mobile/15E148
-      di-backend:
-      - connectapi.garmin.com
     method: GET
-    uri: https://connect.garmin.com/wellness-service/wellness/dailySleepData/mtamizi?nonSleepBufferMinutes=60&date=2021-07-05
+    uri: https://connectapi.garmin.com/wellness-service/wellness/dailySleepData/mtamizi?nonSleepBufferMinutes=60&date=2021-07-05
   response:
     body:
       string: '{"dailySleepDTO": {"id": 1625454360000, "userProfilePK": 2591602, "calendarDate":
         "2021-07-05", "sleepTimeSeconds": 26580, "napTimeSeconds": 0, "sleepWindowConfirmed":
         true, "sleepWindowConfirmationType": "enhanced_confirmed_final", "sleepStartTimestampGMT":
         1625454360000, "sleepEndTimestampGMT": 1625485260000, "sleepStartTimestampLocal":
         1625436360000, "sleepEndTimestampLocal": 1625467260000, "autoSleepStartTimestampGMT":
@@ -1279,38 +1337,38 @@
         "2021-07-05T03:11:00.0", "sleepMeasurementEndGMT": "2021-07-05T11:41:00.0",
         "alertThresholdValue": null, "numberOfEventsBelowThreshold": null, "durationOfEventsBelowThreshold":
         null, "averageSPO2": 93.0, "averageSpO2HR": 49.0, "lowestSPO2": 86}}'
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7edd168698e1154b-QRO
+      - 7f12d02c2b211559-QRO
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json;charset=UTF-8
       Date:
-      - Fri, 28 Jul 2023 12:22:30 GMT
+      - Fri, 04 Aug 2023 00:51:39 GMT
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=ccgRr0MfDX31%2Fez%2B0MQvghj6sTQxRqQyCkYrKv6zk202kGaXHKni1dqw7lypYlJwdMTjsbybYnB1haKtDZTD2eXJ7dSLh2gXqTbGxB3i5C8IOLtwJSysEy5R6CVuX57ahBxRLQ%3D%3D"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=nMs9WRQTY82z8VC93fcCUPrzj%2B%2Fgph7yvVyZmb7YdU48ItUVbvLzI56jo3qT5a2nGser8F7ONUa54J3KOXm%2BmmNwDzStOyGVNNqZULYQow%2BBzf3eazZF%2BjRb3wOxyBmh7dNxswXptw%3D%3D"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Transfer-Encoding:
       - chunked
+      alt-svc:
+      - h3=":443"; ma=86400
       cache-control:
       - no-cache, no-store, private
       pragma:
       - no-cache
       set-cookie:
-      - ADRUM_BT1=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
-        Secure
       - ADRUM_BTa=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
       - ADRUM_BTa=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
       - ADRUM_BTa=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
       - SameSite=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
@@ -1330,24 +1388,20 @@
       Accept-Encoding:
       - gzip, deflate
       Authorization:
       - Bearer SANITIZED
       Connection:
       - keep-alive
       Cookie:
-      - JWT_FGP=SANITIZED; _cfuvid=SANITIZED; GARMIN-SSO=SANITIZED; GARMIN-SSO-CUST-GUID=SANITIZED;
-        GARMIN-SSO-GUID=SANITIZED; GarminNoCache=SANITIZED; ADRUM_BT1=SANITIZED; ADRUM_BTa=SANITIZED;
-        SESSIONID=SANITIZED; SameSite=SANITIZED; __cflb=SANITIZED
+      - _cfuvid=SANITIZED; ADRUM_BT1=SANITIZED; ADRUM_BTa=SANITIZED; SameSite=SANITIZED
       User-Agent:
       - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X) AppleWebKit/605.1.15
         (KHTML, like Gecko) Mobile/15E148
-      di-backend:
-      - connectapi.garmin.com
     method: GET
-    uri: https://connect.garmin.com/wellness-service/wellness/dailySleepData/mtamizi?nonSleepBufferMinutes=60&date=2021-07-04
+    uri: https://connectapi.garmin.com/wellness-service/wellness/dailySleepData/mtamizi?nonSleepBufferMinutes=60&date=2021-07-04
   response:
     body:
       string: '{"dailySleepDTO": {"id": 1625377380000, "userProfilePK": 2591602, "calendarDate":
         "2021-07-04", "sleepTimeSeconds": 28740, "napTimeSeconds": 0, "sleepWindowConfirmed":
         true, "sleepWindowConfirmationType": "enhanced_confirmed_final", "sleepStartTimestampGMT":
         1625377380000, "sleepEndTimestampGMT": 1625408580000, "sleepStartTimestampLocal":
         1625359380000, "sleepEndTimestampLocal": 1625390580000, "autoSleepStartTimestampGMT":
@@ -1362,31 +1416,33 @@
         "2021-07-04T05:44:00.0", "sleepMeasurementEndGMT": "2021-07-04T14:21:00.0",
         "alertThresholdValue": null, "numberOfEventsBelowThreshold": null, "durationOfEventsBelowThreshold":
         null, "averageSPO2": 92.0, "averageSpO2HR": 46.0, "lowestSPO2": 86}}'
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7edd1687e9911549-QRO
+      - 7f12d02d8920b6e5-QRO
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json;charset=UTF-8
       Date:
-      - Fri, 28 Jul 2023 12:22:30 GMT
+      - Fri, 04 Aug 2023 00:51:39 GMT
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=j8n0pEOa6blnbYHgUH2nLfNjxITyiTPPKVTPd%2F%2FY%2B7lA%2FAoVaEMEe6wU8trJRacZU%2ByGD70ttDS7cbN7VyMKNTCQSsgaYNyR4fCwocXjmeEy%2BzixHjY%2BqvkFnC8lHVy1V%2BP9Xg%3D%3D"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=OYnt5vplcguEr%2BMWMZrvvk0GYMP69QkpAj3VQB224nl7BED1UgTx6xl4cREfj7qvsK3c5FoCnCxzTUzuiz76EESc1Fzj1A1FzXo50JchiAGhlwo0PzigjF4iFd2TbIqTpkroihax6A%3D%3D"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Transfer-Encoding:
       - chunked
+      alt-svc:
+      - h3=":443"; ma=86400
       cache-control:
       - no-cache, no-store, private
       pragma:
       - no-cache
       set-cookie:
       - ADRUM_BT1=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
@@ -1413,24 +1469,20 @@
       Accept-Encoding:
       - gzip, deflate
       Authorization:
       - Bearer SANITIZED
       Connection:
       - keep-alive
       Cookie:
-      - JWT_FGP=SANITIZED; _cfuvid=SANITIZED; GARMIN-SSO=SANITIZED; GARMIN-SSO-CUST-GUID=SANITIZED;
-        GARMIN-SSO-GUID=SANITIZED; GarminNoCache=SANITIZED; ADRUM_BT1=SANITIZED; ADRUM_BTa=SANITIZED;
-        SESSIONID=SANITIZED; SameSite=SANITIZED; __cflb=SANITIZED
+      - _cfuvid=SANITIZED; ADRUM_BT1=SANITIZED; ADRUM_BTa=SANITIZED; SameSite=SANITIZED
       User-Agent:
       - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X) AppleWebKit/605.1.15
         (KHTML, like Gecko) Mobile/15E148
-      di-backend:
-      - connectapi.garmin.com
     method: GET
-    uri: https://connect.garmin.com/wellness-service/wellness/dailySleepData/mtamizi?nonSleepBufferMinutes=60&date=2021-07-03
+    uri: https://connectapi.garmin.com/wellness-service/wellness/dailySleepData/mtamizi?nonSleepBufferMinutes=60&date=2021-07-03
   response:
     body:
       string: '{"dailySleepDTO": {"id": 1625287440000, "userProfilePK": 2591602, "calendarDate":
         "2021-07-03", "sleepTimeSeconds": 31560, "napTimeSeconds": 0, "sleepWindowConfirmed":
         true, "sleepWindowConfirmationType": "enhanced_confirmed_final", "sleepStartTimestampGMT":
         1625287440000, "sleepEndTimestampGMT": 1625324100000, "sleepStartTimestampLocal":
         1625269440000, "sleepEndTimestampLocal": 1625306100000, "autoSleepStartTimestampGMT":
@@ -1445,31 +1497,33 @@
         "2021-07-03T04:45:00.0", "sleepMeasurementEndGMT": "2021-07-03T14:51:00.0",
         "alertThresholdValue": null, "numberOfEventsBelowThreshold": null, "durationOfEventsBelowThreshold":
         null, "averageSPO2": 94.0, "averageSpO2HR": 48.0, "lowestSPO2": 86}}'
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7edd16893bc5b6e8-QRO
+      - 7f12d02fdea8479f-DFW
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json;charset=UTF-8
       Date:
-      - Fri, 28 Jul 2023 12:22:30 GMT
+      - Fri, 04 Aug 2023 00:51:40 GMT
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=URqzYuUCORT%2F5JQFvwZCAGJYGEiNT2cbAKjDPXiaLoDPsiu2Kg6b2HNQbvHyKFVtF16O1%2BkvCOGzHGd%2Bze6PAWQfYExaA%2BY7SrgY5HnAIAGp%2BwSLzm3nsZyyfcTyHQdA%2FFvf7w%3D%3D"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=2zDoFbPuDLnEVyOygcc2ffTzJmal6bNbuXT5s8sxRx1k9CXheXfQt8pHYnV1FSYeZZNxh5mCMTBxZiTME442zDoAaHyPGcsPLy8UyjKuPFwp1hm1ohIN6yfKB%2F1cQmLBe3FTPxnQKQ%3D%3D"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Transfer-Encoding:
       - chunked
+      alt-svc:
+      - h3=":443"; ma=86400
       cache-control:
       - no-cache, no-store, private
       pragma:
       - no-cache
       set-cookie:
       - ADRUM_BT1=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
@@ -1496,24 +1550,20 @@
       Accept-Encoding:
       - gzip, deflate
       Authorization:
       - Bearer SANITIZED
       Connection:
       - keep-alive
       Cookie:
-      - JWT_FGP=SANITIZED; _cfuvid=SANITIZED; GARMIN-SSO=SANITIZED; GARMIN-SSO-CUST-GUID=SANITIZED;
-        GARMIN-SSO-GUID=SANITIZED; GarminNoCache=SANITIZED; ADRUM_BT1=SANITIZED; ADRUM_BTa=SANITIZED;
-        SESSIONID=SANITIZED; SameSite=SANITIZED; __cflb=SANITIZED
+      - _cfuvid=SANITIZED; ADRUM_BT1=SANITIZED; ADRUM_BTa=SANITIZED; SameSite=SANITIZED
       User-Agent:
       - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X) AppleWebKit/605.1.15
         (KHTML, like Gecko) Mobile/15E148
-      di-backend:
-      - connectapi.garmin.com
     method: GET
-    uri: https://connect.garmin.com/wellness-service/wellness/dailySleepData/mtamizi?nonSleepBufferMinutes=60&date=2021-07-02
+    uri: https://connectapi.garmin.com/wellness-service/wellness/dailySleepData/mtamizi?nonSleepBufferMinutes=60&date=2021-07-02
   response:
     body:
       string: '{"dailySleepDTO": {"id": 1625199840000, "userProfilePK": 2591602, "calendarDate":
         "2021-07-02", "sleepTimeSeconds": 30600, "napTimeSeconds": 0, "sleepWindowConfirmed":
         true, "sleepWindowConfirmationType": "enhanced_confirmed_final", "sleepStartTimestampGMT":
         1625199840000, "sleepEndTimestampGMT": 1625230740000, "sleepStartTimestampLocal":
         1625181840000, "sleepEndTimestampLocal": 1625212740000, "autoSleepStartTimestampGMT":
@@ -1528,31 +1578,33 @@
         "2021-07-02T04:25:00.0", "sleepMeasurementEndGMT": "2021-07-02T12:56:00.0",
         "alertThresholdValue": null, "numberOfEventsBelowThreshold": null, "durationOfEventsBelowThreshold":
         null, "averageSPO2": 93.0, "averageSpO2HR": 49.0, "lowestSPO2": 76}}'
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7edd168a7bbc155e-QRO
+      - 7f12d0323b94477e-DFW
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json;charset=UTF-8
       Date:
-      - Fri, 28 Jul 2023 12:22:30 GMT
+      - Fri, 04 Aug 2023 00:51:40 GMT
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=5RP3yU27xbdQIFHdAHxr3sf9ZzY1trqkX3%2Bh4vf9BSBGjbbgbDCdcw8fiYFbIfWS2wrVuPcuB2tw4fU%2BQLsMuJTYhL5XBBIFliALE56EfA677mVWZKKlahF7nv4AY4S7kc2NTA%3D%3D"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=GZsQF5tWMyKsN8SH%2Fm9w1R1dbJa%2BGtdX1pKGeCnk7vedyBCwc1XRmF%2FhhO%2B55KOuwMRMelQdt9ztchI7Oe770%2FxMjmdnEk1tOU0Ut%2FrXqE%2B4%2Bfe8yUp5cOmgNyi2T4ZX4yZZqZZgQQ%3D%3D"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Transfer-Encoding:
       - chunked
+      alt-svc:
+      - h3=":443"; ma=86400
       cache-control:
       - no-cache, no-store, private
       pragma:
       - no-cache
       set-cookie:
       - ADRUM_BT1=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
@@ -1579,24 +1631,20 @@
       Accept-Encoding:
       - gzip, deflate
       Authorization:
       - Bearer SANITIZED
       Connection:
       - keep-alive
       Cookie:
-      - JWT_FGP=SANITIZED; _cfuvid=SANITIZED; GARMIN-SSO=SANITIZED; GARMIN-SSO-CUST-GUID=SANITIZED;
-        GARMIN-SSO-GUID=SANITIZED; GarminNoCache=SANITIZED; ADRUM_BT1=SANITIZED; ADRUM_BTa=SANITIZED;
-        SESSIONID=SANITIZED; SameSite=SANITIZED; __cflb=SANITIZED
+      - _cfuvid=SANITIZED; ADRUM_BT1=SANITIZED; ADRUM_BTa=SANITIZED; SameSite=SANITIZED
       User-Agent:
       - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X) AppleWebKit/605.1.15
         (KHTML, like Gecko) Mobile/15E148
-      di-backend:
-      - connectapi.garmin.com
     method: GET
-    uri: https://connect.garmin.com/wellness-service/wellness/dailySleepData/mtamizi?nonSleepBufferMinutes=60&date=2021-07-01
+    uri: https://connectapi.garmin.com/wellness-service/wellness/dailySleepData/mtamizi?nonSleepBufferMinutes=60&date=2021-07-01
   response:
     body:
       string: '{"dailySleepDTO": {"id": 1625121120000, "userProfilePK": 2591602, "calendarDate":
         "2021-07-01", "sleepTimeSeconds": 18540, "napTimeSeconds": 0, "sleepWindowConfirmed":
         true, "sleepWindowConfirmationType": "enhanced_confirmed_final", "sleepStartTimestampGMT":
         1625121120000, "sleepEndTimestampGMT": 1625139660000, "sleepStartTimestampLocal":
         1625103120000, "sleepEndTimestampLocal": 1625121660000, "autoSleepStartTimestampGMT":
@@ -1611,31 +1659,33 @@
         "2021-07-01T06:33:00.0", "sleepMeasurementEndGMT": "2021-07-01T11:41:00.0",
         "alertThresholdValue": null, "numberOfEventsBelowThreshold": null, "durationOfEventsBelowThreshold":
         null, "averageSPO2": 94.0, "averageSpO2HR": 49.0, "lowestSPO2": 89}}'
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7edd168bcd341549-QRO
+      - 7f12d03468604648-DFW
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json;charset=UTF-8
       Date:
-      - Fri, 28 Jul 2023 12:22:31 GMT
+      - Fri, 04 Aug 2023 00:51:40 GMT
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=ci9vTJfRpbpvcu8QB4N4cidFSkj8rkU9XQbrYwYOgkAdEENJzNVWMVTt8%2BBpRVkoj8X2MrFNSjD1sztgeqtu%2BhEC3lUstQL30spOCZzRdhHukaAXiWindpBBhY5KvjVonDgoBA%3D%3D"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=mt8J8CRV5GtFo8E8D26OaBraXA6evjbJYOOVglh7eOBYQxrZMo8A5evAgOGF7%2BJXYx2OQEw4ewL4vDmEFd7sp8XDG9OgCJjPDmAAtcbpRQrWW%2BYIBZ3gljamEq0T1dDz03YQTb4u%2BQ%3D%3D"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Transfer-Encoding:
       - chunked
+      alt-svc:
+      - h3=":443"; ma=86400
       cache-control:
       - no-cache, no-store, private
       pragma:
       - no-cache
       set-cookie:
       - ADRUM_BT1=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
```

### Comparing `garth-0.3.5/tests/resources/cassettes/test_weekly_steps.yaml` & `garth-0.4.0/tests/stats/cassettes/test_weekly_steps.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,19 @@
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Authorization:
       - Bearer SANITIZED
       Connection:
       - keep-alive
-      Cookie:
-      - JWT_FGP=SANITIZED; _cfuvid=SANITIZED; GARMIN-SSO=SANITIZED; GARMIN-SSO-CUST-GUID=SANITIZED;
-        GARMIN-SSO-GUID=SANITIZED; GarminNoCache=SANITIZED; SESSIONID=SANITIZED; __cflb=SANITIZED
       User-Agent:
       - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X) AppleWebKit/605.1.15
         (KHTML, like Gecko) Mobile/15E148
-      di-backend:
-      - connectapi.garmin.com
     method: GET
-    uri: https://connect.garmin.com/usersummary-service/stats/steps/weekly/2023-07-20/52
+    uri: https://connectapi.garmin.com/usersummary-service/stats/steps/weekly/2023-07-20/52
   response:
     body:
       string: '[{"calendarDate": "2022-07-22", "values": {"totalSteps": 55744.0, "averageSteps":
         7963.428571428572, "wellnessDataDaysCount": 7, "averageDistance": 7138.571428571428,
         "totalDistance": 49970.0}}, {"calendarDate": "2022-07-29", "values": {"totalSteps":
         94875.0, "averageSteps": 13553.57142857143, "wellnessDataDaysCount": 7, "averageDistance":
         12255.42857142857, "totalDistance": 85788.0}}, {"calendarDate": "2022-08-05",
@@ -142,31 +137,33 @@
         "2023-07-14", "values": {"totalSteps": 43517.0, "averageSteps": 6216.714285714285,
         "wellnessDataDaysCount": 7, "averageDistance": 5155.857142857143, "totalDistance":
         36091.0}}]'
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7ee737adac3db6ee-QRO
+      - 7f12d0372c6bb6e8-QRO
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json
       Date:
-      - Sat, 29 Jul 2023 17:52:45 GMT
+      - Fri, 04 Aug 2023 00:51:41 GMT
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=wBzsVsqBE0q4MpDCAwxph9mr3nHJyUeDFLqE7r%2Bb7CK0J4rlBK40JSN3Jxs13SN13QBA3fX1X9YDzOJerOJli8lXugo%2FREaYpoNEfW0gdRhUGciwjciDZ63qzN7o%2FEYCJ6HENA%3D%3D"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=%2Bl0XlZIluxXu3lx%2F%2Fvhv0VqJ4KvnGO6IAsrscPL0HZHlylqX0y1KAU6diNA2mkaRA%2F20r75szglAnaZoHg8BB36YlL9OY46kV5b7J3%2BPf%2BhJrMp4E1NBhVysMDNWMSomy15E0rLf3w%3D%3D"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Transfer-Encoding:
       - chunked
+      alt-svc:
+      - h3=":443"; ma=86400
       cache-control:
       - no-cache, no-store, private
       pragma:
       - no-cache
       set-cookie:
       - ADRUM_BTa=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
@@ -174,11 +171,12 @@
         Secure
       - SameSite=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
       - ADRUM_BT1=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
       - ADRUM_BT1=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
+      - _cfuvid=SANITIZED; path=SANITIZED; domain=SANITIZED; HttpOnly; Secure; SameSite=SANITIZED
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `garth-0.3.5/tests/resources/cassettes/test_weekly_stress.yaml` & `garth-0.4.0/tests/stats/cassettes/test_weekly_stress.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -6,26 +6,19 @@
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Authorization:
       - Bearer SANITIZED
       Connection:
       - keep-alive
-      Cookie:
-      - JWT_FGP=SANITIZED; _cfuvid=SANITIZED; GARMIN-SSO=SANITIZED; GARMIN-SSO-CUST-GUID=SANITIZED;
-        GARMIN-SSO-GUID=SANITIZED; GarminNoCache=SANITIZED; SESSIONID=SANITIZED; __cflb=SANITIZED
       User-Agent:
       - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X) AppleWebKit/605.1.15
         (KHTML, like Gecko) Mobile/15E148
-      di-backend:
-      - connectapi.garmin.com
-      referer:
-      - https://connect.garmin.com/modern
     method: GET
-    uri: https://connect.garmin.com/usersummary-service/stats/stress/weekly/2023-07-20/52
+    uri: https://connectapi.garmin.com/usersummary-service/stats/stress/weekly/2023-07-20/52
   response:
     body:
       string: '[{"calendarDate": "2022-07-22", "value": 25}, {"calendarDate": "2022-07-29",
         "value": 26}, {"calendarDate": "2022-08-05", "value": 27}, {"calendarDate":
         "2022-08-12", "value": 29}, {"calendarDate": "2022-08-19", "value": 28}, {"calendarDate":
         "2022-08-26", "value": 25}, {"calendarDate": "2022-09-02", "value": 27}, {"calendarDate":
         "2022-09-09", "value": 23}, {"calendarDate": "2022-09-16", "value": 30}, {"calendarDate":
@@ -51,31 +44,33 @@
         "2023-06-16", "value": 34}, {"calendarDate": "2023-06-23", "value": 32}, {"calendarDate":
         "2023-06-30", "value": 37}, {"calendarDate": "2023-07-07", "value": 30}, {"calendarDate":
         "2023-07-14", "value": 34}]'
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7eb7a4270fc0b6eb-QRO
+      - 7f12d03ffc58b6eb-QRO
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json
       Date:
-      - Sun, 23 Jul 2023 23:18:12 GMT
+      - Fri, 04 Aug 2023 00:51:42 GMT
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=VZFQmFj1Jb3Bf1bfAB418EH1WsmW3C%2BXcVJfLnHdzLsdGwmJ7fDPCIMr6JL1ENYzrM0vFsudzxCrLXWSVm1rIMD6vwxvJmtYci%2Bvvx0cXq6%2BT8makXdIRTegNXuN3NtbBAk1GA%3D%3D"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=c%2Bq23QlhxezPwKLyUBjr6tmWN4AZf%2BwdBFpeaH%2B8ptr8Chz1U7tVP0yr5Iwd3AWLlLKb4%2FU%2FZt9as1Beq5oi7qmkfbZVxerJpLZT5Lgj1AbocbMEZKJMkIuI4iH3JjXtNbisFpZ15A%3D%3D"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Transfer-Encoding:
       - chunked
+      alt-svc:
+      - h3=":443"; ma=86400
       cache-control:
       - no-cache, no-store, private
       pragma:
       - no-cache
       set-cookie:
       - ADRUM_BTa=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
@@ -83,11 +78,12 @@
         Secure
       - SameSite=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
       - ADRUM_BT1=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
       - ADRUM_BT1=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
+      - _cfuvid=SANITIZED; path=SANITIZED; domain=SANITIZED; HttpOnly; Secure; SameSite=SANITIZED
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `garth-0.3.5/tests/resources/cassettes/test_weekly_stress_beyond_data.yaml` & `garth-0.4.0/tests/stats/cassettes/test_weekly_stress_beyond_data.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -6,26 +6,19 @@
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Authorization:
       - Bearer SANITIZED
       Connection:
       - keep-alive
-      Cookie:
-      - JWT_FGP=SANITIZED; _cfuvid=SANITIZED; GARMIN-SSO=SANITIZED; GARMIN-SSO-CUST-GUID=SANITIZED;
-        GARMIN-SSO-GUID=SANITIZED; GarminNoCache=SANITIZED; SESSIONID=SANITIZED; __cflb=SANITIZED
       User-Agent:
       - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X) AppleWebKit/605.1.15
         (KHTML, like Gecko) Mobile/15E148
-      di-backend:
-      - connectapi.garmin.com
-      referer:
-      - https://connect.garmin.com/modern
     method: GET
-    uri: https://connect.garmin.com/usersummary-service/stats/stress/weekly/2023-07-20/52
+    uri: https://connectapi.garmin.com/usersummary-service/stats/stress/weekly/2023-07-20/52
   response:
     body:
       string: '[{"calendarDate": "2022-07-22", "value": 25}, {"calendarDate": "2022-07-29",
         "value": 26}, {"calendarDate": "2022-08-05", "value": 27}, {"calendarDate":
         "2022-08-12", "value": 29}, {"calendarDate": "2022-08-19", "value": 28}, {"calendarDate":
         "2022-08-26", "value": 25}, {"calendarDate": "2022-09-02", "value": 27}, {"calendarDate":
         "2022-09-09", "value": 23}, {"calendarDate": "2022-09-16", "value": 30}, {"calendarDate":
@@ -51,31 +44,33 @@
         "2023-06-16", "value": 34}, {"calendarDate": "2023-06-23", "value": 32}, {"calendarDate":
         "2023-06-30", "value": 37}, {"calendarDate": "2023-07-07", "value": 30}, {"calendarDate":
         "2023-07-14", "value": 34}]'
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7ed31509be6db6e2-QRO
+      - 7f12d0453bdcb6ee-QRO
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json
       Date:
-      - Thu, 27 Jul 2023 07:13:51 GMT
+      - Fri, 04 Aug 2023 00:51:43 GMT
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=dM%2B0KMFMfZr2VIp4NH5rFSxTCoVDh2NcCcj%2FphiSlbZOcSi55BATmyNN0D8buyoKiodPfK0W5eCXvyUGW3Bh42nS7XKQdP6F0ArrX%2FvMk5QIAKcH6XmrIt81CWKeFfFOqPei9g%3D%3D"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=%2Fj7%2FvJ22rfZra5GhmEE5pmlC5Uc5K7RATmiYeptCVaJa1E61Q0f%2BTBQPro8xMN0YITaOvrYVpSdUUbRy7hrfwnTy%2F2zxGhQtGCXOJFwDQahKMB9ZM%2FVdAwbk6%2FzMi7kxx%2BZRJXTUSg%3D%3D"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Transfer-Encoding:
       - chunked
+      alt-svc:
+      - h3=":443"; ma=86400
       cache-control:
       - no-cache, no-store, private
       pragma:
       - no-cache
       set-cookie:
       - ADRUM_BTa=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
@@ -83,14 +78,15 @@
         Secure
       - SameSite=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
       - ADRUM_BT1=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
       - ADRUM_BT1=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
+      - _cfuvid=SANITIZED; path=SANITIZED; domain=SANITIZED; HttpOnly; Secure; SameSite=SANITIZED
     status:
       code: 200
       message: OK
 - request:
     body: null
     headers:
       Accept:
@@ -98,26 +94,20 @@
       Accept-Encoding:
       - gzip, deflate
       Authorization:
       - Bearer SANITIZED
       Connection:
       - keep-alive
       Cookie:
-      - JWT_FGP=SANITIZED; _cfuvid=SANITIZED; GARMIN-SSO=SANITIZED; GARMIN-SSO-CUST-GUID=SANITIZED;
-        GARMIN-SSO-GUID=SANITIZED; GarminNoCache=SANITIZED; ADRUM_BT1=SANITIZED; ADRUM_BTa=SANITIZED;
-        SESSIONID=SANITIZED; SameSite=SANITIZED; __cflb=SANITIZED
+      - _cfuvid=SANITIZED; ADRUM_BT1=SANITIZED; ADRUM_BTa=SANITIZED; SameSite=SANITIZED
       User-Agent:
       - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X) AppleWebKit/605.1.15
         (KHTML, like Gecko) Mobile/15E148
-      di-backend:
-      - connectapi.garmin.com
-      referer:
-      - https://connect.garmin.com/modern
     method: GET
-    uri: https://connect.garmin.com/usersummary-service/stats/stress/weekly/2022-07-21/52
+    uri: https://connectapi.garmin.com/usersummary-service/stats/stress/weekly/2022-07-21/52
   response:
     body:
       string: '[{"calendarDate": "2021-07-23", "value": 28}, {"calendarDate": "2021-07-30",
         "value": 27}, {"calendarDate": "2021-08-06", "value": 25}, {"calendarDate":
         "2021-08-13", "value": 24}, {"calendarDate": "2021-08-20", "value": 28}, {"calendarDate":
         "2021-08-27", "value": 24}, {"calendarDate": "2021-09-03", "value": 32}, {"calendarDate":
         "2021-09-10", "value": 28}, {"calendarDate": "2021-09-17", "value": 26}, {"calendarDate":
@@ -143,31 +133,33 @@
         "2022-06-17", "value": 27}, {"calendarDate": "2022-06-24", "value": 30}, {"calendarDate":
         "2022-07-01", "value": 29}, {"calendarDate": "2022-07-08", "value": 31}, {"calendarDate":
         "2022-07-15", "value": 29}]'
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7ed3150b4cea1557-QRO
+      - 7f12d046b9ab1556-QRO
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json
       Date:
-      - Thu, 27 Jul 2023 07:13:51 GMT
+      - Fri, 04 Aug 2023 00:51:43 GMT
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=cHo7%2BtwVkvRm3Fu%2F4uStl1Rk1Ov82KMzDzmAzMWHkpV433KWK3e%2FUrBozQWb4izknis544WtWpcKL4DUro%2Fiake378rrkkMQ5zjlfE0kn25bXI%2BX3xH0IW83byOE5Wknj%2B4fLw%3D%3D"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=0dABjcBPpyek7KsjPxN92hSMprS3sX9rPZCzqDi%2FrYpCUHfJ0FfvZyzwuaVQ8o5hu7FCdLq2QjQEkMwXslZq7pu1jw7L90TJsAIYtJlRhYw1LNqP6dokxIDbGFHHZsuUjOCsxaOARw%3D%3D"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Transfer-Encoding:
       - chunked
+      alt-svc:
+      - h3=":443"; ma=86400
       cache-control:
       - no-cache, no-store, private
       pragma:
       - no-cache
       set-cookie:
       - ADRUM_BT1=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
@@ -194,26 +186,20 @@
       Accept-Encoding:
       - gzip, deflate
       Authorization:
       - Bearer SANITIZED
       Connection:
       - keep-alive
       Cookie:
-      - JWT_FGP=SANITIZED; _cfuvid=SANITIZED; GARMIN-SSO=SANITIZED; GARMIN-SSO-CUST-GUID=SANITIZED;
-        GARMIN-SSO-GUID=SANITIZED; GarminNoCache=SANITIZED; ADRUM_BT1=SANITIZED; ADRUM_BTa=SANITIZED;
-        SESSIONID=SANITIZED; SameSite=SANITIZED; __cflb=SANITIZED
+      - _cfuvid=SANITIZED; ADRUM_BT1=SANITIZED; ADRUM_BTa=SANITIZED; SameSite=SANITIZED
       User-Agent:
       - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X) AppleWebKit/605.1.15
         (KHTML, like Gecko) Mobile/15E148
-      di-backend:
-      - connectapi.garmin.com
-      referer:
-      - https://connect.garmin.com/modern
     method: GET
-    uri: https://connect.garmin.com/usersummary-service/stats/stress/weekly/2021-07-22/52
+    uri: https://connectapi.garmin.com/usersummary-service/stats/stress/weekly/2021-07-22/52
   response:
     body:
       string: '[{"calendarDate": "2020-11-13", "value": 25}, {"calendarDate": "2020-11-20",
         "value": 25}, {"calendarDate": "2020-11-27", "value": 21}, {"calendarDate":
         "2020-12-04", "value": 26}, {"calendarDate": "2020-12-11", "value": 28}, {"calendarDate":
         "2020-12-18", "value": 21}, {"calendarDate": "2020-12-25", "value": 26}, {"calendarDate":
         "2021-01-01", "value": 21}, {"calendarDate": "2021-01-08", "value": 23}, {"calendarDate":
@@ -231,31 +217,33 @@
         "2021-06-18", "value": 20}, {"calendarDate": "2021-06-25", "value": 22}, {"calendarDate":
         "2021-07-02", "value": 24}, {"calendarDate": "2021-07-09", "value": 28}, {"calendarDate":
         "2021-07-16", "value": 22}]'
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7ed3150d5d5a154d-QRO
+      - 7f12d048dfef4773-DFW
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json
       Date:
-      - Thu, 27 Jul 2023 07:13:52 GMT
+      - Fri, 04 Aug 2023 00:51:44 GMT
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=fWZrjf3u80zEQH%2BnGGVgCyvjgiVJwhA1cQh2CFYE%2FQwVttnv4iWp72O5eO9sOWG5bY%2BNLRnscSpa5aELeyCqu%2FnkNkmE727QALlvo5TzfF66y%2Bx5bDuqUcH9cT2ZkmSCgUc4Ww%3D%3D"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=KB2vAYUsuOIPmTgbNh1mqCxbPxyRAWt4d62WshenVJhz7KjqcN6q387XCXzC2veJ6JaPoC%2B10JQahiQqo5PmFmxgUWSYGeagUmFKB6DX5aXs0AWb8Ru8YrIYDUCD4FWraGQp2bN3jQ%3D%3D"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Transfer-Encoding:
       - chunked
+      alt-svc:
+      - h3=":443"; ma=86400
       cache-control:
       - no-cache, no-store, private
       pragma:
       - no-cache
       set-cookie:
       - ADRUM_BT1=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
@@ -282,48 +270,44 @@
       Accept-Encoding:
       - gzip, deflate
       Authorization:
       - Bearer SANITIZED
       Connection:
       - keep-alive
       Cookie:
-      - JWT_FGP=SANITIZED; _cfuvid=SANITIZED; GARMIN-SSO=SANITIZED; GARMIN-SSO-CUST-GUID=SANITIZED;
-        GARMIN-SSO-GUID=SANITIZED; GarminNoCache=SANITIZED; ADRUM_BT1=SANITIZED; ADRUM_BTa=SANITIZED;
-        SESSIONID=SANITIZED; SameSite=SANITIZED; __cflb=SANITIZED
+      - _cfuvid=SANITIZED; ADRUM_BT1=SANITIZED; ADRUM_BTa=SANITIZED; SameSite=SANITIZED
       User-Agent:
       - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X) AppleWebKit/605.1.15
         (KHTML, like Gecko) Mobile/15E148
-      di-backend:
-      - connectapi.garmin.com
-      referer:
-      - https://connect.garmin.com/modern
     method: GET
-    uri: https://connect.garmin.com/usersummary-service/stats/stress/weekly/2020-07-23/52
+    uri: https://connectapi.garmin.com/usersummary-service/stats/stress/weekly/2020-07-23/52
   response:
     body:
       string: '[]'
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7ed3150f0e51b6e2-QRO
+      - 7f12d04b0d564770-DFW
       Connection:
       - keep-alive
       Content-Length:
       - '2'
       Content-Type:
       - application/json
       Date:
-      - Thu, 27 Jul 2023 07:13:52 GMT
+      - Fri, 04 Aug 2023 00:51:44 GMT
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=Hx9TnuLPiSZYwU7UBacvZo5o5KAbnaYDZlPvat3REcXAAfLp1vxWYbqKIENkqEoRJcBh0uoWTgzeStFAiovj0DZuOeGUGYVsUID1fDvaTBzsg2yWvRJP7Ka3LmuFaTmgvUakLA%3D%3D"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=kJ32Qw3rO%2FNBbdeJVElUsUXTYMQZNCtoUI4S2JDviH%2F3tXkOg1VmlYy%2BlGAEYt79Mss1E09YGwUZFucY%2F3%2FQpcTFcC%2F0dG3wWK8z9B6%2FkpaFPOnKcUvkGpdu%2FVl1lSXK%2BZxv%2FkneQw%3D%3D"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
+      alt-svc:
+      - h3=":443"; ma=86400
       cache-control:
       - no-cache, no-store, private
       pragma:
       - no-cache
       set-cookie:
       - ADRUM_BT1=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
```

### Comparing `garth-0.3.5/tests/resources/cassettes/test_weekly_stress_pagination.yaml` & `garth-0.4.0/tests/stats/cassettes/test_weekly_stress_pagination.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -6,26 +6,19 @@
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Authorization:
       - Bearer SANITIZED
       Connection:
       - keep-alive
-      Cookie:
-      - JWT_FGP=SANITIZED; _cfuvid=SANITIZED; GARMIN-SSO=SANITIZED; GARMIN-SSO-CUST-GUID=SANITIZED;
-        GARMIN-SSO-GUID=SANITIZED; GarminNoCache=SANITIZED; SESSIONID=SANITIZED; __cflb=SANITIZED
       User-Agent:
       - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X) AppleWebKit/605.1.15
         (KHTML, like Gecko) Mobile/15E148
-      di-backend:
-      - connectapi.garmin.com
-      referer:
-      - https://connect.garmin.com/modern
     method: GET
-    uri: https://connect.garmin.com/usersummary-service/stats/stress/weekly/2023-07-20/52
+    uri: https://connectapi.garmin.com/usersummary-service/stats/stress/weekly/2023-07-20/52
   response:
     body:
       string: '[{"calendarDate": "2022-07-22", "value": 25}, {"calendarDate": "2022-07-29",
         "value": 26}, {"calendarDate": "2022-08-05", "value": 27}, {"calendarDate":
         "2022-08-12", "value": 29}, {"calendarDate": "2022-08-19", "value": 28}, {"calendarDate":
         "2022-08-26", "value": 25}, {"calendarDate": "2022-09-02", "value": 27}, {"calendarDate":
         "2022-09-09", "value": 23}, {"calendarDate": "2022-09-16", "value": 30}, {"calendarDate":
@@ -51,31 +44,33 @@
         "2023-06-16", "value": 34}, {"calendarDate": "2023-06-23", "value": 32}, {"calendarDate":
         "2023-06-30", "value": 37}, {"calendarDate": "2023-07-07", "value": 30}, {"calendarDate":
         "2023-07-14", "value": 34}]'
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7eccdf751968155e-QRO
+      - 7f12d0420f64485e-DFW
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json
       Date:
-      - Wed, 26 Jul 2023 13:08:42 GMT
+      - Fri, 04 Aug 2023 00:51:43 GMT
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=5u0kzAqD%2FsVj%2Faw05RbOpHxeW5JTvnqfjcy%2BcYTdOU7EBl9BlQi7%2BrRykG339SCKCwR9WjZk72WObuU0ROFw2QlpeU9lYb%2FURYheL52jWUohfkAesz58bHTIHB0YYuOVWdfXHg%3D%3D"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=r7%2F9tPODwjk6XSInj%2F27RVln6GI1GZS1XPdSqgXUtOAYku0XeefqxhEQ4v2%2FG30cFR9hcMVlnk8G2MWb0GtyRlYFZRMZzpzHbOfdZGCiZDWTKsYcavDHB0iFF07x0XxSZy1NOnZPxQ%3D%3D"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Transfer-Encoding:
       - chunked
+      alt-svc:
+      - h3=":443"; ma=86400
       cache-control:
       - no-cache, no-store, private
       pragma:
       - no-cache
       set-cookie:
       - ADRUM_BTa=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
@@ -83,14 +78,15 @@
         Secure
       - SameSite=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
       - ADRUM_BT1=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
       - ADRUM_BT1=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
+      - _cfuvid=SANITIZED; path=SANITIZED; domain=SANITIZED; HttpOnly; Secure; SameSite=SANITIZED
     status:
       code: 200
       message: OK
 - request:
     body: null
     headers:
       Accept:
@@ -98,54 +94,50 @@
       Accept-Encoding:
       - gzip, deflate
       Authorization:
       - Bearer SANITIZED
       Connection:
       - keep-alive
       Cookie:
-      - JWT_FGP=SANITIZED; _cfuvid=SANITIZED; GARMIN-SSO=SANITIZED; GARMIN-SSO-CUST-GUID=SANITIZED;
-        GARMIN-SSO-GUID=SANITIZED; GarminNoCache=SANITIZED; ADRUM_BT1=SANITIZED; ADRUM_BTa=SANITIZED;
-        SESSIONID=SANITIZED; SameSite=SANITIZED; __cflb=SANITIZED
+      - _cfuvid=SANITIZED; ADRUM_BT1=SANITIZED; ADRUM_BTa=SANITIZED; SameSite=SANITIZED
       User-Agent:
       - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X) AppleWebKit/605.1.15
         (KHTML, like Gecko) Mobile/15E148
-      di-backend:
-      - connectapi.garmin.com
-      referer:
-      - https://connect.garmin.com/modern
     method: GET
-    uri: https://connect.garmin.com/usersummary-service/stats/stress/weekly/2022-07-21/8
+    uri: https://connectapi.garmin.com/usersummary-service/stats/stress/weekly/2022-07-21/8
   response:
     body:
       string: '[{"calendarDate": "2022-05-27", "value": 26}, {"calendarDate": "2022-06-03",
         "value": 29}, {"calendarDate": "2022-06-10", "value": 24}, {"calendarDate":
         "2022-06-17", "value": 27}, {"calendarDate": "2022-06-24", "value": 30}, {"calendarDate":
         "2022-07-01", "value": 29}, {"calendarDate": "2022-07-08", "value": 31}, {"calendarDate":
         "2022-07-15", "value": 29}]'
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7eccdf761f01b6eb-QRO
+      - 7f12d04408c24773-DFW
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json
       Date:
-      - Wed, 26 Jul 2023 13:08:42 GMT
+      - Fri, 04 Aug 2023 00:51:43 GMT
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=b8cgHwmZpRFRz2klNRGTy0qKFuE%2FiF3ozL4lzQ0BvLFCfdkOsAcp90DGvi62773jt1w08x%2FxSZJJ%2BdimmffbaP80gxQ3O9pvwaSii6SAdAt0JUS2XdJqaGkPIZ4mHdfKBnIcww%3D%3D"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=KWq8%2Fp%2Bv4Pju9Cm8%2B1sQhAf4zxg%2FWFLsTGqeifi%2FjsbxHnQiNQ9pMu48Hi7MyeVTYTclB%2FmS0nDslvydNk0TYRKNUY53M37xkPBa5K6XynkHSBcj7tYNozBZBqYRMWeJTf4NJuvobA%3D%3D"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Transfer-Encoding:
       - chunked
+      alt-svc:
+      - h3=":443"; ma=86400
       cache-control:
       - no-cache, no-store, private
       pragma:
       - no-cache
       set-cookie:
       - ADRUM_BT1=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED;
         Secure
```

### Comparing `garth-0.3.5/tests/resources/test_intensity_minutes.py` & `garth-0.4.0/tests/stats/test_intensity_minutes.py`

 * *Files identical despite different names*

### Comparing `garth-0.3.5/tests/resources/test_sleep.py` & `garth-0.4.0/tests/stats/test_sleep.py`

 * *Files identical despite different names*

### Comparing `garth-0.3.5/tests/resources/test_steps.py` & `garth-0.4.0/tests/stats/test_steps.py`

 * *Files identical despite different names*

### Comparing `garth-0.3.5/tests/resources/test_stress.py` & `garth-0.4.0/tests/stats/test_stress.py`

 * *Files identical despite different names*

### Comparing `garth-0.3.5/tests/test_http.py` & `garth-0.4.0/tests/test_http.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,18 @@
-import tempfile
-import time
-
 import pytest
 from requests import HTTPError
-from requests.cookies import RequestsCookieJar
 
-from garth.auth_token import AuthToken
+from garth.auth_tokens import OAuth2Token
 from garth.http import Client
 
 
-def test_configure_auth_token(client: Client, auth_token: AuthToken):
-    assert client.auth_token is None
-    client.configure(auth_token=auth_token)
-    assert client.auth_token == auth_token
-
-
-def test_configure_cookies(client: Client):
-    cookies = RequestsCookieJar()
-    assert client.sess.cookies == {}
-    client.configure(cookies=cookies)
-    assert client.sess.cookies == cookies
+def test_configure_oauth2_token(client: Client, oauth2_token: OAuth2Token):
+    assert client.oauth2_token is None
+    client.configure(oauth2_token=oauth2_token)
+    assert client.oauth2_token == oauth2_token
 
 
 def test_configure_domain(client: Client):
     assert client.domain == "garmin.com"
     client.configure(domain="garmin.cn")
     assert client.domain == "garmin.cn"
 
@@ -81,38 +70,36 @@
 
 @pytest.mark.vcr
 def test_client_request(client: Client):
     resp = client.request("GET", "connect", "/")
     assert resp.ok
 
     with pytest.raises(HTTPError):
-        client.request("GET", "connect", "/", api=True)
+        client.request("GET", "connectapi", "/")
 
 
 @pytest.mark.vcr
 def test_login_success(monkeypatch, client: Client):
     def mock_input(_):
         return "327751"
 
     monkeypatch.setattr("builtins.input", mock_input)
 
-    assert client.auth_token is None
+    assert client.oauth1_token is None
+    assert client.oauth2_token is None
     client.login("user@example.com", "correct_password")
-    assert client.auth_token is not None
+    assert client.oauth1_token
+    assert client.oauth2_token
 
 
-def test_save_and_resume_session(authed_client: Client):
-    with tempfile.TemporaryDirectory() as tempdir:
-        authed_client.dump(tempdir)
-
-        new_client = Client()
-        new_client.load(tempdir)
-
-        assert new_client.sess.cookies == authed_client.sess.cookies
-        assert new_client.auth_token == authed_client.auth_token
+@pytest.mark.vcr
+def test_username(authed_client: Client):
+    assert authed_client._username is None
+    assert authed_client.username
+    assert authed_client._username == authed_client.username
 
 
 @pytest.mark.vcr
 def test_connectapi(authed_client: Client):
     stress = authed_client.connectapi(
         "/usersummary-service/stats/stress/daily/2023-07-21/2023-07-21"
     )
@@ -121,19 +108,7 @@
     assert list(stress[0]["values"].keys()) == [
         "highStressDuration",
         "lowStressDuration",
         "overallStressLevel",
         "restStressDuration",
         "mediumStressDuration",
     ]
-
-
-@pytest.mark.vcr
-def test_connectapi_refresh(authed_client: Client):
-    assert authed_client.auth_token
-    authed_client.auth_token.expires_at = int(time.time() - 1)
-    assert authed_client.auth_token.expired
-    assert not authed_client.auth_token.refresh_expired
-    authed_client.connectapi(
-        "/usersummary-service/stats/stress/daily/2023-07-21/2023-07-21"
-    )
-    assert not authed_client.auth_token.expired
```

### Comparing `garth-0.3.5/tests/test_sso.py` & `garth-0.4.0/tests/test_sso.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import time
 
 import pytest
 from requests import HTTPError
 
 from garth import sso
-from garth.auth_token import AuthToken
+from garth.auth_tokens import OAuth1Token, OAuth2Token
 from garth.exc import GarthException
 from garth.http import Client
 
 
 @pytest.mark.vcr
 def test_login_email_password_fail(client: Client):
     with pytest.raises(HTTPError):
@@ -17,50 +17,45 @@
 
 @pytest.mark.vcr
 def test_login_success(monkeypatch, client: Client):
     def mock_input(_):
         return "327751"
 
     monkeypatch.setattr("builtins.input", mock_input)
-    sso.login("user@example.com", "correct_password", client=client)
+    oauth1, oauth2 = sso.login(
+        "user@example.com", "correct_password", client=client
+    )
+    assert oauth1
+    assert isinstance(oauth1, OAuth1Token)
+    assert oauth2
+    assert isinstance(oauth2, OAuth2Token)
 
 
-def test_set_expirations(auth_token_dict: dict):
-    token = sso.set_expirations(auth_token_dict)
+def test_set_expirations(oauth2_token_dict: dict):
+    token = sso.set_expirations(oauth2_token_dict)
     assert (
-        token["expires_at"] - time.time() - auth_token_dict["expires_in"] < 1
+        token["expires_at"] - time.time() - oauth2_token_dict["expires_in"] < 1
     )
     assert (
         token["refresh_token_expires_at"]
         - time.time()
-        - auth_token_dict["refresh_token_expires_in"]
+        - oauth2_token_dict["refresh_token_expires_in"]
         < 1
     )
 
 
 @pytest.mark.vcr
 def test_exchange(authed_client: Client):
-    token = sso.exchange(authed_client)
-    auth_token = AuthToken(**token)
-    assert not auth_token.expired
-    assert not auth_token.refresh_expired
-    assert auth_token.token_type.title() == "Bearer"
-    assert authed_client.auth_token != auth_token
-
-
-@pytest.mark.vcr
-def test_refresh(authed_client: Client):
-    assert authed_client.auth_token is not None
-    refresh_token = authed_client.auth_token.refresh_token
-    token = sso.refresh(refresh_token, authed_client)
-    auth_token = AuthToken(**token)
-    assert not auth_token.expired
-    assert not auth_token.refresh_expired
-    assert auth_token.token_type.title() == "Bearer"
-    assert authed_client.auth_token != auth_token
+    assert authed_client.oauth1_token
+    oauth1_token = authed_client.oauth1_token
+    oauth2_token = sso.exchange(oauth1_token, client=authed_client)
+    assert not oauth2_token.expired
+    assert not oauth2_token.refresh_expired
+    assert oauth2_token.token_type.title() == "Bearer"
+    assert authed_client.oauth2_token != oauth2_token
 
 
 def test_get_csrf_token():
     html = """
     <html>
     <head>
     </head>
```

### Comparing `garth-0.3.5/PKG-INFO` & `garth-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: garth
-Version: 0.3.5
+Version: 0.4.0
 Summary: Garmin SSO auth + Connect client
 Author-Email: Matin Tamizi <mtamizi@duck.com>
 License: MIT
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.10
 Requires-Dist: requests
 Requires-Dist: pydantic
+Requires-Dist: requests-oauthlib>=1.3.1
 Description-Content-Type: text/markdown
 
 # Garth
 
 [![CI](https://github.com/matin/garth/workflows/CI/badge.svg?event=push)](https://github.com/matin/garth/actions?query=event%3Apush+branch%3Amain+workflow%3ACI)
 [![codecov](https://codecov.io/gh/matin/garth/branch/main/graph/badge.svg?token=0EFFYJNFIL)](https://codecov.io/gh/matin/garth)
 
@@ -173,15 +174,15 @@
         "overallStressLevel": 33,
         "restStressDuration": 30960,
         "mediumStressDuration": 8760
     }
 }
 ```
 
-## Resources
+## Stats resources
 
 ### Stress
 
 Daily stress levels
 
 ```python
 DailyStress.list("2023-07-23", 2)
```

