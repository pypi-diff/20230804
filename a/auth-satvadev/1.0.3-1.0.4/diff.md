# Comparing `tmp/auth_satvadev-1.0.3.tar.gz` & `tmp/auth_satvadev-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auth_satvadev-1.0.3.tar", max compression
+gzip compressed data, was "auth_satvadev-1.0.4.tar", max compression
```

## Comparing `auth_satvadev-1.0.3.tar` & `auth_satvadev-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1052 2023-07-03 14:27:43.030928 auth_satvadev-1.0.3/LICENSE
--rw-r--r--   0        0        0     1323 2023-07-18 14:32:23.278884 auth_satvadev-1.0.3/README.md
--rw-r--r--   0        0        0     1023 2023-07-20 16:36:51.078818 auth_satvadev-1.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-03 14:27:43.030928 auth_satvadev-1.0.3/src/auth_satvadev/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 14:27:43.034928 auth_satvadev-1.0.3/src/auth_satvadev/api/__init__.py
--rw-r--r--   0        0        0      351 2023-07-03 14:27:43.034928 auth_satvadev-1.0.3/src/auth_satvadev/api/exceptions.py
--rw-r--r--   0        0        0      812 2023-07-18 14:32:23.278884 auth_satvadev-1.0.3/src/auth_satvadev/api/serializers.py
--rw-r--r--   0        0        0      558 2023-07-18 14:32:23.282884 auth_satvadev-1.0.3/src/auth_satvadev/api/urls.py
--rw-r--r--   0        0        0     2774 2023-07-18 14:32:23.282884 auth_satvadev-1.0.3/src/auth_satvadev/api/views.py
--rw-r--r--   0        0        0      251 2023-07-18 14:32:23.282884 auth_satvadev-1.0.3/src/auth_satvadev/apps.py
--rw-r--r--   0        0        0     1488 2023-07-03 14:27:43.034928 auth_satvadev-1.0.3/src/auth_satvadev/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-07-03 14:27:43.034928 auth_satvadev-1.0.3/src/auth_satvadev/migrations/__init__.py
--rw-r--r--   0        0        0      546 2023-07-18 14:32:23.282884 auth_satvadev-1.0.3/src/auth_satvadev/models.py
--rw-r--r--   0        0        0     3069 2023-07-18 14:32:23.282884 auth_satvadev-1.0.3/src/auth_satvadev/senders.py
--rw-r--r--   0        0        0     2315 1970-01-01 00:00:00.000000 auth_satvadev-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1052 2023-07-03 14:27:43.030928 auth_satvadev-1.0.4/LICENSE
+-rw-r--r--   0        0        0     1323 2023-07-18 14:32:23.278884 auth_satvadev-1.0.4/README.md
+-rw-r--r--   0        0        0     1023 2023-08-04 08:13:52.004423 auth_satvadev-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-03 14:27:43.030928 auth_satvadev-1.0.4/src/auth_satvadev/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 14:27:43.034928 auth_satvadev-1.0.4/src/auth_satvadev/api/__init__.py
+-rw-r--r--   0        0        0      351 2023-07-03 14:27:43.034928 auth_satvadev-1.0.4/src/auth_satvadev/api/exceptions.py
+-rw-r--r--   0        0        0      812 2023-07-18 14:32:23.278884 auth_satvadev-1.0.4/src/auth_satvadev/api/serializers.py
+-rw-r--r--   0        0        0      558 2023-07-18 14:32:23.282884 auth_satvadev-1.0.4/src/auth_satvadev/api/urls.py
+-rw-r--r--   0        0        0     2774 2023-07-18 14:32:23.282884 auth_satvadev-1.0.4/src/auth_satvadev/api/views.py
+-rw-r--r--   0        0        0      251 2023-07-18 14:32:23.282884 auth_satvadev-1.0.4/src/auth_satvadev/apps.py
+-rw-r--r--   0        0        0     1488 2023-07-03 14:27:43.034928 auth_satvadev-1.0.4/src/auth_satvadev/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-07-03 14:27:43.034928 auth_satvadev-1.0.4/src/auth_satvadev/migrations/__init__.py
+-rw-r--r--   0        0        0      784 2023-08-04 08:12:22.334166 auth_satvadev-1.0.4/src/auth_satvadev/models.py
+-rw-r--r--   0        0        0     3522 2023-08-04 08:12:22.334166 auth_satvadev-1.0.4/src/auth_satvadev/senders.py
+-rw-r--r--   0        0        0     2315 1970-01-01 00:00:00.000000 auth_satvadev-1.0.4/PKG-INFO
```

### Comparing `auth_satvadev-1.0.3/LICENSE` & `auth_satvadev-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `auth_satvadev-1.0.3/README.md` & `auth_satvadev-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `auth_satvadev-1.0.3/pyproject.toml` & `auth_satvadev-1.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "auth_satvadev"
-version = "1.0.3"
+version = "1.0.4"
 description = "Registration with confirmation by code and token authorization"
 authors = ["satva.dev <info@satva.dev>"]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `auth_satvadev-1.0.3/src/auth_satvadev/api/serializers.py` & `auth_satvadev-1.0.4/src/auth_satvadev/api/serializers.py`

 * *Files identical despite different names*

### Comparing `auth_satvadev-1.0.3/src/auth_satvadev/api/urls.py` & `auth_satvadev-1.0.4/src/auth_satvadev/api/urls.py`

 * *Files identical despite different names*

### Comparing `auth_satvadev-1.0.3/src/auth_satvadev/api/views.py` & `auth_satvadev-1.0.4/src/auth_satvadev/api/views.py`

 * *Files identical despite different names*

### Comparing `auth_satvadev-1.0.3/src/auth_satvadev/migrations/0001_initial.py` & `auth_satvadev-1.0.4/src/auth_satvadev/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `auth_satvadev-1.0.3/src/auth_satvadev/senders.py` & `auth_satvadev-1.0.4/src/auth_satvadev/senders.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-import sys
 from abc import abstractmethod
+from importlib import import_module
 from inspect import getmembers, isclass
+from typing import Type
 
 from django.conf import settings
 from django.contrib.auth import get_user_model
+from django.template import Template
 from mail_satvadev.messages import BaseMail
 from mail_satvadev.tasks import send_email
-from django.template import Template
+
 from auth_satvadev.api.exceptions import CodeDoesNotMatchError
 from auth_satvadev.models import VerificationCode
 
 
 class BaseCodeSender:
     """Базовый класс для отправки и проверки кода подтверждения"""
 
@@ -55,22 +57,35 @@
             raise CodeDoesNotMatchError
 
         verification.delete()
 
         return get_user_model().objects.get(email=email)
 
 
-def get_sender_class():
+def get_sender_class() -> Type[BaseCodeSender]:
     """Метод для определения класса для отправки и валидации кодов
     подтверждения
+
+    Возвращает только наследуемые от BaseCodeSender классы
     """
     # TODO: добавить возможность использования нескольких классов для отправки
     # TODO: сообщений с кодом подтверждения
-    sender_class_name = getattr(settings, 'SENDER_CLASS', 'MailSender')
+    sender_settings = getattr(
+        settings,
+        'SENDER_CLASS',
+        'auth_satvadev.senders.MailSender',
+    ).split('.')
+    sender_module = import_module('.'.join(sender_settings[:-1]))
 
     sender_classes = [
         class_
-        for class_name, class_ in getmembers(sys.modules[__name__], isclass)
-        if class_name == sender_class_name
+        for class_name, class_ in getmembers(sender_module, isclass)
+        if (
+            class_name == sender_settings[-1] and
+            issubclass(class_, BaseCodeSender)
+        )
     ]
 
+    if len(sender_classes) == 0:
+        raise ValueError('Sender classes not found')
+
     return sender_classes[0]
```

### Comparing `auth_satvadev-1.0.3/PKG-INFO` & `auth_satvadev-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auth-satvadev
-Version: 1.0.3
+Version: 1.0.4
 Summary: Registration with confirmation by code and token authorization
 Author: satva.dev
 Author-email: info@satva.dev
 Requires-Python: >=3.9.10,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

