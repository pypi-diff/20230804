# Comparing `tmp/authentikate-0.1.2.tar.gz` & `tmp/authentikate-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "authentikate-0.1.2.tar", max compression
+gzip compressed data, was "authentikate-0.1.3.tar", max compression
```

## Comparing `authentikate-0.1.2.tar` & `authentikate-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,20 @@
--rw-r--r--   0        0        0       22 2023-07-28 09:41:36.120221 authentikate-0.1.2/README.md
--rw-r--r--   0        0        0       21 2023-07-28 09:40:37.823933 authentikate-0.1.2/authentikate/__init__.py
--rw-r--r--   0        0        0      157 2023-08-03 14:19:57.192109 authentikate-0.1.2/authentikate/admin.py
--rw-r--r--   0        0        0      156 2023-08-03 14:19:57.200110 authentikate-0.1.2/authentikate/apps.py
--rw-r--r--   0        0        0      474 2023-08-03 14:19:57.204110 authentikate-0.1.2/authentikate/decode.py
--rw-r--r--   0        0        0      409 2023-08-03 14:19:57.212109 authentikate-0.1.2/authentikate/errors.py
--rw-r--r--   0        0        0     2542 2023-08-03 14:19:57.216110 authentikate-0.1.2/authentikate/expand.py
--rw-r--r--   0        0        0     5875 2023-08-03 14:19:57.180109 authentikate-0.1.2/authentikate/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-08-03 14:19:57.180109 authentikate-0.1.2/authentikate/migrations/__init__.py
--rw-r--r--   0        0        0      850 2023-08-03 14:19:57.228110 authentikate-0.1.2/authentikate/models.py
--rw-r--r--   0        0        0     1863 2023-08-03 14:19:57.236110 authentikate-0.1.2/authentikate/settings.py
--rw-r--r--   0        0        0        0 2023-08-03 15:19:29.893577 authentikate-0.1.2/authentikate/strawberry/__init__.py
--rw-r--r--   0        0        0      300 2023-08-03 15:19:17.041502 authentikate-0.1.2/authentikate/strawberry/filters.py
--rw-r--r--   0        0        0      241 2023-08-03 15:19:36.301615 authentikate-0.1.2/authentikate/strawberry/types.py
--rw-r--r--   0        0        0     1810 2023-08-03 14:19:57.244110 authentikate-0.1.2/authentikate/structs.py
--rw-r--r--   0        0        0     1884 2023-08-03 14:19:57.264110 authentikate-0.1.2/authentikate/utils.py
--rw-r--r--   0        0        0     1700 2023-08-04 12:46:37.320469 authentikate-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      488 1970-01-01 00:00:00.000000 authentikate-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       22 2023-07-28 09:41:36.120221 authentikate-0.1.3/README.md
+-rw-r--r--   0        0        0       21 2023-07-28 09:40:37.823933 authentikate-0.1.3/authentikate/__init__.py
+-rw-r--r--   0        0        0      157 2023-08-03 14:19:57.192109 authentikate-0.1.3/authentikate/admin.py
+-rw-r--r--   0        0        0      156 2023-08-03 14:19:57.200110 authentikate-0.1.3/authentikate/apps.py
+-rw-r--r--   0        0        0      474 2023-08-03 14:19:57.204110 authentikate-0.1.3/authentikate/decode.py
+-rw-r--r--   0        0        0      482 2023-08-04 14:25:56.348934 authentikate-0.1.3/authentikate/errors.py
+-rw-r--r--   0        0        0     2731 2023-08-04 14:32:49.539301 authentikate-0.1.3/authentikate/expand.py
+-rw-r--r--   0        0        0      472 2023-08-04 14:41:02.022034 authentikate-0.1.3/authentikate/imitate.py
+-rw-r--r--   0        0        0     5875 2023-08-03 14:19:57.180109 authentikate-0.1.3/authentikate/migrations/0001_initial.py
+-rw-r--r--   0        0        0      655 2023-08-04 14:36:41.296594 authentikate-0.1.3/authentikate/migrations/0002_alter_user_unique_together_and_more.py
+-rw-r--r--   0        0        0        0 2023-08-03 14:19:57.180109 authentikate-0.1.3/authentikate/migrations/__init__.py
+-rw-r--r--   0        0        0     1063 2023-08-04 14:36:27.720519 authentikate-0.1.3/authentikate/models.py
+-rw-r--r--   0        0        0     2550 2023-08-04 14:25:56.324934 authentikate-0.1.3/authentikate/settings.py
+-rw-r--r--   0        0        0        0 2023-08-03 15:19:29.893577 authentikate-0.1.3/authentikate/strawberry/__init__.py
+-rw-r--r--   0        0        0      300 2023-08-03 15:19:17.041502 authentikate-0.1.3/authentikate/strawberry/filters.py
+-rw-r--r--   0        0        0      241 2023-08-03 15:19:36.301615 authentikate-0.1.3/authentikate/strawberry/types.py
+-rw-r--r--   0        0        0     2124 2023-08-04 14:19:27.802571 authentikate-0.1.3/authentikate/structs.py
+-rw-r--r--   0        0        0     2483 2023-08-04 14:19:52.410727 authentikate-0.1.3/authentikate/utils.py
+-rw-r--r--   0        0        0     1727 2023-08-04 14:42:30.542520 authentikate-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      536 1970-01-01 00:00:00.000000 authentikate-0.1.3/PKG-INFO
```

### Comparing `authentikate-0.1.2/authentikate/expand.py` & `authentikate-0.1.3/authentikate/expand.py`

 * *Files 14% similar despite different names*

```diff
@@ -44,26 +44,32 @@
         if token.client_id is None:
             app = None
         else:
             app, _ = models.App.objects.get_or_create(
                 client_id=token.client_id, iss=token.iss
             )
 
-        user = models.User.objects.get(username=token_to_username(token))
+        user = models.User.objects.get(sub=token.sub, iss=token.iss)
         if user.changed_hash != token.changed_hash:
             # User has changed, update the user object
             user.first_name = token.preferred_username
             user.changed_hash = token.changed_hash
             set_user_groups(user, token.roles)
             user.save()
 
     except models.User.DoesNotExist:
+        preexisting_user = models.User.objects.filter(
+            username=token.preferred_username
+        ).first()
+
         user = models.User(
             sub=token.sub,
-            username=token_to_username(token),
+            username=token_to_username(token)
+            if preexisting_user
+            else token.preferred_username,
             iss=token.iss,
             first_name=token.preferred_username,
         )
         user.set_unusable_password()
         user.save()
         user.first_name = token.preferred_username
         user.changed_hash = token.changed_hash
```

### Comparing `authentikate-0.1.2/authentikate/migrations/0001_initial.py` & `authentikate-0.1.3/authentikate/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `authentikate-0.1.2/authentikate/structs.py` & `authentikate-0.1.3/authentikate/structs.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 import dataclasses
 from .models import User, App
-from pydantic import BaseModel, validator
+from pydantic import BaseModel, validator, Field
 
 logger = logging.getLogger(__name__)
 
 
 class JWTToken(BaseModel):
     sub: str
     iss: str
@@ -31,18 +31,24 @@
     def scopes(self) -> list[str]:
         return self.scope.split(" ")
 
     class Config:
         extra = "ignore"
 
 
-class LokSettings(BaseModel):
+class AuthentikateSettings(BaseModel):
     algorithms: list[str]
     public_key: str
     force_client: bool
+    allow_imitate: bool
+    imitate_headers: list[str] = Field(default_factory=lambda: ["X-Imitate-User"])
+    authorization_headers: list[str] = Field(
+        default_factory=lambda: ["Authorization", "X-Authorization", "AUTHORIZATION"]
+    )
+    imitate_permission: str = "authentikate.imitate"
 
 
 @dataclasses.dataclass
 class Auth:
     """
     Mimics the structure of `AbstractAccessToken` so you can use standard
     Django Oauth Toolkit permissions like `TokenHasScope`.
```

### Comparing `authentikate-0.1.2/authentikate/utils.py` & `authentikate-0.1.3/authentikate/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 from authentikate.structs import Auth
 from authentikate.decode import decode_token
-from authentikate.settings import get_settings
+from authentikate.settings import get_settings, AuthentikateSettings
 import re
 import logging
 from authentikate.expand import expand_token
+from authentikate.imitate import imitate_user
 
-logger = logging.getLogger(__name__)#
+logger = logging.getLogger(__name__)  #
 
 
-settings = None
-
-
-def authenticate_token(token: str) -> Auth:
+def authenticate_token(token: str, settings: AuthentikateSettings) -> Auth:
     """
     Authenticate a token and return the auth context
     (containing user, app and scopes)
 
     """
-    global settings
-    if not settings:
-        settings = get_settings()
-
 
     decoded = decode_token(token, settings.algorithms, settings.public_key)
     return expand_token(decoded, settings.force_client)
 
 
 jwt_re = re.compile(r"Bearer\s(?P<token>[^\s]*)")
 
@@ -34,39 +28,66 @@
     if m:
         token = m.group("token")
         return token
 
     raise ValueError("Not a valid token")
 
 
-def authenticate_header_or_none(headers: dict) -> Auth | None:
+def authenticate_header_or_none(
+    headers: dict, settings: AuthentikateSettings = None
+) -> Auth | None:
     """
     Authenticate a request and return the auth context
     (containing user, app and scopes)
 
     """
-    authorization = headers.get("authorization", None)
+    if not settings:
+        settings = get_settings()
+
+    for i in settings.authorization_headers:
+        authorization = headers.get(i, None)
+        if authorization:
+            break
+
     if not authorization:
-        authorization = headers.get("Authorization", None)
-        if not authorization:
-            logger.info("No Authorization header. Skipping!")
-            return None
+        logger.info("No Authorization header. Skipping!")
+        return None
 
     try:
         token = extract_plain_from_authorization(authorization)
     except ValueError:
         logger.error("Not a valid token. Skipping!")
         return None
 
     try:
-        return authenticate_token(token)
+        auth = authenticate_token(token, settings)
     except Exception:
         logger.error("Error authenticating token. Skipping!", exc_info=True)
         return None
 
+    for i in settings.imitate_headers:
+        imitate = headers.get(i, None)
+        if imitate:
+            break
+
+    if not imitate:
+        logger.info("No Imitate header. Returning!")
+        return auth
+
+    try:
+        return imitate_user(auth, imitate, settings)
+    except Exception:
+        logger.error("Error imitating user. Skipping!", exc_info=True)
+        return None
+
+
+def authenticate_token_or_none(
+    token: str, settings: AuthentikateSettings = None
+) -> Auth | None:
+    if not settings:
+        settings = get_settings()
 
-def authenticate_token_or_none(token: dict) -> Auth | None:
     try:
-        return authenticate_token(token)
+        return authenticate_token(token, settings)
     except Exception:
         logger.error("Error authenticating token. Skipping!", exc_info=True)
         return None
```

### Comparing `authentikate-0.1.2/pyproject.toml` & `authentikate-0.1.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [tool.poetry]
 name = "authentikate"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["jhnnsrs <jhnnsrs@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 packages = [{ include = "authentikate" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pyjwt = "^2.8.0"
 pydantic = "<2"
+django-guardian = "^2.4.0"
 
 
 [tool.mypy]
 plugins = ["mypy_django_plugin.main"]
 ignore_missing_imports = true
 strict = true
```

