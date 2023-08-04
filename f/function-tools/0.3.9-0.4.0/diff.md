# Comparing `tmp/function-tools-0.3.9.tar.gz` & `tmp/function-tools-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "function-tools-0.3.9.tar", last modified: Fri Jun 16 09:11:04 2023, max compression
+gzip compressed data, was "function-tools-0.4.0.tar", last modified: Fri Aug  4 12:26:56 2023, max compression
```

## Comparing `function-tools-0.3.9.tar` & `function-tools-0.4.0.tar`

### file list

```diff
@@ -1,73 +1,74 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 09:11:04.141263 function-tools-0.3.9/
--rw-r--r--   0 root         (0) root         (0)    10327 2023-06-16 09:10:54.000000 function-tools-0.3.9/CHANGES.md
--rw-r--r--   0 root         (0) root         (0)     1069 2022-02-16 11:53:12.000000 function-tools-0.3.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)      275 2022-07-12 08:20:24.000000 function-tools-0.3.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    18775 2023-06-16 09:11:04.141263 function-tools-0.3.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7804 2022-02-16 11:53:12.000000 function-tools-0.3.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 09:11:04.109263 function-tools-0.3.9/function_tools/
--rw-r--r--   0 root         (0) root         (0)       63 2022-02-16 11:53:12.000000 function-tools-0.3.9/function_tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)      140 2022-08-01 11:26:19.000000 function-tools-0.3.9/function_tools/apps.py
--rw-r--r--   0 root         (0) root         (0)    19868 2022-07-13 10:58:16.000000 function-tools-0.3.9/function_tools/caches.py
--rw-r--r--   0 root         (0) root         (0)      114 2022-07-25 11:47:49.000000 function-tools-0.3.9/function_tools/consts.py
--rw-r--r--   0 root         (0) root         (0)      458 2022-02-16 11:53:12.000000 function-tools-0.3.9/function_tools/decorators.py
--rw-r--r--   0 root         (0) root         (0)      245 2022-02-16 11:53:12.000000 function-tools-0.3.9/function_tools/enums.py
--rw-r--r--   0 root         (0) root         (0)      451 2022-02-16 11:53:12.000000 function-tools-0.3.9/function_tools/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 09:11:04.112263 function-tools-0.3.9/function_tools/function_templates/
--rw-r--r--   0 root         (0) root         (0)        0 2022-07-05 13:57:48.000000 function-tools-0.3.9/function_tools/function_templates/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 09:11:04.130263 function-tools-0.3.9/function_tools/function_templates/function_sync_template/
--rw-r--r--   0 root         (0) root         (0)      271 2022-07-05 13:57:48.000000 function-tools-0.3.9/function_tools/function_templates/function_sync_template/README.md
--rw-r--r--   0 root         (0) root         (0)       92 2022-07-05 13:57:48.000000 function-tools-0.3.9/function_tools/function_templates/function_sync_template/__init__.py-tpl
--rw-r--r--   0 root         (0) root         (0)      329 2022-07-13 10:58:16.000000 function-tools-0.3.9/function_tools/function_templates/function_sync_template/apps.py-tpl
--rw-r--r--   0 root         (0) root         (0)      651 2022-07-27 13:25:54.000000 function-tools-0.3.9/function_tools/function_templates/function_sync_template/caches.py-tpl
--rw-r--r--   0 root         (0) root         (0)       66 2022-07-05 13:57:48.000000 function-tools-0.3.9/function_tools/function_templates/function_sync_template/consts.py-tpl
--rw-r--r--   0 root         (0) root         (0)       93 2022-07-05 13:57:48.000000 function-tools-0.3.9/function_tools/function_templates/function_sync_template/enums.py-tpl
--rw-r--r--   0 root         (0) root         (0)      257 2022-07-12 08:20:24.000000 function-tools-0.3.9/function_tools/function_templates/function_sync_template/errors.py-tpl
--rw-r--r--   0 root         (0) root         (0)     2831 2022-07-25 11:47:49.000000 function-tools-0.3.9/function_tools/function_templates/function_sync_template/functions.py-tpl
--rw-r--r--   0 root         (0) root         (0)     1310 2022-07-25 11:47:49.000000 function-tools-0.3.9/function_tools/function_templates/function_sync_template/helpers.py-tpl
--rw-r--r--   0 root         (0) root         (0)     1601 2022-07-25 11:47:49.000000 function-tools-0.3.9/function_tools/function_templates/function_sync_template/managers.py-tpl
--rw-r--r--   0 root         (0) root         (0)      326 2022-07-12 08:20:24.000000 function-tools-0.3.9/function_tools/function_templates/function_sync_template/presenters.py-tpl
--rw-r--r--   0 root         (0) root         (0)      609 2022-07-25 11:47:49.000000 function-tools-0.3.9/function_tools/function_templates/function_sync_template/results.py-tpl
--rw-r--r--   0 root         (0) root         (0)     2841 2022-07-25 11:47:49.000000 function-tools-0.3.9/function_tools/function_templates/function_sync_template/runners.py-tpl
--rw-r--r--   0 root         (0) root         (0)      181 2022-07-05 13:57:48.000000 function-tools-0.3.9/function_tools/function_templates/function_sync_template/strings.py-tpl
--rw-r--r--   0 root         (0) root         (0)       59 2022-07-05 13:57:48.000000 function-tools-0.3.9/function_tools/function_templates/function_sync_template/tests.py-tpl
--rw-r--r--   0 root         (0) root         (0)      911 2022-07-13 12:17:45.000000 function-tools-0.3.9/function_tools/function_templates/function_sync_template/validators.py-tpl
--rw-r--r--   0 root         (0) root         (0)    10489 2022-07-25 11:47:49.000000 function-tools-0.3.9/function_tools/functions.py
--rw-r--r--   0 root         (0) root         (0)     5362 2022-07-25 11:47:49.000000 function-tools-0.3.9/function_tools/general.py
--rw-r--r--   0 root         (0) root         (0)     2244 2022-07-25 11:47:49.000000 function-tools-0.3.9/function_tools/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 09:11:04.132263 function-tools-0.3.9/function_tools/management/
--rw-r--r--   0 root         (0) root         (0)        0 2022-02-16 11:53:12.000000 function-tools-0.3.9/function_tools/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 09:11:04.134263 function-tools-0.3.9/function_tools/management/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2022-02-16 11:53:12.000000 function-tools-0.3.9/function_tools/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7507 2022-07-27 13:25:54.000000 function-tools-0.3.9/function_tools/management/commands/register_entities.py
--rw-r--r--   0 root         (0) root         (0)    17844 2023-06-16 09:10:54.000000 function-tools-0.3.9/function_tools/management/commands/startfunction.py
--rw-r--r--   0 root         (0) root         (0)       52 2022-02-16 11:53:12.000000 function-tools-0.3.9/function_tools/management/consts.py
--rw-r--r--   0 root         (0) root         (0)      598 2022-07-25 11:47:49.000000 function-tools-0.3.9/function_tools/management/strategies.py
--rw-r--r--   0 root         (0) root         (0)     4957 2022-07-25 11:47:49.000000 function-tools-0.3.9/function_tools/managers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 09:11:04.140263 function-tools-0.3.9/function_tools/migrations/
--rw-r--r--   0 root         (0) root         (0)     1124 2022-02-16 11:53:12.000000 function-tools-0.3.9/function_tools/migrations/0001_initial.py
--rw-r--r--   0 root         (0) root         (0)      520 2022-02-16 11:53:12.000000 function-tools-0.3.9/function_tools/migrations/0002_registeredfunction_tags.py
--rw-r--r--   0 root         (0) root         (0)      795 2022-02-16 11:53:12.000000 function-tools-0.3.9/function_tools/migrations/0003_implementationstrategy.py
--rw-r--r--   0 root         (0) root         (0)      477 2022-02-16 11:53:12.000000 function-tools-0.3.9/function_tools/migrations/0004_implementationstrategy_order_number.py
--rw-r--r--   0 root         (0) root         (0)     2736 2022-07-25 11:47:49.000000 function-tools-0.3.9/function_tools/migrations/0005_auto_20220724_0050.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-07-12 12:03:22.000000 function-tools-0.3.9/function_tools/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6434 2022-07-25 11:47:49.000000 function-tools-0.3.9/function_tools/mixins.py
--rw-r--r--   0 root         (0) root         (0)     4534 2022-11-01 12:27:02.000000 function-tools-0.3.9/function_tools/models.py
--rw-r--r--   0 root         (0) root         (0)      685 2022-02-16 11:53:12.000000 function-tools-0.3.9/function_tools/presenters.py
--rw-r--r--   0 root         (0) root         (0)      369 2022-07-27 13:25:54.000000 function-tools-0.3.9/function_tools/receivers.py
--rw-r--r--   0 root         (0) root         (0)     2386 2022-02-16 11:53:12.000000 function-tools-0.3.9/function_tools/results.py
--rw-r--r--   0 root         (0) root         (0)    12097 2022-07-25 11:47:49.000000 function-tools-0.3.9/function_tools/runners.py
--rw-r--r--   0 root         (0) root         (0)    11548 2023-06-16 09:10:54.000000 function-tools-0.3.9/function_tools/storages.py
--rw-r--r--   0 root         (0) root         (0)    17851 2022-07-25 11:47:49.000000 function-tools-0.3.9/function_tools/strategies.py
--rw-r--r--   0 root         (0) root         (0)      693 2022-02-16 11:53:12.000000 function-tools-0.3.9/function_tools/strings.py
--rw-r--r--   0 root         (0) root         (0)      603 2022-02-16 11:53:12.000000 function-tools-0.3.9/function_tools/types.py
--rw-r--r--   0 root         (0) root         (0)     3234 2022-03-03 06:03:15.000000 function-tools-0.3.9/function_tools/utils.py
--rw-r--r--   0 root         (0) root         (0)      408 2022-02-16 11:53:12.000000 function-tools-0.3.9/function_tools/validators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 09:11:04.112263 function-tools-0.3.9/function_tools.egg-info/
--rw-r--r--   0 root         (0) root         (0)    18775 2023-06-16 09:11:04.000000 function-tools-0.3.9/function_tools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2648 2023-06-16 09:11:04.000000 function-tools-0.3.9/function_tools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 09:11:04.000000 function-tools-0.3.9/function_tools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2023-06-16 09:11:04.000000 function-tools-0.3.9/function_tools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-06-16 09:11:04.000000 function-tools-0.3.9/function_tools.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       47 2022-07-05 13:57:48.000000 function-tools-0.3.9/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       79 2023-06-16 09:11:04.142263 function-tools-0.3.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1707 2023-06-16 09:10:54.000000 function-tools-0.3.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 12:26:56.373155 function-tools-0.4.0/
+-rw-r--r--   0 root         (0) root         (0)    12614 2023-08-04 12:26:47.000000 function-tools-0.4.0/CHANGES.md
+-rw-r--r--   0 root         (0) root         (0)     1069 2022-02-16 11:53:12.000000 function-tools-0.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      275 2022-07-12 08:20:24.000000 function-tools-0.4.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    21062 2023-08-04 12:26:56.374155 function-tools-0.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7804 2022-02-16 11:53:12.000000 function-tools-0.4.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 12:26:56.342155 function-tools-0.4.0/function_tools/
+-rw-r--r--   0 root         (0) root         (0)       63 2022-02-16 11:53:12.000000 function-tools-0.4.0/function_tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      257 2023-08-04 12:26:47.000000 function-tools-0.4.0/function_tools/app_settings.py
+-rw-r--r--   0 root         (0) root         (0)      863 2023-08-04 12:26:47.000000 function-tools-0.4.0/function_tools/apps.py
+-rw-r--r--   0 root         (0) root         (0)    19868 2022-07-13 10:58:16.000000 function-tools-0.4.0/function_tools/caches.py
+-rw-r--r--   0 root         (0) root         (0)      114 2022-07-25 11:47:49.000000 function-tools-0.4.0/function_tools/consts.py
+-rw-r--r--   0 root         (0) root         (0)      458 2022-02-16 11:53:12.000000 function-tools-0.4.0/function_tools/decorators.py
+-rw-r--r--   0 root         (0) root         (0)      245 2022-02-16 11:53:12.000000 function-tools-0.4.0/function_tools/enums.py
+-rw-r--r--   0 root         (0) root         (0)      451 2022-02-16 11:53:12.000000 function-tools-0.4.0/function_tools/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 12:26:56.345155 function-tools-0.4.0/function_tools/function_templates/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-07-05 13:57:48.000000 function-tools-0.4.0/function_tools/function_templates/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 12:26:56.362155 function-tools-0.4.0/function_tools/function_templates/function_sync_template/
+-rw-r--r--   0 root         (0) root         (0)      271 2022-07-05 13:57:48.000000 function-tools-0.4.0/function_tools/function_templates/function_sync_template/README.md
+-rw-r--r--   0 root         (0) root         (0)       92 2022-07-05 13:57:48.000000 function-tools-0.4.0/function_tools/function_templates/function_sync_template/__init__.py-tpl
+-rw-r--r--   0 root         (0) root         (0)      329 2022-07-13 10:58:16.000000 function-tools-0.4.0/function_tools/function_templates/function_sync_template/apps.py-tpl
+-rw-r--r--   0 root         (0) root         (0)      651 2022-07-27 13:25:54.000000 function-tools-0.4.0/function_tools/function_templates/function_sync_template/caches.py-tpl
+-rw-r--r--   0 root         (0) root         (0)       66 2022-07-05 13:57:48.000000 function-tools-0.4.0/function_tools/function_templates/function_sync_template/consts.py-tpl
+-rw-r--r--   0 root         (0) root         (0)       93 2022-07-05 13:57:48.000000 function-tools-0.4.0/function_tools/function_templates/function_sync_template/enums.py-tpl
+-rw-r--r--   0 root         (0) root         (0)      257 2022-07-12 08:20:24.000000 function-tools-0.4.0/function_tools/function_templates/function_sync_template/errors.py-tpl
+-rw-r--r--   0 root         (0) root         (0)     2831 2022-07-25 11:47:49.000000 function-tools-0.4.0/function_tools/function_templates/function_sync_template/functions.py-tpl
+-rw-r--r--   0 root         (0) root         (0)     1310 2022-07-25 11:47:49.000000 function-tools-0.4.0/function_tools/function_templates/function_sync_template/helpers.py-tpl
+-rw-r--r--   0 root         (0) root         (0)     1601 2022-07-25 11:47:49.000000 function-tools-0.4.0/function_tools/function_templates/function_sync_template/managers.py-tpl
+-rw-r--r--   0 root         (0) root         (0)      326 2022-07-12 08:20:24.000000 function-tools-0.4.0/function_tools/function_templates/function_sync_template/presenters.py-tpl
+-rw-r--r--   0 root         (0) root         (0)      609 2022-07-25 11:47:49.000000 function-tools-0.4.0/function_tools/function_templates/function_sync_template/results.py-tpl
+-rw-r--r--   0 root         (0) root         (0)     2841 2022-07-25 11:47:49.000000 function-tools-0.4.0/function_tools/function_templates/function_sync_template/runners.py-tpl
+-rw-r--r--   0 root         (0) root         (0)      181 2022-07-05 13:57:48.000000 function-tools-0.4.0/function_tools/function_templates/function_sync_template/strings.py-tpl
+-rw-r--r--   0 root         (0) root         (0)       59 2022-07-05 13:57:48.000000 function-tools-0.4.0/function_tools/function_templates/function_sync_template/tests.py-tpl
+-rw-r--r--   0 root         (0) root         (0)      911 2022-07-13 12:17:45.000000 function-tools-0.4.0/function_tools/function_templates/function_sync_template/validators.py-tpl
+-rw-r--r--   0 root         (0) root         (0)    10489 2022-07-25 11:47:49.000000 function-tools-0.4.0/function_tools/functions.py
+-rw-r--r--   0 root         (0) root         (0)     5362 2022-07-25 11:47:49.000000 function-tools-0.4.0/function_tools/general.py
+-rw-r--r--   0 root         (0) root         (0)     2244 2022-07-25 11:47:49.000000 function-tools-0.4.0/function_tools/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 12:26:56.364155 function-tools-0.4.0/function_tools/management/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-02-16 11:53:12.000000 function-tools-0.4.0/function_tools/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 12:26:56.368155 function-tools-0.4.0/function_tools/management/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-02-16 11:53:12.000000 function-tools-0.4.0/function_tools/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7507 2022-07-27 13:25:54.000000 function-tools-0.4.0/function_tools/management/commands/register_entities.py
+-rw-r--r--   0 root         (0) root         (0)    17850 2023-08-04 12:26:47.000000 function-tools-0.4.0/function_tools/management/commands/startfunction.py
+-rw-r--r--   0 root         (0) root         (0)       52 2022-02-16 11:53:12.000000 function-tools-0.4.0/function_tools/management/consts.py
+-rw-r--r--   0 root         (0) root         (0)      598 2022-07-25 11:47:49.000000 function-tools-0.4.0/function_tools/management/strategies.py
+-rw-r--r--   0 root         (0) root         (0)     4957 2022-07-25 11:47:49.000000 function-tools-0.4.0/function_tools/managers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 12:26:56.373155 function-tools-0.4.0/function_tools/migrations/
+-rw-r--r--   0 root         (0) root         (0)     1124 2022-02-16 11:53:12.000000 function-tools-0.4.0/function_tools/migrations/0001_initial.py
+-rw-r--r--   0 root         (0) root         (0)      520 2022-02-16 11:53:12.000000 function-tools-0.4.0/function_tools/migrations/0002_registeredfunction_tags.py
+-rw-r--r--   0 root         (0) root         (0)      795 2022-02-16 11:53:12.000000 function-tools-0.4.0/function_tools/migrations/0003_implementationstrategy.py
+-rw-r--r--   0 root         (0) root         (0)      477 2022-02-16 11:53:12.000000 function-tools-0.4.0/function_tools/migrations/0004_implementationstrategy_order_number.py
+-rw-r--r--   0 root         (0) root         (0)     2736 2022-07-25 11:47:49.000000 function-tools-0.4.0/function_tools/migrations/0005_auto_20220724_0050.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-07-12 12:03:22.000000 function-tools-0.4.0/function_tools/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6434 2022-07-25 11:47:49.000000 function-tools-0.4.0/function_tools/mixins.py
+-rw-r--r--   0 root         (0) root         (0)     4534 2022-11-01 12:27:02.000000 function-tools-0.4.0/function_tools/models.py
+-rw-r--r--   0 root         (0) root         (0)      685 2022-02-16 11:53:12.000000 function-tools-0.4.0/function_tools/presenters.py
+-rw-r--r--   0 root         (0) root         (0)      369 2022-07-27 13:25:54.000000 function-tools-0.4.0/function_tools/receivers.py
+-rw-r--r--   0 root         (0) root         (0)     2386 2022-02-16 11:53:12.000000 function-tools-0.4.0/function_tools/results.py
+-rw-r--r--   0 root         (0) root         (0)    12097 2022-07-25 11:47:49.000000 function-tools-0.4.0/function_tools/runners.py
+-rw-r--r--   0 root         (0) root         (0)    11758 2023-08-04 12:26:47.000000 function-tools-0.4.0/function_tools/storages.py
+-rw-r--r--   0 root         (0) root         (0)    17851 2022-07-25 11:47:49.000000 function-tools-0.4.0/function_tools/strategies.py
+-rw-r--r--   0 root         (0) root         (0)      693 2022-02-16 11:53:12.000000 function-tools-0.4.0/function_tools/strings.py
+-rw-r--r--   0 root         (0) root         (0)      603 2022-02-16 11:53:12.000000 function-tools-0.4.0/function_tools/types.py
+-rw-r--r--   0 root         (0) root         (0)     3234 2022-03-03 06:03:15.000000 function-tools-0.4.0/function_tools/utils.py
+-rw-r--r--   0 root         (0) root         (0)      408 2022-02-16 11:53:12.000000 function-tools-0.4.0/function_tools/validators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 12:26:56.344155 function-tools-0.4.0/function_tools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    21062 2023-08-04 12:26:56.000000 function-tools-0.4.0/function_tools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2679 2023-08-04 12:26:56.000000 function-tools-0.4.0/function_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 12:26:56.000000 function-tools-0.4.0/function_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2023-08-04 12:26:56.000000 function-tools-0.4.0/function_tools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-08-04 12:26:56.000000 function-tools-0.4.0/function_tools.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       47 2022-07-05 13:57:48.000000 function-tools-0.4.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2023-08-04 12:26:56.374155 function-tools-0.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1707 2023-08-04 12:26:47.000000 function-tools-0.4.0/setup.py
```

### Comparing `function-tools-0.3.9/CHANGES.md` & `function-tools-0.4.0/CHANGES.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,56 @@
 # История изменений
+Все изменения проекта должны быть отражены в этом файле.
+
+Формат основан на [Keep a Changelog](http://keepachangelog.com/)
+и проект следует [Семантическому версионированию](http://semver.org/).
+
+## [x.y.z] - гггг-мм-дд
+ 
+Здесь должно быть расширенное описание того, что было сделано, какие есть планы у команды по дальнейшему развитию. 
+Желательно будущие цели привязывать к конкретным задачам. Т.е. на каждую цель нужно поставить отдельную задачу и 
+отразить ее номер здесь.
+ 
+### Добавлено
+- [ПРОЕКТ-ZZZZ](https://jira.bars.group/browse/ПРОЕКТ-ZZZZ)
+  PATCH Название задачи или изменения.
+
+- [ПРОЕКТ-YYYY](https://jira.bars.group/browse/ПРОЕКТ-YYYY)
+  MINOR Название задачи или изменения.
+
+- [ПРОЕКТ-XXXX](https://jira.bars.group/browse/ПРОЕКТ-XXXX)
+  MAJOR Название задачи или изменения.
+ 
+### Изменено
+ 
+### Исправлено
+
+
+## [0.4.0] - 2023-08-04
+ 
+Исправление ошибки поиска сущностей function-tools в пакетах, которые не являются django-приложениями.
+ 
+### Добавлено
+- [EDUSCHL-19919](https://jira.bars.group/browse/EDUSCHL-19919)
+  MINOR Добавление параметра FUNCTION_TOOLS_EXCLUDED_APPS для возможности исключения приложений из поиска сущностей.
+ 
+### Изменено
+
+- [EDUSCHL-19919](https://jira.bars.group/browse/EDUSCHL-19919)
+  PATCH Перенесены настройки для сборки документации в docs.
+ 
+### Исправлено
+
+- [EDUSCHL-19919](https://jira.bars.group/browse/EDUSCHL-19919)
+  PATCH Исправлена ошибка в примере.
+
+
+**0.3.10**
+
+- Исправлена ошибка, из-за которой startfunction не запускался, если в настройках не указан ISORT_CONFIG.
 
 **0.3.9**
 
 - EDUSCHL-19156 Убрана часть кода вызывающая ошибку поиска сущностей, при наличии подключенного приложения, находящегося выше по иерархии, чем, например, функция;
 - EDUSCHL-19156 Добавление описания команды создания Функции;
 - EDUSCHL-19156 Перевод команды создания Функций на использование стратегий из Хранилища;
 - EDUSCHL-19156 Исправление опечаток.
```

### Comparing `function-tools-0.3.9/LICENSE` & `function-tools-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `function-tools-0.3.9/PKG-INFO` & `function-tools-0.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: function-tools
-Version: 0.3.9
+Version: 0.4.0
 Summary: Tools for creating functions
 Home-page: https://github.com/sandanilenko/function-tools
 Author: Alexander Danilenko
 Author-email: a.danilenko@bars.group
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -96,14 +96,62 @@
 
 Подробная актуальная диаграммка классов представлена на Рисунке 2.
 
 ![Рисунок 2](/docs/source/_static/images/class_diagram.png)
 
 С подробной документацией можно ознакомиться на [function-tools.readthedocs.io](https://function-tools.readthedocs.io/ru/latest/)
 # История изменений
+Все изменения проекта должны быть отражены в этом файле.
+
+Формат основан на [Keep a Changelog](http://keepachangelog.com/)
+и проект следует [Семантическому версионированию](http://semver.org/).
+
+## [x.y.z] - гггг-мм-дд
+ 
+Здесь должно быть расширенное описание того, что было сделано, какие есть планы у команды по дальнейшему развитию. 
+Желательно будущие цели привязывать к конкретным задачам. Т.е. на каждую цель нужно поставить отдельную задачу и 
+отразить ее номер здесь.
+ 
+### Добавлено
+- [ПРОЕКТ-ZZZZ](https://jira.bars.group/browse/ПРОЕКТ-ZZZZ)
+  PATCH Название задачи или изменения.
+
+- [ПРОЕКТ-YYYY](https://jira.bars.group/browse/ПРОЕКТ-YYYY)
+  MINOR Название задачи или изменения.
+
+- [ПРОЕКТ-XXXX](https://jira.bars.group/browse/ПРОЕКТ-XXXX)
+  MAJOR Название задачи или изменения.
+ 
+### Изменено
+ 
+### Исправлено
+
+
+## [0.4.0] - 2023-08-04
+ 
+Исправление ошибки поиска сущностей function-tools в пакетах, которые не являются django-приложениями.
+ 
+### Добавлено
+- [EDUSCHL-19919](https://jira.bars.group/browse/EDUSCHL-19919)
+  MINOR Добавление параметра FUNCTION_TOOLS_EXCLUDED_APPS для возможности исключения приложений из поиска сущностей.
+ 
+### Изменено
+
+- [EDUSCHL-19919](https://jira.bars.group/browse/EDUSCHL-19919)
+  PATCH Перенесены настройки для сборки документации в docs.
+ 
+### Исправлено
+
+- [EDUSCHL-19919](https://jira.bars.group/browse/EDUSCHL-19919)
+  PATCH Исправлена ошибка в примере.
+
+
+**0.3.10**
+
+- Исправлена ошибка, из-за которой startfunction не запускался, если в настройках не указан ISORT_CONFIG.
 
 **0.3.9**
 
 - EDUSCHL-19156 Убрана часть кода вызывающая ошибку поиска сущностей, при наличии подключенного приложения, находящегося выше по иерархии, чем, например, функция;
 - EDUSCHL-19156 Добавление описания команды создания Функции;
 - EDUSCHL-19156 Перевод команды создания Функций на использование стратегий из Хранилища;
 - EDUSCHL-19156 Исправление опечаток.
```

### Comparing `function-tools-0.3.9/README.md` & `function-tools-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `function-tools-0.3.9/function_tools/caches.py` & `function-tools-0.4.0/function_tools/caches.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.3.9/function_tools/function_templates/function_sync_template/caches.py-tpl` & `function-tools-0.4.0/function_tools/function_templates/function_sync_template/caches.py-tpl`

 * *Files identical despite different names*

### Comparing `function-tools-0.3.9/function_tools/function_templates/function_sync_template/functions.py-tpl` & `function-tools-0.4.0/function_tools/function_templates/function_sync_template/functions.py-tpl`

 * *Files identical despite different names*

### Comparing `function-tools-0.3.9/function_tools/function_templates/function_sync_template/helpers.py-tpl` & `function-tools-0.4.0/function_tools/function_templates/function_sync_template/helpers.py-tpl`

 * *Files identical despite different names*

### Comparing `function-tools-0.3.9/function_tools/function_templates/function_sync_template/managers.py-tpl` & `function-tools-0.4.0/function_tools/function_templates/function_sync_template/managers.py-tpl`

 * *Files identical despite different names*

### Comparing `function-tools-0.3.9/function_tools/function_templates/function_sync_template/results.py-tpl` & `function-tools-0.4.0/function_tools/function_templates/function_sync_template/results.py-tpl`

 * *Files identical despite different names*

### Comparing `function-tools-0.3.9/function_tools/function_templates/function_sync_template/runners.py-tpl` & `function-tools-0.4.0/function_tools/function_templates/function_sync_template/runners.py-tpl`

 * *Files identical despite different names*

### Comparing `function-tools-0.3.9/function_tools/function_templates/function_sync_template/validators.py-tpl` & `function-tools-0.4.0/function_tools/function_templates/function_sync_template/validators.py-tpl`

 * *Files identical despite different names*

### Comparing `function-tools-0.3.9/function_tools/functions.py` & `function-tools-0.4.0/function_tools/functions.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.3.9/function_tools/general.py` & `function-tools-0.4.0/function_tools/general.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.3.9/function_tools/helpers.py` & `function-tools-0.4.0/function_tools/helpers.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.3.9/function_tools/management/commands/register_entities.py` & `function-tools-0.4.0/function_tools/management/commands/register_entities.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.3.9/function_tools/management/commands/startfunction.py` & `function-tools-0.4.0/function_tools/management/commands/startfunction.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         content: str,
     ):
         """
         Сортировка импортов при помощи isort.
         """
         return sort_code_string(
             code=content,
-            config=getattr(settings, 'ISORT_CONFIG') or DEFAULT_CONFIG,
+            config=getattr(settings, 'ISORT_CONFIG', None) or DEFAULT_CONFIG,
         )
 
     def handle_template(self, template=None, subdir=None):
         """
         Поиск директории с шаблоном функции.
         """
         template_directory_path = None
```

### Comparing `function-tools-0.3.9/function_tools/management/strategies.py` & `function-tools-0.4.0/function_tools/management/strategies.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.3.9/function_tools/managers.py` & `function-tools-0.4.0/function_tools/managers.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.3.9/function_tools/migrations/0001_initial.py` & `function-tools-0.4.0/function_tools/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.3.9/function_tools/migrations/0002_registeredfunction_tags.py` & `function-tools-0.4.0/function_tools/migrations/0002_registeredfunction_tags.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.3.9/function_tools/migrations/0003_implementationstrategy.py` & `function-tools-0.4.0/function_tools/migrations/0003_implementationstrategy.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.3.9/function_tools/migrations/0005_auto_20220724_0050.py` & `function-tools-0.4.0/function_tools/migrations/0005_auto_20220724_0050.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.3.9/function_tools/mixins.py` & `function-tools-0.4.0/function_tools/mixins.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.3.9/function_tools/models.py` & `function-tools-0.4.0/function_tools/models.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.3.9/function_tools/presenters.py` & `function-tools-0.4.0/function_tools/presenters.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.3.9/function_tools/results.py` & `function-tools-0.4.0/function_tools/results.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.3.9/function_tools/runners.py` & `function-tools-0.4.0/function_tools/runners.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.3.9/function_tools/storages.py` & `function-tools-0.4.0/function_tools/storages.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,15 +147,15 @@
         Args:
             application_name: имя приложения
         """
         application_path = self._get_application_path(application_name=application_name)
 
         if application_path:
             for entity_module_pattern in self._entity_module_patterns:
-                entity_module_paths = application_path.glob(entity_module_pattern)
+                entity_module_paths = application_path.rglob(entity_module_pattern)
 
                 for entity_module_path in entity_module_paths:
                     entity_module_path = str(entity_module_path)
 
                     import_path = self._get_module_import_path(
                         module_path=entity_module_path,
                     )
@@ -171,15 +171,21 @@
 
             self._checked_application_paths.append(application_path)
 
     def _find_entities_modules(self):
         """
         Поиск модулей зарегистрированных типов сущностей.
         """
-        for application_name in settings.INSTALLED_APPS:
+        filtered_applications = [
+            application_name
+            for application_name in settings.INSTALLED_APPS
+            if application_name not in settings.FUNCTION_TOOLS_EXCLUDED_APPS
+        ]
+
+        for application_name in filtered_applications:
             self._find_application_entities_modules(application_name=application_name)
 
     def _prepare_entities(self):
         """
         Поиск фабрик во всех подключенных приложениях.
         """
         processed_paths = list()
```

### Comparing `function-tools-0.3.9/function_tools/strategies.py` & `function-tools-0.4.0/function_tools/strategies.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.3.9/function_tools/strings.py` & `function-tools-0.4.0/function_tools/strings.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.3.9/function_tools/types.py` & `function-tools-0.4.0/function_tools/types.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.3.9/function_tools/utils.py` & `function-tools-0.4.0/function_tools/utils.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.3.9/function_tools.egg-info/PKG-INFO` & `function-tools-0.4.0/function_tools.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: function-tools
-Version: 0.3.9
+Version: 0.4.0
 Summary: Tools for creating functions
 Home-page: https://github.com/sandanilenko/function-tools
 Author: Alexander Danilenko
 Author-email: a.danilenko@bars.group
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -96,14 +96,62 @@
 
 Подробная актуальная диаграммка классов представлена на Рисунке 2.
 
 ![Рисунок 2](/docs/source/_static/images/class_diagram.png)
 
 С подробной документацией можно ознакомиться на [function-tools.readthedocs.io](https://function-tools.readthedocs.io/ru/latest/)
 # История изменений
+Все изменения проекта должны быть отражены в этом файле.
+
+Формат основан на [Keep a Changelog](http://keepachangelog.com/)
+и проект следует [Семантическому версионированию](http://semver.org/).
+
+## [x.y.z] - гггг-мм-дд
+ 
+Здесь должно быть расширенное описание того, что было сделано, какие есть планы у команды по дальнейшему развитию. 
+Желательно будущие цели привязывать к конкретным задачам. Т.е. на каждую цель нужно поставить отдельную задачу и 
+отразить ее номер здесь.
+ 
+### Добавлено
+- [ПРОЕКТ-ZZZZ](https://jira.bars.group/browse/ПРОЕКТ-ZZZZ)
+  PATCH Название задачи или изменения.
+
+- [ПРОЕКТ-YYYY](https://jira.bars.group/browse/ПРОЕКТ-YYYY)
+  MINOR Название задачи или изменения.
+
+- [ПРОЕКТ-XXXX](https://jira.bars.group/browse/ПРОЕКТ-XXXX)
+  MAJOR Название задачи или изменения.
+ 
+### Изменено
+ 
+### Исправлено
+
+
+## [0.4.0] - 2023-08-04
+ 
+Исправление ошибки поиска сущностей function-tools в пакетах, которые не являются django-приложениями.
+ 
+### Добавлено
+- [EDUSCHL-19919](https://jira.bars.group/browse/EDUSCHL-19919)
+  MINOR Добавление параметра FUNCTION_TOOLS_EXCLUDED_APPS для возможности исключения приложений из поиска сущностей.
+ 
+### Изменено
+
+- [EDUSCHL-19919](https://jira.bars.group/browse/EDUSCHL-19919)
+  PATCH Перенесены настройки для сборки документации в docs.
+ 
+### Исправлено
+
+- [EDUSCHL-19919](https://jira.bars.group/browse/EDUSCHL-19919)
+  PATCH Исправлена ошибка в примере.
+
+
+**0.3.10**
+
+- Исправлена ошибка, из-за которой startfunction не запускался, если в настройках не указан ISORT_CONFIG.
 
 **0.3.9**
 
 - EDUSCHL-19156 Убрана часть кода вызывающая ошибку поиска сущностей, при наличии подключенного приложения, находящегося выше по иерархии, чем, например, функция;
 - EDUSCHL-19156 Добавление описания команды создания Функции;
 - EDUSCHL-19156 Перевод команды создания Функций на использование стратегий из Хранилища;
 - EDUSCHL-19156 Исправление опечаток.
```

### Comparing `function-tools-0.3.9/function_tools.egg-info/SOURCES.txt` & `function-tools-0.4.0/function_tools.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 LICENSE
 MANIFEST.in
 README.md
 requirements.txt
 setup.cfg
 setup.py
 function_tools/__init__.py
+function_tools/app_settings.py
 function_tools/apps.py
 function_tools/caches.py
 function_tools/consts.py
 function_tools/decorators.py
 function_tools/enums.py
 function_tools/errors.py
 function_tools/functions.py
```

### Comparing `function-tools-0.3.9/setup.py` & `function-tools-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from setuptools import (
     find_packages,
     setup,
 )
 
 
-__version__ = '0.3.9'
+__version__ = '0.4.0'
 
 
 here = path.abspath(path.dirname(__file__))
 
 
 # Get the long description from the README file
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
```

