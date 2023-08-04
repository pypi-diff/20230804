# Comparing `tmp/peek-plugin-inbox-3.4.8.tar.gz` & `tmp/peek-plugin-inbox-3.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peek-plugin-inbox-3.4.8.tar", last modified: Tue Jul 11 02:54:06 2023, max compression
+gzip compressed data, was "peek-plugin-inbox-3.4.9.tar", last modified: Wed Jul 19 06:52:50 2023, max compression
```

## Comparing `peek-plugin-inbox-3.4.8.tar` & `peek-plugin-inbox-3.4.9.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:54:06.360872 peek-plugin-inbox-3.4.8/
--rw-r--r--   0 root         (0) root         (0)      369 2023-07-11 02:54:06.361872 peek-plugin-inbox-3.4.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      899 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:54:06.355872 peek-plugin-inbox-3.4.8/peek_plugin_inbox/
--rw-r--r--   0 root         (0) root         (0)      271 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/TempUnitTest.py
--rw-r--r--   0 root         (0) root         (0)      836 2023-07-11 02:54:06.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:54:06.355872 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/
--rw-r--r--   0 root         (0) root         (0)      210 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/PluginNames.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:54:06.356872 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/admin-app/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:54:06.356872 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/admin-app/activity-list/
--rw-r--r--   0 root         (0) root         (0)     1112 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/admin-app/activity-list/admin-activity-list.component.html
--rw-r--r--   0 root         (0) root         (0)     1259 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/admin-app/activity-list/admin-activity-list.component.ts
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/admin-app/plugin-inbox-admin.component.css
--rw-r--r--   0 root         (0) root         (0)     2683 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/admin-app/plugin-inbox-admin.component.html
--rw-r--r--   0 root         (0) root         (0)      290 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/admin-app/plugin-inbox-admin.component.ts
--rw-r--r--   0 root         (0) root         (0)     2671 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/admin-app/plugin-inbox.module.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:54:06.356872 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/admin-app/send-test-activity/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/admin-app/send-test-activity/send-test-activity.component.css
--rw-r--r--   0 root         (0) root         (0)     3060 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/admin-app/send-test-activity/send-test-activity.component.html
--rw-r--r--   0 root         (0) root         (0)     1581 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/admin-app/send-test-activity/send-test-activity.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:54:06.356872 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/admin-app/send-test-task/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/admin-app/send-test-task/send-test-task.component.css
--rw-r--r--   0 root         (0) root         (0)     8647 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/admin-app/send-test-task/send-test-task.component.html
--rw-r--r--   0 root         (0) root         (0)     2662 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/admin-app/send-test-task/send-test-task.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:54:06.356872 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/admin-app/setting-list/
--rw-r--r--   0 root         (0) root         (0)     1496 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/admin-app/setting-list/admin-setting-list.component.html
--rw-r--r--   0 root         (0) root         (0)     1119 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/admin-app/setting-list/admin-setting-list.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:54:06.356872 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/admin-app/task-list/
--rw-r--r--   0 root         (0) root         (0)     1022 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/admin-app/task-list/admin-task-list.component.html
--rw-r--r--   0 root         (0) root         (0)     1210 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/admin-app/task-list/admin-task-list.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:54:06.357872 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/alembic/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/alembic/__init__.py
--rw-r--r--   0 root         (0) root         (0)      305 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/alembic/env.py
--rw-r--r--   0 root         (0) root         (0)      544 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/alembic/script.py.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:54:06.357872 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/alembic/versions/
--rw-r--r--   0 root         (0) root         (0)     5253 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/alembic/versions/0f8cf37f3af3_created_new_tables.py
--rw-r--r--   0 root         (0) root         (0)     1324 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/alembic/versions/2119b6aab2c5_timezone_aware.py
--rw-r--r--   0 root         (0) root         (0)      813 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/alembic/versions/297359a078eb_added_task_autodelete_time.py
--rw-r--r--   0 root         (0) root         (0)      558 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/alembic/versions/36a9bc546606_fix_task_priorities.py
--rw-r--r--   0 root         (0) root         (0)     8035 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/alembic/versions/3e75fb851c5a_removed_all_tables.py
--rw-r--r--   0 root         (0) root         (0)      807 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/alembic/versions/543ec701c9f7_added_ondialogconfirmpayload.py
--rw-r--r--   0 root         (0) root         (0)     1848 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/alembic/versions/7e6bd0411082_added_pluginname.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/alembic/versions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1012 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/alembic/versions/da155db8b8f1_added_task_displaypriority.py
--rw-r--r--   0 root         (0) root         (0)     5175 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/alembic/versions/db5936c4d50d_initial_table_creation.py
--rw-r--r--   0 root         (0) root         (0)     1985 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/alembic/versions/deab93942032_payload_envelope.py
--rw-r--r--   0 root         (0) root         (0)       96 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/alembic.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:54:06.357872 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/client/
--rw-r--r--   0 root         (0) root         (0)      444 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/client/ClientFeTupleActionProcessorProxy.py
--rw-r--r--   0 root         (0) root         (0)      449 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/client/ClientFeTupleDataObservableProxy.py
--rw-r--r--   0 root         (0) root         (0)     1207 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/client/PluginClientEntryHook.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:54:06.357872 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/mobile-app/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:54:06.358872 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/mobile-app/activity-list/
--rw-r--r--   0 root         (0) root         (0)     2074 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/mobile-app/activity-list/activity-list.component.ts
--rw-r--r--   0 root         (0) root         (0)      949 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/mobile-app/activity-list/activity-list.component.web.html
--rw-r--r--   0 root         (0) root         (0)      637 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/mobile-app/plugin-inbox-client.component.ts
--rw-r--r--   0 root         (0) root         (0)      699 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/mobile-app/plugin-inbox-client.component.web.html
--rw-r--r--   0 root         (0) root         (0)     1230 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/mobile-app/plugin-inbox.module.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:54:06.358872 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/mobile-app/task-list/
--rw-r--r--   0 root         (0) root         (0)     2495 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/mobile-app/task-list/task-list.component.ts
--rw-r--r--   0 root         (0) root         (0)     2474 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/mobile-app/task-list/task-list.component.web.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:54:06.358872 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/mobile-assets/
--rw-r--r--   0 root         (0) root         (0)    97846 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/mobile-assets/alert.mp3
--rw-r--r--   0 root         (0) root         (0)     1539 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/mobile-assets/plugin_icon.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:54:06.358872 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/server/
--rw-r--r--   0 root         (0) root         (0)      566 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/server/ClientTupleActionProcessor.py
--rw-r--r--   0 root         (0) root         (0)      919 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/server/ClientTupleDataObservable.py
--rw-r--r--   0 root         (0) root         (0)     8809 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/server/InboxApi.py
--rw-r--r--   0 root         (0) root         (0)     3792 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/server/PluginLogicEntryHook.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:54:06.358872 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/server/backend/
--rw-r--r--   0 root         (0) root         (0)      976 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/server/backend/PeekAdmSettingHandler.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/server/backend/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:54:06.358872 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/server/controller/
--rw-r--r--   0 root         (0) root         (0)     2173 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/server/controller/AdminTestController.py
--rw-r--r--   0 root         (0) root         (0)    11069 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/server/controller/MainController.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/server/controller/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:54:06.359872 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/server/tuple_providers/
--rw-r--r--   0 root         (0) root         (0)     1079 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/server/tuple_providers/ActivityTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)     1663 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/server/tuple_providers/TaskTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/server/tuple_providers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:54:06.359872 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/storage/
--rw-r--r--   0 root         (0) root         (0)     1747 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/storage/Activity.py
--rw-r--r--   0 root         (0) root         (0)      446 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/storage/DeclarativeBase.py
--rw-r--r--   0 root         (0) root         (0)     7776 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/storage/Setting.py
--rw-r--r--   0 root         (0) root         (0)     4093 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/storage/Task.py
--rw-r--r--   0 root         (0) root         (0)     1720 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/storage/TaskAction.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:54:06.359872 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/tuples/
--rw-r--r--   0 root         (0) root         (0)      340 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/tuples/AdminSendTestActivityActionTuple.py
--rw-r--r--   0 root         (0) root         (0)      331 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/tuples/AdminSendTestTaskActionTuple.py
--rw-r--r--   0 root         (0) root         (0)      348 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/tuples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:54:06.359872 peek-plugin-inbox-3.4.8/peek_plugin_inbox/admin-doc/
--rw-r--r--   0 root         (0) root         (0)    86000 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/admin-doc/design_diagram.png
--rw-r--r--   0 root         (0) root         (0)     1653 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/admin-doc/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:54:06.359872 peek-plugin-inbox-3.4.8/peek_plugin_inbox/both-doc/
--rw-r--r--   0 root         (0) root         (0)      234 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/both-doc/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:54:06.359872 peek-plugin-inbox-3.4.8/peek_plugin_inbox/plugin-module/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:54:06.360872 peek-plugin-inbox-3.4.8/peek_plugin_inbox/plugin-module/_private/
--rw-r--r--   0 root         (0) root         (0)      180 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/plugin-module/_private/index.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:54:06.360872 peek-plugin-inbox-3.4.8/peek_plugin_inbox/plugin-module/_private/notifiers/
--rw-r--r--   0 root         (0) root         (0)     2711 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/plugin-module/_private/notifiers/native-notifier.ts
--rw-r--r--   0 root         (0) root         (0)       94 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/plugin-module/_private/notifiers/notifier.interface.ts
--rw-r--r--   0 root         (0) root         (0)      845 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/plugin-module/_private/notifiers/web-notifier.ts
--rw-r--r--   0 root         (0) root         (0)    10414 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/plugin-module/_private/plugin-inbox-root.service.ts
--rw-r--r--   0 root         (0) root         (0)     5396 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/plugin-module/_private/private-inbox-tuple-provider.service.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:54:06.360872 peek-plugin-inbox-3.4.8/peek_plugin_inbox/plugin-module/_private/tuples/
--rw-r--r--   0 root         (0) root         (0)      419 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/plugin-module/_private/tuples/AdminSendTestActivityActionTuple.ts
--rw-r--r--   0 root         (0) root         (0)      407 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/plugin-module/_private/tuples/AdminSendTestTaskActionTuple.ts
--rw-r--r--   0 root         (0) root         (0)      283 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/plugin-module/index.ts
--rw-r--r--   0 root         (0) root         (0)       66 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/plugin-module/package.json
--rw-r--r--   0 root         (0) root         (0)      379 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/plugin-module/plugin-inbox-names.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:54:06.360872 peek-plugin-inbox-3.4.8/peek_plugin_inbox/plugin-module/tuples/
--rw-r--r--   0 root         (0) root         (0)      629 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/plugin-module/tuples/ActivityTuple.ts
--rw-r--r--   0 root         (0) root         (0)      395 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/plugin-module/tuples/TaskActionTuple.ts
--rw-r--r--   0 root         (0) root         (0)     4815 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/plugin-module/tuples/TaskTuple.ts
--rw-r--r--   0 root         (0) root         (0)     1710 2023-07-11 02:54:06.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/plugin_package.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:54:06.360872 peek-plugin-inbox-3.4.8/peek_plugin_inbox/server/
--rw-r--r--   0 root         (0) root         (0)    13813 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/server/InboxApiABC.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:54:06.360872 peek-plugin-inbox-3.4.8/peek_plugin_inbox/tuples/
--rw-r--r--   0 root         (0) root         (0)     1079 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/tuples/ActivityTuple.py
--rw-r--r--   0 root         (0) root         (0)     1858 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/tuples/TaskTuple.py
--rw-r--r--   0 root         (0) root         (0)      345 2023-07-11 02:51:13.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox/tuples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:54:06.355872 peek-plugin-inbox-3.4.8/peek_plugin_inbox.egg-info/
--rw-r--r--   0 root         (0) root         (0)      369 2023-07-11 02:54:06.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6067 2023-07-11 02:54:06.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 02:54:06.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-07-11 02:54:06.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-11 02:54:06.000000 peek-plugin-inbox-3.4.8/peek_plugin_inbox.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       80 2023-07-11 02:54:06.362872 peek-plugin-inbox-3.4.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2655 2023-07-11 02:54:06.000000 peek-plugin-inbox-3.4.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:52:50.079135 peek-plugin-inbox-3.4.9/
+-rw-r--r--   0 root         (0) root         (0)      369 2023-07-19 06:52:50.079135 peek-plugin-inbox-3.4.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      899 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:52:50.074135 peek-plugin-inbox-3.4.9/peek_plugin_inbox/
+-rw-r--r--   0 root         (0) root         (0)      271 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/TempUnitTest.py
+-rw-r--r--   0 root         (0) root         (0)      836 2023-07-19 06:52:49.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:52:50.074135 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/
+-rw-r--r--   0 root         (0) root         (0)      210 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/PluginNames.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:52:50.074135 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/admin-app/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:52:50.075135 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/admin-app/activity-list/
+-rw-r--r--   0 root         (0) root         (0)     1112 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/admin-app/activity-list/admin-activity-list.component.html
+-rw-r--r--   0 root         (0) root         (0)     1259 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/admin-app/activity-list/admin-activity-list.component.ts
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/admin-app/plugin-inbox-admin.component.css
+-rw-r--r--   0 root         (0) root         (0)     2683 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/admin-app/plugin-inbox-admin.component.html
+-rw-r--r--   0 root         (0) root         (0)      290 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/admin-app/plugin-inbox-admin.component.ts
+-rw-r--r--   0 root         (0) root         (0)     2671 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/admin-app/plugin-inbox.module.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:52:50.075135 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/admin-app/send-test-activity/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/admin-app/send-test-activity/send-test-activity.component.css
+-rw-r--r--   0 root         (0) root         (0)     3060 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/admin-app/send-test-activity/send-test-activity.component.html
+-rw-r--r--   0 root         (0) root         (0)     1581 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/admin-app/send-test-activity/send-test-activity.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:52:50.075135 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/admin-app/send-test-task/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/admin-app/send-test-task/send-test-task.component.css
+-rw-r--r--   0 root         (0) root         (0)     8647 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/admin-app/send-test-task/send-test-task.component.html
+-rw-r--r--   0 root         (0) root         (0)     2662 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/admin-app/send-test-task/send-test-task.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:52:50.075135 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/admin-app/setting-list/
+-rw-r--r--   0 root         (0) root         (0)     1496 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/admin-app/setting-list/admin-setting-list.component.html
+-rw-r--r--   0 root         (0) root         (0)     1119 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/admin-app/setting-list/admin-setting-list.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:52:50.075135 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/admin-app/task-list/
+-rw-r--r--   0 root         (0) root         (0)     1022 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/admin-app/task-list/admin-task-list.component.html
+-rw-r--r--   0 root         (0) root         (0)     1210 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/admin-app/task-list/admin-task-list.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:52:50.075135 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/alembic/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/alembic/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      305 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/alembic/env.py
+-rw-r--r--   0 root         (0) root         (0)      544 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/alembic/script.py.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:52:50.076135 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/alembic/versions/
+-rw-r--r--   0 root         (0) root         (0)     5253 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/alembic/versions/0f8cf37f3af3_created_new_tables.py
+-rw-r--r--   0 root         (0) root         (0)     1324 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/alembic/versions/2119b6aab2c5_timezone_aware.py
+-rw-r--r--   0 root         (0) root         (0)      813 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/alembic/versions/297359a078eb_added_task_autodelete_time.py
+-rw-r--r--   0 root         (0) root         (0)      558 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/alembic/versions/36a9bc546606_fix_task_priorities.py
+-rw-r--r--   0 root         (0) root         (0)     8035 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/alembic/versions/3e75fb851c5a_removed_all_tables.py
+-rw-r--r--   0 root         (0) root         (0)      807 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/alembic/versions/543ec701c9f7_added_ondialogconfirmpayload.py
+-rw-r--r--   0 root         (0) root         (0)     1848 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/alembic/versions/7e6bd0411082_added_pluginname.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/alembic/versions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/alembic/versions/da155db8b8f1_added_task_displaypriority.py
+-rw-r--r--   0 root         (0) root         (0)     5175 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/alembic/versions/db5936c4d50d_initial_table_creation.py
+-rw-r--r--   0 root         (0) root         (0)     1985 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/alembic/versions/deab93942032_payload_envelope.py
+-rw-r--r--   0 root         (0) root         (0)       96 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/alembic.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:52:50.076135 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/client/
+-rw-r--r--   0 root         (0) root         (0)      444 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/client/ClientFeTupleActionProcessorProxy.py
+-rw-r--r--   0 root         (0) root         (0)      449 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/client/ClientFeTupleDataObservableProxy.py
+-rw-r--r--   0 root         (0) root         (0)     1207 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/client/PluginClientEntryHook.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:52:50.076135 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/mobile-app/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:52:50.076135 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/mobile-app/activity-list/
+-rw-r--r--   0 root         (0) root         (0)     2074 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/mobile-app/activity-list/activity-list.component.ts
+-rw-r--r--   0 root         (0) root         (0)      949 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/mobile-app/activity-list/activity-list.component.web.html
+-rw-r--r--   0 root         (0) root         (0)      637 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/mobile-app/plugin-inbox-client.component.ts
+-rw-r--r--   0 root         (0) root         (0)      699 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/mobile-app/plugin-inbox-client.component.web.html
+-rw-r--r--   0 root         (0) root         (0)     1230 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/mobile-app/plugin-inbox.module.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:52:50.076135 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/mobile-app/task-list/
+-rw-r--r--   0 root         (0) root         (0)     2495 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/mobile-app/task-list/task-list.component.ts
+-rw-r--r--   0 root         (0) root         (0)     2474 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/mobile-app/task-list/task-list.component.web.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:52:50.077135 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/mobile-assets/
+-rw-r--r--   0 root         (0) root         (0)    97846 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/mobile-assets/alert.mp3
+-rw-r--r--   0 root         (0) root         (0)     1539 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/mobile-assets/plugin_icon.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:52:50.077135 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/server/
+-rw-r--r--   0 root         (0) root         (0)      566 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/server/ClientTupleActionProcessor.py
+-rw-r--r--   0 root         (0) root         (0)      919 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/server/ClientTupleDataObservable.py
+-rw-r--r--   0 root         (0) root         (0)     8809 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/server/InboxApi.py
+-rw-r--r--   0 root         (0) root         (0)     3792 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/server/PluginLogicEntryHook.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:52:50.077135 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/server/backend/
+-rw-r--r--   0 root         (0) root         (0)      976 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/server/backend/PeekAdmSettingHandler.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/server/backend/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:52:50.077135 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/server/controller/
+-rw-r--r--   0 root         (0) root         (0)     2173 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/server/controller/AdminTestController.py
+-rw-r--r--   0 root         (0) root         (0)    11069 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/server/controller/MainController.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/server/controller/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:52:50.077135 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/server/tuple_providers/
+-rw-r--r--   0 root         (0) root         (0)     1079 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/server/tuple_providers/ActivityTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)     1663 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/server/tuple_providers/TaskTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/server/tuple_providers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:52:50.078135 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/storage/
+-rw-r--r--   0 root         (0) root         (0)     1747 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/storage/Activity.py
+-rw-r--r--   0 root         (0) root         (0)      446 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/storage/DeclarativeBase.py
+-rw-r--r--   0 root         (0) root         (0)     7776 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/storage/Setting.py
+-rw-r--r--   0 root         (0) root         (0)     4093 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/storage/Task.py
+-rw-r--r--   0 root         (0) root         (0)     1720 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/storage/TaskAction.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:52:50.078135 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/tuples/
+-rw-r--r--   0 root         (0) root         (0)      340 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/tuples/AdminSendTestActivityActionTuple.py
+-rw-r--r--   0 root         (0) root         (0)      331 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/tuples/AdminSendTestTaskActionTuple.py
+-rw-r--r--   0 root         (0) root         (0)      348 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/tuples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:52:50.078135 peek-plugin-inbox-3.4.9/peek_plugin_inbox/admin-doc/
+-rw-r--r--   0 root         (0) root         (0)    86000 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/admin-doc/design_diagram.png
+-rw-r--r--   0 root         (0) root         (0)     1653 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/admin-doc/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:52:50.078135 peek-plugin-inbox-3.4.9/peek_plugin_inbox/both-doc/
+-rw-r--r--   0 root         (0) root         (0)      234 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/both-doc/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:52:50.078135 peek-plugin-inbox-3.4.9/peek_plugin_inbox/plugin-module/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:52:50.078135 peek-plugin-inbox-3.4.9/peek_plugin_inbox/plugin-module/_private/
+-rw-r--r--   0 root         (0) root         (0)      180 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/plugin-module/_private/index.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:52:50.078135 peek-plugin-inbox-3.4.9/peek_plugin_inbox/plugin-module/_private/notifiers/
+-rw-r--r--   0 root         (0) root         (0)     2711 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/plugin-module/_private/notifiers/native-notifier.ts
+-rw-r--r--   0 root         (0) root         (0)       94 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/plugin-module/_private/notifiers/notifier.interface.ts
+-rw-r--r--   0 root         (0) root         (0)      845 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/plugin-module/_private/notifiers/web-notifier.ts
+-rw-r--r--   0 root         (0) root         (0)    10414 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/plugin-module/_private/plugin-inbox-root.service.ts
+-rw-r--r--   0 root         (0) root         (0)     5396 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/plugin-module/_private/private-inbox-tuple-provider.service.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:52:50.079135 peek-plugin-inbox-3.4.9/peek_plugin_inbox/plugin-module/_private/tuples/
+-rw-r--r--   0 root         (0) root         (0)      419 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/plugin-module/_private/tuples/AdminSendTestActivityActionTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      407 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/plugin-module/_private/tuples/AdminSendTestTaskActionTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      283 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/plugin-module/index.ts
+-rw-r--r--   0 root         (0) root         (0)       66 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/plugin-module/package.json
+-rw-r--r--   0 root         (0) root         (0)      379 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/plugin-module/plugin-inbox-names.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:52:50.079135 peek-plugin-inbox-3.4.9/peek_plugin_inbox/plugin-module/tuples/
+-rw-r--r--   0 root         (0) root         (0)      629 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/plugin-module/tuples/ActivityTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      395 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/plugin-module/tuples/TaskActionTuple.ts
+-rw-r--r--   0 root         (0) root         (0)     4815 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/plugin-module/tuples/TaskTuple.ts
+-rw-r--r--   0 root         (0) root         (0)     1710 2023-07-19 06:52:49.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/plugin_package.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:52:50.079135 peek-plugin-inbox-3.4.9/peek_plugin_inbox/server/
+-rw-r--r--   0 root         (0) root         (0)    13813 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/server/InboxApiABC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:52:50.079135 peek-plugin-inbox-3.4.9/peek_plugin_inbox/tuples/
+-rw-r--r--   0 root         (0) root         (0)     1079 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/tuples/ActivityTuple.py
+-rw-r--r--   0 root         (0) root         (0)     1858 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/tuples/TaskTuple.py
+-rw-r--r--   0 root         (0) root         (0)      345 2023-07-19 06:49:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox/tuples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:52:50.074135 peek-plugin-inbox-3.4.9/peek_plugin_inbox.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      369 2023-07-19 06:52:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6067 2023-07-19 06:52:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 06:52:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-07-19 06:52:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-19 06:52:50.000000 peek-plugin-inbox-3.4.9/peek_plugin_inbox.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2023-07-19 06:52:50.080135 peek-plugin-inbox-3.4.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2655 2023-07-19 06:52:49.000000 peek-plugin-inbox-3.4.9/setup.py
```

### Comparing `peek-plugin-inbox-3.4.8/README.rst` & `peek-plugin-inbox-3.4.9/README.rst`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.4.8/peek_plugin_inbox/__init__.py` & `peek-plugin-inbox-3.4.9/peek_plugin_inbox/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Type
 
 from peek_plugin_base.client.PluginClientEntryHookABC import PluginClientEntryHookABC
 from peek_plugin_base.server.PluginLogicEntryHookABC import PluginLogicEntryHookABC
 
-__version__ = '3.4.8'
+__version__ = '3.4.9'
 
 
 def peekLogicEntryHook() -> Type[PluginLogicEntryHookABC]:
     from peek_plugin_inbox._private.server.PluginLogicEntryHook import (
         PluginLogicEntryHook,
     )
```

### Comparing `peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/admin-app/activity-list/admin-activity-list.component.html` & `peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/admin-app/activity-list/admin-activity-list.component.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/admin-app/activity-list/admin-activity-list.component.ts` & `peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/admin-app/activity-list/admin-activity-list.component.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/admin-app/plugin-inbox-admin.component.html` & `peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/admin-app/plugin-inbox-admin.component.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/admin-app/plugin-inbox.module.ts` & `peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/admin-app/plugin-inbox.module.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/admin-app/send-test-activity/send-test-activity.component.html` & `peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/admin-app/send-test-activity/send-test-activity.component.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/admin-app/send-test-activity/send-test-activity.component.ts` & `peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/admin-app/send-test-activity/send-test-activity.component.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/admin-app/send-test-task/send-test-task.component.html` & `peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/admin-app/send-test-task/send-test-task.component.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/admin-app/send-test-task/send-test-task.component.ts` & `peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/admin-app/send-test-task/send-test-task.component.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/admin-app/setting-list/admin-setting-list.component.html` & `peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/admin-app/setting-list/admin-setting-list.component.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/admin-app/setting-list/admin-setting-list.component.ts` & `peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/admin-app/setting-list/admin-setting-list.component.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/admin-app/task-list/admin-task-list.component.html` & `peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/admin-app/task-list/admin-task-list.component.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/admin-app/task-list/admin-task-list.component.ts` & `peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/admin-app/task-list/admin-task-list.component.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/alembic/script.py.mako` & `peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/alembic/script.py.mako`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/alembic/versions/0f8cf37f3af3_created_new_tables.py` & `peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/alembic/versions/0f8cf37f3af3_created_new_tables.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/alembic/versions/2119b6aab2c5_timezone_aware.py` & `peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/alembic/versions/2119b6aab2c5_timezone_aware.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/alembic/versions/297359a078eb_added_task_autodelete_time.py` & `peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/alembic/versions/297359a078eb_added_task_autodelete_time.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/alembic/versions/36a9bc546606_fix_task_priorities.py` & `peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/alembic/versions/36a9bc546606_fix_task_priorities.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/alembic/versions/3e75fb851c5a_removed_all_tables.py` & `peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/alembic/versions/3e75fb851c5a_removed_all_tables.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/alembic/versions/543ec701c9f7_added_ondialogconfirmpayload.py` & `peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/alembic/versions/543ec701c9f7_added_ondialogconfirmpayload.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/alembic/versions/7e6bd0411082_added_pluginname.py` & `peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/alembic/versions/7e6bd0411082_added_pluginname.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/alembic/versions/da155db8b8f1_added_task_displaypriority.py` & `peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/alembic/versions/da155db8b8f1_added_task_displaypriority.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/alembic/versions/db5936c4d50d_initial_table_creation.py` & `peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/alembic/versions/db5936c4d50d_initial_table_creation.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/alembic/versions/deab93942032_payload_envelope.py` & `peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/alembic/versions/deab93942032_payload_envelope.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/client/PluginClientEntryHook.py` & `peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/client/PluginClientEntryHook.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/mobile-app/activity-list/activity-list.component.ts` & `peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/mobile-app/activity-list/activity-list.component.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/mobile-app/activity-list/activity-list.component.web.html` & `peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/mobile-app/activity-list/activity-list.component.web.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/mobile-app/plugin-inbox-client.component.ts` & `peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/mobile-app/plugin-inbox-client.component.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/mobile-app/plugin-inbox-client.component.web.html` & `peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/mobile-app/plugin-inbox-client.component.web.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/mobile-app/plugin-inbox.module.ts` & `peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/mobile-app/plugin-inbox.module.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/mobile-app/task-list/task-list.component.ts` & `peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/mobile-app/task-list/task-list.component.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/mobile-app/task-list/task-list.component.web.html` & `peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/mobile-app/task-list/task-list.component.web.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/mobile-assets/alert.mp3` & `peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/mobile-assets/alert.mp3`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/mobile-assets/plugin_icon.png` & `peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/mobile-assets/plugin_icon.png`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/server/ClientTupleActionProcessor.py` & `peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/server/ClientTupleActionProcessor.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/server/ClientTupleDataObservable.py` & `peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/server/ClientTupleDataObservable.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/server/InboxApi.py` & `peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/server/InboxApi.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/server/PluginLogicEntryHook.py` & `peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/server/PluginLogicEntryHook.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/server/backend/PeekAdmSettingHandler.py` & `peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/server/backend/PeekAdmSettingHandler.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/server/controller/AdminTestController.py` & `peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/server/controller/AdminTestController.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/server/controller/MainController.py` & `peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/server/controller/MainController.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/server/tuple_providers/ActivityTupleProvider.py` & `peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/server/tuple_providers/ActivityTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/server/tuple_providers/TaskTupleProvider.py` & `peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/server/tuple_providers/TaskTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/storage/Activity.py` & `peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/storage/Activity.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/storage/Setting.py` & `peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/storage/Setting.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/storage/Task.py` & `peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/storage/Task.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.4.8/peek_plugin_inbox/_private/storage/TaskAction.py` & `peek-plugin-inbox-3.4.9/peek_plugin_inbox/_private/storage/TaskAction.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.4.8/peek_plugin_inbox/admin-doc/design_diagram.png` & `peek-plugin-inbox-3.4.9/peek_plugin_inbox/admin-doc/design_diagram.png`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.4.8/peek_plugin_inbox/admin-doc/index.rst` & `peek-plugin-inbox-3.4.9/peek_plugin_inbox/admin-doc/index.rst`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.4.8/peek_plugin_inbox/plugin-module/_private/notifiers/native-notifier.ts` & `peek-plugin-inbox-3.4.9/peek_plugin_inbox/plugin-module/_private/notifiers/native-notifier.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.4.8/peek_plugin_inbox/plugin-module/_private/notifiers/web-notifier.ts` & `peek-plugin-inbox-3.4.9/peek_plugin_inbox/plugin-module/_private/notifiers/web-notifier.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.4.8/peek_plugin_inbox/plugin-module/_private/plugin-inbox-root.service.ts` & `peek-plugin-inbox-3.4.9/peek_plugin_inbox/plugin-module/_private/plugin-inbox-root.service.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.4.8/peek_plugin_inbox/plugin-module/_private/private-inbox-tuple-provider.service.ts` & `peek-plugin-inbox-3.4.9/peek_plugin_inbox/plugin-module/_private/private-inbox-tuple-provider.service.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.4.8/peek_plugin_inbox/plugin-module/tuples/ActivityTuple.ts` & `peek-plugin-inbox-3.4.9/peek_plugin_inbox/plugin-module/tuples/ActivityTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.4.8/peek_plugin_inbox/plugin-module/tuples/TaskTuple.ts` & `peek-plugin-inbox-3.4.9/peek_plugin_inbox/plugin-module/tuples/TaskTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.4.8/peek_plugin_inbox/plugin_package.json` & `peek-plugin-inbox-3.4.9/peek_plugin_inbox/plugin_package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9960317460317462%*

 * *Differences: {"'plugin'": "{'version': '3.4.9'}"}*

```diff
@@ -42,15 +42,15 @@
     },
     "plugin": {
         "buildDate": "#BUILD_DATE#",
         "buildNumber": "#PLUGIN_BUILD#",
         "creator": "Synerty Pty Ltd",
         "packageName": "peek_plugin_inbox",
         "title": "Inbox",
-        "version": "3.4.8",
+        "version": "3.4.9",
         "website": "www.synerty.com"
     },
     "requiresServices": [
         "logic",
         "field",
         "office",
         "storage",
```

### Comparing `peek-plugin-inbox-3.4.8/peek_plugin_inbox/server/InboxApiABC.py` & `peek-plugin-inbox-3.4.9/peek_plugin_inbox/server/InboxApiABC.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.4.8/peek_plugin_inbox/tuples/ActivityTuple.py` & `peek-plugin-inbox-3.4.9/peek_plugin_inbox/tuples/ActivityTuple.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.4.8/peek_plugin_inbox/tuples/TaskTuple.py` & `peek-plugin-inbox-3.4.9/peek_plugin_inbox/tuples/TaskTuple.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.4.8/peek_plugin_inbox.egg-info/SOURCES.txt` & `peek-plugin-inbox-3.4.9/peek_plugin_inbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peek-plugin-inbox-3.4.8/setup.py` & `peek-plugin-inbox-3.4.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # Modify these values to fork a new plugin
 #
 
 author = "Synerty"
 author_email = "contact@synerty.com"
 py_package_name = "peek_plugin_inbox"
 pip_package_name = py_package_name.replace("_", "-")
-package_version = "3.4.8"
+package_version = "3.4.9"
 description = "Peek Plugin Inbox."
 
 download_url = "https://bitbucket.org/synerty/%s/get/%s.zip"
 download_url %= pip_package_name, package_version
 url = "https://bitbucket.org/synerty/%s" % pip_package_name
 
 ###############################################################################
```

