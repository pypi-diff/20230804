# Comparing `tmp/django_custom_admin_pages-1.0.0.tar.gz` & `tmp/django_custom_admin_pages-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_custom_admin_pages-1.0.0.tar", max compression
+gzip compressed data, was "django_custom_admin_pages-1.1.0.tar", max compression
```

## Comparing `django_custom_admin_pages-1.0.0.tar` & `django_custom_admin_pages-1.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1496 2023-07-29 15:36:01.096792 django_custom_admin_pages-1.0.0/LICENSE
--rw-r--r--   0        0        0     6225 2023-08-02 03:54:28.456719 django_custom_admin_pages-1.0.0/README.md
--rw-r--r--   0        0        0        0 2023-07-30 21:00:31.363211 django_custom_admin_pages-1.0.0/django_custom_admin_pages/__init__.py
--rw-r--r--   0        0        0     5638 2023-07-30 21:00:31.363211 django_custom_admin_pages-1.0.0/django_custom_admin_pages/admin.py
--rw-r--r--   0        0        0      482 2023-07-30 21:00:31.363211 django_custom_admin_pages-1.0.0/django_custom_admin_pages/apps.py
--rw-r--r--   0        0        0       61 2023-07-30 21:00:31.363211 django_custom_admin_pages-1.0.0/django_custom_admin_pages/default_settings.py
--rw-r--r--   0        0        0      344 2023-07-30 22:17:55.133161 django_custom_admin_pages-1.0.0/django_custom_admin_pages/templates/base_custom_admin.html
--rw-r--r--   0        0        0      777 2023-07-30 21:00:31.363211 django_custom_admin_pages-1.0.0/django_custom_admin_pages/urls.py
--rw-r--r--   0        0        0       43 2023-07-30 21:00:31.363211 django_custom_admin_pages-1.0.0/django_custom_admin_pages/views/__init__.py
--rw-r--r--   0        0        0     2408 2023-07-30 21:00:31.363211 django_custom_admin_pages-1.0.0/django_custom_admin_pages/views/admin_base_view.py
--rw-r--r--   0        0        0     2333 2023-08-02 04:07:01.766715 django_custom_admin_pages-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     7912 1970-01-01 00:00:00.000000 django_custom_admin_pages-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1496 2023-07-29 15:36:01.096792 django_custom_admin_pages-1.1.0/LICENSE
+-rw-r--r--   0        0        0     6446 2023-08-04 01:44:19.722360 django_custom_admin_pages-1.1.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-30 21:00:31.363211 django_custom_admin_pages-1.1.0/django_custom_admin_pages/__init__.py
+-rw-r--r--   0        0        0     7024 2023-08-04 01:44:19.722360 django_custom_admin_pages-1.1.0/django_custom_admin_pages/admin.py
+-rw-r--r--   0        0        0      482 2023-07-30 21:00:31.363211 django_custom_admin_pages-1.1.0/django_custom_admin_pages/apps.py
+-rw-r--r--   0        0        0       61 2023-07-30 21:00:31.363211 django_custom_admin_pages-1.1.0/django_custom_admin_pages/default_settings.py
+-rw-r--r--   0        0        0      344 2023-07-30 22:17:55.133161 django_custom_admin_pages-1.1.0/django_custom_admin_pages/templates/base_custom_admin.html
+-rw-r--r--   0        0        0      777 2023-08-04 00:01:10.272365 django_custom_admin_pages-1.1.0/django_custom_admin_pages/urls.py
+-rw-r--r--   0        0        0       43 2023-07-30 21:00:31.363211 django_custom_admin_pages-1.1.0/django_custom_admin_pages/views/__init__.py
+-rw-r--r--   0        0        0     2408 2023-07-30 21:00:31.363211 django_custom_admin_pages-1.1.0/django_custom_admin_pages/views/admin_base_view.py
+-rw-r--r--   0        0        0     2333 2023-08-04 01:44:12.302360 django_custom_admin_pages-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     8133 1970-01-01 00:00:00.000000 django_custom_admin_pages-1.1.0/PKG-INFO
```

### Comparing `django_custom_admin_pages-1.0.0/LICENSE` & `django_custom_admin_pages-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_custom_admin_pages-1.0.0/README.md` & `django_custom_admin_pages-1.1.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-[![PyPI version](https://badge.fury.io/py/django-custom-admin-pages.svg)](https://badge.fury.io/py/django-custom-admin-pages)
+[![PyPI](https://img.shields.io/pypi/v/django-custom-admin-pages)](https://pypi.org/project/django-custom-admin-pages/)
+![Python Supported](https://img.shields.io/badge/Python-3.9,_3.10,_3.11-blue)
+![Django Supported](https://img.shields.io/badge/Django-3.2,_4.0,_4.1,_4.2-blue)
 [![Tests](https://github.com/lekjos/django-custom-admin-pages/actions/workflows/build_and_test.yml/badge.svg)](https://github.com/lekjos/django-custom-admin-pages/actions/workflows/build_and_test.yml)
 [![codecov](https://codecov.io/gh/lekjos/django-custom-admin-pages/branch/master/graph/badge.svg?token=AJG2WICKXA)](https://codecov.io/gh/lekjos/django-custom-admin-pages)
-![Python Versions](https://img.shields.io/badge/Python_Versions-3.9,_3.10,_3.11-blue)
-![Django Versions](https://img.shields.io/badge/Django_Versions-3.2,_4.0,_4.1,_4.2-blue)
+![PyPI - Downloads](https://img.shields.io/pypi/dw/django-custom-admin-pages)
 
 
 # Django Custom Admin Pages
 A django app that lets you add standard class-based views to the django admin index and navigation. Create a view, register it like you would a ModelAdmin, and it appears in the Django Admin Nav.
 
 
 ## Installation
@@ -20,19 +21,23 @@
    # "django.contrib.admin", #REMOVE THIS LINE
    # ...
    "django_custom_admin_pages",
    "django_custom_admin_pages.admin.CustomAdminConfig"
    # ...
 ]
 ```
-4. If you've defined a custom django admin site, you can also subclass `django_custom_admin_pages.admin.CustomAdminConfig`:
+4. If you've defined a custom django admin site, you can also subclass `django_custom_admin_pages.admin.CustomAdminConfig` and/or `django_custom_admin_pages.admin.CustomAdminSite`:
 
 ```python
-from django_custom_admin_pages.admin import CustomAdminConfig
-class MyCustomAdminSite(CustomAdminConfig):
+from django_custom_admin_pages.admin import CustomAdminConfig, CustomAdminSite
+
+class MyCustomAdminConfig(CustomAdminConfig):
+   default_site="path.to.MyCustomAdminSite"
+
+class MyCustomAdminSite(CustomAdminSite):
    pass
 ```
 
 ## Usage
 
 This app is for custom admin views which aren't associated with a specific model. Add dashboards and other custom admin views here.
 
@@ -159,8 +164,8 @@
    - `cd <repo_root>`
    - `poetry run pylint django_custom_admin_pages/`
 
 2. Run black:
    - `poetry run black .`
 
 2. Run isort:
-   - `poetry run isort django_custom_admin_pages/`
+   - `poetry run isort django_custom_admin_pages/`
```

### Comparing `django_custom_admin_pages-1.0.0/django_custom_admin_pages/admin.py` & `django_custom_admin_pages-1.1.0/django_custom_admin_pages/admin.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import contextlib
 from collections import namedtuple
 from collections.abc import Iterable
 from typing import TYPE_CHECKING, List, Type, Union
 
+from django.apps import apps
 from django.conf import settings
 from django.contrib import admin
 from django.contrib.admin.apps import AdminConfig
 from django.core.exceptions import ImproperlyConfigured
 from django.urls import include, path, reverse
 from django.views import View
 
@@ -15,14 +16,19 @@
 if TYPE_CHECKING:
     from .views.admin_base_view import AdminBaseView
 
 
 ViewRegister = namedtuple("ViewRegister", ["app_label", "view"])
 
 
+def get_installed_apps():
+    installed_apps = [app_config.name for app_config in apps.get_app_configs()]
+    return installed_apps
+
+
 def get_app_label(view: View) -> str:
     "returns app label or default app for view"
     return getattr(view, "app_label") or settings.CUSTOM_ADMIN_DEFAULT_APP_LABEL
 
 
 class CustomAdminConfig(AdminConfig):
     default_site = "django_custom_admin_pages.admin.CustomAdminSite"
@@ -91,26 +97,33 @@
                 )
 
             self._view_registry.append(view)
 
             add_view_to_conf(view)
 
     def unregister_view(self, view_or_iterable: Union[Iterable, Type]):
+        def _raise_not_registered(view, e=None):
+            msg = f"The view {view.__name__} is not registered"
+            if e:
+                raise admin.sites.NotRegistered(msg) from e
+            raise admin.sites.NotRegistered(msg)
+
         if not isinstance(view_or_iterable, Iterable):
             view_or_iterable = [view_or_iterable]
 
         original_length = len(self._view_registry)
 
         for view in view_or_iterable:
-            self._view_registry.remove(view)
+            try:
+                self._view_registry.remove(view)
+            except ValueError as e:
+                _raise_not_registered(view, e)
 
             if len(self._view_registry) == original_length:
-                raise admin.sites.NotRegistered(
-                    f"The view {view.__name__} is not registered"
-                )
+                _raise_not_registered(view)
 
     def _build_modelview(self, view) -> dict:
         """
         Creates dict for custom admin view for use in app_list[models]
         """
         url = reverse(f"{self.name}:{view.route_name}")
         name = view.view_name
@@ -119,43 +132,62 @@
             "object_name": name,
             "admin_url": url,
             "view_only": True,
         }
 
     def get_app_list(self, request):
         """
-        Adds registered apps to perch-admin app list used for nav.
+        Adds registered apps to admin app list used for nav.
         """
         app_list = super().get_app_list(request)
         custom_admin_models = []
 
         for view in self._view_registry:
             found = False
             view_app_label = get_app_label(view).lower()
-            if view_app_label == settings.CUSTOM_ADMIN_DEFAULT_APP_LABEL:
-                custom_admin_models.append(self._build_modelview(view))
-                continue
+            if view().user_has_permission(request.user):
+                if view_app_label == settings.CUSTOM_ADMIN_DEFAULT_APP_LABEL:
+                    custom_admin_models.append(self._build_modelview(view))
+                    continue
 
             for app in app_list:
                 if view_app_label == app.get("app_label", "").lower():
-                    if view.user_has_permission(request.user):
+                    found = True
+                    if view().user_has_permission(request.user):
                         app_models = app["models"]
                         app_models.append(self._build_modelview(view))
                         app_models.sort(key=lambda x: x["name"])
-                        found = True
                         break
+
+            if not found:
+                remaining_apps = set(set(get_installed_apps())).difference(app_list)
+                for app in remaining_apps:
+                    if view_app_label == app:
+                        found = True
+                        if view().user_has_permission(request.user):
+                            app_config = apps.get_app_config(view_app_label)
+                            app_name = app_config.verbose_name
+                            app_list.append(
+                                {
+                                    "name": app_name,
+                                    "app_label": view_app_label,
+                                    "app_url": f"{reverse(f'{self.name}:{view.route_name}')}{view_app_label}/",
+                                    "models": [self._build_modelview(view)],
+                                }
+                            )
+
             if not found:
                 raise ImproperlyConfigured(
                     f'The following custom admin view has an app_label that couldn\'t be found: "{view.__name__}". Please check that "{view_app_label}" is a valid app_label.'
                 )
 
         if custom_admin_models:
             app_list += [
                 {
                     "name": "Custom Admin Pages",
                     "app_label": settings.CUSTOM_ADMIN_DEFAULT_APP_LABEL,
-                    "app_url": f"{reverse('admin:index')}{settings.CUSTOM_ADMIN_DEFAULT_APP_LABEL}/",
+                    "app_url": f"{reverse(f'{self.name}:index')}{settings.CUSTOM_ADMIN_DEFAULT_APP_LABEL}/",
                     "models": custom_admin_models,
                 }
             ]
             app_list = sorted(app_list, key=lambda x: x["name"])
         return app_list
```

### Comparing `django_custom_admin_pages-1.0.0/django_custom_admin_pages/urls.py` & `django_custom_admin_pages-1.1.0/django_custom_admin_pages/urls.py`

 * *Files identical despite different names*

### Comparing `django_custom_admin_pages-1.0.0/django_custom_admin_pages/views/admin_base_view.py` & `django_custom_admin_pages-1.1.0/django_custom_admin_pages/views/admin_base_view.py`

 * *Files identical despite different names*

### Comparing `django_custom_admin_pages-1.0.0/pyproject.toml` & `django_custom_admin_pages-1.1.0/pyproject.toml`

 * *Files identical despite different names*

```diff
@@ -2,15 +2,15 @@
 name = "django-custom-admin-pages"
 authors = [
     "Leif Kjos <leif+pypi@leifkjos.com>",
 ]
 maintainers = [
     "Leif Kjos <leif+pypi@leifkjos.com>",
 ]
-version = "1.0.0"
+version = "1.1.0"
 description = "A django app that lets you add standard class-based views to the django admin index and navigation."
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/lekjos/django-custom-admin-pages"
 repository = "https://github.com/lekjos/django-custom-admin-pages"
 keywords = ["django", "admin", "django-admin", "django admin", "interface", "customize admin", "custom admin", "customize"]
 classifiers = [
```

### Comparing `django_custom_admin_pages-1.0.0/PKG-INFO` & `django_custom_admin_pages-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-custom-admin-pages
-Version: 1.0.0
+Version: 1.1.0
 Summary: A django app that lets you add standard class-based views to the django admin index and navigation.
 Home-page: https://github.com/lekjos/django-custom-admin-pages
 License: BSD-3-Clause
 Keywords: django,admin,django-admin,django admin,interface,customize admin,custom admin,customize
 Author: Leif Kjos
 Author-email: leif+pypi@leifkjos.com
 Maintainer: Leif Kjos
@@ -31,19 +31,20 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: django (>=3.2,<4.0)
 Project-URL: Repository, https://github.com/lekjos/django-custom-admin-pages
 Description-Content-Type: text/markdown
 
-[![PyPI version](https://badge.fury.io/py/django-custom-admin-pages.svg)](https://badge.fury.io/py/django-custom-admin-pages)
+[![PyPI](https://img.shields.io/pypi/v/django-custom-admin-pages)](https://pypi.org/project/django-custom-admin-pages/)
+![Python Supported](https://img.shields.io/badge/Python-3.9,_3.10,_3.11-blue)
+![Django Supported](https://img.shields.io/badge/Django-3.2,_4.0,_4.1,_4.2-blue)
 [![Tests](https://github.com/lekjos/django-custom-admin-pages/actions/workflows/build_and_test.yml/badge.svg)](https://github.com/lekjos/django-custom-admin-pages/actions/workflows/build_and_test.yml)
 [![codecov](https://codecov.io/gh/lekjos/django-custom-admin-pages/branch/master/graph/badge.svg?token=AJG2WICKXA)](https://codecov.io/gh/lekjos/django-custom-admin-pages)
-![Python Versions](https://img.shields.io/badge/Python_Versions-3.9,_3.10,_3.11-blue)
-![Django Versions](https://img.shields.io/badge/Django_Versions-3.2,_4.0,_4.1,_4.2-blue)
+![PyPI - Downloads](https://img.shields.io/pypi/dw/django-custom-admin-pages)
 
 
 # Django Custom Admin Pages
 A django app that lets you add standard class-based views to the django admin index and navigation. Create a view, register it like you would a ModelAdmin, and it appears in the Django Admin Nav.
 
 
 ## Installation
@@ -57,19 +58,23 @@
    # "django.contrib.admin", #REMOVE THIS LINE
    # ...
    "django_custom_admin_pages",
    "django_custom_admin_pages.admin.CustomAdminConfig"
    # ...
 ]
 ```
-4. If you've defined a custom django admin site, you can also subclass `django_custom_admin_pages.admin.CustomAdminConfig`:
+4. If you've defined a custom django admin site, you can also subclass `django_custom_admin_pages.admin.CustomAdminConfig` and/or `django_custom_admin_pages.admin.CustomAdminSite`:
 
 ```python
-from django_custom_admin_pages.admin import CustomAdminConfig
-class MyCustomAdminSite(CustomAdminConfig):
+from django_custom_admin_pages.admin import CustomAdminConfig, CustomAdminSite
+
+class MyCustomAdminConfig(CustomAdminConfig):
+   default_site="path.to.MyCustomAdminSite"
+
+class MyCustomAdminSite(CustomAdminSite):
    pass
 ```
 
 ## Usage
 
 This app is for custom admin views which aren't associated with a specific model. Add dashboards and other custom admin views here.
 
@@ -197,7 +202,8 @@
    - `poetry run pylint django_custom_admin_pages/`
 
 2. Run black:
    - `poetry run black .`
 
 2. Run isort:
    - `poetry run isort django_custom_admin_pages/`
+
```

