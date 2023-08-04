# Comparing `tmp/meerschaum-1.6.9.tar.gz` & `tmp/meerschaum-1.7.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meerschaum-1.6.9.tar", last modified: Fri May 12 17:43:14 2023, max compression
+gzip compressed data, was "meerschaum-1.7.0.dev1.tar", last modified: Fri Aug  4 04:46:20 2023, max compression
```

## Comparing `meerschaum-1.6.9.tar` & `meerschaum-1.7.0.dev1.tar`

### file list

```diff
@@ -1,279 +1,280 @@
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.914779 meerschaum-1.6.9/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11359 2021-12-27 13:50:47.000000 meerschaum-1.6.9/LICENSE
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      114 2021-12-27 13:50:47.000000 meerschaum-1.6.9/NOTICE
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10798 2023-05-12 17:43:14.913779 meerschaum-1.6.9/PKG-INFO
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9248 2022-07-13 02:48:08.000000 meerschaum-1.6.9/README.md
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.890779 meerschaum-1.6.9/meerschaum/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1236 2023-04-25 23:57:31.000000 meerschaum-1.6.9/meerschaum/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2774 2022-10-22 06:28:47.000000 meerschaum-1.6.9/meerschaum/__main__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.891779 meerschaum-1.6.9/meerschaum/_internal/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      169 2022-04-23 01:15:00.000000 meerschaum-1.6.9/meerschaum/_internal/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.891779 meerschaum-1.6.9/meerschaum/_internal/arguments/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      519 2022-10-22 06:25:53.000000 meerschaum-1.6.9/meerschaum/_internal/arguments/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9741 2023-04-25 23:57:31.000000 meerschaum-1.6.9/meerschaum/_internal/arguments/_parse_arguments.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12375 2023-05-12 06:36:07.000000 meerschaum-1.6.9/meerschaum/_internal/arguments/_parser.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.892779 meerschaum-1.6.9/meerschaum/_internal/docs/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      126 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/_internal/docs/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7719 2022-04-24 10:29:36.000000 meerschaum-1.6.9/meerschaum/_internal/docs/index.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4625 2023-04-25 23:57:31.000000 meerschaum-1.6.9/meerschaum/_internal/entry.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.892779 meerschaum-1.6.9/meerschaum/_internal/gui/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1332 2022-04-24 10:29:36.000000 meerschaum-1.6.9/meerschaum/_internal/gui/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.892779 meerschaum-1.6.9/meerschaum/_internal/gui/app/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1565 2022-04-24 10:29:36.000000 meerschaum-1.6.9/meerschaum/_internal/gui/app/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2632 2022-10-18 06:13:35.000000 meerschaum-1.6.9/meerschaum/_internal/gui/app/_windows.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1016 2022-04-24 10:29:36.000000 meerschaum-1.6.9/meerschaum/_internal/gui/app/actions.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1678 2022-04-24 10:29:36.000000 meerschaum-1.6.9/meerschaum/_internal/gui/app/pipes.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.892779 meerschaum-1.6.9/meerschaum/_internal/shell/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    31489 2023-01-09 09:23:24.000000 meerschaum-1.6.9/meerschaum/_internal/shell/Shell.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2981 2022-10-22 06:28:01.000000 meerschaum-1.6.9/meerschaum/_internal/shell/ShellCompleter.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1280 2022-10-26 04:20:20.000000 meerschaum-1.6.9/meerschaum/_internal/shell/ValidAutoSuggest.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      281 2022-04-24 10:29:36.000000 meerschaum-1.6.9/meerschaum/_internal/shell/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.893779 meerschaum-1.6.9/meerschaum/_internal/shell/resources/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2022-04-24 10:29:36.000000 meerschaum-1.6.9/meerschaum/_internal/shell/resources/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.893779 meerschaum-1.6.9/meerschaum/_internal/term/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      612 2021-12-09 07:32:03.000000 meerschaum-1.6.9/meerschaum/_internal/term/TermPageHandler.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1495 2021-12-09 07:32:03.000000 meerschaum-1.6.9/meerschaum/_internal/term/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      788 2022-02-28 20:55:01.000000 meerschaum-1.6.9/meerschaum/_internal/term/tools.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.895779 meerschaum-1.6.9/meerschaum/actions/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8129 2022-10-26 04:20:20.000000 meerschaum-1.6.9/meerschaum/actions/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10996 2023-01-09 09:23:24.000000 meerschaum-1.6.9/meerschaum/actions/api.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    14529 2023-04-25 23:57:31.000000 meerschaum-1.6.9/meerschaum/actions/bootstrap.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4857 2022-08-23 06:14:42.000000 meerschaum-1.6.9/meerschaum/actions/clear.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6095 2022-12-05 04:26:42.000000 meerschaum-1.6.9/meerschaum/actions/copy.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    15245 2023-01-09 09:23:24.000000 meerschaum-1.6.9/meerschaum/actions/delete.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2701 2022-06-27 01:07:31.000000 meerschaum-1.6.9/meerschaum/actions/drop.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9492 2023-04-25 23:57:31.000000 meerschaum-1.6.9/meerschaum/actions/edit.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7380 2022-10-18 06:13:35.000000 meerschaum-1.6.9/meerschaum/actions/install.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4206 2022-02-28 20:55:01.000000 meerschaum-1.6.9/meerschaum/actions/login.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2251 2022-08-29 21:54:10.000000 meerschaum-1.6.9/meerschaum/actions/os.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2395 2022-02-28 20:55:01.000000 meerschaum-1.6.9/meerschaum/actions/python.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11219 2023-04-25 23:57:31.000000 meerschaum-1.6.9/meerschaum/actions/register.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      605 2022-02-28 20:55:01.000000 meerschaum-1.6.9/meerschaum/actions/reload.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3211 2023-01-09 09:23:24.000000 meerschaum-1.6.9/meerschaum/actions/setup.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2026 2022-08-29 21:54:10.000000 meerschaum-1.6.9/meerschaum/actions/sh.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    23468 2023-01-11 06:27:06.000000 meerschaum-1.6.9/meerschaum/actions/show.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4224 2022-02-28 20:55:01.000000 meerschaum-1.6.9/meerschaum/actions/sql.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5501 2022-10-25 06:38:00.000000 meerschaum-1.6.9/meerschaum/actions/stack.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    18247 2022-11-22 01:55:36.000000 meerschaum-1.6.9/meerschaum/actions/start.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3948 2023-01-16 21:21:28.000000 meerschaum-1.6.9/meerschaum/actions/stop.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    15339 2022-12-15 02:09:06.000000 meerschaum-1.6.9/meerschaum/actions/sync.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6073 2022-08-19 04:59:44.000000 meerschaum-1.6.9/meerschaum/actions/uninstall.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6307 2022-08-19 04:59:44.000000 meerschaum-1.6.9/meerschaum/actions/upgrade.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3348 2022-10-26 04:20:20.000000 meerschaum-1.6.9/meerschaum/actions/verify.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.896779 meerschaum-1.6.9/meerschaum/api/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7638 2022-12-05 04:26:42.000000 meerschaum-1.6.9/meerschaum/api/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      875 2022-02-28 20:55:01.000000 meerschaum-1.6.9/meerschaum/api/_chain.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      966 2022-08-19 04:59:44.000000 meerschaum-1.6.9/meerschaum/api/_events.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      945 2022-08-19 04:59:44.000000 meerschaum-1.6.9/meerschaum/api/_oauth2.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1226 2022-11-05 03:38:45.000000 meerschaum-1.6.9/meerschaum/api/_websockets.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.897779 meerschaum-1.6.9/meerschaum/api/dash/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2238 2023-01-09 08:57:26.000000 meerschaum-1.6.9/meerschaum/api/dash/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9600 2022-10-31 13:18:31.000000 meerschaum-1.6.9/meerschaum/api/dash/actions.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.898779 meerschaum-1.6.9/meerschaum/api/dash/assets/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/api/dash/assets/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    21923 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/api/dash/assets/ansi_up.js
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)   338636 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/api/dash/assets/banner_1920x320.png
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9662 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/api/dash/assets/favicon.ico
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10218 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/api/dash/assets/logo_48x48.png
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    67702 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/api/dash/assets/logo_500x500.png
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.899779 meerschaum-1.6.9/meerschaum/api/dash/callbacks/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      283 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/api/dash/callbacks/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    24874 2023-01-09 09:23:24.000000 meerschaum-1.6.9/meerschaum/api/dash/callbacks/dashboard.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2529 2023-01-09 09:04:18.000000 meerschaum-1.6.9/meerschaum/api/dash/callbacks/login.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2777 2022-07-26 06:45:25.000000 meerschaum-1.6.9/meerschaum/api/dash/callbacks/plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3446 2023-04-25 23:57:31.000000 meerschaum-1.6.9/meerschaum/api/dash/callbacks/register.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6771 2022-10-31 13:18:31.000000 meerschaum-1.6.9/meerschaum/api/dash/components.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      843 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/api/dash/connectors.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2072 2022-07-26 06:45:25.000000 meerschaum-1.6.9/meerschaum/api/dash/graphs.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3544 2022-07-26 06:45:25.000000 meerschaum-1.6.9/meerschaum/api/dash/jobs.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13682 2022-10-31 13:18:31.000000 meerschaum-1.6.9/meerschaum/api/dash/keys.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.899779 meerschaum-1.6.9/meerschaum/api/dash/pages/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      273 2023-01-09 09:23:24.000000 meerschaum-1.6.9/meerschaum/api/dash/pages/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3838 2022-10-31 13:18:31.000000 meerschaum-1.6.9/meerschaum/api/dash/pages/dashboard.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      598 2022-07-26 06:45:25.000000 meerschaum-1.6.9/meerschaum/api/dash/pages/error.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4601 2022-07-26 06:45:25.000000 meerschaum-1.6.9/meerschaum/api/dash/pages/login.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1425 2022-07-26 06:45:25.000000 meerschaum-1.6.9/meerschaum/api/dash/pages/plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2398 2022-07-26 06:45:25.000000 meerschaum-1.6.9/meerschaum/api/dash/pages/register.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    15039 2022-10-31 14:15:34.000000 meerschaum-1.6.9/meerschaum/api/dash/pipes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3054 2022-07-26 06:45:25.000000 meerschaum-1.6.9/meerschaum/api/dash/plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      504 2022-07-26 06:45:25.000000 meerschaum-1.6.9/meerschaum/api/dash/sync.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      886 2022-07-26 06:45:25.000000 meerschaum-1.6.9/meerschaum/api/dash/users.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      924 2022-10-31 13:18:31.000000 meerschaum-1.6.9/meerschaum/api/dash/websockets.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.900779 meerschaum-1.6.9/meerschaum/api/models/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      276 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/api/models/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      263 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/api/models/_interfaces.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      304 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/api/models/_locations.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      295 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/api/models/_metrics.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      463 2021-11-20 21:54:59.000000 meerschaum-1.6.9/meerschaum/api/models/_pipes.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.900779 meerschaum-1.6.9/meerschaum/api/resources/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      115 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/api/resources/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.900779 meerschaum-1.6.9/meerschaum/api/resources/static/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/api/resources/static/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.901779 meerschaum-1.6.9/meerschaum/api/resources/static/css/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/api/resources/static/css/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)   180286 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/api/resources/static/css/bootstrap.min.css
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1592 2022-10-31 13:18:31.000000 meerschaum-1.6.9/meerschaum/api/resources/static/css/dash.css
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6087 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/api/resources/static/css/dbc_dark.css
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)       81 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/api/resources/static/css/styles.css
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.901779 meerschaum-1.6.9/meerschaum/api/resources/static/ico/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/api/resources/static/ico/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9662 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/api/resources/static/ico/logo.ico
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.901779 meerschaum-1.6.9/meerschaum/api/resources/static/js/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/api/resources/static/js/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      540 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/api/resources/static/js/action_button.js
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/api/resources/static/js/main.js
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.901779 meerschaum-1.6.9/meerschaum/api/resources/static/png/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/api/resources/static/png/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.901779 meerschaum-1.6.9/meerschaum/api/resources/templates/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/api/resources/templates/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1019 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/api/resources/templates/index.html
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1711 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/api/resources/templates/old_index.html
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      141 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/api/resources/templates/secret.html
--rwxr-xr-x   0 bmeares   (1000) bmeares   (1000)     2082 2021-12-09 07:32:03.000000 meerschaum-1.6.9/meerschaum/api/resources/templates/termpage.html
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.903779 meerschaum-1.6.9/meerschaum/api/routes/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      734 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/api/routes/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2240 2022-06-27 01:07:31.000000 meerschaum-1.6.9/meerschaum/api/routes/_actions.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1803 2022-06-27 01:07:31.000000 meerschaum-1.6.9/meerschaum/api/routes/_connectors.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      578 2022-02-28 20:55:01.000000 meerschaum-1.6.9/meerschaum/api/routes/_index.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1882 2023-01-09 09:23:24.000000 meerschaum-1.6.9/meerschaum/api/routes/_login.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1702 2023-01-09 09:23:24.000000 meerschaum-1.6.9/meerschaum/api/routes/_misc.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    21169 2023-01-21 08:00:50.000000 meerschaum-1.6.9/meerschaum/api/routes/_pipes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6152 2023-01-09 09:23:24.000000 meerschaum-1.6.9/meerschaum/api/routes/_plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7239 2023-01-09 09:23:24.000000 meerschaum-1.6.9/meerschaum/api/routes/_users.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      825 2022-06-27 01:07:31.000000 meerschaum-1.6.9/meerschaum/api/routes/_version.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.903779 meerschaum-1.6.9/meerschaum/api/tables/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      615 2022-02-28 20:55:01.000000 meerschaum-1.6.9/meerschaum/api/tables/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.904779 meerschaum-1.6.9/meerschaum/config/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11629 2023-01-11 04:28:52.000000 meerschaum-1.6.9/meerschaum/config/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5135 2023-05-05 04:35:54.000000 meerschaum-1.6.9/meerschaum/config/_default.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8807 2022-07-13 02:48:16.000000 meerschaum-1.6.9/meerschaum/config/_edit.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4507 2022-10-22 07:29:33.000000 meerschaum-1.6.9/meerschaum/config/_environment.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5556 2022-05-02 19:58:56.000000 meerschaum-1.6.9/meerschaum/config/_formatting.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      647 2023-01-09 09:23:24.000000 meerschaum-1.6.9/meerschaum/config/_jobs.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1508 2023-01-11 05:57:34.000000 meerschaum-1.6.9/meerschaum/config/_patch.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6648 2023-01-09 09:23:24.000000 meerschaum-1.6.9/meerschaum/config/_paths.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1220 2022-02-28 20:55:01.000000 meerschaum-1.6.9/meerschaum/config/_preprocess.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    14567 2022-10-14 04:34:51.000000 meerschaum-1.6.9/meerschaum/config/_read_config.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3589 2021-11-21 05:32:46.000000 meerschaum-1.6.9/meerschaum/config/_shell.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4968 2022-02-28 20:55:01.000000 meerschaum-1.6.9/meerschaum/config/_sync.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)       71 2023-05-12 17:42:26.000000 meerschaum-1.6.9/meerschaum/config/_version.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.904779 meerschaum-1.6.9/meerschaum/config/resources/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/config/resources/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.904779 meerschaum-1.6.9/meerschaum/config/stack/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8233 2023-01-09 09:23:24.000000 meerschaum-1.6.9/meerschaum/config/stack/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.904779 meerschaum-1.6.9/meerschaum/config/stack/grafana/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2010 2022-11-01 03:52:40.000000 meerschaum-1.6.9/meerschaum/config/stack/grafana/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.904779 meerschaum-1.6.9/meerschaum/config/stack/mosquitto/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      186 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/config/stack/mosquitto/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.904779 meerschaum-1.6.9/meerschaum/config/stack/mosquitto/resources/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/config/stack/mosquitto/resources/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.905779 meerschaum-1.6.9/meerschaum/config/stack/resources/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/config/stack/resources/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.905779 meerschaum-1.6.9/meerschaum/config/static/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3679 2023-04-25 23:57:31.000000 meerschaum-1.6.9/meerschaum/config/static/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.905779 meerschaum-1.6.9/meerschaum/connectors/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6381 2023-04-25 23:57:31.000000 meerschaum-1.6.9/meerschaum/connectors/Connector.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12064 2023-04-25 23:57:31.000000 meerschaum-1.6.9/meerschaum/connectors/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.906779 meerschaum-1.6.9/meerschaum/connectors/api/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4022 2023-04-25 23:57:31.000000 meerschaum-1.6.9/meerschaum/connectors/api/APIConnector.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      205 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/connectors/api/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2759 2022-10-22 06:21:34.000000 meerschaum-1.6.9/meerschaum/connectors/api/_actions.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      945 2022-12-05 04:26:42.000000 meerschaum-1.6.9/meerschaum/connectors/api/_delete.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2056 2022-11-01 03:12:07.000000 meerschaum-1.6.9/meerschaum/connectors/api/_fetch.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1572 2022-12-05 04:26:42.000000 meerschaum-1.6.9/meerschaum/connectors/api/_get.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2054 2022-11-18 03:44:05.000000 meerschaum-1.6.9/meerschaum/connectors/api/_login.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1185 2022-06-27 01:07:31.000000 meerschaum-1.6.9/meerschaum/connectors/api/_misc.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      933 2022-12-05 04:26:42.000000 meerschaum-1.6.9/meerschaum/connectors/api/_patch.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    19986 2023-04-26 08:12:59.000000 meerschaum-1.6.9/meerschaum/connectors/api/_pipes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5227 2022-06-27 01:07:31.000000 meerschaum-1.6.9/meerschaum/connectors/api/_plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      922 2022-12-05 04:26:42.000000 meerschaum-1.6.9/meerschaum/connectors/api/_post.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1489 2022-07-25 06:37:48.000000 meerschaum-1.6.9/meerschaum/connectors/api/_uri.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5303 2022-08-19 04:59:44.000000 meerschaum-1.6.9/meerschaum/connectors/api/_users.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4048 2022-10-18 06:13:35.000000 meerschaum-1.6.9/meerschaum/connectors/parse.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.907779 meerschaum-1.6.9/meerschaum/connectors/plugin/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2084 2022-10-25 06:38:00.000000 meerschaum-1.6.9/meerschaum/connectors/plugin/PluginConnector.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      198 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/connectors/plugin/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7215 2023-04-25 23:57:31.000000 meerschaum-1.6.9/meerschaum/connectors/poll.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.908779 meerschaum-1.6.9/meerschaum/connectors/sql/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8592 2023-04-25 23:57:31.000000 meerschaum-1.6.9/meerschaum/connectors/sql/SQLConnector.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      175 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/connectors/sql/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3495 2023-04-25 23:57:31.000000 meerschaum-1.6.9/meerschaum/connectors/sql/_cli.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10197 2023-04-25 23:57:31.000000 meerschaum-1.6.9/meerschaum/connectors/sql/_create_engine.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12650 2023-05-12 06:36:07.000000 meerschaum-1.6.9/meerschaum/connectors/sql/_fetch.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    88433 2023-05-09 02:50:23.000000 meerschaum-1.6.9/meerschaum/connectors/sql/_pipes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7921 2023-04-25 23:57:31.000000 meerschaum-1.6.9/meerschaum/connectors/sql/_plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    26869 2023-05-12 06:36:07.000000 meerschaum-1.6.9/meerschaum/connectors/sql/_sql.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3312 2022-10-18 01:38:49.000000 meerschaum-1.6.9/meerschaum/connectors/sql/_uri.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9972 2023-04-25 23:57:31.000000 meerschaum-1.6.9/meerschaum/connectors/sql/_users.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.908779 meerschaum-1.6.9/meerschaum/connectors/sql/tables/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6482 2023-04-25 23:57:31.000000 meerschaum-1.6.9/meerschaum/connectors/sql/tables/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1573 2022-02-28 20:55:01.000000 meerschaum-1.6.9/meerschaum/connectors/sql/tables/types.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      187 2022-04-24 10:29:36.000000 meerschaum-1.6.9/meerschaum/connectors/sql/tools.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.908779 meerschaum-1.6.9/meerschaum/core/
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.909779 meerschaum-1.6.9/meerschaum/core/Pipe/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    15032 2023-05-12 06:36:07.000000 meerschaum-1.6.9/meerschaum/core/Pipe/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13202 2023-04-26 08:12:59.000000 meerschaum-1.6.9/meerschaum/core/Pipe/_attributes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7613 2023-04-25 23:57:31.000000 meerschaum-1.6.9/meerschaum/core/Pipe/_bootstrap.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2112 2022-11-13 04:57:20.000000 meerschaum-1.6.9/meerschaum/core/Pipe/_clear.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10716 2023-05-12 06:36:07.000000 meerschaum-1.6.9/meerschaum/core/Pipe/_data.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1854 2022-12-05 04:26:42.000000 meerschaum-1.6.9/meerschaum/core/Pipe/_delete.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1052 2023-04-25 23:57:31.000000 meerschaum-1.6.9/meerschaum/core/Pipe/_drop.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3146 2023-05-08 21:38:02.000000 meerschaum-1.6.9/meerschaum/core/Pipe/_dtypes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8471 2022-12-05 04:26:42.000000 meerschaum-1.6.9/meerschaum/core/Pipe/_edit.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3005 2023-05-12 17:42:26.000000 meerschaum-1.6.9/meerschaum/core/Pipe/_fetch.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2240 2023-01-16 21:21:28.000000 meerschaum-1.6.9/meerschaum/core/Pipe/_register.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1352 2023-04-25 23:57:31.000000 meerschaum-1.6.9/meerschaum/core/Pipe/_show.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    25706 2023-05-12 06:36:07.000000 meerschaum-1.6.9/meerschaum/core/Pipe/_sync.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.909779 meerschaum-1.6.9/meerschaum/core/Plugin/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      137 2022-04-24 10:29:36.000000 meerschaum-1.6.9/meerschaum/core/Plugin/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.910779 meerschaum-1.6.9/meerschaum/core/User/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2362 2022-04-24 10:29:36.000000 meerschaum-1.6.9/meerschaum/core/User/_User.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      161 2022-04-24 10:29:36.000000 meerschaum-1.6.9/meerschaum/core/User/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      251 2022-04-24 10:29:36.000000 meerschaum-1.6.9/meerschaum/core/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.910779 meerschaum-1.6.9/meerschaum/plugins/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    33813 2023-01-21 08:00:50.000000 meerschaum-1.6.9/meerschaum/plugins/_Plugin.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    18398 2023-04-25 23:57:31.000000 meerschaum-1.6.9/meerschaum/plugins/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.912779 meerschaum-1.6.9/meerschaum/utils/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      444 2021-11-08 16:07:48.000000 meerschaum-1.6.9/meerschaum/utils/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.912779 meerschaum-1.6.9/meerschaum/utils/daemon/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    24801 2023-04-25 23:57:31.000000 meerschaum-1.6.9/meerschaum/utils/daemon/Daemon.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3170 2023-01-09 03:01:33.000000 meerschaum-1.6.9/meerschaum/utils/daemon/Log.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5355 2023-01-09 09:50:51.000000 meerschaum-1.6.9/meerschaum/utils/daemon/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4302 2022-02-28 20:55:01.000000 meerschaum-1.6.9/meerschaum/utils/daemon/_names.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3690 2023-01-09 09:23:24.000000 meerschaum-1.6.9/meerschaum/utils/debug.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.912779 meerschaum-1.6.9/meerschaum/utils/formatting/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9387 2023-01-09 09:23:24.000000 meerschaum-1.6.9/meerschaum/utils/formatting/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2939 2022-02-28 20:55:01.000000 meerschaum-1.6.9/meerschaum/utils/formatting/_jobs.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12729 2022-10-25 06:38:00.000000 meerschaum-1.6.9/meerschaum/utils/formatting/_pipes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3032 2022-10-18 06:13:35.000000 meerschaum-1.6.9/meerschaum/utils/formatting/_pprint.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3844 2023-01-09 09:23:24.000000 meerschaum-1.6.9/meerschaum/utils/formatting/_shell.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11791 2022-12-05 04:26:42.000000 meerschaum-1.6.9/meerschaum/utils/get_pipes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3419 2022-10-18 06:13:35.000000 meerschaum-1.6.9/meerschaum/utils/interactive.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    61453 2023-05-08 21:38:02.000000 meerschaum-1.6.9/meerschaum/utils/misc.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1006 2022-02-28 20:55:01.000000 meerschaum-1.6.9/meerschaum/utils/networking.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.913779 meerschaum-1.6.9/meerschaum/utils/packages/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    53718 2023-05-08 21:38:02.000000 meerschaum-1.6.9/meerschaum/utils/packages/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8054 2023-05-12 17:39:43.000000 meerschaum-1.6.9/meerschaum/utils/packages/_packages.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2540 2022-07-25 06:37:48.000000 meerschaum-1.6.9/meerschaum/utils/packages/lazy_loader.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2781 2022-08-23 06:14:42.000000 meerschaum-1.6.9/meerschaum/utils/pool.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7098 2023-04-25 23:57:31.000000 meerschaum-1.6.9/meerschaum/utils/process.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    16060 2022-05-02 19:58:56.000000 meerschaum-1.6.9/meerschaum/utils/prompt.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1635 2022-08-29 21:54:10.000000 meerschaum-1.6.9/meerschaum/utils/schedule.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    34702 2023-05-12 06:36:07.000000 meerschaum-1.6.9/meerschaum/utils/sql.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2152 2022-10-25 06:38:00.000000 meerschaum-1.6.9/meerschaum/utils/threading.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2517 2023-05-05 21:42:47.000000 meerschaum-1.6.9/meerschaum/utils/typing.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.913779 meerschaum-1.6.9/meerschaum/utils/venv/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3479 2022-10-25 06:38:00.000000 meerschaum-1.6.9/meerschaum/utils/venv/_Venv.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    22150 2023-04-26 08:12:59.000000 meerschaum-1.6.9/meerschaum/utils/venv/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6610 2023-04-25 23:57:31.000000 meerschaum-1.6.9/meerschaum/utils/warnings.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3162 2023-01-09 09:23:24.000000 meerschaum-1.6.9/meerschaum/utils/yaml.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 17:43:14.891779 meerschaum-1.6.9/meerschaum.egg-info/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10798 2023-05-12 17:43:14.000000 meerschaum-1.6.9/meerschaum.egg-info/PKG-INFO
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7834 2023-05-12 17:43:14.000000 meerschaum-1.6.9/meerschaum.egg-info/SOURCES.txt
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        1 2023-05-12 17:43:14.000000 meerschaum-1.6.9/meerschaum.egg-info/dependency_links.txt
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)       88 2023-05-12 17:43:14.000000 meerschaum-1.6.9/meerschaum.egg-info/entry_points.txt
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4703 2023-05-12 17:43:14.000000 meerschaum-1.6.9/meerschaum.egg-info/requires.txt
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)       11 2023-05-12 17:43:14.000000 meerschaum-1.6.9/meerschaum.egg-info/top_level.txt
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        1 2023-05-12 17:43:14.000000 meerschaum-1.6.9/meerschaum.egg-info/zip-safe
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)       38 2023-05-12 17:43:14.914779 meerschaum-1.6.9/setup.cfg
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3056 2023-05-12 17:39:43.000000 meerschaum-1.6.9/setup.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 04:46:20.839579 meerschaum-1.7.0.dev1/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11359 2021-12-27 13:50:47.000000 meerschaum-1.7.0.dev1/LICENSE
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      114 2021-12-27 13:50:47.000000 meerschaum-1.7.0.dev1/NOTICE
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10803 2023-08-04 04:46:20.839579 meerschaum-1.7.0.dev1/PKG-INFO
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9248 2022-07-13 02:48:08.000000 meerschaum-1.7.0.dev1/README.md
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 04:46:20.827579 meerschaum-1.7.0.dev1/meerschaum/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1236 2023-04-25 23:57:31.000000 meerschaum-1.7.0.dev1/meerschaum/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2774 2022-10-22 06:28:47.000000 meerschaum-1.7.0.dev1/meerschaum/__main__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 04:46:20.827579 meerschaum-1.7.0.dev1/meerschaum/_internal/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      169 2022-04-23 01:15:00.000000 meerschaum-1.7.0.dev1/meerschaum/_internal/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 04:46:20.828579 meerschaum-1.7.0.dev1/meerschaum/_internal/arguments/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      519 2022-10-22 06:25:53.000000 meerschaum-1.7.0.dev1/meerschaum/_internal/arguments/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9741 2023-04-25 23:57:31.000000 meerschaum-1.7.0.dev1/meerschaum/_internal/arguments/_parse_arguments.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12641 2023-08-04 03:08:50.000000 meerschaum-1.7.0.dev1/meerschaum/_internal/arguments/_parser.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 04:46:20.828579 meerschaum-1.7.0.dev1/meerschaum/_internal/docs/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      126 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev1/meerschaum/_internal/docs/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7719 2022-04-24 10:29:36.000000 meerschaum-1.7.0.dev1/meerschaum/_internal/docs/index.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4625 2023-04-25 23:57:31.000000 meerschaum-1.7.0.dev1/meerschaum/_internal/entry.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 04:46:20.828579 meerschaum-1.7.0.dev1/meerschaum/_internal/gui/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1332 2022-04-24 10:29:36.000000 meerschaum-1.7.0.dev1/meerschaum/_internal/gui/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 04:46:20.828579 meerschaum-1.7.0.dev1/meerschaum/_internal/gui/app/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1565 2022-04-24 10:29:36.000000 meerschaum-1.7.0.dev1/meerschaum/_internal/gui/app/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2632 2022-10-18 06:13:35.000000 meerschaum-1.7.0.dev1/meerschaum/_internal/gui/app/_windows.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1016 2022-04-24 10:29:36.000000 meerschaum-1.7.0.dev1/meerschaum/_internal/gui/app/actions.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1678 2022-04-24 10:29:36.000000 meerschaum-1.7.0.dev1/meerschaum/_internal/gui/app/pipes.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 04:46:20.828579 meerschaum-1.7.0.dev1/meerschaum/_internal/shell/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    31489 2023-01-09 09:23:24.000000 meerschaum-1.7.0.dev1/meerschaum/_internal/shell/Shell.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2981 2022-10-22 06:28:01.000000 meerschaum-1.7.0.dev1/meerschaum/_internal/shell/ShellCompleter.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1280 2022-10-26 04:20:20.000000 meerschaum-1.7.0.dev1/meerschaum/_internal/shell/ValidAutoSuggest.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      281 2022-04-24 10:29:36.000000 meerschaum-1.7.0.dev1/meerschaum/_internal/shell/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 04:46:20.828579 meerschaum-1.7.0.dev1/meerschaum/_internal/shell/resources/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2022-04-24 10:29:36.000000 meerschaum-1.7.0.dev1/meerschaum/_internal/shell/resources/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 04:46:20.828579 meerschaum-1.7.0.dev1/meerschaum/_internal/term/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      612 2021-12-09 07:32:03.000000 meerschaum-1.7.0.dev1/meerschaum/_internal/term/TermPageHandler.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1495 2021-12-09 07:32:03.000000 meerschaum-1.7.0.dev1/meerschaum/_internal/term/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      716 2023-08-04 03:39:01.000000 meerschaum-1.7.0.dev1/meerschaum/_internal/term/tools.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 04:46:20.830579 meerschaum-1.7.0.dev1/meerschaum/actions/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8023 2023-07-22 12:38:11.000000 meerschaum-1.7.0.dev1/meerschaum/actions/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11815 2023-08-04 03:19:08.000000 meerschaum-1.7.0.dev1/meerschaum/actions/api.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    14529 2023-04-25 23:57:31.000000 meerschaum-1.7.0.dev1/meerschaum/actions/bootstrap.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4857 2022-08-23 06:14:42.000000 meerschaum-1.7.0.dev1/meerschaum/actions/clear.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6259 2023-06-28 23:16:36.000000 meerschaum-1.7.0.dev1/meerschaum/actions/copy.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    15245 2023-01-09 09:23:24.000000 meerschaum-1.7.0.dev1/meerschaum/actions/delete.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2701 2022-06-27 01:07:31.000000 meerschaum-1.7.0.dev1/meerschaum/actions/drop.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9492 2023-04-25 23:57:31.000000 meerschaum-1.7.0.dev1/meerschaum/actions/edit.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7380 2022-10-18 06:13:35.000000 meerschaum-1.7.0.dev1/meerschaum/actions/install.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4206 2022-02-28 20:55:01.000000 meerschaum-1.7.0.dev1/meerschaum/actions/login.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2251 2022-08-29 21:54:10.000000 meerschaum-1.7.0.dev1/meerschaum/actions/os.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2395 2022-02-28 20:55:01.000000 meerschaum-1.7.0.dev1/meerschaum/actions/python.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11219 2023-04-25 23:57:31.000000 meerschaum-1.7.0.dev1/meerschaum/actions/register.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      605 2022-02-28 20:55:01.000000 meerschaum-1.7.0.dev1/meerschaum/actions/reload.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3211 2023-01-09 09:23:24.000000 meerschaum-1.7.0.dev1/meerschaum/actions/setup.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2026 2022-08-29 21:54:10.000000 meerschaum-1.7.0.dev1/meerschaum/actions/sh.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    23468 2023-01-11 06:27:06.000000 meerschaum-1.7.0.dev1/meerschaum/actions/show.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4224 2022-02-28 20:55:01.000000 meerschaum-1.7.0.dev1/meerschaum/actions/sql.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5807 2023-06-28 23:16:36.000000 meerschaum-1.7.0.dev1/meerschaum/actions/stack.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    18247 2022-11-22 01:55:36.000000 meerschaum-1.7.0.dev1/meerschaum/actions/start.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3948 2023-01-16 21:21:28.000000 meerschaum-1.7.0.dev1/meerschaum/actions/stop.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    15339 2022-12-15 02:09:06.000000 meerschaum-1.7.0.dev1/meerschaum/actions/sync.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6073 2022-08-19 04:59:44.000000 meerschaum-1.7.0.dev1/meerschaum/actions/uninstall.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6307 2022-08-19 04:59:44.000000 meerschaum-1.7.0.dev1/meerschaum/actions/upgrade.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3348 2022-10-26 04:20:20.000000 meerschaum-1.7.0.dev1/meerschaum/actions/verify.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 04:46:20.830579 meerschaum-1.7.0.dev1/meerschaum/api/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7704 2023-08-04 03:03:40.000000 meerschaum-1.7.0.dev1/meerschaum/api/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      875 2022-02-28 20:55:01.000000 meerschaum-1.7.0.dev1/meerschaum/api/_chain.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1755 2023-08-04 04:30:57.000000 meerschaum-1.7.0.dev1/meerschaum/api/_events.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      961 2023-07-13 02:20:19.000000 meerschaum-1.7.0.dev1/meerschaum/api/_oauth2.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1226 2022-11-05 03:38:45.000000 meerschaum-1.7.0.dev1/meerschaum/api/_websockets.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 04:46:20.831579 meerschaum-1.7.0.dev1/meerschaum/api/dash/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2238 2023-01-09 08:57:26.000000 meerschaum-1.7.0.dev1/meerschaum/api/dash/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9600 2022-10-31 13:18:31.000000 meerschaum-1.7.0.dev1/meerschaum/api/dash/actions.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 04:46:20.831579 meerschaum-1.7.0.dev1/meerschaum/api/dash/assets/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev1/meerschaum/api/dash/assets/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    21923 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev1/meerschaum/api/dash/assets/ansi_up.js
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)   338636 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev1/meerschaum/api/dash/assets/banner_1920x320.png
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9662 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev1/meerschaum/api/dash/assets/favicon.ico
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10218 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev1/meerschaum/api/dash/assets/logo_48x48.png
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    67702 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev1/meerschaum/api/dash/assets/logo_500x500.png
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 04:46:20.831579 meerschaum-1.7.0.dev1/meerschaum/api/dash/callbacks/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      283 2023-07-21 01:07:26.000000 meerschaum-1.7.0.dev1/meerschaum/api/dash/callbacks/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    25190 2023-08-04 02:45:31.000000 meerschaum-1.7.0.dev1/meerschaum/api/dash/callbacks/dashboard.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2529 2023-01-09 09:04:18.000000 meerschaum-1.7.0.dev1/meerschaum/api/dash/callbacks/login.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2777 2022-07-26 06:45:25.000000 meerschaum-1.7.0.dev1/meerschaum/api/dash/callbacks/plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3446 2023-04-25 23:57:31.000000 meerschaum-1.7.0.dev1/meerschaum/api/dash/callbacks/register.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6373 2023-08-04 04:42:39.000000 meerschaum-1.7.0.dev1/meerschaum/api/dash/components.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      843 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev1/meerschaum/api/dash/connectors.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2046 2023-08-04 04:44:53.000000 meerschaum-1.7.0.dev1/meerschaum/api/dash/graphs.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3544 2022-07-26 06:45:25.000000 meerschaum-1.7.0.dev1/meerschaum/api/dash/jobs.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13682 2022-10-31 13:18:31.000000 meerschaum-1.7.0.dev1/meerschaum/api/dash/keys.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 04:46:20.832579 meerschaum-1.7.0.dev1/meerschaum/api/dash/pages/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      273 2023-07-21 01:07:38.000000 meerschaum-1.7.0.dev1/meerschaum/api/dash/pages/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3838 2022-10-31 13:18:31.000000 meerschaum-1.7.0.dev1/meerschaum/api/dash/pages/dashboard.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      598 2022-07-26 06:45:25.000000 meerschaum-1.7.0.dev1/meerschaum/api/dash/pages/error.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4601 2022-07-26 06:45:25.000000 meerschaum-1.7.0.dev1/meerschaum/api/dash/pages/login.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1382 2023-07-22 12:38:11.000000 meerschaum-1.7.0.dev1/meerschaum/api/dash/pages/plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2398 2022-07-26 06:45:25.000000 meerschaum-1.7.0.dev1/meerschaum/api/dash/pages/register.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    15039 2022-10-31 14:15:34.000000 meerschaum-1.7.0.dev1/meerschaum/api/dash/pipes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3054 2022-07-26 06:45:25.000000 meerschaum-1.7.0.dev1/meerschaum/api/dash/plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      504 2022-07-26 06:45:25.000000 meerschaum-1.7.0.dev1/meerschaum/api/dash/sync.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      895 2023-08-04 02:41:30.000000 meerschaum-1.7.0.dev1/meerschaum/api/dash/users.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      924 2022-10-31 13:18:31.000000 meerschaum-1.7.0.dev1/meerschaum/api/dash/websockets.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1659 2023-08-04 04:24:47.000000 meerschaum-1.7.0.dev1/meerschaum/api/dash/webterm.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 04:46:20.832579 meerschaum-1.7.0.dev1/meerschaum/api/models/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      276 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev1/meerschaum/api/models/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      263 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev1/meerschaum/api/models/_interfaces.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      304 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev1/meerschaum/api/models/_locations.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      295 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev1/meerschaum/api/models/_metrics.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      463 2021-11-20 21:54:59.000000 meerschaum-1.7.0.dev1/meerschaum/api/models/_pipes.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 04:46:20.832579 meerschaum-1.7.0.dev1/meerschaum/api/resources/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      115 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev1/meerschaum/api/resources/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 04:46:20.832579 meerschaum-1.7.0.dev1/meerschaum/api/resources/static/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev1/meerschaum/api/resources/static/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 04:46:20.832579 meerschaum-1.7.0.dev1/meerschaum/api/resources/static/css/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev1/meerschaum/api/resources/static/css/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)   180286 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev1/meerschaum/api/resources/static/css/bootstrap.min.css
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1674 2023-08-04 03:00:27.000000 meerschaum-1.7.0.dev1/meerschaum/api/resources/static/css/dash.css
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6087 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev1/meerschaum/api/resources/static/css/dbc_dark.css
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)       81 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev1/meerschaum/api/resources/static/css/styles.css
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 04:46:20.832579 meerschaum-1.7.0.dev1/meerschaum/api/resources/static/ico/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev1/meerschaum/api/resources/static/ico/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9662 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev1/meerschaum/api/resources/static/ico/logo.ico
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 04:46:20.833579 meerschaum-1.7.0.dev1/meerschaum/api/resources/static/js/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev1/meerschaum/api/resources/static/js/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      540 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev1/meerschaum/api/resources/static/js/action_button.js
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev1/meerschaum/api/resources/static/js/main.js
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 04:46:20.833579 meerschaum-1.7.0.dev1/meerschaum/api/resources/static/png/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev1/meerschaum/api/resources/static/png/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 04:46:20.833579 meerschaum-1.7.0.dev1/meerschaum/api/resources/templates/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev1/meerschaum/api/resources/templates/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1019 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev1/meerschaum/api/resources/templates/index.html
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1711 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev1/meerschaum/api/resources/templates/old_index.html
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      141 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev1/meerschaum/api/resources/templates/secret.html
+-rwxr-xr-x   0 bmeares   (1000) bmeares   (1000)     2082 2021-12-09 07:32:03.000000 meerschaum-1.7.0.dev1/meerschaum/api/resources/templates/termpage.html
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 04:46:20.833579 meerschaum-1.7.0.dev1/meerschaum/api/routes/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      734 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev1/meerschaum/api/routes/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2240 2022-06-27 01:07:31.000000 meerschaum-1.7.0.dev1/meerschaum/api/routes/_actions.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1803 2022-06-27 01:07:31.000000 meerschaum-1.7.0.dev1/meerschaum/api/routes/_connectors.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      578 2022-02-28 20:55:01.000000 meerschaum-1.7.0.dev1/meerschaum/api/routes/_index.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1882 2023-01-09 09:23:24.000000 meerschaum-1.7.0.dev1/meerschaum/api/routes/_login.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1714 2023-07-14 22:01:00.000000 meerschaum-1.7.0.dev1/meerschaum/api/routes/_misc.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    21169 2023-01-21 08:00:50.000000 meerschaum-1.7.0.dev1/meerschaum/api/routes/_pipes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6152 2023-01-09 09:23:24.000000 meerschaum-1.7.0.dev1/meerschaum/api/routes/_plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7204 2023-07-14 20:54:29.000000 meerschaum-1.7.0.dev1/meerschaum/api/routes/_users.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      825 2022-06-27 01:07:31.000000 meerschaum-1.7.0.dev1/meerschaum/api/routes/_version.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 04:46:20.833579 meerschaum-1.7.0.dev1/meerschaum/api/tables/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      615 2022-02-28 20:55:01.000000 meerschaum-1.7.0.dev1/meerschaum/api/tables/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 04:46:20.834579 meerschaum-1.7.0.dev1/meerschaum/config/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11629 2023-01-11 04:28:52.000000 meerschaum-1.7.0.dev1/meerschaum/config/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5135 2023-05-05 04:35:54.000000 meerschaum-1.7.0.dev1/meerschaum/config/_default.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8807 2022-07-13 02:48:16.000000 meerschaum-1.7.0.dev1/meerschaum/config/_edit.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4507 2022-10-22 07:29:33.000000 meerschaum-1.7.0.dev1/meerschaum/config/_environment.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5556 2022-05-02 19:58:56.000000 meerschaum-1.7.0.dev1/meerschaum/config/_formatting.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      647 2023-01-09 09:23:24.000000 meerschaum-1.7.0.dev1/meerschaum/config/_jobs.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1508 2023-01-11 05:57:34.000000 meerschaum-1.7.0.dev1/meerschaum/config/_patch.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6648 2023-01-09 09:23:24.000000 meerschaum-1.7.0.dev1/meerschaum/config/_paths.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1220 2022-02-28 20:55:01.000000 meerschaum-1.7.0.dev1/meerschaum/config/_preprocess.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    14567 2022-10-14 04:34:51.000000 meerschaum-1.7.0.dev1/meerschaum/config/_read_config.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3589 2021-11-21 05:32:46.000000 meerschaum-1.7.0.dev1/meerschaum/config/_shell.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4968 2022-02-28 20:55:01.000000 meerschaum-1.7.0.dev1/meerschaum/config/_sync.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)       76 2023-08-04 04:38:23.000000 meerschaum-1.7.0.dev1/meerschaum/config/_version.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 04:46:20.834579 meerschaum-1.7.0.dev1/meerschaum/config/resources/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev1/meerschaum/config/resources/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 04:46:20.834579 meerschaum-1.7.0.dev1/meerschaum/config/stack/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8616 2023-06-28 23:16:36.000000 meerschaum-1.7.0.dev1/meerschaum/config/stack/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 04:46:20.834579 meerschaum-1.7.0.dev1/meerschaum/config/stack/grafana/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2010 2022-11-01 03:52:40.000000 meerschaum-1.7.0.dev1/meerschaum/config/stack/grafana/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 04:46:20.834579 meerschaum-1.7.0.dev1/meerschaum/config/stack/mosquitto/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      186 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev1/meerschaum/config/stack/mosquitto/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 04:46:20.834579 meerschaum-1.7.0.dev1/meerschaum/config/stack/mosquitto/resources/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev1/meerschaum/config/stack/mosquitto/resources/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 04:46:20.834579 meerschaum-1.7.0.dev1/meerschaum/config/stack/resources/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev1/meerschaum/config/stack/resources/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 04:46:20.834579 meerschaum-1.7.0.dev1/meerschaum/config/static/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3719 2023-08-04 04:10:20.000000 meerschaum-1.7.0.dev1/meerschaum/config/static/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 04:46:20.835579 meerschaum-1.7.0.dev1/meerschaum/connectors/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6381 2023-04-25 23:57:31.000000 meerschaum-1.7.0.dev1/meerschaum/connectors/Connector.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12064 2023-04-25 23:57:31.000000 meerschaum-1.7.0.dev1/meerschaum/connectors/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 04:46:20.835579 meerschaum-1.7.0.dev1/meerschaum/connectors/api/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4055 2023-05-14 14:48:27.000000 meerschaum-1.7.0.dev1/meerschaum/connectors/api/APIConnector.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      205 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev1/meerschaum/connectors/api/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2759 2022-10-22 06:21:34.000000 meerschaum-1.7.0.dev1/meerschaum/connectors/api/_actions.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      945 2022-12-05 04:26:42.000000 meerschaum-1.7.0.dev1/meerschaum/connectors/api/_delete.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2056 2022-11-01 03:12:07.000000 meerschaum-1.7.0.dev1/meerschaum/connectors/api/_fetch.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1572 2022-12-05 04:26:42.000000 meerschaum-1.7.0.dev1/meerschaum/connectors/api/_get.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2054 2022-11-18 03:44:05.000000 meerschaum-1.7.0.dev1/meerschaum/connectors/api/_login.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1185 2022-06-27 01:07:31.000000 meerschaum-1.7.0.dev1/meerschaum/connectors/api/_misc.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      933 2022-12-05 04:26:42.000000 meerschaum-1.7.0.dev1/meerschaum/connectors/api/_patch.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    19986 2023-04-26 08:12:59.000000 meerschaum-1.7.0.dev1/meerschaum/connectors/api/_pipes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5227 2022-06-27 01:07:31.000000 meerschaum-1.7.0.dev1/meerschaum/connectors/api/_plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      922 2022-12-05 04:26:42.000000 meerschaum-1.7.0.dev1/meerschaum/connectors/api/_post.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1489 2022-07-25 06:37:48.000000 meerschaum-1.7.0.dev1/meerschaum/connectors/api/_uri.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5303 2022-08-19 04:59:44.000000 meerschaum-1.7.0.dev1/meerschaum/connectors/api/_users.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4048 2022-10-18 06:13:35.000000 meerschaum-1.7.0.dev1/meerschaum/connectors/parse.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 04:46:20.835579 meerschaum-1.7.0.dev1/meerschaum/connectors/plugin/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2084 2022-10-25 06:38:00.000000 meerschaum-1.7.0.dev1/meerschaum/connectors/plugin/PluginConnector.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      198 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev1/meerschaum/connectors/plugin/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7215 2023-04-25 23:57:31.000000 meerschaum-1.7.0.dev1/meerschaum/connectors/poll.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 04:46:20.836579 meerschaum-1.7.0.dev1/meerschaum/connectors/sql/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9067 2023-07-22 12:38:11.000000 meerschaum-1.7.0.dev1/meerschaum/connectors/sql/SQLConnector.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      175 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev1/meerschaum/connectors/sql/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3495 2023-04-25 23:57:31.000000 meerschaum-1.7.0.dev1/meerschaum/connectors/sql/_cli.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10197 2023-04-25 23:57:31.000000 meerschaum-1.7.0.dev1/meerschaum/connectors/sql/_create_engine.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12669 2023-06-28 23:16:36.000000 meerschaum-1.7.0.dev1/meerschaum/connectors/sql/_fetch.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    86905 2023-07-22 12:38:11.000000 meerschaum-1.7.0.dev1/meerschaum/connectors/sql/_pipes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8126 2023-05-14 14:48:27.000000 meerschaum-1.7.0.dev1/meerschaum/connectors/sql/_plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    26997 2023-07-13 02:20:19.000000 meerschaum-1.7.0.dev1/meerschaum/connectors/sql/_sql.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3312 2022-10-18 01:38:49.000000 meerschaum-1.7.0.dev1/meerschaum/connectors/sql/_uri.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10095 2023-05-14 14:48:27.000000 meerschaum-1.7.0.dev1/meerschaum/connectors/sql/_users.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 04:46:20.836579 meerschaum-1.7.0.dev1/meerschaum/connectors/sql/tables/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6489 2023-05-14 14:48:27.000000 meerschaum-1.7.0.dev1/meerschaum/connectors/sql/tables/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1573 2022-02-28 20:55:01.000000 meerschaum-1.7.0.dev1/meerschaum/connectors/sql/tables/types.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      187 2022-04-24 10:29:36.000000 meerschaum-1.7.0.dev1/meerschaum/connectors/sql/tools.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 04:46:20.836579 meerschaum-1.7.0.dev1/meerschaum/core/
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 04:46:20.837579 meerschaum-1.7.0.dev1/meerschaum/core/Pipe/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    15032 2023-05-14 14:48:27.000000 meerschaum-1.7.0.dev1/meerschaum/core/Pipe/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13202 2023-04-26 08:12:59.000000 meerschaum-1.7.0.dev1/meerschaum/core/Pipe/_attributes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7613 2023-04-25 23:57:31.000000 meerschaum-1.7.0.dev1/meerschaum/core/Pipe/_bootstrap.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2112 2022-11-13 04:57:20.000000 meerschaum-1.7.0.dev1/meerschaum/core/Pipe/_clear.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11702 2023-07-22 12:38:11.000000 meerschaum-1.7.0.dev1/meerschaum/core/Pipe/_data.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1854 2022-12-05 04:26:42.000000 meerschaum-1.7.0.dev1/meerschaum/core/Pipe/_delete.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1052 2023-04-25 23:57:31.000000 meerschaum-1.7.0.dev1/meerschaum/core/Pipe/_drop.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3146 2023-07-13 00:51:30.000000 meerschaum-1.7.0.dev1/meerschaum/core/Pipe/_dtypes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8471 2022-12-05 04:26:42.000000 meerschaum-1.7.0.dev1/meerschaum/core/Pipe/_edit.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3182 2023-05-14 14:48:27.000000 meerschaum-1.7.0.dev1/meerschaum/core/Pipe/_fetch.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2240 2023-01-16 21:21:28.000000 meerschaum-1.7.0.dev1/meerschaum/core/Pipe/_register.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1352 2023-04-25 23:57:31.000000 meerschaum-1.7.0.dev1/meerschaum/core/Pipe/_show.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    26496 2023-07-13 00:51:30.000000 meerschaum-1.7.0.dev1/meerschaum/core/Pipe/_sync.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 04:46:20.837579 meerschaum-1.7.0.dev1/meerschaum/core/Plugin/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      137 2022-04-24 10:29:36.000000 meerschaum-1.7.0.dev1/meerschaum/core/Plugin/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 04:46:20.837579 meerschaum-1.7.0.dev1/meerschaum/core/User/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2362 2022-04-24 10:29:36.000000 meerschaum-1.7.0.dev1/meerschaum/core/User/_User.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      161 2022-04-24 10:29:36.000000 meerschaum-1.7.0.dev1/meerschaum/core/User/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      251 2022-04-24 10:29:36.000000 meerschaum-1.7.0.dev1/meerschaum/core/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 04:46:20.837579 meerschaum-1.7.0.dev1/meerschaum/plugins/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    33813 2023-01-21 08:00:50.000000 meerschaum-1.7.0.dev1/meerschaum/plugins/_Plugin.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    18398 2023-04-25 23:57:31.000000 meerschaum-1.7.0.dev1/meerschaum/plugins/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 04:46:20.838579 meerschaum-1.7.0.dev1/meerschaum/utils/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      444 2021-11-08 16:07:48.000000 meerschaum-1.7.0.dev1/meerschaum/utils/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 04:46:20.838579 meerschaum-1.7.0.dev1/meerschaum/utils/daemon/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    24450 2023-08-04 04:19:36.000000 meerschaum-1.7.0.dev1/meerschaum/utils/daemon/Daemon.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3170 2023-01-09 03:01:33.000000 meerschaum-1.7.0.dev1/meerschaum/utils/daemon/Log.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5355 2023-01-09 09:50:51.000000 meerschaum-1.7.0.dev1/meerschaum/utils/daemon/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4302 2022-02-28 20:55:01.000000 meerschaum-1.7.0.dev1/meerschaum/utils/daemon/_names.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3690 2023-01-09 09:23:24.000000 meerschaum-1.7.0.dev1/meerschaum/utils/debug.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 04:46:20.838579 meerschaum-1.7.0.dev1/meerschaum/utils/formatting/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9387 2023-01-09 09:23:24.000000 meerschaum-1.7.0.dev1/meerschaum/utils/formatting/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2939 2022-02-28 20:55:01.000000 meerschaum-1.7.0.dev1/meerschaum/utils/formatting/_jobs.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12729 2022-10-25 06:38:00.000000 meerschaum-1.7.0.dev1/meerschaum/utils/formatting/_pipes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3032 2022-10-18 06:13:35.000000 meerschaum-1.7.0.dev1/meerschaum/utils/formatting/_pprint.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3844 2023-07-22 12:38:11.000000 meerschaum-1.7.0.dev1/meerschaum/utils/formatting/_shell.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11791 2022-12-05 04:26:42.000000 meerschaum-1.7.0.dev1/meerschaum/utils/get_pipes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3419 2022-10-18 06:13:35.000000 meerschaum-1.7.0.dev1/meerschaum/utils/interactive.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    62176 2023-07-13 00:51:30.000000 meerschaum-1.7.0.dev1/meerschaum/utils/misc.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1006 2022-02-28 20:55:01.000000 meerschaum-1.7.0.dev1/meerschaum/utils/networking.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 04:46:20.838579 meerschaum-1.7.0.dev1/meerschaum/utils/packages/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    53718 2023-07-13 00:51:30.000000 meerschaum-1.7.0.dev1/meerschaum/utils/packages/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7989 2023-07-14 22:02:27.000000 meerschaum-1.7.0.dev1/meerschaum/utils/packages/_packages.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2540 2022-07-25 06:37:48.000000 meerschaum-1.7.0.dev1/meerschaum/utils/packages/lazy_loader.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2781 2022-08-23 06:14:42.000000 meerschaum-1.7.0.dev1/meerschaum/utils/pool.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7098 2023-04-25 23:57:31.000000 meerschaum-1.7.0.dev1/meerschaum/utils/process.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    16060 2022-05-02 19:58:56.000000 meerschaum-1.7.0.dev1/meerschaum/utils/prompt.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1886 2023-07-13 02:20:19.000000 meerschaum-1.7.0.dev1/meerschaum/utils/schedule.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    34702 2023-07-13 00:51:30.000000 meerschaum-1.7.0.dev1/meerschaum/utils/sql.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2152 2022-10-25 06:38:00.000000 meerschaum-1.7.0.dev1/meerschaum/utils/threading.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2535 2023-07-14 20:36:10.000000 meerschaum-1.7.0.dev1/meerschaum/utils/typing.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 04:46:20.838579 meerschaum-1.7.0.dev1/meerschaum/utils/venv/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3479 2022-10-25 06:38:00.000000 meerschaum-1.7.0.dev1/meerschaum/utils/venv/_Venv.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    22150 2023-04-26 08:12:59.000000 meerschaum-1.7.0.dev1/meerschaum/utils/venv/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6535 2023-07-22 12:38:11.000000 meerschaum-1.7.0.dev1/meerschaum/utils/warnings.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3162 2023-01-09 09:23:24.000000 meerschaum-1.7.0.dev1/meerschaum/utils/yaml.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-08-04 04:46:20.827579 meerschaum-1.7.0.dev1/meerschaum.egg-info/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10803 2023-08-04 04:46:20.000000 meerschaum-1.7.0.dev1/meerschaum.egg-info/PKG-INFO
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7865 2023-08-04 04:46:20.000000 meerschaum-1.7.0.dev1/meerschaum.egg-info/SOURCES.txt
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        1 2023-08-04 04:46:20.000000 meerschaum-1.7.0.dev1/meerschaum.egg-info/dependency_links.txt
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)       88 2023-08-04 04:46:20.000000 meerschaum-1.7.0.dev1/meerschaum.egg-info/entry_points.txt
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4657 2023-08-04 04:46:20.000000 meerschaum-1.7.0.dev1/meerschaum.egg-info/requires.txt
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)       11 2023-08-04 04:46:20.000000 meerschaum-1.7.0.dev1/meerschaum.egg-info/top_level.txt
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        1 2023-08-04 04:46:20.000000 meerschaum-1.7.0.dev1/meerschaum.egg-info/zip-safe
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)       38 2023-08-04 04:46:20.839579 meerschaum-1.7.0.dev1/setup.cfg
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3056 2023-07-14 22:02:27.000000 meerschaum-1.7.0.dev1/setup.py
```

### Comparing `meerschaum-1.6.9/LICENSE` & `meerschaum-1.7.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/PKG-INFO` & `meerschaum-1.7.0.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meerschaum
-Version: 1.6.9
+Version: 1.7.0.dev1
 Summary: Sync Time-Series Pipes with Meerschaum
 Home-page: https://meerschaum.io
 Author: Bennett Meares
 Author-email: bennett.meares@gmail.com
 Maintainer-email: bennett.meares@gmail.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://docs.meerschaum.io
```

### Comparing `meerschaum-1.6.9/README.md` & `meerschaum-1.7.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/__init__.py` & `meerschaum-1.7.0.dev1/meerschaum/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/__main__.py` & `meerschaum-1.7.0.dev1/meerschaum/__main__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/_internal/arguments/__init__.py` & `meerschaum-1.7.0.dev1/meerschaum/_internal/arguments/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/_internal/arguments/_parse_arguments.py` & `meerschaum-1.7.0.dev1/meerschaum/_internal/arguments/_parse_arguments.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/_internal/arguments/_parser.py` & `meerschaum-1.7.0.dev1/meerschaum/_internal/arguments/_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -273,15 +273,22 @@
     '--no-auth', '--noauth', action='store_true',
     help = 'When starting the API, do not require authentication. WARNING: This is dangerous!',
 )
 groups['api'].add_argument(
     '--production', '--gunicorn', action='store_true',
     help = 'Start the API with the Gunicorn process manager.'
 )
-
+groups['api'].add_argument(
+    '--keyfile', type=str,
+    help = "Start the API server with this keyfile (requires --certfile).",
+)
+groups['api'].add_argument(
+    '--certfile', type=str,
+    help = "Start the API server with this certfile (requires --keyfile).",
+)
 ### Plugins options
 groups['plugins'].add_argument(
     '-r', '--repository', '--repo', type=str,
     help="Meerschaum plugins repository to connect to. Specify an API label (default: 'mrsm')"
 )
 
 ### Packages options
```

### Comparing `meerschaum-1.6.9/meerschaum/_internal/docs/index.py` & `meerschaum-1.7.0.dev1/meerschaum/_internal/docs/index.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/_internal/entry.py` & `meerschaum-1.7.0.dev1/meerschaum/_internal/entry.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/_internal/gui/__init__.py` & `meerschaum-1.7.0.dev1/meerschaum/_internal/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/_internal/gui/app/__init__.py` & `meerschaum-1.7.0.dev1/meerschaum/_internal/gui/app/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/_internal/gui/app/_windows.py` & `meerschaum-1.7.0.dev1/meerschaum/_internal/gui/app/_windows.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/_internal/gui/app/actions.py` & `meerschaum-1.7.0.dev1/meerschaum/_internal/gui/app/actions.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/_internal/gui/app/pipes.py` & `meerschaum-1.7.0.dev1/meerschaum/_internal/gui/app/pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/_internal/shell/Shell.py` & `meerschaum-1.7.0.dev1/meerschaum/_internal/shell/Shell.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/_internal/shell/ShellCompleter.py` & `meerschaum-1.7.0.dev1/meerschaum/_internal/shell/ShellCompleter.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/_internal/shell/ValidAutoSuggest.py` & `meerschaum-1.7.0.dev1/meerschaum/_internal/shell/ValidAutoSuggest.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/_internal/term/TermPageHandler.py` & `meerschaum-1.7.0.dev1/meerschaum/_internal/term/TermPageHandler.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/_internal/term/__init__.py` & `meerschaum-1.7.0.dev1/meerschaum/_internal/term/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/_internal/term/tools.py` & `meerschaum-1.7.0.dev1/meerschaum/_internal/term/tools.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,32 +4,22 @@
 
 """
 Utility functions regarding the webterm.
 """
 
 from __future__ import annotations
 
-def is_webterm_running(host: str, port: int) -> int:
-    """Determine whether the webterm service is running on a given host and port.
-
-    Parameters
-    ----------
-    host: str :
-        
-    port: int :
-        
-
-    Returns
-    -------
-
+def is_webterm_running(host: str, port: int, protocol: str = 'http') -> int:
+    """
+    Determine whether the webterm service is running on a given host and port.
     """
     from meerschaum.utils.networking import find_open_ports, is_port_in_use
     from meerschaum.utils.packages import attempt_import
     requests = attempt_import('requests')
-    url = f'http://{host}:{port}'
+    url = f'{protocol}://{host}:{port}'
     try:
         r = requests.get(url)
     except Exception as e:
         return False
     if not r:
         return False
     return '<title>Meerschaum Shell</title>' in r.text
```

### Comparing `meerschaum-1.6.9/meerschaum/actions/__init__.py` & `meerschaum-1.7.0.dev1/meerschaum/actions/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 """
 Default actions available to the mrsm CLI.
 """
 
 from __future__ import annotations
 from meerschaum.utils.typing import Callable, Any, Optional, Union, List, Dict, SuccessTuple
 from meerschaum.utils.packages import get_modules_from_package
-from meerschaum.utils.warnings import enable_depreciation_warnings
-enable_depreciation_warnings(__name__)
 _custom_actions = []
 
 ### build __all__ from other .py files in this package
 import sys
 modules = get_modules_from_package(
     sys.modules[__name__],
     names = False,
```

### Comparing `meerschaum-1.6.9/meerschaum/actions/api.py` & `meerschaum-1.7.0.dev1/meerschaum/actions/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -96,36 +96,45 @@
         mrsm_instance: Optional[str] = None,
         no_dash: bool = False,
         no_auth: bool = False,
         private: bool = False,
         debug: bool = False,
         nopretty: bool = False,
         production: bool = False,
+        keyfile: Optional[str] = None,
+        certfile: Optional[str] = None,
         **kw: Any
     ) -> SuccessTuple:
     """Start the API server.
    
     Parameters
     ----------
     port: Optional[int], default None
         Port to bind the API server to.
         If `None`, use 8000.
 
     host: Optional[str], defailt None
         The address to bind to.
-        If `None, use '0.0.0.0'.
+        If `None`, use '0.0.0.0'.
 
     workers: Optional[int], default None
         How many worker threads to run.
         If `None`, defaults to the number of CPU cores or 1 on Android.
 
     production: bool, default False
         Start the API server with Gunicorn instead of Uvicorn.
         Useful for production deployments.
 
+    keyfile: str, default None
+        If provided, serve over HTTPS with this key file.
+        Requires `--certfile`.
+
+    certfile: str, default None
+        If provided, serve over HTTPS with this certfile.
+        Requires `--keyfile`.
     """
     from meerschaum.utils.packages import (
         attempt_import, venv_contains_package, pip_install, run_python_package
     )
     from meerschaum.utils.misc import is_int, filter_keywords
     from meerschaum.utils.formatting import pprint, ANSI, _init
     from meerschaum.utils.debug import dprint
@@ -169,14 +178,18 @@
         if len(action) > 1:
             if is_int(action[1]):
                 port = int(action[1])
 
     if host is None:
         host = uvicorn_config['host']
 
+    if keyfile or certfile:
+        if not keyfile or not certfile:
+            return False, f"HTTPS requires both `--keyfile` and `--certfile`."
+
     pool = get_pool(workers=workers)
     if pool is None:
         workers = 1
     else:
         pool.close()
         pool.join()
     
@@ -216,14 +229,18 @@
         'no_auth': no_auth,
         'private': private,
     })
     if debug:
         uvicorn_config['reload'] = debug
         uvicorn_config['reload_dirs'] = [str(PACKAGE_ROOT_PATH)]
         uvicorn_config['reload_excludes'] = 'plugins/__init__.py'
+    if keyfile:
+        uvicorn_config['ssl_keyfile'] = keyfile
+    if certfile:
+        uvicorn_config['ssl_certfile'] = certfile
     uvicorn_config['use_colors'] = (not nopretty) if nopretty else ANSI
 
     api_config['uvicorn'] = uvicorn_config
     cf['system']['api']['uvicorn'] = uvicorn_config
 
     custom_keys = ['mrsm_instance', 'no_dash', 'no_auth', 'private', 'debug']
 
@@ -293,14 +310,19 @@
         ]
         for key, val in env_dict.items():
             gunicorn_args += [
                 '--env', key + '=' + (json.dumps(val) if isinstance(val, dict) else val)
             ]
         if workers is not None:
             gunicorn_args += ['--workers', str(workers)]
+        if uvicorn_config.get('ssl_keyfile', None):
+            gunicorn_args += [
+                '--keyfile', uvicorn_config['ssl_keyfile'],
+                '--certfile', uvicorn_config['ssl_certfile'],
+            ]
         if debug:
             gunicorn_args += ['--log-level=debug', '--enable-stdio-inheritance', '--reload']
         try:
             run_python_package('gunicorn', gunicorn_args, debug=debug, venv=None)
         except KeyboardInterrupt:
             pass
```

### Comparing `meerschaum-1.6.9/meerschaum/actions/bootstrap.py` & `meerschaum-1.7.0.dev1/meerschaum/actions/bootstrap.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/actions/clear.py` & `meerschaum-1.7.0.dev1/meerschaum/actions/clear.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/actions/copy.py` & `meerschaum-1.7.0.dev1/meerschaum/actions/copy.py`

 * *Files 3% similar despite different names*

```diff
@@ -113,15 +113,23 @@
                 (
                     f"Do you want to copy data from {p} into {_new_pipe}?\n\n"
                     + "If you specified `--begin`, `--end` or `--params`, data will be filtered."
                 ),
                     noask=noask, yes=yes
                 )
         ):
-            _new_pipe.sync(p.get_data(debug=debug, **kw), debug=debug, **kw)
+            _new_pipe.sync(
+                p.get_data(
+                    debug = debug,
+                    as_iterator = True,
+                    **kw
+                ),
+                debug = debug,
+                **kw
+            )
 
     msg = (
         "No pipes were copied." if successes == 0
         else (f"Copied {successes} pipe" + ("s" if successes != 1 else '') + '.')
     )
 
     return successes > 0, msg
```

### Comparing `meerschaum-1.6.9/meerschaum/actions/delete.py` & `meerschaum-1.7.0.dev1/meerschaum/actions/delete.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/actions/drop.py` & `meerschaum-1.7.0.dev1/meerschaum/actions/drop.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/actions/edit.py` & `meerschaum-1.7.0.dev1/meerschaum/actions/edit.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/actions/install.py` & `meerschaum-1.7.0.dev1/meerschaum/actions/install.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/actions/login.py` & `meerschaum-1.7.0.dev1/meerschaum/actions/login.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/actions/os.py` & `meerschaum-1.7.0.dev1/meerschaum/actions/os.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/actions/python.py` & `meerschaum-1.7.0.dev1/meerschaum/actions/python.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/actions/register.py` & `meerschaum-1.7.0.dev1/meerschaum/actions/register.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/actions/reload.py` & `meerschaum-1.7.0.dev1/meerschaum/actions/reload.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/actions/setup.py` & `meerschaum-1.7.0.dev1/meerschaum/actions/setup.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/actions/sh.py` & `meerschaum-1.7.0.dev1/meerschaum/actions/sh.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/actions/show.py` & `meerschaum-1.7.0.dev1/meerschaum/actions/show.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/actions/sql.py` & `meerschaum-1.7.0.dev1/meerschaum/actions/sql.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/actions/stack.py` & `meerschaum-1.7.0.dev1/meerschaum/actions/stack.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,14 +43,23 @@
         pip_install,
     )
     from meerschaum.config import get_config
     from meerschaum.utils.debug import dprint
     from meerschaum.utils.warnings import warn
     from meerschaum.utils.formatting import ANSI
     from meerschaum.utils.misc import is_docker_available
+    from meerschaum.config._read_config import search_and_substitute_config
+
+    stack_env_dict = {
+        var: val
+        for var, val in search_and_substitute_config(
+            meerschaum.config.stack.env_dict
+        ).items()
+        if isinstance(val, str)
+    }
 
     if action is None:
         action = []
     if sysargs is None:
         sysargs = []
     if sub_args is None:
         sub_args = []
@@ -135,22 +144,23 @@
         (
             ['docker', 'compose'] if has_builtin_compose
             else ['docker-compose']
         ) + cmd_list,
         cwd = STACK_COMPOSE_PATH.parent,
         stdout = stdout,
         stderr = stderr,
-        env = os.environ,
+        env = stack_env_dict,
     ) if (has_builtin_compose or has_binary_compose) else run_python_package(
         'compose',
         args = cmd_list,
         cwd = STACK_COMPOSE_PATH.parent,
         venv = _compose_venv,
         capture_output = _capture_output,
         as_proc = True,
+        env = stack_env_dict,
     )
     try:
         rc = proc.wait() if proc is not None else 1
     except KeyboardInterrupt:
         rc = 0
     if _capture_output and proc is not None:
         captured_stdout, captured_stderr = proc.communicate()
```

### Comparing `meerschaum-1.6.9/meerschaum/actions/start.py` & `meerschaum-1.7.0.dev1/meerschaum/actions/start.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/actions/stop.py` & `meerschaum-1.7.0.dev1/meerschaum/actions/stop.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/actions/sync.py` & `meerschaum-1.7.0.dev1/meerschaum/actions/sync.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/actions/uninstall.py` & `meerschaum-1.7.0.dev1/meerschaum/actions/uninstall.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/actions/upgrade.py` & `meerschaum-1.7.0.dev1/meerschaum/actions/upgrade.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/actions/verify.py` & `meerschaum-1.7.0.dev1/meerschaum/actions/verify.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/api/__init__.py` & `meerschaum-1.7.0.dev1/meerschaum/api/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,36 +133,44 @@
         'name': 'Bennett Meares',
         'url': 'https://meerschaum.io',
     },
     license_info = {
         'name': 'Apache 2.0',
         'url': 'https://www.apache.org/licenses/LICENSE-2.0.html',
     },
-    open_api_tags = [{
+    open_api_tags = [
+        {
             'name': 'Pipes',
             'description': 'Access pipes by indexing their keys.',
-        }, {
+        },
+        {
             'name': 'Actions',
             'description': 'Perform actions via the API.',
-        }, {
+        },
+        {
             'name': 'Connectors',
             'description': 'Get information about the registered connectors.'
-        }, {
+        },
+        {
             'name': 'Users',
             'description': 'Access, register, and delete users.',
-        }, {
+        },
+        {
             'name': 'Plugins',
             'description': 'Access, register, and delete plugins.',
-        }, {
+        },
+        {
             'name': 'Misc',
             'description': 'Miscellaneous endpoints.',
-        }, {
+        },
+        {
             'name': 'Version',
             'description': 'Version information.'
-    }],
+        }
+    ],
 )
 
 (
     fastapi_responses,
     fastapi_templating,
     fastapi_staticfiles,
 ) = attempt_import(
```

### Comparing `meerschaum-1.6.9/meerschaum/api/_chain.py` & `meerschaum-1.7.0.dev1/meerschaum/api/_chain.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/api/_oauth2.py` & `meerschaum-1.7.0.dev1/meerschaum/api/_oauth2.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,11 +23,11 @@
         secret_key = os.urandom(24).hex()
         with open(API_SECRET_KEY_PATH, 'w+') as f:
             f.write(secret_key)
     else:
         with open(API_SECRET_KEY_PATH, 'r') as f:
             secret_key = f.read()
 
-    return secret_key
+    return secret_key.encode('utf-8')
 
 SECRET = generate_secret_key()
 manager = LoginManager(SECRET, token_url=endpoints['login'])
```

### Comparing `meerschaum-1.6.9/meerschaum/api/_websockets.py` & `meerschaum-1.7.0.dev1/meerschaum/api/_websockets.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/api/dash/__init__.py` & `meerschaum-1.7.0.dev1/meerschaum/api/dash/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/api/dash/actions.py` & `meerschaum-1.7.0.dev1/meerschaum/api/dash/actions.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/api/dash/assets/ansi_up.js` & `meerschaum-1.7.0.dev1/meerschaum/api/dash/assets/ansi_up.js`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/api/dash/assets/banner_1920x320.png` & `meerschaum-1.7.0.dev1/meerschaum/api/dash/assets/banner_1920x320.png`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/api/dash/assets/favicon.ico` & `meerschaum-1.7.0.dev1/meerschaum/api/dash/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/api/dash/assets/logo_48x48.png` & `meerschaum-1.7.0.dev1/meerschaum/api/dash/assets/logo_48x48.png`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/api/dash/assets/logo_500x500.png` & `meerschaum-1.7.0.dev1/meerschaum/api/dash/assets/logo_500x500.png`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/api/dash/callbacks/dashboard.py` & `meerschaum-1.7.0.dev1/meerschaum/api/dash/callbacks/dashboard.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from meerschaum.api.dash.websockets import ws_url_from_href
 from meerschaum.connectors.parse import parse_instance_keys
 from meerschaum.api.dash.pipes import get_pipes_cards, pipe_from_ctx, accordion_items_from_pipe
 from meerschaum.api.dash.jobs import get_jobs_cards
 from meerschaum.api.dash.plugins import get_plugins_cards
 from meerschaum.api.dash.users import get_users_cards
 from meerschaum.api.dash.graphs import get_graphs_cards
+from meerschaum.api.dash.webterm import get_webterm
 from meerschaum.api.dash.components import alert_from_success_tuple, console_div, build_cards_grid
 from meerschaum.api.dash.actions import execute_action, check_input_interval, stop_action
 import meerschaum.api.dash.pages as pages
 from meerschaum.utils.typing import Dict
 from meerschaum.utils.debug import dprint
 from meerschaum.utils.packages import attempt_import, import_html, import_dcc
 from meerschaum.utils.misc import (
@@ -92,15 +93,15 @@
     'login',
     'copy',
 }
 _paths = {
     'login'   : pages.login.layout,
     ''        : pages.dashboard.layout,
     'plugins' : pages.plugins.layout,
-    'register' : pages.register.layout,
+    'register': pages.register.layout,
 }
 _required_login = {''}
  
 @dash_app.callback(
     Output('page-layout-div', 'children'),
     Output('session-store', 'data'),
     Input('location', 'pathname'),
@@ -125,25 +126,36 @@
     """
     ctx = dash.callback_context
     dash_endpoint = endpoints['dash']
     try:
         session_id = session_store_data.get('session-id', None) 
     except AttributeError:
         session_id = None
+
     ### Bypass login if `--no-auth` is specified.
-    if session_id is None and no_auth:
+    if session_id not in active_sessions and no_auth:
         session_store_data['session-id'] = str(uuid.uuid4())
         active_sessions[session_store_data['session-id']] = {'username': 'no-auth'}
-        session_store_to_return = session_data
+        session_store_to_return = session_store_data
     else:
         session_store_to_return = dash.no_update
 
-    _path = (pathname.rstrip('/') + '/').replace((dash_endpoint + '/'), '').rstrip('/')
-    path = _path if no_auth or _path not in _required_login else (
-        _path if session_id in active_sessions else 'login'
+    _path = (
+        pathname.rstrip('/') + '/'
+    ).replace(
+        (dash_endpoint + '/'),
+        ''
+    ).rstrip('/').split('/')[0]
+    path = (
+        _path
+        if no_auth or _path not in _required_login else (
+            _path
+            if session_id in active_sessions
+            else 'login'
+        )
     )
     layout = _paths.get(path, pages.error.layout)
     return layout, session_store_to_return
 
 
 @dash_app.callback(
     Output('content-div-right', 'children'),
@@ -153,14 +165,15 @@
     Input('go-button', 'n_clicks'),
     Input('cancel-button', 'n_clicks'),
     Input('get-pipes-button', 'n_clicks'),
     Input('get-jobs-button', 'n_clicks'),
     Input('get-plugins-button', 'n_clicks'),
     Input('get-users-button', 'n_clicks'),
     Input('get-graphs-button', 'n_clicks'),
+    Input('open-shell-button', 'n_clicks'),
     Input('check-input-interval', 'n_intervals'),
     State('location', 'href'),
     State('session-store', 'data'),
     *keys_state,
     #  prevent_initial_call=True,
 )
 def update_content(*args):
@@ -188,14 +201,15 @@
         'go-button': execute_action,
         'cancel-button': stop_action,
         'get-pipes-button': get_pipes_cards,
         'get-jobs-button': get_jobs_cards,
         'get-plugins-button': get_plugins_cards,
         'get-users-button': get_users_cards,
         'get-graphs-button': get_graphs_cards,
+        'open-shell-button': get_webterm,
         'check-input-interval': check_input_interval,
     }
     ### Defaults to 3 if not in dict.
     trigger_num_cols = {
         'get-graphs-button': 1,
         'get-pipes-button': 1,
     }
@@ -443,29 +457,30 @@
     """
     return not is_open if n_clicks else is_open
 
 @dash_app.callback(
     Output('ws', 'send'),
     Input('test-button', 'n_clicks'),
     Input('ws', 'url'),
+    Input('session-store', 'data'),
     State('ws', 'state'),
     State('ws', 'message'),
     State('ws', 'error'),
     State('ws', 'protocols'),
-    State('session-store', 'data'),
-    #  prevent_initial_call = True,
 )
-def ws_send(n_clicks: int, url, *states):
+def ws_send(n_clicks: int, url, session_store_data: Dict[str, Any], *states):
     """
     Send an initial connection message over the websocket.
     """
     ctx = dash.callback_context
     if not url:
         raise PreventUpdate
-    session_id = ctx.states['session-store.data']['session-id']
+    session_id = session_store_data.get('session-id', None)
+    if session_id is None:
+        raise PreventUpdate
     return json.dumps({
         'connect-time': json_serialize_datetime(datetime.datetime.utcnow()),
         'session-id': session_id,
     })
 
 @dash_app.callback(
     Output('content-div-right', 'children'),
```

### Comparing `meerschaum-1.6.9/meerschaum/api/dash/callbacks/login.py` & `meerschaum-1.7.0.dev1/meerschaum/api/dash/callbacks/login.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/api/dash/callbacks/plugins.py` & `meerschaum-1.7.0.dev1/meerschaum/api/dash/callbacks/plugins.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/api/dash/callbacks/register.py` & `meerschaum-1.7.0.dev1/meerschaum/api/dash/callbacks/register.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/api/dash/components.py` & `meerschaum-1.7.0.dev1/meerschaum/api/dash/components.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,18 +26,19 @@
 
 }
 
 go_button = dbc.Button('Execute', id='go-button', color='primary', style={'width': '100%'})
 test_button = dbc.Button('Test', id='test-button', color='danger', style={'display' : 'none'})
 get_items_menu = dbc.DropdownMenu(
     label='More', id='get-items-menu', children=[
-        dbc.DropdownMenuItem("Graphs", id='get-graphs-button'),
+        dbc.DropdownMenuItem("Shell", id='open-shell-button'),
         dbc.DropdownMenuItem("Jobs", id='get-jobs-button'),
         dbc.DropdownMenuItem("Plugins", id='get-plugins-button'),
         dbc.DropdownMenuItem("Users", id='get-users-button'),
+        dbc.DropdownMenuItem("Graphs", id='get-graphs-button'),
     ],
     style={'width': '100%', 'font-size': '0.5em'},
     menu_variant='dark',
     toggle_style={'width': '100%'},
     color='secondary',
     size='sm',
 )
@@ -97,45 +98,36 @@
         [
             html.A(
                 dbc.Row(
                     [
                         dbc.Col(
                                 html.Img(
                                     src = endpoints['dash'] + "/assets/logo_48x48.png",
-                                    #  style = {'padding': '0.5em', 'padding-left': '2em'},
                                     title = doc,
                                 ),
-                            #  width = 'auto', 
-                            #  align = 'start'
                         ),
-                        #  dbc.Col(
-                            #  dbc.NavbarBrand(
-                                #  "Web Console",
-                                #  class_name = 'ms-2',
-                                #  style = {'margin-top': '10px', 'display': 'inline-block'}
-                            #  ),
-                            #  align = 'start',
-                            #  width = 2,
-                        #  ),
                     ],
-                    #  style = {'width': '100%'},
                     align = 'center',
                     className = 'g-0 navbar-logo-row',
-                    #  justify = 'around',
                 ),
                 href = '/docs',
                 style = {"textDecoration": "none"},
             ),
             dbc.NavbarToggler(id="navbar-toggler", n_clicks=0),
             dbc.Collapse(
                 dbc.Row(
                     [
-                        dbc.Col(
-                            instance_select,
-                        ),
+                        #  dbc.Col(
+                            #  dbc.Button(
+                                #  html.B("Open Shell"),
+                                #  outline = True,
+                                #  id = "open-shell-button"
+                            #  ),
+                        #  ),
+                        dbc.Col(instance_select),
                         dbc.Col(
                             dbc.Button(
                                 "Sign out",
                                 color = 'link',
                                 style = {'margin-left': '30px'},
                                 id = 'sign-out-button',
                             ),
```

### Comparing `meerschaum-1.6.9/meerschaum/api/dash/connectors.py` & `meerschaum-1.7.0.dev1/meerschaum/api/dash/connectors.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/api/dash/graphs.py` & `meerschaum-1.7.0.dev1/meerschaum/api/dash/graphs.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,21 +23,21 @@
     from meerschaum.api.dash.pipes import pipes_from_state
     pipes = pipes_from_state(state, as_list=True)
     cards, alerts = [], []
     for pipe in pipes:
         dt_name, id_name = pipe.get_columns('datetime', 'id', error=False)
         val_name = pipe.get_val_column(debug=debug)
         if dt_name is not None and val_name is not None:
-            df = pipe.get_backtrack_data(backtrack_minutes=(1440))
+            df = pipe.get_backtrack_data(backtrack_minutes=1440)
             fig_args = {
                 'data_frame': df,
                 'x': dt_name,
                 'y': val_name,
                 'line_group': id_name,
-                'title': f"Recent Data for Pipe\n'{pipe}'"
+                'title': f"{pipe}"
             }
             try:
                 fig = px.line(**fig_args)
                 graph = dcc.Graph(figure=fig)
                 body = graph
             except Exception as e:
                 body = html.P(
```

### Comparing `meerschaum-1.6.9/meerschaum/api/dash/jobs.py` & `meerschaum-1.7.0.dev1/meerschaum/api/dash/jobs.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/api/dash/keys.py` & `meerschaum-1.7.0.dev1/meerschaum/api/dash/keys.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/api/dash/pages/dashboard.py` & `meerschaum-1.7.0.dev1/meerschaum/api/dash/pages/dashboard.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/api/dash/pages/error.py` & `meerschaum-1.7.0.dev1/meerschaum/api/dash/pages/error.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/api/dash/pages/login.py` & `meerschaum-1.7.0.dev1/meerschaum/api/dash/pages/login.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/api/dash/pages/plugins.py` & `meerschaum-1.7.0.dev1/meerschaum/api/dash/pages/plugins.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,36 +11,35 @@
 from meerschaum.utils.packages import import_html, import_dcc
 html, dcc = import_html(check_update=CHECK_UPDATE), import_dcc(check_update=CHECK_UPDATE)
 import dash_bootstrap_components as dbc
 from meerschaum.core import Plugin
 from meerschaum.utils.typing import Optional
 
 search_box = dbc.Input(
-    id="search-plugins-input",
-    placeholder="Search for plugins...",
-    type="text"
+    id = "search-plugins-input",
+    placeholder = "Search for plugins...",
+    type = "text",
 )
 
 layout = dbc.Container([
     html.Div([
         html.Br(),
         html.Div(
             dbc.Container([
                 html.H3('Plugins'),
                 html.P('Plugins extend the functionality of Meerschaum.'),
                 html.A(
                     'To find out more, check out the plugins documentation.',
-                    href='https://meerschaum.io/reference/plugins/using-plugins/',
-                    rel="noreferrer noopener",
-                    target="_blank",
+                    href = 'https://meerschaum.io/reference/plugins/',
+                    rel = "noreferrer noopener",
+                    target = "_blank",
                 ),
             ]),
-            className='page-header',
-            style={'background-color': 'var(--dark)', 'padding': '1em'},
+            className = 'page-header',
+            style = {'background-color': 'var(--dark)', 'padding': '1em'},
         ),
         html.Br(),
-        #  html.Div([], id='edit-alert-div'),
         search_box,
         html.Br(),
         html.Div([], id='plugins-cards-div'),
     ])
 ])
```

### Comparing `meerschaum-1.6.9/meerschaum/api/dash/pages/register.py` & `meerschaum-1.7.0.dev1/meerschaum/api/dash/pages/register.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/api/dash/pipes.py` & `meerschaum-1.7.0.dev1/meerschaum/api/dash/pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/api/dash/plugins.py` & `meerschaum-1.7.0.dev1/meerschaum/api/dash/plugins.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/api/dash/users.py` & `meerschaum-1.7.0.dev1/meerschaum/api/dash/users.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,10 +16,10 @@
 dbc = attempt_import('dash_bootstrap_components', lazy=False, check_update=CHECK_UPDATE)
 
 def get_users_cards(state: WebState) -> Tuple[List[dbc.Card], List[SuccessTuple]]:
     cards, alerts = [], [] 
     conn = get_web_connector(state)
     usernames = conn.get_users(debug=debug)
     for username in usernames:
-        cards.append(dbc.Card(username))
+        cards.append(dbc.Card(html.H4(username)))
 
     return cards, alerts
```

### Comparing `meerschaum-1.6.9/meerschaum/api/dash/websockets.py` & `meerschaum-1.7.0.dev1/meerschaum/api/dash/websockets.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/api/resources/static/css/bootstrap.min.css` & `meerschaum-1.7.0.dev1/meerschaum/api/resources/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/api/resources/static/css/dash.css` & `meerschaum-1.7.0.dev1/meerschaum/api/resources/static/css/dash.css`

 * *Files 10% similar despite different names*

```diff
@@ -13,19 +13,24 @@
   width: 650px!ie7;
   padding-bottom: 20px!ie7;
   max-height: 600px;
 }
 #console-div {
   overflow-y: scroll;
   max-height: 85vh;
-  height: 85vh;
+  height: 84vh;
   color: white;
   background-color: black;
   padding: 0.5em;
 }
+#webterm-iframe {
+  width: 102%;
+  height: 85vh !important;
+  max-height: 85vh;
+}
 .codeblock {
   background-color: var(--bs-secondary) !important;
   color: white !important;
   display: block !important;
   overflow-x: auto !important;
   padding: 0.5em !important;
```

### Comparing `meerschaum-1.6.9/meerschaum/api/resources/static/css/dbc_dark.css` & `meerschaum-1.7.0.dev1/meerschaum/api/resources/static/css/dbc_dark.css`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/api/resources/static/ico/logo.ico` & `meerschaum-1.7.0.dev1/meerschaum/api/resources/static/ico/logo.ico`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/api/resources/static/js/action_button.js` & `meerschaum-1.7.0.dev1/meerschaum/api/resources/static/js/action_button.js`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/api/resources/templates/index.html` & `meerschaum-1.7.0.dev1/meerschaum/api/resources/templates/index.html`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/api/resources/templates/old_index.html` & `meerschaum-1.7.0.dev1/meerschaum/api/resources/templates/old_index.html`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/api/resources/templates/termpage.html` & `meerschaum-1.7.0.dev1/meerschaum/api/resources/templates/termpage.html`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/api/routes/__init__.py` & `meerschaum-1.7.0.dev1/meerschaum/api/routes/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/api/routes/_actions.py` & `meerschaum-1.7.0.dev1/meerschaum/api/routes/_actions.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/api/routes/_connectors.py` & `meerschaum-1.7.0.dev1/meerschaum/api/routes/_connectors.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/api/routes/_index.py` & `meerschaum-1.7.0.dev1/meerschaum/api/routes/_index.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/api/routes/_login.py` & `meerschaum-1.7.0.dev1/meerschaum/api/routes/_login.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/api/routes/_misc.py` & `meerschaum-1.7.0.dev1/meerschaum/api/routes/_misc.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 
 @app.get(endpoints['info'], tags=['Misc'])
 def get_instance_info(
         curr_user = (
             fastapi.Depends(manager) if private else None
         ),
-    ) -> Dict[str, str]:
+    ) -> Dict[str, Union[str, int]]:
     from meerschaum import __version__ as version
     num_plugins = len(get_api_connector().get_plugins(debug=debug))
     num_users = len(get_api_connector().get_users(debug=debug))
     num_pipes = len(get_pipes(mrsm_instance=get_api_connector(), as_list=True))
     return {
         'version': version,
         'num_plugins': num_plugins,
```

### Comparing `meerschaum-1.6.9/meerschaum/api/routes/_pipes.py` & `meerschaum-1.7.0.dev1/meerschaum/api/routes/_pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/api/routes/_plugins.py` & `meerschaum-1.7.0.dev1/meerschaum/api/routes/_plugins.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/api/routes/_users.py` & `meerschaum-1.7.0.dev1/meerschaum/api/routes/_users.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     return get_api_connector().get_users(debug=debug)
 
 
 @app.post(users_endpoint + "/register", tags=['Users'])
 def register_user(
         username: str = Form(None),
         password: str = Form(None),
-        attributes: str = Form(None, examples={'test': {'foo': 'bar'}}),
+        attributes: str = Form(None),
         type: str = Form(None),
         email: str = Form(None),
         curr_user = (
             fastapi.Depends(manager) if private else None
         ),
     ) -> SuccessTuple:
     """
```

### Comparing `meerschaum-1.6.9/meerschaum/api/routes/_version.py` & `meerschaum-1.7.0.dev1/meerschaum/api/routes/_version.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/api/tables/__init__.py` & `meerschaum-1.7.0.dev1/meerschaum/api/tables/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/config/__init__.py` & `meerschaum-1.7.0.dev1/meerschaum/config/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/config/_default.py` & `meerschaum-1.7.0.dev1/meerschaum/config/_default.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/config/_edit.py` & `meerschaum-1.7.0.dev1/meerschaum/config/_edit.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/config/_environment.py` & `meerschaum-1.7.0.dev1/meerschaum/config/_environment.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/config/_formatting.py` & `meerschaum-1.7.0.dev1/meerschaum/config/_formatting.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/config/_jobs.py` & `meerschaum-1.7.0.dev1/meerschaum/config/_jobs.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/config/_patch.py` & `meerschaum-1.7.0.dev1/meerschaum/config/_patch.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/config/_paths.py` & `meerschaum-1.7.0.dev1/meerschaum/config/_paths.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/config/_preprocess.py` & `meerschaum-1.7.0.dev1/meerschaum/config/_preprocess.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/config/_read_config.py` & `meerschaum-1.7.0.dev1/meerschaum/config/_read_config.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/config/_shell.py` & `meerschaum-1.7.0.dev1/meerschaum/config/_shell.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/config/_sync.py` & `meerschaum-1.7.0.dev1/meerschaum/config/_sync.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/config/stack/__init__.py` & `meerschaum-1.7.0.dev1/meerschaum/config/stack/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,14 @@
 }
 ### apply patch to host config to change hostname to the Docker service name
 env_dict['MEERSCHAUM_API_CONFIG'] = json.dumps(
     {
         'meerschaum' : 'MRSM{!meerschaum}',
         'system' : 'MRSM{!system}',
     },
-    #  separators = (',', ':'),
     indent = 4,
 ).replace(
     '"MRSM{!system}"', 'MRSM{!system}'
 ).replace(
     '"MRSM{!meerschaum}"', 'MRSM{!meerschaum}',
 )
 
@@ -90,25 +89,34 @@
 }
 networks = {
     'frontend' : None,
     'backend' : None,
 }
 
 default_docker_compose_config = {
-    'version': '3.2',
+    'version': '3.9',
     'services': {
         'db': {
             'environment': {
                 'TIMESCALEDB_TELEMETRY': 'off',
-                'POSTGRES_USER': env_dict['POSTGRES_USER'],
-                'POSTGRES_DB': env_dict['POSTGRES_DB'],
-                'POSTGRES_PASSWORD': env_dict['POSTGRES_PASSWORD'],
+                'POSTGRES_USER': '$POSTGRES_USER',
+                'POSTGRES_DB': '$POSTGRES_DB',
+                'POSTGRES_PASSWORD': '$POSTGRES_PASSWORD',
                 'ALLOW_IP_RANGE': env_dict['ALLOW_IP_RANGE'],
             },
             'command': 'postgres -c max_connections=1000 -c shared_buffers=1024MB',
+            'healthcheck': {
+                'test': [
+                    'CMD-SHELL', 'pg_isready',
+                    '-U', '$POSTGRES_USER', '-d', '$POSTGRES_DB',
+                ],
+                'interval': '5s',
+                'timeout': '3s',
+                'retries': 3
+            },
             'restart': 'always',
             'image' : 'timescale/timescaledb:' + env_dict['TIMESCALEDB_VERSION'],
             'ports' : [
                 f'{db_port}:5432',
             ],
             'hostname' : f'{db_hostname}',
             'volumes' : [
@@ -128,36 +136,40 @@
                 'backend',
             ],
             'command': f'start api --production --port {api_port}',
             'environment': {
                 'MRSM_CONFIG': env_dict['MEERSCHAUM_API_CONFIG'],
                 'MRSM_PATCH': env_dict['MEERSCHAUM_API_PATCH'],
             },
-            'restart' : 'always',
+            'restart': 'always',
             'init': True,
-            'depends_on' : [
-                'db',
-            ],
+            'depends_on': {
+                'db': {
+                    'condition': 'service_healthy',
+                },
+            },
             'volumes' : [
                 'api_root:' + volumes['api_root'],
             ],
         },
         'grafana': {
             'image': 'grafana/grafana:latest',
             'ports': [
                 '3000:3000',
             ],
             'networks': [
                 'frontend',
                 'backend',
             ],
             'restart': 'always',
-            'depends_on': [
-                'db',
-            ],
+            'depends_on': {
+                'db': {
+                    'condition': 'service_healthy',
+                },
+            },
             'volumes': [
                 'grafana_storage' + ':' + volumes['grafana_storage'],
                 ### NOTE: Mount with the 'z' option for SELinux.
                 f'{GRAFANA_DATASOURCE_PATH.parent}:/etc/grafana/provisioning/datasources:z,ro',
                 f'{GRAFANA_DASHBOARD_PATH.parent}:/etc/grafana/provisioning/dashboards:z,ro',
             ],
             'environment': {
```

### Comparing `meerschaum-1.6.9/meerschaum/config/stack/grafana/__init__.py` & `meerschaum-1.7.0.dev1/meerschaum/config/stack/grafana/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/config/static/__init__.py` & `meerschaum-1.7.0.dev1/meerschaum/config/static/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,14 +31,15 @@
             'dash': '/dash',
             'term': '/term',
             'info': '/info',
         },
         'oauth': {
             'token_expires_minutes': 720,
         },
+        'webterm_job_name': '_webterm',
     },
     'environment': {
         'config': 'MRSM_CONFIG',
         'patch': 'MRSM_PATCH',
         'root': 'MRSM_ROOT_DIR',
         'plugins': 'MRSM_PLUGINS_DIR',
         'runtime': 'MRSM_RUNTIME',
```

### Comparing `meerschaum-1.6.9/meerschaum/connectors/Connector.py` & `meerschaum-1.7.0.dev1/meerschaum/connectors/Connector.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/connectors/__init__.py` & `meerschaum-1.7.0.dev1/meerschaum/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/connectors/api/APIConnector.py` & `meerschaum-1.7.0.dev1/meerschaum/connectors/api/APIConnector.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 class APIConnector(Connector):
     """
     Connect to a Meerschaum API instance.
     """
 
     IS_INSTANCE: bool = True
+    IS_THREAD_SAFE: bool = False
 
     from ._delete import delete
     from ._post import post
     from ._patch import patch
     from ._get import get, wget
     from ._actions import get_actions, do_action
     from ._misc import get_mrsm_version, get_chaining_status
```

### Comparing `meerschaum-1.6.9/meerschaum/connectors/api/_actions.py` & `meerschaum-1.7.0.dev1/meerschaum/connectors/api/_actions.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/connectors/api/_delete.py` & `meerschaum-1.7.0.dev1/meerschaum/connectors/api/_delete.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/connectors/api/_fetch.py` & `meerschaum-1.7.0.dev1/meerschaum/connectors/api/_fetch.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/connectors/api/_get.py` & `meerschaum-1.7.0.dev1/meerschaum/connectors/api/_get.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/connectors/api/_login.py` & `meerschaum-1.7.0.dev1/meerschaum/connectors/api/_login.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/connectors/api/_misc.py` & `meerschaum-1.7.0.dev1/meerschaum/connectors/api/_misc.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/connectors/api/_patch.py` & `meerschaum-1.7.0.dev1/meerschaum/connectors/api/_patch.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/connectors/api/_pipes.py` & `meerschaum-1.7.0.dev1/meerschaum/connectors/api/_pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/connectors/api/_plugins.py` & `meerschaum-1.7.0.dev1/meerschaum/connectors/api/_plugins.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/connectors/api/_post.py` & `meerschaum-1.7.0.dev1/meerschaum/connectors/api/_post.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/connectors/api/_uri.py` & `meerschaum-1.7.0.dev1/meerschaum/connectors/api/_uri.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/connectors/api/_users.py` & `meerschaum-1.7.0.dev1/meerschaum/connectors/api/_users.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/connectors/parse.py` & `meerschaum-1.7.0.dev1/meerschaum/connectors/parse.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/connectors/plugin/PluginConnector.py` & `meerschaum-1.7.0.dev1/meerschaum/connectors/plugin/PluginConnector.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/connectors/poll.py` & `meerschaum-1.7.0.dev1/meerschaum/connectors/poll.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/connectors/sql/SQLConnector.py` & `meerschaum-1.7.0.dev1/meerschaum/connectors/sql/SQLConnector.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,26 +23,25 @@
     """
 
     IS_INSTANCE: bool = True
 
     from ._create_engine import flavor_configs, create_engine
     from ._sql import read, value, exec, execute, to_sql, exec_queries
     from meerschaum.utils.sql import test_connection
-    from ._fetch import fetch, get_pipe_metadef
+    from ._fetch import fetch, get_pipe_metadef, get_pipe_backtrack_minutes
     from ._cli import cli
     from ._pipes import (
         fetch_pipes_keys,
         create_indices,
         drop_indices,
         get_create_index_queries,
         get_drop_index_queries,
         get_add_columns_queries,
         get_alter_columns_queries,
         delete_pipe,
-        get_backtrack_data,
         get_pipe_data,
         get_pipe_data_query,
         register_pipe,
         edit_pipe,
         get_pipe_id,
         get_pipe_attributes,
         sync_pipe,
@@ -220,24 +219,41 @@
         ### handle different threads
         if not same_thread:
             pass
 
         return self._engine
 
     @property
-    def DATABASE_URL(self):
+    def DATABASE_URL(self) -> str:
+        """
+        Return the URI connection string (alias for `SQLConnector.URI`.
+        """
         _ = self.engine
         return str(self._engine_str)
 
     @property
-    def URI(self):
+    def URI(self) -> str:
+        """
+        Return the URI connection string.
+        """
         _ = self.engine
         return str(self._engine_str)
 
     @property
+    def IS_THREAD_SAFE(self) -> str:
+        """
+        Return whether this connector may be multithreaded.
+        """
+        if self.flavor == 'duckdb':
+            return False
+        if self.flavor == 'sqlite':
+            return ':memory:' not in self.URI
+        return True
+
+    @property
     def metadata(self):
         from meerschaum.utils.packages import attempt_import
         sqlalchemy = attempt_import('sqlalchemy')
         if '_metadata' not in self.__dict__:
             self._metadata = sqlalchemy.MetaData()
         return self._metadata
```

### Comparing `meerschaum-1.6.9/meerschaum/connectors/sql/_cli.py` & `meerschaum-1.7.0.dev1/meerschaum/connectors/sql/_cli.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/connectors/sql/_create_engine.py` & `meerschaum-1.7.0.dev1/meerschaum/connectors/sql/_create_engine.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/connectors/sql/_fetch.py` & `meerschaum-1.7.0.dev1/meerschaum/connectors/sql/_fetch.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,15 +133,15 @@
     from meerschaum.utils.debug import dprint
     from meerschaum.utils.warnings import warn, error
     from meerschaum.utils.sql import sql_item_name, dateadd_str, build_where
     from meerschaum.utils.misc import is_int
     from meerschaum.config import get_config
 
     definition = get_pipe_query(pipe)
-    btm = get_pipe_backtrack_minutes(pipe) 
+    btm = self.get_pipe_backtrack_minutes(pipe) 
 
     if not pipe.columns.get('datetime', None):
         _dt = pipe.guess_datetime()
         dt_name = sql_item_name(_dt, self.flavor) if _dt else None
         is_guess = True
     else:
         _dt = pipe.get_columns('datetime')
@@ -266,14 +266,15 @@
     else:
         dict_to_set = pipe.parameters
         key_to_set = 'sql'
 
     dict_to_set[key_to_set] = query
 
 
+@staticmethod
 def get_pipe_backtrack_minutes(pipe) -> Union[int, float]:
     """
     Return the first available value for the following parameter keys:
     
     - fetch, backtrack_minutes
     - backtrack_minutes
     """
```

### Comparing `meerschaum-1.6.9/meerschaum/connectors/sql/_pipes.py` & `meerschaum-1.7.0.dev1/meerschaum/connectors/sql/_pipes.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     """
     from meerschaum.utils.debug import dprint
     from meerschaum.utils.packages import attempt_import
     from meerschaum.utils.sql import json_flavors
 
     ### ensure pipes table exists
     from meerschaum.connectors.sql.tables import get_tables
-    pipes = get_tables(mrsm_instance=self, create=(not pipe.temporary), debug=debug)['pipes']
+    pipes_tbl = get_tables(mrsm_instance=self, create=(not pipe.temporary), debug=debug)['pipes']
 
     if pipe.get_id(debug=debug) is not None:
         return False, f"{pipe} is already registered."
 
     ### NOTE: if `parameters` is supplied in the Pipe constructor,
     ###       then `pipe.parameters` will exist and not be fetched from the database.
 
@@ -57,15 +57,15 @@
         'location_key'   : pipe.location_key,
         'parameters'     : (
             json.dumps(parameters)
             if self.flavor not in json_flavors
             else parameters
         ),
     }
-    query = sqlalchemy.insert(pipes).values(**values)
+    query = sqlalchemy.insert(pipes_tbl).values(**values)
     result = self.exec(query, debug=debug)
     if result is None:
         return False, f"Failed to register {pipe}."
     return True, f"Successfully registered {pipe}."
 
 
 def edit_pipe(
@@ -107,28 +107,28 @@
         parameters = apply_patch_to_config(
             original_parameters,
             pipe.parameters
         )
 
     ### ensure pipes table exists
     from meerschaum.connectors.sql.tables import get_tables
-    pipes = get_tables(mrsm_instance=self, create=(not pipe.temporary), debug=debug)['pipes']
+    pipes_tbl = get_tables(mrsm_instance=self, create=(not pipe.temporary), debug=debug)['pipes']
 
     import json
     sqlalchemy = attempt_import('sqlalchemy')
 
     values = {
         'parameters': (
             json.dumps(parameters)
             if self.flavor not in json_flavors
             else parameters
         ),
     }
-    q = sqlalchemy.update(pipes).values(**values).where(
-        pipes.c.pipe_id == pipe.id
+    q = sqlalchemy.update(pipes_tbl).values(**values).where(
+        pipes_tbl.c.pipe_id == pipe.id
     )
 
     result = self.exec(q, debug=debug)
     message = (
         f"Successfully edited {pipe}."
         if result is not None else f"Failed to edit {pipe}."
     )
@@ -210,77 +210,77 @@
             parameters[col] = vals
     cols = {k: v for k, v in cols.items() if v != [None]}
 
     if not table_exists('pipes', self, debug=debug):
         return []
 
     from meerschaum.connectors.sql.tables import get_tables
-    pipes = get_tables(mrsm_instance=self, create=False, debug=debug)['pipes']
+    pipes_tbl = get_tables(mrsm_instance=self, create=False, debug=debug)['pipes']
 
     _params = {}
     for k, v in parameters.items():
         _v = json.dumps(v) if isinstance(v, dict) else v
         _params[k] = _v
 
     negation_prefix = STATIC_CONFIG['system']['fetch_pipes_keys']['negation_prefix']
     ### Parse regular params.
     ### If a param begins with '_', negate it instead.
     _where = [
         (
-            (pipes.c[key] == val) if not str(val).startswith(negation_prefix)
-            else (pipes.c[key] != key)
+            (pipes_tbl.c[key] == val) if not str(val).startswith(negation_prefix)
+            else (pipes_tbl.c[key] != key)
         ) for key, val in _params.items()
-            if not isinstance(val, (list, tuple)) and key in pipes.c
+            if not isinstance(val, (list, tuple)) and key in pipes_tbl.c
     ]
     select_cols = (
-        [pipes.c.connector_keys, pipes.c.metric_key, pipes.c.location_key]
-        + ([pipes.c.parameters] if tags else [])
+        [pipes_tbl.c.connector_keys, pipes_tbl.c.metric_key, pipes_tbl.c.location_key]
+        + ([pipes_tbl.c.parameters] if tags else [])
     )
 
     q = sqlalchemy.select(*select_cols).where(sqlalchemy.and_(True, *_where))
 
     ### Parse IN params and add OR IS NULL if None in list.
     for c, vals in cols.items():
-        if not isinstance(vals, (list, tuple)) or not vals or not c in pipes.c:
+        if not isinstance(vals, (list, tuple)) or not vals or not c in pipes_tbl.c:
             continue
         _in_vals, _ex_vals = separate_negation_values(vals)
         ### Include params (positive)
         q = (
-            q.where(pipes.c[c].in_(_in_vals)) if None not in _in_vals
-            else q.where(sqlalchemy.or_(pipes.c[c].in_(_in_vals), pipes.c[c].is_(None)))
+            q.where(pipes_tbl.c[c].in_(_in_vals)) if None not in _in_vals
+            else q.where(sqlalchemy.or_(pipes_tbl.c[c].in_(_in_vals), pipes_tbl.c[c].is_(None)))
         ) if _in_vals else q
         ### Exclude params (negative)
-        q = q.where(pipes.c[c].not_in(_ex_vals)) if _ex_vals else q
+        q = q.where(pipes_tbl.c[c].not_in(_ex_vals)) if _ex_vals else q
 
     ### Finally, parse tags.
     _in_tags, _ex_tags = separate_negation_values(tags)
     ors = []
     for nt in _in_tags:
         ors.append(
             sqlalchemy.cast(
-                pipes.c['parameters'],
+                pipes_tbl.c['parameters'],
                 sqlalchemy.String,
             ).like(f'%"tags":%"{nt}"%')
         )
     q = q.where(sqlalchemy.and_(sqlalchemy.or_(*ors).self_group())) if ors else q
     ors = []
     for xt in _ex_tags:
         ors.append(
             sqlalchemy.cast(
-                pipes.c['parameters'],
+                pipes_tbl.c['parameters'],
                 sqlalchemy.String,
             ).not_like(f'%"tags":%"{xt}"%')
         )
     q = q.where(sqlalchemy.and_(sqlalchemy.or_(*ors).self_group())) if ors else q
-    loc_asc = sqlalchemy.asc(pipes.c['location_key'])
+    loc_asc = sqlalchemy.asc(pipes_tbl.c['location_key'])
     if self.flavor not in OMIT_NULLSFIRST_FLAVORS:
         loc_asc = sqlalchemy.nullsfirst(loc_asc)
     q = q.order_by(
-        sqlalchemy.asc(pipes.c['connector_keys']),
-        sqlalchemy.asc(pipes.c['metric_key']),
+        sqlalchemy.asc(pipes_tbl.c['connector_keys']),
+        sqlalchemy.asc(pipes_tbl.c['metric_key']),
         loc_asc,
     )
 
     ### execute the query and return a list of tuples
     if debug:
         dprint(q.compile(compile_kwargs={'literal_binds': True}))
     try:
@@ -561,84 +561,23 @@
         return drop_tuple
 
     if not pipe.id:
         return False, f"{pipe} is not registered."
 
     ### ensure pipes table exists
     from meerschaum.connectors.sql.tables import get_tables
-    pipes = get_tables(mrsm_instance=self, create=(not pipe.temporary), debug=debug)['pipes']
+    pipes_tbl = get_tables(mrsm_instance=self, create=(not pipe.temporary), debug=debug)['pipes']
 
-    q = sqlalchemy.delete(pipes).where(pipes.c.pipe_id == pipe.id)
+    q = sqlalchemy.delete(pipes_tbl).where(pipes_tbl.c.pipe_id == pipe.id)
     if not self.exec(q, debug=debug):
         return False, f"Failed to delete registration for {pipe}."
 
     return True, "Success"
 
 
-def get_backtrack_data(
-        self,
-        pipe: Optional[meerschaum.Pipe] = None,
-        backtrack_minutes: int = 0,
-        begin: Optional[datetime.datetime] = None,
-        params: Optional[Dict[str, Any]] = None,
-        limit: Optional[int] = None,
-        chunksize: Optional[int] = -1,
-        debug: bool = False
-    ) -> Union[pandas.DataFrame, None]:
-    """
-    Get the most recent backtrack_minutes' worth of data from a Pipe.
-
-    Parameters
-    ----------
-    pipe: meerschaum.Pipe:
-        The pipe to get data from.
-
-    backtrack_minutes: int, default 0
-        How far into the past to look for data.
-
-    begin: Optional[datetime.datetime], default None
-        Where to start traversing from. Defaults to `None`, which uses the
-        `meerschaum.Pipe.get_sync_time` value.
-
-    params: Optional[Dict[str, Any]], default None
-        Additional parameters to filter by.
-        See `meerschaum.connectors.sql.build_where`.
-
-    limit: Optional[int], default None
-        If specified, limit the number of rows retrieved to this value.
-
-    chunksize: Optional[int], default -1
-        The size of dataframe chunks to load into memory.
-
-    debug: bool, default False
-        Verbosity toggle.
-
-    Returns
-    -------
-    A `pd.DataFrame` of backtracked data.
-
-    """
-    import datetime
-    from meerschaum.utils.warnings import error
-    if pipe is None:
-        error("Pipe must be provided.")
-    if begin is None:
-        begin = pipe.get_sync_time(debug=debug)
-
-    return pipe.get_data(
-        begin = begin,
-        begin_add_minutes = (-1 * backtrack_minutes),
-        order = 'desc',
-        params = params,
-        limit = limit,
-        chunksize = chunksize,
-        debug = debug,
-    )
-
-
 def get_pipe_data(
         self,
         pipe: Optional[meerschaum.Pipe] = None,
         begin: Union[datetime.datetime, str, None] = None,
         end: Union[datetime.datetime, str, None] = None,
         params: Optional[Dict[str, Any]] = None,
         order: str = 'asc',
@@ -964,23 +903,23 @@
     """
     if pipe.temporary:
         return None
     from meerschaum.utils.packages import attempt_import
     import json
     sqlalchemy = attempt_import('sqlalchemy')
     from meerschaum.connectors.sql.tables import get_tables
-    pipes = get_tables(mrsm_instance=self, create=(not pipe.temporary), debug=debug)['pipes']
+    pipes_tbl = get_tables(mrsm_instance=self, create=(not pipe.temporary), debug=debug)['pipes']
 
-    query = sqlalchemy.select(pipes.c.pipe_id).where(
-        pipes.c.connector_keys == pipe.connector_keys
+    query = sqlalchemy.select(pipes_tbl.c.pipe_id).where(
+        pipes_tbl.c.connector_keys == pipe.connector_keys
     ).where(
-        pipes.c.metric_key == pipe.metric_key
+        pipes_tbl.c.metric_key == pipe.metric_key
     ).where(
-        (pipes.c.location_key == pipe.location_key) if pipe.location_key is not None
-        else pipes.c.location_key.is_(None)
+        (pipes_tbl.c.location_key == pipe.location_key) if pipe.location_key is not None
+        else pipes_tbl.c.location_key.is_(None)
     )
     _id = self.value(query, debug=debug, silent=pipe.temporary)
     if _id is not None:
         _id = int(_id)
     return _id
 
 
@@ -997,18 +936,18 @@
     from meerschaum.connectors.sql.tables import get_tables
     from meerschaum.utils.packages import attempt_import
     sqlalchemy = attempt_import('sqlalchemy')
 
     if pipe.get_id(debug=debug) is None:
         return {}
 
-    pipes = get_tables(mrsm_instance=self, create=(not pipe.temporary), debug=debug)['pipes']
+    pipes_tbl = get_tables(mrsm_instance=self, create=(not pipe.temporary), debug=debug)['pipes']
 
     try:
-        q = sqlalchemy.select(pipes).where(pipes.c.pipe_id == pipe.id)
+        q = sqlalchemy.select(pipes_tbl).where(pipes_tbl.c.pipe_id == pipe.id)
         if debug:
             dprint(q)
         attributes = (
             dict(self.exec(q, silent=True, debug=debug).first()._mapping)
             if self.flavor != 'duckdb'
             else self.read(q, debug=debug).to_dict(orient='records')[0]
         )
@@ -1410,19 +1349,20 @@
         return True, f"Inserted {new_count}, updated 0 rows."
 
 
     backtrack_queries = []
     drop_backtrack_query = f"DROP TABLE {backtrack_table_name}"
     if table_exists(backtrack_table_raw, self, debug=debug):
         backtrack_queries.append(drop_backtrack_query)
+    btm = max(self.get_pipe_backtrack_minutes(pipe), 1)
     backtrack_def = self.get_pipe_data_query(
         pipe,
         begin = begin,
         end = end,
-        begin_add_minutes = -1,
+        begin_add_minutes = (-1 * btm),
         end_add_minutes = 1,
         params = params,
         debug = debug,
         order = None,
     )
 
     create_backtrack_query = (
```

### Comparing `meerschaum-1.6.9/meerschaum/connectors/sql/_plugins.py` & `meerschaum-1.7.0.dev1/meerschaum/connectors/sql/_plugins.py`

 * *Files 25% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     ) -> SuccessTuple:
     """Register a new plugin to the plugins table."""
     from meerschaum.utils.warnings import warn, error
     from meerschaum.utils.packages import attempt_import
     sqlalchemy = attempt_import('sqlalchemy')
     from meerschaum.utils.sql import json_flavors
     from meerschaum.connectors.sql.tables import get_tables
-    plugins = get_tables(mrsm_instance=self, debug=debug)['plugins']
+    plugins_tbl = get_tables(mrsm_instance=self, debug=debug)['plugins']
 
     old_id = self.get_plugin_id(plugin, debug=debug)
 
     ### Check for version conflict. May be overridden with `--force`.
     if old_id is not None and not force:
         old_version = self.get_plugin_version(plugin, debug=debug)
         new_version = plugin.version
@@ -53,20 +53,20 @@
         'attributes' : (
             json.dumps(plugin.attributes) if self.flavor not in json_flavors else plugin.attributes
         ),
         'user_id' : plugin.user_id,
     }
 
     if old_id is None:
-        query = sqlalchemy.insert(plugins).values(**bind_variables)
+        query = sqlalchemy.insert(plugins_tbl).values(**bind_variables)
     else:
         query = (
-            sqlalchemy.update(plugins)
+            sqlalchemy.update(plugins_tbl)
             .values(**bind_variables)
-            .where(plugins.c.plugin_id == old_id)
+            .where(plugins_tbl.c.plugin_id == old_id)
         )
 
     result = self.exec(query, debug=debug)
     if result is None:
         return False, f"Failed to register plugin '{plugin}'."
     return True, f"Successfully registered plugin '{plugin}'."
 
@@ -76,19 +76,23 @@
         debug: bool = False
     ) -> Optional[int]:
     """
     Return a plugin's ID.
     """
     ### ensure plugins table exists
     from meerschaum.connectors.sql.tables import get_tables
-    plugins = get_tables(mrsm_instance=self, debug=debug)['plugins']
+    plugins_tbl = get_tables(mrsm_instance=self, debug=debug)['plugins']
     from meerschaum.utils.packages import attempt_import
     sqlalchemy = attempt_import('sqlalchemy')
 
-    query = sqlalchemy.select(plugins.c.plugin_id).where(plugins.c.plugin_name == plugin.name)
+    query = (
+        sqlalchemy
+        .select(plugins_tbl.c.plugin_id)
+        .where(plugins_tbl.c.plugin_name == plugin.name)
+    )
     
     try:
         return int(self.value(query, debug=debug))
     except Exception as e:
         return None
 
 def get_plugin_version(
@@ -97,37 +101,41 @@
         debug: bool = False
     ) -> Optional[str]:
     """
     Return a plugin's version.
     """
     ### ensure plugins table exists
     from meerschaum.connectors.sql.tables import get_tables
-    plugins = get_tables(mrsm_instance=self, debug=debug)['plugins']
+    plugins_tbl = get_tables(mrsm_instance=self, debug=debug)['plugins']
     from meerschaum.utils.packages import attempt_import
     sqlalchemy = attempt_import('sqlalchemy')
 
-    query = sqlalchemy.select(plugins.c.version).where(plugins.c.plugin_name == plugin.name)
+    query = sqlalchemy.select(plugins_tbl.c.version).where(plugins_tbl.c.plugin_name == plugin.name)
 
     return self.value(query, debug=debug)
 
 def get_plugin_user_id(
         self,
         plugin: 'meerschaum.core.Plugin',
         debug: bool = False
     ) -> Optional[int]:
     """
     Return a plugin's user ID.
     """
     ### ensure plugins table exists
     from meerschaum.connectors.sql.tables import get_tables
-    plugins = get_tables(mrsm_instance=self, debug=debug)['plugins']
+    plugins_tbl = get_tables(mrsm_instance=self, debug=debug)['plugins']
     from meerschaum.utils.packages import attempt_import
     sqlalchemy = attempt_import('sqlalchemy')
 
-    query = sqlalchemy.select(plugins.c.user_id).where(plugins.c.plugin_name == plugin.name)
+    query = (
+        sqlalchemy
+        .select(plugins_tbl.c.user_id)
+        .where(plugins_tbl.c.plugin_name == plugin.name)
+    )
 
     try:
         return int(self.value(query, debug=debug))
     except Exception as e:
         return None
 
 def get_plugin_username(
@@ -136,24 +144,24 @@
         debug: bool = False
     ) -> Optional[str]:
     """
     Return the username of a plugin's owner.
     """
     ### ensure plugins table exists
     from meerschaum.connectors.sql.tables import get_tables
-    plugins = get_tables(mrsm_instance=self, debug=debug)['plugins']
+    plugins_tbl = get_tables(mrsm_instance=self, debug=debug)['plugins']
     users = get_tables(mrsm_instance=self, debug=debug)['users']
     from meerschaum.utils.packages import attempt_import
     sqlalchemy = attempt_import('sqlalchemy')
 
     query = (
         sqlalchemy.select(users.c.username)
         .where(
-            users.c.user_id == plugins.c.user_id
-            and plugins.c.plugin_name == plugin.name
+            users.c.user_id == plugins_tbl.c.user_id
+            and plugins_tbl.c.plugin_name == plugin.name
         )
     )
 
     return self.value(query, debug=debug)
 
 
 def get_plugin_attributes(
@@ -163,19 +171,23 @@
     ) -> Dict[str, Any]:
     """
     Return the attributes of a plugin.
     """
     ### ensure plugins table exists
     from meerschaum.connectors.sql.tables import get_tables
     import json
-    plugins = get_tables(mrsm_instance=self, debug=debug)['plugins']
+    plugins_tbl = get_tables(mrsm_instance=self, debug=debug)['plugins']
     from meerschaum.utils.packages import attempt_import
     sqlalchemy = attempt_import('sqlalchemy')
 
-    query = sqlalchemy.select(plugins.c.attributes).where(plugins.c.plugin_name == plugin.name)
+    query = (
+        sqlalchemy
+        .select(plugins_tbl.c.attributes)
+        .where(plugins_tbl.c.plugin_name == plugin.name)
+    )
 
     _attr = self.value(query, debug=debug)
     if isinstance(_attr, str):
         _attr = json.loads(_attr)
     elif _attr is None:
         _attr = {}
     return _attr
@@ -201,23 +213,23 @@
 
     Returns
     -------
     A list of plugin names.
     """
     ### ensure plugins table exists
     from meerschaum.connectors.sql.tables import get_tables
-    plugins = get_tables(mrsm_instance=self, debug=debug)['plugins']
+    plugins_tbl = get_tables(mrsm_instance=self, debug=debug)['plugins']
     from meerschaum.utils.packages import attempt_import
     sqlalchemy = attempt_import('sqlalchemy')
 
-    query = sqlalchemy.select(plugins.c.plugin_name)
+    query = sqlalchemy.select(plugins_tbl.c.plugin_name)
     if user_id is not None:
-        query = query.where(plugins.c.user_id == user_id)
+        query = query.where(plugins_tbl.c.user_id == user_id)
     if search_term is not None:
-        query = query.where(plugins.c.plugin_name.like(search_term + '%'))
+        query = query.where(plugins_tbl.c.plugin_name.like(search_term + '%'))
 
     return [row[0] for row in self.execute(query).fetchall()]
 
 
 def delete_plugin(
         self,
         plugin: 'meerschaum.core.Plugin',
@@ -225,23 +237,22 @@
         **kw: Any
     ) -> SuccessTuple:
     """Delete a plugin from the plugins table."""
     from meerschaum.utils.warnings import warn, error
     from meerschaum.utils.packages import attempt_import
     sqlalchemy = attempt_import('sqlalchemy')
     from meerschaum.connectors.sql.tables import get_tables
-    plugins = get_tables(mrsm_instance=self, debug=debug)['plugins']
+    plugins_tbl = get_tables(mrsm_instance=self, debug=debug)['plugins']
 
     plugin_id = self.get_plugin_id(plugin, debug=debug)
     if plugin_id is None:
         return True, f"Plugin '{plugin}' was not registered."
 
     bind_variables = {
         'plugin_id' : plugin_id,
     }
 
-    query = sqlalchemy.delete(plugins).where(plugins.c.plugin_id == plugin_id)
+    query = sqlalchemy.delete(plugins_tbl).where(plugins_tbl.c.plugin_id == plugin_id)
     result = self.exec(query, debug=debug)
     if result is None:
         return False, f"Failed to delete plugin '{plugin}'."
     return True, f"Successfully deleted plugin '{plugin}'."
-
```

### Comparing `meerschaum-1.6.9/meerschaum/connectors/sql/_sql.py` & `meerschaum-1.7.0.dev1/meerschaum/connectors/sql/_sql.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,15 +140,15 @@
     if chunksize is not None and self.flavor in _disallow_chunks_flavors:
         chunksize = None
 
     if debug:
         import time
         start = time.perf_counter()
         dprint(query_or_table)
-        dprint(f"Fetching with chunksize: {chunksize}")
+        dprint(f"[{self}] Fetching with chunksize: {chunksize}")
 
     ### This might be sqlalchemy object or the string of a table name.
     ### We check for spaces and quotes to see if it might be a weird table.
     if (
         ' ' not in str(query_or_table)
         or (
             ' ' in str(query_or_table)
@@ -161,15 +161,15 @@
             warn(
                 f"Table '{name}' is too long for '{self.flavor}',"
                 + f" will instead create the table '{truncated_name}'."
             )
 
         query_or_table = sql_item_name(str(query_or_table), self.flavor)
         if debug:
-            dprint(f"Reading from table {query_or_table}")
+            dprint(f"[{self}] Reading from table {query_or_table}")
         formatted_query = sqlalchemy.text("SELECT * FROM " + str(query_or_table))
     else:
         try:
             formatted_query = sqlalchemy.text(query_or_table)
         except Exception as e:
             formatted_query = query_or_table
 
@@ -440,15 +440,15 @@
             debug = debug,
             **kw
         )
 
     from meerschaum.utils.packages import attempt_import
     sqlalchemy = attempt_import("sqlalchemy")
     if debug:
-        dprint("Executing query:\n" + f"{query}")
+        dprint(f"[{self}] Executing query:\n{query}")
 
     _close = close if close is not None else (self.flavor != 'mssql')
     _commit = commit if commit is not None else (
         (self.flavor != 'mssql' or 'select' not in str(query).lower())
     )
 
     ### Select and Insert objects need to be compiled (SQLAlchemy 2.0.0+).
@@ -459,15 +459,15 @@
     transaction = connection.begin() if _commit else None
     try:
         result = connection.execute(query, *args, **kw)
         if _commit:
             transaction.commit()
     except Exception as e:
         if debug:
-            dprint(f"Failed to execute query:\n\n{query}\n\n{e}")
+            dprint(f"[{self}] Failed to execute query:\n\n{query}\n\n{e}")
         if not silent:
             warn(str(e))
         result = None
         if _commit:
             transaction.rollback()
     finally:
         if _close:
@@ -509,26 +509,26 @@
     from meerschaum.utils.packages import attempt_import
     sqlalchemy = attempt_import('sqlalchemy')
 
     results = []
     with self.engine.begin() as connection:
         for query in queries:
             if debug:
-                dprint(query)
+                dprint(f"[{self}]\n" + str(query))
             if isinstance(query, str):
                 query = sqlalchemy.text(query)
 
             try:
                 result = connection.execute(query)
             except Exception as e:
                 msg = (f"Encountered error while executing:\n{e}")
                 if not silent:
                     warn(msg)
                 elif debug:
-                    dprint(msg)
+                    dprint(f"[{self}]\n" + str(msg))
                 result = None
             results.append(result)
             if result is None and break_on_error:
                 break
     return results
 
 
@@ -624,15 +624,15 @@
                 )
             chunksize = _max_chunks_flavors[self.flavor]
     stats['chunksize'] = chunksize
 
     success, msg = False, "Default to_sql message"
     start = time.perf_counter()
     if debug:
-        msg = f"Inserting {len(df)} rows with chunksize: {chunksize}..."
+        msg = f"[{self}] Inserting {len(df)} rows with chunksize: {chunksize}..."
         print(msg, end="", flush=True)
     stats['num_rows'] = len(df)
 
     ### filter out non-pandas args
     import inspect
     to_sql_params = inspect.signature(df.to_sql).parameters
     to_sql_kw = {}
@@ -750,20 +750,20 @@
     from meerschaum.utils.sql import sql_item_name
 
     ### NOTE: PostgreSQL doesn't support NUL chars in text, so they're removed from strings.
     data_iter = (
         (
             (
                 (
-                    json.dumps(item).replace('\0', '')
+                    json.dumps(item).replace('\0', '').replace('\\u0000', '')
                     if isinstance(item, (dict, list))
                     else (
                         item
                         if not isinstance(item, str)
-                        else item.replace('\0', '')
+                        else item.replace('\0', '').replace('\\u0000', '')
                     )
                 )
             ) if item is not None
             else r'\N'
             for item in row
         ) for row in data_iter
     )
```

### Comparing `meerschaum-1.6.9/meerschaum/connectors/sql/_uri.py` & `meerschaum-1.7.0.dev1/meerschaum/connectors/sql/_uri.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/connectors/sql/_users.py` & `meerschaum-1.7.0.dev1/meerschaum/connectors/sql/_users.py`

 * *Files 7% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         **kw: Any
     ) -> SuccessTuple:
     """Update an existing user's metadata."""
     from meerschaum.utils.packages import attempt_import
     sqlalchemy = attempt_import('sqlalchemy')
     from meerschaum.connectors.sql.tables import get_tables
     from meerschaum.utils.sql import json_flavors
-    users = get_tables(mrsm_instance=self, debug=debug)['users']
+    users_tbl = get_tables(mrsm_instance=self, debug=debug)['users']
 
     user_id = user.user_id if user.user_id is not None else self.get_user_id(user, debug=debug)
     if user_id is None:
         return False, (
             f"User '{user.username}' does not exist. " +
             f"Register user '{user.username}' before editing."
         )
@@ -129,15 +129,20 @@
         bind_variables['attributes'] = (
             json.dumps(user.attributes) if self.flavor in ('duckdb',)
             else user.attributes
         )
     if user.type != '':
         bind_variables['user_type'] = user.type
 
-    query = sqlalchemy.update(users).values(**bind_variables).where(users.c.user_id == user_id)
+    query = (
+        sqlalchemy
+        .update(users_tbl)
+        .values(**bind_variables)
+        .where(users_tbl.c.user_id == user_id)
+    )
 
     result = self.exec(query, debug=debug)
     if result is None:
         return False, f"Failed to edit user '{user}'."
     return True, f"Successfully edited user '{user}'."
 
 def get_user_id(
@@ -146,19 +151,19 @@
         debug : bool = False
     ) -> Optional[int]:
     """If a user is registered, return the `user_id`."""
     ### ensure users table exists
     from meerschaum.utils.packages import attempt_import
     sqlalchemy = attempt_import('sqlalchemy')
     from meerschaum.connectors.sql.tables import get_tables
-    users = get_tables(mrsm_instance=self, debug=debug)['users']
+    users_tbl = get_tables(mrsm_instance=self, debug=debug)['users']
 
     query = (
-        sqlalchemy.select(users.c.user_id)
-        .where(users.c.username == user.username)
+        sqlalchemy.select(users_tbl.c.user_id)
+        .where(users_tbl.c.username == user.username)
     )
 
     result = self.value(query, debug=debug)
     if result is not None:
         return int(result)
     return None
 
@@ -171,21 +176,21 @@
     Return the user's attributes.
     """
     ### ensure users table exists
     from meerschaum.utils.warnings import warn
     from meerschaum.utils.packages import attempt_import
     sqlalchemy = attempt_import('sqlalchemy')
     from meerschaum.connectors.sql.tables import get_tables
-    users = get_tables(mrsm_instance=self, debug=debug)['users']
+    users_tbl = get_tables(mrsm_instance=self, debug=debug)['users']
 
     user_id = user.user_id if user.user_id is not None else self.get_user_id(user, debug=debug)
 
     query = (
-        sqlalchemy.select(users.c.attributes).
-        where(users.c.user_id == user_id)
+        sqlalchemy.select(users_tbl.c.attributes)
+        .where(users_tbl.c.user_id == user_id)
     )
 
     result = self.value(query, debug=debug)
     if result is not None and not isinstance(result, dict):
         try:
             result = dict(result)
             _parsed = True
@@ -206,25 +211,25 @@
         self,
         user: meerschaum.core.User,
         debug: bool = False
     ) -> SuccessTuple:
     """Delete a user's record from the users table."""
     ### ensure users table exists
     from meerschaum.connectors.sql.tables import get_tables
-    users = get_tables(mrsm_instance=self, debug=debug)['users']
+    users_tbl = get_tables(mrsm_instance=self, debug=debug)['users']
     plugins = get_tables(mrsm_instance=self, debug=debug)['plugins']
     from meerschaum.utils.packages import attempt_import
     sqlalchemy = attempt_import('sqlalchemy')
 
     user_id = user.user_id if user.user_id is not None else self.get_user_id(user, debug=debug)
 
     if user_id is None:
         return False, f"User '{user.username}' is not registered and cannot be deleted."
 
-    query = sqlalchemy.delete(users).where(users.c.user_id == user_id)
+    query = sqlalchemy.delete(users_tbl).where(users_tbl.c.user_id == user_id)
 
     result = self.exec(query, debug=debug)
     if result is None:
         return False, f"Failed to delete user '{user}'."
 
     query = sqlalchemy.delete(plugins).where(plugins.c.user_id == user_id)
     result = self.exec(query, debug=debug)
@@ -239,19 +244,19 @@
         **kw: Any
     ) -> List[str]:
     """
     Get the registered usernames.
     """
     ### ensure users table exists
     from meerschaum.connectors.sql.tables import get_tables
-    users = get_tables(mrsm_instance=self, debug=debug)['users']
+    users_tbl = get_tables(mrsm_instance=self, debug=debug)['users']
     from meerschaum.utils.packages import attempt_import
     sqlalchemy = attempt_import('sqlalchemy')
 
-    query = sqlalchemy.select(users.c.username)
+    query = sqlalchemy.select(users_tbl.c.username)
 
     return list(self.read(query, debug=debug)['username'])
 
 def get_user_password_hash(
         self,
         user: meerschaum.core.User,
         debug: bool = False,
@@ -259,15 +264,15 @@
     ) -> Optional[str]:
     """
     Return the password has for a user.
     **NOTE**: This may be dangerous and is only allowed if the security settings explicity allow it.
     """
     from meerschaum.utils.debug import dprint
     from meerschaum.connectors.sql.tables import get_tables
-    users = get_tables(mrsm_instance=self, debug=debug)['users']
+    users_tbl = get_tables(mrsm_instance=self, debug=debug)['users']
     from meerschaum.utils.packages import attempt_import
     sqlalchemy = attempt_import('sqlalchemy')
 
     if user.user_id is not None:
         user_id = user.user_id
         if debug:
             dprint(f"Already given user_id: {user_id}")
@@ -275,33 +280,33 @@
         if debug:
             dprint(f"Fetching user_id...")
         user_id = self.get_user_id(user, debug=debug)
 
     if user_id is None:
         return None
 
-    query = sqlalchemy.select(users.c.password_hash).where(users.c.user_id == user_id)
+    query = sqlalchemy.select(users_tbl.c.password_hash).where(users_tbl.c.user_id == user_id)
 
     return self.value(query, debug=debug)
 
 def get_user_type(
         self,
         user: meerschaum.core.User,
         debug: bool = False,
         **kw: Any
     ) -> Optional[str]:
     """
     Return the user's type.
     """
     from meerschaum.connectors.sql.tables import get_tables
-    users = get_tables(mrsm_instance=self, debug=debug)['users']
+    users_tbl = get_tables(mrsm_instance=self, debug=debug)['users']
     from meerschaum.utils.packages import attempt_import
     sqlalchemy = attempt_import('sqlalchemy')
 
     user_id = user.user_id if user.user_id is not None else self.get_user_id(user, debug=debug)
 
     if user_id is None:
         return None
 
-    query = sqlalchemy.select(users.c.user_type).where(users.c.user_id == user_id)
+    query = sqlalchemy.select(users_tbl.c.user_type).where(users_tbl.c.user_id == user_id)
 
     return self.value(query, debug=debug)
```

### Comparing `meerschaum-1.6.9/meerschaum/connectors/sql/tables/__init__.py` & `meerschaum-1.7.0.dev1/meerschaum/connectors/sql/tables/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,15 +163,15 @@
             create_tables(conn, tables=_tables)
 
     return connector_tables[conn]
 
 
 def create_tables(
         conn: 'meerschaum.connectors.SQLConnector',
-        tables: Optional[Dict[str, 'sqlalchemy.Table']],
+        tables: Optional[Dict[str, 'sqlalchemy.Table']] = None,
     ) -> bool:
     """
     Create the tables on the database.
     """
     from meerschaum.utils.warnings import warn
     _tables = tables if tables is not None else get_tables(conn)
     try:
```

### Comparing `meerschaum-1.6.9/meerschaum/connectors/sql/tables/types.py` & `meerschaum-1.7.0.dev1/meerschaum/connectors/sql/tables/types.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/core/Pipe/__init__.py` & `meerschaum-1.7.0.dev1/meerschaum/core/Pipe/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/core/Pipe/_attributes.py` & `meerschaum-1.7.0.dev1/meerschaum/core/Pipe/_attributes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/core/Pipe/_bootstrap.py` & `meerschaum-1.7.0.dev1/meerschaum/core/Pipe/_bootstrap.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/core/Pipe/_clear.py` & `meerschaum-1.7.0.dev1/meerschaum/core/Pipe/_clear.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/core/Pipe/_data.py` & `meerschaum-1.7.0.dev1/meerschaum/core/Pipe/_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -122,24 +122,29 @@
         fresh: bool = False,
         debug: bool = False,
         **kw: Any
     ) -> Generator['pd.DataFrame']:
     """
     Return a pipe's data as a generator.
     """
+    from meerschaum.config import get_config
     from meerschaum.utils.misc import round_time
     parse_begin = isinstance(begin, str)
     parse_end = isinstance(end, str)
     if parse_begin or parse_end:
         from meerschaum.utils.packages import attempt_import
         dateutil_parser = attempt_import('dateutil.parser')
     if parse_begin:
         begin = dateutil_parser.parse(begin)
     if parse_end:
         end = dateutil_parser.parse(end)
+
+    if not self.exists(debug=debug):
+        return
+
     _ = kw.pop('as_chunks', None)
     _ = kw.pop('as_iterator', None)
     min_dt = (
         begin if begin is not None
         else self.get_sync_time(round_down=False, newest=False, params=params, debug=debug)
     )
     max_dt = (
@@ -157,32 +162,30 @@
     if chunk_interval is None:
         chunk_interval = (
             get_config('system', 'connectors', 'sql', 'chunksize')
             if isinstance(min_dt, int)
             else datetime.timedelta(days=1)
         )
 
-
     ### If we can't determine bounds
     ### or if chunk_interval exceeds the max,
     ### return a single chunk.
     if (
         (min_dt is None and max_dt is None)
         or
         (min_dt + chunk_interval) > max_dt
     ):
-        return (
-            self.get_data(
-                begin = begin,
-                end = end,
-                params = params,
-                fresh = fresh,
-                debug = debug,
-            ) for i in range(1)
+        yield self.get_data(
+            begin = begin,
+            end = end,
+            params = params,
+            fresh = fresh,
+            debug = debug,
         )
+        return
 
     chunk_begin = min_dt
     chunk_end = min_dt + chunk_interval
     while chunk_end < max_dt:
         yield self.get_data(
             begin = chunk_begin,
             end = chunk_end,
@@ -203,30 +206,35 @@
         )
 
 
 def get_backtrack_data(
         self,
         backtrack_minutes: int = 0,
         begin: Optional['datetime.datetime'] = None,
+        params: Optional[Dict[str, Any]] = None,
         fresh: bool = False,
         debug: bool = False,
         **kw: Any
     ) -> Optional['pd.DataFrame']:
     """
     Get the most recent data from the instance connector as a Pandas DataFrame.
 
     Parameters
     ----------
     backtrack_minutes: int, default 0
         How many minutes from `begin` to select from.
         Defaults to 0. This may return a few rows due to a rounding quirk.
+
     begin: Optional[datetime.datetime], default None
         The starting point to search for data.
         If begin is `None` (default), use the most recent observed datetime
         (AKA sync_time).
+
+    params: Optional[Dict[str, Any]], default None
+        The standard Meerschaum `params` query dictionary.
         
         
     ```
     E.g. begin = 02:00
 
     Search this region.           Ignore this, even if there's data.
     /  /  /  /  /  /  /  /  /  |
@@ -248,41 +256,67 @@
     is a convenient way to get a pipe's data "backtracked" from the most recent datetime.
 
     """
     from meerschaum.utils.warnings import warn
     from meerschaum.utils.venv import Venv
     from meerschaum.connectors import get_connector_plugin
 
-    kw.update({'backtrack_minutes': backtrack_minutes, 'begin': begin,})
-
     if not self.exists(debug=debug):
         return None
 
     if self.cache_pipe is not None:
         if not fresh:
-            _sync_cache_tuple = self.cache_pipe.sync(debug=debug, **kw)
+            _sync_cache_tuple = self.cache_pipe.sync(begin=begin, params=params, debug=debug, **kw)
             if not _sync_cache_tuple[0]:
                 warn(f"Failed to sync cache for {self}:\n" + _sync_cache_tuple[1])
                 fresh = True
             else: ### Successfully synced cache.
                 return self.enforce_dtypes(
-                    self.cache_pipe.get_backtrack_data(debug=debug, fresh=True, **kw),
+                    self.cache_pipe.get_backtrack_data(
+                        fresh = True,
+                        begin = begin,
+                        backtrack_minutes = backtrack_minutes,
+                        params = params,
+                        debug = deubg,
+                        **kw
+                    ),
                     debug = debug,
                 )
 
-    ### If `fresh` or the syncing failed, directly pull from the instance connector.
-    with Venv(get_connector_plugin(self.instance_connector)):
-        return self.enforce_dtypes(
-            self.instance_connector.get_backtrack_data(
-                pipe = self,
+    if hasattr(self.instance_connector, 'get_backtrack_data'):
+        with Venv(get_connector_plugin(self.instance_connector)):
+            return self.enforce_dtypes(
+                self.instance_connector.get_backtrack_data(
+                    pipe = self,
+                    begin = begin,
+                    backtrack_minutes = backtrack_minutes,
+                    params = params,
+                    debug = debug,
+                    **kw
+                ),
                 debug = debug,
-                **kw
-            ),
-            debug = debug,
-        )
+            )
+
+    if begin is None:
+        begin = self.get_sync_time(params=params, debug=debug)
+
+    backtrack_interval = (
+        datetime.timedelta(minutes=backtrack_minutes)
+        if isinstance(begin, datetime.datetime)
+        else backtrack_minutes
+    )
+    if begin is not None:
+        begin = begin - backtrack_interval
+
+    return self.get_data(
+        begin = begin,
+        params = params,
+        debug = debug,
+        **kw
+    )
 
 
 def get_rowcount(
         self,
         begin: Optional['datetime.datetime'] = None,
         end: Optional['datetime.datetime'] = None,
         remote: bool = False,
```

### Comparing `meerschaum-1.6.9/meerschaum/core/Pipe/_delete.py` & `meerschaum-1.7.0.dev1/meerschaum/core/Pipe/_delete.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/core/Pipe/_drop.py` & `meerschaum-1.7.0.dev1/meerschaum/core/Pipe/_drop.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/core/Pipe/_dtypes.py` & `meerschaum-1.7.0.dev1/meerschaum/core/Pipe/_dtypes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/core/Pipe/_edit.py` & `meerschaum-1.7.0.dev1/meerschaum/core/Pipe/_edit.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/core/Pipe/_fetch.py` & `meerschaum-1.7.0.dev1/meerschaum/core/Pipe/_fetch.py`

 * *Files 7% similar despite different names*

```diff
@@ -73,14 +73,19 @@
             kwargs = apply_patch_to_config(kw, _kw)
             chunk_success, chunk_message = self.sync(chunk, **kwargs)
             chunk_label = self._get_chunk_label(chunk, self.columns.get('datetime', None))
             if chunk_label:
                 chunk_message = '\n' + chunk_label + '\n' + chunk_message
             return chunk_success, chunk_message
 
+    workers = kw.get('workers', None)
+    if workers is None and not getattr(self.instance_connector, 'IS_THREAD_SAFE', False):
+        workers = 1
+    kw['workers'] = workers
+
     df = self.connector.fetch(
         self,
         begin = begin,
         end = end,
         chunk_hook = _chunk_hook,
         debug = debug,
         **kw
```

### Comparing `meerschaum-1.6.9/meerschaum/core/Pipe/_register.py` & `meerschaum-1.7.0.dev1/meerschaum/core/Pipe/_register.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/core/Pipe/_show.py` & `meerschaum-1.7.0.dev1/meerschaum/core/Pipe/_show.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/core/Pipe/_sync.py` & `meerschaum-1.7.0.dev1/meerschaum/core/Pipe/_sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,21 @@
 """
 Synchronize a pipe's data with its source via its connector
 """
 
 from __future__ import annotations
 
 import json
+import datetime
+import time
+import threading
+
 from meerschaum.utils.typing import (
-    Union, Optional, Callable, Any, Tuple, SuccessTuple, Mapping, Dict, List, Iterable, Generator
+    Union, Optional, Callable, Any, Tuple, SuccessTuple, Mapping, Dict, List, Iterable, Generator,
+    Iterator,
 )
 
 class InferFetch:
     MRSM_INFER_FETCH: bool = True
 
 def sync(
         self,
@@ -112,18 +117,18 @@
     from meerschaum.utils.debug import dprint, _checkpoint
     from meerschaum.utils.warnings import warn, error
     from meerschaum.connectors import custom_types
     from meerschaum.plugins import Plugin
     from meerschaum.utils.formatting import get_console
     from meerschaum.utils.venv import Venv
     from meerschaum.connectors import get_connector_plugin
-
+    from meerschaum.utils.misc import df_is_chunk_generator
+    from meerschaum.utils.pool import get_pool
     from meerschaum.config import get_config
-    import datetime
-    import time
+
     if (callback is not None or error_callback is not None) and blocking:
         warn("Callback functions are only executed when blocking = False. Ignoring...")
 
     _checkpoint(_total=2, **kw)
 
     if chunksize == 0:
         chunksize = None
@@ -260,33 +265,37 @@
                 p._exists = None
                 return True, f"{p} is being synced in parallel."
 
         ### CHECKPOINT: Retrieved the DataFrame.
         _checkpoint(**kw)
         
         ### Allow for dataframe generators or iterables.
-        if (
-            not isinstance(df, (dict, list, str))
-            and 'DataFrame' not in str(type(df))
-            and isinstance(df, (Generator, Iterable))
-        ):
-            from meerschaum.utils.pool import get_pool
-            import threading
-            engine_pool_size = (
-                p.instance_connector.engine.pool.size()
-                if p.instance_connector.type == 'sql'
-                else 1
-            )
-            current_num_threads = len(threading.enumerate())
-            workers = kw.get('workers', None)
-            desired_workers = min(workers or engine_pool_size, engine_pool_size)
-            kw['workers'] = max(
-                (desired_workers - current_num_threads),
-                1,
-            )
+        if df_is_chunk_generator(df):
+            is_thread_safe = getattr(self.instance_connector, 'IS_THREAD_SAFE', False)
+            if is_thread_safe:
+                engine_pool_size = (
+                    p.instance_connector.engine.pool.size()
+                    if p.instance_connector.type == 'sql'
+                    else None
+                )
+                current_num_threads = len(threading.enumerate())
+                workers = kw.get('workers', None)
+                desired_workers = (
+                    min(workers or engine_pool_size, engine_pool_size)
+                    if engine_pool_size is not None
+                    else (workers if is_thread_safe else 1)
+                )
+                if desired_workers is None:
+                    desired_workers = (current_num_threads if is_thread_safe else 1)
+                kw['workers'] = max(
+                    (desired_workers - current_num_threads),
+                    1,
+                )
+            else:
+                kw['workers'] = 1
 
             dt_col = p.columns.get('datetime', None)
 
 
             pool = get_pool(workers=kw.get('workers', 1))
             if debug:
                 dprint(f"Received {type(df)}. Attempting to sync first chunk...")
@@ -305,37 +314,50 @@
             def _process_chunk(_chunk):
                 try:
                     _chunk_success, _chunk_msg = _sync(p, _chunk)
                 except Exception as e:
                     _chunk_success, _chunk_msg = False, str(e)
                 if not _chunk_success:
                     failed_chunks.append(_chunk)
-                return _chunk_success, '\n' + self._get_chunk_label(_chunk, dt_col) + '\n' + _chunk_msg
+                return (
+                    _chunk_success,
+                    (
+                        '\n'
+                        + self._get_chunk_label(_chunk, dt_col)
+                        + '\n'
+                        + _chunk_msg
+                    )
+                )
 
 
             results = sorted(
-                [(chunk_success, chunk_msg)] + list(pool.imap(_process_chunk, df))
+                [(chunk_success, chunk_msg)] + (
+                    list(pool.imap(_process_chunk, df))
+                    if not df_is_chunk_generator(chunk)
+                    else [
+                        _process_chunk(_child_chunks)
+                        for _child_chunks in df
+                    ]
+                )
             )
             chunk_messages = [chunk_msg for _, chunk_msg in results]
             success_bools = [chunk_success for chunk_success, _ in results]
-            failure_indices = [
-                i for i, _success_bool in enumerate(success_bools)
-                if not _success_bool
-            ]
             success = all(success_bools)
             msg = '\n'.join(chunk_messages)
 
             ### If some chunks succeeded, retry the failures.
             retry_success = True
             if not success and any(success_bools):
                 if debug:
                     dprint(f"Retrying failed chunks...")
-                for chunk in failed_chunks:
+                chunks_to_retry = [c for c in failed_chunks]
+                failed_chunks = []
+                for chunk in chunks_to_retry:
                     chunk_success, chunk_msg = _process_chunk(chunk)
-                    msg += f"\nRetried chunk:\n{chunk_msg}"
+                    msg += f"\n\nRetried chunk:\n{chunk_msg}\n"
                     retry_success = retry_success and chunk_success
 
             success = success and retry_success
             return success, msg
 
         ### Cast to a dataframe and ensure datatypes are what we expect.
         df = self.enforce_dtypes(df, debug=debug)
```

### Comparing `meerschaum-1.6.9/meerschaum/core/User/_User.py` & `meerschaum-1.7.0.dev1/meerschaum/core/User/_User.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/plugins/_Plugin.py` & `meerschaum-1.7.0.dev1/meerschaum/plugins/_Plugin.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/plugins/__init__.py` & `meerschaum-1.7.0.dev1/meerschaum/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/utils/daemon/Daemon.py` & `meerschaum-1.7.0.dev1/meerschaum/utils/daemon/Daemon.py`

 * *Files 5% similar despite different names*

```diff
@@ -328,26 +328,15 @@
             process.wait(timeout=10)
         except Exception as e:
             return False, f"Failed to kill job {self} with exception: {e}"
         return True, "Success"
 
 
     def quit(self, timeout: Optional[int] = 3) -> SuccessTuple:
-        """Gracefully quit a running daemon.
-        Sends a SIGINT signal the to process.
-
-        Parameters
-        ----------
-        timeout: Optional[int] :
-             (Default value = 3)
-
-        Returns
-        -------
-
-        """
+        """Gracefully quit a running daemon."""
         daemoniker, psutil = attempt_import('daemoniker', 'psutil')
         return self._send_signal(daemoniker.SIGINT, timeout=timeout)
 
     def _send_signal(
             self,
             signal,
             timeout: Optional[Union[float, int]] = 3,
@@ -392,30 +381,20 @@
             f"Failed to stop daemon '{self.daemon_id}' within {timeout} second"
             + ('s' if timeout != 1 else '') + '.'
         )
 
     @property
     def sighandler(self) -> Optional[daemoniker.SignalHandler1]:
         """
-
-        Parameters
-        ----------
-
-        Returns
-        -------
-        type
-            If the process is not running, return `None`.
-
+        If the process is not running, return `None`.
         """
-        # if not self.pid_path.exists():
-        #     return None
-
         def _quit(*args, **kw):
             from meerschaum.__main__ import _exit
             _exit()
+
         daemoniker = attempt_import('daemoniker')
         if '_sighandler' not in self.__dict__:
             self._sighandler = daemoniker.SignalHandler1(
                 str(self.pid_path.as_posix()),
                 sigint = _quit,
                 sigterm = _quit,
                 sigabrt = _quit,
```

### Comparing `meerschaum-1.6.9/meerschaum/utils/daemon/Log.py` & `meerschaum-1.7.0.dev1/meerschaum/utils/daemon/Log.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/utils/daemon/__init__.py` & `meerschaum-1.7.0.dev1/meerschaum/utils/daemon/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/utils/daemon/_names.py` & `meerschaum-1.7.0.dev1/meerschaum/utils/daemon/_names.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/utils/debug.py` & `meerschaum-1.7.0.dev1/meerschaum/utils/debug.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/utils/formatting/__init__.py` & `meerschaum-1.7.0.dev1/meerschaum/utils/formatting/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/utils/formatting/_jobs.py` & `meerschaum-1.7.0.dev1/meerschaum/utils/formatting/_jobs.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/utils/formatting/_pipes.py` & `meerschaum-1.7.0.dev1/meerschaum/utils/formatting/_pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/utils/formatting/_pprint.py` & `meerschaum-1.7.0.dev1/meerschaum/utils/formatting/_pprint.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/utils/formatting/_shell.py` & `meerschaum-1.7.0.dev1/meerschaum/utils/formatting/_shell.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/utils/get_pipes.py` & `meerschaum-1.7.0.dev1/meerschaum/utils/get_pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/utils/interactive.py` & `meerschaum-1.7.0.dev1/meerschaum/utils/interactive.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/utils/misc.py` & `meerschaum-1.7.0.dev1/meerschaum/utils/misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 """
 Miscellaneous functions go here
 """
 
 from __future__ import annotations
 from meerschaum.utils.typing import (
     Union, Mapping, Any, Callable, Optional, List, Dict, SuccessTuple, Iterable, PipesDict, Tuple,
-    InstanceConnector, Hashable
+    InstanceConnector, Hashable, Generator, Iterator,
 )
 import meerschaum as mrsm
 
 def add_method_to_class(
         func: Callable[[Any], Any],
         class_def: 'Class',
         method_name: Optional[str] = None,
@@ -2123,14 +2123,16 @@
     """
     if not datetime_column:
         return None
 
     def compare(a, b):
         if a is None:
             return b
+        if b is None:
+            return a
         if minimum:
             return a if a < b else b
         return a if a > b else b
 
     if isinstance(df, list):
         if len(df) == 0:
             return None
@@ -2144,12 +2146,37 @@
         if datetime_column not in df:
             return None
         best_yet = df[datetime_column][0]
         for val in df[datetime_column]:
             best_yet = compare(best_yet, val)
         return best_yet
 
+    if 'DataFrame' in str(type(df)):
+        return (
+            df[datetime_column].min(skipna=True)
+            if minimum
+            else df[datetime_column].max(skipna=True)
+        )
+
+    return None
+
+
+def df_is_chunk_generator(df: Any) -> bool:
+    """
+    Determine whether to treat `df` as a chunk generator.
+
+    Note this should only be used in a context where generators are expected,
+    as it will return `True` for any iterable.
+
+    Parameters
+    ----------
+    The DataFrame or chunk generator to evaluate.
+
+    Returns
+    -------
+    A `bool` indicating whether to treat `df` as a generator.
+    """
     return (
-        df[datetime_column].min(skipna=True)
-        if minimum
-        else df[datetime_column].max(skipna=True)
+        not isinstance(df, (dict, list, str))
+        and 'DataFrame' not in str(type(df))
+        and isinstance(df, (Generator, Iterable, Iterator))
     )
```

### Comparing `meerschaum-1.6.9/meerschaum/utils/networking.py` & `meerschaum-1.7.0.dev1/meerschaum/utils/networking.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/utils/packages/__init__.py` & `meerschaum-1.7.0.dev1/meerschaum/utils/packages/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/utils/packages/_packages.py` & `meerschaum-1.7.0.dev1/meerschaum/utils/packages/_packages.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,18 +19,18 @@
 packages: Dict[str, Dict[str, str]] = {
     'required': {
     },
     'minimal': {},
     'formatting': {
         'pprintpp'                   : 'pprintpp>=0.4.0',
         'asciitree'                  : 'asciitree>=0.3.3',
-        'typing_extensions'          : 'typing_extensions>=4.4.0',
+        'typing_extensions'          : 'typing-extensions>=4.7.1',
         'pygments'                   : 'pygments>=2.7.2',
         'colorama'                   : 'colorama>=0.4.3',
-        'rich'                       : 'rich>=12.4.4',
+        'rich'                       : 'rich>=13.4.2',
         'more_termcolor'             : 'more-termcolor>=1.1.3',
         'humanfriendly'              : 'humanfriendly>=10.0.0',
     },
     '_required': {
         'wheel'                      : 'wheel>=0.34.2',
         'setuptools'                 : 'setuptools>=63.3.0',
         'yaml'                       : 'PyYAML>=5.3.1',
@@ -40,22 +40,22 @@
         'pathspec'                   : 'pathspec>=0.9.0',
         'dateutil'                   : 'python-dateutil>=2.7.5',
         'requests'                   : 'requests>=2.23.0',
         'binaryornot'                : 'binaryornot>=0.4.4',
         'pyvim'                      : 'pyvim>=3.0.2',
         'aiofiles'                   : 'aiofiles>=0.6.0',
         'packaging'                  : 'packaging>=21.3.0',
-        'prompt_toolkit'             : 'prompt-toolkit>=3.0.11',
+        'prompt_toolkit'             : 'prompt-toolkit>=3.0.39',
         'more_itertools'             : 'more-itertools>=8.7.0',
         'daemoniker'                 : 'daemoniker>=0.2.3',
         'psutil'                     : 'psutil>=5.8.0',
         'watchgod'                   : 'watchgod>=0.7.0',
         'dill'                       : 'dill>=0.3.3',
         'virtualenv'                 : 'virtualenv>=20.1.0',
-        'rocketry'                   : 'rocketry>=2.3.0',
+        'rocketry'                   : 'rocketry>=2.5.1',
     },
     'drivers': {
         'cryptography'               : 'cryptography>=38.0.1',
         'psycopg2'                   : 'psycopg2-binary>=2.8.6',
         'pymysql'                    : 'PyMySQL>=0.9.0',
         'aiomysql'                   : 'aiomysql>=0.0.21',
         'sqlalchemy_cockroachdb'     : 'sqlalchemy-cockroachdb>=2.0.0',
@@ -139,24 +139,23 @@
     'dash'                           : 'dash>=2.6.2',
     'dash_bootstrap_components'      : 'dash-bootstrap-components>=1.2.1',
     'dash_ace'                       : 'dash-ace>=0.2.1',
     'dash_extensions'                : 'dash-extensions>=0.1.6',
     'dash_daq'                       : 'dash-daq>=0.5.0',
 }
 packages['api'] = {
-    'uvicorn'                        : 'uvicorn[standard]>=0.17.5',
+    'uvicorn'                        : 'uvicorn[standard]>=0.22.0',
     'gunicorn'                       : 'gunicorn>=20.1.0',
     'dotenv'                         : 'python-dotenv>=0.20.0',
-    'websockets'                     : 'websockets>=8.1.0',
-    'fastapi'                        : 'fastapi>=0.89.0',
-    'fastapi_jwt_auth'               : 'fastapi-jwt-auth>=0.5.0',
+    'websockets'                     : 'websockets>=11.0.3',
+    'fastapi'                        : 'fastapi>=0.100.0',
     'passlib'                        : 'passlib>=1.7.4',
     'fastapi_login'                  : 'fastapi-login>=1.7.2',
     'multipart'                      : 'python-multipart>=0.0.5',
-    'pydantic'                       : 'pydantic>=1.10.2',
+    'pydantic'                       : 'pydantic>=1.7.4',
 }
 packages['api'].update(packages['sql'])
 packages['api'].update(packages['formatting'])
 packages['api'].update(packages['dash'])
 
 all_packages = {}
 for group, import_names in packages.items():
```

### Comparing `meerschaum-1.6.9/meerschaum/utils/packages/lazy_loader.py` & `meerschaum-1.7.0.dev1/meerschaum/utils/packages/lazy_loader.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/utils/pool.py` & `meerschaum-1.7.0.dev1/meerschaum/utils/pool.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/utils/process.py` & `meerschaum-1.7.0.dev1/meerschaum/utils/process.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/utils/prompt.py` & `meerschaum-1.7.0.dev1/meerschaum/utils/prompt.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/utils/schedule.py` & `meerschaum-1.7.0.dev1/meerschaum/utils/schedule.py`

 * *Files 18% similar despite different names*

```diff
@@ -26,14 +26,15 @@
         The function to execute.
 
     frequency: str
         The frequency at which `function` should be executed (e.g. `'daily'`).
 
     """
     import warnings
+    from meerschaum.utils.warnings import warn
     from meerschaum.utils.packages import attempt_import
     from meerschaum.utils.misc import filter_keywords
     from concurrent.futures._base import CancelledError
     kw['debug'] = debug
     kw = filter_keywords(function, **kw)
 
     def _wrapper():
@@ -50,7 +51,14 @@
         return app.run(debug=debug)
     except (KeyboardInterrupt, CancelledError):
         try:
             app.session.shut_down(force=True)
         except CancelledError:
             pass
         return None
+    except AttributeError:
+        warn(
+            "Failed to import scheduler.\n\n   "
+            + "Run `mrsm install package 'pydantic<2.0.0'` and try again.",
+            stack = False,
+        )
+
```

### Comparing `meerschaum-1.6.9/meerschaum/utils/sql.py` & `meerschaum-1.7.0.dev1/meerschaum/utils/sql.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/utils/threading.py` & `meerschaum-1.7.0.dev1/meerschaum/utils/threading.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/utils/typing.py` & `meerschaum-1.7.0.dev1/meerschaum/utils/typing.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
         Sequence,
         Callable,
         Union,
         Any,
         Iterable,
         Hashable,
         Generator,
+        Iterator,
     )
 except Exception as e:
     import urllib.request, sys, pathlib, os
     old_cwd = os.getcwd()
     cache_dir = pathlib.Path.home() / '.cache'
     if not cache_dir.exists():
         try:
```

### Comparing `meerschaum-1.6.9/meerschaum/utils/venv/_Venv.py` & `meerschaum-1.7.0.dev1/meerschaum/utils/venv/_Venv.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/utils/venv/__init__.py` & `meerschaum-1.7.0.dev1/meerschaum/utils/venv/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum/utils/warnings.py` & `meerschaum-1.7.0.dev1/meerschaum/utils/warnings.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,14 @@
 import warnings
 
 warnings.filterwarnings(
     "always",
     category = UserWarning
 )
 warnings.filterwarnings(
-    "ignore",
-    category = DeprecationWarning
-)
-warnings.filterwarnings(
     "always",
     category = ImportWarning
 )
 warnings.filterwarnings(
     "ignore",
     category = RuntimeWarning
 )
```

### Comparing `meerschaum-1.6.9/meerschaum/utils/yaml.py` & `meerschaum-1.7.0.dev1/meerschaum/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.9/meerschaum.egg-info/PKG-INFO` & `meerschaum-1.7.0.dev1/meerschaum.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meerschaum
-Version: 1.6.9
+Version: 1.7.0.dev1
 Summary: Sync Time-Series Pipes with Meerschaum
 Home-page: https://meerschaum.io
 Author: Bennett Meares
 Author-email: bennett.meares@gmail.com
 Maintainer-email: bennett.meares@gmail.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://docs.meerschaum.io
```

### Comparing `meerschaum-1.6.9/meerschaum.egg-info/SOURCES.txt` & `meerschaum-1.7.0.dev1/meerschaum.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -69,14 +69,15 @@
 meerschaum/api/dash/jobs.py
 meerschaum/api/dash/keys.py
 meerschaum/api/dash/pipes.py
 meerschaum/api/dash/plugins.py
 meerschaum/api/dash/sync.py
 meerschaum/api/dash/users.py
 meerschaum/api/dash/websockets.py
+meerschaum/api/dash/webterm.py
 meerschaum/api/dash/assets/__init__.py
 meerschaum/api/dash/assets/ansi_up.js
 meerschaum/api/dash/assets/banner_1920x320.png
 meerschaum/api/dash/assets/favicon.ico
 meerschaum/api/dash/assets/logo_48x48.png
 meerschaum/api/dash/assets/logo_500x500.png
 meerschaum/api/dash/callbacks/__init__.py
```

### Comparing `meerschaum-1.6.9/meerschaum.egg-info/requires.txt` & `meerschaum-1.7.0.dev1/meerschaum.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -13,34 +13,33 @@
 pathspec>=0.9.0
 python-dateutil>=2.7.5
 requests>=2.23.0
 binaryornot>=0.4.4
 pyvim>=3.0.2
 aiofiles>=0.6.0
 packaging>=21.3.0
-prompt-toolkit>=3.0.11
+prompt-toolkit>=3.0.39
 more-itertools>=8.7.0
 daemoniker>=0.2.3
 psutil>=5.8.0
 watchgod>=0.7.0
 dill>=0.3.3
 virtualenv>=20.1.0
-rocketry>=2.3.0
+rocketry>=2.5.1
 
 [api]
-uvicorn[standard]>=0.17.5
+uvicorn[standard]>=0.22.0
 gunicorn>=20.1.0
 python-dotenv>=0.20.0
-websockets>=8.1.0
-fastapi>=0.89.0
-fastapi-jwt-auth>=0.5.0
+websockets>=11.0.3
+fastapi>=0.100.0
 passlib>=1.7.4
 fastapi-login>=1.7.2
 python-multipart>=0.0.5
-pydantic>=1.10.2
+pydantic>=1.7.4
 numpy>=1.18.5
 pandas>=1.5.3
 pytz>=2022.1.0
 joblib>=0.17.0
 SQLAlchemy>=2.0.5
 databases>=0.4.0
 aiosqlite>=0.16.0
@@ -61,28 +60,28 @@
 pathspec>=0.9.0
 python-dateutil>=2.7.5
 requests>=2.23.0
 binaryornot>=0.4.4
 pyvim>=3.0.2
 aiofiles>=0.6.0
 packaging>=21.3.0
-prompt-toolkit>=3.0.11
+prompt-toolkit>=3.0.39
 more-itertools>=8.7.0
 daemoniker>=0.2.3
 psutil>=5.8.0
 watchgod>=0.7.0
 dill>=0.3.3
 virtualenv>=20.1.0
-rocketry>=2.3.0
+rocketry>=2.5.1
 pprintpp>=0.4.0
 asciitree>=0.3.3
-typing_extensions>=4.4.0
+typing-extensions>=4.7.1
 pygments>=2.7.2
 colorama>=0.4.3
-rich>=12.4.4
+rich>=13.4.2
 more-termcolor>=1.1.3
 humanfriendly>=10.0.0
 Flask-Compress>=1.10.1
 dash>=2.6.2
 dash-bootstrap-components>=1.2.1
 dash-ace>=0.2.1
 dash-extensions>=0.1.6
@@ -144,28 +143,28 @@
 modin[ray]>=0.8.3
 nanoid>=2.0.0
 importlib-metadata>=4.12.0
 
 [formatting]
 pprintpp>=0.4.0
 asciitree>=0.3.3
-typing_extensions>=4.4.0
+typing-extensions>=4.7.1
 pygments>=2.7.2
 colorama>=0.4.3
-rich>=12.4.4
+rich>=13.4.2
 more-termcolor>=1.1.3
 humanfriendly>=10.0.0
 
 [full]
 pprintpp>=0.4.0
 asciitree>=0.3.3
-typing_extensions>=4.4.0
+typing-extensions>=4.7.1
 pygments>=2.7.2
 colorama>=0.4.3
-rich>=12.4.4
+rich>=13.4.2
 more-termcolor>=1.1.3
 humanfriendly>=10.0.0
 wheel>=0.34.2
 setuptools>=63.3.0
 PyYAML>=5.3.1
 pip>=22.0.4
 update-checker>=0.18.0
@@ -173,22 +172,22 @@
 pathspec>=0.9.0
 python-dateutil>=2.7.5
 requests>=2.23.0
 binaryornot>=0.4.4
 pyvim>=3.0.2
 aiofiles>=0.6.0
 packaging>=21.3.0
-prompt-toolkit>=3.0.11
+prompt-toolkit>=3.0.39
 more-itertools>=8.7.0
 daemoniker>=0.2.3
 psutil>=5.8.0
 watchgod>=0.7.0
 dill>=0.3.3
 virtualenv>=20.1.0
-rocketry>=2.3.0
+rocketry>=2.5.1
 cryptography>=38.0.1
 psycopg2-binary>=2.8.6
 PyMySQL>=0.9.0
 aiomysql>=0.0.21
 sqlalchemy-cockroachdb>=2.0.0
 duckdb>=0.7.1
 duckdb-engine>=0.7.0
@@ -210,24 +209,23 @@
 asyncpg>=0.21.0
 Flask-Compress>=1.10.1
 dash>=2.6.2
 dash-bootstrap-components>=1.2.1
 dash-ace>=0.2.1
 dash-extensions>=0.1.6
 dash-daq>=0.5.0
-uvicorn[standard]>=0.17.5
+uvicorn[standard]>=0.22.0
 gunicorn>=20.1.0
 python-dotenv>=0.20.0
-websockets>=8.1.0
-fastapi>=0.89.0
-fastapi-jwt-auth>=0.5.0
+websockets>=11.0.3
+fastapi>=0.100.0
 passlib>=1.7.4
 fastapi-login>=1.7.2
 python-multipart>=0.0.5
-pydantic>=1.10.2
+pydantic>=1.7.4
 
 [gui]
 toga>=0.3.0-dev29
 terminado>=0.12.1
 tornado>=6.1.0
 tornado-xstatic>=0.2.0
 XStatic>=1.0.2
@@ -266,18 +264,18 @@
 pathspec>=0.9.0
 python-dateutil>=2.7.5
 requests>=2.23.0
 binaryornot>=0.4.4
 pyvim>=3.0.2
 aiofiles>=0.6.0
 packaging>=21.3.0
-prompt-toolkit>=3.0.11
+prompt-toolkit>=3.0.39
 more-itertools>=8.7.0
 daemoniker>=0.2.3
 psutil>=5.8.0
 watchgod>=0.7.0
 dill>=0.3.3
 virtualenv>=20.1.0
-rocketry>=2.3.0
+rocketry>=2.5.1
 
 [stack]
 docker-compose>=1.27.4
```

### Comparing `meerschaum-1.6.9/setup.py` & `meerschaum-1.7.0.dev1/setup.py`

 * *Files identical despite different names*

