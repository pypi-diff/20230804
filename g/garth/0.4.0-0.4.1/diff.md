# Comparing `tmp/garth-0.4.0.tar.gz` & `tmp/garth-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garth-0.4.0.tar", last modified: Fri Aug  4 04:47:08 2023, max compression
+gzip compressed data, was "garth-0.4.1.tar", last modified: Fri Aug  4 20:53:46 2023, max compression
```

## Comparing `garth-0.4.0.tar` & `garth-0.4.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     1071 2023-07-20 12:44:00.130760 garth-0.4.0/LICENSE
--rw-r--r--   0        0        0    13332 2023-08-01 00:53:50.423067 garth-0.4.0/README.md
--rw-r--r--   0        0        0      679 2023-08-01 00:53:18.694307 garth-0.4.0/garth/__init__.py
--rw-r--r--   0        0        0      734 2023-08-04 01:10:15.046660 garth-0.4.0/garth/auth_tokens.py
--rw-r--r--   0        0        0      145 2023-07-18 22:32:58.010661 garth-0.4.0/garth/exc.py
--rw-r--r--   0        0        0     4922 2023-08-04 04:12:36.576282 garth-0.4.0/garth/http.py
--rw-r--r--   0        0        0        0 2023-07-27 13:16:10.642595 garth-0.4.0/garth/py.typed
--rw-r--r--   0        0        0     4656 2023-08-04 04:07:53.677094 garth-0.4.0/garth/sso.py
--rw-r--r--   0        0        0      434 2023-07-30 01:10:27.575730 garth-0.4.0/garth/stats/__init__.py
--rw-r--r--   0        0        0     1531 2023-08-01 00:53:16.612824 garth-0.4.0/garth/stats/_base.py
--rw-r--r--   0        0        0     1726 2023-07-30 04:26:19.317148 garth-0.4.0/garth/stats/hrv.py
--rw-r--r--   0        0        0      611 2023-08-01 00:53:21.402342 garth-0.4.0/garth/stats/intensity_minutes.py
--rw-r--r--   0        0        0     3523 2023-08-01 01:10:51.104099 garth-0.4.0/garth/stats/sleep.py
--rw-r--r--   0        0        0      653 2023-08-01 00:53:20.538257 garth-0.4.0/garth/stats/steps.py
--rw-r--r--   0        0        0      652 2023-08-01 00:53:19.922467 garth-0.4.0/garth/stats/stress.py
--rw-r--r--   0        0        0     1767 2023-08-04 01:10:15.047656 garth-0.4.0/garth/utils.py
--rw-r--r--   0        0        0       22 2023-08-04 04:47:02.589550 garth-0.4.0/garth/version.py
--rw-r--r--   0        0        0     1221 2023-08-04 04:47:08.260255 garth-0.4.0/pyproject.toml
--rw-r--r--   0        0        0   100792 2023-08-04 01:10:15.050440 garth-0.4.0/tests/cassettes/test_client_request.yaml
--rw-r--r--   0        0        0     2602 2023-08-04 01:10:15.050693 garth-0.4.0/tests/cassettes/test_connectapi.yaml
--rw-r--r--   0        0        0     3102 2023-08-04 03:43:23.879883 garth-0.4.0/tests/cassettes/test_exchange.yaml
--rw-r--r--   0        0        0    50571 2023-08-04 01:10:15.051257 garth-0.4.0/tests/cassettes/test_login_email_password_fail.yaml
--rw-r--r--   0        0        0    71668 2023-08-04 01:10:15.052079 garth-0.4.0/tests/cassettes/test_login_success.yaml
--rw-r--r--   0        0        0     4883 2023-08-04 01:10:15.052284 garth-0.4.0/tests/cassettes/test_username.yaml
--rw-r--r--   0        0        0     3692 2023-08-04 01:10:15.052523 garth-0.4.0/tests/conftest.py
--rw-r--r--   0        0        0     8412 2023-08-04 01:10:15.052774 garth-0.4.0/tests/stats/cassettes/test_daily_hrv.yaml
--rw-r--r--   0        0        0     1893 2023-08-04 01:10:15.052978 garth-0.4.0/tests/stats/cassettes/test_daily_hrv_no_results.yaml
--rw-r--r--   0        0        0    16982 2023-08-04 01:10:15.053232 garth-0.4.0/tests/stats/cassettes/test_daily_hrv_paginate.yaml
--rw-r--r--   0        0        0     1897 2023-08-04 01:10:15.053481 garth-0.4.0/tests/stats/cassettes/test_daily_hrv_paginate_no_results.yaml
--rw-r--r--   0        0        0     3926 2023-08-04 01:10:15.053705 garth-0.4.0/tests/stats/cassettes/test_daily_intensity_minutes.yaml
--rw-r--r--   0        0        0     2759 2023-08-04 01:10:15.053918 garth-0.4.0/tests/stats/cassettes/test_daily_sleep.yaml
--rw-r--r--   0        0        0     4067 2023-08-04 01:10:15.054145 garth-0.4.0/tests/stats/cassettes/test_daily_steps.yaml
--rw-r--r--   0        0        0     6085 2023-08-04 01:10:15.054397 garth-0.4.0/tests/stats/cassettes/test_daily_stress.yaml
--rw-r--r--   0        0        0    18594 2023-08-04 01:10:15.054680 garth-0.4.0/tests/stats/cassettes/test_daily_stress_pagination.yaml
--rw-r--r--   0        0        0     8588 2023-08-04 01:10:15.054936 garth-0.4.0/tests/stats/cassettes/test_sleep_data_get.yaml
--rw-r--r--   0        0        0    78725 2023-08-04 01:10:15.055303 garth-0.4.0/tests/stats/cassettes/test_sleep_data_list.yaml
--rw-r--r--   0        0        0     3259 2023-08-04 01:10:15.055564 garth-0.4.0/tests/stats/cassettes/test_weekly_intensity_minutes.yaml
--rw-r--r--   0        0        0    12946 2023-08-04 01:10:15.055800 garth-0.4.0/tests/stats/cassettes/test_weekly_steps.yaml
--rw-r--r--   0        0        0     4552 2023-08-04 01:10:15.056039 garth-0.4.0/tests/stats/cassettes/test_weekly_stress.yaml
--rw-r--r--   0        0        0    15357 2023-08-04 01:10:15.056262 garth-0.4.0/tests/stats/cassettes/test_weekly_stress_beyond_data.yaml
--rw-r--r--   0        0        0     7120 2023-08-04 01:10:15.056491 garth-0.4.0/tests/stats/cassettes/test_weekly_stress_pagination.yaml
--rw-r--r--   0        0        0     1001 2023-07-30 04:28:17.698327 garth-0.4.0/tests/stats/test_hrv.py
--rw-r--r--   0        0        0      748 2023-07-29 23:40:27.912636 garth-0.4.0/tests/stats/test_intensity_minutes.py
--rw-r--r--   0        0        0      849 2023-07-28 12:22:22.098284 garth-0.4.0/tests/stats/test_sleep.py
--rw-r--r--   0        0        0      667 2023-07-29 17:53:35.423973 garth-0.4.0/tests/stats/test_steps.py
--rw-r--r--   0        0        0     1437 2023-07-27 13:31:20.424008 garth-0.4.0/tests/stats/test_stress.py
--rw-r--r--   0        0        0      455 2023-08-04 01:10:15.056632 garth-0.4.0/tests/test_auth_tokens.py
--rw-r--r--   0        0        0     3331 2023-08-04 04:13:58.627319 garth-0.4.0/tests/test_http.py
--rw-r--r--   0        0        0     2397 2023-08-04 04:07:40.517972 garth-0.4.0/tests/test_sso.py
--rw-r--r--   0        0        0     1655 2023-08-04 04:10:40.202147 garth-0.4.0/tests/test_utils.py
--rw-r--r--   0        0        0    13784 1970-01-01 00:00:00.000000 garth-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-20 12:44:00.130760 garth-0.4.1/LICENSE
+-rw-r--r--   0        0        0    13332 2023-08-01 00:53:50.423067 garth-0.4.1/README.md
+-rw-r--r--   0        0        0      679 2023-08-01 00:53:18.694307 garth-0.4.1/garth/__init__.py
+-rw-r--r--   0        0        0      796 2023-08-04 15:13:28.651836 garth-0.4.1/garth/auth_tokens.py
+-rw-r--r--   0        0        0      145 2023-07-18 22:32:58.010661 garth-0.4.1/garth/exc.py
+-rw-r--r--   0        0        0     4922 2023-08-04 05:03:14.761571 garth-0.4.1/garth/http.py
+-rw-r--r--   0        0        0        0 2023-07-27 13:16:10.642595 garth-0.4.1/garth/py.typed
+-rw-r--r--   0        0        0     4565 2023-08-04 20:40:51.804547 garth-0.4.1/garth/sso.py
+-rw-r--r--   0        0        0      434 2023-07-30 01:10:27.575730 garth-0.4.1/garth/stats/__init__.py
+-rw-r--r--   0        0        0     1531 2023-08-01 00:53:16.612824 garth-0.4.1/garth/stats/_base.py
+-rw-r--r--   0        0        0     1726 2023-07-30 04:26:19.317148 garth-0.4.1/garth/stats/hrv.py
+-rw-r--r--   0        0        0      611 2023-08-01 00:53:21.402342 garth-0.4.1/garth/stats/intensity_minutes.py
+-rw-r--r--   0        0        0     3523 2023-08-01 01:10:51.104099 garth-0.4.1/garth/stats/sleep.py
+-rw-r--r--   0        0        0      653 2023-08-01 00:53:20.538257 garth-0.4.1/garth/stats/steps.py
+-rw-r--r--   0        0        0      652 2023-08-01 00:53:19.922467 garth-0.4.1/garth/stats/stress.py
+-rw-r--r--   0        0        0     1767 2023-08-04 01:10:15.047656 garth-0.4.1/garth/utils.py
+-rw-r--r--   0        0        0       22 2023-08-04 20:53:30.325813 garth-0.4.1/garth/version.py
+-rw-r--r--   0        0        0     1221 2023-08-04 20:53:46.447734 garth-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0   100792 2023-08-04 01:10:15.050440 garth-0.4.1/tests/cassettes/test_client_request.yaml
+-rw-r--r--   0        0        0     2602 2023-08-04 01:10:15.050693 garth-0.4.1/tests/cassettes/test_connectapi.yaml
+-rw-r--r--   0        0        0     3102 2023-08-04 03:43:23.879883 garth-0.4.1/tests/cassettes/test_exchange.yaml
+-rw-r--r--   0        0        0    50571 2023-08-04 01:10:15.051257 garth-0.4.1/tests/cassettes/test_login_email_password_fail.yaml
+-rw-r--r--   0        0        0    71237 2023-08-04 20:44:41.137445 garth-0.4.1/tests/cassettes/test_login_success_mfa.yaml
+-rw-r--r--   0        0        0     4883 2023-08-04 01:10:15.052284 garth-0.4.1/tests/cassettes/test_username.yaml
+-rw-r--r--   0        0        0     3605 2023-08-04 15:10:55.580644 garth-0.4.1/tests/conftest.py
+-rw-r--r--   0        0        0     8412 2023-08-04 01:10:15.052774 garth-0.4.1/tests/stats/cassettes/test_daily_hrv.yaml
+-rw-r--r--   0        0        0     1893 2023-08-04 01:10:15.052978 garth-0.4.1/tests/stats/cassettes/test_daily_hrv_no_results.yaml
+-rw-r--r--   0        0        0    16982 2023-08-04 01:10:15.053232 garth-0.4.1/tests/stats/cassettes/test_daily_hrv_paginate.yaml
+-rw-r--r--   0        0        0     1897 2023-08-04 01:10:15.053481 garth-0.4.1/tests/stats/cassettes/test_daily_hrv_paginate_no_results.yaml
+-rw-r--r--   0        0        0     3926 2023-08-04 01:10:15.053705 garth-0.4.1/tests/stats/cassettes/test_daily_intensity_minutes.yaml
+-rw-r--r--   0        0        0     2759 2023-08-04 01:10:15.053918 garth-0.4.1/tests/stats/cassettes/test_daily_sleep.yaml
+-rw-r--r--   0        0        0     4067 2023-08-04 01:10:15.054145 garth-0.4.1/tests/stats/cassettes/test_daily_steps.yaml
+-rw-r--r--   0        0        0     6085 2023-08-04 01:10:15.054397 garth-0.4.1/tests/stats/cassettes/test_daily_stress.yaml
+-rw-r--r--   0        0        0    18594 2023-08-04 01:10:15.054680 garth-0.4.1/tests/stats/cassettes/test_daily_stress_pagination.yaml
+-rw-r--r--   0        0        0     8588 2023-08-04 01:10:15.054936 garth-0.4.1/tests/stats/cassettes/test_sleep_data_get.yaml
+-rw-r--r--   0        0        0    78725 2023-08-04 01:10:15.055303 garth-0.4.1/tests/stats/cassettes/test_sleep_data_list.yaml
+-rw-r--r--   0        0        0     3259 2023-08-04 01:10:15.055564 garth-0.4.1/tests/stats/cassettes/test_weekly_intensity_minutes.yaml
+-rw-r--r--   0        0        0    12946 2023-08-04 01:10:15.055800 garth-0.4.1/tests/stats/cassettes/test_weekly_steps.yaml
+-rw-r--r--   0        0        0     4552 2023-08-04 01:10:15.056039 garth-0.4.1/tests/stats/cassettes/test_weekly_stress.yaml
+-rw-r--r--   0        0        0    15357 2023-08-04 01:10:15.056262 garth-0.4.1/tests/stats/cassettes/test_weekly_stress_beyond_data.yaml
+-rw-r--r--   0        0        0     7120 2023-08-04 01:10:15.056491 garth-0.4.1/tests/stats/cassettes/test_weekly_stress_pagination.yaml
+-rw-r--r--   0        0        0     1001 2023-07-30 04:28:17.698327 garth-0.4.1/tests/stats/test_hrv.py
+-rw-r--r--   0        0        0      748 2023-07-29 23:40:27.912636 garth-0.4.1/tests/stats/test_intensity_minutes.py
+-rw-r--r--   0        0        0      849 2023-07-28 12:22:22.098284 garth-0.4.1/tests/stats/test_sleep.py
+-rw-r--r--   0        0        0      667 2023-07-29 17:53:35.423973 garth-0.4.1/tests/stats/test_steps.py
+-rw-r--r--   0        0        0     1437 2023-07-27 13:31:20.424008 garth-0.4.1/tests/stats/test_stress.py
+-rw-r--r--   0        0        0      455 2023-08-04 01:10:15.056632 garth-0.4.1/tests/test_auth_tokens.py
+-rw-r--r--   0        0        0     3335 2023-08-04 20:42:44.643135 garth-0.4.1/tests/test_http.py
+-rw-r--r--   0        0        0     2402 2023-08-04 20:44:58.232522 garth-0.4.1/tests/test_sso.py
+-rw-r--r--   0        0        0     1655 2023-08-04 04:10:40.202147 garth-0.4.1/tests/test_utils.py
+-rw-r--r--   0        0        0    13784 1970-01-01 00:00:00.000000 garth-0.4.1/PKG-INFO
```

### Comparing `garth-0.4.0/LICENSE` & `garth-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `garth-0.4.0/README.md` & `garth-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `garth-0.4.0/garth/__init__.py` & `garth-0.4.1/garth/__init__.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.0/garth/auth_tokens.py` & `garth-0.4.1/garth/auth_tokens.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import time
 from datetime import datetime
+from typing import Optional
 
 from pydantic.dataclasses import dataclass
 
 
 @dataclass
 class OAuth1Token:
     oauth_token: str
     oauth_token_secret: str
-    mfa_token: str
-    mfa_expiration_timestamp: datetime
+    mfa_token: Optional[str] = None
+    mfa_expiration_timestamp: Optional[datetime] = None
 
 
 @dataclass
 class OAuth2Token:
     scope: str
     jti: str
     token_type: str
```

### Comparing `garth-0.4.0/garth/http.py` & `garth-0.4.1/garth/http.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.0/garth/sso.py` & `garth-0.4.1/garth/sso.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,38 +86,35 @@
     assert title == "Success"
 
     # Parse ticket
     m = re.search(r'embed\?ticket=([^"]+)"', client.last_resp.text)
     assert m
     ticket = m.group(1)
 
-    oauth1 = get_oauth1_token(ticket, client=client)
-    oauth2 = exchange(oauth1, client=client)
+    oauth1 = get_oauth1_token(ticket, client)
+    oauth2 = exchange(oauth1, client)
 
     return oauth1, oauth2
 
 
-def get_oauth1_token(ticket: str, /, client: "http.Client") -> OAuth1Token:
+def get_oauth1_token(ticket: str, client: "http.Client") -> OAuth1Token:
     sess = GarminOAuth1Session()
     resp = sess.get(
         f"https://connectapi.{client.domain}/oauth-service/oauth/"
         f"preauthorized?ticket={ticket}&login-url="
         f"https://sso.{client.domain}/sso/embed&accepts-mfa-tokens=true",
         headers=USER_AGENT,
     )
     resp.raise_for_status()
     parsed = parse_qs(resp.text)
     token = {k: v[0] for k, v in parsed.items()}
     return OAuth1Token(**token)  # type: ignore
 
 
-def exchange(
-    oauth1: OAuth1Token, /, client: Optional["http.Client"] = None
-) -> OAuth2Token:
-    client = client or http.client
+def exchange(oauth1: OAuth1Token, client: "http.Client") -> OAuth2Token:
     sess = GarminOAuth1Session(
         resource_owner_key=oauth1.oauth_token,
         resource_owner_secret=oauth1.oauth_token_secret,
     )
     token = sess.post(
         "https://connectapi.garmin.com/oauth-service/oauth/exchange/user/2.0",
         headers=USER_AGENT
@@ -129,15 +126,15 @@
 
 def handle_mfa(client: "http.Client", signin_params: dict) -> None:
     csrf_token = get_csrf_token(client.last_resp.text)
     mfa_code = input("Enter MFA code: ")
     client.post(
         "sso",
         "/sso/verifyMFA/loginEnterMfaCode",
-        params=signin_params | dict(rememberMyBrowserChecked="true"),
+        params=signin_params | dict(embedWidget="true"),
         referrer=True,
         data={
             "mfa-code": mfa_code,
             "embed": "true",
             "_csrf": csrf_token,
             "fromPage": "setupEnterMfaCode",
         },
```

### Comparing `garth-0.4.0/garth/stats/_base.py` & `garth-0.4.1/garth/stats/_base.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.0/garth/stats/hrv.py` & `garth-0.4.1/garth/stats/hrv.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.0/garth/stats/intensity_minutes.py` & `garth-0.4.1/garth/stats/intensity_minutes.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.0/garth/stats/sleep.py` & `garth-0.4.1/garth/stats/sleep.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.0/garth/stats/steps.py` & `garth-0.4.1/garth/stats/steps.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.0/garth/stats/stress.py` & `garth-0.4.1/garth/stats/stress.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.0/garth/utils.py` & `garth-0.4.1/garth/utils.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.0/pyproject.toml` & `garth-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     "Operating System :: MacOS :: MacOS X",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: POSIX :: Linux",
 ]
 packages = [
     { include = "garth" },
 ]
-version = "0.4.0"
+version = "0.4.1"
 
 [project.license]
 text = "MIT"
 
 [build-system]
 requires = [
     "pdm-backend",
```

### Comparing `garth-0.4.0/tests/cassettes/test_client_request.yaml` & `garth-0.4.1/tests/cassettes/test_client_request.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.0/tests/cassettes/test_connectapi.yaml` & `garth-0.4.1/tests/cassettes/test_connectapi.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.0/tests/cassettes/test_exchange.yaml` & `garth-0.4.1/tests/cassettes/test_exchange.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.0/tests/cassettes/test_login_email_password_fail.yaml` & `garth-0.4.1/tests/cassettes/test_login_email_password_fail.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.0/tests/cassettes/test_login_success.yaml` & `garth-0.4.1/tests/cassettes/test_login_success_mfa.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,14 @@
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
       - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X) AppleWebKit/605.1.15
         (KHTML, like Gecko) Mobile/15E148
-      referer:
-      - https://sso.garmin.com/sso/signin?id=gauth-widget&service=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&source=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountLoginUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountCreationUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&gauthHost=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed
     method: GET
     uri: https://sso.garmin.com/sso/embed?id=gauth-widget&embedWidget=true&gauthHost=https%3A%2F%2Fsso.garmin.com%2Fsso
   response:
     body:
       string: "<html>\n\t<head>\n\t    <title>GAuth Embedded Version</title>\n\t    <meta
         http-equiv=\"X-UA-Compatible\" content=\"IE=edge;\" />\n\t    <style type=\"text/css\">\n\t
         \   \t#gauth-widget {border: none !important;}\n\t    </style>\n\t</head>\n\t<body>\n\t\t<script
@@ -133,15 +131,15 @@
         a multi factor authentication check. (Only valid for an already logged in
         user.)\n\trememberMyBrowserShown          No  true/false (Default value is
         false)                      Whether the \"Remember My Browser\" check box
         is shown in the GAuth login widget MFA verification screen.\n\trememberMyBrowserChecked
         \       No  true/false (Default value is false)                      Whether
         the \"Remember My Browser\" check box feature is checked by default.\n\tconsentTypeIds\t\t\t\t\tNo\tconsent_types
         ids\t\t \t\t\t\t\t\t\t\t multiple consent types ids can be passed as consentTypeIds=type1&consentTypeIds=type2\n\t</pre>\n</div>\n\n\n\t<script>(function(){var
-        js = \"window['__CF$cv$params']={r:'7f0efe9dbf82154b'};_cpo=document.createElement('script');_cpo.nonce='',_cpo.src='/cdn-cgi/challenge-platform/scripts/invisible.js',document.getElementsByTagName('head')[0].appendChild(_cpo);\";var
+        js = \"window['__CF$cv$params']={r:'7f19a351192546a1'};_cpo=document.createElement('script');_cpo.nonce='',_cpo.src='/cdn-cgi/challenge-platform/scripts/invisible.js',document.getElementsByTagName('head')[0].appendChild(_cpo);\";var
         _0xh = document.createElement('iframe');_0xh.height = 1;_0xh.width = 1;_0xh.style.position
         = 'absolute';_0xh.style.top = 0;_0xh.style.left = 0;_0xh.style.border = 'none';_0xh.style.visibility
         = 'hidden';document.body.appendChild(_0xh);function handler() {var _0xi =
         _0xh.contentDocument || _0xh.contentWindow.document;if (_0xi) {var _0xj =
         _0xi.createElement('script');_0xj.innerHTML = js;_0xi.getElementsByTagName('head')[0].appendChild(_0xj);}}if
         (document.readyState !== 'loading') {handler();} else if (window.addEventListener)
         {document.addEventListener('DOMContentLoaded', handler);} else {var prev =
@@ -157,49 +155,49 @@
       Access-Control-Allow-Methods:
       - GET,POST,OPTIONS
       Access-Control-Allow-Origin:
       - https://www.garmin.com
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7f0efe9dbf82154b-QRO
+      - 7f19a351192546a1-DFW
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Language:
       - en
       Content-Type:
       - text/html;charset=UTF-8
       Date:
-      - Thu, 03 Aug 2023 13:44:18 GMT
+      - Fri, 04 Aug 2023 20:44:22 GMT
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=EpNuus5s1jsWqmwuAEQuwmJKl4R4x7yKry6fR6Y7YC6inOY0FhOQEkhOEsVh%2FjT2slREgwE8mXWp21snNnLiSMNaYAg%2FXMYN7%2BQXy%2FyZGKBPH63E5AJ7ggao6H0iXiXh"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=ytG3iKzcFS5%2B99VJD7%2FtqNm2w0E8GcBl0PO%2FS5qsCmdfQkBSJ6ekYSPKRo4ICSZ7qTGOe0aGYYvlGTJhYzx4Z5A46RMoBaAS2EdJ0JfNbriBi4n6TElpPegnmwjqc7Hj"}],"group":"cf-nel","max_age":604800}'
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
-      - casServer:cloud,prod,prod-US_1102:4
+      - casServer:cloud,prod,prod-US_1102:2
       X-B3-Traceid:
-      - 41fd0fc56c11edb61c8a219b7d5e8aab
+      - 7de36dd29fa2d733290a6725dc47dfb8
       X-Robots-Tag:
       - noindex
       X-Vcap-Request-Id:
-      - 63aed3d0-af94-4f44-791e-87b33f700916
+      - f780910f-ccdf-4771-49c7-aad225e3c68d
     status:
       code: 200
       message: OK
 - request:
     body: null
     headers:
       Accept:
@@ -309,15 +307,15 @@
         \                           <label for=\"password\">Password</label>\n                            <a
         id=\"loginforgotpassword\" class=\"login-forgot-password\" style=\"cursor:pointer\">(Forgot?)</a>\n
         \                           <input type=\"password\" name=\"password\" id=\"password\"
         spellcheck=\"false\" autocorrect=\"off\" autocapitalize=\"off\" />\n                             <strong
         id=\"capslock-warning\" class=\"information\" title=\"Caps lock is on.\" style=\"display:
         none;\">Caps lock is on.</strong>\n\t\t\t\t\t    </div>\n                        <input
         type=\"hidden\" name=\"embed\" value=\"false\"/>\n                        <input
-        type=\"hidden\" name=\"_csrf\" value=\"085E32B1AAC1E7C4FEE1CCA0CE94D87C4F295B638C604CD3637E11B1D90C2A9992FE5B6DF974136AB8FC45E97D508322F317\"
+        type=\"hidden\" name=\"_csrf\" value=\"884C8386EF425D4BA55B54C0B893A3B750BFD7FC791A34EC0BA934444EC04CE6B1FA7484E35E2DF94006783318F9980B7A3A\"
         />\n                        <button type=\"submit\" id=\"login-btn-signin\"
         class=\"btn1\" accesskey=\"l\">Sign In</button>\n                        \n\n\n
         \                       <!-- The existence of the \"rememberme\" parameter
         at all will remember the user! -->\n                        \n\n                    </form>\n
         \               </div>\n                <!-- end login form -->\n\n                <!--
         begin Create Account message -->\n\t            <div id=\"login-create-account\">\n\t
         \               \n\t            </div>\n\t            <!-- end Create Account
@@ -335,15 +333,15 @@
         Otherwise focus them in the username field of the login dialog.\n                    jQuery(\"#username\").focus();\n
         \               }\n\n                // Scroll to top of iframe to fix problem
         where Firefox 3.0-3.6 browsers initially show top of iframe cutoff.\n                location.href=\"#\";\n\n
         \               if(!embedWidget){\n                \tjQuery('.createAccountLink').click(function(){\n\t
         \                   send({'openLiteBox':'createAccountLink', 'popupUrl': createAccountConfigURL,
         'popupTitle':'Create An Account', 'clientId':clientId});\n\t                });\n
         \               }\n            });\n        </script>\n    <script>(function(){var
-        js = \"window['__CF$cv$params']={r:'7f0efe9ed8421547'};_cpo=document.createElement('script');_cpo.nonce='',_cpo.src='/cdn-cgi/challenge-platform/scripts/invisible.js',document.getElementsByTagName('head')[0].appendChild(_cpo);\";var
+        js = \"window['__CF$cv$params']={r:'7f19a3536a19468a'};_cpo=document.createElement('script');_cpo.nonce='',_cpo.src='/cdn-cgi/challenge-platform/scripts/invisible.js',document.getElementsByTagName('head')[0].appendChild(_cpo);\";var
         _0xh = document.createElement('iframe');_0xh.height = 1;_0xh.width = 1;_0xh.style.position
         = 'absolute';_0xh.style.top = 0;_0xh.style.left = 0;_0xh.style.border = 'none';_0xh.style.visibility
         = 'hidden';document.body.appendChild(_0xh);function handler() {var _0xi =
         _0xh.contentDocument || _0xh.contentWindow.document;if (_0xi) {var _0xj =
         _0xi.createElement('script');_0xj.innerHTML = js;_0xi.getElementsByTagName('head')[0].appendChild(_0xj);}}if
         (document.readyState !== 'loading') {handler();} else if (window.addEventListener)
         {document.addEventListener('DOMContentLoaded', handler);} else {var prev =
@@ -359,53 +357,53 @@
       Access-Control-Allow-Methods:
       - GET,POST,OPTIONS
       Access-Control-Allow-Origin:
       - https://www.garmin.com
       CF-Cache-Status:
       - DYNAMIC
       CF-Ray:
-      - 7f0efe9ed8421547-QRO
+      - 7f19a3536a19468a-DFW
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Language:
       - en
       Content-Type:
       - text/html;charset=UTF-8
       Date:
-      - Thu, 03 Aug 2023 13:44:19 GMT
+      - Fri, 04 Aug 2023 20:44:23 GMT
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=pUFwZ3E%2F0mJFNFwFoMN7HO5XgGTMP6zxm53htk%2Fdysfp324tli1JN8eL05f4Y1OzTbq%2FlPJr3Ky177Ui6fqBrdPOJs4Iuoi%2Fu6RfDU0p6ku8mha7OD5ihAwayz8H18hH"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=%2FFRtmPmaDfGDypVhatXfunnrGA%2BA8%2FxV6e%2BuekUdoE5fp2JNEw4bdoizvGG90r1BbOkbo3Ux5ybFDdoX4bKGqoKZWemHOBRFCYnaxHW3Ewoy9EHnNXohVMAu47T3dGnV"}],"group":"cf-nel","max_age":604800}'
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
-      - casServer:cloud,prod,prod-US_1102:5
+      - casServer:cloud,prod,prod-US_1102:7
       X-B3-Traceid:
-      - 0c7105857742ac230da0842492b92d1d
+      - 66c4d064ee4981291e470a27733c75c8
       X-Robots-Tag:
       - noindex
       X-Vcap-Request-Id:
-      - ba3d4826-a22e-49aa-7888-d62b15cc43b6
+      - 97a74fb2-172b-46bf-69fb-dc6d6ac7ca6b
     status:
       code: 200
       message: OK
 - request:
-    body: username=SANITIZED&password=SANITIZED&embed=true&_csrf=085E32B1AAC1E7C4FEE1CCA0CE94D87C4F295B638C604CD3637E11B1D90C2A9992FE5B6DF974136AB8FC45E97D508322F317
+    body: username=SANITIZED&password=SANITIZED&embed=true&_csrf=884C8386EF425D4BA55B54C0B893A3B750BFD7FC791A34EC0BA934444EC04CE6B1FA7484E35E2DF94006783318F9980B7A3A
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
@@ -435,45 +433,45 @@
       Access-Control-Allow-Methods:
       - GET,POST,OPTIONS
       Access-Control-Allow-Origin:
       - https://www.garmin.com
       CF-Cache-Status:
       - DYNAMIC
       CF-Ray:
-      - 7f0efea05a41155e-QRO
+      - 7f19a354dcda1547-QRO
       Connection:
       - keep-alive
       Content-Language:
       - en
       Content-Length:
       - '0'
       Date:
-      - Thu, 03 Aug 2023 13:44:20 GMT
+      - Fri, 04 Aug 2023 20:44:24 GMT
       Location:
       - https://sso.garmin.com/sso/verifyMFA/loginEnterMfaCode?id=gauth-widget&service=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&source=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountLoginUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountCreationUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&gauthHost=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=vZ9OuYl3ehAIn6QRonsHx3lnITP4uLKmQn0RBoyd46XkiNYBeslEOPJz9aPo%2BYnt4ICK9fi2l0m6VI7aXMQSlM5H5sWUeD9DVN1fZtehugkdvNWbk3995Vi4BP6OTPzK"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=tT3Bm66IlHoACTPEW5aaWCih7nnzM48aWyyucJvJmXCHD6IH9yzYzqrcuZRsM3bzCgO5iQl0GWdKr4pSX%2Bbww%2F1QQ2HgTgnaYSYzYE9M9%2BiXwO8Z9zPyD5ShoR5IaGGZ"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Set-Cookie:
       - org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED;
         Path=SANITIZED
       - __cfruid=SANITIZED; path=SANITIZED; domain=SANITIZED; HttpOnly; Secure; SameSite=SANITIZED
       Vary:
       - Accept-Encoding
       X-Application-Context:
-      - casServer:cloud,prod,prod-US_1102:5
+      - casServer:cloud,prod,prod-US_1102:7
       X-B3-Traceid:
-      - 6c198084522013542873ac2373afbacf
+      - 55b92cb20bd883142b4f3a21212f1a1c
       X-Robots-Tag:
       - noindex
       X-Vcap-Request-Id:
-      - 154052d5-8818-447a-7151-48678d95a078
+      - 2993f7d4-157a-412b-4177-8315cd0e0f50
     status:
       code: 302
       message: Found
 - request:
     body: null
     headers:
       Accept:
@@ -552,21 +550,21 @@
         \                       <div id=\"requestNewCodeWrapper\" class=\"requestNewCode\">\n
         \                           <a href=\"#\" id=\"newCode\">Request a new code</a>\n
         \                       </div>\n                        \n                        \n
         \                       <br>\n                            \n                        <br/>\n
         \                       <button type=\"submit\" id=\"mfa-verification-code-submit\"
         class=\"btn1\">Next</button>\n                    </div>\n                    <input
         type=\"hidden\" name=\"embed\"            value=\"\"/>\n                    <input
-        type=\"hidden\" name=\"_csrf\"            value=\"ED28063867B6DC6292FDDAFD2EE1C1803C77B15CF598FE3CA38ED40784D19D3B3555BBC20B72DE2727D377FDC8793AA43259\"
+        type=\"hidden\" name=\"_csrf\"            value=\"89E48A5A52FDC9A4B5C29D2918F619B337621D199A534539AAD83C0AA2AB17DAF3C4CF9F56195AEE3BCE4B6866A34928D8BF\"
         />\n                    <input type=\"hidden\" name=\"fromPage\"            value=\"setupEnterMfaCode\"/>\n
         \                   <br/>\n                </form>\n            </div>\n            <div
         class=\"clearfix\"></div> <!-- Ensure that GAuth-component div's height is
         computed correctly. -->\n        </div>\n    </div>\n    <script type=\"text/javascript\">\n
         \       resizePageOnLoad(jQuery(\"#GAuth-component\").height());\n    </script>\n<script>(function(){var
-        js = \"window['__CF$cv$params']={r:'7f0efeaa1972b6e1'};_cpo=document.createElement('script');_cpo.nonce='',_cpo.src='/cdn-cgi/challenge-platform/scripts/invisible.js',document.getElementsByTagName('head')[0].appendChild(_cpo);\";var
+        js = \"window['__CF$cv$params']={r:'7f19a35eadf64797'};_cpo=document.createElement('script');_cpo.nonce='',_cpo.src='/cdn-cgi/challenge-platform/scripts/invisible.js',document.getElementsByTagName('head')[0].appendChild(_cpo);\";var
         _0xh = document.createElement('iframe');_0xh.height = 1;_0xh.width = 1;_0xh.style.position
         = 'absolute';_0xh.style.top = 0;_0xh.style.left = 0;_0xh.style.border = 'none';_0xh.style.visibility
         = 'hidden';document.body.appendChild(_0xh);function handler() {var _0xi =
         _0xh.contentDocument || _0xh.contentWindow.document;if (_0xi) {var _0xj =
         _0xi.createElement('script');_0xj.innerHTML = js;_0xi.getElementsByTagName('head')[0].appendChild(_0xj);}}if
         (document.readyState !== 'loading') {handler();} else if (window.addEventListener)
         {document.addEventListener('DOMContentLoaded', handler);} else {var prev =
@@ -582,49 +580,49 @@
       Access-Control-Allow-Methods:
       - GET,POST,OPTIONS
       Access-Control-Allow-Origin:
       - https://www.garmin.com
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7f0efeaa1972b6e1-QRO
+      - 7f19a35eadf64797-DFW
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Language:
       - en
       Content-Type:
       - text/html;charset=UTF-8
       Date:
-      - Thu, 03 Aug 2023 13:44:20 GMT
+      - Fri, 04 Aug 2023 20:44:24 GMT
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=GAfA2uzl%2F0ZTzFGx6iieBcuC3Bs9Fp%2FrU87lPm%2BoacZdwC9Yj6Y5IYXwyD%2FvuiGhzM3aMcWBJyq7akJUlX3iM5mTQZGqKMkD5QP4Yr0Wp%2BIZJe3repljvx%2FadT%2Bzhdjg"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=Cx2KhXZ92%2Fc38BjEH2TJ8bKkuzKrXn7G4k2KBB4F77VUlfrRtd3Ma36EuNIuEwPKt0MbbTBkiKz6cmCVpLHL78Grb1yaW4qioaOhRpKmselHhTiRADUtZ986y6gwrMzF"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Set-Cookie:
       - org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED;
         Path=SANITIZED
       Transfer-Encoding:
       - chunked
       X-Application-Context:
-      - casServer:cloud,prod,prod-US_1102:5
+      - casServer:cloud,prod,prod-US_1102:7
       X-B3-Traceid:
-      - 32f6eaa23f7f351b363bc86bb39d27ce
+      - 7af5fbfce51e803d25255d01c1881b84
       X-Robots-Tag:
       - noindex
       X-Vcap-Request-Id:
-      - d31fc9af-b2cb-4c64-4031-bd85769894e5
+      - b3ef8bab-184d-4715-4701-3c7749dfb38d
     status:
       code: 200
       message: OK
 - request:
-    body: mfa-code=884445&embed=true&_csrf=ED28063867B6DC6292FDDAFD2EE1C1803C77B15CF598FE3CA38ED40784D19D3B3555BBC20B72DE2727D377FDC8793AA43259&fromPage=setupEnterMfaCode
+    body: mfa-code=577212&embed=true&_csrf=89E48A5A52FDC9A4B5C29D2918F619B337621D199A534539AAD83C0AA2AB17DAF3C4CF9F56195AEE3BCE4B6866A34928D8BF&fromPage=setupEnterMfaCode
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
@@ -637,15 +635,15 @@
         __VCAP_ID__=SANITIZED; __cflb=SANITIZED; org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED
       User-Agent:
       - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X) AppleWebKit/605.1.15
         (KHTML, like Gecko) Mobile/15E148
       referer:
       - https://sso.garmin.com/sso/verifyMFA/loginEnterMfaCode?id=gauth-widget&service=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&source=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountLoginUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountCreationUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&gauthHost=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed
     method: POST
-    uri: https://sso.garmin.com/sso/verifyMFA/loginEnterMfaCode?id=gauth-widget&service=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&source=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountLoginUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountCreationUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&gauthHost=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&rememberMyBrowserChecked=true
+    uri: https://sso.garmin.com/sso/verifyMFA/loginEnterMfaCode?id=gauth-widget&service=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&source=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountLoginUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountCreationUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&gauthHost=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&embedWidget=true
   response:
     body:
       string: ''
     headers:
       Access-Control-Allow-Credentials:
       - 'true'
       Access-Control-Allow-Headers:
@@ -654,42 +652,42 @@
       Access-Control-Allow-Methods:
       - GET,POST,OPTIONS
       Access-Control-Allow-Origin:
       - https://www.garmin.com
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7f0efefd9b09b6e8-QRO
+      - 7f19a3b10f7a475e-DFW
       Connection:
       - keep-alive
       Content-Language:
       - en
       Content-Length:
       - '0'
       Date:
-      - Thu, 03 Aug 2023 13:44:34 GMT
+      - Fri, 04 Aug 2023 20:44:38 GMT
       Location:
-      - https://sso.garmin.com/sso/login?logintoken=KBDAhvPbGI&service=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&locale=en&embed=true&source=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountLoginUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&rememberMyBrowserChecked=true
+      - https://sso.garmin.com/sso/login?logintoken=VuQcJ7ivPg&service=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&locale=en&embed=true&source=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountLoginUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&embedWidget=true
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=agJu1oZ7N7%2Fv7KL7B9%2BF6aIm4EnHWTgYtuAlIidaNhYJOYS1h6rSyhD2Ioh4nbgIyaoBuBcF24b7PfZlzbHGBzWck%2ForkSXc4uSuDIJ7sJabXyyXqAbZLZNk8BrKsDFQ"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=NGgvN3mY6mMbca0W6oPgP77yYti09%2FRuMFbc%2B3TANMVXaqj0LqEANMWpu2bhQ3eP7bUp%2FJHcPil5lor7r%2FZj%2FeqlikvJC40NazuUT3fD0gr%2FhpkVtHuFxfupzOnFljZr"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Set-Cookie:
       - org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED;
         Path=SANITIZED
       X-Application-Context:
-      - casServer:cloud,prod,prod-US_1102:5
+      - casServer:cloud,prod,prod-US_1102:7
       X-B3-Traceid:
-      - 4d99b5adfb5f4e0e5c5d3cb0167df354
+      - 2da2090d89494ce45f9fac6d04602be8
       X-Robots-Tag:
       - noindex
       X-Vcap-Request-Id:
-      - e7aeda65-91ba-49b3-64aa-f2f6f09d5f87
+      - e7305dea-ccb7-422a-4d05-8e07ecb69277
     status:
       code: 302
       message: Found
 - request:
     body: null
     headers:
       Accept:
@@ -703,31 +701,31 @@
         __VCAP_ID__=SANITIZED; __cflb=SANITIZED; org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED
       User-Agent:
       - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X) AppleWebKit/605.1.15
         (KHTML, like Gecko) Mobile/15E148
       referer:
       - https://sso.garmin.com/sso/verifyMFA/loginEnterMfaCode?id=gauth-widget&service=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&source=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountLoginUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountCreationUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&gauthHost=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed
     method: GET
-    uri: https://sso.garmin.com/sso/login?logintoken=KBDAhvPbGI&service=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&locale=en&embed=true&source=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountLoginUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&rememberMyBrowserChecked=true
+    uri: https://sso.garmin.com/sso/login?logintoken=VuQcJ7ivPg&service=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&locale=en&embed=true&source=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountLoginUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&embedWidget=true
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
-        response_url                 \t  = \"https:\\/\\/sso.garmin.com\\/sso\\/embed?ticket=ST-2291079-RkvmCoLwBmLIumhwWYo3-cas\";\n\t\t\tvar
-        logintoken                   \t  = \"KBDAhvPbGI\";\n\t\t\tvar socialLogin
+        response_url                 \t  = \"https:\\/\\/sso.garmin.com\\/sso\\/embed?ticket=ST-2435197-JpeHGkPdeOMWbeob04zU-cas\";\n\t\t\tvar
+        logintoken                   \t  = \"VuQcJ7ivPg\";\n\t\t\tvar socialLogin
         \                  \t  = \"\";\n\t\t\tvar performMFACheck                 =
         \"\";\n\n\t\t\t// Decode url if it's encoded unnecessarily (which is happening
         when SSO GAuth logins redisplay the login page due to session timeouts.)\n\t\t\tif
         (response_url.indexOf('%3A%2F%2F') != -1) {\n\t\t\t\tresponse_url = decodeURIComponent(response_url);\n\t\t\t}\n\t\t\tresponse_url
         = response_url.replace(new RegExp(\"&amp;\", 'g'),\"&\");\n\n\t\t\tvar service_ticket
         = response_url.substring(response_url.indexOf('ticket=') + 7, response_url.length);\n\n\t\t\tif
         (redirectAfterAccountLoginUrl) {\n\t\t\t\tconsoleInfo('casEmbedSuccess.html:
@@ -739,18 +737,19 @@
         service_ticket:               [' + service_ticket + ']');\n\t\t\tif (logintoken)
         {\n\t\t\t\tconsoleInfo('casEmbedSuccess.html: logintoken:                   ['
         + logintoken + ']');\n\t\t\t}\n\t\t\tif (socialLogin) {\n\t\t\t\tconsoleInfo('casEmbedSuccess.html:
         socialLogin:                   [' + socialLogin + ']');\n\t\t\t}\n\n\t\t\tfunction
         send(msg) {\n\t\t\t\tconsoleInfo('casEmbedSuccess.html: send(): Calling XD.postMessage(msg:['
         + JSON.stringify(msg) + '], target_url:[' + parent_url + '])...');\n\t\t\t\tXD.postMessage(msg,
         parent_url, parent);\n\t\t\t\treturn false;\n\t\t\t}\n\n\t\t\tfunction redirect(target){\n\t\t\t\tvar
-        embedWidget = \"\";\n\t\t\t\tif (embedWidget != 'true') {\n\t\t\t\t\tif (logintoken
-        || socialLogin) {\n\t\t\t\t\t\t//  Tell parent to close opened Gauth lite
-        box.\n\t\t\t\t\t\tsend({'closeLiteBox':'1'});\n\t\t\t\t\t} else {\n\t\t\t\t\t\t//
-        Tell parent to resize Gauth widget's height to just that of the loading icon.\n\t\t\t\t\t\tsend({'gauthHeight':jQuery(\"#GAuth-component\").height()});\n\t\t\t\t\t}\n\t\t\t\t}\n\n\t\t\t\tif
+        embedWidget = \"true\";\n\t\t\t\tif (embedWidget != 'true') {\n\t\t\t\t\tif
+        (logintoken || socialLogin) {\n\t\t\t\t\t\t//  Tell parent to close opened
+        Gauth lite box.\n\t\t\t\t\t\tsend({'closeLiteBox':'1'});\n\t\t\t\t\t} else
+        {\n\t\t\t\t\t\t// Tell parent to resize Gauth widget's height to just that
+        of the loading icon.\n\t\t\t\t\t\tsend({'gauthHeight':jQuery(\"#GAuth-component\").height()});\n\t\t\t\t\t}\n\t\t\t\t}\n\n\t\t\t\tif
         (window.opener != null) {\n\t\t\t\t\tvar iframeParent = window.opener.parent;\n\t\t\t\t\tiframeParent.location.href
         = target;\n\t\t\t\t\twindow.close();\n\t\t\t\t} else {\n\t\t\t\t\t// If the
         \"redirectAfterAccountLoginUrl\" GAuth config parameter was specified,\n\t\t\t\t\t//
         a full page refresh upon logon was requested, so redirect the parent window
         upon login.\n\t\t\t\t\tif (redirectAfterAccountLoginUrl || redirectAfterAccountCreationUrl
         || (socialLogin && socialLogin === 'true') || (performMFACheck && performMFACheck
         === 'true')) {\n\n\t\t\t\t\t\tif (embedWidget != 'true') {\n\t\t\t\t\t\t\tsend({'status':'SUCCESS',
@@ -811,15 +810,15 @@
         userdata.country,\n\t\t\t\t\t\t\t\t\t\t\t'passwordChangeRequired' : userdata.passwordChangeRequired,\n\t\t\t\t\t\t\t\t\t\t\t'lastLogin'
         \             : userdata.lastLogin,\n\t\t\t\t\t\t\t\t\t\t\t'erpCustomerNumber'
         \     : userdata.erpCustomerNumber\n\t\t\t\t\t\t\t\t});\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t});\n\t\t\t\t\t}\n\t\t\t\t}\n\t\t\t}\n\t\t</script>\n\t</head>\n\t<body>\n\t\t<div
         id=\"GAuth-component\">\n\t\t\t<img src='/sso/images/ajax-loader.gif' class=\"loaderImage\"/>\n\t\t</div>\n\t\t<script
         type=\"text/javascript\">\n\t\t\tjQuery(document).ready(function(){\n\t\t\t\tvar
         service = \"https:\\/\\/sso.garmin.com\\/sso\\/embed\";\n\t\t\t\tconsoleInfo(\"casEmbedSuccess.html:
         ready, calling redirect('\" + service + \"')...\");\n\t\t\t\tredirect(service);\n\t\t\t});\n\t\t</script>\n\t<script>(function(){var
-        js = \"window['__CF$cv$params']={r:'7f0eff037e33b6df'};_cpo=document.createElement('script');_cpo.nonce='',_cpo.src='/cdn-cgi/challenge-platform/scripts/invisible.js',document.getElementsByTagName('head')[0].appendChild(_cpo);\";var
+        js = \"window['__CF$cv$params']={r:'7f19a3b83f801549'};_cpo=document.createElement('script');_cpo.nonce='',_cpo.src='/cdn-cgi/challenge-platform/scripts/invisible.js',document.getElementsByTagName('head')[0].appendChild(_cpo);\";var
         _0xh = document.createElement('iframe');_0xh.height = 1;_0xh.width = 1;_0xh.style.position
         = 'absolute';_0xh.style.top = 0;_0xh.style.left = 0;_0xh.style.border = 'none';_0xh.style.visibility
         = 'hidden';document.body.appendChild(_0xh);function handler() {var _0xi =
         _0xh.contentDocument || _0xh.contentWindow.document;if (_0xi) {var _0xj =
         _0xi.createElement('script');_0xj.innerHTML = js;_0xi.getElementsByTagName('head')[0].appendChild(_0xj);}}if
         (document.readyState !== 'loading') {handler();} else if (window.addEventListener)
         {document.addEventListener('DOMContentLoaded', handler);} else {var prev =
@@ -835,29 +834,29 @@
       Access-Control-Allow-Methods:
       - GET,POST,OPTIONS
       Access-Control-Allow-Origin:
       - https://www.garmin.com
       CF-Cache-Status:
       - DYNAMIC
       CF-Ray:
-      - 7f0eff037e33b6df-QRO
+      - 7f19a3b83f801549-QRO
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Language:
       - en
       Content-Type:
       - text/html;charset=UTF-8
       Date:
-      - Thu, 03 Aug 2023 13:44:35 GMT
+      - Fri, 04 Aug 2023 20:44:39 GMT
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=Zrk%2F09QvnWGN7H99r%2BKA274jAsm%2FYB8g1ws29goFETQcejOoUds2wKIJ1khOezReb76fYOVVuqTCK1qDo5Zl0PHfA5JM3T2BgYO%2BA45%2BzBAq3yYfS11ZEmcSnwZTnUY%2F"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=imfmx6AwwEBoeOxkjGZH0%2Fuo7TerKPfAo3lexzqusMZoSuUvTb9NcJ%2ByyJcQ2tpq2ir22LFjOMkQL1I3GIaG3fryTvPe4zy0OUoN6zviNS23J9BNLEXkCIiTx381dS8m"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Set-Cookie:
       - org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED;
         Path=SANITIZED
       - CASTGC=SANITIZED; Path=SANITIZED; Secure; HttpOnly
       - CASTGC=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED; Secure;
@@ -882,21 +881,21 @@
       - CASTGC=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED; Secure;
         HttpOnly
       Transfer-Encoding:
       - chunked
       Vary:
       - Accept-Encoding
       X-Application-Context:
-      - casServer:cloud,prod,prod-US_1102:5
+      - casServer:cloud,prod,prod-US_1102:7
       X-B3-Traceid:
-      - 69ae874215e7224b59d4c4946d43e589
+      - 4fcf72f20e7a66dc13e58e89d1664544
       X-Robots-Tag:
       - noindex
       X-Vcap-Request-Id:
-      - 28d5c20f-0bb1-4775-5681-0eef16703ccd
+      - 6feb25a6-e44a-4549-47fa-75badeb102f8
     status:
       code: 200
       message: OK
 - request:
     body: null
     headers:
       Accept:
@@ -916,25 +915,25 @@
       Accept-Ranges:
       - bytes
       Content-Length:
       - '124'
       Content-Type:
       - application/json
       Date:
-      - Thu, 03 Aug 2023 13:44:37 GMT
+      - Fri, 04 Aug 2023 20:44:40 GMT
       ETag:
       - '"20240b1013cb35419bb5b2cff1407a4e"'
       Last-Modified:
       - Thu, 03 Aug 2023 00:16:11 GMT
       Server:
       - AmazonS3
       x-amz-id-2:
-      - 5kBqVpLRbTyIWKiOf3iqFe3UngcAwmTXV/SXVeQGzgS0dDxoXL/3w24eA5EQYuU5VcFgPCVhP499dEGMmVxr9A==
+      - /eMqmlK8obld8yP0MiiccJ5jEcyJNyjP5NUEl5p0NQ6WmCSo+GNI0sthWE+8i64u6u61lY+iJr4=
       x-amz-request-id:
-      - X37BGHYK6YY1J2YX
+      - 29FWE9MM7JBZB8MM
       x-amz-server-side-encryption:
       - AES256
     status:
       code: 200
       message: OK
 - request:
     body: null
@@ -950,36 +949,36 @@
       Connection:
       - !!binary |
         a2VlcC1hbGl2ZQ==
       User-Agent:
       - !!binary |
         Y29tLmdhcm1pbi5hbmRyb2lkLmFwcHMuY29ubmVjdG1vYmlsZQ==
     method: GET
-    uri: https://connectapi.garmin.com/oauth-service/oauth/preauthorized?ticket=ST-2291079-RkvmCoLwBmLIumhwWYo3-cas&login-url=https://sso.garmin.com/sso/embed&accepts-mfa-tokens=true
+    uri: https://connectapi.garmin.com/oauth-service/oauth/preauthorized?ticket=ST-2435197-JpeHGkPdeOMWbeob04zU-cas&login-url=https://sso.garmin.com/sso/embed&accepts-mfa-tokens=true
   response:
     body:
-      string: oauth_token=SANITIZED&oauth_token_secret=SANITIZED&mfa_token=SANITIZED&mfa_expiration_timestamp=2023-08-03
-        15:44:35.000
+      string: oauth_token=SANITIZED&oauth_token_secret=SANITIZED&mfa_token=SANITIZED&mfa_expiration_timestamp=2024-08-03
+        20:44:39.000
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7f0eff0a3f4f1557-QRO
+      - 7f19a3beb9b71557-QRO
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - text/plain;charset=utf-8
       Date:
-      - Thu, 03 Aug 2023 13:44:36 GMT
+      - Fri, 04 Aug 2023 20:44:40 GMT
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=wx6PD3r3tVRMWclSoxaB3Dm82pfy4XmhSvh7od0%2Fux%2FJHi7FudxJADY%2BICt8sKbMK%2B1ywjlmylnj70wO6I4LEL4btzHWgNKZ9LG5aKSKn00w0ZqqHRQiT93c9DptWX7WY24hqz9V8Q%3D%3D"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=cG8UfEpttvW4gX8RkcgEbc%2Fjz0MOIm5YWeo68x2UdO4WGG3DSY1lC1dGGocc%2BZj7p%2BqZy2yZNbmtfxjXlFnSxBfQJ0RE1907rivdo8lAIeNjlyk35y6acqUmJCio9gc9xyTMxWZkSA%3D%3D"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Set-Cookie:
       - _cfuvid=SANITIZED; path=SANITIZED; domain=SANITIZED; HttpOnly; Secure; SameSite=SANITIZED
       Transfer-Encoding:
       - chunked
       alt-svc:
@@ -1015,32 +1014,32 @@
   response:
     body:
       string: '{"scope": "COMMUNITY_COURSE_READ GARMINPAY_WRITE GOLF_API_READ ATP_READ
         GHS_SAMD GHS_UPLOAD INSIGHTS_READ COMMUNITY_COURSE_WRITE CONNECT_WRITE GCOFFER_WRITE
         GARMINPAY_READ DT_CLIENT_ANALYTICS_WRITE GOLF_API_WRITE INSIGHTS_WRITE PRODUCT_SEARCH_READ
         GCOFFER_READ CONNECT_READ ATP_WRITE", "jti": "SANITIZED", "access_token":
         "SANITIZED", "token_type": "Bearer", "refresh_token": "SANITIZED", "expires_in":
-        95631, "refresh_token_expires_in": 2591999}'
+        90758, "refresh_token_expires_in": 2591999}'
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7f0eff0daa741547-QRO
+      - 7f19a3c2d926479c-DFW
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json
       Date:
-      - Thu, 03 Aug 2023 13:44:37 GMT
+      - Fri, 04 Aug 2023 20:44:41 GMT
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=UWx0LW8l%2Bzswc3LmvfMCaKHSQvKAeBn6tXX2wu0jpjPXnK%2Bvyt9%2FibwHSbLvJa43YjJXG8MWRYH5CcV9M1TCjuDE%2BwQ5kMIO684fQExIQLiGQQLqC7OR%2FBjXjV%2BY4ItI3sYempKLpQ%3D%3D"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=iIakQJY4Wz4BRd8mQXfQOMjElxMfZq5J4gzbTACzNHp9kt41Bxc9H%2BBRkdEbAGQPKU08O%2Bb0x67cPAQq1%2FhiQVtxLq%2FrWxUY68hK0Jt4npTqoiIUeHLjsYph3hpIQlEbligc2nhR0w%3D%3D"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Set-Cookie:
       - _cfuvid=SANITIZED; path=SANITIZED; domain=SANITIZED; HttpOnly; Secure; SameSite=SANITIZED
       Transfer-Encoding:
       - chunked
       alt-svc:
```

#### html2text {}

```diff
@@ -1,13 +1,11 @@
 interactions: - request: body: null headers: Accept: - '*/*' Accept-Encoding: -
 gzip, deflate Connection: - keep-alive User-Agent: - Mozilla/5.0 (iPhone; CPU
 iPhone OS 16_5 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Mobile/
-15E148 referer: - https://sso.garmin.com/sso/signin?id=gauth-
-widget&service=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&source=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountLoginUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountCreationUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&gauthHost=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed
-method: GET uri: https://sso.garmin.com/sso/embed?id=gauth-
+15E148 method: GET uri: https://sso.garmin.com/sso/embed?id=gauth-
 widget&embedWidget=true&gauthHost=https%3A%2F%2Fsso.garmin.com%2Fsso response:
 body: string: "
 \n\t
 \n\t
 \n\t
 \n\t
 \n\t
@@ -251,30 +249,30 @@
 \n
 \n\n\n\t
 \n
 \n" headers: Access-Control-Allow-Credentials: - 'true' Access-Control-Allow-
 Headers: - Access-Control-Allow-Headers, Origin,Accept, X-Requested-With,
 Content-Type, Access-Control-Request-Method, Access-Control-Request-Headers
 Access-Control-Allow-Methods: - GET,POST,OPTIONS Access-Control-Allow-Origin: -
-https://www.garmin.com CF-Cache-Status: - DYNAMIC CF-RAY: - 7f0efe9dbf82154b-
-QRO Connection: - keep-alive Content-Encoding: - gzip Content-Language: - en
-Content-Type: - text/html;charset=UTF-8 Date: - Thu, 03 Aug 2023 13:44:18 GMT
+https://www.garmin.com CF-Cache-Status: - DYNAMIC CF-RAY: - 7f19a351192546a1-
+DFW Connection: - keep-alive Content-Encoding: - gzip Content-Language: - en
+Content-Type: - text/html;charset=UTF-8 Date: - Fri, 04 Aug 2023 20:44:22 GMT
 NEL: - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
 Report-To: - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/
-v3?s=EpNuus5s1jsWqmwuAEQuwmJKl4R4x7yKry6fR6Y7YC6inOY0FhOQEkhOEsVh%2FjT2slREgwE8mXWp21snNnLiSMNaYAg%2FXMYN7%2BQXy%2FyZGKBPH63E5AJ7ggao6H0iXiXh"}],"group":
+v3?s=ytG3iKzcFS5%2B99VJD7%2FtqNm2w0E8GcBl0PO%2FS5qsCmdfQkBSJ6ekYSPKRo4ICSZ7qTGOe0aGYYvlGTJhYzx4Z5A46RMoBaAS2EdJ0JfNbriBi4n6TElpPegnmwjqc7Hj"}],"group":
 "cf-nel","max_age":604800}' Server: - cloudflare Set-Cookie: -
 org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED;
 Path=SANITIZED - __cf_bm=SANITIZED; path=SANITIZED; expires=SANITIZED;
 domain=SANITIZED; HttpOnly; Secure; SameSite=SANITIZED - __cflb=SANITIZED;
 SameSite=SANITIZED; Secure; path=SANITIZED; expires=SANITIZED; HttpOnly -
 _cfuvid=SANITIZED; path=SANITIZED; domain=SANITIZED; HttpOnly; Secure;
 SameSite=SANITIZED Transfer-Encoding: - chunked X-Application-Context: -
-casServer:cloud,prod,prod-US_1102:4 X-B3-Traceid: -
-41fd0fc56c11edb61c8a219b7d5e8aab X-Robots-Tag: - noindex X-Vcap-Request-Id: -
-63aed3d0-af94-4f44-791e-87b33f700916 status: code: 200 message: OK - request:
+casServer:cloud,prod,prod-US_1102:2 X-B3-Traceid: -
+7de36dd29fa2d733290a6725dc47dfb8 X-Robots-Tag: - noindex X-Vcap-Request-Id: -
+f780910f-ccdf-4771-49c7-aad225e3c68d status: code: 200 message: OK - request:
 body: null headers: Accept: - '*/*' Accept-Encoding: - gzip, deflate
 Connection: - keep-alive Cookie: - __cf_bm=SANITIZED; _cfuvid=SANITIZED;
 __cflb=SANITIZED;
 org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED
 User-Agent: - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X)
 AppleWebKit/605.1.15 (KHTML, like Gecko) Mobile/15E148 referer: - https://
 sso.garmin.com/sso/embed?id=gauth-
@@ -335,29 +333,29 @@
 \n\t\t\n\n
 \n
 \n
 \n" headers: Access-Control-Allow-Credentials: - 'true' Access-Control-Allow-
 Headers: - Access-Control-Allow-Headers, Origin,Accept, X-Requested-With,
 Content-Type, Access-Control-Request-Method, Access-Control-Request-Headers
 Access-Control-Allow-Methods: - GET,POST,OPTIONS Access-Control-Allow-Origin: -
-https://www.garmin.com CF-Cache-Status: - DYNAMIC CF-Ray: - 7f0efe9ed8421547-
-QRO Connection: - keep-alive Content-Encoding: - gzip Content-Language: - en
-Content-Type: - text/html;charset=UTF-8 Date: - Thu, 03 Aug 2023 13:44:19 GMT
+https://www.garmin.com CF-Cache-Status: - DYNAMIC CF-Ray: - 7f19a3536a19468a-
+DFW Connection: - keep-alive Content-Encoding: - gzip Content-Language: - en
+Content-Type: - text/html;charset=UTF-8 Date: - Fri, 04 Aug 2023 20:44:23 GMT
 NEL: - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
 Report-To: - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/
-v3?s=pUFwZ3E%2F0mJFNFwFoMN7HO5XgGTMP6zxm53htk%2Fdysfp324tli1JN8eL05f4Y1OzTbq%2FlPJr3Ky177Ui6fqBrdPOJs4Iuoi%2Fu6RfDU0p6ku8mha7OD5ihAwayz8H18hH"}],"group":
+v3?s=%2FFRtmPmaDfGDypVhatXfunnrGA%2BA8%2FxV6e%2BuekUdoE5fp2JNEw4bdoizvGG90r1BbOkbo3Ux5ybFDdoX4bKGqoKZWemHOBRFCYnaxHW3Ewoy9EHnNXohVMAu47T3dGnV"}],"group":
 "cf-nel","max_age":604800}' Server: - cloudflare Set-Cookie: -
 org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED;
 Path=SANITIZED - SESSION=SANITIZED; Path=SANITIZED; Secure; HttpOnly -
 __VCAP_ID__=SANITIZED; Path=SANITIZED; HttpOnly; Secure Transfer-Encoding: -
 chunked Vary: - Accept-Encoding X-Application-Context: - casServer:
-cloud,prod,prod-US_1102:5 X-B3-Traceid: - 0c7105857742ac230da0842492b92d1d X-
-Robots-Tag: - noindex X-Vcap-Request-Id: - ba3d4826-a22e-49aa-7888-d62b15cc43b6
+cloud,prod,prod-US_1102:7 X-B3-Traceid: - 66c4d064ee4981291e470a27733c75c8 X-
+Robots-Tag: - noindex X-Vcap-Request-Id: - 97a74fb2-172b-46bf-69fb-dc6d6ac7ca6b
 status: code: 200 message: OK - request: body:
-username=SANITIZED&password=SANITIZED&embed=true&_csrf=085E32B1AAC1E7C4FEE1CCA0CE94D87C4F295B638C604CD3637E11B1D90C2A9992FE5B6DF974136AB8FC45E97D508322F317
+username=SANITIZED&password=SANITIZED&embed=true&_csrf=884C8386EF425D4BA55B54C0B893A3B750BFD7FC791A34EC0BA934444EC04CE6B1FA7484E35E2DF94006783318F9980B7A3A
 headers: Accept: - '*/*' Accept-Encoding: - gzip, deflate Connection: - keep-
 alive Content-Length: - '177' Content-Type: - application/x-www-form-urlencoded
 Cookie: - SESSION=SANITIZED; __cf_bm=SANITIZED; _cfuvid=SANITIZED;
 __VCAP_ID__=SANITIZED; __cflb=SANITIZED;
 org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED
 User-Agent: - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X)
 AppleWebKit/605.1.15 (KHTML, like Gecko) Mobile/15E148 referer: - https://
@@ -366,28 +364,28 @@
 method: POST uri: https://sso.garmin.com/sso/signin?id=gauth-
 widget&service=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&source=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountLoginUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountCreationUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&gauthHost=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed
 response: body: string: '' headers: Access-Control-Allow-Credentials: - 'true'
 Access-Control-Allow-Headers: - Access-Control-Allow-Headers, Origin,Accept, X-
 Requested-With, Content-Type, Access-Control-Request-Method, Access-Control-
 Request-Headers Access-Control-Allow-Methods: - GET,POST,OPTIONS Access-
 Control-Allow-Origin: - https://www.garmin.com CF-Cache-Status: - DYNAMIC CF-
-Ray: - 7f0efea05a41155e-QRO Connection: - keep-alive Content-Language: - en
-Content-Length: - '0' Date: - Thu, 03 Aug 2023 13:44:20 GMT Location: - https:/
+Ray: - 7f19a354dcda1547-QRO Connection: - keep-alive Content-Language: - en
+Content-Length: - '0' Date: - Fri, 04 Aug 2023 20:44:24 GMT Location: - https:/
 /sso.garmin.com/sso/verifyMFA/loginEnterMfaCode?id=gauth-
 widget&service=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&source=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountLoginUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountCreationUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&gauthHost=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed
 NEL: - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
 Report-To: - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/
-v3?s=vZ9OuYl3ehAIn6QRonsHx3lnITP4uLKmQn0RBoyd46XkiNYBeslEOPJz9aPo%2BYnt4ICK9fi2l0m6VI7aXMQSlM5H5sWUeD9DVN1fZtehugkdvNWbk3995Vi4BP6OTPzK"}],"group":
+v3?s=tT3Bm66IlHoACTPEW5aaWCih7nnzM48aWyyucJvJmXCHD6IH9yzYzqrcuZRsM3bzCgO5iQl0GWdKr4pSX%2Bbww%2F1QQ2HgTgnaYSYzYE9M9%2BiXwO8Z9zPyD5ShoR5IaGGZ"}],"group":
 "cf-nel","max_age":604800}' Server: - cloudflare Set-Cookie: -
 org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED;
 Path=SANITIZED - __cfruid=SANITIZED; path=SANITIZED; domain=SANITIZED;
 HttpOnly; Secure; SameSite=SANITIZED Vary: - Accept-Encoding X-Application-
-Context: - casServer:cloud,prod,prod-US_1102:5 X-B3-Traceid: -
-6c198084522013542873ac2373afbacf X-Robots-Tag: - noindex X-Vcap-Request-Id: -
-154052d5-8818-447a-7151-48678d95a078 status: code: 302 message: Found -
+Context: - casServer:cloud,prod,prod-US_1102:7 X-B3-Traceid: -
+55b92cb20bd883142b4f3a21212f1a1c X-Robots-Tag: - noindex X-Vcap-Request-Id: -
+2993f7d4-157a-412b-4177-8315cd0e0f50 status: code: 302 message: Found -
 request: body: null headers: Accept: - '*/*' Accept-Encoding: - gzip, deflate
 Connection: - keep-alive Cookie: - SESSION=SANITIZED; __cf_bm=SANITIZED;
 _cfuvid=SANITIZED; __cfruid=SANITIZED; __VCAP_ID__=SANITIZED; __cflb=SANITIZED;
 org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED
 User-Agent: - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X)
 AppleWebKit/605.1.15 (KHTML, like Gecko) Mobile/15E148 referer: - https://
 sso.garmin.com/sso/signin?id=gauth-
@@ -461,67 +459,67 @@
 \n
 \n
 \n
 " headers: Access-Control-Allow-Credentials: - 'true' Access-Control-Allow-
 Headers: - Access-Control-Allow-Headers, Origin,Accept, X-Requested-With,
 Content-Type, Access-Control-Request-Method, Access-Control-Request-Headers
 Access-Control-Allow-Methods: - GET,POST,OPTIONS Access-Control-Allow-Origin: -
-https://www.garmin.com CF-Cache-Status: - DYNAMIC CF-RAY: - 7f0efeaa1972b6e1-
-QRO Connection: - keep-alive Content-Encoding: - gzip Content-Language: - en
-Content-Type: - text/html;charset=UTF-8 Date: - Thu, 03 Aug 2023 13:44:20 GMT
+https://www.garmin.com CF-Cache-Status: - DYNAMIC CF-RAY: - 7f19a35eadf64797-
+DFW Connection: - keep-alive Content-Encoding: - gzip Content-Language: - en
+Content-Type: - text/html;charset=UTF-8 Date: - Fri, 04 Aug 2023 20:44:24 GMT
 NEL: - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
 Report-To: - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/
-v3?s=GAfA2uzl%2F0ZTzFGx6iieBcuC3Bs9Fp%2FrU87lPm%2BoacZdwC9Yj6Y5IYXwyD%2FvuiGhzM3aMcWBJyq7akJUlX3iM5mTQZGqKMkD5QP4Yr0Wp%2BIZJe3repljvx%2FadT%2Bzhdjg"}],"group":
+v3?s=Cx2KhXZ92%2Fc38BjEH2TJ8bKkuzKrXn7G4k2KBB4F77VUlfrRtd3Ma36EuNIuEwPKt0MbbTBkiKz6cmCVpLHL78Grb1yaW4qioaOhRpKmselHhTiRADUtZ986y6gwrMzF"}],"group":
 "cf-nel","max_age":604800}' Server: - cloudflare Set-Cookie: -
 org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED;
 Path=SANITIZED Transfer-Encoding: - chunked X-Application-Context: - casServer:
-cloud,prod,prod-US_1102:5 X-B3-Traceid: - 32f6eaa23f7f351b363bc86bb39d27ce X-
-Robots-Tag: - noindex X-Vcap-Request-Id: - d31fc9af-b2cb-4c64-4031-bd85769894e5
+cloud,prod,prod-US_1102:7 X-B3-Traceid: - 7af5fbfce51e803d25255d01c1881b84 X-
+Robots-Tag: - noindex X-Vcap-Request-Id: - b3ef8bab-184d-4715-4701-3c7749dfb38d
 status: code: 200 message: OK - request: body: mfa-
-code=884445&embed=true&_csrf=ED28063867B6DC6292FDDAFD2EE1C1803C77B15CF598FE3CA38ED40784D19D3B3555BBC20B72DE2727D377FDC8793AA43259&fromPage=setupEnterMfaCode
+code=577212&embed=true&_csrf=89E48A5A52FDC9A4B5C29D2918F619B337621D199A534539AAD83C0AA2AB17DAF3C4CF9F56195AEE3BCE4B6866A34928D8BF&fromPage=setupEnterMfaCode
 headers: Accept: - '*/*' Accept-Encoding: - gzip, deflate Connection: - keep-
 alive Content-Length: - '160' Content-Type: - application/x-www-form-urlencoded
 Cookie: - SESSION=SANITIZED; __cf_bm=SANITIZED; __cfruid=SANITIZED;
 _cfuvid=SANITIZED; __VCAP_ID__=SANITIZED; __cflb=SANITIZED;
 org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED
 User-Agent: - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X)
 AppleWebKit/605.1.15 (KHTML, like Gecko) Mobile/15E148 referer: - https://
 sso.garmin.com/sso/verifyMFA/loginEnterMfaCode?id=gauth-
 widget&service=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&source=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountLoginUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountCreationUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&gauthHost=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed
 method: POST uri: https://sso.garmin.com/sso/verifyMFA/
 loginEnterMfaCode?id=gauth-
-widget&service=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&source=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountLoginUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountCreationUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&gauthHost=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&rememberMyBrowserChecked=true
+widget&service=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&source=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountLoginUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountCreationUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&gauthHost=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&embedWidget=true
 response: body: string: '' headers: Access-Control-Allow-Credentials: - 'true'
 Access-Control-Allow-Headers: - Access-Control-Allow-Headers, Origin,Accept, X-
 Requested-With, Content-Type, Access-Control-Request-Method, Access-Control-
 Request-Headers Access-Control-Allow-Methods: - GET,POST,OPTIONS Access-
 Control-Allow-Origin: - https://www.garmin.com CF-Cache-Status: - DYNAMIC CF-
-RAY: - 7f0efefd9b09b6e8-QRO Connection: - keep-alive Content-Language: - en
-Content-Length: - '0' Date: - Thu, 03 Aug 2023 13:44:34 GMT Location: - https:/
+RAY: - 7f19a3b10f7a475e-DFW Connection: - keep-alive Content-Language: - en
+Content-Length: - '0' Date: - Fri, 04 Aug 2023 20:44:38 GMT Location: - https:/
 /sso.garmin.com/sso/
-login?logintoken=KBDAhvPbGI&service=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&locale=en&embed=true&source=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountLoginUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&rememberMyBrowserChecked=true
+login?logintoken=VuQcJ7ivPg&service=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&locale=en&embed=true&source=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountLoginUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&embedWidget=true
 NEL: - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
 Report-To: - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/
-v3?s=agJu1oZ7N7%2Fv7KL7B9%2BF6aIm4EnHWTgYtuAlIidaNhYJOYS1h6rSyhD2Ioh4nbgIyaoBuBcF24b7PfZlzbHGBzWck%2ForkSXc4uSuDIJ7sJabXyyXqAbZLZNk8BrKsDFQ"}],"group":
+v3?s=NGgvN3mY6mMbca0W6oPgP77yYti09%2FRuMFbc%2B3TANMVXaqj0LqEANMWpu2bhQ3eP7bUp%2FJHcPil5lor7r%2FZj%2FeqlikvJC40NazuUT3fD0gr%2FhpkVtHuFxfupzOnFljZr"}],"group":
 "cf-nel","max_age":604800}' Server: - cloudflare Set-Cookie: -
 org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED;
-Path=SANITIZED X-Application-Context: - casServer:cloud,prod,prod-US_1102:5 X-
-B3-Traceid: - 4d99b5adfb5f4e0e5c5d3cb0167df354 X-Robots-Tag: - noindex X-Vcap-
-Request-Id: - e7aeda65-91ba-49b3-64aa-f2f6f09d5f87 status: code: 302 message:
+Path=SANITIZED X-Application-Context: - casServer:cloud,prod,prod-US_1102:7 X-
+B3-Traceid: - 2da2090d89494ce45f9fac6d04602be8 X-Robots-Tag: - noindex X-Vcap-
+Request-Id: - e7305dea-ccb7-422a-4d05-8e07ecb69277 status: code: 302 message:
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
-login?logintoken=KBDAhvPbGI&service=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&locale=en&embed=true&source=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountLoginUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&rememberMyBrowserChecked=true
+login?logintoken=VuQcJ7ivPg&service=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&locale=en&embed=true&source=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountLoginUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&embedWidget=true
 response: body: string: "
 \n
 \n\t
 \n\t\t
 \n\t\t
 \n\t\t
 \n\t\t
@@ -540,20 +538,20 @@
 \n\t\t
 \n\t
 \n
 \n" headers: Access-Control-Allow-Credentials: - 'true' Access-Control-Allow-
 Headers: - Access-Control-Allow-Headers, Origin,Accept, X-Requested-With,
 Content-Type, Access-Control-Request-Method, Access-Control-Request-Headers
 Access-Control-Allow-Methods: - GET,POST,OPTIONS Access-Control-Allow-Origin: -
-https://www.garmin.com CF-Cache-Status: - DYNAMIC CF-Ray: - 7f0eff037e33b6df-
+https://www.garmin.com CF-Cache-Status: - DYNAMIC CF-Ray: - 7f19a3b83f801549-
 QRO Connection: - keep-alive Content-Encoding: - gzip Content-Language: - en
-Content-Type: - text/html;charset=UTF-8 Date: - Thu, 03 Aug 2023 13:44:35 GMT
+Content-Type: - text/html;charset=UTF-8 Date: - Fri, 04 Aug 2023 20:44:39 GMT
 NEL: - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
 Report-To: - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/
-v3?s=Zrk%2F09QvnWGN7H99r%2BKA274jAsm%2FYB8g1ws29goFETQcejOoUds2wKIJ1khOezReb76fYOVVuqTCK1qDo5Zl0PHfA5JM3T2BgYO%2BA45%2BzBAq3yYfS11ZEmcSnwZTnUY%2F"}],"group":
+v3?s=imfmx6AwwEBoeOxkjGZH0%2Fuo7TerKPfAo3lexzqusMZoSuUvTb9NcJ%2ByyJcQ2tpq2ir22LFjOMkQL1I3GIaG3fryTvPe4zy0OUoN6zviNS23J9BNLEXkCIiTx381dS8m"}],"group":
 "cf-nel","max_age":604800}' Server: - cloudflare Set-Cookie: -
 org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED;
 Path=SANITIZED - CASTGC=SANITIZED; Path=SANITIZED; Secure; HttpOnly -
 CASTGC=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED; Secure;
 HttpOnly - GARMIN-SSO=SANITIZED; Domain=SANITIZED; Path=SANITIZED - GARMIN-
 SSO=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Domain=SANITIZED;
 Path=SANITIZED - GarminNoCache=SANITIZED; Domain=SANITIZED; Path=SANITIZED -
@@ -565,41 +563,40 @@
 Path=SANITIZED - GARMIN-SSO-GUID=SANITIZED; Max-Age=SANITIZED;
 Expires=SANITIZED; Domain=SANITIZED; Path=SANITIZED - GARMIN-SSO-CUST-
 GUID=SANITIZED; Domain=SANITIZED; Path=SANITIZED - GARMIN-SSO-CUST-
 GUID=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Domain=SANITIZED;
 Path=SANITIZED - CASTGC=SANITIZED; Path=SANITIZED; Secure; HttpOnly -
 CASTGC=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED; Secure;
 HttpOnly Transfer-Encoding: - chunked Vary: - Accept-Encoding X-Application-
-Context: - casServer:cloud,prod,prod-US_1102:5 X-B3-Traceid: -
-69ae874215e7224b59d4c4946d43e589 X-Robots-Tag: - noindex X-Vcap-Request-Id: -
-28d5c20f-0bb1-4775-5681-0eef16703ccd status: code: 200 message: OK - request:
+Context: - casServer:cloud,prod,prod-US_1102:7 X-B3-Traceid: -
+4fcf72f20e7a66dc13e58e89d1664544 X-Robots-Tag: - noindex X-Vcap-Request-Id: -
+6feb25a6-e44a-4549-47fa-75badeb102f8 status: code: 200 message: OK - request:
 body: null headers: Accept: - '*/*' Accept-Encoding: - gzip, deflate
 Connection: - keep-alive User-Agent: - python-requests/2.31.0 method: GET uri:
 https://thegarth.s3.amazonaws.com/oauth_consumer.json response: body: string: '
 {"consumer_key": "SANITIZED", "consumer_secret": "SANITIZED"}' headers: Accept-
 Ranges: - bytes Content-Length: - '124' Content-Type: - application/json Date:
-- Thu, 03 Aug 2023 13:44:37 GMT ETag: - '"20240b1013cb35419bb5b2cff1407a4e"'
+- Fri, 04 Aug 2023 20:44:40 GMT ETag: - '"20240b1013cb35419bb5b2cff1407a4e"'
 Last-Modified: - Thu, 03 Aug 2023 00:16:11 GMT Server: - AmazonS3 x-amz-id-2: -
-5kBqVpLRbTyIWKiOf3iqFe3UngcAwmTXV/SXVeQGzgS0dDxoXL/
-3w24eA5EQYuU5VcFgPCVhP499dEGMmVxr9A== x-amz-request-id: - X37BGHYK6YY1J2YX x-
-amz-server-side-encryption: - AES256 status: code: 200 message: OK - request:
-body: null headers: Accept: - !!binary | Ki8q Accept-Encoding: - !!binary |
-Z3ppcCwgZGVmbGF0ZQ== Authorization: - Bearer SANITIZED Connection: - !!binary |
-a2VlcC1hbGl2ZQ== User-Agent: - !!binary |
-Y29tLmdhcm1pbi5hbmRyb2lkLmFwcHMuY29ubmVjdG1vYmlsZQ== method: GET uri: https://
-connectapi.garmin.com/oauth-service/oauth/preauthorized?ticket=ST-2291079-
-RkvmCoLwBmLIumhwWYo3-cas&login-url=https://sso.garmin.com/sso/embed&accepts-
-mfa-tokens=true response: body: string:
-oauth_token=SANITIZED&oauth_token_secret=SANITIZED&mfa_token=SANITIZED&mfa_expiration_timestamp=2023-
-08-03 15:44:35.000 headers: CF-Cache-Status: - DYNAMIC CF-RAY: -
-7f0eff0a3f4f1557-QRO Connection: - keep-alive Content-Encoding: - gzip Content-
-Type: - text/plain;charset=utf-8 Date: - Thu, 03 Aug 2023 13:44:36 GMT NEL: - '
+/eMqmlK8obld8yP0MiiccJ5jEcyJNyjP5NUEl5p0NQ6WmCSo+GNI0sthWE+8i64u6u61lY+iJr4= x-
+amz-request-id: - 29FWE9MM7JBZB8MM x-amz-server-side-encryption: - AES256
+status: code: 200 message: OK - request: body: null headers: Accept: - !!binary
+| Ki8q Accept-Encoding: - !!binary | Z3ppcCwgZGVmbGF0ZQ== Authorization: -
+Bearer SANITIZED Connection: - !!binary | a2VlcC1hbGl2ZQ== User-Agent: -
+!!binary | Y29tLmdhcm1pbi5hbmRyb2lkLmFwcHMuY29ubmVjdG1vYmlsZQ== method: GET
+uri: https://connectapi.garmin.com/oauth-service/oauth/preauthorized?ticket=ST-
+2435197-JpeHGkPdeOMWbeob04zU-cas&login-url=https://sso.garmin.com/sso/
+embed&accepts-mfa-tokens=true response: body: string:
+oauth_token=SANITIZED&oauth_token_secret=SANITIZED&mfa_token=SANITIZED&mfa_expiration_timestamp=2024-
+08-03 20:44:39.000 headers: CF-Cache-Status: - DYNAMIC CF-RAY: -
+7f19a3beb9b71557-QRO Connection: - keep-alive Content-Encoding: - gzip Content-
+Type: - text/plain;charset=utf-8 Date: - Fri, 04 Aug 2023 20:44:40 GMT NEL: - '
 {"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}' Report-To: - '
 {"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/
-v3?s=wx6PD3r3tVRMWclSoxaB3Dm82pfy4XmhSvh7od0%2Fux%2FJHi7FudxJADY%2BICt8sKbMK%2B1ywjlmylnj70wO6I4LEL4btzHWgNKZ9LG5aKSKn00w0ZqqHRQiT93c9DptWX7WY24hqz9V8Q%3D%3D"}],"group":
+v3?s=cG8UfEpttvW4gX8RkcgEbc%2Fjz0MOIm5YWeo68x2UdO4WGG3DSY1lC1dGGocc%2BZj7p%2BqZy2yZNbmtfxjXlFnSxBfQJ0RE1907rivdo8lAIeNjlyk35y6acqUmJCio9gc9xyTMxWZkSA%3D%3D"}],"group":
 "cf-nel","max_age":604800}' Server: - cloudflare Set-Cookie: -
 _cfuvid=SANITIZED; path=SANITIZED; domain=SANITIZED; HttpOnly; Secure;
 SameSite=SANITIZED Transfer-Encoding: - chunked alt-svc: - h3=":443"; ma=86400
 status: code: 200 message: OK - request: body: '' headers: Accept: - !!binary |
 Ki8q Accept-Encoding: - !!binary | Z3ppcCwgZGVmbGF0ZQ== Authorization: - Bearer
 SANITIZED Connection: - !!binary | a2VlcC1hbGl2ZQ== Content-Length: - !!binary
 | MA== Content-Type: - !!binary | YXBwbGljYXRpb24veC13d3ctZm9ybS11cmxlbmNvZGVk
@@ -607,19 +604,19 @@
 method: POST uri: https://connectapi.garmin.com/oauth-service/oauth/exchange/
 user/2.0 response: body: string: '{"scope": "COMMUNITY_COURSE_READ
 GARMINPAY_WRITE GOLF_API_READ ATP_READ GHS_SAMD GHS_UPLOAD INSIGHTS_READ
 COMMUNITY_COURSE_WRITE CONNECT_WRITE GCOFFER_WRITE GARMINPAY_READ
 DT_CLIENT_ANALYTICS_WRITE GOLF_API_WRITE INSIGHTS_WRITE PRODUCT_SEARCH_READ
 GCOFFER_READ CONNECT_READ ATP_WRITE", "jti": "SANITIZED", "access_token":
 "SANITIZED", "token_type": "Bearer", "refresh_token": "SANITIZED",
-"expires_in": 95631, "refresh_token_expires_in": 2591999}' headers: CF-Cache-
-Status: - DYNAMIC CF-RAY: - 7f0eff0daa741547-QRO Connection: - keep-alive
-Content-Encoding: - gzip Content-Type: - application/json Date: - Thu, 03 Aug
-2023 13:44:37 GMT NEL: - '{"success_fraction":0.01,"report_to":"cf-
+"expires_in": 90758, "refresh_token_expires_in": 2591999}' headers: CF-Cache-
+Status: - DYNAMIC CF-RAY: - 7f19a3c2d926479c-DFW Connection: - keep-alive
+Content-Encoding: - gzip Content-Type: - application/json Date: - Fri, 04 Aug
+2023 20:44:41 GMT NEL: - '{"success_fraction":0.01,"report_to":"cf-
 nel","max_age":604800}' Report-To: - '{"endpoints":[{"url":"https:\/\/
 a.nel.cloudflare.com\/report\/
-v3?s=UWx0LW8l%2Bzswc3LmvfMCaKHSQvKAeBn6tXX2wu0jpjPXnK%2Bvyt9%2FibwHSbLvJa43YjJXG8MWRYH5CcV9M1TCjuDE%2BwQ5kMIO684fQExIQLiGQQLqC7OR%2FBjXjV%2BY4ItI3sYempKLpQ%3D%3D"}],"group":
+v3?s=iIakQJY4Wz4BRd8mQXfQOMjElxMfZq5J4gzbTACzNHp9kt41Bxc9H%2BBRkdEbAGQPKU08O%2Bb0x67cPAQq1%2FhiQVtxLq%2FrWxUY68hK0Jt4npTqoiIUeHLjsYph3hpIQlEbligc2nhR0w%3D%3D"}],"group":
 "cf-nel","max_age":604800}' Server: - cloudflare Set-Cookie: -
 _cfuvid=SANITIZED; path=SANITIZED; domain=SANITIZED; HttpOnly; Secure;
 SameSite=SANITIZED Transfer-Encoding: - chunked alt-svc: - h3=":443"; ma=86400
 cache-control: - no-cache, no-store, private pragma: - no-cache status: code:
 200 message: OK version: 1
```

### Comparing `garth-0.4.0/tests/cassettes/test_username.yaml` & `garth-0.4.1/tests/cassettes/test_username.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.0/tests/conftest.py` & `garth-0.4.1/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -98,17 +98,14 @@
 def sanitize_response(response):
     for key in ["set-cookie", "Set-Cookie"]:
         if key in response["headers"]:
             cookies = response["headers"][key]
             sanitized_cookies = [sanitize_cookie(cookie) for cookie in cookies]
             response["headers"][key] = sanitized_cookies
 
-    if "body" not in response and response["body"]["string"]:
-        return response
-
     body = response["body"]["string"].decode("utf8")
     patterns = [
         "oauth_token=[^&]*",
         "oauth_token_secret=[^&]*",
         "mfa_token=[^&]*",
     ]
     for pattern in patterns:
```

### Comparing `garth-0.4.0/tests/stats/cassettes/test_daily_hrv.yaml` & `garth-0.4.1/tests/stats/cassettes/test_daily_hrv.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.0/tests/stats/cassettes/test_daily_hrv_no_results.yaml` & `garth-0.4.1/tests/stats/cassettes/test_daily_hrv_no_results.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.0/tests/stats/cassettes/test_daily_hrv_paginate.yaml` & `garth-0.4.1/tests/stats/cassettes/test_daily_hrv_paginate.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.0/tests/stats/cassettes/test_daily_hrv_paginate_no_results.yaml` & `garth-0.4.1/tests/stats/cassettes/test_daily_hrv_paginate_no_results.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.0/tests/stats/cassettes/test_daily_intensity_minutes.yaml` & `garth-0.4.1/tests/stats/cassettes/test_daily_intensity_minutes.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.0/tests/stats/cassettes/test_daily_sleep.yaml` & `garth-0.4.1/tests/stats/cassettes/test_daily_sleep.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.0/tests/stats/cassettes/test_daily_steps.yaml` & `garth-0.4.1/tests/stats/cassettes/test_daily_steps.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.0/tests/stats/cassettes/test_daily_stress.yaml` & `garth-0.4.1/tests/stats/cassettes/test_daily_stress.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.0/tests/stats/cassettes/test_daily_stress_pagination.yaml` & `garth-0.4.1/tests/stats/cassettes/test_daily_stress_pagination.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.0/tests/stats/cassettes/test_sleep_data_get.yaml` & `garth-0.4.1/tests/stats/cassettes/test_sleep_data_get.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.0/tests/stats/cassettes/test_sleep_data_list.yaml` & `garth-0.4.1/tests/stats/cassettes/test_sleep_data_list.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.0/tests/stats/cassettes/test_weekly_intensity_minutes.yaml` & `garth-0.4.1/tests/stats/cassettes/test_weekly_intensity_minutes.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.0/tests/stats/cassettes/test_weekly_steps.yaml` & `garth-0.4.1/tests/stats/cassettes/test_weekly_steps.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.0/tests/stats/cassettes/test_weekly_stress.yaml` & `garth-0.4.1/tests/stats/cassettes/test_weekly_stress.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.0/tests/stats/cassettes/test_weekly_stress_beyond_data.yaml` & `garth-0.4.1/tests/stats/cassettes/test_weekly_stress_beyond_data.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.0/tests/stats/cassettes/test_weekly_stress_pagination.yaml` & `garth-0.4.1/tests/stats/cassettes/test_weekly_stress_pagination.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.0/tests/stats/test_hrv.py` & `garth-0.4.1/tests/stats/test_hrv.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.0/tests/stats/test_intensity_minutes.py` & `garth-0.4.1/tests/stats/test_intensity_minutes.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.0/tests/stats/test_sleep.py` & `garth-0.4.1/tests/stats/test_sleep.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.0/tests/stats/test_steps.py` & `garth-0.4.1/tests/stats/test_steps.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.0/tests/stats/test_stress.py` & `garth-0.4.1/tests/stats/test_stress.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.0/tests/test_http.py` & `garth-0.4.1/tests/test_http.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
     assert resp.ok
 
     with pytest.raises(HTTPError):
         client.request("GET", "connectapi", "/")
 
 
 @pytest.mark.vcr
-def test_login_success(monkeypatch, client: Client):
+def test_login_success_mfa(monkeypatch, client: Client):
     def mock_input(_):
         return "327751"
 
     monkeypatch.setattr("builtins.input", mock_input)
 
     assert client.oauth1_token is None
     assert client.oauth2_token is None
```

### Comparing `garth-0.4.0/tests/test_sso.py` & `garth-0.4.1/tests/test_sso.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,22 +12,23 @@
 @pytest.mark.vcr
 def test_login_email_password_fail(client: Client):
     with pytest.raises(HTTPError):
         sso.login("user@example.com", "wrong_p@ssword", client=client)
 
 
 @pytest.mark.vcr
-def test_login_success(monkeypatch, client: Client):
+def test_login_success_mfa(monkeypatch, client: Client):
     def mock_input(_):
         return "327751"
 
     monkeypatch.setattr("builtins.input", mock_input)
     oauth1, oauth2 = sso.login(
         "user@example.com", "correct_password", client=client
     )
+
     assert oauth1
     assert isinstance(oauth1, OAuth1Token)
     assert oauth2
     assert isinstance(oauth2, OAuth2Token)
 
 
 def test_set_expirations(oauth2_token_dict: dict):
```

### Comparing `garth-0.4.0/tests/test_utils.py` & `garth-0.4.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.0/PKG-INFO` & `garth-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garth
-Version: 0.4.0
+Version: 0.4.1
 Summary: Garmin SSO auth + Connect client
 Author-Email: Matin Tamizi <mtamizi@duck.com>
 License: MIT
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.10
```

