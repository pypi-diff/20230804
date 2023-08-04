# Comparing `tmp/borgmatic-1.8.0.tar.gz` & `tmp/borgmatic-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "borgmatic-1.8.0.tar", last modified: Wed Jul 19 05:50:44 2023, max compression
+gzip compressed data, was "borgmatic-1.8.1.tar", last modified: Fri Aug  4 04:56:36 2023, max compression
```

## Comparing `borgmatic-1.8.0.tar` & `borgmatic-1.8.1.tar`

### file list

```diff
@@ -1,319 +1,320 @@
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-07-19 05:50:44.012133 borgmatic-1.8.0/
--rw-r--r--   0 witten    (1000) witten    (1000)       10 2021-06-08 17:56:15.000000 borgmatic-1.8.0/.dockerignore
--rw-r--r--   0 witten    (1000) witten    (1000)     1923 2023-07-10 16:39:03.000000 borgmatic-1.8.0/.drone.yml
--rw-r--r--   0 witten    (1000) witten    (1000)     1624 2023-06-27 21:37:40.000000 borgmatic-1.8.0/.eleventy.js
--rw-r--r--   0 witten    (1000) witten    (1000)       12 2023-06-27 21:37:40.000000 borgmatic-1.8.0/.flake8
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-07-19 05:50:43.962132 borgmatic-1.8.0/.gitea/
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-07-19 05:50:43.972132 borgmatic-1.8.0/.gitea/issue_template/
--rw-r--r--   0 witten    (1000) witten    (1000)     2113 2023-07-15 05:25:42.000000 borgmatic-1.8.0/.gitea/issue_template/bug_template.yaml
--rw-r--r--   0 witten    (1000) witten    (1000)       28 2023-07-15 05:17:31.000000 borgmatic-1.8.0/.gitea/issue_template/config.yaml
--rw-r--r--   0 witten    (1000) witten    (1000)      334 2023-07-15 05:24:16.000000 borgmatic-1.8.0/.gitea/issue_template/feature_template.yaml
--rw-r--r--   0 witten    (1000) witten    (1000)      105 2023-05-12 23:35:39.000000 borgmatic-1.8.0/.gitignore
--rw-r--r--   0 witten    (1000) witten    (1000)      631 2021-06-08 17:56:15.000000 borgmatic-1.8.0/AUTHORS
--rw-r--r--   0 witten    (1000) witten    (1000)    35122 2021-06-08 17:56:15.000000 borgmatic-1.8.0/LICENSE
--rw-r--r--   0 witten    (1000) witten    (1000)       58 2021-06-08 17:56:15.000000 borgmatic-1.8.0/MANIFEST.in
--rw-r--r--   0 witten    (1000) witten    (1000)    63363 2023-07-19 05:49:54.000000 borgmatic-1.8.0/NEWS
--rw-r--r--   0 witten    (1000) witten    (1000)      682 2023-07-19 05:50:44.012133 borgmatic-1.8.0/PKG-INFO
--rw-r--r--   0 witten    (1000) witten    (1000)     6650 2023-07-14 03:21:38.000000 borgmatic-1.8.0/README.md
--rw-r--r--   0 witten    (1000) witten    (1000)      658 2023-07-10 16:39:03.000000 borgmatic-1.8.0/SECURITY.md
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-07-19 05:50:43.972132 borgmatic-1.8.0/borgmatic/
--rw-r--r--   0 witten    (1000) witten    (1000)        0 2021-06-08 17:56:15.000000 borgmatic-1.8.0/borgmatic/__init__.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-07-19 05:50:43.975466 borgmatic-1.8.0/borgmatic/actions/
--rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-05-12 23:35:39.000000 borgmatic-1.8.0/borgmatic/actions/__init__.py
--rw-r--r--   0 witten    (1000) witten    (1000)      327 2023-07-10 16:39:03.000000 borgmatic-1.8.0/borgmatic/actions/arguments.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1190 2023-07-14 03:21:38.000000 borgmatic-1.8.0/borgmatic/actions/borg.py
--rw-r--r--   0 witten    (1000) witten    (1000)      878 2023-07-14 03:21:38.000000 borgmatic-1.8.0/borgmatic/actions/break_lock.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1458 2023-07-14 03:21:38.000000 borgmatic-1.8.0/borgmatic/actions/check.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1914 2023-07-14 03:21:38.000000 borgmatic-1.8.0/borgmatic/actions/compact.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-07-19 05:50:43.975466 borgmatic-1.8.0/borgmatic/actions/config/
--rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-07-10 16:39:03.000000 borgmatic-1.8.0/borgmatic/actions/config/__init__.py
--rw-r--r--   0 witten    (1000) witten    (1000)     3525 2023-07-14 03:21:38.000000 borgmatic-1.8.0/borgmatic/actions/config/bootstrap.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1622 2023-07-14 03:21:38.000000 borgmatic-1.8.0/borgmatic/actions/config/generate.py
--rw-r--r--   0 witten    (1000) witten    (1000)      858 2023-07-14 03:21:38.000000 borgmatic-1.8.0/borgmatic/actions/config/validate.py
--rw-r--r--   0 witten    (1000) witten    (1000)     3785 2023-07-14 03:21:38.000000 borgmatic-1.8.0/borgmatic/actions/create.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1521 2023-07-14 03:21:38.000000 borgmatic-1.8.0/borgmatic/actions/export_tar.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1962 2023-07-14 03:21:38.000000 borgmatic-1.8.0/borgmatic/actions/extract.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1543 2023-07-14 03:21:38.000000 borgmatic-1.8.0/borgmatic/actions/info.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1641 2023-07-14 03:21:38.000000 borgmatic-1.8.0/borgmatic/actions/list.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1385 2023-07-14 03:21:38.000000 borgmatic-1.8.0/borgmatic/actions/mount.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1380 2023-07-14 03:21:38.000000 borgmatic-1.8.0/borgmatic/actions/prune.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1091 2023-07-14 03:21:38.000000 borgmatic-1.8.0/borgmatic/actions/rcreate.py
--rw-r--r--   0 witten    (1000) witten    (1000)    13089 2023-07-14 03:21:38.000000 borgmatic-1.8.0/borgmatic/actions/restore.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1200 2023-07-14 03:21:38.000000 borgmatic-1.8.0/borgmatic/actions/rinfo.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1134 2023-07-14 03:21:38.000000 borgmatic-1.8.0/borgmatic/actions/rlist.py
--rw-r--r--   0 witten    (1000) witten    (1000)      705 2023-07-14 03:21:38.000000 borgmatic-1.8.0/borgmatic/actions/transfer.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-07-19 05:50:43.978799 borgmatic-1.8.0/borgmatic/borg/
--rw-r--r--   0 witten    (1000) witten    (1000)        0 2022-06-30 18:18:03.000000 borgmatic-1.8.0/borgmatic/borg/__init__.py
--rw-r--r--   0 witten    (1000) witten    (1000)     2360 2023-07-14 03:21:38.000000 borgmatic-1.8.0/borgmatic/borg/borg.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1348 2023-07-14 03:21:38.000000 borgmatic-1.8.0/borgmatic/borg/break_lock.py
--rw-r--r--   0 witten    (1000) witten    (1000)    15244 2023-07-14 03:21:38.000000 borgmatic-1.8.0/borgmatic/borg/check.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1800 2023-07-14 03:21:38.000000 borgmatic-1.8.0/borgmatic/borg/compact.py
--rw-r--r--   0 witten    (1000) witten    (1000)    19716 2023-07-14 03:21:38.000000 borgmatic-1.8.0/borgmatic/borg/create.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1783 2023-07-14 03:21:38.000000 borgmatic-1.8.0/borgmatic/borg/environment.py
--rw-r--r--   0 witten    (1000) witten    (1000)     2573 2023-07-14 03:21:38.000000 borgmatic-1.8.0/borgmatic/borg/export_tar.py
--rw-r--r--   0 witten    (1000) witten    (1000)     5530 2023-07-14 03:21:38.000000 borgmatic-1.8.0/borgmatic/borg/extract.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1368 2023-07-12 16:12:01.000000 borgmatic-1.8.0/borgmatic/borg/feature.py
--rw-r--r--   0 witten    (1000) witten    (1000)     2870 2023-07-07 05:26:07.000000 borgmatic-1.8.0/borgmatic/borg/flags.py
--rw-r--r--   0 witten    (1000) witten    (1000)     2670 2023-07-14 03:21:38.000000 borgmatic-1.8.0/borgmatic/borg/info.py
--rw-r--r--   0 witten    (1000) witten    (1000)     8470 2023-07-14 03:21:38.000000 borgmatic-1.8.0/borgmatic/borg/list.py
--rw-r--r--   0 witten    (1000) witten    (1000)     2851 2023-07-14 03:21:38.000000 borgmatic-1.8.0/borgmatic/borg/mount.py
--rw-r--r--   0 witten    (1000) witten    (1000)     3274 2023-07-14 03:21:38.000000 borgmatic-1.8.0/borgmatic/borg/prune.py
--rw-r--r--   0 witten    (1000) witten    (1000)     3056 2023-07-14 03:21:38.000000 borgmatic-1.8.0/borgmatic/borg/rcreate.py
--rw-r--r--   0 witten    (1000) witten    (1000)     2055 2023-07-14 03:21:38.000000 borgmatic-1.8.0/borgmatic/borg/rinfo.py
--rw-r--r--   0 witten    (1000) witten    (1000)     4998 2023-07-14 03:21:38.000000 borgmatic-1.8.0/borgmatic/borg/rlist.py
--rw-r--r--   0 witten    (1000) witten    (1000)       52 2023-07-07 05:36:58.000000 borgmatic-1.8.0/borgmatic/borg/state.py
--rw-r--r--   0 witten    (1000) witten    (1000)     2136 2023-07-14 03:21:38.000000 borgmatic-1.8.0/borgmatic/borg/transfer.py
--rw-r--r--   0 witten    (1000) witten    (1000)      576 2023-07-07 05:37:41.000000 borgmatic-1.8.0/borgmatic/borg/umount.py
--rw-r--r--   0 witten    (1000) witten    (1000)      991 2023-07-14 03:21:38.000000 borgmatic-1.8.0/borgmatic/borg/version.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-07-19 05:50:43.978799 borgmatic-1.8.0/borgmatic/commands/
--rw-r--r--   0 witten    (1000) witten    (1000)        0 2021-06-08 17:56:15.000000 borgmatic-1.8.0/borgmatic/commands/__init__.py
--rw-r--r--   0 witten    (1000) witten    (1000)    51275 2023-07-14 03:21:38.000000 borgmatic-1.8.0/borgmatic/commands/arguments.py
--rw-r--r--   0 witten    (1000) witten    (1000)    31188 2023-07-14 03:21:38.000000 borgmatic-1.8.0/borgmatic/commands/borgmatic.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-07-19 05:50:43.982133 borgmatic-1.8.0/borgmatic/commands/completion/
--rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-07-10 16:39:03.000000 borgmatic-1.8.0/borgmatic/commands/completion/__init__.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1382 2023-07-10 16:39:03.000000 borgmatic-1.8.0/borgmatic/commands/completion/actions.py
--rw-r--r--   0 witten    (1000) witten    (1000)     2390 2023-07-10 16:39:03.000000 borgmatic-1.8.0/borgmatic/commands/completion/bash.py
--rw-r--r--   0 witten    (1000) witten    (1000)     6785 2023-07-10 16:39:03.000000 borgmatic-1.8.0/borgmatic/commands/completion/fish.py
--rw-r--r--   0 witten    (1000) witten    (1000)      488 2023-07-10 16:39:03.000000 borgmatic-1.8.0/borgmatic/commands/generate_config.py
--rw-r--r--   0 witten    (1000) witten    (1000)      488 2023-07-10 16:39:03.000000 borgmatic-1.8.0/borgmatic/commands/validate_config.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-07-19 05:50:43.982133 borgmatic-1.8.0/borgmatic/config/
--rw-r--r--   0 witten    (1000) witten    (1000)        0 2021-06-08 17:56:16.000000 borgmatic-1.8.0/borgmatic/config/__init__.py
--rw-r--r--   0 witten    (1000) witten    (1000)      349 2023-07-01 05:36:11.000000 borgmatic-1.8.0/borgmatic/config/checks.py
--rw-r--r--   0 witten    (1000) witten    (1000)     2210 2023-07-10 16:39:03.000000 borgmatic-1.8.0/borgmatic/config/collect.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1542 2023-06-27 21:37:40.000000 borgmatic-1.8.0/borgmatic/config/environment.py
--rw-r--r--   0 witten    (1000) witten    (1000)    10882 2023-07-14 03:21:38.000000 borgmatic-1.8.0/borgmatic/config/generate.py
--rw-r--r--   0 witten    (1000) witten    (1000)    12749 2023-07-14 03:21:38.000000 borgmatic-1.8.0/borgmatic/config/load.py
--rw-r--r--   0 witten    (1000) witten    (1000)    11064 2023-07-19 05:45:57.000000 borgmatic-1.8.0/borgmatic/config/normalize.py
--rw-r--r--   0 witten    (1000) witten    (1000)     2984 2023-07-14 03:21:38.000000 borgmatic-1.8.0/borgmatic/config/override.py
--rw-r--r--   0 witten    (1000) witten    (1000)    54538 2023-07-14 03:21:38.000000 borgmatic-1.8.0/borgmatic/config/schema.yaml
--rw-r--r--   0 witten    (1000) witten    (1000)     7260 2023-07-14 03:21:38.000000 borgmatic-1.8.0/borgmatic/config/validate.py
--rw-r--r--   0 witten    (1000) witten    (1000)    13958 2023-07-14 03:21:38.000000 borgmatic-1.8.0/borgmatic/execute.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-07-19 05:50:43.985466 borgmatic-1.8.0/borgmatic/hooks/
--rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-07-10 00:33:30.000000 borgmatic-1.8.0/borgmatic/hooks/__init__.py
--rw-r--r--   0 witten    (1000) witten    (1000)     3276 2023-06-27 21:37:40.000000 borgmatic-1.8.0/borgmatic/hooks/command.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1929 2023-07-14 03:21:38.000000 borgmatic-1.8.0/borgmatic/hooks/cronhub.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1810 2023-07-14 03:21:38.000000 borgmatic-1.8.0/borgmatic/hooks/cronitor.py
--rw-r--r--   0 witten    (1000) witten    (1000)     3203 2023-07-14 03:21:38.000000 borgmatic-1.8.0/borgmatic/hooks/dispatch.py
--rw-r--r--   0 witten    (1000) witten    (1000)     2387 2023-07-10 00:33:27.000000 borgmatic-1.8.0/borgmatic/hooks/dump.py
--rw-r--r--   0 witten    (1000) witten    (1000)     4896 2023-07-14 03:21:38.000000 borgmatic-1.8.0/borgmatic/hooks/healthchecks.py
--rw-r--r--   0 witten    (1000) witten    (1000)     7495 2023-07-14 03:21:38.000000 borgmatic-1.8.0/borgmatic/hooks/mongodb.py
--rw-r--r--   0 witten    (1000) witten    (1000)      180 2023-07-10 00:33:34.000000 borgmatic-1.8.0/borgmatic/hooks/monitor.py
--rw-r--r--   0 witten    (1000) witten    (1000)     9391 2023-07-14 03:21:38.000000 borgmatic-1.8.0/borgmatic/hooks/mysql.py
--rw-r--r--   0 witten    (1000) witten    (1000)     2852 2023-07-14 03:21:38.000000 borgmatic-1.8.0/borgmatic/hooks/ntfy.py
--rw-r--r--   0 witten    (1000) witten    (1000)     2606 2023-07-14 03:21:38.000000 borgmatic-1.8.0/borgmatic/hooks/pagerduty.py
--rw-r--r--   0 witten    (1000) witten    (1000)    12327 2023-07-14 03:21:38.000000 borgmatic-1.8.0/borgmatic/hooks/postgresql.py
--rw-r--r--   0 witten    (1000) witten    (1000)     5075 2023-07-14 03:21:38.000000 borgmatic-1.8.0/borgmatic/hooks/sqlite.py
--rw-r--r--   0 witten    (1000) witten    (1000)     7242 2023-07-10 16:39:03.000000 borgmatic-1.8.0/borgmatic/logger.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1048 2023-05-12 23:35:39.000000 borgmatic-1.8.0/borgmatic/signals.py
--rw-r--r--   0 witten    (1000) witten    (1000)      586 2023-07-10 16:39:03.000000 borgmatic-1.8.0/borgmatic/verbosity.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-07-19 05:50:43.972132 borgmatic-1.8.0/borgmatic.egg-info/
--rw-r--r--   0 witten    (1000) witten    (1000)      682 2023-07-19 05:50:43.000000 borgmatic-1.8.0/borgmatic.egg-info/PKG-INFO
--rw-r--r--   0 witten    (1000) witten    (1000)     8586 2023-07-19 05:50:43.000000 borgmatic-1.8.0/borgmatic.egg-info/SOURCES.txt
--rw-r--r--   0 witten    (1000) witten    (1000)        1 2023-07-19 05:50:43.000000 borgmatic-1.8.0/borgmatic.egg-info/dependency_links.txt
--rw-r--r--   0 witten    (1000) witten    (1000)      200 2023-07-19 05:50:43.000000 borgmatic-1.8.0/borgmatic.egg-info/entry_points.txt
--rw-r--r--   0 witten    (1000) witten    (1000)       89 2023-07-19 05:50:43.000000 borgmatic-1.8.0/borgmatic.egg-info/requires.txt
--rw-r--r--   0 witten    (1000) witten    (1000)       10 2023-07-19 05:50:43.000000 borgmatic-1.8.0/borgmatic.egg-info/top_level.txt
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-07-19 05:50:43.985466 borgmatic-1.8.0/docs/
--rw-r--r--   0 witten    (1000) witten    (1000)     1544 2023-07-10 16:39:03.000000 borgmatic-1.8.0/docs/Dockerfile
--rw-r--r--   0 witten    (1000) witten    (1000)     6650 2023-07-14 03:21:38.000000 borgmatic-1.8.0/docs/README.md
--rw-r--r--   0 witten    (1000) witten    (1000)      673 2023-05-12 23:35:39.000000 borgmatic-1.8.0/docs/SECURITY.md
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-07-19 05:50:43.985466 borgmatic-1.8.0/docs/_data/
--rw-r--r--   0 witten    (1000) witten    (1000)      112 2023-07-12 03:00:10.000000 borgmatic-1.8.0/docs/_data/borgmatic.js
--rw-r--r--   0 witten    (1000) witten    (1000)       19 2021-06-08 17:56:16.000000 borgmatic-1.8.0/docs/_data/layout.json
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-07-19 05:50:43.985466 borgmatic-1.8.0/docs/_includes/
--rw-r--r--   0 witten    (1000) witten    (1000)       52 2021-06-08 17:56:16.000000 borgmatic-1.8.0/docs/_includes/asciinema.css
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-07-19 05:50:43.985466 borgmatic-1.8.0/docs/_includes/components/
--rw-r--r--   0 witten    (1000) witten    (1000)      492 2021-06-08 17:56:16.000000 borgmatic-1.8.0/docs/_includes/components/external-links.css
--rw-r--r--   0 witten    (1000) witten    (1000)      636 2021-06-08 17:56:16.000000 borgmatic-1.8.0/docs/_includes/components/info-blocks.css
--rw-r--r--   0 witten    (1000) witten    (1000)     5125 2023-06-27 21:37:40.000000 borgmatic-1.8.0/docs/_includes/components/lists.css
--rw-r--r--   0 witten    (1000) witten    (1000)     1788 2023-06-27 21:37:40.000000 borgmatic-1.8.0/docs/_includes/components/minilink.css
--rw-r--r--   0 witten    (1000) witten    (1000)      219 2023-07-14 03:21:38.000000 borgmatic-1.8.0/docs/_includes/components/suggestion-link.html
--rw-r--r--   0 witten    (1000) witten    (1000)     1862 2023-06-27 21:37:40.000000 borgmatic-1.8.0/docs/_includes/components/toc.css
--rw-r--r--   0 witten    (1000) witten    (1000)      265 2021-06-08 17:56:16.000000 borgmatic-1.8.0/docs/_includes/header.njk
--rw-r--r--   0 witten    (1000) witten    (1000)    26340 2023-06-27 21:37:40.000000 borgmatic-1.8.0/docs/_includes/index.css
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-07-19 05:50:43.985466 borgmatic-1.8.0/docs/_includes/layouts/
--rw-r--r--   0 witten    (1000) witten    (1000)      909 2023-06-27 21:37:40.000000 borgmatic-1.8.0/docs/_includes/layouts/base.njk
--rw-r--r--   0 witten    (1000) witten    (1000)     1184 2023-07-12 03:00:10.000000 borgmatic-1.8.0/docs/_includes/layouts/main.njk
--rw-r--r--   0 witten    (1000) witten    (1000)     3039 2023-05-12 23:35:39.000000 borgmatic-1.8.0/docs/_includes/prism-theme.css
--rw-r--r--   0 witten    (1000) witten    (1000)      422 2023-07-12 03:00:10.000000 borgmatic-1.8.0/docs/docker-compose.yaml
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-07-19 05:50:43.988799 borgmatic-1.8.0/docs/how-to/
--rw-r--r--   0 witten    (1000) witten    (1000)     5278 2023-07-14 03:21:38.000000 borgmatic-1.8.0/docs/how-to/add-preparation-and-cleanup-steps-to-backups.md
--rw-r--r--   0 witten    (1000) witten    (1000)     5401 2023-07-14 03:21:38.000000 borgmatic-1.8.0/docs/how-to/backup-to-a-removable-drive-or-an-intermittent-server.md
--rw-r--r--   0 witten    (1000) witten    (1000)    15709 2023-07-14 03:21:38.000000 borgmatic-1.8.0/docs/how-to/backup-your-databases.md
--rw-r--r--   0 witten    (1000) witten    (1000)     7909 2023-07-14 03:21:38.000000 borgmatic-1.8.0/docs/how-to/deal-with-very-large-backups.md
--rw-r--r--   0 witten    (1000) witten    (1000)     6240 2023-07-14 03:21:38.000000 borgmatic-1.8.0/docs/how-to/develop-on-borgmatic.md
--rw-r--r--   0 witten    (1000) witten    (1000)     4363 2023-07-14 03:21:38.000000 borgmatic-1.8.0/docs/how-to/extract-a-backup.md
--rw-r--r--   0 witten    (1000) witten    (1000)       77 2023-07-14 03:21:38.000000 borgmatic-1.8.0/docs/how-to/index.md
--rw-r--r--   0 witten    (1000) witten    (1000)     6424 2023-07-14 03:21:38.000000 borgmatic-1.8.0/docs/how-to/inspect-your-backups.md
--rw-r--r--   0 witten    (1000) witten    (1000)     2165 2023-07-14 03:21:38.000000 borgmatic-1.8.0/docs/how-to/make-backups-redundant.md
--rw-r--r--   0 witten    (1000) witten    (1000)    19367 2023-07-14 03:21:38.000000 borgmatic-1.8.0/docs/how-to/make-per-application-backups.md
--rw-r--r--   0 witten    (1000) witten    (1000)    14685 2023-07-14 03:21:38.000000 borgmatic-1.8.0/docs/how-to/monitor-your-backups.md
--rw-r--r--   0 witten    (1000) witten    (1000)     3322 2023-07-14 03:21:38.000000 borgmatic-1.8.0/docs/how-to/provide-your-passwords.md
--rw-r--r--   0 witten    (1000) witten    (1000)      124 2022-06-16 18:55:15.000000 borgmatic-1.8.0/docs/how-to/restore-a-backup.md
--rw-r--r--   0 witten    (1000) witten    (1000)     5925 2023-07-10 16:39:03.000000 borgmatic-1.8.0/docs/how-to/run-arbitrary-borg-commands.md
--rw-r--r--   0 witten    (1000) witten    (1000)      152 2022-06-16 18:55:21.000000 borgmatic-1.8.0/docs/how-to/run-preparation-steps-before-backups.md
--rw-r--r--   0 witten    (1000) witten    (1000)    15841 2023-07-14 03:21:38.000000 borgmatic-1.8.0/docs/how-to/set-up-backups.md
--rw-r--r--   0 witten    (1000) witten    (1000)     7637 2023-07-14 03:21:38.000000 borgmatic-1.8.0/docs/how-to/upgrade.md
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-07-19 05:50:43.988799 borgmatic-1.8.0/docs/reference/
--rw-r--r--   0 witten    (1000) witten    (1000)      853 2023-07-14 03:21:38.000000 borgmatic-1.8.0/docs/reference/command-line.md
--rw-r--r--   0 witten    (1000) witten    (1000)      810 2023-07-10 16:39:03.000000 borgmatic-1.8.0/docs/reference/configuration.md
--rw-r--r--   0 witten    (1000) witten    (1000)       80 2023-07-14 03:21:38.000000 borgmatic-1.8.0/docs/reference/index.md
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-07-19 05:50:43.992133 borgmatic-1.8.0/docs/static/
--rw-r--r--   0 witten    (1000) witten    (1000)     5822 2021-06-08 17:56:16.000000 borgmatic-1.8.0/docs/static/borgbase.png
--rw-r--r--   0 witten    (1000) witten    (1000)     3593 2021-06-08 17:56:16.000000 borgmatic-1.8.0/docs/static/borgmatic.png
--rw-r--r--   0 witten    (1000) witten    (1000)     1674 2021-06-08 17:56:16.000000 borgmatic-1.8.0/docs/static/borgmatic.svg
--rw-r--r--   0 witten    (1000) witten    (1000)    23536 2021-06-08 17:56:16.000000 borgmatic-1.8.0/docs/static/cronhub.png
--rw-r--r--   0 witten    (1000) witten    (1000)    10364 2021-06-08 17:56:16.000000 borgmatic-1.8.0/docs/static/cronitor.png
--rw-r--r--   0 witten    (1000) witten    (1000)     4556 2021-06-08 17:56:16.000000 borgmatic-1.8.0/docs/static/healthchecks.png
--rw-r--r--   0 witten    (1000) witten    (1000)     9474 2021-06-08 17:56:16.000000 borgmatic-1.8.0/docs/static/mariadb.png
--rw-r--r--   0 witten    (1000) witten    (1000)    12839 2023-05-12 23:35:39.000000 borgmatic-1.8.0/docs/static/mongodb.png
--rw-r--r--   0 witten    (1000) witten    (1000)     3761 2021-06-08 17:56:16.000000 borgmatic-1.8.0/docs/static/mysql.png
--rw-r--r--   0 witten    (1000) witten    (1000)    10266 2023-05-12 23:35:39.000000 borgmatic-1.8.0/docs/static/ntfy.png
--rw-r--r--   0 witten    (1000) witten    (1000)    20107 2023-05-12 23:35:39.000000 borgmatic-1.8.0/docs/static/pagerduty.png
--rw-r--r--   0 witten    (1000) witten    (1000)    31528 2021-06-08 17:56:16.000000 borgmatic-1.8.0/docs/static/postgresql.png
--rw-r--r--   0 witten    (1000) witten    (1000)     4668 2023-06-27 21:37:40.000000 borgmatic-1.8.0/docs/static/sqlite.png
--rw-r--r--   0 witten    (1000) witten    (1000)       64 2023-04-15 02:33:57.000000 borgmatic-1.8.0/pyproject.toml
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-07-19 05:50:43.965466 borgmatic-1.8.0/sample/
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-07-19 05:50:43.992133 borgmatic-1.8.0/sample/cron/
--rw-r--r--   0 witten    (1000) witten    (1000)      183 2023-05-12 23:35:39.000000 borgmatic-1.8.0/sample/cron/borgmatic
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-07-19 05:50:43.992133 borgmatic-1.8.0/sample/systemd/
--rw-r--r--   0 witten    (1000) witten    (1000)      499 2023-07-10 16:39:03.000000 borgmatic-1.8.0/sample/systemd/borgmatic-user.service
--rw-r--r--   0 witten    (1000) witten    (1000)      138 2023-06-14 21:55:41.000000 borgmatic-1.8.0/sample/systemd/borgmatic-user.timer
--rw-r--r--   0 witten    (1000) witten    (1000)     2612 2023-07-10 16:39:03.000000 borgmatic-1.8.0/sample/systemd/borgmatic.service
--rw-r--r--   0 witten    (1000) witten    (1000)      138 2023-06-14 21:55:41.000000 borgmatic-1.8.0/sample/systemd/borgmatic.timer
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-07-19 05:50:43.992133 borgmatic-1.8.0/scripts/
--rwxr-xr-x   0 witten    (1000) witten    (1000)      259 2023-07-10 16:39:03.000000 borgmatic-1.8.0/scripts/dev-docs
--rwxr-xr-x   0 witten    (1000) witten    (1000)     3108 2023-05-12 23:35:39.000000 borgmatic-1.8.0/scripts/find-unsupported-borg-options
--rwxr-xr-x   0 witten    (1000) witten    (1000)      137 2021-06-08 17:56:16.000000 borgmatic-1.8.0/scripts/push
--rwxr-xr-x   0 witten    (1000) witten    (1000)     1685 2023-07-10 16:39:03.000000 borgmatic-1.8.0/scripts/release
--rwxr-xr-x   0 witten    (1000) witten    (1000)      658 2023-06-27 21:37:40.000000 borgmatic-1.8.0/scripts/run-end-to-end-dev-tests
--rwxr-xr-x   0 witten    (1000) witten    (1000)     1334 2023-07-10 16:39:03.000000 borgmatic-1.8.0/scripts/run-full-tests
--rw-r--r--   0 witten    (1000) witten    (1000)      505 2023-07-19 05:50:44.012133 borgmatic-1.8.0/setup.cfg
--rw-r--r--   0 witten    (1000) witten    (1000)     1312 2023-07-19 05:50:00.000000 borgmatic-1.8.0/setup.py
--rw-r--r--   0 witten    (1000) witten    (1000)      818 2023-07-10 16:39:03.000000 borgmatic-1.8.0/test_requirements.txt
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-07-19 05:50:43.992133 borgmatic-1.8.0/tests/
--rw-r--r--   0 witten    (1000) witten    (1000)        0 2021-06-08 17:56:16.000000 borgmatic-1.8.0/tests/__init__.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-07-19 05:50:43.995466 borgmatic-1.8.0/tests/end-to-end/
--rw-r--r--   0 witten    (1000) witten    (1000)        0 2021-06-08 17:56:16.000000 borgmatic-1.8.0/tests/end-to-end/__init__.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1383 2023-07-10 16:39:03.000000 borgmatic-1.8.0/tests/end-to-end/docker-compose.yaml
--rw-r--r--   0 witten    (1000) witten    (1000)     2981 2023-07-14 03:21:38.000000 borgmatic-1.8.0/tests/end-to-end/test_borgmatic.py
--rw-r--r--   0 witten    (1000) witten    (1000)      268 2023-07-14 02:24:28.000000 borgmatic-1.8.0/tests/end-to-end/test_completion.py
--rw-r--r--   0 witten    (1000) witten    (1000)    12221 2023-07-14 03:21:38.000000 borgmatic-1.8.0/tests/end-to-end/test_database.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1711 2023-07-14 02:24:16.000000 borgmatic-1.8.0/tests/end-to-end/test_dev_parity_with_build_server.py
--rw-r--r--   0 witten    (1000) witten    (1000)      588 2023-07-14 02:24:23.000000 borgmatic-1.8.0/tests/end-to-end/test_generate_config.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1980 2023-07-14 03:21:38.000000 borgmatic-1.8.0/tests/end-to-end/test_override.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1630 2023-07-14 03:21:38.000000 borgmatic-1.8.0/tests/end-to-end/test_validate_config.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-07-19 05:50:43.995466 borgmatic-1.8.0/tests/integration/
--rw-r--r--   0 witten    (1000) witten    (1000)        0 2021-06-08 17:56:16.000000 borgmatic-1.8.0/tests/integration/__init__.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-07-19 05:50:43.995466 borgmatic-1.8.0/tests/integration/actions/
--rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-07-10 16:39:03.000000 borgmatic-1.8.0/tests/integration/actions/__init__.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-07-19 05:50:43.995466 borgmatic-1.8.0/tests/integration/actions/config/
--rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-07-10 16:39:03.000000 borgmatic-1.8.0/tests/integration/actions/config/__init__.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1088 2023-07-10 16:39:03.000000 borgmatic-1.8.0/tests/integration/actions/config/test_validate.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-07-19 05:50:43.995466 borgmatic-1.8.0/tests/integration/borg/
--rw-r--r--   0 witten    (1000) witten    (1000)     5352 2023-07-14 03:21:38.000000 borgmatic-1.8.0/tests/integration/borg/test_commands.py
--rw-r--r--   0 witten    (1000) witten    (1000)      546 2023-05-12 23:35:39.000000 borgmatic-1.8.0/tests/integration/borg/test_feature.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-07-19 05:50:43.995466 borgmatic-1.8.0/tests/integration/commands/
--rw-r--r--   0 witten    (1000) witten    (1000)        0 2021-06-08 17:56:16.000000 borgmatic-1.8.0/tests/integration/commands/__init__.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-07-19 05:50:43.998800 borgmatic-1.8.0/tests/integration/commands/completion/
--rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-07-10 16:39:03.000000 borgmatic-1.8.0/tests/integration/commands/completion/__init__.py
--rw-r--r--   0 witten    (1000) witten    (1000)      811 2023-07-10 16:39:03.000000 borgmatic-1.8.0/tests/integration/commands/completion/test_actions.py
--rw-r--r--   0 witten    (1000) witten    (1000)      138 2023-07-10 16:39:03.000000 borgmatic-1.8.0/tests/integration/commands/completion/test_bash.py
--rw-r--r--   0 witten    (1000) witten    (1000)      138 2023-07-10 16:39:03.000000 borgmatic-1.8.0/tests/integration/commands/completion/test_fish.py
--rw-r--r--   0 witten    (1000) witten    (1000)    23211 2023-07-14 03:21:38.000000 borgmatic-1.8.0/tests/integration/commands/test_arguments.py
--rw-r--r--   0 witten    (1000) witten    (1000)      432 2023-04-15 02:32:17.000000 borgmatic-1.8.0/tests/integration/commands/test_borgmatic.py
--rw-r--r--   0 witten    (1000) witten    (1000)      214 2023-07-10 16:39:03.000000 borgmatic-1.8.0/tests/integration/commands/test_generate_config.py
--rw-r--r--   0 witten    (1000) witten    (1000)      214 2023-07-10 16:39:03.000000 borgmatic-1.8.0/tests/integration/commands/test_validate_config.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-07-19 05:50:43.998800 borgmatic-1.8.0/tests/integration/config/
--rw-r--r--   0 witten    (1000) witten    (1000)        0 2021-06-08 17:56:16.000000 borgmatic-1.8.0/tests/integration/config/__init__.py
--rw-r--r--   0 witten    (1000) witten    (1000)     8563 2023-07-14 03:21:38.000000 borgmatic-1.8.0/tests/integration/config/test_generate.py
--rw-r--r--   0 witten    (1000) witten    (1000)    35294 2023-07-10 16:39:03.000000 borgmatic-1.8.0/tests/integration/config/test_load.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1039 2023-05-12 23:35:39.000000 borgmatic-1.8.0/tests/integration/config/test_override.py
--rw-r--r--   0 witten    (1000) witten    (1000)      234 2023-05-12 23:35:39.000000 borgmatic-1.8.0/tests/integration/config/test_schema.py
--rw-r--r--   0 witten    (1000) witten    (1000)     7158 2023-07-14 03:21:38.000000 borgmatic-1.8.0/tests/integration/config/test_validate.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-07-19 05:50:43.998800 borgmatic-1.8.0/tests/integration/hooks/
--rw-r--r--   0 witten    (1000) witten    (1000)      753 2023-07-14 03:21:38.000000 borgmatic-1.8.0/tests/integration/hooks/test_healthchecks.py
--rw-r--r--   0 witten    (1000) witten    (1000)    11256 2023-06-27 21:37:40.000000 borgmatic-1.8.0/tests/integration/test_execute.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-07-19 05:50:43.998800 borgmatic-1.8.0/tests/unit/
--rw-r--r--   0 witten    (1000) witten    (1000)        0 2021-06-08 17:56:16.000000 borgmatic-1.8.0/tests/unit/__init__.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-07-19 05:50:44.002133 borgmatic-1.8.0/tests/unit/actions/
--rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-05-12 23:35:39.000000 borgmatic-1.8.0/tests/unit/actions/__init__.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-07-19 05:50:44.002133 borgmatic-1.8.0/tests/unit/actions/config/
--rw-r--r--   0 witten    (1000) witten    (1000)     4024 2023-07-10 16:39:03.000000 borgmatic-1.8.0/tests/unit/actions/config/test_bootstrap.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1305 2023-07-10 16:39:03.000000 borgmatic-1.8.0/tests/unit/actions/config/test_generate.py
--rw-r--r--   0 witten    (1000) witten    (1000)      599 2023-07-10 16:39:03.000000 borgmatic-1.8.0/tests/unit/actions/config/test_validate.py
--rw-r--r--   0 witten    (1000) witten    (1000)      390 2023-07-10 16:39:03.000000 borgmatic-1.8.0/tests/unit/actions/test_arguments.py
--rw-r--r--   0 witten    (1000) witten    (1000)      821 2023-07-14 03:21:38.000000 borgmatic-1.8.0/tests/unit/actions/test_borg.py
--rw-r--r--   0 witten    (1000) witten    (1000)      682 2023-07-14 03:21:38.000000 borgmatic-1.8.0/tests/unit/actions/test_break_lock.py
--rw-r--r--   0 witten    (1000) witten    (1000)     2847 2023-07-14 03:21:38.000000 borgmatic-1.8.0/tests/unit/actions/test_check.py
--rw-r--r--   0 witten    (1000) witten    (1000)     3049 2023-07-14 03:21:38.000000 borgmatic-1.8.0/tests/unit/actions/test_compact.py
--rw-r--r--   0 witten    (1000) witten    (1000)     6076 2023-07-14 03:21:38.000000 borgmatic-1.8.0/tests/unit/actions/test_create.py
--rw-r--r--   0 witten    (1000) witten    (1000)      967 2023-07-14 03:21:38.000000 borgmatic-1.8.0/tests/unit/actions/test_export_tar.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1074 2023-07-14 03:21:38.000000 borgmatic-1.8.0/tests/unit/actions/test_extract.py
--rw-r--r--   0 witten    (1000) witten    (1000)      993 2023-07-14 03:21:38.000000 borgmatic-1.8.0/tests/unit/actions/test_info.py
--rw-r--r--   0 witten    (1000) witten    (1000)      984 2023-07-14 03:21:38.000000 borgmatic-1.8.0/tests/unit/actions/test_list.py
--rw-r--r--   0 witten    (1000) witten    (1000)      824 2023-07-14 03:21:38.000000 borgmatic-1.8.0/tests/unit/actions/test_mount.py
--rw-r--r--   0 witten    (1000) witten    (1000)     2609 2023-07-14 03:21:38.000000 borgmatic-1.8.0/tests/unit/actions/test_prune.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1748 2023-07-14 03:21:38.000000 borgmatic-1.8.0/tests/unit/actions/test_rcreate.py
--rw-r--r--   0 witten    (1000) witten    (1000)    19198 2023-07-14 03:21:38.000000 borgmatic-1.8.0/tests/unit/actions/test_restore.py
--rw-r--r--   0 witten    (1000) witten    (1000)      743 2023-07-14 03:21:38.000000 borgmatic-1.8.0/tests/unit/actions/test_rinfo.py
--rw-r--r--   0 witten    (1000) witten    (1000)      721 2023-07-14 03:21:38.000000 borgmatic-1.8.0/tests/unit/actions/test_rlist.py
--rw-r--r--   0 witten    (1000) witten    (1000)      630 2023-07-14 03:21:38.000000 borgmatic-1.8.0/tests/unit/actions/test_transfer.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-07-19 05:50:44.005466 borgmatic-1.8.0/tests/unit/borg/
--rw-r--r--   0 witten    (1000) witten    (1000)        0 2021-06-08 17:56:16.000000 borgmatic-1.8.0/tests/unit/borg/__init__.py
--rw-r--r--   0 witten    (1000) witten    (1000)    10406 2023-07-14 03:21:38.000000 borgmatic-1.8.0/tests/unit/borg/test_borg.py
--rw-r--r--   0 witten    (1000) witten    (1000)     3332 2023-07-14 03:21:38.000000 borgmatic-1.8.0/tests/unit/borg/test_break_lock.py
--rw-r--r--   0 witten    (1000) witten    (1000)    39722 2023-07-14 03:21:38.000000 borgmatic-1.8.0/tests/unit/borg/test_check.py
--rw-r--r--   0 witten    (1000) witten    (1000)     6675 2023-07-14 03:21:38.000000 borgmatic-1.8.0/tests/unit/borg/test_compact.py
--rw-r--r--   0 witten    (1000) witten    (1000)   126262 2023-07-14 03:21:38.000000 borgmatic-1.8.0/tests/unit/borg/test_create.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1655 2023-07-12 05:16:01.000000 borgmatic-1.8.0/tests/unit/borg/test_environment.py
--rw-r--r--   0 witten    (1000) witten    (1000)    11144 2023-07-14 03:21:38.000000 borgmatic-1.8.0/tests/unit/borg/test_export_tar.py
--rw-r--r--   0 witten    (1000) witten    (1000)    19818 2023-07-14 03:21:38.000000 borgmatic-1.8.0/tests/unit/borg/test_extract.py
--rw-r--r--   0 witten    (1000) witten    (1000)     4866 2023-07-07 05:57:27.000000 borgmatic-1.8.0/tests/unit/borg/test_flags.py
--rw-r--r--   0 witten    (1000) witten    (1000)    24164 2023-07-14 03:21:38.000000 borgmatic-1.8.0/tests/unit/borg/test_info.py
--rw-r--r--   0 witten    (1000) witten    (1000)    25878 2023-07-14 03:21:38.000000 borgmatic-1.8.0/tests/unit/borg/test_list.py
--rw-r--r--   0 witten    (1000) witten    (1000)    10756 2023-07-14 03:21:38.000000 borgmatic-1.8.0/tests/unit/borg/test_mount.py
--rw-r--r--   0 witten    (1000) witten    (1000)    15245 2023-07-14 03:21:38.000000 borgmatic-1.8.0/tests/unit/borg/test_prune.py
--rw-r--r--   0 witten    (1000) witten    (1000)    12524 2023-07-14 03:21:38.000000 borgmatic-1.8.0/tests/unit/borg/test_rcreate.py
--rw-r--r--   0 witten    (1000) witten    (1000)    11325 2023-07-14 03:21:38.000000 borgmatic-1.8.0/tests/unit/borg/test_rinfo.py
--rw-r--r--   0 witten    (1000) witten    (1000)    23462 2023-07-14 03:21:38.000000 borgmatic-1.8.0/tests/unit/borg/test_rlist.py
--rw-r--r--   0 witten    (1000) witten    (1000)    20749 2023-07-14 03:21:38.000000 borgmatic-1.8.0/tests/unit/borg/test_transfer.py
--rw-r--r--   0 witten    (1000) witten    (1000)      920 2023-07-07 06:06:19.000000 borgmatic-1.8.0/tests/unit/borg/test_umount.py
--rw-r--r--   0 witten    (1000) witten    (1000)     2112 2023-07-14 03:21:38.000000 borgmatic-1.8.0/tests/unit/borg/test_version.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-07-19 05:50:44.005466 borgmatic-1.8.0/tests/unit/commands/
--rw-r--r--   0 witten    (1000) witten    (1000)        0 2021-06-08 17:56:16.000000 borgmatic-1.8.0/tests/unit/commands/__init__.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-07-19 05:50:44.008800 borgmatic-1.8.0/tests/unit/commands/completion/
--rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-07-10 16:39:03.000000 borgmatic-1.8.0/tests/unit/commands/completion/__init__.py
--rw-r--r--   0 witten    (1000) witten    (1000)      226 2023-07-10 16:39:03.000000 borgmatic-1.8.0/tests/unit/commands/completion/test_actions.py
--rw-r--r--   0 witten    (1000) witten    (1000)      431 2023-07-10 16:39:03.000000 borgmatic-1.8.0/tests/unit/commands/completion/test_bash.py
--rw-r--r--   0 witten    (1000) witten    (1000)     4616 2023-07-10 16:39:03.000000 borgmatic-1.8.0/tests/unit/commands/completion/test_fish.py
--rw-r--r--   0 witten    (1000) witten    (1000)    17204 2023-07-10 16:39:03.000000 borgmatic-1.8.0/tests/unit/commands/test_arguments.py
--rw-r--r--   0 witten    (1000) witten    (1000)    49716 2023-07-14 03:21:38.000000 borgmatic-1.8.0/tests/unit/commands/test_borgmatic.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-07-19 05:50:44.008800 borgmatic-1.8.0/tests/unit/config/
--rw-r--r--   0 witten    (1000) witten    (1000)        0 2021-06-08 17:56:16.000000 borgmatic-1.8.0/tests/unit/config/__init__.py
--rw-r--r--   0 witten    (1000) witten    (1000)      709 2023-04-15 02:32:17.000000 borgmatic-1.8.0/tests/unit/config/test_checks.py
--rw-r--r--   0 witten    (1000) witten    (1000)     8085 2023-07-10 16:39:03.000000 borgmatic-1.8.0/tests/unit/config/test_collect.py
--rw-r--r--   0 witten    (1000) witten    (1000)     3090 2023-06-27 21:37:40.000000 borgmatic-1.8.0/tests/unit/config/test_environment.py
--rw-r--r--   0 witten    (1000) witten    (1000)     4980 2023-07-14 03:21:38.000000 borgmatic-1.8.0/tests/unit/config/test_generate.py
--rw-r--r--   0 witten    (1000) witten    (1000)     7006 2023-07-14 03:21:38.000000 borgmatic-1.8.0/tests/unit/config/test_normalize.py
--rw-r--r--   0 witten    (1000) witten    (1000)     3804 2023-07-14 03:21:38.000000 borgmatic-1.8.0/tests/unit/config/test_override.py
--rw-r--r--   0 witten    (1000) witten    (1000)     7837 2023-07-14 03:21:38.000000 borgmatic-1.8.0/tests/unit/config/test_validate.py
-drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-07-19 05:50:44.012133 borgmatic-1.8.0/tests/unit/hooks/
--rw-r--r--   0 witten    (1000) witten    (1000)        0 2021-06-08 17:56:16.000000 borgmatic-1.8.0/tests/unit/hooks/__init__.py
--rw-r--r--   0 witten    (1000) witten    (1000)     3920 2023-07-01 23:41:53.000000 borgmatic-1.8.0/tests/unit/hooks/test_command.py
--rw-r--r--   0 witten    (1000) witten    (1000)     3726 2023-07-14 03:21:38.000000 borgmatic-1.8.0/tests/unit/hooks/test_cronhub.py
--rw-r--r--   0 witten    (1000) witten    (1000)     3162 2023-07-14 03:21:38.000000 borgmatic-1.8.0/tests/unit/hooks/test_cronitor.py
--rw-r--r--   0 witten    (1000) witten    (1000)     4490 2023-07-14 03:21:38.000000 borgmatic-1.8.0/tests/unit/hooks/test_dispatch.py
--rw-r--r--   0 witten    (1000) witten    (1000)     2938 2023-05-12 23:35:39.000000 borgmatic-1.8.0/tests/unit/hooks/test_dump.py
--rw-r--r--   0 witten    (1000) witten    (1000)    11731 2023-07-14 03:21:38.000000 borgmatic-1.8.0/tests/unit/hooks/test_healthchecks.py
--rw-r--r--   0 witten    (1000) witten    (1000)    17940 2023-07-14 03:21:38.000000 borgmatic-1.8.0/tests/unit/hooks/test_mongodb.py
--rw-r--r--   0 witten    (1000) witten    (1000)    20116 2023-07-14 03:21:38.000000 borgmatic-1.8.0/tests/unit/hooks/test_mysql.py
--rw-r--r--   0 witten    (1000) witten    (1000)     7411 2023-07-14 03:21:38.000000 borgmatic-1.8.0/tests/unit/hooks/test_ntfy.py
--rw-r--r--   0 witten    (1000) witten    (1000)     2303 2023-07-14 03:21:38.000000 borgmatic-1.8.0/tests/unit/hooks/test_pagerduty.py
--rw-r--r--   0 witten    (1000) witten    (1000)    38402 2023-07-14 03:21:38.000000 borgmatic-1.8.0/tests/unit/hooks/test_postgresql.py
--rw-r--r--   0 witten    (1000) witten    (1000)     7431 2023-07-14 03:21:38.000000 borgmatic-1.8.0/tests/unit/hooks/test_sqlite.py
--rw-r--r--   0 witten    (1000) witten    (1000)    18294 2023-06-27 21:37:40.000000 borgmatic-1.8.0/tests/unit/test_execute.py
--rw-r--r--   0 witten    (1000) witten    (1000)    16634 2023-07-10 16:39:03.000000 borgmatic-1.8.0/tests/unit/test_logger.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1405 2023-05-12 23:35:39.000000 borgmatic-1.8.0/tests/unit/test_signals.py
--rw-r--r--   0 witten    (1000) witten    (1000)     1426 2023-07-10 16:39:03.000000 borgmatic-1.8.0/tests/unit/test_verbosity.py
--rw-r--r--   0 witten    (1000) witten    (1000)      838 2023-06-27 21:37:40.000000 borgmatic-1.8.0/tox.ini
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-08-04 04:56:36.083221 borgmatic-1.8.1/
+-rw-r--r--   0 witten    (1000) witten    (1000)       10 2021-06-08 17:56:15.000000 borgmatic-1.8.1/.dockerignore
+-rw-r--r--   0 witten    (1000) witten    (1000)     1923 2023-07-10 16:39:03.000000 borgmatic-1.8.1/.drone.yml
+-rw-r--r--   0 witten    (1000) witten    (1000)     1624 2023-06-27 21:37:40.000000 borgmatic-1.8.1/.eleventy.js
+-rw-r--r--   0 witten    (1000) witten    (1000)       12 2023-06-27 21:37:40.000000 borgmatic-1.8.1/.flake8
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-08-04 04:56:36.036554 borgmatic-1.8.1/.gitea/
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-08-04 04:56:36.043220 borgmatic-1.8.1/.gitea/issue_template/
+-rw-r--r--   0 witten    (1000) witten    (1000)     2113 2023-07-22 17:14:49.000000 borgmatic-1.8.1/.gitea/issue_template/bug_template.yaml
+-rw-r--r--   0 witten    (1000) witten    (1000)       28 2023-07-22 17:14:49.000000 borgmatic-1.8.1/.gitea/issue_template/config.yaml
+-rw-r--r--   0 witten    (1000) witten    (1000)      334 2023-07-22 17:14:49.000000 borgmatic-1.8.1/.gitea/issue_template/feature_template.yaml
+-rw-r--r--   0 witten    (1000) witten    (1000)      105 2023-05-12 23:35:39.000000 borgmatic-1.8.1/.gitignore
+-rw-r--r--   0 witten    (1000) witten    (1000)      631 2021-06-08 17:56:15.000000 borgmatic-1.8.1/AUTHORS
+-rw-r--r--   0 witten    (1000) witten    (1000)    35122 2021-06-08 17:56:15.000000 borgmatic-1.8.1/LICENSE
+-rw-r--r--   0 witten    (1000) witten    (1000)       58 2021-06-08 17:56:15.000000 borgmatic-1.8.1/MANIFEST.in
+-rw-r--r--   0 witten    (1000) witten    (1000)    64448 2023-08-04 04:55:40.000000 borgmatic-1.8.1/NEWS
+-rw-r--r--   0 witten    (1000) witten    (1000)      682 2023-08-04 04:56:36.083221 borgmatic-1.8.1/PKG-INFO
+-rw-r--r--   0 witten    (1000) witten    (1000)     6650 2023-07-22 17:14:49.000000 borgmatic-1.8.1/README.md
+-rw-r--r--   0 witten    (1000) witten    (1000)      658 2023-07-10 16:39:03.000000 borgmatic-1.8.1/SECURITY.md
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-08-04 04:56:36.043220 borgmatic-1.8.1/borgmatic/
+-rw-r--r--   0 witten    (1000) witten    (1000)        0 2021-06-08 17:56:15.000000 borgmatic-1.8.1/borgmatic/__init__.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-08-04 04:56:36.049887 borgmatic-1.8.1/borgmatic/actions/
+-rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-05-12 23:35:39.000000 borgmatic-1.8.1/borgmatic/actions/__init__.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      327 2023-07-10 16:39:03.000000 borgmatic-1.8.1/borgmatic/actions/arguments.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1190 2023-07-22 17:14:49.000000 borgmatic-1.8.1/borgmatic/actions/borg.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      878 2023-07-22 17:14:49.000000 borgmatic-1.8.1/borgmatic/actions/break_lock.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1458 2023-07-22 17:14:49.000000 borgmatic-1.8.1/borgmatic/actions/check.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1914 2023-07-22 17:14:49.000000 borgmatic-1.8.1/borgmatic/actions/compact.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-08-04 04:56:36.049887 borgmatic-1.8.1/borgmatic/actions/config/
+-rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-07-10 16:39:03.000000 borgmatic-1.8.1/borgmatic/actions/config/__init__.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     3525 2023-07-22 17:14:49.000000 borgmatic-1.8.1/borgmatic/actions/config/bootstrap.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1622 2023-07-22 17:14:49.000000 borgmatic-1.8.1/borgmatic/actions/config/generate.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      858 2023-07-22 17:14:49.000000 borgmatic-1.8.1/borgmatic/actions/config/validate.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     3858 2023-07-31 21:00:38.000000 borgmatic-1.8.1/borgmatic/actions/create.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1521 2023-07-22 17:14:49.000000 borgmatic-1.8.1/borgmatic/actions/export_tar.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1962 2023-07-22 17:14:49.000000 borgmatic-1.8.1/borgmatic/actions/extract.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1543 2023-07-22 17:14:49.000000 borgmatic-1.8.1/borgmatic/actions/info.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1641 2023-07-22 17:14:49.000000 borgmatic-1.8.1/borgmatic/actions/list.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1385 2023-07-22 17:14:49.000000 borgmatic-1.8.1/borgmatic/actions/mount.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1380 2023-07-22 17:14:49.000000 borgmatic-1.8.1/borgmatic/actions/prune.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1091 2023-07-22 17:14:49.000000 borgmatic-1.8.1/borgmatic/actions/rcreate.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    13089 2023-07-22 17:14:49.000000 borgmatic-1.8.1/borgmatic/actions/restore.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1200 2023-07-22 17:14:49.000000 borgmatic-1.8.1/borgmatic/actions/rinfo.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1134 2023-07-22 17:14:49.000000 borgmatic-1.8.1/borgmatic/actions/rlist.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      705 2023-07-22 17:14:49.000000 borgmatic-1.8.1/borgmatic/actions/transfer.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-08-04 04:56:36.049887 borgmatic-1.8.1/borgmatic/borg/
+-rw-r--r--   0 witten    (1000) witten    (1000)        0 2022-06-30 18:18:03.000000 borgmatic-1.8.1/borgmatic/borg/__init__.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     2360 2023-07-22 17:14:49.000000 borgmatic-1.8.1/borgmatic/borg/borg.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1348 2023-07-22 17:14:49.000000 borgmatic-1.8.1/borgmatic/borg/break_lock.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    15274 2023-07-22 22:03:46.000000 borgmatic-1.8.1/borgmatic/borg/check.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1800 2023-07-22 17:14:49.000000 borgmatic-1.8.1/borgmatic/borg/compact.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    19844 2023-07-31 21:00:38.000000 borgmatic-1.8.1/borgmatic/borg/create.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1837 2023-07-22 22:25:10.000000 borgmatic-1.8.1/borgmatic/borg/environment.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     2573 2023-07-22 17:14:49.000000 borgmatic-1.8.1/borgmatic/borg/export_tar.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     5530 2023-07-22 17:14:49.000000 borgmatic-1.8.1/borgmatic/borg/extract.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1368 2023-07-12 16:12:01.000000 borgmatic-1.8.1/borgmatic/borg/feature.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     2927 2023-08-02 17:21:10.000000 borgmatic-1.8.1/borgmatic/borg/flags.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     2670 2023-07-22 17:14:49.000000 borgmatic-1.8.1/borgmatic/borg/info.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     8470 2023-07-22 17:14:49.000000 borgmatic-1.8.1/borgmatic/borg/list.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     2851 2023-07-22 17:14:49.000000 borgmatic-1.8.1/borgmatic/borg/mount.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     3313 2023-07-22 17:24:10.000000 borgmatic-1.8.1/borgmatic/borg/prune.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     3056 2023-07-22 17:14:49.000000 borgmatic-1.8.1/borgmatic/borg/rcreate.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     2055 2023-07-22 17:14:49.000000 borgmatic-1.8.1/borgmatic/borg/rinfo.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     4998 2023-07-22 17:14:49.000000 borgmatic-1.8.1/borgmatic/borg/rlist.py
+-rw-r--r--   0 witten    (1000) witten    (1000)       52 2023-07-07 05:36:58.000000 borgmatic-1.8.1/borgmatic/borg/state.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     2136 2023-07-22 17:14:49.000000 borgmatic-1.8.1/borgmatic/borg/transfer.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      576 2023-07-07 05:37:41.000000 borgmatic-1.8.1/borgmatic/borg/umount.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      991 2023-07-22 17:14:49.000000 borgmatic-1.8.1/borgmatic/borg/version.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-08-04 04:56:36.053221 borgmatic-1.8.1/borgmatic/commands/
+-rw-r--r--   0 witten    (1000) witten    (1000)        0 2021-06-08 17:56:15.000000 borgmatic-1.8.1/borgmatic/commands/__init__.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    51247 2023-08-02 04:47:09.000000 borgmatic-1.8.1/borgmatic/commands/arguments.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    31188 2023-07-22 17:14:49.000000 borgmatic-1.8.1/borgmatic/commands/borgmatic.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-08-04 04:56:36.053221 borgmatic-1.8.1/borgmatic/commands/completion/
+-rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-07-10 16:39:03.000000 borgmatic-1.8.1/borgmatic/commands/completion/__init__.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1382 2023-07-10 16:39:03.000000 borgmatic-1.8.1/borgmatic/commands/completion/actions.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     2390 2023-07-10 16:39:03.000000 borgmatic-1.8.1/borgmatic/commands/completion/bash.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     6785 2023-07-10 16:39:03.000000 borgmatic-1.8.1/borgmatic/commands/completion/fish.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      488 2023-07-10 16:39:03.000000 borgmatic-1.8.1/borgmatic/commands/generate_config.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      488 2023-07-10 16:39:03.000000 borgmatic-1.8.1/borgmatic/commands/validate_config.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-08-04 04:56:36.053221 borgmatic-1.8.1/borgmatic/config/
+-rw-r--r--   0 witten    (1000) witten    (1000)        0 2021-06-08 17:56:16.000000 borgmatic-1.8.1/borgmatic/config/__init__.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      349 2023-07-01 05:36:11.000000 borgmatic-1.8.1/borgmatic/config/checks.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     2210 2023-07-10 16:39:03.000000 borgmatic-1.8.1/borgmatic/config/collect.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1542 2023-06-27 21:37:40.000000 borgmatic-1.8.1/borgmatic/config/environment.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    10882 2023-07-22 17:14:49.000000 borgmatic-1.8.1/borgmatic/config/generate.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    15539 2023-08-02 04:47:09.000000 borgmatic-1.8.1/borgmatic/config/load.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    11176 2023-08-02 04:47:09.000000 borgmatic-1.8.1/borgmatic/config/normalize.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     2984 2023-07-22 17:14:49.000000 borgmatic-1.8.1/borgmatic/config/override.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    54905 2023-07-31 21:00:38.000000 borgmatic-1.8.1/borgmatic/config/schema.yaml
+-rw-r--r--   0 witten    (1000) witten    (1000)     7260 2023-08-01 06:01:43.000000 borgmatic-1.8.1/borgmatic/config/validate.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    13958 2023-07-22 17:14:49.000000 borgmatic-1.8.1/borgmatic/execute.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-08-04 04:56:36.056554 borgmatic-1.8.1/borgmatic/hooks/
+-rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-07-10 00:33:30.000000 borgmatic-1.8.1/borgmatic/hooks/__init__.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     3276 2023-06-27 21:37:40.000000 borgmatic-1.8.1/borgmatic/hooks/command.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1929 2023-07-22 17:14:49.000000 borgmatic-1.8.1/borgmatic/hooks/cronhub.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1810 2023-07-22 17:14:49.000000 borgmatic-1.8.1/borgmatic/hooks/cronitor.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     3203 2023-07-22 17:14:49.000000 borgmatic-1.8.1/borgmatic/hooks/dispatch.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     2387 2023-07-10 00:33:27.000000 borgmatic-1.8.1/borgmatic/hooks/dump.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     4896 2023-07-22 17:14:49.000000 borgmatic-1.8.1/borgmatic/hooks/healthchecks.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     7495 2023-07-22 17:14:49.000000 borgmatic-1.8.1/borgmatic/hooks/mongodb.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      180 2023-07-10 00:33:34.000000 borgmatic-1.8.1/borgmatic/hooks/monitor.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     9391 2023-07-22 17:14:49.000000 borgmatic-1.8.1/borgmatic/hooks/mysql.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     2852 2023-07-27 06:36:40.000000 borgmatic-1.8.1/borgmatic/hooks/ntfy.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     2606 2023-07-22 17:14:49.000000 borgmatic-1.8.1/borgmatic/hooks/pagerduty.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    12327 2023-07-22 17:14:49.000000 borgmatic-1.8.1/borgmatic/hooks/postgresql.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     5075 2023-07-22 17:14:49.000000 borgmatic-1.8.1/borgmatic/hooks/sqlite.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     7242 2023-07-10 16:39:03.000000 borgmatic-1.8.1/borgmatic/logger.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1048 2023-05-12 23:35:39.000000 borgmatic-1.8.1/borgmatic/signals.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      586 2023-07-10 16:39:03.000000 borgmatic-1.8.1/borgmatic/verbosity.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-08-04 04:56:36.046554 borgmatic-1.8.1/borgmatic.egg-info/
+-rw-r--r--   0 witten    (1000) witten    (1000)      682 2023-08-04 04:56:35.000000 borgmatic-1.8.1/borgmatic.egg-info/PKG-INFO
+-rw-r--r--   0 witten    (1000) witten    (1000)     8617 2023-08-04 04:56:35.000000 borgmatic-1.8.1/borgmatic.egg-info/SOURCES.txt
+-rw-r--r--   0 witten    (1000) witten    (1000)        1 2023-08-04 04:56:35.000000 borgmatic-1.8.1/borgmatic.egg-info/dependency_links.txt
+-rw-r--r--   0 witten    (1000) witten    (1000)      200 2023-08-04 04:56:35.000000 borgmatic-1.8.1/borgmatic.egg-info/entry_points.txt
+-rw-r--r--   0 witten    (1000) witten    (1000)       89 2023-08-04 04:56:35.000000 borgmatic-1.8.1/borgmatic.egg-info/requires.txt
+-rw-r--r--   0 witten    (1000) witten    (1000)       10 2023-08-04 04:56:35.000000 borgmatic-1.8.1/borgmatic.egg-info/top_level.txt
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-08-04 04:56:36.056554 borgmatic-1.8.1/docs/
+-rw-r--r--   0 witten    (1000) witten    (1000)     1544 2023-07-10 16:39:03.000000 borgmatic-1.8.1/docs/Dockerfile
+-rw-r--r--   0 witten    (1000) witten    (1000)     6650 2023-07-22 17:14:49.000000 borgmatic-1.8.1/docs/README.md
+-rw-r--r--   0 witten    (1000) witten    (1000)      672 2023-07-22 17:14:49.000000 borgmatic-1.8.1/docs/SECURITY.md
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-08-04 04:56:36.056554 borgmatic-1.8.1/docs/_data/
+-rw-r--r--   0 witten    (1000) witten    (1000)      112 2023-07-22 17:14:49.000000 borgmatic-1.8.1/docs/_data/borgmatic.js
+-rw-r--r--   0 witten    (1000) witten    (1000)       19 2021-06-08 17:56:16.000000 borgmatic-1.8.1/docs/_data/layout.json
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-08-04 04:56:36.056554 borgmatic-1.8.1/docs/_includes/
+-rw-r--r--   0 witten    (1000) witten    (1000)       52 2021-06-08 17:56:16.000000 borgmatic-1.8.1/docs/_includes/asciinema.css
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-08-04 04:56:36.056554 borgmatic-1.8.1/docs/_includes/components/
+-rw-r--r--   0 witten    (1000) witten    (1000)      492 2021-06-08 17:56:16.000000 borgmatic-1.8.1/docs/_includes/components/external-links.css
+-rw-r--r--   0 witten    (1000) witten    (1000)      636 2021-06-08 17:56:16.000000 borgmatic-1.8.1/docs/_includes/components/info-blocks.css
+-rw-r--r--   0 witten    (1000) witten    (1000)     5125 2023-06-27 21:37:40.000000 borgmatic-1.8.1/docs/_includes/components/lists.css
+-rw-r--r--   0 witten    (1000) witten    (1000)     1788 2023-06-27 21:37:40.000000 borgmatic-1.8.1/docs/_includes/components/minilink.css
+-rw-r--r--   0 witten    (1000) witten    (1000)      219 2023-07-22 17:14:49.000000 borgmatic-1.8.1/docs/_includes/components/suggestion-link.html
+-rw-r--r--   0 witten    (1000) witten    (1000)     1862 2023-06-27 21:37:40.000000 borgmatic-1.8.1/docs/_includes/components/toc.css
+-rw-r--r--   0 witten    (1000) witten    (1000)      265 2021-06-08 17:56:16.000000 borgmatic-1.8.1/docs/_includes/header.njk
+-rw-r--r--   0 witten    (1000) witten    (1000)    26340 2023-06-27 21:37:40.000000 borgmatic-1.8.1/docs/_includes/index.css
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-08-04 04:56:36.056554 borgmatic-1.8.1/docs/_includes/layouts/
+-rw-r--r--   0 witten    (1000) witten    (1000)      909 2023-06-27 21:37:40.000000 borgmatic-1.8.1/docs/_includes/layouts/base.njk
+-rw-r--r--   0 witten    (1000) witten    (1000)     1184 2023-07-22 17:14:49.000000 borgmatic-1.8.1/docs/_includes/layouts/main.njk
+-rw-r--r--   0 witten    (1000) witten    (1000)     3039 2023-05-12 23:35:39.000000 borgmatic-1.8.1/docs/_includes/prism-theme.css
+-rw-r--r--   0 witten    (1000) witten    (1000)      422 2023-07-22 17:14:49.000000 borgmatic-1.8.1/docs/docker-compose.yaml
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-08-04 04:56:36.059888 borgmatic-1.8.1/docs/how-to/
+-rw-r--r--   0 witten    (1000) witten    (1000)     5277 2023-07-22 17:14:49.000000 borgmatic-1.8.1/docs/how-to/add-preparation-and-cleanup-steps-to-backups.md
+-rw-r--r--   0 witten    (1000) witten    (1000)     5401 2023-07-22 17:14:49.000000 borgmatic-1.8.1/docs/how-to/backup-to-a-removable-drive-or-an-intermittent-server.md
+-rw-r--r--   0 witten    (1000) witten    (1000)    16460 2023-07-31 18:56:56.000000 borgmatic-1.8.1/docs/how-to/backup-your-databases.md
+-rw-r--r--   0 witten    (1000) witten    (1000)     7908 2023-07-22 17:14:49.000000 borgmatic-1.8.1/docs/how-to/deal-with-very-large-backups.md
+-rw-r--r--   0 witten    (1000) witten    (1000)     6240 2023-07-22 17:14:49.000000 borgmatic-1.8.1/docs/how-to/develop-on-borgmatic.md
+-rw-r--r--   0 witten    (1000) witten    (1000)     6004 2023-07-31 18:56:56.000000 borgmatic-1.8.1/docs/how-to/extract-a-backup.md
+-rw-r--r--   0 witten    (1000) witten    (1000)       77 2023-07-22 17:14:49.000000 borgmatic-1.8.1/docs/how-to/index.md
+-rw-r--r--   0 witten    (1000) witten    (1000)     6424 2023-07-22 17:14:49.000000 borgmatic-1.8.1/docs/how-to/inspect-your-backups.md
+-rw-r--r--   0 witten    (1000) witten    (1000)     2165 2023-07-22 17:14:49.000000 borgmatic-1.8.1/docs/how-to/make-backups-redundant.md
+-rw-r--r--   0 witten    (1000) witten    (1000)    20140 2023-08-02 04:47:09.000000 borgmatic-1.8.1/docs/how-to/make-per-application-backups.md
+-rw-r--r--   0 witten    (1000) witten    (1000)    14678 2023-07-27 06:36:52.000000 borgmatic-1.8.1/docs/how-to/monitor-your-backups.md
+-rw-r--r--   0 witten    (1000) witten    (1000)     3322 2023-07-22 17:14:49.000000 borgmatic-1.8.1/docs/how-to/provide-your-passwords.md
+-rw-r--r--   0 witten    (1000) witten    (1000)      124 2022-06-16 18:55:15.000000 borgmatic-1.8.1/docs/how-to/restore-a-backup.md
+-rw-r--r--   0 witten    (1000) witten    (1000)     5925 2023-07-22 17:14:49.000000 borgmatic-1.8.1/docs/how-to/run-arbitrary-borg-commands.md
+-rw-r--r--   0 witten    (1000) witten    (1000)      152 2022-06-16 18:55:21.000000 borgmatic-1.8.1/docs/how-to/run-preparation-steps-before-backups.md
+-rw-r--r--   0 witten    (1000) witten    (1000)    15838 2023-07-22 17:14:49.000000 borgmatic-1.8.1/docs/how-to/set-up-backups.md
+-rw-r--r--   0 witten    (1000) witten    (1000)     7636 2023-07-22 17:14:49.000000 borgmatic-1.8.1/docs/how-to/upgrade.md
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-08-04 04:56:36.059888 borgmatic-1.8.1/docs/reference/
+-rw-r--r--   0 witten    (1000) witten    (1000)      853 2023-07-22 17:14:49.000000 borgmatic-1.8.1/docs/reference/command-line.md
+-rw-r--r--   0 witten    (1000) witten    (1000)      810 2023-07-10 16:39:03.000000 borgmatic-1.8.1/docs/reference/configuration.md
+-rw-r--r--   0 witten    (1000) witten    (1000)       80 2023-07-22 17:14:49.000000 borgmatic-1.8.1/docs/reference/index.md
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-08-04 04:56:36.063221 borgmatic-1.8.1/docs/static/
+-rw-r--r--   0 witten    (1000) witten    (1000)     5822 2021-06-08 17:56:16.000000 borgmatic-1.8.1/docs/static/borgbase.png
+-rw-r--r--   0 witten    (1000) witten    (1000)     3593 2021-06-08 17:56:16.000000 borgmatic-1.8.1/docs/static/borgmatic.png
+-rw-r--r--   0 witten    (1000) witten    (1000)     1674 2021-06-08 17:56:16.000000 borgmatic-1.8.1/docs/static/borgmatic.svg
+-rw-r--r--   0 witten    (1000) witten    (1000)    23536 2021-06-08 17:56:16.000000 borgmatic-1.8.1/docs/static/cronhub.png
+-rw-r--r--   0 witten    (1000) witten    (1000)    10364 2021-06-08 17:56:16.000000 borgmatic-1.8.1/docs/static/cronitor.png
+-rw-r--r--   0 witten    (1000) witten    (1000)     4556 2021-06-08 17:56:16.000000 borgmatic-1.8.1/docs/static/healthchecks.png
+-rw-r--r--   0 witten    (1000) witten    (1000)     9474 2021-06-08 17:56:16.000000 borgmatic-1.8.1/docs/static/mariadb.png
+-rw-r--r--   0 witten    (1000) witten    (1000)    12839 2023-05-12 23:35:39.000000 borgmatic-1.8.1/docs/static/mongodb.png
+-rw-r--r--   0 witten    (1000) witten    (1000)     3761 2021-06-08 17:56:16.000000 borgmatic-1.8.1/docs/static/mysql.png
+-rw-r--r--   0 witten    (1000) witten    (1000)    10266 2023-05-12 23:35:39.000000 borgmatic-1.8.1/docs/static/ntfy.png
+-rw-r--r--   0 witten    (1000) witten    (1000)    20107 2023-05-12 23:35:39.000000 borgmatic-1.8.1/docs/static/pagerduty.png
+-rw-r--r--   0 witten    (1000) witten    (1000)    31528 2021-06-08 17:56:16.000000 borgmatic-1.8.1/docs/static/postgresql.png
+-rw-r--r--   0 witten    (1000) witten    (1000)     4668 2023-06-27 21:37:40.000000 borgmatic-1.8.1/docs/static/sqlite.png
+-rw-r--r--   0 witten    (1000) witten    (1000)       64 2023-04-15 02:33:57.000000 borgmatic-1.8.1/pyproject.toml
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-08-04 04:56:36.039887 borgmatic-1.8.1/sample/
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-08-04 04:56:36.063221 borgmatic-1.8.1/sample/cron/
+-rw-r--r--   0 witten    (1000) witten    (1000)      183 2023-05-12 23:35:39.000000 borgmatic-1.8.1/sample/cron/borgmatic
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-08-04 04:56:36.063221 borgmatic-1.8.1/sample/systemd/
+-rw-r--r--   0 witten    (1000) witten    (1000)      499 2023-07-10 16:39:03.000000 borgmatic-1.8.1/sample/systemd/borgmatic-user.service
+-rw-r--r--   0 witten    (1000) witten    (1000)      138 2023-06-14 21:55:41.000000 borgmatic-1.8.1/sample/systemd/borgmatic-user.timer
+-rw-r--r--   0 witten    (1000) witten    (1000)     2612 2023-07-10 16:39:03.000000 borgmatic-1.8.1/sample/systemd/borgmatic.service
+-rw-r--r--   0 witten    (1000) witten    (1000)      138 2023-06-14 21:55:41.000000 borgmatic-1.8.1/sample/systemd/borgmatic.timer
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-08-04 04:56:36.063221 borgmatic-1.8.1/scripts/
+-rwxr-xr-x   0 witten    (1000) witten    (1000)      259 2023-07-10 16:39:03.000000 borgmatic-1.8.1/scripts/dev-docs
+-rwxr-xr-x   0 witten    (1000) witten    (1000)     3108 2023-05-12 23:35:39.000000 borgmatic-1.8.1/scripts/find-unsupported-borg-options
+-rwxr-xr-x   0 witten    (1000) witten    (1000)      137 2021-06-08 17:56:16.000000 borgmatic-1.8.1/scripts/push
+-rwxr-xr-x   0 witten    (1000) witten    (1000)     1685 2023-07-10 16:39:03.000000 borgmatic-1.8.1/scripts/release
+-rwxr-xr-x   0 witten    (1000) witten    (1000)      658 2023-06-27 21:37:40.000000 borgmatic-1.8.1/scripts/run-end-to-end-dev-tests
+-rwxr-xr-x   0 witten    (1000) witten    (1000)     1334 2023-07-10 16:39:03.000000 borgmatic-1.8.1/scripts/run-full-tests
+-rw-r--r--   0 witten    (1000) witten    (1000)      505 2023-08-04 04:56:36.083221 borgmatic-1.8.1/setup.cfg
+-rw-r--r--   0 witten    (1000) witten    (1000)     1312 2023-08-04 04:55:34.000000 borgmatic-1.8.1/setup.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      818 2023-07-10 16:39:03.000000 borgmatic-1.8.1/test_requirements.txt
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-08-04 04:56:36.063221 borgmatic-1.8.1/tests/
+-rw-r--r--   0 witten    (1000) witten    (1000)        0 2021-06-08 17:56:16.000000 borgmatic-1.8.1/tests/__init__.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-08-04 04:56:36.066554 borgmatic-1.8.1/tests/end-to-end/
+-rw-r--r--   0 witten    (1000) witten    (1000)        0 2021-06-08 17:56:16.000000 borgmatic-1.8.1/tests/end-to-end/__init__.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1383 2023-07-10 16:39:03.000000 borgmatic-1.8.1/tests/end-to-end/docker-compose.yaml
+-rw-r--r--   0 witten    (1000) witten    (1000)     2981 2023-07-22 17:14:49.000000 borgmatic-1.8.1/tests/end-to-end/test_borgmatic.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      268 2023-07-14 02:24:28.000000 borgmatic-1.8.1/tests/end-to-end/test_completion.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    12221 2023-07-22 17:14:49.000000 borgmatic-1.8.1/tests/end-to-end/test_database.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1711 2023-07-14 02:24:16.000000 borgmatic-1.8.1/tests/end-to-end/test_dev_parity_with_build_server.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      588 2023-07-14 02:24:23.000000 borgmatic-1.8.1/tests/end-to-end/test_generate_config.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1980 2023-07-22 17:14:49.000000 borgmatic-1.8.1/tests/end-to-end/test_override.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1630 2023-07-22 17:14:49.000000 borgmatic-1.8.1/tests/end-to-end/test_validate_config.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-08-04 04:56:36.066554 borgmatic-1.8.1/tests/integration/
+-rw-r--r--   0 witten    (1000) witten    (1000)        0 2021-06-08 17:56:16.000000 borgmatic-1.8.1/tests/integration/__init__.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-08-04 04:56:36.066554 borgmatic-1.8.1/tests/integration/actions/
+-rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-07-10 16:39:03.000000 borgmatic-1.8.1/tests/integration/actions/__init__.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-08-04 04:56:36.066554 borgmatic-1.8.1/tests/integration/actions/config/
+-rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-07-10 16:39:03.000000 borgmatic-1.8.1/tests/integration/actions/config/__init__.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1088 2023-07-10 16:39:03.000000 borgmatic-1.8.1/tests/integration/actions/config/test_validate.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-08-04 04:56:36.066554 borgmatic-1.8.1/tests/integration/borg/
+-rw-r--r--   0 witten    (1000) witten    (1000)     5352 2023-07-22 17:14:49.000000 borgmatic-1.8.1/tests/integration/borg/test_commands.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      546 2023-05-12 23:35:39.000000 borgmatic-1.8.1/tests/integration/borg/test_feature.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-08-04 04:56:36.066554 borgmatic-1.8.1/tests/integration/commands/
+-rw-r--r--   0 witten    (1000) witten    (1000)        0 2021-06-08 17:56:16.000000 borgmatic-1.8.1/tests/integration/commands/__init__.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-08-04 04:56:36.066554 borgmatic-1.8.1/tests/integration/commands/completion/
+-rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-07-10 16:39:03.000000 borgmatic-1.8.1/tests/integration/commands/completion/__init__.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      811 2023-07-10 16:39:03.000000 borgmatic-1.8.1/tests/integration/commands/completion/test_actions.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      138 2023-07-10 16:39:03.000000 borgmatic-1.8.1/tests/integration/commands/completion/test_bash.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      138 2023-07-10 16:39:03.000000 borgmatic-1.8.1/tests/integration/commands/completion/test_fish.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    23211 2023-07-22 17:14:49.000000 borgmatic-1.8.1/tests/integration/commands/test_arguments.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      432 2023-04-15 02:32:17.000000 borgmatic-1.8.1/tests/integration/commands/test_borgmatic.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      214 2023-07-10 16:39:03.000000 borgmatic-1.8.1/tests/integration/commands/test_generate_config.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      214 2023-07-10 16:39:03.000000 borgmatic-1.8.1/tests/integration/commands/test_validate_config.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-08-04 04:56:36.069887 borgmatic-1.8.1/tests/integration/config/
+-rw-r--r--   0 witten    (1000) witten    (1000)        0 2021-06-08 17:56:16.000000 borgmatic-1.8.1/tests/integration/config/__init__.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     8563 2023-07-22 17:14:49.000000 borgmatic-1.8.1/tests/integration/config/test_generate.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    43449 2023-08-02 04:47:09.000000 borgmatic-1.8.1/tests/integration/config/test_load.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1039 2023-05-12 23:35:39.000000 borgmatic-1.8.1/tests/integration/config/test_override.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      234 2023-05-12 23:35:39.000000 borgmatic-1.8.1/tests/integration/config/test_schema.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     7184 2023-08-02 04:47:09.000000 borgmatic-1.8.1/tests/integration/config/test_validate.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-08-04 04:56:36.069887 borgmatic-1.8.1/tests/integration/hooks/
+-rw-r--r--   0 witten    (1000) witten    (1000)      753 2023-07-22 17:14:49.000000 borgmatic-1.8.1/tests/integration/hooks/test_healthchecks.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    11256 2023-06-27 21:37:40.000000 borgmatic-1.8.1/tests/integration/test_execute.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-08-04 04:56:36.069887 borgmatic-1.8.1/tests/unit/
+-rw-r--r--   0 witten    (1000) witten    (1000)        0 2021-06-08 17:56:16.000000 borgmatic-1.8.1/tests/unit/__init__.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-08-04 04:56:36.073221 borgmatic-1.8.1/tests/unit/actions/
+-rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-05-12 23:35:39.000000 borgmatic-1.8.1/tests/unit/actions/__init__.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-08-04 04:56:36.073221 borgmatic-1.8.1/tests/unit/actions/config/
+-rw-r--r--   0 witten    (1000) witten    (1000)     4024 2023-07-10 16:39:03.000000 borgmatic-1.8.1/tests/unit/actions/config/test_bootstrap.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1305 2023-07-10 16:39:03.000000 borgmatic-1.8.1/tests/unit/actions/config/test_generate.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      599 2023-07-10 16:39:03.000000 borgmatic-1.8.1/tests/unit/actions/config/test_validate.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      390 2023-07-10 16:39:03.000000 borgmatic-1.8.1/tests/unit/actions/test_arguments.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      821 2023-07-22 17:14:49.000000 borgmatic-1.8.1/tests/unit/actions/test_borg.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      682 2023-07-22 17:14:49.000000 borgmatic-1.8.1/tests/unit/actions/test_break_lock.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     2847 2023-07-22 17:14:49.000000 borgmatic-1.8.1/tests/unit/actions/test_check.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     3049 2023-07-22 17:14:49.000000 borgmatic-1.8.1/tests/unit/actions/test_compact.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     7475 2023-07-31 21:01:08.000000 borgmatic-1.8.1/tests/unit/actions/test_create.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      967 2023-07-22 17:14:49.000000 borgmatic-1.8.1/tests/unit/actions/test_export_tar.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1074 2023-07-22 17:14:49.000000 borgmatic-1.8.1/tests/unit/actions/test_extract.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      993 2023-07-22 17:14:49.000000 borgmatic-1.8.1/tests/unit/actions/test_info.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      984 2023-07-22 17:14:49.000000 borgmatic-1.8.1/tests/unit/actions/test_list.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      824 2023-07-22 17:14:49.000000 borgmatic-1.8.1/tests/unit/actions/test_mount.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     2609 2023-07-22 17:14:49.000000 borgmatic-1.8.1/tests/unit/actions/test_prune.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1748 2023-07-22 17:14:49.000000 borgmatic-1.8.1/tests/unit/actions/test_rcreate.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    19198 2023-07-22 17:14:49.000000 borgmatic-1.8.1/tests/unit/actions/test_restore.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      743 2023-07-22 17:14:49.000000 borgmatic-1.8.1/tests/unit/actions/test_rinfo.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      721 2023-07-22 17:14:49.000000 borgmatic-1.8.1/tests/unit/actions/test_rlist.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      630 2023-07-22 17:14:49.000000 borgmatic-1.8.1/tests/unit/actions/test_transfer.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-08-04 04:56:36.076554 borgmatic-1.8.1/tests/unit/borg/
+-rw-r--r--   0 witten    (1000) witten    (1000)        0 2021-06-08 17:56:16.000000 borgmatic-1.8.1/tests/unit/borg/__init__.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    10406 2023-07-22 17:14:49.000000 borgmatic-1.8.1/tests/unit/borg/test_borg.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     3332 2023-07-22 17:14:49.000000 borgmatic-1.8.1/tests/unit/borg/test_break_lock.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    39722 2023-07-22 17:14:49.000000 borgmatic-1.8.1/tests/unit/borg/test_check.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     6675 2023-07-22 17:14:49.000000 borgmatic-1.8.1/tests/unit/borg/test_compact.py
+-rw-r--r--   0 witten    (1000) witten    (1000)   128726 2023-07-31 21:01:10.000000 borgmatic-1.8.1/tests/unit/borg/test_create.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1988 2023-07-22 22:21:03.000000 borgmatic-1.8.1/tests/unit/borg/test_environment.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    11144 2023-07-22 17:14:49.000000 borgmatic-1.8.1/tests/unit/borg/test_export_tar.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    19818 2023-07-22 17:14:49.000000 borgmatic-1.8.1/tests/unit/borg/test_extract.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     5084 2023-08-02 17:19:11.000000 borgmatic-1.8.1/tests/unit/borg/test_flags.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    24164 2023-07-22 17:14:49.000000 borgmatic-1.8.1/tests/unit/borg/test_info.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    25878 2023-07-22 17:14:49.000000 borgmatic-1.8.1/tests/unit/borg/test_list.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    10756 2023-07-22 17:14:49.000000 borgmatic-1.8.1/tests/unit/borg/test_mount.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    15671 2023-07-22 17:25:15.000000 borgmatic-1.8.1/tests/unit/borg/test_prune.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    12524 2023-07-22 17:14:49.000000 borgmatic-1.8.1/tests/unit/borg/test_rcreate.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    11325 2023-07-22 17:14:49.000000 borgmatic-1.8.1/tests/unit/borg/test_rinfo.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    23462 2023-07-22 17:14:49.000000 borgmatic-1.8.1/tests/unit/borg/test_rlist.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    20749 2023-07-22 17:14:49.000000 borgmatic-1.8.1/tests/unit/borg/test_transfer.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      920 2023-07-07 06:06:19.000000 borgmatic-1.8.1/tests/unit/borg/test_umount.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     2112 2023-07-22 17:14:49.000000 borgmatic-1.8.1/tests/unit/borg/test_version.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-08-04 04:56:36.076554 borgmatic-1.8.1/tests/unit/commands/
+-rw-r--r--   0 witten    (1000) witten    (1000)        0 2021-06-08 17:56:16.000000 borgmatic-1.8.1/tests/unit/commands/__init__.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-08-04 04:56:36.076554 borgmatic-1.8.1/tests/unit/commands/completion/
+-rw-r--r--   0 witten    (1000) witten    (1000)        0 2023-07-10 16:39:03.000000 borgmatic-1.8.1/tests/unit/commands/completion/__init__.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      226 2023-07-10 16:39:03.000000 borgmatic-1.8.1/tests/unit/commands/completion/test_actions.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      431 2023-07-10 16:39:03.000000 borgmatic-1.8.1/tests/unit/commands/completion/test_bash.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     4616 2023-07-10 16:39:03.000000 borgmatic-1.8.1/tests/unit/commands/completion/test_fish.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    17204 2023-08-01 21:00:45.000000 borgmatic-1.8.1/tests/unit/commands/test_arguments.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    49716 2023-07-22 17:14:49.000000 borgmatic-1.8.1/tests/unit/commands/test_borgmatic.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-08-04 04:56:36.079888 borgmatic-1.8.1/tests/unit/config/
+-rw-r--r--   0 witten    (1000) witten    (1000)        0 2021-06-08 17:56:16.000000 borgmatic-1.8.1/tests/unit/config/__init__.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      709 2023-04-15 02:32:17.000000 borgmatic-1.8.1/tests/unit/config/test_checks.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     8085 2023-07-10 16:39:03.000000 borgmatic-1.8.1/tests/unit/config/test_collect.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     3090 2023-06-27 21:37:40.000000 borgmatic-1.8.1/tests/unit/config/test_environment.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     4980 2023-07-22 17:14:49.000000 borgmatic-1.8.1/tests/unit/config/test_generate.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1390 2023-08-02 04:47:09.000000 borgmatic-1.8.1/tests/unit/config/test_load.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     7171 2023-08-02 04:47:09.000000 borgmatic-1.8.1/tests/unit/config/test_normalize.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     3804 2023-07-22 17:14:49.000000 borgmatic-1.8.1/tests/unit/config/test_override.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     7837 2023-07-22 17:14:49.000000 borgmatic-1.8.1/tests/unit/config/test_validate.py
+drwxr-xr-x   0 witten    (1000) witten    (1000)        0 2023-08-04 04:56:36.083221 borgmatic-1.8.1/tests/unit/hooks/
+-rw-r--r--   0 witten    (1000) witten    (1000)        0 2021-06-08 17:56:16.000000 borgmatic-1.8.1/tests/unit/hooks/__init__.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     3920 2023-07-01 23:41:53.000000 borgmatic-1.8.1/tests/unit/hooks/test_command.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     3726 2023-07-22 17:14:49.000000 borgmatic-1.8.1/tests/unit/hooks/test_cronhub.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     3162 2023-07-22 17:14:49.000000 borgmatic-1.8.1/tests/unit/hooks/test_cronitor.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     4490 2023-07-22 17:14:49.000000 borgmatic-1.8.1/tests/unit/hooks/test_dispatch.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     2938 2023-05-12 23:35:39.000000 borgmatic-1.8.1/tests/unit/hooks/test_dump.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    11731 2023-07-22 17:14:49.000000 borgmatic-1.8.1/tests/unit/hooks/test_healthchecks.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    17940 2023-07-22 17:14:49.000000 borgmatic-1.8.1/tests/unit/hooks/test_mongodb.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    20116 2023-07-22 17:14:49.000000 borgmatic-1.8.1/tests/unit/hooks/test_mysql.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     7411 2023-07-27 06:36:13.000000 borgmatic-1.8.1/tests/unit/hooks/test_ntfy.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     2303 2023-07-22 17:14:49.000000 borgmatic-1.8.1/tests/unit/hooks/test_pagerduty.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    38402 2023-07-22 17:14:49.000000 borgmatic-1.8.1/tests/unit/hooks/test_postgresql.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     7431 2023-07-22 17:14:49.000000 borgmatic-1.8.1/tests/unit/hooks/test_sqlite.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    18294 2023-06-27 21:37:40.000000 borgmatic-1.8.1/tests/unit/test_execute.py
+-rw-r--r--   0 witten    (1000) witten    (1000)    16634 2023-07-10 16:39:03.000000 borgmatic-1.8.1/tests/unit/test_logger.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1405 2023-05-12 23:35:39.000000 borgmatic-1.8.1/tests/unit/test_signals.py
+-rw-r--r--   0 witten    (1000) witten    (1000)     1426 2023-07-10 16:39:03.000000 borgmatic-1.8.1/tests/unit/test_verbosity.py
+-rw-r--r--   0 witten    (1000) witten    (1000)      838 2023-06-27 21:37:40.000000 borgmatic-1.8.1/tox.ini
```

### Comparing `borgmatic-1.8.0/.drone.yml` & `borgmatic-1.8.1/.drone.yml`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/.eleventy.js` & `borgmatic-1.8.1/.eleventy.js`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/.gitea/issue_template/bug_template.yaml` & `borgmatic-1.8.1/.gitea/issue_template/bug_template.yaml`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/AUTHORS` & `borgmatic-1.8.1/AUTHORS`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/LICENSE` & `borgmatic-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/NEWS` & `borgmatic-1.8.1/NEWS`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+1.8.1
+ * #326: Add documentation for restoring a database to an alternate host:
+   https://torsion.org/borgmatic/docs/how-to/backup-your-databases/#restore-to-an-alternate-host
+ * #697: Add documentation for "bootstrap" action:
+   https://torsion.org/borgmatic/docs/how-to/extract-a-backup/#extract-the-configuration-files-used-to-create-an-archive
+ * #725: Add "store_config_files" option for disabling the automatic backup of configuration files
+   used by the "config bootstrap" action.
+ * #728: Fix for "prune" action error when using the "keep_exclude_tags" option.
+ * #730: Fix for Borg's interactive prompt on the "check --repair" action automatically getting
+   answered "NO" even when the "check_i_know_what_i_am_doing" option isn't set.
+ * #732: Include multiple configuration files with a single "!include". See the documentation for
+   more information:
+   https://torsion.org/borgmatic/docs/how-to/make-per-application-backups/#multiple-merge-includes
+ * #734: Omit "--glob-archives" or "--match-archives" Borg flag when its value would be "*" (meaning
+   all archives).
+
 1.8.0
  * #575: BREAKING: For the "borgmatic borg" action, instead of implicitly injecting
    repository/archive into the resulting Borg command-line, pass repository to Borg via an
    environment variable and make archive available for explicit use in your commands. See the
    documentation for more information:
    https://torsion.org/borgmatic/docs/how-to/run-arbitrary-borg-commands/
  * #719: Fix an error when running "borg key export" through borgmatic.
```

### Comparing `borgmatic-1.8.0/PKG-INFO` & `borgmatic-1.8.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: borgmatic
-Version: 1.8.0
+Version: 1.8.1
 Summary: Simple, configuration-driven backup software for servers and workstations
 Home-page: https://torsion.org/borgmatic
 Author: Dan Helfman
 Author-email: witten@torsion.org
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: System Administrators
```

### Comparing `borgmatic-1.8.0/README.md` & `borgmatic-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/SECURITY.md` & `borgmatic-1.8.1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/borgmatic/actions/borg.py` & `borgmatic-1.8.1/borgmatic/actions/borg.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/borgmatic/actions/break_lock.py` & `borgmatic-1.8.1/borgmatic/actions/break_lock.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/borgmatic/actions/check.py` & `borgmatic-1.8.1/borgmatic/actions/check.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/borgmatic/actions/compact.py` & `borgmatic-1.8.1/borgmatic/actions/compact.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/borgmatic/actions/config/bootstrap.py` & `borgmatic-1.8.1/borgmatic/actions/config/bootstrap.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/borgmatic/actions/config/generate.py` & `borgmatic-1.8.1/borgmatic/actions/config/generate.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/borgmatic/actions/config/validate.py` & `borgmatic-1.8.1/borgmatic/actions/config/validate.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/borgmatic/actions/create.py` & `borgmatic-1.8.1/borgmatic/actions/create.py`

 * *Files 5% similar despite different names*

```diff
@@ -87,15 +87,18 @@
     active_dumps = borgmatic.hooks.dispatch.call_hooks(
         'dump_databases',
         config,
         repository['path'],
         borgmatic.hooks.dump.DATABASE_HOOK_NAMES,
         global_arguments.dry_run,
     )
-    create_borgmatic_manifest(config, global_arguments.used_config_paths, global_arguments.dry_run)
+    if config.get('store_config_files', True):
+        create_borgmatic_manifest(
+            config, global_arguments.used_config_paths, global_arguments.dry_run
+        )
     stream_processes = [process for processes in active_dumps.values() for process in processes]
 
     json_output = borgmatic.borg.create.create_archive(
         global_arguments.dry_run,
         repository['path'],
         config,
         local_borg_version,
```

### Comparing `borgmatic-1.8.0/borgmatic/actions/export_tar.py` & `borgmatic-1.8.1/borgmatic/actions/export_tar.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/borgmatic/actions/extract.py` & `borgmatic-1.8.1/borgmatic/actions/extract.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/borgmatic/actions/info.py` & `borgmatic-1.8.1/borgmatic/actions/info.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/borgmatic/actions/list.py` & `borgmatic-1.8.1/borgmatic/actions/list.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/borgmatic/actions/mount.py` & `borgmatic-1.8.1/borgmatic/actions/mount.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/borgmatic/actions/prune.py` & `borgmatic-1.8.1/borgmatic/actions/prune.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/borgmatic/actions/rcreate.py` & `borgmatic-1.8.1/borgmatic/actions/rcreate.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/borgmatic/actions/restore.py` & `borgmatic-1.8.1/borgmatic/actions/restore.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/borgmatic/actions/rinfo.py` & `borgmatic-1.8.1/borgmatic/actions/rinfo.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/borgmatic/actions/rlist.py` & `borgmatic-1.8.1/borgmatic/actions/rlist.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/borgmatic/actions/transfer.py` & `borgmatic-1.8.1/borgmatic/actions/transfer.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/borgmatic/borg/borg.py` & `borgmatic-1.8.1/borgmatic/borg/borg.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/borgmatic/borg/break_lock.py` & `borgmatic-1.8.1/borgmatic/borg/break_lock.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/borgmatic/borg/check.py` & `borgmatic-1.8.1/borgmatic/borg/check.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,15 @@
             continue
 
         # If we've not yet reached the time when the frequency dictates we're ready for another
         # check, skip this check.
         if datetime.datetime.now() < check_time + frequency_delta:
             remaining = check_time + frequency_delta - datetime.datetime.now()
             logger.info(
-                f'Skipping {check} check due to configured frequency; {remaining} until next check'
+                f'Skipping {check} check due to configured frequency; {remaining} until next check (use --force to check anyway)'
             )
             filtered_checks.remove(check)
 
     return tuple(filtered_checks)
 
 
 def make_archive_filter_flags(local_borg_version, config, checks, check_last=None, prefix=None):
```

### Comparing `borgmatic-1.8.0/borgmatic/borg/compact.py` & `borgmatic-1.8.1/borgmatic/borg/compact.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/borgmatic/borg/create.py` & `borgmatic-1.8.1/borgmatic/borg/create.py`

 * *Files 0% similar despite different names*

```diff
@@ -350,15 +350,19 @@
     if config.get('source_directories_must_exist', False):
         check_all_source_directories_exist(config.get('source_directories'))
     sources = deduplicate_directories(
         map_directories_to_devices(
             expand_directories(
                 tuple(config.get('source_directories', ()))
                 + borgmatic_source_directories
-                + tuple(global_arguments.used_config_paths)
+                + tuple(
+                    global_arguments.used_config_paths
+                    if config.get('store_config_files', True)
+                    else ()
+                )
             )
         ),
         additional_directory_devices=map_directories_to_devices(
             expand_directories(pattern_root_directories(config.get('patterns')))
         ),
     )
```

### Comparing `borgmatic-1.8.0/borgmatic/borg/environment.py` & `borgmatic-1.8.1/borgmatic/borg/environment.py`

 * *Files 11% similar despite different names*

```diff
@@ -34,18 +34,20 @@
         if value:
             environment[environment_variable_name] = str(value)
 
     for (
         option_name,
         environment_variable_name,
     ) in DEFAULT_BOOL_OPTION_TO_DOWNCASE_ENVIRONMENT_VARIABLE.items():
-        value = config.get(option_name, False)
-        environment[environment_variable_name] = 'yes' if value else 'no'
+        value = config.get(option_name)
+        if value is not None:
+            environment[environment_variable_name] = 'yes' if value else 'no'
 
     for (
         option_name,
         environment_variable_name,
     ) in DEFAULT_BOOL_OPTION_TO_UPPERCASE_ENVIRONMENT_VARIABLE.items():
-        value = config.get(option_name, False)
-        environment[environment_variable_name] = 'YES' if value else 'NO'
+        value = config.get(option_name)
+        if value is not None:
+            environment[environment_variable_name] = 'YES' if value else 'NO'
 
     return environment
```

### Comparing `borgmatic-1.8.0/borgmatic/borg/export_tar.py` & `borgmatic-1.8.1/borgmatic/borg/export_tar.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/borgmatic/borg/extract.py` & `borgmatic-1.8.1/borgmatic/borg/extract.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/borgmatic/borg/feature.py` & `borgmatic-1.8.1/borgmatic/borg/feature.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/borgmatic/borg/flags.py` & `borgmatic-1.8.1/borgmatic/borg/flags.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,11 +73,14 @@
             return ('--glob-archives', re.sub(r'^sh:', '', match_archives))
 
     if not archive_name_format:
         return ()
 
     derived_match_archives = re.sub(r'\{(now|utcnow|pid)([:%\w\.-]*)\}', '*', archive_name_format)
 
+    if derived_match_archives == '*':
+        return ()
+
     if feature.available(feature.Feature.MATCH_ARCHIVES, local_borg_version):
         return ('--match-archives', f'sh:{derived_match_archives}')
     else:
         return ('--glob-archives', f'{derived_match_archives}')
```

### Comparing `borgmatic-1.8.0/borgmatic/borg/info.py` & `borgmatic-1.8.1/borgmatic/borg/info.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/borgmatic/borg/list.py` & `borgmatic-1.8.1/borgmatic/borg/list.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/borgmatic/borg/mount.py` & `borgmatic-1.8.1/borgmatic/borg/mount.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/borgmatic/borg/prune.py` & `borgmatic-1.8.1/borgmatic/borg/prune.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,15 +22,15 @@
             ('--keep-weekly', '4'),
             ('--keep-monthly', '6'),
         )
     '''
     flag_pairs = (
         ('--' + option_name.replace('_', '-'), str(value))
         for option_name, value in config.items()
-        if option_name.startswith('keep_')
+        if option_name.startswith('keep_') and option_name != 'keep_exclude_tags'
     )
     prefix = config.get('prefix')
 
     return tuple(element for pair in flag_pairs for element in pair) + (
         (
             ('--match-archives', f'sh:{prefix}*')
             if feature.available(feature.Feature.MATCH_ARCHIVES, local_borg_version)
```

### Comparing `borgmatic-1.8.0/borgmatic/borg/rcreate.py` & `borgmatic-1.8.1/borgmatic/borg/rcreate.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/borgmatic/borg/rinfo.py` & `borgmatic-1.8.1/borgmatic/borg/rinfo.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/borgmatic/borg/rlist.py` & `borgmatic-1.8.1/borgmatic/borg/rlist.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/borgmatic/borg/transfer.py` & `borgmatic-1.8.1/borgmatic/borg/transfer.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/borgmatic/borg/umount.py` & `borgmatic-1.8.1/borgmatic/borg/umount.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/borgmatic/borg/version.py` & `borgmatic-1.8.1/borgmatic/borg/version.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/borgmatic/commands/arguments.py` & `borgmatic-1.8.1/borgmatic/commands/arguments.py`

 * *Files 0% similar despite different names*

```diff
@@ -327,17 +327,16 @@
         default=False,
         action='store_true',
         help='Display installed version number of borgmatic and exit',
     )
 
     global_plus_action_parser = ArgumentParser(
         description='''
-            Simple, configuration-driven backup software for servers and workstations. If none of
-            the action options are given, then borgmatic defaults to: create, prune, compact, and
-            check.
+            Simple, configuration-driven backup software for servers and workstations. If no actions
+            are given, then borgmatic defaults to: create, prune, compact, and check.
             ''',
         parents=[global_parser],
     )
 
     action_parsers = global_plus_action_parser.add_subparsers(
         title='actions',
         metavar='',
```

### Comparing `borgmatic-1.8.0/borgmatic/commands/borgmatic.py` & `borgmatic-1.8.1/borgmatic/commands/borgmatic.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/borgmatic/commands/completion/actions.py` & `borgmatic-1.8.1/borgmatic/commands/completion/actions.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/borgmatic/commands/completion/bash.py` & `borgmatic-1.8.1/borgmatic/commands/completion/bash.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/borgmatic/commands/completion/fish.py` & `borgmatic-1.8.1/borgmatic/commands/completion/fish.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/borgmatic/config/collect.py` & `borgmatic-1.8.1/borgmatic/config/collect.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/borgmatic/config/environment.py` & `borgmatic-1.8.1/borgmatic/config/environment.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/borgmatic/config/generate.py` & `borgmatic-1.8.1/borgmatic/config/generate.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/borgmatic/config/load.py` & `borgmatic-1.8.1/borgmatic/config/load.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,80 @@
 import functools
+import itertools
 import json
 import logging
+import operator
 import os
 
 import ruamel.yaml
 
 logger = logging.getLogger(__name__)
 
 
+def probe_and_include_file(filename, include_directories):
+    '''
+    Given a filename to include and a list of include directories to search for matching files,
+    probe for the file, load it, and return the loaded configuration as a data structure of nested
+    dicts, lists, etc.
+
+    Raise FileNotFoundError if the included file was not found.
+    '''
+    expanded_filename = os.path.expanduser(filename)
+
+    if os.path.isabs(expanded_filename):
+        return load_configuration(expanded_filename)
+
+    candidate_filenames = {
+        os.path.join(directory, expanded_filename) for directory in include_directories
+    }
+
+    for candidate_filename in candidate_filenames:
+        if os.path.exists(candidate_filename):
+            return load_configuration(candidate_filename)
+
+    raise FileNotFoundError(
+        f'Could not find include {filename} at {" or ".join(candidate_filenames)}'
+    )
+
+
 def include_configuration(loader, filename_node, include_directory):
     '''
-    Given a ruamel.yaml.loader.Loader, a ruamel.yaml.serializer.ScalarNode containing the included
-    filename, and an include directory path to search for matching files, load the given YAML
-    filename (ignoring the given loader so we can use our own) and return its contents as a data
-    structure of nested dicts and lists. If the filename is relative, probe for it within 1. the
-    current working directory and 2. the given include directory.
+    Given a ruamel.yaml.loader.Loader, a ruamel.yaml.nodes.ScalarNode containing the included
+    filename (or a list containing multiple such filenames), and an include directory path to search
+    for matching files, load the given YAML filenames (ignoring the given loader so we can use our
+    own) and return their contents as data structure of nested dicts, lists, etc. If the given
+    filename node's value is a scalar string, then the return value will be a single value. But if
+    the given node value is a list, then the return value will be a list of values, one per loaded
+    configuration file.
+
+    If a filename is relative, probe for it within 1. the current working directory and 2. the given
+    include directory.
 
     Raise FileNotFoundError if an included file was not found.
     '''
     include_directories = [os.getcwd(), os.path.abspath(include_directory)]
-    include_filename = os.path.expanduser(filename_node.value)
 
-    if not os.path.isabs(include_filename):
-        candidate_filenames = [
-            os.path.join(directory, include_filename) for directory in include_directories
-        ]
+    if isinstance(filename_node.value, str):
+        return probe_and_include_file(filename_node.value, include_directories)
 
-        for candidate_filename in candidate_filenames:
-            if os.path.exists(candidate_filename):
-                include_filename = candidate_filename
-                break
-        else:
-            raise FileNotFoundError(
-                f'Could not find include {filename_node.value} at {" or ".join(candidate_filenames)}'
-            )
+    if (
+        isinstance(filename_node.value, list)
+        and len(filename_node.value)
+        and isinstance(filename_node.value[0], ruamel.yaml.nodes.ScalarNode)
+    ):
+        # Reversing the values ensures the correct ordering if these includes are subsequently
+        # merged together.
+        return [
+            probe_and_include_file(node.value, include_directories)
+            for node in reversed(filename_node.value)
+        ]
 
-    return load_configuration(include_filename)
+    raise ValueError(
+        '!include value is not supported; use a single filename or a list of filenames'
+    )
 
 
 def raise_retain_node_error(loader, node):
     '''
     Given a ruamel.yaml.loader.Loader and a YAML node, raise an error about "!retain" usage.
 
     Raise ValueError if a mapping or sequence node is given, as that indicates that "!retain" was
@@ -49,68 +84,77 @@
     Also raise ValueError if a scalar node is given, as "!retain" is not supported on scalar nodes.
     '''
     if isinstance(node, (ruamel.yaml.nodes.MappingNode, ruamel.yaml.nodes.SequenceNode)):
         raise ValueError(
             'The !retain tag may only be used within a configuration file containing a merged !include tag.'
         )
 
-    raise ValueError('The !retain tag may only be used on a YAML mapping or sequence.')
+    raise ValueError('The !retain tag may only be used on a mapping or list.')
 
 
 def raise_omit_node_error(loader, node):
     '''
     Given a ruamel.yaml.loader.Loader and a YAML node, raise an error about "!omit" usage.
 
     Raise ValueError unconditionally, as an "!omit" node here indicates it was used in a
     configuration file without a merge. In configuration files with a merge, nodes with "!omit"
     tags are handled by deep_merge_nodes() below.
     '''
     raise ValueError(
-        'The !omit tag may only be used on a scalar (e.g., string) list element within a configuration file containing a merged !include tag.'
+        'The !omit tag may only be used on a scalar (e.g., string) or list element within a configuration file containing a merged !include tag.'
     )
 
 
 class Include_constructor(ruamel.yaml.SafeConstructor):
     '''
     A YAML "constructor" (a ruamel.yaml concept) that supports a custom "!include" tag for including
-    separate YAML configuration files. Example syntax: `retention: !include common.yaml`
+    separate YAML configuration files. Example syntax: `option: !include common.yaml`
     '''
 
     def __init__(self, preserve_quotes=None, loader=None, include_directory=None):
         super(Include_constructor, self).__init__(preserve_quotes, loader)
         self.add_constructor(
             '!include',
             functools.partial(include_configuration, include_directory=include_directory),
         )
+
+        # These are catch-all error handlers for tags that don't get applied and removed by
+        # deep_merge_nodes() below.
         self.add_constructor('!retain', raise_retain_node_error)
         self.add_constructor('!omit', raise_omit_node_error)
 
     def flatten_mapping(self, node):
         '''
         Support the special case of deep merging included configuration into an existing mapping
         using the YAML '<<' merge key. Example syntax:
 
         ```
-        retention:
-            keep_daily: 1
+        option:
+            sub_option: 1
 
         <<: !include common.yaml
         ```
 
         These includes are deep merged into the current configuration file. For instance, in this
         example, any "option" with sub-options in common.yaml will get merged into the corresponding
         "option" with sub-options in the example configuration file.
         '''
         representer = ruamel.yaml.representer.SafeRepresenter()
 
         for index, (key_node, value_node) in enumerate(node.value):
             if key_node.tag == u'tag:yaml.org,2002:merge' and value_node.tag == '!include':
-                included_value = representer.represent_data(self.construct_object(value_node))
-                node.value[index] = (key_node, included_value)
+                # Replace the merge include with a sequence of included configuration nodes ready
+                # for merging. The construct_object() call here triggers include_configuration()
+                # among other constructors.
+                node.value[index] = (
+                    key_node,
+                    representer.represent_data(self.construct_object(value_node)),
+                )
 
+        # This super().flatten_mapping() call actually performs "<<" merges.
         super(Include_constructor, self).flatten_mapping(node)
 
         node.value = deep_merge_nodes(node.value)
 
 
 def load_configuration(filename):
     '''
@@ -134,160 +178,211 @@
     yaml = ruamel.yaml.YAML(typ='safe')
     yaml.Constructor = Include_constructor_with_include_directory
 
     with open(filename) as file:
         file_contents = file.read()
         config = yaml.load(file_contents)
 
-        if config and 'constants' in config:
+        try:
+            has_constants = bool(config and 'constants' in config)
+        except TypeError:
+            has_constants = False
+
+        if has_constants:
             for key, value in config['constants'].items():
                 value = json.dumps(value)
                 file_contents = file_contents.replace(f'{{{key}}}', value.strip('"'))
 
             config = yaml.load(file_contents)
             del config['constants']
 
         return config
 
 
-def filter_omitted_nodes(nodes):
+def filter_omitted_nodes(nodes, values):
     '''
-    Given a list of nodes, return a filtered list omitting any nodes with an "!omit" tag or with a
-    value matching such nodes.
+    Given a nested borgmatic configuration data structure as a list of tuples in the form of:
+
+    [
+        (
+            ruamel.yaml.nodes.ScalarNode as a key,
+            ruamel.yaml.nodes.MappingNode or other Node as a value,
+        ),
+        ...
+    ]
+
+    ... and a combined list of all values for those nodes, return a filtered list of the values,
+    omitting any that have an "!omit" tag (or with a value matching such nodes).
+
+    But if only a single node is given, bail and return the given values unfiltered, as "!omit" only
+    applies when there are merge includes (and therefore multiple nodes).
     '''
-    omitted_values = tuple(node.value for node in nodes if node.tag == '!omit')
+    if len(nodes) <= 1:
+        return values
 
-    return [node for node in nodes if node.value not in omitted_values]
+    omitted_values = tuple(node.value for node in values if node.tag == '!omit')
 
+    return [node for node in values if node.value not in omitted_values]
 
-DELETED_NODE = object()
+
+def merge_values(nodes):
+    '''
+    Given a nested borgmatic configuration data structure as a list of tuples in the form of:
+
+    [
+        (
+            ruamel.yaml.nodes.ScalarNode as a key,
+            ruamel.yaml.nodes.MappingNode or other Node as a value,
+        ),
+        ...
+    ]
+
+    ... merge its sequence or mapping node values and return the result. For sequence nodes, this
+    means appending together its contained lists. For mapping nodes, it means merging its contained
+    dicts.
+    '''
+    return functools.reduce(operator.add, (value.value for key, value in nodes))
 
 
 def deep_merge_nodes(nodes):
     '''
     Given a nested borgmatic configuration data structure as a list of tuples in the form of:
 
+    [
         (
             ruamel.yaml.nodes.ScalarNode as a key,
             ruamel.yaml.nodes.MappingNode or other Node as a value,
         ),
+        ...
+    ]
 
-    ... deep merge any node values corresponding to duplicate keys and return the result. If
-    there are colliding keys with non-MappingNode values (e.g., integers or strings), the last
-    of the values wins.
+    ... deep merge any node values corresponding to duplicate keys and return the result. The
+    purpose of merging like this is to support, for instance, merging one borgmatic configuration
+    file into another for reuse, such that a configuration option with sub-options does not
+    completely replace the corresponding option in a merged file.
+
+    If there are colliding keys with scalar values (e.g., integers or strings), the last of the
+    values wins.
 
     For instance, given node values of:
 
         [
             (
-                ScalarNode(tag='tag:yaml.org,2002:str', value='retention'),
+                ScalarNode(tag='tag:yaml.org,2002:str', value='option'),
                 MappingNode(tag='tag:yaml.org,2002:map', value=[
                     (
-                        ScalarNode(tag='tag:yaml.org,2002:str', value='keep_hourly'),
-                        ScalarNode(tag='tag:yaml.org,2002:int', value='24')
+                        ScalarNode(tag='tag:yaml.org,2002:str', value='sub_option1'),
+                        ScalarNode(tag='tag:yaml.org,2002:int', value='1')
                     ),
                     (
-                        ScalarNode(tag='tag:yaml.org,2002:str', value='keep_daily'),
-                        ScalarNode(tag='tag:yaml.org,2002:int', value='7')
+                        ScalarNode(tag='tag:yaml.org,2002:str', value='sub_option2'),
+                        ScalarNode(tag='tag:yaml.org,2002:int', value='2')
                     ),
                 ]),
             ),
             (
-                ScalarNode(tag='tag:yaml.org,2002:str', value='retention'),
+                ScalarNode(tag='tag:yaml.org,2002:str', value='option'),
                 MappingNode(tag='tag:yaml.org,2002:map', value=[
                     (
-                        ScalarNode(tag='tag:yaml.org,2002:str', value='keep_daily'),
+                        ScalarNode(tag='tag:yaml.org,2002:str', value='sub_option2'),
                         ScalarNode(tag='tag:yaml.org,2002:int', value='5')
                     ),
                 ]),
             ),
         ]
 
     ... the returned result would be:
 
         [
             (
-                ScalarNode(tag='tag:yaml.org,2002:str', value='retention'),
+                ScalarNode(tag='tag:yaml.org,2002:str', value='option'),
                 MappingNode(tag='tag:yaml.org,2002:map', value=[
                     (
-                        ScalarNode(tag='tag:yaml.org,2002:str', value='keep_hourly'),
-                        ScalarNode(tag='tag:yaml.org,2002:int', value='24')
+                        ScalarNode(tag='tag:yaml.org,2002:str', value='sub_option1'),
+                        ScalarNode(tag='tag:yaml.org,2002:int', value='1')
                     ),
                     (
-                        ScalarNode(tag='tag:yaml.org,2002:str', value='keep_daily'),
+                        ScalarNode(tag='tag:yaml.org,2002:str', value='sub_option2'),
                         ScalarNode(tag='tag:yaml.org,2002:int', value='5')
                     ),
                 ]),
             ),
         ]
 
+    This function supports multi-way merging, meaning that if the same option name exists three or
+    more times (at the same scope level), all of those instances get merged together.
+
     If a mapping or sequence node has a YAML "!retain" tag, then that node is not merged.
 
-    The purpose of deep merging like this is to support, for instance, merging one borgmatic
-    configuration file into another for reuse, such that a configuration option with sub-options
-    does not completely replace the corresponding option in a merged file.
-
-    Raise ValueError if a merge is implied using two incompatible types.
-    '''
-    # Map from original node key/value to the replacement merged node. DELETED_NODE as a replacement
-    # node indications deletion.
-    replaced_nodes = {}
-
-    # To find nodes that require merging, compare each node with each other node.
-    for a_key, a_value in nodes:
-        for b_key, b_value in nodes:
-            # If we've already considered one of the nodes for merging, skip it.
-            if (a_key, a_value) in replaced_nodes or (b_key, b_value) in replaced_nodes:
-                continue
-
-            # If the keys match and the values are different, we need to merge these two A and B nodes.
-            if a_key.tag == b_key.tag and a_key.value == b_key.value and a_value != b_value:
-                if not type(a_value) is type(b_value):
-                    raise ValueError(
-                        f'Incompatible types found when trying to merge "{a_key.value}:" values across configuration files: {type(a_value).id} and {type(b_value).id}'
+    Raise ValueError if a merge is implied using multiple incompatible types.
+    '''
+    merged_nodes = []
+
+    def get_node_key_name(node):
+        return node[0].value
+
+    # Bucket the nodes by their keys. Then merge all of the values sharing the same key.
+    for key_name, grouped_nodes in itertools.groupby(
+        sorted(nodes, key=get_node_key_name), get_node_key_name
+    ):
+        grouped_nodes = list(grouped_nodes)
+
+        # The merged node inherits its attributes from the final node in the group.
+        (last_node_key, last_node_value) = grouped_nodes[-1]
+        value_types = set(type(value) for (_, value) in grouped_nodes)
+
+        if len(value_types) > 1:
+            raise ValueError(
+                f'Incompatible types found when trying to merge "{key_name}:" values across configuration files: {", ".join(value_type.id for value_type in value_types)}'
+            )
+
+        # If we're dealing with MappingNodes, recurse and merge its values as well.
+        if ruamel.yaml.nodes.MappingNode in value_types:
+            # A "!retain" tag says to skip deep merging for this node. Replace the tag so
+            # downstream schema validation doesn't break on our application-specific tag.
+            if last_node_value.tag == '!retain' and len(grouped_nodes) > 1:
+                last_node_value.tag = 'tag:yaml.org,2002:map'
+                merged_nodes.append((last_node_key, last_node_value))
+            else:
+                merged_nodes.append(
+                    (
+                        last_node_key,
+                        ruamel.yaml.nodes.MappingNode(
+                            tag=last_node_value.tag,
+                            value=deep_merge_nodes(merge_values(grouped_nodes)),
+                            start_mark=last_node_value.start_mark,
+                            end_mark=last_node_value.end_mark,
+                            flow_style=last_node_value.flow_style,
+                            comment=last_node_value.comment,
+                            anchor=last_node_value.anchor,
+                        ),
+                    )
+                )
+
+            continue
+
+        # If we're dealing with SequenceNodes, merge by appending sequences together.
+        if ruamel.yaml.nodes.SequenceNode in value_types:
+            if last_node_value.tag == '!retain' and len(grouped_nodes) > 1:
+                last_node_value.tag = 'tag:yaml.org,2002:seq'
+                merged_nodes.append((last_node_key, last_node_value))
+            else:
+                merged_nodes.append(
+                    (
+                        last_node_key,
+                        ruamel.yaml.nodes.SequenceNode(
+                            tag=last_node_value.tag,
+                            value=filter_omitted_nodes(grouped_nodes, merge_values(grouped_nodes)),
+                            start_mark=last_node_value.start_mark,
+                            end_mark=last_node_value.end_mark,
+                            flow_style=last_node_value.flow_style,
+                            comment=last_node_value.comment,
+                            anchor=last_node_value.anchor,
+                        ),
                     )
+                )
 
-                # Since we're merging into the B node, consider the A node a duplicate and remove it.
-                replaced_nodes[(a_key, a_value)] = DELETED_NODE
+            continue
 
-                # If we're dealing with MappingNodes, recurse and merge its values as well.
-                if isinstance(b_value, ruamel.yaml.nodes.MappingNode):
-                    # A "!retain" tag says to skip deep merging for this node. Replace the tag so
-                    # downstream schema validation doesn't break on our application-specific tag.
-                    if b_value.tag == '!retain':
-                        b_value.tag = 'tag:yaml.org,2002:map'
-                    else:
-                        replaced_nodes[(b_key, b_value)] = (
-                            b_key,
-                            ruamel.yaml.nodes.MappingNode(
-                                tag=b_value.tag,
-                                value=deep_merge_nodes(a_value.value + b_value.value),
-                                start_mark=b_value.start_mark,
-                                end_mark=b_value.end_mark,
-                                flow_style=b_value.flow_style,
-                                comment=b_value.comment,
-                                anchor=b_value.anchor,
-                            ),
-                        )
-                # If we're dealing with SequenceNodes, merge by appending one sequence to the other.
-                elif isinstance(b_value, ruamel.yaml.nodes.SequenceNode):
-                    # A "!retain" tag says to skip deep merging for this node. Replace the tag so
-                    # downstream schema validation doesn't break on our application-specific tag.
-                    if b_value.tag == '!retain':
-                        b_value.tag = 'tag:yaml.org,2002:seq'
-                    else:
-                        replaced_nodes[(b_key, b_value)] = (
-                            b_key,
-                            ruamel.yaml.nodes.SequenceNode(
-                                tag=b_value.tag,
-                                value=filter_omitted_nodes(a_value.value + b_value.value),
-                                start_mark=b_value.start_mark,
-                                end_mark=b_value.end_mark,
-                                flow_style=b_value.flow_style,
-                                comment=b_value.comment,
-                                anchor=b_value.anchor,
-                            ),
-                        )
+        merged_nodes.append((last_node_key, last_node_value))
 
-    return [
-        replaced_nodes.get(node, node) for node in nodes if replaced_nodes.get(node) != DELETED_NODE
-    ]
+    return merged_nodes
```

### Comparing `borgmatic-1.8.0/borgmatic/config/normalize.py` & `borgmatic-1.8.1/borgmatic/config/normalize.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,19 @@
     '''
     Given a configuration filename and a configuration dict of its loaded contents, airlift any
     options out of sections ("location:", etc.) to the global scope and delete those sections.
     Return any log message warnings produced based on the normalization performed.
 
     Raise ValueError if the "prefix" option is set in both "location" and "consistency" sections.
     '''
-    location = config.get('location') or {}
+    try:
+        location = config.get('location') or {}
+    except AttributeError:
+        raise ValueError('Configuration does not contain any options')
+
     storage = config.get('storage') or {}
     consistency = config.get('consistency') or {}
     hooks = config.get('hooks') or {}
 
     if (
         location.get('prefix')
         and consistency.get('prefix')
```

### Comparing `borgmatic-1.8.0/borgmatic/config/override.py` & `borgmatic-1.8.1/borgmatic/config/override.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/borgmatic/config/schema.yaml` & `borgmatic-1.8.1/borgmatic/config/schema.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -206,14 +206,21 @@
         type: string
         description: |
             Path for additional source files used for temporary internal state
             like borgmatic database dumps. Note that changing this path prevents
             "borgmatic restore" from finding any database dumps created before
             the change. Defaults to ~/.borgmatic
         example: /tmp/borgmatic
+    store_config_files:
+        type: boolean
+        description: |
+            Store configuration files used to create a backup in the backup
+            itself. Defaults to true. Changing this to false prevents "borgmatic
+            bootstrap" from extracting configuration files from the backup. 
+        example: true
     source_directories_must_exist:
         type: boolean
         description: |
             If true, then source directories must exist, otherwise an error is
             raised. Defaults to false.
         example: true
     encryption_passcommand:
@@ -361,27 +368,27 @@
             If match_archives is not specified, borgmatic defaults to deriving
             the match_archives value from archive_name_format.
         example: "sh:{hostname}-*"
     relocated_repo_access_is_ok:
         type: boolean
         description: |
             Bypass Borg error about a repository that has been moved. Defaults
-            to false.
+            to not bypassing.
         example: true
     unknown_unencrypted_repo_access_is_ok:
         type: boolean
         description: |
             Bypass Borg error about a previously unknown unencrypted repository.
-            Defaults to false.
+            Defaults to not bypassing.
         example: true
     check_i_know_what_i_am_doing:
         type: boolean
         description: |
-            Bypass Borg confirmation about check with repair option.
-            Defaults to false.
+            Bypass Borg confirmation about check with repair option. Defaults to
+            an interactive prompt from Borg.
         example: true
     extra_borg_options:
         type: object
         additionalProperties: false
         properties:
             init:
                 type: string
```

### Comparing `borgmatic-1.8.0/borgmatic/config/validate.py` & `borgmatic-1.8.1/borgmatic/config/validate.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/borgmatic/execute.py` & `borgmatic-1.8.1/borgmatic/execute.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/borgmatic/hooks/command.py` & `borgmatic-1.8.1/borgmatic/hooks/command.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/borgmatic/hooks/cronhub.py` & `borgmatic-1.8.1/borgmatic/hooks/cronhub.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/borgmatic/hooks/cronitor.py` & `borgmatic-1.8.1/borgmatic/hooks/cronitor.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/borgmatic/hooks/dispatch.py` & `borgmatic-1.8.1/borgmatic/hooks/dispatch.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/borgmatic/hooks/dump.py` & `borgmatic-1.8.1/borgmatic/hooks/dump.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/borgmatic/hooks/healthchecks.py` & `borgmatic-1.8.1/borgmatic/hooks/healthchecks.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/borgmatic/hooks/mongodb.py` & `borgmatic-1.8.1/borgmatic/hooks/mongodb.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/borgmatic/hooks/mysql.py` & `borgmatic-1.8.1/borgmatic/hooks/mysql.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/borgmatic/hooks/ntfy.py` & `borgmatic-1.8.1/borgmatic/hooks/ntfy.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 
     if state.name.lower() in run_states:
         dry_run_label = ' (dry run; not actually pinging)' if dry_run else ''
 
         state_config = hook_config.get(
             state.name.lower(),
             {
-                'title': f'A Borgmatic {state.name} event happened',
-                'message': f'A Borgmatic {state.name} event happened',
+                'title': f'A borgmatic {state.name} event happened',
+                'message': f'A borgmatic {state.name} event happened',
                 'priority': 'default',
                 'tags': 'borgmatic',
             },
         )
 
         base_url = hook_config.get('server', 'https://ntfy.sh')
         topic = hook_config.get('topic')
```

### Comparing `borgmatic-1.8.0/borgmatic/hooks/pagerduty.py` & `borgmatic-1.8.1/borgmatic/hooks/pagerduty.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/borgmatic/hooks/postgresql.py` & `borgmatic-1.8.1/borgmatic/hooks/postgresql.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/borgmatic/hooks/sqlite.py` & `borgmatic-1.8.1/borgmatic/hooks/sqlite.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/borgmatic/logger.py` & `borgmatic-1.8.1/borgmatic/logger.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/borgmatic/signals.py` & `borgmatic-1.8.1/borgmatic/signals.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/borgmatic/verbosity.py` & `borgmatic-1.8.1/borgmatic/verbosity.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/borgmatic.egg-info/PKG-INFO` & `borgmatic-1.8.1/borgmatic.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: borgmatic
-Version: 1.8.0
+Version: 1.8.1
 Summary: Simple, configuration-driven backup software for servers and workstations
 Home-page: https://torsion.org/borgmatic
 Author: Dan Helfman
 Author-email: witten@torsion.org
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: System Administrators
```

### Comparing `borgmatic-1.8.0/borgmatic.egg-info/SOURCES.txt` & `borgmatic-1.8.1/borgmatic.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -254,14 +254,15 @@
 tests/unit/commands/completion/test_bash.py
 tests/unit/commands/completion/test_fish.py
 tests/unit/config/__init__.py
 tests/unit/config/test_checks.py
 tests/unit/config/test_collect.py
 tests/unit/config/test_environment.py
 tests/unit/config/test_generate.py
+tests/unit/config/test_load.py
 tests/unit/config/test_normalize.py
 tests/unit/config/test_override.py
 tests/unit/config/test_validate.py
 tests/unit/hooks/__init__.py
 tests/unit/hooks/test_command.py
 tests/unit/hooks/test_cronhub.py
 tests/unit/hooks/test_cronitor.py
```

### Comparing `borgmatic-1.8.0/docs/Dockerfile` & `borgmatic-1.8.1/docs/Dockerfile`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/docs/README.md` & `borgmatic-1.8.1/docs/README.md`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/docs/SECURITY.md` & `borgmatic-1.8.1/docs/SECURITY.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 each.
 
 ## Reporting a vulnerability
 
 If you find a security vulnerability, please [file a
 ticket](https://torsion.org/borgmatic/#issues) or [send email
 directly](mailto:witten@torsion.org) as appropriate. You should expect to hear
-back within a few days at most, and generally sooner.
+back within a few days at most and generally sooner.
```

### Comparing `borgmatic-1.8.0/docs/_includes/components/info-blocks.css` & `borgmatic-1.8.1/docs/_includes/components/info-blocks.css`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/docs/_includes/components/lists.css` & `borgmatic-1.8.1/docs/_includes/components/lists.css`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/docs/_includes/components/minilink.css` & `borgmatic-1.8.1/docs/_includes/components/minilink.css`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/docs/_includes/components/toc.css` & `borgmatic-1.8.1/docs/_includes/components/toc.css`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/docs/_includes/index.css` & `borgmatic-1.8.1/docs/_includes/index.css`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/docs/_includes/layouts/base.njk` & `borgmatic-1.8.1/docs/_includes/layouts/base.njk`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/docs/_includes/layouts/main.njk` & `borgmatic-1.8.1/docs/_includes/layouts/main.njk`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/docs/_includes/prism-theme.css` & `borgmatic-1.8.1/docs/_includes/prism-theme.css`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/docs/how-to/add-preparation-and-cleanup-steps-to-backups.md` & `borgmatic-1.8.1/docs/how-to/add-preparation-and-cleanup-steps-to-backups.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 they're configured in the `hooks` section of your configuration file. But if
 you're looking to backup a database, it's probably easier to use the [database
 backup
 feature](https://torsion.org/borgmatic/docs/how-to/backup-your-databases/)
 instead.
 
 You can specify `before_backup` hooks to perform preparation steps before
-running backups, and specify `after_backup` hooks to perform cleanup steps
+running backups and specify `after_backup` hooks to perform cleanup steps
 afterwards. Here's an example:
 
 ```yaml
 before_backup:
     - mount /some/filesystem
 after_backup:
     - umount /some/filesystem
```

### Comparing `borgmatic-1.8.0/docs/how-to/backup-to-a-removable-drive-or-an-intermittent-server.md` & `borgmatic-1.8.1/docs/how-to/backup-to-a-removable-drive-or-an-intermittent-server.md`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/docs/how-to/backup-your-databases.md` & `borgmatic-1.8.1/docs/how-to/backup-your-databases.md`

 * *Files 4% similar despite different names*

```diff
@@ -334,14 +334,36 @@
 PostgreSQL and MongoDB, you can limit the restore to a single schema found
 within the database dump:
 
 ```bash
 borgmatic restore --archive latest --database users --schema tentant1
 ```
 
+### Restore to an alternate host
+<span class="minilink minilink-addedin">New in version 1.7.15</span>
+A database dump can be restored to a host other than the one from which it was
+originally dumped. The connection parameters like the username, password, and
+port can also be changed. This can be done from the command line:
+
+```bash
+borgmatic restore --archive latest --database users --hostname database2.example.org --port 5433 --username postgres --password trustsome1
+```
+
+Or from the configuration file:
+
+```yaml
+postgresql_databases:
+    - name: users
+        hostname: database1.example.org
+        restore_hostname: database1.example.org
+        restore_port: 5433
+        restore_username: postgres
+        restore_password: trustsome1
+```
+
 
 ### Limitations
 
 There are a few important limitations with borgmatic's current database
 restoration feature that you should know about:
 
 1. You must restore as the same Unix user that created the archive containing
```

### Comparing `borgmatic-1.8.0/docs/how-to/deal-with-very-large-backups.md` & `borgmatic-1.8.1/docs/how-to/deal-with-very-large-backups.md`

 * *Files 1% similar despite different names*

```diff
@@ -185,15 +185,15 @@
 repositories:
 
 ```yaml
 check_repositories:
     - path/of/repository_to_check.borg
 ```
 
-Finally, you can override your configuration file's consistency checks, and
+Finally, you can override your configuration file's consistency checks and
 run particular checks via the command-line. For instance:
 
 ```bash
 borgmatic check --only data --only extract
 ```
 
 This is useful for running slow consistency checks on an infrequent basis,
```

### Comparing `borgmatic-1.8.0/docs/how-to/develop-on-borgmatic.md` & `borgmatic-1.8.1/docs/how-to/develop-on-borgmatic.md`

 * *Files 1% similar despite different names*

```diff
@@ -145,16 +145,16 @@
 certain code style requirements will be enforced when running automated tests.
 See the Black, Flake8, and isort documentation for more information.
 
 ## Continuous integration
 
 Each pull request triggers a continuous integration build which runs the test
 suite. You can view these builds on
-[build.torsion.org](https://build.torsion.org/borgmatic-collective/borgmatic), and they're
-also linked from the commits list on each pull request.
+[build.torsion.org](https://build.torsion.org/borgmatic-collective/borgmatic),
+and they're also linked from the commits list on each pull request.
 
 ## Documentation development
 
 Updates to borgmatic's documentation are welcome. It's formatted in Markdown
 and located in the `docs/` directory in borgmatic's source, plus the
 `README.md` file at the root.
```

### Comparing `borgmatic-1.8.0/docs/how-to/extract-a-backup.md` & `borgmatic-1.8.1/docs/how-to/extract-a-backup.md`

 * *Files 18% similar despite different names*

```diff
@@ -40,15 +40,14 @@
 ```
 
 The `--archive` value is the name of the archive to extract. This extracts the
 entire contents of the archive to the current directory, so make sure you're
 in the right place before running the command—or see below about the
 `--destination` flag.
 
-
 ## Repository selection
 
 If you have a single repository in your borgmatic configuration file(s), no
 problem: the `extract` action figures out which repository to use.
 
 But if you have multiple repositories configured, then you'll need to specify
 the repository to use via the `--repository` flag. This can be done either
@@ -141,7 +140,33 @@
 
 When you're all done exploring your files, unmount your mount point. No
 `--archive` flag is needed:
 
 ```bash
 borgmatic umount --mount-point /mnt
 ```
+
+## Extract the configuration files used to create an archive
+
+<span class="minilink minilink-addedin">New in version 1.7.15</span> borgmatic
+automatically stores all the configuration files used to create an archive inside the
+archive itself. This is useful in cases where you've lost a configuration
+file or you want to see what configurations were used to create a particular
+archive.
+
+To extract the configuration files from an archive, use the `config bootstrap` action. For example:
+
+```bash 
+borgmatic config bootstrap --repository repo.borg --destination /tmp
+```
+
+This extracts the configuration file from the latest archive in the repository `repo.borg` to `/tmp/etc/borgmatic/config.yaml`, assuming that the only configuration file used to create this archive was located at `/etc/borgmatic/config.yaml` when the archive was created.
+
+Note that to run the `config bootstrap` action, you don't need to have a borgmatic configuration file. You only need to specify the repository to use via the `--repository` flag; borgmatic will figure out the rest.
+
+If a destination directory is not specified, the configuration files will be extracted to their original locations, silently **overwriting** any configuration files that may already exist. For example, if a configuration file was located at `/etc/borgmatic/config.yaml` when the archive was created, it will be extracted to `/etc/borgmatic/config.yaml` too.
+
+If you want to extract the configuration file from a specific archive, use the `--archive` flag:
+
+```bash
+borgmatic config bootstrap --repository repo.borg --archive host-2023-01-02T04:06:07.080910 --destination /tmp
+```
```

### Comparing `borgmatic-1.8.0/docs/how-to/inspect-your-backups.md` & `borgmatic-1.8.1/docs/how-to/inspect-your-backups.md`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/docs/how-to/make-backups-redundant.md` & `borgmatic-1.8.1/docs/how-to/make-backups-redundant.md`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/docs/how-to/make-per-application-backups.md` & `borgmatic-1.8.1/docs/how-to/make-per-application-backups.md`

 * *Files 2% similar despite different names*

```diff
@@ -149,15 +149,15 @@
 
 
 ## Configuration includes
 
 Once you have multiple different configuration files, you might want to share
 common configuration options across these files with having to copy and paste
 them. To achieve this, you can put fragments of common configuration options
-into a file, and then include or inline that file into one or more borgmatic
+into a file and then include or inline that file into one or more borgmatic
 configuration files.
 
 Let's say that you want to include common consistency check configuration across all
 of your configuration files. You could do that in each configuration file with
 the following:
 
 ```yaml
@@ -229,26 +229,65 @@
     - name: archives
       frequency: 2 weeks
 ```
 
 <span class="minilink minilink-addedin">Prior to version 1.8.0</span> These
 options were organized into sections like `retention:` and `consistency:`.
 
-Once this include gets merged in, the resulting configuration would have all
-of the options from the original configuration file *and* the options from the
+Once this include gets merged in, the resulting configuration has all of the
+options from the original configuration file *and* the options from the
 include.
 
 Note that this `<<` include merging syntax is only for merging in mappings
-(configuration options and their values). But if you'd like to include a
-single value directly, please see the above about standard includes.
+(configuration options and their values). If you'd like to include a single
+value directly, please see above about standard includes.
 
-Additionally, there is a limitation preventing multiple `<<` include merges
-per file or option value. So for instance, that means you can do one `<<`
-merge at the global level, another `<<` within each nested option value, etc.
-(This is a YAML limitation.)
+
+### Multiple merge includes
+
+borgmatic has a limitation preventing multiple `<<` include merges per file or
+option value. This means you can do a single `<<` merge at the global level,
+another `<<` within each nested option value, etc. (This is a YAML
+limitation.) For instance:
+
+```yaml
+repositories:
+   - path: repo.borg
+
+# This won't work! You can't do multiple merges like this at the same level.
+<<: !include common1.yaml
+<<: !include common2.yaml
+```
+
+But read on for a way around this.
+
+<span class="minilink minilink-addedin">New in version 1.8.1</span> You can
+include and merge multiple configuration files all at once. For instance:
+
+```yaml
+repositories:
+   - path: repo.borg
+
+<<: !include [common1.yaml, common2.yaml, common3.yaml]
+```
+
+This merges in each included configuration file in turn, such that later files
+replace the options in earlier ones.
+
+Here's another way to do the same thing:
+
+```yaml
+repositories:
+   - path: repo.borg
+
+<<: !include
+    - common1.yaml
+    - common2.yaml
+    - common3.yaml
+```
 
 
 ### Deep merge
 
 <span class="minilink minilink-addedin">New in version 1.6.0</span> borgmatic
 performs a deep merge of merged include files, meaning that values are merged
 at all levels in the two configuration files. This allows you to include
@@ -305,16 +344,16 @@
 
 ```yaml
 source_directories:
     - /home
     - /etc
 ```
 
-<span class="minilink minilink-addedin">Prior to version 1.8.0</span> Put
-this option in the `location:` section of your configuration.
+<span class="minilink minilink-addedin">Prior to version 1.8.0</span> Put the
+`source_directories` option in the `location:` section of your configuration.
 
 Once this include gets merged in, the resulting configuration will have a
 `source_directories` value of `/etc` and `/var`—with `/home` omitted.
 
 This feature currently only works on scalar (e.g. string or number) list items
 and will not work elsewhere in a configuration file. Be sure to put the
 `!omit` tag *before* the list item (after the dash). Putting `!omit` after the
@@ -438,16 +477,16 @@
 Whatever the reason, you can override borgmatic configuration options at the
 command-line via the `--override` flag. Here's an example:
 
 ```bash
 borgmatic create --override remote_path=/usr/local/bin/borg1
 ```
 
-What this does is load your configuration files, and for each one, disregard
-the configured value for the `remote_path` option, and use the value of
+What this does is load your configuration files and for each one, disregard
+the configured value for the `remote_path` option and use the value of
 `/usr/local/bin/borg1` instead.
 
 You can even override nested values or multiple values at once. For instance:
 
 ```bash
 borgmatic create --override parent_option.option1=value1 --override parent_option.option2=value2
 ```
```

### Comparing `borgmatic-1.8.0/docs/how-to/monitor-your-backups.md` & `borgmatic-1.8.1/docs/how-to/monitor-your-backups.md`

 * *Files 1% similar despite different names*

```diff
@@ -102,27 +102,27 @@
 
 ```yaml
 on_error:
     - send-text-message.sh "{configuration_filename}" "{repository}"
 ```
 
 In this example, when the error occurs, borgmatic interpolates runtime values
-into the hook command: the borgmatic configuration filename, and the path of
+into the hook command: the borgmatic configuration filename and the path of
 the repository. Here's the full set of supported variables you can use here:
 
  * `configuration_filename`: borgmatic configuration filename in which the
    error occurred
  * `repository`: path of the repository in which the error occurred (may be
    blank if the error occurs in a hook)
  * `error`: the error message itself
  * `output`: output of the command that failed (may be blank if an error
    occurred without running a command)
 
 Note that borgmatic runs the `on_error` hooks only for `create`, `prune`,
-`compact`, or `check` actions or hooks in which an error occurs, and not other
+`compact`, or `check` actions/hooks in which an error occurs and not other
 actions. borgmatic does not run `on_error` hooks if an error occurs within a
 `before_everything` or `after_everything` hook. For more about hooks, see the
 [borgmatic hooks
 documentation](https://torsion.org/borgmatic/docs/how-to/add-preparation-and-cleanup-steps-to-backups/),
 especially the security information.
 
 
@@ -146,15 +146,15 @@
 With this hook in place, borgmatic pings your Healthchecks project when a
 backup begins, ends, or errors. Specifically, after the <a
 href="https://torsion.org/borgmatic/docs/how-to/add-preparation-and-cleanup-steps-to-backups/">`before_backup`
 hooks</a> run, borgmatic lets Healthchecks know that it has started if any of
 the `create`, `prune`, `compact`, or `check` actions are run.
 
 Then, if the actions complete successfully, borgmatic notifies Healthchecks of
-the success after the `after_backup` hooks run, and includes borgmatic logs in
+the success after the `after_backup` hooks run and includes borgmatic logs in
 the payload data sent to Healthchecks. This means that borgmatic logs show up
 in the Healthchecks UI, although be aware that Healthchecks currently has a
 10-kilobyte limit for the logs in each ping.
 
 If an error occurs during any action or hook, borgmatic notifies Healthchecks
 after the `on_error` hooks run, also tacking on logs including the error
 itself. But the logs are only included for errors that occur when a `create`,
@@ -300,25 +300,25 @@
 [tags](https://ntfy.sh/docs/publish/#tags-emojis):
 
 ```yaml
 ntfy:
     topic: my-unique-topic
     server: https://ntfy.my-domain.com
     start:
-        title: A Borgmatic backup started
+        title: A borgmatic backup started
         message: Watch this space...
         tags: borgmatic
         priority: min
     finish:
-        title: A Borgmatic backup completed successfully
+        title: A borgmatic backup completed successfully
         message: Nice!
         tags: borgmatic,+1
         priority: min
     fail:
-        title: A Borgmatic backup failed
+        title: A borgmatic backup failed
         message: You should probably fix it
         tags: borgmatic,-1,skull
         priority: max
     states:
         - start
         - finish
         - fail
@@ -332,15 +332,15 @@
 
 To consume the output of borgmatic in other software, you can include an
 optional `--json` flag with `create`, `rlist`, `rinfo`, or `info` to get the
 output formatted as JSON.
 
 Note that when you specify the `--json` flag, Borg's other non-JSON output is
 suppressed so as not to interfere with the captured JSON. Also note that JSON
-output only shows up at the console, and not in syslog.
+output only shows up at the console and not in syslog.
 
 
 ### Latest backups
 
 All borgmatic actions that accept an `--archive` flag allow you to specify an
 archive name of `latest`. This lets you get the latest archive without having
 to first run `borgmatic rlist` manually, which can be handy in automated
```

### Comparing `borgmatic-1.8.0/docs/how-to/provide-your-passwords.md` & `borgmatic-1.8.1/docs/how-to/provide-your-passwords.md`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/docs/how-to/run-arbitrary-borg-commands.md` & `borgmatic-1.8.1/docs/how-to/run-arbitrary-borg-commands.md`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/docs/how-to/set-up-backups.md` & `borgmatic-1.8.1/docs/how-to/set-up-backups.md`

 * *Files 0% similar despite different names*

```diff
@@ -55,19 +55,19 @@
 to run borgmatic, you can configure [sudo's
 `secure_path` option](https://man.archlinux.org/man/sudoers.5) to include
 borgmatic's path.
 
 
 ### Global install option
 
-If you try the user site installation above, and have problems making
-borgmatic commands runnable on your system `PATH`, an alternate approach is to
-install borgmatic globally.
+If you try the user site installation above and have problems making borgmatic
+commands runnable on your system `PATH`, an alternate approach is to install
+borgmatic globally.
 
-The following uninstalls borgmatic, and then reinstalls it such that borgmatic
+The following uninstalls borgmatic and then reinstalls it such that borgmatic
 commands are on the default system `PATH`:
 
 ```bash
 sudo pip3 uninstall borgmatic
 sudo pip3 install --upgrade borgmatic
 ```
 
@@ -225,15 +225,15 @@
 sudo borgmatic rcreate --encryption repokey-aes-ocb
 ```
 
 (Note that `repokey-chacha20-poly1305` may be faster than `repokey-aes-ocb` on
 certain platforms like ARM64.)
 
 This uses the borgmatic configuration file you created above to determine
-which local or remote repository to create, and encrypts it with the
+which local or remote repository to create and encrypts it with the
 encryption passphrase specified there if one is provided. Read about [Borg
 encryption
 modes](https://borgbackup.readthedocs.io/en/stable/usage/init.html#encryption-mode-tldr)
 for the menu of available encryption modes.
 
 Also, optionally check out the [Borg Quick
 Start](https://borgbackup.readthedocs.org/en/stable/quickstart.html) for more
```

### Comparing `borgmatic-1.8.0/docs/how-to/upgrade.md` & `borgmatic-1.8.1/docs/how-to/upgrade.md`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 configuration files in-place. So it's up to you to review the generated file
 and, if desired, replace your original configuration file with it.
 
 
 ### Upgrading from borgmatic 1.0.x
 
 borgmatic changed its configuration file format in version 1.1.0 from
-INI-style to YAML. This better supports validation, and has a more natural way
+INI-style to YAML. This better supports validation and has a more natural way
 to express lists of values. To upgrade your existing configuration, first
 upgrade to the last version of borgmatic to support converting configuration:
 borgmatic 1.7.14.
 
 As of version 1.1.0, borgmatic no longer supports Python 2. If you were
 already running borgmatic with Python 3, then you can upgrade borgmatic
 in-place:
```

### Comparing `borgmatic-1.8.0/docs/reference/command-line.md` & `borgmatic-1.8.1/docs/reference/command-line.md`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/docs/reference/configuration.md` & `borgmatic-1.8.1/docs/reference/configuration.md`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/docs/static/borgbase.png` & `borgmatic-1.8.1/docs/static/borgbase.png`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/docs/static/borgmatic.png` & `borgmatic-1.8.1/docs/static/borgmatic.png`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/docs/static/borgmatic.svg` & `borgmatic-1.8.1/docs/static/borgmatic.svg`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/docs/static/cronhub.png` & `borgmatic-1.8.1/docs/static/cronhub.png`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/docs/static/cronitor.png` & `borgmatic-1.8.1/docs/static/cronitor.png`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/docs/static/healthchecks.png` & `borgmatic-1.8.1/docs/static/healthchecks.png`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/docs/static/mariadb.png` & `borgmatic-1.8.1/docs/static/mariadb.png`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/docs/static/mongodb.png` & `borgmatic-1.8.1/docs/static/mongodb.png`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/docs/static/mysql.png` & `borgmatic-1.8.1/docs/static/mysql.png`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/docs/static/ntfy.png` & `borgmatic-1.8.1/docs/static/ntfy.png`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/docs/static/pagerduty.png` & `borgmatic-1.8.1/docs/static/pagerduty.png`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/docs/static/postgresql.png` & `borgmatic-1.8.1/docs/static/postgresql.png`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/docs/static/sqlite.png` & `borgmatic-1.8.1/docs/static/sqlite.png`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/sample/systemd/borgmatic.service` & `borgmatic-1.8.1/sample/systemd/borgmatic.service`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/scripts/find-unsupported-borg-options` & `borgmatic-1.8.1/scripts/find-unsupported-borg-options`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/scripts/release` & `borgmatic-1.8.1/scripts/release`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/scripts/run-end-to-end-dev-tests` & `borgmatic-1.8.1/scripts/run-end-to-end-dev-tests`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/scripts/run-full-tests` & `borgmatic-1.8.1/scripts/run-full-tests`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/setup.py` & `borgmatic-1.8.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-VERSION = '1.8.0'
+VERSION = '1.8.1'
 
 
 setup(
     name='borgmatic',
     version=VERSION,
     description='Simple, configuration-driven backup software for servers and workstations',
     author='Dan Helfman',
```

### Comparing `borgmatic-1.8.0/test_requirements.txt` & `borgmatic-1.8.1/test_requirements.txt`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/end-to-end/docker-compose.yaml` & `borgmatic-1.8.1/tests/end-to-end/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/end-to-end/test_borgmatic.py` & `borgmatic-1.8.1/tests/end-to-end/test_borgmatic.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/end-to-end/test_database.py` & `borgmatic-1.8.1/tests/end-to-end/test_database.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/end-to-end/test_dev_parity_with_build_server.py` & `borgmatic-1.8.1/tests/end-to-end/test_dev_parity_with_build_server.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/end-to-end/test_generate_config.py` & `borgmatic-1.8.1/tests/end-to-end/test_generate_config.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/end-to-end/test_override.py` & `borgmatic-1.8.1/tests/end-to-end/test_override.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/end-to-end/test_validate_config.py` & `borgmatic-1.8.1/tests/end-to-end/test_validate_config.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/integration/actions/config/test_validate.py` & `borgmatic-1.8.1/tests/integration/actions/config/test_validate.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/integration/borg/test_commands.py` & `borgmatic-1.8.1/tests/integration/borg/test_commands.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/integration/borg/test_feature.py` & `borgmatic-1.8.1/tests/integration/borg/test_feature.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/integration/commands/completion/test_actions.py` & `borgmatic-1.8.1/tests/integration/commands/completion/test_actions.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/integration/commands/test_arguments.py` & `borgmatic-1.8.1/tests/integration/commands/test_arguments.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/integration/config/test_generate.py` & `borgmatic-1.8.1/tests/integration/config/test_generate.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/integration/config/test_load.py` & `borgmatic-1.8.1/tests/integration/config/test_load.py`

 * *Files 9% similar despite different names*

```diff
@@ -40,14 +40,22 @@
         '''
     )
     config_file.name = 'config.yaml'
     builtins.should_receive('open').with_args('config.yaml').and_return(config_file)
     assert module.load_configuration('config.yaml') == {'key': {'subkey': 'value'}}
 
 
+def test_load_configuration_with_only_integer_value_does_not_raise():
+    builtins = flexmock(sys.modules['builtins'])
+    config_file = io.StringIO('33')
+    config_file.name = 'config.yaml'
+    builtins.should_receive('open').with_args('config.yaml').and_return(config_file)
+    assert module.load_configuration('config.yaml') == 33
+
+
 def test_load_configuration_inlines_include_relative_to_current_directory():
     builtins = flexmock(sys.modules['builtins'])
     flexmock(module.os).should_receive('getcwd').and_return('/tmp')
     flexmock(module.os.path).should_receive('isabs').and_return(False)
     flexmock(module.os.path).should_receive('exists').and_return(True)
     include_file = io.StringIO('value')
     include_file.name = 'include.yaml'
@@ -120,14 +128,45 @@
     config_file.name = 'config.yaml'
     builtins.should_receive('open').with_args('config.yaml').and_return(config_file)
 
     with pytest.raises(FileNotFoundError):
         assert module.load_configuration('config.yaml')
 
 
+def test_load_configuration_inlines_multiple_file_include_as_list():
+    builtins = flexmock(sys.modules['builtins'])
+    flexmock(module.os).should_receive('getcwd').and_return('/tmp')
+    flexmock(module.os.path).should_receive('isabs').and_return(True)
+    flexmock(module.os.path).should_receive('exists').never()
+    include1_file = io.StringIO('value1')
+    include1_file.name = '/root/include1.yaml'
+    builtins.should_receive('open').with_args('/root/include1.yaml').and_return(include1_file)
+    include2_file = io.StringIO('value2')
+    include2_file.name = '/root/include2.yaml'
+    builtins.should_receive('open').with_args('/root/include2.yaml').and_return(include2_file)
+    config_file = io.StringIO('key: !include [/root/include1.yaml, /root/include2.yaml]')
+    config_file.name = 'config.yaml'
+    builtins.should_receive('open').with_args('config.yaml').and_return(config_file)
+
+    assert module.load_configuration('config.yaml') == {'key': ['value2', 'value1']}
+
+
+def test_load_configuration_include_with_unsupported_filename_type_raises():
+    builtins = flexmock(sys.modules['builtins'])
+    flexmock(module.os).should_receive('getcwd').and_return('/tmp')
+    flexmock(module.os.path).should_receive('isabs').and_return(True)
+    flexmock(module.os.path).should_receive('exists').never()
+    config_file = io.StringIO('key: !include {path: /root/include.yaml}')
+    config_file.name = 'config.yaml'
+    builtins.should_receive('open').with_args('config.yaml').and_return(config_file)
+
+    with pytest.raises(ValueError):
+        module.load_configuration('config.yaml')
+
+
 def test_load_configuration_merges_include():
     builtins = flexmock(sys.modules['builtins'])
     flexmock(module.os).should_receive('getcwd').and_return('/tmp')
     flexmock(module.os.path).should_receive('isabs').and_return(False)
     flexmock(module.os.path).should_receive('exists').and_return(True)
     include_file = io.StringIO(
         '''
@@ -145,14 +184,51 @@
     )
     config_file.name = 'config.yaml'
     builtins.should_receive('open').with_args('config.yaml').and_return(config_file)
 
     assert module.load_configuration('config.yaml') == {'foo': 'override', 'baz': 'quux'}
 
 
+def test_load_configuration_merges_multiple_file_include():
+    builtins = flexmock(sys.modules['builtins'])
+    flexmock(module.os).should_receive('getcwd').and_return('/tmp')
+    flexmock(module.os.path).should_receive('isabs').and_return(False)
+    flexmock(module.os.path).should_receive('exists').and_return(True)
+    include1_file = io.StringIO(
+        '''
+        foo: bar
+        baz: quux
+        original: yes
+        '''
+    )
+    include1_file.name = 'include1.yaml'
+    builtins.should_receive('open').with_args('/tmp/include1.yaml').and_return(include1_file)
+    include2_file = io.StringIO(
+        '''
+        baz: second
+        '''
+    )
+    include2_file.name = 'include2.yaml'
+    builtins.should_receive('open').with_args('/tmp/include2.yaml').and_return(include2_file)
+    config_file = io.StringIO(
+        '''
+        foo: override
+        <<: !include [include1.yaml, include2.yaml]
+        '''
+    )
+    config_file.name = 'config.yaml'
+    builtins.should_receive('open').with_args('config.yaml').and_return(config_file)
+
+    assert module.load_configuration('config.yaml') == {
+        'foo': 'override',
+        'baz': 'second',
+        'original': 'yes',
+    }
+
+
 def test_load_configuration_with_retain_tag_merges_include_but_keeps_local_values():
     builtins = flexmock(sys.modules['builtins'])
     flexmock(module.os).should_receive('getcwd').and_return('/tmp')
     flexmock(module.os.path).should_receive('isabs').and_return(False)
     flexmock(module.os.path).should_receive('exists').and_return(True)
     include_file = io.StringIO(
         '''
@@ -434,29 +510,158 @@
 
 
 def test_raise_omit_node_error_raises():
     with pytest.raises(ValueError):
         module.raise_omit_node_error(loader=flexmock(), node=flexmock())
 
 
-def test_filter_omitted_nodes():
-    nodes = [
+def test_filter_omitted_nodes_discards_values_with_omit_tag_and_also_equal_values():
+    nodes = [flexmock(), flexmock()]
+    values = [
         module.ruamel.yaml.nodes.ScalarNode(tag='tag:yaml.org,2002:str', value='a'),
         module.ruamel.yaml.nodes.ScalarNode(tag='tag:yaml.org,2002:str', value='b'),
         module.ruamel.yaml.nodes.ScalarNode(tag='tag:yaml.org,2002:str', value='c'),
         module.ruamel.yaml.nodes.ScalarNode(tag='tag:yaml.org,2002:str', value='a'),
         module.ruamel.yaml.nodes.ScalarNode(tag='!omit', value='b'),
         module.ruamel.yaml.nodes.ScalarNode(tag='tag:yaml.org,2002:str', value='c'),
     ]
 
-    result = module.filter_omitted_nodes(nodes)
+    result = module.filter_omitted_nodes(nodes, values)
 
     assert [item.value for item in result] == ['a', 'c', 'a', 'c']
 
 
+def test_filter_omitted_nodes_keeps_all_values_when_given_only_one_node():
+    nodes = [flexmock()]
+    values = [
+        module.ruamel.yaml.nodes.ScalarNode(tag='tag:yaml.org,2002:str', value='a'),
+        module.ruamel.yaml.nodes.ScalarNode(tag='tag:yaml.org,2002:str', value='b'),
+        module.ruamel.yaml.nodes.ScalarNode(tag='tag:yaml.org,2002:str', value='c'),
+        module.ruamel.yaml.nodes.ScalarNode(tag='tag:yaml.org,2002:str', value='a'),
+        module.ruamel.yaml.nodes.ScalarNode(tag='!omit', value='b'),
+        module.ruamel.yaml.nodes.ScalarNode(tag='tag:yaml.org,2002:str', value='c'),
+    ]
+
+    result = module.filter_omitted_nodes(nodes, values)
+
+    assert [item.value for item in result] == ['a', 'b', 'c', 'a', 'b', 'c']
+
+
+def test_merge_values_combines_mapping_values():
+    nodes = [
+        (
+            module.ruamel.yaml.nodes.ScalarNode(tag='tag:yaml.org,2002:str', value='option'),
+            module.ruamel.yaml.nodes.MappingNode(
+                tag='tag:yaml.org,2002:map',
+                value=[
+                    (
+                        module.ruamel.yaml.nodes.ScalarNode(
+                            tag='tag:yaml.org,2002:str', value='keep_hourly'
+                        ),
+                        module.ruamel.yaml.nodes.ScalarNode(
+                            tag='tag:yaml.org,2002:int', value='24'
+                        ),
+                    ),
+                    (
+                        module.ruamel.yaml.nodes.ScalarNode(
+                            tag='tag:yaml.org,2002:str', value='keep_daily'
+                        ),
+                        module.ruamel.yaml.nodes.ScalarNode(tag='tag:yaml.org,2002:int', value='7'),
+                    ),
+                ],
+            ),
+        ),
+        (
+            module.ruamel.yaml.nodes.ScalarNode(tag='tag:yaml.org,2002:str', value='option'),
+            module.ruamel.yaml.nodes.MappingNode(
+                tag='tag:yaml.org,2002:map',
+                value=[
+                    (
+                        module.ruamel.yaml.nodes.ScalarNode(
+                            tag='tag:yaml.org,2002:str', value='keep_daily'
+                        ),
+                        module.ruamel.yaml.nodes.ScalarNode(
+                            tag='tag:yaml.org,2002:int', value='25'
+                        ),
+                    ),
+                ],
+            ),
+        ),
+        (
+            module.ruamel.yaml.nodes.ScalarNode(tag='tag:yaml.org,2002:str', value='option'),
+            module.ruamel.yaml.nodes.MappingNode(
+                tag='tag:yaml.org,2002:map',
+                value=[
+                    (
+                        module.ruamel.yaml.nodes.ScalarNode(
+                            tag='tag:yaml.org,2002:str', value='keep_nanosecondly'
+                        ),
+                        module.ruamel.yaml.nodes.ScalarNode(
+                            tag='tag:yaml.org,2002:int', value='1000'
+                        ),
+                    ),
+                ],
+            ),
+        ),
+    ]
+
+    values = module.merge_values(nodes)
+
+    assert len(values) == 4
+    assert values[0][0].value == 'keep_hourly'
+    assert values[0][1].value == '24'
+    assert values[1][0].value == 'keep_daily'
+    assert values[1][1].value == '7'
+    assert values[2][0].value == 'keep_daily'
+    assert values[2][1].value == '25'
+    assert values[3][0].value == 'keep_nanosecondly'
+    assert values[3][1].value == '1000'
+
+
+def test_merge_values_combines_sequence_values():
+    nodes = [
+        (
+            module.ruamel.yaml.nodes.ScalarNode(tag='tag:yaml.org,2002:str', value='option'),
+            module.ruamel.yaml.nodes.SequenceNode(
+                tag='tag:yaml.org,2002:seq',
+                value=[
+                    module.ruamel.yaml.nodes.ScalarNode(tag='tag:yaml.org,2002:int', value='1'),
+                    module.ruamel.yaml.nodes.ScalarNode(tag='tag:yaml.org,2002:int', value='2'),
+                ],
+            ),
+        ),
+        (
+            module.ruamel.yaml.nodes.ScalarNode(tag='tag:yaml.org,2002:str', value='option'),
+            module.ruamel.yaml.nodes.SequenceNode(
+                tag='tag:yaml.org,2002:seq',
+                value=[
+                    module.ruamel.yaml.nodes.ScalarNode(tag='tag:yaml.org,2002:int', value='3'),
+                ],
+            ),
+        ),
+        (
+            module.ruamel.yaml.nodes.ScalarNode(tag='tag:yaml.org,2002:str', value='option'),
+            module.ruamel.yaml.nodes.SequenceNode(
+                tag='tag:yaml.org,2002:seq',
+                value=[
+                    module.ruamel.yaml.nodes.ScalarNode(tag='tag:yaml.org,2002:int', value='4'),
+                ],
+            ),
+        ),
+    ]
+
+    values = module.merge_values(nodes)
+
+    assert len(values) == 4
+    assert values[0].value == '1'
+    assert values[1].value == '2'
+    assert values[2].value == '3'
+    assert values[3].value == '4'
+
+
 def test_deep_merge_nodes_replaces_colliding_scalar_values():
     node_values = [
         (
             module.ruamel.yaml.nodes.ScalarNode(tag='tag:yaml.org,2002:str', value='retention'),
             module.ruamel.yaml.nodes.MappingNode(
                 tag='tag:yaml.org,2002:map',
                 value=[
@@ -495,18 +700,18 @@
 
     result = module.deep_merge_nodes(node_values)
     assert len(result) == 1
     (section_key, section_value) = result[0]
     assert section_key.value == 'retention'
     options = section_value.value
     assert len(options) == 2
-    assert options[0][0].value == 'keep_hourly'
-    assert options[0][1].value == '24'
-    assert options[1][0].value == 'keep_daily'
-    assert options[1][1].value == '5'
+    assert options[0][0].value == 'keep_daily'
+    assert options[0][1].value == '5'
+    assert options[1][0].value == 'keep_hourly'
+    assert options[1][1].value == '24'
 
 
 def test_deep_merge_nodes_keeps_non_colliding_scalar_values():
     node_values = [
         (
             module.ruamel.yaml.nodes.ScalarNode(tag='tag:yaml.org,2002:str', value='retention'),
             module.ruamel.yaml.nodes.MappingNode(
@@ -549,18 +754,18 @@
 
     result = module.deep_merge_nodes(node_values)
     assert len(result) == 1
     (section_key, section_value) = result[0]
     assert section_key.value == 'retention'
     options = section_value.value
     assert len(options) == 3
-    assert options[0][0].value == 'keep_hourly'
-    assert options[0][1].value == '24'
-    assert options[1][0].value == 'keep_daily'
-    assert options[1][1].value == '7'
+    assert options[0][0].value == 'keep_daily'
+    assert options[0][1].value == '7'
+    assert options[1][0].value == 'keep_hourly'
+    assert options[1][1].value == '24'
     assert options[2][0].value == 'keep_minutely'
     assert options[2][1].value == '10'
 
 
 def test_deep_merge_nodes_keeps_deeply_nested_values():
     node_values = [
         (
@@ -625,18 +830,18 @@
 
     result = module.deep_merge_nodes(node_values)
     assert len(result) == 1
     (section_key, section_value) = result[0]
     assert section_key.value == 'storage'
     options = section_value.value
     assert len(options) == 2
-    assert options[0][0].value == 'lock_wait'
-    assert options[0][1].value == '5'
-    assert options[1][0].value == 'extra_borg_options'
-    nested_options = options[1][1].value
+    assert options[0][0].value == 'extra_borg_options'
+    assert options[1][0].value == 'lock_wait'
+    assert options[1][1].value == '5'
+    nested_options = options[0][1].value
     assert len(nested_options) == 2
     assert nested_options[0][0].value == 'init'
     assert nested_options[0][1].value == '--init-option'
     assert nested_options[1][0].value == 'prune'
     assert nested_options[1][1].value == '--prune-option'
```

### Comparing `borgmatic-1.8.0/tests/integration/config/test_override.py` & `borgmatic-1.8.1/tests/integration/config/test_override.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/integration/config/test_validate.py` & `borgmatic-1.8.1/tests/integration/config/test_validate.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,15 +113,15 @@
                     - type: scalar
         ''',
     )
 
     module.parse_configuration('/tmp/config.yaml', '/tmp/schema.yaml')
 
 
-def test_parse_configuration_inlines_include():
+def test_parse_configuration_inlines_include_inside_deprecated_section():
     mock_config_and_schema(
         '''
         source_directories:
             - /home
 
         repositories:
             - path: hostname.borg
```

### Comparing `borgmatic-1.8.0/tests/integration/hooks/test_healthchecks.py` & `borgmatic-1.8.1/tests/integration/hooks/test_healthchecks.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/integration/test_execute.py` & `borgmatic-1.8.1/tests/integration/test_execute.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/unit/actions/config/test_bootstrap.py` & `borgmatic-1.8.1/tests/unit/actions/config/test_bootstrap.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/unit/actions/config/test_generate.py` & `borgmatic-1.8.1/tests/unit/actions/config/test_generate.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/unit/actions/config/test_validate.py` & `borgmatic-1.8.1/tests/unit/actions/config/test_validate.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/unit/actions/test_borg.py` & `borgmatic-1.8.1/tests/unit/actions/test_borg.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/unit/actions/test_break_lock.py` & `borgmatic-1.8.1/tests/unit/actions/test_break_lock.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/unit/actions/test_check.py` & `borgmatic-1.8.1/tests/unit/actions/test_check.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/unit/actions/test_compact.py` & `borgmatic-1.8.1/tests/unit/actions/test_compact.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/unit/actions/test_create.py` & `borgmatic-1.8.1/tests/unit/actions/test_create.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,14 +36,49 @@
             dry_run_label='',
             local_path=None,
             remote_path=None,
         )
     )
 
 
+def test_run_create_with_store_config_files_false_does_not_create_borgmatic_manifest():
+    flexmock(module.logger).answer = lambda message: None
+    flexmock(module.borgmatic.config.validate).should_receive('repositories_match').never()
+    flexmock(module.borgmatic.borg.create).should_receive('create_archive').once()
+    flexmock(module).should_receive('create_borgmatic_manifest').never()
+    flexmock(module.borgmatic.hooks.command).should_receive('execute_hook').times(2)
+    flexmock(module.borgmatic.hooks.dispatch).should_receive('call_hooks').and_return({})
+    flexmock(module.borgmatic.hooks.dispatch).should_receive(
+        'call_hooks_even_if_unconfigured'
+    ).and_return({})
+    create_arguments = flexmock(
+        repository=None,
+        progress=flexmock(),
+        stats=flexmock(),
+        json=flexmock(),
+        list_files=flexmock(),
+    )
+    global_arguments = flexmock(monitoring_verbosity=1, dry_run=False, used_config_paths=[])
+
+    list(
+        module.run_create(
+            config_filename='test.yaml',
+            repository={'path': 'repo'},
+            config={'store_config_files': False},
+            hook_context={},
+            local_borg_version=None,
+            create_arguments=create_arguments,
+            global_arguments=global_arguments,
+            dry_run_label='',
+            local_path=None,
+            remote_path=None,
+        )
+    )
+
+
 def test_run_create_runs_with_selected_repository():
     flexmock(module.logger).answer = lambda message: None
     flexmock(module.borgmatic.config.validate).should_receive(
         'repositories_match'
     ).once().and_return(True)
     flexmock(module.borgmatic.borg.create).should_receive('create_archive').once()
     flexmock(module).should_receive('create_borgmatic_manifest').once()
```

### Comparing `borgmatic-1.8.0/tests/unit/actions/test_export_tar.py` & `borgmatic-1.8.1/tests/unit/actions/test_export_tar.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/unit/actions/test_extract.py` & `borgmatic-1.8.1/tests/unit/actions/test_extract.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/unit/actions/test_info.py` & `borgmatic-1.8.1/tests/unit/actions/test_info.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/unit/actions/test_list.py` & `borgmatic-1.8.1/tests/unit/actions/test_list.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/unit/actions/test_mount.py` & `borgmatic-1.8.1/tests/unit/actions/test_mount.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/unit/actions/test_prune.py` & `borgmatic-1.8.1/tests/unit/actions/test_prune.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/unit/actions/test_rcreate.py` & `borgmatic-1.8.1/tests/unit/actions/test_rcreate.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/unit/actions/test_restore.py` & `borgmatic-1.8.1/tests/unit/actions/test_restore.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/unit/actions/test_rinfo.py` & `borgmatic-1.8.1/tests/unit/actions/test_rinfo.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/unit/actions/test_rlist.py` & `borgmatic-1.8.1/tests/unit/actions/test_rlist.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/unit/actions/test_transfer.py` & `borgmatic-1.8.1/tests/unit/actions/test_transfer.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/unit/borg/test_borg.py` & `borgmatic-1.8.1/tests/unit/borg/test_borg.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/unit/borg/test_break_lock.py` & `borgmatic-1.8.1/tests/unit/borg/test_break_lock.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/unit/borg/test_check.py` & `borgmatic-1.8.1/tests/unit/borg/test_check.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/unit/borg/test_compact.py` & `borgmatic-1.8.1/tests/unit/borg/test_compact.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/unit/borg/test_create.py` & `borgmatic-1.8.1/tests/unit/borg/test_create.py`

 * *Files 0% similar despite different names*

```diff
@@ -643,14 +643,61 @@
             'repositories': ['repo'],
         },
         local_borg_version='1.2.3',
         global_arguments=flexmock(log_json=False, used_config_paths=['/etc/borgmatic/config.yaml']),
     )
 
 
+def test_create_archive_with_sources_and_used_config_paths_with_store_config_files_false_calls_borg_with_sources_and_no_config_paths():
+    flexmock(module.borgmatic.logger).should_receive('add_custom_log_levels')
+    flexmock(module.logging).ANSWER = module.borgmatic.logger.ANSWER
+    flexmock(module).should_receive('collect_borgmatic_source_directories').and_return([])
+    flexmock(module).should_receive('deduplicate_directories').and_return(('foo', 'bar'))
+    flexmock(module).should_receive('map_directories_to_devices').and_return({})
+    flexmock(module).should_receive('expand_directories').with_args([]).and_return(())
+    flexmock(module).should_receive('expand_directories').with_args(('foo', 'bar')).and_return(
+        ('foo', 'bar')
+    )
+    flexmock(module).should_receive('expand_directories').with_args([]).and_return(())
+    flexmock(module).should_receive('pattern_root_directories').and_return([])
+    flexmock(module.os.path).should_receive('expanduser').and_raise(TypeError)
+    flexmock(module).should_receive('expand_home_directories').and_return(())
+    flexmock(module).should_receive('write_pattern_file').and_return(None)
+    flexmock(module).should_receive('make_list_filter_flags').and_return('FOO')
+    flexmock(module.feature).should_receive('available').and_return(True)
+    flexmock(module).should_receive('ensure_files_readable')
+    flexmock(module).should_receive('make_pattern_flags').and_return(())
+    flexmock(module).should_receive('make_exclude_flags').and_return(())
+    flexmock(module.flags).should_receive('make_repository_archive_flags').and_return(
+        (f'repo::{DEFAULT_ARCHIVE_NAME}',)
+    )
+    environment = {'BORG_THINGY': 'YUP'}
+    flexmock(module.environment).should_receive('make_environment').and_return(environment)
+    flexmock(module).should_receive('execute_command').with_args(
+        ('borg', 'create') + REPO_ARCHIVE_WITH_PATHS,
+        output_log_level=logging.INFO,
+        output_file=None,
+        borg_local_path='borg',
+        working_directory=None,
+        extra_environment=environment,
+    )
+
+    module.create_archive(
+        dry_run=False,
+        repository_path='repo',
+        config={
+            'source_directories': ['foo', 'bar'],
+            'repositories': ['repo'],
+            'store_config_files': False,
+        },
+        local_borg_version='1.2.3',
+        global_arguments=flexmock(log_json=False, used_config_paths=['/etc/borgmatic/config.yaml']),
+    )
+
+
 def test_create_archive_with_exclude_patterns_calls_borg_with_excludes():
     flexmock(module.borgmatic.logger).should_receive('add_custom_log_levels')
     flexmock(module.logging).ANSWER = module.borgmatic.logger.ANSWER
     exclude_flags = ('--exclude-from', 'excludes')
     flexmock(module).should_receive('collect_borgmatic_source_directories').and_return([])
     flexmock(module).should_receive('deduplicate_directories').and_return(('foo', 'bar'))
     flexmock(module).should_receive('map_directories_to_devices').and_return({})
```

### Comparing `borgmatic-1.8.0/tests/unit/borg/test_environment.py` & `borgmatic-1.8.1/tests/unit/borg/test_environment.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,32 +15,40 @@
 
 def test_make_environment_with_ssh_command_should_set_environment():
     environment = module.make_environment({'ssh_command': 'ssh -C'})
 
     assert environment.get('BORG_RSH') == 'ssh -C'
 
 
-def test_make_environment_without_configuration_should_only_set_default_environment():
+def test_make_environment_without_configuration_should_not_set_environment():
     environment = module.make_environment({})
 
-    assert environment == {
-        'BORG_RELOCATED_REPO_ACCESS_IS_OK': 'no',
-        'BORG_UNKNOWN_UNENCRYPTED_REPO_ACCESS_IS_OK': 'no',
-        'BORG_CHECK_I_KNOW_WHAT_I_AM_DOING': 'NO',
-    }
+    assert environment == {}
 
 
-def test_make_environment_with_relocated_repo_access_should_override_default():
+def test_make_environment_with_relocated_repo_access_true_should_set_environment_yes():
     environment = module.make_environment({'relocated_repo_access_is_ok': True})
 
     assert environment.get('BORG_RELOCATED_REPO_ACCESS_IS_OK') == 'yes'
 
 
-def test_make_environment_check_i_know_what_i_am_doing_should_override_default():
+def test_make_environment_with_relocated_repo_access_false_should_set_environment_no():
+    environment = module.make_environment({'relocated_repo_access_is_ok': False})
+
+    assert environment.get('BORG_RELOCATED_REPO_ACCESS_IS_OK') == 'no'
+
+
+def test_make_environment_check_i_know_what_i_am_doing_true_should_set_environment_YES():
     environment = module.make_environment({'check_i_know_what_i_am_doing': True})
 
     assert environment.get('BORG_CHECK_I_KNOW_WHAT_I_AM_DOING') == 'YES'
 
 
+def test_make_environment_check_i_know_what_i_am_doing_false_should_set_environment_NO():
+    environment = module.make_environment({'check_i_know_what_i_am_doing': False})
+
+    assert environment.get('BORG_CHECK_I_KNOW_WHAT_I_AM_DOING') == 'NO'
+
+
 def test_make_environment_with_integer_variable_value():
     environment = module.make_environment({'borg_files_cache_ttl': 40})
     assert environment.get('BORG_FILES_CACHE_TTL') == '40'
```

### Comparing `borgmatic-1.8.0/tests/unit/borg/test_export_tar.py` & `borgmatic-1.8.1/tests/unit/borg/test_export_tar.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/unit/borg/test_extract.py` & `borgmatic-1.8.1/tests/unit/borg/test_extract.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/unit/borg/test_flags.py` & `borgmatic-1.8.1/tests/unit/borg/test_flags.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,36 +82,36 @@
 
     assert module.make_repository_archive_flags(
         repository_path='repo', archive='archive', local_borg_version='1.2.3'
     ) == ('repo::archive',)
 
 
 @pytest.mark.parametrize(
-    'match_archives, archive_name_format,feature_available,expected_result',
+    'match_archives,archive_name_format,feature_available,expected_result',
     (
         (None, None, True, ()),
         (None, '', True, ()),
         (
             're:foo-.*',
-            '{hostname}-{now}',
+            '{hostname}-{now}',  # noqa: FS003
             True,
             ('--match-archives', 're:foo-.*'),
-        ),  # noqa: FS003
+        ),
         (
             'sh:foo-*',
-            '{hostname}-{now}',
+            '{hostname}-{now}',  # noqa: FS003
             False,
             ('--glob-archives', 'foo-*'),
-        ),  # noqa: FS003
+        ),
         (
             'foo-*',
-            '{hostname}-{now}',
+            '{hostname}-{now}',  # noqa: FS003
             False,
             ('--glob-archives', 'foo-*'),
-        ),  # noqa: FS003
+        ),
         (
             None,
             '{hostname}-docs-{now}',  # noqa: FS003
             True,
             ('--match-archives', 'sh:{hostname}-docs-*'),  # noqa: FS003
         ),
         (
@@ -129,14 +129,26 @@
         ),
         (
             None,
             '{hostname}-docs-{now}',  # noqa: FS003
             False,
             ('--glob-archives', '{hostname}-docs-*'),  # noqa: FS003
         ),
+        (
+            None,
+            '{now}',  # noqa: FS003
+            False,
+            (),
+        ),
+        (
+            None,
+            '{now}',  # noqa: FS003
+            True,
+            (),
+        ),
         (None, '{utcnow}-docs-{user}', False, ('--glob-archives', '*-docs-{user}')),  # noqa: FS003
     ),
 )
 def test_make_match_archives_flags_makes_flags_with_globs(
     match_archives, archive_name_format, feature_available, expected_result
 ):
     flexmock(module.feature).should_receive('available').and_return(feature_available)
```

### Comparing `borgmatic-1.8.0/tests/unit/borg/test_info.py` & `borgmatic-1.8.1/tests/unit/borg/test_info.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/unit/borg/test_list.py` & `borgmatic-1.8.1/tests/unit/borg/test_list.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/unit/borg/test_mount.py` & `borgmatic-1.8.1/tests/unit/borg/test_mount.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/unit/borg/test_prune.py` & `borgmatic-1.8.1/tests/unit/borg/test_prune.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,14 +114,27 @@
         '--match-archives',
         'sh:bar-*',  # noqa: FS003
     )
 
     assert result == expected
 
 
+def test_make_prune_flags_ignores_keep_exclude_tags_in_config():
+    config = {
+        'keep_daily': 1,
+        'keep_exclude_tags': True,
+    }
+    flexmock(module.feature).should_receive('available').and_return(True)
+    flexmock(module.flags).should_receive('make_match_archives_flags').and_return(())
+
+    result = module.make_prune_flags(config, local_borg_version='1.2.3')
+
+    assert result == ('--keep-daily', '1')
+
+
 PRUNE_COMMAND = ('borg', 'prune', '--keep-daily', '1', '--keep-weekly', '2', '--keep-monthly', '3')
 
 
 def test_prune_archives_calls_borg_with_flags():
     flexmock(module.borgmatic.logger).should_receive('add_custom_log_levels')
     flexmock(module.logging).ANSWER = module.borgmatic.logger.ANSWER
     flexmock(module).should_receive('make_prune_flags').and_return(BASE_PRUNE_FLAGS)
```

### Comparing `borgmatic-1.8.0/tests/unit/borg/test_rcreate.py` & `borgmatic-1.8.1/tests/unit/borg/test_rcreate.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/unit/borg/test_rinfo.py` & `borgmatic-1.8.1/tests/unit/borg/test_rinfo.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/unit/borg/test_rlist.py` & `borgmatic-1.8.1/tests/unit/borg/test_rlist.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/unit/borg/test_transfer.py` & `borgmatic-1.8.1/tests/unit/borg/test_transfer.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/unit/borg/test_umount.py` & `borgmatic-1.8.1/tests/unit/borg/test_umount.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/unit/borg/test_version.py` & `borgmatic-1.8.1/tests/unit/borg/test_version.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/unit/commands/completion/test_fish.py` & `borgmatic-1.8.1/tests/unit/commands/completion/test_fish.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/unit/commands/test_arguments.py` & `borgmatic-1.8.1/tests/unit/commands/test_arguments.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/unit/commands/test_borgmatic.py` & `borgmatic-1.8.1/tests/unit/commands/test_borgmatic.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/unit/config/test_checks.py` & `borgmatic-1.8.1/tests/unit/config/test_checks.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/unit/config/test_collect.py` & `borgmatic-1.8.1/tests/unit/config/test_collect.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/unit/config/test_environment.py` & `borgmatic-1.8.1/tests/unit/config/test_environment.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/unit/config/test_generate.py` & `borgmatic-1.8.1/tests/unit/config/test_generate.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/unit/config/test_normalize.py` & `borgmatic-1.8.1/tests/unit/config/test_normalize.py`

 * *Files 4% similar despite different names*

```diff
@@ -107,14 +107,21 @@
 def test_normalize_sections_with_different_umask_values_raises():
     config = {'storage': {'umask': 'foo'}, 'hooks': {'umask': 'bar'}}
 
     with pytest.raises(ValueError):
         module.normalize_sections('test.yaml', config)
 
 
+def test_normalize_sections_with_only_scalar_raises():
+    config = 33
+
+    with pytest.raises(ValueError):
+        module.normalize_sections('test.yaml', config)
+
+
 @pytest.mark.parametrize(
     'config,expected_config,produces_logs',
     (
         (
             {'exclude_if_present': '.nobackup'},
             {'exclude_if_present': ['.nobackup']},
             True,
```

### Comparing `borgmatic-1.8.0/tests/unit/config/test_override.py` & `borgmatic-1.8.1/tests/unit/config/test_override.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/unit/config/test_validate.py` & `borgmatic-1.8.1/tests/unit/config/test_validate.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/unit/hooks/test_command.py` & `borgmatic-1.8.1/tests/unit/hooks/test_command.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/unit/hooks/test_cronhub.py` & `borgmatic-1.8.1/tests/unit/hooks/test_cronhub.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/unit/hooks/test_cronitor.py` & `borgmatic-1.8.1/tests/unit/hooks/test_cronitor.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/unit/hooks/test_dispatch.py` & `borgmatic-1.8.1/tests/unit/hooks/test_dispatch.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/unit/hooks/test_dump.py` & `borgmatic-1.8.1/tests/unit/hooks/test_dump.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/unit/hooks/test_healthchecks.py` & `borgmatic-1.8.1/tests/unit/hooks/test_healthchecks.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/unit/hooks/test_mongodb.py` & `borgmatic-1.8.1/tests/unit/hooks/test_mongodb.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/unit/hooks/test_mysql.py` & `borgmatic-1.8.1/tests/unit/hooks/test_mysql.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/unit/hooks/test_ntfy.py` & `borgmatic-1.8.1/tests/unit/hooks/test_ntfy.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,32 +6,32 @@
 from borgmatic.hooks import ntfy as module
 
 default_base_url = 'https://ntfy.sh'
 custom_base_url = 'https://ntfy.example.com'
 topic = 'borgmatic-unit-testing'
 
 custom_message_config = {
-    'title': 'Borgmatic unit testing',
-    'message': 'Borgmatic unit testing',
+    'title': 'borgmatic unit testing',
+    'message': 'borgmatic unit testing',
     'priority': 'min',
     'tags': '+1',
 }
 
 custom_message_headers = {
     'X-Title': custom_message_config['title'],
     'X-Message': custom_message_config['message'],
     'X-Priority': custom_message_config['priority'],
     'X-Tags': custom_message_config['tags'],
 }
 
 
 def return_default_message_headers(state=Enum):
     headers = {
-        'X-Title': f'A Borgmatic {state.name} event happened',
-        'X-Message': f'A Borgmatic {state.name} event happened',
+        'X-Title': f'A borgmatic {state.name} event happened',
+        'X-Message': f'A borgmatic {state.name} event happened',
         'X-Priority': 'default',
         'X-Tags': 'borgmatic',
     }
     return headers
 
 
 def test_ping_monitor_minimal_config_hits_hosted_ntfy_on_fail():
```

### Comparing `borgmatic-1.8.0/tests/unit/hooks/test_pagerduty.py` & `borgmatic-1.8.1/tests/unit/hooks/test_pagerduty.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/unit/hooks/test_postgresql.py` & `borgmatic-1.8.1/tests/unit/hooks/test_postgresql.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/unit/hooks/test_sqlite.py` & `borgmatic-1.8.1/tests/unit/hooks/test_sqlite.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/unit/test_execute.py` & `borgmatic-1.8.1/tests/unit/test_execute.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/unit/test_logger.py` & `borgmatic-1.8.1/tests/unit/test_logger.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/unit/test_signals.py` & `borgmatic-1.8.1/tests/unit/test_signals.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tests/unit/test_verbosity.py` & `borgmatic-1.8.1/tests/unit/test_verbosity.py`

 * *Files identical despite different names*

### Comparing `borgmatic-1.8.0/tox.ini` & `borgmatic-1.8.1/tox.ini`

 * *Files identical despite different names*

