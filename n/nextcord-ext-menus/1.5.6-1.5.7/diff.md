# Comparing `tmp/nextcord-ext-menus-1.5.6.tar.gz` & `tmp/nextcord-ext-menus-1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nextcord-ext-menus-1.5.6.tar", last modified: Mon Oct 31 22:31:59 2022, max compression
+gzip compressed data, was "nextcord-ext-menus-1.5.7.tar", last modified: Fri Aug  4 11:51:28 2023, max compression
```

## Comparing `nextcord-ext-menus-1.5.6.tar` & `nextcord-ext-menus-1.5.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 22:31:59.570115 nextcord-ext-menus-1.5.6/
--rw-r--r--   0 runner    (1001) docker     (121)     1132 2022-10-31 22:31:50.000000 nextcord-ext-menus-1.5.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1876 2022-10-31 22:31:59.570115 nextcord-ext-menus-1.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1439 2022-10-31 22:31:50.000000 nextcord-ext-menus-1.5.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 22:31:59.566115 nextcord-ext-menus-1.5.6/nextcord/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 22:31:59.566115 nextcord-ext-menus-1.5.6/nextcord/ext/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 22:31:59.570115 nextcord-ext-menus-1.5.6/nextcord/ext/menus/
--rw-r--r--   0 runner    (1001) docker     (121)      202 2022-10-31 22:31:50.000000 nextcord-ext-menus-1.5.6/nextcord/ext/menus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      600 2022-10-31 22:31:50.000000 nextcord-ext-menus-1.5.6/nextcord/ext/menus/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)      922 2022-10-31 22:31:50.000000 nextcord-ext-menus-1.5.6/nextcord/ext/menus/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    13280 2022-10-31 22:31:50.000000 nextcord-ext-menus-1.5.6/nextcord/ext/menus/menu_pages.py
--rw-r--r--   0 runner    (1001) docker     (121)    34459 2022-10-31 22:31:50.000000 nextcord-ext-menus-1.5.6/nextcord/ext/menus/menus.py
--rw-r--r--   0 runner    (1001) docker     (121)    14920 2022-10-31 22:31:50.000000 nextcord-ext-menus-1.5.6/nextcord/ext/menus/page_source.py
--rw-r--r--   0 runner    (1001) docker     (121)     3083 2022-10-31 22:31:50.000000 nextcord-ext-menus-1.5.6/nextcord/ext/menus/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 22:31:59.570115 nextcord-ext-menus-1.5.6/nextcord_ext_menus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1876 2022-10-31 22:31:59.000000 nextcord-ext-menus-1.5.6/nextcord_ext_menus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      469 2022-10-31 22:31:59.000000 nextcord-ext-menus-1.5.6/nextcord_ext_menus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-31 22:31:59.000000 nextcord-ext-menus-1.5.6/nextcord_ext_menus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-10-31 22:31:59.000000 nextcord-ext-menus-1.5.6/nextcord_ext_menus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-10-31 22:31:59.000000 nextcord-ext-menus-1.5.6/nextcord_ext_menus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1755 2022-10-31 22:31:50.000000 nextcord-ext-menus-1.5.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-31 22:31:59.574115 nextcord-ext-menus-1.5.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2286 2022-10-31 22:31:50.000000 nextcord-ext-menus-1.5.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:51:28.958096 nextcord-ext-menus-1.5.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-08-04 11:51:17.000000 nextcord-ext-menus-1.5.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-08-04 11:51:28.958096 nextcord-ext-menus-1.5.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-08-04 11:51:17.000000 nextcord-ext-menus-1.5.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:51:28.954096 nextcord-ext-menus-1.5.7/nextcord/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:51:28.954096 nextcord-ext-menus-1.5.7/nextcord/ext/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:51:28.958096 nextcord-ext-menus-1.5.7/nextcord/ext/menus/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-08-04 11:51:17.000000 nextcord-ext-menus-1.5.7/nextcord/ext/menus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-08-04 11:51:17.000000 nextcord-ext-menus-1.5.7/nextcord/ext/menus/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-08-04 11:51:17.000000 nextcord-ext-menus-1.5.7/nextcord/ext/menus/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13280 2023-08-04 11:51:17.000000 nextcord-ext-menus-1.5.7/nextcord/ext/menus/menu_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34641 2023-08-04 11:51:17.000000 nextcord-ext-menus-1.5.7/nextcord/ext/menus/menus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14920 2023-08-04 11:51:17.000000 nextcord-ext-menus-1.5.7/nextcord/ext/menus/page_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-08-04 11:51:17.000000 nextcord-ext-menus-1.5.7/nextcord/ext/menus/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:51:28.958096 nextcord-ext-menus-1.5.7/nextcord_ext_menus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-08-04 11:51:28.000000 nextcord-ext-menus-1.5.7/nextcord_ext_menus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-08-04 11:51:28.000000 nextcord-ext-menus-1.5.7/nextcord_ext_menus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 11:51:28.000000 nextcord-ext-menus-1.5.7/nextcord_ext_menus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-04 11:51:28.000000 nextcord-ext-menus-1.5.7/nextcord_ext_menus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-04 11:51:28.000000 nextcord-ext-menus-1.5.7/nextcord_ext_menus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-08-04 11:51:17.000000 nextcord-ext-menus-1.5.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 11:51:28.958096 nextcord-ext-menus-1.5.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-08-04 11:51:17.000000 nextcord-ext-menus-1.5.7/setup.py
```

### Comparing `nextcord-ext-menus-1.5.6/LICENSE` & `nextcord-ext-menus-1.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nextcord-ext-menus-1.5.6/PKG-INFO` & `nextcord-ext-menus-1.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextcord-ext-menus
-Version: 1.5.6
+Version: 1.5.7
 Summary: An extension module to make reaction and button component menus with nextcord
 Home-page: https://github.com/nextcord/nextcord-ext-menus
 Author: Nextcord Developers
 License: MIT
 Project-URL: Bug Tracker, https://github.com/nextcord/nextcord-ext-menus/issues
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
```

### Comparing `nextcord-ext-menus-1.5.6/README.md` & `nextcord-ext-menus-1.5.7/README.md`

 * *Files identical despite different names*

### Comparing `nextcord-ext-menus-1.5.6/nextcord/ext/menus/constants.py` & `nextcord-ext-menus-1.5.7/nextcord/ext/menus/constants.py`

 * *Files identical despite different names*

### Comparing `nextcord-ext-menus-1.5.6/nextcord/ext/menus/exceptions.py` & `nextcord-ext-menus-1.5.7/nextcord/ext/menus/exceptions.py`

 * *Files identical despite different names*

### Comparing `nextcord-ext-menus-1.5.6/nextcord/ext/menus/menu_pages.py` & `nextcord-ext-menus-1.5.7/nextcord/ext/menus/menu_pages.py`

 * *Files identical despite different names*

### Comparing `nextcord-ext-menus-1.5.6/nextcord/ext/menus/menus.py` & `nextcord-ext-menus-1.5.7/nextcord/ext/menus/menus.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,14 @@
         emoji: EmojiType,
         action: Callable[..., Coroutine[Any, Any, Any]],
         *,
         skip_if: Optional[Callable[..., bool]] = None,
         position: Optional[Position] = None,
         lock: Optional[bool] = True,
     ):
-
         self.emoji = _cast_emoji(emoji)
         self.action = action
         self.skip_if = skip_if
         self.position = position or Position(0)
         self.lock = lock
 
     @property
@@ -268,15 +267,14 @@
         *,
         timeout: float = DEFAULT_TIMEOUT,
         delete_message_after: bool = False,
         clear_reactions_after: bool = False,
         check_embeds: bool = False,
         message: Optional[Union[nextcord.Message, nextcord.PartialInteractionMessage]] = None,
     ):
-
         self.timeout = timeout
         self.delete_message_after = delete_message_after
         self.clear_reactions_after = clear_reactions_after
         self.check_embeds = check_embeds
         self._can_remove_reactions = False
         self.__tasks = []
         self._running = True
@@ -687,15 +685,19 @@
         elif interaction is not None:
             self.bot = getattr(interaction, "client", interaction._state._get_client())
             self._author_id = interaction.user.id  # type: ignore
             channel = channel or interaction.channel  # type: ignore
         else:
             raise ValueError("ctx or interaction must be set.")
         me: Union[Member, ClientUser] = channel.guild.me if hasattr(channel, "guild") else self.bot.user  # type: ignore
-        permissions = channel.permissions_for(me)  # type: ignore
+        permissions = Permissions.all()
+        if interaction is not None:
+            permissions = interaction.app_permissions
+        elif hasattr(channel, "permissions_for"):
+            permissions = channel.permissions_for(me)  # type: ignore
         self.__me = nextcord.Object(id=me.id)
         self._verify_permissions(ctx, channel, permissions)
         self._event.clear()
         msg = self.message
         if msg is None:
             self.message = msg = await self.send_initial_message(ctx, channel)
```

### Comparing `nextcord-ext-menus-1.5.6/nextcord/ext/menus/page_source.py` & `nextcord-ext-menus-1.5.7/nextcord/ext/menus/page_source.py`

 * *Files identical despite different names*

### Comparing `nextcord-ext-menus-1.5.6/nextcord/ext/menus/utils.py` & `nextcord-ext-menus-1.5.7/nextcord/ext/menus/utils.py`

 * *Files identical despite different names*

### Comparing `nextcord-ext-menus-1.5.6/nextcord_ext_menus.egg-info/PKG-INFO` & `nextcord-ext-menus-1.5.7/nextcord_ext_menus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextcord-ext-menus
-Version: 1.5.6
+Version: 1.5.7
 Summary: An extension module to make reaction and button component menus with nextcord
 Home-page: https://github.com/nextcord/nextcord-ext-menus
 Author: Nextcord Developers
 License: MIT
 Project-URL: Bug Tracker, https://github.com/nextcord/nextcord-ext-menus/issues
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
```

### Comparing `nextcord-ext-menus-1.5.6/pyproject.toml` & `nextcord-ext-menus-1.5.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nextcord-ext-menus-1.5.6/setup.py` & `nextcord-ext-menus-1.5.7/setup.py`

 * *Files identical despite different names*

