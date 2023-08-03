# Comparing `tmp/pdpp-0.4.7.tar.gz` & `tmp/pdpp-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdpp-0.4.7.tar", last modified: Thu Aug  3 23:52:38 2023, max compression
+gzip compressed data, was "pdpp-0.4.8.tar", last modified: Thu Aug  3 23:55:37 2023, max compression
```

## Comparing `pdpp-0.4.7.tar` & `pdpp-0.4.8.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxr-x   0 pierson   (1000) pierson   (1000)        0 2023-08-03 23:52:38.577529 pdpp-0.4.7/
--rwxrwxr-x   0 pierson   (1000) pierson   (1000)     1063 2023-03-30 23:25:51.000000 pdpp-0.4.7/LICENSE.txt
--rw-rw-r--   0 pierson   (1000) pierson   (1000)      481 2023-08-03 23:52:38.577529 pdpp-0.4.7/PKG-INFO
--rw-rw-r--   0 pierson   (1000) pierson   (1000)    12037 2023-08-03 23:51:09.000000 pdpp-0.4.7/README.md
-drwxrwxr-x   0 pierson   (1000) pierson   (1000)        0 2023-08-03 23:52:38.569529 pdpp-0.4.7/pdpp/
--rwxrwxr-x   0 pierson   (1000) pierson   (1000)        0 2022-10-17 19:41:09.000000 pdpp-0.4.7/pdpp/__init__.py
-drwxrwxr-x   0 pierson   (1000) pierson   (1000)        0 2023-08-03 23:52:38.573529 pdpp-0.4.7/pdpp/automation/
--rwxrwxr-x   0 pierson   (1000) pierson   (1000)        0 2022-10-17 19:41:09.000000 pdpp-0.4.7/pdpp/automation/__init__.py
--rwxrwxr-x   0 pierson   (1000) pierson   (1000)      165 2022-10-17 19:41:09.000000 pdpp-0.4.7/pdpp/automation/doit_run.py
--rwxrwxr-x   0 pierson   (1000) pierson   (1000)     2393 2022-10-17 19:41:09.000000 pdpp-0.4.7/pdpp/automation/link_task.py
--rwxrwxr-x   0 pierson   (1000) pierson   (1000)      459 2022-10-17 19:41:09.000000 pdpp-0.4.7/pdpp/automation/mylinker.py
--rwxrwxr-x   0 pierson   (1000) pierson   (1000)     1838 2022-10-17 20:28:37.000000 pdpp-0.4.7/pdpp/automation/task_creator.py
--rwxrwxr-x   0 pierson   (1000) pierson   (1000)     1115 2022-10-17 19:41:09.000000 pdpp-0.4.7/pdpp/automation/task_enabler.py
-drwxrwxr-x   0 pierson   (1000) pierson   (1000)        0 2023-08-03 23:52:38.573529 pdpp-0.4.7/pdpp/languages/
--rwxrwxr-x   0 pierson   (1000) pierson   (1000)        0 2022-10-17 19:41:09.000000 pdpp-0.4.7/pdpp/languages/__init__.py
--rw-rw-r--   0 pierson   (1000) pierson   (1000)      612 2022-10-17 19:41:09.000000 pdpp-0.4.7/pdpp/languages/extension_parser.py
--rw-rw-r--   0 pierson   (1000) pierson   (1000)       92 2022-10-17 19:41:09.000000 pdpp-0.4.7/pdpp/languages/language_enum.py
--rw-rw-r--   0 pierson   (1000) pierson   (1000)      370 2022-10-17 19:41:09.000000 pdpp-0.4.7/pdpp/languages/language_parser.py
--rw-rw-r--   0 pierson   (1000) pierson   (1000)      650 2022-10-17 19:41:09.000000 pdpp-0.4.7/pdpp/languages/runners.py
--rwxrwxr-x   0 pierson   (1000) pierson   (1000)     5278 2022-10-17 20:25:25.000000 pdpp-0.4.7/pdpp/main.py
-drwxrwxr-x   0 pierson   (1000) pierson   (1000)        0 2023-08-03 23:52:38.573529 pdpp-0.4.7/pdpp/questions/
--rwxrwxr-x   0 pierson   (1000) pierson   (1000)      163 2022-10-17 19:41:09.000000 pdpp-0.4.7/pdpp/questions/__init__.py
--rwxrwxr-x   0 pierson   (1000) pierson   (1000)      873 2022-10-17 19:41:09.000000 pdpp-0.4.7/pdpp/questions/question_0.py
--rwxrwxr-x   0 pierson   (1000) pierson   (1000)     1668 2022-10-17 19:41:09.000000 pdpp-0.4.7/pdpp/questions/question_1.py
--rwxrwxr-x   0 pierson   (1000) pierson   (1000)     2914 2022-10-17 19:41:09.000000 pdpp-0.4.7/pdpp/questions/question_2.py
--rwxrwxr-x   0 pierson   (1000) pierson   (1000)     1417 2022-10-17 19:41:09.000000 pdpp-0.4.7/pdpp/questions/question_3.py
--rwxrwxr-x   0 pierson   (1000) pierson   (1000)     1944 2023-07-26 20:34:29.000000 pdpp-0.4.7/pdpp/questions/question_4.py
--rw-rw-r--   0 pierson   (1000) pierson   (1000)     1113 2022-10-17 19:41:09.000000 pdpp-0.4.7/pdpp/questions/question_extant.py
-drwxrwxr-x   0 pierson   (1000) pierson   (1000)        0 2023-08-03 23:52:38.577529 pdpp-0.4.7/pdpp/styles/
--rwxrwxr-x   0 pierson   (1000) pierson   (1000)        0 2022-10-17 19:41:09.000000 pdpp-0.4.7/pdpp/styles/__init__.py
--rw-rw-r--   0 pierson   (1000) pierson   (1000)     1716 2022-10-17 19:41:09.000000 pdpp-0.4.7/pdpp/styles/graph_style.py
--rwxrwxr-x   0 pierson   (1000) pierson   (1000)      593 2022-10-17 19:41:09.000000 pdpp-0.4.7/pdpp/styles/prompt_style.py
-drwxrwxr-x   0 pierson   (1000) pierson   (1000)        0 2023-08-03 23:52:38.577529 pdpp-0.4.7/pdpp/tasks/
--rw-rw-r--   0 pierson   (1000) pierson   (1000)        0 2022-10-17 19:41:09.000000 pdpp-0.4.7/pdpp/tasks/__init__.py
--rw-rw-r--   0 pierson   (1000) pierson   (1000)     2430 2022-10-17 19:41:09.000000 pdpp-0.4.7/pdpp/tasks/base_task.py
--rw-rw-r--   0 pierson   (1000) pierson   (1000)     1692 2022-10-17 19:41:09.000000 pdpp-0.4.7/pdpp/tasks/custom_task.py
--rw-rw-r--   0 pierson   (1000) pierson   (1000)     1136 2022-10-17 19:41:09.000000 pdpp-0.4.7/pdpp/tasks/export_task.py
--rw-rw-r--   0 pierson   (1000) pierson   (1000)     1286 2022-10-17 19:41:09.000000 pdpp-0.4.7/pdpp/tasks/import_task.py
--rw-rw-r--   0 pierson   (1000) pierson   (1000)     1666 2022-10-17 19:41:09.000000 pdpp-0.4.7/pdpp/tasks/standard_task.py
--rw-rw-r--   0 pierson   (1000) pierson   (1000)     1466 2022-10-17 19:41:09.000000 pdpp-0.4.7/pdpp/tasks/sub_task.py
-drwxrwxr-x   0 pierson   (1000) pierson   (1000)        0 2023-08-03 23:52:38.577529 pdpp-0.4.7/pdpp/templates/
--rw-rw-r--   0 pierson   (1000) pierson   (1000)        0 2022-10-17 19:41:09.000000 pdpp-0.4.7/pdpp/templates/__init__.py
--rw-rw-r--   0 pierson   (1000) pierson   (1000)     2323 2022-10-17 19:41:09.000000 pdpp-0.4.7/pdpp/templates/create_gitignore.py
--rw-rw-r--   0 pierson   (1000) pierson   (1000)      542 2022-10-17 19:41:09.000000 pdpp-0.4.7/pdpp/templates/create_in_out_src.py
--rw-rw-r--   0 pierson   (1000) pierson   (1000)      502 2022-10-17 19:41:09.000000 pdpp-0.4.7/pdpp/templates/dep_dataclass.py
--rw-rw-r--   0 pierson   (1000) pierson   (1000)      210 2022-10-17 19:41:09.000000 pdpp-0.4.7/pdpp/templates/dodo_template.py
--rw-rw-r--   0 pierson   (1000) pierson   (1000)      575 2022-10-17 19:41:09.000000 pdpp-0.4.7/pdpp/templates/populate_new_project.py
-drwxrwxr-x   0 pierson   (1000) pierson   (1000)        0 2023-08-03 23:52:38.577529 pdpp-0.4.7/pdpp/utils/
--rwxrwxr-x   0 pierson   (1000) pierson   (1000)        0 2022-10-17 19:41:09.000000 pdpp-0.4.7/pdpp/utils/__init__.py
--rw-rw-r--   0 pierson   (1000) pierson   (1000)     1918 2022-10-17 19:41:09.000000 pdpp-0.4.7/pdpp/utils/directory_test.py
--rw-rw-r--   0 pierson   (1000) pierson   (1000)      313 2022-10-17 19:41:09.000000 pdpp-0.4.7/pdpp/utils/execute_at_target.py
--rwxrwxr-x   0 pierson   (1000) pierson   (1000)     7336 2022-10-17 21:03:33.000000 pdpp-0.4.7/pdpp/utils/graph_dependencies.py
--rw-rw-r--   0 pierson   (1000) pierson   (1000)      131 2022-10-17 19:41:09.000000 pdpp-0.4.7/pdpp/utils/ignorelist.py
--rwxrwxr-x   0 pierson   (1000) pierson   (1000)     1171 2022-10-17 19:41:09.000000 pdpp-0.4.7/pdpp/utils/immediate_link.py
--rwxrwxr-x   0 pierson   (1000) pierson   (1000)      252 2022-10-17 19:41:09.000000 pdpp-0.4.7/pdpp/utils/rem_slash.py
--rwxrwxr-x   0 pierson   (1000) pierson   (1000)     2241 2022-10-17 19:41:09.000000 pdpp-0.4.7/pdpp/utils/task_directory_test.py
--rw-rw-r--   0 pierson   (1000) pierson   (1000)      513 2022-10-17 19:41:09.000000 pdpp-0.4.7/pdpp/utils/yaml_task.py
-drwxrwxr-x   0 pierson   (1000) pierson   (1000)        0 2023-08-03 23:52:38.569529 pdpp-0.4.7/pdpp.egg-info/
--rw-rw-r--   0 pierson   (1000) pierson   (1000)      481 2023-08-03 23:52:38.000000 pdpp-0.4.7/pdpp.egg-info/PKG-INFO
--rw-rw-r--   0 pierson   (1000) pierson   (1000)     1476 2023-08-03 23:52:38.000000 pdpp-0.4.7/pdpp.egg-info/SOURCES.txt
--rw-rw-r--   0 pierson   (1000) pierson   (1000)        1 2023-08-03 23:52:38.000000 pdpp-0.4.7/pdpp.egg-info/dependency_links.txt
--rw-rw-r--   0 pierson   (1000) pierson   (1000)       40 2023-08-03 23:52:38.000000 pdpp-0.4.7/pdpp.egg-info/entry_points.txt
--rw-rw-r--   0 pierson   (1000) pierson   (1000)       99 2023-08-03 23:52:38.000000 pdpp-0.4.7/pdpp.egg-info/requires.txt
--rw-rw-r--   0 pierson   (1000) pierson   (1000)        5 2023-08-03 23:52:38.000000 pdpp-0.4.7/pdpp.egg-info/top_level.txt
--rw-rw-r--   0 pierson   (1000) pierson   (1000)       38 2023-08-03 23:52:38.577529 pdpp-0.4.7/setup.cfg
--rwxrwxr-x   0 pierson   (1000) pierson   (1000)      923 2023-08-03 23:52:04.000000 pdpp-0.4.7/setup.py
+drwxrwxr-x   0 pierson   (1000) pierson   (1000)        0 2023-08-03 23:55:37.523433 pdpp-0.4.8/
+-rwxrwxr-x   0 pierson   (1000) pierson   (1000)     1063 2023-03-30 23:25:51.000000 pdpp-0.4.8/LICENSE.txt
+-rw-rw-r--   0 pierson   (1000) pierson   (1000)    12560 2023-08-03 23:55:37.523433 pdpp-0.4.8/PKG-INFO
+-rw-rw-r--   0 pierson   (1000) pierson   (1000)    12037 2023-08-03 23:51:09.000000 pdpp-0.4.8/README.md
+drwxrwxr-x   0 pierson   (1000) pierson   (1000)        0 2023-08-03 23:55:37.519432 pdpp-0.4.8/pdpp/
+-rwxrwxr-x   0 pierson   (1000) pierson   (1000)        0 2022-10-17 19:41:09.000000 pdpp-0.4.8/pdpp/__init__.py
+drwxrwxr-x   0 pierson   (1000) pierson   (1000)        0 2023-08-03 23:55:37.519432 pdpp-0.4.8/pdpp/automation/
+-rwxrwxr-x   0 pierson   (1000) pierson   (1000)        0 2022-10-17 19:41:09.000000 pdpp-0.4.8/pdpp/automation/__init__.py
+-rwxrwxr-x   0 pierson   (1000) pierson   (1000)      165 2022-10-17 19:41:09.000000 pdpp-0.4.8/pdpp/automation/doit_run.py
+-rwxrwxr-x   0 pierson   (1000) pierson   (1000)     2393 2022-10-17 19:41:09.000000 pdpp-0.4.8/pdpp/automation/link_task.py
+-rwxrwxr-x   0 pierson   (1000) pierson   (1000)      459 2022-10-17 19:41:09.000000 pdpp-0.4.8/pdpp/automation/mylinker.py
+-rwxrwxr-x   0 pierson   (1000) pierson   (1000)     1838 2022-10-17 20:28:37.000000 pdpp-0.4.8/pdpp/automation/task_creator.py
+-rwxrwxr-x   0 pierson   (1000) pierson   (1000)     1115 2022-10-17 19:41:09.000000 pdpp-0.4.8/pdpp/automation/task_enabler.py
+drwxrwxr-x   0 pierson   (1000) pierson   (1000)        0 2023-08-03 23:55:37.519432 pdpp-0.4.8/pdpp/languages/
+-rwxrwxr-x   0 pierson   (1000) pierson   (1000)        0 2022-10-17 19:41:09.000000 pdpp-0.4.8/pdpp/languages/__init__.py
+-rw-rw-r--   0 pierson   (1000) pierson   (1000)      612 2022-10-17 19:41:09.000000 pdpp-0.4.8/pdpp/languages/extension_parser.py
+-rw-rw-r--   0 pierson   (1000) pierson   (1000)       92 2022-10-17 19:41:09.000000 pdpp-0.4.8/pdpp/languages/language_enum.py
+-rw-rw-r--   0 pierson   (1000) pierson   (1000)      370 2022-10-17 19:41:09.000000 pdpp-0.4.8/pdpp/languages/language_parser.py
+-rw-rw-r--   0 pierson   (1000) pierson   (1000)      650 2022-10-17 19:41:09.000000 pdpp-0.4.8/pdpp/languages/runners.py
+-rwxrwxr-x   0 pierson   (1000) pierson   (1000)     5278 2022-10-17 20:25:25.000000 pdpp-0.4.8/pdpp/main.py
+drwxrwxr-x   0 pierson   (1000) pierson   (1000)        0 2023-08-03 23:55:37.523433 pdpp-0.4.8/pdpp/questions/
+-rwxrwxr-x   0 pierson   (1000) pierson   (1000)      163 2022-10-17 19:41:09.000000 pdpp-0.4.8/pdpp/questions/__init__.py
+-rwxrwxr-x   0 pierson   (1000) pierson   (1000)      873 2022-10-17 19:41:09.000000 pdpp-0.4.8/pdpp/questions/question_0.py
+-rwxrwxr-x   0 pierson   (1000) pierson   (1000)     1668 2022-10-17 19:41:09.000000 pdpp-0.4.8/pdpp/questions/question_1.py
+-rwxrwxr-x   0 pierson   (1000) pierson   (1000)     2914 2022-10-17 19:41:09.000000 pdpp-0.4.8/pdpp/questions/question_2.py
+-rwxrwxr-x   0 pierson   (1000) pierson   (1000)     1417 2022-10-17 19:41:09.000000 pdpp-0.4.8/pdpp/questions/question_3.py
+-rwxrwxr-x   0 pierson   (1000) pierson   (1000)     1944 2023-07-26 20:34:29.000000 pdpp-0.4.8/pdpp/questions/question_4.py
+-rw-rw-r--   0 pierson   (1000) pierson   (1000)     1113 2022-10-17 19:41:09.000000 pdpp-0.4.8/pdpp/questions/question_extant.py
+drwxrwxr-x   0 pierson   (1000) pierson   (1000)        0 2023-08-03 23:55:37.523433 pdpp-0.4.8/pdpp/styles/
+-rwxrwxr-x   0 pierson   (1000) pierson   (1000)        0 2022-10-17 19:41:09.000000 pdpp-0.4.8/pdpp/styles/__init__.py
+-rw-rw-r--   0 pierson   (1000) pierson   (1000)     1716 2022-10-17 19:41:09.000000 pdpp-0.4.8/pdpp/styles/graph_style.py
+-rwxrwxr-x   0 pierson   (1000) pierson   (1000)      593 2022-10-17 19:41:09.000000 pdpp-0.4.8/pdpp/styles/prompt_style.py
+drwxrwxr-x   0 pierson   (1000) pierson   (1000)        0 2023-08-03 23:55:37.523433 pdpp-0.4.8/pdpp/tasks/
+-rw-rw-r--   0 pierson   (1000) pierson   (1000)        0 2022-10-17 19:41:09.000000 pdpp-0.4.8/pdpp/tasks/__init__.py
+-rw-rw-r--   0 pierson   (1000) pierson   (1000)     2430 2022-10-17 19:41:09.000000 pdpp-0.4.8/pdpp/tasks/base_task.py
+-rw-rw-r--   0 pierson   (1000) pierson   (1000)     1692 2022-10-17 19:41:09.000000 pdpp-0.4.8/pdpp/tasks/custom_task.py
+-rw-rw-r--   0 pierson   (1000) pierson   (1000)     1136 2022-10-17 19:41:09.000000 pdpp-0.4.8/pdpp/tasks/export_task.py
+-rw-rw-r--   0 pierson   (1000) pierson   (1000)     1286 2022-10-17 19:41:09.000000 pdpp-0.4.8/pdpp/tasks/import_task.py
+-rw-rw-r--   0 pierson   (1000) pierson   (1000)     1666 2022-10-17 19:41:09.000000 pdpp-0.4.8/pdpp/tasks/standard_task.py
+-rw-rw-r--   0 pierson   (1000) pierson   (1000)     1466 2022-10-17 19:41:09.000000 pdpp-0.4.8/pdpp/tasks/sub_task.py
+drwxrwxr-x   0 pierson   (1000) pierson   (1000)        0 2023-08-03 23:55:37.523433 pdpp-0.4.8/pdpp/templates/
+-rw-rw-r--   0 pierson   (1000) pierson   (1000)        0 2022-10-17 19:41:09.000000 pdpp-0.4.8/pdpp/templates/__init__.py
+-rw-rw-r--   0 pierson   (1000) pierson   (1000)     2323 2022-10-17 19:41:09.000000 pdpp-0.4.8/pdpp/templates/create_gitignore.py
+-rw-rw-r--   0 pierson   (1000) pierson   (1000)      542 2022-10-17 19:41:09.000000 pdpp-0.4.8/pdpp/templates/create_in_out_src.py
+-rw-rw-r--   0 pierson   (1000) pierson   (1000)      502 2022-10-17 19:41:09.000000 pdpp-0.4.8/pdpp/templates/dep_dataclass.py
+-rw-rw-r--   0 pierson   (1000) pierson   (1000)      210 2022-10-17 19:41:09.000000 pdpp-0.4.8/pdpp/templates/dodo_template.py
+-rw-rw-r--   0 pierson   (1000) pierson   (1000)      575 2022-10-17 19:41:09.000000 pdpp-0.4.8/pdpp/templates/populate_new_project.py
+drwxrwxr-x   0 pierson   (1000) pierson   (1000)        0 2023-08-03 23:55:37.523433 pdpp-0.4.8/pdpp/utils/
+-rwxrwxr-x   0 pierson   (1000) pierson   (1000)        0 2022-10-17 19:41:09.000000 pdpp-0.4.8/pdpp/utils/__init__.py
+-rw-rw-r--   0 pierson   (1000) pierson   (1000)     1918 2022-10-17 19:41:09.000000 pdpp-0.4.8/pdpp/utils/directory_test.py
+-rw-rw-r--   0 pierson   (1000) pierson   (1000)      313 2022-10-17 19:41:09.000000 pdpp-0.4.8/pdpp/utils/execute_at_target.py
+-rwxrwxr-x   0 pierson   (1000) pierson   (1000)     7336 2022-10-17 21:03:33.000000 pdpp-0.4.8/pdpp/utils/graph_dependencies.py
+-rw-rw-r--   0 pierson   (1000) pierson   (1000)      131 2022-10-17 19:41:09.000000 pdpp-0.4.8/pdpp/utils/ignorelist.py
+-rwxrwxr-x   0 pierson   (1000) pierson   (1000)     1171 2022-10-17 19:41:09.000000 pdpp-0.4.8/pdpp/utils/immediate_link.py
+-rwxrwxr-x   0 pierson   (1000) pierson   (1000)      252 2022-10-17 19:41:09.000000 pdpp-0.4.8/pdpp/utils/rem_slash.py
+-rwxrwxr-x   0 pierson   (1000) pierson   (1000)     2241 2022-10-17 19:41:09.000000 pdpp-0.4.8/pdpp/utils/task_directory_test.py
+-rw-rw-r--   0 pierson   (1000) pierson   (1000)      513 2022-10-17 19:41:09.000000 pdpp-0.4.8/pdpp/utils/yaml_task.py
+drwxrwxr-x   0 pierson   (1000) pierson   (1000)        0 2023-08-03 23:55:37.519432 pdpp-0.4.8/pdpp.egg-info/
+-rw-rw-r--   0 pierson   (1000) pierson   (1000)    12560 2023-08-03 23:55:37.000000 pdpp-0.4.8/pdpp.egg-info/PKG-INFO
+-rw-rw-r--   0 pierson   (1000) pierson   (1000)     1476 2023-08-03 23:55:37.000000 pdpp-0.4.8/pdpp.egg-info/SOURCES.txt
+-rw-rw-r--   0 pierson   (1000) pierson   (1000)        1 2023-08-03 23:55:37.000000 pdpp-0.4.8/pdpp.egg-info/dependency_links.txt
+-rw-rw-r--   0 pierson   (1000) pierson   (1000)       40 2023-08-03 23:55:37.000000 pdpp-0.4.8/pdpp.egg-info/entry_points.txt
+-rw-rw-r--   0 pierson   (1000) pierson   (1000)       99 2023-08-03 23:55:37.000000 pdpp-0.4.8/pdpp.egg-info/requires.txt
+-rw-rw-r--   0 pierson   (1000) pierson   (1000)        5 2023-08-03 23:55:37.000000 pdpp-0.4.8/pdpp.egg-info/top_level.txt
+-rw-rw-r--   0 pierson   (1000) pierson   (1000)       38 2023-08-03 23:55:37.523433 pdpp-0.4.8/setup.cfg
+-rwxrwxr-x   0 pierson   (1000) pierson   (1000)     1134 2023-08-03 23:55:31.000000 pdpp-0.4.8/setup.py
```

### Comparing `pdpp-0.4.7/LICENSE.txt` & `pdpp-0.4.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pdpp-0.4.7/README.md` & `pdpp-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `pdpp-0.4.7/pdpp/automation/link_task.py` & `pdpp-0.4.8/pdpp/automation/link_task.py`

 * *Files identical despite different names*

### Comparing `pdpp-0.4.7/pdpp/automation/task_creator.py` & `pdpp-0.4.8/pdpp/automation/task_creator.py`

 * *Files identical despite different names*

### Comparing `pdpp-0.4.7/pdpp/automation/task_enabler.py` & `pdpp-0.4.8/pdpp/automation/task_enabler.py`

 * *Files identical despite different names*

### Comparing `pdpp-0.4.7/pdpp/languages/extension_parser.py` & `pdpp-0.4.8/pdpp/languages/extension_parser.py`

 * *Files identical despite different names*

### Comparing `pdpp-0.4.7/pdpp/languages/runners.py` & `pdpp-0.4.8/pdpp/languages/runners.py`

 * *Files identical despite different names*

### Comparing `pdpp-0.4.7/pdpp/main.py` & `pdpp-0.4.8/pdpp/main.py`

 * *Files identical despite different names*

### Comparing `pdpp-0.4.7/pdpp/questions/question_0.py` & `pdpp-0.4.8/pdpp/questions/question_0.py`

 * *Files identical despite different names*

### Comparing `pdpp-0.4.7/pdpp/questions/question_1.py` & `pdpp-0.4.8/pdpp/questions/question_1.py`

 * *Files identical despite different names*

### Comparing `pdpp-0.4.7/pdpp/questions/question_2.py` & `pdpp-0.4.8/pdpp/questions/question_2.py`

 * *Files identical despite different names*

### Comparing `pdpp-0.4.7/pdpp/questions/question_3.py` & `pdpp-0.4.8/pdpp/questions/question_3.py`

 * *Files identical despite different names*

### Comparing `pdpp-0.4.7/pdpp/questions/question_4.py` & `pdpp-0.4.8/pdpp/questions/question_4.py`

 * *Files identical despite different names*

### Comparing `pdpp-0.4.7/pdpp/questions/question_extant.py` & `pdpp-0.4.8/pdpp/questions/question_extant.py`

 * *Files identical despite different names*

### Comparing `pdpp-0.4.7/pdpp/styles/graph_style.py` & `pdpp-0.4.8/pdpp/styles/graph_style.py`

 * *Files identical despite different names*

### Comparing `pdpp-0.4.7/pdpp/styles/prompt_style.py` & `pdpp-0.4.8/pdpp/styles/prompt_style.py`

 * *Files identical despite different names*

### Comparing `pdpp-0.4.7/pdpp/tasks/base_task.py` & `pdpp-0.4.8/pdpp/tasks/base_task.py`

 * *Files identical despite different names*

### Comparing `pdpp-0.4.7/pdpp/tasks/custom_task.py` & `pdpp-0.4.8/pdpp/tasks/custom_task.py`

 * *Files identical despite different names*

### Comparing `pdpp-0.4.7/pdpp/tasks/export_task.py` & `pdpp-0.4.8/pdpp/tasks/export_task.py`

 * *Files identical despite different names*

### Comparing `pdpp-0.4.7/pdpp/tasks/import_task.py` & `pdpp-0.4.8/pdpp/tasks/import_task.py`

 * *Files identical despite different names*

### Comparing `pdpp-0.4.7/pdpp/tasks/standard_task.py` & `pdpp-0.4.8/pdpp/tasks/standard_task.py`

 * *Files identical despite different names*

### Comparing `pdpp-0.4.7/pdpp/tasks/sub_task.py` & `pdpp-0.4.8/pdpp/tasks/sub_task.py`

 * *Files identical despite different names*

### Comparing `pdpp-0.4.7/pdpp/templates/create_gitignore.py` & `pdpp-0.4.8/pdpp/templates/create_gitignore.py`

 * *Files identical despite different names*

### Comparing `pdpp-0.4.7/pdpp/templates/create_in_out_src.py` & `pdpp-0.4.8/pdpp/templates/create_in_out_src.py`

 * *Files identical despite different names*

### Comparing `pdpp-0.4.7/pdpp/templates/populate_new_project.py` & `pdpp-0.4.8/pdpp/templates/populate_new_project.py`

 * *Files identical despite different names*

### Comparing `pdpp-0.4.7/pdpp/utils/directory_test.py` & `pdpp-0.4.8/pdpp/utils/directory_test.py`

 * *Files identical despite different names*

### Comparing `pdpp-0.4.7/pdpp/utils/graph_dependencies.py` & `pdpp-0.4.8/pdpp/utils/graph_dependencies.py`

 * *Files identical despite different names*

### Comparing `pdpp-0.4.7/pdpp/utils/immediate_link.py` & `pdpp-0.4.8/pdpp/utils/immediate_link.py`

 * *Files identical despite different names*

### Comparing `pdpp-0.4.7/pdpp/utils/task_directory_test.py` & `pdpp-0.4.8/pdpp/utils/task_directory_test.py`

 * *Files identical despite different names*

### Comparing `pdpp-0.4.7/pdpp/utils/yaml_task.py` & `pdpp-0.4.8/pdpp/utils/yaml_task.py`

 * *Files identical despite different names*

### Comparing `pdpp-0.4.7/pdpp.egg-info/SOURCES.txt` & `pdpp-0.4.8/pdpp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

