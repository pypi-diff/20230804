# Comparing `tmp/formkit_ninja-0.3.5.tar.gz` & `tmp/formkit_ninja-0.4.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "formkit_ninja-0.3.5.tar", max compression
+gzip compressed data, was "formkit_ninja-0.4.0a0.tar", max compression
```

## Comparing `formkit_ninja-0.3.5.tar` & `formkit_ninja-0.4.0a0.tar`

### file list

```diff
@@ -1,21 +1,25 @@
--rw-r--r--   0        0        0      813 2023-04-06 13:15:44.220033 formkit_ninja-0.3.5/README.md
--rw-r--r--   0        0        0        0 2023-04-06 13:15:44.220033 formkit_ninja-0.3.5/formkit_ninja/__init__.py
--rw-r--r--   0        0        0       21 2023-04-06 13:15:44.224033 formkit_ninja-0.3.5/formkit_ninja/__main__.py
--rw-r--r--   0        0        0    14860 2023-05-09 05:40:10.838963 formkit_ninja-0.3.5/formkit_ninja/admin.py
--rw-r--r--   0        0        0     2568 2023-05-09 05:38:40.651974 formkit_ninja-0.3.5/formkit_ninja/api.py
--rw-r--r--   0        0        0     4333 2023-04-10 00:27:28.783846 formkit_ninja-0.3.5/formkit_ninja/fields.py
--rw-r--r--   0        0        0    14103 2023-07-14 02:28:58.188490 formkit_ninja-0.3.5/formkit_ninja/formkit_schema.py
--rw-r--r--   0        0        0        0 2023-04-23 01:43:59.588049 formkit_ninja-0.3.5/formkit_ninja/management/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 13:15:44.220033 formkit_ninja-0.3.5/formkit_ninja/management/commands/__init__.py
--rw-r--r--   0        0        0     3807 2023-05-09 05:37:21.012799 formkit_ninja-0.3.5/formkit_ninja/management/commands/common_nodes.py
--rw-r--r--   0        0        0    19033 2023-05-09 05:17:09.351553 formkit_ninja-0.3.5/formkit_ninja/management/commands/create_sf11_form.py
--rw-r--r--   0        0        0     3190 2023-04-26 06:36:11.021575 formkit_ninja-0.3.5/formkit_ninja/management/commands/create_sf12_form.py
--rw-r--r--   0        0        0     1360 2023-04-26 06:10:12.411087 formkit_ninja-0.3.5/formkit_ninja/management/commands/create_sf13_form.py
--rw-r--r--   0        0        0    15059 2023-05-09 05:38:40.671974 formkit_ninja-0.3.5/formkit_ninja/migrations/0001_initial.py
--rw-r--r--   0        0        0      605 2023-05-09 05:15:03.707613 formkit_ninja-0.3.5/formkit_ninja/migrations/0002_alter_formcomponents_label_alter_formkitschema_key.py
--rw-r--r--   0        0        0      339 2023-05-09 05:37:27.484727 formkit_ninja-0.3.5/formkit_ninja/migrations/0003_delete_translatable.py
--rw-r--r--   0        0        0        0 2023-04-13 11:58:36.247052 formkit_ninja-0.3.5/formkit_ninja/migrations/__init__.py
--rw-r--r--   0        0        0     9588 2023-05-09 05:38:40.647974 formkit_ninja-0.3.5/formkit_ninja/models.py
--rw-r--r--   0        0        0      101 2023-04-06 13:15:44.224033 formkit_ninja-0.3.5/formkit_ninja/urls.py
--rw-r--r--   0        0        0     1199 2023-07-14 02:29:38.161397 formkit_ninja-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     1572 1970-01-01 00:00:00.000000 formkit_ninja-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0      813 2023-08-02 03:08:55.535863 formkit_ninja-0.4.0a0/README.md
+-rw-r--r--   0        0        0        0 2023-08-02 03:08:55.547864 formkit_ninja-0.4.0a0/formkit_ninja/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-02 03:08:55.535863 formkit_ninja-0.4.0a0/formkit_ninja/__main__.py
+-rw-r--r--   0        0        0    14803 2023-08-02 03:08:55.551864 formkit_ninja-0.4.0a0/formkit_ninja/admin.py
+-rw-r--r--   0        0        0     2568 2023-08-02 03:08:55.551864 formkit_ninja-0.4.0a0/formkit_ninja/api.py
+-rw-r--r--   0        0        0     4333 2023-08-02 03:08:55.551864 formkit_ninja-0.4.0a0/formkit_ninja/fields.py
+-rw-r--r--   0        0        0    14920 2023-08-02 03:08:55.555865 formkit_ninja-0.4.0a0/formkit_ninja/formkit_schema.py
+-rw-r--r--   0        0        0        0 2023-08-02 03:08:55.551864 formkit_ninja-0.4.0a0/formkit_ninja/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-02 03:08:55.551864 formkit_ninja-0.4.0a0/formkit_ninja/management/commands/__init__.py
+-rw-r--r--   0        0        0     3807 2023-08-02 03:08:55.555865 formkit_ninja-0.4.0a0/formkit_ninja/management/commands/common_nodes.py
+-rw-r--r--   0        0        0    19033 2023-08-02 03:08:55.555865 formkit_ninja-0.4.0a0/formkit_ninja/management/commands/create_sf11_form.py
+-rw-r--r--   0        0        0     3190 2023-08-02 03:08:55.555865 formkit_ninja-0.4.0a0/formkit_ninja/management/commands/create_sf12_form.py
+-rw-r--r--   0        0        0     1359 2023-08-02 03:08:55.555865 formkit_ninja-0.4.0a0/formkit_ninja/management/commands/create_sf13_form.py
+-rw-r--r--   0        0        0    15058 2023-08-02 03:08:55.555865 formkit_ninja-0.4.0a0/formkit_ninja/migrations/0001_initial.py
+-rw-r--r--   0        0        0      605 2023-08-02 03:08:55.555865 formkit_ninja-0.4.0a0/formkit_ninja/migrations/0002_alter_formcomponents_label_alter_formkitschema_key.py
+-rw-r--r--   0        0        0      338 2023-08-02 03:08:55.555865 formkit_ninja-0.4.0a0/formkit_ninja/migrations/0003_delete_translatable.py
+-rw-r--r--   0        0        0        0 2023-08-02 03:08:55.551864 formkit_ninja-0.4.0a0/formkit_ninja/migrations/__init__.py
+-rw-r--r--   0        0        0     9571 2023-08-02 03:08:55.555865 formkit_ninja-0.4.0a0/formkit_ninja/models.py
+-rw-r--r--   0        0        0        0 2023-08-02 03:08:55.551864 formkit_ninja-0.4.0a0/formkit_ninja/parser/__init__.py
+-rw-r--r--   0        0        0     1674 2023-08-02 03:08:55.555865 formkit_ninja-0.4.0a0/formkit_ninja/parser/get_tables.py
+-rw-r--r--   0        0        0       72 2023-08-02 03:08:55.555865 formkit_ninja-0.4.0a0/formkit_ninja/parser/logger.py
+-rw-r--r--   0        0        0    16186 2023-08-04 07:51:08.403190 formkit_ninja-0.4.0a0/formkit_ninja/parser/type_convert.py
+-rw-r--r--   0        0        0      101 2023-08-02 03:08:55.555865 formkit_ninja-0.4.0a0/formkit_ninja/urls.py
+-rw-r--r--   0        0        0     1208 2023-08-04 07:51:40.578409 formkit_ninja-0.4.0a0/pyproject.toml
+-rw-r--r--   0        0        0     1574 1970-01-01 00:00:00.000000 formkit_ninja-0.4.0a0/PKG-INFO
```

### Comparing `formkit_ninja-0.3.5/README.md` & `formkit_ninja-0.4.0a0/README.md`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.3.5/formkit_ninja/admin.py` & `formkit_ninja-0.4.0a0/formkit_ninja/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 from django import forms
 from django.contrib import admin
 from django.http import HttpRequest
 from ordered_model.admin import OrderedInlineModelAdminMixin, OrderedModelAdmin, OrderedTabularInline
 
 from formkit_ninja import models
-from formkit_ninja.formkit_schema import FORMKIT_TYPE
 
 logger = logging.getLogger(__name__)
 
 
 class ItemAdmin(OrderedModelAdmin):
     list_display = ("name", "move_up_down_links")
 
@@ -37,15 +36,14 @@
     def get_json_fields(self) -> dict[str, tuple[str]]:
         """
         Custom which json fields will be included in the return
         """
         return self._json_fields
 
     def __init__(self, *args, **kwargs):
-
         super().__init__(*args, **kwargs)
         instance = kwargs["instance"]
         for field, keys in self.get_json_fields().items():
             # Extract the dict of JSON values from the model instance if supplied
             values = {}
             if instance:
                 values = getattr(instance, field, {}) or {}  # Don't allow none
@@ -351,19 +349,17 @@
     class Meta:
         model = models.FormKitSchema
         exclude = ("name",)
 
 
 @admin.register(models.FormKitSchemaNode)
 class FormKitSchemaNodeAdmin(OrderedInlineModelAdminMixin, admin.ModelAdmin):
-
     list_display = ("label", "id", "node_type")
 
     def get_inlines(self, request, obj: models.FormKitSchemaNode | None):
-
         if not obj:
             return []
 
         formkit_node_type = (obj.node or {}).get("formkit", None)
 
         if formkit_node_type == "group":
             return [
```

### Comparing `formkit_ninja-0.3.5/formkit_ninja/api.py` & `formkit_ninja-0.4.0a0/formkit_ninja/api.py`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.3.5/formkit_ninja/fields.py` & `formkit_ninja-0.4.0a0/formkit_ninja/fields.py`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.3.5/formkit_ninja/formkit_schema.py` & `formkit_ninja-0.4.0a0/formkit_ninja/formkit_schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import logging
+import warnings
 from html.parser import HTMLParser
 from typing import Annotated, Any, ForwardRef, List, Literal, Type, TypedDict, TypeVar, Union
 
 from pydantic import BaseModel, Field
 
 """
 This is a port of selected parts of the FormKit schema
@@ -154,17 +155,17 @@
 
 
 class DatePickerNode(FormKitSchemaProps):
     node_type: Literal["formkit"] = "formkit"
     formkit: Literal["datepicker"] = "datepicker"
     dollar_formkit: str = Field(default="datepicker", alias="$formkit")
     calendarIcon: str = "calendar"
-    format: str = 'DD/MM/YY'
-    nextIcon: str = 'angleRight'
-    prevIcon: str = 'angleLeft'
+    format: str = "DD/MM/YY"
+    nextIcon: str = "angleRight"
+    prevIcon: str = "angleLeft"
 
 
 class CheckBoxNode(FormKitSchemaProps):
     node_type: Literal["formkit"] = "formkit"
     formkit: Literal["checkbox"] = "checkbox"
     dollar_formkit: str = Field(default="checkbox", alias="$formkit")
 
@@ -172,15 +173,15 @@
 class NumberNode(FormKitSchemaProps):
     node_type: Literal["formkit"] = "formkit"
     formkit: Literal["number"] = "number"
     dollar_formkit: str = Field(default="number", alias="$formkit")
     text: str | None
     max: int | None = None
     min: int | None = None
-    step: int | None = None
+    step: str | None = None
 
 
 class PasswordNode(FormKitSchemaProps):
     node_type: Literal["formkit"] = "formkit"
     formkit: Literal["password"] = "password"
     dollar_formkit: str = Field(default="password", alias="$formkit")
     name: str | None
@@ -197,14 +198,21 @@
 class SelectNode(FormKitSchemaProps):
     node_type: Literal["formkit"] = "formkit"
     formkit: Literal["select"] = "select"
     dollar_formkit: str = Field(default="select", alias="$formkit")
     options: str | list[dict[str, Any]] | list[str] | dict[str, str] | None = Field(None)
 
 
+class AutocompleteNode(FormKitSchemaProps):
+    node_type: Literal["formkit"] = "formkit"
+    formkit: Literal["autocomplete"] = "autocomplete"
+    dollar_formkit: str = Field(default="autocomplete", alias="$formkit")
+    options: str | list[dict[str, Any]] | list[str] | dict[str, str] | None = Field(None)
+
+
 class EmailNode(FormKitSchemaProps):
     node_type: Literal["formkit"] = "formkit"
     formkit: Literal["email"] = "email"
     dollar_formkit: str = Field(default="email", alias="$formkit")
 
 
 class TelNode(FormKitSchemaProps):
@@ -242,24 +250,25 @@
 
 FormKitSchemaFormKit = Annotated[
     Union[
         TextNode,
         CheckBoxNode,
         PasswordNode,
         SelectNode,
+        AutocompleteNode,
         EmailNode,
         NumberNode,
         RadioNode,
         GroupNode,
         DateNode,
         DatePickerNode,
         DropDownNode,
         RepeaterNode,
         TelNode,
-        CurrencyNode
+        CurrencyNode,
     ],
     Field(discriminator="formkit"),
 ]
 
 
 class FormKitSchemaDOMNode(FormKitSchemaProps):
     """
@@ -441,15 +450,26 @@
         """
         This classmethod differentiates between the different "Node" types
         when deserializing
         """
         if "id" in obj:
             obj["html_id"] = obj.pop("id")
         try:
-            return super().parse_obj({**get_node_type(obj), **obj})
+            parsed = super().parse_obj({**get_node_type(obj), **obj})
+            if getattr(parsed.__root__, "children", None):
+                children = []
+                for n in obj["children"]:
+                    if isinstance(n, str):
+                        pass
+                    try:
+                        children.append(cls.parse_obj(n).__root__)
+                    except Exception as E:
+                        warnings.warn(f"{E}")
+                parsed.__root__.children = children
+            return parsed
         except KeyError as E:
             raise Exception(f"Unable to parse content {obj} to a {cls}") from E
 
 
 class FormKitSchema(BaseModel):
     __root__: list[Node]
```

### Comparing `formkit_ninja-0.3.5/formkit_ninja/management/commands/common_nodes.py` & `formkit_ninja-0.4.0a0/formkit_ninja/management/commands/common_nodes.py`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.3.5/formkit_ninja/management/commands/create_sf11_form.py` & `formkit_ninja-0.4.0a0/formkit_ninja/management/commands/create_sf11_form.py`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.3.5/formkit_ninja/management/commands/create_sf12_form.py` & `formkit_ninja-0.4.0a0/formkit_ninja/management/commands/create_sf12_form.py`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.3.5/formkit_ninja/management/commands/create_sf13_form.py` & `formkit_ninja-0.4.0a0/formkit_ninja/management/commands/create_sf13_form.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from django.core.management.base import BaseCommand
 
 from formkit_ninja.management.commands.common_nodes import create_location_nodes
 
 
 def create():
-
     # The SF 13 form has the following schemas
     # meetingInformation
     # participants
     # projectteam
     # planning
     # sukus
```

### Comparing `formkit_ninja-0.3.5/formkit_ninja/migrations/0001_initial.py` & `formkit_ninja-0.4.0a0/formkit_ninja/migrations/0001_initial.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
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

### Comparing `formkit_ninja-0.3.5/formkit_ninja/migrations/0002_alter_formcomponents_label_alter_formkitschema_key.py` & `formkit_ninja-0.4.0a0/formkit_ninja/migrations/0002_alter_formcomponents_label_alter_formkitschema_key.py`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.3.5/formkit_ninja/models.py` & `formkit_ninja-0.4.0a0/formkit_ninja/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import itertools
 import json
 import logging
 import uuid
 from typing import Iterable, TypedDict, get_args
 
 from django.conf import settings
 from django.core.exceptions import ValidationError
```

### Comparing `formkit_ninja-0.3.5/pyproject.toml` & `formkit_ninja-0.4.0a0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "formkit-ninja"
-version = "0.3.5"
+version = "0.4.0a0"
 description = "A Django-Ninja backend to specify FormKit schemas"
 authors = ["Josh Brooks <josh@catalpa.io>"]
 license = "GPLv3"
 readme = "README.md"
 homepage = "https://github.com/catalpainternational/formkit-ninja"
 repository = "https://github.com/catalpainternational/formkit-ninja"
 packages = [{include = "formkit_ninja"}]
@@ -17,21 +17,22 @@
 django-ordered-model = "^3.6"
 pydantic = "<2"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.2.0"
-pytest-django = "^4.5.2"
+pytest = "^7.0"
+pytest-django = "^4.5"
 isort = "^5.11.4"
-black = "^22.12.0"
-flake8 = "^6.0.0"
-django-extensions = "^3.2.1"
-rich = "^13.1.0"
+black = "^23.0"
+flake8 = "^6.0"
+django-extensions = "^3.2"
+rich = "^13.0"
+sqlparse = "^0.4.4"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs-material = "^9.1.6"
 mkdocstrings = {extras = ["python"], version = "^0.21.2"}
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `formkit_ninja-0.3.5/PKG-INFO` & `formkit_ninja-0.4.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formkit-ninja
-Version: 0.3.5
+Version: 0.4.0a0
 Summary: A Django-Ninja backend to specify FormKit schemas
 Home-page: https://github.com/catalpainternational/formkit-ninja
 License: GPLv3
 Author: Josh Brooks
 Author-email: josh@catalpa.io
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
```

