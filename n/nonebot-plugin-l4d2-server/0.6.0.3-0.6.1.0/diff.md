# Comparing `tmp/nonebot_plugin_l4d2_server-0.6.0.3.tar.gz` & `tmp/nonebot_plugin_l4d2_server-0.6.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_l4d2_server-0.6.0.3.tar", last modified: Mon Jul 31 08:18:16 2023, max compression
+gzip compressed data, was "nonebot_plugin_l4d2_server-0.6.1.0.tar", last modified: Fri Aug  4 00:46:22 2023, max compression
```

## Comparing `nonebot_plugin_l4d2_server-0.6.0.3.tar` & `nonebot_plugin_l4d2_server-0.6.1.0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0    35149 2023-07-31 08:17:59.133239 nonebot_plugin_l4d2_server-0.6.0.3/LICENSE
--rw-r--r--   0        0        0     5749 2023-07-31 08:17:59.133239 nonebot_plugin_l4d2_server-0.6.0.3/README.md
--rw-r--r--   0        0        0    19681 2023-07-31 08:17:59.137240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/__init__.py
--rw-r--r--   0        0        0   158357 2023-07-31 08:17:59.137240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png
--rw-r--r--   0        0        0   631630 2023-07-31 08:17:59.137240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png
--rw-r--r--   0        0        0   405369 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg
--rw-r--r--   0        0        0     1590 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html
--rw-r--r--   0        0        0   242997 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png
--rw-r--r--   0        0        0     2135 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg
--rw-r--r--   0        0        0     7067 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/group_ip.html
--rw-r--r--   0        0        0     6135 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html
--rw-r--r--   0        0        0     6170 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html
--rw-r--r--   0        0        0     1523 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html
--rw-r--r--   0        0        0     5506 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg
--rw-r--r--   0        0        0     2408 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg
--rw-r--r--   0        0        0     7874 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css
--rw-r--r--   0        0        0      486 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/w.svg
--rw-r--r--   0        0        0     1350 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/data/img/white.png
--rw-r--r--   0        0        0     8647 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py
--rw-r--r--   0        0        0     1618 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py
--rw-r--r--   0        0        0     2980 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py
--rw-r--r--   0        0        0     1887 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_anne/server.py
--rw-r--r--   0        0        0      369 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_anne/startand.py
--rw-r--r--   0        0        0     3541 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_data/__init__.py
--rw-r--r--   0        0        0      449 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_data/config.py
--rw-r--r--   0        0        0        0 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_data/database.py
--rw-r--r--   0        0        0     3368 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_data/players.py
--rw-r--r--   0        0        0     1293 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_data/serverip.py
--rw-r--r--   0        0        0     3056 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_file/__init__.py
--rw-r--r--   0        0        0     1868 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py
--rw-r--r--   0        0        0     1976 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_file/input_json.py
--rw-r--r--   0        0        0     3074 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_file/remote.py
--rw-r--r--   0        0        0     3990 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_image/__init__.py
--rw-r--r--   0        0        0     4248 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_image/download.py
--rw-r--r--   0        0        0      664 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py
--rw-r--r--   0        0        0     2801 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_image/images.py
--rw-r--r--   0        0        0     1142 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_image/one.py
--rw-r--r--   0        0        0      922 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py
--rw-r--r--   0        0        0     2203 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_image/steam.py
--rw-r--r--   0        0        0     1399 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py
--rw-r--r--   0        0        0     7543 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_push/__init__.py
--rw-r--r--   0        0        0     1266 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py
--rw-r--r--   0        0        0     1148 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_queries/api.py
--rw-r--r--   0        0        0     1177 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_queries/local_ip.py
--rw-r--r--   0        0        0    12995 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py
--rw-r--r--   0        0        0     5273 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_queries/utils.py
--rw-r--r--   0        0        0     1403 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_server/__init__.py
--rw-r--r--   0        0        0        0 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_server/index.py
--rw-r--r--   0        0        0     1321 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_server/rcon.py
--rw-r--r--   0        0        0     1583 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_server/workshop.py
--rw-r--r--   0        0        0     4029 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_update/__init__.py
--rw-r--r--   0        0        0     1186 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py
--rw-r--r--   0        0        0     2181 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_update/restart.py
--rw-r--r--   0        0        0     1465 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_update/update.py
--rw-r--r--   0        0        0     9074 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_utils/command.py
--rw-r--r--   0        0        0     5985 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_utils/config.py
--rw-r--r--   0        0        0     1631 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_utils/message.py
--rw-r--r--   0        0        0     1007 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_utils/rule.py
--rw-r--r--   0        0        0     1230 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_utils/seach.py
--rw-r--r--   0        0        0      781 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py
--rw-r--r--   0        0        0     7384 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_utils/utils.py
--rw-r--r--   0        0        0     9778 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_web/web.py
--rw-r--r--   0        0        0    16217 2023-07-31 08:17:59.145240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_web/webUI.py
--rw-r--r--   0        0        0     3339 2023-07-31 08:17:59.145240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_web/webUI_s.py
--rw-r--r--   0        0        0     2196 2023-07-31 08:18:16.869506 nonebot_plugin_l4d2_server-0.6.0.3/pyproject.toml
--rw-r--r--   0        0        0     6565 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.6.0.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-08-04 00:46:03.402769 nonebot_plugin_l4d2_server-0.6.1.0/LICENSE
+-rw-r--r--   0        0        0     5815 2023-08-04 00:46:03.402769 nonebot_plugin_l4d2_server-0.6.1.0/README.md
+-rw-r--r--   0        0        0    19676 2023-08-04 00:46:03.406769 nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/__init__.py
+-rw-r--r--   0        0        0   158357 2023-08-04 00:46:03.406769 nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png
+-rw-r--r--   0        0        0   631630 2023-08-04 00:46:03.406769 nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png
+-rw-r--r--   0        0        0   405369 2023-08-04 00:46:03.410769 nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg
+-rw-r--r--   0        0        0     1590 2023-08-04 00:46:03.410769 nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html
+-rw-r--r--   0        0        0   242997 2023-08-04 00:46:03.410769 nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png
+-rw-r--r--   0        0        0     2135 2023-08-04 00:46:03.410769 nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg
+-rw-r--r--   0        0        0     7067 2023-08-04 00:46:03.410769 nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/group_ip.html
+-rw-r--r--   0        0        0     6135 2023-08-04 00:46:03.410769 nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html
+-rw-r--r--   0        0        0     6170 2023-08-04 00:46:03.410769 nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html
+-rw-r--r--   0        0        0     1523 2023-08-04 00:46:03.410769 nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html
+-rw-r--r--   0        0        0     5506 2023-08-04 00:46:03.410769 nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg
+-rw-r--r--   0        0        0     2408 2023-08-04 00:46:03.410769 nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg
+-rw-r--r--   0        0        0     7874 2023-08-04 00:46:03.410769 nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css
+-rw-r--r--   0        0        0      486 2023-08-04 00:46:03.410769 nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/w.svg
+-rw-r--r--   0        0        0     1350 2023-08-04 00:46:03.410769 nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/data/img/white.png
+-rw-r--r--   0        0        0     8647 2023-08-04 00:46:03.410769 nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py
+-rw-r--r--   0        0        0     1618 2023-08-04 00:46:03.410769 nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py
+-rw-r--r--   0        0        0     2980 2023-08-04 00:46:03.410769 nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py
+-rw-r--r--   0        0        0     1887 2023-08-04 00:46:03.410769 nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_anne/server.py
+-rw-r--r--   0        0        0      369 2023-08-04 00:46:03.410769 nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_anne/startand.py
+-rw-r--r--   0        0        0     3541 2023-08-04 00:46:03.410769 nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_data/__init__.py
+-rw-r--r--   0        0        0      449 2023-08-04 00:46:03.410769 nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_data/config.py
+-rw-r--r--   0        0        0        0 2023-08-04 00:46:03.410769 nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_data/database.py
+-rw-r--r--   0        0        0     3368 2023-08-04 00:46:03.410769 nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_data/players.py
+-rw-r--r--   0        0        0     1293 2023-08-04 00:46:03.410769 nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_data/serverip.py
+-rw-r--r--   0        0        0     3056 2023-08-04 00:46:03.410769 nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_file/__init__.py
+-rw-r--r--   0        0        0     1868 2023-08-04 00:46:03.410769 nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py
+-rw-r--r--   0        0        0     1976 2023-08-04 00:46:03.410769 nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_file/input_json.py
+-rw-r--r--   0        0        0     3074 2023-08-04 00:46:03.410769 nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_file/remote.py
+-rw-r--r--   0        0        0     3990 2023-08-04 00:46:03.410769 nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_image/__init__.py
+-rw-r--r--   0        0        0     4248 2023-08-04 00:46:03.410769 nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_image/download.py
+-rw-r--r--   0        0        0      664 2023-08-04 00:46:03.410769 nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py
+-rw-r--r--   0        0        0     2801 2023-08-04 00:46:03.410769 nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_image/images.py
+-rw-r--r--   0        0        0     1142 2023-08-04 00:46:03.410769 nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_image/one.py
+-rw-r--r--   0        0        0      922 2023-08-04 00:46:03.410769 nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py
+-rw-r--r--   0        0        0     2203 2023-08-04 00:46:03.410769 nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_image/steam.py
+-rw-r--r--   0        0        0     1399 2023-08-04 00:46:03.410769 nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py
+-rw-r--r--   0        0        0     7543 2023-08-04 00:46:03.410769 nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_push/__init__.py
+-rw-r--r--   0        0        0     1266 2023-08-04 00:46:03.410769 nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py
+-rw-r--r--   0        0        0     1148 2023-08-04 00:46:03.410769 nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_queries/api.py
+-rw-r--r--   0        0        0     1177 2023-08-04 00:46:03.410769 nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_queries/local_ip.py
+-rw-r--r--   0        0        0    12817 2023-08-04 00:46:03.410769 nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py
+-rw-r--r--   0        0        0     5282 2023-08-04 00:46:03.410769 nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_queries/utils.py
+-rw-r--r--   0        0        0     1403 2023-08-04 00:46:03.410769 nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_server/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-04 00:46:03.410769 nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_server/index.py
+-rw-r--r--   0        0        0     1321 2023-08-04 00:46:03.410769 nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_server/rcon.py
+-rw-r--r--   0        0        0     1583 2023-08-04 00:46:03.410769 nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_server/workshop.py
+-rw-r--r--   0        0        0     4029 2023-08-04 00:46:03.410769 nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_update/__init__.py
+-rw-r--r--   0        0        0     1186 2023-08-04 00:46:03.410769 nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py
+-rw-r--r--   0        0        0     2181 2023-08-04 00:46:03.410769 nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_update/restart.py
+-rw-r--r--   0        0        0     1465 2023-08-04 00:46:03.410769 nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_update/update.py
+-rw-r--r--   0        0        0     8874 2023-08-04 00:46:03.410769 nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_utils/command.py
+-rw-r--r--   0        0        0     5985 2023-08-04 00:46:03.414770 nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_utils/config.py
+-rw-r--r--   0        0        0     1631 2023-08-04 00:46:03.414770 nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_utils/message.py
+-rw-r--r--   0        0        0     1007 2023-08-04 00:46:03.414770 nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_utils/rule.py
+-rw-r--r--   0        0        0     1230 2023-08-04 00:46:03.414770 nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_utils/seach.py
+-rw-r--r--   0        0        0      783 2023-08-04 00:46:03.414770 nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py
+-rw-r--r--   0        0        0     7359 2023-08-04 00:46:03.414770 nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_utils/utils.py
+-rw-r--r--   0        0        0     9778 2023-08-04 00:46:03.414770 nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_web/web.py
+-rw-r--r--   0        0        0    16217 2023-08-04 00:46:03.414770 nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_web/webUI.py
+-rw-r--r--   0        0        0     3339 2023-08-04 00:46:03.414770 nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_web/webUI_s.py
+-rw-r--r--   0        0        0     2303 2023-08-04 00:46:22.103079 nonebot_plugin_l4d2_server-0.6.1.0/pyproject.toml
+-rw-r--r--   0        0        0     7457 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.6.1.0/PKG-INFO
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0.3/LICENSE` & `nonebot_plugin_l4d2_server-0.6.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.3/README.md` & `nonebot_plugin_l4d2_server-0.6.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+<!-- markdownlint-disable MD026 MD031 MD033 MD036 MD041 MD046 -->
 <div align="center">
   <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png" width="180" height="180"  alt="AgnesDigitalLogo">
   <br>
   <p><img src="https://s2.loli.net/2022/06/16/xsVUGRrkbn1ljTD.png" width="240" alt="NoneBotPluginText"></p>
 </div>
 
 <div align="center">
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/__init__.py` & `nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     NoticeEvent,
 )
 from nonebot.log import logger
 from nonebot.matcher import Matcher
 from nonebot.params import Arg, ArgPlainText, CommandArg, Keyword, RegexGroup
 from nonebot.plugin import PluginMetadata
 from nonebot.typing import T_State
+from nonebot_plugin_saa import Image, MessageFactory, Text
 
 from .l4d2_anne.server import updata_anne_server
 from .l4d2_data import sq_L4D2
 from .l4d2_file import all_zip_to_one, updown_l4d2_vpk
 
 # from .l4d2_file.input_json import *
 from .l4d2_image.steam import url_to_byte, url_to_byte_name
@@ -86,15 +87,15 @@
 require("nonebot_plugin_apscheduler")
 require("nonebot_plugin_htmlrender")
 require("nonebot_plugin_txt2img")
 scheduler = require("nonebot_plugin_apscheduler").scheduler
 
 driver = get_driver()
 
-__version__ = "0.6.0"
+__version__ = "0.6.1"
 __plugin_meta__ = PluginMetadata(
     name="求生之路小助手",
     description="可用于管理求生之路查服和本地管理",
     usage="群内对有关求生之路的查询和操作",
     type="application",
     homepage="https://github.com/Agnes4m/nonebot_plugin_l4d2_server",
     supported_adapters={"~onebot.v11"},
@@ -184,23 +185,22 @@
     else:
         mes = "你可能上传了相同的文件，或者解压失败了捏"
 
     await matcher.finish(mes_list(mes, vpk_files))
 
 
 @find_vpk.handle()
-async def _(matcher: Matcher):
+async def _():
     map_path = Path(l4_config.l4_ipall[l4_config.l4_number]["location"], vpk_path)
     name_vpk = get_vpk(map_path)
     logger.info("获取文件列表成功")
     mes = "当前服务器下有以下vpk文件"
-    msg = ""
-    msg = mes_list(msg, name_vpk).replace(" ", "")
+    msg = mes_list("", name_vpk).replace(" ", "")
 
-    await matcher.finish(mode_txt_to_img(mes, msg))
+    await mode_txt_to_img(mes, msg)
 
 
 @del_vpk.handle()
 async def _(matcher: Matcher, args: Message = CommandArg()):
     num1 = args.extract_plain_text()
     if num1:
         matcher.set_arg("num", args)
@@ -241,15 +241,15 @@
     if not usr_id:
         usr_id = event.user_id
     # 没有参数则从db里找数据
     msg = await search_anne(name, str(usr_id))
     if isinstance(msg, str):
         await matcher.finish(msg)
     elif isinstance(msg, bytes):
-        await matcher.finish(MessageSegment.image(msg))
+        await MessageFactory([Image(msg)]).finish()
 
 
 @anne_bind.handle()
 async def _(matcher: Matcher, event: MessageEvent, args: Message = CommandArg()):
     tag = args.extract_plain_text()
     tag = tag.strip()
     if tag == "" or tag.isspace():
@@ -261,30 +261,33 @@
     msg = await bind_steam(usr_id, tag, nickname)
     await matcher.finish(msg)
 
 
 @del_bind.handle()
 async def _(matcher: Matcher, event: MessageEvent):
     usr_id = event.user_id
-    await matcher.finish(name_exist(str(usr_id)))
+    msg = name_exist(str(usr_id))
+    if not msg:
+        return
+    await matcher.finish(msg)
 
 
 @rcon_to_server.handle()
 async def _(matcher: Matcher, args: Message = CommandArg()):
     msg = args.extract_plain_text()
     if msg:
         matcher.set_arg("command", args)
 
 
 @rcon_to_server.got("command", prompt="请输入向服务器发送的指令")
 async def _(matcher: Matcher, tag: str = ArgPlainText("command")):
     tag = tag.strip()
     msg = await command_server(tag)
     try:
-        await matcher.finish(mode_txt_to_img("服务器返回", msg))
+        await mode_txt_to_img("服务器返回", msg)
     except Exception as E:
         await matcher.finish(str(E), reply_message=True)
 
 
 @check_path.handle()
 async def _(matcher: Matcher, args: Message = CommandArg()):
     msg = args.extract_plain_text()
@@ -349,15 +352,15 @@
     group_id = event.group_id
     msg = await show_ip(group_id)
     if not msg:
         await matcher.finish("当前没有启动的服务器捏")
     if isinstance(msg, str):
         await matcher.finish(msg)
     else:
-        await matcher.finish(MessageSegment.image(msg))
+        await MessageFactory([Image(msg)]).finish()
 
 
 @join_server.handle()
 async def _(args: Message = CommandArg()):
     msg = args.extract_plain_text()
     url = await get_number_url(msg)
     await join_server.finish(url)
@@ -382,15 +385,15 @@
             return
         message: str = ""
         for item, value in msg.items():
             if item in ["图片地址", "下载地址", "细节"] or not isinstance(item, str):
                 continue
             message += item + ":" + value + "\n"
         state["dic"] = msg
-        await matcher.finish(MessageSegment.image(pic) + (message))
+        await MessageFactory([Image(pic), Text(message)]).finish()
     elif isinstance(msg, list):
         lenge = len(msg)
         pic = await url_to_byte(msg[0]["图片地址"])  # type: ignore
         message: str = f"有{lenge}个文件\n"
         ones = []
         for one in msg:
             for item, value in one.items():
@@ -466,27 +469,25 @@
     img_bytes = img_io.getbuffer()
     usr_id = event.user_id
     file_name: str = str(usr_id) + ".vtf"
     await upload_file(bot, event, img_bytes, file_name)
 
 
 @smx_file.handle()
-async def _(
-    matcher: Matcher,
-):
+async def _():
     smx_path = Path(
         l4_config.l4_ipall[l4_config.l4_number]["location"],
         "left4dead2/addons/sourcemod/plugins",
     )
     name_smx = get_vpk(smx_path, file_=".smx")
     logger.info("获取文件列表成功")
     mes = "当前服务器下有以下smx文件"
     msg = ""
     msg = mes_list(msg, name_smx).replace(" ", "")
-    await matcher.finish(mode_txt_to_img(mes, msg))
+    await mode_txt_to_img(mes, msg)
 
 
 # @search_api.handle()
 # async def _(matcher:Matcher,state:T_State,event:GroupMessageEvent,args:Message = CommandArg()):  # noqa: E501
 #     msg:str = args.extract_plain_text()
 #     # if msg.startswith('代码'):
 #         # 建图代码返回三方图信息
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png` & `nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png` & `nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg` & `nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html` & `nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png` & `nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg` & `nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/group_ip.html` & `nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/group_ip.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html` & `nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html` & `nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html` & `nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg` & `nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg` & `nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css` & `nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/data/img/white.png` & `nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/data/img/white.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py` & `nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py` & `nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py` & `nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_anne/server.py` & `nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_anne/server.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_data/__init__.py` & `nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_data/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_data/players.py` & `nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_data/players.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_data/serverip.py` & `nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_data/serverip.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_file/__init__.py` & `nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_file/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py` & `nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_file/input_json.py` & `nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_file/input_json.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_file/remote.py` & `nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_file/remote.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_image/__init__.py` & `nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_image/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_image/download.py` & `nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_image/download.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py` & `nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_image/images.py` & `nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_image/images.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_image/one.py` & `nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_image/one.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py` & `nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_image/steam.py` & `nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_image/steam.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py` & `nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_push/__init__.py` & `nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_push/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py` & `nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_queries/api.py` & `nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_queries/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_queries/local_ip.py` & `nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_queries/local_ip.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py` & `nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 from pathlib import Path
 from typing import Any, Dict, List, Tuple
 
 import a2s
 import aiofiles
 from nonebot.log import logger
 
-from nonebot_plugin_l4d2_server.l4d2_data.serverip import L4D2Server
-from nonebot_plugin_l4d2_server.l4d2_image import server_ip_pic
-from nonebot_plugin_l4d2_server.l4d2_queries.local_ip import ALL_HOST
-from nonebot_plugin_l4d2_server.l4d2_queries.utils import (
+from ..l4d2_data.serverip import L4D2Server
+from ..l4d2_image import server_ip_pic
+from ..l4d2_utils.message import KAILAO, PRISON, QUEREN
+from ..l4d2_utils.utils import split_maohao
+from .local_ip import ALL_HOST
+from .utils import (
     msg_ip_to_list,
     player_queries,
     player_queries_anne_dict,
     queries,
     queries_dict,
 )
-from nonebot_plugin_l4d2_server.l4d2_utils.message import KAILAO, PRISON, QUEREN
-from nonebot_plugin_l4d2_server.l4d2_utils.utils import split_maohao
 
 try:
     import ujson as json
 except ImportError:
     import json
 si = L4D2Server()
 errors = (
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_queries/utils.py` & `nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_queries/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,28 +42,27 @@
         pass
     # except Exception:
     # msgs = '有无法识别的用户名'
     # return msgs
     return msgs
 
 
-async def get_anne_server_ip(ip, ismsg: bool = False):
+async def get_anne_server_ip(ip: str, ismsg: bool = False):
     """输出查询ip和ping"""
     if ismsg:
         ...
     host, port = split_maohao(ip)
     data = await queries_server([host, port])
-
     if l4_config.l4_image:
-        data = mode_txt_to_img(
+        await mode_txt_to_img(
             data.split("\n")[0],
             data.replace(data.split("\n")[0], f"\nconnect {ip}"),
         )
-    else:
-        data += f"\nconnect {ip}"
+        return None
+    data += f"\nconnect {ip}"
     return data
 
 
 async def json_server_to_tag_dict(key: str, msg: str):
     """
     l4d2字典转tag的dict结果
      - 1、先匹配腐竹
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_server/__init__.py` & `nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_server/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_server/rcon.py` & `nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_server/rcon.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_server/workshop.py` & `nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_server/workshop.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_update/__init__.py` & `nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_update/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py` & `nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_update/restart.py` & `nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_update/restart.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_update/update.py` & `nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_update/update.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_utils/command.py` & `nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_utils/command.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import asyncio
 import re
 from time import sleep
 from typing import Dict, List, Tuple, Type
 
 from nonebot import on_command, on_keyword, on_notice, on_regex
-from nonebot.adapters.onebot.v11 import Message, MessageSegment
+from nonebot.adapters import Message
 from nonebot.log import logger
 from nonebot.matcher import Matcher
 from nonebot.params import CommandArg, CommandStart, RawCommand
+from nonebot_plugin_saa import Image, MessageFactory, Text
 
 from ..l4d2_anne.server import group_key, server_key
 from ..l4d2_queries import get_group_ip_to_msg
 from ..l4d2_queries.local_ip import ALL_HOST
 from ..l4d2_queries.qqgroup import get_tan_jian, qq_ip_queries_pic, split_maohao
 from ..l4d2_queries.utils import get_anne_server_ip, json_server_to_tag_dict
 from .config import MASTER, driver, l4_config
@@ -200,29 +201,23 @@
     ):
         if start:
             command = command.replace(start, "")
         if command == "anne":
             command = "云"
         msg: str = args.extract_plain_text()
         push_msg = await get_ip_to_mes(msg, command)
-        if not push_msg:
+        if push_msg is None:
             return
-        if isinstance(push_msg, Message):
-            logger.info("构造")
-            try:
-                await matcher.finish(push_msg)
-            except Exception as E:
-                logger.warning(E)
-                return
-        elif isinstance(push_msg, bytes):
+
+        if isinstance(push_msg, bytes):
             logger.info("直接发送图片")
-            send_msg = MessageSegment.image(push_msg)
+            await MessageFactory([Image(push_msg)]).finish()
         elif msg and type(push_msg) == list:
             logger.info("更加构造函数")
-            send_msg = Message(MessageSegment.image(push_msg[0]) + push_msg[-1])
+            await MessageFactory([Image(push_msg[0]), Text(push_msg[-1])]).finish()
         elif msg and isinstance(push_msg, str):
             send_msg = push_msg
         else:
             logger.info("出错了")
             return
         logger.info(type(send_msg))
         if not send_msg:
@@ -243,31 +238,33 @@
         this_ips = ALL_HOST[command]
         ip_list: List[Tuple[str, str, str]] = []
         for one_ip in this_ips:
             host, port = split_maohao(one_ip["ip"])
             msg_tuple = (one_ip["id"], host, port)
             ip_list.append(msg_tuple)
         img = await qq_ip_queries_pic(ip_list, igr)
-
-        return img if img else "服务器无响应"
+        return img if img else None
 
     if not msg[0].isdigit():
         # if any(mode in msg for mode in gamemode_list):
         #     pass
         # else:
         return None
     message = await json_server_to_tag_dict(command, msg)
     if len(message) == 0:
         # 关键词不匹配，忽略
         return None
     ip = str(message["ip"])
     logger.info(ip)
 
     try:
-        return await get_anne_server_ip(ip)
+        msg_send = await get_anne_server_ip(ip)
+        if msg_send:
+            return msg_send
+
     except (OSError, asyncio.exceptions.TimeoutError):
         return "服务器无响应"
 
 
 async def get_read_group_ip():
     """输出群组服务器"""
     get_grou_ip = on_command("anne", aliases=group_key(), priority=80, block=True)
@@ -280,23 +277,20 @@
         args: Message = CommandArg(),
     ):
         if start:
             command = command.replace(start, "")
         msg: str = args.extract_plain_text()
         push_msg = await get_group_ip_to_msg(msg, command)
         if isinstance(push_msg, bytes):
-            send_msg = MessageSegment.image(push_msg)
+            await MessageFactory([Image(push_msg)]).finish()
         elif msg and type(push_msg) == list:
-            send_msg = Message(MessageSegment.image(push_msg[0]) + push_msg[-1])
+            await MessageFactory([Image(push_msg[0]), Text(push_msg[-1])]).finish()
         elif msg and isinstance(push_msg, str):
             await str_to_picstr(push_msg, matcher)
-            return
-        else:
-            return
-        await matcher.finish(send_msg)
+        await matcher.finish()
 
 
 # tests = on_command("测试1")
 
 # @tests.handle()
 # async def _(event: Event,arg:Message=CommandArg()):
 #     logger.info(event)
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_utils/config.py` & `nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_utils/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_utils/message.py` & `nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_utils/message.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_utils/rule.py` & `nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_utils/rule.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_utils/seach.py` & `nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_utils/seach.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_utils/utils.py` & `nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 import tempfile
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, Dict, List, Optional, Tuple, Union
 
 import aiofiles
 import httpx
 from nonebot.adapters.onebot.v11 import Bot, GroupMessageEvent, MessageEvent
 from nonebot.log import logger
 from nonebot.matcher import Matcher
 
@@ -208,15 +208,15 @@
     def decorator(f):
         register_menu_func(*args, **kwargs)
         return f
 
     return decorator
 
 
-async def extract_last_digit(msg: str) -> tuple[str, str]:
+async def extract_last_digit(msg: str) -> Tuple[str, str]:
     "分离str和数字"
     for i in range(len(msg) - 1, -1, -1):
         if msg[i].isdigit():
             last_digit = msg[i]
             new_msg = msg[:i]
             return new_msg, last_digit
     return msg, ""
@@ -226,17 +226,17 @@
     """判断图片输出还是正常输出"""
     if l4_config.l4_image:
         lines = push_msg.splitlines()
         first_str = lines[0]
         last_str = lines[-1]
         push_msg = "\n".join(lines[1:-1])
         if l4_config.l4_connect:
-            await matcher.finish(mode_txt_to_img(first_str, push_msg, last_str))
+            await mode_txt_to_img(first_str, push_msg, last_str)
         else:
-            await matcher.finish(mode_txt_to_img(first_str, push_msg))
+            await mode_txt_to_img(first_str, push_msg)
     else:
         if l4_config.l4_connect or keyword == "connect":
             await matcher.send(push_msg)
         else:
             await matcher.send("\n".join(push_msg.splitlines()[1:-2]))
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_web/web.py` & `nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_web/web.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_web/webUI.py` & `nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_web/webUI.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_web/webUI_s.py` & `nonebot_plugin_l4d2_server-0.6.1.0/nonebot_plugin_l4d2_server/l4d2_web/webUI_s.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.3/pyproject.toml` & `nonebot_plugin_l4d2_server-0.6.1.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,48 @@
 [project]
 name = "nonebot-plugin-l4d2-server"
-version = "0.6.0.3"
+version = "0.6.1.0"
 description = "L4D2 server related operations plugin for NoneBot2"
 authors = [
     { name = "Agnes_Digital", email = "Z735803792@163.com" },
 ]
 requires-python = ">=3.9,<4.0"
 keywords = [
     "steam",
     "game",
     "l4d2",
     "nonebot2",
     "plugin",
 ]
+dependencies = [
+    "nonebot2>=2.0.0",
+    "nonebot-plugin-htmlrender==0.2.0.3",
+    "nonebot_plugin_txt2img>=0.3.0",
+    "nonebot-plugin-apscheduler>=0.2.0",
+    "nonebot-adapter-onebot>=2.2.3",
+    "nonebot-plugin-send-anything-anywhere>=0.2.7",
+    "asyncio>=3.4.3",
+    "aiohttp>=3.8.4",
+    "jinja2>=3.0.0",
+    "srctools>=2.3.9",
+    "bs4==0.0.1",
+    "httpx>=0.22.0",
+    "rcon==2.1.0",
+    "pillow>=9.4.0",
+    "pyunpack>=0.3.0",
+    "ruamel.yaml>=0.17.21",
+    "rarfile>=4.0",
+    "patool>=1.12",
+    "python-a2s>=1.3.0",
+    "amis-python>=1.0.6",
+    "pandas>=1.5.2",
+    "python-jose>=3.3.0",
+    "gitpython>=3.1.27",
+    "attrs>=23.1.0",
+]
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
@@ -26,44 +52,19 @@
 
 [project.license]
 text = "GPLv3"
 
 [project.urls]
 homepage = "https://github.com/Agnes4m/nonebot_plugin_l4d2_server"
 
-[tool.pdm.dependencies]
-nonebot2 = "^2.0.0"
-nonebot-plugin-htmlrender = "^0.2.0.3"
-nonebot_plugin_txt2img = ">=0.3.0"
-nonebot_plugin_apscheduler = "^0.2.0"
-nonebot-adapter-onebot = "^2.2.3"
-asyncio = ">=3.4.3"
-aiohttp = "^3.8.4"
-jinja2 = ">=3.0.0"
-srctools = "^2.3.9"
-bs4 = "0.0.1"
-httpx = ">=0.22.0"
-rcon = "^2.1.0"
-pillow = "^9.4.0"
-pyunpack = "^0.3.0"
-"ruamel.yaml" = "^0.17.21"
-rarfile = "^4.0"
-patool = "^1.12"
-python-a2s = "^1.3.0"
-amis-python = "^1.0.6"
-pandas = ">=1.5.2"
-python-jose = ">=3.3.0"
-gitpython = ">=3.1.27"
-attrs = "^23.1.0"
-
 [tool.pdm.build]
 includes = []
 
 [tool.pyright]
-pythonVersion = "3.9"
+pythonVersion = "3.8"
 
 [tool.black]
 line-length = 89
 target-version = [
     "py39",
     "py310",
     "py311",
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0.3/PKG-INFO` & `nonebot_plugin_l4d2_server-0.6.1.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,51 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-l4d2-server
-Version: 0.6.0.3
+Version: 0.6.1.0
 Summary: L4D2 server related operations plugin for NoneBot2
 Keywords: steam game l4d2 nonebot2 plugin
 Home-page: https://github.com/Agnes4m/nonebot_plugin_l4d2_server
 Author-Email: Agnes_Digital <Z735803792@163.com>
 License: GPLv3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Project-URL: Homepage, https://github.com/Agnes4m/nonebot_plugin_l4d2_server
 Requires-Python: <4.0,>=3.9
+Requires-Dist: nonebot2>=2.0.0
+Requires-Dist: nonebot-plugin-htmlrender==0.2.0.3
+Requires-Dist: nonebot_plugin_txt2img>=0.3.0
+Requires-Dist: nonebot-plugin-apscheduler>=0.2.0
+Requires-Dist: nonebot-adapter-onebot>=2.2.3
+Requires-Dist: nonebot-plugin-send-anything-anywhere>=0.2.7
+Requires-Dist: asyncio>=3.4.3
+Requires-Dist: aiohttp>=3.8.4
+Requires-Dist: jinja2>=3.0.0
+Requires-Dist: srctools>=2.3.9
+Requires-Dist: bs4==0.0.1
+Requires-Dist: httpx>=0.22.0
+Requires-Dist: rcon==2.1.0
+Requires-Dist: pillow>=9.4.0
+Requires-Dist: pyunpack>=0.3.0
+Requires-Dist: ruamel.yaml>=0.17.21
+Requires-Dist: rarfile>=4.0
+Requires-Dist: patool>=1.12
+Requires-Dist: python-a2s>=1.3.0
+Requires-Dist: amis-python>=1.0.6
+Requires-Dist: pandas>=1.5.2
+Requires-Dist: python-jose>=3.3.0
+Requires-Dist: gitpython>=3.1.27
+Requires-Dist: attrs>=23.1.0
 Description-Content-Type: text/markdown
 
+<!-- markdownlint-disable MD026 MD031 MD033 MD036 MD041 MD046 -->
 <div align="center">
   <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png" width="180" height="180"  alt="AgnesDigitalLogo">
   <br>
   <p><img src="https://s2.loli.net/2022/06/16/xsVUGRrkbn1ljTD.png" width="240" alt="NoneBotPluginText"></p>
 </div>
 
 <div align="center">
```

#### html2text {}

```diff
@@ -1,19 +1,30 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-l4d2-server Version: 0.6.0.3
+Metadata-Version: 2.1 Name: nonebot-plugin-l4d2-server Version: 0.6.1.0
 Summary: L4D2 server related operations plugin for NoneBot2 Keywords: steam
 game l4d2 nonebot2 plugin Home-page: https://github.com/Agnes4m/
 nonebot_plugin_l4d2_server Author-Email: Agnes_Digital
 163.com> License: GPLv3 Classifier: License :: OSI Approved :: GNU General
 Public License v3 (GPLv3) Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Operating System
 :: OS Independent Project-URL: Homepage, https://github.com/Agnes4m/
-nonebot_plugin_l4d2_server Requires-Python: <4.0,>=3.9 Description-Content-
-Type: text/markdown
+nonebot_plugin_l4d2_server Requires-Python: <4.0,>=3.9 Requires-Dist:
+nonebot2>=2.0.0 Requires-Dist: nonebot-plugin-htmlrender==0.2.0.3 Requires-
+Dist: nonebot_plugin_txt2img>=0.3.0 Requires-Dist: nonebot-plugin-
+apscheduler>=0.2.0 Requires-Dist: nonebot-adapter-onebot>=2.2.3 Requires-Dist:
+nonebot-plugin-send-anything-anywhere>=0.2.7 Requires-Dist: asyncio>=3.4.3
+Requires-Dist: aiohttp>=3.8.4 Requires-Dist: jinja2>=3.0.0 Requires-Dist:
+srctools>=2.3.9 Requires-Dist: bs4==0.0.1 Requires-Dist: httpx>=0.22.0
+Requires-Dist: rcon==2.1.0 Requires-Dist: pillow>=9.4.0 Requires-Dist:
+pyunpack>=0.3.0 Requires-Dist: ruamel.yaml>=0.17.21 Requires-Dist: rarfile>=4.0
+Requires-Dist: patool>=1.12 Requires-Dist: python-a2s>=1.3.0 Requires-Dist:
+amis-python>=1.0.6 Requires-Dist: pandas>=1.5.2 Requires-Dist: python-
+jose>=3.3.0 Requires-Dist: gitpython>=3.1.27 Requires-Dist: attrs>=23.1.0
+Description-Content-Type: text/markdown
                               [AgnesDigitalLogo]
                               [NoneBotPluginText]
  # nonebot_plugin_l4d2_server 0.6 _â¨Nonebot & Left 4 Dead 2 serveræä½â¨_
                 ææ¡£   Â·   æä»¤åè¡¨   Â·   å¸¸è§é®é¢
 
 [GitHub_stars] [GitHub_issues] [QQ_Chat_Group] [pypi] [pypi_download] [python]
                                    [NoneBot]
```

