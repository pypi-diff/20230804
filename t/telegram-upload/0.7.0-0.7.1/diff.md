# Comparing `tmp/telegram-upload-0.7.0.tar.gz` & `tmp/telegram-upload-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telegram-upload-0.7.0.tar", last modified: Thu Jun 29 16:27:54 2023, max compression
+gzip compressed data, was "telegram-upload-0.7.1.tar", last modified: Fri Aug  4 19:39:13 2023, max compression
```

## Comparing `telegram-upload-0.7.0.tar` & `telegram-upload-0.7.1.tar`

### file list

```diff
@@ -1,70 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:27:54.431312 telegram-upload-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8159 2023-06-29 16:27:54.431312 telegram-upload-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7150 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:27:54.419312 telegram-upload-0.7.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7452 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:27:54.419312 telegram-upload-0.7.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    49610 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/docs/_static/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10371 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/docs/caption_format.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     9637 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/docs/troubleshooting.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7056 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-29 16:27:54.431312 telegram-upload-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:27:54.423312 telegram-upload-0.7.0/telegram_upload/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/telegram_upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/telegram_upload/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    10692 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/telegram_upload/caption_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/telegram_upload/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:27:54.427312 telegram-upload-0.7.0/telegram_upload/client/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/telegram_upload/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/telegram_upload/client/progress_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/telegram_upload/client/telegram_download_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/telegram_upload/client/telegram_manager_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18180 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/telegram_upload/client/telegram_upload_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/telegram_upload/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8052 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/telegram_upload/download_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/telegram_upload/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11933 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/telegram_upload/management.py
--rw-r--r--   0 runner    (1001) docker     (123)     8487 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/telegram_upload/upload_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-06-29 16:27:30.000000 telegram-upload-0.7.0/telegram_upload/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-06-29 16:27:30.000000 telegram-upload-0.7.0/telegram_upload/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:27:54.423312 telegram-upload-0.7.0/telegram_upload.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8159 2023-06-29 16:27:54.000000 telegram-upload-0.7.0/telegram_upload.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-29 16:27:54.000000 telegram-upload-0.7.0/telegram_upload.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 16:27:54.000000 telegram-upload-0.7.0/telegram_upload.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-29 16:27:54.000000 telegram-upload-0.7.0/telegram_upload.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 16:27:54.000000 telegram-upload-0.7.0/telegram_upload.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-29 16:27:54.000000 telegram-upload-0.7.0/telegram_upload.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-29 16:27:54.000000 telegram-upload-0.7.0/telegram_upload.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:27:54.427312 telegram-upload-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 16:27:30.000000 telegram-upload-0.7.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-29 16:27:30.000000 telegram-upload-0.7.0/tests/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    19710 2023-06-29 16:27:30.000000 telegram-upload-0.7.0/tests/test_caption_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-29 16:27:30.000000 telegram-upload-0.7.0/tests/test_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:27:54.431312 telegram-upload-0.7.0/tests/test_client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 16:27:30.000000 telegram-upload-0.7.0/tests/test_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-29 16:27:30.000000 telegram-upload-0.7.0/tests/test_client/test_progress_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-06-29 16:27:30.000000 telegram-upload-0.7.0/tests/test_client/test_telegram_download_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-06-29 16:27:30.000000 telegram-upload-0.7.0/tests/test_client/test_telegram_manager_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8819 2023-06-29 16:27:30.000000 telegram-upload-0.7.0/tests/test_client/test_telegram_upload_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-29 16:27:30.000000 telegram-upload-0.7.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10678 2023-06-29 16:27:30.000000 telegram-upload-0.7.0/tests/test_download_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-29 16:27:30.000000 telegram-upload-0.7.0/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-06-29 16:27:30.000000 telegram-upload-0.7.0/tests/test_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-06-29 16:27:30.000000 telegram-upload-0.7.0/tests/test_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-29 16:27:30.000000 telegram-upload-0.7.0/tests/test_upload_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-29 16:27:30.000000 telegram-upload-0.7.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-06-29 16:27:30.000000 telegram-upload-0.7.0/tests/test_video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:39:13.562871 telegram-upload-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-08-04 19:38:44.000000 telegram-upload-0.7.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-08-04 19:38:44.000000 telegram-upload-0.7.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-08-04 19:38:44.000000 telegram-upload-0.7.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-04 19:38:44.000000 telegram-upload-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-08-04 19:38:44.000000 telegram-upload-0.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8160 2023-08-04 19:39:13.562871 telegram-upload-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7150 2023-08-04 19:38:44.000000 telegram-upload-0.7.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:39:13.554871 telegram-upload-0.7.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7452 2023-08-04 19:38:44.000000 telegram-upload-0.7.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:39:13.554871 telegram-upload-0.7.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    49610 2023-08-04 19:38:44.000000 telegram-upload-0.7.1/docs/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-04 19:38:44.000000 telegram-upload-0.7.1/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    44622 2023-08-04 19:38:44.000000 telegram-upload-0.7.1/docs/benchmark_2.0_GiB.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-08-04 19:38:44.000000 telegram-upload-0.7.1/docs/benchmark_2.0_GiB.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    43777 2023-08-04 19:38:44.000000 telegram-upload-0.7.1/docs/benchmark_20.0_MiB.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-08-04 19:38:44.000000 telegram-upload-0.7.1/docs/benchmark_20.0_MiB.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    48786 2023-08-04 19:38:44.000000 telegram-upload-0.7.1/docs/benchmark_200.0_MiB.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-08-04 19:38:44.000000 telegram-upload-0.7.1/docs/benchmark_200.0_MiB.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    49074 2023-08-04 19:38:44.000000 telegram-upload-0.7.1/docs/benchmark_512.0_KiB.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-04 19:38:44.000000 telegram-upload-0.7.1/docs/benchmark_512.0_KiB.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14396 2023-08-04 19:38:44.000000 telegram-upload-0.7.1/docs/benchmark_full.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10371 2023-08-04 19:38:44.000000 telegram-upload-0.7.1/docs/caption_format.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9638 2023-08-04 19:38:44.000000 telegram-upload-0.7.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-04 19:38:44.000000 telegram-upload-0.7.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-04 19:38:44.000000 telegram-upload-0.7.1/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-08-04 19:38:44.000000 telegram-upload-0.7.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-08-04 19:38:44.000000 telegram-upload-0.7.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-04 19:38:44.000000 telegram-upload-0.7.1/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14189 2023-08-04 19:38:44.000000 telegram-upload-0.7.1/docs/supported_file_types.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-08-04 19:38:44.000000 telegram-upload-0.7.1/docs/troubleshooting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-08-04 19:38:44.000000 telegram-upload-0.7.1/docs/upload_benchmark.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7056 2023-08-04 19:38:44.000000 telegram-upload-0.7.1/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-04 19:38:44.000000 telegram-upload-0.7.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-08-04 19:39:13.562871 telegram-upload-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-08-04 19:38:44.000000 telegram-upload-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:39:13.558871 telegram-upload-0.7.1/telegram_upload/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-08-04 19:38:44.000000 telegram-upload-0.7.1/telegram_upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-08-04 19:38:44.000000 telegram-upload-0.7.1/telegram_upload/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10692 2023-08-04 19:38:44.000000 telegram-upload-0.7.1/telegram_upload/caption_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-08-04 19:38:44.000000 telegram-upload-0.7.1/telegram_upload/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:39:13.558871 telegram-upload-0.7.1/telegram_upload/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-08-04 19:38:44.000000 telegram-upload-0.7.1/telegram_upload/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-08-04 19:38:44.000000 telegram-upload-0.7.1/telegram_upload/client/progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-08-04 19:38:44.000000 telegram-upload-0.7.1/telegram_upload/client/telegram_download_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-08-04 19:38:44.000000 telegram-upload-0.7.1/telegram_upload/client/telegram_manager_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18187 2023-08-04 19:38:44.000000 telegram-upload-0.7.1/telegram_upload/client/telegram_upload_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-08-04 19:38:44.000000 telegram-upload-0.7.1/telegram_upload/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8052 2023-08-04 19:38:44.000000 telegram-upload-0.7.1/telegram_upload/download_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-08-04 19:38:44.000000 telegram-upload-0.7.1/telegram_upload/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11977 2023-08-04 19:38:44.000000 telegram-upload-0.7.1/telegram_upload/management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8487 2023-08-04 19:38:44.000000 telegram-upload-0.7.1/telegram_upload/upload_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-08-04 19:38:44.000000 telegram-upload-0.7.1/telegram_upload/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-08-04 19:38:44.000000 telegram-upload-0.7.1/telegram_upload/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:39:13.558871 telegram-upload-0.7.1/telegram_upload.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8160 2023-08-04 19:39:13.000000 telegram-upload-0.7.1/telegram_upload.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-08-04 19:39:13.000000 telegram-upload-0.7.1/telegram_upload.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 19:39:13.000000 telegram-upload-0.7.1/telegram_upload.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-08-04 19:39:13.000000 telegram-upload-0.7.1/telegram_upload.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 19:39:13.000000 telegram-upload-0.7.1/telegram_upload.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-04 19:39:13.000000 telegram-upload-0.7.1/telegram_upload.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 19:39:13.000000 telegram-upload-0.7.1/telegram_upload.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:39:13.562871 telegram-upload-0.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 19:38:44.000000 telegram-upload-0.7.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-08-04 19:38:44.000000 telegram-upload-0.7.1/tests/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19710 2023-08-04 19:38:44.000000 telegram-upload-0.7.1/tests/test_caption_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-08-04 19:38:44.000000 telegram-upload-0.7.1/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:39:13.562871 telegram-upload-0.7.1/tests/test_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 19:38:44.000000 telegram-upload-0.7.1/tests/test_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-08-04 19:38:44.000000 telegram-upload-0.7.1/tests/test_client/test_progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-08-04 19:38:44.000000 telegram-upload-0.7.1/tests/test_client/test_telegram_download_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-08-04 19:38:44.000000 telegram-upload-0.7.1/tests/test_client/test_telegram_manager_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8819 2023-08-04 19:38:44.000000 telegram-upload-0.7.1/tests/test_client/test_telegram_upload_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-08-04 19:38:44.000000 telegram-upload-0.7.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10678 2023-08-04 19:38:44.000000 telegram-upload-0.7.1/tests/test_download_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-08-04 19:38:44.000000 telegram-upload-0.7.1/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-08-04 19:38:44.000000 telegram-upload-0.7.1/tests/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-08-04 19:38:44.000000 telegram-upload-0.7.1/tests/test_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-08-04 19:38:44.000000 telegram-upload-0.7.1/tests/test_upload_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-08-04 19:38:44.000000 telegram-upload-0.7.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-08-04 19:38:44.000000 telegram-upload-0.7.1/tests/test_video.py
```

### Comparing `telegram-upload-0.7.0/CONTRIBUTING.rst` & `telegram-upload-0.7.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.7.0/HISTORY.rst` & `telegram-upload-0.7.1/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =======
 History
 =======
 
+0.7.1 (2023-08-04)
+------------------
+
+* Issue #215: "TypeError: __init__() got an unexpected keyword argument 'reply_to_msg_id'" in command - "telegram-upload --directories "recursive" --album"
+
 0.7.0 (2023-06-29)
 ------------------
 
 * Issue #140: Speed up upload & download speed
 * Issue #115: Add support for variables in the caption argument
 * Issue #159: Telegram premium
 * Issue #176: Bug uploading .flv files
```

### Comparing `telegram-upload-0.7.0/LICENSE` & `telegram-upload-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.7.0/PKG-INFO` & `telegram-upload-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: telegram-upload
-Version: 0.7.0
-Summary: Upload (and download) files to Telegram up to 2 GiB using your account 
+Version: 0.7.1
+Summary: Upload (and download) files to Telegram up to 4 GiB using your account. 
 Home-page: https://github.com/Nekmo/telegram-upload/
 Download-URL: https://github.com/Nekmo/telegram-upload/archive/master.zip
 Author: Nekmo
 Author-email: contacto@nekmo.com
 Keywords: telegram-upload,telegram,upload,video
 Platform: linux
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Natural Language :: English
 Classifier: Development Status :: 5 - Production/Stable
-Provides: telegram_upload
 Provides: tests
+Provides: telegram_upload
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 
 .. image:: https://raw.githubusercontent.com/Nekmo/telegram-upload/master/logo.png
     :width: 100%
```

### Comparing `telegram-upload-0.7.0/README.rst` & `telegram-upload-0.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.7.0/docs/Makefile` & `telegram-upload-0.7.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.7.0/docs/_static/logo.png` & `telegram-upload-0.7.1/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.7.0/docs/caption_format.rst` & `telegram-upload-0.7.1/docs/caption_format.rst`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.7.0/docs/conf.py` & `telegram-upload-0.7.1/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,15 +130,15 @@
 html_theme = os.environ.get('HTML_THEME', 'alabaster')
 
 # Theme options are theme-specific and customize the look and feel of a
 # theme further.  For a list of options available for each theme, see the
 # documentation.
 html_theme_options = {
     'logo': 'logo.png',
-    'description': 'Upload and download files to Telegram up to 2GiB',
+    'description': 'Upload and download files to Telegram up to 4 GiB',
     'github_user': 'Nekmo',
     'github_repo': 'telegram-upload',
     'github_type': 'star',
     'github_banner': True,
     'travis_button': True,
     'codecov_button': True,
     'analytics_id': 'UA-62276079-1',
```

### Comparing `telegram-upload-0.7.0/docs/index.rst` & `telegram-upload-0.7.1/docs/index.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Welcome to telegram-upload's documentation!
 ===========================================
-Telegram-upload uses your personal Telegram account to upload and download files up to 2GiB (bots are limited to 50
-MiB). Turn Telegram into your personal cloud!
+Telegram-upload uses your personal Telegram account to upload and download files up to 4 GiB (2 GiB for free users).
+Turn Telegram into your personal cloud!
 
 
 To **install** telegram-upload, run this command in your terminal:
 
 .. code-block:: console
 
     $ pip install -U telegram-upload
@@ -18,14 +18,16 @@
    :maxdepth: 2
    :glob:
 
    installation
    readme
    usage
    caption_format
+   supported_file_types
+   upload_benchmark
    troubleshooting
    contributing
    authors
    history
 
 
 ..
```

### Comparing `telegram-upload-0.7.0/docs/installation.rst` & `telegram-upload-0.7.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.7.0/docs/troubleshooting.rst` & `telegram-upload-0.7.1/docs/troubleshooting.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Troubleshooting
 ===============
 
 Videos are not streameable in Telegram app
 -------------------------------------------
-**Only mp4 videos can be played on Telegram without downloading them first**. To stream your video in Telegram you must
-convert it before uploading it. For example you can use ffmpeg to convert your video::
+**Only some videos can be played on Telegram without downloading them first**. To stream your video in Telegram you must
+convert it before uploading it. For example you can use ffmpeg to convert your video to mp4::
 
     $ ffmpeg -i input.mov -preset slow -codec:a libfdk_aac -b:a 128k \
              -codec:v libx264 -pix_fmt yuv420p -b:v 2500k -minrate 1500k \
              -maxrate 4000k -bufsize 5000k -vf scale=-1:720 output.mp4
 
+You can see the :ref:`supported_file_types` reference for more information.
 
 Database is locked
 ------------------
 Telegram-upload is already running, or an old process **has locked the session** (``telegram-upload.session``). Only one
 Telegram-upload session can be run at a time.
 
 **If you need to run Telegram-upload multiple times anyway**, you need to duplicate the session and config files:
@@ -26,14 +27,15 @@
 
 If you are sure that Telegram-upload is not running, search for the process that is blocking the file::
 
     fuser ~/.config/telegram-upload.session
 
 As a last resort, you can restart your machine.
 
+.. _troubleshooting_429_errors:
 
 I am getting 429 errors during upload
 -------------------------------------
 Since version v0.7.0 Telegram-upload uploads several parts of the file in parallel. Become of this, the Telegram API
 can become overloaded and return 429 errors. This is normal and you don't have to worry. If you are getting too many of
 these errors, you can try to reduce the number of parallel uploads using the ``PARALLEL_UPLOAD_BLOCKS`` environment
 variable. For example::
@@ -49,14 +51,16 @@
 an error will try to reconnect to the API before ``TELEGRAM_UPLOAD_MIN_RECONNECT_WAIT`` seconds. The default value is 2.
 This value will be increased with each retry. Each retry will decrease the number of ``PARALLEL_UPLOAD_BLOCKS``. The
 minimum of ``PARALLEL_UPLOAD_BLOCKS`` is one. Telegram-upload will retry connecting up to
 ``TELEGRAM_UPLOAD_MAX_RECONNECT_RETRIES`` times. The default value is 5. Each retry has a maximum wait time of
 ``TELEGRAM_UPLOAD_RECONNECT_TIMEOUT`` seconds before failing. All of these variables can be defined using environment
 variables.
 
+Read more about the parallel chunks in the :ref:`upload_benchmark` section.
+
 Telegram-upload does not work! An error occurs when executing it
 -----------------------------------------------------------------
 Telegram-upload is not tested with all versions of all dependencies it uses. If you have installed Telegram-upload
 on your system (using root) maybe some existing dependency is on an incompatible version. You can try updating the
 dependencies carefully::
 
     $ pip install -U telegram-upload Telethon hachoir cryptg click
@@ -65,7 +69,17 @@
 
 Before asking for help, remember to find out if `the issue already exists <https://github
 .com/Nekmo/telegram-upload/issues>`_. If you open a ticket remember to paste your system dependencies on the issue::
 
     $ pip freeze
 
 Some problems may not be related to Telegram-upload. If possible, `Google before asking <https://google.com/>`_.
+
+Telegram-upload is very slow uploading files!
+---------------------------------------------
+Telegram-upload since version v0.7.0 uploads several parts of the file in parallel. This can increase the upload speed
+of the files. By default it uploads 4 parts of the file in parallel. You can change this value using the
+``PARALLEL_UPLOAD_BLOCKS`` environment variable (read more about this in the :ref:`troubleshooting_429_errors` section).
+Make sure you have updated Telegram-upload to the latest version and you have ``libssl`` installed on your system and
+``cryptg`` installed on your Python environment.
+
+Read more about the Telegram-upload speed in the :ref:`upload_benchmark` section.
```

### Comparing `telegram-upload-0.7.0/docs/usage.rst` & `telegram-upload-0.7.1/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.7.0/setup.py` & `telegram-upload-0.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-"""Upload (and download) files to Telegram up to 2 GiB using your account
+"""Upload (and download) files to Telegram up to 4 GiB using your account.
 """
 import copy
 import os
 import glob
 from itertools import chain
 from setuptools import setup, find_packages
```

### Comparing `telegram-upload-0.7.0/telegram_upload/_compat.py` & `telegram-upload-0.7.1/telegram_upload/_compat.py`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.7.0/telegram_upload/caption_formatter.py` & `telegram-upload-0.7.1/telegram_upload/caption_formatter.py`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.7.0/telegram_upload/cli.py` & `telegram-upload-0.7.1/telegram_upload/cli.py`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.7.0/telegram_upload/client/telegram_download_client.py` & `telegram-upload-0.7.1/telegram_upload/client/telegram_download_client.py`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.7.0/telegram_upload/client/telegram_manager_client.py` & `telegram-upload-0.7.1/telegram_upload/client/telegram_manager_client.py`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.7.0/telegram_upload/client/telegram_upload_client.py` & `telegram-upload-0.7.1/telegram_upload/client/telegram_upload_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,16 +35,15 @@
     def forward_to(self, message, destinations):
         for destination in destinations:
             self.forward_messages(destination, [message])
 
     async def _send_album_media(self, entity, media):
         entity = await self.get_input_entity(entity)
         request = functions.messages.SendMultiMediaRequest(
-            entity, reply_to_msg_id=None, multi_media=media,
-            silent=None, schedule_date=None, clear_draft=None
+            entity, multi_media=media, silent=None, schedule_date=None, clear_draft=None
         )
         result = await self(request)
 
         random_ids = [m.random_id for m in media]
         return self._get_response_message(random_ids, result, entity)
 
     def send_files_as_album(self, entity, files, delete_on_success=False, print_file_id=False,
@@ -134,14 +133,15 @@
                 click.echo('Uploaded successfully "{}" (file_id {})'.format(file.file_name,
                                                                             pack_bot_file_id(message.media)))
             if message and delete_on_success:
                 click.echo('Deleting "{}"'.format(file))
                 os.remove(file.path)
             if message:
                 self.forward_to(message, forward)
+                messages.append(message)
         if not has_files:
             raise MissingFileError('Files do not exist.')
         return messages
 
     async def upload_file(
             self: 'TelegramClient',
             file: 'hints.FileLike',
```

### Comparing `telegram-upload-0.7.0/telegram_upload/config.py` & `telegram-upload-0.7.1/telegram_upload/config.py`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.7.0/telegram_upload/download_files.py` & `telegram-upload-0.7.1/telegram_upload/download_files.py`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.7.0/telegram_upload/exceptions.py` & `telegram-upload-0.7.1/telegram_upload/exceptions.py`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.7.0/telegram_upload/management.py` & `telegram-upload-0.7.1/telegram_upload/management.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,16 +141,16 @@
 @click.option('-i', '--interactive', is_flag=True,
               help='Use interactive mode.')
 @click.option('--sort', is_flag=True,
               help='Sort files by name before upload it. Install the natsort Python package for natural sorting.')
 def upload(files, to, config, delete_on_success, print_file_id, force_file, forward, directories, large_files, caption,
            no_thumbnail, thumbnail_file, proxy, album, interactive, sort):
     """Upload one or more files to Telegram using your personal account.
-    The maximum file size is 2 GiB and by default they will be saved in
-    your saved messages.
+    The maximum file size is 2 GiB for free users and 4 GiB for premium accounts.
+    By default, they will be saved in your saved messages.
     """
     client = TelegramManagerClient(config or default_config(), proxy=proxy)
     client.start()
     if interactive and not files:
         click.echo('Select the local files to upload:')
         click.echo('[SPACE] Select file [ENTER] Next step')
         files = async_to_sync(interactive_select_local_files())
```

### Comparing `telegram-upload-0.7.0/telegram_upload/upload_files.py` & `telegram-upload-0.7.1/telegram_upload/upload_files.py`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.7.0/telegram_upload/utils.py` & `telegram-upload-0.7.1/telegram_upload/utils.py`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.7.0/telegram_upload/video.py` & `telegram-upload-0.7.1/telegram_upload/video.py`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.7.0/telegram_upload.egg-info/PKG-INFO` & `telegram-upload-0.7.1/telegram_upload.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: telegram-upload
-Version: 0.7.0
-Summary: Upload (and download) files to Telegram up to 2 GiB using your account 
+Version: 0.7.1
+Summary: Upload (and download) files to Telegram up to 4 GiB using your account. 
 Home-page: https://github.com/Nekmo/telegram-upload/
 Download-URL: https://github.com/Nekmo/telegram-upload/archive/master.zip
 Author: Nekmo
 Author-email: contacto@nekmo.com
 Keywords: telegram-upload,telegram,upload,video
 Platform: linux
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Natural Language :: English
 Classifier: Development Status :: 5 - Production/Stable
-Provides: telegram_upload
 Provides: tests
+Provides: telegram_upload
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 
 .. image:: https://raw.githubusercontent.com/Nekmo/telegram-upload/master/logo.png
     :width: 100%
```

### Comparing `telegram-upload-0.7.0/telegram_upload.egg-info/SOURCES.txt` & `telegram-upload-0.7.1/telegram_upload.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -5,22 +5,33 @@
 MANIFEST.in
 README.rst
 requirements.txt
 setup.cfg
 setup.py
 docs/Makefile
 docs/authors.rst
+docs/benchmark_2.0_GiB.png
+docs/benchmark_2.0_GiB.rst
+docs/benchmark_20.0_MiB.png
+docs/benchmark_20.0_MiB.rst
+docs/benchmark_200.0_MiB.png
+docs/benchmark_200.0_MiB.rst
+docs/benchmark_512.0_KiB.png
+docs/benchmark_512.0_KiB.rst
+docs/benchmark_full.rst
 docs/caption_format.rst
 docs/conf.py
 docs/contributing.rst
 docs/history.rst
 docs/index.rst
 docs/installation.rst
 docs/readme.rst
+docs/supported_file_types.rst
 docs/troubleshooting.rst
+docs/upload_benchmark.rst
 docs/usage.rst
 docs/_static/logo.png
 telegram_upload/__init__.py
 telegram_upload/_compat.py
 telegram_upload/caption_formatter.py
 telegram_upload/cli.py
 telegram_upload/config.py
```

### Comparing `telegram-upload-0.7.0/tests/test_caption_formatter.py` & `telegram-upload-0.7.1/tests/test_caption_formatter.py`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.7.0/tests/test_cli.py` & `telegram-upload-0.7.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.7.0/tests/test_client/test_progress_bar.py` & `telegram-upload-0.7.1/tests/test_client/test_progress_bar.py`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.7.0/tests/test_client/test_telegram_download_client.py` & `telegram-upload-0.7.1/tests/test_client/test_telegram_download_client.py`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.7.0/tests/test_client/test_telegram_manager_client.py` & `telegram-upload-0.7.1/tests/test_client/test_telegram_manager_client.py`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.7.0/tests/test_client/test_telegram_upload_client.py` & `telegram-upload-0.7.1/tests/test_client/test_telegram_upload_client.py`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.7.0/tests/test_config.py` & `telegram-upload-0.7.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.7.0/tests/test_download_files.py` & `telegram-upload-0.7.1/tests/test_download_files.py`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.7.0/tests/test_exceptions.py` & `telegram-upload-0.7.1/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.7.0/tests/test_files.py` & `telegram-upload-0.7.1/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.7.0/tests/test_management.py` & `telegram-upload-0.7.1/tests/test_management.py`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.7.0/tests/test_upload_files.py` & `telegram-upload-0.7.1/tests/test_upload_files.py`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.7.0/tests/test_utils.py` & `telegram-upload-0.7.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.7.0/tests/test_video.py` & `telegram-upload-0.7.1/tests/test_video.py`

 * *Files identical despite different names*

