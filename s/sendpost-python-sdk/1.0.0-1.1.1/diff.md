# Comparing `tmp/sendpost_python_sdk-1.0.0.tar.gz` & `tmp/sendpost_python_sdk-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sendpost_python_sdk-1.0.0.tar", last modified: Wed Jul 26 13:31:19 2023, max compression
+gzip compressed data, was "dist/sendpost_python_sdk-1.1.1.tar", last modified: Fri Aug  4 13:11:42 2023, max compression
```

## Comparing `sendpost_python_sdk-1.0.0.tar` & `sendpost_python_sdk-1.1.1.tar`

### file list

```diff
@@ -1,82 +1,113 @@
-drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 13:31:19.000000 sendpost_python_sdk-1.0.0/
--rw-r--r--   0 arseniy    (501) staff       (20)      663 2023-07-26 13:31:19.000000 sendpost_python_sdk-1.0.0/PKG-INFO
--rw-r--r--   0 arseniy    (501) staff       (20)     3180 2023-07-26 12:36:30.000000 sendpost_python_sdk-1.0.0/README.md
-drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 13:31:19.000000 sendpost_python_sdk-1.0.0/sendpost_python_sdk/
--rw-r--r--   0 arseniy    (501) staff       (20)      979 2023-07-26 12:34:01.000000 sendpost_python_sdk-1.0.0/sendpost_python_sdk/__init__.py
--rw-r--r--   0 arseniy    (501) staff       (20)    58859 2023-07-26 12:39:50.000000 sendpost_python_sdk-1.0.0/sendpost_python_sdk/api_client.py
-drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 13:31:19.000000 sendpost_python_sdk-1.0.0/sendpost_python_sdk/apis/
--rw-r--r--   0 arseniy    (501) staff       (20)      214 2023-07-26 12:34:02.000000 sendpost_python_sdk-1.0.0/sendpost_python_sdk/apis/__init__.py
--rw-r--r--   0 arseniy    (501) staff       (20)      610 2023-07-26 12:34:01.000000 sendpost_python_sdk-1.0.0/sendpost_python_sdk/apis/path_to_api.py
-drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 13:31:19.000000 sendpost_python_sdk-1.0.0/sendpost_python_sdk/apis/paths/
--rw-r--r--   0 arseniy    (501) staff       (20)      246 2023-07-26 12:34:01.000000 sendpost_python_sdk-1.0.0/sendpost_python_sdk/apis/paths/__init__.py
--rw-r--r--   0 arseniy    (501) staff       (20)      125 2023-07-26 12:34:01.000000 sendpost_python_sdk-1.0.0/sendpost_python_sdk/apis/paths/subaccount_email_.py
--rw-r--r--   0 arseniy    (501) staff       (20)      141 2023-07-26 12:34:01.000000 sendpost_python_sdk-1.0.0/sendpost_python_sdk/apis/paths/subaccount_email_template.py
--rw-r--r--   0 arseniy    (501) staff       (20)      318 2023-07-26 12:34:01.000000 sendpost_python_sdk-1.0.0/sendpost_python_sdk/apis/tag_to_api.py
-drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 13:31:19.000000 sendpost_python_sdk-1.0.0/sendpost_python_sdk/apis/tags/
--rw-r--r--   0 arseniy    (501) staff       (20)      312 2023-07-26 12:34:01.000000 sendpost_python_sdk-1.0.0/sendpost_python_sdk/apis/tags/__init__.py
--rw-r--r--   0 arseniy    (501) staff       (20)      800 2023-07-26 12:34:01.000000 sendpost_python_sdk-1.0.0/sendpost_python_sdk/apis/tags/email_api.py
--rw-r--r--   0 arseniy    (501) staff       (20)    15568 2023-07-26 12:34:01.000000 sendpost_python_sdk-1.0.0/sendpost_python_sdk/configuration.py
--rw-r--r--   0 arseniy    (501) staff       (20)     4702 2023-07-26 12:34:01.000000 sendpost_python_sdk-1.0.0/sendpost_python_sdk/exceptions.py
-drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 13:31:19.000000 sendpost_python_sdk-1.0.0/sendpost_python_sdk/model/
--rw-r--r--   0 arseniy    (501) staff       (20)      353 2023-07-26 12:34:02.000000 sendpost_python_sdk-1.0.0/sendpost_python_sdk/model/__init__.py
--rw-r--r--   0 arseniy    (501) staff       (20)     3139 2023-07-26 12:33:55.000000 sendpost_python_sdk-1.0.0/sendpost_python_sdk/model/attachment.py
--rw-r--r--   0 arseniy    (501) staff       (20)     4856 2023-07-26 12:33:56.000000 sendpost_python_sdk-1.0.0/sendpost_python_sdk/model/city.py
--rw-r--r--   0 arseniy    (501) staff       (20)     3661 2023-07-26 12:33:56.000000 sendpost_python_sdk-1.0.0/sendpost_python_sdk/model/copy_to.py
--rw-r--r--   0 arseniy    (501) staff       (20)     2587 2023-07-26 12:33:57.000000 sendpost_python_sdk-1.0.0/sendpost_python_sdk/model/device.py
--rw-r--r--   0 arseniy    (501) staff       (20)    12636 2023-07-26 12:33:57.000000 sendpost_python_sdk-1.0.0/sendpost_python_sdk/model/email_message.py
--rw-r--r--   0 arseniy    (501) staff       (20)     4761 2023-07-26 12:33:58.000000 sendpost_python_sdk-1.0.0/sendpost_python_sdk/model/email_response.py
--rw-r--r--   0 arseniy    (501) staff       (20)     6066 2023-07-26 12:33:58.000000 sendpost_python_sdk-1.0.0/sendpost_python_sdk/model/event_metadata.py
--rw-r--r--   0 arseniy    (501) staff       (20)     3059 2023-07-26 12:33:58.000000 sendpost_python_sdk-1.0.0/sendpost_python_sdk/model/model_from.py
--rw-r--r--   0 arseniy    (501) staff       (20)     4612 2023-07-26 12:33:58.000000 sendpost_python_sdk-1.0.0/sendpost_python_sdk/model/os.py
--rw-r--r--   0 arseniy    (501) staff       (20)    20181 2023-07-26 12:33:59.000000 sendpost_python_sdk-1.0.0/sendpost_python_sdk/model/q_email_message.py
--rw-r--r--   0 arseniy    (501) staff       (20)     9817 2023-07-26 12:33:59.000000 sendpost_python_sdk-1.0.0/sendpost_python_sdk/model/q_event.py
--rw-r--r--   0 arseniy    (501) staff       (20)     3055 2023-07-26 12:34:00.000000 sendpost_python_sdk-1.0.0/sendpost_python_sdk/model/reply_to.py
--rw-r--r--   0 arseniy    (501) staff       (20)     6319 2023-07-26 12:34:00.000000 sendpost_python_sdk-1.0.0/sendpost_python_sdk/model/to.py
--rw-r--r--   0 arseniy    (501) staff       (20)     4069 2023-07-26 12:34:00.000000 sendpost_python_sdk-1.0.0/sendpost_python_sdk/model/user_agent.py
--rw-r--r--   0 arseniy    (501) staff       (20)     3347 2023-07-26 12:34:00.000000 sendpost_python_sdk-1.0.0/sendpost_python_sdk/model/webhook_event.py
-drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 13:31:19.000000 sendpost_python_sdk-1.0.0/sendpost_python_sdk/models/
--rw-r--r--   0 arseniy    (501) staff       (20)     1252 2023-07-26 12:34:02.000000 sendpost_python_sdk-1.0.0/sendpost_python_sdk/models/__init__.py
-drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 13:31:19.000000 sendpost_python_sdk-1.0.0/sendpost_python_sdk/paths/
--rw-r--r--   0 arseniy    (501) staff       (20)      401 2023-07-26 12:34:01.000000 sendpost_python_sdk-1.0.0/sendpost_python_sdk/paths/__init__.py
-drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 13:31:19.000000 sendpost_python_sdk-1.0.0/sendpost_python_sdk/paths/subaccount_email_/
--rw-r--r--   0 arseniy    (501) staff       (20)      331 2023-07-26 12:34:01.000000 sendpost_python_sdk-1.0.0/sendpost_python_sdk/paths/subaccount_email_/__init__.py
--rw-r--r--   0 arseniy    (501) staff       (20)    15448 2023-07-26 12:34:01.000000 sendpost_python_sdk-1.0.0/sendpost_python_sdk/paths/subaccount_email_/post.py
-drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 13:31:19.000000 sendpost_python_sdk-1.0.0/sendpost_python_sdk/paths/subaccount_email_template/
--rw-r--r--   0 arseniy    (501) staff       (20)      347 2023-07-26 12:34:01.000000 sendpost_python_sdk-1.0.0/sendpost_python_sdk/paths/subaccount_email_template/__init__.py
--rw-r--r--   0 arseniy    (501) staff       (20)    15628 2023-07-26 12:34:01.000000 sendpost_python_sdk-1.0.0/sendpost_python_sdk/paths/subaccount_email_template/post.py
--rw-r--r--   0 arseniy    (501) staff       (20)    10860 2023-07-26 12:34:01.000000 sendpost_python_sdk-1.0.0/sendpost_python_sdk/rest.py
--rw-r--r--   0 arseniy    (501) staff       (20)    97848 2023-07-26 12:34:01.000000 sendpost_python_sdk-1.0.0/sendpost_python_sdk/schemas.py
-drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 13:31:19.000000 sendpost_python_sdk-1.0.0/sendpost_python_sdk.egg-info/
--rw-r--r--   0 arseniy    (501) staff       (20)      663 2023-07-26 13:31:19.000000 sendpost_python_sdk-1.0.0/sendpost_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 arseniy    (501) staff       (20)     2530 2023-07-26 13:31:19.000000 sendpost_python_sdk-1.0.0/sendpost_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 arseniy    (501) staff       (20)        1 2023-07-26 13:31:19.000000 sendpost_python_sdk-1.0.0/sendpost_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 arseniy    (501) staff       (20)      118 2023-07-26 13:31:19.000000 sendpost_python_sdk-1.0.0/sendpost_python_sdk.egg-info/requires.txt
--rw-r--r--   0 arseniy    (501) staff       (20)       25 2023-07-26 13:31:19.000000 sendpost_python_sdk-1.0.0/sendpost_python_sdk.egg-info/top_level.txt
--rw-r--r--   0 arseniy    (501) staff       (20)      110 2023-07-26 13:31:19.000000 sendpost_python_sdk-1.0.0/setup.cfg
--rw-r--r--   0 arseniy    (501) staff       (20)     1642 2023-07-26 13:31:08.000000 sendpost_python_sdk-1.0.0/setup.py
-drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 13:31:19.000000 sendpost_python_sdk-1.0.0/test/
-drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 13:31:19.000000 sendpost_python_sdk-1.0.0/test/test_models/
--rw-r--r--   0 arseniy    (501) staff       (20)        0 2023-07-26 12:34:01.000000 sendpost_python_sdk-1.0.0/test/test_models/__init__.py
--rw-r--r--   0 arseniy    (501) staff       (20)      748 2023-07-26 12:33:55.000000 sendpost_python_sdk-1.0.0/test/test_models/test_attachment.py
--rw-r--r--   0 arseniy    (501) staff       (20)      724 2023-07-26 12:33:56.000000 sendpost_python_sdk-1.0.0/test/test_models/test_city.py
--rw-r--r--   0 arseniy    (501) staff       (20)      733 2023-07-26 12:33:56.000000 sendpost_python_sdk-1.0.0/test/test_models/test_copy_to.py
--rw-r--r--   0 arseniy    (501) staff       (20)      732 2023-07-26 12:33:57.000000 sendpost_python_sdk-1.0.0/test/test_models/test_device.py
--rw-r--r--   0 arseniy    (501) staff       (20)      757 2023-07-26 12:33:57.000000 sendpost_python_sdk-1.0.0/test/test_models/test_email_message.py
--rw-r--r--   0 arseniy    (501) staff       (20)      761 2023-07-26 12:33:58.000000 sendpost_python_sdk-1.0.0/test/test_models/test_email_response.py
--rw-r--r--   0 arseniy    (501) staff       (20)      761 2023-07-26 12:33:58.000000 sendpost_python_sdk-1.0.0/test/test_models/test_event_metadata.py
--rw-r--r--   0 arseniy    (501) staff       (20)      745 2023-07-26 12:33:58.000000 sendpost_python_sdk-1.0.0/test/test_models/test_model_from.py
--rw-r--r--   0 arseniy    (501) staff       (20)      716 2023-07-26 12:33:58.000000 sendpost_python_sdk-1.0.0/test/test_models/test_os.py
--rw-r--r--   0 arseniy    (501) staff       (20)      762 2023-07-26 12:33:59.000000 sendpost_python_sdk-1.0.0/test/test_models/test_q_email_message.py
--rw-r--r--   0 arseniy    (501) staff       (20)      733 2023-07-26 12:34:00.000000 sendpost_python_sdk-1.0.0/test/test_models/test_q_event.py
--rw-r--r--   0 arseniy    (501) staff       (20)      737 2023-07-26 12:34:00.000000 sendpost_python_sdk-1.0.0/test/test_models/test_reply_to.py
--rw-r--r--   0 arseniy    (501) staff       (20)      716 2023-07-26 12:34:00.000000 sendpost_python_sdk-1.0.0/test/test_models/test_to.py
--rw-r--r--   0 arseniy    (501) staff       (20)      745 2023-07-26 12:34:00.000000 sendpost_python_sdk-1.0.0/test/test_models/test_user_agent.py
--rw-r--r--   0 arseniy    (501) staff       (20)      757 2023-07-26 12:34:00.000000 sendpost_python_sdk-1.0.0/test/test_models/test_webhook_event.py
-drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 13:31:19.000000 sendpost_python_sdk-1.0.0/test/test_paths/
--rw-r--r--   0 arseniy    (501) staff       (20)     1995 2023-07-26 12:34:01.000000 sendpost_python_sdk-1.0.0/test/test_paths/__init__.py
-drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 13:31:19.000000 sendpost_python_sdk-1.0.0/test/test_paths/test_subaccount_email_/
--rw-r--r--   0 arseniy    (501) staff       (20)        0 2023-07-26 12:34:01.000000 sendpost_python_sdk-1.0.0/test/test_paths/test_subaccount_email_/__init__.py
--rw-r--r--   0 arseniy    (501) staff       (20)      802 2023-07-26 12:34:01.000000 sendpost_python_sdk-1.0.0/test/test_paths/test_subaccount_email_/test_post.py
-drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 13:31:19.000000 sendpost_python_sdk-1.0.0/test/test_paths/test_subaccount_email_template/
--rw-r--r--   0 arseniy    (501) staff       (20)        0 2023-07-26 12:34:01.000000 sendpost_python_sdk-1.0.0/test/test_paths/test_subaccount_email_template/__init__.py
--rw-r--r--   0 arseniy    (501) staff       (20)      826 2023-07-26 12:34:01.000000 sendpost_python_sdk-1.0.0/test/test_paths/test_subaccount_email_template/test_post.py
+drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-08-04 13:11:42.000000 sendpost_python_sdk-1.1.1/
+-rw-r--r--   0 arseniy    (501) staff       (20)      663 2023-08-04 13:11:42.000000 sendpost_python_sdk-1.1.1/PKG-INFO
+-rw-r--r--   0 arseniy    (501) staff       (20)     5131 2023-08-04 13:10:27.000000 sendpost_python_sdk-1.1.1/README.md
+drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-08-04 13:11:42.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk/
+-rw-r--r--   0 arseniy    (501) staff       (20)      979 2023-08-04 13:09:41.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk/__init__.py
+-rw-r--r--   0 arseniy    (501) staff       (20)    58859 2023-08-04 13:11:24.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk/api_client.py
+drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-08-04 13:11:42.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk/apis/
+-rw-r--r--   0 arseniy    (501) staff       (20)      214 2023-08-04 13:09:41.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk/apis/__init__.py
+-rw-r--r--   0 arseniy    (501) staff       (20)     1086 2023-08-04 13:09:40.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk/apis/path_to_api.py
+drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-08-04 13:11:42.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk/apis/paths/
+-rw-r--r--   0 arseniy    (501) staff       (20)      246 2023-08-04 13:09:40.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk/apis/paths/__init__.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      125 2023-08-04 13:09:39.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk/apis/paths/subaccount_email_.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      141 2023-08-04 13:09:39.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk/apis/paths/subaccount_email_template.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      328 2023-08-04 13:09:40.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk/apis/paths/subaccount_suppression_.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      144 2023-08-04 13:09:40.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk/apis/paths/subaccount_suppression_count.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      485 2023-08-04 13:09:40.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk/apis/tag_to_api.py
+drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-08-04 13:11:42.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk/apis/tags/
+-rw-r--r--   0 arseniy    (501) staff       (20)      344 2023-08-04 13:09:40.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk/apis/tags/__init__.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      800 2023-08-04 13:09:39.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk/apis/tags/email_api.py
+-rw-r--r--   0 arseniy    (501) staff       (20)     1013 2023-08-04 13:09:40.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk/apis/tags/suppression_api.py
+-rw-r--r--   0 arseniy    (501) staff       (20)    15568 2023-08-04 13:09:41.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk/configuration.py
+-rw-r--r--   0 arseniy    (501) staff       (20)     4702 2023-08-04 13:09:41.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk/exceptions.py
+drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-08-04 13:11:42.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk/model/
+-rw-r--r--   0 arseniy    (501) staff       (20)      353 2023-08-04 13:09:41.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk/model/__init__.py
+-rw-r--r--   0 arseniy    (501) staff       (20)     3139 2023-08-04 13:09:33.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk/model/attachment.py
+-rw-r--r--   0 arseniy    (501) staff       (20)     4856 2023-08-04 13:09:34.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk/model/city.py
+-rw-r--r--   0 arseniy    (501) staff       (20)     3661 2023-08-04 13:09:34.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk/model/copy_to.py
+-rw-r--r--   0 arseniy    (501) staff       (20)     2599 2023-08-04 13:09:34.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk/model/count_stat.py
+-rw-r--r--   0 arseniy    (501) staff       (20)     3088 2023-08-04 13:09:34.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk/model/delete_response.py
+-rw-r--r--   0 arseniy    (501) staff       (20)     2587 2023-08-04 13:09:35.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk/model/device.py
+-rw-r--r--   0 arseniy    (501) staff       (20)    12636 2023-08-04 13:09:35.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk/model/email_message.py
+-rw-r--r--   0 arseniy    (501) staff       (20)     4761 2023-08-04 13:09:36.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk/model/email_response.py
+-rw-r--r--   0 arseniy    (501) staff       (20)     6066 2023-08-04 13:09:36.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk/model/event_metadata.py
+-rw-r--r--   0 arseniy    (501) staff       (20)     3059 2023-08-04 13:09:36.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk/model/model_from.py
+-rw-r--r--   0 arseniy    (501) staff       (20)     4612 2023-08-04 13:09:36.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk/model/os.py
+-rw-r--r--   0 arseniy    (501) staff       (20)    20181 2023-08-04 13:09:37.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk/model/q_email_message.py
+-rw-r--r--   0 arseniy    (501) staff       (20)     9817 2023-08-04 13:09:37.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk/model/q_event.py
+-rw-r--r--   0 arseniy    (501) staff       (20)     8012 2023-08-04 13:09:38.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk/model/r_suppression.py
+-rw-r--r--   0 arseniy    (501) staff       (20)     3659 2023-08-04 13:09:38.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk/model/rd_suppression.py
+-rw-r--r--   0 arseniy    (501) staff       (20)     3055 2023-08-04 13:09:38.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk/model/reply_to.py
+-rw-r--r--   0 arseniy    (501) staff       (20)     4674 2023-08-04 13:09:38.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk/model/suppression.py
+-rw-r--r--   0 arseniy    (501) staff       (20)     2594 2023-08-04 13:09:38.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk/model/suppression_email.py
+-rw-r--r--   0 arseniy    (501) staff       (20)     6319 2023-08-04 13:09:38.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk/model/to.py
+-rw-r--r--   0 arseniy    (501) staff       (20)     4069 2023-08-04 13:09:39.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk/model/user_agent.py
+-rw-r--r--   0 arseniy    (501) staff       (20)     3347 2023-08-04 13:09:39.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk/model/webhook_event.py
+drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-08-04 13:11:42.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk/models/
+-rw-r--r--   0 arseniy    (501) staff       (20)     1647 2023-08-04 13:09:41.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk/models/__init__.py
+drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-08-04 13:11:42.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk/paths/
+-rw-r--r--   0 arseniy    (501) staff       (20)      525 2023-08-04 13:09:40.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk/paths/__init__.py
+drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-08-04 13:11:42.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk/paths/subaccount_email_/
+-rw-r--r--   0 arseniy    (501) staff       (20)      331 2023-08-04 13:09:39.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk/paths/subaccount_email_/__init__.py
+-rw-r--r--   0 arseniy    (501) staff       (20)    15448 2023-08-04 13:09:39.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk/paths/subaccount_email_/post.py
+drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-08-04 13:11:42.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk/paths/subaccount_email_template/
+-rw-r--r--   0 arseniy    (501) staff       (20)      347 2023-08-04 13:09:39.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk/paths/subaccount_email_template/__init__.py
+-rw-r--r--   0 arseniy    (501) staff       (20)    15628 2023-08-04 13:09:39.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk/paths/subaccount_email_template/post.py
+drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-08-04 13:11:42.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk/paths/subaccount_suppression_/
+-rw-r--r--   0 arseniy    (501) staff       (20)      343 2023-08-04 13:09:40.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk/paths/subaccount_suppression_/__init__.py
+-rw-r--r--   0 arseniy    (501) staff       (20)    15876 2023-08-04 13:09:40.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk/paths/subaccount_suppression_/delete.py
+-rw-r--r--   0 arseniy    (501) staff       (20)    14134 2023-08-04 13:09:40.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk/paths/subaccount_suppression_/get.py
+-rw-r--r--   0 arseniy    (501) staff       (20)    15848 2023-08-04 13:09:40.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk/paths/subaccount_suppression_/post.py
+drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-08-04 13:11:42.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk/paths/subaccount_suppression_count/
+-rw-r--r--   0 arseniy    (501) staff       (20)      353 2023-08-04 13:09:40.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk/paths/subaccount_suppression_count/__init__.py
+-rw-r--r--   0 arseniy    (501) staff       (20)    12544 2023-08-04 13:09:40.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk/paths/subaccount_suppression_count/get.py
+-rw-r--r--   0 arseniy    (501) staff       (20)    10860 2023-08-04 13:09:41.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk/rest.py
+-rw-r--r--   0 arseniy    (501) staff       (20)    97848 2023-08-04 13:09:41.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk/schemas.py
+drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-08-04 13:11:42.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk.egg-info/
+-rw-r--r--   0 arseniy    (501) staff       (20)      663 2023-08-04 13:11:41.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 arseniy    (501) staff       (20)     3918 2023-08-04 13:11:41.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 arseniy    (501) staff       (20)        1 2023-08-04 13:11:41.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 arseniy    (501) staff       (20)      118 2023-08-04 13:11:41.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 arseniy    (501) staff       (20)       25 2023-08-04 13:11:41.000000 sendpost_python_sdk-1.1.1/sendpost_python_sdk.egg-info/top_level.txt
+-rw-r--r--   0 arseniy    (501) staff       (20)      110 2023-08-04 13:11:42.000000 sendpost_python_sdk-1.1.1/setup.cfg
+-rw-r--r--   0 arseniy    (501) staff       (20)     1642 2023-08-04 13:10:49.000000 sendpost_python_sdk-1.1.1/setup.py
+drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-08-04 13:11:42.000000 sendpost_python_sdk-1.1.1/test/
+drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-08-04 13:11:42.000000 sendpost_python_sdk-1.1.1/test/test_models/
+-rw-r--r--   0 arseniy    (501) staff       (20)        0 2023-08-04 13:09:41.000000 sendpost_python_sdk-1.1.1/test/test_models/__init__.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      748 2023-07-26 12:33:55.000000 sendpost_python_sdk-1.1.1/test/test_models/test_attachment.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      724 2023-07-26 12:33:56.000000 sendpost_python_sdk-1.1.1/test/test_models/test_city.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      733 2023-07-26 12:33:56.000000 sendpost_python_sdk-1.1.1/test/test_models/test_copy_to.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      745 2023-08-04 09:45:37.000000 sendpost_python_sdk-1.1.1/test/test_models/test_count_stat.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      765 2023-08-04 09:45:38.000000 sendpost_python_sdk-1.1.1/test/test_models/test_delete_response.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      732 2023-07-26 12:33:57.000000 sendpost_python_sdk-1.1.1/test/test_models/test_device.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      757 2023-07-26 12:33:57.000000 sendpost_python_sdk-1.1.1/test/test_models/test_email_message.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      761 2023-07-26 12:33:58.000000 sendpost_python_sdk-1.1.1/test/test_models/test_email_response.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      761 2023-07-26 12:33:58.000000 sendpost_python_sdk-1.1.1/test/test_models/test_event_metadata.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      745 2023-07-26 12:33:58.000000 sendpost_python_sdk-1.1.1/test/test_models/test_model_from.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      716 2023-07-26 12:33:58.000000 sendpost_python_sdk-1.1.1/test/test_models/test_os.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      762 2023-07-26 12:33:59.000000 sendpost_python_sdk-1.1.1/test/test_models/test_q_email_message.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      733 2023-07-26 12:34:00.000000 sendpost_python_sdk-1.1.1/test/test_models/test_q_event.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      757 2023-08-04 09:45:42.000000 sendpost_python_sdk-1.1.1/test/test_models/test_r_suppression.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      761 2023-08-04 09:45:41.000000 sendpost_python_sdk-1.1.1/test/test_models/test_rd_suppression.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      737 2023-07-26 12:34:00.000000 sendpost_python_sdk-1.1.1/test/test_models/test_reply_to.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      752 2023-08-04 09:45:42.000000 sendpost_python_sdk-1.1.1/test/test_models/test_suppression.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      773 2023-08-04 09:45:42.000000 sendpost_python_sdk-1.1.1/test/test_models/test_suppression_email.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      716 2023-07-26 12:34:00.000000 sendpost_python_sdk-1.1.1/test/test_models/test_to.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      745 2023-07-26 12:34:00.000000 sendpost_python_sdk-1.1.1/test/test_models/test_user_agent.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      757 2023-07-26 12:34:00.000000 sendpost_python_sdk-1.1.1/test/test_models/test_webhook_event.py
+drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-08-04 13:11:42.000000 sendpost_python_sdk-1.1.1/test/test_paths/
+-rw-r--r--   0 arseniy    (501) staff       (20)     1995 2023-08-04 13:09:40.000000 sendpost_python_sdk-1.1.1/test/test_paths/__init__.py
+drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-08-04 13:11:42.000000 sendpost_python_sdk-1.1.1/test/test_paths/test_subaccount_email_/
+-rw-r--r--   0 arseniy    (501) staff       (20)        0 2023-08-04 13:09:39.000000 sendpost_python_sdk-1.1.1/test/test_paths/test_subaccount_email_/__init__.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      802 2023-08-04 13:09:39.000000 sendpost_python_sdk-1.1.1/test/test_paths/test_subaccount_email_/test_post.py
+drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-08-04 13:11:42.000000 sendpost_python_sdk-1.1.1/test/test_paths/test_subaccount_email_template/
+-rw-r--r--   0 arseniy    (501) staff       (20)        0 2023-08-04 13:09:39.000000 sendpost_python_sdk-1.1.1/test/test_paths/test_subaccount_email_template/__init__.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      826 2023-08-04 13:09:39.000000 sendpost_python_sdk-1.1.1/test/test_paths/test_subaccount_email_template/test_post.py
+drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-08-04 13:11:42.000000 sendpost_python_sdk-1.1.1/test/test_paths/test_subaccount_suppression_/
+-rw-r--r--   0 arseniy    (501) staff       (20)        0 2023-08-04 13:09:40.000000 sendpost_python_sdk-1.1.1/test/test_paths/test_subaccount_suppression_/__init__.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      826 2023-08-04 13:09:40.000000 sendpost_python_sdk-1.1.1/test/test_paths/test_subaccount_suppression_/test_delete.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      817 2023-08-04 13:09:40.000000 sendpost_python_sdk-1.1.1/test/test_paths/test_subaccount_suppression_/test_get.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      820 2023-08-04 13:09:40.000000 sendpost_python_sdk-1.1.1/test/test_paths/test_subaccount_suppression_/test_post.py
+drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-08-04 13:11:42.000000 sendpost_python_sdk-1.1.1/test/test_paths/test_subaccount_suppression_count/
+-rw-r--r--   0 arseniy    (501) staff       (20)        0 2023-08-04 13:09:40.000000 sendpost_python_sdk-1.1.1/test/test_paths/test_subaccount_suppression_count/__init__.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      832 2023-08-04 13:09:40.000000 sendpost_python_sdk-1.1.1/test/test_paths/test_subaccount_suppression_count/test_get.py
```

### Comparing `sendpost_python_sdk-1.0.0/PKG-INFO` & `sendpost_python_sdk-1.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 1.2
 Name: sendpost_python_sdk
-Version: 1.0.0
+Version: 1.1.1
 Summary: SendPost API
 Home-page: https://github.com/sendpost/sendpost_python_sdk
 Author: Sendpost
 Author-email: dev@sendpost.io
 License: UNKNOWN
-Download-URL: https://github.com/sendpost/sendpost_python_sdk/archive/refs/tags/1.0.0.tar.gz
+Download-URL: https://github.com/sendpost/sendpost_python_sdk/archive/refs/tags/1.1.1.tar.gz
 Description:     Email API and SMTP relay to not just send and measure email sending, but also alert and optimise. We provide you with tools, expertise and support needed to reliably deliver emails to your customers inboxes on time, every time.  # noqa: E501
             
 Keywords: OpenAPI,OpenAPI-Generator,SendPost API
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `sendpost_python_sdk-1.0.0/sendpost_python_sdk/__init__.py` & `sendpost_python_sdk-1.1.1/sendpost_python_sdk/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     Email API and SMTP relay to not just send and measure email sending, but also alert and optimise. We provide you with tools, expertise and support needed to reliably deliver emails to your customers inboxes on time, every time.  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Contact: hello@sendpost.io
     Generated by: https://openapi-generator.tech
 """
 
-__version__ = "1.0.0"
+__version__ = "1.1.1"
 
 # import ApiClient
 from sendpost_python_sdk.api_client import ApiClient
 
 # import Configuration
 from sendpost_python_sdk.configuration import Configuration
```

### Comparing `sendpost_python_sdk-1.0.0/sendpost_python_sdk/api_client.py` & `sendpost_python_sdk-1.1.1/sendpost_python_sdk/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1002,15 +1002,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = HTTPHeaderDict()
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.0.0/python'
+        self.user_agent = 'OpenAPI-Generator/1.1.1/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `sendpost_python_sdk-1.0.0/sendpost_python_sdk/apis/tags/email_api.py` & `sendpost_python_sdk-1.1.1/sendpost_python_sdk/apis/tags/email_api.py`

 * *Files identical despite different names*

### Comparing `sendpost_python_sdk-1.0.0/sendpost_python_sdk/configuration.py` & `sendpost_python_sdk-1.1.1/sendpost_python_sdk/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -357,15 +357,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 1.0.0\n"\
-               "SDK Package Version: 1.0.0".\
+               "SDK Package Version: 1.1.1".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `sendpost_python_sdk-1.0.0/sendpost_python_sdk/exceptions.py` & `sendpost_python_sdk-1.1.1/sendpost_python_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `sendpost_python_sdk-1.0.0/sendpost_python_sdk/model/attachment.py` & `sendpost_python_sdk-1.1.1/sendpost_python_sdk/model/attachment.py`

 * *Files identical despite different names*

### Comparing `sendpost_python_sdk-1.0.0/sendpost_python_sdk/model/city.py` & `sendpost_python_sdk-1.1.1/sendpost_python_sdk/model/city.py`

 * *Files identical despite different names*

### Comparing `sendpost_python_sdk-1.0.0/sendpost_python_sdk/model/copy_to.py` & `sendpost_python_sdk-1.1.1/sendpost_python_sdk/model/copy_to.py`

 * *Files identical despite different names*

### Comparing `sendpost_python_sdk-1.0.0/sendpost_python_sdk/model/device.py` & `sendpost_python_sdk-1.1.1/sendpost_python_sdk/model/device.py`

 * *Files identical despite different names*

### Comparing `sendpost_python_sdk-1.0.0/sendpost_python_sdk/model/email_message.py` & `sendpost_python_sdk-1.1.1/sendpost_python_sdk/model/email_message.py`

 * *Files identical despite different names*

### Comparing `sendpost_python_sdk-1.0.0/sendpost_python_sdk/model/email_response.py` & `sendpost_python_sdk-1.1.1/sendpost_python_sdk/model/email_response.py`

 * *Files identical despite different names*

### Comparing `sendpost_python_sdk-1.0.0/sendpost_python_sdk/model/event_metadata.py` & `sendpost_python_sdk-1.1.1/sendpost_python_sdk/model/event_metadata.py`

 * *Files identical despite different names*

### Comparing `sendpost_python_sdk-1.0.0/sendpost_python_sdk/model/model_from.py` & `sendpost_python_sdk-1.1.1/sendpost_python_sdk/model/model_from.py`

 * *Files identical despite different names*

### Comparing `sendpost_python_sdk-1.0.0/sendpost_python_sdk/model/os.py` & `sendpost_python_sdk-1.1.1/sendpost_python_sdk/model/os.py`

 * *Files identical despite different names*

### Comparing `sendpost_python_sdk-1.0.0/sendpost_python_sdk/model/q_email_message.py` & `sendpost_python_sdk-1.1.1/sendpost_python_sdk/model/q_email_message.py`

 * *Files identical despite different names*

### Comparing `sendpost_python_sdk-1.0.0/sendpost_python_sdk/model/q_event.py` & `sendpost_python_sdk-1.1.1/sendpost_python_sdk/model/q_event.py`

 * *Files identical despite different names*

### Comparing `sendpost_python_sdk-1.0.0/sendpost_python_sdk/model/reply_to.py` & `sendpost_python_sdk-1.1.1/sendpost_python_sdk/model/reply_to.py`

 * *Files identical despite different names*

### Comparing `sendpost_python_sdk-1.0.0/sendpost_python_sdk/model/to.py` & `sendpost_python_sdk-1.1.1/sendpost_python_sdk/model/to.py`

 * *Files identical despite different names*

### Comparing `sendpost_python_sdk-1.0.0/sendpost_python_sdk/model/user_agent.py` & `sendpost_python_sdk-1.1.1/sendpost_python_sdk/model/user_agent.py`

 * *Files identical despite different names*

### Comparing `sendpost_python_sdk-1.0.0/sendpost_python_sdk/model/webhook_event.py` & `sendpost_python_sdk-1.1.1/sendpost_python_sdk/model/webhook_event.py`

 * *Files identical despite different names*

### Comparing `sendpost_python_sdk-1.0.0/sendpost_python_sdk/models/__init__.py` & `sendpost_python_sdk-1.1.1/sendpost_python_sdk/models/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,19 +10,25 @@
 # or import this package, but before doing it, use:
 # import sys
 # sys.setrecursionlimit(n)
 
 from sendpost_python_sdk.model.attachment import Attachment
 from sendpost_python_sdk.model.city import City
 from sendpost_python_sdk.model.copy_to import CopyTo
+from sendpost_python_sdk.model.count_stat import CountStat
+from sendpost_python_sdk.model.delete_response import DeleteResponse
 from sendpost_python_sdk.model.device import Device
 from sendpost_python_sdk.model.email_message import EmailMessage
 from sendpost_python_sdk.model.email_response import EmailResponse
 from sendpost_python_sdk.model.event_metadata import EventMetadata
 from sendpost_python_sdk.model.model_from import ModelFrom
 from sendpost_python_sdk.model.os import Os
 from sendpost_python_sdk.model.q_email_message import QEmailMessage
 from sendpost_python_sdk.model.q_event import QEvent
+from sendpost_python_sdk.model.rd_suppression import RDSuppression
+from sendpost_python_sdk.model.r_suppression import RSuppression
 from sendpost_python_sdk.model.reply_to import ReplyTo
+from sendpost_python_sdk.model.suppression import Suppression
+from sendpost_python_sdk.model.suppression_email import SuppressionEmail
 from sendpost_python_sdk.model.to import To
 from sendpost_python_sdk.model.user_agent import UserAgent
 from sendpost_python_sdk.model.webhook_event import WebhookEvent
```

### Comparing `sendpost_python_sdk-1.0.0/sendpost_python_sdk/paths/subaccount_email_/post.py` & `sendpost_python_sdk-1.1.1/sendpost_python_sdk/paths/subaccount_email_/post.py`

 * *Files identical despite different names*

### Comparing `sendpost_python_sdk-1.0.0/sendpost_python_sdk/paths/subaccount_email_template/post.py` & `sendpost_python_sdk-1.1.1/sendpost_python_sdk/paths/subaccount_email_template/post.py`

 * *Files identical despite different names*

### Comparing `sendpost_python_sdk-1.0.0/sendpost_python_sdk/rest.py` & `sendpost_python_sdk-1.1.1/sendpost_python_sdk/rest.py`

 * *Files identical despite different names*

### Comparing `sendpost_python_sdk-1.0.0/sendpost_python_sdk/schemas.py` & `sendpost_python_sdk-1.1.1/sendpost_python_sdk/schemas.py`

 * *Files identical despite different names*

### Comparing `sendpost_python_sdk-1.0.0/sendpost_python_sdk.egg-info/PKG-INFO` & `sendpost_python_sdk-1.1.1/sendpost_python_sdk.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 1.2
 Name: sendpost-python-sdk
-Version: 1.0.0
+Version: 1.1.1
 Summary: SendPost API
 Home-page: https://github.com/sendpost/sendpost_python_sdk
 Author: Sendpost
 Author-email: dev@sendpost.io
 License: UNKNOWN
-Download-URL: https://github.com/sendpost/sendpost_python_sdk/archive/refs/tags/1.0.0.tar.gz
+Download-URL: https://github.com/sendpost/sendpost_python_sdk/archive/refs/tags/1.1.1.tar.gz
 Description:     Email API and SMTP relay to not just send and measure email sending, but also alert and optimise. We provide you with tools, expertise and support needed to reliably deliver emails to your customers inboxes on time, every time.  # noqa: E501
             
 Keywords: OpenAPI,OpenAPI-Generator,SendPost API
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `sendpost_python_sdk-1.0.0/setup.py` & `sendpost_python_sdk-1.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Contact: hello@sendpost.io
     Generated by: https://openapi-generator.tech
 """
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "sendpost_python_sdk"
-VERSION = "1.0.0"
+VERSION = "1.1.1"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 
@@ -31,15 +31,15 @@
 ]
 
 setup(
     name=NAME,
     version=VERSION,
     description="SendPost API",
     url = 'https://github.com/sendpost/sendpost_python_sdk',
-    download_url = 'https://github.com/sendpost/sendpost_python_sdk/archive/refs/tags/1.0.0.tar.gz',
+    download_url = 'https://github.com/sendpost/sendpost_python_sdk/archive/refs/tags/1.1.1.tar.gz',
     author="Sendpost",
     author_email="dev@sendpost.io",
     keywords=["OpenAPI", "OpenAPI-Generator", "SendPost API"],
     python_requires=">=3.7",
     install_requires=REQUIRES,
     packages=find_packages(exclude=["test", "tests"]),
     include_package_data=True,
```

### Comparing `sendpost_python_sdk-1.0.0/test/test_models/test_attachment.py` & `sendpost_python_sdk-1.1.1/test/test_models/test_attachment.py`

 * *Files identical despite different names*

### Comparing `sendpost_python_sdk-1.0.0/test/test_models/test_city.py` & `sendpost_python_sdk-1.1.1/test/test_models/test_city.py`

 * *Files identical despite different names*

### Comparing `sendpost_python_sdk-1.0.0/test/test_models/test_copy_to.py` & `sendpost_python_sdk-1.1.1/test/test_models/test_copy_to.py`

 * *Files identical despite different names*

### Comparing `sendpost_python_sdk-1.0.0/test/test_models/test_device.py` & `sendpost_python_sdk-1.1.1/test/test_models/test_device.py`

 * *Files identical despite different names*

### Comparing `sendpost_python_sdk-1.0.0/test/test_models/test_email_message.py` & `sendpost_python_sdk-1.1.1/test/test_models/test_email_message.py`

 * *Files identical despite different names*

### Comparing `sendpost_python_sdk-1.0.0/test/test_models/test_email_response.py` & `sendpost_python_sdk-1.1.1/test/test_models/test_email_response.py`

 * *Files identical despite different names*

### Comparing `sendpost_python_sdk-1.0.0/test/test_models/test_event_metadata.py` & `sendpost_python_sdk-1.1.1/test/test_models/test_event_metadata.py`

 * *Files identical despite different names*

### Comparing `sendpost_python_sdk-1.0.0/test/test_models/test_model_from.py` & `sendpost_python_sdk-1.1.1/test/test_models/test_model_from.py`

 * *Files identical despite different names*

### Comparing `sendpost_python_sdk-1.0.0/test/test_models/test_os.py` & `sendpost_python_sdk-1.1.1/test/test_models/test_os.py`

 * *Files identical despite different names*

### Comparing `sendpost_python_sdk-1.0.0/test/test_models/test_q_email_message.py` & `sendpost_python_sdk-1.1.1/test/test_models/test_q_email_message.py`

 * *Files identical despite different names*

### Comparing `sendpost_python_sdk-1.0.0/test/test_models/test_q_event.py` & `sendpost_python_sdk-1.1.1/test/test_models/test_q_event.py`

 * *Files identical despite different names*

### Comparing `sendpost_python_sdk-1.0.0/test/test_models/test_reply_to.py` & `sendpost_python_sdk-1.1.1/test/test_models/test_reply_to.py`

 * *Files identical despite different names*

### Comparing `sendpost_python_sdk-1.0.0/test/test_models/test_to.py` & `sendpost_python_sdk-1.1.1/test/test_models/test_to.py`

 * *Files identical despite different names*

### Comparing `sendpost_python_sdk-1.0.0/test/test_models/test_user_agent.py` & `sendpost_python_sdk-1.1.1/test/test_models/test_user_agent.py`

 * *Files identical despite different names*

### Comparing `sendpost_python_sdk-1.0.0/test/test_models/test_webhook_event.py` & `sendpost_python_sdk-1.1.1/test/test_models/test_webhook_event.py`

 * *Files identical despite different names*

### Comparing `sendpost_python_sdk-1.0.0/test/test_paths/__init__.py` & `sendpost_python_sdk-1.1.1/test/test_paths/__init__.py`

 * *Files identical despite different names*

### Comparing `sendpost_python_sdk-1.0.0/test/test_paths/test_subaccount_email_/test_post.py` & `sendpost_python_sdk-1.1.1/test/test_paths/test_subaccount_email_/test_post.py`

 * *Files identical despite different names*

### Comparing `sendpost_python_sdk-1.0.0/test/test_paths/test_subaccount_email_template/test_post.py` & `sendpost_python_sdk-1.1.1/test/test_paths/test_subaccount_email_template/test_post.py`

 * *Files identical despite different names*

