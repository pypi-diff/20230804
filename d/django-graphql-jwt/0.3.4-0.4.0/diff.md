# Comparing `tmp/django-graphql-jwt-0.3.4.tar.gz` & `tmp/django_graphql_jwt-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-graphql-jwt-0.3.4.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `django-graphql-jwt-0.3.4.tar` & `django_graphql_jwt-0.4.0.tar`

### file list

```diff
@@ -1,61 +1,64 @@
--rw-r--r--   0        0        0     1074 2021-08-11 20:58:19.091164 django-graphql-jwt-0.3.4/LICENSE
--rw-r--r--   0        0        0     2253 2021-08-11 20:58:19.091164 django-graphql-jwt-0.3.4/README.md
--rw-r--r--   0        0        0      406 2021-08-11 20:58:19.091164 django-graphql-jwt-0.3.4/graphql_jwt/__init__.py
--rw-r--r--   0        0        0      662 2021-08-11 20:58:19.091164 django-graphql-jwt-0.3.4/graphql_jwt/backends.py
--rw-r--r--   0        0        0      292 2021-08-11 20:58:19.091164 django-graphql-jwt-0.3.4/graphql_jwt/compat.py
--rw-r--r--   0        0        0     5838 2021-08-11 20:58:19.091164 django-graphql-jwt-0.3.4/graphql_jwt/decorators.py
--rw-r--r--   0        0        0      484 2021-08-11 20:58:19.091164 django-graphql-jwt-0.3.4/graphql_jwt/exceptions.py
--rw-r--r--   0        0        0     1191 2021-08-11 20:58:19.091164 django-graphql-jwt-0.3.4/graphql_jwt/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1570 2021-08-11 20:58:19.091164 django-graphql-jwt-0.3.4/graphql_jwt/locale/ar/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1039 2021-08-11 20:58:19.095165 django-graphql-jwt-0.3.4/graphql_jwt/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1413 2021-08-11 20:58:19.095165 django-graphql-jwt-0.3.4/graphql_jwt/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1078 2021-08-11 20:58:19.095165 django-graphql-jwt-0.3.4/graphql_jwt/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1453 2021-08-11 20:58:19.095165 django-graphql-jwt-0.3.4/graphql_jwt/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1043 2021-08-11 20:58:19.095165 django-graphql-jwt-0.3.4/graphql_jwt/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1303 2021-08-11 20:58:19.095165 django-graphql-jwt-0.3.4/graphql_jwt/locale/nl/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1069 2021-08-11 20:58:19.095165 django-graphql-jwt-0.3.4/graphql_jwt/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1443 2021-08-11 20:58:19.095165 django-graphql-jwt-0.3.4/graphql_jwt/locale/pt_BR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1402 2021-08-11 20:58:19.095165 django-graphql-jwt-0.3.4/graphql_jwt/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2570 2021-08-11 20:58:19.095165 django-graphql-jwt-0.3.4/graphql_jwt/middleware.py
--rw-r--r--   0        0        0     3537 2021-08-11 20:58:19.095165 django-graphql-jwt-0.3.4/graphql_jwt/mixins.py
--rw-r--r--   0        0        0     1652 2021-08-11 20:58:19.095165 django-graphql-jwt-0.3.4/graphql_jwt/mutations.py
--rw-r--r--   0        0        0      651 2021-08-11 20:58:19.095165 django-graphql-jwt-0.3.4/graphql_jwt/path.py
--rw-r--r--   0        0        0        0 2021-08-11 20:58:19.095165 django-graphql-jwt-0.3.4/graphql_jwt/refresh_token/__init__.py
--rw-r--r--   0        0        0      787 2021-08-11 20:58:19.095165 django-graphql-jwt-0.3.4/graphql_jwt/refresh_token/admin/__init__.py
--rw-r--r--   0        0        0      993 2021-08-11 20:58:19.095165 django-graphql-jwt-0.3.4/graphql_jwt/refresh_token/admin/filters.py
--rw-r--r--   0        0        0      205 2021-08-11 20:58:19.095165 django-graphql-jwt-0.3.4/graphql_jwt/refresh_token/apps.py
--rw-r--r--   0        0        0      666 2021-08-11 20:58:19.095165 django-graphql-jwt-0.3.4/graphql_jwt/refresh_token/decorators.py
--rw-r--r--   0        0        0     1119 2021-08-11 20:58:19.095165 django-graphql-jwt-0.3.4/graphql_jwt/refresh_token/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1742 2021-08-11 20:58:19.095165 django-graphql-jwt-0.3.4/graphql_jwt/refresh_token/locale/ar/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1051 2021-08-11 20:58:19.095165 django-graphql-jwt-0.3.4/graphql_jwt/refresh_token/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1603 2021-08-11 20:58:19.095165 django-graphql-jwt-0.3.4/graphql_jwt/refresh_token/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1135 2021-08-11 20:58:19.095165 django-graphql-jwt-0.3.4/graphql_jwt/refresh_token/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1658 2021-08-11 20:58:19.095165 django-graphql-jwt-0.3.4/graphql_jwt/refresh_token/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1102 2021-08-11 20:58:19.095165 django-graphql-jwt-0.3.4/graphql_jwt/refresh_token/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1504 2021-08-11 20:58:19.095165 django-graphql-jwt-0.3.4/graphql_jwt/refresh_token/locale/nl/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1144 2021-08-11 20:58:19.095165 django-graphql-jwt-0.3.4/graphql_jwt/refresh_token/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1847 2021-08-11 20:58:19.095165 django-graphql-jwt-0.3.4/graphql_jwt/refresh_token/locale/pt_BR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1660 2021-08-11 20:58:19.095165 django-graphql-jwt-0.3.4/graphql_jwt/refresh_token/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2021-08-11 20:58:19.095165 django-graphql-jwt-0.3.4/graphql_jwt/refresh_token/management/__init__.py
--rw-r--r--   0        0        0        0 2021-08-11 20:58:19.095165 django-graphql-jwt-0.3.4/graphql_jwt/refresh_token/management/commands/__init__.py
--rw-r--r--   0        0        0      824 2021-08-11 20:58:19.095165 django-graphql-jwt-0.3.4/graphql_jwt/refresh_token/management/commands/cleartokens.py
--rw-r--r--   0        0        0      579 2021-08-11 20:58:19.095165 django-graphql-jwt-0.3.4/graphql_jwt/refresh_token/managers.py
--rw-r--r--   0        0        0     1707 2021-08-11 20:58:19.095165 django-graphql-jwt-0.3.4/graphql_jwt/refresh_token/migrations/0001_initial.py
--rw-r--r--   0        0        0      395 2021-08-11 20:58:19.095165 django-graphql-jwt-0.3.4/graphql_jwt/refresh_token/migrations/0002_auto_20190130_0900.py
--rw-r--r--   0        0        0        0 2021-08-11 20:58:19.095165 django-graphql-jwt-0.3.4/graphql_jwt/refresh_token/migrations/__init__.py
--rw-r--r--   0        0        0     2868 2021-08-11 20:58:19.095165 django-graphql-jwt-0.3.4/graphql_jwt/refresh_token/mixins.py
--rw-r--r--   0        0        0     2172 2021-08-11 20:58:19.095165 django-graphql-jwt-0.3.4/graphql_jwt/refresh_token/models.py
--rw-r--r--   0        0        0      451 2021-08-11 20:58:19.095165 django-graphql-jwt-0.3.4/graphql_jwt/refresh_token/mutations.py
--rw-r--r--   0        0        0      506 2021-08-11 20:58:19.095165 django-graphql-jwt-0.3.4/graphql_jwt/refresh_token/relay.py
--rw-r--r--   0        0        0      990 2021-08-11 20:58:19.095165 django-graphql-jwt-0.3.4/graphql_jwt/refresh_token/shortcuts.py
--rw-r--r--   0        0        0      219 2021-08-11 20:58:19.095165 django-graphql-jwt-0.3.4/graphql_jwt/refresh_token/signals.py
--rw-r--r--   0        0        0      317 2021-08-11 20:58:19.095165 django-graphql-jwt-0.3.4/graphql_jwt/refresh_token/utils.py
--rw-r--r--   0        0        0     1868 2021-08-11 20:58:19.095165 django-graphql-jwt-0.3.4/graphql_jwt/relay.py
--rw-r--r--   0        0        0     4277 2021-08-11 20:58:19.095165 django-graphql-jwt-0.3.4/graphql_jwt/settings.py
--rw-r--r--   0        0        0      597 2021-08-11 20:58:19.095165 django-graphql-jwt-0.3.4/graphql_jwt/shortcuts.py
--rw-r--r--   0        0        0      162 2021-08-11 20:58:19.095165 django-graphql-jwt-0.3.4/graphql_jwt/signals.py
--rw-r--r--   0        0        0     1949 2021-08-11 20:58:19.095165 django-graphql-jwt-0.3.4/graphql_jwt/testcases.py
--rw-r--r--   0        0        0     4130 2021-08-11 20:58:19.095165 django-graphql-jwt-0.3.4/graphql_jwt/utils.py
--rw-r--r--   0        0        0     2329 2021-08-11 20:58:19.095165 django-graphql-jwt-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     3876 2021-08-11 20:58:29.596688 django-graphql-jwt-0.3.4/setup.py
--rw-r--r--   0        0        0     4070 2021-08-11 20:58:29.597083 django-graphql-jwt-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 django_graphql_jwt-0.4.0/graphql_jwt/__init__.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 django_graphql_jwt-0.4.0/graphql_jwt/_compat.py
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 django_graphql_jwt-0.4.0/graphql_jwt/backends.py
+-rw-r--r--   0        0        0     5825 2020-02-02 00:00:00.000000 django_graphql_jwt-0.4.0/graphql_jwt/decorators.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 django_graphql_jwt-0.4.0/graphql_jwt/exceptions.py
+-rw-r--r--   0        0        0     2500 2020-02-02 00:00:00.000000 django_graphql_jwt-0.4.0/graphql_jwt/middleware.py
+-rw-r--r--   0        0        0     3537 2020-02-02 00:00:00.000000 django_graphql_jwt-0.4.0/graphql_jwt/mixins.py
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 django_graphql_jwt-0.4.0/graphql_jwt/mutations.py
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 django_graphql_jwt-0.4.0/graphql_jwt/path.py
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 django_graphql_jwt-0.4.0/graphql_jwt/relay.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 django_graphql_jwt-0.4.0/graphql_jwt/settings.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 django_graphql_jwt-0.4.0/graphql_jwt/shortcuts.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 django_graphql_jwt-0.4.0/graphql_jwt/signals.py
+-rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 django_graphql_jwt-0.4.0/graphql_jwt/testcases.py
+-rw-r--r--   0        0        0     4130 2020-02-02 00:00:00.000000 django_graphql_jwt-0.4.0/graphql_jwt/utils.py
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 django_graphql_jwt-0.4.0/graphql_jwt/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 django_graphql_jwt-0.4.0/graphql_jwt/locale/ar/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 django_graphql_jwt-0.4.0/graphql_jwt/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 django_graphql_jwt-0.4.0/graphql_jwt/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 django_graphql_jwt-0.4.0/graphql_jwt/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 django_graphql_jwt-0.4.0/graphql_jwt/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 django_graphql_jwt-0.4.0/graphql_jwt/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 django_graphql_jwt-0.4.0/graphql_jwt/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 django_graphql_jwt-0.4.0/graphql_jwt/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 django_graphql_jwt-0.4.0/graphql_jwt/locale/nl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 django_graphql_jwt-0.4.0/graphql_jwt/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 django_graphql_jwt-0.4.0/graphql_jwt/locale/pt_BR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 django_graphql_jwt-0.4.0/graphql_jwt/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_graphql_jwt-0.4.0/graphql_jwt/refresh_token/__init__.py
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 django_graphql_jwt-0.4.0/graphql_jwt/refresh_token/apps.py
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 django_graphql_jwt-0.4.0/graphql_jwt/refresh_token/decorators.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 django_graphql_jwt-0.4.0/graphql_jwt/refresh_token/managers.py
+-rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 django_graphql_jwt-0.4.0/graphql_jwt/refresh_token/mixins.py
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 django_graphql_jwt-0.4.0/graphql_jwt/refresh_token/models.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 django_graphql_jwt-0.4.0/graphql_jwt/refresh_token/mutations.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 django_graphql_jwt-0.4.0/graphql_jwt/refresh_token/relay.py
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 django_graphql_jwt-0.4.0/graphql_jwt/refresh_token/shortcuts.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 django_graphql_jwt-0.4.0/graphql_jwt/refresh_token/signals.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 django_graphql_jwt-0.4.0/graphql_jwt/refresh_token/utils.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 django_graphql_jwt-0.4.0/graphql_jwt/refresh_token/admin/__init__.py
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 django_graphql_jwt-0.4.0/graphql_jwt/refresh_token/admin/filters.py
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 django_graphql_jwt-0.4.0/graphql_jwt/refresh_token/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 django_graphql_jwt-0.4.0/graphql_jwt/refresh_token/locale/ar/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 django_graphql_jwt-0.4.0/graphql_jwt/refresh_token/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 django_graphql_jwt-0.4.0/graphql_jwt/refresh_token/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 django_graphql_jwt-0.4.0/graphql_jwt/refresh_token/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 django_graphql_jwt-0.4.0/graphql_jwt/refresh_token/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 django_graphql_jwt-0.4.0/graphql_jwt/refresh_token/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 django_graphql_jwt-0.4.0/graphql_jwt/refresh_token/locale/nl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 django_graphql_jwt-0.4.0/graphql_jwt/refresh_token/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 django_graphql_jwt-0.4.0/graphql_jwt/refresh_token/locale/pt_BR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 django_graphql_jwt-0.4.0/graphql_jwt/refresh_token/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_graphql_jwt-0.4.0/graphql_jwt/refresh_token/management/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_graphql_jwt-0.4.0/graphql_jwt/refresh_token/management/commands/__init__.py
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 django_graphql_jwt-0.4.0/graphql_jwt/refresh_token/management/commands/cleartokens.py
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 django_graphql_jwt-0.4.0/graphql_jwt/refresh_token/migrations/0001_initial.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 django_graphql_jwt-0.4.0/graphql_jwt/refresh_token/migrations/0002_auto_20190130_0900.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_graphql_jwt-0.4.0/graphql_jwt/refresh_token/migrations/__init__.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 django_graphql_jwt-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 django_graphql_jwt-0.4.0/AUTHORS.rst
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 django_graphql_jwt-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 django_graphql_jwt-0.4.0/README.md
+-rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 django_graphql_jwt-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4811 2020-02-02 00:00:00.000000 django_graphql_jwt-0.4.0/PKG-INFO
```

### Comparing `django-graphql-jwt-0.3.4/LICENSE` & `django_graphql_jwt-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-graphql-jwt-0.3.4/README.md` & `django_graphql_jwt-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `django-graphql-jwt-0.3.4/graphql_jwt/backends.py` & `django_graphql_jwt-0.4.0/graphql_jwt/backends.py`

 * *Files identical despite different names*

### Comparing `django-graphql-jwt-0.3.4/graphql_jwt/decorators.py` & `django_graphql_jwt-0.4.0/graphql_jwt/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 from datetime import datetime
 from functools import wraps
 
 from django.contrib.auth import authenticate, get_user_model
 from django.middleware.csrf import rotate_token
 from django.utils.translation import gettext as _
 
+from graphene import ResolveInfo
 from graphene.utils.thenables import maybe_thenable
 
 from . import exceptions, signals
-from .compat import GraphQLResolveInfo
 from .refresh_token.shortcuts import create_refresh_token, refresh_token_lazy
 from .settings import jwt_settings
 from .utils import delete_cookie, set_cookie
 
 __all__ = [
     "user_passes_test",
     "login_required",
@@ -27,15 +27,15 @@
     "ensure_token",
 ]
 
 
 def context(f):
     def decorator(func):
         def wrapper(*args, **kwargs):
-            info = next(arg for arg in args if isinstance(arg, GraphQLResolveInfo))
+            info = next(arg for arg in args if isinstance(arg, ResolveInfo))
             return func(info.context, *args, **kwargs)
 
         return wrapper
 
     return decorator
```

### Comparing `django-graphql-jwt-0.3.4/graphql_jwt/locale/ar/LC_MESSAGES/django.mo` & `django_graphql_jwt-0.4.0/graphql_jwt/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-graphql-jwt-0.3.4/graphql_jwt/locale/ar/LC_MESSAGES/django.po` & `django_graphql_jwt-0.4.0/graphql_jwt/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-graphql-jwt-0.3.4/graphql_jwt/locale/es/LC_MESSAGES/django.mo` & `django_graphql_jwt-0.4.0/graphql_jwt/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-graphql-jwt-0.3.4/graphql_jwt/locale/es/LC_MESSAGES/django.po` & `django_graphql_jwt-0.4.0/graphql_jwt/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-graphql-jwt-0.3.4/graphql_jwt/locale/fr/LC_MESSAGES/django.mo` & `django_graphql_jwt-0.4.0/graphql_jwt/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-graphql-jwt-0.3.4/graphql_jwt/locale/fr/LC_MESSAGES/django.po` & `django_graphql_jwt-0.4.0/graphql_jwt/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-graphql-jwt-0.3.4/graphql_jwt/locale/nl/LC_MESSAGES/django.mo` & `django_graphql_jwt-0.4.0/graphql_jwt/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-graphql-jwt-0.3.4/graphql_jwt/locale/nl/LC_MESSAGES/django.po` & `django_graphql_jwt-0.4.0/graphql_jwt/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-graphql-jwt-0.3.4/graphql_jwt/locale/pt_BR/LC_MESSAGES/django.mo` & `django_graphql_jwt-0.4.0/graphql_jwt/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-graphql-jwt-0.3.4/graphql_jwt/locale/pt_BR/LC_MESSAGES/django.po` & `django_graphql_jwt-0.4.0/graphql_jwt/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-graphql-jwt-0.3.4/graphql_jwt/locale/zh_Hans/LC_MESSAGES/django.po` & `django_graphql_jwt-0.4.0/graphql_jwt/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-graphql-jwt-0.3.4/graphql_jwt/middleware.py` & `django_graphql_jwt-0.4.0/graphql_jwt/middleware.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from django.contrib.auth import authenticate
 from django.contrib.auth.middleware import get_user
 from django.contrib.auth.models import AnonymousUser
 
-from .compat import get_operation_name
+from ._compat import get_root_type
 from .path import PathDict
 from .settings import jwt_settings
 from .utils import get_http_authorization, get_token_argument
 
 __all__ = [
     "allow_any",
     "JSONWebTokenMiddleware",
 ]
 
 
 def allow_any(info, **kwargs):
-    operation_name = get_operation_name(info.operation.operation).title()
-    field = info.schema.get_type(operation_name).fields.get(info.field_name)
+    root_type = get_root_type(info)
+    field = root_type.fields.get(info.field_name)
 
     if field is None:
         return False
 
     graphene_type = getattr(field.type, "graphene_type", None)
 
     return graphene_type is not None and issubclass(
@@ -65,15 +65,14 @@
                     self.cached_authentication.insert(info.path, context.user)
                 else:
                     context.user = AnonymousUser()
 
         if (
             _authenticate(context) or token_argument is not None
         ) and self.authenticate_context(info, **kwargs):
-
             user = authenticate(request=context, **kwargs)
 
             if user is not None:
                 context.user = user
 
                 if jwt_settings.JWT_ALLOW_ARGUMENT:
                     self.cached_authentication.insert(info.path, user)
```

### Comparing `django-graphql-jwt-0.3.4/graphql_jwt/mixins.py` & `django_graphql_jwt-0.4.0/graphql_jwt/mixins.py`

 * *Files identical despite different names*

### Comparing `django-graphql-jwt-0.3.4/graphql_jwt/mutations.py` & `django_graphql_jwt-0.4.0/graphql_jwt/mutations.py`

 * *Files identical despite different names*

### Comparing `django-graphql-jwt-0.3.4/graphql_jwt/path.py` & `django_graphql_jwt-0.4.0/graphql_jwt/path.py`

 * *Files identical despite different names*

### Comparing `django-graphql-jwt-0.3.4/graphql_jwt/refresh_token/admin/__init__.py` & `django_graphql_jwt-0.4.0/graphql_jwt/refresh_token/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `django-graphql-jwt-0.3.4/graphql_jwt/refresh_token/admin/filters.py` & `django_graphql_jwt-0.4.0/graphql_jwt/refresh_token/admin/filters.py`

 * *Files identical despite different names*

### Comparing `django-graphql-jwt-0.3.4/graphql_jwt/refresh_token/decorators.py` & `django_graphql_jwt-0.4.0/graphql_jwt/refresh_token/decorators.py`

 * *Files identical despite different names*

### Comparing `django-graphql-jwt-0.3.4/graphql_jwt/refresh_token/locale/ar/LC_MESSAGES/django.mo` & `django_graphql_jwt-0.4.0/graphql_jwt/refresh_token/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-graphql-jwt-0.3.4/graphql_jwt/refresh_token/locale/ar/LC_MESSAGES/django.po` & `django_graphql_jwt-0.4.0/graphql_jwt/refresh_token/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-graphql-jwt-0.3.4/graphql_jwt/refresh_token/locale/es/LC_MESSAGES/django.mo` & `django_graphql_jwt-0.4.0/graphql_jwt/refresh_token/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-graphql-jwt-0.3.4/graphql_jwt/refresh_token/locale/es/LC_MESSAGES/django.po` & `django_graphql_jwt-0.4.0/graphql_jwt/refresh_token/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-graphql-jwt-0.3.4/graphql_jwt/refresh_token/locale/fr/LC_MESSAGES/django.mo` & `django_graphql_jwt-0.4.0/graphql_jwt/refresh_token/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-graphql-jwt-0.3.4/graphql_jwt/refresh_token/locale/fr/LC_MESSAGES/django.po` & `django_graphql_jwt-0.4.0/graphql_jwt/refresh_token/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-graphql-jwt-0.3.4/graphql_jwt/refresh_token/locale/nl/LC_MESSAGES/django.mo` & `django_graphql_jwt-0.4.0/graphql_jwt/refresh_token/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-graphql-jwt-0.3.4/graphql_jwt/refresh_token/locale/nl/LC_MESSAGES/django.po` & `django_graphql_jwt-0.4.0/graphql_jwt/refresh_token/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-graphql-jwt-0.3.4/graphql_jwt/refresh_token/locale/pt_BR/LC_MESSAGES/django.mo` & `django_graphql_jwt-0.4.0/graphql_jwt/refresh_token/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-graphql-jwt-0.3.4/graphql_jwt/refresh_token/locale/pt_BR/LC_MESSAGES/django.po` & `django_graphql_jwt-0.4.0/graphql_jwt/refresh_token/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-graphql-jwt-0.3.4/graphql_jwt/refresh_token/locale/zh_Hans/LC_MESSAGES/django.po` & `django_graphql_jwt-0.4.0/graphql_jwt/refresh_token/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-graphql-jwt-0.3.4/graphql_jwt/refresh_token/management/commands/cleartokens.py` & `django_graphql_jwt-0.4.0/graphql_jwt/refresh_token/management/commands/cleartokens.py`

 * *Files identical despite different names*

### Comparing `django-graphql-jwt-0.3.4/graphql_jwt/refresh_token/managers.py` & `django_graphql_jwt-0.4.0/graphql_jwt/refresh_token/managers.py`

 * *Files identical despite different names*

### Comparing `django-graphql-jwt-0.3.4/graphql_jwt/refresh_token/migrations/0001_initial.py` & `django_graphql_jwt-0.4.0/graphql_jwt/refresh_token/migrations/0001_initial.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from django.conf import settings
 from django.db import migrations, models
 import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
-
     initial = True
 
     dependencies = [
         migrations.swappable_dependency(settings.AUTH_USER_MODEL),
     ]
 
     operations = [
```

### Comparing `django-graphql-jwt-0.3.4/graphql_jwt/refresh_token/mixins.py` & `django_graphql_jwt-0.4.0/graphql_jwt/refresh_token/mixins.py`

 * *Files identical despite different names*

### Comparing `django-graphql-jwt-0.3.4/graphql_jwt/refresh_token/models.py` & `django_graphql_jwt-0.4.0/graphql_jwt/refresh_token/models.py`

 * *Files identical despite different names*

### Comparing `django-graphql-jwt-0.3.4/graphql_jwt/refresh_token/shortcuts.py` & `django_graphql_jwt-0.4.0/graphql_jwt/refresh_token/shortcuts.py`

 * *Files identical despite different names*

### Comparing `django-graphql-jwt-0.3.4/graphql_jwt/relay.py` & `django_graphql_jwt-0.4.0/graphql_jwt/relay.py`

 * *Files identical despite different names*

### Comparing `django-graphql-jwt-0.3.4/graphql_jwt/settings.py` & `django_graphql_jwt-0.4.0/graphql_jwt/settings.py`

 * *Files identical despite different names*

### Comparing `django-graphql-jwt-0.3.4/graphql_jwt/shortcuts.py` & `django_graphql_jwt-0.4.0/graphql_jwt/shortcuts.py`

 * *Files identical despite different names*

### Comparing `django-graphql-jwt-0.3.4/graphql_jwt/testcases.py` & `django_graphql_jwt-0.4.0/graphql_jwt/testcases.py`

 * *Files identical despite different names*

### Comparing `django-graphql-jwt-0.3.4/graphql_jwt/utils.py` & `django_graphql_jwt-0.4.0/graphql_jwt/utils.py`

 * *Files identical despite different names*

### Comparing `django-graphql-jwt-0.3.4/pyproject.toml` & `django_graphql_jwt-0.4.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,22 @@
 [build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+requires = ["hatchling"]
+build-backend = "hatchling.build"
 
-[tool.poetry]
+[project]
 name = "django-graphql-jwt"
-version = "0.3.4"
 description = "JSON Web Token for Django GraphQL."
-license = "MIT"
-authors = ["mongkok <dani@domake.io>"]
 readme = "README.md"
-include = ["LICENSE", "README.md"]
-keywords = ["django", "graphql", "jwt"]
-
-homepage = "https://github.com/flavors/django-graphql-jwt"
-repository = "https://github.com/flavors/django-graphql-jwt"
-documentation = "https://django-graphql-jwt.domake.io"
-
-packages = [
-    { include = "graphql_jwt" },
+license = "MIT"
+requires-python = ">=3.6"
+dynamic = ["version"]
+authors = [
+  { name = "Dani", email = "dani@domake.io" }
 ]
+keywords = ["django", "graphql", "jwt"]
 
 classifiers = [
     "Intended Audience :: Information Technology",
     "Intended Audience :: System Administrators",
     "Operating System :: OS Independent",
     "License :: OSI Approved :: MIT License",
     "Development Status :: 4 - Beta",
@@ -30,48 +24,72 @@
     "Intended Audience :: Developers",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Framework :: Django",
     "Framework :: Django :: 2.0",
     "Framework :: Django :: 2.1",
     "Framework :: Django :: 2.2",
     "Framework :: Django :: 3.0",
     "Framework :: Django :: 3.1",
     "Framework :: Django :: 3.2",
+    "Framework :: Django :: 4.0",
+    "Framework :: Django :: 4.1",
+    "Framework :: Django :: 4.2",
     "Topic :: Security",
     "Topic :: Software Development",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Internet",
     "Topic :: Internet :: WWW/HTTP",
     "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
 ]
 
-[tool.poetry.dependencies]
-python = "^3.6"
+dependencies = [
+    "Django >=2.0",
+    "graphene >=2.1.5",
+    "graphene-django >=2.0.0",
+    "PyJWT >=2,<3",
+]
+
+[project.urls]
+homepage = "https://github.com/flavors/django-graphql-jwt"
+repository = "https://github.com/flavors/django-graphql-jwt"
+documentation = "https://django-graphql-jwt.domake.io"
+changelog = "https://django-graphql-jwt.domake.io/changelog"
+
+[project.optional-dependencies]
+test = [
+    "black",
+    "codecov",
+    "cryptography",
+    "flake8",
+    "isort",
+    "pytest",
+    "pytest-cov",
+    "pytest-django",
+]
+
+doc = [
+    "sphinx",
+]
+
+[tool.hatch.build.targets.sdist]
+include = ["graphql_jwt"]
+
+[tool.hatch.build.targets.wheel]
+packages = ["graphql_jwt"]
 
-Django = ">=2.0"
-graphene = ">=2.1.5"
-graphene-django = ">=2.0.0"
-PyJWT = ">=2,<3"
-
-[tool.poetry.dev-dependencies]
-black = "*"
-codecov = "*"
-cryptography = "2.8"
-flake8 = "*"
-isort = "*"
-pytest = "*"
-pytest-cov = "*"
-pytest-django = "*"
-sphinx = "*"
+[tool.hatch.version]
+path = "graphql_jwt/__init__.py"
 
 [tool.pytest.ini_options]
 DJANGO_SETTINGS_MODULE = "tests.settings"
 
 [tool.black]
 extend-exclude = '''
 /(
```

### Comparing `django-graphql-jwt-0.3.4/PKG-INFO` & `django_graphql_jwt-0.4.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,50 +1,68 @@
 Metadata-Version: 2.1
 Name: django-graphql-jwt
-Version: 0.3.4
+Version: 0.4.0
 Summary: JSON Web Token for Django GraphQL.
-Home-page: https://github.com/flavors/django-graphql-jwt
-License: MIT
+Project-URL: homepage, https://github.com/flavors/django-graphql-jwt
+Project-URL: repository, https://github.com/flavors/django-graphql-jwt
+Project-URL: documentation, https://django-graphql-jwt.domake.io
+Project-URL: changelog, https://django-graphql-jwt.domake.io/changelog
+Author-email: Dani <dani@domake.io>
+License-Expression: MIT
+License-File: AUTHORS.rst
+License-File: LICENSE
 Keywords: django,graphql,jwt
-Author: mongkok
-Author-email: dani@domake.io
-Requires-Python: >=3.6,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.0
 Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: Django (>=2.0)
-Requires-Dist: PyJWT (>=2,<3)
-Requires-Dist: graphene (>=2.1.5)
-Requires-Dist: graphene-django (>=2.0.0)
-Project-URL: Documentation, https://django-graphql-jwt.domake.io
-Project-URL: Repository, https://github.com/flavors/django-graphql-jwt
+Requires-Python: >=3.6
+Requires-Dist: django>=2.0
+Requires-Dist: graphene-django>=2.0.0
+Requires-Dist: graphene>=2.1.5
+Requires-Dist: pyjwt<3,>=2
+Provides-Extra: doc
+Requires-Dist: sphinx; extra == 'doc'
+Provides-Extra: test
+Requires-Dist: black; extra == 'test'
+Requires-Dist: codecov; extra == 'test'
+Requires-Dist: cryptography; extra == 'test'
+Requires-Dist: flake8; extra == 'test'
+Requires-Dist: isort; extra == 'test'
+Requires-Dist: pytest; extra == 'test'
+Requires-Dist: pytest-cov; extra == 'test'
+Requires-Dist: pytest-django; extra == 'test'
 Description-Content-Type: text/markdown
 
 <p align="center">
   <a href="https://django-graphql-jwt.domake.io/"><img width="420px" src="https://django-graphql-jwt.domake.io/_static/logo.png" alt='Django GraphQL JWT'></a>
 </p>
 
 <p align="center">
@@ -118,8 +136,7 @@
     token_auth = graphql_jwt.ObtainJSONWebToken.Field()
     verify_token = graphql_jwt.Verify.Field()
     refresh_token = graphql_jwt.Refresh.Field()
 
 
 schema = graphene.Schema(mutation=Mutation)
 ```
-
```

