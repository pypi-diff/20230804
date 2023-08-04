# Comparing `tmp/django_oauth_login-0.2.3.tar.gz` & `tmp/django_oauth_login-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_oauth_login-0.2.3.tar", max compression
+gzip compressed data, was "django_oauth_login-0.2.4.tar", max compression
```

## Comparing `django_oauth_login-0.2.3.tar` & `django_oauth_login-0.2.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1065 2023-01-31 17:18:07.510378 django_oauth_login-0.2.3/LICENSE
--rw-r--r--   0        0        0    10098 2023-01-31 17:18:07.510378 django_oauth_login-0.2.3/README.md
--rw-r--r--   0        0        0        0 2023-01-31 17:18:07.510378 django_oauth_login-0.2.3/oauthlogin/__init__.py
--rw-r--r--   0        0        0      344 2023-01-31 17:18:07.510378 django_oauth_login-0.2.3/oauthlogin/admin.py
--rw-r--r--   0        0        0      152 2023-01-31 17:18:07.510378 django_oauth_login-0.2.3/oauthlogin/apps.py
--rw-r--r--   0        0        0      246 2023-01-31 17:18:07.510378 django_oauth_login-0.2.3/oauthlogin/exceptions.py
--rw-r--r--   0        0        0     1987 2023-01-31 17:18:07.510378 django_oauth_login-0.2.3/oauthlogin/migrations/0001_initial.py
--rw-r--r--   0        0        0      568 2023-01-31 17:18:07.510378 django_oauth_login-0.2.3/oauthlogin/migrations/0002_alter_oauthconnection_options_and_more.py
--rw-r--r--   0        0        0        0 2023-01-31 17:18:07.510378 django_oauth_login-0.2.3/oauthlogin/migrations/__init__.py
--rw-r--r--   0        0        0     6391 2023-01-31 17:18:07.510378 django_oauth_login-0.2.3/oauthlogin/models.py
--rw-r--r--   0        0        0     7739 2023-01-31 17:18:07.510378 django_oauth_login-0.2.3/oauthlogin/providers.py
--rw-r--r--   0        0        0      108 2023-01-31 17:18:07.510378 django_oauth_login-0.2.3/oauthlogin/templates/oauthlogin/error.html
--rw-r--r--   0        0        0      713 2023-01-31 17:18:07.510378 django_oauth_login-0.2.3/oauthlogin/urls.py
--rw-r--r--   0        0        0     2431 2023-01-31 17:18:07.510378 django_oauth_login-0.2.3/oauthlogin/views.py
--rw-r--r--   0        0        0     1405 2023-01-31 17:18:07.514378 django_oauth_login-0.2.3/pyproject.toml
--rw-r--r--   0        0        0    11061 1970-01-01 00:00:00.000000 django_oauth_login-0.2.3/setup.py
--rw-r--r--   0        0        0    11360 1970-01-01 00:00:00.000000 django_oauth_login-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-08-04 16:11:06.527853 django_oauth_login-0.2.4/LICENSE
+-rw-r--r--   0        0        0    10098 2023-08-04 16:11:06.527853 django_oauth_login-0.2.4/README.md
+-rw-r--r--   0        0        0        0 2023-08-04 16:11:06.527853 django_oauth_login-0.2.4/oauthlogin/__init__.py
+-rw-r--r--   0        0        0      344 2023-08-04 16:11:06.531853 django_oauth_login-0.2.4/oauthlogin/admin.py
+-rw-r--r--   0        0        0      152 2023-08-04 16:11:06.531853 django_oauth_login-0.2.4/oauthlogin/apps.py
+-rw-r--r--   0        0        0      246 2023-08-04 16:11:06.531853 django_oauth_login-0.2.4/oauthlogin/exceptions.py
+-rw-r--r--   0        0        0     1986 2023-08-04 16:11:06.531853 django_oauth_login-0.2.4/oauthlogin/migrations/0001_initial.py
+-rw-r--r--   0        0        0      567 2023-08-04 16:11:06.531853 django_oauth_login-0.2.4/oauthlogin/migrations/0002_alter_oauthconnection_options_and_more.py
+-rw-r--r--   0        0        0      608 2023-08-04 16:11:06.531853 django_oauth_login-0.2.4/oauthlogin/migrations/0003_alter_oauthconnection_access_token_and_more.py
+-rw-r--r--   0        0        0        0 2023-08-04 16:11:06.531853 django_oauth_login-0.2.4/oauthlogin/migrations/__init__.py
+-rw-r--r--   0        0        0     6393 2023-08-04 16:11:06.531853 django_oauth_login-0.2.4/oauthlogin/models.py
+-rw-r--r--   0        0        0     7769 2023-08-04 16:11:06.531853 django_oauth_login-0.2.4/oauthlogin/providers.py
+-rw-r--r--   0        0        0      108 2023-08-04 16:11:06.531853 django_oauth_login-0.2.4/oauthlogin/templates/oauthlogin/error.html
+-rw-r--r--   0        0        0      713 2023-08-04 16:11:06.531853 django_oauth_login-0.2.4/oauthlogin/urls.py
+-rw-r--r--   0        0        0     2431 2023-08-04 16:11:06.531853 django_oauth_login-0.2.4/oauthlogin/views.py
+-rw-r--r--   0        0        0     1410 2023-08-04 16:11:06.531853 django_oauth_login-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0    11161 1970-01-01 00:00:00.000000 django_oauth_login-0.2.4/PKG-INFO
```

### Comparing `django_oauth_login-0.2.3/LICENSE` & `django_oauth_login-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django_oauth_login-0.2.3/README.md` & `django_oauth_login-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `django_oauth_login-0.2.3/oauthlogin/migrations/0001_initial.py` & `django_oauth_login-0.2.4/oauthlogin/migrations/0001_initial.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import django.db.models.deletion
 from django.conf import settings
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     initial = True
 
     dependencies = [
         migrations.swappable_dependency(settings.AUTH_USER_MODEL),
     ]
 
     operations = [
```

### Comparing `django_oauth_login-0.2.3/oauthlogin/migrations/0002_alter_oauthconnection_options_and_more.py` & `django_oauth_login-0.2.4/oauthlogin/migrations/0002_alter_oauthconnection_options_and_more.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 4.0.3 on 2022-03-18 18:24
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("oauthlogin", "0001_initial"),
     ]
 
     operations = [
         migrations.AlterModelOptions(
             name="oauthconnection",
```

### Comparing `django_oauth_login-0.2.3/oauthlogin/models.py` & `django_oauth_login-0.2.4/oauthlogin/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,16 +29,16 @@
     # The key used to refer to this provider type (in settings)
     provider_key = models.CharField(max_length=100, db_index=True)
 
     # The unique ID of the user on the provider's system
     provider_user_id = models.CharField(max_length=100, db_index=True)
 
     # Token data
-    access_token = models.CharField(max_length=100)
-    refresh_token = models.CharField(max_length=100, blank=True)
+    access_token = models.CharField(max_length=2000)
+    refresh_token = models.CharField(max_length=2000, blank=True)
     access_token_expires_at = models.DateTimeField(blank=True, null=True)
     refresh_token_expires_at = models.DateTimeField(blank=True, null=True)
 
     class Meta:
         unique_together = ("provider_key", "provider_user_id")
         ordering = ("provider_key",)
         verbose_name = "OAuth Connection"
```

### Comparing `django_oauth_login-0.2.3/oauthlogin/providers.py` & `django_oauth_login-0.2.4/oauthlogin/providers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import datetime
 import secrets
-from typing import Any, List
+from typing import Any, List, Optional
 from urllib.parse import urlencode
 
 from django.conf import settings
 from django.contrib.auth import login as auth_login
 from django.http import HttpRequest, HttpResponse, HttpResponseRedirect
 from django.urls import NoReverseMatch, reverse
 from django.utils.crypto import get_random_string
@@ -19,16 +19,16 @@
 
 class OAuthToken:
     def __init__(
         self,
         *,
         access_token: str,
         refresh_token: str = "",
-        access_token_expires_at: datetime.datetime = None,
-        refresh_token_expires_at: datetime.datetime = None,
+        access_token_expires_at: Optional[datetime.datetime] = None,
+        refresh_token_expires_at: Optional[datetime.datetime] = None,
     ):
         self.access_token = access_token
         self.refresh_token = refresh_token
         self.access_token_expires_at = access_token_expires_at
         self.refresh_token_expires_at = refresh_token_expires_at
```

### Comparing `django_oauth_login-0.2.3/oauthlogin/urls.py` & `django_oauth_login-0.2.4/oauthlogin/urls.py`

 * *Files identical despite different names*

### Comparing `django_oauth_login-0.2.3/oauthlogin/views.py` & `django_oauth_login-0.2.4/oauthlogin/views.py`

 * *Files identical despite different names*

### Comparing `django_oauth_login-0.2.3/pyproject.toml` & `django_oauth_login-0.2.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-oauth-login"
-version = "0.2.3"
+version = "0.2.4"
 description = ""
 authors = ["Dave Gaeddert <dave.gaeddert@dropseed.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/dropseed/django-oauth-login"
 documentation = "https://github.com/dropseed/django-oauth-login"
 repository = "https://github.com/dropseed/django-oauth-login"
@@ -31,21 +31,21 @@
 python_files = "tests.py test_*.py *_tests.py"
 DJANGO_SETTINGS_MODULE = "tests.settings"
 FAIL_INVALID_TEMPLATE_VARS = true
 
 [tool.poetry.dependencies]
 python = "^3.8"
 
-[tool.poetry.dev-dependencies]
-black = "^22.1.0"
+[tool.poetry.group.dev.dependencies]
+black = "^23.7.0"
 Django = "^4.0.0"
 pytest = "^7.1.0"
 pytest-django = "^4.5.2"
 ipdb = "^0.13.9"
 requests = "^2.27.1"
 mypy = "*"
 isort = "^5.10.1"
-python-dotenv = "^0.20.0"
+python-dotenv = "^1.0.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `django_oauth_login-0.2.3/setup.py` & `django_oauth_login-0.2.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,329 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: django-oauth-login
+Version: 0.2.4
+Summary: 
+Home-page: https://github.com/dropseed/django-oauth-login
+License: MIT
+Author: Dave Gaeddert
+Author-email: dave.gaeddert@dropseed.dev
+Requires-Python: >=3.8,<4.0
+Classifier: Environment :: Web Environment
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 3
+Classifier: Framework :: Django :: 4
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Project-URL: Documentation, https://github.com/dropseed/django-oauth-login
+Project-URL: Repository, https://github.com/dropseed/django-oauth-login
+Description-Content-Type: text/markdown
 
-packages = \
-['oauthlogin', 'oauthlogin.migrations']
+# django-oauth-login
 
-package_data = \
-{'': ['*'], 'oauthlogin': ['templates/oauthlogin/*']}
+**Add OAuth login support to your Django project.**
 
-setup_kwargs = {
-    'name': 'django-oauth-login',
-    'version': '0.2.3',
-    'description': '',
-    'long_description': '# django-oauth-login\n\n**Add OAuth login support to your Django project.**\n\n[Watch on YouTube (3 mins) →](https://youtu.be/UxbxBa6AFsU)\n\nThis library is intentionally minimal.\nIt has no dependencies and a single database model.\nIf you simply want users to log in with GitHub, Google, Twitter, etc. (and maybe use that access token for API calls),\nthen this is the library for you.\n\nThere are three OAuth flows that it makes possible:\n\n1. Signup via OAuth (new user, new OAuth connection)\n2. Login via OAuth (existing user, existing OAuth connection)\n3. Connect/disconnect OAuth accounts to a user (existing user, new OAuth connection)\n\n\n## Usage\n\nInstall the package from PyPi:\n\n```sh\npip install django-oauth-login\n```\n\nAdd `oauthlogin` to your `INSTALLED_APPS` in `settings.py`:\n\n```python\nINSTALLED_APPS = [\n    ...\n    "oauthlogin",\n]\n```\n\nIn your `urls.py`, include `oauthlogin.urls`:\n\n```python\nurlpatterns = [\n    path("oauth/", include("oauthlogin.urls")),\n    ...\n]\n```\n\nThen run migrations:\n\n```sh\npython manage.py migrate oauthlogin\n```\n\nCreate a new OAuth provider ([or copy one from our examples](provider_examples)):\n\n```python\n# yourapp/oauth.py\nimport requests\n\nfrom oauthlogin.providers import OAuthProvider, OAuthToken, OAuthUser\n\n\nclass ExampleOAuthProvider(OAuthProvider):\n    authorization_url = "https://example.com/login/oauth/authorize"\n\n    def get_oauth_token(self, *, code, request):\n        response = requests.post(\n            "https://example.com/login/oauth/token",\n            headers={\n                "Accept": "application/json",\n            },\n            data={\n                "client_id": self.get_client_id(),\n                "client_secret": self.get_client_secret(),\n                "code": code,\n            },\n        )\n        response.raise_for_status()\n        data = response.json()\n        return OAuthToken(\n            access_token=data["access_token"],\n        )\n\n    def get_oauth_user(self, *, oauth_token):\n        response = requests.get(\n            "https://example.com/api/user",\n            headers={\n                "Accept": "application/json",\n                "Authorization": f"token {oauth_token.access_token}",\n            },\n        )\n        response.raise_for_status()\n        data = response.json()\n        return OAuthUser(\n            id=data["id"],\n            username=data["username"],\n            email=data["email"],\n        )\n```\n\nCreate your OAuth app/consumer on the provider\'s site (GitHub, Google, etc.).\nWhen setting it up, you\'ll likely need to give it a callback URL.\nIn development this can be `http://localhost:8000/oauth/github/callback/` (if you name it `"github"` like in the example below).\nAt the end you should get some sort of "client id" and "client secret" which you can then use in your `settings.py`:\n\n```python\nOAUTH_LOGIN_PROVIDERS = {\n    "github": {\n        "class": "yourapp.oauth.GitHubOAuthProvider",\n        "kwargs": {\n            "client_id": environ["GITHUB_CLIENT_ID"],\n            "client_secret": environ["GITHUB_CLIENT_SECRET"],\n            # "scope" is optional, defaults to ""\n\n            # You can add other fields if you have additional kwargs in your class __init__\n            # def __init__(self, *args, custom_arg="default", **kwargs):\n            #     self.custom_arg = custom_arg\n            #     super().__init__(*args, **kwargs)\n        },\n    },\n}\n```\n\nThen add a login button (which is a form using POST rather than a basic link, for security purposes):\n\n```html\n<h1>Login</h1>\n<form action="{% url \'oauthlogin:login\' \'github\' %}" method="post">\n    {% csrf_token %}\n    <button type="submit">Login with GitHub</button>\n</form>\n```\n\nThat\'s pretty much it!\n\n## Advanced usage\n\n### Email addresses should be unique\n\nWhen you\'re integrating with an OAuth provider,\nwe think that the user\'s email address is the best "primary key" when linking to your `User` model in your app.\nUnfortunately in Django, by default an email address is not required to be unique!\n**We strongly recommend you require email addresses to be unique in your app.**\n\n[As suggested by the Django docs](https://docs.djangoproject.com/en/4.0/topics/auth/customizing/#using-a-custom-user-model-when-starting-a-project),\none way to do this is to have your own `User` model:\n\n```python\n# In an app named "users", for example\nfrom django.contrib.auth.models import AbstractUser\n\nclass User(AbstractUser):\n    email = models.EmailField(unique=True)\n\n\n# In settings.py\nAUTH_USER_MODEL = \'users.User\'\n```\n\nYou\'ll also notice that there are no "email confirmation" or "email verification" flows in this library.\nThis is also intentional.\nYou can implement something like that yourself if you need to,\nbut the easier solution in our opinion is to use an OAuth provider you *trust to have done that already*.\nIf you look at our [provider examples](provider_examples) you\'ll notice how we often use provider APIs to get the email address which is "primary" and "verified" already.\nIf they\'ve already done that work,\nthen we can just use that information.\n\n### Handling OAuth errors\n\nThe most common error you\'ll run into is if an existing user clicks a login button,\nbut they haven\'t yet connected that provider to their account.\nFor security reasons,\nthe required flow here is that the user actually logs in with another method (however they signed up) and then *connects* the OAuth provider from a settings page.\n\nFor this error (and a couple others),\nthere is an error template that is rendered.\nYou can customize this by copying `oauthlogin/error.html` to one of your own template directories:\n\n```html\n{% extends "base.html" %}\n\n{% block content %}\n<h1>OAuth Error</h1>\n<p>{{ oauth_error }}</p>\n{% endblock %}\n```\n\n![Django OAuth duplicate email address error](https://user-images.githubusercontent.com/649496/159065848-b4ee6e63-9aa0-47b5-94e8-7bee9b509e60.png)\n\n### Connecting and disconnecting OAuth accounts\n\nTo connect and disconnect OAuth accounts,\nyou can add a series of forms to a user/profile settings page.\nHere\'s an very basic example:\n\n```html\n{% extends "base.html" %}\n\n{% block content %}\nHello {{ request.user }}!\n\n<h2>Existing connections</h2>\n<ul>\n    {% for connection in request.user.oauth_connections.all %}\n    <li>\n        {{ connection.provider_key }} [ID: {{ connection.provider_user_id }}]\n        {% if connection.can_be_disconnected %}\n        <form action="{% url \'oauthlogin:disconnect\' connection.provider_key %}" method="post">\n            {% csrf_token %}\n            <input type="hidden" name="provider_user_id" value="{{ connection.provider_user_id }}">\n            <button type="submit">Disconnect</button>\n        </form>\n        {% endif %}\n    </li>\n    {% endfor %}\n</ul>\n\n<h2>Add a connection</h2>\n<ul>\n    {% for provider_key in oauth_provider_keys %}\n    <li>\n        {{ provider_key}}\n        <form action="{% url \'oauthlogin:connect\' provider_key %}" method="post">\n            {% csrf_token %}\n            <button type="submit">Connect</button>\n        </form>\n    </li>\n    {% endfor %}\n</ul>\n\n{% endblock %}\n```\n\n![Connecting and disconnecting Django OAuth accounts](https://user-images.githubusercontent.com/649496/159065096-30239a1f-62f6-4ee2-a944-45140f45af6f.png)\n\n### Using a saved access token\n\n```python\nimport requests\n\n# Get the OAuth connection for a user\nconnection = user.oauth_connections.get(provider_key="github")\n\n# If the token can expire, check and refresh it\nif connection.access_token_expired():\n    connection.refresh_access_token()\n\n# Use the token in an API call\ntoken = connection.oauth_token\nresponse = requests.get(...)\n```\n\n### Using the Django system check\n\nThis library comes with a Django system check to ensure you don\'t *remove* a provider from `settings.py` that is still in use in your database.\nYou do need to specify the `--database` for this to run when using the check command by itself:\n\n```sh\npython manage.py check --database default\n```\n\n## FAQs\n\n### How is this different from [other Django OAuth libraries](https://djangopackages.org/grids/g/oauth/)?\n\nThe short answer is that *it does less*.\n\nIn [django-allauth](https://github.com/pennersr/django-allauth)\n(maybe the most popular alternative)\nyou get all kinds of other features like managing multiple email addresses,\nemail verification,\na long list of supported providers,\nand a whole suite of forms/urls/views/templates/signals/tags.\nAnd in my experience,\nit\'s too much.\nIt often adds more complexity to your app than you actually need (or want) and honestly it can just be a lot to wrap your head around.\nPersonally, I don\'t like the way that your OAuth settings are stored in the database vs when you use `settings.py`,\nand the implications for doing it one way or another.\n\nThe other popular OAuth libraries have similar issues,\nand I think their *weight* outweighs their usefulness for 80% of the use cases.\n\n### Why aren\'t providers included in the library itself?\n\nOne thing you\'ll notice is that we don\'t have a long list of pre-configured providers in this library.\nInstead, we have some examples (which you can usually just copy, paste, and use) and otherwise encourage you to wire up the provider yourself.\nOften times all this means is finding the two OAuth URLs ("oauth/authorize" and "oauth/token") in their docs,\nand writing two class methods that do the actual work of getting the user\'s data (which is often customized anyway).\n\nWe\'ve written examples for the following providers:\n\n- [GitHub](provider_examples/github.py)\n- [GitLab](provider_examples/gitlab.py)\n- [Bitbucket](provider_examples/bitbucket.py)\n\nJust copy that code and paste it in your project.\nTweak as necessary!\n\nThis might sound strange at first.\nBut in the long run we think it\'s actually *much* more maintainable for both us (as library authors) and you (as app author).\nIf something breaks with a provider, you can fix it immediately!\nYou don\'t need to try to run changes through us or wait for an upstream update.\nYou\'re welcome to contribute an example to this repo,\nand there won\'t be an expectation that it "works perfectly for every use case until the end of time".\n',
-    'author': 'Dave Gaeddert',
-    'author_email': 'dave.gaeddert@dropseed.dev',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/dropseed/django-oauth-login',
-    'packages': packages,
-    'package_data': package_data,
-    'python_requires': '>=3.8,<4.0',
+[Watch on YouTube (3 mins) →](https://youtu.be/UxbxBa6AFsU)
+
+This library is intentionally minimal.
+It has no dependencies and a single database model.
+If you simply want users to log in with GitHub, Google, Twitter, etc. (and maybe use that access token for API calls),
+then this is the library for you.
+
+There are three OAuth flows that it makes possible:
+
+1. Signup via OAuth (new user, new OAuth connection)
+2. Login via OAuth (existing user, existing OAuth connection)
+3. Connect/disconnect OAuth accounts to a user (existing user, new OAuth connection)
+
+
+## Usage
+
+Install the package from PyPi:
+
+```sh
+pip install django-oauth-login
+```
+
+Add `oauthlogin` to your `INSTALLED_APPS` in `settings.py`:
+
+```python
+INSTALLED_APPS = [
+    ...
+    "oauthlogin",
+]
+```
+
+In your `urls.py`, include `oauthlogin.urls`:
+
+```python
+urlpatterns = [
+    path("oauth/", include("oauthlogin.urls")),
+    ...
+]
+```
+
+Then run migrations:
+
+```sh
+python manage.py migrate oauthlogin
+```
+
+Create a new OAuth provider ([or copy one from our examples](provider_examples)):
+
+```python
+# yourapp/oauth.py
+import requests
+
+from oauthlogin.providers import OAuthProvider, OAuthToken, OAuthUser
+
+
+class ExampleOAuthProvider(OAuthProvider):
+    authorization_url = "https://example.com/login/oauth/authorize"
+
+    def get_oauth_token(self, *, code, request):
+        response = requests.post(
+            "https://example.com/login/oauth/token",
+            headers={
+                "Accept": "application/json",
+            },
+            data={
+                "client_id": self.get_client_id(),
+                "client_secret": self.get_client_secret(),
+                "code": code,
+            },
+        )
+        response.raise_for_status()
+        data = response.json()
+        return OAuthToken(
+            access_token=data["access_token"],
+        )
+
+    def get_oauth_user(self, *, oauth_token):
+        response = requests.get(
+            "https://example.com/api/user",
+            headers={
+                "Accept": "application/json",
+                "Authorization": f"token {oauth_token.access_token}",
+            },
+        )
+        response.raise_for_status()
+        data = response.json()
+        return OAuthUser(
+            id=data["id"],
+            username=data["username"],
+            email=data["email"],
+        )
+```
+
+Create your OAuth app/consumer on the provider's site (GitHub, Google, etc.).
+When setting it up, you'll likely need to give it a callback URL.
+In development this can be `http://localhost:8000/oauth/github/callback/` (if you name it `"github"` like in the example below).
+At the end you should get some sort of "client id" and "client secret" which you can then use in your `settings.py`:
+
+```python
+OAUTH_LOGIN_PROVIDERS = {
+    "github": {
+        "class": "yourapp.oauth.GitHubOAuthProvider",
+        "kwargs": {
+            "client_id": environ["GITHUB_CLIENT_ID"],
+            "client_secret": environ["GITHUB_CLIENT_SECRET"],
+            # "scope" is optional, defaults to ""
+
+            # You can add other fields if you have additional kwargs in your class __init__
+            # def __init__(self, *args, custom_arg="default", **kwargs):
+            #     self.custom_arg = custom_arg
+            #     super().__init__(*args, **kwargs)
+        },
+    },
 }
+```
+
+Then add a login button (which is a form using POST rather than a basic link, for security purposes):
+
+```html
+<h1>Login</h1>
+<form action="{% url 'oauthlogin:login' 'github' %}" method="post">
+    {% csrf_token %}
+    <button type="submit">Login with GitHub</button>
+</form>
+```
+
+That's pretty much it!
+
+## Advanced usage
+
+### Email addresses should be unique
+
+When you're integrating with an OAuth provider,
+we think that the user's email address is the best "primary key" when linking to your `User` model in your app.
+Unfortunately in Django, by default an email address is not required to be unique!
+**We strongly recommend you require email addresses to be unique in your app.**
+
+[As suggested by the Django docs](https://docs.djangoproject.com/en/4.0/topics/auth/customizing/#using-a-custom-user-model-when-starting-a-project),
+one way to do this is to have your own `User` model:
+
+```python
+# In an app named "users", for example
+from django.contrib.auth.models import AbstractUser
+
+class User(AbstractUser):
+    email = models.EmailField(unique=True)
+
+
+# In settings.py
+AUTH_USER_MODEL = 'users.User'
+```
+
+You'll also notice that there are no "email confirmation" or "email verification" flows in this library.
+This is also intentional.
+You can implement something like that yourself if you need to,
+but the easier solution in our opinion is to use an OAuth provider you *trust to have done that already*.
+If you look at our [provider examples](provider_examples) you'll notice how we often use provider APIs to get the email address which is "primary" and "verified" already.
+If they've already done that work,
+then we can just use that information.
+
+### Handling OAuth errors
+
+The most common error you'll run into is if an existing user clicks a login button,
+but they haven't yet connected that provider to their account.
+For security reasons,
+the required flow here is that the user actually logs in with another method (however they signed up) and then *connects* the OAuth provider from a settings page.
+
+For this error (and a couple others),
+there is an error template that is rendered.
+You can customize this by copying `oauthlogin/error.html` to one of your own template directories:
+
+```html
+{% extends "base.html" %}
+
+{% block content %}
+<h1>OAuth Error</h1>
+<p>{{ oauth_error }}</p>
+{% endblock %}
+```
+
+![Django OAuth duplicate email address error](https://user-images.githubusercontent.com/649496/159065848-b4ee6e63-9aa0-47b5-94e8-7bee9b509e60.png)
+
+### Connecting and disconnecting OAuth accounts
+
+To connect and disconnect OAuth accounts,
+you can add a series of forms to a user/profile settings page.
+Here's an very basic example:
+
+```html
+{% extends "base.html" %}
+
+{% block content %}
+Hello {{ request.user }}!
+
+<h2>Existing connections</h2>
+<ul>
+    {% for connection in request.user.oauth_connections.all %}
+    <li>
+        {{ connection.provider_key }} [ID: {{ connection.provider_user_id }}]
+        {% if connection.can_be_disconnected %}
+        <form action="{% url 'oauthlogin:disconnect' connection.provider_key %}" method="post">
+            {% csrf_token %}
+            <input type="hidden" name="provider_user_id" value="{{ connection.provider_user_id }}">
+            <button type="submit">Disconnect</button>
+        </form>
+        {% endif %}
+    </li>
+    {% endfor %}
+</ul>
+
+<h2>Add a connection</h2>
+<ul>
+    {% for provider_key in oauth_provider_keys %}
+    <li>
+        {{ provider_key}}
+        <form action="{% url 'oauthlogin:connect' provider_key %}" method="post">
+            {% csrf_token %}
+            <button type="submit">Connect</button>
+        </form>
+    </li>
+    {% endfor %}
+</ul>
+
+{% endblock %}
+```
+
+![Connecting and disconnecting Django OAuth accounts](https://user-images.githubusercontent.com/649496/159065096-30239a1f-62f6-4ee2-a944-45140f45af6f.png)
+
+### Using a saved access token
+
+```python
+import requests
+
+# Get the OAuth connection for a user
+connection = user.oauth_connections.get(provider_key="github")
+
+# If the token can expire, check and refresh it
+if connection.access_token_expired():
+    connection.refresh_access_token()
+
+# Use the token in an API call
+token = connection.oauth_token
+response = requests.get(...)
+```
+
+### Using the Django system check
+
+This library comes with a Django system check to ensure you don't *remove* a provider from `settings.py` that is still in use in your database.
+You do need to specify the `--database` for this to run when using the check command by itself:
+
+```sh
+python manage.py check --database default
+```
+
+## FAQs
+
+### How is this different from [other Django OAuth libraries](https://djangopackages.org/grids/g/oauth/)?
+
+The short answer is that *it does less*.
+
+In [django-allauth](https://github.com/pennersr/django-allauth)
+(maybe the most popular alternative)
+you get all kinds of other features like managing multiple email addresses,
+email verification,
+a long list of supported providers,
+and a whole suite of forms/urls/views/templates/signals/tags.
+And in my experience,
+it's too much.
+It often adds more complexity to your app than you actually need (or want) and honestly it can just be a lot to wrap your head around.
+Personally, I don't like the way that your OAuth settings are stored in the database vs when you use `settings.py`,
+and the implications for doing it one way or another.
+
+The other popular OAuth libraries have similar issues,
+and I think their *weight* outweighs their usefulness for 80% of the use cases.
+
+### Why aren't providers included in the library itself?
+
+One thing you'll notice is that we don't have a long list of pre-configured providers in this library.
+Instead, we have some examples (which you can usually just copy, paste, and use) and otherwise encourage you to wire up the provider yourself.
+Often times all this means is finding the two OAuth URLs ("oauth/authorize" and "oauth/token") in their docs,
+and writing two class methods that do the actual work of getting the user's data (which is often customized anyway).
+
+We've written examples for the following providers:
+
+- [GitHub](provider_examples/github.py)
+- [GitLab](provider_examples/gitlab.py)
+- [Bitbucket](provider_examples/bitbucket.py)
+
+Just copy that code and paste it in your project.
+Tweak as necessary!
 
+This might sound strange at first.
+But in the long run we think it's actually *much* more maintainable for both us (as library authors) and you (as app author).
+If something breaks with a provider, you can fix it immediately!
+You don't need to try to run changes through us or wait for an upstream update.
+You're welcome to contribute an example to this repo,
+and there won't be an expectation that it "works perfectly for every use case until the end of time".
 
-setup(**setup_kwargs)
```

