# Comparing `tmp/fastapi_amis_admin-0.6.2a1.tar.gz` & `tmp/fastapi_amis_admin-0.6.3a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_amis_admin-0.6.2a1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "fastapi_amis_admin-0.6.3a1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fastapi_amis_admin-0.6.2a1.tar` & `fastapi_amis_admin-0.6.3a1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0    11789 2023-07-25 07:16:49.201564 fastapi_amis_admin-0.6.2a1/README.md
--rw-r--r--   0        0        0      603 2023-07-26 10:34:07.496014 fastapi_amis_admin-0.6.2a1/fastapi_amis_admin/__init__.py
--rw-r--r--   0        0        0      431 2023-04-12 06:50:08.587080 fastapi_amis_admin-0.6.2a1/fastapi_amis_admin/admin/__init__.py
--rw-r--r--   0        0        0    59537 2023-07-26 10:05:17.232130 fastapi_amis_admin-0.6.2a1/fastapi_amis_admin/admin/admin.py
--rw-r--r--   0        0        0     3488 2023-07-25 07:16:49.216523 fastapi_amis_admin-0.6.2a1/fastapi_amis_admin/admin/handlers.py
--rw-r--r--   0        0        0    14171 2023-07-25 07:16:49.217520 fastapi_amis_admin-0.6.2a1/fastapi_amis_admin/admin/parser.py
--rw-r--r--   0        0        0     2446 2023-07-25 07:16:49.218518 fastapi_amis_admin-0.6.2a1/fastapi_amis_admin/admin/settings.py
--rw-r--r--   0        0        0     5515 2023-04-12 06:50:08.590120 fastapi_amis_admin-0.6.2a1/fastapi_amis_admin/admin/site.py
--rw-r--r--   0        0        0     4074 2022-10-24 02:06:23.827774 fastapi_amis_admin-0.6.2a1/fastapi_amis_admin/amis/README.md
--rw-r--r--   0        0        0      495 2023-04-12 06:50:08.590658 fastapi_amis_admin-0.6.2a1/fastapi_amis_admin/amis/__init__.py
--rw-r--r--   0        0        0   152004 2023-07-25 07:16:49.221509 fastapi_amis_admin-0.6.2a1/fastapi_amis_admin/amis/components.py
--rw-r--r--   0        0        0     2480 2023-04-28 14:12:09.921152 fastapi_amis_admin-0.6.2a1/fastapi_amis_admin/amis/constants.py
--rw-r--r--   0        0        0     6850 2023-02-21 08:37:04.511335 fastapi_amis_admin-0.6.2a1/fastapi_amis_admin/amis/templates/app.html
--rw-r--r--   0        0        0     1275 2023-02-21 08:37:04.512336 fastapi_amis_admin-0.6.2a1/fastapi_amis_admin/amis/templates/page.html
--rw-r--r--   0        0        0     4977 2023-07-25 07:16:49.222507 fastapi_amis_admin-0.6.2a1/fastapi_amis_admin/amis/types.py
--rw-r--r--   0        0        0      265 2022-10-24 02:06:23.834769 fastapi_amis_admin-0.6.2a1/fastapi_amis_admin/amis/utils.py
--rw-r--r--   0        0        0     1727 2022-10-24 02:06:23.836768 fastapi_amis_admin-0.6.2a1/fastapi_amis_admin/crud/README.md
--rw-r--r--   0        0        0      211 2023-07-25 07:16:49.223506 fastapi_amis_admin-0.6.2a1/fastapi_amis_admin/crud/__init__.py
--rw-r--r--   0        0        0    24356 2023-07-26 08:52:20.491935 fastapi_amis_admin-0.6.2a1/fastapi_amis_admin/crud/_sqlalchemy.py
--rw-r--r--   0        0        0      419 2023-07-25 07:16:49.224503 fastapi_amis_admin-0.6.2a1/fastapi_amis_admin/crud/_sqlmodel.py
--rw-r--r--   0        0        0     8079 2023-07-25 07:16:49.225500 fastapi_amis_admin-0.6.2a1/fastapi_amis_admin/crud/base.py
--rw-r--r--   0        0        0    14942 2023-07-26 02:02:34.279406 fastapi_amis_admin-0.6.2a1/fastapi_amis_admin/crud/parser.py
--rw-r--r--   0        0        0     1689 2023-07-25 07:16:49.227491 fastapi_amis_admin-0.6.2a1/fastapi_amis_admin/crud/schema.py
--rw-r--r--   0        0        0     1714 2023-07-25 07:16:49.227491 fastapi_amis_admin-0.6.2a1/fastapi_amis_admin/crud/utils.py
--rw-r--r--   0        0        0     1882 2022-05-21 14:37:43.776550 fastapi_amis_admin-0.6.2a1/fastapi_amis_admin/locale/base.pot
--rw-r--r--   0        0        0     1719 2022-10-15 09:37:05.704518 fastapi_amis_admin-0.6.2a1/fastapi_amis_admin/locale/de_DE/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     2652 2022-10-15 13:48:06.829794 fastapi_amis_admin-0.6.2a1/fastapi_amis_admin/locale/de_DE/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1563 2023-03-13 12:29:37.252078 fastapi_amis_admin-0.6.2a1/fastapi_amis_admin/locale/zh_CN/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     2709 2023-03-13 12:29:37.252078 fastapi_amis_admin-0.6.2a1/fastapi_amis_admin/locale/zh_CN/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0      156 2023-07-25 07:16:49.228518 fastapi_amis_admin-0.6.2a1/fastapi_amis_admin/models/__init__.py
--rw-r--r--   0        0        0     2911 2022-09-22 08:34:57.596807 fastapi_amis_admin-0.6.2a1/fastapi_amis_admin/models/enums.py
--rw-r--r--   0        0        0     2964 2023-07-25 07:16:49.228518 fastapi_amis_admin-0.6.2a1/fastapi_amis_admin/models/fields.py
--rw-r--r--   0        0        0        0 2021-12-03 06:56:03.696000 fastapi_amis_admin-0.6.2a1/fastapi_amis_admin/utils/__init__.py
--rw-r--r--   0        0        0     2145 2022-09-22 08:34:57.599806 fastapi_amis_admin-0.6.2a1/fastapi_amis_admin/utils/functools.py
--rw-r--r--   0        0        0     8494 2023-07-26 02:46:58.141914 fastapi_amis_admin-0.6.2a1/fastapi_amis_admin/utils/pydantic.py
--rw-r--r--   0        0        0     1905 2023-07-25 07:16:49.230503 fastapi_amis_admin-0.6.2a1/fastapi_amis_admin/utils/translation.py
--rw-r--r--   0        0        0     2820 2023-07-25 07:16:49.233593 fastapi_amis_admin-0.6.2a1/pyproject.toml
--rw-r--r--   0        0        0    13828 1970-01-01 00:00:00.000000 fastapi_amis_admin-0.6.2a1/PKG-INFO
+-rw-r--r--   0        0        0    11789 2023-07-11 03:47:06.502739 fastapi_amis_admin-0.6.3a1/README.md
+-rw-r--r--   0        0        0      603 2023-08-04 07:53:08.550698 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/__init__.py
+-rw-r--r--   0        0        0      431 2023-04-09 14:42:19.167596 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/admin/__init__.py
+-rw-r--r--   0        0        0    60045 2023-08-04 07:48:22.236266 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/admin/admin.py
+-rw-r--r--   0        0        0     3488 2023-07-07 10:00:42.574847 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/admin/handlers.py
+-rw-r--r--   0        0        0    14171 2023-07-17 01:57:26.105611 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/admin/parser.py
+-rw-r--r--   0        0        0     2446 2023-08-04 02:30:10.829405 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/admin/settings.py
+-rw-r--r--   0        0        0     5515 2023-04-10 02:48:14.773714 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/admin/site.py
+-rw-r--r--   0        0        0     4074 2022-10-24 02:06:23.827774 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/amis/README.md
+-rw-r--r--   0        0        0      495 2023-04-10 02:29:06.105345 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/amis/__init__.py
+-rw-r--r--   0        0        0   152222 2023-08-04 07:48:19.695786 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/amis/components.py
+-rw-r--r--   0        0        0     2480 2023-04-18 02:58:25.165709 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/amis/constants.py
+-rw-r--r--   0        0        0     6850 2023-02-16 12:50:32.161558 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/amis/templates/app.html
+-rw-r--r--   0        0        0     1275 2023-02-17 13:46:40.329429 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/amis/templates/page.html
+-rw-r--r--   0        0        0     4977 2023-07-11 06:11:29.701954 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/amis/types.py
+-rw-r--r--   0        0        0      265 2022-10-24 02:06:23.834769 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/amis/utils.py
+-rw-r--r--   0        0        0     1727 2022-10-24 02:06:23.836768 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/crud/README.md
+-rw-r--r--   0        0        0      211 2023-07-08 02:15:45.947633 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/crud/__init__.py
+-rw-r--r--   0        0        0    25066 2023-08-04 07:48:22.238245 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/crud/_sqlalchemy.py
+-rw-r--r--   0        0        0      419 2023-07-07 10:02:58.918305 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/crud/_sqlmodel.py
+-rw-r--r--   0        0        0     8260 2023-08-04 07:48:22.239246 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/crud/base.py
+-rw-r--r--   0        0        0    14984 2023-08-04 07:48:19.698800 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/crud/parser.py
+-rw-r--r--   0        0        0     1712 2023-08-04 07:48:22.240245 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/crud/schema.py
+-rw-r--r--   0        0        0     1714 2023-07-11 15:07:52.748913 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/crud/utils.py
+-rw-r--r--   0        0        0     2200 2023-03-03 00:56:42.771550 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/locale/base.pot
+-rw-r--r--   0        0        0     1719 2023-03-03 01:02:59.621695 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/locale/de_DE/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2652 2023-03-03 00:58:11.049585 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/locale/de_DE/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1563 2023-03-03 01:14:57.935868 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/locale/zh_CN/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2709 2023-03-03 01:14:57.936867 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/locale/zh_CN/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0      156 2023-07-06 03:28:44.283974 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/models/__init__.py
+-rw-r--r--   0        0        0     2911 2023-04-10 02:48:14.997586 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/models/enums.py
+-rw-r--r--   0        0        0     2964 2023-07-06 03:28:22.246379 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/models/fields.py
+-rw-r--r--   0        0        0        0 2021-12-03 06:56:03.696000 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/utils/__init__.py
+-rw-r--r--   0        0        0     2145 2023-04-10 02:48:15.066546 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/utils/functools.py
+-rw-r--r--   0        0        0     8494 2023-07-28 08:46:05.738068 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/utils/pydantic.py
+-rw-r--r--   0        0        0     1905 2023-07-06 03:28:44.284973 fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/utils/translation.py
+-rw-r--r--   0        0        0     2820 2023-07-11 07:17:31.634284 fastapi_amis_admin-0.6.3a1/pyproject.toml
+-rw-r--r--   0        0        0    13828 1970-01-01 00:00:00.000000 fastapi_amis_admin-0.6.3a1/PKG-INFO
```

### Comparing `fastapi_amis_admin-0.6.2a1/README.md` & `fastapi_amis_admin-0.6.3a1/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.6.2a1/fastapi_amis_admin/__init__.py` & `fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.6.2a1"
+__version__ = "0.6.3a1"
 __url__ = "https://github.com/amisadmin/fastapi_amis_admin"
 
 import gettext
 import os
 
 from .utils.translation import i18n
```

### Comparing `fastapi_amis_admin-0.6.2a1/fastapi_amis_admin/admin/admin.py` & `fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/admin/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -728,31 +728,33 @@
                     label=_("Operation"),
                     buttons=actions,
                 )
             )
         return columns
 
     async def get_list_table_api(self, request: Request) -> AmisAPI:
-        data = {"&": "$$"}
+        api = AmisAPI(
+            method="POST",
+            url=f"{self.router_path}/list?" + "page=${page}&perPage=${perPage}&orderBy=${orderBy}&orderDir=${orderDir}",
+            data={"&": "$$"},
+        )
+        if not await self.has_filter_permission(request, None):
+            return api
         for field in self.search_fields:
             alias = self.parser.get_alias(field)
             if alias:
-                data[alias] = f"[~]${alias}"
+                api.data[alias] = f"[~]${alias}"
         for field in await self.get_list_filter(request):
             if isinstance(field, FormItem):
-                data[field.name] = f"${field.name}"
+                api.data[field.name] = f"${field.name}"
             else:
                 modelfield = self.parser.get_modelfield(field)
                 if modelfield and issubclass(modelfield.type_, (datetime.datetime, datetime.date, datetime.time)):
-                    data[modelfield.alias] = f"[-]${modelfield.alias}"
-        return AmisAPI(
-            method="POST",
-            url=f"{self.router_path}/list?" + "page=${page}&perPage=${perPage}&orderBy=${orderBy}&orderDir=${orderDir}",
-            data=data,
-        )
+                    api.data[modelfield.alias] = f"[-]${modelfield.alias}"
+        return api
 
     async def get_list_table(self, request: Request) -> TableCRUD:
         headerToolbar = [
             "filter-toggler",
             "reload",
             "bulkActions",
             {"type": "columns-toggler", "align": "right", "draggable": True},
@@ -765,21 +767,24 @@
                 "align": "right",
             },
         ]
         headerToolbar.extend(await self.get_actions(request, flag="toolbar"))
         itemActions = []
         if not self.display_item_action_as_column:
             itemActions = await self.get_actions(request, flag="item")
+        filter_form = None
+        if await self.has_filter_permission(request, None):
+            filter_form = await self.get_list_filter_form(request)
         table = TableCRUD(
             api=await self.get_list_table_api(request),
             autoFillHeight=True,
             headerToolbar=headerToolbar,
             filterTogglable=True,
             filterDefaultVisible=False,
-            filter=await self.get_list_filter_form(request),
+            filter=filter_form,
             syncLocation=False,
             keepItemSelectionOnPageChange=True,
             perPage=self.list_per_page,
             itemActions=itemActions,
             bulkActions=await self.get_actions(request, flag="bulk"),
             footerToolbar=[
                 "statistics",
@@ -842,26 +847,26 @@
                 responseData={"controls": [picker]},
             ),
         )
 
     async def get_form_item(
         self, request: Request, modelfield: ModelField, action: CrudEnum
     ) -> Union[FormItem, SchemaNode, None]:
-        is_filter = action == CrudEnum.list
+        is_filter = True if action in [CrudEnum.filter, CrudEnum.list] else False
         set_default = action == CrudEnum.create
         return await self.get_form_item_on_foreign_key(request, modelfield, is_filter=is_filter) or self.amis_parser.as_form_item(
             modelfield, is_filter=is_filter, set_default=set_default
         )
 
     async def get_list_filter_form(self, request: Request) -> Form:
-        body = await self._conv_modelfields_to_formitems(request, await self.get_list_filter(request), CrudEnum.list)
+        body = await self._conv_modelfields_to_formitems(request, await self.get_list_filter(request), CrudEnum.filter)
         return Form(
             type="",
             title=_("Filter"),
-            name=CrudEnum.list,
+            name=CrudEnum.filter,
             body=body,
             mode=DisplayModeEnum.inline,
             actions=[
                 Action(
                     actionType="clear-and-submit",
                     label=_("Clear"),
                     level=LevelEnum.default,
@@ -1103,14 +1108,22 @@
         request: Request,
         paginator: Paginator,
         filters: SchemaFilterT = None,
         **kwargs,
     ) -> bool:
         return await self.has_page_permission(request, action=CrudEnum.list)
 
+    async def has_filter_permission(
+        self,
+        request: Request,
+        filters: Optional[SchemaFilterT],
+        **kwargs,
+    ) -> bool:
+        return await self.has_page_permission(request, action=CrudEnum.filter)
+
     async def has_create_permission(self, request: Request, data: SchemaCreateT, **kwargs) -> bool:  # type self.schema_create
         return await self.has_page_permission(request, action=CrudEnum.create)
 
     async def has_read_permission(self, request: Request, item_id: List[str], **kwargs) -> bool:
         return await self.has_page_permission(request, action=CrudEnum.read)
 
     async def has_update_permission(
@@ -1138,30 +1151,30 @@
             return await self.has_read_permission(request, None)  # type: ignore
         else:
             return True
 
 
 class AdminAction:
     admin: BaseActionAdmin
-    action: Action = None
+    action: Action = Action()
 
     def __init__(
         self,
         admin: BaseActionAdmin,
         *,
         name: str = None,
         label: str = None,
         action: Action = None,
         flags: Union[str, List[str]] = None,
         getter: Callable[[Request], ActionT] = None,
         **kwargs,
     ):
         self.admin = admin
         assert self.admin, "admin is None"
-        self.action = action or self.action or Action()
+        self.action = action or self.action.copy()
         self.action = self.action.update_from_dict(kwargs)
         self.name = name or self.action.id or self.action.name
         assert self.name, "name is None"
         self.label = label or self.action.label or self.action.tooltip
         assert self.label, "label is None"
         self.flags = flags or ["item"]
         if isinstance(self.flags, str):
```

### Comparing `fastapi_amis_admin-0.6.2a1/fastapi_amis_admin/admin/handlers.py` & `fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/admin/handlers.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.6.2a1/fastapi_amis_admin/admin/parser.py` & `fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/admin/parser.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.6.2a1/fastapi_amis_admin/admin/settings.py` & `fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/admin/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     site_icon: str = "https://baidu.gitee.io/amis/static/favicon_b3b0647.png"
     site_url: str = ""
     site_path: str = "/admin"
     database_url_async: str = ""
     database_url: str = ""
     language: Union[Literal["zh_CN", "en_US", "de_DE"], str] = ""
     amis_cdn: str = "https://unpkg.com"
-    amis_pkg: str = "amis@3.2.0"
+    amis_pkg: str = "amis@3.3.0"
     amis_theme: Literal["cxd", "antd", "dark", "ang"] = "cxd"
     amis_image_receiver: API = None  # Image upload interface
     amis_file_receiver: API = None  # File upload interface
     logger: Union[logging.Logger, Any] = logging.getLogger("fastapi_amis_admin")
 
     @classmethod
     def valid_url_(cls, url: str):
```

### Comparing `fastapi_amis_admin-0.6.2a1/fastapi_amis_admin/admin/site.py` & `fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/admin/site.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.6.2a1/fastapi_amis_admin/amis/README.md` & `fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/amis/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.6.2a1/fastapi_amis_admin/amis/components.py` & `fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/amis/components.py`

 * *Files 0% similar despite different names*

```diff
@@ -2828,14 +2828,22 @@
     steps: List[Step] = None  # Array, configure step information
     startStep: int = None  # "1" # Start default value, starting from the first step. Templates can be supported,
     # but only when the component is created, the template is rendered and the current number of steps is set. When
     # the component is refreshed later,
     # The current step will not change according to startStep
 
 
+class AmisRender(AmisNode):
+    """Amis render"""
+
+    type: str = "amis"  # Specify as amis renderer
+    schema_: SchemaNode = Field(None, alias="schema")  # amis schema
+    props: dict = None  # amis props
+
+
 PageSchema.update_forward_refs()
 ActionType.Dialog.update_forward_refs()
 ActionType.Drawer.update_forward_refs()
 TableCRUD.update_forward_refs()
 Form.update_forward_refs()
 Tpl.update_forward_refs()
 InputText.update_forward_refs()
```

### Comparing `fastapi_amis_admin-0.6.2a1/fastapi_amis_admin/amis/constants.py` & `fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/amis/constants.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.6.2a1/fastapi_amis_admin/amis/templates/app.html` & `fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/amis/templates/app.html`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.6.2a1/fastapi_amis_admin/amis/templates/page.html` & `fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/amis/templates/page.html`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.6.2a1/fastapi_amis_admin/amis/types.py` & `fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/amis/types.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.6.2a1/fastapi_amis_admin/crud/README.md` & `fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/crud/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.6.2a1/fastapi_amis_admin/crud/_sqlalchemy.py` & `fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/crud/_sqlalchemy.py`

 * *Files 4% similar despite different names*

```diff
@@ -392,42 +392,55 @@
         sel = select(self.model).where(self.pk.in_(list(map(get_python_type_parse(self.pk), item_id))))
         return session.scalars(sel).all()
 
     async def fetch_items(self, *item_id: str) -> List[TableModelT]:
         """Fetch the database data by id."""
         return await self.db.async_run_sync(self._fetch_item_scalars, item_id)
 
-    def _create_items(self, session: Session, items: List[Dict[str, Any]]) -> Union[int, SchemaModelT]:
-        count = len(items)
-        for item in items:
-            obj = self.create_item(item)
-            session.add(obj)
-            if count > 1:
-                continue
-            session.flush()
-            session.refresh(obj)
-            return parse_obj_to_schema(obj, self.schema_model)
-        return count
+    def _create_items(self, session: Session, items: List[Dict[str, Any]]) -> List[TableModelT]:
+        if not items:
+            return []
+        objs = [self.create_item(item) for item in items]
+        session.add_all(objs)
+        session.flush()
+        return objs
+
+    async def create_items(self, request: Request, items: List[SchemaCreateT]) -> List[TableModelT]:
+        """Create multiple database data."""
+        items = [await self.on_create_pre(request, obj) for obj in items]
+        return await self.db.async_run_sync(self._create_items, items)
 
     def _read_items(self, session: Session, item_id: List[str]) -> List[SchemaReadT]:
         items = self._fetch_item_scalars(session, item_id)
         return [self.read_item(obj) for obj in items]
 
-    def _update_items(self, session: Session, item_id: List[str], values: Dict[str, Any]):
+    async def read_items(self, request: Request, item_id: List[str]) -> List[SchemaReadT]:
+        """Fetch the database data by id."""
+        return await self.db.async_run_sync(self._read_items, item_id)
+
+    def _update_items(self, session: Session, item_id: List[str], values: Dict[str, Any]) -> List[TableModelT]:
         items = self._fetch_item_scalars(session, item_id)
         for item in items:
             self.update_item(item, values)
-        return len(items)
+        return items
+
+    async def update_items(self, request: Request, item_id: List[str], values: Dict[str, Any]) -> List[TableModelT]:
+        """Update the database data by id."""
+        return await self.db.async_run_sync(self._update_items, item_id, values)
 
     def _delete_items(self, session: Session, item_id: List[str]) -> List[TableModelT]:
         items = self._fetch_item_scalars(session, item_id)
         for item in items:
             self.delete_item(item)
         return items
 
+    async def delete_items(self, request: Request, item_id: List[str]) -> List[TableModelT]:
+        """Delete the database data by id."""
+        return await self.db.async_run_sync(self._delete_items, item_id)
+
     @property
     def schema_name_prefix(self):
         if self.__class__ is SqlalchemyCrud:
             return self.model.__name__
         return super().schema_name_prefix
 
     async def on_create_pre(self, request: Request, obj: SchemaCreateT, **kwargs) -> Dict[str, Any]:
@@ -452,17 +465,14 @@
 
     async def on_list_after(self, request: Request, result: Result, data: ItemListSchema, **kwargs) -> ItemListSchema:
         """Parse the database data query result dictionary into schema_list."""
         data.items = self.parser.conv_row_to_dict(result.all())
         data.items = [self.list_item(item) for item in data.items]
         return data
 
-    async def on_delete_after(self, request: Request, items: List[TableModelT]) -> int:
-        return len(items)
-
     @property
     def AnnotatedSelect(self):
         """Annotated Select, used to automatically perform fastapi dependency injection"""
         return Annotated[Select, Depends(self._select_maker)]
 
     @property
     def AnnotatedItemIdList(self):
@@ -475,14 +485,15 @@
     def filtered_item_id(self) -> Callable:
         """Filter the id of the data that the user has permission to operate on."""
 
         async def depend(
             item_id: ItemIdListDepend,
             sel: self.AnnotatedSelect,  # type: ignore
         ):
+            item_id = list(map(get_python_type_parse(self.pk), item_id))
             filtered_id = await self.db.async_scalars(sel.where(self.pk.in_(item_id)).with_only_columns(self.pk))
             return filtered_id.all()
 
         return depend
 
     @property
     def route_list(self) -> Callable:
@@ -492,17 +503,18 @@
             paginator: Annotated[self.paginator, Depends()],  # type: ignore
             filters: Annotated[self.schema_filter, Body()] = None,  # type: ignore
         ):
             if not await self.has_list_permission(request, paginator, filters):
                 return self.error_no_router_permission(request)
             data = ItemListSchema(items=[])
             data.query = request.query_params
-            data.filters = await self.on_filter_pre(request, filters)
-            if data.filters:
-                sel = sel.filter(*self.calc_filter_clause(data.filters))
+            if await self.has_filter_permission(request, filters):
+                data.filters = await self.on_filter_pre(request, filters)
+                if data.filters:
+                    sel = sel.filter(*self.calc_filter_clause(data.filters))
             if paginator.show_total:
                 data.total = await self.db.async_scalar(
                     select(func.count("*")).select_from(sel.with_only_columns(self.pk).subquery())
                 )
             orderBy = self._calc_ordering(paginator.orderBy, paginator.orderDir)
             if orderBy:
                 sel = sel.order_by(*orderBy)
@@ -518,64 +530,60 @@
             request: Request,
             data: Annotated[Union[List[self.schema_create], self.schema_create], Body()],  # type: ignore
         ) -> BaseApiOut[Union[int, self.schema_model]]:  # type: ignore
             if not await self.has_create_permission(request, data):
                 return self.error_no_router_permission(request)
             if not isinstance(data, list):
                 data = [data]
-            items = [await self.on_create_pre(request, obj) for obj in data]
-            if not items:
-                return self.error_data_handle(request)
             try:
-                result = await self.db.async_run_sync(self._create_items, items=items)
+                items = await self.create_items(request, data)
             except Exception as error:
                 return self.error_execute_sql(request=request, error=error)
+            result = len(items)
+            if result == 1:  # if only one item, return the first item
+                result = await self.db.async_run_sync(lambda _: parse_obj_to_schema(items[0], self.schema_model, refresh=True))
             return BaseApiOut(data=result)
 
         return route
 
     @property
     def route_read(self) -> Callable:
         async def route(
             request: Request,
             item_id: self.AnnotatedItemIdList,  # type: ignore
         ):
             if not await self.has_read_permission(request, item_id):
                 return self.error_no_router_permission(request)
-            items = await self.db.async_run_sync(self._read_items, item_id)
-            if len(items) == 1:
-                items = items[0]
-            return BaseApiOut(data=items)
+            items = await self.read_items(request, item_id)
+            return BaseApiOut(data=items if len(items) > 1 else items[0])
 
         return route
 
     @property
     def route_update(self) -> Callable:
         async def route(
             request: Request,
             item_id: self.AnnotatedItemIdList,  # type: ignore
             data: Annotated[self.schema_update, Body()],  # type: ignore
         ):
             if not await self.has_update_permission(request, item_id, data):
                 return self.error_no_router_permission(request)
-            item_id = list(map(get_python_type_parse(self.pk), item_id))
             values = await self.on_update_pre(request, data, item_id=item_id)
             if not values:
                 return self.error_data_handle(request)
-            result = await self.db.async_run_sync(self._update_items, item_id, values)
-            return BaseApiOut(data=result)
+            items = await self.update_items(request, item_id, values)
+            return BaseApiOut(data=len(items))
 
         return route
 
     @property
     def route_delete(self) -> Callable:
         async def route(
             request: Request,
             item_id: self.AnnotatedItemIdList,  # type: ignore
         ):
             if not await self.has_delete_permission(request, item_id):
                 return self.error_no_router_permission(request)
-            items = await self.db.async_run_sync(self._delete_items, item_id)
-            data = await self.on_delete_after(request, items)
-            return BaseApiOut(data=data)
+            items = await self.delete_items(request, item_id)
+            return BaseApiOut(data=len(items))
 
         return route
```

### Comparing `fastapi_amis_admin-0.6.2a1/fastapi_amis_admin/crud/base.py` & `fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/crud/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,14 +177,22 @@
         request: Request,
         paginator: Optional[Paginator],
         filters: Optional[SchemaFilterT],
         **kwargs,
     ) -> bool:
         return True
 
+    async def has_filter_permission(
+        self,
+        request: Request,
+        filters: Optional[SchemaFilterT],
+        **kwargs,
+    ) -> bool:
+        return True
+
     async def has_create_permission(self, request: Request, obj: Optional[SchemaCreateT], **kwargs) -> bool:
         return True
 
     async def has_read_permission(self, request: Request, item_id: Optional[List[str]], **kwargs) -> bool:
         return True
 
     async def has_update_permission(
```

### Comparing `fastapi_amis_admin-0.6.2a1/fastapi_amis_admin/crud/parser.py` & `fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/crud/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,18 @@
 
 import sqlalchemy
 from fastapi.utils import create_cloned_field, create_response_field
 from pydantic import BaseConfig, BaseModel
 from pydantic.fields import Field, FieldInfo
 from sqlalchemy import Column, String, Table
 from sqlalchemy.engine import Row
-from sqlalchemy.orm import ColumnProperty, DeclarativeMeta, InstrumentedAttribute, RelationshipProperty
+from sqlalchemy.orm import ColumnProperty, DeclarativeMeta, InstrumentedAttribute, RelationshipProperty, object_session
 from sqlalchemy.sql import Select
 from sqlalchemy.sql.elements import Label
 
-from fastapi_amis_admin.crud.base import SchemaModelT
 from fastapi_amis_admin.utils.pydantic import (
     PYDANTIC_V2,
     ModelField,
     create_model_by_fields,
     model_config_attr,
     model_fields,
     parse_date,
@@ -319,16 +318,18 @@
     fields = TableModelParser.get_table_model_fields(table_model).values()
     for field in fields:
         if field.alias == alias:
             return field
     return None
 
 
-def parse_obj_to_schema(obj: SchemaModelT, schema: Type[SchemaT]) -> SchemaT:
+def parse_obj_to_schema(obj: TableModelT, schema: Type[SchemaT], refresh: bool = False) -> SchemaT:
     """parse obj to schema"""
+    if refresh:
+        object_session(obj).refresh(obj)
     orm_mode = model_config_attr(schema, "orm_mode", False) or model_config_attr(schema, "from_attributes", False)
     parse = schema.from_orm if orm_mode else schema.parse_obj
     return parse(obj)
 
 
 def insfield_to_modelfield(insfield: InstrumentedAttribute) -> Optional[ModelField]:
     """InstrumentedAttribute to ModelField"""
```

### Comparing `fastapi_amis_admin-0.6.2a1/fastapi_amis_admin/crud/schema.py` & `fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/crud/schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     total: Optional[int] = None  # Data total
     query: Optional[Dict[str, Any]] = None
     filter: Optional[Dict[str, Any]] = None
 
 
 class CrudEnum(str, Enum):
     list = "list"
+    filter = "filter"
     create = "create"
     read = "read"
     update = "update"
     delete = "delete"
 
 
 class Paginator:
```

### Comparing `fastapi_amis_admin-0.6.2a1/fastapi_amis_admin/crud/utils.py` & `fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/crud/utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.6.2a1/fastapi_amis_admin/locale/de_DE/LC_MESSAGES/messages.mo` & `fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/locale/de_DE/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.6.2a1/fastapi_amis_admin/locale/de_DE/LC_MESSAGES/messages.po` & `fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/locale/de_DE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.6.2a1/fastapi_amis_admin/locale/zh_CN/LC_MESSAGES/messages.mo` & `fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/locale/zh_CN/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.6.2a1/fastapi_amis_admin/locale/zh_CN/LC_MESSAGES/messages.po` & `fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/locale/zh_CN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.6.2a1/fastapi_amis_admin/models/enums.py` & `fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/models/enums.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.6.2a1/fastapi_amis_admin/models/fields.py` & `fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/models/fields.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.6.2a1/fastapi_amis_admin/utils/functools.py` & `fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/utils/functools.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.6.2a1/fastapi_amis_admin/utils/pydantic.py` & `fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/utils/pydantic.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.6.2a1/fastapi_amis_admin/utils/translation.py` & `fastapi_amis_admin-0.6.3a1/fastapi_amis_admin/utils/translation.py`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.6.2a1/pyproject.toml` & `fastapi_amis_admin-0.6.3a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin-0.6.2a1/PKG-INFO` & `fastapi_amis_admin-0.6.3a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_amis_admin
-Version: 0.6.2a1
+Version: 0.6.3a1
 Summary: FastAPI-Amis-Admin is a high-performance, efficient and easily extensible FastAPI admin framework. Inspired by Django-admin, and has as many powerful functions as Django-admin. 
 Keywords: fastapi,fastapi-admin,fastapi-amis-admin,django-admin,sqlmodel,sqlalchemy
 Author-email: Atomi <1456417373@qq.com>
 Maintainer-email: Atomi <1456417373@qq.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Framework :: FastAPI
```

