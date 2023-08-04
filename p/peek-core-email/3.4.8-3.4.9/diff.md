# Comparing `tmp/peek-core-email-3.4.8.tar.gz` & `tmp/peek-core-email-3.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peek-core-email-3.4.8.tar", last modified: Tue Jul 11 02:52:09 2023, max compression
+gzip compressed data, was "peek-core-email-3.4.9.tar", last modified: Wed Jul 19 06:50:48 2023, max compression
```

## Comparing `peek-core-email-3.4.8.tar` & `peek-core-email-3.4.9.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:52:09.238092 peek-core-email-3.4.8/
--rw-r--r--   0 root         (0) root         (0)      368 2023-07-11 02:52:09.238092 peek-core-email-3.4.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      899 2023-07-11 02:51:10.000000 peek-core-email-3.4.8/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:52:09.236092 peek-core-email-3.4.8/peek_core_email/
--rw-r--r--   0 root         (0) root         (0)      460 2023-07-11 02:51:10.000000 peek-core-email-3.4.8/peek_core_email/PlatformDependencyTest.py
--rw-r--r--   0 root         (0) root         (0)      271 2023-07-11 02:51:10.000000 peek-core-email-3.4.8/peek_core_email/TempUnitTest.py
--rw-r--r--   0 root         (0) root         (0)      830 2023-07-11 02:52:09.000000 peek-core-email-3.4.8/peek_core_email/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:52:09.237092 peek-core-email-3.4.8/peek_core_email/_private/
--rw-r--r--   0 root         (0) root         (0)      163 2023-07-11 02:51:10.000000 peek-core-email-3.4.8/peek_core_email/_private/PluginNames.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 02:51:10.000000 peek-core-email-3.4.8/peek_core_email/_private/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:52:09.237092 peek-core-email-3.4.8/peek_core_email/_private/admin-app/
--rw-r--r--   0 root         (0) root         (0)      393 2023-07-11 02:51:10.000000 peek-core-email-3.4.8/peek_core_email/_private/admin-app/PluginNames.ts
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 02:51:10.000000 peek-core-email-3.4.8/peek_core_email/_private/admin-app/core-email-admin.component.css
--rw-r--r--   0 root         (0) root         (0)     1169 2023-07-11 02:51:10.000000 peek-core-email-3.4.8/peek_core_email/_private/admin-app/core-email-admin.component.html
--rw-r--r--   0 root         (0) root         (0)      282 2023-07-11 02:51:10.000000 peek-core-email-3.4.8/peek_core_email/_private/admin-app/core-email-admin.component.ts
--rw-r--r--   0 root         (0) root         (0)     1706 2023-07-11 02:51:10.000000 peek-core-email-3.4.8/peek_core_email/_private/admin-app/core-email.module.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:52:09.237092 peek-core-email-3.4.8/peek_core_email/_private/admin-app/setting-list/
--rw-r--r--   0 root         (0) root         (0)     2628 2023-07-11 02:51:10.000000 peek-core-email-3.4.8/peek_core_email/_private/admin-app/setting-list/admin-setting-list.component.html
--rw-r--r--   0 root         (0) root         (0)     1676 2023-07-11 02:51:10.000000 peek-core-email-3.4.8/peek_core_email/_private/admin-app/setting-list/admin-setting-list.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:52:09.237092 peek-core-email-3.4.8/peek_core_email/_private/alembic/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 02:51:10.000000 peek-core-email-3.4.8/peek_core_email/_private/alembic/__init__.py
--rw-r--r--   0 root         (0) root         (0)      301 2023-07-11 02:51:10.000000 peek-core-email-3.4.8/peek_core_email/_private/alembic/env.py
--rw-r--r--   0 root         (0) root         (0)      544 2023-07-11 02:51:10.000000 peek-core-email-3.4.8/peek_core_email/_private/alembic/script.py.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:52:09.237092 peek-core-email-3.4.8/peek_core_email/_private/alembic/versions/
--rw-r--r--   0 root         (0) root         (0)     1863 2023-07-11 02:51:10.000000 peek-core-email-3.4.8/peek_core_email/_private/alembic/versions/616e295c146d_initial.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 02:51:10.000000 peek-core-email-3.4.8/peek_core_email/_private/alembic/versions/__init__.py
--rw-r--r--   0 root         (0) root         (0)       96 2023-07-11 02:51:10.000000 peek-core-email-3.4.8/peek_core_email/_private/alembic.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:52:09.238092 peek-core-email-3.4.8/peek_core_email/_private/server/
--rw-r--r--   0 root         (0) root         (0)     2160 2023-07-11 02:51:10.000000 peek-core-email-3.4.8/peek_core_email/_private/server/EmailApi.py
--rw-r--r--   0 root         (0) root         (0)     1533 2023-07-11 02:51:10.000000 peek-core-email-3.4.8/peek_core_email/_private/server/EmailUtil.py
--rw-r--r--   0 root         (0) root         (0)     1716 2023-07-11 02:51:10.000000 peek-core-email-3.4.8/peek_core_email/_private/server/PluginLogicEntryHook.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 02:51:10.000000 peek-core-email-3.4.8/peek_core_email/_private/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:52:09.238092 peek-core-email-3.4.8/peek_core_email/_private/server/admin_backend/
--rw-r--r--   0 root         (0) root         (0)      970 2023-07-11 02:51:10.000000 peek-core-email-3.4.8/peek_core_email/_private/server/admin_backend/PeekAdmSettingHandler.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 02:51:10.000000 peek-core-email-3.4.8/peek_core_email/_private/server/admin_backend/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:52:09.238092 peek-core-email-3.4.8/peek_core_email/_private/storage/
--rw-r--r--   0 root         (0) root         (0)      275 2023-07-11 02:51:10.000000 peek-core-email-3.4.8/peek_core_email/_private/storage/DeclarativeBase.py
--rw-r--r--   0 root         (0) root         (0)     8274 2023-07-11 02:51:10.000000 peek-core-email-3.4.8/peek_core_email/_private/storage/Setting.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 02:51:10.000000 peek-core-email-3.4.8/peek_core_email/_private/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:52:09.238092 peek-core-email-3.4.8/peek_core_email/admin-doc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:52:09.238092 peek-core-email-3.4.8/peek_core_email/admin-doc/admin_task/
--rw-r--r--   0 root         (0) root         (0)      423 2023-07-11 02:51:10.000000 peek-core-email-3.4.8/peek_core_email/admin-doc/admin_task/admin_tasks.rst
--rw-r--r--   0 root         (0) root         (0)    42134 2023-07-11 02:51:10.000000 peek-core-email-3.4.8/peek_core_email/admin-doc/admin_task/edit_email_settings.png
--rw-r--r--   0 root         (0) root         (0)      233 2023-07-11 02:51:10.000000 peek-core-email-3.4.8/peek_core_email/admin-doc/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:52:09.238092 peek-core-email-3.4.8/peek_core_email/admin-doc/setup/
--rw-r--r--   0 root         (0) root         (0)    39549 2023-07-11 02:51:10.000000 peek-core-email-3.4.8/peek_core_email/admin-doc/setup/settings.png
--rw-r--r--   0 root         (0) root         (0)      497 2023-07-11 02:51:10.000000 peek-core-email-3.4.8/peek_core_email/admin-doc/setup/setup.rst
--rw-r--r--   0 root         (0) root         (0)      698 2023-07-11 02:52:09.000000 peek-core-email-3.4.8/peek_core_email/plugin_package.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:52:09.238092 peek-core-email-3.4.8/peek_core_email/server/
--rw-r--r--   0 root         (0) root         (0)      775 2023-07-11 02:51:10.000000 peek-core-email-3.4.8/peek_core_email/server/EmailApiABC.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 02:51:10.000000 peek-core-email-3.4.8/peek_core_email/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:52:09.237092 peek-core-email-3.4.8/peek_core_email.egg-info/
--rw-r--r--   0 root         (0) root         (0)      368 2023-07-11 02:52:09.000000 peek-core-email-3.4.8/peek_core_email.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1963 2023-07-11 02:52:09.000000 peek-core-email-3.4.8/peek_core_email.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 02:52:09.000000 peek-core-email-3.4.8/peek_core_email.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-07-11 02:52:09.000000 peek-core-email-3.4.8/peek_core_email.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-07-11 02:52:09.000000 peek-core-email-3.4.8/peek_core_email.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       80 2023-07-11 02:52:09.248092 peek-core-email-3.4.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2658 2023-07-11 02:52:09.000000 peek-core-email-3.4.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:50:48.307882 peek-core-email-3.4.9/
+-rw-r--r--   0 root         (0) root         (0)      368 2023-07-19 06:50:48.307882 peek-core-email-3.4.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      899 2023-07-19 06:49:47.000000 peek-core-email-3.4.9/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:50:48.305882 peek-core-email-3.4.9/peek_core_email/
+-rw-r--r--   0 root         (0) root         (0)      460 2023-07-19 06:49:47.000000 peek-core-email-3.4.9/peek_core_email/PlatformDependencyTest.py
+-rw-r--r--   0 root         (0) root         (0)      271 2023-07-19 06:49:47.000000 peek-core-email-3.4.9/peek_core_email/TempUnitTest.py
+-rw-r--r--   0 root         (0) root         (0)      830 2023-07-19 06:50:48.000000 peek-core-email-3.4.9/peek_core_email/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:50:48.305882 peek-core-email-3.4.9/peek_core_email/_private/
+-rw-r--r--   0 root         (0) root         (0)      163 2023-07-19 06:49:47.000000 peek-core-email-3.4.9/peek_core_email/_private/PluginNames.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 06:49:47.000000 peek-core-email-3.4.9/peek_core_email/_private/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:50:48.306882 peek-core-email-3.4.9/peek_core_email/_private/admin-app/
+-rw-r--r--   0 root         (0) root         (0)      393 2023-07-19 06:49:47.000000 peek-core-email-3.4.9/peek_core_email/_private/admin-app/PluginNames.ts
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 06:49:47.000000 peek-core-email-3.4.9/peek_core_email/_private/admin-app/core-email-admin.component.css
+-rw-r--r--   0 root         (0) root         (0)     1169 2023-07-19 06:49:47.000000 peek-core-email-3.4.9/peek_core_email/_private/admin-app/core-email-admin.component.html
+-rw-r--r--   0 root         (0) root         (0)      282 2023-07-19 06:49:47.000000 peek-core-email-3.4.9/peek_core_email/_private/admin-app/core-email-admin.component.ts
+-rw-r--r--   0 root         (0) root         (0)     1706 2023-07-19 06:49:47.000000 peek-core-email-3.4.9/peek_core_email/_private/admin-app/core-email.module.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:50:48.306882 peek-core-email-3.4.9/peek_core_email/_private/admin-app/setting-list/
+-rw-r--r--   0 root         (0) root         (0)     2628 2023-07-19 06:49:47.000000 peek-core-email-3.4.9/peek_core_email/_private/admin-app/setting-list/admin-setting-list.component.html
+-rw-r--r--   0 root         (0) root         (0)     1676 2023-07-19 06:49:47.000000 peek-core-email-3.4.9/peek_core_email/_private/admin-app/setting-list/admin-setting-list.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:50:48.306882 peek-core-email-3.4.9/peek_core_email/_private/alembic/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 06:49:47.000000 peek-core-email-3.4.9/peek_core_email/_private/alembic/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      301 2023-07-19 06:49:47.000000 peek-core-email-3.4.9/peek_core_email/_private/alembic/env.py
+-rw-r--r--   0 root         (0) root         (0)      544 2023-07-19 06:49:47.000000 peek-core-email-3.4.9/peek_core_email/_private/alembic/script.py.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:50:48.306882 peek-core-email-3.4.9/peek_core_email/_private/alembic/versions/
+-rw-r--r--   0 root         (0) root         (0)     1863 2023-07-19 06:49:47.000000 peek-core-email-3.4.9/peek_core_email/_private/alembic/versions/616e295c146d_initial.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 06:49:47.000000 peek-core-email-3.4.9/peek_core_email/_private/alembic/versions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       96 2023-07-19 06:49:47.000000 peek-core-email-3.4.9/peek_core_email/_private/alembic.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:50:48.306882 peek-core-email-3.4.9/peek_core_email/_private/server/
+-rw-r--r--   0 root         (0) root         (0)     2160 2023-07-19 06:49:47.000000 peek-core-email-3.4.9/peek_core_email/_private/server/EmailApi.py
+-rw-r--r--   0 root         (0) root         (0)     1533 2023-07-19 06:49:47.000000 peek-core-email-3.4.9/peek_core_email/_private/server/EmailUtil.py
+-rw-r--r--   0 root         (0) root         (0)     1716 2023-07-19 06:49:47.000000 peek-core-email-3.4.9/peek_core_email/_private/server/PluginLogicEntryHook.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 06:49:47.000000 peek-core-email-3.4.9/peek_core_email/_private/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:50:48.306882 peek-core-email-3.4.9/peek_core_email/_private/server/admin_backend/
+-rw-r--r--   0 root         (0) root         (0)      970 2023-07-19 06:49:47.000000 peek-core-email-3.4.9/peek_core_email/_private/server/admin_backend/PeekAdmSettingHandler.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 06:49:47.000000 peek-core-email-3.4.9/peek_core_email/_private/server/admin_backend/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:50:48.307882 peek-core-email-3.4.9/peek_core_email/_private/storage/
+-rw-r--r--   0 root         (0) root         (0)      275 2023-07-19 06:49:47.000000 peek-core-email-3.4.9/peek_core_email/_private/storage/DeclarativeBase.py
+-rw-r--r--   0 root         (0) root         (0)     8274 2023-07-19 06:49:47.000000 peek-core-email-3.4.9/peek_core_email/_private/storage/Setting.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 06:49:47.000000 peek-core-email-3.4.9/peek_core_email/_private/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:50:48.307882 peek-core-email-3.4.9/peek_core_email/admin-doc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:50:48.307882 peek-core-email-3.4.9/peek_core_email/admin-doc/admin_task/
+-rw-r--r--   0 root         (0) root         (0)      423 2023-07-19 06:49:47.000000 peek-core-email-3.4.9/peek_core_email/admin-doc/admin_task/admin_tasks.rst
+-rw-r--r--   0 root         (0) root         (0)    42134 2023-07-19 06:49:47.000000 peek-core-email-3.4.9/peek_core_email/admin-doc/admin_task/edit_email_settings.png
+-rw-r--r--   0 root         (0) root         (0)      233 2023-07-19 06:49:47.000000 peek-core-email-3.4.9/peek_core_email/admin-doc/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:50:48.307882 peek-core-email-3.4.9/peek_core_email/admin-doc/setup/
+-rw-r--r--   0 root         (0) root         (0)    39549 2023-07-19 06:49:47.000000 peek-core-email-3.4.9/peek_core_email/admin-doc/setup/settings.png
+-rw-r--r--   0 root         (0) root         (0)      497 2023-07-19 06:49:47.000000 peek-core-email-3.4.9/peek_core_email/admin-doc/setup/setup.rst
+-rw-r--r--   0 root         (0) root         (0)      698 2023-07-19 06:50:48.000000 peek-core-email-3.4.9/peek_core_email/plugin_package.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:50:48.307882 peek-core-email-3.4.9/peek_core_email/server/
+-rw-r--r--   0 root         (0) root         (0)      775 2023-07-19 06:49:47.000000 peek-core-email-3.4.9/peek_core_email/server/EmailApiABC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 06:49:47.000000 peek-core-email-3.4.9/peek_core_email/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:50:48.305882 peek-core-email-3.4.9/peek_core_email.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      368 2023-07-19 06:50:48.000000 peek-core-email-3.4.9/peek_core_email.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1963 2023-07-19 06:50:48.000000 peek-core-email-3.4.9/peek_core_email.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 06:50:48.000000 peek-core-email-3.4.9/peek_core_email.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-07-19 06:50:48.000000 peek-core-email-3.4.9/peek_core_email.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-19 06:50:48.000000 peek-core-email-3.4.9/peek_core_email.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2023-07-19 06:50:48.308882 peek-core-email-3.4.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2658 2023-07-19 06:50:48.000000 peek-core-email-3.4.9/setup.py
```

### Comparing `peek-core-email-3.4.8/README.rst` & `peek-core-email-3.4.9/README.rst`

 * *Files identical despite different names*

### Comparing `peek-core-email-3.4.8/peek_core_email/__init__.py` & `peek-core-email-3.4.9/peek_core_email/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Type
 
 from peek_plugin_base.client.PluginClientEntryHookABC import PluginClientEntryHookABC
 from peek_plugin_base.server.PluginLogicEntryHookABC import PluginLogicEntryHookABC
 
-__version__ = '3.4.8'
+__version__ = '3.4.9'
 
 
 def peekLogicEntryHook() -> Type[PluginLogicEntryHookABC]:
     from peek_core_email._private.server.PluginLogicEntryHook import (
         PluginLogicEntryHook,
     )
```

### Comparing `peek-core-email-3.4.8/peek_core_email/_private/admin-app/core-email-admin.component.html` & `peek-core-email-3.4.9/peek_core_email/_private/admin-app/core-email-admin.component.html`

 * *Files identical despite different names*

### Comparing `peek-core-email-3.4.8/peek_core_email/_private/admin-app/core-email.module.ts` & `peek-core-email-3.4.9/peek_core_email/_private/admin-app/core-email.module.ts`

 * *Files identical despite different names*

### Comparing `peek-core-email-3.4.8/peek_core_email/_private/admin-app/setting-list/admin-setting-list.component.html` & `peek-core-email-3.4.9/peek_core_email/_private/admin-app/setting-list/admin-setting-list.component.html`

 * *Files identical despite different names*

### Comparing `peek-core-email-3.4.8/peek_core_email/_private/admin-app/setting-list/admin-setting-list.component.ts` & `peek-core-email-3.4.9/peek_core_email/_private/admin-app/setting-list/admin-setting-list.component.ts`

 * *Files identical despite different names*

### Comparing `peek-core-email-3.4.8/peek_core_email/_private/alembic/script.py.mako` & `peek-core-email-3.4.9/peek_core_email/_private/alembic/script.py.mako`

 * *Files identical despite different names*

### Comparing `peek-core-email-3.4.8/peek_core_email/_private/alembic/versions/616e295c146d_initial.py` & `peek-core-email-3.4.9/peek_core_email/_private/alembic/versions/616e295c146d_initial.py`

 * *Files identical despite different names*

### Comparing `peek-core-email-3.4.8/peek_core_email/_private/server/EmailApi.py` & `peek-core-email-3.4.9/peek_core_email/_private/server/EmailApi.py`

 * *Files identical despite different names*

### Comparing `peek-core-email-3.4.8/peek_core_email/_private/server/EmailUtil.py` & `peek-core-email-3.4.9/peek_core_email/_private/server/EmailUtil.py`

 * *Files identical despite different names*

### Comparing `peek-core-email-3.4.8/peek_core_email/_private/server/PluginLogicEntryHook.py` & `peek-core-email-3.4.9/peek_core_email/_private/server/PluginLogicEntryHook.py`

 * *Files identical despite different names*

### Comparing `peek-core-email-3.4.8/peek_core_email/_private/server/admin_backend/PeekAdmSettingHandler.py` & `peek-core-email-3.4.9/peek_core_email/_private/server/admin_backend/PeekAdmSettingHandler.py`

 * *Files identical despite different names*

### Comparing `peek-core-email-3.4.8/peek_core_email/_private/storage/Setting.py` & `peek-core-email-3.4.9/peek_core_email/_private/storage/Setting.py`

 * *Files identical despite different names*

### Comparing `peek-core-email-3.4.8/peek_core_email/admin-doc/admin_task/edit_email_settings.png` & `peek-core-email-3.4.9/peek_core_email/admin-doc/admin_task/edit_email_settings.png`

 * *Files identical despite different names*

### Comparing `peek-core-email-3.4.8/peek_core_email/admin-doc/setup/settings.png` & `peek-core-email-3.4.9/peek_core_email/admin-doc/setup/settings.png`

 * *Files identical despite different names*

### Comparing `peek-core-email-3.4.8/peek_core_email/plugin_package.json` & `peek-core-email-3.4.9/peek_core_email/plugin_package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9940476190476191%*

 * *Differences: {"'plugin'": "{'version': '3.4.9'}"}*

```diff
@@ -12,15 +12,15 @@
     "logic": {},
     "plugin": {
         "buildDate": "#BUILD_DATE#",
         "buildNumber": "#PLUGIN_BUILD#",
         "creator": "Synerty Pty Ltd",
         "packageName": "peek_core_email",
         "title": "Email",
-        "version": "3.4.8",
+        "version": "3.4.9",
         "website": "www.synerty.com"
     },
     "requiresServices": [
         "logic",
         "admin",
         "storage",
         "admin-doc"
```

### Comparing `peek-core-email-3.4.8/peek_core_email/server/EmailApiABC.py` & `peek-core-email-3.4.9/peek_core_email/server/EmailApiABC.py`

 * *Files identical despite different names*

### Comparing `peek-core-email-3.4.8/peek_core_email.egg-info/SOURCES.txt` & `peek-core-email-3.4.9/peek_core_email.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peek-core-email-3.4.8/setup.py` & `peek-core-email-3.4.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # Modify these values to fork a new plugin
 #
 
 author = "Synerty"
 author_email = "contact@synerty.com"
 py_package_name = "peek_core_email"
 pip_package_name = py_package_name.replace("_", "-")
-package_version = "3.4.8"
+package_version = "3.4.9"
 description = "Peek Core Plugin Email."
 
 download_url = "https://bitbucket.org/synerty/%s/get/%s.zip"
 download_url %= pip_package_name, package_version
 url = "https://bitbucket.org/synerty/%s" % pip_package_name
 
 ###############################################################################
```

