# Comparing `tmp/django-debug-toolbar-user-panel-1.1.1.tar.gz` & `tmp/django-debug-toolbar-user-panel-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-debug-toolbar-user-panel-1.1.1.tar", last modified: Mon Mar 19 22:42:31 2018, max compression
+gzip compressed data, was "django-debug-toolbar-user-panel-2.0.0.tar", last modified: Fri Aug  4 07:52:36 2023, max compression
```

## Comparing `django-debug-toolbar-user-panel-1.1.1.tar` & `django-debug-toolbar-user-panel-2.0.0.tar`

### file list

```diff
@@ -1,13 +1,21 @@
-drwxr-xr-x   0 lamby     (1000) lamby     (1000)        0 2018-03-19 22:42:31.000000 django-debug-toolbar-user-panel-1.1.1/
-drwxr-xr-x   0 lamby     (1000) lamby     (1000)        0 2018-03-19 22:42:31.000000 django-debug-toolbar-user-panel-1.1.1/debug_toolbar_user_panel/
--rw-r--r--   0 lamby     (1000) lamby     (1000)        0 2014-12-30 16:46:24.000000 django-debug-toolbar-user-panel-1.1.1/debug_toolbar_user_panel/__init__.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)      342 2014-12-30 16:46:24.000000 django-debug-toolbar-user-panel-1.1.1/debug_toolbar_user_panel/forms.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     3985 2018-03-19 22:42:03.000000 django-debug-toolbar-user-panel-1.1.1/debug_toolbar_user_panel/panels.py
-drwxr-xr-x   0 lamby     (1000) lamby     (1000)        0 2018-03-19 22:42:31.000000 django-debug-toolbar-user-panel-1.1.1/debug_toolbar_user_panel/templates/
-drwxr-xr-x   0 lamby     (1000) lamby     (1000)        0 2018-03-19 22:42:31.000000 django-debug-toolbar-user-panel-1.1.1/debug_toolbar_user_panel/templates/debug_toolbar_user_panel/
--rw-r--r--   0 lamby     (1000) lamby     (1000)      899 2017-05-03 19:11:28.000000 django-debug-toolbar-user-panel-1.1.1/debug_toolbar_user_panel/templates/debug_toolbar_user_panel/panel.html
--rw-r--r--   0 lamby     (1000) lamby     (1000)      356 2014-12-30 16:46:24.000000 django-debug-toolbar-user-panel-1.1.1/debug_toolbar_user_panel/decorators.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)        0 2014-12-30 16:46:24.000000 django-debug-toolbar-user-panel-1.1.1/debug_toolbar_user_panel/models.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)     1115 2014-12-30 16:46:24.000000 django-debug-toolbar-user-panel-1.1.1/debug_toolbar_user_panel/views.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)      533 2018-03-19 22:42:30.000000 django-debug-toolbar-user-panel-1.1.1/setup.py
--rw-r--r--   0 lamby     (1000) lamby     (1000)      337 2018-03-19 22:42:31.000000 django-debug-toolbar-user-panel-1.1.1/PKG-INFO
+drwxr-xr-x   0 lamby     (1000) lamby     (1000)        0 2023-08-04 07:52:36.742055 django-debug-toolbar-user-panel-2.0.0/
+-rw-r--r--   0 lamby     (1000) lamby     (1000)     1527 2014-12-30 16:46:24.000000 django-debug-toolbar-user-panel-2.0.0/COPYING
+-rw-r--r--   0 lamby     (1000) lamby     (1000)      320 2023-08-04 07:52:36.742055 django-debug-toolbar-user-panel-2.0.0/PKG-INFO
+-rw-r--r--   0 lamby     (1000) lamby     (1000)      276 2018-03-07 14:19:35.000000 django-debug-toolbar-user-panel-2.0.0/README.rst
+drwxr-xr-x   0 lamby     (1000) lamby     (1000)        0 2023-08-04 07:52:36.742055 django-debug-toolbar-user-panel-2.0.0/debug_toolbar_user_panel/
+-rw-r--r--   0 lamby     (1000) lamby     (1000)        0 2014-12-30 16:46:24.000000 django-debug-toolbar-user-panel-2.0.0/debug_toolbar_user_panel/__init__.py
+-rw-r--r--   0 lamby     (1000) lamby     (1000)      356 2014-12-30 16:46:24.000000 django-debug-toolbar-user-panel-2.0.0/debug_toolbar_user_panel/decorators.py
+-rw-r--r--   0 lamby     (1000) lamby     (1000)      342 2014-12-30 16:46:24.000000 django-debug-toolbar-user-panel-2.0.0/debug_toolbar_user_panel/forms.py
+-rw-r--r--   0 lamby     (1000) lamby     (1000)        0 2014-12-30 16:46:24.000000 django-debug-toolbar-user-panel-2.0.0/debug_toolbar_user_panel/models.py
+-rw-r--r--   0 lamby     (1000) lamby     (1000)     4103 2023-08-04 07:51:31.000000 django-debug-toolbar-user-panel-2.0.0/debug_toolbar_user_panel/panels.py
+drwxr-xr-x   0 lamby     (1000) lamby     (1000)        0 2023-08-04 07:52:36.742055 django-debug-toolbar-user-panel-2.0.0/debug_toolbar_user_panel/templates/
+drwxr-xr-x   0 lamby     (1000) lamby     (1000)        0 2023-08-04 07:52:36.742055 django-debug-toolbar-user-panel-2.0.0/debug_toolbar_user_panel/templates/debug_toolbar_user_panel/
+-rw-r--r--   0 lamby     (1000) lamby     (1000)      899 2017-05-03 19:11:28.000000 django-debug-toolbar-user-panel-2.0.0/debug_toolbar_user_panel/templates/debug_toolbar_user_panel/panel.html
+-rw-r--r--   0 lamby     (1000) lamby     (1000)     1115 2014-12-30 16:46:24.000000 django-debug-toolbar-user-panel-2.0.0/debug_toolbar_user_panel/views.py
+drwxr-xr-x   0 lamby     (1000) lamby     (1000)        0 2023-08-04 07:52:36.742055 django-debug-toolbar-user-panel-2.0.0/django_debug_toolbar_user_panel.egg-info/
+-rw-r--r--   0 lamby     (1000) lamby     (1000)      320 2023-08-04 07:52:36.000000 django-debug-toolbar-user-panel-2.0.0/django_debug_toolbar_user_panel.egg-info/PKG-INFO
+-rw-r--r--   0 lamby     (1000) lamby     (1000)      532 2023-08-04 07:52:36.000000 django-debug-toolbar-user-panel-2.0.0/django_debug_toolbar_user_panel.egg-info/SOURCES.txt
+-rw-r--r--   0 lamby     (1000) lamby     (1000)        1 2023-08-04 07:52:36.000000 django-debug-toolbar-user-panel-2.0.0/django_debug_toolbar_user_panel.egg-info/dependency_links.txt
+-rw-r--r--   0 lamby     (1000) lamby     (1000)       25 2023-08-04 07:52:36.000000 django-debug-toolbar-user-panel-2.0.0/django_debug_toolbar_user_panel.egg-info/top_level.txt
+-rw-r--r--   0 lamby     (1000) lamby     (1000)       38 2023-08-04 07:52:36.742055 django-debug-toolbar-user-panel-2.0.0/setup.cfg
+-rwxr-xr-x   0 lamby     (1000) lamby     (1000)      534 2023-08-04 07:52:35.000000 django-debug-toolbar-user-panel-2.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-debug-toolbar-user-panel-1.1.1/debug_toolbar_user_panel/panels.py` & `django-debug-toolbar-user-panel-2.0.0/debug_toolbar_user_panel/panels.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,26 +50,26 @@
 File a bug
   https://github.com/playfire/django-debug-toolbar-user-panel/issues
 """
 
 from django import VERSION
 from django.conf import settings
 from django.http import HttpResponseForbidden
-from django.conf.urls import url
+from django.urls import re_path
 from django.template.loader import render_to_string
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 from django.contrib.auth import get_user_model
 
-from debug_toolbar.panels import DebugPanel
+from debug_toolbar.panels import Panel
 
 from . import views
 from .forms import UserForm
 
-class UserPanel(DebugPanel):
+class UserPanel(Panel):
     """
     Panel that allows you to login as other recently-logged in users.
     """
 
     name = 'User'
     has_content = True
 
@@ -114,22 +114,26 @@
             'current': current,
         })
 
     def is_authenticated(self, request):
         if VERSION >= (1, 10):
             # Django 1.10 onwards `is_authenticated` is a property
             return request.user.is_authenticated
-        return request.user.is_authenticated()
+        return request.user.is_authenticated
+
+    def process_request(self, request):
+        self.request = request
+        return super().process_request(request)
 
     def process_response(self, request, response):
         self.request = request
 
     @classmethod
     def get_urls(cls):
         return (
-            url(r'^users/login/$', views.login_form,
+            re_path(r'^users/login/$', views.login_form,
                 name='debug-userpanel-login-form'),
-            url(r'^users/login/(?P<pk>-?\d+)$', views.login,
+            re_path(r'^users/login/(?P<pk>-?\d+)$', views.login,
                 name='debug-userpanel-login'),
-            url(r'^users/logout$', views.logout,
+            re_path(r'^users/logout$', views.logout,
                 name='debug-userpanel-logout'),
         )
```

### Comparing `django-debug-toolbar-user-panel-1.1.1/debug_toolbar_user_panel/templates/debug_toolbar_user_panel/panel.html` & `django-debug-toolbar-user-panel-2.0.0/debug_toolbar_user_panel/templates/debug_toolbar_user_panel/panel.html`

 * *Files identical despite different names*

### Comparing `django-debug-toolbar-user-panel-1.1.1/debug_toolbar_user_panel/views.py` & `django-debug-toolbar-user-panel-2.0.0/debug_toolbar_user_panel/views.py`

 * *Files identical despite different names*

### Comparing `django-debug-toolbar-user-panel-1.1.1/setup.py` & `django-debug-toolbar-user-panel-2.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-#!/usr/bin/env python
+#!/usr/bin/env python3
 
 from distutils.core import setup
 
 setup(
     name='django-debug-toolbar-user-panel',
     description="Panel for the Django Debug toolbar to quickly switch between "
         "users.",
-    version='1.1.1',
+    version='2.0.0',
     url='https://chris-lamb.co.uk/projects/django-debug-toolbar-user-panel',
 
     author="Chris Lamb",
     author_email="chris@chris-lamb.co.uk",
     license='BSD',
 
     packages=(
```

