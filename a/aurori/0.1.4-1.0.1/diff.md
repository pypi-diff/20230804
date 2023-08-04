# Comparing `tmp/aurori-0.1.4.tar.gz` & `tmp/aurori-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aurori-0.1.4.tar", last modified: Sun Sep 18 11:45:26 2022, max compression
+gzip compressed data, was "aurori-1.0.1.tar", last modified: Fri Aug  4 09:24:06 2023, max compression
```

## Comparing `aurori-0.1.4.tar` & `aurori-1.0.1.tar`

### file list

```diff
@@ -1,212 +1,95 @@
-drwxrwxrwx   0        0        0        0 2022-09-18 11:45:26.089886 aurori-0.1.4/
--rw-rw-rw-   0        0        0       81 2022-09-18 11:13:50.000000 aurori-0.1.4/.gitignore
--rw-rw-rw-   0        0        0     1575 2022-07-26 21:50:23.000000 aurori-0.1.4/.gitlab-ci.yml
-drwxrwxrwx   0        0        0        0 2022-09-18 11:45:25.874887 aurori-0.1.4/.vscode/
--rw-rw-rw-   0        0        0      986 2022-07-28 10:26:45.000000 aurori-0.1.4/.vscode/launch.json
--rw-rw-rw-   0        0        0    35005 2022-08-05 13:57:15.000000 aurori-0.1.4/LICENSE
--rw-rw-rw-   0        0        0      633 2022-09-18 11:45:26.090885 aurori-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0       75 2022-08-05 14:13:14.000000 aurori-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2022-09-18 11:45:25.885887 aurori-0.1.4/aurori/
--rw-rw-rw-   0        0        0    35005 2022-08-05 07:33:15.000000 aurori-0.1.4/aurori/LICENSE.md
--rw-rw-rw-   0        0        0       75 2022-08-05 14:15:01.000000 aurori-0.1.4/aurori/README.md
--rw-rw-rw-   0        0        0     6232 2022-09-05 06:45:39.000000 aurori-0.1.4/aurori/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-18 11:45:25.920886 aurori-0.1.4/aurori/actions/
--rw-rw-rw-   0        0        0     1618 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/actions/__init__.py
--rw-rw-rw-   0        0        0     1489 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/actions/action.py
--rw-rw-rw-   0        0        0     1393 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/actions/actionGenerator.py
--rw-rw-rw-   0        0        0    10306 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/actions/actionManager.py
--rw-rw-rw-   0        0        0     1722 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/actions/models.py
--rw-rw-rw-   0        0        0      951 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/actions/routes.py
--rw-rw-rw-   0        0        0     3356 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/actions/webclientActions.py
--rw-rw-rw-   0        0        0     2049 2022-01-25 10:07:21.000000 aurori-0.1.4/aurori/alembic.ini
-drwxrwxrwx   0        0        0        0 2022-09-18 11:45:25.926886 aurori-0.1.4/aurori/api/
--rw-rw-rw-   0        0        0      936 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/api/__init__.py
--rw-rw-rw-   0        0        0     2191 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/api/check.py
--rw-rw-rw-   0        0        0     1839 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/api/decorator.py
--rw-rw-rw-   0        0        0     3397 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/api/routes.py
-drwxrwxrwx   0        0        0        0 2022-09-18 11:45:25.932886 aurori-0.1.4/aurori/common/
--rw-rw-rw-   0        0        0      833 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/common/__init__.py
--rw-rw-rw-   0        0        0     1567 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/common/intEnum.py
--rw-rw-rw-   0        0        0     1499 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/common/intFlag.py
--rw-rw-rw-   0        0        0     1401 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/common/jsonDict.py
--rw-rw-rw-   0        0        0     1579 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/common/objDict.py
--rw-rw-rw-   0        0        0     5156 2022-08-05 07:31:42.000000 aurori-0.1.4/aurori/config.py
--rw-rw-rw-   0        0        0      926 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/exceptions.py
-drwxrwxrwx   0        0        0        0 2022-09-18 11:45:25.937886 aurori-0.1.4/aurori/files/
--rw-rw-rw-   0        0        0      202 2022-08-04 21:24:36.000000 aurori-0.1.4/aurori/files/__init__.py
--rw-rw-rw-   0        0        0     1540 2022-08-04 21:24:37.000000 aurori-0.1.4/aurori/files/fileManager.py
--rw-rw-rw-   0        0        0     6193 2022-08-04 21:24:37.000000 aurori-0.1.4/aurori/files/models.py
--rw-rw-rw-   0        0        0     2532 2022-08-04 21:24:37.000000 aurori-0.1.4/aurori/files/routes.py
-drwxrwxrwx   0        0        0        0 2022-09-18 11:45:25.939886 aurori-0.1.4/aurori/files/storage_backends/
--rw-rw-rw-   0        0        0      264 2022-07-19 08:18:08.000000 aurori-0.1.4/aurori/files/storage_backends/base.py
--rw-rw-rw-   0        0        0     1426 2022-08-04 21:24:37.000000 aurori-0.1.4/aurori/files/storage_backends/local.py
-drwxrwxrwx   0        0        0        0 2022-09-18 11:45:25.945884 aurori-0.1.4/aurori/jobs/
--rw-rw-rw-   0        0        0     2745 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/jobs/__init__.py
--rw-rw-rw-   0        0        0     7763 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/jobs/job.py
--rw-rw-rw-   0        0        0     8262 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/jobs/jobManager.py
--rw-rw-rw-   0        0        0     1705 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/jobs/models.py
--rw-rw-rw-   0        0        0      833 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/jobs/routes.py
-drwxrwxrwx   0        0        0        0 2022-09-18 11:45:25.948887 aurori-0.1.4/aurori/logs/
--rw-rw-rw-   0        0        0     1011 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/logs/__init__.py
--rw-rw-rw-   0        0        0     4826 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/logs/logManager.py
--rw-rw-rw-   0        0        0     1067 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/logs/routes.py
-drwxrwxrwx   0        0        0        0 2022-09-18 11:45:25.952885 aurori-0.1.4/aurori/menus/
--rw-rw-rw-   0        0        0     1019 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/menus/__init__.py
--rw-rw-rw-   0        0        0     7433 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/menus/menuBuilder.py
--rw-rw-rw-   0        0        0     1025 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/menus/routes.py
-drwxrwxrwx   0        0        0        0 2022-09-18 11:45:25.958886 aurori-0.1.4/aurori/messages/
--rw-rw-rw-   0        0        0     2224 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/messages/__init__.py
--rw-rw-rw-   0        0        0     3202 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/messages/mailingJob.py
--rw-rw-rw-   0        0        0     3051 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/messages/messageManager.py
--rw-rw-rw-   0        0        0     1826 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/messages/models.py
--rw-rw-rw-   0        0        0     1440 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/messages/routes.py
-drwxrwxrwx   0        0        0        0 2022-09-18 11:45:25.962885 aurori-0.1.4/aurori/migrations/
--rw-rw-rw-   0        0        0      323 2022-02-22 10:25:17.000000 aurori-0.1.4/aurori/migrations/README.md
--rw-rw-rw-   0        0        0     4804 2022-08-04 21:24:37.000000 aurori-0.1.4/aurori/migrations/env.py
--rw-rw-rw-   0        0        0      518 2022-01-25 10:07:21.000000 aurori-0.1.4/aurori/migrations/script.py.mako
-drwxrwxrwx   0        0        0        0 2022-09-18 11:45:25.963886 aurori-0.1.4/aurori/migrations/versions/
--rw-rw-rw-   0        0        0     5218 2022-09-02 14:01:55.000000 aurori-0.1.4/aurori/migrations/versions/00000_initialisation.py
-drwxrwxrwx   0        0        0        0 2022-09-18 11:45:25.978886 aurori-0.1.4/aurori/monits/
--rw-rw-rw-   0        0        0     1041 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/monits/__init__.py
--rw-rw-rw-   0        0        0     1637 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/monits/cleanupMonitorEventsJob.py
--rw-rw-rw-   0        0        0     2285 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/monits/cleanupMonitorItemsJob.py
--rw-rw-rw-   0        0        0     1061 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/monits/events.py
--rw-rw-rw-   0        0        0     2454 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/monits/models.py
--rw-rw-rw-   0        0        0    15964 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/monits/monitManager.py
--rw-rw-rw-   0        0        0     7068 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/monits/monits.py
--rw-rw-rw-   0        0        0      833 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/monits/process.py
--rw-rw-rw-   0        0        0    13308 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/monits/processMonitJob.py
--rw-rw-rw-   0        0        0     1308 2022-09-01 11:25:50.000000 aurori-0.1.4/aurori/monits/triggerMonitProcessingJob.py
--rw-rw-rw-   0        0        0     2593 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/monits/types.py
--rw-rw-rw-   0        0        0     1677 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/monits/views.py
-drwxrwxrwx   0        0        0        0 2022-09-18 11:45:25.985893 aurori-0.1.4/aurori/nodes/
--rw-rw-rw-   0        0        0     1011 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/nodes/__init__.py
--rw-rw-rw-   0        0        0     2540 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/nodes/models.py
--rw-rw-rw-   0        0        0     1727 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/nodes/nodeClass.py
--rw-rw-rw-   0        0        0     2669 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/nodes/nodeManager.py
--rw-rw-rw-   0        0        0     1530 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/nodes/routes.py
-drwxrwxrwx   0        0        0        0 2022-09-18 11:45:25.988885 aurori-0.1.4/aurori/openproject/
--rw-rw-rw-   0        0        0     1176 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/openproject/__init__.py
--rw-rw-rw-   0        0        0     9495 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/openproject/api.py
-drwxrwxrwx   0        0        0        0 2022-09-18 11:45:25.990885 aurori-0.1.4/aurori/openproject/jobs/
--rw-rw-rw-   0        0        0       44 2021-08-24 16:09:25.000000 aurori-0.1.4/aurori/openproject/jobs/__init__.py
--rw-rw-rw-   0        0        0      752 2022-08-04 21:24:37.000000 aurori-0.1.4/aurori/openproject/jobs/create_ticket.py
-drwxrwxrwx   0        0        0        0 2022-09-18 11:45:25.992885 aurori-0.1.4/aurori/openproject/models/
--rw-rw-rw-   0        0        0       38 2022-07-29 08:13:22.000000 aurori-0.1.4/aurori/openproject/models/__init__.py
--rw-rw-rw-   0        0        0      267 2022-08-04 21:24:37.000000 aurori-0.1.4/aurori/openproject/models/openproject.py
--rw-rw-rw-   0        0        0     2530 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/openproject/openprojectManager.py
-drwxrwxrwx   0        0        0        0 2022-09-18 11:45:25.996886 aurori-0.1.4/aurori/pages/
--rw-rw-rw-   0        0        0      940 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/pages/__init__.py
--rw-rw-rw-   0        0        0     1189 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/pages/pageBuilder.py
--rw-rw-rw-   0        0        0     1026 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/pages/routes.py
--rw-rw-rw-   0        0        0     1813 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/routes.py
-drwxrwxrwx   0        0        0        0 2022-09-18 11:45:26.003886 aurori-0.1.4/aurori/users/
--rw-rw-rw-   0        0        0     1060 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/users/__init__.py
--rw-rw-rw-   0        0        0     4434 2022-09-05 07:24:36.000000 aurori-0.1.4/aurori/users/basemodels.py
--rw-rw-rw-   0        0        0     1283 2022-09-05 06:41:37.000000 aurori-0.1.4/aurori/users/defaultmodels.py
--rw-rw-rw-   0        0        0     3358 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/users/routes.py
--rw-rw-rw-   0        0        0     5849 2022-09-05 07:21:13.000000 aurori-0.1.4/aurori/users/userManager.py
--rw-rw-rw-   0        0        0     1193 2022-09-18 11:45:11.000000 aurori-0.1.4/aurori/version.py
-drwxrwxrwx   0        0        0        0 2022-09-18 11:45:26.007886 aurori-0.1.4/aurori/widgets/
--rw-rw-rw-   0        0        0     1042 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/widgets/__init__.py
--rw-rw-rw-   0        0        0     2993 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/widgets/widget.py
--rw-rw-rw-   0        0        0     2730 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/widgets/widgetmanager.py
-drwxrwxrwx   0        0        0        0 2022-09-18 11:45:26.022885 aurori-0.1.4/aurori/workspaces/
--rw-rw-rw-   0        0        0     1214 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/workspaces/__init__.py
--rw-rw-rw-   0        0        0    18696 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/workspaces/dataView.py
--rw-rw-rw-   0        0        0     2597 2022-09-05 06:38:15.000000 aurori-0.1.4/aurori/workspaces/models.py
--rw-rw-rw-   0        0        0     1728 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/workspaces/page.py
--rw-rw-rw-   0        0        0     1056 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/workspaces/permission.py
--rw-rw-rw-   0        0        0     1048 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/workspaces/routes.py
--rw-rw-rw-   0        0        0     1000 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/workspaces/section.py
--rw-rw-rw-   0        0        0    19494 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/workspaces/viewHandler.py
--rw-rw-rw-   0        0        0    18820 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/workspaces/workspace.py
--rw-rw-rw-   0        0        0      953 2022-08-05 14:12:46.000000 aurori-0.1.4/aurori/workspaces/workspaceHooks.py
--rw-rw-rw-   0        0        0    18356 2022-09-18 11:44:39.000000 aurori-0.1.4/aurori/workspaces/workspaceManager.py
-drwxrwxrwx   0        0        0        0 2022-09-18 11:45:25.910889 aurori-0.1.4/aurori.egg-info/
--rw-rw-rw-   0        0        0      633 2022-09-18 11:45:25.000000 aurori-0.1.4/aurori.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5882 2022-09-18 11:45:25.000000 aurori-0.1.4/aurori.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-18 11:45:25.000000 aurori-0.1.4/aurori.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      236 2022-09-18 11:45:25.000000 aurori-0.1.4/aurori.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-09-18 11:45:25.000000 aurori-0.1.4/aurori.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4119 2022-08-04 21:04:02.000000 aurori-0.1.4/aurori_icon.inkscape.svg
--rw-rw-rw-   0        0        0     9474 2022-08-04 21:10:24.000000 aurori-0.1.4/aurori_logo.inkscape.svg
--rw-rw-rw-   0        0        0      414 2022-08-05 11:58:54.000000 aurori-0.1.4/config.ini.template
-drwxrwxrwx   0        0        0        0 2022-09-18 11:45:26.023886 aurori-0.1.4/examples/
--rw-rw-rw-   0        0        0        4 2022-09-02 13:45:54.000000 aurori-0.1.4/examples/.gitignore
-drwxrwxrwx   0        0        0        0 2022-09-18 11:45:26.026887 aurori-0.1.4/examples/EmptyExample/
--rw-rw-rw-   0        0        0      379 2022-09-02 12:42:17.000000 aurori-0.1.4/examples/EmptyExample/.gitignore
--rw-rw-rw-   0        0        0       79 2022-09-02 13:14:21.000000 aurori-0.1.4/examples/EmptyExample/README.md
-drwxrwxrwx   0        0        0        0 2022-09-18 11:45:26.030887 aurori-0.1.4/examples/EmptyExample/backend/
--rw-rw-rw-   0        0        0      348 2022-09-02 15:06:49.000000 aurori-0.1.4/examples/EmptyExample/backend/app.py
--rw-rw-rw-   0        0        0      326 2022-09-02 13:48:11.000000 aurori-0.1.4/examples/EmptyExample/backend/config.ini.template
--rw-rw-rw-   0        0        0     2036 2022-09-05 07:24:44.000000 aurori-0.1.4/examples/EmptyExample/backend/environment.py
-drwxrwxrwx   0        0        0        0 2022-09-18 11:45:25.849889 aurori-0.1.4/examples/EmptyExample/backend/workspaces/
-drwxrwxrwx   0        0        0        0 2022-09-18 11:45:26.032885 aurori-0.1.4/examples/EmptyExample/backend/workspaces/Log/
-drwxrwxrwx   0        0        0        0 2022-09-18 11:45:26.033886 aurori-0.1.4/examples/EmptyExample/backend/workspaces/Log/actions/
--rw-rw-rw-   0        0        0       35 2022-08-05 15:01:00.000000 aurori-0.1.4/examples/EmptyExample/backend/workspaces/Log/actions/README.md
-drwxrwxrwx   0        0        0        0 2022-09-18 11:45:26.035885 aurori-0.1.4/examples/EmptyExample/backend/workspaces/Log/jobs/
--rw-rw-rw-   0        0        0        0 2022-08-05 15:01:00.000000 aurori-0.1.4/examples/EmptyExample/backend/workspaces/Log/jobs/README.md
-drwxrwxrwx   0        0        0        0 2022-09-18 11:45:26.037887 aurori-0.1.4/examples/EmptyExample/backend/workspaces/Log/pages/
--rw-rw-rw-   0        0        0       31 2022-08-05 15:01:00.000000 aurori-0.1.4/examples/EmptyExample/backend/workspaces/Log/pages/README.md
--rw-rw-rw-   0        0        0      740 2022-08-05 15:22:11.000000 aurori-0.1.4/examples/EmptyExample/backend/workspaces/Log/pages/log.py
--rw-rw-rw-   0        0        0      219 2022-08-08 07:46:12.000000 aurori-0.1.4/examples/EmptyExample/backend/workspaces/Log/permissions.py
-drwxrwxrwx   0        0        0        0 2022-09-18 11:45:26.038885 aurori-0.1.4/examples/EmptyExample/backend/workspaces/Log/views/
--rw-rw-rw-   0        0        0       36 2022-08-05 15:01:00.000000 aurori-0.1.4/examples/EmptyExample/backend/workspaces/Log/views/README.md
--rw-rw-rw-   0        0        0      196 2022-08-05 15:26:20.000000 aurori-0.1.4/examples/EmptyExample/backend/workspaces/Log/workspace.py
-drwxrwxrwx   0        0        0        0 2022-09-18 11:45:26.042886 aurori-0.1.4/examples/EmptyExample/backend/workspaces/Users/
-drwxrwxrwx   0        0        0        0 2022-09-18 11:45:26.055885 aurori-0.1.4/examples/EmptyExample/backend/workspaces/Users/actions/
--rw-rw-rw-   0        0        0       35 2022-08-05 15:01:00.000000 aurori-0.1.4/examples/EmptyExample/backend/workspaces/Users/actions/README.md
--rw-rw-rw-   0        0        0     4870 2022-08-05 15:01:00.000000 aurori-0.1.4/examples/EmptyExample/backend/workspaces/Users/actions/login.py
--rw-rw-rw-   0        0        0     1730 2022-08-05 15:28:08.000000 aurori-0.1.4/examples/EmptyExample/backend/workspaces/Users/actions/lostPassword.py
--rw-rw-rw-   0        0        0      828 2022-08-05 15:23:52.000000 aurori-0.1.4/examples/EmptyExample/backend/workspaces/Users/actions/provideMenu.py
--rw-rw-rw-   0        0        0     2105 2022-09-02 12:21:10.000000 aurori-0.1.4/examples/EmptyExample/backend/workspaces/Users/actions/register.py
--rw-rw-rw-   0        0        0     1667 2022-08-05 15:19:58.000000 aurori-0.1.4/examples/EmptyExample/backend/workspaces/Users/actions/resendVerificationRequest.py
--rw-rw-rw-   0        0        0     1197 2022-09-02 14:45:03.000000 aurori-0.1.4/examples/EmptyExample/backend/workspaces/Users/actions/resetPassword.py
--rw-rw-rw-   0        0        0     1459 2022-08-08 07:52:23.000000 aurori-0.1.4/examples/EmptyExample/backend/workspaces/Users/actions/runActionlink.py
--rw-rw-rw-   0        0        0      699 2022-09-02 14:45:23.000000 aurori-0.1.4/examples/EmptyExample/backend/workspaces/Users/actions/verifyUser.py
-drwxrwxrwx   0        0        0        0 2022-09-18 11:45:26.056886 aurori-0.1.4/examples/EmptyExample/backend/workspaces/Users/jobs/
--rw-rw-rw-   0        0        0        0 2022-08-05 15:01:00.000000 aurori-0.1.4/examples/EmptyExample/backend/workspaces/Users/jobs/README.md
-drwxrwxrwx   0        0        0        0 2022-09-18 11:45:26.060887 aurori-0.1.4/examples/EmptyExample/backend/workspaces/Users/models/
--rw-rw-rw-   0        0        0      281 2022-02-22 15:28:56.000000 aurori-0.1.4/examples/EmptyExample/backend/workspaces/Users/models/README.md
--rw-rw-rw-   0        0        0       83 2022-09-02 14:47:28.000000 aurori-0.1.4/examples/EmptyExample/backend/workspaces/Users/models/__init__.py
--rw-rw-rw-   0        0        0     2049 2022-08-05 15:01:00.000000 aurori-0.1.4/examples/EmptyExample/backend/workspaces/Users/models/alembic.ini
-drwxrwxrwx   0        0        0        0 2022-09-18 11:45:26.065885 aurori-0.1.4/examples/EmptyExample/backend/workspaces/Users/models/migrations/
--rw-rw-rw-   0        0        0       38 2022-08-05 15:01:00.000000 aurori-0.1.4/examples/EmptyExample/backend/workspaces/Users/models/migrations/README
--rw-rw-rw-   0        0        0     4756 2022-09-01 12:23:05.000000 aurori-0.1.4/examples/EmptyExample/backend/workspaces/Users/models/migrations/env.py
--rw-rw-rw-   0        0        0      518 2022-08-05 15:01:00.000000 aurori-0.1.4/examples/EmptyExample/backend/workspaces/Users/models/migrations/script.py.mako
--rw-rw-rw-   0        0        0      265 2022-09-05 07:26:50.000000 aurori-0.1.4/examples/EmptyExample/backend/workspaces/Users/models/user.py
--rw-rw-rw-   0        0        0     1755 2022-08-05 15:01:00.000000 aurori-0.1.4/examples/EmptyExample/backend/workspaces/Users/monits.py
-drwxrwxrwx   0        0        0        0 2022-09-18 11:45:26.068888 aurori-0.1.4/examples/EmptyExample/backend/workspaces/Users/pages/
--rw-rw-rw-   0        0        0       31 2022-08-05 15:01:00.000000 aurori-0.1.4/examples/EmptyExample/backend/workspaces/Users/pages/README.md
--rw-rw-rw-   0        0        0      602 2022-08-05 15:14:48.000000 aurori-0.1.4/examples/EmptyExample/backend/workspaces/Users/pages/users.py
--rw-rw-rw-   0        0        0      162 2022-08-05 15:01:00.000000 aurori-0.1.4/examples/EmptyExample/backend/workspaces/Users/permissions.py
-drwxrwxrwx   0        0        0        0 2022-09-18 11:45:26.074886 aurori-0.1.4/examples/EmptyExample/backend/workspaces/Users/templates/
--rw-rw-rw-   0        0        0      196 2022-08-05 15:01:00.000000 aurori-0.1.4/examples/EmptyExample/backend/workspaces/Users/templates/lostPassword.mail
--rw-rw-rw-   0        0        0      164 2022-08-05 15:01:00.000000 aurori-0.1.4/examples/EmptyExample/backend/workspaces/Users/templates/requestVerification.mail
--rw-rw-rw-   0        0        0      184 2022-08-05 15:01:00.000000 aurori-0.1.4/examples/EmptyExample/backend/workspaces/Users/templates/welcome.mail
--rw-rw-rw-   0        0        0      156 2022-08-05 15:01:00.000000 aurori-0.1.4/examples/EmptyExample/backend/workspaces/Users/templates/welcome.message
-drwxrwxrwx   0        0        0        0 2022-09-18 11:45:26.077886 aurori-0.1.4/examples/EmptyExample/backend/workspaces/Users/views/
--rw-rw-rw-   0        0        0       36 2022-08-05 15:01:00.000000 aurori-0.1.4/examples/EmptyExample/backend/workspaces/Users/views/README.md
--rw-rw-rw-   0        0        0     4322 2022-09-02 14:44:44.000000 aurori-0.1.4/examples/EmptyExample/backend/workspaces/Users/views/userList.py
--rw-rw-rw-   0        0        0     2518 2022-09-02 14:46:30.000000 aurori-0.1.4/examples/EmptyExample/backend/workspaces/Users/views/userLockedList.py
--rw-rw-rw-   0        0        0      188 2022-09-02 14:18:03.000000 aurori-0.1.4/examples/EmptyExample/backend/workspaces/Users/workspace.py
-drwxrwxrwx   0        0        0        0 2022-09-18 11:45:26.080885 aurori-0.1.4/examples/MinimalExample/
--rw-rw-rw-   0        0        0      379 2022-09-02 12:42:19.000000 aurori-0.1.4/examples/MinimalExample/.gitignore
--rw-rw-rw-   0        0        0       86 2022-09-02 12:37:40.000000 aurori-0.1.4/examples/MinimalExample/README.md
-drwxrwxrwx   0        0        0        0 2022-09-18 11:45:26.081886 aurori-0.1.4/examples/MinimalExample/backend/
--rw-rw-rw-   0        0        0       82 2022-09-02 12:38:28.000000 aurori-0.1.4/examples/MinimalExample/backend/app.py
--rw-rw-rw-   0        0        0     1520 2022-09-18 11:09:52.000000 aurori-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0     1015 2022-07-26 16:29:03.000000 aurori-0.1.4/requirements.txt
-drwxrwxrwx   0        0        0        0 2022-09-18 11:45:26.082886 aurori-0.1.4/scripts/
--rw-rw-rw-   0        0        0     2439 2022-08-05 14:12:46.000000 aurori-0.1.4/scripts/quality_report.py
--rw-rw-rw-   0        0        0      516 2022-09-18 11:45:26.094885 aurori-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0       39 2022-07-28 09:17:51.000000 aurori-0.1.4/setup.py
--rw-rw-rw-   0        0        0       88 2022-07-26 22:13:52.000000 aurori-0.1.4/test.py
-drwxrwxrwx   0        0        0        0 2022-09-18 11:45:25.855887 aurori-0.1.4/tests/
-drwxrwxrwx   0        0        0        0 2022-09-18 11:45:26.088886 aurori-0.1.4/tests/api_test/
--rw-rw-rw-   0        0        0       80 2021-08-24 16:09:25.000000 aurori-0.1.4/tests/api_test/action.req
--rw-rw-rw-   0        0        0     2117 2022-07-26 21:50:23.000000 aurori-0.1.4/tests/api_test/action_test.py
--rw-rw-rw-   0        0        0      130 2021-08-24 16:09:25.000000 aurori-0.1.4/tests/api_test/dashboard.req
--rw-rw-rw-   0        0        0      130 2021-08-24 16:09:25.000000 aurori-0.1.4/tests/api_test/login.req
--rw-rw-rw-   0        0        0      135 2021-08-24 16:09:25.000000 aurori-0.1.4/tests/api_test/refresh.req
+drwxrwxrwx   0        0        0        0 2023-08-04 09:24:06.179782 aurori-1.0.1/
+-rw-rw-rw-   0        0        0      100 2023-07-17 04:28:08.000000 aurori-1.0.1/.gitignore
+-rw-rw-rw-   0        0        0     1575 2022-07-26 21:50:23.000000 aurori-1.0.1/.gitlab-ci.yml
+drwxrwxrwx   0        0        0        0 2023-08-04 09:24:06.077782 aurori-1.0.1/.vscode/
+-rw-rw-rw-   0        0        0      986 2022-07-28 10:26:45.000000 aurori-1.0.1/.vscode/launch.json
+-rw-rw-rw-   0        0        0    35005 2022-08-05 13:57:15.000000 aurori-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      615 2023-08-04 09:24:06.180781 aurori-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       75 2022-08-05 14:13:14.000000 aurori-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-04 09:24:06.090782 aurori-1.0.1/aurori/
+-rw-rw-rw-   0        0        0    35005 2022-08-05 07:33:15.000000 aurori-1.0.1/aurori/LICENSE.md
+-rw-rw-rw-   0        0        0       75 2022-08-05 14:15:01.000000 aurori-1.0.1/aurori/README.md
+-rw-rw-rw-   0        0        0     2854 2023-07-28 05:52:22.000000 aurori-1.0.1/aurori/__init__.py
+-rw-rw-rw-   0        0        0     2049 2022-01-25 10:07:21.000000 aurori-1.0.1/aurori/alembic.ini
+drwxrwxrwx   0        0        0        0 2023-08-04 09:24:06.122781 aurori-1.0.1/aurori/api/
+-rw-rw-rw-   0        0        0       33 2023-07-27 08:48:58.000000 aurori-1.0.1/aurori/api/__init__.py
+-rw-rw-rw-   0        0        0      259 2023-07-27 11:58:48.000000 aurori-1.0.1/aurori/api/dependencies.py
+-rw-rw-rw-   0        0        0       56 2023-07-27 10:07:47.000000 aurori-1.0.1/aurori/api/security.py
+drwxrwxrwx   0        0        0        0 2023-08-04 09:24:06.124781 aurori-1.0.1/aurori/cli/
+-rw-rw-rw-   0        0        0      154 2023-07-27 15:09:45.000000 aurori-1.0.1/aurori/cli/__init__.py
+-rw-rw-rw-   0        0        0      216 2023-07-27 15:11:13.000000 aurori-1.0.1/aurori/cli/core.py
+-rw-rw-rw-   0        0        0     5204 2023-07-18 07:21:56.000000 aurori-1.0.1/aurori/config.py
+-rw-rw-rw-   0        0        0      909 2023-07-28 05:43:43.000000 aurori-1.0.1/aurori/database.py
+drwxrwxrwx   0        0        0        0 2023-08-04 09:24:06.131782 aurori-1.0.1/aurori/jobs/
+-rw-rw-rw-   0        0        0     2640 2023-07-27 06:56:13.000000 aurori-1.0.1/aurori/jobs/__init__.py
+-rw-rw-rw-   0        0        0     6237 2023-07-17 04:39:58.000000 aurori-1.0.1/aurori/jobs/job.py
+-rw-rw-rw-   0        0        0     1929 2023-07-27 06:08:05.000000 aurori-1.0.1/aurori/jobs/jobManager.py
+-rw-rw-rw-   0        0        0     1726 2023-07-17 04:40:43.000000 aurori-1.0.1/aurori/jobs/models.py
+-rw-rw-rw-   0        0        0     1105 2023-07-27 06:50:14.000000 aurori-1.0.1/aurori/jobs/routes.py
+drwxrwxrwx   0        0        0        0 2023-08-04 09:24:06.136782 aurori-1.0.1/aurori/logs/
+-rw-rw-rw-   0        0        0     1005 2023-07-27 15:29:46.000000 aurori-1.0.1/aurori/logs/__init__.py
+-rw-rw-rw-   0        0        0     4899 2023-07-28 06:12:36.000000 aurori-1.0.1/aurori/logs/logManager.py
+-rw-rw-rw-   0        0        0     3605 2023-07-28 06:10:15.000000 aurori-1.0.1/aurori/logs/logger.py
+-rw-rw-rw-   0        0        0     1064 2023-07-17 04:33:39.000000 aurori-1.0.1/aurori/logs/routes.py
+drwxrwxrwx   0        0        0        0 2023-08-04 09:24:06.140781 aurori-1.0.1/aurori/migrations/
+-rw-rw-rw-   0        0        0      323 2022-02-22 10:25:17.000000 aurori-1.0.1/aurori/migrations/README.md
+-rw-rw-rw-   0        0        0     4804 2022-08-04 21:24:37.000000 aurori-1.0.1/aurori/migrations/env.py
+-rw-rw-rw-   0        0        0      518 2022-01-25 10:07:21.000000 aurori-1.0.1/aurori/migrations/script.py.mako
+drwxrwxrwx   0        0        0        0 2023-08-04 09:24:06.142781 aurori-1.0.1/aurori/pages/
+-rw-rw-rw-   0        0        0      936 2023-07-27 08:21:25.000000 aurori-1.0.1/aurori/pages/__init__.py
+-rw-rw-rw-   0        0        0     5500 2023-07-27 08:16:14.000000 aurori-1.0.1/aurori/pages/menuBuilder.py
+-rw-rw-rw-   0        0        0     1256 2023-07-18 05:52:08.000000 aurori-1.0.1/aurori/routes.py
+drwxrwxrwx   0        0        0        0 2023-08-04 09:24:06.148783 aurori-1.0.1/aurori/types/
+-rw-rw-rw-   0        0        0      926 2022-08-05 14:12:46.000000 aurori-1.0.1/aurori/types/exceptions.py
+-rw-rw-rw-   0        0        0     1567 2022-08-05 14:12:46.000000 aurori-1.0.1/aurori/types/intEnum.py
+-rw-rw-rw-   0        0        0     1499 2022-08-05 14:12:46.000000 aurori-1.0.1/aurori/types/intFlag.py
+-rw-rw-rw-   0        0        0     1401 2022-08-05 14:12:46.000000 aurori-1.0.1/aurori/types/jsonDict.py
+-rw-rw-rw-   0        0        0     1579 2022-08-05 14:12:46.000000 aurori-1.0.1/aurori/types/objDict.py
+drwxrwxrwx   0        0        0        0 2023-08-04 09:24:06.156781 aurori-1.0.1/aurori/users/
+-rw-rw-rw-   0        0        0     1036 2023-07-27 10:31:03.000000 aurori-1.0.1/aurori/users/__init__.py
+-rw-rw-rw-   0        0        0     4896 2023-07-28 06:29:13.000000 aurori-1.0.1/aurori/users/basemodels.py
+-rw-rw-rw-   0        0        0     1116 2023-07-17 21:05:05.000000 aurori-1.0.1/aurori/users/defaultmodels.py
+-rw-rw-rw-   0        0        0     2083 2023-07-27 11:58:38.000000 aurori-1.0.1/aurori/users/dependencies.py
+-rw-rw-rw-   0        0        0     2920 2023-07-27 13:53:11.000000 aurori-1.0.1/aurori/users/routes.py
+-rw-rw-rw-   0        0        0      165 2023-07-27 13:52:21.000000 aurori-1.0.1/aurori/users/typemodels.py
+-rw-rw-rw-   0        0        0     5437 2023-07-27 14:51:50.000000 aurori-1.0.1/aurori/users/userManager.py
+drwxrwxrwx   0        0        0        0 2023-08-04 09:24:06.159781 aurori-1.0.1/aurori/utils/
+-rw-rw-rw-   0        0        0      879 2023-07-18 07:32:21.000000 aurori-1.0.1/aurori/utils/__init__.py
+-rw-rw-rw-   0        0        0      183 2023-07-17 20:48:28.000000 aurori-1.0.1/aurori/utils/converter.py
+-rw-rw-rw-   0        0        0     1193 2023-08-04 08:59:07.000000 aurori-1.0.1/aurori/version.py
+drwxrwxrwx   0        0        0        0 2023-08-04 09:24:06.168783 aurori-1.0.1/aurori/workspaces/
+-rw-rw-rw-   0        0        0     1136 2023-07-27 06:56:41.000000 aurori-1.0.1/aurori/workspaces/__init__.py
+-rw-rw-rw-   0        0        0     2707 2023-07-26 14:56:10.000000 aurori-1.0.1/aurori/workspaces/models.py
+-rw-rw-rw-   0        0        0     1728 2022-08-05 14:12:46.000000 aurori-1.0.1/aurori/workspaces/page.py
+-rw-rw-rw-   0        0        0     1056 2022-08-05 14:12:46.000000 aurori-1.0.1/aurori/workspaces/permission.py
+-rw-rw-rw-   0        0        0      884 2023-07-17 04:48:54.000000 aurori-1.0.1/aurori/workspaces/routes.py
+-rw-rw-rw-   0        0        0    18745 2023-07-27 08:56:40.000000 aurori-1.0.1/aurori/workspaces/workspace.py
+-rw-rw-rw-   0        0        0    13495 2023-07-27 07:35:51.000000 aurori-1.0.1/aurori/workspaces/workspaceManager.py
+drwxrwxrwx   0        0        0        0 2023-08-04 09:24:06.118781 aurori-1.0.1/aurori.egg-info/
+-rw-rw-rw-   0        0        0      615 2023-08-04 09:24:05.000000 aurori-1.0.1/aurori.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1754 2023-08-04 09:24:06.000000 aurori-1.0.1/aurori.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 09:24:05.000000 aurori-1.0.1/aurori.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-08-04 09:24:05.000000 aurori-1.0.1/aurori.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      158 2023-08-04 09:24:05.000000 aurori-1.0.1/aurori.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-04 09:24:05.000000 aurori-1.0.1/aurori.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4119 2022-08-04 21:04:02.000000 aurori-1.0.1/aurori_icon.inkscape.svg
+-rw-rw-rw-   0        0        0     9474 2022-08-04 21:10:24.000000 aurori-1.0.1/aurori_logo.inkscape.svg
+-rw-rw-rw-   0        0        0      563 2023-07-27 09:48:20.000000 aurori-1.0.1/config.ini.template
+drwxrwxrwx   0        0        0        0 2023-08-04 09:24:06.169783 aurori-1.0.1/dist/
+-rw-rw-rw-   0        0        0      199 2023-08-04 09:18:47.000000 aurori-1.0.1/dist/DEPLOY.md
+drwxrwxrwx   0        0        0        0 2023-08-04 09:24:06.171784 aurori-1.0.1/examples/
+-rw-rw-rw-   0        0        0        4 2022-09-02 13:45:54.000000 aurori-1.0.1/examples/.gitignore
+-rw-rw-rw-   0        0        0     1439 2023-08-04 09:23:44.000000 aurori-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0      184 2023-07-27 10:10:03.000000 aurori-1.0.1/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-08-04 09:24:06.172781 aurori-1.0.1/scripts/
+-rw-rw-rw-   0        0        0     2439 2022-08-05 14:12:46.000000 aurori-1.0.1/scripts/quality_report.py
+-rw-rw-rw-   0        0        0      516 2023-08-04 09:24:06.183784 aurori-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0       39 2022-07-28 09:17:51.000000 aurori-1.0.1/setup.py
+-rw-rw-rw-   0        0        0       88 2022-07-26 22:13:52.000000 aurori-1.0.1/test.py
+drwxrwxrwx   0        0        0        0 2023-08-04 09:24:06.056782 aurori-1.0.1/tests/
+drwxrwxrwx   0        0        0        0 2023-08-04 09:24:06.178781 aurori-1.0.1/tests/api_test/
+-rw-rw-rw-   0        0        0       80 2021-08-24 16:09:25.000000 aurori-1.0.1/tests/api_test/action.req
+-rw-rw-rw-   0        0        0     2117 2022-07-26 21:50:23.000000 aurori-1.0.1/tests/api_test/action_test.py
+-rw-rw-rw-   0        0        0      130 2021-08-24 16:09:25.000000 aurori-1.0.1/tests/api_test/dashboard.req
+-rw-rw-rw-   0        0        0      130 2021-08-24 16:09:25.000000 aurori-1.0.1/tests/api_test/login.req
+-rw-rw-rw-   0        0        0      135 2021-08-24 16:09:25.000000 aurori-1.0.1/tests/api_test/refresh.req
```

### Comparing `aurori-0.1.4/.gitlab-ci.yml` & `aurori-1.0.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `aurori-0.1.4/.vscode/launch.json` & `aurori-1.0.1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `aurori-0.1.4/LICENSE` & `aurori-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aurori-0.1.4/aurori/LICENSE.md` & `aurori-1.0.1/aurori/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aurori-0.1.4/aurori/actions/__init__.py` & `aurori-1.0.1/aurori/users/defaultmodels.py`

 * *Files 26% similar despite different names*

```diff
@@ -18,32 +18,15 @@
 """
 
 __authors__ = ["Marcus Drobisch"]
 __contact__ = "aurori@fabba.space"
 __credits__ = []
 __license__ = "AGPLv3+"
 
-from flask import Blueprint
-from aurori.actions.actionManager import ActionManager
+from aurori.users.basemodels import UserBase
 
-actions_bp = Blueprint('actions', __name__)
-
-actionManager = ActionManager()
-
-
-def generateActionLink(workspace,
-                       action_uri,
-                       action_params,
-                       redirect_to="",
-                       once=True,
-                       need_login=True,
-                       expire_days=7):
-    return actionManager.createActionLink(workspace, action_uri, action_params,
-                                          redirect_to, once, need_login,
-                                          expire_days)
-
-
-def executeActionLink(hash, user):
-    return actionManager.executeActionLink(hash, user)
-
-
-from aurori.actions import routes
+class User(UserBase):
+    def __init__(self, email, password, isAdmin=False, skip_password=False):
+        self.email = email
+        if skip_password is False:
+            self.password = password
+        self.admin = isAdmin
```

### Comparing `aurori-0.1.4/aurori/actions/action.py` & `aurori-1.0.1/aurori/routes.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,31 +18,29 @@
 """
 
 __authors__ = ["Marcus Drobisch"]
 __contact__ = "aurori@fabba.space"
 __credits__ = []
 __license__ = "AGPLv3+"
 
+from aurori import app_router
+import time
 
-class Action(object):
-    """Base class that each action for every workspace have to inherit from.
-       The class define methods that all action must implement by the plugin
-    """
-
-    disable = False
-
-    def __init__(self, app, uri=None):
-        if uri is None:
-            self.uri = self.__class__.__name__
-        else:
-            self.uri = uri
-
-    def handle(self, action, user, workspace, actionManager):
-        """ Action handler method
-        """
-        raise NotImplementedError
-
-    @staticmethod
-    def generate(**kwargs):
-        """ Action generator method
-        """
-        raise NotImplementedError
+# index route
+@app_router.get('/')
+def index():
+    return {}
+
+@app_router.get('/<path:path>')
+def static_proxy(path):
+    return {}
+
+'''
+@app_bp.after_request
+def add_header(r):
+
+    r.headers[
+        "Cache-Control"] = "no-cache, no-store, must-revalidate, max-age=0"
+    r.headers["Pragma"] = "no-cache"
+    r.headers["Expires"] = "0"
+    return r
+'''
```

### Comparing `aurori-0.1.4/aurori/actions/actionGenerator.py` & `aurori-1.0.1/aurori/workspaces/permission.py`

 * *Files 21% similar despite different names*

```diff
@@ -19,28 +19,13 @@
 
 __authors__ = ["Marcus Drobisch"]
 __contact__ = "aurori@fabba.space"
 __credits__ = []
 __license__ = "AGPLv3+"
 
 
-class BaseAction(object):
-    action = 'undefined'
-    target = 'undefined'
-    source = 'undefined'
-    version = 1.0
-
-    def __init__(self, ):
-        print("Instance of BaseAction created")
-
-    def execute(self, ):
-        print("Execute not defined")
-
-    @classmethod
-    def generate(cls, delay=0.0):
-        action = {}
-        action['action'] = cls.action
-        action['target'] = cls.target
-        action['version'] = cls.version
-        action['source'] = cls.source
-        action['delay'] = delay
-        return action
+class Permission(object):
+    """Base class to create and handle permissions in the workspaces
+    """
+    def __init__(self):
+        if not hasattr(self, 'name'):
+            self.name = self.__class__.__name__
```

### Comparing `aurori-0.1.4/aurori/actions/models.py` & `aurori-1.0.1/aurori/types/intEnum.py`

 * *Files 26% similar despite different names*

```diff
@@ -19,29 +19,31 @@
 
 __authors__ = ["Marcus Drobisch"]
 __contact__ = "aurori@fabba.space"
 __credits__ = []
 __license__ = "AGPLv3+"
 
 from aurori import db
-from sqlalchemy_utils import ArrowType
-import arrow
 
-from aurori.common.jsonDict import JsonDict
 
+class IntEnum(db.TypeDecorator):
+    """
+    Enables passing in a Python enum and storing the enum's *value* in the db.
+    The default would have stored the enum's *name* (ie the string).
 
-class ActionLink(db.Model):
-    __tablename__ = 'actionlinks'
-    # nonvolatile data stored in the db
-    id = db.Column(db.Integer, primary_key=True)
-    hash = db.Column(db.String(128), default="")
-    workspace = db.Column(db.String(120), default="")
-    need_login = db.Column(db.Boolean, default=True)
-    action = db.Column(db.String(120), default="")
-    action_data_json = db.Column(JsonDict)
-    run_only_once = db.Column(db.Boolean, default=True)
-    expire_on_date = db.Column(ArrowType, default=arrow.utcnow)
-    redirect_to = db.Column(db.String(255), default="")
-
-    def __repr__(self):
-        return '<ActionLink {} for {}/{} [expires on {}] >'.format(
-            self.link, self.workspace, self.action, self.expire_on_date)
+    Usage example: message_type = db.Column(IntEnum(MessageTypes), default=MessageTypes.text)
+
+    """
+    impl = db.Integer
+
+    def __init__(self, enumtype, *args, **kwargs):
+        super(IntEnum, self).__init__(*args, **kwargs)
+        self._enumtype = enumtype
+
+    def process_bind_param(self, value, dialect):
+        if isinstance(value, int):
+            return value
+
+        return value.value
+
+    def process_result_value(self, value, dialect):
+        return self._enumtype(value)
```

### Comparing `aurori-0.1.4/aurori/actions/routes.py` & `aurori-1.0.1/aurori/pages/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,9 +18,11 @@
 """
 
 __authors__ = ["Marcus Drobisch"]
 __contact__ = "aurori@fabba.space"
 __credits__ = []
 __license__ = "AGPLv3+"
 
-from aurori.actions import actions_bp
-from flask_jwt_extended import jwt_required, jwt_optional, get_jwt_identity
+from fastapi import APIRouter
+from .menuBuilder import MenuBuilder
+
+menu_builder = MenuBuilder()
```

### Comparing `aurori-0.1.4/aurori/alembic.ini` & `aurori-1.0.1/aurori/alembic.ini`

 * *Files identical despite different names*

### Comparing `aurori-0.1.4/aurori/api/__init__.py` & `aurori-1.0.1/aurori/workspaces/routes.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,12 +18,8 @@
 """
 
 __authors__ = ["Marcus Drobisch"]
 __contact__ = "aurori@fabba.space"
 __credits__ = []
 __license__ = "AGPLv3+"
 
-from flask import Blueprint
-
-api_bp = Blueprint('api', __name__)
-
-from aurori.api import routes
+from aurori.workspaces import workspaces_router
```

### Comparing `aurori-0.1.4/aurori/api/check.py` & `aurori-1.0.1/aurori/jobs/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -18,40 +18,70 @@
 """
 
 __authors__ = ["Marcus Drobisch"]
 __contact__ = "aurori@fabba.space"
 __credits__ = []
 __license__ = "AGPLv3+"
 
-import base64
-from flask import request, g
-from flask_jwt_extended import jwt_optional, get_jwt_identity
-from aurori.users import userManager
-
-
-def check_before_request():
-    g.user = None
-    jwt_id = get_jwt_identity()
-    auth_header = request.headers.get('Authorization')
-
-    if jwt_id is not None:  # check for jwt token
-        user = (userManager.getUser(jwt_id))
-        g.user = user
-    else:  # check for header authentication basic
-        if auth_header is not None:
-            split_auth_header = auth_header.split()
-            auth_type = split_auth_header[0]
-            if auth_type == "Basic":
-                decoded_auth = base64.b64decode(
-                    split_auth_header[1]).decode('utf8').split(':')
-                if decoded_auth[
-                        0] == 'api_key':  # check for api_key authentication
-                    user = userManager.get_user_by_api_key(decoded_auth[1])
-                    g.user = user
-                else:  # check for email and password authentication
-                    user = userManager.getUser(decoded_auth[0])
-                    if user is not None:
-                        if userManager.checkUserPassword(
-                                user, decoded_auth[1]):
-                            g.user = user
+from datetime import datetime
+from fastapi import APIRouter
+from aurori.jobs.job import Job
+
+from aurori.jobs.jobManager import JobManager
+from aurori.logs import logManager
+from inspect import isclass
+
+jobManager = JobManager()
+
+jobs_router = APIRouter()
+
+def trigger_job(job_key, args, user):
+    if user is None:
+        logManager.info("Internal job {} triggered".format(job_key))
+    else:
+        logManager.info("User {} triggered job {}".format(user.email, job_key))
+
+    job_id = jobManager.run_job(user,
+                                job_key,
+                                args,
+                                datetime.now(),
+                                log_trigger=True)
+    return job_id
+
+
+def add_dated_job(user,
+                  job,
+                  args,
+                  date=None,
+                  workspace=None,
+                  max_instances=10):
+    if date is None:
+        date = datetime.now()
+    key = ""
+    if workspace is not None:
+        if type(workspace) == str:
+            key += workspace + '/'
+        elif isclass(workspace):
+            logManager.error(
+                "Class parameters are not allowed for add_dated_job")
+            return
+        else:
+            key += workspace.name + '/'
+
+    if type(job) == str:
+        key += job
+    elif isclass(workspace):
+        logManager.error("Class parameters are not allowed for add_dated_job")
+        return
+    elif issubclass(type(job), Job):
+        key += job.name
+    else:
+        logManager.error("Unknown type of job in add_dated_job")
+        return
+    jobManager.run_job(user, key, args, date, max_instances)
 
-    request.view_args['user'] = g.user
+
+def print_job_list():
+    print("jobs.print_job_list not implemented yet")
+
+
+from aurori.jobs import routes
```

### Comparing `aurori-0.1.4/aurori/api/decorator.py` & `aurori-1.0.1/aurori/jobs/jobManager.py`

 * *Files 25% similar despite different names*

```diff
@@ -18,40 +18,43 @@
 """
 
 __authors__ = ["Marcus Drobisch"]
 __contact__ = "aurori@fabba.space"
 __credits__ = []
 __license__ = "AGPLv3+"
 
-from functools import wraps
-from flask import g, Response
-
-
-def require_user_permission(permissions):
-    def decorator(func):
-        @wraps(func)
-        def wrapper(*args, **kwargs):
-            if g.user is None:
-                return Response('Authentication required', 401, {
-                    'WWW-Authenticate':
-                    'Basic realm="Authentication required"'
-                })
-            for p in permissions:
-                if g.user.has_permission(p):
-                    return func(*args, **kwargs)
-            return Response('Insufficient user permissions', 403)
-
-        return wrapper
-
-    return decorator
-
-
-def require_user_authentification(f):
-    @wraps(f)
-    def decorator(*args, **kwargs):
-        if g.user is None:
-            return Response(
-                'Authentication required', 401,
-                {'WWW-Authenticate': 'Basic realm="Authentication required"'})
-        return f(*args, **kwargs)
-
-    return decorator
+import logging
+from datetime import datetime
+from apscheduler.schedulers.asyncio  import AsyncIOScheduler
+
+from aurori.logs import logManager
+
+class JobManager(object):
+    """ The JobManager ...
+    """
+    def __init__(self, ):
+        # preparation to instanciate
+        self.config = None
+        self.workspaceManager = None
+        self.job_counter = 0
+        self.jobs = {}
+        self.scheduler = AsyncIOScheduler()
+        logging.getLogger('apscheduler.scheduler').name = "SCHEDULER"
+        logging.getLogger('apscheduler.executors.default').name = "EXECUTOR"
+
+    def init_manager(self, config):
+        self.config = config
+
+    def get_jobs(self):
+        return self.jobs
+
+    def register_job(self, workspace, job_class, log_in_db=False):
+        print("jobManager.register_job not implemented yet")
+
+    def run_job(self,
+                user,
+                jobkey,
+                args,
+                date,
+                max_instances=10,
+                log_trigger=False):
+        print("jobManager.run_job not implemented yet")
```

### Comparing `aurori-0.1.4/aurori/common/__init__.py` & `aurori-1.0.1/aurori/types/exceptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,7 +17,15 @@
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 __authors__ = ["Marcus Drobisch"]
 __contact__ = "aurori@fabba.space"
 __credits__ = []
 __license__ = "AGPLv3+"
+
+
+class ExpiredError(Exception):
+    pass
+
+
+class NotFoundError(Exception):
+    pass
```

### Comparing `aurori-0.1.4/aurori/common/intEnum.py` & `aurori-1.0.1/aurori/types/intFlag.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,29 +21,28 @@
 __contact__ = "aurori@fabba.space"
 __credits__ = []
 __license__ = "AGPLv3+"
 
 from aurori import db
 
 
-class IntEnum(db.TypeDecorator):
+class IntFlag(db.TypeDecorator):
     """
     Enables passing in a Python enum and storing the enum's *value* in the db.
-    The default would have stored the enum's *name* (ie the string).
 
-    Usage example: message_type = db.Column(IntEnum(MessageTypes), default=MessageTypes.text)
+    Usage example: message_type = db.Column(IntFlag(MessageTypes), default=MessageTypes.text)
 
     """
     impl = db.Integer
 
     def __init__(self, enumtype, *args, **kwargs):
-        super(IntEnum, self).__init__(*args, **kwargs)
+        super(IntFlag, self).__init__(*args, **kwargs)
         self._enumtype = enumtype
 
     def process_bind_param(self, value, dialect):
         if isinstance(value, int):
             return value
 
         return value.value
 
     def process_result_value(self, value, dialect):
-        return self._enumtype(value)
+        return self._enumtype(value)
```

### Comparing `aurori-0.1.4/aurori/common/intFlag.py` & `aurori-1.0.1/aurori/version.py`

 * *Files 27% similar despite different names*

```diff
@@ -18,31 +18,17 @@
 """
 
 __authors__ = ["Marcus Drobisch"]
 __contact__ = "aurori@fabba.space"
 __credits__ = []
 __license__ = "AGPLv3+"
 
-from aurori import db
+import subprocess
 
-
-class IntFlag(db.TypeDecorator):
-    """
-    Enables passing in a Python enum and storing the enum's *value* in the db.
-
-    Usage example: message_type = db.Column(IntFlag(MessageTypes), default=MessageTypes.text)
-
-    """
-    impl = db.Integer
-
-    def __init__(self, enumtype, *args, **kwargs):
-        super(IntFlag, self).__init__(*args, **kwargs)
-        self._enumtype = enumtype
-
-    def process_bind_param(self, value, dialect):
-        if isinstance(value, int):
-            return value
-
-        return value.value
-
-    def process_result_value(self, value, dialect):
-        return self._enumtype(value)
+version = "1.0.1"
+# WARNING: will be overwritten by CI, see docker/.gitlab-ci.yml
+# try:
+#    label = subprocess.check_output(["git", "describe"]).strip()
+#    version = label.decode(encoding='UTF-8')
+# except Exception as e:
+#    print("Unable to get version", e)
+# WARNING: will be overwritten by CI, see docker/.gitlab-ci.yml
```

### Comparing `aurori-0.1.4/aurori/common/jsonDict.py` & `aurori-1.0.1/aurori/types/jsonDict.py`

 * *Files identical despite different names*

### Comparing `aurori-0.1.4/aurori/common/objDict.py` & `aurori-1.0.1/aurori/types/objDict.py`

 * *Files identical despite different names*

### Comparing `aurori-0.1.4/aurori/config.py` & `aurori-1.0.1/aurori/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     # read and overwrite
     cfg_parser.read(path)
     data = json.loads(json.dumps(cfg_parser._sections))
     config = remove_quotes(data)
     return config
 
 
-def configure_app(app, config, flask_config):
+def configure_app(app, config, fastapi_config):
     # Configure application to store JWTs in cookies
     app.config['JWT_TOKEN_LOCATION'] = ['headers']
     app.config['CORS_HEADERS'] = 'Content-Type'
 
     # Only allow JWT cookies to be sent over https. In production, this
     # should likely be True
     app.config['JWT_COOKIE_SECURE'] = False
@@ -124,29 +124,30 @@
     app.config['MAIL_PORT'] = config['MAIL'].get('port', 465)
     app.config['MAIL_USERNAME'] = config['MAIL'].get('username', 'username')
     app.config['MAIL_PASSWORD'] = config['MAIL'].get('password', 'password')
     app.config['MAIL_USE_TLS'] = config['MAIL'].get('tls', False)
     app.config['MAIL_USE_SSL'] = config['MAIL'].get('ssl', True)
     app.config['MAIL_SENDER'] = config['MAIL'].get('sender', 'test@test.com')
 
-    if flask_config:
-        app.config.update(flask_config)
+    if fastapi_config:
+        app.config.update(fastapi_config)
     # app.config.from_pyfile('config.cfg', silent=True) # instance-folders configuration
     print("Cofing loaded")
 
 
 class ConfigManager(object):
     """ The MonitManager ...
     """
     def __init__(self):
         self.config = None
+        self.fastapi_config = None
 
-    def init_manager(self, config, flask_config):
+    def init_manager(self, config, fastapi_config):
         self.config = config
-        self.flask_config = flask_config
+        self.fastapi_config = fastapi_config
 
 
 class Config(dict):
     def __init__(self, config_path="config.ini"):
         super(Config, self).__init__()
         cfg = load_config(config_path)
         self.update(cfg)
```

### Comparing `aurori-0.1.4/aurori/exceptions.py` & `aurori-1.0.1/aurori/utils/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-"""
-The aurori project
+'''The aurori project
 
 Copyright (C) 2022  Marcus Drobisch,
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU Affero General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
@@ -11,21 +10,15 @@
 This program is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU Affero General Public License for more details.
 
 You should have received a copy of the GNU Affero General Public License
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
-"""
+'''
 
 __authors__ = ["Marcus Drobisch"]
 __contact__ = "aurori@fabba.space"
 __credits__ = []
 __license__ = "AGPLv3+"
 
-
-class ExpiredError(Exception):
-    pass
-
-
-class NotFoundError(Exception):
-    pass
+from .converter import unicode_string_to_bytes
```

### Comparing `aurori-0.1.4/aurori/jobs/models.py` & `aurori-1.0.1/aurori/jobs/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,28 +20,28 @@
 """
 
 __authors__ = ["Marcus Drobisch"]
 __contact__ = "aurori@fabba.space"
 __credits__ = []
 __license__ = "AGPLv3+"
 
+from datetime import datetime
 from sqlalchemy_utils import ArrowType
-import arrow
 
-from aurori.common.jsonDict import JsonDict
+from aurori.types.jsonDict import JsonDict
 
 
 class JobExecute(db.Model):
     __tablename__ = 'jobs'
     id = db.Column(db.Integer, primary_key=True)
     name = db.Column(db.String(120), default="")
     workspace = db.Column(db.String(120), default="")
     job = db.Column(db.String(120), default="")
     state = db.Column(db.String(120), default="")
-    triggered_on = db.Column(ArrowType, default=arrow.utcnow)
+    triggered_on = db.Column(db.DateTime, default=datetime.utcnow)
     triggered_by = db.Column(db.String(120), default="")
     lifetime = db.Column(db.Integer, default=0)
     args = db.Column(JsonDict)
     results = db.Column(JsonDict)
 
     def __repr__(self):
         return '<Job {} for {}/{} >'.format(self.name, self.workspace,
```

### Comparing `aurori-0.1.4/aurori/jobs/routes.py` & `aurori-1.0.1/aurori/logs/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -17,7 +17,17 @@
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 __authors__ = ["Marcus Drobisch"]
 __contact__ = "aurori@fabba.space"
 __credits__ = []
 __license__ = "AGPLv3+"
+
+from fastapi import APIRouter
+from aurori.logs.logManager import LogManager
+
+
+logManager = LogManager()
+
+logs_router = APIRouter()
+
+from aurori.logs import routes
```

### Comparing `aurori-0.1.4/aurori/logs/__init__.py` & `aurori-1.0.1/aurori/users/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 """
 
 __authors__ = ["Marcus Drobisch"]
 __contact__ = "aurori@fabba.space"
 __credits__ = []
 __license__ = "AGPLv3+"
 
-from aurori.logs.logManager import LogManager
-from flask import Blueprint
+from fastapi import APIRouter
+from aurori.users.userManager import UserManager
 
-logManager = LogManager()
-logs_bp = Blueprint('logs', __name__)
+user_router = APIRouter()
+core_router = APIRouter()
 
-from aurori.logs import routes
+userManager = UserManager()
+
+from aurori.users import routes
```

### Comparing `aurori-0.1.4/aurori/logs/logManager.py` & `aurori-1.0.1/aurori/logs/logManager.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,35 +22,40 @@
 __credits__ = []
 __license__ = "AGPLv3+"
 
 import sys
 import collections
 import datetime
 import threading
-
+import logging
+from .logger import Logger
 
 class LogManager(object):
     def __init__(self):
-        self.logQueue = collections.deque(maxlen=512)
-        self.app = None
-
-    def init_app(self, app):
-        self.app = app
         gettrace = getattr(sys, 'gettrace', None)
         if gettrace and gettrace():
             self.run_in_debug_mode = True
         else:
             self.run_in_debug_mode = False
+          
+        self.logQueue = collections.deque(maxlen=512)
+        self.loggers = {
+            "core": Logger("core", self.run_in_debug_mode, app_logger=False)
+        }
+        self.logger = self.loggers["core"]
+
+        logging.basicConfig(level=logging.INFO, format='[%(asctime)s]-[%(name)s]-[%(levelname)s]: %(message)s', datefmt="%Y-%m-%dT%H:%M:%S")     
+
+    def register_logger(self, logger, name):
+        self.loggers[name.lower()] = logger
 
     def info(self, msg, *args, **kwargs):
         """
         Delegate a info log call to the underlying logger,
         """
-        if self.app is None:
-            return
         if type(msg) is str:
             try:
                 s = msg % args
             except Exception:
                 s = msg.format(*args)
             indents = s.replace("\n", "\n" + " " * 29)
             self.logQueue.append(
@@ -59,18 +64,16 @@
         else:
             s = str(msg)
             indents = s.replace("\n", "\n" + " " * 29)
             self.logQueue.append(
                 datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S") +
                 " [INFO] : " + indents)
         try:
-            self.app.logger.info(msg, *args, **kwargs)
+            self.logger.info(msg, *args, **kwargs)
             indents = s.replace("\n", "\n" + " " * 14)
-            print("[{:4.4}][INFO]: {}".format(threading.current_thread().name,
-                                              indents))
         except Exception as e:
             print("logger failed to print: ", s, e)
 
     def warning(self, msg, *args, **kwargs):
         """
         Delegate a warning log call to the underlying logger,
         """
@@ -85,16 +88,15 @@
         else:
             s = str(msg)
             self.logQueue.append(
                 datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S") +
                 " [WARN] : " + s)
 
         try:
-            self.app.logger.info(msg, *args, **kwargs)
-            print("[WARNING]:", s)
+            self.logger.warning(msg, *args, **kwargs)
         except Exception:
             print("logger failed to print: ", s)
 
     def error(self, msg, *args, **kwargs):
         """
         Delegate a error log call to the underlying logger,
         """
@@ -109,16 +111,15 @@
         else:
             s = str(msg)
             self.logQueue.append(
                 datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S") +
                 " [FAIL] : " + s)
 
         try:
-            self.app.logger.info(msg, *args, **kwargs)
-            print("[FAIL]:", s)
+            self.logger.error(msg, *args, **kwargs)
         except Exception:
             print("logger failed to print: ", s)
 
     def debug(self, msg, *args, **kwargs):
         """
         Delegate a error log call to the underlying logger,
         """
@@ -135,11 +136,10 @@
         else:
             s = str(msg)
             self.logQueue.append(
                 datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S") +
                 " [DEBUG] : " + s)
 
         try:
-            self.app.logger.info(msg, *args, **kwargs)
-            print("[DEBUG]:", s)
+            self.logger.debug(msg, *args, **kwargs)
         except Exception:
             print("logger failed to print: ", s)
```

### Comparing `aurori-0.1.4/aurori/logs/routes.py` & `aurori-1.0.1/aurori/logs/routes.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,16 +18,15 @@
 """
 
 __authors__ = ["Marcus Drobisch"]
 __contact__ = "aurori@fabba.space"
 __credits__ = []
 __license__ = "AGPLv3+"
 
-from aurori.logs import logs_bp, logManager
+from aurori.logs import logs_router, logManager
 
-
-@logs_bp.route('/api/v1/log', methods=["GET"])
+@logs_router.get("/log/", tags=["users"])
 def log():
     log_string = ""
     for e in logManager.logQueue:
         log_string = log_string + e + "\n"
     return log_string
```

### Comparing `aurori-0.1.4/aurori/menus/__init__.py` & `aurori-1.0.1/aurori/jobs/routes.py`

 * *Files 22% similar despite different names*

```diff
@@ -18,14 +18,21 @@
 """
 
 __authors__ = ["Marcus Drobisch"]
 __contact__ = "aurori@fabba.space"
 __credits__ = []
 __license__ = "AGPLv3+"
 
-from flask import Blueprint
-from aurori.menus.menuBuilder import MenuBuilder
+import time
+from datetime import datetime
+from aurori.jobs import jobs_router, jobManager
+import logging
 
-menuBuilder = MenuBuilder()
-menus_bp = Blueprint('menus', __name__)
 
-from aurori.menus import routes
+def check_list_len():
+    time.sleep(3)
+    print("test")
+
+
+@jobs_router.on_event('startup')
+async def init_data():
+    jobManager.scheduler.start()
```

### Comparing `aurori-0.1.4/aurori/menus/menuBuilder.py` & `aurori-1.0.1/aurori/pages/menuBuilder.py`

 * *Files 18% similar despite different names*

```diff
@@ -32,159 +32,108 @@
 
     def init_builder(self, app, db, userManager, workspaceManager):
         self.app = app
         self.db = db
         self.workspaceManager = workspaceManager
         self.userManager = userManager
 
-    def makeHeader(self, name):
+    def make_menu_header(self, name):
         header = {}
         header['header'] = name
         return header
 
-    def makeGroup(self, name):
+    def make_menu_group(self, name):
         group = {}
         group['title'] = name
         group['entries'] = []
         group['active'] = False
         group['disabled'] = False  # whether group can be collapsed
         return group
 
-    def makeDivider(self, ):
+    def make_menu_divider(self, ):
         divider = {}
         divider['divider'] = True
         return divider
 
-    def makeEntry(self, title, group, name, icon, path, external=False):
+    def make_menu_entry(self, title, group, name, icon, path, external=False):
         entry = {}
         entry['title'] = title
         entry['group'] = group
         entry['name'] = name
         entry['icon'] = icon
         entry['href'] = path
         entry['external'] = external
         return entry
 
-    def buildGuestMenu(self, ):
-        print("buildGuestMenu")
-        menu = []
-        menu.append(self.makeHeader('Aurori'))
-        menu.append(
-            self.makeEntry('Home', 'app', 'Dashboard', 'dashboard',
-                           '/dashboard'))
-        menu.append(self.makeDivider())
-        return menu
-
-    def buildUserMenu(self, user):
-        print("buildUserMenu")
-        menu = self.buildGuestMenu()
-        menu.append(self.makeHeader('User'))
-        menu.append(
-            self.makeEntry(title='Account',
-                           group='user',
-                           name='Account',
-                           icon='face',
-                           path='/user/account'))
-        menu.append(self.makeDivider())
-        return menu
-
-    def buildAdminMenu(self, user):
-        print("buildAdminMenu")
-        menu = self.buildUserMenu(user)
-        menu.append(self.makeHeader('Admin'))
-        menu.append(
-            self.makeEntry('Users', 'admin', 'Users', 'supervisor_account',
-                           '/admin/users'))
-        menu.append(
-            self.makeEntry('Permissions', 'admin', 'Permissions',
-                           'verified_user', '/admin/permissions'))
-        # menu.append(self.makeEntry('Access cards', 'admin', 'Cards', 'credit_card', '/admin/cards'))
-        # menu.append(self.makeEntry('Space access', 'admin', 'Access', 'lock', '/admin/access'))
-        # menu.append(self.makeEntry('Nodes', 'admin', 'Nodes', 'adjust', '/admin/nodes'))
-        menu.append(
-            self.makeEntry('Log', 'admin', 'Log', 'description', '/admin/log'))
-
-        menu.append(self.makeDivider())
-        return menu
-
-    def checkUserPermissions(self, user, requirement, workspace):
+    def check_users_permissions(self, user, requirement, workspace):
         key = workspace.name + '.' + requirement.name
         for g in user.permission_groups:
             for p in g.permissions:
                 if key == p.name:
                     return True
         return False
 
-    def hasPermission(self, user, page, workspace):
+    def has_permission(self, user, page, workspace):
         if user is None:
             if page.requireLogin is False:
                 return True
         else:
             if user.admin is True:
                 return True
             if page.requireAdmin is False:
                 if hasattr(page, 'requirePermission'):
                     if page.requirePermission is None:
                         return True
                     else:
-                        return self.checkUserPermissions(
+                        return self.check_users_permissions(
                             user, page.requirePermission, workspace)
         return False
 
-    def buildMenu(self, user):
+    def build_menu(self, user):
         menu_groups = {}
         for w in self.workspaceManager.workspaces:
             for key, p in w.pages.items():
                 # is pages in a group
                 if p.group is not None:
                     if str(p.group) in menu_groups:
                         rankSum, pageList = menu_groups[str(p.group)]
 
-                        if self.hasPermission(user, p, w):
+                        if self.has_permission(user, p, w):
                             pageList.append(p)
 
                         pageList.sort(key=lambda x: x.rank, reverse=True)
                         menu_groups[str(p.group)] = rankSum + p.rank, pageList
                     else:
-                        if self.hasPermission(user, p, w):
+                        if self.has_permission(user, p, w):
                             menu_groups[str(p.group)] = p.rank, [p]
                         else:
                             menu_groups[str(p.group)] = p.rank, []
                 else:
-                    if self.hasPermission(user, p, w):
+                    if self.has_permission(user, p, w):
                         menu_groups['_' + str(p.name)] = p.rank, [p]
 
         sorted_menu_groups = sorted(menu_groups.items(),
                                     key=lambda x: x[1][0],
                                     reverse=True)
 
         menu = []
         for key, element in enumerate(sorted_menu_groups):
             group, (rank, pagelist) = element
             if len(pagelist) > 0:
-                entry = self.makeGroup(str(group))
+                entry = self.make_menu_group(str(group))
                 for p in pagelist:
                     entry['entries'].append(
-                        self.makeEntry(title=p.title,
+                        self.make_menu_entry(title=p.title,
                                        group=p.group,
                                        name=p.name,
                                        icon=p.icon,
                                        path=p.route))
                 menu.append(entry)
 
         return menu
-        '''
-        if user is None:
-            return  self.buildGuestMenu()
-        else:
-            if user.admin is False:
-                return self.buildUserMenu(user)
-            else:
-                return self.buildAdminMenu(user)
-        '''
 
 
 '''
 EXAMPLE of menu structure
 [
   {header: 'aurori'},
   {
```

### Comparing `aurori-0.1.4/aurori/migrations/env.py` & `aurori-1.0.1/aurori/migrations/env.py`

 * *Files identical despite different names*

### Comparing `aurori-0.1.4/aurori/migrations/script.py.mako` & `aurori-1.0.1/aurori/migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `aurori-0.1.4/aurori/monits/cleanupMonitorEventsJob.py` & `aurori-1.0.1/aurori/workspaces/page.py`

 * *Files 25% similar despite different names*

```diff
@@ -17,32 +17,28 @@
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 __authors__ = ["Marcus Drobisch"]
 __contact__ = "aurori@fabba.space"
 __credits__ = []
 __license__ = "AGPLv3+"
-
-from aurori.jobs.job import Job
-from aurori.logs import logManager
-from datetime import datetime, timedelta
+"""Base class to create and handle pages in the workspaces
+"""
 
 
-class CleanupMonitorEventsJob(Job):
+class Page(object):
+    title = 'Missing title'  # Shown label of the page in the menu
+    group = None  # groupname multiple pages
+    icon = 'warning'  # icon (in typeset of material design icons)
+    route = '/error'  # routing
+    builder = 'frontend'  # page get build by the client (frontend)
+    rank = 0.0  # ranks (double) the page higher values are at the top of the menu
+    # groups will be ranked by the sum of the rank-values of their entries
+    requireLogin = True  # login is required to view the page
+    requireAdmin = True  # admin is required to view the page
+    requirePermission = None  # a permission is required in the meaning of one of the following
 
-    cron = True
-    hour = "*/4"
-    minute = "0"
     disable = False
-    description = "Cleanup monitor events"
-
-    def run(self, **kwargs):
-        from aurori.monits.models import MonitorEvent
-        now = datetime.utcnow()
-        datetime_threshold = now.replace(minute=0, second=0,
-                                         microsecond=0) - timedelta(hours=2)
 
-        monit_event_older_2hours = MonitorEvent.query.filter(
-            MonitorEvent.created_at < datetime_threshold).all()
-        for m in monit_event_older_2hours:
-            self.db.session.delete(m)
-        logManager.info("CleanupMonitorEventsJob done")
+    def __init__(self):
+        if not hasattr(self, 'name'):
+            self.name = self.__class__.__name__
```

### Comparing `aurori-0.1.4/aurori/nodes/__init__.py` & `aurori-1.0.1/aurori/workspaces/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-"""
-The aurori project
+'''The aurori project
 
 Copyright (C) 2022  Marcus Drobisch,
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU Affero General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
@@ -11,23 +10,26 @@
 This program is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU Affero General Public License for more details.
 
 You should have received a copy of the GNU Affero General Public License
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
-"""
+'''
 
 __authors__ = ["Marcus Drobisch"]
 __contact__ = "aurori@fabba.space"
 __credits__ = []
 __license__ = "AGPLv3+"
 
-from flask import Blueprint
+from fastapi import APIRouter
 
-from .nodeManager import NodeManager
+from .workspaceManager import WorkspaceManager
+from .workspace import Workspace
+from .permission import Permission
+from .page import Page
 
-nodeManager = NodeManager()
+workspaceManager = WorkspaceManager('workspaces')
 
-nodes_bp = Blueprint('nodes', __name__)
+workspaces_router = APIRouter()
 
-from aurori.nodes import routes
+from aurori.workspaces import routes
```

### Comparing `aurori-0.1.4/aurori/users/basemodels.py` & `aurori-1.0.1/aurori/users/basemodels.py`

 * *Files 21% similar despite different names*

```diff
@@ -18,92 +18,105 @@
 """
 
 __authors__ = ["Marcus Drobisch"]
 __contact__ = "aurori@fabba.space"
 __credits__ = []
 __license__ = "AGPLv3+"
 
-from aurori import db, bcrypt
 import hashlib
+import bcrypt
+from datetime import datetime 
+from sqlalchemy import Boolean, Column, DateTime, Integer, String, LargeBinary
 from sqlalchemy.ext.hybrid import hybrid_property, hybrid_method
-from sqlalchemy_utils import ArrowType
-import arrow
 
+from aurori.database import SQLModelBase
+from aurori.utils import unicode_string_to_bytes
 
-class UserBase(db.Model):
+
+class UserBase(SQLModelBase):
     __abstract__ = True
     __tablename__ = 'users'
     # nonvolatile data stored in the db
-    id = db.Column(db.Integer, primary_key=True, autoincrement=True)
-    _password_hash = db.Column(db.LargeBinary(60), nullable=False)
-    _pin_hash = db.Column(db.LargeBinary(60))
-    _salt = db.Column(db.String(128))
-    _api_key_hash = db.Column(db.String(256), nullable=True, default=None)
-    email = db.Column(db.String(120), index=True, unique=True)
-    firstname = db.Column(db.String(64), default="")
-    lastname = db.Column(db.String(64), default="")
-    organization = db.Column(db.String(64), default="")
-    phone = db.Column(db.String(64), default="")
-    account_created_date = db.Column(ArrowType, default=arrow.utcnow)
-    last_login_date = db.Column(ArrowType, default=arrow.utcnow)
-    password_reset_expired_date = db.Column(ArrowType, default=arrow.utcnow)
-    password_reset_hash = db.Column(db.String(128), default="")
-    account_verified = db.Column(db.Boolean, default=False)
-    account_activated = db.Column(db.Boolean, default=False)
-    account_locked = db.Column(db.Boolean, default=False)
-    ldap = db.Column(db.Boolean, default=False)
-    ldap_dn = db.Column(db.String(64), default="")
-    ldap_username = db.Column(db.String(64), default="")
-    admin = db.Column(db.Boolean, default=False)
-    pinAttempts = db.Integer()
-    loginAttempts = db.Integer()
+    id = Column(Integer, primary_key=True, autoincrement=True)
+    _password_hash = Column(LargeBinary(60), nullable=False)
+    _pin_hash = Column(LargeBinary(60))
+    _salt = Column(String(128))
+    _api_key_hash = Column(String(256), nullable=True, default=None)
+    email = Column(String(120), index=True, unique=True)
+    username = Column(String(120), index=True, unique=True)
+    firstname = Column(String(120), default="")
+    lastname = Column(String(120), default="")
+    organization = Column(String(120), default="")
+    phone = Column(String(64), default="")
+    account_created_date = Column(DateTime, default=datetime.utcnow)
+    last_login_date = Column(DateTime, default=datetime.utcnow)
+    password_reset_expired_date = Column(DateTime, default=datetime.utcnow)
+    password_reset_hash = Column(String(128), default="")
+    account_verified = Column(Boolean, default=False)
+    account_activated = Column(Boolean, default=False)
+    account_locked = Column(Boolean, default=False)
+    ldap = Column(Boolean, default=False)
+    ldap_dn = Column(String(64), default="")
+    ldap_username = Column(String(64), default="")
+    admin = Column(Boolean, default=False)
+    pinAttempts = Integer()
+    loginAttempts = Integer()
 
     def __init__(self, email, password, isAdmin=False, skip_password=False):
         self.email = email
         if skip_password is False:
             self.password = password
         self.admin = isAdmin
 
     def __repr__(self):
-        return '<User {} {} : {}>'.format(self.firstname, self.lastname,
+        return '<User {} {} {}>'.format(self.firstname, self.lastname,
                                           self.email)
 
     @hybrid_property
     def password(self):
         return self._password_hash
 
     @password.setter
     def password(self, plaintext_password):
-        self._password_hash = bcrypt.generate_password_hash(plaintext_password)
+        password_bytes = unicode_string_to_bytes(plaintext_password)
+        salt = bcrypt.gensalt(rounds=12, prefix=b'2b')
+        self._password_hash =  bcrypt.hashpw(password_bytes, salt)
 
     @hybrid_method
     def checkPassword(self, plaintext_password):
-        return bcrypt.check_password_hash(self.password, plaintext_password)
+        return bcrypt.checkpw(unicode_string_to_bytes(plaintext_password),self.password)
+
+    @hybrid_property
+    def pin(self):
+        return self._pin_hash
+
+    @pin.setter
+    def pin(self, plaintext_pin):
+        pin_bytes = unicode_string_to_bytes(plaintext_pin)
+        salt = bcrypt.gensalt(rounds=12, prefix=b'2b')
+        self._password_hash =  bcrypt.hashpw(pin_bytes, salt)
+
+    @hybrid_method
+    def checkPin(self, plaintext_pin):
+        return bcrypt.checkpw(unicode_string_to_bytes(plaintext_pin),self.pin)
+
 
     @hybrid_property
     def api_key(self):
         return self._api_key_hash
 
     @api_key.setter
     def api_key(self, plaintext_api_key):
         self._api_key_hash = hashlib.sha512(
             plaintext_api_key.encode('utf8')).hexdigest()
 
     @hybrid_method
     def check_api_key(self, plaintext_api_key):
         return hashlib.sha512(plaintext_api_key).hexdigest() == self.api_key
 
-    @hybrid_property
-    def pin(self):
-        return self._pin_hash
-
-    @pin.setter
-    def pin(self, plaintext_pin):
-        self._pin_hash = bcrypt.generate_password_hash(plaintext_pin)
-
     # checks if user has a certain permission
     @hybrid_method
     def has_permission(self, permission_to_check):
         for permission_group in self.permission_groups:
             for permission in permission_group.permissions:
                 if type(permission_to_check) is str:
                     permission_key = permission_to_check
```

### Comparing `aurori-0.1.4/aurori/users/userManager.py` & `aurori-1.0.1/aurori/users/userManager.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,21 +20,14 @@
 __authors__ = ["Marcus Drobisch"]
 __contact__ = "aurori@fabba.space"
 __credits__ = []
 __license__ = "AGPLv3+"
 
 from aurori.logs import logManager
 import hashlib
-try:
-    import ldap
-except ImportError:
-    logManager.info("Unable to import ldap")
-
-from aurori.workspaces.workspaceHooks import WorkspaceHooks
-
 
 class UserManager(object):
     """ The UserManager ...
     """
     def __init__(self, ):
         # preparation to instanciate
         pass
@@ -42,29 +35,28 @@
     def init_manager(self, app, db, workspaceManager, config):
         self.config = config
         self.app = app
         self.db = db
         self.workspaceManager = workspaceManager
         logManager.info("UserManager initialized")
 
+        try:
+            __import__("ldap")
+        except ImportError:
+            logManager.info("Unable to import ldap")
+
+
         self.user = workspaceManager.user_class
 
     def remove_user(self, email):
         u = self.user.query.filter_by(email=email).first()
         if u is not None:
-            self.workspaceManager.triggerWorkspaceHooks(WorkspaceHooks.REMOVEUSER, user=u)
             self.db.session.delete(u)
             self.db.session.commit()
 
-    def raise_user_creation(self, user):
-        self.workspaceManager.triggerWorkspaceHooks(WorkspaceHooks.CREATEUSER, user=user)                
-
-    def raise_user_removal(self, user):
-        self.workspaceManager.triggerWorkspaceHooks(WorkspaceHooks.REMOVEUSER, user=user)                
-
     def register_user(self, userdata, ldap=False):
         if self.checkUserExist(userdata['email']):
             return None
         else:
             u = self.user(email=userdata['email'],
                           password=userdata['password'],
                           isAdmin=False)
@@ -72,15 +64,14 @@
             u.lastname = userdata['lastname']
             u.organization = userdata['organization']
             u.account_activated = True
             u.ldap = ldap
             if ldap is True:
                 u.ldap_dn = userdata['ldap_dn']
                 u.ldap_username = userdata['ldap_username']
-            self.workspaceManager.triggerWorkspaceHooks(WorkspaceHooks.CREATEUSER, user=u)                
             self.db.session.add(u)
             self.db.session.commit()
             return u
 
     def registerLdapUser(self, email):
         print("")
 
@@ -121,26 +112,27 @@
             api_key_hash = hashlib.sha512(
                 plaintext_api_key.encode('utf8')).hexdigest()
             return self.user.query.filter_by(api_key=api_key_hash).first()
         else:
             return None
 
     def getUser(self, userid):
-        user = self.user.query.filter_by(email=userid).first()
-        if userid is not None:
-            if user is None and self.config['LDAP'].get("enable", False):
-                print("Search for ldap user locally")
-                user = self.user.query.filter_by(ldap_username=userid).first()
-                if user is None:
-                    print("Search for ldap user on server")
-                    try:
-                        user = self.checkLdapUser(userid)
-                    except Exception:
-                        user = None
-        return user
+        with self.db.get_session() as db_session:
+            user = db_session.query(self.user).filter_by(email=userid).first()
+            if userid is not None:
+                if user is None and self.config['LDAP'].get("enable", False):
+                    print("Search for ldap user locally")
+                    user = self.user.query.filter_by(ldap_username=userid).first()
+                    if user is None:
+                        print("Search for ldap user on server")
+                        try:
+                            user = self.checkLdapUser(userid)
+                        except Exception:
+                            user = None
+            return user
 
     def checkUserExist(self, email):
         user = self.user.query.filter_by(email=email).first()
         if user is None:
             return False
         else:
             return True
```

### Comparing `aurori-0.1.4/aurori/workspaces/workspace.py` & `aurori-1.0.1/aurori/workspaces/workspace.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,36 +22,28 @@
 __credits__ = []
 __license__ = "AGPLv3+"
 
 import inspect
 import pkgutil
 import sqlalchemy as sa
 
-from aurori.actions.action import Action
-from aurori.nodes.nodeClass import NodeClass
-from aurori.workspaces import viewHandler
-from aurori.workspaces.dataView import DataView
 from aurori.workspaces.page import Page
 from aurori.workspaces.permission import Permission
 from aurori.jobs.job import Job
-from aurori.monits.monits import Monit
-from aurori.widgets.widget import Widget
 from aurori.jobs import jobManager
-from aurori.nodes import nodeManager
 from aurori.logs import logManager
-from aurori.monits import monit_manager
-from aurori.widgets import widgetManager
+from fastapi import APIRouter
 
 
 class Workspace(object):
     """Base class that each workspaceinherit from. 
        The class define methods that all workspaces have to implement
     """
 
-    disable = False
+    disabled = False
 
     def __init__(self, app, db, name=None, uri=None):
         self.description = 'UNKNOWN'
         if name is None:
             self.name = type(self).__name__
         else:
             self.name = name
@@ -83,99 +75,95 @@
             caption = name
         self.pages[key] = {
             "caption": caption,
             "callback": callback,
             "permission": permission
         }
 
-    def addDataView(self, dataView):
-        key = dataView.name
-        self.dataViews[key] = dataView
-
-    def getPage(self, name):
+    def get_page(self, name):
         key = self.name + "_" + name
         return self.pages[key]
 
-    def discoverJobs(self, workspaceSource):
-        jobSource = workspaceSource + '.' + self.name + '.' + 'jobs'
+    def discover_jobs(self, workspace_source_path):
+        jobSource = workspace_source_path + '.' + self.name + '.jobs'
         imported_source = __import__(jobSource, fromlist=['blah'])
 
         for _, jobname, ispkg in pkgutil.iter_modules(
                 imported_source.__path__, imported_source.__name__ + '.'):
             if not ispkg:
                 job_module = __import__(jobname, fromlist=['blah'])
                 clsmembers = inspect.getmembers(job_module, inspect.isclass)
                 for (_, c) in clsmembers:
-                    # Check for DataView classes
                     if issubclass(c, Job) & (c is not Job):
                         if c.disable is False:
                             logManager.info(
-                                f'Job registered from "{c.__module__}"')
+                                f'    Job registered from "{c.__module__}"')
                             jobManager.register_job(self, c, True)
 
-    def discoverMonits(self, workspaceSource, workspace):
-        monit_source = workspaceSource + '.' + self.name + '.monits'
-
-        monit_module = __import__(monit_source, fromlist=['blah'])
+    def discover_apis(self, workspace_source_path, api_prefix):
+        api_workspace_path = workspace_source_path + '.' + self.name + '.api'
+        api_source = __import__(api_workspace_path, fromlist=['blah'])
+        for _, modulename, ispkg in pkgutil.iter_modules(
+                api_source.__path__, api_source.__name__ + '.'):
+            if not ispkg:
+                api_module = __import__(modulename,
+                                               fromlist=['blah'])
+                clsmembers = inspect.getmembers(api_module)
+                for (api_name, c) in clsmembers:
+                    if isinstance(c, APIRouter):
+                        logManager.info(
+                            f'    API "{api_name}" loaded from "{modulename}"'
+                        )
+                        self.app.include_router(c,prefix=api_prefix+"/" + self.uri, tags=["App." + self.name])
 
-        clsmembers = inspect.getmembers(monit_module, inspect.isclass)
-        for (_, c) in clsmembers:
-            # Check for Monit classes
-            if issubclass(c, Monit) & (c is not Monit):
-                monit_instance = c(workspace)
-                monit_instance.define_views()
-                logManager.info(
-                    f'Monit: "{monit_instance.name}"" loaded from "{c.__module__}"'
-                )
-                monit_manager.register_monit(monit_instance)
 
-    def discoverPermissions(self, workspaceSource):
-        permissionsSource = workspaceSource + '.' + self.name
+    def discover_permissions(self, workspace_source):
+        permissionsSource = workspace_source + '.' + self.name
         imported_source = __import__(permissionsSource, fromlist=['blah'])
 
         for _, permissionname, ispkg in pkgutil.iter_modules(
                 imported_source.__path__, imported_source.__name__ + '.'):
             if not ispkg:
                 permission_module = __import__(permissionname,
                                                fromlist=['blah'])
                 clsmembers = inspect.getmembers(permission_module,
                                                 inspect.isclass)
                 for (_, c) in clsmembers:
                     # Check for Permission classes
                     if issubclass(c, Permission) & (c is not Permission):
                         permissionInstance = c()
                         logManager.info(
-                            f'Permission: "{permissionInstance.name}"" loaded from "{c.__module__}"'
+                            f'    Permission "{permissionInstance.name}" loaded from "{c.__module__}"'
                         )
-                        self.addPermission(str(permissionInstance.name),
+                        self.add_permission(str(permissionInstance.name),
                                            permissionInstance)
 
-    def discoverSections(self, workspaceSource):
+    def discoverSections(self, workspace_source_path):
         '''
-        sectionsSource = workspaceSource + '.' + self.name
+        sectionsSource = workspace_source_path + '.' + self.name
         imported_source = __import__(sectionsSource, fromlist=['blah'])
 
         for _, sectionname, ispkg in pkgutil.iter_modules(imported_source.__path__, imported_source.__name__ + '.'):
             if not ispkg:
                 section_module = __import__(sectionname, fromlist=['blah'])
                 clsmembers = inspect.getmembers(section_module, inspect.isclass)
                 for (_, c) in clsmembers:
                     # Check for Section classes
                     if issubclass(c, Section) & (c is not Section):
                         sectionInstance = c()
                         logManager.info(f'Section: "{c.__module__}" created for workspace: "{self.name}"')
                         #self.dataViews[str(dataViewInstance.uri)] = (dataViewInstance)
         '''
 
-    def discoverNodeClasses(self, workspaceSource):
+    def discoverNodeClasses(self, workspace_source_path):
         # for _, node_class, ispkg in pkgutil.iter_modules(imported_source.__path__, imported_source.__name__ + '.'):
         #    if ispkg:
         #        print(node_class)
 
-        node_sources = workspaceSource + '.' + self.name + '.' + 'nodes'
+        node_sources = workspace_source_path + '.' + self.name + '.' + 'nodes'
         imported_source = __import__(node_sources, fromlist=['blah'])
 
         for _, nodename, ispkg in pkgutil.iter_modules(
                 imported_source.__path__, imported_source.__name__ + '.'):
             if not ispkg:
                 node_module = __import__(nodename, fromlist=['blah'])
                 clsmembers = inspect.getmembers(node_module, inspect.isclass)
@@ -206,39 +194,39 @@
                         if c.disable is False:
                             logManager.info(f'NodeClass: "{c.__module__}" loaded from "{node_sources}"')
                             nodeManager.register_node_class(self, c)
                         else:
                             logManager.info(f'NodeClass: "{c.__module__}" is disabled and wont show up"')
         '''
 
-    def discoverPages(self, workspaceSource):
-        pagesSource = workspaceSource + '.' + self.name + '.' + 'pages'
+    def discover_pages(self, workspace_source_path):
+        pagesSource = workspace_source_path + '.' + self.name + '.' + 'pages'
         imported_source = __import__(pagesSource, fromlist=['blah'])
 
         for _, pagename, ispkg in pkgutil.iter_modules(
                 imported_source.__path__, imported_source.__name__ + '.'):
             if not ispkg:
                 page_module = __import__(pagename, fromlist=['blah'])
                 clsmembers = inspect.getmembers(page_module, inspect.isclass)
                 for (_, c) in clsmembers:
                     # Check for DataView classes
                     if issubclass(c, Page) & (c is not Page):
                         pageInstance = c()
                         logManager.info(
-                            f'Page: "{pageInstance.name}" loaded from "{c.__module__}"'
+                            f'    Page: "{pageInstance.name}" loaded from "{c.__module__}"'
                         )
                         if pageInstance.disable is True:
                             logManager.info(
-                                f'Page: "{pageInstance.name}" is disabled and wont show up'
+                                f'    Page: "{pageInstance.name}" is disabled and wont show up'
                             )
                         else:
                             self.pages[str(pageInstance.name)] = pageInstance
 
-    def discoverDataViews(self, workspaceSource):
-        actionsSource = workspaceSource + '.' + self.name + '.' + 'views'
+    def discoverDataViews(self, workspace_source_path):
+        actionsSource = workspace_source_path + '.' + self.name + '.' + 'views'
         imported_source = __import__(actionsSource, fromlist=['blah'])
 
         for _, actionname, ispkg in pkgutil.iter_modules(
                 imported_source.__path__, imported_source.__name__ + '.'):
             if not ispkg:
                 action_module = __import__(actionname, fromlist=['blah'])
                 clsmembers = inspect.getmembers(action_module, inspect.isclass)
@@ -268,15 +256,15 @@
                                 dataViewInstance.uri)] = (dataViewInstance)
 
                         if dataViewInstance.entrykey is None:
                             raise LookupError(
                                 "DataView {} dont define a key".format(
                                     dataViewInstance.name))
 
-    def discoverActions(self, workspaceSource):
+    def discoverActions(self, workspace_source_path):
 
         # create manager wide generic handlers for the view
         self.getViewActionHandler = viewHandler.GetViewActionHandler(
             self.app, self.db)
         self.createViewEntryActionHandler = viewHandler.CreateViewEntryActionHandler(
             self.app, self.db)
         self.removeViewEntryActionHandler = viewHandler.RemoveViewEntryActionHandler(
@@ -294,15 +282,15 @@
         self.actions.append(self.updateViewEntryActionHandler)
         self.actions.append(self.executeViewActionsActionHandler)
 
         logManager.info(
             f'Actions for handling DataViews created for workspace "{self.name}"'
         )
 
-        actionsSource = workspaceSource + '.' + self.name + '.' + 'actions'
+        actionsSource = workspace_source_path + '.' + self.name + '.' + 'actions'
         # print("Discover actions for", self.uri, "from", actionsSource)
         imported_source = __import__(actionsSource, fromlist=['blah'])
 
         # print(imported_source)
 
         for _, actionname, ispkg in pkgutil.iter_modules(
                 imported_source.__path__, imported_source.__name__ + '.'):
@@ -319,16 +307,16 @@
                         if actionInstance.disable is True:
                             logManager.info(
                                 f'Action: "{actionInstance.name}" is disabled and wont show up'
                             )
                         else:
                             self.actions.append(actionInstance)
 
-    def discoverCommands(self, workspaceSource):
-        commandSource = workspaceSource + '.' + self.name + '.' + 'commands'
+    def discoverCommands(self, workspace_source_path):
+        commandSource = workspace_source_path + '.' + self.name + '.' + 'commands'
         try:
             imported_source = __import__(commandSource, fromlist=['blah'])
             for _, commandname, ispkg in pkgutil.iter_modules(
                     imported_source.__path__, imported_source.__name__ + '.'):
                 if not ispkg:
                     try:
                         command_module = __import__(commandname,
@@ -344,16 +332,16 @@
                             'Unable to import: {}, exception: {}'.format(
                                 commandname, e))
 
             self.app.cli.add_command(imported_source.user_cli)
         except Exception:
             pass
 
-    def discoverWidgets(self, workspaceSource):
-        widgetSource = workspaceSource + '.' + self.name + '.' + 'widgets'
+    def discoverWidgets(self, workspace_source_path):
+        widgetSource = workspace_source_path + '.' + self.name + '.' + 'widgets'
         try:
             imported_source = __import__(widgetSource, fromlist=['blah'])
             for _, widgetname, ispkg in pkgutil.iter_modules(
                     imported_source.__path__, imported_source.__name__ + '.'):
                 if not ispkg:
                     widget_module = __import__(widgetname, fromlist=['blah'])
                     clsmembers = inspect.getmembers(widget_module,
@@ -373,36 +361,37 @@
                                 logManager.info(
                                     f'Widget disabled and not registered from "{c.__module__}"'
                                 )
 
         except Exception:
             pass
 
-    def addPermission(self, name, permission):
+    def add_permission(self, name, permission):
         from .models import Permission
         from aurori import db
         key = self.name + "." + name
         description = "No description available"
 
         if hasattr(permission, 'description'):
             description = permission.description
 
-        engine = db.get_engine()
+        engine = db.engine
         table_exists = sa.inspect(engine).has_table(Permission.__tablename__)
         if table_exists:
-            p = Permission.query.filter_by(name=key).first()
-            if p is None:
-                p = Permission(name=key, description=description)
-                db.session.add(p)
-                db.session.commit()
-                p = Permission.query.filter_by(name=key).first()
-            else:
-                p.caption = description
-                db.session.commit()
-            self.permissions[key] = p
+            with db.get_session() as db_session:
+                p = db_session.query(Permission).filter_by(name=key).first()
+                if p is None:
+                    p = Permission(name=key, description=description)
+                    db_session.add(p)
+                    db_session.commit()
+                    p = db_session.query(Permission).filter_by(name=key).first()
+                else:
+                    p.caption = description
+                    db_session.commit()
+                self.permissions[key] = p
         else:
             logManager.error(
                 'Unable to create permission "{}" for workspace {}'.format(
                     name, self.name))
 
     def getPermission(self, name):
         key = self.name + "." + name
```

### Comparing `aurori-0.1.4/aurori/workspaces/workspaceManager.py` & `aurori-1.0.1/aurori/workspaces/workspaceManager.py`

 * *Files 20% similar despite different names*

```diff
@@ -23,243 +23,150 @@
 __license__ = "AGPLv3+"
 
 import os
 import pathlib
 import pkgutil
 import inspect
 from aurori.workspaces.workspace import Workspace
-from aurori.workspaces.workspaceHooks import WorkspaceHooks
 from aurori.logs import logManager
 import sys
 import traceback
 import sqlalchemy as sa
 
 
 class WorkspaceManager(object):
     """ The WorkspaceManager holds all available workspaces and load them while creation.
     """
-    def __init__(self, workspaceSource):
-        self.workspaceSource = workspaceSource
+    def __init__(self, workspace_source_path):
+        self.workspace_source_path = workspace_source_path
         self.app = None
         self.db = None
         self.config = None
         self.workspaces = None
         self.user_class = None
+        self.api_prefix = None
 
-    def init_app(self, app, db, config):
+    def init_app(self, app, config, minimal = False, api_prefix="api/v1"):
         self.app = app
-        self.db = db
         self.config = config
-        with self.app.app_context():
-            self.reloadWorkspaces()
-            self.registerWorkspacePlugins()
-            self.registerWorkspacePermissions()
-            self.registerWorkspaceAPIs()
-            logManager.info("Workspaces initialized")
+        self.workspaces = []
+        self.seen_paths = []
+        self.api_prefix = api_prefix
+        logManager.info("")
+        logManager.info(
+            f'Discover workspaces in path : {self.workspace_source_path}')
+        self.discover_workspaces(self.workspace_source_path)
+        self.discover_models()
+        if minimal is False:
+            self.discover_permissions()
+            self.create_permissions()
+            self.discover_jobs()
+            self.discover_pages()
+            self.discover_apis()
+
+        #    self.registerWorkspacePermissions()
+        #    self.registerWorkspaceAPIs()
+
+        logManager.info("")
+        logManager.info("Workspaces and their components initialized")
 
-    def getWorkspace(self, name):
+    def get_workspace(self, name):
         for w in self.workspaces:
             if w.name is name:
                 return w
         return None
 
-    def triggerWorkspaceHooks(self, hook: WorkspaceHooks, **kwargs):
-        for w in self.workspaces:
-            try:
-                if hook == WorkspaceHooks.CREATEUSER:
-                    w.createUserHook(**kwargs)
-                if hook == WorkspaceHooks.REMOVEUSER:
-                    w.removeUserHook(**kwargs)
-            except Exception as e:
-                logManager.error('Failed to run hook {} on {} with {}'.format(
-                    hook, w.name, e))
-
-    def reloadWorkspaces(self):
+    def reload_workspaces(self):
         """Reset the list of all plugins and initiate the walk over the main
         provided plugin package to load all available plugins
         """
         self.workspaces = []
         self.seen_paths = []
         logManager.info("")
         logManager.info(
-            f'Discover workspaces in path : {self.workspaceSource}')
-        self.discover_workspaces(self.workspaceSource)
-
-    def registerWorkspacePermissions(self):
-        """ Run createPermissions for all workspaces and store permissions
-        """
-        logManager.info("")
-        all_permissions = {}
-        for ws in self.workspaces:
-
-            workspace_permissions = ws.permissions
-            if workspace_permissions is not None:
-                all_permissions = {**all_permissions, **workspace_permissions}
-            logManager.info(
-                f'Register permissions for {ws.name}-workspace : {workspace_permissions}'
-            )
-
-        logManager.info(f'Delete orphaned permissions')
-
-        # delete orphaned permissions for security reasons
-        from .models import Permission
-        from aurori import db
-        engine = db.get_engine()
-        table_exists = sa.inspect(engine).has_table(Permission.__tablename__)
-        if table_exists:
-            db_permissions = Permission.query.all()
-            for permission in db_permissions:
-                if permission.name not in all_permissions:
-                    print("Delete orphaned permission: ", permission)
-                    db.session.delete(permission)
-                    db.session.commit()
-
-    def registerWorkspaceAPIs(self):
-        from aurori.api.check import check_before_request
+            f'Discover workspaces in path : {self.workspace_source_path}')
+        self.discover_workspaces(self.workspace_source_path)
 
-        logManager.info("")
-        logManager.info("Register api's of workspaces:")
-        logManager.info("")
-        for w in self.workspaces:
-            api_workspace_path = (self.workspaceSource) + '.' + w.name + '.api'
-            try:
-                api_module = __import__(api_workspace_path, fromlist=['blah'])
-                module_members = inspect.getmembers(api_module)
-                blueprint = None
-                for _name, member in module_members:
-                    if _name == 'workspace_bp':
-                        blueprint = member
-                if blueprint is not None:
-                    logManager.info(f'Register "{w.name}" workspace API')
-                    blueprint.before_request(check_before_request)
-                    self.app.register_blueprint(
-                        blueprint,
-                        url_prefix='/api/v1/workspaces/' + str(w.name.lower()))
-                    pass
-            except ModuleNotFoundError:
-                logManager.info(
-                    f'No specific API found for "{w.name}" workspace')
-        logManager.info("")
+    def discover_permissions(self):
 
-    def registerWorkspacePlugins(self):
-        """Recursively walk the supplied package to retrieve components for all plugins (workspaces)
-        """
-        logManager.info("")
-        logManager.info("Register components from workspaces:")
         logManager.info("")
+        logManager.info("Discover permissions:")
 
         for w in self.workspaces:
-            logManager.info(f'Workspace: "{w.name}"')
+            logManager.info(f'  For workspace: "{w.name}"')
 
             # try to register permissions
             try:
-                w.discoverPermissions(self.workspaceSource)
+                w.discover_permissions(self.workspace_source_path)
             except Exception as e:
                 traceback.print_exc(file=sys.stdout)
                 logManager.error(
-                    f'Workspace "{w.name}" unable to discover permissions  ({str(type(e).__name__)}:{e})'
+                    f'  Workspace "{w.uri}" unable to discover permissions  ({str(type(e).__name__)}:{e})'
                 )
 
-            # try to register monits
-            try:
-                w.discoverMonits(self.workspaceSource, w)
-            except ModuleNotFoundError:
-                logManager.info(f'No monits discovered for "{w.name}"')
-            except Exception as e:
-                traceback.print_exc(file=sys.stdout)
-                logManager.error(
-                    f'Workspace "{w.name}" unable to discover monits  ({str(type(e).__name__)}:{e})'
-                )
+    def discover_pages(self):
+        logManager.info("")
+        logManager.info("Discover pages:")
+
+        for w in self.workspaces:
+            logManager.info(f'  For workspace: "{w.name}"')
+            workspace_config_section_name = pathlib.Path(
+                w.path).resolve().name.upper()
+            # try to register permissions
 
-            # try to register dataViews
             try:
-                w.discoverDataViews(self.workspaceSource)
-            except Exception as e:
+                w.discover_pages(self.workspace_source_path)
+            except Exception as exception:
                 traceback.print_exc(file=sys.stdout)
                 logManager.error(
-                    f'Workspace "{w.name}" unable to discover dataviews  ({str(type(e).__name__)}:{e})'
+                    f'  Workspace "{w.name}" unable to discover pages  ({str(type(exception).__name__)}:{exception})'
                 )
 
+    def discover_jobs(self):
+        logManager.info("")
+        logManager.info("Discover jobs:")
+
+        for w in self.workspaces:
+            logManager.info(f'  For workspace: "{w.name}"')
             workspace_config_section_name = pathlib.Path(
                 w.path).resolve().name.upper()
 
             if workspace_config_section_name in self.config and "disable_jobs" in self.config[
                     workspace_config_section_name] and self.config[
                         workspace_config_section_name]["disable_jobs"]:
-                logManager.info(f'Jobs for "{w.name}" are disabled by config')
+                logManager.info(f'    Jobs for "{w.name}" are disabled by config')
             else:
                 # try to register jobs
                 try:
-                    w.discoverJobs(self.workspaceSource)
+                    w.discover_jobs(self.workspace_source_path)
                 except Exception as e:
                     traceback.print_exc(file=sys.stdout)
                     logManager.error(
-                        f'Workspace "{w.name}" unable to discover jobs  ({str(type(e).__name__)}:{e})'
+                        f'    Workspace "{w.name}" unable to discover jobs  ({str(type(e).__name__)}:{e})'
                     )
 
-            # try to register actions
-            try:
-                w.discoverActions(self.workspaceSource)
-            except Exception as exception:
-                traceback.print_exc(file=sys.stdout)
-                logManager.error(
-                    f'Workspace "{w.name}" unable to discover actions  ({str(type(exception).__name__)}:{exception})'
-                )
-
-            # try to register sections
-            try:
-                w.discoverSections(self.workspaceSource)
-            except Exception as exception:
-                traceback.print_exc(file=sys.stdout)
-                logManager.error(
-                    f'Workspace "{w.name}" unable to discover sections  ({str(type(exception).__name__)}:{exception})'
-                )
-
-            # try to register node classes
-            try:
-                w.discoverNodeClasses(self.workspaceSource)
-            except ModuleNotFoundError as me:
-                logManager.info(f'No node classes discover for "{w.name}"')
-            except Exception as exception:
-                traceback.print_exc(file=sys.stdout)
-                logManager.error(
-                    f'Workspace "{w.name}" unable to discover node classes ' +
-                    f'({str(type(exception).__name__)}:{exception})')
-
-            # try to register permissions
-            try:
-                w.discoverPages(self.workspaceSource)
-            except Exception as exception:
-                traceback.print_exc(file=sys.stdout)
-                logManager.error(
-                    f'Workspace "{w.name}" unable to discover pages  ({str(type(exception).__name__)}:{exception})'
-                )
-
-            # try to register command line commands
-            try:
-                w.discoverCommands(self.workspaceSource)
-            except Exception as exception:
-                traceback.print_exc(file=sys.stdout)
-                logManager.error(
-                    f'Workspace "{w.name}" unable to discover commands  ({str(type(exception).__name__)}:{exception})'
-                )
+    def discover_apis(self):
+        logManager.info("")
+        logManager.info("Discover apis:")
 
-            # try to register widgets
+        for w in self.workspaces:
+            logManager.info(f'  For workspace: "{w.name}"')
+            workspace_config_section_name = pathlib.Path(
+                w.path).resolve().name.upper()
+            
             try:
-                w.discoverWidgets(self.workspaceSource)
+                w.discover_apis(self.workspace_source_path, self.api_prefix)
             except Exception as exception:
                 traceback.print_exc(file=sys.stdout)
                 logManager.error(
-                    f'Workspace "{w.name}" unable to discover widgets ({str(type(exception).__name__)}:{exception})'
+                    f'  Workspace "{w.name}" unable to apis pages  ({str(type(exception).__name__)}:{exception})'
                 )
-
-            logManager.info("")
-
+                
     def discover_models(self):
-        source = self.workspaceSource
+        source = self.workspace_source_path
         try:
             imported_source = __import__(source, fromlist=['blah'])
         except Exception as exception:
             logManager.error(f"Unable to locate workspaces {str(exception)}")
             return
         all_current_paths = []
 
@@ -300,15 +207,14 @@
                             if issubclass(c, UserBase) & (c is not UserBase):
                                 if self.user_class is not None and self.user_class != c:
                                     raise Exception("Multiple User models found. For a aurori app only one is allowed.")
                                 self.user_class = c
                 except ModuleNotFoundError:
                     modelmodule = source + '.' + child_pkg + '.models'
                     logManager.info(f'No model found for {modelmodule}')
-                print(child_pkg)
         
         if self.user_class is None:
             logManager.warning(f'No User model derived from aurori.users.basemodels.UserBase found.')
             logManager.warning(f'A aurori app needs a user model to work properly.')
             logManager.warning(f'Please define a derived model named "User" in your workspaces, if needed.')
             logManager.warning(f'The default model will be used, please reference: aurori.users.defaultmodels.User ')
             from aurori.users.defaultmodels import User
@@ -342,71 +248,80 @@
                 if os.path.isdir(os.path.join(pkg_path, p))
             ]
 
             # Every sub directory contains one workspace
             for child_pkg in child_pkgs:
                 imported_package = __import__(source + '.' + child_pkg,
                                               fromlist=['blah'])
-                for _, workspacename, ispkg in pkgutil.iter_modules(
-                        imported_package.__path__,
-                        imported_package.__name__ + '.'):
-                    workspaceCounter = 0
-                    if not ispkg:
-                        workspace_module = __import__(workspacename,
-                                                      fromlist=['blah'])
-                        clsmembers = inspect.getmembers(
-                            workspace_module, inspect.isclass)
+                
+                clsmembers = inspect.getmembers(imported_package)
+              
+                uri = ""
+                if hasattr(imported_package,"uri"):
+                    uri = imported_package.uri
+                else:
+                    uri = str(child_pkg).lower()
+
+                logger = None
+                if hasattr(imported_package,"logger"):
+                    logger = imported_package.logger
+
+
+                workspaceInstance = Workspace(self.app, self.db, str(child_pkg), uri)
+
+                if hasattr(imported_package,"description"):
+                    workspaceInstance.description = imported_package.description
+
+                if hasattr(imported_package,"disabled"):
+                    workspaceInstance.disabled = imported_package.disabled
+
+                workspaceInstance.path = os.path.dirname(
+                    imported_package.__file__)
+                workspace_config_section_name = pathlib.Path(
+                    imported_package.__file__).parent.resolve(
+                    ).name.upper()
+                logManager.info(
+                    f'  Discovered workspace "{workspaceInstance.name}" as "{workspaceInstance.uri}" from "{source + "." + child_pkg}"')
 
-                        for (_, c) in clsmembers:
-                            # Check for workspace classes
-                            if issubclass(c, Workspace) & (c is not Workspace):
-                                workspaceCounter += 1
-                                if workspaceCounter > 1:
-                                    logManager.error(
-                                        'Only one workspace is allowed for one folder, other workspaces will skipped'
-                                    )
-                                    break
-
-                                uri = ""
-                                if hasattr(c, 'uri'):
-                                    uri = c.uri
-                                else:
-                                    logManager.error(
-                                        f'No uri defined and will not be accessable for workspace: {c.__module__}'
-                                    )
-
-                                name = c.__name__
-                                if hasattr(c, 'name'):
-                                    name = c.name
-                                workspaceInstance = c(self.app, self.db, name,
-                                                      uri)
-                                workspaceInstance.path = os.path.dirname(
-                                    workspace_module.__file__)
-                                workspace_config_section_name = pathlib.Path(
-                                    workspace_module.__file__).parent.resolve(
-                                    ).name.upper()
-                                logManager.info(
-                                    f'Workspace discovered : {workspaceInstance.name} [{c.__module__}]'
-                                    + f' with uri "{workspaceInstance.uri}"')
-
-                                if (workspace_config_section_name
-                                        in self.config) and (
-                                            "disable" in self.config[
-                                                workspace_config_section_name]
-                                        ) and (self.config[
-                                            workspace_config_section_name]
-                                               ["disable"]):
-                                    logManager.info(
-                                        f'Workspace {workspaceInstance.name} [{c.__module__}]'
-                                        +
-                                        ' is disabled by config and wont show up'
-                                    )
-                                else:
-                                    if workspaceInstance.disable is True:
-                                        logManager.info(
-                                            f'Workspace {workspaceInstance.name} [{c.__module__}]'
-                                            +
-                                            ' is disabled by definition and wont show up'
-                                        )
-                                    else:
-                                        self.workspaces.append(
-                                            workspaceInstance)
+                if (workspace_config_section_name
+                        in self.config) and (
+                            "disabled" in self.config[
+                                workspace_config_section_name]
+                        ) and (self.config[
+                            workspace_config_section_name]
+                                ["disabled"]):
+                    logManager.info(
+                        '  The workspace is disabled by config and wont show up'
+                    )
+                else:
+                    if workspaceInstance.disabled is True:
+                        logManager.info(
+                            '  The workspace is disabled by module definition and wont show up'
+                        )
+                    else:
+                        logManager.register_logger(logger, workspaceInstance.name)
+                        self.workspaces.append(
+                            workspaceInstance)
+
+    def create_permissions(self):
+        """ Run createPermissions for all workspaces and store permissions
+        """
+        all_permissions = {}
+        for ws in self.workspaces:
+
+            workspace_permissions = ws.permissions
+            if workspace_permissions is not None:
+                all_permissions = {**all_permissions, **workspace_permissions}
+
+        # delete orphaned permissions for security reasons
+        from .models import Permission
+        from aurori import db
+        engine = db.engine
+        table_exists = sa.inspect(engine).has_table(Permission.__tablename__)
+        if table_exists:
+            with db.get_session() as db_session:
+                db_permissions = db_session.query(Permission).all()
+                for permission in db_permissions:
+                    if permission.name not in all_permissions:
+                        logManager.warning(f'  Delete orphaned {permission}')
+                        db_session.delete(permission)
+                        db_session.commit()
```

### Comparing `aurori-0.1.4/aurori_icon.inkscape.svg` & `aurori-1.0.1/aurori_icon.inkscape.svg`

 * *Files identical despite different names*

### Comparing `aurori-0.1.4/aurori_logo.inkscape.svg` & `aurori-1.0.1/aurori_logo.inkscape.svg`

 * *Files identical despite different names*

### Comparing `aurori-0.1.4/scripts/quality_report.py` & `aurori-1.0.1/scripts/quality_report.py`

 * *Files identical despite different names*

### Comparing `aurori-0.1.4/setup.cfg` & `aurori-1.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `aurori-0.1.4/tests/api_test/action_test.py` & `aurori-1.0.1/tests/api_test/action_test.py`

 * *Files identical despite different names*

