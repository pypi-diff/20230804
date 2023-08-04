# Comparing `tmp/alex_ber_utils-0.6.6b3.tar.gz` & `tmp/alex_ber_utils-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alex_ber_utils-0.6.6b3.tar", last modified: Sun Jun 13 11:52:59 2021, max compression
+gzip compressed data, was "alex_ber_utils-0.7.0.tar", last modified: Fri Aug  4 09:44:55 2023, max compression
```

## Comparing `alex_ber_utils-0.6.6b3.tar` & `alex_ber_utils-0.7.0.tar`

### file list

```diff
@@ -1,91 +1,93 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-06-13 11:52:57.935463 alex_ber_utils-0.6.6b3/
--rwxr-xr-x   0 root         (0) root         (0)    24866 2021-06-13 11:51:04.000000 alex_ber_utils-0.6.6b3/CHANGELOG.md
--rwxr-xr-x   0 root         (0) root         (0)     1317 2019-05-22 09:49:27.000000 alex_ber_utils-0.6.6b3/LICENSE.txt
--rwxr-xr-x   0 root         (0) root         (0)      202 2019-12-15 05:14:26.000000 alex_ber_utils-0.6.6b3/MANIFEST.in
--rwxr-xr-x   0 root         (0) root         (0)    34831 2021-06-13 11:52:59.346450 alex_ber_utils-0.6.6b3/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)     3713 2021-04-07 11:32:02.000000 alex_ber_utils-0.6.6b3/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-06-13 11:52:58.107453 alex_ber_utils-0.6.6b3/alex_ber_utils.egg-info/
--rwxr-xr-x   0 root         (0) root         (0)    34831 2021-06-13 11:52:56.000000 alex_ber_utils-0.6.6b3/alex_ber_utils.egg-info/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)     2080 2021-06-13 11:52:57.000000 alex_ber_utils-0.6.6b3/alex_ber_utils.egg-info/SOURCES.txt
--rwxr-xr-x   0 root         (0) root         (0)        1 2021-06-13 11:52:56.000000 alex_ber_utils-0.6.6b3/alex_ber_utils.egg-info/dependency_links.txt
--rwxr-xr-x   0 root         (0) root         (0)        8 2021-06-13 11:52:56.000000 alex_ber_utils-0.6.6b3/alex_ber_utils.egg-info/namespace_packages.txt
--rwxr-xr-x   0 root         (0) root         (0)        1 2021-06-13 11:52:52.000000 alex_ber_utils-0.6.6b3/alex_ber_utils.egg-info/not-zip-safe
--rwxr-xr-x   0 root         (0) root         (0)      366 2021-06-13 11:52:56.000000 alex_ber_utils-0.6.6b3/alex_ber_utils.egg-info/requires.txt
--rwxr-xr-x   0 root         (0) root         (0)       19 2021-06-13 11:52:56.000000 alex_ber_utils-0.6.6b3/alex_ber_utils.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-06-13 11:52:57.370487 alex_ber_utils-0.6.6b3/alexber/
--rwxr-xr-x   0 root         (0) root         (0)       63 2019-05-12 06:22:19.000000 alex_ber_utils-0.6.6b3/alexber/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-06-13 11:52:58.378459 alex_ber_utils-0.6.6b3/alexber/utils/
--rwxr-xr-x   0 root         (0) root         (0)      256 2019-05-22 15:14:47.000000 alex_ber_utils-0.6.6b3/alexber/utils/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     8401 2020-05-06 15:27:53.000000 alex_ber_utils-0.6.6b3/alexber/utils/_ymlparsers_extra.py
--rwxr-xr-x   0 root         (0) root         (0)     4037 2020-07-30 11:19:18.000000 alex_ber_utils-0.6.6b3/alexber/utils/deploys.py
--rwxr-xr-x   0 root         (0) root         (0)    17807 2020-11-04 09:55:32.000000 alex_ber_utils-0.6.6b3/alexber/utils/emails.py
--rwxr-xr-x   0 root         (0) root         (0)     1485 2019-05-22 14:33:17.000000 alex_ber_utils-0.6.6b3/alexber/utils/enums.py
--rwxr-xr-x   0 root         (0) root         (0)     1561 2020-05-06 10:36:11.000000 alex_ber_utils-0.6.6b3/alexber/utils/fabs.py
--rwxr-xr-x   0 root         (0) root         (0)      888 2021-04-05 07:51:03.000000 alex_ber_utils-0.6.6b3/alexber/utils/files.py
--rwxr-xr-x   0 root         (0) root         (0)     3405 2020-07-28 12:02:05.000000 alex_ber_utils-0.6.6b3/alexber/utils/importer.py
--rwxr-xr-x   0 root         (0) root         (0)    19807 2020-07-28 05:43:19.000000 alex_ber_utils-0.6.6b3/alexber/utils/init_app_conf.py
--rwxr-xr-x   0 root         (0) root         (0)     1439 2020-10-20 17:32:41.000000 alex_ber_utils-0.6.6b3/alexber/utils/inspects.py
--rwxr-xr-x   0 root         (0) root         (0)    11467 2021-04-11 06:23:17.000000 alex_ber_utils-0.6.6b3/alexber/utils/mains.py
--rwxr-xr-x   0 root         (0) root         (0)     4363 2020-07-28 05:43:53.000000 alex_ber_utils-0.6.6b3/alexber/utils/parsers.py
--rwxr-xr-x   0 root         (0) root         (0)    10683 2020-05-06 22:26:59.000000 alex_ber_utils-0.6.6b3/alexber/utils/processinvokes.py
--rwxr-xr-x   0 root         (0) root         (0)    12074 2020-07-23 13:42:13.000000 alex_ber_utils-0.6.6b3/alexber/utils/props.py
--rwxr-xr-x   0 root         (0) root         (0)     2368 2020-04-01 18:42:42.000000 alex_ber_utils-0.6.6b3/alexber/utils/setups.py
--rwxr-xr-x   0 root         (0) root         (0)     3284 2021-06-13 11:51:04.000000 alex_ber_utils-0.6.6b3/alexber/utils/stdlogging.py
--rwxr-xr-x   0 root         (0) root         (0)      679 2019-05-23 11:42:44.000000 alex_ber_utils-0.6.6b3/alexber/utils/thread_locals.py
--rwxr-xr-x   0 root         (0) root         (0)     1785 2019-05-22 13:01:03.000000 alex_ber_utils-0.6.6b3/alexber/utils/uuids.py
--rwxr-xr-x   0 root         (0) root         (0)    11830 2020-07-28 05:44:13.000000 alex_ber_utils-0.6.6b3/alexber/utils/ymlparsers.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-06-13 11:52:57.390453 alex_ber_utils-0.6.6b3/data/
--rwxr-xr-x   0 root         (0) root         (0)        0 2019-05-22 10:08:43.000000 alex_ber_utils-0.6.6b3/data/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)       23 2020-05-01 21:22:23.000000 alex_ber_utils-0.6.6b3/req-env.txt
--rwxr-xr-x   0 root         (0) root         (0)       13 2020-04-02 20:06:26.000000 alex_ber_utils-0.6.6b3/req-fabric.txt
--rwxr-xr-x   0 root         (0) root         (0)       18 2020-04-02 20:06:20.000000 alex_ber_utils-0.6.6b3/req-md.txt
--rwxr-xr-x   0 root         (0) root         (0)       37 2020-04-02 20:07:00.000000 alex_ber_utils-0.6.6b3/req-yml.txt
--rwxr-xr-x   0 root         (0) root         (0)       21 2020-10-31 19:56:18.000000 alex_ber_utils-0.6.6b3/requirements-env.txt
--rwxr-xr-x   0 root         (0) root         (0)      142 2021-06-13 09:52:59.000000 alex_ber_utils-0.6.6b3/requirements-fabric.txt
--rwxr-xr-x   0 root         (0) root         (0)       18 2019-05-22 13:41:32.000000 alex_ber_utils-0.6.6b3/requirements-md.txt
--rwxr-xr-x   0 root         (0) root         (0)      192 2020-12-12 00:22:57.000000 alex_ber_utils-0.6.6b3/requirements-tests.txt
--rwxr-xr-x   0 root         (0) root         (0)       64 2021-05-23 20:56:58.000000 alex_ber_utils-0.6.6b3/requirements-yml.txt
--rwxr-xr-x   0 root         (0) root         (0)       11 2020-04-02 20:09:09.000000 alex_ber_utils-0.6.6b3/requirements.txt
--rwxr-xr-x   0 root         (0) root         (0)      189 2021-06-13 11:52:59.363486 alex_ber_utils-0.6.6b3/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     4703 2021-06-13 11:51:04.000000 alex_ber_utils-0.6.6b3/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-06-13 11:52:57.411453 alex_ber_utils-0.6.6b3/tests/
--rwxr-xr-x   0 root         (0) root         (0)        0 2019-05-22 09:59:23.000000 alex_ber_utils-0.6.6b3/tests/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     1992 2020-11-02 14:02:48.000000 alex_ber_utils-0.6.6b3/tests/conftest.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-06-13 11:52:57.456453 alex_ber_utils-0.6.6b3/tests/utils/
--rwxr-xr-x   0 root         (0) root         (0)        0 2019-05-22 09:59:46.000000 alex_ber_utils-0.6.6b3/tests/utils/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     6227 2020-12-02 09:31:00.000000 alex_ber_utils-0.6.6b3/tests/utils/deploys_test.py
--rwxr-xr-x   0 root         (0) root         (0)     8937 2020-11-18 17:01:37.000000 alex_ber_utils-0.6.6b3/tests/utils/emails_test.py
--rwxr-xr-x   0 root         (0) root         (0)    10567 2019-05-22 15:14:47.000000 alex_ber_utils-0.6.6b3/tests/utils/enums_mixin_test.py
--rwxr-xr-x   0 root         (0) root         (0)     5242 2020-05-13 12:41:58.000000 alex_ber_utils-0.6.6b3/tests/utils/importer_test.py
--rwxr-xr-x   0 root         (0) root         (0)    31305 2021-02-16 18:59:01.000000 alex_ber_utils-0.6.6b3/tests/utils/init_app_conf_test.py
--rwxr-xr-x   0 root         (0) root         (0)     3830 2020-05-08 17:20:32.000000 alex_ber_utils-0.6.6b3/tests/utils/inspect_test.py
--rwxr-xr-x   0 root         (0) root         (0)     1383 2020-05-13 12:47:10.000000 alex_ber_utils-0.6.6b3/tests/utils/mains_test.py
--rwxr-xr-x   0 root         (0) root         (0)     2541 2019-05-22 13:38:31.000000 alex_ber_utils-0.6.6b3/tests/utils/method_overloading_test.py
--rwxr-xr-x   0 root         (0) root         (0)     5338 2020-06-07 12:37:42.000000 alex_ber_utils-0.6.6b3/tests/utils/parsers_test.py
--rwxr-xr-x   0 root         (0) root         (0)     5517 2020-09-09 13:07:15.000000 alex_ber_utils-0.6.6b3/tests/utils/processinvokes_test.py
--rwxr-xr-x   0 root         (0) root         (0)     1583 2020-04-07 19:11:13.000000 alex_ber_utils-0.6.6b3/tests/utils/properties_test.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-06-13 11:52:57.434458 alex_ber_utils-0.6.6b3/tests/utils/splitpackage/
--rwxr-xr-x   0 root         (0) root         (0)      119 2020-05-06 08:59:28.000000 alex_ber_utils-0.6.6b3/tests/utils/splitpackage/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)        0 2020-05-06 08:16:17.000000 alex_ber_utils-0.6.6b3/tests/utils/splitpackage/mymodule.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-06-13 11:52:57.456453 alex_ber_utils-0.6.6b3/tests/utils/splitpackage_cont/
--rwxr-xr-x   0 root         (0) root         (0)        0 2020-05-06 08:59:03.000000 alex_ber_utils-0.6.6b3/tests/utils/splitpackage_cont/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)       37 2020-05-06 08:23:59.000000 alex_ber_utils-0.6.6b3/tests/utils/splitpackage_cont/other_module.py
--rwxr-xr-x   0 root         (0) root         (0)     4077 2019-05-23 12:48:33.000000 alex_ber_utils-0.6.6b3/tests/utils/threadlocal_test.py
--rwxr-xr-x   0 root         (0) root         (0)     1099 2019-05-12 07:19:25.000000 alex_ber_utils-0.6.6b3/tests/utils/uuids_test.py
--rwxr-xr-x   0 root         (0) root         (0)    15188 2020-05-03 18:26:06.000000 alex_ber_utils-0.6.6b3/tests/utils/ymlparsers_extra_test.py
--rwxr-xr-x   0 root         (0) root         (0)    28051 2020-11-02 18:19:53.000000 alex_ber_utils-0.6.6b3/tests/utils/ymlparsers_test.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-06-13 11:52:57.502464 alex_ber_utils-0.6.6b3/tests_data/
--rwxr-xr-x   0 root         (0) root         (0)        0 2019-05-22 09:59:32.000000 alex_ber_utils-0.6.6b3/tests_data/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-06-13 11:52:57.514456 alex_ber_utils-0.6.6b3/tests_data/tests/
--rwxr-xr-x   0 root         (0) root         (0)        0 2019-05-22 09:59:53.000000 alex_ber_utils-0.6.6b3/tests_data/tests/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-06-13 11:52:57.576464 alex_ber_utils-0.6.6b3/tests_data/tests/utils/
--rwxr-xr-x   0 root         (0) root         (0)        0 2019-05-22 10:00:01.000000 alex_ber_utils-0.6.6b3/tests_data/tests/utils/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      141 2019-05-12 07:19:16.000000 alex_ber_utils-0.6.6b3/tests_data/tests/utils/config.properties
--rwxr-xr-x   0 root         (0) root         (0)       86 2019-05-12 07:19:23.000000 alex_ber_utils-0.6.6b3/tests_data/tests/utils/config2.properties
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-06-13 11:52:57.536454 alex_ber_utils-0.6.6b3/tests_data/tests/utils/initappconf/
--rwxr-xr-x   0 root         (0) root         (0)        0 2020-04-06 17:32:42.000000 alex_ber_utils-0.6.6b3/tests_data/tests/utils/initappconf/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-06-13 11:52:57.557455 alex_ber_utils-0.6.6b3/tests_data/tests/utils/parser/
--rwxr-xr-x   0 root         (0) root         (0)        0 2019-05-22 12:34:09.000000 alex_ber_utils-0.6.6b3/tests_data/tests/utils/parser/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      196 2020-04-21 07:39:22.000000 alex_ber_utils-0.6.6b3/tests_data/tests/utils/parser/config.ini
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-06-13 11:52:57.576464 alex_ber_utils-0.6.6b3/tests_data/tests/utils/ymlparsers/
--rwxr-xr-x   0 root         (0) root         (0)        0 2020-04-06 17:32:42.000000 alex_ber_utils-0.6.6b3/tests_data/tests/utils/ymlparsers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 09:44:55.026902 alex_ber_utils-0.7.0/
+-rw-rw-r--   0 root         (0) root         (0)    25446 2023-08-04 09:28:15.000000 alex_ber_utils-0.7.0/CHANGELOG.md
+-rw-rw-r--   0 root         (0) root         (0)     1295 2022-08-28 13:06:40.000000 alex_ber_utils-0.7.0/LICENSE.txt
+-rw-rw-r--   0 root         (0) root         (0)      195 2022-08-28 13:06:40.000000 alex_ber_utils-0.7.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    30228 2023-08-04 09:44:55.026902 alex_ber_utils-0.7.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     3569 2023-08-02 08:51:34.000000 alex_ber_utils-0.7.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 09:44:55.022902 alex_ber_utils-0.7.0/alex_ber_utils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    30228 2023-08-04 09:44:54.000000 alex_ber_utils-0.7.0/alex_ber_utils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2111 2023-08-04 09:44:54.000000 alex_ber_utils-0.7.0/alex_ber_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 09:44:54.000000 alex_ber_utils-0.7.0/alex_ber_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-08-04 09:44:54.000000 alex_ber_utils-0.7.0/alex_ber_utils.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 09:42:49.000000 alex_ber_utils-0.7.0/alex_ber_utils.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      364 2023-08-04 09:44:54.000000 alex_ber_utils-0.7.0/alex_ber_utils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-08-04 09:44:54.000000 alex_ber_utils-0.7.0/alex_ber_utils.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 09:44:55.022902 alex_ber_utils-0.7.0/alexber/
+-rw-rw-r--   0 root         (0) root         (0)       55 2023-08-04 09:19:50.000000 alex_ber_utils-0.7.0/alexber/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 09:44:55.022902 alex_ber_utils-0.7.0/alexber/utils/
+-rw-rw-r--   0 root         (0) root         (0)      250 2022-08-28 13:06:40.000000 alex_ber_utils-0.7.0/alexber/utils/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8188 2022-08-28 13:06:40.000000 alex_ber_utils-0.7.0/alexber/utils/_ymlparsers_extra.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 09:44:55.022902 alex_ber_utils-0.7.0/alexber/utils/data/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-08-28 13:06:40.000000 alex_ber_utils-0.7.0/alexber/utils/data/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3928 2022-08-28 13:06:40.000000 alex_ber_utils-0.7.0/alexber/utils/deploys.py
+-rw-rw-r--   0 root         (0) root         (0)    17354 2022-08-28 13:06:40.000000 alex_ber_utils-0.7.0/alexber/utils/emails.py
+-rw-rw-r--   0 root         (0) root         (0)     1425 2022-08-28 13:06:40.000000 alex_ber_utils-0.7.0/alexber/utils/enums.py
+-rw-rw-r--   0 root         (0) root         (0)     1512 2022-08-28 13:06:40.000000 alex_ber_utils-0.7.0/alexber/utils/fabs.py
+-rw-rw-r--   0 root         (0) root         (0)      857 2022-08-28 13:06:40.000000 alex_ber_utils-0.7.0/alexber/utils/files.py
+-rw-rw-r--   0 root         (0) root         (0)     3300 2022-08-28 13:06:40.000000 alex_ber_utils-0.7.0/alexber/utils/importer.py
+-rw-rw-r--   0 root         (0) root         (0)    19314 2022-08-28 13:06:40.000000 alex_ber_utils-0.7.0/alexber/utils/init_app_conf.py
+-rw-rw-r--   0 root         (0) root         (0)     1385 2022-08-28 13:06:40.000000 alex_ber_utils-0.7.0/alexber/utils/inspects.py
+-rw-rw-r--   0 root         (0) root         (0)    11144 2022-08-28 13:06:40.000000 alex_ber_utils-0.7.0/alexber/utils/mains.py
+-rw-rw-r--   0 root         (0) root         (0)     4210 2022-08-28 13:06:40.000000 alex_ber_utils-0.7.0/alexber/utils/parsers.py
+-rw-rw-r--   0 root         (0) root         (0)    10390 2022-08-28 13:06:40.000000 alex_ber_utils-0.7.0/alexber/utils/processinvokes.py
+-rw-rw-r--   0 root         (0) root         (0)    11721 2022-08-28 13:06:40.000000 alex_ber_utils-0.7.0/alexber/utils/props.py
+-rw-rw-r--   0 root         (0) root         (0)     2296 2022-08-28 13:06:40.000000 alex_ber_utils-0.7.0/alexber/utils/setups.py
+-rw-rw-r--   0 root         (0) root         (0)     3204 2022-08-28 13:06:40.000000 alex_ber_utils-0.7.0/alexber/utils/stdlogging.py
+-rw-rw-r--   0 root         (0) root         (0)      658 2022-08-28 13:06:40.000000 alex_ber_utils-0.7.0/alexber/utils/thread_locals.py
+-rw-rw-r--   0 root         (0) root         (0)     1745 2022-08-28 13:06:40.000000 alex_ber_utils-0.7.0/alexber/utils/uuids.py
+-rw-rw-r--   0 root         (0) root         (0)    11517 2022-08-28 13:06:40.000000 alex_ber_utils-0.7.0/alexber/utils/ymlparsers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 09:44:55.022902 alex_ber_utils-0.7.0/data/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-08-28 13:06:40.000000 alex_ber_utils-0.7.0/data/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)       22 2022-08-28 13:06:40.000000 alex_ber_utils-0.7.0/req-env.txt
+-rw-rw-r--   0 root         (0) root         (0)       13 2022-08-28 13:06:40.000000 alex_ber_utils-0.7.0/req-fabric.txt
+-rw-rw-r--   0 root         (0) root         (0)       18 2022-08-28 13:06:40.000000 alex_ber_utils-0.7.0/req-md.txt
+-rw-rw-r--   0 root         (0) root         (0)       32 2023-08-02 08:42:54.000000 alex_ber_utils-0.7.0/req-yml.txt
+-rw-rw-r--   0 root         (0) root         (0)       21 2022-08-28 13:06:40.000000 alex_ber_utils-0.7.0/requirements-env.txt
+-rw-rw-r--   0 root         (0) root         (0)      152 2023-08-04 09:06:54.000000 alex_ber_utils-0.7.0/requirements-fabric.txt
+-rw-rw-r--   0 root         (0) root         (0)       18 2023-08-03 21:18:06.000000 alex_ber_utils-0.7.0/requirements-md.txt
+-rw-rw-r--   0 root         (0) root         (0)      182 2023-08-03 14:10:05.000000 alex_ber_utils-0.7.0/requirements-tests.txt
+-rw-rw-r--   0 root         (0) root         (0)       61 2023-08-02 08:43:59.000000 alex_ber_utils-0.7.0/requirements-yml.txt
+-rw-rw-r--   0 root         (0) root         (0)       13 2023-08-02 11:23:45.000000 alex_ber_utils-0.7.0/requirements.txt
+-rw-rw-r--   0 root         (0) root         (0)      189 2023-08-04 09:44:55.030902 alex_ber_utils-0.7.0/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     4865 2023-08-04 09:41:56.000000 alex_ber_utils-0.7.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 09:44:55.022902 alex_ber_utils-0.7.0/tests/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-08-28 13:06:40.000000 alex_ber_utils-0.7.0/tests/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1931 2022-08-28 13:06:40.000000 alex_ber_utils-0.7.0/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 09:44:55.026902 alex_ber_utils-0.7.0/tests/utils/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-08-28 13:06:40.000000 alex_ber_utils-0.7.0/tests/utils/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6071 2022-08-28 13:06:40.000000 alex_ber_utils-0.7.0/tests/utils/deploys_test.py
+-rw-rw-r--   0 root         (0) root         (0)     8680 2022-08-28 13:06:40.000000 alex_ber_utils-0.7.0/tests/utils/emails_test.py
+-rw-rw-r--   0 root         (0) root         (0)    10227 2022-08-28 13:06:40.000000 alex_ber_utils-0.7.0/tests/utils/enums_mixin_test.py
+-rw-rw-r--   0 root         (0) root         (0)     5067 2022-08-28 13:06:40.000000 alex_ber_utils-0.7.0/tests/utils/importer_test.py
+-rw-rw-r--   0 root         (0) root         (0)    30475 2022-08-28 13:06:40.000000 alex_ber_utils-0.7.0/tests/utils/init_app_conf_test.py
+-rw-rw-r--   0 root         (0) root         (0)     3654 2022-08-28 13:06:40.000000 alex_ber_utils-0.7.0/tests/utils/inspect_test.py
+-rw-rw-r--   0 root         (0) root         (0)     1328 2022-08-28 13:06:40.000000 alex_ber_utils-0.7.0/tests/utils/mains_test.py
+-rw-rw-r--   0 root         (0) root         (0)     2444 2022-08-28 13:06:40.000000 alex_ber_utils-0.7.0/tests/utils/method_overloading_test.py
+-rw-rw-r--   0 root         (0) root         (0)     5106 2022-08-28 13:06:40.000000 alex_ber_utils-0.7.0/tests/utils/parsers_test.py
+-rw-rw-r--   0 root         (0) root         (0)     5372 2022-08-28 13:06:40.000000 alex_ber_utils-0.7.0/tests/utils/processinvokes_test.py
+-rw-rw-r--   0 root         (0) root         (0)     1529 2022-08-28 13:06:40.000000 alex_ber_utils-0.7.0/tests/utils/properties_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 09:44:55.026902 alex_ber_utils-0.7.0/tests/utils/splitpackage/
+-rw-rw-r--   0 root         (0) root         (0)      116 2022-08-28 13:06:40.000000 alex_ber_utils-0.7.0/tests/utils/splitpackage/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-08-28 13:06:40.000000 alex_ber_utils-0.7.0/tests/utils/splitpackage/mymodule.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 09:44:55.026902 alex_ber_utils-0.7.0/tests/utils/splitpackage_cont/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-08-28 13:06:40.000000 alex_ber_utils-0.7.0/tests/utils/splitpackage_cont/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)       34 2022-08-28 13:06:40.000000 alex_ber_utils-0.7.0/tests/utils/splitpackage_cont/other_module.py
+-rw-rw-r--   0 root         (0) root         (0)     3914 2022-08-28 13:06:40.000000 alex_ber_utils-0.7.0/tests/utils/threadlocal_test.py
+-rw-rw-r--   0 root         (0) root         (0)     1064 2022-08-28 13:06:40.000000 alex_ber_utils-0.7.0/tests/utils/uuids_test.py
+-rw-rw-r--   0 root         (0) root         (0)    14847 2022-08-28 13:06:40.000000 alex_ber_utils-0.7.0/tests/utils/ymlparsers_extra_test.py
+-rw-rw-r--   0 root         (0) root         (0)    27324 2022-08-28 13:06:40.000000 alex_ber_utils-0.7.0/tests/utils/ymlparsers_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 09:44:55.026902 alex_ber_utils-0.7.0/tests_data/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-08-28 13:06:40.000000 alex_ber_utils-0.7.0/tests_data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 09:44:55.026902 alex_ber_utils-0.7.0/tests_data/tests/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-08-28 13:06:40.000000 alex_ber_utils-0.7.0/tests_data/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 09:44:55.026902 alex_ber_utils-0.7.0/tests_data/tests/utils/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-08-28 13:06:40.000000 alex_ber_utils-0.7.0/tests_data/tests/utils/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      135 2022-08-28 13:06:40.000000 alex_ber_utils-0.7.0/tests_data/tests/utils/config.properties
+-rw-rw-r--   0 root         (0) root         (0)       81 2022-08-28 13:06:40.000000 alex_ber_utils-0.7.0/tests_data/tests/utils/config2.properties
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 09:44:55.026902 alex_ber_utils-0.7.0/tests_data/tests/utils/initappconf/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-08-28 13:06:40.000000 alex_ber_utils-0.7.0/tests_data/tests/utils/initappconf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 09:44:55.026902 alex_ber_utils-0.7.0/tests_data/tests/utils/parser/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-08-28 13:06:40.000000 alex_ber_utils-0.7.0/tests_data/tests/utils/parser/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      187 2022-08-28 13:06:40.000000 alex_ber_utils-0.7.0/tests_data/tests/utils/parser/config.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 09:44:55.026902 alex_ber_utils-0.7.0/tests_data/tests/utils/ymlparsers/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-08-28 13:06:40.000000 alex_ber_utils-0.7.0/tests_data/tests/utils/ymlparsers/__init__.py
```

### Comparing `alex_ber_utils-0.6.6b3/CHANGELOG.md` & `alex_ber_utils-0.7.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,41 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 \#https://pypi.org/manage/project/alex-ber-utils/releases/
 
 ## Unreleased
-## [0.6.6b3] - 13-06-2021
+
+
+## [0.7.0] - 04-08-2023
+
+#### Changed
+- 
+- Upgrade pyparsing==2.4.7 to 3.1.1.
+- Upgrade cryptography from 3.4.7 to 41.0.3.
+- Upgrade invoke from 1.4.1 to 1.7.3.
+- Upgrade six from 1.15.0 to 1.16.0.
+- Upgrade colorama from 0.4.3 to 0.4.4.
+- Change declaration of namespace to `declare_namespace()` mechanism.
+
+### Added
+- Explicit dependency on pyOpenSSL==22.1.0 (lowest version where cryptography version is 
+pinned). cryptography's and pyOpenSSL's version change should be in sync.
+
+## [0.6.6] - 13-06-2021
 ### Added
 - `stdLogging` module. The main function is `initStream()`. This is Thin adapter layer that redirects stdout/stderr 
 (or any other stream-like object) to standard Python's logger. Based on 
 https://github.com/fx-kirin/py-stdlogging/blob/master/stdlogging.py See https://github.com/fx-kirin/py-stdlogging/pull/1
 Quote from  https://stackoverflow.com/questions/47325506/making-python-loggers-log-all-stdout-and-stderr-messages :
 "But be careful to capture stdout because it's very fragile". I decided to focus on redirecting stderr only to the 
 logger. If you want you can also redirect stdout, by making 2 calls to initStream() package-level method. 
 But, because of https://unix.stackexchange.com/questions/616616/separate-stdout-and-stderr-for-docker-run it is 
 sufficient only to do it for stderr for me.
+See [https://alex-ber.medium.com/stdlogging-module-d5d69ff7103f] for details.
  
 #### Changed
 - `Doockerfiles` base-image. Now, you can transparentely switch betwee AMD64 to ARM 64 proccessor.
 - `cffi` dependency from 1.14.3 to 1.14.5.
 - `cryptography` dependency from 3.1.1 to 3.4.7.
```

### Comparing `alex_ber_utils-0.6.6b3/LICENSE.txt` & `alex_ber_utils-0.7.0/LICENSE.txt`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-Copyright (c) 2011, Donald Stufft
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-* Redistributions of source code must retain the above copyright notice,
-  this list of conditions and the following disclaimer.
-
-* Redistributions in binary form must reproduce the above copyright notice,
-  this list of conditions and the following disclaimer in the documentation
-  and/or other materials provided with the distribution.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
-ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
-WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED.
-IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT,
-INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT
-NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
-OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
-WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
-ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY
+Copyright (c) 2011, Donald Stufft
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+* Redistributions of source code must retain the above copyright notice,
+  this list of conditions and the following disclaimer.
+
+* Redistributions in binary form must reproduce the above copyright notice,
+  this list of conditions and the following disclaimer in the documentation
+  and/or other materials provided with the distribution.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
+ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
+WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED.
+IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT,
+INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT
+NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
+OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
+WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY
 OF SUCH DAMAGE.
```

### Comparing `alex_ber_utils-0.6.6b3/README.md` & `alex_ber_utils-0.7.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,146 +1,146 @@
-## AlexBerUtils
-
-AlexBerUtils is collection of the small utilities. See CHANGELOG.md for detail description.
-
-
-
-### Getting Help
-
-
-### QuickStart
-```bash
-python3 -m pip install -U alex-ber-utils
-```
-
-
-### Installing from Github
-
-```bash
-python3 -m pip install -U https://github.com/alex-ber/AlexBerUtils/archive/master.zip
-```
-Optionally installing tests requirements.
-
-```bash
-python3 -m pip install -U https://github.com/alex-ber/AlexBerUtils/archive/master.zip#egg=alex-ber-utils[tests]
-```
-
-Or explicitly:
-
-```bash
-wget https://github.com/alex-ber/AlexBerUtils/archive/master.zip -O master.zip; unzip master.zip; rm master.zip
-```
-And then installing from source (see below).
-
-
-### Installing from source
-```bash
-python3 -m pip install . # only installs "required"
-```
-```bash
-python3 -m pip install .[tests] # installs dependencies for tests
-```
-```bash
-python3 -m pip install .[md]   # installs multidispatcher (used in method_overloading_test.py)
-```
-```bash
-python3 -m pip install .[fabric]   # installs fabric (used in fabs.py)
-```
-```bash
-python3 -m pip install .[yml]   # installs Yml related dependencies 
-                                # (used in ymlparsers.py, init_app_conf.py, deploys.py;
-                                # optionally used in ymlparsers_extra.py, emails.py)
-```
-```bash
-python3 -m pip install .[env]   # installs pydotenv (optionally used in deploys.py and mains.py)
-```
-
-#### Alternatively you install install from requirements file:
-```bash
-python3 -m pip install -r requirements.txt # only installs "required"
-```
-```bash
-python3 -m pip install -r requirements-tests.txt # installs dependencies for tests
-```
-```bash
-python3 -m pip install -r requirements-md.txt   # installs multidispatcher (used in method_overloading_test.py)
-```
-```bash
-python3 -m pip install -r requirements-fabric.txt   # installs fabric (used in fabs.py)
-```
-```bash
-python3 -m pip install -r requirements-yml.txt   # installs Yml related dependencies 
-                                                 # (used in ymlparsers.py, init_app_conf.py, deploys.py;
-                                                 # optionally used in ymlparsers_extra.py, emails.py)
-```
-```bash
-python3 -m pip install -r requirements-env.txt   # installs pydotenv (optionally used in deploys.py)
-```
-
-### Using Docker
-`alexberkovich/AlexBerUtils:latest`  contains all `AlexBerUtils` dependencies.
-This Dockerfile is very simple, you can take relevant part for you and put them into your Dockerfile.
-
-##
-Alternatively, you can use it as base Docker image for your project and add/upgrade 
-another dependencies as you need.
-
-For example:
-
-```Dockerfile
-FROM alexberkovich/alex_ber_utils:latest
-
-COPY requirements.txt etc/requirements.txt
-
-RUN set -ex && \
-    #latest pip,setuptools,wheel
-    pip install --upgrade pip setuptools wheel && \
-    pip install alex_ber_utils 
-    pip install -r etc/requirements.txt 
-
-CMD ["/bin/sh"]
-#CMD tail -f /dev/null
-```
-
-where `requirements.txt` is requirements for your project.
-
-  
-
-##
-
-From the directory with setup.py
-```bash
-python3 setup.py test #run all tests
-```
-
-or
-
-```bash
-
-pytest
-```
-
-## Installing new version
-See https://docs.python.org/3.1/distutils/uploading.html 
-
-
-## Installing new version to venv
-```bash
-python38 -m pip uninstall --yes alex_ber_utils
-python38 setup.py clean sdist bdist_wheel
-python38 -m pip install --find-links=./dist alex_ber_utils==0.6.5
-```
-
-##Manual upload
-```bash
-#python setup.py clean sdist upload
-```
-
-
-## Requirements
-
-
-AlexBerUtils requires the following modules.
-
-* Python 3.6+
-
-* PyYAML==5.1
+## AlexBerUtils
+
+AlexBerUtils is collection of the small utilities. See CHANGELOG.md for detail description.
+
+
+
+### Getting Help
+
+
+### QuickStart
+```bash
+python3 -m pip install -U alex-ber-utils
+```
+
+
+### Installing from Github
+
+```bash
+python3 -m pip install -U https://github.com/alex-ber/AlexBerUtils/archive/master.zip
+```
+Optionally installing tests requirements.
+
+```bash
+python3 -m pip install -U https://github.com/alex-ber/AlexBerUtils/archive/master.zip#egg=alex-ber-utils[tests]
+```
+
+Or explicitly:
+
+```bash
+wget https://github.com/alex-ber/AlexBerUtils/archive/master.zip -O master.zip; unzip master.zip; rm master.zip
+```
+And then installing from source (see below).
+
+
+### Installing from source
+```bash
+python3 -m pip install . # only installs "required"
+```
+```bash
+python3 -m pip install .[tests] # installs dependencies for tests
+```
+```bash
+python3 -m pip install .[md]   # installs multidispatcher (used in method_overloading_test.py)
+```
+```bash
+python3 -m pip install .[fabric]   # installs fabric (used in fabs.py)
+```
+```bash
+python3 -m pip install .[yml]   # installs Yml related dependencies 
+                                # (used in ymlparsers.py, init_app_conf.py, deploys.py;
+                                # optionally used in ymlparsers_extra.py, emails.py)
+```
+```bash
+python3 -m pip install .[env]   # installs pydotenv (optionally used in deploys.py and mains.py)
+```
+
+#### Alternatively you install install from requirements file:
+```bash
+python3 -m pip install -r requirements.txt # only installs "required"
+```
+```bash
+python3 -m pip install -r requirements-tests.txt # installs dependencies for tests
+```
+```bash
+python3 -m pip install -r requirements-md.txt   # installs multidispatcher (used in method_overloading_test.py)
+```
+```bash
+python3 -m pip install -r requirements-fabric.txt   # installs fabric (used in fabs.py)
+```
+```bash
+python3 -m pip install -r requirements-yml.txt   # installs Yml related dependencies 
+                                                 # (used in ymlparsers.py, init_app_conf.py, deploys.py;
+                                                 # optionally used in ymlparsers_extra.py, emails.py)
+```
+```bash
+python3 -m pip install -r requirements-env.txt   # installs pydotenv (optionally used in deploys.py)
+```
+
+### Using Docker
+`alexberkovich/AlexBerUtils:latest`  contains all `AlexBerUtils` dependencies.
+This Dockerfile is very simple, you can take relevant part for you and put them into your Dockerfile.
+
+##
+Alternatively, you can use it as base Docker image for your project and add/upgrade 
+another dependencies as you need.
+
+For example:
+
+```Dockerfile
+FROM alexberkovich/alex_ber_utils:latest
+
+COPY requirements.txt etc/requirements.txt
+
+RUN set -ex && \
+    #latest pip,setuptools,wheel
+    pip install --upgrade pip setuptools wheel && \
+    pip install alex_ber_utils 
+    pip install -r etc/requirements.txt 
+
+CMD ["/bin/sh"]
+#CMD tail -f /dev/null
+```
+
+where `requirements.txt` is requirements for your project.
+
+  
+
+##
+
+From the directory with setup.py
+```bash
+python3 setup.py test #run all tests
+```
+
+or
+
+```bash
+
+pytest
+```
+
+## Installing new version
+See https://docs.python.org/3.1/distutils/uploading.html 
+
+
+## Installing new version to venv
+```bash
+python38 -m pip uninstall --yes alex_ber_utils
+python38 setup.py clean sdist bdist_wheel
+python38 -m pip install --find-links=./dist alex_ber_utils==0.6.5
+```
+
+##Manual upload
+```bash
+#python setup.py clean sdist upload
+```
+
+
+## Requirements
+
+
+AlexBerUtils requires the following modules.
+
+* Python 3.6+
+
+* PyYAML>=6.0.1
```

### Comparing `alex_ber_utils-0.6.6b3/alex_ber_utils.egg-info/SOURCES.txt` & `alex_ber_utils-0.7.0/alex_ber_utils.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 alexber/utils/processinvokes.py
 alexber/utils/props.py
 alexber/utils/setups.py
 alexber/utils/stdlogging.py
 alexber/utils/thread_locals.py
 alexber/utils/uuids.py
 alexber/utils/ymlparsers.py
+alexber/utils/data/__init__.py
 data/__init__.py
 tests/__init__.py
 tests/conftest.py
 tests/utils/__init__.py
 tests/utils/deploys_test.py
 tests/utils/emails_test.py
 tests/utils/enums_mixin_test.py
```

### Comparing `alex_ber_utils-0.6.6b3/alexber/utils/_ymlparsers_extra.py` & `alex_ber_utils-0.7.0/alexber/utils/_ymlparsers_extra.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,213 +1,213 @@
-"""
-This module adopts its behavior dependent on availability of Python packages.
-
-This module optionally depends on ymlparseser module.
-Method format_template() is used in emails module.
-
-Note: This module will work if you have only standard Python package. You just can't change delimiters values.
-Note: API and implementation of this module is unstable and can change without prior notice.
-"""
-
-import warnings
-
-def format_template(template, **kwargs):
-    """
-    This is main method of this module.
-    Note: API of this method is unstable and can change without prior notice.
-
-    Template is expected to be compatible with Jinja2 one.
-
-    Current implementation make delimiters compatible with str.format() and use it.
-
-
-    :param template: str, typically with {{my_variable}}
-    :param jinja2ctx:  Jinja2 Environment that is consulted what is delimiter for variable's names.
-                       if is not provided, HiYaPyCo.jinja2ctx is used. See ymlparsers.initConfig().
-                       if is not provided, than defaults are used (see jinja2.defaults).
-    :param jinja2Lock: Lock to be used to atomically get variable_start_string and variable_end_string from jinja2ctx.
-                       if is not provided, HiYaPyCo.jinja2Lock is used.. See ymlparsers.initConfig().
-    :return: fromated str
-    """
-    if template is None:
-        return None
-    s = _convert_template_to_string_format(template, **kwargs)
-    ret = s.format(template, **kwargs)
-    return ret
-
-
-try:
-    with warnings.catch_warnings():
-        warnings.filterwarnings("ignore", message=r'.*?yaml*?', module=r'.*?ymlparsers.*?')
-    from . ymlparsers import HiYaPyCo
-    _isHiYaPyCoAvailable = True
-except ImportError:
-    _isHiYaPyCoAvailable = False
-
-_a1 = None
-_a2 = None
-try:
-    try:
-        from jinja2.defaults import VARIABLE_START_STRING as _a1, VARIABLE_END_STRING as _a2
-        _isJinja2DefaultAvailable = True
-    except ImportError:
-        try:
-            from jinja2.environment import VARIABLE_START_STRING as _a1, VARIABLE_END_STRING as _a2
-            _isJinja2DefaultAvailable = True
-        except ImportError:
-            _isJinja2DefaultAvailable = False
-finally:
-    del _a1
-    del _a2
-
-_VARIABLE_START_STRING = None
-_VARIABLE_END_STRING = None
-
-
-def _init_globals():
-    """
-    This method is called during module import.
-    This method is idempotent.
-    """
-    global _VARIABLE_START_STRING, _VARIABLE_END_STRING
-
-    if _isJinja2DefaultAvailable:
-        p1 = None
-        p2 = None
-        try:
-            from jinja2.defaults import VARIABLE_START_STRING as p1, VARIABLE_END_STRING as p2
-        except ImportError:
-            from jinja2.environment import VARIABLE_START_STRING as p1, VARIABLE_END_STRING as p2
-
-        if p1 is None or p2 is None:
-            raise ImportError('VARIABLE_START_STRING or VARIABLE_END_STRING are not defined')
-
-        _VARIABLE_START_STRING = p1
-        _VARIABLE_END_STRING = p2
-    else:
-        _VARIABLE_START_STRING = '{{'
-        _VARIABLE_END_STRING = '}}'
-
-
-_init_globals()
-
-def _normalize_var_name(text, start_del, end_del):
-    """
-    Search&replace all pairs of (start_del, end_del) with pairs of ({, }).
-
-    :param text: str to normalize
-    :param start_del: delimiter that indicates start of variable name, typically {{
-    :param end_del: delimiter that indicates end of variable name, typically }}
-    :return:
-    """
-
-    if start_del is None or start_del not in text or end_del not in text:
-        return text
-
-    first_ind = 0
-    len_end_del = len(end_del)
-
-    while True:
-        first_ind = text.find(start_del, first_ind)
-        if first_ind < 0:
-            break
-        last_ind =  text.find(end_del, first_ind)
-        var = text[first_ind:last_ind+len_end_del]
-        var = var.replace('.', '_')
-        #text[first_ind:last_ind] = var
-        text = text[:first_ind]+var+text[last_ind+len_end_del:]
-        first_ind = last_ind+len_end_del
-    return text
-
-
-def __convert_template_to_string_format(template, **kwargs):
-    """
-    This is utility method that make template usable with string format.
-
-
-    :param template: str, typically with {{my_variable}}
-    :param default_start: Typically {{ but can be any other delimiter that points to start of the token variable.
-    :param default_end:   Typically }} but can be any other delimiter that points to end of the token variable.
-    :return: template: str with {my_variable}
-    """
-    if template is None:
-        return None
-
-    default_start = kwargs.pop('default_start', None)
-    default_end = kwargs.pop('default_end', None)
-
-    template = _normalize_var_name(template, default_start, default_end)
-
-    ret = template.replace(f'{default_start} ', f'{default_start}') \
-        .replace(f'{default_start}', '{') \
-        .replace(f' {default_end}', f'{default_end}') \
-        .replace(f'{default_end}', '}')
-    return ret
-
-def _convert_template_to_string_format(template, **kwargs):
-    """
-    This is utility method that make template usable with string format.
-
-    if both jinja2ctx and jinja2Lock are provided, than they are used to determine various delimiters
-    (jinja2Lock is used to read the values from jinja2ctx atomically).
-
-    if both jinja2ctx and jinja2Lock are not provided, than
-        If ymlparsers is usable (it's 3rd party dependencies are available, one if each is jinja2)
-        than it's jinja2ctx (Jinja2's Environment) will be consulted for the various delimiters.
-        Otherwise, if jinja2 is available than we will use it's defaults for constricting Jinja2's Environment
-        for the various delimiters.
-        Otherwise, some sensible defaults (default values from some version of Jinja2) will be used.
-
-    You can't provide jinja2Lock without providing jinja2ctx (you can't provide your jinja2Lock for HiYaPyCo.jinja2ctx).
-
-    You can provide jinja2ctx without jinja2Lock. Than you will give up atomicity for determining various delimiters.
-
-    :param template: str, typically with {{my_variable}}
-    :param jinja2ctx:  Jinja2 Environment that is consulted what is delimiter for variable's names.
-                       if is not provided, HiYaPyCo.jinja2ctx is used. See ymlparsers.initConfig().
-                       if is not provided, than defaults are used (see jinja2.defaults).
-    :param jinja2Lock: Lock to be used to atomically get variable_start_string and variable_end_string from jinja2ctx.
-                       if is not provided, HiYaPyCo.jinja2Lock is used.. See ymlparsers.initConfig().
-    :return: template: str with {my_variable}
-    """
-
-    if template is None:
-        return None
-
-    jinja2ctx = kwargs.pop('jinja2ctx', None)
-    jinja2Lock = kwargs.pop('jinja2Lock', None)
-
-    if _isHiYaPyCoAvailable and jinja2ctx is None and jinja2Lock is not None:
-        raise ValueError("You can't provide your jinja2Lock for HiYaPyCo.jinja2ctx")
-
-    if _isHiYaPyCoAvailable and jinja2ctx is None:
-        jinja2ctx  = HiYaPyCo.jinja2ctx
-        jinja2Lock = HiYaPyCo.jinja2Lock    #we should use HiYaPyCo.jinja2Lock for HiYaPyCo.jinja2ctx
-
-    #default_start, default_end
-    if jinja2ctx is None:
-        if jinja2Lock is None:
-            default_start = _VARIABLE_START_STRING
-            default_end = _VARIABLE_END_STRING
-        else:
-            with jinja2Lock:
-                default_start = _VARIABLE_START_STRING
-                default_end = _VARIABLE_END_STRING
-
-    else:
-        if _isHiYaPyCoAvailable and HiYaPyCo.jinja2ctx is not None and HiYaPyCo.jinja2Lock is None:
-            raise ValueError('HiYaPyCo.jinja2ctx is not None, but HiYaPyCo.jinja2Lock is None')
-
-        if jinja2Lock is None:
-            # jinja2ctx was provided, but jinja2Lock wasn't, it is ok
-            # (maybe jinja2ctx is local variable?)
-            default_start = jinja2ctx.variable_start_string
-            default_end = jinja2ctx.variable_end_string
-        else:
-            with jinja2Lock:
-                default_start = jinja2ctx.variable_start_string
-                default_end = jinja2ctx.variable_end_string
-
-    ret = __convert_template_to_string_format(template, default_start=default_start, default_end=default_end)
-    return ret
-
-
+"""
+This module adopts its behavior dependent on availability of Python packages.
+
+This module optionally depends on ymlparseser module.
+Method format_template() is used in emails module.
+
+Note: This module will work if you have only standard Python package. You just can't change delimiters values.
+Note: API and implementation of this module is unstable and can change without prior notice.
+"""
+
+import warnings
+
+def format_template(template, **kwargs):
+    """
+    This is main method of this module.
+    Note: API of this method is unstable and can change without prior notice.
+
+    Template is expected to be compatible with Jinja2 one.
+
+    Current implementation make delimiters compatible with str.format() and use it.
+
+
+    :param template: str, typically with {{my_variable}}
+    :param jinja2ctx:  Jinja2 Environment that is consulted what is delimiter for variable's names.
+                       if is not provided, HiYaPyCo.jinja2ctx is used. See ymlparsers.initConfig().
+                       if is not provided, than defaults are used (see jinja2.defaults).
+    :param jinja2Lock: Lock to be used to atomically get variable_start_string and variable_end_string from jinja2ctx.
+                       if is not provided, HiYaPyCo.jinja2Lock is used.. See ymlparsers.initConfig().
+    :return: fromated str
+    """
+    if template is None:
+        return None
+    s = _convert_template_to_string_format(template, **kwargs)
+    ret = s.format(template, **kwargs)
+    return ret
+
+
+try:
+    with warnings.catch_warnings():
+        warnings.filterwarnings("ignore", message=r'.*?yaml*?', module=r'.*?ymlparsers.*?')
+    from . ymlparsers import HiYaPyCo
+    _isHiYaPyCoAvailable = True
+except ImportError:
+    _isHiYaPyCoAvailable = False
+
+_a1 = None
+_a2 = None
+try:
+    try:
+        from jinja2.defaults import VARIABLE_START_STRING as _a1, VARIABLE_END_STRING as _a2
+        _isJinja2DefaultAvailable = True
+    except ImportError:
+        try:
+            from jinja2.environment import VARIABLE_START_STRING as _a1, VARIABLE_END_STRING as _a2
+            _isJinja2DefaultAvailable = True
+        except ImportError:
+            _isJinja2DefaultAvailable = False
+finally:
+    del _a1
+    del _a2
+
+_VARIABLE_START_STRING = None
+_VARIABLE_END_STRING = None
+
+
+def _init_globals():
+    """
+    This method is called during module import.
+    This method is idempotent.
+    """
+    global _VARIABLE_START_STRING, _VARIABLE_END_STRING
+
+    if _isJinja2DefaultAvailable:
+        p1 = None
+        p2 = None
+        try:
+            from jinja2.defaults import VARIABLE_START_STRING as p1, VARIABLE_END_STRING as p2
+        except ImportError:
+            from jinja2.environment import VARIABLE_START_STRING as p1, VARIABLE_END_STRING as p2
+
+        if p1 is None or p2 is None:
+            raise ImportError('VARIABLE_START_STRING or VARIABLE_END_STRING are not defined')
+
+        _VARIABLE_START_STRING = p1
+        _VARIABLE_END_STRING = p2
+    else:
+        _VARIABLE_START_STRING = '{{'
+        _VARIABLE_END_STRING = '}}'
+
+
+_init_globals()
+
+def _normalize_var_name(text, start_del, end_del):
+    """
+    Search&replace all pairs of (start_del, end_del) with pairs of ({, }).
+
+    :param text: str to normalize
+    :param start_del: delimiter that indicates start of variable name, typically {{
+    :param end_del: delimiter that indicates end of variable name, typically }}
+    :return:
+    """
+
+    if start_del is None or start_del not in text or end_del not in text:
+        return text
+
+    first_ind = 0
+    len_end_del = len(end_del)
+
+    while True:
+        first_ind = text.find(start_del, first_ind)
+        if first_ind < 0:
+            break
+        last_ind =  text.find(end_del, first_ind)
+        var = text[first_ind:last_ind+len_end_del]
+        var = var.replace('.', '_')
+        #text[first_ind:last_ind] = var
+        text = text[:first_ind]+var+text[last_ind+len_end_del:]
+        first_ind = last_ind+len_end_del
+    return text
+
+
+def __convert_template_to_string_format(template, **kwargs):
+    """
+    This is utility method that make template usable with string format.
+
+
+    :param template: str, typically with {{my_variable}}
+    :param default_start: Typically {{ but can be any other delimiter that points to start of the token variable.
+    :param default_end:   Typically }} but can be any other delimiter that points to end of the token variable.
+    :return: template: str with {my_variable}
+    """
+    if template is None:
+        return None
+
+    default_start = kwargs.pop('default_start', None)
+    default_end = kwargs.pop('default_end', None)
+
+    template = _normalize_var_name(template, default_start, default_end)
+
+    ret = template.replace(f'{default_start} ', f'{default_start}') \
+        .replace(f'{default_start}', '{') \
+        .replace(f' {default_end}', f'{default_end}') \
+        .replace(f'{default_end}', '}')
+    return ret
+
+def _convert_template_to_string_format(template, **kwargs):
+    """
+    This is utility method that make template usable with string format.
+
+    if both jinja2ctx and jinja2Lock are provided, than they are used to determine various delimiters
+    (jinja2Lock is used to read the values from jinja2ctx atomically).
+
+    if both jinja2ctx and jinja2Lock are not provided, than
+        If ymlparsers is usable (it's 3rd party dependencies are available, one if each is jinja2)
+        than it's jinja2ctx (Jinja2's Environment) will be consulted for the various delimiters.
+        Otherwise, if jinja2 is available than we will use it's defaults for constricting Jinja2's Environment
+        for the various delimiters.
+        Otherwise, some sensible defaults (default values from some version of Jinja2) will be used.
+
+    You can't provide jinja2Lock without providing jinja2ctx (you can't provide your jinja2Lock for HiYaPyCo.jinja2ctx).
+
+    You can provide jinja2ctx without jinja2Lock. Than you will give up atomicity for determining various delimiters.
+
+    :param template: str, typically with {{my_variable}}
+    :param jinja2ctx:  Jinja2 Environment that is consulted what is delimiter for variable's names.
+                       if is not provided, HiYaPyCo.jinja2ctx is used. See ymlparsers.initConfig().
+                       if is not provided, than defaults are used (see jinja2.defaults).
+    :param jinja2Lock: Lock to be used to atomically get variable_start_string and variable_end_string from jinja2ctx.
+                       if is not provided, HiYaPyCo.jinja2Lock is used.. See ymlparsers.initConfig().
+    :return: template: str with {my_variable}
+    """
+
+    if template is None:
+        return None
+
+    jinja2ctx = kwargs.pop('jinja2ctx', None)
+    jinja2Lock = kwargs.pop('jinja2Lock', None)
+
+    if _isHiYaPyCoAvailable and jinja2ctx is None and jinja2Lock is not None:
+        raise ValueError("You can't provide your jinja2Lock for HiYaPyCo.jinja2ctx")
+
+    if _isHiYaPyCoAvailable and jinja2ctx is None:
+        jinja2ctx  = HiYaPyCo.jinja2ctx
+        jinja2Lock = HiYaPyCo.jinja2Lock    #we should use HiYaPyCo.jinja2Lock for HiYaPyCo.jinja2ctx
+
+    #default_start, default_end
+    if jinja2ctx is None:
+        if jinja2Lock is None:
+            default_start = _VARIABLE_START_STRING
+            default_end = _VARIABLE_END_STRING
+        else:
+            with jinja2Lock:
+                default_start = _VARIABLE_START_STRING
+                default_end = _VARIABLE_END_STRING
+
+    else:
+        if _isHiYaPyCoAvailable and HiYaPyCo.jinja2ctx is not None and HiYaPyCo.jinja2Lock is None:
+            raise ValueError('HiYaPyCo.jinja2ctx is not None, but HiYaPyCo.jinja2Lock is None')
+
+        if jinja2Lock is None:
+            # jinja2ctx was provided, but jinja2Lock wasn't, it is ok
+            # (maybe jinja2ctx is local variable?)
+            default_start = jinja2ctx.variable_start_string
+            default_end = jinja2ctx.variable_end_string
+        else:
+            with jinja2Lock:
+                default_start = jinja2ctx.variable_start_string
+                default_end = jinja2ctx.variable_end_string
+
+    ret = __convert_template_to_string_format(template, default_start=default_start, default_end=default_end)
+    return ret
+
+
```

### Comparing `alex_ber_utils-0.6.6b3/alexber/utils/deploys.py` & `alex_ber_utils-0.7.0/alexber/utils/deploys.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,109 +1,109 @@
-"""
-This module is usable in your deployment script. See also `fabs` module.
-
-See here https://medium.com/analytics-vidhya/my-ymlparsers-module-88221edf16a6 for documentation.
-
-This module depends on some 3-rd party dependencies, in order to use it, you should have installed first. To do it
-run `python3 -m pip install alex-ber-utils[yml]`.
-"""
-
-from collections import OrderedDict
-from pathlib import Path
-from collections import deque
-try:
-    import alexber.utils.ymlparsers as ymlparsers
-except ImportError:
-    pass
-
-from .init_app_conf import merge_list_value_in_dicts, conf
-from .parsers import is_empty, parse_sys_args
-
-
-def split_path(filename, split_dirname):
-    """
-    Split filename in 2 part parts by split_dirname.
-    first_part will ends with split_dirname.
-    second_part will start immediately after split_dirname.
-
-    if split_dirname is not in filename or split_dirname is None, the behaviour is undefined.
-    if split_dirname exists twice in the path, the last one will be used for splitting.
-
-    :param filename: path to filename, can be relative or absolute.
-    :param split_dirname: directory name in filename that will be used to split the path
-    :return: (first_part, second_part) - such that first_part+second_part is absolute path.
-
-    """
-    if split_dirname is None:
-        raise FileNotFoundError("can't split on None")
-
-    parts = Path(filename).parts
-    split_dirname = str(split_dirname)
-
-
-    if split_dirname not in parts:
-        raise FileNotFoundError(f"{split_dirname} is not found in {filename}")
-    length = len(parts)
-
-    use = False
-    second_parts = deque(maxlen=length)
-    first_parts = deque(maxlen=length)
-    for part in reversed(parts):
-        if part == split_dirname:
-            use = True
-        if use:
-            first_parts.appendleft(part)
-        else:
-            second_parts.appendleft(part)
-
-
-    return Path(*first_parts), Path(*second_parts)
-
-def add_to_zip_copy_function(split_dirname=None, zf=None):
-    """
-    Factory method that returns closure that can be used as copy_function param in shutil.copytree()
-
-    :param split_dirname: path from this directory and below will be used in archive.
-    :param zf: zipfile.ZipFile
-    :return:
-    """
-    def add_to_zip_file(src,dst):
-        """
-        Closure that can be used as copy_function param in shutil.copytree()
-        shutil.copytree() is used to add from src to archive with entries evaluted according to split_dirname.
-
-        :param src: soource file to use in entry in archive
-        :param dst: ignored, see split_dirname in enclused function
-        :return:
-        """
-        _, last_parts = split_path(src, split_dirname)
-        dest_path = Path(split_dirname) / last_parts
-        zf.write(str(src), str(dest_path))
-    return add_to_zip_file
-
-def load_config(argumentParser=None, args=None):
-    """
-    Simplified method for parsing yml configuration file with optionally overrided profiles only.
-    See alexber.utils.init_app_conf.parse_config() for another variant.
-
-    :param argumentParser with instruction how to interpret args. If None, the default one will be instantiated.
-    :param args: if not None will be used instead of sys.argv
-    :return:
-    """
-    if ymlparsers.HiYaPyCo.jinja2ctx is None:
-        raise ValueError("ymlparsers.HiYaPyCo.jinja2ctx can't be None")
-
-    params, sys_d = parse_sys_args(argumentParser, args)
-    config_file = params.config_file
-    full_path = Path(config_file).resolve()  # relative to cwd
-
-    with ymlparsers.DisableVarSubst():
-        default_d = ymlparsers.load([str(full_path)])
-
-    profiles = merge_list_value_in_dicts(sys_d, default_d, conf.GENERAL_KEY, conf.PROFILES_KEY)
-    b = is_empty(profiles)
-    if not b:
-        # merge to default_d
-        general_d = default_d.setdefault(conf.GENERAL_KEY, OrderedDict())
-        general_d[conf.PROFILES_KEY] = profiles
-        return full_path, default_d
-
+"""
+This module is usable in your deployment script. See also `fabs` module.
+
+See here https://medium.com/analytics-vidhya/my-ymlparsers-module-88221edf16a6 for documentation.
+
+This module depends on some 3-rd party dependencies, in order to use it, you should have installed first. To do it
+run `python3 -m pip install alex-ber-utils[yml]`.
+"""
+
+from collections import OrderedDict
+from pathlib import Path
+from collections import deque
+try:
+    import alexber.utils.ymlparsers as ymlparsers
+except ImportError:
+    pass
+
+from .init_app_conf import merge_list_value_in_dicts, conf
+from .parsers import is_empty, parse_sys_args
+
+
+def split_path(filename, split_dirname):
+    """
+    Split filename in 2 part parts by split_dirname.
+    first_part will ends with split_dirname.
+    second_part will start immediately after split_dirname.
+
+    if split_dirname is not in filename or split_dirname is None, the behaviour is undefined.
+    if split_dirname exists twice in the path, the last one will be used for splitting.
+
+    :param filename: path to filename, can be relative or absolute.
+    :param split_dirname: directory name in filename that will be used to split the path
+    :return: (first_part, second_part) - such that first_part+second_part is absolute path.
+
+    """
+    if split_dirname is None:
+        raise FileNotFoundError("can't split on None")
+
+    parts = Path(filename).parts
+    split_dirname = str(split_dirname)
+
+
+    if split_dirname not in parts:
+        raise FileNotFoundError(f"{split_dirname} is not found in {filename}")
+    length = len(parts)
+
+    use = False
+    second_parts = deque(maxlen=length)
+    first_parts = deque(maxlen=length)
+    for part in reversed(parts):
+        if part == split_dirname:
+            use = True
+        if use:
+            first_parts.appendleft(part)
+        else:
+            second_parts.appendleft(part)
+
+
+    return Path(*first_parts), Path(*second_parts)
+
+def add_to_zip_copy_function(split_dirname=None, zf=None):
+    """
+    Factory method that returns closure that can be used as copy_function param in shutil.copytree()
+
+    :param split_dirname: path from this directory and below will be used in archive.
+    :param zf: zipfile.ZipFile
+    :return:
+    """
+    def add_to_zip_file(src,dst):
+        """
+        Closure that can be used as copy_function param in shutil.copytree()
+        shutil.copytree() is used to add from src to archive with entries evaluted according to split_dirname.
+
+        :param src: soource file to use in entry in archive
+        :param dst: ignored, see split_dirname in enclused function
+        :return:
+        """
+        _, last_parts = split_path(src, split_dirname)
+        dest_path = Path(split_dirname) / last_parts
+        zf.write(str(src), str(dest_path))
+    return add_to_zip_file
+
+def load_config(argumentParser=None, args=None):
+    """
+    Simplified method for parsing yml configuration file with optionally overrided profiles only.
+    See alexber.utils.init_app_conf.parse_config() for another variant.
+
+    :param argumentParser with instruction how to interpret args. If None, the default one will be instantiated.
+    :param args: if not None will be used instead of sys.argv
+    :return:
+    """
+    if ymlparsers.HiYaPyCo.jinja2ctx is None:
+        raise ValueError("ymlparsers.HiYaPyCo.jinja2ctx can't be None")
+
+    params, sys_d = parse_sys_args(argumentParser, args)
+    config_file = params.config_file
+    full_path = Path(config_file).resolve()  # relative to cwd
+
+    with ymlparsers.DisableVarSubst():
+        default_d = ymlparsers.load([str(full_path)])
+
+    profiles = merge_list_value_in_dicts(sys_d, default_d, conf.GENERAL_KEY, conf.PROFILES_KEY)
+    b = is_empty(profiles)
+    if not b:
+        # merge to default_d
+        general_d = default_d.setdefault(conf.GENERAL_KEY, OrderedDict())
+        general_d[conf.PROFILES_KEY] = profiles
+        return full_path, default_d
+
```

### Comparing `alex_ber_utils-0.6.6b3/alexber/utils/enums.py` & `alex_ber_utils-0.7.0/alexber/utils/enums.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-
-
-from enum import *
-import enum #don't delete
-import logging
-logger = logging.getLogger(__name__)
-
-
-_orig_enum_new = Enum.__new__
-
-#we want to use None to indicate missing Enumm, but
-#https://bugs.python.org/issue34536 prohibts using None in _missing_() @classmethod
-#this fix re-enable it
-def _fixed_new_enum(cls, value):
-    try:
-        return _orig_enum_new(cls, value)
-    except ValueError as e:
-        msg = str(e)
-        if 'is not a valid' in msg:
-            return None
-        raise e
-
-Enum.__new__ = _fixed_new_enum
-
-class StrAsReprMixinEnum(Enum):
-    '''
-    This is Enum Mixin that has __str__() equal to __repr__().
-    '''
-    def __str__(self):
-        return self.__repr__()
-
-
-class AutoNameMixinEnum(Enum):
-    '''
-    This is Enum Mixin that generate value equal to the name.
-    '''
-    def _generate_next_value_(name, start, count, last_values):
-        return name
-
-
-
-class MissingNoneMixinEnum(Enum):
-    '''
-    This is Enum Mixin will return None if value will not be found.
-    '''
-
-    @classmethod
-    def _missing_(cls, value):
-        # raise ValueError("%r is not a valid %s" % (value, cls.__name__))
-        return None
-
-
-class LookUpMixinEnum(StrAsReprMixinEnum, MissingNoneMixinEnum):
-    '''
-    This is Enim Mixin that is designed to be used for lookup by value.
-    If lookup fail, None will be return.
-    Also, __str__() will return the same value as __repr__()
-    '''
-    pass
-
+
+
+from enum import *
+import enum #don't delete
+import logging
+logger = logging.getLogger(__name__)
+
+
+_orig_enum_new = Enum.__new__
+
+#we want to use None to indicate missing Enumm, but
+#https://bugs.python.org/issue34536 prohibts using None in _missing_() @classmethod
+#this fix re-enable it
+def _fixed_new_enum(cls, value):
+    try:
+        return _orig_enum_new(cls, value)
+    except ValueError as e:
+        msg = str(e)
+        if 'is not a valid' in msg:
+            return None
+        raise e
+
+Enum.__new__ = _fixed_new_enum
+
+class StrAsReprMixinEnum(Enum):
+    '''
+    This is Enum Mixin that has __str__() equal to __repr__().
+    '''
+    def __str__(self):
+        return self.__repr__()
+
+
+class AutoNameMixinEnum(Enum):
+    '''
+    This is Enum Mixin that generate value equal to the name.
+    '''
+    def _generate_next_value_(name, start, count, last_values):
+        return name
+
+
+
+class MissingNoneMixinEnum(Enum):
+    '''
+    This is Enum Mixin will return None if value will not be found.
+    '''
+
+    @classmethod
+    def _missing_(cls, value):
+        # raise ValueError("%r is not a valid %s" % (value, cls.__name__))
+        return None
+
+
+class LookUpMixinEnum(StrAsReprMixinEnum, MissingNoneMixinEnum):
+    '''
+    This is Enim Mixin that is designed to be used for lookup by value.
+    If lookup fail, None will be return.
+    Also, __str__() will return the same value as __repr__()
+    '''
+    pass
+
```

### Comparing `alex_ber_utils-0.6.6b3/alexber/utils/fabs.py` & `alex_ber_utils-0.7.0/alexber/utils/fabs.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-"""
-This module is usable in your deployment script. See also `deploys` module.
-
-This module depends on some 3-rd party dependencies, in order to use it, you should have installed first. To do it
-run `python3 -m pip install alex-ber-utils[fabric]`.
-
-"""
-
-
-import logging
-logger = logging.getLogger(__name__)
-from pathlib import PurePath
-
-try:
-    from fabric import Connection
-except ImportError:
-    import warnings
-
-    warning = (
-        "You appear to be missing some optional dependencies;"
-        "please 'python3 -m pip install alex-ber-utils[fabric]'."
-    )
-    warnings.warn(warning, ImportWarning)
-    raise
-
-
-
-
-def _cp(self, remote_dir, local_file):
-    """
-    This is helper method that cp single file from local machine to remote (Posix) machine.
-    If file exists on the remote machine, it will be overwritten.
-
-    :param remote_dir: can be str or Path
-    :param local_file:  can be str or Path
-    """
-    remote_dir_path = PurePath(remote_dir)
-    self.run(f'mkdir -p {remote_dir_path.as_posix()}')
-    #self.run('ls -l {}'.format(remote_dir))
-    full_local_dir = PurePath(local_file)
-    file_name = full_local_dir.name
-    local_dir = full_local_dir.parent
-
-    full_remote_dir = remote_dir_path / file_name
-    self.run(f'rm -fr {full_remote_dir.as_posix()}')
-    full_local_dir = PurePath(local_dir, file_name)
-    result = self.put(local=full_local_dir.as_posix(), remote=remote_dir_path.as_posix())
-    logger.info(f"Uploaded {result.local} to {result.remote}")
-
+"""
+This module is usable in your deployment script. See also `deploys` module.
+
+This module depends on some 3-rd party dependencies, in order to use it, you should have installed first. To do it
+run `python3 -m pip install alex-ber-utils[fabric]`.
+
+"""
+
+
+import logging
+logger = logging.getLogger(__name__)
+from pathlib import PurePath
+
+try:
+    from fabric import Connection
+except ImportError:
+    import warnings
+
+    warning = (
+        "You appear to be missing some optional dependencies;"
+        "please 'python3 -m pip install alex-ber-utils[fabric]'."
+    )
+    warnings.warn(warning, ImportWarning)
+    raise
+
+
+
+
+def _cp(self, remote_dir, local_file):
+    """
+    This is helper method that cp single file from local machine to remote (Posix) machine.
+    If file exists on the remote machine, it will be overwritten.
+
+    :param remote_dir: can be str or Path
+    :param local_file:  can be str or Path
+    """
+    remote_dir_path = PurePath(remote_dir)
+    self.run(f'mkdir -p {remote_dir_path.as_posix()}')
+    #self.run('ls -l {}'.format(remote_dir))
+    full_local_dir = PurePath(local_file)
+    file_name = full_local_dir.name
+    local_dir = full_local_dir.parent
+
+    full_remote_dir = remote_dir_path / file_name
+    self.run(f'rm -fr {full_remote_dir.as_posix()}')
+    full_local_dir = PurePath(local_dir, file_name)
+    result = self.put(local=full_local_dir.as_posix(), remote=remote_dir_path.as_posix())
+    logger.info(f"Uploaded {result.local} to {result.remote}")
+
 Connection.cp = _cp
```

### Comparing `alex_ber_utils-0.6.6b3/alexber/utils/importer.py` & `alex_ber_utils-0.7.0/alexber/utils/importer.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,106 +1,106 @@
-"""
-See here https://medium.com/analytics-vidhya/how-to-write-easily-customizable-code-8b00b43406b2 for documentation.
-"""
-import importlib
-import logging
-import inspect
-import pkgutil
-
-logger = logging.getLogger(__name__)
-
-
-
-
-#adopted from scrapy
-def _walk_modules(path):
-    """
-    Loads a module and all its submodules from the given module path and
-    returns them. If *any* module throws an exception while importing, that
-    exception is thrown back.
-    """
-
-    # Support for namespace packages is added. See PEP 420.
-    # Namespace packages are a mechanism for splitting a single Python package across multiple directories on disk.
-    # When interpreted encounter with non-empty __path__ attribute it adds modules found in those locations
-    # to the current package.
-
-    mods = []
-    mod = importlib.import_module(path)
-    mods.append(mod)
-    if hasattr(mod, '__path__'):
-        for _, subpath, ispkg in pkgutil.iter_modules(mod.__path__):
-            fullpath = path + '.' + subpath
-            if ispkg:
-                mods += _walk_modules(fullpath)
-            else:
-                submod = importlib.import_module(fullpath)
-                mods.append(submod)
-    return mods
-
-
-#adopted from mock.mock._dot_lookup
-def _dot_lookup(thing, comp, import_path):
-    '''
-    Recursively import packages (if needed) by dotes.
-    '''
-    try:
-        return getattr(thing, comp)
-    except AttributeError:
-        importlib.import_module(import_path)
-        _walk_modules(import_path)
-        return getattr(thing, comp)
-
-#adopted from mock.mock._importer
-def importer(target):
-    '''
-    Convert str to Python construct that target is represented.
-    This method will recursively import packages (if needed)
-    Following dot notation from left to right. If the component
-    exists in packagage (is defined and imported) it will be used,
-    otherwrise, it will be imported.
-
-    This method supports PEP 420 (implicit Namespace Packages).
-
-    Note: only compile-time construct is supported.
-    Note: no instances will be returned from here, only classes.
-
-    :param target: str to lookup
-    :return: function/module/class, etc
-    '''
-
-    components = target.split('.')
-    import_path = components.pop(0)
-    thing = importlib.import_module(import_path)
-    _walk_modules(import_path)
-
-    for comp in components:
-        import_path += f".{comp}"
-        thing = _dot_lookup(thing, comp, import_path)
-    return thing
-
-
-
-def new_instance(target, *args, **kwargs):
-    '''
-    Convert str to Python construct that target is represented.
-    This method will recursively import packages (if needed)
-    Following dot notation from left to right. If the component
-    exists in package (is defined and imported) it will be used,
-    otherwrise, it will be imported.
-
-    If target doesn't represent the class, it will be returned as is.
-    If target is the class, instance of it will be created,
-    args and kwargs will be passed in to appropriate
-    __new__() / __init__() / __init_subclass__() methods.
-
-
-    :param target:
-    :param args:   - position args  for c-tor
-    :param kwargs: - key-value args for c-tor
-    :return:
-    '''
-    thing = importer(target)
-    ret = thing
-    if inspect.isclass(thing):
-        ret = thing(*args, **kwargs)
+"""
+See here https://medium.com/analytics-vidhya/how-to-write-easily-customizable-code-8b00b43406b2 for documentation.
+"""
+import importlib
+import logging
+import inspect
+import pkgutil
+
+logger = logging.getLogger(__name__)
+
+
+
+
+#adopted from scrapy
+def _walk_modules(path):
+    """
+    Loads a module and all its submodules from the given module path and
+    returns them. If *any* module throws an exception while importing, that
+    exception is thrown back.
+    """
+
+    # Support for namespace packages is added. See PEP 420.
+    # Namespace packages are a mechanism for splitting a single Python package across multiple directories on disk.
+    # When interpreted encounter with non-empty __path__ attribute it adds modules found in those locations
+    # to the current package.
+
+    mods = []
+    mod = importlib.import_module(path)
+    mods.append(mod)
+    if hasattr(mod, '__path__'):
+        for _, subpath, ispkg in pkgutil.iter_modules(mod.__path__):
+            fullpath = path + '.' + subpath
+            if ispkg:
+                mods += _walk_modules(fullpath)
+            else:
+                submod = importlib.import_module(fullpath)
+                mods.append(submod)
+    return mods
+
+
+#adopted from mock.mock._dot_lookup
+def _dot_lookup(thing, comp, import_path):
+    '''
+    Recursively import packages (if needed) by dotes.
+    '''
+    try:
+        return getattr(thing, comp)
+    except AttributeError:
+        importlib.import_module(import_path)
+        _walk_modules(import_path)
+        return getattr(thing, comp)
+
+#adopted from mock.mock._importer
+def importer(target):
+    '''
+    Convert str to Python construct that target is represented.
+    This method will recursively import packages (if needed)
+    Following dot notation from left to right. If the component
+    exists in packagage (is defined and imported) it will be used,
+    otherwrise, it will be imported.
+
+    This method supports PEP 420 (implicit Namespace Packages).
+
+    Note: only compile-time construct is supported.
+    Note: no instances will be returned from here, only classes.
+
+    :param target: str to lookup
+    :return: function/module/class, etc
+    '''
+
+    components = target.split('.')
+    import_path = components.pop(0)
+    thing = importlib.import_module(import_path)
+    _walk_modules(import_path)
+
+    for comp in components:
+        import_path += f".{comp}"
+        thing = _dot_lookup(thing, comp, import_path)
+    return thing
+
+
+
+def new_instance(target, *args, **kwargs):
+    '''
+    Convert str to Python construct that target is represented.
+    This method will recursively import packages (if needed)
+    Following dot notation from left to right. If the component
+    exists in package (is defined and imported) it will be used,
+    otherwrise, it will be imported.
+
+    If target doesn't represent the class, it will be returned as is.
+    If target is the class, instance of it will be created,
+    args and kwargs will be passed in to appropriate
+    __new__() / __init__() / __init_subclass__() methods.
+
+
+    :param target:
+    :param args:   - position args  for c-tor
+    :param kwargs: - key-value args for c-tor
+    :return:
+    '''
+    thing = importer(target)
+    ret = thing
+    if inspect.isclass(thing):
+        ret = thing(*args, **kwargs)
     return ret
```

### Comparing `alex_ber_utils-0.6.6b3/alexber/utils/init_app_conf.py` & `alex_ber_utils-0.7.0/alexber/utils/init_app_conf.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,494 +1,494 @@
-"""
-`ymlparsers` and `parser` modules serves as Low-Level API for this module.
-
-You may need to install some 3-rd party dependencies, in order to use it, you should have installed first. To do it
-run `python3 -m pip install alex-ber-utils[yml]` in order to use it.
-
-See https://medium.com/analytics-vidhya/my-major-init-app-conf-module-1a5d9fb3998c for documentation.
-"""
-import logging
-logger = logging.getLogger(__name__)
-
-from collections import OrderedDict, deque
-from pathlib import Path
-import io as _io
-from alexber.utils.parsers import is_empty, safe_eval as _convert, parse_boolean, ArgumentParser, \
-    parse_sys_args as uparse_sys_args
-try:
-    import alexber.utils.ymlparsers as ymlparsers
-except ImportError:
-    pass
-
-from .importer import importer
-
-
-class conf(object):
-    """
-    See parse_config() function for details.
-    """
-    GENERAL_KEY = 'general'
-    PROFILES_KEY = 'profiles'
-    #WHITE_LIST_IMPLICIT_KEY = 'whiteListImplicitely'    #default True
-    WHITE_LIST_KEY = 'whiteListSysOverride'
-    LIST_ENSURE_KEY ='listEnsure'
-
-    CONFIG_KEY = 'config'
-    FILE_LEY = 'file'
-
-
-class AppConfParser(object):
-    def __init__(self, *args, **kwargs):
-        self.implicit_convert = kwargs.pop('implicit_convert')
-        if self.implicit_convert is None:
-            raise ValueError("implicit_convert can't be None")
-
-    basic_parse_sys_args = staticmethod(uparse_sys_args)
-
-    def _parse_yml(self, sys_d, profiles, config_file='config.yml'):
-        if ymlparsers.HiYaPyCo.jinja2ctx is None:
-            raise ValueError("ymlparsers.HiYaPyCo.jinja2ctx can't be None")
-
-        base_full_path = Path(config_file).resolve()  # relative to cwd
-
-        base_suffix = base_full_path.suffix
-        base_name = base_full_path.with_suffix("").name
-
-        with _io.StringIO() as sys_buf:
-            ymlparsers.safe_dump(sys_d, sys_buf)
-
-            buffersize = len(profiles) + 1  # default_profile
-            yml_files = deque(maxlen=buffersize)
-
-            yml_files.append(str(base_full_path))
-            full_path = base_full_path
-
-            for profile in profiles:
-                name = base_name + '-' + profile + base_suffix
-                full_path = full_path.with_name(name)
-                yml_files.append(str(full_path))
-
-            dd = ymlparsers.load([*yml_files, sys_buf.getvalue()])
-
-        return dd
-
-    def _parse_white_list_implicitely(self, default_d):
-        subvalue = default_d.get(conf.GENERAL_KEY, {})
-        value = subvalue.get(conf.WHITE_LIST_KEY, {})
-
-        ret = is_empty(value)
-        if ret is None:
-            ret = True
-        return ret
-
-    def _parse_white_list(self, default_d):
-        calc_implicitely = self._parse_white_list_implicitely(default_d)
-
-        if calc_implicitely:
-            white_list = [key for key in default_d.keys() if key not in conf.WHITE_LIST_KEY]
-            return white_list
-
-        # default_d[conf.GENERAL_KEY][conf.WHITE_LIST_KEY] is not empty
-        subvalue = default_d.get(conf.GENERAL_KEY, {})
-        white_list = subvalue.get(conf.WHITE_LIST_KEY, {})
-
-        return white_list
-
-    def _is_white_listed(self, white_list_flat_keys, flat_key):
-        b = is_empty(white_list_flat_keys)
-        if b:
-            return True
-
-        for white_list_flat_key in white_list_flat_keys:
-            if flat_key.startswith(white_list_flat_key):
-                return True
-        return False
-
-    def to_convex_map(self, d, white_list_flat_keys=None):
-        dd = OrderedDict()
-
-        for flat_key, value in d.items():
-            if not ('.' in flat_key and self._is_white_listed(white_list_flat_keys, flat_key)):
-                logger.info(f"Skipping key {flat_key}. It doesn't contain dot.")
-                continue
-
-            keys = flat_key.split(".")
-            length = len(keys)
-
-            inner_d = dd
-            for i, part_key in enumerate(keys):
-                if i + 1 == length:  # last element
-                    inner_d = inner_d.setdefault(part_key, self.mask_value(value))
-                else:
-                    inner_d = inner_d.setdefault(part_key, OrderedDict())
-        return dd
-
-    def merge_list_value_in_dicts(self, flat_d, d, main_key, sub_key):
-        if flat_d is None:
-            raise TypeError("flat_d can't be None")
-
-        if d is None:
-            raise TypeError("d can't be None")
-
-        flat_key = '.'.join([main_key, sub_key])
-        flat_value = self._ensure_list(flat_d, flat_key)
-
-        length_flat_value = len(flat_value)
-
-        subvalue = d.get(main_key, {})
-        value = subvalue.get(sub_key, {})
-
-        merged_value = value if length_flat_value == 0 else flat_value
-        return merged_value
-
-    def _parse_profiles(self, sys_d, default_d):
-        profiles = self.merge_list_value_in_dicts(sys_d, default_d, conf.GENERAL_KEY, conf.PROFILES_KEY)
-        b = is_empty(profiles)
-        if b:
-            profiles = []
-        return profiles
-
-    def _parse_list_ensure(self, sys_d, default_d):
-        list_ensure = self.merge_list_value_in_dicts(sys_d, default_d, conf.GENERAL_KEY, conf.LIST_ENSURE_KEY)
-
-        b = is_empty(list_ensure)
-        if not b:
-            # we already proceesed profiles, white_list
-            # we should process list_ensure
-            profiles_flat_key = '.'.join([conf.GENERAL_KEY, conf.PROFILES_KEY])
-            list_ensure_flat_key = '.'.join([conf.GENERAL_KEY, conf.LIST_ENSURE_KEY])
-            white_list_flat_key = '.'.join([conf.GENERAL_KEY, conf.WHITE_LIST_KEY])
-
-            list_ensure = [flat_key for flat_key in list_ensure \
-                           if flat_key not in {profiles_flat_key, list_ensure_flat_key, white_list_flat_key}]
-        else:
-            list_ensure = []
-        return list_ensure
-
-    def _get_white_listed(self, d, white_list_flat_keys):
-        b = is_empty(d)
-        if b:
-            return d
-        dd = OrderedDict()
-
-        for flat_key, value in d.items():
-            if not ('.' in flat_key and self._is_white_listed(white_list_flat_keys, flat_key)):
-                logger.info(f"Skipping key {flat_key}. It doesn't white listed.")
-                continue
-
-            dd[flat_key] = value
-        return dd
-
-    def _do_ensure_list(self, flat_d, list_ensure):
-        b = is_empty(list)
-        if b:
-            return
-
-        for flat_key in list_ensure:
-            flat_value = self._ensure_list(flat_d, flat_key)
-            flat_d[flat_key] = flat_value
-
-    def _bool_is_empty(self, value):
-        try:
-            ret = parse_boolean(value)
-            return ret is None
-        except ValueError:
-            ret = is_empty(value)
-        return ret
-
-    def _bool_convert(self, value):
-        try:
-            ret = parse_boolean(value)
-            return ret
-        except ValueError:
-            ret = _convert(value)
-        return ret
-
-    def mask_value(self, value):
-        ret = self._bool_convert(value) \
-            if self.implicit_convert \
-            else value
-        return ret
-
-    def _ensure_list(self, flat_d, key):
-        def _ensure_list(v):
-            value = str(v)
-            elements = value.split(",")
-
-            # empty string will become null
-            elements = [None if is_empty(value) else value for value in elements]
-            ret = [self.mask_value(value) for value in elements]
-
-            return ret
-
-        if flat_d is None:
-            flat_d = {}
-        val = flat_d.get(key, None)
-        b = self._bool_is_empty(val)
-        if b:
-            if key in flat_d.keys():
-                # we have key:None?
-                return [val]
-            return []
-        return _ensure_list(val)
-
-    def _parse_sys_args(self, argumentParser=None, args=None):
-        if ymlparsers.HiYaPyCo.jinja2ctx is None:
-            raise ValueError("ymlparsers.HiYaPyCo.jinja2ctx can't be None")
-
-        params, sys_d0 = self.basic_parse_sys_args(argumentParser, args)
-        config_file = params.config_file
-
-        full_path = Path(config_file).resolve()  # relative to cwd
-
-        with ymlparsers.DisableVarSubst():
-            default_d = ymlparsers.load([str(full_path)])
-
-        white_list = self._parse_white_list(default_d)
-        sys_d = self._get_white_listed(sys_d0, white_list)
-
-        profiles = self._parse_profiles(sys_d, default_d)
-
-        list_ensure = self._parse_list_ensure(sys_d, default_d)
-
-        self._do_ensure_list(sys_d, list_ensure)
-
-        dd = self.to_convex_map(sys_d)
-        return dd, profiles, white_list, list_ensure, full_path
-
-    def parse_config(self, argumentParser=None, args=None):
-
-        sys_d, profiles, white_list, list_ensure, config_file = self._parse_sys_args(argumentParser=argumentParser,
-                                                                                     args=args)
-        dd = self._parse_yml(sys_d, profiles, config_file)
-
-        # merge all to dd
-        general_d = dd.setdefault(conf.GENERAL_KEY, OrderedDict())
-        config_d = general_d.setdefault(conf.CONFIG_KEY, OrderedDict())
-        config_d[conf.FILE_LEY] = str(config_file)
-
-        general_d[conf.PROFILES_KEY] = profiles
-        general_d[conf.WHITE_LIST_KEY] = white_list
-        general_d[conf.LIST_ENSURE_KEY] = list_ensure
-
-        general_d = dd.setdefault(conf.GENERAL_KEY, OrderedDict())
-        config_d = general_d.setdefault(conf.CONFIG_KEY, OrderedDict())
-        config_d[conf.FILE_LEY] = str(config_file)
-
-        general_d[conf.PROFILES_KEY] = profiles
-        general_d[conf.WHITE_LIST_KEY] = white_list
-        general_d[conf.LIST_ENSURE_KEY] = list_ensure
-        return dd
-
-def _create_default_parser(**kwargs):
-    if default_parser_cls is None:
-        raise ValueError("default_parser_cls can't be None")
-
-    implicit_convert = kwargs['implicit_convert']
-    if implicit_convert is None:
-        implicit_convert=default_parser_kwargs['implicit_convert']
-
-    kwargs = {
-        **default_parser_kwargs,
-        'implicit_convert': implicit_convert,
-
-    }
-    parser = default_parser_cls(**kwargs)
-    return parser
-
-def mask_value(value, implicit_convert=None):
-    """
-    If implicit_convert=True, than for system args we assume Python built-in types, including bool,
-    and we're converting it to appropriate type.
-    Otherwise, implicit_convert will have the value that was set in `intiConfig()`. By default it is True.
-
-
-    Bool values are case-insensitive.
-
-    :param value: str to ccnvert
-    :param implicit_convert: if none, than value that was passed to initConfig() is used (default).
-                             if True value attempt to convert value to appropriate type will be done,
-                             if False value will be used as is. See mask_value() function.
-    :return:
-    """
-    if default_parser_cls is None:
-        raise ValueError("default_parser_cls can't be None")
-
-    parser = _create_default_parser(**{'implicit_convert': implicit_convert})
-    ret = parser.mask_value(value)
-    return ret
-
-
-def to_convex_map(d, white_list_flat_keys=None, implicit_convert=None):
-    """
-    This method receives dictionary with 'flat keys', it has simple key:value structure
-    where value can't be another dictionary.
-    It will return dictionary of dictionaries with natural key mapping (see bellow),
-    optionally, entries will be filtered out according to white_list_flat_keys and,
-    optionally, value will be implicitly converted to appropriate type.
-
-    In order to simulate dictionary of dictionaries 'flat keys' compose key from outer dict with key from inner dict
-    separated with dot.
-    For example, 'general.profiles' 'flat key' corresponds to convex map with 'general' key with dictionary as value
-    that have one of the keys 'profiles' with corresponding value.
-
-    if white_list_flat_keys is not None, it will be used to filter out entries from d.
-    If implicit_convert=True, than for system args we assume Python built-in types, including bool,
-    and we're converting it to appropriate type.
-    Otherwise, implicit_convert will have the value that was set in `intiConfig()`. By default it is True.
-
-
-    :param d: dict with flat keys
-    :param white_list_flat_keys: Optional. if present, only keys that start with one of the elements listed here
-                                            will be considered.
-    :param implicit_convert: if none, than value that was passed to initConfig() is used (default).
-                             if True value attempt to convert value to appropriate type will be done,
-                             if False value will be used as is. See mask_value() function.
-    :return: convex map with optionally filtered entrys
-    """
-    if default_parser_cls is None:
-        raise ValueError("default_parser_cls can't be None")
-
-    parser = _create_default_parser(**{'implicit_convert': implicit_convert})
-    dd = parser.to_convex_map(d, white_list_flat_keys)
-    return dd
-
-
-
-def merge_list_value_in_dicts(flat_d, d, main_key, sub_key, implicit_convert=None):
-    """
-    This method merge value of 2 dicts. This value represents list of values.
-
-    Value from flat_d is roughly obtained by flat_d[main_key+'.'+sub_key].
-    Value from d is roughly obtained by d[main_key][sub_key].
-
-    If value (or intermediate value) is not found empty dict is used.
-
-    This method assumes that flat_d value contain str that represent list (comma-delimited).
-    This method assumes that d[main_key] contains dict.
-    implicit_convert is applied only for flat_d.
-
-
-    If implicit_convert=True, than for system args we assume Python built-in types, including bool,
-    and we're converting it to appropriate type.
-    Otherwise, implicit_convert will have the value that was set in `intiConfig()`. By default it is True.
-
-
-
-    :param flat_d: flat dictionary, usually one that was created from parsing system args.
-    :param d: dictionary of dictionaries,  usually one that was created from parsing YAML file.
-    :param main_key: d[main_key] is absent or dict.
-    :param sub_key: d[main_key][sub_key] is absent or list.
-    :param implicit_convert: if none, than value that was passed to initConfig() is used (default).
-                             if True value attempt to convert value to appropriate type will be done,
-                             if False value will be used as is. See mask_value() function.
-    :return: merged converted value, typically one from flat_d, if empty than from d
-    """
-    if default_parser_cls is None:
-        raise ValueError("default_parser_cls can't be None")
-
-    parser = _create_default_parser(**{'implicit_convert': implicit_convert})
-    merged_value = parser.merge_list_value_in_dicts(flat_d, d, main_key, sub_key)
-    return merged_value
-
-def parse_config(argumentParser=None, args=None, implicit_convert=None):
-    """
-    This is the main function of the module.
-
-    This function parses command line arguments first.
-    Than it parse yml files.
-    Command line arguments overrides yml files arguments.
-
-    Parameters of yml files we always try to convert on best-effort basses.
-    Parameters of system args we try convert according to implicit_convert param (see below).
-
-    In more detail, command line arguments of the form --key=value are parsed first.
-    If exists --config_file it's value is used to search for yml file.
-    if --config_file is absent, 'config.yml' is used for yml file.
-    If yml file is not found, only command line arguments are used.
-    If yml file is found, both arguments are used, while
-    command line arguments overrides yml arguments.
-
-    --general.profiles or appropriate key in default yml file is used to find 'profiles'.
-    Let suppose, that --config_file is resolved to config.yml.
-    If 'profiles' is not empty, than it will be used to calculate filenames
-    that will be used to override default yml file.
-    Let suppose, 'profiles' resolved to ['dev', 'local']. Than first config.yml
-    will be loaded, than it will be overridden with config-dev.yml, than
-    it will be overridden with config-local.yml.
-    At last, it will be overridden with system args.
-    This entry can be always be overridden with system args.
-
-    general.whiteListSysOverride key in yml file is optional.
-    If not provided, than any key that exists in the default yml file can be overridden
-    with system args.
-    If provided, than only key that start with one of the key provided here can be used
-    to override entrys with system args.
-    This entry can't be overridden with system args.
-
-    --general.listEnsure or appropriate key in default yml file is used to instruct that
-    listed key should be interpreted as comma-delimited list when is used to override
-    entrys with system args.
-    This entry can be always be overridden with system args.
-
-    general.config.file is key that is used in returned dict that points to default yml file.
-
-    If implicit_convert=True, than for system args we assume Python built-in types, including bool,
-    and we're converting it to appropriate type.
-    Otherwise, implicit_convert will have the value that was set in `intiConfig()`. By default it is True.
-
-
-
-    :param argumentParser:
-    :param args: if not None, suppresses sys.args
-    :param implicit_convert: if none, than value that was passed to initConfig() is used (default).
-                             if True value attempt to convert value from system args to appropriate type will be done,
-                             if False value from system args will be used as is. See mask_value() function.
-    :return: dict ready to use
-    """
-    if default_parser_cls is None:
-        raise ValueError("default_parser_cls can't be None")
-
-    if ymlparsers.HiYaPyCo.jinja2ctx is None:
-        raise ValueError("ymlparsers.HiYaPyCo.jinja2ctx can't be None")
-
-    parser = _create_default_parser(**{'implicit_convert': implicit_convert})
-    dd = parser.parse_config(argumentParser=argumentParser, args=args)
-    return dd
-
-
-default_parser_cls = None
-default_parser_kwargs = None
-
-def initConfig(**kwargs):
-    """
-    This method can be optionally called prior any call to another function in this module.
-    It is indented to be called in the MainThread.
-    This method can be call with empty params.
-
-    :param default_parser_cls: can be class or str. Optional.
-                Default values is: AppConfParser
-    :param default_parser_kwargs: this params will be used as default values in default_parser_cls.__init__() function.
-                Default values are
-                      'implicit_convert':True,
-                This means, by default:
-                    We're converting values using mask_value() function.
-
-    This method is idempotent.
-    :return:
-    """
-    default_parser_cls_p = kwargs.get('default_parser_cls', None)
-    if default_parser_cls_p is None:
-        default_parser_cls_p = AppConfParser
-    elif isinstance(default_parser_cls_p, str):
-        default_parser_cls_p = importer(default_parser_cls_p)
-    global default_parser_cls
-    default_parser_cls = default_parser_cls_p
-
-    default_parser_kwargs_p = kwargs.get('default_parser_kwargs', {})
-    default_parser_kwargs_p = {
-        'implicit_convert':True,
-        **default_parser_kwargs_p}
-    global default_parser_kwargs
-    default_parser_kwargs = default_parser_kwargs_p
-
+"""
+`ymlparsers` and `parser` modules serves as Low-Level API for this module.
+
+You may need to install some 3-rd party dependencies, in order to use it, you should have installed first. To do it
+run `python3 -m pip install alex-ber-utils[yml]` in order to use it.
+
+See https://medium.com/analytics-vidhya/my-major-init-app-conf-module-1a5d9fb3998c for documentation.
+"""
+import logging
+logger = logging.getLogger(__name__)
+
+from collections import OrderedDict, deque
+from pathlib import Path
+import io as _io
+from alexber.utils.parsers import is_empty, safe_eval as _convert, parse_boolean, ArgumentParser, \
+    parse_sys_args as uparse_sys_args
+try:
+    import alexber.utils.ymlparsers as ymlparsers
+except ImportError:
+    pass
+
+from .importer import importer
+
+
+class conf(object):
+    """
+    See parse_config() function for details.
+    """
+    GENERAL_KEY = 'general'
+    PROFILES_KEY = 'profiles'
+    #WHITE_LIST_IMPLICIT_KEY = 'whiteListImplicitely'    #default True
+    WHITE_LIST_KEY = 'whiteListSysOverride'
+    LIST_ENSURE_KEY ='listEnsure'
+
+    CONFIG_KEY = 'config'
+    FILE_LEY = 'file'
+
+
+class AppConfParser(object):
+    def __init__(self, *args, **kwargs):
+        self.implicit_convert = kwargs.pop('implicit_convert')
+        if self.implicit_convert is None:
+            raise ValueError("implicit_convert can't be None")
+
+    basic_parse_sys_args = staticmethod(uparse_sys_args)
+
+    def _parse_yml(self, sys_d, profiles, config_file='config.yml'):
+        if ymlparsers.HiYaPyCo.jinja2ctx is None:
+            raise ValueError("ymlparsers.HiYaPyCo.jinja2ctx can't be None")
+
+        base_full_path = Path(config_file).resolve()  # relative to cwd
+
+        base_suffix = base_full_path.suffix
+        base_name = base_full_path.with_suffix("").name
+
+        with _io.StringIO() as sys_buf:
+            ymlparsers.safe_dump(sys_d, sys_buf)
+
+            buffersize = len(profiles) + 1  # default_profile
+            yml_files = deque(maxlen=buffersize)
+
+            yml_files.append(str(base_full_path))
+            full_path = base_full_path
+
+            for profile in profiles:
+                name = base_name + '-' + profile + base_suffix
+                full_path = full_path.with_name(name)
+                yml_files.append(str(full_path))
+
+            dd = ymlparsers.load([*yml_files, sys_buf.getvalue()])
+
+        return dd
+
+    def _parse_white_list_implicitely(self, default_d):
+        subvalue = default_d.get(conf.GENERAL_KEY, {})
+        value = subvalue.get(conf.WHITE_LIST_KEY, {})
+
+        ret = is_empty(value)
+        if ret is None:
+            ret = True
+        return ret
+
+    def _parse_white_list(self, default_d):
+        calc_implicitely = self._parse_white_list_implicitely(default_d)
+
+        if calc_implicitely:
+            white_list = [key for key in default_d.keys() if key not in conf.WHITE_LIST_KEY]
+            return white_list
+
+        # default_d[conf.GENERAL_KEY][conf.WHITE_LIST_KEY] is not empty
+        subvalue = default_d.get(conf.GENERAL_KEY, {})
+        white_list = subvalue.get(conf.WHITE_LIST_KEY, {})
+
+        return white_list
+
+    def _is_white_listed(self, white_list_flat_keys, flat_key):
+        b = is_empty(white_list_flat_keys)
+        if b:
+            return True
+
+        for white_list_flat_key in white_list_flat_keys:
+            if flat_key.startswith(white_list_flat_key):
+                return True
+        return False
+
+    def to_convex_map(self, d, white_list_flat_keys=None):
+        dd = OrderedDict()
+
+        for flat_key, value in d.items():
+            if not ('.' in flat_key and self._is_white_listed(white_list_flat_keys, flat_key)):
+                logger.info(f"Skipping key {flat_key}. It doesn't contain dot.")
+                continue
+
+            keys = flat_key.split(".")
+            length = len(keys)
+
+            inner_d = dd
+            for i, part_key in enumerate(keys):
+                if i + 1 == length:  # last element
+                    inner_d = inner_d.setdefault(part_key, self.mask_value(value))
+                else:
+                    inner_d = inner_d.setdefault(part_key, OrderedDict())
+        return dd
+
+    def merge_list_value_in_dicts(self, flat_d, d, main_key, sub_key):
+        if flat_d is None:
+            raise TypeError("flat_d can't be None")
+
+        if d is None:
+            raise TypeError("d can't be None")
+
+        flat_key = '.'.join([main_key, sub_key])
+        flat_value = self._ensure_list(flat_d, flat_key)
+
+        length_flat_value = len(flat_value)
+
+        subvalue = d.get(main_key, {})
+        value = subvalue.get(sub_key, {})
+
+        merged_value = value if length_flat_value == 0 else flat_value
+        return merged_value
+
+    def _parse_profiles(self, sys_d, default_d):
+        profiles = self.merge_list_value_in_dicts(sys_d, default_d, conf.GENERAL_KEY, conf.PROFILES_KEY)
+        b = is_empty(profiles)
+        if b:
+            profiles = []
+        return profiles
+
+    def _parse_list_ensure(self, sys_d, default_d):
+        list_ensure = self.merge_list_value_in_dicts(sys_d, default_d, conf.GENERAL_KEY, conf.LIST_ENSURE_KEY)
+
+        b = is_empty(list_ensure)
+        if not b:
+            # we already proceesed profiles, white_list
+            # we should process list_ensure
+            profiles_flat_key = '.'.join([conf.GENERAL_KEY, conf.PROFILES_KEY])
+            list_ensure_flat_key = '.'.join([conf.GENERAL_KEY, conf.LIST_ENSURE_KEY])
+            white_list_flat_key = '.'.join([conf.GENERAL_KEY, conf.WHITE_LIST_KEY])
+
+            list_ensure = [flat_key for flat_key in list_ensure \
+                           if flat_key not in {profiles_flat_key, list_ensure_flat_key, white_list_flat_key}]
+        else:
+            list_ensure = []
+        return list_ensure
+
+    def _get_white_listed(self, d, white_list_flat_keys):
+        b = is_empty(d)
+        if b:
+            return d
+        dd = OrderedDict()
+
+        for flat_key, value in d.items():
+            if not ('.' in flat_key and self._is_white_listed(white_list_flat_keys, flat_key)):
+                logger.info(f"Skipping key {flat_key}. It doesn't white listed.")
+                continue
+
+            dd[flat_key] = value
+        return dd
+
+    def _do_ensure_list(self, flat_d, list_ensure):
+        b = is_empty(list)
+        if b:
+            return
+
+        for flat_key in list_ensure:
+            flat_value = self._ensure_list(flat_d, flat_key)
+            flat_d[flat_key] = flat_value
+
+    def _bool_is_empty(self, value):
+        try:
+            ret = parse_boolean(value)
+            return ret is None
+        except ValueError:
+            ret = is_empty(value)
+        return ret
+
+    def _bool_convert(self, value):
+        try:
+            ret = parse_boolean(value)
+            return ret
+        except ValueError:
+            ret = _convert(value)
+        return ret
+
+    def mask_value(self, value):
+        ret = self._bool_convert(value) \
+            if self.implicit_convert \
+            else value
+        return ret
+
+    def _ensure_list(self, flat_d, key):
+        def _ensure_list(v):
+            value = str(v)
+            elements = value.split(",")
+
+            # empty string will become null
+            elements = [None if is_empty(value) else value for value in elements]
+            ret = [self.mask_value(value) for value in elements]
+
+            return ret
+
+        if flat_d is None:
+            flat_d = {}
+        val = flat_d.get(key, None)
+        b = self._bool_is_empty(val)
+        if b:
+            if key in flat_d.keys():
+                # we have key:None?
+                return [val]
+            return []
+        return _ensure_list(val)
+
+    def _parse_sys_args(self, argumentParser=None, args=None):
+        if ymlparsers.HiYaPyCo.jinja2ctx is None:
+            raise ValueError("ymlparsers.HiYaPyCo.jinja2ctx can't be None")
+
+        params, sys_d0 = self.basic_parse_sys_args(argumentParser, args)
+        config_file = params.config_file
+
+        full_path = Path(config_file).resolve()  # relative to cwd
+
+        with ymlparsers.DisableVarSubst():
+            default_d = ymlparsers.load([str(full_path)])
+
+        white_list = self._parse_white_list(default_d)
+        sys_d = self._get_white_listed(sys_d0, white_list)
+
+        profiles = self._parse_profiles(sys_d, default_d)
+
+        list_ensure = self._parse_list_ensure(sys_d, default_d)
+
+        self._do_ensure_list(sys_d, list_ensure)
+
+        dd = self.to_convex_map(sys_d)
+        return dd, profiles, white_list, list_ensure, full_path
+
+    def parse_config(self, argumentParser=None, args=None):
+
+        sys_d, profiles, white_list, list_ensure, config_file = self._parse_sys_args(argumentParser=argumentParser,
+                                                                                     args=args)
+        dd = self._parse_yml(sys_d, profiles, config_file)
+
+        # merge all to dd
+        general_d = dd.setdefault(conf.GENERAL_KEY, OrderedDict())
+        config_d = general_d.setdefault(conf.CONFIG_KEY, OrderedDict())
+        config_d[conf.FILE_LEY] = str(config_file)
+
+        general_d[conf.PROFILES_KEY] = profiles
+        general_d[conf.WHITE_LIST_KEY] = white_list
+        general_d[conf.LIST_ENSURE_KEY] = list_ensure
+
+        general_d = dd.setdefault(conf.GENERAL_KEY, OrderedDict())
+        config_d = general_d.setdefault(conf.CONFIG_KEY, OrderedDict())
+        config_d[conf.FILE_LEY] = str(config_file)
+
+        general_d[conf.PROFILES_KEY] = profiles
+        general_d[conf.WHITE_LIST_KEY] = white_list
+        general_d[conf.LIST_ENSURE_KEY] = list_ensure
+        return dd
+
+def _create_default_parser(**kwargs):
+    if default_parser_cls is None:
+        raise ValueError("default_parser_cls can't be None")
+
+    implicit_convert = kwargs['implicit_convert']
+    if implicit_convert is None:
+        implicit_convert=default_parser_kwargs['implicit_convert']
+
+    kwargs = {
+        **default_parser_kwargs,
+        'implicit_convert': implicit_convert,
+
+    }
+    parser = default_parser_cls(**kwargs)
+    return parser
+
+def mask_value(value, implicit_convert=None):
+    """
+    If implicit_convert=True, than for system args we assume Python built-in types, including bool,
+    and we're converting it to appropriate type.
+    Otherwise, implicit_convert will have the value that was set in `intiConfig()`. By default it is True.
+
+
+    Bool values are case-insensitive.
+
+    :param value: str to ccnvert
+    :param implicit_convert: if none, than value that was passed to initConfig() is used (default).
+                             if True value attempt to convert value to appropriate type will be done,
+                             if False value will be used as is. See mask_value() function.
+    :return:
+    """
+    if default_parser_cls is None:
+        raise ValueError("default_parser_cls can't be None")
+
+    parser = _create_default_parser(**{'implicit_convert': implicit_convert})
+    ret = parser.mask_value(value)
+    return ret
+
+
+def to_convex_map(d, white_list_flat_keys=None, implicit_convert=None):
+    """
+    This method receives dictionary with 'flat keys', it has simple key:value structure
+    where value can't be another dictionary.
+    It will return dictionary of dictionaries with natural key mapping (see bellow),
+    optionally, entries will be filtered out according to white_list_flat_keys and,
+    optionally, value will be implicitly converted to appropriate type.
+
+    In order to simulate dictionary of dictionaries 'flat keys' compose key from outer dict with key from inner dict
+    separated with dot.
+    For example, 'general.profiles' 'flat key' corresponds to convex map with 'general' key with dictionary as value
+    that have one of the keys 'profiles' with corresponding value.
+
+    if white_list_flat_keys is not None, it will be used to filter out entries from d.
+    If implicit_convert=True, than for system args we assume Python built-in types, including bool,
+    and we're converting it to appropriate type.
+    Otherwise, implicit_convert will have the value that was set in `intiConfig()`. By default it is True.
+
+
+    :param d: dict with flat keys
+    :param white_list_flat_keys: Optional. if present, only keys that start with one of the elements listed here
+                                            will be considered.
+    :param implicit_convert: if none, than value that was passed to initConfig() is used (default).
+                             if True value attempt to convert value to appropriate type will be done,
+                             if False value will be used as is. See mask_value() function.
+    :return: convex map with optionally filtered entrys
+    """
+    if default_parser_cls is None:
+        raise ValueError("default_parser_cls can't be None")
+
+    parser = _create_default_parser(**{'implicit_convert': implicit_convert})
+    dd = parser.to_convex_map(d, white_list_flat_keys)
+    return dd
+
+
+
+def merge_list_value_in_dicts(flat_d, d, main_key, sub_key, implicit_convert=None):
+    """
+    This method merge value of 2 dicts. This value represents list of values.
+
+    Value from flat_d is roughly obtained by flat_d[main_key+'.'+sub_key].
+    Value from d is roughly obtained by d[main_key][sub_key].
+
+    If value (or intermediate value) is not found empty dict is used.
+
+    This method assumes that flat_d value contain str that represent list (comma-delimited).
+    This method assumes that d[main_key] contains dict.
+    implicit_convert is applied only for flat_d.
+
+
+    If implicit_convert=True, than for system args we assume Python built-in types, including bool,
+    and we're converting it to appropriate type.
+    Otherwise, implicit_convert will have the value that was set in `intiConfig()`. By default it is True.
+
+
+
+    :param flat_d: flat dictionary, usually one that was created from parsing system args.
+    :param d: dictionary of dictionaries,  usually one that was created from parsing YAML file.
+    :param main_key: d[main_key] is absent or dict.
+    :param sub_key: d[main_key][sub_key] is absent or list.
+    :param implicit_convert: if none, than value that was passed to initConfig() is used (default).
+                             if True value attempt to convert value to appropriate type will be done,
+                             if False value will be used as is. See mask_value() function.
+    :return: merged converted value, typically one from flat_d, if empty than from d
+    """
+    if default_parser_cls is None:
+        raise ValueError("default_parser_cls can't be None")
+
+    parser = _create_default_parser(**{'implicit_convert': implicit_convert})
+    merged_value = parser.merge_list_value_in_dicts(flat_d, d, main_key, sub_key)
+    return merged_value
+
+def parse_config(argumentParser=None, args=None, implicit_convert=None):
+    """
+    This is the main function of the module.
+
+    This function parses command line arguments first.
+    Than it parse yml files.
+    Command line arguments overrides yml files arguments.
+
+    Parameters of yml files we always try to convert on best-effort basses.
+    Parameters of system args we try convert according to implicit_convert param (see below).
+
+    In more detail, command line arguments of the form --key=value are parsed first.
+    If exists --config_file it's value is used to search for yml file.
+    if --config_file is absent, 'config.yml' is used for yml file.
+    If yml file is not found, only command line arguments are used.
+    If yml file is found, both arguments are used, while
+    command line arguments overrides yml arguments.
+
+    --general.profiles or appropriate key in default yml file is used to find 'profiles'.
+    Let suppose, that --config_file is resolved to config.yml.
+    If 'profiles' is not empty, than it will be used to calculate filenames
+    that will be used to override default yml file.
+    Let suppose, 'profiles' resolved to ['dev', 'local']. Than first config.yml
+    will be loaded, than it will be overridden with config-dev.yml, than
+    it will be overridden with config-local.yml.
+    At last, it will be overridden with system args.
+    This entry can be always be overridden with system args.
+
+    general.whiteListSysOverride key in yml file is optional.
+    If not provided, than any key that exists in the default yml file can be overridden
+    with system args.
+    If provided, than only key that start with one of the key provided here can be used
+    to override entrys with system args.
+    This entry can't be overridden with system args.
+
+    --general.listEnsure or appropriate key in default yml file is used to instruct that
+    listed key should be interpreted as comma-delimited list when is used to override
+    entrys with system args.
+    This entry can be always be overridden with system args.
+
+    general.config.file is key that is used in returned dict that points to default yml file.
+
+    If implicit_convert=True, than for system args we assume Python built-in types, including bool,
+    and we're converting it to appropriate type.
+    Otherwise, implicit_convert will have the value that was set in `intiConfig()`. By default it is True.
+
+
+
+    :param argumentParser:
+    :param args: if not None, suppresses sys.args
+    :param implicit_convert: if none, than value that was passed to initConfig() is used (default).
+                             if True value attempt to convert value from system args to appropriate type will be done,
+                             if False value from system args will be used as is. See mask_value() function.
+    :return: dict ready to use
+    """
+    if default_parser_cls is None:
+        raise ValueError("default_parser_cls can't be None")
+
+    if ymlparsers.HiYaPyCo.jinja2ctx is None:
+        raise ValueError("ymlparsers.HiYaPyCo.jinja2ctx can't be None")
+
+    parser = _create_default_parser(**{'implicit_convert': implicit_convert})
+    dd = parser.parse_config(argumentParser=argumentParser, args=args)
+    return dd
+
+
+default_parser_cls = None
+default_parser_kwargs = None
+
+def initConfig(**kwargs):
+    """
+    This method can be optionally called prior any call to another function in this module.
+    It is indented to be called in the MainThread.
+    This method can be call with empty params.
+
+    :param default_parser_cls: can be class or str. Optional.
+                Default values is: AppConfParser
+    :param default_parser_kwargs: this params will be used as default values in default_parser_cls.__init__() function.
+                Default values are
+                      'implicit_convert':True,
+                This means, by default:
+                    We're converting values using mask_value() function.
+
+    This method is idempotent.
+    :return:
+    """
+    default_parser_cls_p = kwargs.get('default_parser_cls', None)
+    if default_parser_cls_p is None:
+        default_parser_cls_p = AppConfParser
+    elif isinstance(default_parser_cls_p, str):
+        default_parser_cls_p = importer(default_parser_cls_p)
+    global default_parser_cls
+    default_parser_cls = default_parser_cls_p
+
+    default_parser_kwargs_p = kwargs.get('default_parser_kwargs', {})
+    default_parser_kwargs_p = {
+        'implicit_convert':True,
+        **default_parser_kwargs_p}
+    global default_parser_kwargs
+    default_parser_kwargs = default_parser_kwargs_p
+
 initConfig()
```

### Comparing `alex_ber_utils-0.6.6b3/alexber/utils/mains.py` & `alex_ber_utils-0.7.0/alexber/utils/mains.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,323 +1,323 @@
-import logging
-
-import os as _os
-import sys as _sys
-import contextlib
-from collections import deque
-from .parsers import is_empty
-from .importer import importer
-
-logger = logging.getLogger(__name__)
-
-
-# inspider by https://github.com/theskumar/python-dotenv/blob/12439aac2d7c98b5acaf51ae3044b1659dc086ae/src/dotenv/main.py#L250
-def _is_interactive(module):
-    """ Decide whether this is running in a REPL or IPython notebook """
-    return not hasattr(module, '__file__')
-
-
-def fixabscwd():
-    """
-    See here https://medium.com/@alex_ber/making-relative-path-to-file-to-work-d5d0f1da67bf for documentation.
-    """
-    logger.info(f"cwd is {_os.getcwd()}")
-
-    main_module = _sys.modules['__main__']
-
-    if _is_interactive(main_module) or getattr(_sys, 'frozen', False):
-        # Should work without __file__, e.g. in REPL or IPython notebook.
-        pass
-    else:
-        main_dir = _os.path.dirname(_os.path.realpath(main_module.__file__))
-
-        logger.info(f"Going to change os.chdir('{main_dir}')")
-
-        _os.chdir(main_dir)
-
-def path():
-    """
-    For older Python version uses`importlib_resources` module.
-    For newer version built in `importlib.resources`.
-    :return:
-    """
-    if _sys.version_info >= (3, 7):
-        from importlib.resources import path as _path
-    else:
-        try:
-            from importlib_resources import path as _path
-        except ImportError:
-            import warnings
-
-            warning = (
-                "You appear to be missing some optional dependencies (importlib_resources);"
-            )
-            warnings.warn(warning, ImportWarning)
-            raise
-    return _path
-
-
-def load_env(**kwargs):
-    """
-    Convenient method from loading environment variables
-    inside packed format (eggs, etc).
-
-    if dotenv_path or stream is present it will be used.
-    if ENV_PCK is present, dotenv_path will be constructed from ENV_PCK and ENV_NAME.
-    Otherwise, kwargs will be forwarded as is to load_dotenv.
-
-
-    Implementaion note:
-    If available it uses importlib.resources API,
-    if not it assumes existence of backport of importlib_resources.
-
-    :param ENV_PCK: package where to find .env file Optional.
-    :param ENV_NAME: Name of .env file. Optional.
-    :param dotenv_path:  absolute or relative path to .env file. Optional.
-    :param stream: `StringIO` object with .env content. Optional.
-    :return:
-    """
-
-    # os.environ['AWS_DEFAULT_REGION'] = 'eu-central-1'
-    try:
-        from dotenv import load_dotenv
-    except ImportError:
-        import warnings
-
-
-        warning = (
-            "You appear to be missing some optional dependencies (python-dotenv);"
-            "please 'python3 -m pip install alex-ber-utils[python-dotenv]'."
-        )
-
-        warnings.warn(warning, ImportWarning)
-        raise
-
-    l_path = path()
-
-    dotenv_path = kwargs.get('dotenv_path', None)
-    stream = kwargs.get('stream', None)
-    ENV_PCK = kwargs.pop('ENV_PCK', None)
-
-    if not is_empty(dotenv_path) or not is_empty(stream) or \
-            (is_empty(dotenv_path) and is_empty(stream) and is_empty(ENV_PCK)):
-        load_dotenv(**kwargs)
-
-    else:
-        if is_empty(ENV_PCK):
-            raise ValueError("ENV_PCK can't be empty")
-
-        ENV_NAME = kwargs.pop('ENV_NAME', '.env')
-        with l_path(ENV_PCK, ENV_NAME) as full_path:
-            d = {**kwargs, 'dotenv_path': full_path}
-
-            load_dotenv(**d)
-
-
-
-class BaseOsEnvrion:
-    DEFAULT_DELIMSEP = _os.pathsep  # ';'
-    DEFAULT_ENVSEP = _os.path.sep  # /
-    DEFAULT_KEYSEP = ','
-
-    def __init__(self, **kwargs):
-        delimsep = kwargs.get('ENV_DELIM_SEP', None)
-        if is_empty(delimsep):
-            delimsep = self.DEFAULT_DELIMSEP
-        self.delimsep = delimsep
-
-        envsep = kwargs.get('ENV_SEP', None)
-        if is_empty(envsep):
-            envsep = self.DEFAULT_ENVSEP
-        self.envsep = envsep
-
-
-        keysep = kwargs.get('ENV_KEY_SEP', None)
-        if is_empty(keysep):
-            keysep = self.DEFAULT_KEYSEP
-        self.keysep = keysep
-
-        env_keys = kwargs.get('ENV_KEYS', None) # 'KEY'
-        if is_empty(env_keys):
-            raise ValueError('ENV_KEYS is not found in kwargs')
-        self.env_keys = self._str_to_list(self.keysep, env_keys)
-
-    def _str_to_list(self, sep, value):
-        ret = [w.strip() for w in value.split(sep)]
-        return ret
-
-    def _list_to_str(self, sep, *args):
-        ret = sep.join([*args])
-        return ret
-
-
-class OsEnvrionPathExpender(BaseOsEnvrion):
-
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-
-        pck = kwargs.get('ENV_MAIN_PCK', None)
-        if is_empty(pck):
-            raise ValueError('ENV_MAIN_PCK is not found in kwargs')
-
-        self.pck = pck
-
-    def fix_abs_path(self):
-        l_path = path()
-
-        with l_path(self.pck, '__init__.py') as init_file:
-            full_prefix = str(init_file.parent.parent)
-
-            for env_key in self.env_keys:
-                rel_paths = self._str_to_list(self.delimsep, _os.environ[env_key])
-
-                buffersize = 0 if rel_paths is None else len(rel_paths)
-                env_values = deque(maxlen=buffersize)
-
-                for rel_path in rel_paths:
-                    abs_path = self._list_to_str(self.envsep, *[full_prefix, rel_path])
-                    env_values.append(abs_path)
-
-                values = self._list_to_str(self.delimsep, *env_values)
-                _os.environ[env_key] = values
-
-
-class OsEnvrionPathRetry(BaseOsEnvrion):
-
-    def fix_retry_path(self):
-        from pathlib import Path
-
-        for env_key in self.env_keys:
-            env_paths = self._str_to_list(self.delimsep, _os.environ[env_key])
-
-            buffersize = 0 if env_paths is None else len(env_paths)
-            env_values = deque(maxlen=buffersize)
-
-            for env_path in env_paths:
-                is_too_short = len(env_path) == 1 and env_path != '/' and env_path != '\\'
-                if is_too_short:
-                    continue
-
-                env_path_p = Path(env_path)
-                is_exists = env_path_p.exists()
-
-                if not is_exists:
-                    drive = env_path_p.drive
-                    if len(drive) == 2 and drive[1] == ':':
-                        env_path_p = env_path_p.as_posix()[2:]
-
-                env_values.append(str(env_path_p))
-
-            values = self._list_to_str(self.delimsep, *env_values)
-            _os.environ[env_key] = values
-
-
-
-def fix_env(**kwargs):
-    """
-    This method "fixes" os.environ relatively to the given ENV_MAIN_PCK package.
-    This method ignores current working directory or __main__ module's __file__ atrribute.
-    For each key in ENV_KEYS, this method prepends full_prefix to os.environ[key].
-    full_prefix is calculated as absolute path of __init__.py of ENV_MAIN_PCK.
-
-
-
-    :param ENV_KEYS keys of os.environ which will be fixed.
-    :param ENV_MAIN_PCK: package to calcualte full_prefix.
-    :param ENV_KEY_SEP: seperator used in ENV_PCK. Optional. Default is ','
-    :param ENV_SEP: seperator that is used inside path. Optional. Default is os.path.sep.
-    :param ENV_DELIM_SEP: seperator that is used inside os.environ. Optional. Default is os.pathsep.
-    :param cls: class or str with implementation logic. Optional. Default is OsEnvrionPathExpender.
-    """
-
-    cls = kwargs.pop('cls', OsEnvrionPathExpender)
-    if isinstance(cls, str):
-        cls = importer(cls)
-    expender = cls(**kwargs)
-    expender.fix_abs_path()
-
-
-def fix_retry_env(**kwargs):
-    """
-    This method "fixes" os.environ making path to Work both on Windows and Linux.
-
-    For each key in ENV_KEYS, this method check if the value can be successfully resolved
-    as path. If so, it does nothing. Otherwise, it strip away the drive part (i.e. C:\\)
-    changing os.environ entry.
-
-
-    :param ENV_KEYS keys of os.environ which will be "fixed".
-    :param ENV_KEY_SEP: seperator used in ENV_PCK. Optional. Default is ','
-    :param ENV_SEP: seperator that is used inside path. Optional. Default is os.path.sep.
-    :param ENV_DELIM_SEP: seperator that is used inside os.environ. Optional. Default is os.pathsep.
-    :param cls: class or str with implementation logic. Optional. Default is OsEnvrionPathRetry.
-    """
-
-    cls = kwargs.pop('cls', OsEnvrionPathRetry)
-    if isinstance(cls, str):
-        cls = importer(cls)
-    path_retry = cls(**kwargs)
-    path_retry.fix_retry_path()
-
-
-@contextlib.contextmanager
-def FixRelCwd(relPackage, logger=None):
-    """
-    This context-manager temporary changes current working directory to the one where relPackage is installed.
-    If relPackage is Python script (or main method of entire application) that relies on relative path,
-    for example, in order to get some resource from the file-system (for example, some configuration file,
-    that lies in the same directory as relPackage) and you want to call relPackage from another directory, this
-    context-manager makes relPackage 'just work'.
-
-    :param relPackage: - installed package
-    :param logger: - optionally, logger to be used, if not specified, default one will be used.
-    :return:
-    """
-    if logger is None:
-        logger = logging.getLogger(__name__)
-    logger.debug(f"cwd is {_os.getcwd()}")
-
-    main_module = _sys.modules['__main__']
-
-    if _is_interactive(main_module) or getattr(_sys, 'frozen', False):
-        # Should work without __file__, e.g. in REPL or IPython notebook.
-        pass
-    else:
-        try:
-            cwd = _os.getcwd()
-            dir = _os.path.dirname(_os.path.realpath(relPackage.__file__))
-            logger.debug(f"Going to change os.chdir('{dir}')")
-            _os.chdir(dir)
-            yield dir
-        finally:
-             _os.chdir(cwd)
-
-@contextlib.contextmanager
-def GuardedWorkerException(logger=None, suppress=False, default_exc_message="Worker failed"):
-    """
-    surround with try-except because of worker exceptions cause the pool.join() to halt forever - and thus memory leak!
-
-    It is very difficult if not impossible to pickle 'exceptions' back to the parent process.
-    Simple ones work, but many others don't.
-    For example, CalledProcessError is not pickable (my guess, this is because of stdout, stderr data-members).
-
-    see https://stackoverflow.com/questions/15314189/python-multiprocessing-pool-hangs-at-join
-    see https://bugs.python.org/issue9400
-
-    This bug still exists in Python 3.
-
-    :param logger to log the exception. If None, exception will be logged to sys.stderr.
-    :param suppress whether to suppress exception. Default False - Exception with default_exc_message
-    will be raised.
-    :param default_exc_message. If suppress is False, this will be used as message for Exception.
-    """
-    try:
-        yield None
-    except Exception as e:
-        if logger is None:
-            import traceback
-            print("Caught exception in worker proccess", file=_sys.stderr)
-            traceback.print_exc(file=_sys.stderr)
-        else:
-            logger.error("Caught exception in worker proccess", exc_info=e)
-        if not suppress:
-            raise Exception(default_exc_message)
+import logging
+
+import os as _os
+import sys as _sys
+import contextlib
+from collections import deque
+from .parsers import is_empty
+from .importer import importer
+
+logger = logging.getLogger(__name__)
+
+
+# inspider by https://github.com/theskumar/python-dotenv/blob/12439aac2d7c98b5acaf51ae3044b1659dc086ae/src/dotenv/main.py#L250
+def _is_interactive(module):
+    """ Decide whether this is running in a REPL or IPython notebook """
+    return not hasattr(module, '__file__')
+
+
+def fixabscwd():
+    """
+    See here https://medium.com/@alex_ber/making-relative-path-to-file-to-work-d5d0f1da67bf for documentation.
+    """
+    logger.info(f"cwd is {_os.getcwd()}")
+
+    main_module = _sys.modules['__main__']
+
+    if _is_interactive(main_module) or getattr(_sys, 'frozen', False):
+        # Should work without __file__, e.g. in REPL or IPython notebook.
+        pass
+    else:
+        main_dir = _os.path.dirname(_os.path.realpath(main_module.__file__))
+
+        logger.info(f"Going to change os.chdir('{main_dir}')")
+
+        _os.chdir(main_dir)
+
+def path():
+    """
+    For older Python version uses`importlib_resources` module.
+    For newer version built in `importlib.resources`.
+    :return:
+    """
+    if _sys.version_info >= (3, 7):
+        from importlib.resources import path as _path
+    else:
+        try:
+            from importlib_resources import path as _path
+        except ImportError:
+            import warnings
+
+            warning = (
+                "You appear to be missing some optional dependencies (importlib_resources);"
+            )
+            warnings.warn(warning, ImportWarning)
+            raise
+    return _path
+
+
+def load_env(**kwargs):
+    """
+    Convenient method from loading environment variables
+    inside packed format (eggs, etc).
+
+    if dotenv_path or stream is present it will be used.
+    if ENV_PCK is present, dotenv_path will be constructed from ENV_PCK and ENV_NAME.
+    Otherwise, kwargs will be forwarded as is to load_dotenv.
+
+
+    Implementaion note:
+    If available it uses importlib.resources API,
+    if not it assumes existence of backport of importlib_resources.
+
+    :param ENV_PCK: package where to find .env file Optional.
+    :param ENV_NAME: Name of .env file. Optional.
+    :param dotenv_path:  absolute or relative path to .env file. Optional.
+    :param stream: `StringIO` object with .env content. Optional.
+    :return:
+    """
+
+    # os.environ['AWS_DEFAULT_REGION'] = 'eu-central-1'
+    try:
+        from dotenv import load_dotenv
+    except ImportError:
+        import warnings
+
+
+        warning = (
+            "You appear to be missing some optional dependencies (python-dotenv);"
+            "please 'python3 -m pip install alex-ber-utils[python-dotenv]'."
+        )
+
+        warnings.warn(warning, ImportWarning)
+        raise
+
+    l_path = path()
+
+    dotenv_path = kwargs.get('dotenv_path', None)
+    stream = kwargs.get('stream', None)
+    ENV_PCK = kwargs.pop('ENV_PCK', None)
+
+    if not is_empty(dotenv_path) or not is_empty(stream) or \
+            (is_empty(dotenv_path) and is_empty(stream) and is_empty(ENV_PCK)):
+        load_dotenv(**kwargs)
+
+    else:
+        if is_empty(ENV_PCK):
+            raise ValueError("ENV_PCK can't be empty")
+
+        ENV_NAME = kwargs.pop('ENV_NAME', '.env')
+        with l_path(ENV_PCK, ENV_NAME) as full_path:
+            d = {**kwargs, 'dotenv_path': full_path}
+
+            load_dotenv(**d)
+
+
+
+class BaseOsEnvrion:
+    DEFAULT_DELIMSEP = _os.pathsep  # ';'
+    DEFAULT_ENVSEP = _os.path.sep  # /
+    DEFAULT_KEYSEP = ','
+
+    def __init__(self, **kwargs):
+        delimsep = kwargs.get('ENV_DELIM_SEP', None)
+        if is_empty(delimsep):
+            delimsep = self.DEFAULT_DELIMSEP
+        self.delimsep = delimsep
+
+        envsep = kwargs.get('ENV_SEP', None)
+        if is_empty(envsep):
+            envsep = self.DEFAULT_ENVSEP
+        self.envsep = envsep
+
+
+        keysep = kwargs.get('ENV_KEY_SEP', None)
+        if is_empty(keysep):
+            keysep = self.DEFAULT_KEYSEP
+        self.keysep = keysep
+
+        env_keys = kwargs.get('ENV_KEYS', None) # 'KEY'
+        if is_empty(env_keys):
+            raise ValueError('ENV_KEYS is not found in kwargs')
+        self.env_keys = self._str_to_list(self.keysep, env_keys)
+
+    def _str_to_list(self, sep, value):
+        ret = [w.strip() for w in value.split(sep)]
+        return ret
+
+    def _list_to_str(self, sep, *args):
+        ret = sep.join([*args])
+        return ret
+
+
+class OsEnvrionPathExpender(BaseOsEnvrion):
+
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+
+        pck = kwargs.get('ENV_MAIN_PCK', None)
+        if is_empty(pck):
+            raise ValueError('ENV_MAIN_PCK is not found in kwargs')
+
+        self.pck = pck
+
+    def fix_abs_path(self):
+        l_path = path()
+
+        with l_path(self.pck, '__init__.py') as init_file:
+            full_prefix = str(init_file.parent.parent)
+
+            for env_key in self.env_keys:
+                rel_paths = self._str_to_list(self.delimsep, _os.environ[env_key])
+
+                buffersize = 0 if rel_paths is None else len(rel_paths)
+                env_values = deque(maxlen=buffersize)
+
+                for rel_path in rel_paths:
+                    abs_path = self._list_to_str(self.envsep, *[full_prefix, rel_path])
+                    env_values.append(abs_path)
+
+                values = self._list_to_str(self.delimsep, *env_values)
+                _os.environ[env_key] = values
+
+
+class OsEnvrionPathRetry(BaseOsEnvrion):
+
+    def fix_retry_path(self):
+        from pathlib import Path
+
+        for env_key in self.env_keys:
+            env_paths = self._str_to_list(self.delimsep, _os.environ[env_key])
+
+            buffersize = 0 if env_paths is None else len(env_paths)
+            env_values = deque(maxlen=buffersize)
+
+            for env_path in env_paths:
+                is_too_short = len(env_path) == 1 and env_path != '/' and env_path != '\\'
+                if is_too_short:
+                    continue
+
+                env_path_p = Path(env_path)
+                is_exists = env_path_p.exists()
+
+                if not is_exists:
+                    drive = env_path_p.drive
+                    if len(drive) == 2 and drive[1] == ':':
+                        env_path_p = env_path_p.as_posix()[2:]
+
+                env_values.append(str(env_path_p))
+
+            values = self._list_to_str(self.delimsep, *env_values)
+            _os.environ[env_key] = values
+
+
+
+def fix_env(**kwargs):
+    """
+    This method "fixes" os.environ relatively to the given ENV_MAIN_PCK package.
+    This method ignores current working directory or __main__ module's __file__ atrribute.
+    For each key in ENV_KEYS, this method prepends full_prefix to os.environ[key].
+    full_prefix is calculated as absolute path of __init__.py of ENV_MAIN_PCK.
+
+
+
+    :param ENV_KEYS keys of os.environ which will be fixed.
+    :param ENV_MAIN_PCK: package to calcualte full_prefix.
+    :param ENV_KEY_SEP: seperator used in ENV_PCK. Optional. Default is ','
+    :param ENV_SEP: seperator that is used inside path. Optional. Default is os.path.sep.
+    :param ENV_DELIM_SEP: seperator that is used inside os.environ. Optional. Default is os.pathsep.
+    :param cls: class or str with implementation logic. Optional. Default is OsEnvrionPathExpender.
+    """
+
+    cls = kwargs.pop('cls', OsEnvrionPathExpender)
+    if isinstance(cls, str):
+        cls = importer(cls)
+    expender = cls(**kwargs)
+    expender.fix_abs_path()
+
+
+def fix_retry_env(**kwargs):
+    """
+    This method "fixes" os.environ making path to Work both on Windows and Linux.
+
+    For each key in ENV_KEYS, this method check if the value can be successfully resolved
+    as path. If so, it does nothing. Otherwise, it strip away the drive part (i.e. C:\\)
+    changing os.environ entry.
+
+
+    :param ENV_KEYS keys of os.environ which will be "fixed".
+    :param ENV_KEY_SEP: seperator used in ENV_PCK. Optional. Default is ','
+    :param ENV_SEP: seperator that is used inside path. Optional. Default is os.path.sep.
+    :param ENV_DELIM_SEP: seperator that is used inside os.environ. Optional. Default is os.pathsep.
+    :param cls: class or str with implementation logic. Optional. Default is OsEnvrionPathRetry.
+    """
+
+    cls = kwargs.pop('cls', OsEnvrionPathRetry)
+    if isinstance(cls, str):
+        cls = importer(cls)
+    path_retry = cls(**kwargs)
+    path_retry.fix_retry_path()
+
+
+@contextlib.contextmanager
+def FixRelCwd(relPackage, logger=None):
+    """
+    This context-manager temporary changes current working directory to the one where relPackage is installed.
+    If relPackage is Python script (or main method of entire application) that relies on relative path,
+    for example, in order to get some resource from the file-system (for example, some configuration file,
+    that lies in the same directory as relPackage) and you want to call relPackage from another directory, this
+    context-manager makes relPackage 'just work'.
+
+    :param relPackage: - installed package
+    :param logger: - optionally, logger to be used, if not specified, default one will be used.
+    :return:
+    """
+    if logger is None:
+        logger = logging.getLogger(__name__)
+    logger.debug(f"cwd is {_os.getcwd()}")
+
+    main_module = _sys.modules['__main__']
+
+    if _is_interactive(main_module) or getattr(_sys, 'frozen', False):
+        # Should work without __file__, e.g. in REPL or IPython notebook.
+        pass
+    else:
+        try:
+            cwd = _os.getcwd()
+            dir = _os.path.dirname(_os.path.realpath(relPackage.__file__))
+            logger.debug(f"Going to change os.chdir('{dir}')")
+            _os.chdir(dir)
+            yield dir
+        finally:
+             _os.chdir(cwd)
+
+@contextlib.contextmanager
+def GuardedWorkerException(logger=None, suppress=False, default_exc_message="Worker failed"):
+    """
+    surround with try-except because of worker exceptions cause the pool.join() to halt forever - and thus memory leak!
+
+    It is very difficult if not impossible to pickle 'exceptions' back to the parent process.
+    Simple ones work, but many others don't.
+    For example, CalledProcessError is not pickable (my guess, this is because of stdout, stderr data-members).
+
+    see https://stackoverflow.com/questions/15314189/python-multiprocessing-pool-hangs-at-join
+    see https://bugs.python.org/issue9400
+
+    This bug still exists in Python 3.
+
+    :param logger to log the exception. If None, exception will be logged to sys.stderr.
+    :param suppress whether to suppress exception. Default False - Exception with default_exc_message
+    will be raised.
+    :param default_exc_message. If suppress is False, this will be used as message for Exception.
+    """
+    try:
+        yield None
+    except Exception as e:
+        if logger is None:
+            import traceback
+            print("Caught exception in worker proccess", file=_sys.stderr)
+            traceback.print_exc(file=_sys.stderr)
+        else:
+            logger.error("Caught exception in worker proccess", exc_info=e)
+        if not suppress:
+            raise Exception(default_exc_message)
```

### Comparing `alex_ber_utils-0.6.6b3/alexber/utils/parsers.py` & `alex_ber_utils-0.7.0/alexber/utils/parsers.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,153 +1,153 @@
-"""
-See https://medium.com/analytics-vidhya/my-parser-module-429ed1457718 for documentation.
-"""
-import logging
-logger = logging.getLogger(__name__)
-from collections import OrderedDict
-
-from configparser import ConfigParser
-from argparse import ArgumentParser
-import sys
-import ast
-
-
-def _as_dict(parser):
-    """
-    Go over all sections in the parser,
-    convert's there's key/value as dictionary that
-    for every section in the parser has dictionary
-    with key/value pairs (both str).
-
-    :param parser: (self)
-    :return: dict with key/value as str
-    """
-    d = OrderedDict()
-    for section in parser.sections():
-        d[section] = OrderedDict()
-        for key in parser.options(section):
-            d[section][key] = parser.get(section, key)
-    return d
-
-ConfigParser.as_dict = _as_dict
-
-#inspired by
-#https://stackoverflow.com/questions/21920989/parse-non-pre-defined-argument
-#https://stackoverflow.com/questions/51267814/argparse-for-unknown-number-of-arguments-and-unknown-names
-def _args_as_dict(parser, args=None):
-    """
-    Go over source for arguments, takes argument of the form --key=value.
-    Create dictionary.
-    Strip out '--' prefix from the key and put key/value (as str) to dict.
-
-    If args is None, sys.argv[1:] will be used as source for arguments.
-    Note: sys.argv[0] is ignored as it contain the name of main .py file to run.
-
-    :param parser: ArgumentParser (self)
-    :param args: if is not None, will be used as source for arguments.
-    :return:
-    """
-
-    #see #argumentParser.parse_known_args()
-    if args is None:
-        # args default to the system args
-        args = sys.argv[1:]
-    else:
-        # make sure that args are mutable
-        args = list(args)
-
-    d = OrderedDict()
-
-    key = None
-    value = None
-    for arg in args:
-        if arg.startswith('--') and '=' in arg:
-            key, value = arg.rsplit("=", 1)
-        else:
-            key = arg
-            value = None
-        if key.startswith('--'):
-            key = key[2:]
-
-        d[key] = value
-
-    return d
-
-
-ArgumentParser.as_dict = _args_as_dict
-
-
-#insipred by https://stackoverflow.com/a/14258151/1137529
-#
-def safe_eval(value):
-    '''
-    The purpose of this function is convert numbers from str to correct type.
-    This function support convertion of built-in Python number to correct type (int, float)
-    This function doesn't support decimal.Decimal or datetime.datetime or numpy types.
-    '''
-    try:
-        ret = ast.literal_eval(value)
-    except (SyntaxError, ValueError):
-        ret = value
-    return ret
-
-def is_empty(value):
-    '''
-    if value is None returns True.
-
-    if value is empty iterable (for example, empty str or emptry list),
-    returns true
-    otherwise false
-
-    Note: For not iterable values, behaivour is undefined.
-
-    :param value:
-    :return:
-    '''
-    if value is None:
-        return True
-    if value:
-        ret = False
-    else:
-        ret = True
-    return ret
-
-
-def parse_boolean(value):
-    '''
-    if value is None returns None.
-
-    if value is boolean, it is returned as it is.
-    if value is str and value is equals ignoring case to "True", True is returned.
-    if value is str and value is equals ignoring case to "False", False is returned.
-
-    For every other value, the answer is undefined.
-
-    :param value:
-    :return:
-    '''
-    if value is None:
-        return None
-
-    if value in (True, False):
-        return value
-    try:
-        return {"true": True, "false": False}[value.casefold()]
-    except (AttributeError, KeyError):
-        raise ValueError(f"unknown string for bool: {value!r}")
-
-def parse_sys_args(argumentParser=None, args=None):
-    """
-    This function parses command line arguments.
-
-    :param argumentParser:
-    :param args: if not None, suppresses sys.args
-    :return:
-    """
-    if argumentParser is None:
-        argumentParser = ArgumentParser()
-    argumentParser.add_argument("--general.config.file", nargs='?', dest='config_file', default='config.yml',
-                                const='config.yml')
-    params, unknown_arg = argumentParser.parse_known_args(args=args)
-
-    sys_d = argumentParser.as_dict(args=unknown_arg)
-    return params, sys_d
+"""
+See https://medium.com/analytics-vidhya/my-parser-module-429ed1457718 for documentation.
+"""
+import logging
+logger = logging.getLogger(__name__)
+from collections import OrderedDict
+
+from configparser import ConfigParser
+from argparse import ArgumentParser
+import sys
+import ast
+
+
+def _as_dict(parser):
+    """
+    Go over all sections in the parser,
+    convert's there's key/value as dictionary that
+    for every section in the parser has dictionary
+    with key/value pairs (both str).
+
+    :param parser: (self)
+    :return: dict with key/value as str
+    """
+    d = OrderedDict()
+    for section in parser.sections():
+        d[section] = OrderedDict()
+        for key in parser.options(section):
+            d[section][key] = parser.get(section, key)
+    return d
+
+ConfigParser.as_dict = _as_dict
+
+#inspired by
+#https://stackoverflow.com/questions/21920989/parse-non-pre-defined-argument
+#https://stackoverflow.com/questions/51267814/argparse-for-unknown-number-of-arguments-and-unknown-names
+def _args_as_dict(parser, args=None):
+    """
+    Go over source for arguments, takes argument of the form --key=value.
+    Create dictionary.
+    Strip out '--' prefix from the key and put key/value (as str) to dict.
+
+    If args is None, sys.argv[1:] will be used as source for arguments.
+    Note: sys.argv[0] is ignored as it contain the name of main .py file to run.
+
+    :param parser: ArgumentParser (self)
+    :param args: if is not None, will be used as source for arguments.
+    :return:
+    """
+
+    #see #argumentParser.parse_known_args()
+    if args is None:
+        # args default to the system args
+        args = sys.argv[1:]
+    else:
+        # make sure that args are mutable
+        args = list(args)
+
+    d = OrderedDict()
+
+    key = None
+    value = None
+    for arg in args:
+        if arg.startswith('--') and '=' in arg:
+            key, value = arg.rsplit("=", 1)
+        else:
+            key = arg
+            value = None
+        if key.startswith('--'):
+            key = key[2:]
+
+        d[key] = value
+
+    return d
+
+
+ArgumentParser.as_dict = _args_as_dict
+
+
+#insipred by https://stackoverflow.com/a/14258151/1137529
+#
+def safe_eval(value):
+    '''
+    The purpose of this function is convert numbers from str to correct type.
+    This function support convertion of built-in Python number to correct type (int, float)
+    This function doesn't support decimal.Decimal or datetime.datetime or numpy types.
+    '''
+    try:
+        ret = ast.literal_eval(value)
+    except (SyntaxError, ValueError):
+        ret = value
+    return ret
+
+def is_empty(value):
+    '''
+    if value is None returns True.
+
+    if value is empty iterable (for example, empty str or emptry list),
+    returns true
+    otherwise false
+
+    Note: For not iterable values, behaivour is undefined.
+
+    :param value:
+    :return:
+    '''
+    if value is None:
+        return True
+    if value:
+        ret = False
+    else:
+        ret = True
+    return ret
+
+
+def parse_boolean(value):
+    '''
+    if value is None returns None.
+
+    if value is boolean, it is returned as it is.
+    if value is str and value is equals ignoring case to "True", True is returned.
+    if value is str and value is equals ignoring case to "False", False is returned.
+
+    For every other value, the answer is undefined.
+
+    :param value:
+    :return:
+    '''
+    if value is None:
+        return None
+
+    if value in (True, False):
+        return value
+    try:
+        return {"true": True, "false": False}[value.casefold()]
+    except (AttributeError, KeyError):
+        raise ValueError(f"unknown string for bool: {value!r}")
+
+def parse_sys_args(argumentParser=None, args=None):
+    """
+    This function parses command line arguments.
+
+    :param argumentParser:
+    :param args: if not None, suppresses sys.args
+    :return:
+    """
+    if argumentParser is None:
+        argumentParser = ArgumentParser()
+    argumentParser.add_argument("--general.config.file", nargs='?', dest='config_file', default='config.yml',
+                                const='config.yml')
+    params, unknown_arg = argumentParser.parse_known_args(args=args)
+
+    sys_d = argumentParser.as_dict(args=unknown_arg)
+    return params, sys_d
```

### Comparing `alex_ber_utils-0.6.6b3/alexber/utils/processinvokes.py` & `alex_ber_utils-0.7.0/alexber/utils/processinvokes.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,294 +1,294 @@
-import logging
-import os as _os
-import subprocess
-import threading
-from concurrent.futures import ThreadPoolExecutor
-from . importer import importer
-
-executor = None
-default_log_name  = None
-default_log_level = None
-default_logpipe_cls = None
-default_log_subprocess_cls = None
-
-#inspired by https://codereview.stackexchange.com/questions/6567/redirecting-subprocesses-output-stdout-and-stderr-to-the-logging-module/175382
-#for alternatives see https://gist.github.com/jaketame/3ed43d1c52e9abccd742b1792c449079
-# that is itself adoptation of https://gist.github.com/bgreenlee/1402841
-
-
-class BasePipe(object):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.fdRead, self.fdWrite = _os.pipe()
-        self.fdWriteLock = threading.RLock()
-
-        with self.fdWriteLock:
-            self.is_closed = False
-
-    def fileno(self):
-        """
-        Return the write file descriptor of the pipe
-        """
-        return self.fdWrite
-
-    def processLine(self, line):
-        """
-        Hook to be overridden in the sub-class.
-        """
-        pass
-
-    def run(self):
-        """
-        Run the thread, process output line by line.
-        """
-        with _os.fdopen(self.fdRead) as pipeReader:
-            for line in iter(pipeReader.readline, ''):
-                self.processLine(line)
-
-    def breakPipe(self):
-        self.close()
-
-    def cleanUp(self):
-        """
-        Hook to be overridden in the sub-class.
-        """
-        pass
-
-    def close(self):
-        """
-        Close the write end of the pipe.
-        """
-        with self.fdWriteLock:
-            if not self.is_closed:
-                self.cleanUp()
-                _os.close(self.fdWrite)
-            self.is_closed = True
-
-    def __enter__(self):
-        if self.is_closed:
-            raise ValueError("I/O operation on closed pipe")
-
-        return self
-
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        self.close()
-
-
-class LogPipe(BasePipe):
-    def __init__(self, *args, **kwargs):
-        """
-        Setup the logger with logName and loglevel
-        Create read and write file descriptor of the pipe
-        """
-        logName = kwargs.pop('logName', default_log_name)
-        logLevel = kwargs.pop('logLevel', default_log_level)
-
-        super().__init__(*args, **kwargs)
-
-        self.logger = logging.getLogger(logName)
-
-        self.level = logLevel
-
-    def processLine(self, line):
-        self.logger.log(self.level, line.rstrip('\r\n'))
-
-class FilePipe(BasePipe):
-    def __init__(self, *args, **kwargs):
-        filename = kwargs.pop('fileName', None)
-        if filename is None:
-            raise ValueError('fileName should be specified')
-
-        super().__init__(*args, **kwargs)
-
-        d = {
-            'file': filename,
-            'mode': 'w',
-            **kwargs
-        }
-
-        self.f = open(**d)
-
-    def processLine(self, line):
-        aline = f"{line.rstrip()}\n"
-        self.f.write(aline)
-
-    def cleanUp(self):
-        if self.f is not None:
-            self.f.close()
-
-
-
-
-
-class LogSubProcessCall(object):
-    def __init__(self, *args, **kwargs):
-
-        self.pipe = kwargs.pop('pipe')
-        d = kwargs.pop('popen', {})
-
-        self.popenargs = d.pop('args', [])
-        self.popenkwargs = d.pop('kwargs', {})
-        super().__init__(*args, **kwargs)
-
-    def calc_subprocess_run_kwargs(self):
-        kwargs= {'stdout':self.pipe, 'stderr':subprocess.STDOUT,
-            'text':True, 'bufsize':1, 'check':True,
-                 **self.popenkwargs}
-        return kwargs
-
-    def run_sub_process(self):
-        f = executor.submit(self.pipe.run)
-        try:
-            kwargs = self.calc_subprocess_run_kwargs()
-            process = subprocess.run(self.popenargs, **kwargs)
-        finally:
-            self.pipe.breakPipe()
-            f.result()
-
-
-
-def run_sub_process(*args, **kwargs):
-    """
-    This method run subprocess and logs it's output to the logger.
-    This method is sophisticated decorator to subprocess.run(). It is useful, when your subprocess
-    run's a lot of time and you're interesting to receive it's stdout and stderr. By default, it's streamed to log.
-    You can easily customize this behavior, see `initConig()` method.
-
-    This method is sophisticated decorator to subprocess.run(). See it's docstring for more information. Note, that
-    some parameters (cwd, for example) that can be used in popenkwargs are listed in Popen constructor.
-
-    logPipe is customizable object that essentially forwards output from subprocess to the logger using
-    logName and logLevel (see below).
-
-    default_log_subprocess_cls by default is LogSubProcessCall.
-    default_logpipe_cls by default is LogPipe.
-    logName by default is processinvokes.
-    logLevel by default is logger.INFO.
-    See initConfig() for more details.
-
-    Default parameters for subprocess.run() are (it can be overridden in popenkwargs):
-        'stdout':logPipe,
-        'stderr':STDOUT,
-        'text':True,
-        'bufsize': 1,
-        'check': True
-
-    This means:
-        logPipe is used as subprocess's standard output and standard error.
-        Do decode stdin, stdout and stderr using the given encoding
-          or the system default otherwise.
-        1 is supplied as the buffering argument to the open() function when
-          creating the stdin/stdout/stderr pipe file objects.
-          Essentially, no OS-level buffering between process, provided that call to write contains a newline character.
-        If the exit code of subprocess is non-zero, it raises a CalledProcessError.
-
-    It is generally not advice to override them, but you can if you know, what you're doing.
-
-    :param args: will be passed as popenargs to subprocess.run() method
-    :param roughly kwargs['kwargs'] will be passed as popenkwargs to subprocess.run() method
-    :param roughly kwargs['logPipe']['cls'] or default_logpipe_cls (if first one is empty)
-                                             will be passed as logPipeCls to create logPipe.
-                                             Can be class or str.
-    :param roughly kwargs['logPipe']['kwargs'] will be passed as kwargs to logPipeCls to create logPipe.
-    :param roughly kwargs['logSubprocess']['cls'] or default_log_subprocess_cls (if first one is empty)
-                                             will be passed as logSubProcessCls to create LogSubProcessCall.
-                                              Can be class or str.
-    :param roughly kwargs['logSubprocess']['kwargs'] will be passed as kwargs to logSubprocess.
-
-    :return:
-    """
-    if default_logpipe_cls is None:
-        raise ValueError("default_logpipe_cls can't be None")
-
-    logPipe_p = kwargs.pop('logPipe', {})
-    logPipeCls = logPipe_p.pop('cls', default_logpipe_cls)
-    if isinstance(logPipeCls, str):
-        logPipeCls = importer(logPipeCls)
-
-    logPipeKwargs = logPipe_p.pop('kwargs', {})
-    callKwargs = kwargs.pop('kwargs', {})
-    logSubprocess_p = kwargs.pop('logSubprocess', {})
-    logSubProcessCls = logSubprocess_p.pop('cls', default_log_subprocess_cls)
-    if isinstance(logSubProcessCls, str):
-        logSubProcessCls = importer(logSubProcessCls)
-    logSubprocessKwargs = logSubprocess_p.pop('kwargs', {})
-
-    with logPipeCls(**logPipeKwargs) as logPipe:
-
-        kwargs = {'pipe': logPipe,
-                 'popen':
-                      {'args': args,
-                       'kwargs': callKwargs
-                      },
-                 **logSubprocessKwargs
-                  }
-
-        call = logSubProcessCls(**kwargs)
-        call.run_sub_process()
-
-
-
-def initConfig(**kwargs):
-    """
-    This method can be optionally called prior any call to another function in this module.
-    It is indented to be called in the MainThread.
-    This method can be call with empty params.
-
-    :param default_log_name: Optional. - name of the logger where the messages will be streamed to.
-                Default values is: processinvokes
-    :param default_log_level: Optional. - log level to be used in logger.
-                Default values is: logging.INFO
-    :param default_logpipe_cls: can be class or str. Optional. You can use your custom class for the logging.
-                For example, FilePipe.
-                Default values is: LogPipe
-    :param default_log_subprocess_cls: can be class or str. Optional.
-                Default values is: LogSubProcessCall
-    :param executor: internally used to run sub-process
-                Default values are
-                      'max_workers':1,
-                      'thread_name_prefix': processinvokes
-                This means, by default:
-                    We're using up to 1 worker.
-                    In log message generated from the worker processinvokes-xxx will be used as thread_name.
-
-    If running from the MainThread, this method is idempotent.
-    :return:
-    """
-    default_log_name_p = kwargs.get('default_log_name', None)
-    if default_log_name_p is None:
-        default_log_name_p = __name__
-    global default_log_name
-    default_log_name = default_log_name_p
-
-    default_log_level_p = kwargs.get('default_log_level', None)
-    if default_log_level_p is None:
-        default_log_level_p = logging.INFO
-    global default_log_level
-    default_log_level = default_log_level_p
-
-    default_logpipe_cls_p = kwargs.get('default_logpipe_cls', None)
-    if default_logpipe_cls_p is None:
-        default_logpipe_cls_p = LogPipe
-    elif isinstance(default_logpipe_cls_p, str):
-        default_logpipe_cls_p = importer(default_logpipe_cls_p)
-    global default_logpipe_cls
-    default_logpipe_cls = default_logpipe_cls_p
-
-    default_log_subprocess_cls_p = kwargs.get('default_log_subprocess_cls', None)
-    if default_log_subprocess_cls_p is None:
-        default_log_subprocess_cls_p = LogSubProcessCall
-    elif isinstance(default_log_subprocess_cls_p, str):
-        default_log_subprocess_cls_p = importer(default_log_subprocess_cls_p)
-    global default_log_subprocess_cls
-    default_log_subprocess_cls = default_log_subprocess_cls_p
-
-    executor_d = kwargs.get('executor', {})
-    executor_d = {'max_workers': 1,
-                  'thread_name_prefix': __name__,
-                  **executor_d}
-    global executor
-    if executor is not None:
-        executor.shutdown(wait=False)
-    executor = ThreadPoolExecutor(**executor_d)
-
+import logging
+import os as _os
+import subprocess
+import threading
+from concurrent.futures import ThreadPoolExecutor
+from . importer import importer
+
+executor = None
+default_log_name  = None
+default_log_level = None
+default_logpipe_cls = None
+default_log_subprocess_cls = None
+
+#inspired by https://codereview.stackexchange.com/questions/6567/redirecting-subprocesses-output-stdout-and-stderr-to-the-logging-module/175382
+#for alternatives see https://gist.github.com/jaketame/3ed43d1c52e9abccd742b1792c449079
+# that is itself adoptation of https://gist.github.com/bgreenlee/1402841
+
+
+class BasePipe(object):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.fdRead, self.fdWrite = _os.pipe()
+        self.fdWriteLock = threading.RLock()
+
+        with self.fdWriteLock:
+            self.is_closed = False
+
+    def fileno(self):
+        """
+        Return the write file descriptor of the pipe
+        """
+        return self.fdWrite
+
+    def processLine(self, line):
+        """
+        Hook to be overridden in the sub-class.
+        """
+        pass
+
+    def run(self):
+        """
+        Run the thread, process output line by line.
+        """
+        with _os.fdopen(self.fdRead) as pipeReader:
+            for line in iter(pipeReader.readline, ''):
+                self.processLine(line)
+
+    def breakPipe(self):
+        self.close()
+
+    def cleanUp(self):
+        """
+        Hook to be overridden in the sub-class.
+        """
+        pass
+
+    def close(self):
+        """
+        Close the write end of the pipe.
+        """
+        with self.fdWriteLock:
+            if not self.is_closed:
+                self.cleanUp()
+                _os.close(self.fdWrite)
+            self.is_closed = True
+
+    def __enter__(self):
+        if self.is_closed:
+            raise ValueError("I/O operation on closed pipe")
+
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        self.close()
+
+
+class LogPipe(BasePipe):
+    def __init__(self, *args, **kwargs):
+        """
+        Setup the logger with logName and loglevel
+        Create read and write file descriptor of the pipe
+        """
+        logName = kwargs.pop('logName', default_log_name)
+        logLevel = kwargs.pop('logLevel', default_log_level)
+
+        super().__init__(*args, **kwargs)
+
+        self.logger = logging.getLogger(logName)
+
+        self.level = logLevel
+
+    def processLine(self, line):
+        self.logger.log(self.level, line.rstrip('\r\n'))
+
+class FilePipe(BasePipe):
+    def __init__(self, *args, **kwargs):
+        filename = kwargs.pop('fileName', None)
+        if filename is None:
+            raise ValueError('fileName should be specified')
+
+        super().__init__(*args, **kwargs)
+
+        d = {
+            'file': filename,
+            'mode': 'w',
+            **kwargs
+        }
+
+        self.f = open(**d)
+
+    def processLine(self, line):
+        aline = f"{line.rstrip()}\n"
+        self.f.write(aline)
+
+    def cleanUp(self):
+        if self.f is not None:
+            self.f.close()
+
+
+
+
+
+class LogSubProcessCall(object):
+    def __init__(self, *args, **kwargs):
+
+        self.pipe = kwargs.pop('pipe')
+        d = kwargs.pop('popen', {})
+
+        self.popenargs = d.pop('args', [])
+        self.popenkwargs = d.pop('kwargs', {})
+        super().__init__(*args, **kwargs)
+
+    def calc_subprocess_run_kwargs(self):
+        kwargs= {'stdout':self.pipe, 'stderr':subprocess.STDOUT,
+            'text':True, 'bufsize':1, 'check':True,
+                 **self.popenkwargs}
+        return kwargs
+
+    def run_sub_process(self):
+        f = executor.submit(self.pipe.run)
+        try:
+            kwargs = self.calc_subprocess_run_kwargs()
+            process = subprocess.run(self.popenargs, **kwargs)
+        finally:
+            self.pipe.breakPipe()
+            f.result()
+
+
+
+def run_sub_process(*args, **kwargs):
+    """
+    This method run subprocess and logs it's output to the logger.
+    This method is sophisticated decorator to subprocess.run(). It is useful, when your subprocess
+    run's a lot of time and you're interesting to receive it's stdout and stderr. By default, it's streamed to log.
+    You can easily customize this behavior, see `initConig()` method.
+
+    This method is sophisticated decorator to subprocess.run(). See it's docstring for more information. Note, that
+    some parameters (cwd, for example) that can be used in popenkwargs are listed in Popen constructor.
+
+    logPipe is customizable object that essentially forwards output from subprocess to the logger using
+    logName and logLevel (see below).
+
+    default_log_subprocess_cls by default is LogSubProcessCall.
+    default_logpipe_cls by default is LogPipe.
+    logName by default is processinvokes.
+    logLevel by default is logger.INFO.
+    See initConfig() for more details.
+
+    Default parameters for subprocess.run() are (it can be overridden in popenkwargs):
+        'stdout':logPipe,
+        'stderr':STDOUT,
+        'text':True,
+        'bufsize': 1,
+        'check': True
+
+    This means:
+        logPipe is used as subprocess's standard output and standard error.
+        Do decode stdin, stdout and stderr using the given encoding
+          or the system default otherwise.
+        1 is supplied as the buffering argument to the open() function when
+          creating the stdin/stdout/stderr pipe file objects.
+          Essentially, no OS-level buffering between process, provided that call to write contains a newline character.
+        If the exit code of subprocess is non-zero, it raises a CalledProcessError.
+
+    It is generally not advice to override them, but you can if you know, what you're doing.
+
+    :param args: will be passed as popenargs to subprocess.run() method
+    :param roughly kwargs['kwargs'] will be passed as popenkwargs to subprocess.run() method
+    :param roughly kwargs['logPipe']['cls'] or default_logpipe_cls (if first one is empty)
+                                             will be passed as logPipeCls to create logPipe.
+                                             Can be class or str.
+    :param roughly kwargs['logPipe']['kwargs'] will be passed as kwargs to logPipeCls to create logPipe.
+    :param roughly kwargs['logSubprocess']['cls'] or default_log_subprocess_cls (if first one is empty)
+                                             will be passed as logSubProcessCls to create LogSubProcessCall.
+                                              Can be class or str.
+    :param roughly kwargs['logSubprocess']['kwargs'] will be passed as kwargs to logSubprocess.
+
+    :return:
+    """
+    if default_logpipe_cls is None:
+        raise ValueError("default_logpipe_cls can't be None")
+
+    logPipe_p = kwargs.pop('logPipe', {})
+    logPipeCls = logPipe_p.pop('cls', default_logpipe_cls)
+    if isinstance(logPipeCls, str):
+        logPipeCls = importer(logPipeCls)
+
+    logPipeKwargs = logPipe_p.pop('kwargs', {})
+    callKwargs = kwargs.pop('kwargs', {})
+    logSubprocess_p = kwargs.pop('logSubprocess', {})
+    logSubProcessCls = logSubprocess_p.pop('cls', default_log_subprocess_cls)
+    if isinstance(logSubProcessCls, str):
+        logSubProcessCls = importer(logSubProcessCls)
+    logSubprocessKwargs = logSubprocess_p.pop('kwargs', {})
+
+    with logPipeCls(**logPipeKwargs) as logPipe:
+
+        kwargs = {'pipe': logPipe,
+                 'popen':
+                      {'args': args,
+                       'kwargs': callKwargs
+                      },
+                 **logSubprocessKwargs
+                  }
+
+        call = logSubProcessCls(**kwargs)
+        call.run_sub_process()
+
+
+
+def initConfig(**kwargs):
+    """
+    This method can be optionally called prior any call to another function in this module.
+    It is indented to be called in the MainThread.
+    This method can be call with empty params.
+
+    :param default_log_name: Optional. - name of the logger where the messages will be streamed to.
+                Default values is: processinvokes
+    :param default_log_level: Optional. - log level to be used in logger.
+                Default values is: logging.INFO
+    :param default_logpipe_cls: can be class or str. Optional. You can use your custom class for the logging.
+                For example, FilePipe.
+                Default values is: LogPipe
+    :param default_log_subprocess_cls: can be class or str. Optional.
+                Default values is: LogSubProcessCall
+    :param executor: internally used to run sub-process
+                Default values are
+                      'max_workers':1,
+                      'thread_name_prefix': processinvokes
+                This means, by default:
+                    We're using up to 1 worker.
+                    In log message generated from the worker processinvokes-xxx will be used as thread_name.
+
+    If running from the MainThread, this method is idempotent.
+    :return:
+    """
+    default_log_name_p = kwargs.get('default_log_name', None)
+    if default_log_name_p is None:
+        default_log_name_p = __name__
+    global default_log_name
+    default_log_name = default_log_name_p
+
+    default_log_level_p = kwargs.get('default_log_level', None)
+    if default_log_level_p is None:
+        default_log_level_p = logging.INFO
+    global default_log_level
+    default_log_level = default_log_level_p
+
+    default_logpipe_cls_p = kwargs.get('default_logpipe_cls', None)
+    if default_logpipe_cls_p is None:
+        default_logpipe_cls_p = LogPipe
+    elif isinstance(default_logpipe_cls_p, str):
+        default_logpipe_cls_p = importer(default_logpipe_cls_p)
+    global default_logpipe_cls
+    default_logpipe_cls = default_logpipe_cls_p
+
+    default_log_subprocess_cls_p = kwargs.get('default_log_subprocess_cls', None)
+    if default_log_subprocess_cls_p is None:
+        default_log_subprocess_cls_p = LogSubProcessCall
+    elif isinstance(default_log_subprocess_cls_p, str):
+        default_log_subprocess_cls_p = importer(default_log_subprocess_cls_p)
+    global default_log_subprocess_cls
+    default_log_subprocess_cls = default_log_subprocess_cls_p
+
+    executor_d = kwargs.get('executor', {})
+    executor_d = {'max_workers': 1,
+                  'thread_name_prefix': __name__,
+                  **executor_d}
+    global executor
+    if executor is not None:
+        executor.shutdown(wait=False)
+    executor = ThreadPoolExecutor(**executor_d)
+
 initConfig()
```

### Comparing `alex_ber_utils-0.6.6b3/alexber/utils/props.py` & `alex_ber_utils-0.7.0/alexber/utils/props.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,353 +1,353 @@
-
-
-
-"""
-A Python replacement for java.util.Properties class
-This is modelled as closely as possible to the Java original.
-
-Created - Anand B Pillai <abpillai@gmail.com>,
-Update to Python 3 by Alex.
-Also there are some tweeks that was done by Alex.
-"""
-
-# see https://code.activestate.com/recipes/496795-a-python-replacement-for-javautilproperties/
-import sys
-import re
-import time
-from collections import OrderedDict
-
-
-class IllegalArgumentException(Exception):
-
-    def __init__(self, lineno, msg):
-        self.lineno = lineno
-        self.msg = msg
-
-    def __str__(self):
-        s='Exception at line number %d => %s' % (self.lineno, self.msg)
-        return s
-                 
-class Properties(object):
-    """ A Python replacement for java.util.Properties """
-    # Alex fix, handle ${}
-    #curlies = re.compile('\\${.+?}')
-    PLACEHOLDER_TOKEN = '$'
-
-    def __init__(self, props=None):
-
-        # Note: We don't take a default properties object
-        # as argument yet
-
-        # Dictionary of properties.
-        # Alex changed {} to OrderedDict
-        self._props = OrderedDict()
-        # Dictionary of properties with 'pristine' keys
-        # This is used for dumping the properties to a file
-        # using the 'store' method
-        # Alex changed {} to OrderedDict
-        self._origprops = OrderedDict()
-
-        # Dictionary mapping keys from property
-        # dictionary to pristine dictionary
-        # Alex changed {} to OrderedDict
-        self._keymap = OrderedDict()
-        # Alex changed {} to OrderedDict
-        self._unresolved = OrderedDict()
-        
-        self.othercharre = re.compile(r'(?<!\\)(\s*\=)|(?<!\\)(\s*\:)')
-        self.othercharre2 = re.compile(r'(\s*\=)|(\s*\:)')
-        self.bspacere = re.compile(r'\\(?!\s$)')
-        
-    def __str__(self):
-        s='{'
-        for key,value in self._props.items():
-            s = ''.join((s,key,'=',value,', '))
-
-        s=''.join((s[:-2],'}'))
-        return s
-
-    def __parse(self, lines):
-        """ Parse a list of lines and create
-        an internal property dictionary """
-
-        # Every line in the file must consist of either a comment
-        # or a key-value pair. A key-value pair is a line consisting
-        # of a key which is a combination of non-white space characters
-        # The separator character between key-value pairs is a '=',
-        # ':' or a whitespace character not including the newline.
-        # If the '=' or ':' characters are found, in the line, even
-        # keys containing whitespace chars are allowed.
-
-        # A line with only a key according to the rules above is also
-        # fine. In such case, the value is considered as the empty string.
-         # In order to include characters '=' or ':' in a key or value,
-        # they have to be properly escaped using the backslash character.
-
-        # Some examples of valid key-value pairs:
-        #
-        # key     value
-        # key=value
-        # key:value
-        # key     value1,value2,value3
-        # key     value1,value2,value3 \
-        #         value4, value5
-        # key
-        # This key= this value
-        # key = value1 value2 value3
-        
-        # Any line that starts with a '#' is considerered a comment
-        # and skipped. Also any trailing or preceding whitespaces
-        # are removed from the key/value.
-        
-        # This is a line parser. It parses the
-        # contents like by line.
-
-        lineno=0
-        i = iter(lines)
-
-        for line in i:
-            lineno += 1
-            line = line.strip()
-            # Skip null lines
-            if not line: continue
-            # Skip lines which are comments
-            if line[0] == '#': continue
-            # Some flags
-            escaped=False
-            # Position of first separation char
-            sepidx = -1
-            # A flag for performing wspace re check
-            flag = 0
-            # Check for valid space separation
-            # First obtain the max index to which we
-            # can search.
-            m = self.othercharre.search(line)
-            if m:
-                first, last = m.span()
-                start, end = 0, first
-                flag = 1
-                wspacere = re.compile(r'(?<![\\\=\:])(\s)')        
-            else:
-                if self.othercharre2.search(line):
-                    # Check if either '=' or ':' is present
-                    # in the line. If they are then it means
-                    # they are preceded by a backslash.
-                    
-                    # This means, we need to modify the
-                    # wspacere a bit, not to look for
-                    # : or = characters.
-                    wspacere = re.compile(r'(?<![\\])(\s)')        
-                start, end = 0, len(line)
-                
-            m2 = wspacere.search(line, start, end)
-            if m2:
-                # print 'Space match=>',line
-                # Means we need to split by space.
-                first, last = m2.span()
-                sepidx = first
-            elif m:
-                # print 'Other match=>',line
-                # No matching wspace char found, need
-                # to split by either '=' or ':'
-                first, last = m.span()
-                sepidx = last - 1
-                # print line[sepidx]
-                
-                
-            # If the last character is a backslash
-            # it has to be preceded by a space in which
-            # case the next line is read as part of the
-            # same property
-            while line[-1] == '\\':
-                # Read next line
-                nextline = i.next()
-                nextline = nextline.strip()
-                lineno += 1
-                # This line will become part of the value
-                line = line[:-1] + nextline
-
-            # Now split to key,value according to separation char
-            if sepidx != -1:
-                key, value = line[:sepidx], line[sepidx+1:]
-            else:
-                key,value = line,''
-
-            self.processPair(key, value)
-            
-    def processPair(self, key, value):
-        """ Process a (key, value) pair """
-
-        oldkey = key
-        oldvalue = value
-        
-        # Create key intelligently
-        keyparts = self.bspacere.split(key)
-        # print keyparts
-
-        strippable = False
-        lastpart = keyparts[-1]
-
-        if lastpart.find('\\ ') != -1:
-            keyparts[-1] = lastpart.replace('\\','')
-
-        # If no backspace is found at the end, but empty
-        # space is found, strip it
-        elif lastpart and lastpart[-1] == ' ':
-            strippable = True
-
-        key = ''.join(keyparts)
-        if strippable:
-            key = key.strip()
-            oldkey = oldkey.strip()
-        
-        oldvalue = self.unescape(oldvalue)
-        value = self.unescape(value)
-        
-        # Alex fix, handle ${}
-        _regex ='\\${.+?}'
-        if '$' != Properties.PLACEHOLDER_TOKEN:
-            _regex = _regex[0:1] + Properties.PLACEHOLDER_TOKEN + _regex[2:]
-        curlies = re.compile(_regex)
-        found = curlies.findall(value)
-        
-        for f in found:
-            srcKey = f[2:-1]
-            if srcKey in self._props:
-                value = value.replace(f, self._props[srcKey], 2)
-        
-        self._props[key] = value.strip()
-        found = curlies.findall(value.strip())
-        
-        for f in found:
-            srcKey = f[2:-1]
-            if self._unresolved.has_key(srcKey):
-                self._unresolved[srcKey] += [key]
-            else:
-                self._unresolved[srcKey] = [key]
-
-        #End of Alex fix
-        
-        # Check if an entry exists in pristine keys
-        if key in self._keymap:
-            oldkey = self._keymap.get(key)
-            self._origprops[oldkey] = oldvalue.strip()
-        else:
-            self._origprops[oldkey] = oldvalue.strip()
-            # Store entry in keymap
-            self._keymap[key] = oldkey
-            
-         # Alex fix, handle ${}
-        if key in self._unresolved:
-            for updateKey in self._unresolved[key]:
-                self.processPair(updateKey, self._props[updateKey])
-        
-    def escape(self, value):
-
-        # Java escapes the '=' and ':' in the value
-        # string with backslashes in the store method.
-        # So let us do the same.
-        #Alex fix added r prefix to str
-        newvalue = value.replace(':',r'\:')
-        # Alex fix added r prefix to str
-        newvalue = newvalue.replace('=',r'\=')
-
-        return newvalue
-
-    def unescape(self, value):
-
-        # Reverse of escape
-        # Alex fix added r prefix to str
-        newvalue = value.replace(r'\:',':')
-        # Alex fix added r prefix to str
-        newvalue = newvalue.replace(r'\=','=')
-
-        return newvalue    
-        
-    def load(self, stream):
-        """ Load properties from an open file stream """
-
-        #Alex disabled unneccesery stricked validations
-        # For the time being only accept file input streams
-        #if type(stream) is not file:
-        #    raise TypeError('Argument should be a file object!')
-        ## Check for the opened mode
-        #if stream.mode != 'r':
-        #    raise ValueError('Stream should be opened in read-only mode!')
-
-        try:
-            lines = stream.readlines()
-            self.__parse(lines)
-        except IOError as e:
-            raise
-
-    def getProperty(self, key):
-        """ Return a property for the given key """
-        
-        return self._props.get(key,'')
-
-    def setProperty(self, key, value):
-        """ Set the property for the given key """
-
-        if type(key) is str and type(value) is str:
-            self.processPair(key, value)
-        else:
-            raise TypeError('both key and value should be strings!')
-
-    def propertyNames(self):
-        """ Return an iterator over all the keys of the property
-        dictionary, i.e the names of the properties """
-
-        return self._props.keys()
-
-    def list(self, out=sys.stdout):
-        """ Prints a listing of the properties to the
-        stream 'out' which defaults to the standard output """
-
-        out.write('-- listing properties --\n')
-        for key,value in self._props.items():
-            out.write(''.join((key,'=',value,'\n')))
-
-    def store(self, out, header=""):
-        """ Write the properties list to the stream 'out' along
-        with the optional 'header' """
-
-        if out.mode[0] != 'w':
-            raise ValueError('Steam should be opened in write mode!')
-
-        try:
-            out.write(''.join(('#',header,'\n')))
-            # Write timestamp
-            tstamp = time.strftime('%a %b %d %H:%M:%S %Z %Y', time.localtime())
-            out.write(''.join(('#',tstamp,'\n')))
-            # Write properties from the pristine dictionary
-            for prop, val in self._origprops.items():
-                out.write(''.join((prop,'=',self.escape(val),'\n')))
-                
-            out.close()
-        except IOError as e:
-            raise
-
-    # Alex changed name getPropertyDict() to current
-    def as_dict(self):
-        return self._props
-
-    def __getitem__(self, name):
-        """ To support direct dictionary like access """
-
-        return self.getProperty(name)
-
-    def __setitem__(self, name, value):
-        """ To support direct dictionary like access """
-
-        self.setProperty(name, value)
-        
-    def __getattr__(self, name):
-        """ For attributes not found in self, redirect
-        to the properties dictionary """
-
-        try:
-            return self.__dict__[name]
-        except KeyError:
-            if hasattr(self._props,name):
-                return getattr(self._props, name)
-
+
+
+
+"""
+A Python replacement for java.util.Properties class
+This is modelled as closely as possible to the Java original.
+
+Created - Anand B Pillai <abpillai@gmail.com>,
+Update to Python 3 by Alex.
+Also there are some tweeks that was done by Alex.
+"""
+
+# see https://code.activestate.com/recipes/496795-a-python-replacement-for-javautilproperties/
+import sys
+import re
+import time
+from collections import OrderedDict
+
+
+class IllegalArgumentException(Exception):
+
+    def __init__(self, lineno, msg):
+        self.lineno = lineno
+        self.msg = msg
+
+    def __str__(self):
+        s='Exception at line number %d => %s' % (self.lineno, self.msg)
+        return s
+                 
+class Properties(object):
+    """ A Python replacement for java.util.Properties """
+    # Alex fix, handle ${}
+    #curlies = re.compile('\\${.+?}')
+    PLACEHOLDER_TOKEN = '$'
+
+    def __init__(self, props=None):
+
+        # Note: We don't take a default properties object
+        # as argument yet
+
+        # Dictionary of properties.
+        # Alex changed {} to OrderedDict
+        self._props = OrderedDict()
+        # Dictionary of properties with 'pristine' keys
+        # This is used for dumping the properties to a file
+        # using the 'store' method
+        # Alex changed {} to OrderedDict
+        self._origprops = OrderedDict()
+
+        # Dictionary mapping keys from property
+        # dictionary to pristine dictionary
+        # Alex changed {} to OrderedDict
+        self._keymap = OrderedDict()
+        # Alex changed {} to OrderedDict
+        self._unresolved = OrderedDict()
+        
+        self.othercharre = re.compile(r'(?<!\\)(\s*\=)|(?<!\\)(\s*\:)')
+        self.othercharre2 = re.compile(r'(\s*\=)|(\s*\:)')
+        self.bspacere = re.compile(r'\\(?!\s$)')
+        
+    def __str__(self):
+        s='{'
+        for key,value in self._props.items():
+            s = ''.join((s,key,'=',value,', '))
+
+        s=''.join((s[:-2],'}'))
+        return s
+
+    def __parse(self, lines):
+        """ Parse a list of lines and create
+        an internal property dictionary """
+
+        # Every line in the file must consist of either a comment
+        # or a key-value pair. A key-value pair is a line consisting
+        # of a key which is a combination of non-white space characters
+        # The separator character between key-value pairs is a '=',
+        # ':' or a whitespace character not including the newline.
+        # If the '=' or ':' characters are found, in the line, even
+        # keys containing whitespace chars are allowed.
+
+        # A line with only a key according to the rules above is also
+        # fine. In such case, the value is considered as the empty string.
+         # In order to include characters '=' or ':' in a key or value,
+        # they have to be properly escaped using the backslash character.
+
+        # Some examples of valid key-value pairs:
+        #
+        # key     value
+        # key=value
+        # key:value
+        # key     value1,value2,value3
+        # key     value1,value2,value3 \
+        #         value4, value5
+        # key
+        # This key= this value
+        # key = value1 value2 value3
+        
+        # Any line that starts with a '#' is considerered a comment
+        # and skipped. Also any trailing or preceding whitespaces
+        # are removed from the key/value.
+        
+        # This is a line parser. It parses the
+        # contents like by line.
+
+        lineno=0
+        i = iter(lines)
+
+        for line in i:
+            lineno += 1
+            line = line.strip()
+            # Skip null lines
+            if not line: continue
+            # Skip lines which are comments
+            if line[0] == '#': continue
+            # Some flags
+            escaped=False
+            # Position of first separation char
+            sepidx = -1
+            # A flag for performing wspace re check
+            flag = 0
+            # Check for valid space separation
+            # First obtain the max index to which we
+            # can search.
+            m = self.othercharre.search(line)
+            if m:
+                first, last = m.span()
+                start, end = 0, first
+                flag = 1
+                wspacere = re.compile(r'(?<![\\\=\:])(\s)')        
+            else:
+                if self.othercharre2.search(line):
+                    # Check if either '=' or ':' is present
+                    # in the line. If they are then it means
+                    # they are preceded by a backslash.
+                    
+                    # This means, we need to modify the
+                    # wspacere a bit, not to look for
+                    # : or = characters.
+                    wspacere = re.compile(r'(?<![\\])(\s)')        
+                start, end = 0, len(line)
+                
+            m2 = wspacere.search(line, start, end)
+            if m2:
+                # print 'Space match=>',line
+                # Means we need to split by space.
+                first, last = m2.span()
+                sepidx = first
+            elif m:
+                # print 'Other match=>',line
+                # No matching wspace char found, need
+                # to split by either '=' or ':'
+                first, last = m.span()
+                sepidx = last - 1
+                # print line[sepidx]
+                
+                
+            # If the last character is a backslash
+            # it has to be preceded by a space in which
+            # case the next line is read as part of the
+            # same property
+            while line[-1] == '\\':
+                # Read next line
+                nextline = i.next()
+                nextline = nextline.strip()
+                lineno += 1
+                # This line will become part of the value
+                line = line[:-1] + nextline
+
+            # Now split to key,value according to separation char
+            if sepidx != -1:
+                key, value = line[:sepidx], line[sepidx+1:]
+            else:
+                key,value = line,''
+
+            self.processPair(key, value)
+            
+    def processPair(self, key, value):
+        """ Process a (key, value) pair """
+
+        oldkey = key
+        oldvalue = value
+        
+        # Create key intelligently
+        keyparts = self.bspacere.split(key)
+        # print keyparts
+
+        strippable = False
+        lastpart = keyparts[-1]
+
+        if lastpart.find('\\ ') != -1:
+            keyparts[-1] = lastpart.replace('\\','')
+
+        # If no backspace is found at the end, but empty
+        # space is found, strip it
+        elif lastpart and lastpart[-1] == ' ':
+            strippable = True
+
+        key = ''.join(keyparts)
+        if strippable:
+            key = key.strip()
+            oldkey = oldkey.strip()
+        
+        oldvalue = self.unescape(oldvalue)
+        value = self.unescape(value)
+        
+        # Alex fix, handle ${}
+        _regex ='\\${.+?}'
+        if '$' != Properties.PLACEHOLDER_TOKEN:
+            _regex = _regex[0:1] + Properties.PLACEHOLDER_TOKEN + _regex[2:]
+        curlies = re.compile(_regex)
+        found = curlies.findall(value)
+        
+        for f in found:
+            srcKey = f[2:-1]
+            if srcKey in self._props:
+                value = value.replace(f, self._props[srcKey], 2)
+        
+        self._props[key] = value.strip()
+        found = curlies.findall(value.strip())
+        
+        for f in found:
+            srcKey = f[2:-1]
+            if self._unresolved.has_key(srcKey):
+                self._unresolved[srcKey] += [key]
+            else:
+                self._unresolved[srcKey] = [key]
+
+        #End of Alex fix
+        
+        # Check if an entry exists in pristine keys
+        if key in self._keymap:
+            oldkey = self._keymap.get(key)
+            self._origprops[oldkey] = oldvalue.strip()
+        else:
+            self._origprops[oldkey] = oldvalue.strip()
+            # Store entry in keymap
+            self._keymap[key] = oldkey
+            
+         # Alex fix, handle ${}
+        if key in self._unresolved:
+            for updateKey in self._unresolved[key]:
+                self.processPair(updateKey, self._props[updateKey])
+        
+    def escape(self, value):
+
+        # Java escapes the '=' and ':' in the value
+        # string with backslashes in the store method.
+        # So let us do the same.
+        #Alex fix added r prefix to str
+        newvalue = value.replace(':',r'\:')
+        # Alex fix added r prefix to str
+        newvalue = newvalue.replace('=',r'\=')
+
+        return newvalue
+
+    def unescape(self, value):
+
+        # Reverse of escape
+        # Alex fix added r prefix to str
+        newvalue = value.replace(r'\:',':')
+        # Alex fix added r prefix to str
+        newvalue = newvalue.replace(r'\=','=')
+
+        return newvalue    
+        
+    def load(self, stream):
+        """ Load properties from an open file stream """
+
+        #Alex disabled unneccesery stricked validations
+        # For the time being only accept file input streams
+        #if type(stream) is not file:
+        #    raise TypeError('Argument should be a file object!')
+        ## Check for the opened mode
+        #if stream.mode != 'r':
+        #    raise ValueError('Stream should be opened in read-only mode!')
+
+        try:
+            lines = stream.readlines()
+            self.__parse(lines)
+        except IOError as e:
+            raise
+
+    def getProperty(self, key):
+        """ Return a property for the given key """
+        
+        return self._props.get(key,'')
+
+    def setProperty(self, key, value):
+        """ Set the property for the given key """
+
+        if type(key) is str and type(value) is str:
+            self.processPair(key, value)
+        else:
+            raise TypeError('both key and value should be strings!')
+
+    def propertyNames(self):
+        """ Return an iterator over all the keys of the property
+        dictionary, i.e the names of the properties """
+
+        return self._props.keys()
+
+    def list(self, out=sys.stdout):
+        """ Prints a listing of the properties to the
+        stream 'out' which defaults to the standard output """
+
+        out.write('-- listing properties --\n')
+        for key,value in self._props.items():
+            out.write(''.join((key,'=',value,'\n')))
+
+    def store(self, out, header=""):
+        """ Write the properties list to the stream 'out' along
+        with the optional 'header' """
+
+        if out.mode[0] != 'w':
+            raise ValueError('Steam should be opened in write mode!')
+
+        try:
+            out.write(''.join(('#',header,'\n')))
+            # Write timestamp
+            tstamp = time.strftime('%a %b %d %H:%M:%S %Z %Y', time.localtime())
+            out.write(''.join(('#',tstamp,'\n')))
+            # Write properties from the pristine dictionary
+            for prop, val in self._origprops.items():
+                out.write(''.join((prop,'=',self.escape(val),'\n')))
+                
+            out.close()
+        except IOError as e:
+            raise
+
+    # Alex changed name getPropertyDict() to current
+    def as_dict(self):
+        return self._props
+
+    def __getitem__(self, name):
+        """ To support direct dictionary like access """
+
+        return self.getProperty(name)
+
+    def __setitem__(self, name, value):
+        """ To support direct dictionary like access """
+
+        self.setProperty(name, value)
+        
+    def __getattr__(self, name):
+        """ For attributes not found in self, redirect
+        to the properties dictionary """
+
+        try:
+            return self.__dict__[name]
+        except KeyError:
+            if hasattr(self._props,name):
+                return getattr(self._props, name)
+
```

### Comparing `alex_ber_utils-0.6.6b3/alexber/utils/setups.py` & `alex_ber_utils-0.7.0/alexber/utils/setups.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-import logging
-import setuptools
-from shutil import rmtree
-import os
-import sys
-
-logger = logging.getLogger(__name__)
-
-_setup_module = sys.modules['__main__']
-
-_setup_dir = os.path.dirname(os.path.realpath(_setup_module.__file__)) if hasattr(_setup_module, '__file__') \
-                                                                        else os.getcwd()
-VERSION = getattr(_setup_module, 'VERSION', None)
-
-def _my_rmtree(path, ignore_errors=False, onerror=None):
-    try:
-        rmtree(path, ignore_errors, onerror)
-    except OSError:
-        pass
-
-#adapted from https://github.com/kennethreitz/setup.py/blob/master/setup.py
-class UploadCommand(setuptools.Command):
-    '''
-    Support setup.py upload.
-    UploadCommand is intented to be used only from setup.py
-    It's builds Source and Wheel distribution.
-    It's uploads the package to PyPI via Twine.
-    It's pushes the git tags.
-    '''
-
-    description = 'Build and publish the package.'
-    user_options = []
-
-    @staticmethod
-    def status(s):
-        """Prints things in bold."""
-        print(f'\033[1m{s}\033[0m')
-
-    def initialize_options(self):
-        pass
-
-    def finalize_options(self):
-        pass
-
-    def run(self):
-        self.status('Removing previous builds...')
-        # rm -rf build *.egg-info dist
-        _my_rmtree(os.path.join(_setup_dir, 'build'))
-        _my_rmtree(os.path.join(_setup_dir, 'f{NAME}.egg-info'))
-        _my_rmtree(os.path.join(_setup_dir, 'dist'))
-
-        self.status('Building Source and Wheel distribution...')
-        os.system(f'{sys.executable} setup.py sdist bdist_wheel')
-        #os.system('python3 setup.py sdist bdist_wheel')
-
-        self.status('Uploading the package to PyPI via Twine...')
-        # python3 -m keyring set https://upload.pypi.org/legacy/ alex-ber
-        os.system('twine upload dist/*')
-
-        self.status('Pushing git tags...')
-        os.system('git fetch')
-        os.system('git commit -m "setup.py changed" setup.py')
-        os.system('git push')
-        if VERSION is not None:
-            os.system(f'git tag v{VERSION}')
-            os.system(f'git push origin v{VERSION}')
-        #os.system(f'git tag -d v{VERSION}')
-        #os.system(f'git push --delete origin v{VERSION}')
-        #os.system('git push --tags')
-
-        sys.exit()
-
+import logging
+import setuptools
+from shutil import rmtree
+import os
+import sys
+
+logger = logging.getLogger(__name__)
+
+_setup_module = sys.modules['__main__']
+
+_setup_dir = os.path.dirname(os.path.realpath(_setup_module.__file__)) if hasattr(_setup_module, '__file__') \
+                                                                        else os.getcwd()
+VERSION = getattr(_setup_module, 'VERSION', None)
+
+def _my_rmtree(path, ignore_errors=False, onerror=None):
+    try:
+        rmtree(path, ignore_errors, onerror)
+    except OSError:
+        pass
+
+#adapted from https://github.com/kennethreitz/setup.py/blob/master/setup.py
+class UploadCommand(setuptools.Command):
+    '''
+    Support setup.py upload.
+    UploadCommand is intented to be used only from setup.py
+    It's builds Source and Wheel distribution.
+    It's uploads the package to PyPI via Twine.
+    It's pushes the git tags.
+    '''
+
+    description = 'Build and publish the package.'
+    user_options = []
+
+    @staticmethod
+    def status(s):
+        """Prints things in bold."""
+        print(f'\033[1m{s}\033[0m')
+
+    def initialize_options(self):
+        pass
+
+    def finalize_options(self):
+        pass
+
+    def run(self):
+        self.status('Removing previous builds...')
+        # rm -rf build *.egg-info dist
+        _my_rmtree(os.path.join(_setup_dir, 'build'))
+        _my_rmtree(os.path.join(_setup_dir, 'f{NAME}.egg-info'))
+        _my_rmtree(os.path.join(_setup_dir, 'dist'))
+
+        self.status('Building Source and Wheel distribution...')
+        os.system(f'{sys.executable} setup.py sdist bdist_wheel')
+        #os.system('python3 setup.py sdist bdist_wheel')
+
+        self.status('Uploading the package to PyPI via Twine...')
+        # python3 -m keyring set https://upload.pypi.org/legacy/ alex-ber
+        os.system('twine upload dist/*')
+
+        self.status('Pushing git tags...')
+        os.system('git fetch')
+        os.system('git commit -m "setup.py changed" setup.py')
+        os.system('git push')
+        if VERSION is not None:
+            os.system(f'git tag v{VERSION}')
+            os.system(f'git push origin v{VERSION}')
+        #os.system(f'git tag -d v{VERSION}')
+        #os.system(f'git push --delete origin v{VERSION}')
+        #os.system('git push --tags')
+
+        sys.exit()
+
```

### Comparing `alex_ber_utils-0.6.6b3/alexber/utils/stdlogging.py` & `alex_ber_utils-0.7.0/alexber/utils/stdlogging.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-import logging
-import sys
-from . importer import importer
-
-# This modules is based upon https://github.com/fx-kirin/py-stdlogging/blob/master/stdlogging.py
-# See also https://github.com/fx-kirin/py-stdlogging/pull/1.
-# I have encountered on this module here
-# https://stackoverflow.com/questions/47325506/making-python-loggers-log-all-stdout-and-stderr-messages 
-# Quote: "But be careful to capture stdout because it's very fragile"
-
-def _validate_param(d, param_name):
-    if d is None:
-        raise ValueError(f"Expected '{param_name} param not found")
-
-class StreamToLogger:
-    """
-    This is adapter class from any stream-like object to logging.Logger.
-    """
-
-    def __init__(self, **kwargs):
-        """
-        It is recommended to use package-level initStream() function and not this method directly.
-        :param logger: Required. Standard Python's Logger or any Logger-like object.
-        :param stream: Required. sys.stderr, sys.stdout or any other stream-like object.
-        :param log_level: Optional. If not supplied, logging.DEBUG will be used.
-        """
-
-        _validate_param(kwargs, 'logger')
-        _validate_param(kwargs, 'log_level')
-        _validate_param(kwargs, 'stream')
-
-        self.logger = kwargs.pop('logger')
-        self.log_level = kwargs.pop('log_level', logging.DEBUG)
-        self.stream = kwargs.pop('stream')
-
-    def write(self, lines):
-        if lines:
-            lines = lines+'\n'
-            for line in lines.split('\n'):
-                if line:
-                    self.logger.log(self.log_level, line.rstrip())
-
-    def flush(self):
-        self.stream.flush()
-
-
-
-def initStream(logger=None, logger_level=logging.ERROR, stream_getter=None, stream_setter=None, adapter_cls=None):
-    """
-    Preffered API.
-    stream_getter() is supplier/factory method that returns stream-like object (i.e. sys.stderr) that we're adapting upon.
-                   It's intended usage is to supply stream-like object that we want to apapt upon.
-    stream_setter() is consumer method that receives wrapped object as parameter.
-                   It's intended usage is to overwrite source stream-like, i.e. sys.stderr = s.
-    :param logger: Optional. If not supplied logging.getLogger('stderr') will be used.
-    :param logger_level: Optional. If not supplied logging.ERROR will be used.
-    :param stream_getter: Optional. if not supplied method that returns sys.stderr will be used.
-    :param stream_setter: Optional. if not supplied method that get's strema-like object and set's sys.stderr will be used.
-    :param adapter_cls: Optional. Can be str or class. if not supplied than StreamToLogger is used.
-    :return:
-    """
-    if logger is None:
-        logger = logging.getLogger('stderr')
-
-    if stream_getter is None:
-        def stream_getter():
-            return sys.stderr
-
-    if stream_setter is None:
-        def stream_setter(s):
-            sys.stderr = s
-
-    stream = stream_getter()
-
-    if adapter_cls is None:
-        adapter_cls = StreamToLogger
-    elif isinstance(adapter_cls, str):
-        adapter_cls = importer(adapter_cls)
-
-    sl = adapter_cls(logger=logger, stream=stream, logger_level=logger_level)
+import logging
+import sys
+from . importer import importer
+
+# This modules is based upon https://github.com/fx-kirin/py-stdlogging/blob/master/stdlogging.py
+# See also https://github.com/fx-kirin/py-stdlogging/pull/1.
+# I have encountered on this module here
+# https://stackoverflow.com/questions/47325506/making-python-loggers-log-all-stdout-and-stderr-messages 
+# Quote: "But be careful to capture stdout because it's very fragile"
+
+def _validate_param(d, param_name):
+    if d is None:
+        raise ValueError(f"Expected '{param_name} param not found")
+
+class StreamToLogger:
+    """
+    This is adapter class from any stream-like object to logging.Logger.
+    """
+
+    def __init__(self, **kwargs):
+        """
+        It is recommended to use package-level initStream() function and not this method directly.
+        :param logger: Required. Standard Python's Logger or any Logger-like object.
+        :param stream: Required. sys.stderr, sys.stdout or any other stream-like object.
+        :param log_level: Optional. If not supplied, logging.DEBUG will be used.
+        """
+
+        _validate_param(kwargs, 'logger')
+        _validate_param(kwargs, 'log_level')
+        _validate_param(kwargs, 'stream')
+
+        self.logger = kwargs.pop('logger')
+        self.log_level = kwargs.pop('log_level', logging.DEBUG)
+        self.stream = kwargs.pop('stream')
+
+    def write(self, lines):
+        if lines:
+            lines = lines+'\n'
+            for line in lines.split('\n'):
+                if line:
+                    self.logger.log(self.log_level, line.rstrip())
+
+    def flush(self):
+        self.stream.flush()
+
+
+
+def initStream(logger=None, logger_level=logging.ERROR, stream_getter=None, stream_setter=None, adapter_cls=None):
+    """
+    Preffered API.
+    stream_getter() is supplier/factory method that returns stream-like object (i.e. sys.stderr) that we're adapting upon.
+                   It's intended usage is to supply stream-like object that we want to apapt upon.
+    stream_setter() is consumer method that receives wrapped object as parameter.
+                   It's intended usage is to overwrite source stream-like, i.e. sys.stderr = s.
+    :param logger: Optional. If not supplied logging.getLogger('stderr') will be used.
+    :param logger_level: Optional. If not supplied logging.ERROR will be used.
+    :param stream_getter: Optional. if not supplied method that returns sys.stderr will be used.
+    :param stream_setter: Optional. if not supplied method that get's strema-like object and set's sys.stderr will be used.
+    :param adapter_cls: Optional. Can be str or class. if not supplied than StreamToLogger is used.
+    :return:
+    """
+    if logger is None:
+        logger = logging.getLogger('stderr')
+
+    if stream_getter is None:
+        def stream_getter():
+            return sys.stderr
+
+    if stream_setter is None:
+        def stream_setter(s):
+            sys.stderr = s
+
+    stream = stream_getter()
+
+    if adapter_cls is None:
+        adapter_cls = StreamToLogger
+    elif isinstance(adapter_cls, str):
+        adapter_cls = importer(adapter_cls)
+
+    sl = adapter_cls(logger=logger, stream=stream, logger_level=logger_level)
     stream_setter(sl)
```

### Comparing `alex_ber_utils-0.6.6b3/alexber/utils/thread_locals.py` & `alex_ber_utils-0.7.0/alexber/utils/thread_locals.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-#inspired by https://stackoverflow.com/questions/1408171/thread-local-storage-in-python
-
-
-def threadlocal_var(thread_locals, varname, factory, *args, **kwargs):
-  v = getattr(thread_locals, varname, None)
-  if v is None:
-    v = factory(*args, **kwargs)
-    setattr(thread_locals, varname, v)
-  return v
-
-def get_threadlocal_var(thread_locals, varname):
-    v = threadlocal_var(thread_locals, varname, lambda : None)
-    if v is None:
-        raise ValueError(f"threadlocal's {varname} is not initilized")
-    return v
-
-def del_threadlocal_var(thread_locals, varname):
-    try:
-        delattr(thread_locals, varname)
-    except AttributeError:
-        pass
+#inspired by https://stackoverflow.com/questions/1408171/thread-local-storage-in-python
+
+
+def threadlocal_var(thread_locals, varname, factory, *args, **kwargs):
+  v = getattr(thread_locals, varname, None)
+  if v is None:
+    v = factory(*args, **kwargs)
+    setattr(thread_locals, varname, v)
+  return v
+
+def get_threadlocal_var(thread_locals, varname):
+    v = threadlocal_var(thread_locals, varname, lambda : None)
+    if v is None:
+        raise ValueError(f"threadlocal's {varname} is not initilized")
+    return v
+
+def del_threadlocal_var(thread_locals, varname):
+    try:
+        delattr(thread_locals, varname)
+    except AttributeError:
+        pass
```

### Comparing `alex_ber_utils-0.6.6b3/alexber/utils/uuids.py` & `alex_ber_utils-0.7.0/alexber/utils/uuids.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-#see https://stackoverflow.com/questions/1785503/when-should-i-use-uuid-uuid1-vs-uuid-uuid4-in-python
-#https://stackoverflow.com/questions/703035/when-are-you-truly-forced-to-use-uuid-as-part-of-the-design/786541#786541
-
-from uuid import uuid1 as _uuid1
-_int_from_bytes = int.from_bytes  # py3 only
-
-from random import SystemRandom as _SystemRandom
-
-_system_random = _SystemRandom()
-
-
-
-
-
-def uuid1mc():
-    '''
-    This is v1 with random MAC ("v1mc"). This is a hybrid between version 1 & version 4.
-
-    Version 1 UUIDs use the network card's MAC address (which unless spoofed, should be unique),
-    plus a timestamp, plus the usual bit-twiddling to generate the UUID.
-
-    Version 4 UUIDs Generate a random UUID.
-
-    uuid1mc() is deliberately generating v1 UUIDs with a random broadcast MAC address (this is allowed by the v1 spec).
-    The resulting v1 UUID is time dependant (like regular v1), but lacks all host-specific information (like v4).
-    It's also much closer to v4 in it's collision-resistance:
-        v1mc = 60 bits of time + 61 random bits = 121 unique bits; v4 = 122 random bits.
-
-    Note: somebody reported that ran into trouble using UUID1 in Amazon EC2 instances.
-    He use UUID1 for a database upgrade script where he generated ~120k UUIDs within a couple of minutes.
-    The UUID collision led to violation of a primary key constraint.
-    He suspect poor clock resolution and switching to UUID4 solved it for him.
-
-    '''
-    #return uuid1(_int_from_bytes(urandom(6), "big") | 0x010000000000)
-    node = _system_random.getrandbits(8) #6 and not 8, because this function round up to bits / 8 and rounded up
-    # NOTE: The constant here is required by the UUIDv1 spec...
-    return  _uuid1(node | 0x010000000000)
-
-
+#see https://stackoverflow.com/questions/1785503/when-should-i-use-uuid-uuid1-vs-uuid-uuid4-in-python
+#https://stackoverflow.com/questions/703035/when-are-you-truly-forced-to-use-uuid-as-part-of-the-design/786541#786541
+
+from uuid import uuid1 as _uuid1
+_int_from_bytes = int.from_bytes  # py3 only
+
+from random import SystemRandom as _SystemRandom
+
+_system_random = _SystemRandom()
+
+
+
+
+
+def uuid1mc():
+    '''
+    This is v1 with random MAC ("v1mc"). This is a hybrid between version 1 & version 4.
+
+    Version 1 UUIDs use the network card's MAC address (which unless spoofed, should be unique),
+    plus a timestamp, plus the usual bit-twiddling to generate the UUID.
+
+    Version 4 UUIDs Generate a random UUID.
+
+    uuid1mc() is deliberately generating v1 UUIDs with a random broadcast MAC address (this is allowed by the v1 spec).
+    The resulting v1 UUID is time dependant (like regular v1), but lacks all host-specific information (like v4).
+    It's also much closer to v4 in it's collision-resistance:
+        v1mc = 60 bits of time + 61 random bits = 121 unique bits; v4 = 122 random bits.
+
+    Note: somebody reported that ran into trouble using UUID1 in Amazon EC2 instances.
+    He use UUID1 for a database upgrade script where he generated ~120k UUIDs within a couple of minutes.
+    The UUID collision led to violation of a primary key constraint.
+    He suspect poor clock resolution and switching to UUID4 solved it for him.
+
+    '''
+    #return uuid1(_int_from_bytes(urandom(6), "big") | 0x010000000000)
+    node = _system_random.getrandbits(8) #6 and not 8, because this function round up to bits / 8 and rounded up
+    # NOTE: The constant here is required by the UUIDv1 spec...
+    return  _uuid1(node | 0x010000000000)
+
+
```

### Comparing `alex_ber_utils-0.6.6b3/alexber/utils/ymlparsers.py` & `alex_ber_utils-0.7.0/alexber/utils/ymlparsers.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,314 +1,314 @@
-"""
-This is essentially wrapper arround HiYaPyCo project with streamlined and extended API and couple of work-arrounds.
-
-This module depends on some 3-rd party dependencies, in order to use it, you should have installed first. To do it
-run `python3 -m pip install alex-ber-utils[yml]`.
-
-This module doesn't use any package-level variables in hiYaPyCo module, including hiYaPyCo.jinja2env.
-This module do use Jinja2's `Environment`.
-
-This module is low level API for init_app_conf.py, deploys.py. It is also optionally used in emails.py.
-
-See here https://medium.com/analytics-vidhya/my-ymlparsers-module-88221edf16a6 for documentation.
-
-"""
-
-import warnings
-try:
-    with warnings.catch_warnings():
-        warnings.filterwarnings("ignore", message=r'.*?collections\.abc.*?', module=r'.*?jinja2.*?')
-        from jinja2 import Environment as _Environment, \
-                        DebugUndefined as _DebugUndefined
-except ImportError:
-    import warnings
-
-    warning = (
-        "You appear to be missing some optional dependencies (jinja2);"
-        "please 'python3 -m pip install alex-ber-utils[yml]'."
-    )
-    warnings.warn(warning, ImportWarning)
-    raise
-
-try:
-    import hiyapyco as _hiyapyco
-except ImportError:
-    import warnings
-
-    warning = (
-        "You appear to be missing some optional dependencies (hiyapyco);"
-        "please 'python3 -m pip install alex-ber-utils[yml]'."
-    )
-    warnings.warn(warning, ImportWarning)
-    raise
-
-try:
-    _hiyapyco.METHOD_SUBSTITUTE
-except AttributeError as e:
-    import warnings
-
-    warning = (
-        "You appear to be missing some optional yml parsing dependencies (hiyapyco should be at least 0.4.16);"
-        "please 'python3 -m pip install alex-ber-utils[yml]'."
-    )
-    warnings.warn(warning, ImportWarning)
-    raise ImportError(str(e)) from e
-
-import io as _io
-import os as _os
-import contextlib
-from threading import RLock as _Lock
-
-
-from hiyapyco import logger, HiYaPyCoImplementationException, HiYaPyCoInvocationException, TemplateError, \
-    re, strtobool, HiYaPyCo as _HiYaPyCo
-from hiyapyco.odyldo import safe_dump as _safe_dump
-
-_safe_dump_d = None
-_load_d = None
-
-from platform import uname as _uname
-from . _ymlparsers_extra import format_template as _format_template
-
-format_template = _format_template
-
-class HiYaPyCo(_HiYaPyCo):
-    jinja2ctx = None
-    jinja2Lock = None
-
-
-    #this adopted version
-    #1. In order to change reference of jinja2env
-    #2. In order to use reentrant lock
-    def _interpolatestr(self, s):
-        try:
-            with self.jinja2Lock:
-                si = HiYaPyCo.jinja2ctx.from_string(s).render(self._data)
-        except TemplateError as e:
-            # FIXME: this seems to be broken for unicode str?
-            raise HiYaPyCoImplementationException('error interpolating string "%s" : %s' % (s, e,))
-        if not s == si:
-            if self.castinterpolated:
-                if not re.match( r'^\d+\.*\d*$', si):
-                    try:
-                        si = bool(strtobool(si))
-                    except ValueError:
-                        pass
-                else:
-                    try:
-                        if '.' in si:
-                            si = float(si)
-                        else:
-                            si = int(si)
-                    except ValueError:
-                        pass
-            logger.debug('interpolated "%s" to "%s" (type: %s)' % (s, si, type(si),))
-        return si
-
-
-def safe_dump(data, stream=None, **kwds):
-    """
-    Dumping data to stream.
-
-    Simple Python objects like primitive types (str, integer, etc), list, dict, OrderedDict are supported.
-
-    Note: that collections.OrderedDict is also supported.
-
-    :param data: data-structure to dump.
-    :param stream: where to write the representation.
-    :param kwds: See initConfig() for default values. See yaml.dump_all()
-    :return: str representation of data
-    """
-    if _safe_dump_d is None:
-        raise ValueError("_safe_dump_d can't be None")
-
-    kwargs = {**_safe_dump_d, **kwds}
-    _safe_dump(data, stream, **kwargs)
-
-
-def load(*args, **kwds):
-    """
-    Load a Hierarchical yml files
-    --------------------------------------
-
-    See initConfig() for default values.
-    If you want to disable variable substitution, use DisableVarSubst context manager like this:
-
-    with ymlparsers.DisableVarSubst():
-        d = ymlparsers.load([str(full_path)])
-
-    :param args: YMLfile(s)
-    :param kwargs:
-      * method: one of hiyapyco.METHOD_SIMPLE | hiyapyco.METHOD_MERGE | hiyapyco.METHOD_SUBSTITUTE
-      * mergelists: boolean (default: True) try to merge lists (only makes sense if hiyapyco.METHOD_MERGE or hiyapyco.METHOD_SUBSTITUTE)
-      * interpolate: boolean (default: False)
-      * castinterpolated: boolean (default: False) try to cast values after interpolating
-      * encoding: (default: 'utf-8') encoding used to read yml files
-      * loglevel: one of  the valid levels from the logging module
-      * failonmissingfiles: boolean (default: True)
-      * loglevelmissingfiles
-
-    :returns a representation of the merged and (if requested) interpolated config using OrderedDict.
-    """
-    if _load_d is None:
-        raise ValueError("_load_d can't be None")
-
-    kwargs = {**_load_d, **kwds}
-    #return _hiyapyco.load(*args, **kwargs)
-    hiyapyco = HiYaPyCo(*args, **kwargs)
-    return hiyapyco.data()
-
-
-def as_str(data, **kwds):
-    """
-    Return str representation of the data.
-
-    Simple Python objects like primitive types (str, integer, etc), list, dict, OrderedDict are supported.
-
-    Note: that collections.OrderedDict is also supported.
-
-    :param data: data-structure to dump.
-    :param kwds: See initConfig() for default values. See yaml.dump_all()
-    :return: str representation of data
-    """
-    with _io.StringIO() as buf:
-        buf.write(_os.linesep)
-        safe_dump(data, stream=buf, **kwds)
-        return buf.getvalue()
-
-@contextlib.contextmanager
-def DisableVarSubst(*args, **kwargs):
-    """
-    Use of this context manager disables variable substation in the load() function.
-
-
-    :param jinja2ctx - Jinja2 Environment. If not provided HiYaPyCo.jinja2ctx is used.
-    :param jinja2Lock - lock to use for synchronization. Should be the same here and in load() function.
-                        If not provided HiYaPyCo.jinja2ctx is used.
-    """
-    jinja2ctx = kwargs.pop('jinja2ctx', None)
-    jinja2Lock = kwargs.pop('jinja2Lock', None)
-
-    if jinja2ctx is None and jinja2Lock is not None:
-        raise ValueError("You can't provide your jinja2Lock for HiYaPyCo.jinja2ctx")
-
-    if HiYaPyCo.jinja2ctx is not None and HiYaPyCo.jinja2Lock is None:
-        raise ValueError('HiYaPyCo.jinja2ctx is not None, but HiYaPyCo.jinja2Lock is None')
-
-    if jinja2ctx is None:
-        jinja2ctx = HiYaPyCo.jinja2ctx
-        jinja2Lock = HiYaPyCo.jinja2Lock
-
-    if jinja2ctx is None or jinja2Lock is None:
-        raise ValueError("You should pass both jinja2ctx and jinja2Lock or "
-                         "You should have HiYaPyCo.jinja2ctx and HiYaPyCo.jinja2Lock not None"
-                         )
-
-    with jinja2Lock:
-        variable_start_string = jinja2ctx.variable_start_string
-        variable_end_string = jinja2ctx.variable_end_string
-        block_start_string = jinja2ctx.block_start_string
-        block_end_string = jinja2ctx.block_end_string
-
-        jinja2ctx.variable_start_string = '@@{@|'
-        jinja2ctx.variable_end_string = '|@}@@'
-        jinja2ctx.block_start_string = '%%{%|'
-        jinja2ctx.block_end_string = '|%}%%'
-
-        try:
-            yield jinja2ctx
-        finally:
-            jinja2ctx.variable_start_string = variable_start_string
-            jinja2ctx.variable_end_string = variable_end_string
-            jinja2ctx.block_start_string = block_start_string
-            jinja2ctx.block_end_string = block_end_string
-
-
-# # support for tag 'tag:yaml.org,2002:python/object/apply:collections.OrderedDict'
-# _represent_dict_order = lambda self, data:  self.represent_mapping('tag:yaml.org,2002:map', data.items())
-# yaml.add_representer(OrderedDict, _represent_dict_order)
-
-#
-# _hiyapyco.load("\n") #_hiyapyco._usedefaultyamlloader = False
-
-
-
-def initConfig(**kwargs):
-    """
-    This method can be optionally called prior any call to another function in this module.
-    It is indented to be called in the MainThread.
-    This method can be call with empty params.
-
-    Note: this module doesn't use any package-level variables in hiYaPyCo module.
-
-    :param jinja2Lock: lock to use for synchronization in DisableVarSubst and load().
-                      If not supplied, default RLock is used.
-                      Will be available as HiYaPyCo.jinja2Lock.
-    :param jinja2ctx: context for overriding values in initialization (default is _DebugUndefined) of Jinja2 Environment:
-                      gloabls will be override values in Environment.globals.update(**globals)
-                      Default is 'uname':platform.uname
-                      Will be available as HiYaPyCo.jinja2ctx.
-    :param load: this params will be used as default values in load() function. See hiyapyco.load()
-                Default values are
-                      'method':_hiyapyco.METHOD_SUBSTITUTE,
-                      'mergelists':False,
-                      'interpolate':True,
-                      'castinterpolated':True
-                This means, by default:
-                      We're replacing list, not merging them.
-                      We're interpolating values in the data (to scalar/list/OrderDict).
-                      We're also using casting to appropriate type.
-    :param safe_dump: this params will be used as default values in safe_dump() and as_str(). See yaml.dump_all()
-                Default values are
-                      'default_flow_style':False,
-                      'sort_keys':False
-                This means, by default:
-                       we prefer block style always.
-                       we preserve the key order (no sorting for key in the dictionary).
-
-    If running from the MainThread, this method is idempotent.
-
-    :return:
-    """
-    jinja2Lock_p = kwargs.get('jinja2Lock', None)
-    if jinja2Lock_p is None:
-        jinja2Lock_p = _Lock()
-    HiYaPyCo.jinja2Lock = jinja2Lock_p
-
-    jinja2ctx_d = kwargs.get('jinja2ctx', {})
-    globals_d = jinja2ctx_d.pop('globals', {})
-    # jinja2ctx_p = _Environment(undefined=_StrictUndefined)
-    jinja2ctx_p = _Environment(**{'undefined':_DebugUndefined, **jinja2ctx_d})
-    jinja2ctx_p.globals.update(**{'uname':_uname, **globals_d})
-
-
-    with HiYaPyCo.jinja2Lock:
-        HiYaPyCo.jinja2ctx = jinja2ctx_p
-
-
-    load_d = kwargs.get('load', {})
-    _load_d_p = {'method':_hiyapyco.METHOD_SUBSTITUTE,
-               'mergelists':False,
-               'interpolate':True,
-               'castinterpolated':True,
-               **load_d}
-
-    method = _load_d_p['method']
-    # TODO: HiYaPyCo._substmerge() bug workarround, see https://github.com/zerwes/hiyapyco/pull/38
-    HiYaPyCo._deepmerge = _HiYaPyCo._substmerge
-    if method == _hiyapyco.METHOD_MERGE:
-        #restore original _deepmerge
-        HiYaPyCo._deepmerge = _HiYaPyCo._deepmerge
-    global _load_d
-    _load_d = _load_d_p
-
-
-    safe_dump_d = kwargs.get('safe_dump', {})
-    global _safe_dump_d
-    #See https://github.com/yaml/pyyaml/pull/256
-    _safe_dump_d = {'default_flow_style':False,
-                        'sort_keys':False,
-                        **safe_dump_d}
-
-
-
+"""
+This is essentially wrapper arround HiYaPyCo project with streamlined and extended API and couple of work-arrounds.
+
+This module depends on some 3-rd party dependencies, in order to use it, you should have installed first. To do it
+run `python3 -m pip install alex-ber-utils[yml]`.
+
+This module doesn't use any package-level variables in hiYaPyCo module, including hiYaPyCo.jinja2env.
+This module do use Jinja2's `Environment`.
+
+This module is low level API for init_app_conf.py, deploys.py. It is also optionally used in emails.py.
+
+See here https://medium.com/analytics-vidhya/my-ymlparsers-module-88221edf16a6 for documentation.
+
+"""
+
+import warnings
+try:
+    with warnings.catch_warnings():
+        warnings.filterwarnings("ignore", message=r'.*?collections\.abc.*?', module=r'.*?jinja2.*?')
+        from jinja2 import Environment as _Environment, \
+                        DebugUndefined as _DebugUndefined
+except ImportError:
+    import warnings
+
+    warning = (
+        "You appear to be missing some optional dependencies (jinja2);"
+        "please 'python3 -m pip install alex-ber-utils[yml]'."
+    )
+    warnings.warn(warning, ImportWarning)
+    raise
+
+try:
+    import hiyapyco as _hiyapyco
+except ImportError:
+    import warnings
+
+    warning = (
+        "You appear to be missing some optional dependencies (hiyapyco);"
+        "please 'python3 -m pip install alex-ber-utils[yml]'."
+    )
+    warnings.warn(warning, ImportWarning)
+    raise
+
+try:
+    _hiyapyco.METHOD_SUBSTITUTE
+except AttributeError as e:
+    import warnings
+
+    warning = (
+        "You appear to be missing some optional yml parsing dependencies (hiyapyco should be at least 0.4.16);"
+        "please 'python3 -m pip install alex-ber-utils[yml]'."
+    )
+    warnings.warn(warning, ImportWarning)
+    raise ImportError(str(e)) from e
+
+import io as _io
+import os as _os
+import contextlib
+from threading import RLock as _Lock
+
+
+from hiyapyco import logger, HiYaPyCoImplementationException, HiYaPyCoInvocationException, TemplateError, \
+    re, strtobool, HiYaPyCo as _HiYaPyCo
+from hiyapyco.odyldo import safe_dump as _safe_dump
+
+_safe_dump_d = None
+_load_d = None
+
+from platform import uname as _uname
+from . _ymlparsers_extra import format_template as _format_template
+
+format_template = _format_template
+
+class HiYaPyCo(_HiYaPyCo):
+    jinja2ctx = None
+    jinja2Lock = None
+
+
+    #this adopted version
+    #1. In order to change reference of jinja2env
+    #2. In order to use reentrant lock
+    def _interpolatestr(self, s):
+        try:
+            with self.jinja2Lock:
+                si = HiYaPyCo.jinja2ctx.from_string(s).render(self._data)
+        except TemplateError as e:
+            # FIXME: this seems to be broken for unicode str?
+            raise HiYaPyCoImplementationException('error interpolating string "%s" : %s' % (s, e,))
+        if not s == si:
+            if self.castinterpolated:
+                if not re.match( r'^\d+\.*\d*$', si):
+                    try:
+                        si = bool(strtobool(si))
+                    except ValueError:
+                        pass
+                else:
+                    try:
+                        if '.' in si:
+                            si = float(si)
+                        else:
+                            si = int(si)
+                    except ValueError:
+                        pass
+            logger.debug('interpolated "%s" to "%s" (type: %s)' % (s, si, type(si),))
+        return si
+
+
+def safe_dump(data, stream=None, **kwds):
+    """
+    Dumping data to stream.
+
+    Simple Python objects like primitive types (str, integer, etc), list, dict, OrderedDict are supported.
+
+    Note: that collections.OrderedDict is also supported.
+
+    :param data: data-structure to dump.
+    :param stream: where to write the representation.
+    :param kwds: See initConfig() for default values. See yaml.dump_all()
+    :return: str representation of data
+    """
+    if _safe_dump_d is None:
+        raise ValueError("_safe_dump_d can't be None")
+
+    kwargs = {**_safe_dump_d, **kwds}
+    _safe_dump(data, stream, **kwargs)
+
+
+def load(*args, **kwds):
+    """
+    Load a Hierarchical yml files
+    --------------------------------------
+
+    See initConfig() for default values.
+    If you want to disable variable substitution, use DisableVarSubst context manager like this:
+
+    with ymlparsers.DisableVarSubst():
+        d = ymlparsers.load([str(full_path)])
+
+    :param args: YMLfile(s)
+    :param kwargs:
+      * method: one of hiyapyco.METHOD_SIMPLE | hiyapyco.METHOD_MERGE | hiyapyco.METHOD_SUBSTITUTE
+      * mergelists: boolean (default: True) try to merge lists (only makes sense if hiyapyco.METHOD_MERGE or hiyapyco.METHOD_SUBSTITUTE)
+      * interpolate: boolean (default: False)
+      * castinterpolated: boolean (default: False) try to cast values after interpolating
+      * encoding: (default: 'utf-8') encoding used to read yml files
+      * loglevel: one of  the valid levels from the logging module
+      * failonmissingfiles: boolean (default: True)
+      * loglevelmissingfiles
+
+    :returns a representation of the merged and (if requested) interpolated config using OrderedDict.
+    """
+    if _load_d is None:
+        raise ValueError("_load_d can't be None")
+
+    kwargs = {**_load_d, **kwds}
+    #return _hiyapyco.load(*args, **kwargs)
+    hiyapyco = HiYaPyCo(*args, **kwargs)
+    return hiyapyco.data()
+
+
+def as_str(data, **kwds):
+    """
+    Return str representation of the data.
+
+    Simple Python objects like primitive types (str, integer, etc), list, dict, OrderedDict are supported.
+
+    Note: that collections.OrderedDict is also supported.
+
+    :param data: data-structure to dump.
+    :param kwds: See initConfig() for default values. See yaml.dump_all()
+    :return: str representation of data
+    """
+    with _io.StringIO() as buf:
+        buf.write(_os.linesep)
+        safe_dump(data, stream=buf, **kwds)
+        return buf.getvalue()
+
+@contextlib.contextmanager
+def DisableVarSubst(*args, **kwargs):
+    """
+    Use of this context manager disables variable substation in the load() function.
+
+
+    :param jinja2ctx - Jinja2 Environment. If not provided HiYaPyCo.jinja2ctx is used.
+    :param jinja2Lock - lock to use for synchronization. Should be the same here and in load() function.
+                        If not provided HiYaPyCo.jinja2ctx is used.
+    """
+    jinja2ctx = kwargs.pop('jinja2ctx', None)
+    jinja2Lock = kwargs.pop('jinja2Lock', None)
+
+    if jinja2ctx is None and jinja2Lock is not None:
+        raise ValueError("You can't provide your jinja2Lock for HiYaPyCo.jinja2ctx")
+
+    if HiYaPyCo.jinja2ctx is not None and HiYaPyCo.jinja2Lock is None:
+        raise ValueError('HiYaPyCo.jinja2ctx is not None, but HiYaPyCo.jinja2Lock is None')
+
+    if jinja2ctx is None:
+        jinja2ctx = HiYaPyCo.jinja2ctx
+        jinja2Lock = HiYaPyCo.jinja2Lock
+
+    if jinja2ctx is None or jinja2Lock is None:
+        raise ValueError("You should pass both jinja2ctx and jinja2Lock or "
+                         "You should have HiYaPyCo.jinja2ctx and HiYaPyCo.jinja2Lock not None"
+                         )
+
+    with jinja2Lock:
+        variable_start_string = jinja2ctx.variable_start_string
+        variable_end_string = jinja2ctx.variable_end_string
+        block_start_string = jinja2ctx.block_start_string
+        block_end_string = jinja2ctx.block_end_string
+
+        jinja2ctx.variable_start_string = '@@{@|'
+        jinja2ctx.variable_end_string = '|@}@@'
+        jinja2ctx.block_start_string = '%%{%|'
+        jinja2ctx.block_end_string = '|%}%%'
+
+        try:
+            yield jinja2ctx
+        finally:
+            jinja2ctx.variable_start_string = variable_start_string
+            jinja2ctx.variable_end_string = variable_end_string
+            jinja2ctx.block_start_string = block_start_string
+            jinja2ctx.block_end_string = block_end_string
+
+
+# # support for tag 'tag:yaml.org,2002:python/object/apply:collections.OrderedDict'
+# _represent_dict_order = lambda self, data:  self.represent_mapping('tag:yaml.org,2002:map', data.items())
+# yaml.add_representer(OrderedDict, _represent_dict_order)
+
+#
+# _hiyapyco.load("\n") #_hiyapyco._usedefaultyamlloader = False
+
+
+
+def initConfig(**kwargs):
+    """
+    This method can be optionally called prior any call to another function in this module.
+    It is indented to be called in the MainThread.
+    This method can be call with empty params.
+
+    Note: this module doesn't use any package-level variables in hiYaPyCo module.
+
+    :param jinja2Lock: lock to use for synchronization in DisableVarSubst and load().
+                      If not supplied, default RLock is used.
+                      Will be available as HiYaPyCo.jinja2Lock.
+    :param jinja2ctx: context for overriding values in initialization (default is _DebugUndefined) of Jinja2 Environment:
+                      gloabls will be override values in Environment.globals.update(**globals)
+                      Default is 'uname':platform.uname
+                      Will be available as HiYaPyCo.jinja2ctx.
+    :param load: this params will be used as default values in load() function. See hiyapyco.load()
+                Default values are
+                      'method':_hiyapyco.METHOD_SUBSTITUTE,
+                      'mergelists':False,
+                      'interpolate':True,
+                      'castinterpolated':True
+                This means, by default:
+                      We're replacing list, not merging them.
+                      We're interpolating values in the data (to scalar/list/OrderDict).
+                      We're also using casting to appropriate type.
+    :param safe_dump: this params will be used as default values in safe_dump() and as_str(). See yaml.dump_all()
+                Default values are
+                      'default_flow_style':False,
+                      'sort_keys':False
+                This means, by default:
+                       we prefer block style always.
+                       we preserve the key order (no sorting for key in the dictionary).
+
+    If running from the MainThread, this method is idempotent.
+
+    :return:
+    """
+    jinja2Lock_p = kwargs.get('jinja2Lock', None)
+    if jinja2Lock_p is None:
+        jinja2Lock_p = _Lock()
+    HiYaPyCo.jinja2Lock = jinja2Lock_p
+
+    jinja2ctx_d = kwargs.get('jinja2ctx', {})
+    globals_d = jinja2ctx_d.pop('globals', {})
+    # jinja2ctx_p = _Environment(undefined=_StrictUndefined)
+    jinja2ctx_p = _Environment(**{'undefined':_DebugUndefined, **jinja2ctx_d})
+    jinja2ctx_p.globals.update(**{'uname':_uname, **globals_d})
+
+
+    with HiYaPyCo.jinja2Lock:
+        HiYaPyCo.jinja2ctx = jinja2ctx_p
+
+
+    load_d = kwargs.get('load', {})
+    _load_d_p = {'method':_hiyapyco.METHOD_SUBSTITUTE,
+               'mergelists':False,
+               'interpolate':True,
+               'castinterpolated':True,
+               **load_d}
+
+    method = _load_d_p['method']
+    # TODO: HiYaPyCo._substmerge() bug workarround, see https://github.com/zerwes/hiyapyco/pull/38
+    HiYaPyCo._deepmerge = _HiYaPyCo._substmerge
+    if method == _hiyapyco.METHOD_MERGE:
+        #restore original _deepmerge
+        HiYaPyCo._deepmerge = _HiYaPyCo._deepmerge
+    global _load_d
+    _load_d = _load_d_p
+
+
+    safe_dump_d = kwargs.get('safe_dump', {})
+    global _safe_dump_d
+    #See https://github.com/yaml/pyyaml/pull/256
+    _safe_dump_d = {'default_flow_style':False,
+                        'sort_keys':False,
+                        **safe_dump_d}
+
+
+
 initConfig()
```

### Comparing `alex_ber_utils-0.6.6b3/setup.py` & `alex_ber_utils-0.7.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 
 import setuptools
 from setuptools import setup
 
 
 #VERSION should be defined before importing UploadCommand
-VERSION = '0.6.6b3'
+VERSION = '0.7.0'
 from alexber.utils import UploadCommand
 NAME = 'alex_ber_utils'
 SHORT_NAME = 'utils'
 VCS_URL = 'https://github.com/alex-ber/AlexBerUtils'
 DESCRIPTION = 'AlexBerUtils is collection of the small utilities'
 AUTHOR = 'Alexander Berkovich'
 
@@ -97,14 +97,17 @@
             # List of python versions and their support status:
             # https://en.wikipedia.org/wiki/CPython#Version_history
             'Programming Language :: Python',
             'Programming Language :: Python :: 3 :: Only',
             'Programming Language :: Python :: 3.6',
             'Programming Language :: Python :: 3.7',
             'Programming Language :: Python :: 3.8',
+            'Programming Language :: Python :: 3.9',
+            'Programming Language :: Python :: 3.10',
+            'Programming Language :: Python :: 3.11',
             'Programming Language :: Python :: Implementation :: CPython',
             "Topic :: Utilities",
             'Topic :: Software Development :: Libraries :: Python Modules',
             'Topic :: Desktop Environment',
             'Topic :: Education',
             'Operating System :: OS Independent',
             'Operating System :: Microsoft :: Windows',
```

### Comparing `alex_ber_utils-0.6.6b3/tests/conftest.py` & `alex_ber_utils-0.7.0/tests/conftest.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-#one-time setup
-import os
-cwd = os.getcwd()
-if cwd.endswith('AlexBerUtils'):
-    os.chdir(os.path.join(cwd, 'data'))
-
-import pytest
-
-ismultidispatchfound = False
-try:
-    # pip install multidispatch==0.2
-    #python3 -m pip install .[md]
-    from multidispatch import multimethod
-    ismultidispatchfound = True
-except ImportError:
-    pass
-
-isyamlrelatedfound = False
-try:
-    #python3 -m pip install .[yaml]
-    import alexber.utils._ymlparsers_extra as ymlparsers_extra
-    if ymlparsers_extra._isHiYaPyCoAvailable and ymlparsers_extra._isJinja2DefaultAvailable:
-        isyamlrelatedfound = True
-except ImportError:
-    pass
-
-
-#see https://docs.pytest.org/en/latest/example/simple.html#control-skipping-of-tests-according-to-command-line-option
-def skip_tests(config=None, items=None, keyword=None, reason=None):
-    if items is None:
-        TypeError("items can't be None")
-
-    if reason is None:
-        TypeError("reason can't be None")
-
-    if keyword is None:
-        TypeError("keyword can't be None")
-
-    skip = pytest.mark.skip(reason=reason)
-    for item in items:
-        if keyword in item.keywords:
-            item.add_marker(skip)
-
-
-
-#see https://docs.pytest.org/en/latest/example/simple.html#control-skipping-of-tests-according-to-command-line-option
-def pytest_collection_modifyitems(config, items):
-    if not ismultidispatchfound:
-        skip_tests(items=items, keyword="md", reason="multidispatch is not installed..")
-
-    if not isyamlrelatedfound:
-        skip_tests(items=items, keyword="yml", reason="yml is not installed..")
-
-#see https://docs.pytest.org/en/latest/mark.html
-#see https://docs.pytest.org/en/latest/example/simple.html#control-skipping-of-tests-according-to-command-line-option
-def pytest_configure(config):
-    config.addinivalue_line(
-        "markers", "yml: yml is not installed.."
-    )
-    config.addinivalue_line(
-        "markers", "md: multidispatch is not installed.."
+#one-time setup
+import os
+cwd = os.getcwd()
+if cwd.endswith('AlexBerUtils'):
+    os.chdir(os.path.join(cwd, 'data'))
+
+import pytest
+
+ismultidispatchfound = False
+try:
+    # pip install multidispatch==0.2
+    #python3 -m pip install .[md]
+    from multidispatch import multimethod
+    ismultidispatchfound = True
+except ImportError:
+    pass
+
+isyamlrelatedfound = False
+try:
+    #python3 -m pip install .[yaml]
+    import alexber.utils._ymlparsers_extra as ymlparsers_extra
+    if ymlparsers_extra._isHiYaPyCoAvailable and ymlparsers_extra._isJinja2DefaultAvailable:
+        isyamlrelatedfound = True
+except ImportError:
+    pass
+
+
+#see https://docs.pytest.org/en/latest/example/simple.html#control-skipping-of-tests-according-to-command-line-option
+def skip_tests(config=None, items=None, keyword=None, reason=None):
+    if items is None:
+        TypeError("items can't be None")
+
+    if reason is None:
+        TypeError("reason can't be None")
+
+    if keyword is None:
+        TypeError("keyword can't be None")
+
+    skip = pytest.mark.skip(reason=reason)
+    for item in items:
+        if keyword in item.keywords:
+            item.add_marker(skip)
+
+
+
+#see https://docs.pytest.org/en/latest/example/simple.html#control-skipping-of-tests-according-to-command-line-option
+def pytest_collection_modifyitems(config, items):
+    if not ismultidispatchfound:
+        skip_tests(items=items, keyword="md", reason="multidispatch is not installed..")
+
+    if not isyamlrelatedfound:
+        skip_tests(items=items, keyword="yml", reason="yml is not installed..")
+
+#see https://docs.pytest.org/en/latest/mark.html
+#see https://docs.pytest.org/en/latest/example/simple.html#control-skipping-of-tests-according-to-command-line-option
+def pytest_configure(config):
+    config.addinivalue_line(
+        "markers", "yml: yml is not installed.."
+    )
+    config.addinivalue_line(
+        "markers", "md: multidispatch is not installed.."
     )
```

### Comparing `alex_ber_utils-0.6.6b3/tests/utils/deploys_test.py` & `alex_ber_utils-0.7.0/tests/utils/deploys_test.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,156 +1,156 @@
-import logging
-import pytest
-from importlib.resources import path
-from pathlib import Path
-
-from alexber.utils.deploys import split_path, load_config, add_to_zip_copy_function
-from tests.utils.ymlparsers_test import ymlparsersSetup, ymlparsersCleanup, exp_config_d
-from tests.utils.init_app_conf_test import initappconfFixture
-import copy
-import tempfile
-import zipfile
-import shutil
-try:
-    import alexber.utils.ymlparsers as ymlparsers
-except ImportError:
-    pass
-logger = logging.getLogger(__name__)
-
-class TestSplitPath(object):
-    def test_split_path_intented(self, request):
-        logger.info(f'{request._pyfuncitem.name}()')
-        split_dirname = 'ymlparsers'
-        pck = '.'.join(['tests_data', __package__, split_dirname])
-
-        with path(pck, 'config.yml') as f:
-            first_part, second_part = split_path(f, split_dirname)
-            pytest.assume(f.parent==first_part)
-            pytest.assume('config.yml'==str(second_part))
-
-    def test_split_path_intented_path(self, request):
-        logger.info(f'{request._pyfuncitem.name}()')
-        split_dirname = 'ymlparsers'
-        pck = '.'.join(['tests_data', __package__, split_dirname])
-
-        with path(pck, 'config.yml') as f:
-            first_part, second_part = split_path(Path(f), Path(split_dirname))
-            pytest.assume(f.parent==first_part)
-            pytest.assume('config.yml'==str(second_part))
-
-
-
-    def test_split_path_absent_undefined_behaviour(self, request):
-        logger.info(f'{request._pyfuncitem.name}()')
-        pck = '.'.join(['tests_data', __package__, 'ymlparsers'])
-
-        with path(pck, 'config.yml') as f:
-            with pytest.raises(BaseException):
-                split_path(f, 'xxxnotfoundxxx')
-
-
-    def test_split_path_absent_compount_name(self, request):
-        logger.info(f'{request._pyfuncitem.name}()')
-        pck = '.'.join(['tests_data', __package__, 'ymlparsers'])
-
-        with path(pck, 'config.yml') as f:
-            with pytest.raises(BaseException):
-                split_path(f, str(Path('ymlparsers', 'config.yml')))
-
-    def test_split_path_None(self, request):
-        logger.info(f'{request._pyfuncitem.name}()')
-        split_dirname = 'ymlparsers'
-        pck = '.'.join(['tests_data', __package__, split_dirname])
-
-        with path(pck, 'config.yml') as f:
-            with pytest.raises(BaseException, match='None'):
-                split_path(f, None)
-
-    def test_split_path_empty_str(self, request):
-        logger.info(f'{request._pyfuncitem.name}()')
-        split_dirname = 'ymlparsers'
-        pck = '.'.join(['tests_data', __package__, split_dirname])
-
-        with path(pck, 'config.yml') as f:
-            with pytest.raises(BaseException):
-                split_path(f, None)
-
-    def test_split_path_twice_split_dir(self, request):
-        logger.info(f'{request._pyfuncitem.name}()')
-        split_dirname = 'tests'
-        pck = '.'.join(['tests_data', __package__, 'ymlparsers'])
-
-        with path(pck, 'config.yml') as f:
-            assert split_dirname in f.parts
-            duplicate_dir_base = f.parent / split_dirname
-            duplicate_dir_full_path = duplicate_dir_base / f.name
-            first_part, second_part = split_path(duplicate_dir_full_path, split_dirname)
-
-            pytest.assume(duplicate_dir_base==first_part)
-            pytest.assume('config.yml'==str(second_part))
-
-def check_config_yml(default_d, exp_d):
-
-
-    app_d = default_d.get('app', None)
-    exp_app_d = exp_d.get('app', None)
-
-    inner_host_name = app_d.get('inner_host_name', None)
-    exp_host_name = exp_app_d.get('inner_host_name', None)
-    pytest.assume(exp_host_name==inner_host_name)
-    cli_template = app_d.get('cli_template')
-    pytest.assume('inner_host_name' in cli_template)
-    pytest.assume(exp_d == default_d)
-
-@pytest.mark.yml
-def test_load_config(request, mocker, ymlparsersSetup, ymlparsersCleanup, initappconfFixture, exp_config_d):
-    logger.info(f'{request._pyfuncitem.name}()')
-
-    pck = '.'.join(['tests_data', __package__, 'ymlparsers'])
-    exp_profiles=['dev']
-    with path(pck, 'config.yml') as full_path:
-        args = f"--general.config.file={full_path} --general.profiles={exp_profiles[0]}".split()
-        config_path, default_d = load_config(None, args)
-
-    pytest.assume(full_path == config_path)
-    general_d = default_d.get('general', None)
-    profiles = general_d.get('profiles', None)
-    pytest.assume(exp_profiles == profiles)
-
-    exp_d = copy.deepcopy(exp_config_d)
-    exp_d['general']['profiles'] = exp_profiles
-
-    check_config_yml(default_d, exp_d)
-
-@pytest.mark.yml
-def test_add_to_zip_copy_function(request, mocker,  ymlparsersSetup, ymlparsersCleanup, exp_config_d):
-    logger.info(f'{request._pyfuncitem.name}()')
-    split_dirname = 'ymlparsers'
-    pck = '.'.join(['tests_data', __package__, 'ymlparsers'])
-
-    with path(pck, 'config.yml') as full_path:
-
-
-        with tempfile.TemporaryDirectory() as temp_dir:
-            local_folder = Path(temp_dir)
-            zip_path = local_folder / "my.zip"
-            with zipfile.ZipFile(zip_path, mode="w") as zf:
-                # not real copy, add to zip archive
-                shutil.copytree(str(full_path.parent), str(local_folder / "xxxirrelevantxxx"),
-                                ignore=shutil.ignore_patterns('__pycache__', 'venv', 'logs', '*.pyc', 'tmp*',
-                                                              '.*', "__init__.py"),
-                                copy_function=add_to_zip_copy_function(split_dirname=split_dirname, zf=zf),
-                                symlinks=True, ignore_dangling_symlinks=True)
-            with zipfile.ZipFile(zip_path, mode="r") as zf:
-                entry_path = (Path(split_dirname) / 'config.yml').as_posix()
-                entry_content_bytes = zf.read(str(entry_path))
-
-                with ymlparsers.DisableVarSubst():
-                    default_d = ymlparsers.load([entry_content_bytes.decode('utf-8')])
-
-        check_config_yml(default_d, exp_config_d)
-
-
-
-if __name__ == "__main__":
-    pytest.main([__file__])
-
+import logging
+import pytest
+from importlib.resources import path
+from pathlib import Path
+
+from alexber.utils.deploys import split_path, load_config, add_to_zip_copy_function
+from tests.utils.ymlparsers_test import ymlparsersSetup, ymlparsersCleanup, exp_config_d
+from tests.utils.init_app_conf_test import initappconfFixture
+import copy
+import tempfile
+import zipfile
+import shutil
+try:
+    import alexber.utils.ymlparsers as ymlparsers
+except ImportError:
+    pass
+logger = logging.getLogger(__name__)
+
+class TestSplitPath(object):
+    def test_split_path_intented(self, request):
+        logger.info(f'{request._pyfuncitem.name}()')
+        split_dirname = 'ymlparsers'
+        pck = '.'.join(['tests_data', __package__, split_dirname])
+
+        with path(pck, 'config.yml') as f:
+            first_part, second_part = split_path(f, split_dirname)
+            pytest.assume(f.parent==first_part)
+            pytest.assume('config.yml'==str(second_part))
+
+    def test_split_path_intented_path(self, request):
+        logger.info(f'{request._pyfuncitem.name}()')
+        split_dirname = 'ymlparsers'
+        pck = '.'.join(['tests_data', __package__, split_dirname])
+
+        with path(pck, 'config.yml') as f:
+            first_part, second_part = split_path(Path(f), Path(split_dirname))
+            pytest.assume(f.parent==first_part)
+            pytest.assume('config.yml'==str(second_part))
+
+
+
+    def test_split_path_absent_undefined_behaviour(self, request):
+        logger.info(f'{request._pyfuncitem.name}()')
+        pck = '.'.join(['tests_data', __package__, 'ymlparsers'])
+
+        with path(pck, 'config.yml') as f:
+            with pytest.raises(BaseException):
+                split_path(f, 'xxxnotfoundxxx')
+
+
+    def test_split_path_absent_compount_name(self, request):
+        logger.info(f'{request._pyfuncitem.name}()')
+        pck = '.'.join(['tests_data', __package__, 'ymlparsers'])
+
+        with path(pck, 'config.yml') as f:
+            with pytest.raises(BaseException):
+                split_path(f, str(Path('ymlparsers', 'config.yml')))
+
+    def test_split_path_None(self, request):
+        logger.info(f'{request._pyfuncitem.name}()')
+        split_dirname = 'ymlparsers'
+        pck = '.'.join(['tests_data', __package__, split_dirname])
+
+        with path(pck, 'config.yml') as f:
+            with pytest.raises(BaseException, match='None'):
+                split_path(f, None)
+
+    def test_split_path_empty_str(self, request):
+        logger.info(f'{request._pyfuncitem.name}()')
+        split_dirname = 'ymlparsers'
+        pck = '.'.join(['tests_data', __package__, split_dirname])
+
+        with path(pck, 'config.yml') as f:
+            with pytest.raises(BaseException):
+                split_path(f, None)
+
+    def test_split_path_twice_split_dir(self, request):
+        logger.info(f'{request._pyfuncitem.name}()')
+        split_dirname = 'tests'
+        pck = '.'.join(['tests_data', __package__, 'ymlparsers'])
+
+        with path(pck, 'config.yml') as f:
+            assert split_dirname in f.parts
+            duplicate_dir_base = f.parent / split_dirname
+            duplicate_dir_full_path = duplicate_dir_base / f.name
+            first_part, second_part = split_path(duplicate_dir_full_path, split_dirname)
+
+            pytest.assume(duplicate_dir_base==first_part)
+            pytest.assume('config.yml'==str(second_part))
+
+def check_config_yml(default_d, exp_d):
+
+
+    app_d = default_d.get('app', None)
+    exp_app_d = exp_d.get('app', None)
+
+    inner_host_name = app_d.get('inner_host_name', None)
+    exp_host_name = exp_app_d.get('inner_host_name', None)
+    pytest.assume(exp_host_name==inner_host_name)
+    cli_template = app_d.get('cli_template')
+    pytest.assume('inner_host_name' in cli_template)
+    pytest.assume(exp_d == default_d)
+
+@pytest.mark.yml
+def test_load_config(request, mocker, ymlparsersSetup, ymlparsersCleanup, initappconfFixture, exp_config_d):
+    logger.info(f'{request._pyfuncitem.name}()')
+
+    pck = '.'.join(['tests_data', __package__, 'ymlparsers'])
+    exp_profiles=['dev']
+    with path(pck, 'config.yml') as full_path:
+        args = f"--general.config.file={full_path} --general.profiles={exp_profiles[0]}".split()
+        config_path, default_d = load_config(None, args)
+
+    pytest.assume(full_path == config_path)
+    general_d = default_d.get('general', None)
+    profiles = general_d.get('profiles', None)
+    pytest.assume(exp_profiles == profiles)
+
+    exp_d = copy.deepcopy(exp_config_d)
+    exp_d['general']['profiles'] = exp_profiles
+
+    check_config_yml(default_d, exp_d)
+
+@pytest.mark.yml
+def test_add_to_zip_copy_function(request, mocker,  ymlparsersSetup, ymlparsersCleanup, exp_config_d):
+    logger.info(f'{request._pyfuncitem.name}()')
+    split_dirname = 'ymlparsers'
+    pck = '.'.join(['tests_data', __package__, 'ymlparsers'])
+
+    with path(pck, 'config.yml') as full_path:
+
+
+        with tempfile.TemporaryDirectory() as temp_dir:
+            local_folder = Path(temp_dir)
+            zip_path = local_folder / "my.zip"
+            with zipfile.ZipFile(zip_path, mode="w") as zf:
+                # not real copy, add to zip archive
+                shutil.copytree(str(full_path.parent), str(local_folder / "xxxirrelevantxxx"),
+                                ignore=shutil.ignore_patterns('__pycache__', 'venv', 'logs', '*.pyc', 'tmp*',
+                                                              '.*', "__init__.py"),
+                                copy_function=add_to_zip_copy_function(split_dirname=split_dirname, zf=zf),
+                                symlinks=True, ignore_dangling_symlinks=True)
+            with zipfile.ZipFile(zip_path, mode="r") as zf:
+                entry_path = (Path(split_dirname) / 'config.yml').as_posix()
+                entry_content_bytes = zf.read(str(entry_path))
+
+                with ymlparsers.DisableVarSubst():
+                    default_d = ymlparsers.load([entry_content_bytes.decode('utf-8')])
+
+        check_config_yml(default_d, exp_config_d)
+
+
+
+if __name__ == "__main__":
+    pytest.main([__file__])
+
```

### Comparing `alex_ber_utils-0.6.6b3/tests/utils/emails_test.py` & `alex_ber_utils-0.7.0/tests/utils/emails_test.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,257 +1,257 @@
-import logging
-import threading
-import time
-import pytest
-from smtplib import SMTP as _SMTP, LMTP as _LMTP
-from alexber.utils.emails import SMTPHandler, OneMemoryHandler
-import alexber.utils.emails as emails
-#don't remove this
-from platform import uname
-from alexber.utils.emails import EmailStatus, FINISHED
-logger = logging.getLogger(__name__)
-emailLogger = None
-
-@pytest.fixture
-def errorMailHandler(mocker):
-
-    d1 = {
-     #   'level': logging.DEBUG,
-        'smtpclsname': 'smtplib.SMTP',
-        'mailhost': ['smtp-relay.gmail.com', 587],
-        'fromaddr': f'{{uname()[1]}}@gmail.com',
-        'toaddrs': ['no-reply@gmail.com'],
-        'subject': 'mail_subject'
-    }
-
-    error_email_handler = SMTPHandler(**d1)
-    error_email_handler.setLevel(logging.DEBUG)
-
-    mocker.patch.object(error_email_handler, 'emit',autospec=True, spec_set=True)
-    return error_email_handler
-
-
-@pytest.fixture
-def emailsSubject(request, mocker):
-    request_param = 'Process Status : {{status}}' if (
-        not hasattr(request, 'param')) else request.param
-    yield request_param
-
-@pytest.fixture
-def errorMailMemoryHandler(request, mocker, errorMailHandler, emailsSubject):
-
-    d2 = {
-        #'formatter': detailFormatter,
-        #'subject': 'Process Status : {{status}}',
-        'subject': emailsSubject,
-        #'target': error_email_handler
-    }
-
-    detailFormatter = logging.Formatter('%(asctime)-15s %(levelname)s [%(name)s.%(funcName)s] %(message)s',
-                                        '%Y-%m-%d %H:%M:%S')
-    error_mail_memory_handler = OneMemoryHandler(**d2)
-    error_mail_memory_handler.setFormatter(detailFormatter)
-    error_mail_memory_handler.setTarget(errorMailHandler)
-    return error_mail_memory_handler
-
-@pytest.fixture
-def emailsFixture(request, mocker, errorMailMemoryHandler):
-    global emailLogger
-    emailLogger = logging.getLogger('emails')
-    propagate_param = emailLogger.propagate if (not hasattr(request, 'param')) else request.param
-    prev_propogate = emailLogger.propagate
-    emailLogger.propagate = propagate_param
-    emailLogger.addHandler(errorMailMemoryHandler)
-    yield errorMailMemoryHandler.target
-    emailLogger.removeHandler(errorMailMemoryHandler)
-    emailLogger.propagate = prev_propogate
-
-def run_successfuly():
-    logger.debug("run_successfuly()")
-    emailLogger.info("Start - Process")
-    emailLogger.info("Step 1")
-    emailLogger.info("Step 2")
-    emailLogger.info("Done Successfully - Process")
-
-def run_with_failure():
-    logger.debug("run_with_failure()")
-    emailLogger.info("Start - Process")
-    emailLogger.info("Step 1")
-    1/0
-    emailLogger.info("Step 2")
-    emailLogger.info("Done Successfully - Process")
-
-def is_failed(logrecord):
-    subject = str(logrecord.msg['subject'])
-    assert '{status}' not in subject
-    assert 'Done' in subject or 'Failed' in subject
-    b = 'Failed' in subject
-    return b
-
-def check_failed(logrecord):
-    subject = str(logrecord.msg['subject'])
-    pytest.assume('Failed' in subject)
-    pytest.assume('{status}' not in subject)
-    message = str(logrecord.msg)
-    pytest.assume('Start' in message)
-    pytest.assume('division by zero' in message)
-    pytest.assume('Step 1' in message)
-    pytest.assume('Step 2' not in message)
-
-
-def check_sucess(logrecord):
-    subject = str(logrecord.msg['subject'])
-    pytest.assume('Done' in subject)
-    pytest.assume('{status}' not in subject)
-    message = str(logrecord.msg)
-    pytest.assume('Start' in message)
-    pytest.assume('Step 1' in message)
-    pytest.assume('Step 2' in message)
-
-def test_emails_intented_success(request, mocker, emailsFixture):
-    logger.info(f'{request._pyfuncitem.name}()')
-
-    with EmailStatus(emailLogger=emailLogger, logger=None, faildargs={'status': 'Failed'},
-                     successargs={'status': 'Done'}):
-        run_successfuly()
-    mock_log = emailsFixture.emit
-    pytest.assume(mock_log.call_count == 1)
-    (logrecord,), _ = mock_log.call_args
-
-    check_sucess(logrecord)
-
-#emailsSubject
-@pytest.mark.parametrize('emailsSubject', ['Aggregates log from the Demo application',
-                                                    ], indirect=True)
-def test_emails_intented_simple_success(request, mocker, emailsFixture, emailsSubject):
-    logger.info(f'{request._pyfuncitem.name}()')
-
-    emailLogger.log(FINISHED, None)
-    mock_log = emailsFixture.emit
-    pytest.assume(mock_log.call_count == 1)
-    (logrecord,), _ = mock_log.call_args
-    subject = str(logrecord.msg['subject'])
-    pytest.assume(emailsSubject in subject)
-
-#emailsSubject
-@pytest.mark.parametrize('emailsSubject', ['Aggregates log from the Demo application',
-                                                    ], indirect=True)
-def test_emails_intented_simple_success2(request, mocker, emailsFixture, emailsSubject):
-    logger.info(f'{request._pyfuncitem.name}()')
-
-    emailLogger.log(FINISHED, '')
-    mock_log = emailsFixture.emit
-    pytest.assume(mock_log.call_count == 1)
-    (logrecord,), _ = mock_log.call_args
-    subject = str(logrecord.msg['subject'])
-    pytest.assume(emailsSubject in subject)
-
-#emailsSubject
-@pytest.mark.parametrize('emailsSubject', ['Aggregates log from the Demo application',
-                                                    ], indirect=True)
-def test_emails_intented_simple_success_wrong(request, mocker, emailsFixture, emailsSubject):
-    logger.info(f'{request._pyfuncitem.name}()')
-
-    with pytest.raises(ValueError):
-        emailLogger.log(FINISHED, ['some non-dict value'])
-
-@pytest.fixture
-def specialAbruptCleanup(request, mocker):
-    yield None
-    setattr(emails._thread_locals, 'buffer', [])
-
-
-def test_emails_intented_abrupt_execution(request, mocker, emailsFixture, errorMailMemoryHandler, specialAbruptCleanup):
-    logger.info(f'{request._pyfuncitem.name}()')
-    emailLogger.info("Started")
-    emailLogger.info('Step 1')
-    logging.shutdown([lambda: errorMailMemoryHandler])
-    emailLogger.info('Step 2')
-
-    mock_log = emailsFixture.emit
-    pytest.assume(mock_log.call_count == 1)
-    (logrecord,), _ = mock_log.call_args
-
-    subject = str(logrecord.msg['subject'])
-    pytest.assume('Abrupt' in subject)
-    pytest.assume('{status}' not in subject)
-    message = str(logrecord.msg)
-    pytest.assume('Start' in message)
-    pytest.assume('Step 1' in message)
-    pytest.assume('Step 2' not in message)
-
-
-@pytest.mark.parametrize('emailsFixture', [False], indirect=True)
-def test_emails_intented_failure(request, mocker, emailsFixture):
-    logger.info(f'{request._pyfuncitem.name}()')
-
-
-    with EmailStatus(emailLogger=emailLogger, logger=None, faildargs={'status': 'Failed'},
-                     successargs={'status': 'Done'}):
-        run_with_failure()
-    mock_log = emailsFixture.emit
-    pytest.assume(mock_log.call_count == 1)
-    (logrecord,), _ = mock_log.call_args
-
-
-    check_failed(logrecord)
-
-
-def test_init_config_default(request, mocker, emailsFixture):
-    logger.info(f'{request._pyfuncitem.name}()')
-    emails.initConfig()
-    pytest.assume(_SMTP==emails.default_smtp_cls)
-
-
-def test_init_config2(request, mocker, emailsFixture):
-    logger.info(f'{request._pyfuncitem.name}()')
-    exp_default_smtp_port='9000'
-    emails.initConfig(default_smtp_cls_name='smtplib.LMTP')
-    pytest.assume(_LMTP==emails.default_smtp_cls)
-
-
-@pytest.mark.parametrize('emailsFixture', [False], indirect=True)
-def test_emails_multithreaded(request, mocker, emailsFixture):
-    logger.info(f'{request._pyfuncitem.name}()')
-
-    stop =10
-
-    def _run_successfuly(stop):
-        for i in range(stop):
-            with EmailStatus(emailLogger=emailLogger, logger=None, faildargs={'status': 'Failed'},
-                             successargs={'status': 'Done'}):
-                run_successfuly()
-        time.sleep(1)
-
-    def _run_with_failure(stop):
-        for i in range(stop):
-            with EmailStatus(emailLogger=emailLogger, logger=None, faildargs={'status': 'Failed'},
-                             successargs={'status': 'Done'}):
-                run_with_failure()
-
-
-    th1 = threading.Thread(name="run_successfuly",
-                               target=_run_successfuly, args=(stop,))
-
-    th2 = threading.Thread(name="run_with_failure",
-                           target=_run_with_failure, args=(stop,))
-
-    th1.start()
-    th2.start()
-    th1.join()
-    th2.join()
-
-    mock_log = emailsFixture.emit
-    pytest.assume(mock_log.call_count == 2*stop)
-    for kall in mock_log.call_args_list:
-        (logrecord,), _ = kall
-        if is_failed(logrecord):
-            check_failed(logrecord)
-        else:
-            check_sucess(logrecord)
-
-
-
-
-
-if __name__ == "__main__":
-    pytest.main([__file__])
+import logging
+import threading
+import time
+import pytest
+from smtplib import SMTP as _SMTP, LMTP as _LMTP
+from alexber.utils.emails import SMTPHandler, OneMemoryHandler
+import alexber.utils.emails as emails
+#don't remove this
+from platform import uname
+from alexber.utils.emails import EmailStatus, FINISHED
+logger = logging.getLogger(__name__)
+emailLogger = None
+
+@pytest.fixture
+def errorMailHandler(mocker):
+
+    d1 = {
+     #   'level': logging.DEBUG,
+        'smtpclsname': 'smtplib.SMTP',
+        'mailhost': ['smtp-relay.gmail.com', 587],
+        'fromaddr': f'{{uname()[1]}}@gmail.com',
+        'toaddrs': ['no-reply@gmail.com'],
+        'subject': 'mail_subject'
+    }
+
+    error_email_handler = SMTPHandler(**d1)
+    error_email_handler.setLevel(logging.DEBUG)
+
+    mocker.patch.object(error_email_handler, 'emit',autospec=True, spec_set=True)
+    return error_email_handler
+
+
+@pytest.fixture
+def emailsSubject(request, mocker):
+    request_param = 'Process Status : {{status}}' if (
+        not hasattr(request, 'param')) else request.param
+    yield request_param
+
+@pytest.fixture
+def errorMailMemoryHandler(request, mocker, errorMailHandler, emailsSubject):
+
+    d2 = {
+        #'formatter': detailFormatter,
+        #'subject': 'Process Status : {{status}}',
+        'subject': emailsSubject,
+        #'target': error_email_handler
+    }
+
+    detailFormatter = logging.Formatter('%(asctime)-15s %(levelname)s [%(name)s.%(funcName)s] %(message)s',
+                                        '%Y-%m-%d %H:%M:%S')
+    error_mail_memory_handler = OneMemoryHandler(**d2)
+    error_mail_memory_handler.setFormatter(detailFormatter)
+    error_mail_memory_handler.setTarget(errorMailHandler)
+    return error_mail_memory_handler
+
+@pytest.fixture
+def emailsFixture(request, mocker, errorMailMemoryHandler):
+    global emailLogger
+    emailLogger = logging.getLogger('emails')
+    propagate_param = emailLogger.propagate if (not hasattr(request, 'param')) else request.param
+    prev_propogate = emailLogger.propagate
+    emailLogger.propagate = propagate_param
+    emailLogger.addHandler(errorMailMemoryHandler)
+    yield errorMailMemoryHandler.target
+    emailLogger.removeHandler(errorMailMemoryHandler)
+    emailLogger.propagate = prev_propogate
+
+def run_successfuly():
+    logger.debug("run_successfuly()")
+    emailLogger.info("Start - Process")
+    emailLogger.info("Step 1")
+    emailLogger.info("Step 2")
+    emailLogger.info("Done Successfully - Process")
+
+def run_with_failure():
+    logger.debug("run_with_failure()")
+    emailLogger.info("Start - Process")
+    emailLogger.info("Step 1")
+    1/0
+    emailLogger.info("Step 2")
+    emailLogger.info("Done Successfully - Process")
+
+def is_failed(logrecord):
+    subject = str(logrecord.msg['subject'])
+    assert '{status}' not in subject
+    assert 'Done' in subject or 'Failed' in subject
+    b = 'Failed' in subject
+    return b
+
+def check_failed(logrecord):
+    subject = str(logrecord.msg['subject'])
+    pytest.assume('Failed' in subject)
+    pytest.assume('{status}' not in subject)
+    message = str(logrecord.msg)
+    pytest.assume('Start' in message)
+    pytest.assume('division by zero' in message)
+    pytest.assume('Step 1' in message)
+    pytest.assume('Step 2' not in message)
+
+
+def check_sucess(logrecord):
+    subject = str(logrecord.msg['subject'])
+    pytest.assume('Done' in subject)
+    pytest.assume('{status}' not in subject)
+    message = str(logrecord.msg)
+    pytest.assume('Start' in message)
+    pytest.assume('Step 1' in message)
+    pytest.assume('Step 2' in message)
+
+def test_emails_intented_success(request, mocker, emailsFixture):
+    logger.info(f'{request._pyfuncitem.name}()')
+
+    with EmailStatus(emailLogger=emailLogger, logger=None, faildargs={'status': 'Failed'},
+                     successargs={'status': 'Done'}):
+        run_successfuly()
+    mock_log = emailsFixture.emit
+    pytest.assume(mock_log.call_count == 1)
+    (logrecord,), _ = mock_log.call_args
+
+    check_sucess(logrecord)
+
+#emailsSubject
+@pytest.mark.parametrize('emailsSubject', ['Aggregates log from the Demo application',
+                                                    ], indirect=True)
+def test_emails_intented_simple_success(request, mocker, emailsFixture, emailsSubject):
+    logger.info(f'{request._pyfuncitem.name}()')
+
+    emailLogger.log(FINISHED, None)
+    mock_log = emailsFixture.emit
+    pytest.assume(mock_log.call_count == 1)
+    (logrecord,), _ = mock_log.call_args
+    subject = str(logrecord.msg['subject'])
+    pytest.assume(emailsSubject in subject)
+
+#emailsSubject
+@pytest.mark.parametrize('emailsSubject', ['Aggregates log from the Demo application',
+                                                    ], indirect=True)
+def test_emails_intented_simple_success2(request, mocker, emailsFixture, emailsSubject):
+    logger.info(f'{request._pyfuncitem.name}()')
+
+    emailLogger.log(FINISHED, '')
+    mock_log = emailsFixture.emit
+    pytest.assume(mock_log.call_count == 1)
+    (logrecord,), _ = mock_log.call_args
+    subject = str(logrecord.msg['subject'])
+    pytest.assume(emailsSubject in subject)
+
+#emailsSubject
+@pytest.mark.parametrize('emailsSubject', ['Aggregates log from the Demo application',
+                                                    ], indirect=True)
+def test_emails_intented_simple_success_wrong(request, mocker, emailsFixture, emailsSubject):
+    logger.info(f'{request._pyfuncitem.name}()')
+
+    with pytest.raises(ValueError):
+        emailLogger.log(FINISHED, ['some non-dict value'])
+
+@pytest.fixture
+def specialAbruptCleanup(request, mocker):
+    yield None
+    setattr(emails._thread_locals, 'buffer', [])
+
+
+def test_emails_intented_abrupt_execution(request, mocker, emailsFixture, errorMailMemoryHandler, specialAbruptCleanup):
+    logger.info(f'{request._pyfuncitem.name}()')
+    emailLogger.info("Started")
+    emailLogger.info('Step 1')
+    logging.shutdown([lambda: errorMailMemoryHandler])
+    emailLogger.info('Step 2')
+
+    mock_log = emailsFixture.emit
+    pytest.assume(mock_log.call_count == 1)
+    (logrecord,), _ = mock_log.call_args
+
+    subject = str(logrecord.msg['subject'])
+    pytest.assume('Abrupt' in subject)
+    pytest.assume('{status}' not in subject)
+    message = str(logrecord.msg)
+    pytest.assume('Start' in message)
+    pytest.assume('Step 1' in message)
+    pytest.assume('Step 2' not in message)
+
+
+@pytest.mark.parametrize('emailsFixture', [False], indirect=True)
+def test_emails_intented_failure(request, mocker, emailsFixture):
+    logger.info(f'{request._pyfuncitem.name}()')
+
+
+    with EmailStatus(emailLogger=emailLogger, logger=None, faildargs={'status': 'Failed'},
+                     successargs={'status': 'Done'}):
+        run_with_failure()
+    mock_log = emailsFixture.emit
+    pytest.assume(mock_log.call_count == 1)
+    (logrecord,), _ = mock_log.call_args
+
+
+    check_failed(logrecord)
+
+
+def test_init_config_default(request, mocker, emailsFixture):
+    logger.info(f'{request._pyfuncitem.name}()')
+    emails.initConfig()
+    pytest.assume(_SMTP==emails.default_smtp_cls)
+
+
+def test_init_config2(request, mocker, emailsFixture):
+    logger.info(f'{request._pyfuncitem.name}()')
+    exp_default_smtp_port='9000'
+    emails.initConfig(default_smtp_cls_name='smtplib.LMTP')
+    pytest.assume(_LMTP==emails.default_smtp_cls)
+
+
+@pytest.mark.parametrize('emailsFixture', [False], indirect=True)
+def test_emails_multithreaded(request, mocker, emailsFixture):
+    logger.info(f'{request._pyfuncitem.name}()')
+
+    stop =10
+
+    def _run_successfuly(stop):
+        for i in range(stop):
+            with EmailStatus(emailLogger=emailLogger, logger=None, faildargs={'status': 'Failed'},
+                             successargs={'status': 'Done'}):
+                run_successfuly()
+        time.sleep(1)
+
+    def _run_with_failure(stop):
+        for i in range(stop):
+            with EmailStatus(emailLogger=emailLogger, logger=None, faildargs={'status': 'Failed'},
+                             successargs={'status': 'Done'}):
+                run_with_failure()
+
+
+    th1 = threading.Thread(name="run_successfuly",
+                               target=_run_successfuly, args=(stop,))
+
+    th2 = threading.Thread(name="run_with_failure",
+                           target=_run_with_failure, args=(stop,))
+
+    th1.start()
+    th2.start()
+    th1.join()
+    th2.join()
+
+    mock_log = emailsFixture.emit
+    pytest.assume(mock_log.call_count == 2*stop)
+    for kall in mock_log.call_args_list:
+        (logrecord,), _ = kall
+        if is_failed(logrecord):
+            check_failed(logrecord)
+        else:
+            check_sucess(logrecord)
+
+
+
+
+
+if __name__ == "__main__":
+    pytest.main([__file__])
```

### Comparing `alex_ber_utils-0.6.6b3/tests/utils/enums_mixin_test.py` & `alex_ber_utils-0.7.0/tests/utils/enums_mixin_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,661 +1,640 @@
-00000000: 0d0a 696d 706f 7274 206c 6f67 6769 6e67  ..import logging
-00000010: 0d0a 696d 706f 7274 2070 7974 6573 740d  ..import pytest.
-00000020: 0a0d 0a66 726f 6d20 616c 6578 6265 722e  ...from alexber.
-00000030: 7574 696c 7320 696d 706f 7274 2053 7472  utils import Str
-00000040: 4173 5265 7072 4d69 7869 6e45 6e75 6d2c  AsReprMixinEnum,
-00000050: 204c 6f6f 6b55 704d 6978 696e 456e 756d   LookUpMixinEnum
-00000060: 2c20 4175 746f 4e61 6d65 4d69 7869 6e45  , AutoNameMixinE
-00000070: 6e75 6d2c 204d 6973 7369 6e67 4e6f 6e65  num, MissingNone
-00000080: 4d69 7869 6e45 6e75 6d2c 2045 6e75 6d0d  MixinEnum, Enum.
-00000090: 0a66 726f 6d20 616c 6578 6265 722e 7574  .from alexber.ut
-000000a0: 696c 732e 656e 756d 7320 696d 706f 7274  ils.enums import
-000000b0: 2065 6e75 6d2c 2061 7574 6f0d 0a0d 0a23   enum, auto....#
-000000c0: 2023 7573 6520 7374 616e 6461 7264 2045   #use standard E
-000000d0: 6e75 6d2e 5f5f 6e65 775f 5f0d 0a64 6566  num.__new__..def
-000000e0: 205f 6f72 6967 5f65 6e75 6d5f 6e65 7728   _orig_enum_new(
-000000f0: 636c 732c 2076 616c 7565 293a 0d0a 2020  cls, value):..  
-00000100: 2020 2320 616c 6c20 656e 756d 2069 6e73    # all enum ins
-00000110: 7461 6e63 6573 2061 7265 2061 6374 7561  tances are actua
-00000120: 6c6c 7920 6372 6561 7465 6420 6475 7269  lly created duri
-00000130: 6e67 2063 6c61 7373 2063 6f6e 7374 7275  ng class constru
-00000140: 6374 696f 6e0d 0a20 2020 2023 2077 6974  ction..    # wit
-00000150: 686f 7574 2063 616c 6c69 6e67 2074 6869  hout calling thi
-00000160: 7320 6d65 7468 6f64 3b20 7468 6973 206d  s method; this m
-00000170: 6574 686f 6420 6973 2063 616c 6c65 6420  ethod is called 
-00000180: 6279 2074 6865 206d 6574 6163 6c61 7373  by the metaclass
-00000190: 270d 0a20 2020 2023 205f 5f63 616c 6c5f  '..    # __call_
-000001a0: 5f20 2869 2e65 2e20 436f 6c6f 7228 3329  _ (i.e. Color(3)
-000001b0: 2029 2c20 616e 6420 6279 2070 6963 6b6c   ), and by pickl
-000001c0: 650d 0a20 2020 2069 6620 7479 7065 2876  e..    if type(v
-000001d0: 616c 7565 2920 6973 2063 6c73 3a0d 0a20  alue) is cls:.. 
-000001e0: 2020 2020 2020 2023 2046 6f72 206c 6f6f         # For loo
-000001f0: 6b75 7073 206c 696b 6520 436f 6c6f 7228  kups like Color(
-00000200: 436f 6c6f 722e 5245 4429 0d0a 2020 2020  Color.RED)..    
-00000210: 2020 2020 7265 7475 726e 2076 616c 7565      return value
-00000220: 0d0a 2020 2020 2320 6279 2d76 616c 7565  ..    # by-value
-00000230: 2073 6561 7263 6820 666f 7220 6120 6d61   search for a ma
-00000240: 7463 6869 6e67 2065 6e75 6d20 6d65 6d62  tching enum memb
-00000250: 6572 0d0a 2020 2020 2320 7365 6520 6966  er..    # see if
-00000260: 2069 7427 7320 696e 2074 6865 2072 6576   it's in the rev
-00000270: 6572 7365 206d 6170 7069 6e67 2028 666f  erse mapping (fo
-00000280: 7220 6861 7368 6162 6c65 2076 616c 7565  r hashable value
-00000290: 7329 0d0a 2020 2020 7472 793a 0d0a 2020  s)..    try:..  
-000002a0: 2020 2020 2020 6966 2076 616c 7565 2069        if value i
-000002b0: 6e20 636c 732e 5f76 616c 7565 326d 656d  n cls._value2mem
-000002c0: 6265 725f 6d61 705f 3a0d 0a20 2020 2020  ber_map_:..     
-000002d0: 2020 2020 2020 2072 6574 7572 6e20 636c         return cl
-000002e0: 732e 5f76 616c 7565 326d 656d 6265 725f  s._value2member_
-000002f0: 6d61 705f 5b76 616c 7565 5d0d 0a20 2020  map_[value]..   
-00000300: 2065 7863 6570 7420 5479 7065 4572 726f   except TypeErro
-00000310: 723a 0d0a 2020 2020 2020 2020 2320 6e6f  r:..        # no
-00000320: 7420 7468 6572 652c 206e 6f77 2064 6f20  t there, now do 
-00000330: 6c6f 6e67 2073 6561 7263 6820 2d2d 204f  long search -- O
-00000340: 286e 2920 6265 6861 7669 6f72 0d0a 2020  (n) behavior..  
-00000350: 2020 2020 2020 666f 7220 6d65 6d62 6572        for member
-00000360: 2069 6e20 636c 732e 5f6d 656d 6265 725f   in cls._member_
-00000370: 6d61 705f 2e76 616c 7565 7328 293a 0d0a  map_.values():..
-00000380: 2020 2020 2020 2020 2020 2020 6966 206d              if m
-00000390: 656d 6265 722e 5f76 616c 7565 5f20 3d3d  ember._value_ ==
-000003a0: 2076 616c 7565 3a0d 0a20 2020 2020 2020   value:..       
-000003b0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-000003c0: 6d65 6d62 6572 0d0a 2020 2020 2320 7374  member..    # st
-000003d0: 696c 6c20 6e6f 7420 666f 756e 6420 2d2d  ill not found --
-000003e0: 2074 7279 205f 6d69 7373 696e 675f 2068   try _missing_ h
-000003f0: 6f6f 6b0d 0a20 2020 2074 7279 3a0d 0a20  ook..    try:.. 
-00000400: 2020 2020 2020 2065 7863 203d 204e 6f6e         exc = Non
-00000410: 650d 0a20 2020 2020 2020 2072 6573 756c  e..        resul
-00000420: 7420 3d20 636c 732e 5f6d 6973 7369 6e67  t = cls._missing
-00000430: 5f28 7661 6c75 6529 0d0a 2020 2020 6578  _(value)..    ex
-00000440: 6365 7074 2045 7863 6570 7469 6f6e 2061  cept Exception a
-00000450: 7320 653a 0d0a 2020 2020 2020 2020 6578  s e:..        ex
-00000460: 6320 3d20 650d 0a20 2020 2020 2020 2072  c = e..        r
-00000470: 6573 756c 7420 3d20 4e6f 6e65 0d0a 0d0a  esult = None....
-00000480: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
-00000490: 6528 7265 7375 6c74 2c20 636c 7329 3a0d  e(result, cls):.
-000004a0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000004b0: 7265 7375 6c74 0d0a 2020 2020 656c 7365  result..    else
-000004c0: 3a0d 0a20 2020 2020 2020 2076 655f 6578  :..        ve_ex
-000004d0: 6320 3d20 5661 6c75 6545 7272 6f72 2822  c = ValueError("
-000004e0: 2572 2069 7320 6e6f 7420 6120 7661 6c69  %r is not a vali
-000004f0: 6420 2573 2220 2520 2876 616c 7565 2c20  d %s" % (value, 
-00000500: 636c 732e 5f5f 6e61 6d65 5f5f 2929 0d0a  cls.__name__))..
-00000510: 2020 2020 2020 2020 6966 2072 6573 756c          if resul
-00000520: 7420 6973 204e 6f6e 6520 616e 6420 6578  t is None and ex
-00000530: 6320 6973 204e 6f6e 653a 0d0a 2020 2020  c is None:..    
-00000540: 2020 2020 2020 2020 7261 6973 6520 7665          raise ve
-00000550: 5f65 7863 0d0a 2020 2020 2020 2020 656c  _exc..        el
-00000560: 6966 2065 7863 2069 7320 4e6f 6e65 3a0d  if exc is None:.
-00000570: 0a20 2020 2020 2020 2020 2020 2065 7863  .            exc
-00000580: 203d 2054 7970 6545 7272 6f72 280d 0a20   = TypeError(.. 
-00000590: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-000005a0: 6572 726f 7220 696e 2025 732e 5f6d 6973  error in %s._mis
-000005b0: 7369 6e67 5f3a 2072 6574 7572 6e65 6420  sing_: returned 
-000005c0: 2572 2069 6e73 7465 6164 206f 6620 4e6f  %r instead of No
-000005d0: 6e65 206f 7220 6120 7661 6c69 6420 6d65  ne or a valid me
-000005e0: 6d62 6572 270d 0a20 2020 2020 2020 2020  mber'..         
-000005f0: 2020 2020 2020 2025 2028 636c 732e 5f5f         % (cls.__
-00000600: 6e61 6d65 5f5f 2c20 7265 7375 6c74 290d  name__, result).
-00000610: 0a20 2020 2020 2020 2020 2020 2029 0d0a  .            )..
-00000620: 2020 2020 2020 2020 6578 632e 5f5f 636f          exc.__co
-00000630: 6e74 6578 745f 5f20 3d20 7665 5f65 7863  ntext__ = ve_exc
-00000640: 0d0a 2020 2020 2020 2020 7261 6973 6520  ..        raise 
-00000650: 6578 630d 0a0d 0a0d 0a45 6e75 6d2e 5f5f  exc......Enum.__
-00000660: 6e65 775f 5f20 3d20 5f6f 7269 675f 656e  new__ = _orig_en
-00000670: 756d 5f6e 6577 0d0a 5374 7241 7352 6570  um_new..StrAsRep
-00000680: 724d 6978 696e 456e 756d 2e5f 5f6e 6577  rMixinEnum.__new
-00000690: 5f5f 203d 205f 6f72 6967 5f65 6e75 6d5f  __ = _orig_enum_
-000006a0: 6e65 770d 0a4c 6f6f 6b55 704d 6978 696e  new..LookUpMixin
-000006b0: 456e 756d 2e5f 5f6e 6577 5f5f 203d 205f  Enum.__new__ = _
-000006c0: 6f72 6967 5f65 6e75 6d5f 6e65 770d 0a41  orig_enum_new..A
-000006d0: 7574 6f4e 616d 654d 6978 696e 456e 756d  utoNameMixinEnum
-000006e0: 2e5f 5f6e 6577 5f5f 203d 205f 6f72 6967  .__new__ = _orig
-000006f0: 5f65 6e75 6d5f 6e65 770d 0a4d 6973 7369  _enum_new..Missi
-00000700: 6e67 4e6f 6e65 4d69 7869 6e45 6e75 6d2e  ngNoneMixinEnum.
-00000710: 5f5f 6e65 775f 5f20 3d20 5f6f 7269 675f  __new__ = _orig_
-00000720: 656e 756d 5f6e 6577 0d0a 0d0a 0d0a 6c6f  enum_new......lo
-00000730: 6767 6572 203d 206c 6f67 6769 6e67 2e67  gger = logging.g
-00000740: 6574 4c6f 6767 6572 285f 5f6e 616d 655f  etLogger(__name_
-00000750: 5f29 0d0a 0d0a 230d 0a23 2040 7079 7465  _)....#..# @pyte
-00000760: 7374 2e66 6978 7475 7265 2829 0d0a 2320  st.fixture()..# 
-00000770: 6465 6620 6d79 5f64 6570 656e 6465 6e63  def my_dependenc
-00000780: 7928 293a 0d0a 2320 2020 2020 7265 7475  y():..#     retu
-00000790: 726e 2034 320d 0a23 0d0a 2320 2340 7079  rn 42..#..# #@py
-000007a0: 7465 7374 2e6d 6172 6b2e 7773 0d0a 2320  test.mark.ws..# 
-000007b0: 6465 6620 7465 7374 5f66 6972 7374 286d  def test_first(m
-000007c0: 795f 6465 7065 6e64 656e 6379 2029 3a0d  y_dependency ):.
-000007d0: 0a23 2020 2020 206c 6f67 6765 722e 696e  .#     logger.in
-000007e0: 666f 2827 5465 7374 696e 6720 6669 7273  fo('Testing firs
-000007f0: 7427 290d 0a23 0d0a 0d0a 0d0a 636c 6173  t')..#......clas
-00000800: 7320 5465 7374 5374 616e 6461 7264 456e  s TestStandardEn
-00000810: 756d 286f 626a 6563 7429 3a0d 0a20 2020  um(object):..   
-00000820: 2040 656e 756d 2e75 6e69 7175 650d 0a20   @enum.unique.. 
-00000830: 2020 2063 6c61 7373 2043 6f6c 6f72 3128     class Color1(
-00000840: 456e 756d 293a 0d0a 2020 2020 2020 2020  Enum):..        
-00000850: 5245 4420 3d20 3130 0d0a 2020 2020 2020  RED = 10..      
-00000860: 2020 424c 5545 203d 2032 300d 0a20 2020    BLUE = 20..   
-00000870: 2020 2020 2047 5245 454e 203d 2033 300d       GREEN = 30.
-00000880: 0a0d 0a20 2020 2040 656e 756d 2e75 6e69  ...    @enum.uni
-00000890: 7175 650d 0a20 2020 2063 6c61 7373 2043  que..    class C
-000008a0: 6f6c 6f72 3228 456e 756d 293a 0d0a 2020  olor2(Enum):..  
-000008b0: 2020 2020 2020 5245 4420 3d20 2772 270d        RED = 'r'.
-000008c0: 0a20 2020 2020 2020 2042 4c55 4520 3d20  .        BLUE = 
-000008d0: 2762 270d 0a20 2020 2020 2020 2047 5245  'b'..        GRE
-000008e0: 454e 203d 2027 6727 0d0a 0d0a 2020 2020  EN = 'g'....    
-000008f0: 4065 6e75 6d2e 756e 6971 7565 0d0a 2020  @enum.unique..  
-00000900: 2020 636c 6173 7320 436f 6c6f 7233 2845    class Color3(E
-00000910: 6e75 6d29 3a0d 0a20 2020 2020 2020 2052  num):..        R
-00000920: 4544 203d 2061 7574 6f28 290d 0a20 2020  ED = auto()..   
-00000930: 2020 2020 2042 4c55 4520 3d20 6175 746f       BLUE = auto
-00000940: 2829 0d0a 2020 2020 2020 2020 4752 4545  ()..        GREE
-00000950: 4e20 3d20 6175 746f 2829 0d0a 0d0a 0d0a  N = auto()......
-00000960: 2020 2020 4070 7974 6573 742e 6d61 726b      @pytest.mark
-00000970: 2e70 6172 616d 6574 7269 7a65 280d 0a20  .parametrize(.. 
-00000980: 2020 2020 2020 2027 636c 732c 6973 5f62         'cls,is_b
-00000990: 795f 6e61 6d65 2c76 616c 7565 272c 0d0a  y_name,value',..
-000009a0: 2020 2020 2020 2020 5b0d 0a20 2020 2020          [..     
-000009b0: 2020 2020 2020 2028 436f 6c6f 7231 2c20         (Color1, 
-000009c0: 5472 7565 2c20 3130 292c 0d0a 2020 2020  True, 10),..    
-000009d0: 2020 2020 2020 2020 2320 2843 6f6c 6f72          # (Color
-000009e0: 312c 2046 616c 7365 2c20 2752 4544 2729  1, False, 'RED')
-000009f0: 2c0d 0a20 2020 2020 2020 2020 2020 2023  ,..            #
-00000a00: 2028 436f 6c6f 7232 2c20 5472 7565 2c20   (Color2, True, 
-00000a10: 2762 2729 2c0d 0a20 2020 2020 2020 2020  'b'),..         
-00000a20: 2020 2023 2028 436f 6c6f 7232 2c20 4661     # (Color2, Fa
-00000a30: 6c73 652c 2027 424c 5545 2729 2c0d 0a20  lse, 'BLUE'),.. 
-00000a40: 2020 2020 2020 2020 2020 2023 2028 436f             # (Co
-00000a50: 6c6f 7233 2c20 5472 7565 2c20 3329 2c0d  lor3, True, 3),.
-00000a60: 0a20 2020 2020 2020 2020 2020 2023 2028  .            # (
-00000a70: 436f 6c6f 7233 2c20 4661 6c73 652c 2027  Color3, False, '
-00000a80: 4752 4545 4e27 292c 0d0a 2020 2020 2020  GREEN'),..      
-00000a90: 2020 5d0d 0a20 2020 2029 0d0a 2020 2020    ]..    )..    
-00000aa0: 6465 6620 7465 7374 5f62 7569 6c74 696e  def test_builtin
-00000ab0: 5f65 6e75 6d75 7261 7469 6f6e 2873 656c  _enumuration(sel
-00000ac0: 662c 2072 6571 7565 7374 2c20 636c 732c  f, request, cls,
-00000ad0: 2069 735f 6279 5f6e 616d 652c 2076 616c   is_by_name, val
-00000ae0: 7565 293a 0d0a 2020 2020 2020 2020 6c6f  ue):..        lo
-00000af0: 6767 6572 2e69 6e66 6f28 6627 7b72 6571  gger.info(f'{req
-00000b00: 7565 7374 2e5f 7079 6675 6e63 6974 656d  uest._pyfuncitem
-00000b10: 2e6e 616d 657d 2829 2729 0d0a 2020 2020  .name}()')..    
-00000b20: 2020 2020 736f 6d65 5f65 6e75 6d20 3d20      some_enum = 
-00000b30: 636c 7328 7661 6c75 6529 2069 6620 6973  cls(value) if is
-00000b40: 5f62 795f 6e61 6d65 2065 6c73 6520 636c  _by_name else cl
-00000b50: 735b 7661 6c75 655d 0d0a 2020 2020 2020  s[value]..      
-00000b60: 2020 6c6f 6767 6572 2e69 6e66 6f28 6627    logger.info(f'
-00000b70: 6e61 6d65 2069 7320 7b73 6f6d 655f 656e  name is {some_en
-00000b80: 756d 2172 7d27 290d 0a20 2020 2020 2020  um!r}')..       
-00000b90: 2073 6563 5f65 6e75 6d20 3d20 636c 735b   sec_enum = cls[
-00000ba0: 736f 6d65 5f65 6e75 6d2e 6e61 6d65 5d0d  some_enum.name].
-00000bb0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-00000bc0: 736f 6d65 5f65 6e75 6d20 3d3d 2073 6563  some_enum == sec
-00000bd0: 5f65 6e75 6d0d 0a0d 0a20 2020 2020 2020  _enum....       
-00000be0: 206c 6f67 6765 722e 6465 6275 6728 736f   logger.debug(so
-00000bf0: 6d65 5f65 6e75 6d29 0d0a 2020 2020 2020  me_enum)..      
-00000c00: 2020 6c6f 6767 6572 2e64 6562 7567 2866    logger.debug(f
-00000c10: 2772 6570 7220 6973 207b 736f 6d65 5f65  'repr is {some_e
-00000c20: 6e75 6d21 727d 2729 0d0a 2020 2020 2020  num!r}')..      
-00000c30: 2020 6c6f 6767 6572 2e64 6562 7567 2866    logger.debug(f
-00000c40: 2773 7472 2069 7320 7b73 6f6d 655f 656e  'str is {some_en
-00000c50: 756d 2173 7d27 290d 0a20 2020 2020 2020  um!s}')..       
-00000c60: 205b 6c6f 6767 6572 2e64 6562 7567 2866   [logger.debug(f
-00000c70: 277b 6d65 6d62 6572 2172 7d27 2920 666f  '{member!r}') fo
-00000c80: 7220 6d65 6d62 6572 2069 6e20 636c 732e  r member in cls.
-00000c90: 5f5f 6d65 6d62 6572 735f 5f2e 7661 6c75  __members__.valu
-00000ca0: 6573 2829 5d0d 0a0d 0a20 2020 2020 2020  es()]....       
-00000cb0: 2077 6974 6820 7079 7465 7374 2e72 6169   with pytest.rai
-00000cc0: 7365 7328 4b65 7945 7272 6f72 2920 6173  ses(KeyError) as
-00000cd0: 2065 7863 696e 666f 3a0d 0a20 2020 2020   excinfo:..     
-00000ce0: 2020 2020 2020 2063 6c73 5b27 6d69 7373         cls['miss
-00000cf0: 696e 675f 6b65 795f 6865 7265 5f69 745f  ing_key_here_it_
-00000d00: 6973 275d 0d0a 2020 2020 2020 2020 2020  is']..          
-00000d10: 2020 2320 6c6f 6767 6572 2e64 6562 7567    # logger.debug
-00000d20: 2865 7863 696e 666f 2e76 616c 7565 2c20  (excinfo.value, 
-00000d30: 6578 635f 696e 666f 3d28 6578 6369 6e66  exc_info=(excinf
-00000d40: 6f2e 7479 7065 2c20 6578 6369 6e66 6f2e  o.type, excinfo.
-00000d50: 7661 6c75 652c 2065 7863 696e 666f 2e74  value, excinfo.t
-00000d60: 6229 290d 0a0d 0a20 2020 2020 2020 2077  b))....        w
-00000d70: 6974 6820 7079 7465 7374 2e72 6169 7365  ith pytest.raise
-00000d80: 7328 5661 6c75 6545 7272 6f72 2920 6173  s(ValueError) as
-00000d90: 2065 7863 696e 666f 3a0d 0a20 2020 2020   excinfo:..     
-00000da0: 2020 2020 2020 2063 6c73 2827 6d69 7373         cls('miss
-00000db0: 696e 675f 7661 6c75 655f 6865 7265 5f69  ing_value_here_i
-00000dc0: 745f 6973 2729 0d0a 2020 2020 2020 2020  t_is')..        
-00000dd0: 2020 2020 2320 6c6f 6767 6572 2e64 6562      # logger.deb
-00000de0: 7567 2865 7863 696e 666f 2e76 616c 7565  ug(excinfo.value
-00000df0: 2c20 6578 635f 696e 666f 3d28 6578 6369  , exc_info=(exci
-00000e00: 6e66 6f2e 7479 7065 2c20 6578 6369 6e66  nfo.type, excinf
-00000e10: 6f2e 7661 6c75 652c 2065 7863 696e 666f  o.value, excinfo
-00000e20: 2e74 6229 290d 0a0d 0a0d 0a63 6c61 7373  .tb))......class
-00000e30: 2054 6573 7453 7472 4173 5265 7072 4d69   TestStrAsReprMi
-00000e40: 7869 6e45 6e75 6d28 6f62 6a65 6374 293a  xinEnum(object):
-00000e50: 0d0a 0d0a 2020 2020 4065 6e75 6d2e 756e  ....    @enum.un
-00000e60: 6971 7565 0d0a 2020 2020 636c 6173 7320  ique..    class 
-00000e70: 436f 6c6f 7253 7472 2853 7472 4173 5265  ColorStr(StrAsRe
-00000e80: 7072 4d69 7869 6e45 6e75 6d29 3a0d 0a20  prMixinEnum):.. 
-00000e90: 2020 2020 2020 2052 4544 203d 2061 7574         RED = aut
-00000ea0: 6f28 290d 0a20 2020 2020 2020 2042 4c55  o()..        BLU
-00000eb0: 4520 3d20 6175 746f 2829 0d0a 2020 2020  E = auto()..    
-00000ec0: 2020 2020 4752 4545 4e20 3d20 6175 746f      GREEN = auto
-00000ed0: 2829 0d0a 0d0a 2020 2020 4065 6e75 6d2e  ()....    @enum.
-00000ee0: 756e 6971 7565 0d0a 2020 2020 636c 6173  unique..    clas
-00000ef0: 7320 436f 6c6f 7253 7472 3228 5374 7241  s ColorStr2(StrA
-00000f00: 7352 6570 724d 6978 696e 456e 756d 2c20  sReprMixinEnum, 
-00000f10: 456e 756d 293a 0d0a 2020 2020 2020 2020  Enum):..        
-00000f20: 5245 4420 3d20 6175 746f 2829 0d0a 2020  RED = auto()..  
-00000f30: 2020 2020 2020 424c 5545 203d 2061 7574        BLUE = aut
-00000f40: 6f28 290d 0a20 2020 2020 2020 2047 5245  o()..        GRE
-00000f50: 454e 203d 2061 7574 6f28 290d 0a0d 0a0d  EN = auto().....
-00000f60: 0a0d 0a20 2020 2040 7079 7465 7374 2e6d  ...    @pytest.m
-00000f70: 6172 6b2e 7061 7261 6d65 7472 697a 6528  ark.parametrize(
-00000f80: 0d0a 2020 2020 2020 2020 2027 636c 7327  ..         'cls'
-00000f90: 2c0d 0a20 2020 2020 2020 205b 0d0a 2020  ,..        [..  
-00000fa0: 2020 2020 2020 2020 2020 436f 6c6f 7253            ColorS
-00000fb0: 7472 2c0d 0a20 2020 2020 2020 2020 2020  tr,..           
-00000fc0: 2043 6f6c 6f72 5374 7232 0d0a 2020 2020   ColorStr2..    
-00000fd0: 2020 2020 5d29 0d0a 2020 2020 6465 6620      ])..    def 
-00000fe0: 7465 7374 5f53 7472 4173 5265 7072 4d69  test_StrAsReprMi
-00000ff0: 7869 6e45 6e75 6d28 7365 6c66 2c20 7265  xinEnum(self, re
-00001000: 7175 6573 742c 2063 6c73 293a 0d0a 2020  quest, cls):..  
-00001010: 2020 2020 2020 6c6f 6767 6572 2e69 6e66        logger.inf
-00001020: 6f28 6627 7b72 6571 7565 7374 2e5f 7079  o(f'{request._py
-00001030: 6675 6e63 6974 656d 2e6e 616d 657d 2829  funcitem.name}()
-00001040: 2729 0d0a 2020 2020 2020 2020 736f 6d65  ')..        some
-00001050: 5f65 6e75 6d20 3d20 636c 7328 3129 0d0a  _enum = cls(1)..
-00001060: 2020 2020 2020 2020 6c6f 6767 6572 2e69          logger.i
-00001070: 6e66 6f28 6627 6e61 6d65 2069 7320 7b73  nfo(f'name is {s
-00001080: 6f6d 655f 656e 756d 2172 7d27 290d 0a20  ome_enum!r}').. 
-00001090: 2020 2020 2020 2073 6563 5f65 6e75 6d20         sec_enum 
-000010a0: 3d20 636c 735b 736f 6d65 5f65 6e75 6d2e  = cls[some_enum.
-000010b0: 6e61 6d65 5d0d 0a20 2020 2020 2020 2061  name]..        a
-000010c0: 7373 6572 7420 736f 6d65 5f65 6e75 6d3d  ssert some_enum=
-000010d0: 3d73 6563 5f65 6e75 6d0d 0a0d 0a20 2020  =sec_enum....   
-000010e0: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
-000010f0: 6728 736f 6d65 5f65 6e75 6d29 0d0a 2020  g(some_enum)..  
-00001100: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
-00001110: 7567 2866 2772 6570 7220 6973 207b 736f  ug(f'repr is {so
-00001120: 6d65 5f65 6e75 6d21 727d 2729 0d0a 2020  me_enum!r}')..  
-00001130: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
-00001140: 7567 2866 2773 7472 2069 7320 7b73 6f6d  ug(f'str is {som
-00001150: 655f 656e 756d 2173 7d27 290d 0a20 2020  e_enum!s}')..   
-00001160: 2020 2020 205b 6c6f 6767 6572 2e64 6562       [logger.deb
-00001170: 7567 2866 277b 6d65 6d62 6572 2172 7d27  ug(f'{member!r}'
-00001180: 2920 666f 7220 6d65 6d62 6572 2069 6e20  ) for member in 
-00001190: 636c 732e 5f5f 6d65 6d62 6572 735f 5f2e  cls.__members__.
-000011a0: 7661 6c75 6573 2829 5d0d 0a0d 0a20 2020  values()]....   
-000011b0: 2020 2020 2061 7373 6572 7420 7265 7072       assert repr
-000011c0: 2873 6f6d 655f 656e 756d 2920 3d3d 2073  (some_enum) == s
-000011d0: 7472 2873 6f6d 655f 656e 756d 290d 0a0d  tr(some_enum)...
-000011e0: 0a0d 0a63 6c61 7373 2054 6573 7441 7574  ...class TestAut
-000011f0: 6f4e 616d 654d 6978 696e 456e 756d 286f  oNameMixinEnum(o
-00001200: 626a 6563 7429 3a0d 0a20 2020 2040 656e  bject):..    @en
-00001210: 756d 2e75 6e69 7175 650d 0a20 2020 2063  um.unique..    c
-00001220: 6c61 7373 2043 6f6c 6f72 4175 746f 4e61  lass ColorAutoNa
-00001230: 6d65 2841 7574 6f4e 616d 654d 6978 696e  me(AutoNameMixin
-00001240: 456e 756d 293a 0d0a 2020 2020 2020 2020  Enum):..        
-00001250: 5245 4420 3d20 6175 746f 2829 0d0a 2020  RED = auto()..  
-00001260: 2020 2020 2020 424c 5545 203d 2061 7574        BLUE = aut
-00001270: 6f28 290d 0a20 2020 2020 2020 2047 5245  o()..        GRE
-00001280: 454e 203d 2061 7574 6f28 290d 0a0d 0a20  EN = auto().... 
-00001290: 2020 2040 656e 756d 2e75 6e69 7175 6520     @enum.unique 
-000012a0: 2341 7574 6f4e 616d 654d 6978 696e 456e  #AutoNameMixinEn
-000012b0: 756d 2068 6173 2074 6f20 6265 206c 6173  um has to be las
-000012c0: 7420 2873 6565 2045 6e75 6d4d 6574 612e  t (see EnumMeta.
-000012d0: 5f5f 7072 6570 6172 655f 5f28 2929 0d0a  __prepare__())..
-000012e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012f0: 2023 6d65 7468 6f64 205f 6765 6e65 7261   #method _genera
-00001300: 7465 5f6e 6578 745f 7661 6c75 655f 2829  te_next_value_()
-00001310: 2077 696c 6c20 6265 2074 616b 656e 2066   will be taken f
-00001320: 726f 6d20 7468 6569 7265 0d0a 2020 2020  rom theire..    
-00001330: 636c 6173 7320 436f 6c6f 7241 7574 6f4e  class ColorAutoN
-00001340: 616d 6532 2853 7472 4173 5265 7072 4d69  ame2(StrAsReprMi
-00001350: 7869 6e45 6e75 6d2c 2041 7574 6f4e 616d  xinEnum, AutoNam
-00001360: 654d 6978 696e 456e 756d 293a 0d0a 2020  eMixinEnum):..  
-00001370: 2020 2020 2020 5245 4420 3d20 6175 746f        RED = auto
-00001380: 2829 0d0a 2020 2020 2020 2020 424c 5545  ()..        BLUE
-00001390: 203d 2061 7574 6f28 290d 0a20 2020 2020   = auto()..     
-000013a0: 2020 2047 5245 454e 203d 2061 7574 6f28     GREEN = auto(
-000013b0: 290d 0a0d 0a20 2020 2040 656e 756d 2e75  )....    @enum.u
-000013c0: 6e69 7175 6520 2341 7574 6f4e 616d 654d  nique #AutoNameM
-000013d0: 6978 696e 456e 756d 2068 6173 2074 6f20  ixinEnum has to 
-000013e0: 6265 206c 6173 7420 2873 6565 2045 6e75  be last (see Enu
-000013f0: 6d4d 6574 612e 5f5f 7072 6570 6172 655f  mMeta.__prepare_
-00001400: 5f28 2929 0d0a 2020 2020 636c 6173 7320  _())..    class 
-00001410: 436f 6c6f 7241 7574 6f4e 616d 6557 726f  ColorAutoNameWro
-00001420: 6e67 2841 7574 6f4e 616d 654d 6978 696e  ng(AutoNameMixin
-00001430: 456e 756d 2c20 5374 7241 7352 6570 724d  Enum, StrAsReprM
-00001440: 6978 696e 456e 756d 293a 0d0a 2020 2020  ixinEnum):..    
-00001450: 2020 2020 5245 4420 3d20 6175 746f 2829      RED = auto()
-00001460: 0d0a 2020 2020 2020 2020 424c 5545 203d  ..        BLUE =
-00001470: 2061 7574 6f28 290d 0a20 2020 2020 2020   auto()..       
-00001480: 2047 5245 454e 203d 2061 7574 6f28 290d   GREEN = auto().
-00001490: 0a0d 0a20 2020 2040 656e 756d 2e75 6e69  ...    @enum.uni
-000014a0: 7175 6520 2341 7574 6f4e 616d 654d 6978  que #AutoNameMix
-000014b0: 696e 456e 756d 2068 6173 2074 6f20 6265  inEnum has to be
-000014c0: 206c 6173 7420 2873 6565 2045 6e75 6d4d   last (see EnumM
-000014d0: 6574 612e 5f5f 7072 6570 6172 655f 5f28  eta.__prepare__(
-000014e0: 2929 0d0a 2020 2020 636c 6173 7320 436f  ))..    class Co
-000014f0: 6c6f 7241 7574 6f4e 616d 6557 726f 6e67  lorAutoNameWrong
-00001500: 3228 4175 746f 4e61 6d65 4d69 7869 6e45  2(AutoNameMixinE
-00001510: 6e75 6d2c 2045 6e75 6d29 3a0d 0a20 2020  num, Enum):..   
-00001520: 2020 2020 2052 4544 203d 2061 7574 6f28       RED = auto(
-00001530: 290d 0a20 2020 2020 2020 2042 4c55 4520  )..        BLUE 
-00001540: 3d20 6175 746f 2829 0d0a 2020 2020 2020  = auto()..      
-00001550: 2020 4752 4545 4e20 3d20 6175 746f 2829    GREEN = auto()
-00001560: 0d0a 0d0a 0d0a 0d0a 0d0a 2020 2020 4070  ..........    @p
-00001570: 7974 6573 742e 6d61 726b 2e70 6172 616d  ytest.mark.param
-00001580: 6574 7269 7a65 280d 0a20 2020 2020 2020  etrize(..       
-00001590: 2020 2763 6c73 272c 0d0a 2020 2020 2020    'cls',..      
-000015a0: 2020 5b0d 0a20 2020 2020 2020 2020 2020    [..           
-000015b0: 2043 6f6c 6f72 4175 746f 4e61 6d65 2c0d   ColorAutoName,.
-000015c0: 0a20 2020 2020 2020 2020 2020 2043 6f6c  .            Col
-000015d0: 6f72 4175 746f 4e61 6d65 322c 0d0a 2020  orAutoName2,..  
-000015e0: 2020 2020 2020 5d29 0d0a 2020 2020 6465        ])..    de
-000015f0: 6620 7465 7374 5f41 7574 6f4e 616d 654d  f test_AutoNameM
-00001600: 6978 696e 456e 756d 2873 656c 662c 2072  ixinEnum(self, r
-00001610: 6571 7565 7374 2c20 636c 7329 3a0d 0a20  equest, cls):.. 
-00001620: 2020 2020 2020 206c 6f67 6765 722e 696e         logger.in
-00001630: 666f 2866 277b 7265 7175 6573 742e 5f70  fo(f'{request._p
-00001640: 7966 756e 6369 7465 6d2e 6e61 6d65 7d28  yfuncitem.name}(
-00001650: 2927 290d 0a20 2020 2020 2020 2073 6f6d  )')..        som
-00001660: 655f 656e 756d 203d 2063 6c73 2827 5245  e_enum = cls('RE
-00001670: 4427 290d 0a20 2020 2020 2020 206c 6f67  D')..        log
-00001680: 6765 722e 696e 666f 2866 276e 616d 6520  ger.info(f'name 
-00001690: 6973 207b 736f 6d65 5f65 6e75 6d21 727d  is {some_enum!r}
-000016a0: 2729 0d0a 2020 2020 2020 2020 7365 635f  ')..        sec_
-000016b0: 656e 756d 203d 2063 6c73 5b73 6f6d 655f  enum = cls[some_
-000016c0: 656e 756d 2e6e 616d 655d 0d0a 2020 2020  enum.name]..    
-000016d0: 2020 2020 6173 7365 7274 2073 6f6d 655f      assert some_
-000016e0: 656e 756d 3d3d 7365 635f 656e 756d 0d0a  enum==sec_enum..
-000016f0: 0d0a 2020 2020 4070 7974 6573 742e 6d61  ..    @pytest.ma
-00001700: 726b 2e70 6172 616d 6574 7269 7a65 280d  rk.parametrize(.
-00001710: 0a20 2020 2020 2020 2020 2763 6c73 2c69  .         'cls,i
-00001720: 735f 7265 705f 6368 6563 6b27 2c0d 0a20  s_rep_check',.. 
-00001730: 2020 2020 2020 205b 0d0a 2020 2020 2020         [..      
-00001740: 2020 2020 2020 2843 6f6c 6f72 4175 746f        (ColorAuto
-00001750: 4e61 6d65 5772 6f6e 672c 2054 7275 6529  NameWrong, True)
-00001760: 2c0d 0a20 2020 2020 2020 2020 2020 2028  ,..            (
-00001770: 436f 6c6f 7241 7574 6f4e 616d 6557 726f  ColorAutoNameWro
-00001780: 6e67 322c 2046 616c 7365 292c 0d0a 2020  ng2, False),..  
-00001790: 2020 2020 2020 5d29 0d0a 0d0a 2020 2020        ])....    
-000017a0: 6465 6620 7465 7374 5f41 7574 6f4e 616d  def test_AutoNam
-000017b0: 6557 726f 6e67 4d69 7869 6e45 6e75 6d28  eWrongMixinEnum(
-000017c0: 7365 6c66 2c20 7265 7175 6573 742c 2063  self, request, c
-000017d0: 6c73 2c20 6973 5f72 6570 5f63 6865 636b  ls, is_rep_check
-000017e0: 293a 0d0a 2020 2020 2020 2020 6c6f 6767  ):..        logg
-000017f0: 6572 2e69 6e66 6f28 6627 7b72 6571 7565  er.info(f'{reque
-00001800: 7374 2e5f 7079 6675 6e63 6974 656d 2e6e  st._pyfuncitem.n
-00001810: 616d 657d 2829 2729 0d0a 0d0a 2020 2020  ame}()')....    
-00001820: 2020 2020 7769 7468 2070 7974 6573 742e      with pytest.
-00001830: 7261 6973 6573 2856 616c 7565 4572 726f  raises(ValueErro
-00001840: 7229 2061 7320 6578 6369 6e66 6f3a 0d0a  r) as excinfo:..
-00001850: 2020 2020 2020 2020 2020 2020 736f 6d65              some
-00001860: 5f65 6e75 6d20 3d20 636c 7328 2752 4544  _enum = cls('RED
-00001870: 2729 0d0a 2020 2020 2020 2020 2020 2020  ')..            
-00001880: 6c6f 6767 6572 2e64 6562 7567 2865 7863  logger.debug(exc
-00001890: 696e 666f 2e76 616c 7565 2c20 6578 635f  info.value, exc_
-000018a0: 696e 666f 3d28 6578 6369 6e66 6f2e 7479  info=(excinfo.ty
-000018b0: 7065 2c20 6578 6369 6e66 6f2e 7661 6c75  pe, excinfo.valu
-000018c0: 652c 2065 7863 696e 666f 2e74 6229 290d  e, excinfo.tb)).
-000018d0: 0a0d 0a20 2020 2020 2020 2073 6f6d 655f  ...        some_
-000018e0: 656e 756d 203d 2063 6c73 2831 290d 0a20  enum = cls(1).. 
-000018f0: 2020 2020 2020 206c 6f67 6765 722e 696e         logger.in
-00001900: 666f 2866 276e 616d 6520 6973 207b 736f  fo(f'name is {so
-00001910: 6d65 5f65 6e75 6d21 727d 2729 0d0a 2020  me_enum!r}')..  
-00001920: 2020 2020 2020 7365 635f 656e 756d 203d        sec_enum =
-00001930: 2063 6c73 5b73 6f6d 655f 656e 756d 2e6e   cls[some_enum.n
-00001940: 616d 655d 0d0a 2020 2020 2020 2020 6173  ame]..        as
-00001950: 7365 7274 2073 6f6d 655f 656e 756d 3d3d  sert some_enum==
-00001960: 7365 635f 656e 756d 0d0a 0d0a 2020 2020  sec_enum....    
-00001970: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
-00001980: 2873 6f6d 655f 656e 756d 290d 0a20 2020  (some_enum)..   
-00001990: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
-000019a0: 6728 6627 7265 7072 2069 7320 7b73 6f6d  g(f'repr is {som
-000019b0: 655f 656e 756d 2172 7d27 290d 0a20 2020  e_enum!r}')..   
-000019c0: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
-000019d0: 6728 6627 7374 7220 6973 207b 736f 6d65  g(f'str is {some
-000019e0: 5f65 6e75 6d21 737d 2729 0d0a 2020 2020  _enum!s}')..    
-000019f0: 2020 2020 5b6c 6f67 6765 722e 6465 6275      [logger.debu
-00001a00: 6728 6627 7b6d 656d 6265 7221 727d 2729  g(f'{member!r}')
-00001a10: 2066 6f72 206d 656d 6265 7220 696e 2063   for member in c
-00001a20: 6c73 2e5f 5f6d 656d 6265 7273 5f5f 2e76  ls.__members__.v
-00001a30: 616c 7565 7328 295d 0d0a 0d0a 2020 2020  alues()]....    
-00001a40: 2020 2020 6966 2069 735f 7265 705f 6368      if is_rep_ch
-00001a50: 6563 6b3a 0d0a 2020 2020 2020 2020 2020  eck:..          
-00001a60: 2020 6173 7365 7274 2072 6570 7228 736f    assert repr(so
-00001a70: 6d65 5f65 6e75 6d29 203d 3d20 7374 7228  me_enum) == str(
-00001a80: 736f 6d65 5f65 6e75 6d29 0d0a 0d0a 0d0a  some_enum)......
-00001a90: 636c 6173 7320 5465 7374 4d69 7373 696e  class TestMissin
-00001aa0: 674e 6f6e 654d 6978 696e 456e 756d 286f  gNoneMixinEnum(o
-00001ab0: 626a 6563 7429 3a0d 0a0d 0a20 2020 2040  bject):....    @
-00001ac0: 656e 756d 2e75 6e69 7175 650d 0a20 2020  enum.unique..   
-00001ad0: 2063 6c61 7373 2043 6f6c 6f72 4d69 7373   class ColorMiss
-00001ae0: 696e 674e 6f6e 6528 4d69 7373 696e 674e  ingNone(MissingN
-00001af0: 6f6e 654d 6978 696e 456e 756d 293a 0d0a  oneMixinEnum):..
-00001b00: 2020 2020 2020 2020 5245 4420 3d20 6175          RED = au
-00001b10: 746f 2829 0d0a 2020 2020 2020 2020 424c  to()..        BL
-00001b20: 5545 203d 2061 7574 6f28 290d 0a20 2020  UE = auto()..   
-00001b30: 2020 2020 2047 5245 454e 203d 2061 7574       GREEN = aut
-00001b40: 6f28 290d 0a0d 0a0d 0a20 2020 2064 6566  o()......    def
-00001b50: 2074 6573 745f 4d69 7373 696e 674e 6f6e   test_MissingNon
-00001b60: 6545 6e75 6d28 7365 6c66 2c20 7265 7175  eEnum(self, requ
-00001b70: 6573 7429 3a0d 0a20 2020 2020 2020 206c  est):..        l
-00001b80: 6f67 6765 722e 696e 666f 2866 277b 7265  ogger.info(f'{re
-00001b90: 7175 6573 742e 5f70 7966 756e 6369 7465  quest._pyfuncite
-00001ba0: 6d2e 6e61 6d65 7d28 2927 290d 0a0d 0a20  m.name}()').... 
-00001bb0: 2020 2020 2020 2073 6f6d 655f 656e 756d         some_enum
-00001bc0: 203d 2054 6573 744d 6973 7369 6e67 4e6f   = TestMissingNo
-00001bd0: 6e65 4d69 7869 6e45 6e75 6d2e 436f 6c6f  neMixinEnum.Colo
-00001be0: 724d 6973 7369 6e67 4e6f 6e65 2831 290d  rMissingNone(1).
-00001bf0: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
-00001c00: 696e 666f 2866 276e 616d 6520 6973 207b  info(f'name is {
-00001c10: 736f 6d65 5f65 6e75 6d21 727d 2729 0d0a  some_enum!r}')..
-00001c20: 2020 2020 2020 2020 7365 635f 656e 756d          sec_enum
-00001c30: 203d 2054 6573 744d 6973 7369 6e67 4e6f   = TestMissingNo
-00001c40: 6e65 4d69 7869 6e45 6e75 6d2e 436f 6c6f  neMixinEnum.Colo
-00001c50: 724d 6973 7369 6e67 4e6f 6e65 5b73 6f6d  rMissingNone[som
-00001c60: 655f 656e 756d 2e6e 616d 655d 0d0a 2020  e_enum.name]..  
-00001c70: 2020 2020 2020 6173 7365 7274 2073 6f6d        assert som
-00001c80: 655f 656e 756d 3d3d 7365 635f 656e 756d  e_enum==sec_enum
-00001c90: 0d0a 0d0a 2020 2020 2020 2020 7769 7468  ....        with
-00001ca0: 2070 7974 6573 742e 7261 6973 6573 284b   pytest.raises(K
-00001cb0: 6579 4572 726f 7229 2061 7320 6578 6369  eyError) as exci
-00001cc0: 6e66 6f3a 0d0a 2020 2020 2020 2020 2020  nfo:..          
-00001cd0: 2020 5465 7374 4d69 7373 696e 674e 6f6e    TestMissingNon
-00001ce0: 654d 6978 696e 456e 756d 2e43 6f6c 6f72  eMixinEnum.Color
-00001cf0: 4d69 7373 696e 674e 6f6e 655b 3130 5f30  MissingNone[10_0
-00001d00: 3030 5d0d 0a20 2020 2020 2020 2020 2020  00]..           
-00001d10: 2023 6c6f 6767 6572 2e64 6562 7567 2865   #logger.debug(e
-00001d20: 7863 696e 666f 2e76 616c 7565 2c20 6578  xcinfo.value, ex
-00001d30: 635f 696e 666f 3d28 6578 6369 6e66 6f2e  c_info=(excinfo.
-00001d40: 7479 7065 2c20 6578 6369 6e66 6f2e 7661  type, excinfo.va
-00001d50: 6c75 652c 2065 7863 696e 666f 2e74 6229  lue, excinfo.tb)
-00001d60: 290d 0a0d 0a20 2020 2020 2020 2077 6974  )....        wit
-00001d70: 6820 7079 7465 7374 2e72 6169 7365 7328  h pytest.raises(
-00001d80: 5661 6c75 6545 7272 6f72 2920 6173 2065  ValueError) as e
-00001d90: 7863 696e 666f 3a0d 0a20 2020 2020 2020  xcinfo:..       
-00001da0: 2020 2020 2054 6573 744d 6973 7369 6e67       TestMissing
-00001db0: 4e6f 6e65 4d69 7869 6e45 6e75 6d2e 436f  NoneMixinEnum.Co
-00001dc0: 6c6f 724d 6973 7369 6e67 4e6f 6e65 2831  lorMissingNone(1
-00001dd0: 305f 3030 3029 0d0a 0d0a 0d0a 0d0a 636c  0_000)........cl
-00001de0: 6173 7320 5465 7374 4c6f 6f6b 5570 4d69  ass TestLookUpMi
-00001df0: 7869 6e45 6e75 6d28 6f62 6a65 6374 293a  xinEnum(object):
-00001e00: 0d0a 0d0a 2020 2020 4065 6e75 6d2e 756e  ....    @enum.un
-00001e10: 6971 7565 0d0a 2020 2020 636c 6173 7320  ique..    class 
-00001e20: 436f 6c6f 724c 6f6f 6b55 7028 4c6f 6f6b  ColorLookUp(Look
-00001e30: 5570 4d69 7869 6e45 6e75 6d29 3a0d 0a20  UpMixinEnum):.. 
-00001e40: 2020 2020 2020 2052 4544 203d 2027 7227         RED = 'r'
-00001e50: 0d0a 2020 2020 2020 2020 424c 5545 203d  ..        BLUE =
-00001e60: 2027 6227 0d0a 2020 2020 2020 2020 4752   'b'..        GR
-00001e70: 4545 4e20 3d20 2767 270d 0a0d 0a20 2020  EEN = 'g'....   
-00001e80: 2040 656e 756d 2e75 6e69 7175 650d 0a20   @enum.unique.. 
-00001e90: 2020 2063 6c61 7373 2043 6f6c 6f72 4c6f     class ColorLo
-00001ea0: 6f6b 5570 4175 746f 284c 6f6f 6b55 704d  okUpAuto(LookUpM
-00001eb0: 6978 696e 456e 756d 2c20 4175 746f 4e61  ixinEnum, AutoNa
-00001ec0: 6d65 4d69 7869 6e45 6e75 6d29 3a0d 0a20  meMixinEnum):.. 
-00001ed0: 2020 2020 2020 2052 4544 203d 2061 7574         RED = aut
-00001ee0: 6f28 290d 0a20 2020 2020 2020 2042 4c55  o()..        BLU
-00001ef0: 4520 3d20 6175 746f 2829 0d0a 2020 2020  E = auto()..    
-00001f00: 2020 2020 4752 4545 4e20 3d20 6175 746f      GREEN = auto
-00001f10: 2829 0d0a 0d0a 0d0a 0d0a 2020 2020 6465  ()........    de
-00001f20: 6620 7465 7374 5f43 6f6c 6f72 4c6f 6f6b  f test_ColorLook
-00001f30: 5570 2873 656c 662c 2072 6571 7565 7374  Up(self, request
-00001f40: 293a 0d0a 2020 2020 2020 2020 6c6f 6767  ):..        logg
-00001f50: 6572 2e69 6e66 6f28 6627 7b72 6571 7565  er.info(f'{reque
-00001f60: 7374 2e5f 7079 6675 6e63 6974 656d 2e6e  st._pyfuncitem.n
-00001f70: 616d 657d 2829 2729 0d0a 0d0a 2020 2020  ame}()')....    
-00001f80: 2020 2020 736f 6d65 5f65 6e75 6d20 3d20      some_enum = 
-00001f90: 5465 7374 4c6f 6f6b 5570 4d69 7869 6e45  TestLookUpMixinE
-00001fa0: 6e75 6d2e 436f 6c6f 724c 6f6f 6b55 7028  num.ColorLookUp(
-00001fb0: 2772 2729 0d0a 2020 2020 2020 2020 6c6f  'r')..        lo
-00001fc0: 6767 6572 2e69 6e66 6f28 6627 6e61 6d65  gger.info(f'name
-00001fd0: 2069 7320 7b73 6f6d 655f 656e 756d 2172   is {some_enum!r
-00001fe0: 7d27 290d 0a20 2020 2020 2020 2073 6563  }')..        sec
-00001ff0: 5f65 6e75 6d20 3d20 5465 7374 4c6f 6f6b  _enum = TestLook
-00002000: 5570 4d69 7869 6e45 6e75 6d2e 436f 6c6f  UpMixinEnum.Colo
-00002010: 724c 6f6f 6b55 705b 736f 6d65 5f65 6e75  rLookUp[some_enu
-00002020: 6d2e 6e61 6d65 5d0d 0a20 2020 2020 2020  m.name]..       
-00002030: 2061 7373 6572 7420 736f 6d65 5f65 6e75   assert some_enu
-00002040: 6d20 3d3d 2073 6563 5f65 6e75 6d0d 0a0d  m == sec_enum...
-00002050: 0a20 2020 2020 2020 2077 6974 6820 7079  .        with py
-00002060: 7465 7374 2e72 6169 7365 7328 4b65 7945  test.raises(KeyE
-00002070: 7272 6f72 2920 6173 2065 7863 696e 666f  rror) as excinfo
-00002080: 3a0d 0a20 2020 2020 2020 2020 2020 2054  :..            T
-00002090: 6573 744c 6f6f 6b55 704d 6978 696e 456e  estLookUpMixinEn
-000020a0: 756d 2e43 6f6c 6f72 4c6f 6f6b 5570 5b27  um.ColorLookUp['
-000020b0: 6d69 7373 696e 675f 7661 6c75 655f 6865  missing_value_he
-000020c0: 7265 5f69 745f 6973 275d 0d0a 2020 2020  re_it_is']..    
-000020d0: 2020 2020 2020 2020 2320 6c6f 6767 6572          # logger
-000020e0: 2e64 6562 7567 2865 7863 696e 666f 2e76  .debug(excinfo.v
-000020f0: 616c 7565 2c20 6578 635f 696e 666f 3d28  alue, exc_info=(
-00002100: 6578 6369 6e66 6f2e 7479 7065 2c20 6578  excinfo.type, ex
-00002110: 6369 6e66 6f2e 7661 6c75 652c 2065 7863  cinfo.value, exc
-00002120: 696e 666f 2e74 6229 290d 0a20 2020 2020  info.tb))..     
-00002130: 2020 2077 6974 6820 7079 7465 7374 2e72     with pytest.r
-00002140: 6169 7365 7328 5661 6c75 6545 7272 6f72  aises(ValueError
-00002150: 2920 6173 2065 7863 696e 666f 3a0d 0a20  ) as excinfo:.. 
-00002160: 2020 2020 2020 2020 2020 2054 6573 744c             TestL
-00002170: 6f6f 6b55 704d 6978 696e 456e 756d 2e43  ookUpMixinEnum.C
-00002180: 6f6c 6f72 4c6f 6f6b 5570 2827 6d69 7373  olorLookUp('miss
-00002190: 696e 675f 7661 6c75 655f 6865 7265 5f69  ing_value_here_i
-000021a0: 745f 6973 2729 0d0a 0d0a 0d0a 2020 2020  t_is')......    
-000021b0: 6465 6620 7465 7374 5f43 6f6c 6f72 4c6f  def test_ColorLo
-000021c0: 6f6b 5570 4175 746f 2873 656c 662c 2072  okUpAuto(self, r
-000021d0: 6571 7565 7374 293a 0d0a 2020 2020 2020  equest):..      
-000021e0: 2020 6c6f 6767 6572 2e69 6e66 6f28 6627    logger.info(f'
-000021f0: 7b72 6571 7565 7374 2e5f 7079 6675 6e63  {request._pyfunc
-00002200: 6974 656d 2e6e 616d 657d 2829 2729 0d0a  item.name}()')..
-00002210: 0d0a 2020 2020 2020 2020 736f 6d65 5f65  ..        some_e
-00002220: 6e75 6d20 3d20 5465 7374 4c6f 6f6b 5570  num = TestLookUp
-00002230: 4d69 7869 6e45 6e75 6d2e 436f 6c6f 724c  MixinEnum.ColorL
-00002240: 6f6f 6b55 7041 7574 6f28 2752 4544 2729  ookUpAuto('RED')
-00002250: 0d0a 2020 2020 2020 2020 6c6f 6767 6572  ..        logger
-00002260: 2e69 6e66 6f28 6627 6e61 6d65 2069 7320  .info(f'name is 
-00002270: 7b73 6f6d 655f 656e 756d 2172 7d27 290d  {some_enum!r}').
-00002280: 0a20 2020 2020 2020 2073 6563 5f65 6e75  .        sec_enu
-00002290: 6d20 3d20 5465 7374 4c6f 6f6b 5570 4d69  m = TestLookUpMi
-000022a0: 7869 6e45 6e75 6d2e 436f 6c6f 724c 6f6f  xinEnum.ColorLoo
-000022b0: 6b55 7041 7574 6f5b 736f 6d65 5f65 6e75  kUpAuto[some_enu
-000022c0: 6d2e 6e61 6d65 5d0d 0a20 2020 2020 2020  m.name]..       
-000022d0: 2061 7373 6572 7420 736f 6d65 5f65 6e75   assert some_enu
-000022e0: 6d20 3d3d 2073 6563 5f65 6e75 6d0d 0a0d  m == sec_enum...
-000022f0: 0a20 2020 2020 2020 2077 6974 6820 7079  .        with py
-00002300: 7465 7374 2e72 6169 7365 7328 4b65 7945  test.raises(KeyE
-00002310: 7272 6f72 2920 6173 2065 7863 696e 666f  rror) as excinfo
-00002320: 3a0d 0a20 2020 2020 2020 2020 2020 2054  :..            T
-00002330: 6573 744c 6f6f 6b55 704d 6978 696e 456e  estLookUpMixinEn
-00002340: 756d 2e43 6f6c 6f72 4c6f 6f6b 5570 4175  um.ColorLookUpAu
-00002350: 746f 5b27 6d69 7373 696e 675f 7661 6c75  to['missing_valu
-00002360: 655f 6865 7265 5f69 745f 6973 275d 0d0a  e_here_it_is']..
-00002370: 2020 2020 2020 2020 2020 2020 2320 6c6f              # lo
-00002380: 6767 6572 2e64 6562 7567 2865 7863 696e  gger.debug(excin
-00002390: 666f 2e76 616c 7565 2c20 6578 635f 696e  fo.value, exc_in
-000023a0: 666f 3d28 6578 6369 6e66 6f2e 7479 7065  fo=(excinfo.type
-000023b0: 2c20 6578 6369 6e66 6f2e 7661 6c75 652c  , excinfo.value,
-000023c0: 2065 7863 696e 666f 2e74 6229 290d 0a20   excinfo.tb)).. 
-000023d0: 2020 2020 2020 2077 6974 6820 7079 7465         with pyte
-000023e0: 7374 2e72 6169 7365 7328 5661 6c75 6545  st.raises(ValueE
-000023f0: 7272 6f72 2920 6173 2065 7863 696e 666f  rror) as excinfo
-00002400: 3a0d 0a20 2020 2020 2020 2020 2020 2054  :..            T
-00002410: 6573 744c 6f6f 6b55 704d 6978 696e 456e  estLookUpMixinEn
-00002420: 756d 2e43 6f6c 6f72 4c6f 6f6b 5570 4175  um.ColorLookUpAu
-00002430: 746f 2827 6d69 7373 696e 675f 7661 6c75  to('missing_valu
-00002440: 655f 6865 7265 5f69 745f 6973 2729 0d0a  e_here_it_is')..
-00002450: 0d0a 0d0a 0d0a 636c 6173 7320 5465 7374  ......class Test
-00002460: 4c6f 6f6b 5570 4175 746f 4e61 6d65 4d69  LookUpAutoNameMi
-00002470: 7869 6e45 6e75 6d28 6f62 6a65 6374 293a  xinEnum(object):
-00002480: 0d0a 0d0a 2020 2020 6465 6620 6164 6443  ....    def addC
-00002490: 6f6d 7028 656e 756d 6572 6174 696f 6e29  omp(enumeration)
-000024a0: 3a0d 0a20 2020 2020 2020 2022 2222 436c  :..        """Cl
-000024b0: 6173 7320 6465 636f 7261 746f 7220 666f  ass decorator fo
-000024c0: 7220 656e 756d 6572 6174 696f 6e73 2022  r enumerations "
-000024d0: 2222 0d0a 2020 2020 2020 2020 616c 6c20  ""..        all 
-000024e0: 3d20 5b5d 0d0a 2020 2020 2020 2020 666f  = []..        fo
-000024f0: 7220 6d65 6d62 6572 2069 6e20 656e 756d  r member in enum
-00002500: 6572 6174 696f 6e2e 5f5f 6d65 6d62 6572  eration.__member
-00002510: 735f 5f2e 7661 6c75 6573 2829 3a0d 0a20  s__.values():.. 
-00002520: 2020 2020 2020 2020 2020 2061 6c6c 2e61             all.a
-00002530: 7070 656e 6428 6d65 6d62 6572 2e76 616c  ppend(member.val
-00002540: 7565 290d 0a0d 0a20 2020 2020 2020 2065  ue)....        e
-00002550: 6e75 6d65 7261 7469 6f6e 2e63 6f6d 7020  numeration.comp 
-00002560: 3d20 616c 6c0d 0a20 2020 2020 2020 2072  = all..        r
-00002570: 6574 7572 6e20 656e 756d 6572 6174 696f  eturn enumeratio
-00002580: 6e0d 0a0d 0a20 2020 2040 656e 756d 2e75  n....    @enum.u
-00002590: 6e69 7175 650d 0a20 2020 2040 6164 6443  nique..    @addC
-000025a0: 6f6d 700d 0a20 2020 2063 6c61 7373 2043  omp..    class C
-000025b0: 6f6c 6f72 284c 6f6f 6b55 704d 6978 696e  olor(LookUpMixin
-000025c0: 456e 756d 2c20 4175 746f 4e61 6d65 4d69  Enum, AutoNameMi
-000025d0: 7869 6e45 6e75 6d29 3a0d 0a20 2020 2020  xinEnum):..     
-000025e0: 2020 2052 4544 203d 2027 5227 0d0a 2020     RED = 'R'..  
-000025f0: 2020 2020 2020 424c 5545 203d 2027 4227        BLUE = 'B'
-00002600: 0d0a 2020 2020 2020 2020 4752 4545 4e20  ..        GREEN 
-00002610: 3d20 2247 220d 0a0d 0a20 2020 2064 6566  = "G"....    def
-00002620: 2074 6573 745f 436f 6c6f 7228 7365 6c66   test_Color(self
-00002630: 2c20 7265 7175 6573 7429 3a0d 0a20 2020  , request):..   
-00002640: 2020 2020 206c 6f67 6765 722e 696e 666f       logger.info
-00002650: 2866 277b 7265 7175 6573 742e 5f70 7966  (f'{request._pyf
-00002660: 756e 6369 7465 6d2e 6e61 6d65 7d28 2927  uncitem.name}()'
-00002670: 290d 0a0d 0a20 2020 2020 2020 2073 6f6d  )....        som
-00002680: 655f 656e 756d 203d 2054 6573 744c 6f6f  e_enum = TestLoo
-00002690: 6b55 7041 7574 6f4e 616d 654d 6978 696e  kUpAutoNameMixin
-000026a0: 456e 756d 2e43 6f6c 6f72 2827 5227 290d  Enum.Color('R').
-000026b0: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
-000026c0: 696e 666f 2866 276e 616d 6520 6973 207b  info(f'name is {
-000026d0: 736f 6d65 5f65 6e75 6d21 727d 2729 0d0a  some_enum!r}')..
-000026e0: 2020 2020 2020 2020 7365 635f 656e 756d          sec_enum
-000026f0: 203d 2054 6573 744c 6f6f 6b55 7041 7574   = TestLookUpAut
-00002700: 6f4e 616d 654d 6978 696e 456e 756d 2e43  oNameMixinEnum.C
-00002710: 6f6c 6f72 5b73 6f6d 655f 656e 756d 2e6e  olor[some_enum.n
-00002720: 616d 655d 0d0a 2020 2020 2020 2020 6173  ame]..        as
-00002730: 7365 7274 2073 6f6d 655f 656e 756d 203d  sert some_enum =
-00002740: 3d20 7365 635f 656e 756d 0d0a 0d0a 2020  = sec_enum....  
-00002750: 2020 2020 2020 7769 7468 2070 7974 6573        with pytes
-00002760: 742e 7261 6973 6573 284b 6579 4572 726f  t.raises(KeyErro
-00002770: 7229 2061 7320 6578 6369 6e66 6f3a 0d0a  r) as excinfo:..
-00002780: 2020 2020 2020 2020 2020 2020 5465 7374              Test
-00002790: 4c6f 6f6b 5570 4175 746f 4e61 6d65 4d69  LookUpAutoNameMi
-000027a0: 7869 6e45 6e75 6d2e 436f 6c6f 725b 276d  xinEnum.Color['m
-000027b0: 6973 7369 6e67 5f76 616c 7565 5f68 6572  issing_value_her
-000027c0: 655f 6974 5f69 7327 5d0d 0a20 2020 2020  e_it_is']..     
-000027d0: 2020 2020 2020 2023 206c 6f67 6765 722e         # logger.
-000027e0: 6465 6275 6728 6578 6369 6e66 6f2e 7661  debug(excinfo.va
-000027f0: 6c75 652c 2065 7863 5f69 6e66 6f3d 2865  lue, exc_info=(e
-00002800: 7863 696e 666f 2e74 7970 652c 2065 7863  xcinfo.type, exc
-00002810: 696e 666f 2e76 616c 7565 2c20 6578 6369  info.value, exci
-00002820: 6e66 6f2e 7462 2929 0d0a 2020 2020 2020  nfo.tb))..      
-00002830: 2020 7769 7468 2070 7974 6573 742e 7261    with pytest.ra
-00002840: 6973 6573 2856 616c 7565 4572 726f 7229  ises(ValueError)
-00002850: 2061 7320 6578 6369 6e66 6f3a 0d0a 2020   as excinfo:..  
-00002860: 2020 2020 2020 2020 2020 2054 6573 744c             TestL
-00002870: 6f6f 6b55 7041 7574 6f4e 616d 654d 6978  ookUpAutoNameMix
-00002880: 696e 456e 756d 2e43 6f6c 6f72 2827 6d69  inEnum.Color('mi
-00002890: 7373 696e 675f 7661 6c75 655f 6865 7265  ssing_value_here
-000028a0: 5f69 745f 6973 2729 0d0a 0d0a 2020 2020  _it_is')....    
-000028b0: 2020 2020 7661 6c75 6520 3d20 5465 7374      value = Test
-000028c0: 4c6f 6f6b 5570 4175 746f 4e61 6d65 4d69  LookUpAutoNameMi
-000028d0: 7869 6e45 6e75 6d2e 436f 6c6f 722e 636f  xinEnum.Color.co
-000028e0: 6d70 0d0a 2020 2020 2020 2020 6173 7365  mp..        asse
-000028f0: 7274 2076 616c 7565 2069 7320 6e6f 7420  rt value is not 
-00002900: 4e6f 6e65 0d0a 0d0a 0d0a 0d0a 6966 205f  None........if _
-00002910: 5f6e 616d 655f 5f20 3d3d 2022 5f5f 6d61  _name__ == "__ma
-00002920: 696e 5f5f 223a 0d0a 2020 2020 7079 7465  in__":..    pyte
-00002930: 7374 2e6d 6169 6e28 5b5f 5f66 696c 655f  st.main([__file_
-00002940: 5f5d 290d 0a0d 0a                        _])....
+00000000: 0a69 6d70 6f72 7420 6c6f 6767 696e 670a  .import logging.
+00000010: 696d 706f 7274 2070 7974 6573 740a 0a66  import pytest..f
+00000020: 726f 6d20 616c 6578 6265 722e 7574 696c  rom alexber.util
+00000030: 7320 696d 706f 7274 2053 7472 4173 5265  s import StrAsRe
+00000040: 7072 4d69 7869 6e45 6e75 6d2c 204c 6f6f  prMixinEnum, Loo
+00000050: 6b55 704d 6978 696e 456e 756d 2c20 4175  kUpMixinEnum, Au
+00000060: 746f 4e61 6d65 4d69 7869 6e45 6e75 6d2c  toNameMixinEnum,
+00000070: 204d 6973 7369 6e67 4e6f 6e65 4d69 7869   MissingNoneMixi
+00000080: 6e45 6e75 6d2c 2045 6e75 6d0a 6672 6f6d  nEnum, Enum.from
+00000090: 2061 6c65 7862 6572 2e75 7469 6c73 2e65   alexber.utils.e
+000000a0: 6e75 6d73 2069 6d70 6f72 7420 656e 756d  nums import enum
+000000b0: 2c20 6175 746f 0a0a 2320 2375 7365 2073  , auto..# #use s
+000000c0: 7461 6e64 6172 6420 456e 756d 2e5f 5f6e  tandard Enum.__n
+000000d0: 6577 5f5f 0a64 6566 205f 6f72 6967 5f65  ew__.def _orig_e
+000000e0: 6e75 6d5f 6e65 7728 636c 732c 2076 616c  num_new(cls, val
+000000f0: 7565 293a 0a20 2020 2023 2061 6c6c 2065  ue):.    # all e
+00000100: 6e75 6d20 696e 7374 616e 6365 7320 6172  num instances ar
+00000110: 6520 6163 7475 616c 6c79 2063 7265 6174  e actually creat
+00000120: 6564 2064 7572 696e 6720 636c 6173 7320  ed during class 
+00000130: 636f 6e73 7472 7563 7469 6f6e 0a20 2020  construction.   
+00000140: 2023 2077 6974 686f 7574 2063 616c 6c69   # without calli
+00000150: 6e67 2074 6869 7320 6d65 7468 6f64 3b20  ng this method; 
+00000160: 7468 6973 206d 6574 686f 6420 6973 2063  this method is c
+00000170: 616c 6c65 6420 6279 2074 6865 206d 6574  alled by the met
+00000180: 6163 6c61 7373 270a 2020 2020 2320 5f5f  aclass'.    # __
+00000190: 6361 6c6c 5f5f 2028 692e 652e 2043 6f6c  call__ (i.e. Col
+000001a0: 6f72 2833 2920 292c 2061 6e64 2062 7920  or(3) ), and by 
+000001b0: 7069 636b 6c65 0a20 2020 2069 6620 7479  pickle.    if ty
+000001c0: 7065 2876 616c 7565 2920 6973 2063 6c73  pe(value) is cls
+000001d0: 3a0a 2020 2020 2020 2020 2320 466f 7220  :.        # For 
+000001e0: 6c6f 6f6b 7570 7320 6c69 6b65 2043 6f6c  lookups like Col
+000001f0: 6f72 2843 6f6c 6f72 2e52 4544 290a 2020  or(Color.RED).  
+00000200: 2020 2020 2020 7265 7475 726e 2076 616c        return val
+00000210: 7565 0a20 2020 2023 2062 792d 7661 6c75  ue.    # by-valu
+00000220: 6520 7365 6172 6368 2066 6f72 2061 206d  e search for a m
+00000230: 6174 6368 696e 6720 656e 756d 206d 656d  atching enum mem
+00000240: 6265 720a 2020 2020 2320 7365 6520 6966  ber.    # see if
+00000250: 2069 7427 7320 696e 2074 6865 2072 6576   it's in the rev
+00000260: 6572 7365 206d 6170 7069 6e67 2028 666f  erse mapping (fo
+00000270: 7220 6861 7368 6162 6c65 2076 616c 7565  r hashable value
+00000280: 7329 0a20 2020 2074 7279 3a0a 2020 2020  s).    try:.    
+00000290: 2020 2020 6966 2076 616c 7565 2069 6e20      if value in 
+000002a0: 636c 732e 5f76 616c 7565 326d 656d 6265  cls._value2membe
+000002b0: 725f 6d61 705f 3a0a 2020 2020 2020 2020  r_map_:.        
+000002c0: 2020 2020 7265 7475 726e 2063 6c73 2e5f      return cls._
+000002d0: 7661 6c75 6532 6d65 6d62 6572 5f6d 6170  value2member_map
+000002e0: 5f5b 7661 6c75 655d 0a20 2020 2065 7863  _[value].    exc
+000002f0: 6570 7420 5479 7065 4572 726f 723a 0a20  ept TypeError:. 
+00000300: 2020 2020 2020 2023 206e 6f74 2074 6865         # not the
+00000310: 7265 2c20 6e6f 7720 646f 206c 6f6e 6720  re, now do long 
+00000320: 7365 6172 6368 202d 2d20 4f28 6e29 2062  search -- O(n) b
+00000330: 6568 6176 696f 720a 2020 2020 2020 2020  ehavior.        
+00000340: 666f 7220 6d65 6d62 6572 2069 6e20 636c  for member in cl
+00000350: 732e 5f6d 656d 6265 725f 6d61 705f 2e76  s._member_map_.v
+00000360: 616c 7565 7328 293a 0a20 2020 2020 2020  alues():.       
+00000370: 2020 2020 2069 6620 6d65 6d62 6572 2e5f       if member._
+00000380: 7661 6c75 655f 203d 3d20 7661 6c75 653a  value_ == value:
+00000390: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000003a0: 2072 6574 7572 6e20 6d65 6d62 6572 0a20   return member. 
+000003b0: 2020 2023 2073 7469 6c6c 206e 6f74 2066     # still not f
+000003c0: 6f75 6e64 202d 2d20 7472 7920 5f6d 6973  ound -- try _mis
+000003d0: 7369 6e67 5f20 686f 6f6b 0a20 2020 2074  sing_ hook.    t
+000003e0: 7279 3a0a 2020 2020 2020 2020 6578 6320  ry:.        exc 
+000003f0: 3d20 4e6f 6e65 0a20 2020 2020 2020 2072  = None.        r
+00000400: 6573 756c 7420 3d20 636c 732e 5f6d 6973  esult = cls._mis
+00000410: 7369 6e67 5f28 7661 6c75 6529 0a20 2020  sing_(value).   
+00000420: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
+00000430: 6e20 6173 2065 3a0a 2020 2020 2020 2020  n as e:.        
+00000440: 6578 6320 3d20 650a 2020 2020 2020 2020  exc = e.        
+00000450: 7265 7375 6c74 203d 204e 6f6e 650a 0a20  result = None.. 
+00000460: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+00000470: 2872 6573 756c 742c 2063 6c73 293a 0a20  (result, cls):. 
+00000480: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+00000490: 7375 6c74 0a20 2020 2065 6c73 653a 0a20  sult.    else:. 
+000004a0: 2020 2020 2020 2076 655f 6578 6320 3d20         ve_exc = 
+000004b0: 5661 6c75 6545 7272 6f72 2822 2572 2069  ValueError("%r i
+000004c0: 7320 6e6f 7420 6120 7661 6c69 6420 2573  s not a valid %s
+000004d0: 2220 2520 2876 616c 7565 2c20 636c 732e  " % (value, cls.
+000004e0: 5f5f 6e61 6d65 5f5f 2929 0a20 2020 2020  __name__)).     
+000004f0: 2020 2069 6620 7265 7375 6c74 2069 7320     if result is 
+00000500: 4e6f 6e65 2061 6e64 2065 7863 2069 7320  None and exc is 
+00000510: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00000520: 2020 7261 6973 6520 7665 5f65 7863 0a20    raise ve_exc. 
+00000530: 2020 2020 2020 2065 6c69 6620 6578 6320         elif exc 
+00000540: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+00000550: 2020 2020 2065 7863 203d 2054 7970 6545       exc = TypeE
+00000560: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
+00000570: 2020 2020 2020 2765 7272 6f72 2069 6e20        'error in 
+00000580: 2573 2e5f 6d69 7373 696e 675f 3a20 7265  %s._missing_: re
+00000590: 7475 726e 6564 2025 7220 696e 7374 6561  turned %r instea
+000005a0: 6420 6f66 204e 6f6e 6520 6f72 2061 2076  d of None or a v
+000005b0: 616c 6964 206d 656d 6265 7227 0a20 2020  alid member'.   
+000005c0: 2020 2020 2020 2020 2020 2020 2025 2028               % (
+000005d0: 636c 732e 5f5f 6e61 6d65 5f5f 2c20 7265  cls.__name__, re
+000005e0: 7375 6c74 290a 2020 2020 2020 2020 2020  sult).          
+000005f0: 2020 290a 2020 2020 2020 2020 6578 632e    ).        exc.
+00000600: 5f5f 636f 6e74 6578 745f 5f20 3d20 7665  __context__ = ve
+00000610: 5f65 7863 0a20 2020 2020 2020 2072 6169  _exc.        rai
+00000620: 7365 2065 7863 0a0a 0a45 6e75 6d2e 5f5f  se exc...Enum.__
+00000630: 6e65 775f 5f20 3d20 5f6f 7269 675f 656e  new__ = _orig_en
+00000640: 756d 5f6e 6577 0a53 7472 4173 5265 7072  um_new.StrAsRepr
+00000650: 4d69 7869 6e45 6e75 6d2e 5f5f 6e65 775f  MixinEnum.__new_
+00000660: 5f20 3d20 5f6f 7269 675f 656e 756d 5f6e  _ = _orig_enum_n
+00000670: 6577 0a4c 6f6f 6b55 704d 6978 696e 456e  ew.LookUpMixinEn
+00000680: 756d 2e5f 5f6e 6577 5f5f 203d 205f 6f72  um.__new__ = _or
+00000690: 6967 5f65 6e75 6d5f 6e65 770a 4175 746f  ig_enum_new.Auto
+000006a0: 4e61 6d65 4d69 7869 6e45 6e75 6d2e 5f5f  NameMixinEnum.__
+000006b0: 6e65 775f 5f20 3d20 5f6f 7269 675f 656e  new__ = _orig_en
+000006c0: 756d 5f6e 6577 0a4d 6973 7369 6e67 4e6f  um_new.MissingNo
+000006d0: 6e65 4d69 7869 6e45 6e75 6d2e 5f5f 6e65  neMixinEnum.__ne
+000006e0: 775f 5f20 3d20 5f6f 7269 675f 656e 756d  w__ = _orig_enum
+000006f0: 5f6e 6577 0a0a 0a6c 6f67 6765 7220 3d20  _new...logger = 
+00000700: 6c6f 6767 696e 672e 6765 744c 6f67 6765  logging.getLogge
+00000710: 7228 5f5f 6e61 6d65 5f5f 290a 0a23 0a23  r(__name__)..#.#
+00000720: 2040 7079 7465 7374 2e66 6978 7475 7265   @pytest.fixture
+00000730: 2829 0a23 2064 6566 206d 795f 6465 7065  ().# def my_depe
+00000740: 6e64 656e 6379 2829 3a0a 2320 2020 2020  ndency():.#     
+00000750: 7265 7475 726e 2034 320a 230a 2320 2340  return 42.#.# #@
+00000760: 7079 7465 7374 2e6d 6172 6b2e 7773 0a23  pytest.mark.ws.#
+00000770: 2064 6566 2074 6573 745f 6669 7273 7428   def test_first(
+00000780: 6d79 5f64 6570 656e 6465 6e63 7920 293a  my_dependency ):
+00000790: 0a23 2020 2020 206c 6f67 6765 722e 696e  .#     logger.in
+000007a0: 666f 2827 5465 7374 696e 6720 6669 7273  fo('Testing firs
+000007b0: 7427 290a 230a 0a0a 636c 6173 7320 5465  t').#...class Te
+000007c0: 7374 5374 616e 6461 7264 456e 756d 286f  stStandardEnum(o
+000007d0: 626a 6563 7429 3a0a 2020 2020 4065 6e75  bject):.    @enu
+000007e0: 6d2e 756e 6971 7565 0a20 2020 2063 6c61  m.unique.    cla
+000007f0: 7373 2043 6f6c 6f72 3128 456e 756d 293a  ss Color1(Enum):
+00000800: 0a20 2020 2020 2020 2052 4544 203d 2031  .        RED = 1
+00000810: 300a 2020 2020 2020 2020 424c 5545 203d  0.        BLUE =
+00000820: 2032 300a 2020 2020 2020 2020 4752 4545   20.        GREE
+00000830: 4e20 3d20 3330 0a0a 2020 2020 4065 6e75  N = 30..    @enu
+00000840: 6d2e 756e 6971 7565 0a20 2020 2063 6c61  m.unique.    cla
+00000850: 7373 2043 6f6c 6f72 3228 456e 756d 293a  ss Color2(Enum):
+00000860: 0a20 2020 2020 2020 2052 4544 203d 2027  .        RED = '
+00000870: 7227 0a20 2020 2020 2020 2042 4c55 4520  r'.        BLUE 
+00000880: 3d20 2762 270a 2020 2020 2020 2020 4752  = 'b'.        GR
+00000890: 4545 4e20 3d20 2767 270a 0a20 2020 2040  EEN = 'g'..    @
+000008a0: 656e 756d 2e75 6e69 7175 650a 2020 2020  enum.unique.    
+000008b0: 636c 6173 7320 436f 6c6f 7233 2845 6e75  class Color3(Enu
+000008c0: 6d29 3a0a 2020 2020 2020 2020 5245 4420  m):.        RED 
+000008d0: 3d20 6175 746f 2829 0a20 2020 2020 2020  = auto().       
+000008e0: 2042 4c55 4520 3d20 6175 746f 2829 0a20   BLUE = auto(). 
+000008f0: 2020 2020 2020 2047 5245 454e 203d 2061         GREEN = a
+00000900: 7574 6f28 290a 0a0a 2020 2020 4070 7974  uto()...    @pyt
+00000910: 6573 742e 6d61 726b 2e70 6172 616d 6574  est.mark.paramet
+00000920: 7269 7a65 280a 2020 2020 2020 2020 2763  rize(.        'c
+00000930: 6c73 2c69 735f 6279 5f6e 616d 652c 7661  ls,is_by_name,va
+00000940: 6c75 6527 2c0a 2020 2020 2020 2020 5b0a  lue',.        [.
+00000950: 2020 2020 2020 2020 2020 2020 2843 6f6c              (Col
+00000960: 6f72 312c 2054 7275 652c 2031 3029 2c0a  or1, True, 10),.
+00000970: 2020 2020 2020 2020 2020 2020 2320 2843              # (C
+00000980: 6f6c 6f72 312c 2046 616c 7365 2c20 2752  olor1, False, 'R
+00000990: 4544 2729 2c0a 2020 2020 2020 2020 2020  ED'),.          
+000009a0: 2020 2320 2843 6f6c 6f72 322c 2054 7275    # (Color2, Tru
+000009b0: 652c 2027 6227 292c 0a20 2020 2020 2020  e, 'b'),.       
+000009c0: 2020 2020 2023 2028 436f 6c6f 7232 2c20       # (Color2, 
+000009d0: 4661 6c73 652c 2027 424c 5545 2729 2c0a  False, 'BLUE'),.
+000009e0: 2020 2020 2020 2020 2020 2020 2320 2843              # (C
+000009f0: 6f6c 6f72 332c 2054 7275 652c 2033 292c  olor3, True, 3),
+00000a00: 0a20 2020 2020 2020 2020 2020 2023 2028  .            # (
+00000a10: 436f 6c6f 7233 2c20 4661 6c73 652c 2027  Color3, False, '
+00000a20: 4752 4545 4e27 292c 0a20 2020 2020 2020  GREEN'),.       
+00000a30: 205d 0a20 2020 2029 0a20 2020 2064 6566   ].    ).    def
+00000a40: 2074 6573 745f 6275 696c 7469 6e5f 656e   test_builtin_en
+00000a50: 756d 7572 6174 696f 6e28 7365 6c66 2c20  umuration(self, 
+00000a60: 7265 7175 6573 742c 2063 6c73 2c20 6973  request, cls, is
+00000a70: 5f62 795f 6e61 6d65 2c20 7661 6c75 6529  _by_name, value)
+00000a80: 3a0a 2020 2020 2020 2020 6c6f 6767 6572  :.        logger
+00000a90: 2e69 6e66 6f28 6627 7b72 6571 7565 7374  .info(f'{request
+00000aa0: 2e5f 7079 6675 6e63 6974 656d 2e6e 616d  ._pyfuncitem.nam
+00000ab0: 657d 2829 2729 0a20 2020 2020 2020 2073  e}()').        s
+00000ac0: 6f6d 655f 656e 756d 203d 2063 6c73 2876  ome_enum = cls(v
+00000ad0: 616c 7565 2920 6966 2069 735f 6279 5f6e  alue) if is_by_n
+00000ae0: 616d 6520 656c 7365 2063 6c73 5b76 616c  ame else cls[val
+00000af0: 7565 5d0a 2020 2020 2020 2020 6c6f 6767  ue].        logg
+00000b00: 6572 2e69 6e66 6f28 6627 6e61 6d65 2069  er.info(f'name i
+00000b10: 7320 7b73 6f6d 655f 656e 756d 2172 7d27  s {some_enum!r}'
+00000b20: 290a 2020 2020 2020 2020 7365 635f 656e  ).        sec_en
+00000b30: 756d 203d 2063 6c73 5b73 6f6d 655f 656e  um = cls[some_en
+00000b40: 756d 2e6e 616d 655d 0a20 2020 2020 2020  um.name].       
+00000b50: 2061 7373 6572 7420 736f 6d65 5f65 6e75   assert some_enu
+00000b60: 6d20 3d3d 2073 6563 5f65 6e75 6d0a 0a20  m == sec_enum.. 
+00000b70: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
+00000b80: 6275 6728 736f 6d65 5f65 6e75 6d29 0a20  bug(some_enum). 
+00000b90: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
+00000ba0: 6275 6728 6627 7265 7072 2069 7320 7b73  bug(f'repr is {s
+00000bb0: 6f6d 655f 656e 756d 2172 7d27 290a 2020  ome_enum!r}').  
+00000bc0: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
+00000bd0: 7567 2866 2773 7472 2069 7320 7b73 6f6d  ug(f'str is {som
+00000be0: 655f 656e 756d 2173 7d27 290a 2020 2020  e_enum!s}').    
+00000bf0: 2020 2020 5b6c 6f67 6765 722e 6465 6275      [logger.debu
+00000c00: 6728 6627 7b6d 656d 6265 7221 727d 2729  g(f'{member!r}')
+00000c10: 2066 6f72 206d 656d 6265 7220 696e 2063   for member in c
+00000c20: 6c73 2e5f 5f6d 656d 6265 7273 5f5f 2e76  ls.__members__.v
+00000c30: 616c 7565 7328 295d 0a0a 2020 2020 2020  alues()]..      
+00000c40: 2020 7769 7468 2070 7974 6573 742e 7261    with pytest.ra
+00000c50: 6973 6573 284b 6579 4572 726f 7229 2061  ises(KeyError) a
+00000c60: 7320 6578 6369 6e66 6f3a 0a20 2020 2020  s excinfo:.     
+00000c70: 2020 2020 2020 2063 6c73 5b27 6d69 7373         cls['miss
+00000c80: 696e 675f 6b65 795f 6865 7265 5f69 745f  ing_key_here_it_
+00000c90: 6973 275d 0a20 2020 2020 2020 2020 2020  is'].           
+00000ca0: 2023 206c 6f67 6765 722e 6465 6275 6728   # logger.debug(
+00000cb0: 6578 6369 6e66 6f2e 7661 6c75 652c 2065  excinfo.value, e
+00000cc0: 7863 5f69 6e66 6f3d 2865 7863 696e 666f  xc_info=(excinfo
+00000cd0: 2e74 7970 652c 2065 7863 696e 666f 2e76  .type, excinfo.v
+00000ce0: 616c 7565 2c20 6578 6369 6e66 6f2e 7462  alue, excinfo.tb
+00000cf0: 2929 0a0a 2020 2020 2020 2020 7769 7468  ))..        with
+00000d00: 2070 7974 6573 742e 7261 6973 6573 2856   pytest.raises(V
+00000d10: 616c 7565 4572 726f 7229 2061 7320 6578  alueError) as ex
+00000d20: 6369 6e66 6f3a 0a20 2020 2020 2020 2020  cinfo:.         
+00000d30: 2020 2063 6c73 2827 6d69 7373 696e 675f     cls('missing_
+00000d40: 7661 6c75 655f 6865 7265 5f69 745f 6973  value_here_it_is
+00000d50: 2729 0a20 2020 2020 2020 2020 2020 2023  ').            #
+00000d60: 206c 6f67 6765 722e 6465 6275 6728 6578   logger.debug(ex
+00000d70: 6369 6e66 6f2e 7661 6c75 652c 2065 7863  cinfo.value, exc
+00000d80: 5f69 6e66 6f3d 2865 7863 696e 666f 2e74  _info=(excinfo.t
+00000d90: 7970 652c 2065 7863 696e 666f 2e76 616c  ype, excinfo.val
+00000da0: 7565 2c20 6578 6369 6e66 6f2e 7462 2929  ue, excinfo.tb))
+00000db0: 0a0a 0a63 6c61 7373 2054 6573 7453 7472  ...class TestStr
+00000dc0: 4173 5265 7072 4d69 7869 6e45 6e75 6d28  AsReprMixinEnum(
+00000dd0: 6f62 6a65 6374 293a 0a0a 2020 2020 4065  object):..    @e
+00000de0: 6e75 6d2e 756e 6971 7565 0a20 2020 2063  num.unique.    c
+00000df0: 6c61 7373 2043 6f6c 6f72 5374 7228 5374  lass ColorStr(St
+00000e00: 7241 7352 6570 724d 6978 696e 456e 756d  rAsReprMixinEnum
+00000e10: 293a 0a20 2020 2020 2020 2052 4544 203d  ):.        RED =
+00000e20: 2061 7574 6f28 290a 2020 2020 2020 2020   auto().        
+00000e30: 424c 5545 203d 2061 7574 6f28 290a 2020  BLUE = auto().  
+00000e40: 2020 2020 2020 4752 4545 4e20 3d20 6175        GREEN = au
+00000e50: 746f 2829 0a0a 2020 2020 4065 6e75 6d2e  to()..    @enum.
+00000e60: 756e 6971 7565 0a20 2020 2063 6c61 7373  unique.    class
+00000e70: 2043 6f6c 6f72 5374 7232 2853 7472 4173   ColorStr2(StrAs
+00000e80: 5265 7072 4d69 7869 6e45 6e75 6d2c 2045  ReprMixinEnum, E
+00000e90: 6e75 6d29 3a0a 2020 2020 2020 2020 5245  num):.        RE
+00000ea0: 4420 3d20 6175 746f 2829 0a20 2020 2020  D = auto().     
+00000eb0: 2020 2042 4c55 4520 3d20 6175 746f 2829     BLUE = auto()
+00000ec0: 0a20 2020 2020 2020 2047 5245 454e 203d  .        GREEN =
+00000ed0: 2061 7574 6f28 290a 0a0a 0a20 2020 2040   auto()....    @
+00000ee0: 7079 7465 7374 2e6d 6172 6b2e 7061 7261  pytest.mark.para
+00000ef0: 6d65 7472 697a 6528 0a20 2020 2020 2020  metrize(.       
+00000f00: 2020 2763 6c73 272c 0a20 2020 2020 2020    'cls',.       
+00000f10: 205b 0a20 2020 2020 2020 2020 2020 2043   [.            C
+00000f20: 6f6c 6f72 5374 722c 0a20 2020 2020 2020  olorStr,.       
+00000f30: 2020 2020 2043 6f6c 6f72 5374 7232 0a20       ColorStr2. 
+00000f40: 2020 2020 2020 205d 290a 2020 2020 6465         ]).    de
+00000f50: 6620 7465 7374 5f53 7472 4173 5265 7072  f test_StrAsRepr
+00000f60: 4d69 7869 6e45 6e75 6d28 7365 6c66 2c20  MixinEnum(self, 
+00000f70: 7265 7175 6573 742c 2063 6c73 293a 0a20  request, cls):. 
+00000f80: 2020 2020 2020 206c 6f67 6765 722e 696e         logger.in
+00000f90: 666f 2866 277b 7265 7175 6573 742e 5f70  fo(f'{request._p
+00000fa0: 7966 756e 6369 7465 6d2e 6e61 6d65 7d28  yfuncitem.name}(
+00000fb0: 2927 290a 2020 2020 2020 2020 736f 6d65  )').        some
+00000fc0: 5f65 6e75 6d20 3d20 636c 7328 3129 0a20  _enum = cls(1). 
+00000fd0: 2020 2020 2020 206c 6f67 6765 722e 696e         logger.in
+00000fe0: 666f 2866 276e 616d 6520 6973 207b 736f  fo(f'name is {so
+00000ff0: 6d65 5f65 6e75 6d21 727d 2729 0a20 2020  me_enum!r}').   
+00001000: 2020 2020 2073 6563 5f65 6e75 6d20 3d20       sec_enum = 
+00001010: 636c 735b 736f 6d65 5f65 6e75 6d2e 6e61  cls[some_enum.na
+00001020: 6d65 5d0a 2020 2020 2020 2020 6173 7365  me].        asse
+00001030: 7274 2073 6f6d 655f 656e 756d 3d3d 7365  rt some_enum==se
+00001040: 635f 656e 756d 0a0a 2020 2020 2020 2020  c_enum..        
+00001050: 6c6f 6767 6572 2e64 6562 7567 2873 6f6d  logger.debug(som
+00001060: 655f 656e 756d 290a 2020 2020 2020 2020  e_enum).        
+00001070: 6c6f 6767 6572 2e64 6562 7567 2866 2772  logger.debug(f'r
+00001080: 6570 7220 6973 207b 736f 6d65 5f65 6e75  epr is {some_enu
+00001090: 6d21 727d 2729 0a20 2020 2020 2020 206c  m!r}').        l
+000010a0: 6f67 6765 722e 6465 6275 6728 6627 7374  ogger.debug(f'st
+000010b0: 7220 6973 207b 736f 6d65 5f65 6e75 6d21  r is {some_enum!
+000010c0: 737d 2729 0a20 2020 2020 2020 205b 6c6f  s}').        [lo
+000010d0: 6767 6572 2e64 6562 7567 2866 277b 6d65  gger.debug(f'{me
+000010e0: 6d62 6572 2172 7d27 2920 666f 7220 6d65  mber!r}') for me
+000010f0: 6d62 6572 2069 6e20 636c 732e 5f5f 6d65  mber in cls.__me
+00001100: 6d62 6572 735f 5f2e 7661 6c75 6573 2829  mbers__.values()
+00001110: 5d0a 0a20 2020 2020 2020 2061 7373 6572  ]..        asser
+00001120: 7420 7265 7072 2873 6f6d 655f 656e 756d  t repr(some_enum
+00001130: 2920 3d3d 2073 7472 2873 6f6d 655f 656e  ) == str(some_en
+00001140: 756d 290a 0a0a 636c 6173 7320 5465 7374  um)...class Test
+00001150: 4175 746f 4e61 6d65 4d69 7869 6e45 6e75  AutoNameMixinEnu
+00001160: 6d28 6f62 6a65 6374 293a 0a20 2020 2040  m(object):.    @
+00001170: 656e 756d 2e75 6e69 7175 650a 2020 2020  enum.unique.    
+00001180: 636c 6173 7320 436f 6c6f 7241 7574 6f4e  class ColorAutoN
+00001190: 616d 6528 4175 746f 4e61 6d65 4d69 7869  ame(AutoNameMixi
+000011a0: 6e45 6e75 6d29 3a0a 2020 2020 2020 2020  nEnum):.        
+000011b0: 5245 4420 3d20 6175 746f 2829 0a20 2020  RED = auto().   
+000011c0: 2020 2020 2042 4c55 4520 3d20 6175 746f       BLUE = auto
+000011d0: 2829 0a20 2020 2020 2020 2047 5245 454e  ().        GREEN
+000011e0: 203d 2061 7574 6f28 290a 0a20 2020 2040   = auto()..    @
+000011f0: 656e 756d 2e75 6e69 7175 6520 2341 7574  enum.unique #Aut
+00001200: 6f4e 616d 654d 6978 696e 456e 756d 2068  oNameMixinEnum h
+00001210: 6173 2074 6f20 6265 206c 6173 7420 2873  as to be last (s
+00001220: 6565 2045 6e75 6d4d 6574 612e 5f5f 7072  ee EnumMeta.__pr
+00001230: 6570 6172 655f 5f28 2929 0a20 2020 2020  epare__()).     
+00001240: 2020 2020 2020 2020 2020 2020 236d 6574              #met
+00001250: 686f 6420 5f67 656e 6572 6174 655f 6e65  hod _generate_ne
+00001260: 7874 5f76 616c 7565 5f28 2920 7769 6c6c  xt_value_() will
+00001270: 2062 6520 7461 6b65 6e20 6672 6f6d 2074   be taken from t
+00001280: 6865 6972 650a 2020 2020 636c 6173 7320  heire.    class 
+00001290: 436f 6c6f 7241 7574 6f4e 616d 6532 2853  ColorAutoName2(S
+000012a0: 7472 4173 5265 7072 4d69 7869 6e45 6e75  trAsReprMixinEnu
+000012b0: 6d2c 2041 7574 6f4e 616d 654d 6978 696e  m, AutoNameMixin
+000012c0: 456e 756d 293a 0a20 2020 2020 2020 2052  Enum):.        R
+000012d0: 4544 203d 2061 7574 6f28 290a 2020 2020  ED = auto().    
+000012e0: 2020 2020 424c 5545 203d 2061 7574 6f28      BLUE = auto(
+000012f0: 290a 2020 2020 2020 2020 4752 4545 4e20  ).        GREEN 
+00001300: 3d20 6175 746f 2829 0a0a 2020 2020 4065  = auto()..    @e
+00001310: 6e75 6d2e 756e 6971 7565 2023 4175 746f  num.unique #Auto
+00001320: 4e61 6d65 4d69 7869 6e45 6e75 6d20 6861  NameMixinEnum ha
+00001330: 7320 746f 2062 6520 6c61 7374 2028 7365  s to be last (se
+00001340: 6520 456e 756d 4d65 7461 2e5f 5f70 7265  e EnumMeta.__pre
+00001350: 7061 7265 5f5f 2829 290a 2020 2020 636c  pare__()).    cl
+00001360: 6173 7320 436f 6c6f 7241 7574 6f4e 616d  ass ColorAutoNam
+00001370: 6557 726f 6e67 2841 7574 6f4e 616d 654d  eWrong(AutoNameM
+00001380: 6978 696e 456e 756d 2c20 5374 7241 7352  ixinEnum, StrAsR
+00001390: 6570 724d 6978 696e 456e 756d 293a 0a20  eprMixinEnum):. 
+000013a0: 2020 2020 2020 2052 4544 203d 2061 7574         RED = aut
+000013b0: 6f28 290a 2020 2020 2020 2020 424c 5545  o().        BLUE
+000013c0: 203d 2061 7574 6f28 290a 2020 2020 2020   = auto().      
+000013d0: 2020 4752 4545 4e20 3d20 6175 746f 2829    GREEN = auto()
+000013e0: 0a0a 2020 2020 4065 6e75 6d2e 756e 6971  ..    @enum.uniq
+000013f0: 7565 2023 4175 746f 4e61 6d65 4d69 7869  ue #AutoNameMixi
+00001400: 6e45 6e75 6d20 6861 7320 746f 2062 6520  nEnum has to be 
+00001410: 6c61 7374 2028 7365 6520 456e 756d 4d65  last (see EnumMe
+00001420: 7461 2e5f 5f70 7265 7061 7265 5f5f 2829  ta.__prepare__()
+00001430: 290a 2020 2020 636c 6173 7320 436f 6c6f  ).    class Colo
+00001440: 7241 7574 6f4e 616d 6557 726f 6e67 3228  rAutoNameWrong2(
+00001450: 4175 746f 4e61 6d65 4d69 7869 6e45 6e75  AutoNameMixinEnu
+00001460: 6d2c 2045 6e75 6d29 3a0a 2020 2020 2020  m, Enum):.      
+00001470: 2020 5245 4420 3d20 6175 746f 2829 0a20    RED = auto(). 
+00001480: 2020 2020 2020 2042 4c55 4520 3d20 6175         BLUE = au
+00001490: 746f 2829 0a20 2020 2020 2020 2047 5245  to().        GRE
+000014a0: 454e 203d 2061 7574 6f28 290a 0a0a 0a0a  EN = auto().....
+000014b0: 2020 2020 4070 7974 6573 742e 6d61 726b      @pytest.mark
+000014c0: 2e70 6172 616d 6574 7269 7a65 280a 2020  .parametrize(.  
+000014d0: 2020 2020 2020 2027 636c 7327 2c0a 2020         'cls',.  
+000014e0: 2020 2020 2020 5b0a 2020 2020 2020 2020        [.        
+000014f0: 2020 2020 436f 6c6f 7241 7574 6f4e 616d      ColorAutoNam
+00001500: 652c 0a20 2020 2020 2020 2020 2020 2043  e,.            C
+00001510: 6f6c 6f72 4175 746f 4e61 6d65 322c 0a20  olorAutoName2,. 
+00001520: 2020 2020 2020 205d 290a 2020 2020 6465         ]).    de
+00001530: 6620 7465 7374 5f41 7574 6f4e 616d 654d  f test_AutoNameM
+00001540: 6978 696e 456e 756d 2873 656c 662c 2072  ixinEnum(self, r
+00001550: 6571 7565 7374 2c20 636c 7329 3a0a 2020  equest, cls):.  
+00001560: 2020 2020 2020 6c6f 6767 6572 2e69 6e66        logger.inf
+00001570: 6f28 6627 7b72 6571 7565 7374 2e5f 7079  o(f'{request._py
+00001580: 6675 6e63 6974 656d 2e6e 616d 657d 2829  funcitem.name}()
+00001590: 2729 0a20 2020 2020 2020 2073 6f6d 655f  ').        some_
+000015a0: 656e 756d 203d 2063 6c73 2827 5245 4427  enum = cls('RED'
+000015b0: 290a 2020 2020 2020 2020 6c6f 6767 6572  ).        logger
+000015c0: 2e69 6e66 6f28 6627 6e61 6d65 2069 7320  .info(f'name is 
+000015d0: 7b73 6f6d 655f 656e 756d 2172 7d27 290a  {some_enum!r}').
+000015e0: 2020 2020 2020 2020 7365 635f 656e 756d          sec_enum
+000015f0: 203d 2063 6c73 5b73 6f6d 655f 656e 756d   = cls[some_enum
+00001600: 2e6e 616d 655d 0a20 2020 2020 2020 2061  .name].        a
+00001610: 7373 6572 7420 736f 6d65 5f65 6e75 6d3d  ssert some_enum=
+00001620: 3d73 6563 5f65 6e75 6d0a 0a20 2020 2040  =sec_enum..    @
+00001630: 7079 7465 7374 2e6d 6172 6b2e 7061 7261  pytest.mark.para
+00001640: 6d65 7472 697a 6528 0a20 2020 2020 2020  metrize(.       
+00001650: 2020 2763 6c73 2c69 735f 7265 705f 6368    'cls,is_rep_ch
+00001660: 6563 6b27 2c0a 2020 2020 2020 2020 5b0a  eck',.        [.
+00001670: 2020 2020 2020 2020 2020 2020 2843 6f6c              (Col
+00001680: 6f72 4175 746f 4e61 6d65 5772 6f6e 672c  orAutoNameWrong,
+00001690: 2054 7275 6529 2c0a 2020 2020 2020 2020   True),.        
+000016a0: 2020 2020 2843 6f6c 6f72 4175 746f 4e61      (ColorAutoNa
+000016b0: 6d65 5772 6f6e 6732 2c20 4661 6c73 6529  meWrong2, False)
+000016c0: 2c0a 2020 2020 2020 2020 5d29 0a0a 2020  ,.        ])..  
+000016d0: 2020 6465 6620 7465 7374 5f41 7574 6f4e    def test_AutoN
+000016e0: 616d 6557 726f 6e67 4d69 7869 6e45 6e75  ameWrongMixinEnu
+000016f0: 6d28 7365 6c66 2c20 7265 7175 6573 742c  m(self, request,
+00001700: 2063 6c73 2c20 6973 5f72 6570 5f63 6865   cls, is_rep_che
+00001710: 636b 293a 0a20 2020 2020 2020 206c 6f67  ck):.        log
+00001720: 6765 722e 696e 666f 2866 277b 7265 7175  ger.info(f'{requ
+00001730: 6573 742e 5f70 7966 756e 6369 7465 6d2e  est._pyfuncitem.
+00001740: 6e61 6d65 7d28 2927 290a 0a20 2020 2020  name}()')..     
+00001750: 2020 2077 6974 6820 7079 7465 7374 2e72     with pytest.r
+00001760: 6169 7365 7328 5661 6c75 6545 7272 6f72  aises(ValueError
+00001770: 2920 6173 2065 7863 696e 666f 3a0a 2020  ) as excinfo:.  
+00001780: 2020 2020 2020 2020 2020 736f 6d65 5f65            some_e
+00001790: 6e75 6d20 3d20 636c 7328 2752 4544 2729  num = cls('RED')
+000017a0: 0a20 2020 2020 2020 2020 2020 206c 6f67  .            log
+000017b0: 6765 722e 6465 6275 6728 6578 6369 6e66  ger.debug(excinf
+000017c0: 6f2e 7661 6c75 652c 2065 7863 5f69 6e66  o.value, exc_inf
+000017d0: 6f3d 2865 7863 696e 666f 2e74 7970 652c  o=(excinfo.type,
+000017e0: 2065 7863 696e 666f 2e76 616c 7565 2c20   excinfo.value, 
+000017f0: 6578 6369 6e66 6f2e 7462 2929 0a0a 2020  excinfo.tb))..  
+00001800: 2020 2020 2020 736f 6d65 5f65 6e75 6d20        some_enum 
+00001810: 3d20 636c 7328 3129 0a20 2020 2020 2020  = cls(1).       
+00001820: 206c 6f67 6765 722e 696e 666f 2866 276e   logger.info(f'n
+00001830: 616d 6520 6973 207b 736f 6d65 5f65 6e75  ame is {some_enu
+00001840: 6d21 727d 2729 0a20 2020 2020 2020 2073  m!r}').        s
+00001850: 6563 5f65 6e75 6d20 3d20 636c 735b 736f  ec_enum = cls[so
+00001860: 6d65 5f65 6e75 6d2e 6e61 6d65 5d0a 2020  me_enum.name].  
+00001870: 2020 2020 2020 6173 7365 7274 2073 6f6d        assert som
+00001880: 655f 656e 756d 3d3d 7365 635f 656e 756d  e_enum==sec_enum
+00001890: 0a0a 2020 2020 2020 2020 6c6f 6767 6572  ..        logger
+000018a0: 2e64 6562 7567 2873 6f6d 655f 656e 756d  .debug(some_enum
+000018b0: 290a 2020 2020 2020 2020 6c6f 6767 6572  ).        logger
+000018c0: 2e64 6562 7567 2866 2772 6570 7220 6973  .debug(f'repr is
+000018d0: 207b 736f 6d65 5f65 6e75 6d21 727d 2729   {some_enum!r}')
+000018e0: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
+000018f0: 6465 6275 6728 6627 7374 7220 6973 207b  debug(f'str is {
+00001900: 736f 6d65 5f65 6e75 6d21 737d 2729 0a20  some_enum!s}'). 
+00001910: 2020 2020 2020 205b 6c6f 6767 6572 2e64         [logger.d
+00001920: 6562 7567 2866 277b 6d65 6d62 6572 2172  ebug(f'{member!r
+00001930: 7d27 2920 666f 7220 6d65 6d62 6572 2069  }') for member i
+00001940: 6e20 636c 732e 5f5f 6d65 6d62 6572 735f  n cls.__members_
+00001950: 5f2e 7661 6c75 6573 2829 5d0a 0a20 2020  _.values()]..   
+00001960: 2020 2020 2069 6620 6973 5f72 6570 5f63       if is_rep_c
+00001970: 6865 636b 3a0a 2020 2020 2020 2020 2020  heck:.          
+00001980: 2020 6173 7365 7274 2072 6570 7228 736f    assert repr(so
+00001990: 6d65 5f65 6e75 6d29 203d 3d20 7374 7228  me_enum) == str(
+000019a0: 736f 6d65 5f65 6e75 6d29 0a0a 0a63 6c61  some_enum)...cla
+000019b0: 7373 2054 6573 744d 6973 7369 6e67 4e6f  ss TestMissingNo
+000019c0: 6e65 4d69 7869 6e45 6e75 6d28 6f62 6a65  neMixinEnum(obje
+000019d0: 6374 293a 0a0a 2020 2020 4065 6e75 6d2e  ct):..    @enum.
+000019e0: 756e 6971 7565 0a20 2020 2063 6c61 7373  unique.    class
+000019f0: 2043 6f6c 6f72 4d69 7373 696e 674e 6f6e   ColorMissingNon
+00001a00: 6528 4d69 7373 696e 674e 6f6e 654d 6978  e(MissingNoneMix
+00001a10: 696e 456e 756d 293a 0a20 2020 2020 2020  inEnum):.       
+00001a20: 2052 4544 203d 2061 7574 6f28 290a 2020   RED = auto().  
+00001a30: 2020 2020 2020 424c 5545 203d 2061 7574        BLUE = aut
+00001a40: 6f28 290a 2020 2020 2020 2020 4752 4545  o().        GREE
+00001a50: 4e20 3d20 6175 746f 2829 0a0a 0a20 2020  N = auto()...   
+00001a60: 2064 6566 2074 6573 745f 4d69 7373 696e   def test_Missin
+00001a70: 674e 6f6e 6545 6e75 6d28 7365 6c66 2c20  gNoneEnum(self, 
+00001a80: 7265 7175 6573 7429 3a0a 2020 2020 2020  request):.      
+00001a90: 2020 6c6f 6767 6572 2e69 6e66 6f28 6627    logger.info(f'
+00001aa0: 7b72 6571 7565 7374 2e5f 7079 6675 6e63  {request._pyfunc
+00001ab0: 6974 656d 2e6e 616d 657d 2829 2729 0a0a  item.name}()')..
+00001ac0: 2020 2020 2020 2020 736f 6d65 5f65 6e75          some_enu
+00001ad0: 6d20 3d20 5465 7374 4d69 7373 696e 674e  m = TestMissingN
+00001ae0: 6f6e 654d 6978 696e 456e 756d 2e43 6f6c  oneMixinEnum.Col
+00001af0: 6f72 4d69 7373 696e 674e 6f6e 6528 3129  orMissingNone(1)
+00001b00: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
+00001b10: 696e 666f 2866 276e 616d 6520 6973 207b  info(f'name is {
+00001b20: 736f 6d65 5f65 6e75 6d21 727d 2729 0a20  some_enum!r}'). 
+00001b30: 2020 2020 2020 2073 6563 5f65 6e75 6d20         sec_enum 
+00001b40: 3d20 5465 7374 4d69 7373 696e 674e 6f6e  = TestMissingNon
+00001b50: 654d 6978 696e 456e 756d 2e43 6f6c 6f72  eMixinEnum.Color
+00001b60: 4d69 7373 696e 674e 6f6e 655b 736f 6d65  MissingNone[some
+00001b70: 5f65 6e75 6d2e 6e61 6d65 5d0a 2020 2020  _enum.name].    
+00001b80: 2020 2020 6173 7365 7274 2073 6f6d 655f      assert some_
+00001b90: 656e 756d 3d3d 7365 635f 656e 756d 0a0a  enum==sec_enum..
+00001ba0: 2020 2020 2020 2020 7769 7468 2070 7974          with pyt
+00001bb0: 6573 742e 7261 6973 6573 284b 6579 4572  est.raises(KeyEr
+00001bc0: 726f 7229 2061 7320 6578 6369 6e66 6f3a  ror) as excinfo:
+00001bd0: 0a20 2020 2020 2020 2020 2020 2054 6573  .            Tes
+00001be0: 744d 6973 7369 6e67 4e6f 6e65 4d69 7869  tMissingNoneMixi
+00001bf0: 6e45 6e75 6d2e 436f 6c6f 724d 6973 7369  nEnum.ColorMissi
+00001c00: 6e67 4e6f 6e65 5b31 305f 3030 305d 0a20  ngNone[10_000]. 
+00001c10: 2020 2020 2020 2020 2020 2023 6c6f 6767             #logg
+00001c20: 6572 2e64 6562 7567 2865 7863 696e 666f  er.debug(excinfo
+00001c30: 2e76 616c 7565 2c20 6578 635f 696e 666f  .value, exc_info
+00001c40: 3d28 6578 6369 6e66 6f2e 7479 7065 2c20  =(excinfo.type, 
+00001c50: 6578 6369 6e66 6f2e 7661 6c75 652c 2065  excinfo.value, e
+00001c60: 7863 696e 666f 2e74 6229 290a 0a20 2020  xcinfo.tb))..   
+00001c70: 2020 2020 2077 6974 6820 7079 7465 7374       with pytest
+00001c80: 2e72 6169 7365 7328 5661 6c75 6545 7272  .raises(ValueErr
+00001c90: 6f72 2920 6173 2065 7863 696e 666f 3a0a  or) as excinfo:.
+00001ca0: 2020 2020 2020 2020 2020 2020 5465 7374              Test
+00001cb0: 4d69 7373 696e 674e 6f6e 654d 6978 696e  MissingNoneMixin
+00001cc0: 456e 756d 2e43 6f6c 6f72 4d69 7373 696e  Enum.ColorMissin
+00001cd0: 674e 6f6e 6528 3130 5f30 3030 290a 0a0a  gNone(10_000)...
+00001ce0: 0a63 6c61 7373 2054 6573 744c 6f6f 6b55  .class TestLookU
+00001cf0: 704d 6978 696e 456e 756d 286f 626a 6563  pMixinEnum(objec
+00001d00: 7429 3a0a 0a20 2020 2040 656e 756d 2e75  t):..    @enum.u
+00001d10: 6e69 7175 650a 2020 2020 636c 6173 7320  nique.    class 
+00001d20: 436f 6c6f 724c 6f6f 6b55 7028 4c6f 6f6b  ColorLookUp(Look
+00001d30: 5570 4d69 7869 6e45 6e75 6d29 3a0a 2020  UpMixinEnum):.  
+00001d40: 2020 2020 2020 5245 4420 3d20 2772 270a        RED = 'r'.
+00001d50: 2020 2020 2020 2020 424c 5545 203d 2027          BLUE = '
+00001d60: 6227 0a20 2020 2020 2020 2047 5245 454e  b'.        GREEN
+00001d70: 203d 2027 6727 0a0a 2020 2020 4065 6e75   = 'g'..    @enu
+00001d80: 6d2e 756e 6971 7565 0a20 2020 2063 6c61  m.unique.    cla
+00001d90: 7373 2043 6f6c 6f72 4c6f 6f6b 5570 4175  ss ColorLookUpAu
+00001da0: 746f 284c 6f6f 6b55 704d 6978 696e 456e  to(LookUpMixinEn
+00001db0: 756d 2c20 4175 746f 4e61 6d65 4d69 7869  um, AutoNameMixi
+00001dc0: 6e45 6e75 6d29 3a0a 2020 2020 2020 2020  nEnum):.        
+00001dd0: 5245 4420 3d20 6175 746f 2829 0a20 2020  RED = auto().   
+00001de0: 2020 2020 2042 4c55 4520 3d20 6175 746f       BLUE = auto
+00001df0: 2829 0a20 2020 2020 2020 2047 5245 454e  ().        GREEN
+00001e00: 203d 2061 7574 6f28 290a 0a0a 0a20 2020   = auto()....   
+00001e10: 2064 6566 2074 6573 745f 436f 6c6f 724c   def test_ColorL
+00001e20: 6f6f 6b55 7028 7365 6c66 2c20 7265 7175  ookUp(self, requ
+00001e30: 6573 7429 3a0a 2020 2020 2020 2020 6c6f  est):.        lo
+00001e40: 6767 6572 2e69 6e66 6f28 6627 7b72 6571  gger.info(f'{req
+00001e50: 7565 7374 2e5f 7079 6675 6e63 6974 656d  uest._pyfuncitem
+00001e60: 2e6e 616d 657d 2829 2729 0a0a 2020 2020  .name}()')..    
+00001e70: 2020 2020 736f 6d65 5f65 6e75 6d20 3d20      some_enum = 
+00001e80: 5465 7374 4c6f 6f6b 5570 4d69 7869 6e45  TestLookUpMixinE
+00001e90: 6e75 6d2e 436f 6c6f 724c 6f6f 6b55 7028  num.ColorLookUp(
+00001ea0: 2772 2729 0a20 2020 2020 2020 206c 6f67  'r').        log
+00001eb0: 6765 722e 696e 666f 2866 276e 616d 6520  ger.info(f'name 
+00001ec0: 6973 207b 736f 6d65 5f65 6e75 6d21 727d  is {some_enum!r}
+00001ed0: 2729 0a20 2020 2020 2020 2073 6563 5f65  ').        sec_e
+00001ee0: 6e75 6d20 3d20 5465 7374 4c6f 6f6b 5570  num = TestLookUp
+00001ef0: 4d69 7869 6e45 6e75 6d2e 436f 6c6f 724c  MixinEnum.ColorL
+00001f00: 6f6f 6b55 705b 736f 6d65 5f65 6e75 6d2e  ookUp[some_enum.
+00001f10: 6e61 6d65 5d0a 2020 2020 2020 2020 6173  name].        as
+00001f20: 7365 7274 2073 6f6d 655f 656e 756d 203d  sert some_enum =
+00001f30: 3d20 7365 635f 656e 756d 0a0a 2020 2020  = sec_enum..    
+00001f40: 2020 2020 7769 7468 2070 7974 6573 742e      with pytest.
+00001f50: 7261 6973 6573 284b 6579 4572 726f 7229  raises(KeyError)
+00001f60: 2061 7320 6578 6369 6e66 6f3a 0a20 2020   as excinfo:.   
+00001f70: 2020 2020 2020 2020 2054 6573 744c 6f6f           TestLoo
+00001f80: 6b55 704d 6978 696e 456e 756d 2e43 6f6c  kUpMixinEnum.Col
+00001f90: 6f72 4c6f 6f6b 5570 5b27 6d69 7373 696e  orLookUp['missin
+00001fa0: 675f 7661 6c75 655f 6865 7265 5f69 745f  g_value_here_it_
+00001fb0: 6973 275d 0a20 2020 2020 2020 2020 2020  is'].           
+00001fc0: 2023 206c 6f67 6765 722e 6465 6275 6728   # logger.debug(
+00001fd0: 6578 6369 6e66 6f2e 7661 6c75 652c 2065  excinfo.value, e
+00001fe0: 7863 5f69 6e66 6f3d 2865 7863 696e 666f  xc_info=(excinfo
+00001ff0: 2e74 7970 652c 2065 7863 696e 666f 2e76  .type, excinfo.v
+00002000: 616c 7565 2c20 6578 6369 6e66 6f2e 7462  alue, excinfo.tb
+00002010: 2929 0a20 2020 2020 2020 2077 6974 6820  )).        with 
+00002020: 7079 7465 7374 2e72 6169 7365 7328 5661  pytest.raises(Va
+00002030: 6c75 6545 7272 6f72 2920 6173 2065 7863  lueError) as exc
+00002040: 696e 666f 3a0a 2020 2020 2020 2020 2020  info:.          
+00002050: 2020 5465 7374 4c6f 6f6b 5570 4d69 7869    TestLookUpMixi
+00002060: 6e45 6e75 6d2e 436f 6c6f 724c 6f6f 6b55  nEnum.ColorLookU
+00002070: 7028 276d 6973 7369 6e67 5f76 616c 7565  p('missing_value
+00002080: 5f68 6572 655f 6974 5f69 7327 290a 0a0a  _here_it_is')...
+00002090: 2020 2020 6465 6620 7465 7374 5f43 6f6c      def test_Col
+000020a0: 6f72 4c6f 6f6b 5570 4175 746f 2873 656c  orLookUpAuto(sel
+000020b0: 662c 2072 6571 7565 7374 293a 0a20 2020  f, request):.   
+000020c0: 2020 2020 206c 6f67 6765 722e 696e 666f       logger.info
+000020d0: 2866 277b 7265 7175 6573 742e 5f70 7966  (f'{request._pyf
+000020e0: 756e 6369 7465 6d2e 6e61 6d65 7d28 2927  uncitem.name}()'
+000020f0: 290a 0a20 2020 2020 2020 2073 6f6d 655f  )..        some_
+00002100: 656e 756d 203d 2054 6573 744c 6f6f 6b55  enum = TestLookU
+00002110: 704d 6978 696e 456e 756d 2e43 6f6c 6f72  pMixinEnum.Color
+00002120: 4c6f 6f6b 5570 4175 746f 2827 5245 4427  LookUpAuto('RED'
+00002130: 290a 2020 2020 2020 2020 6c6f 6767 6572  ).        logger
+00002140: 2e69 6e66 6f28 6627 6e61 6d65 2069 7320  .info(f'name is 
+00002150: 7b73 6f6d 655f 656e 756d 2172 7d27 290a  {some_enum!r}').
+00002160: 2020 2020 2020 2020 7365 635f 656e 756d          sec_enum
+00002170: 203d 2054 6573 744c 6f6f 6b55 704d 6978   = TestLookUpMix
+00002180: 696e 456e 756d 2e43 6f6c 6f72 4c6f 6f6b  inEnum.ColorLook
+00002190: 5570 4175 746f 5b73 6f6d 655f 656e 756d  UpAuto[some_enum
+000021a0: 2e6e 616d 655d 0a20 2020 2020 2020 2061  .name].        a
+000021b0: 7373 6572 7420 736f 6d65 5f65 6e75 6d20  ssert some_enum 
+000021c0: 3d3d 2073 6563 5f65 6e75 6d0a 0a20 2020  == sec_enum..   
+000021d0: 2020 2020 2077 6974 6820 7079 7465 7374       with pytest
+000021e0: 2e72 6169 7365 7328 4b65 7945 7272 6f72  .raises(KeyError
+000021f0: 2920 6173 2065 7863 696e 666f 3a0a 2020  ) as excinfo:.  
+00002200: 2020 2020 2020 2020 2020 5465 7374 4c6f            TestLo
+00002210: 6f6b 5570 4d69 7869 6e45 6e75 6d2e 436f  okUpMixinEnum.Co
+00002220: 6c6f 724c 6f6f 6b55 7041 7574 6f5b 276d  lorLookUpAuto['m
+00002230: 6973 7369 6e67 5f76 616c 7565 5f68 6572  issing_value_her
+00002240: 655f 6974 5f69 7327 5d0a 2020 2020 2020  e_it_is'].      
+00002250: 2020 2020 2020 2320 6c6f 6767 6572 2e64        # logger.d
+00002260: 6562 7567 2865 7863 696e 666f 2e76 616c  ebug(excinfo.val
+00002270: 7565 2c20 6578 635f 696e 666f 3d28 6578  ue, exc_info=(ex
+00002280: 6369 6e66 6f2e 7479 7065 2c20 6578 6369  cinfo.type, exci
+00002290: 6e66 6f2e 7661 6c75 652c 2065 7863 696e  nfo.value, excin
+000022a0: 666f 2e74 6229 290a 2020 2020 2020 2020  fo.tb)).        
+000022b0: 7769 7468 2070 7974 6573 742e 7261 6973  with pytest.rais
+000022c0: 6573 2856 616c 7565 4572 726f 7229 2061  es(ValueError) a
+000022d0: 7320 6578 6369 6e66 6f3a 0a20 2020 2020  s excinfo:.     
+000022e0: 2020 2020 2020 2054 6573 744c 6f6f 6b55         TestLookU
+000022f0: 704d 6978 696e 456e 756d 2e43 6f6c 6f72  pMixinEnum.Color
+00002300: 4c6f 6f6b 5570 4175 746f 2827 6d69 7373  LookUpAuto('miss
+00002310: 696e 675f 7661 6c75 655f 6865 7265 5f69  ing_value_here_i
+00002320: 745f 6973 2729 0a0a 0a0a 636c 6173 7320  t_is')....class 
+00002330: 5465 7374 4c6f 6f6b 5570 4175 746f 4e61  TestLookUpAutoNa
+00002340: 6d65 4d69 7869 6e45 6e75 6d28 6f62 6a65  meMixinEnum(obje
+00002350: 6374 293a 0a0a 2020 2020 6465 6620 6164  ct):..    def ad
+00002360: 6443 6f6d 7028 656e 756d 6572 6174 696f  dComp(enumeratio
+00002370: 6e29 3a0a 2020 2020 2020 2020 2222 2243  n):.        """C
+00002380: 6c61 7373 2064 6563 6f72 6174 6f72 2066  lass decorator f
+00002390: 6f72 2065 6e75 6d65 7261 7469 6f6e 7320  or enumerations 
+000023a0: 2222 220a 2020 2020 2020 2020 616c 6c20  """.        all 
+000023b0: 3d20 5b5d 0a20 2020 2020 2020 2066 6f72  = [].        for
+000023c0: 206d 656d 6265 7220 696e 2065 6e75 6d65   member in enume
+000023d0: 7261 7469 6f6e 2e5f 5f6d 656d 6265 7273  ration.__members
+000023e0: 5f5f 2e76 616c 7565 7328 293a 0a20 2020  __.values():.   
+000023f0: 2020 2020 2020 2020 2061 6c6c 2e61 7070           all.app
+00002400: 656e 6428 6d65 6d62 6572 2e76 616c 7565  end(member.value
+00002410: 290a 0a20 2020 2020 2020 2065 6e75 6d65  )..        enume
+00002420: 7261 7469 6f6e 2e63 6f6d 7020 3d20 616c  ration.comp = al
+00002430: 6c0a 2020 2020 2020 2020 7265 7475 726e  l.        return
+00002440: 2065 6e75 6d65 7261 7469 6f6e 0a0a 2020   enumeration..  
+00002450: 2020 4065 6e75 6d2e 756e 6971 7565 0a20    @enum.unique. 
+00002460: 2020 2040 6164 6443 6f6d 700a 2020 2020     @addComp.    
+00002470: 636c 6173 7320 436f 6c6f 7228 4c6f 6f6b  class Color(Look
+00002480: 5570 4d69 7869 6e45 6e75 6d2c 2041 7574  UpMixinEnum, Aut
+00002490: 6f4e 616d 654d 6978 696e 456e 756d 293a  oNameMixinEnum):
+000024a0: 0a20 2020 2020 2020 2052 4544 203d 2027  .        RED = '
+000024b0: 5227 0a20 2020 2020 2020 2042 4c55 4520  R'.        BLUE 
+000024c0: 3d20 2742 270a 2020 2020 2020 2020 4752  = 'B'.        GR
+000024d0: 4545 4e20 3d20 2247 220a 0a20 2020 2064  EEN = "G"..    d
+000024e0: 6566 2074 6573 745f 436f 6c6f 7228 7365  ef test_Color(se
+000024f0: 6c66 2c20 7265 7175 6573 7429 3a0a 2020  lf, request):.  
+00002500: 2020 2020 2020 6c6f 6767 6572 2e69 6e66        logger.inf
+00002510: 6f28 6627 7b72 6571 7565 7374 2e5f 7079  o(f'{request._py
+00002520: 6675 6e63 6974 656d 2e6e 616d 657d 2829  funcitem.name}()
+00002530: 2729 0a0a 2020 2020 2020 2020 736f 6d65  ')..        some
+00002540: 5f65 6e75 6d20 3d20 5465 7374 4c6f 6f6b  _enum = TestLook
+00002550: 5570 4175 746f 4e61 6d65 4d69 7869 6e45  UpAutoNameMixinE
+00002560: 6e75 6d2e 436f 6c6f 7228 2752 2729 0a20  num.Color('R'). 
+00002570: 2020 2020 2020 206c 6f67 6765 722e 696e         logger.in
+00002580: 666f 2866 276e 616d 6520 6973 207b 736f  fo(f'name is {so
+00002590: 6d65 5f65 6e75 6d21 727d 2729 0a20 2020  me_enum!r}').   
+000025a0: 2020 2020 2073 6563 5f65 6e75 6d20 3d20       sec_enum = 
+000025b0: 5465 7374 4c6f 6f6b 5570 4175 746f 4e61  TestLookUpAutoNa
+000025c0: 6d65 4d69 7869 6e45 6e75 6d2e 436f 6c6f  meMixinEnum.Colo
+000025d0: 725b 736f 6d65 5f65 6e75 6d2e 6e61 6d65  r[some_enum.name
+000025e0: 5d0a 2020 2020 2020 2020 6173 7365 7274  ].        assert
+000025f0: 2073 6f6d 655f 656e 756d 203d 3d20 7365   some_enum == se
+00002600: 635f 656e 756d 0a0a 2020 2020 2020 2020  c_enum..        
+00002610: 7769 7468 2070 7974 6573 742e 7261 6973  with pytest.rais
+00002620: 6573 284b 6579 4572 726f 7229 2061 7320  es(KeyError) as 
+00002630: 6578 6369 6e66 6f3a 0a20 2020 2020 2020  excinfo:.       
+00002640: 2020 2020 2054 6573 744c 6f6f 6b55 7041       TestLookUpA
+00002650: 7574 6f4e 616d 654d 6978 696e 456e 756d  utoNameMixinEnum
+00002660: 2e43 6f6c 6f72 5b27 6d69 7373 696e 675f  .Color['missing_
+00002670: 7661 6c75 655f 6865 7265 5f69 745f 6973  value_here_it_is
+00002680: 275d 0a20 2020 2020 2020 2020 2020 2023  '].            #
+00002690: 206c 6f67 6765 722e 6465 6275 6728 6578   logger.debug(ex
+000026a0: 6369 6e66 6f2e 7661 6c75 652c 2065 7863  cinfo.value, exc
+000026b0: 5f69 6e66 6f3d 2865 7863 696e 666f 2e74  _info=(excinfo.t
+000026c0: 7970 652c 2065 7863 696e 666f 2e76 616c  ype, excinfo.val
+000026d0: 7565 2c20 6578 6369 6e66 6f2e 7462 2929  ue, excinfo.tb))
+000026e0: 0a20 2020 2020 2020 2077 6974 6820 7079  .        with py
+000026f0: 7465 7374 2e72 6169 7365 7328 5661 6c75  test.raises(Valu
+00002700: 6545 7272 6f72 2920 6173 2065 7863 696e  eError) as excin
+00002710: 666f 3a0a 2020 2020 2020 2020 2020 2020  fo:.            
+00002720: 2054 6573 744c 6f6f 6b55 7041 7574 6f4e   TestLookUpAutoN
+00002730: 616d 654d 6978 696e 456e 756d 2e43 6f6c  ameMixinEnum.Col
+00002740: 6f72 2827 6d69 7373 696e 675f 7661 6c75  or('missing_valu
+00002750: 655f 6865 7265 5f69 745f 6973 2729 0a0a  e_here_it_is')..
+00002760: 2020 2020 2020 2020 7661 6c75 6520 3d20          value = 
+00002770: 5465 7374 4c6f 6f6b 5570 4175 746f 4e61  TestLookUpAutoNa
+00002780: 6d65 4d69 7869 6e45 6e75 6d2e 436f 6c6f  meMixinEnum.Colo
+00002790: 722e 636f 6d70 0a20 2020 2020 2020 2061  r.comp.        a
+000027a0: 7373 6572 7420 7661 6c75 6520 6973 206e  ssert value is n
+000027b0: 6f74 204e 6f6e 650a 0a0a 0a69 6620 5f5f  ot None....if __
+000027c0: 6e61 6d65 5f5f 203d 3d20 225f 5f6d 6169  name__ == "__mai
+000027d0: 6e5f 5f22 3a0a 2020 2020 7079 7465 7374  n__":.    pytest
+000027e0: 2e6d 6169 6e28 5b5f 5f66 696c 655f 5f5d  .main([__file__]
+000027f0: 290a 0a                                  )..
```

### Comparing `alex_ber_utils-0.6.6b3/tests/utils/init_app_conf_test.py` & `alex_ber_utils-0.7.0/tests/utils/init_app_conf_test.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,830 +1,830 @@
-import logging
-from collections import OrderedDict
-from collections.abc import Mapping
-import pytest
-import copy
-
-logger = logging.getLogger(__name__)
-from alexber.utils.init_app_conf import mask_value, merge_list_value_in_dicts, to_convex_map, \
-    parse_config
-import alexber.utils.init_app_conf as init_app_conf
-from alexber.utils.init_app_conf import _create_default_parser, AppConfParser
-from alexber.utils.parsers import is_empty
-from tests.utils.ymlparsers_test import ymlparsersSetup, ymlparsersCleanup, exp_config_d
-from importlib.resources import path
-
-def create_default_parser(implicit_convert=None):
-    parser=_create_default_parser(**{'implicit_convert': implicit_convert})
-    return parser
-
-def _reset_initappconf():
-    init_app_conf.default_parser_cls  = None
-    init_app_conf.default_parser_kwargs = None
-
-
-
-@pytest.fixture
-def initappconfFixture(mocker):
-    _reset_initappconf()
-
-    init_app_conf.initConfig()
-    yield None
-    _reset_initappconf()
-
-@pytest.fixture
-def initappconfFalseFixture(mocker):
-    _reset_initappconf()
-
-    init_app_conf.initConfig(**{'default_parser_kwargs': {'implicit_convert': False}})
-    yield None
-    _reset_initappconf()
-
-
-
-class MyAppConfParser(AppConfParser):
-    pass
-
-def test_mask_value_default_as_none(request, initappconfFalseFixture):
-    logger.info(f'{request._pyfuncitem.name}()')
-
-    with pytest.raises(ValueError, match='None'):
-        init_app_conf.initConfig(**{'default_parser_kwargs': {'implicit_convert': None}})
-        mask_value('0.1')
-
-def test_initConfig_default_parser_cls_str(request, initappconfFalseFixture):
-    logger.info(f'{request._pyfuncitem.name}()')
-
-    class_name = '.'.join([__name__, MyAppConfParser.__name__])
-    init_app_conf.initConfig(**{'default_parser_cls': class_name})
-
-    pytest.assume(init_app_conf.default_parser_cls == MyAppConfParser)
-
-
-
-@pytest.mark.parametrize(
-    'value, exp_value, exp_type',
-
-    [
-        ('John', 'John', str),
-        ('1000', '1000', str),
-        ('0.1', '0.1', str),
-        ('None', 'None', str),
-        ('True', 'True', str),
-        ('False', 'False', str),
-
-
-    ]
-)
-def test_mask_value_without_implicit_convert(request, initappconfFixture, value, exp_value, exp_type):
-    logger.info(f'{request._pyfuncitem.name}()')
-
-
-    result = mask_value(value, implicit_convert=False)
-    type_result = type(result)
-    pytest.assume(exp_value == result)
-    pytest.assume(exp_type == type_result)
-
-
-@pytest.mark.parametrize(
-     'value, exp_value, exp_type',
-
-    [
-        ('John', 'John', str),
-        ('alexber.utils.players.ConstantPlayer', 'alexber.utils.players.ConstantPlayer', str),
-        ('1000', 1000, int),
-        ('0.1', 0.1, float),
-        ('0.0', 0.0, float),
-        ('-0.0', 0.0, float),
-        ('-5', -5, int),
-        ('None', None, type(None)),
-        ('True', True, bool),
-        ('False', False, bool),
-
-
-
-    ]
-)
-def test_mask_value(request, initappconfFixture, value, exp_value, exp_type):
-    logger.info(f'{request._pyfuncitem.name}()')
-
-
-    result = mask_value(value)
-    type_result = type(result)
-    pytest.assume(exp_value == result)
-    pytest.assume(exp_type == type_result)
-
-def test_mask_value_default_as_true(request, initappconfFixture):
-    logger.info(f'{request._pyfuncitem.name}()')
-
-    value = '0.1'
-    exp_value = 0.1
-    exp_type = float
-
-    result = mask_value(value)  #implicit_convert=None as True
-    type_result = type(result)
-    pytest.assume(exp_value == result)
-    pytest.assume(exp_type == type_result)
-
-def test_mask_value_default_as_false(request, initappconfFalseFixture):
-    logger.info(f'{request._pyfuncitem.name}()')
-
-    value = '0.1'
-    exp_value = '0.1'
-    exp_type = str
-
-    result = mask_value(value)  #implicit_convert=None as False
-    type_result = type(result)
-    pytest.assume(exp_value == result)
-    pytest.assume(exp_type == type_result)
-
-
-
-
-def _calc_exp_ports(ports):
-    if ports is None:
-        return None
-    arr = str(ports).split(',')
-    ret=[mask_value(port) for port in arr]
-    return ret
-
-
-@pytest.mark.parametrize(
-     'value, exp_value',
-
-    [
-         (10000, [10000]),
-        ('10000', [10000]),
-        ('10000,', [10000, None]),
-        ('10000,10001',  [10000,10001]),
-        ('10000,10001,', [10000,10001, None]),
-        ('10000,,10003', [10000,None, 10003]),
-
-        (True, [True]),
-        (False, [False]),
-        ('True', [True]),
-        ('False', [False]),
-        ('False,True,False', [False,True,False]),
-
-        ([False], [False]), #Not_Supported
-        ([None], [None]), #Not_Supported
-        (['False'], [False]), #Not_Supported
-        (['None'], ['None']), #Not_Supported
-
-        ([None], ["innervalue"]),
-        ([''], ["innervalue"]),
-    ]
-)
-def test_merge_list_value_in_dicts(request, initappconfFixture, value, exp_value):
-    logger.info(f'{request._pyfuncitem.name}()')
-    if type(value) is list:
-        logger.debug(f"Complex types (such as list) are not supported.")
-        return
-
-    flat_d = OrderedDict()
-    flat_d['app.ports'] = value
-    d = OrderedDict()
-    inner_value = ["innervalue"]
-    d.setdefault('app', OrderedDict()).setdefault('ports', inner_value)
-
-    ret = merge_list_value_in_dicts(flat_d, d, 'app', 'ports', implicit_convert=True)
-    f_value = flat_d['app.ports']
-    i_value = d['app']['ports']
-
-    pytest.assume(value==f_value)
-    pytest.assume(inner_value==i_value)
-    pytest.assume(exp_value==ret)
-
-def test_merge_list_value_in_dicts_absent(request, initappconfFixture):
-    logger.info(f'{request._pyfuncitem.name}()')
-    flat_d = OrderedDict()
-    d = OrderedDict()
-    ret = merge_list_value_in_dicts(flat_d, d, 'general', 'profiles')
-    b = is_empty(ret)
-    pytest.assume(b)
-
-def test_merge_list_value_in_dicts_default_as_true(request, initappconfFixture):
-    logger.info(f'{request._pyfuncitem.name}()')
-
-    flat_d = {'app.ports': 10000}
-    d = {'app': {'ports': ["innervalue"]}}
-    inner_value = ["innervalue"]
-
-    ret = merge_list_value_in_dicts(flat_d, d, 'app', 'ports')
-    f_value = flat_d['app.ports']
-    i_value = d['app']['ports']
-
-    pytest.assume(10000==f_value)
-    pytest.assume(inner_value==i_value)
-    pytest.assume([10000]==ret)
-
-
-def test_merge_list_value_in_dicts_default_as_false(request, initappconfFalseFixture):
-    logger.info(f'{request._pyfuncitem.name}()')
-
-    flat_d = {'app.ports': 10000}
-    d = {'app': {'ports': ["innervalue"]}}
-    inner_value = ["innervalue"]
-
-    ret = merge_list_value_in_dicts(flat_d, d, 'app', 'ports')
-    f_value = flat_d['app.ports']
-    i_value = d['app']['ports']
-
-    pytest.assume(10000==f_value)
-    pytest.assume(inner_value==i_value)
-    pytest.assume(['10000']==ret)
-
-def test_merge_list_value_in_dicts_false(request, initappconfFixture):
-    logger.info(f'{request._pyfuncitem.name}()')
-
-    flat_d = {'app.ports': 10000}
-    d = {'app': {'ports': ["innervalue"]}}
-    inner_value = ["innervalue"]
-
-    ret = merge_list_value_in_dicts(flat_d, d, 'app', 'ports', implicit_convert=False)
-    f_value = flat_d['app.ports']
-    i_value = d['app']['ports']
-
-    pytest.assume(10000==f_value)
-    pytest.assume(inner_value==i_value)
-    pytest.assume(['10000']==ret)
-
-
-
-
-
-def check_exp_sys(exp_d, default_d):
-    general_d = default_d.get('general', None)
-    assert general_d is not None
-    app_d = default_d.get('app', None)
-    assert app_d is not None
-    app_str_d = app_d.get('as_str', None)
-    assert app_str_d is not None
-
-    exp_val = exp_d['general.profiles']
-    val = general_d.get('profiles', None)
-    pytest.assume(exp_val==val)
-
-    for flat_key, exp_val in exp_d.items():
-        if flat_key.startswith("general"):
-            continue
-        arr = flat_key.split('.')
-        key = arr[-1]
-        dd = app_str_d if 'as_str' in flat_key else app_d
-        val = dd.get(key, None)
-        pytest.assume(exp_val == val)
-
-
-def test_to_convex_map_intented(request, mocker, initappconfFixture):
-    logger.info(f'{request._pyfuncitem.name}()')
-    exp_d = {'general.profiles': ["dev"],
-             'app.white_list': ['one', 'two', 'three'],
-             'app.as_str.alt_white_list': [10],
-             'app.num_scalar': 5,
-             'app.none_scalar': None,
-             'app.str_scalar': 'Hello',
-             'app.as_str.bool1_scalar': True,
-             'app.as_str.bool2_scalar': False,
-
-             'app.as_str.list_bool': [True, False],
-             'app.as_str.list_bool_true': [True],
-             'app.as_str.list_bool_false': [False],
-             'app.as_str.list_none': [None],
-             'app.as_str.list_empty_str': [''],
-             }
-
-    sys_d = {'general.profiles': "dev",
-             'app.white_list': 'one,two,three',
-             'app.as_str.alt_white_list': '10',
-             'app.num_scalar': 5,
-             'app.none_scalar': None,
-             'app.str_scalar': 'Hello',
-             'app.as_str.bool1_scalar': 'True',
-             'app.as_str.bool2_scalar': 'False',
-
-             'app.as_str.list_bool': 'True,False',
-             'app.as_str.list_bool_true': True,
-             'app.as_str.list_bool_false': False,
-             'app.as_str.list_none': None,
-             'app.as_str.list_empty_str': '',
-             }
-    list_ensure = [key for key in sys_d.keys() if 'scalar' not in key]
-    create_default_parser()._do_ensure_list(sys_d, list_ensure)
-    default_d = to_convex_map(sys_d)
-
-    check_exp_sys(exp_d, default_d)
-
-
-
-def test_to_convex_map_whitelist(request, mocker, initappconfFixture):
-    logger.info(f'{request._pyfuncitem.name}()')
-    exp_d = {'general.profiles': ["dev"],
-             'app.as_str.alt_white_list': [10],
-             'app.as_str.bool1_scalar': True,
-             }
-
-    sys_d = {'general.profiles': "dev",
-             'app.white_list': 'one,two,three',
-             'app.as_str.alt_white_list': '10',
-             'app.as_str.bool1_scalar': 'True',
-             'db.unused': 'localhost',
-             }
-    list_ensure = [key for key in sys_d.keys() if 'scalar' not in key]
-    create_default_parser()._do_ensure_list(sys_d, list_ensure)
-    default_d = to_convex_map(sys_d, white_list_flat_keys=['general', 'app.as_str'], implicit_convert=True)
-
-    check_exp_sys(exp_d, default_d)
-
-def test_to_convex_map_whitelist_implicit_convert_false(request, mocker, initappconfFalseFixture):
-    logger.info(f'{request._pyfuncitem.name}()')
-    exp_d = {'general.profiles': ["dev"],
-             'app.as_str.alt_white_list': ['10'],
-             'app.as_str.bool1_scalar': 'True',
-             }
-
-    sys_d = {'general.profiles': "dev",
-             'app.white_list': 'one,two,three',
-             'app.as_str.alt_white_list': '10',
-             'app.as_str.bool1_scalar': 'True',
-             'db.unused': 'localhost',
-             }
-    list_ensure = [key for key in sys_d.keys() if 'scalar' not in key]
-    create_default_parser()._do_ensure_list(sys_d, list_ensure)
-    default_d = to_convex_map(sys_d, white_list_flat_keys=['general', 'app.as_str'], implicit_convert=False)
-
-    check_exp_sys(exp_d, default_d)
-
-def test_to_convex_map_whitelist_implicit_convert_false_default_as_false(request, mocker, initappconfFalseFixture):
-    logger.info(f'{request._pyfuncitem.name}()')
-    exp_d = {'general.profiles': ["dev"],
-             'app.as_str.alt_white_list': ['10'],
-             'app.as_str.bool1_scalar': 'True',
-             }
-
-    sys_d = {'general.profiles': "dev",
-             'app.white_list': 'one,two,three',
-             'app.as_str.alt_white_list': '10',
-             'app.as_str.bool1_scalar': 'True',
-             'db.unused': 'localhost',
-             }
-    list_ensure = [key for key in sys_d.keys() if 'scalar' not in key]
-    create_default_parser()._do_ensure_list(sys_d, list_ensure)
-    default_d = to_convex_map(sys_d, white_list_flat_keys=['general', 'app.as_str'], implicit_convert=False)
-
-    check_exp_sys(exp_d, default_d)
-
-def test_to_convex_map_whitelist_default_as_true(request, mocker, initappconfFixture):
-    logger.info(f'{request._pyfuncitem.name}()')
-    exp_d = {'general.profiles': ["dev"],
-             'app.as_str.alt_white_list': [10],
-             'app.as_str.bool1_scalar': True,
-             }
-
-    sys_d = {'general.profiles': "dev",
-             'app.white_list': 'one,two,three',
-             'app.as_str.alt_white_list': '10',
-             'app.as_str.bool1_scalar': 'True',
-             'db.unused': 'localhost',
-             }
-    list_ensure = [key for key in sys_d.keys() if 'scalar' not in key]
-    create_default_parser()._do_ensure_list(sys_d, list_ensure)
-    default_d = to_convex_map(sys_d, white_list_flat_keys=['general', 'app.as_str'])
-
-    check_exp_sys(exp_d, default_d)
-
-@pytest.mark.parametrize(
-     'exp_profiles, sys_d, default_d',
-    [
-        (['dev', 'local'], {'general.profiles': "dev,local"}, {'general': {'profiles': ["dev"]}}),
-        (['prod'], {'general.profiles': "prod"}, {'general': {'profiles': ["dev"]}}),
-        (['dev'], {}, {'general': {'profiles': ["dev"]}}),
-        (['prod'], {'general.profiles': "prod"}, {}),
-        (['prod'], {'general.profiles': "prod"}, {'general': {'profiles': None}}),
-        (['prod'], {'general.profiles': "prod"}, {'general': {'profiles': [""]}}),
-        ([None], {'general.profiles': None}, {'general': {'profiles': ["dev"]}}),
-        ([""], {'general.profiles': ""}, {'general': {'profiles': ["dev"]}}),
-        ([], {'general.log': "something"}, {'general': {'log': {'root': 'INFO'}}}), #it should be list, not dict
-    ]
-)
-def test_parse_profiles(request, mocker, initappconfFixture, exp_profiles, sys_d, default_d):
-    logger.info(f'{request._pyfuncitem.name}()')
-
-    profiles = create_default_parser()._parse_profiles(sys_d, default_d)
-    pytest.assume(exp_profiles == profiles)
-
-
-@pytest.mark.parametrize(
-     'exp_value, default_d',
-
-    [
-        (False, {'general': {'whiteListSysOverride': ["general,app"]}}),
-        (False, {'general': {'whiteListSysOverride': ["general"]}}),
-        (True, {'general': {'whiteListSysOverride': []}}),
-        (False, {'general': {'whiteListSysOverride': ['']}}),
-        (False, {'general': {'whiteListSysOverride': [None]}}),
-        (True, {'general': {'whiteListSysOverride': None}}),
-    ]
-
-)
-
-def test_parse_white_list_implicitely(request, mocker, initappconfFixture, exp_value, default_d):
-    logger.info(f'{request._pyfuncitem.name}()')
-    result = create_default_parser()._parse_white_list_implicitely(default_d)
-    pytest.assume(exp_value==result)
-
-
-
-
-@pytest.mark.parametrize(
-     'default_d',
-
-    [
-        {'general': {'profiles': ["dev"]}, 'some_unique_key': 'value'},
-        {'general': {'profiles': ["dev"], 'whiteListSysOverride':None}, 'some_unique_key': 'value'},
-        {'general': {'profiles': ["dev"], 'whiteListSysOverride':[]}, 'some_unique_key': 'value'},
-    ]
-
-)
-
-def test_parse_white_list_implicit(request, mocker, initappconfFixture, default_d):
-    logger.info(f'{request._pyfuncitem.name}()')
-    #whiteListSysOverride
-
-    white_list = create_default_parser()._parse_white_list(default_d)
-    length = 0 if white_list is None else len(white_list)
-    pytest.assume(length==2)
-    pytest.assume('general' in white_list)
-    pytest.assume('some_unique_key' in white_list)
-
-def test_parse_white_list_explicit(request, mocker, initappconfFixture):
-    logger.info(f'{request._pyfuncitem.name}()')
-    #whiteListSysOverride
-    default_d={'general': {'profiles': ["dev"], 'whiteListSysOverride': ['general']},
-               'app': {
-                   'ignoredKey': 1,
-               }}
-
-    white_list = create_default_parser()._parse_white_list(default_d)
-    length = 0 if white_list is None else len(white_list)
-    pytest.assume(length==1)
-    pytest.assume('general' in white_list)
-    pytest.assume('app' not in white_list)
-
-def test_parse_white_list_explicit2(request, initappconfFixture, mocker):
-    logger.info(f'{request._pyfuncitem.name}()')
-    #whiteListSysOverride
-
-    default_d={'general': {'profiles': ["dev"],
-                           'log': None,
-                           'whiteListSysOverride': ['general', 'app']},
-               'app': {
-                  'ignoredKey': 1,
-                }
-    }
-
-    white_list = create_default_parser()._parse_white_list(default_d)
-    length = 0 if white_list is None else len(white_list)
-    pytest.assume(length==2)
-    pytest.assume('general' in white_list)
-    pytest.assume('app' in white_list)
-
-
-def test_parse_list_ensure(request, mocker, initappconfFixture):
-    logger.info(f'{request._pyfuncitem.name}()')
-    sys_d = {}
-    default_d={'general': {'listEnsure': ['general.profiles', 'general.listEnsure',
-                                          'general.listEnsure', 'general.whiteListSysOverride',
-                                          'app.check_list']}}
-
-    list_ensure = create_default_parser()._parse_list_ensure(sys_d, default_d)
-    length = 0 if list_ensure is None else len(list_ensure)
-    pytest.assume(length==1)
-    pytest.assume('app.check_list' in list_ensure)
-
-
-def test_parse_list_ensure_empty(request, mocker, initappconfFixture):
-    logger.info(f'{request._pyfuncitem.name}()')
-    sys_d = {}
-    default_d={'general': {'listEnsure': []}}
-
-    list_ensure = create_default_parser()._parse_list_ensure(sys_d, default_d)
-    length = 0 if list_ensure is None else len(list_ensure)
-    pytest.assume(length==0)
-
-def test_parse_list_ensure2(request, mocker, initappconfFixture):
-    logger.info(f'{request._pyfuncitem.name}()')
-    sys_d = {'general.listEnsure':'general.profiles,app.white_list'}
-
-    default_d={'general': {'listEnsure': ['general.profiles', 'general.listEnsure',
-                                          'general.listEnsure', 'general.whiteListSysOverride',
-                                          'app.check_list']}}
-
-    list_ensure = create_default_parser()._parse_list_ensure(sys_d, default_d)
-    length = 0 if list_ensure is None else len(list_ensure)
-    pytest.assume(length==1)
-    pytest.assume('app.white_list' in list_ensure)
-
-def test_get_white_listed_empty_src_d(request, mocker, initappconfFixture):
-    logger.info(f'{request._pyfuncitem.name}()')
-    exp_d = {}
-    d = create_default_parser()._get_white_listed({}, {'a':'b'})
-    pytest.assume(exp_d==d)
-
-def test_get_white_listed_empty_white_list_flat_keys(request, mocker, initappconfFixture):
-    logger.info(f'{request._pyfuncitem.name}()')
-    exp_d = {'general.profiles': "dev",
-             'app.white_list': 'one,two,three',
-             'app.as_str.alt_white_list': '10',
-             'app.as_str.bool1_scalar': 'True',
-             'db.unused': 'localhost',
-             }
-
-    sys_d = {'general.profiles': "dev",
-             'app.white_list': 'one,two,three',
-             'app.as_str.alt_white_list': '10',
-             'app.as_str.bool1_scalar': 'True',
-             'db.unused': 'localhost',
-             }
-
-    d = create_default_parser()._get_white_listed(sys_d, None)
-    pytest.assume(exp_d==d)
-
-def test_get_white_listed(request, mocker, initappconfFixture):
-    logger.info(f'{request._pyfuncitem.name}()')
-    exp_d = {'general.profiles': "dev",
-             'app.white_list': 'one,two,three',
-             'app.as_str.alt_white_list': '10',
-             'app.as_str.bool1_scalar': 'True',
-             }
-
-    sys_d = {'general.profiles': "dev",
-             'app.white_list': 'one,two,three',
-             'app.as_str.alt_white_list': '10',
-             'app.as_str.bool1_scalar': 'True',
-             'db.unused': 'localhost',
-             }
-
-    white_list_flat_keys = ['app', 'general']
-
-    d = create_default_parser()._get_white_listed(sys_d, white_list_flat_keys)
-    pytest.assume(exp_d==d)
-
-@pytest.mark.yml
-def test_parse_sys_args(request, mocker, ymlparsersSetup, ymlparsersCleanup, initappconfFixture):
-    logger.info(f'{request._pyfuncitem.name}()')
-
-    expdd = {
-        'general': {'profiles': ['dev'],  # list
-                    'log': {
-                        'formatters': {
-                            'detail': {
-                                'format': '%(message)s'
-                            }
-                        },
-                        'root': {
-                            'level': 20  # logging.INFO
-                        }
-                    },
-                    'listEnsure': ['app.white_list','app.alt_white_list']
-                    },  # list
-        'app': {'host_name': 'yahoo.com',
-                'portal': 'reddit.com',     #this will be proceses because of implicit general.whiteListSysOverride
-                'white_list': ['alpha', 'betha', 'gamma'],
-                'alt_white_list': [],  # not part of sys.args, so value from config.yml will be ignored
-                }
-    }
-
-    pck = '.'.join(['tests_data', __package__, 'initappconf'])
-    with path(pck, 'config.yml') as full_path:
-        argsv = f'--general.config.file={full_path} '\
-                '--general.profiles=dev ' \
-                '--general.log.formatters.detail.format=%(message)s ' \
-                '--general.log.root.level=20 ' \
-                '--general.listEnsure=app.white_list,app.alt_white_list ' \
-                '--app.host_name=yahoo.com ' \
-                '--app.portal=reddit.com ' \
-                '--app.white_list=alpha,betha,gamma ' \
-            .split()
-
-
-        dd, profiles, _, list_ensure, _ = create_default_parser()._parse_sys_args(None, argsv)
-        dd['general']['profiles'] = profiles
-        dd['general']['listEnsure'] = list_ensure
-
-        pytest.assume(expdd==dd)
-
-@pytest.mark.yml
-def test_parse_yml(request, mocker, ymlparsersSetup, ymlparsersCleanup, initappconfFixture):
-    logger.info(f'{request._pyfuncitem.name}()')
-
-    expdd = {
-        'general': {'profiles': ['dev'],  # list
-                    'log': {
-                        'version': 1,
-                        'disable_existing_loggers': False,
-                        'formatters': {
-                            'brief': {
-                                'format': '%(message)s'
-                            },
-                            'detail': {
-                                'format': '%(asctime)-15s %(levelname)s [%(name)s.%(funcName)s] %(message)s',
-                                'datefmt': '%Y-%m-%d %H:%M:%S'
-                            },
-                        },
-                        'root': {
-                            'level': 'INFO'  # logging.INFO
-                        }
-                    },
-                    'listEnsure': ['app.white_list', 'app.alt_white_list']
-                    },  # list
-        'app': {'host_name': 'yahoo.com',
-                'portal': 'reddit.com',  # this will be proceses because of implicit general.whiteListSysOverride
-                'news': 'cnn.com',
-                'white_list': ['alpha', 'betha', 'gamma'],
-                'alt_white_list': [100, 10.0],  #value from config.yml will be parsed
-                }
-    }
-
-
-
-    sys_d = {
-        'general': {'profiles': ['dev'],
-                    'listEnsure': ['app.white_list','app.alt_white_list']
-                    },
-        'app': {'host_name': 'yahoo.com',
-                'portal': 'reddit.com',     #this will be proceses because of implicit general.whiteListSysOverride
-                'white_list': ['alpha', 'betha', 'gamma'],
-                }
-    }
-
-    pck = '.'.join(['tests_data', __package__, 'initappconf'])
-    with path(pck, 'config.yml') as full_path:
-        dd = create_default_parser()._parse_yml(sys_d, ['dev'], config_file=full_path)
-        del dd['general']['log']['handlers']
-        del dd['general']['log']['root']['handlers']
-        pytest.assume(expdd==dd)
-
-@pytest.mark.yml
-def test_parse_config_true(request, mocker, ymlparsersSetup, ymlparsersCleanup, initappconfFixture):
-    logger.info(f'{request._pyfuncitem.name}()')
-
-    expdd = {
-        'general': {'profiles': ['dev'],
-                    'log': {
-                        'version': 1,
-                        'disable_existing_loggers': False,
-                        'formatters': {
-                            'brief': {
-                                'format': '%(message)s'
-                            },
-                            'detail': {
-                                'format': '%(asctime)-15s %(levelname)s [%(name)s.%(funcName)s] %(message)s',
-                                'datefmt': '%Y-%m-%d %H:%M:%S'
-                            },
-                        },
-                        'root': {
-                            'level': 'INFO'  # logging.INFO
-                        }
-                    },
-                    'config':{
-                        'file' : None   #will be be populated below
-                    },
-                    'whiteListSysOverride': ['general', 'app'],   #implictely populated
-                    'listEnsure': [],   #profile can be overridden in sysargs, regargless,  \
-                                        # we don't override any (other) list value from sysargs
-                    },  # list
-        'app': {'host_name': 'yahoo.com',
-                'news': 'cnn.com',
-                'portal': 'reddit.com',     #this will be proceses because of implicit general.whiteListSysOverride
-                'white_list': ['gamma', 'alpha', 'betha'],
-                'alt_white_list': [100, 10.0],
-                }
-    }
-
-    pck = '.'.join(['tests_data', __package__, 'initappconf'])
-
-    with path(pck, 'config.yml') as full_path:
-        expdd['general']['config']['file'] = str(full_path)
-
-        argsv = f'--general.config.file={full_path} '\
-                '--app.portal=reddit.com ' \
-                '--general.profiles=dev ' \
-            .split()
-
-
-        dd = parse_config(None, argsv)
-        del dd['general']['log']['handlers']
-        del dd['general']['log']['root']['handlers']
-
-        pytest.assume(expdd==dd)
-
-@pytest.mark.yml
-def test_parse_config_explicit_white_list(request, mocker, ymlparsersSetup, ymlparsersCleanup, initappconfFixture):
-    logger.info(f'{request._pyfuncitem.name}()')
-
-    expdd = {
-        'general': {'profiles': [],
-                    'log': {
-                        'version': 1,
-                        'disable_existing_loggers': False,
-                        'formatters': {
-                            'brief': {
-                                'format': '%(message)s'
-                            },
-                            'detail': {
-                                'format': '%(asctime)-15s %(levelname)s [%(name)s.%(funcName)s] %(message)s',
-                                'datefmt': '%Y-%m-%d %H:%M:%S'
-                            },
-                        },
-                        'root': {
-                            'level': 'DEBUG'
-                        }
-                    },
-                    'config':{
-                        'file' : None   #will be be populated below
-                    },
-                    'whiteListSysOverride': ['app.host_name'],   #explicetly populated
-                    'listEnsure': [],   #whiteListSysOverride can be overridden in sysargs, regargless,  \
-                                        # we don't override any (other) list value from sysargs
-                    },  # list
-        'app': {'host_name': '10.20.40.60',
-                'news': 'cnn.com',
-                #'portal': 'reddit.com',     #this will NOT be proceses because of explicit general.whiteListSysOverride
-                'white_list': ['gamma', 'alpha', 'betha'],
-                'alt_white_list': [100, 10.0],
-                }
-    }
-
-    pck = '.'.join(['tests_data', __package__, 'initappconf'])
-
-    with path(pck, 'confige.yml') as full_path:
-        expdd['general']['config']['file'] = str(full_path)
-
-        #app.host_name is in general.whiteListSysOverridem it will be process
-        #app.portal and last line will be ignored
-        argsv = f'--general.config.file={full_path} '\
-                '--app.portal=reddit.com ' \
-                '--app.host_name=10.20.40.60 ' \
-                '10.20.40.60:8082 ' \
-            .split()
-
-
-        dd = parse_config(None, argsv)
-        del dd['general']['log']['handlers']
-        del dd['general']['log']['root']['handlers']
-
-        pytest.assume(expdd==dd)
-
-@pytest.mark.yml
-def test_parse_config_false(request, mocker, ymlparsersSetup, ymlparsersCleanup, initappconfFixture):
-    logger.info(f'{request._pyfuncitem.name}()')
-    pck = '.'.join(['tests_data', __package__, 'initappconf'])
-    exp_disable_existing_loggers = 'False'
-
-    with path(pck, 'config.yml') as full_path:
-        argsv = f'--general.config.file={full_path} ' \
-                '--general.profiles=dev ' \
-                f'--general.log.disable_existing_loggers={exp_disable_existing_loggers} ' \
-            .split()
-
-        dd = parse_config(None, argsv, implicit_convert=False)
-        disable_existing_loggers = dd['general']['log']['disable_existing_loggers']
-        pytest.assume(exp_disable_existing_loggers==disable_existing_loggers)
-
-@pytest.mark.yml
-def test_parse_config_default_as_false(request, mocker, ymlparsersSetup, ymlparsersCleanup, initappconfFalseFixture):
-    logger.info(f'{request._pyfuncitem.name}()')
-    pck = '.'.join(['tests_data', __package__, 'initappconf'])
-    exp_disable_existing_loggers = 'False'
-
-    with path(pck, 'config.yml') as full_path:
-        argsv = f'--general.config.file={full_path} ' \
-                '--general.profiles=dev ' \
-                f'--general.log.disable_existing_loggers={exp_disable_existing_loggers} ' \
-            .split()
-
-        dd = parse_config(None, argsv)
-        disable_existing_loggers = dd['general']['log']['disable_existing_loggers']
-        pytest.assume(exp_disable_existing_loggers==disable_existing_loggers)
-
-@pytest.mark.yml
-def test_parse_config_default_as_true(request, mocker, ymlparsersSetup, ymlparsersCleanup, initappconfFixture):
-    logger.info(f'{request._pyfuncitem.name}()')
-    pck = '.'.join(['tests_data', __package__, 'initappconf'])
-    exp_disable_existing_loggers = False
-
-    with path(pck, 'config.yml') as full_path:
-        argsv = f'--general.config.file={full_path} ' \
-                '--general.profiles=dev ' \
-                f'--general.log.disable_existing_loggers={exp_disable_existing_loggers} ' \
-            .split()
-
-        dd = parse_config(None, argsv)
-        disable_existing_loggers = dd['general']['log']['disable_existing_loggers']
-        pytest.assume(exp_disable_existing_loggers==disable_existing_loggers)
-
-
-
-if __name__ == "__main__":
-    pytest.main([__file__])
-
-
+import logging
+from collections import OrderedDict
+from collections.abc import Mapping
+import pytest
+import copy
+
+logger = logging.getLogger(__name__)
+from alexber.utils.init_app_conf import mask_value, merge_list_value_in_dicts, to_convex_map, \
+    parse_config
+import alexber.utils.init_app_conf as init_app_conf
+from alexber.utils.init_app_conf import _create_default_parser, AppConfParser
+from alexber.utils.parsers import is_empty
+from tests.utils.ymlparsers_test import ymlparsersSetup, ymlparsersCleanup, exp_config_d
+from importlib.resources import path
+
+def create_default_parser(implicit_convert=None):
+    parser=_create_default_parser(**{'implicit_convert': implicit_convert})
+    return parser
+
+def _reset_initappconf():
+    init_app_conf.default_parser_cls  = None
+    init_app_conf.default_parser_kwargs = None
+
+
+
+@pytest.fixture
+def initappconfFixture(mocker):
+    _reset_initappconf()
+
+    init_app_conf.initConfig()
+    yield None
+    _reset_initappconf()
+
+@pytest.fixture
+def initappconfFalseFixture(mocker):
+    _reset_initappconf()
+
+    init_app_conf.initConfig(**{'default_parser_kwargs': {'implicit_convert': False}})
+    yield None
+    _reset_initappconf()
+
+
+
+class MyAppConfParser(AppConfParser):
+    pass
+
+def test_mask_value_default_as_none(request, initappconfFalseFixture):
+    logger.info(f'{request._pyfuncitem.name}()')
+
+    with pytest.raises(ValueError, match='None'):
+        init_app_conf.initConfig(**{'default_parser_kwargs': {'implicit_convert': None}})
+        mask_value('0.1')
+
+def test_initConfig_default_parser_cls_str(request, initappconfFalseFixture):
+    logger.info(f'{request._pyfuncitem.name}()')
+
+    class_name = '.'.join([__name__, MyAppConfParser.__name__])
+    init_app_conf.initConfig(**{'default_parser_cls': class_name})
+
+    pytest.assume(init_app_conf.default_parser_cls == MyAppConfParser)
+
+
+
+@pytest.mark.parametrize(
+    'value, exp_value, exp_type',
+
+    [
+        ('John', 'John', str),
+        ('1000', '1000', str),
+        ('0.1', '0.1', str),
+        ('None', 'None', str),
+        ('True', 'True', str),
+        ('False', 'False', str),
+
+
+    ]
+)
+def test_mask_value_without_implicit_convert(request, initappconfFixture, value, exp_value, exp_type):
+    logger.info(f'{request._pyfuncitem.name}()')
+
+
+    result = mask_value(value, implicit_convert=False)
+    type_result = type(result)
+    pytest.assume(exp_value == result)
+    pytest.assume(exp_type == type_result)
+
+
+@pytest.mark.parametrize(
+     'value, exp_value, exp_type',
+
+    [
+        ('John', 'John', str),
+        ('alexber.utils.players.ConstantPlayer', 'alexber.utils.players.ConstantPlayer', str),
+        ('1000', 1000, int),
+        ('0.1', 0.1, float),
+        ('0.0', 0.0, float),
+        ('-0.0', 0.0, float),
+        ('-5', -5, int),
+        ('None', None, type(None)),
+        ('True', True, bool),
+        ('False', False, bool),
+
+
+
+    ]
+)
+def test_mask_value(request, initappconfFixture, value, exp_value, exp_type):
+    logger.info(f'{request._pyfuncitem.name}()')
+
+
+    result = mask_value(value)
+    type_result = type(result)
+    pytest.assume(exp_value == result)
+    pytest.assume(exp_type == type_result)
+
+def test_mask_value_default_as_true(request, initappconfFixture):
+    logger.info(f'{request._pyfuncitem.name}()')
+
+    value = '0.1'
+    exp_value = 0.1
+    exp_type = float
+
+    result = mask_value(value)  #implicit_convert=None as True
+    type_result = type(result)
+    pytest.assume(exp_value == result)
+    pytest.assume(exp_type == type_result)
+
+def test_mask_value_default_as_false(request, initappconfFalseFixture):
+    logger.info(f'{request._pyfuncitem.name}()')
+
+    value = '0.1'
+    exp_value = '0.1'
+    exp_type = str
+
+    result = mask_value(value)  #implicit_convert=None as False
+    type_result = type(result)
+    pytest.assume(exp_value == result)
+    pytest.assume(exp_type == type_result)
+
+
+
+
+def _calc_exp_ports(ports):
+    if ports is None:
+        return None
+    arr = str(ports).split(',')
+    ret=[mask_value(port) for port in arr]
+    return ret
+
+
+@pytest.mark.parametrize(
+     'value, exp_value',
+
+    [
+         (10000, [10000]),
+        ('10000', [10000]),
+        ('10000,', [10000, None]),
+        ('10000,10001',  [10000,10001]),
+        ('10000,10001,', [10000,10001, None]),
+        ('10000,,10003', [10000,None, 10003]),
+
+        (True, [True]),
+        (False, [False]),
+        ('True', [True]),
+        ('False', [False]),
+        ('False,True,False', [False,True,False]),
+
+        ([False], [False]), #Not_Supported
+        ([None], [None]), #Not_Supported
+        (['False'], [False]), #Not_Supported
+        (['None'], ['None']), #Not_Supported
+
+        ([None], ["innervalue"]),
+        ([''], ["innervalue"]),
+    ]
+)
+def test_merge_list_value_in_dicts(request, initappconfFixture, value, exp_value):
+    logger.info(f'{request._pyfuncitem.name}()')
+    if type(value) is list:
+        logger.debug(f"Complex types (such as list) are not supported.")
+        return
+
+    flat_d = OrderedDict()
+    flat_d['app.ports'] = value
+    d = OrderedDict()
+    inner_value = ["innervalue"]
+    d.setdefault('app', OrderedDict()).setdefault('ports', inner_value)
+
+    ret = merge_list_value_in_dicts(flat_d, d, 'app', 'ports', implicit_convert=True)
+    f_value = flat_d['app.ports']
+    i_value = d['app']['ports']
+
+    pytest.assume(value==f_value)
+    pytest.assume(inner_value==i_value)
+    pytest.assume(exp_value==ret)
+
+def test_merge_list_value_in_dicts_absent(request, initappconfFixture):
+    logger.info(f'{request._pyfuncitem.name}()')
+    flat_d = OrderedDict()
+    d = OrderedDict()
+    ret = merge_list_value_in_dicts(flat_d, d, 'general', 'profiles')
+    b = is_empty(ret)
+    pytest.assume(b)
+
+def test_merge_list_value_in_dicts_default_as_true(request, initappconfFixture):
+    logger.info(f'{request._pyfuncitem.name}()')
+
+    flat_d = {'app.ports': 10000}
+    d = {'app': {'ports': ["innervalue"]}}
+    inner_value = ["innervalue"]
+
+    ret = merge_list_value_in_dicts(flat_d, d, 'app', 'ports')
+    f_value = flat_d['app.ports']
+    i_value = d['app']['ports']
+
+    pytest.assume(10000==f_value)
+    pytest.assume(inner_value==i_value)
+    pytest.assume([10000]==ret)
+
+
+def test_merge_list_value_in_dicts_default_as_false(request, initappconfFalseFixture):
+    logger.info(f'{request._pyfuncitem.name}()')
+
+    flat_d = {'app.ports': 10000}
+    d = {'app': {'ports': ["innervalue"]}}
+    inner_value = ["innervalue"]
+
+    ret = merge_list_value_in_dicts(flat_d, d, 'app', 'ports')
+    f_value = flat_d['app.ports']
+    i_value = d['app']['ports']
+
+    pytest.assume(10000==f_value)
+    pytest.assume(inner_value==i_value)
+    pytest.assume(['10000']==ret)
+
+def test_merge_list_value_in_dicts_false(request, initappconfFixture):
+    logger.info(f'{request._pyfuncitem.name}()')
+
+    flat_d = {'app.ports': 10000}
+    d = {'app': {'ports': ["innervalue"]}}
+    inner_value = ["innervalue"]
+
+    ret = merge_list_value_in_dicts(flat_d, d, 'app', 'ports', implicit_convert=False)
+    f_value = flat_d['app.ports']
+    i_value = d['app']['ports']
+
+    pytest.assume(10000==f_value)
+    pytest.assume(inner_value==i_value)
+    pytest.assume(['10000']==ret)
+
+
+
+
+
+def check_exp_sys(exp_d, default_d):
+    general_d = default_d.get('general', None)
+    assert general_d is not None
+    app_d = default_d.get('app', None)
+    assert app_d is not None
+    app_str_d = app_d.get('as_str', None)
+    assert app_str_d is not None
+
+    exp_val = exp_d['general.profiles']
+    val = general_d.get('profiles', None)
+    pytest.assume(exp_val==val)
+
+    for flat_key, exp_val in exp_d.items():
+        if flat_key.startswith("general"):
+            continue
+        arr = flat_key.split('.')
+        key = arr[-1]
+        dd = app_str_d if 'as_str' in flat_key else app_d
+        val = dd.get(key, None)
+        pytest.assume(exp_val == val)
+
+
+def test_to_convex_map_intented(request, mocker, initappconfFixture):
+    logger.info(f'{request._pyfuncitem.name}()')
+    exp_d = {'general.profiles': ["dev"],
+             'app.white_list': ['one', 'two', 'three'],
+             'app.as_str.alt_white_list': [10],
+             'app.num_scalar': 5,
+             'app.none_scalar': None,
+             'app.str_scalar': 'Hello',
+             'app.as_str.bool1_scalar': True,
+             'app.as_str.bool2_scalar': False,
+
+             'app.as_str.list_bool': [True, False],
+             'app.as_str.list_bool_true': [True],
+             'app.as_str.list_bool_false': [False],
+             'app.as_str.list_none': [None],
+             'app.as_str.list_empty_str': [''],
+             }
+
+    sys_d = {'general.profiles': "dev",
+             'app.white_list': 'one,two,three',
+             'app.as_str.alt_white_list': '10',
+             'app.num_scalar': 5,
+             'app.none_scalar': None,
+             'app.str_scalar': 'Hello',
+             'app.as_str.bool1_scalar': 'True',
+             'app.as_str.bool2_scalar': 'False',
+
+             'app.as_str.list_bool': 'True,False',
+             'app.as_str.list_bool_true': True,
+             'app.as_str.list_bool_false': False,
+             'app.as_str.list_none': None,
+             'app.as_str.list_empty_str': '',
+             }
+    list_ensure = [key for key in sys_d.keys() if 'scalar' not in key]
+    create_default_parser()._do_ensure_list(sys_d, list_ensure)
+    default_d = to_convex_map(sys_d)
+
+    check_exp_sys(exp_d, default_d)
+
+
+
+def test_to_convex_map_whitelist(request, mocker, initappconfFixture):
+    logger.info(f'{request._pyfuncitem.name}()')
+    exp_d = {'general.profiles': ["dev"],
+             'app.as_str.alt_white_list': [10],
+             'app.as_str.bool1_scalar': True,
+             }
+
+    sys_d = {'general.profiles': "dev",
+             'app.white_list': 'one,two,three',
+             'app.as_str.alt_white_list': '10',
+             'app.as_str.bool1_scalar': 'True',
+             'db.unused': 'localhost',
+             }
+    list_ensure = [key for key in sys_d.keys() if 'scalar' not in key]
+    create_default_parser()._do_ensure_list(sys_d, list_ensure)
+    default_d = to_convex_map(sys_d, white_list_flat_keys=['general', 'app.as_str'], implicit_convert=True)
+
+    check_exp_sys(exp_d, default_d)
+
+def test_to_convex_map_whitelist_implicit_convert_false(request, mocker, initappconfFalseFixture):
+    logger.info(f'{request._pyfuncitem.name}()')
+    exp_d = {'general.profiles': ["dev"],
+             'app.as_str.alt_white_list': ['10'],
+             'app.as_str.bool1_scalar': 'True',
+             }
+
+    sys_d = {'general.profiles': "dev",
+             'app.white_list': 'one,two,three',
+             'app.as_str.alt_white_list': '10',
+             'app.as_str.bool1_scalar': 'True',
+             'db.unused': 'localhost',
+             }
+    list_ensure = [key for key in sys_d.keys() if 'scalar' not in key]
+    create_default_parser()._do_ensure_list(sys_d, list_ensure)
+    default_d = to_convex_map(sys_d, white_list_flat_keys=['general', 'app.as_str'], implicit_convert=False)
+
+    check_exp_sys(exp_d, default_d)
+
+def test_to_convex_map_whitelist_implicit_convert_false_default_as_false(request, mocker, initappconfFalseFixture):
+    logger.info(f'{request._pyfuncitem.name}()')
+    exp_d = {'general.profiles': ["dev"],
+             'app.as_str.alt_white_list': ['10'],
+             'app.as_str.bool1_scalar': 'True',
+             }
+
+    sys_d = {'general.profiles': "dev",
+             'app.white_list': 'one,two,three',
+             'app.as_str.alt_white_list': '10',
+             'app.as_str.bool1_scalar': 'True',
+             'db.unused': 'localhost',
+             }
+    list_ensure = [key for key in sys_d.keys() if 'scalar' not in key]
+    create_default_parser()._do_ensure_list(sys_d, list_ensure)
+    default_d = to_convex_map(sys_d, white_list_flat_keys=['general', 'app.as_str'], implicit_convert=False)
+
+    check_exp_sys(exp_d, default_d)
+
+def test_to_convex_map_whitelist_default_as_true(request, mocker, initappconfFixture):
+    logger.info(f'{request._pyfuncitem.name}()')
+    exp_d = {'general.profiles': ["dev"],
+             'app.as_str.alt_white_list': [10],
+             'app.as_str.bool1_scalar': True,
+             }
+
+    sys_d = {'general.profiles': "dev",
+             'app.white_list': 'one,two,three',
+             'app.as_str.alt_white_list': '10',
+             'app.as_str.bool1_scalar': 'True',
+             'db.unused': 'localhost',
+             }
+    list_ensure = [key for key in sys_d.keys() if 'scalar' not in key]
+    create_default_parser()._do_ensure_list(sys_d, list_ensure)
+    default_d = to_convex_map(sys_d, white_list_flat_keys=['general', 'app.as_str'])
+
+    check_exp_sys(exp_d, default_d)
+
+@pytest.mark.parametrize(
+     'exp_profiles, sys_d, default_d',
+    [
+        (['dev', 'local'], {'general.profiles': "dev,local"}, {'general': {'profiles': ["dev"]}}),
+        (['prod'], {'general.profiles': "prod"}, {'general': {'profiles': ["dev"]}}),
+        (['dev'], {}, {'general': {'profiles': ["dev"]}}),
+        (['prod'], {'general.profiles': "prod"}, {}),
+        (['prod'], {'general.profiles': "prod"}, {'general': {'profiles': None}}),
+        (['prod'], {'general.profiles': "prod"}, {'general': {'profiles': [""]}}),
+        ([None], {'general.profiles': None}, {'general': {'profiles': ["dev"]}}),
+        ([""], {'general.profiles': ""}, {'general': {'profiles': ["dev"]}}),
+        ([], {'general.log': "something"}, {'general': {'log': {'root': 'INFO'}}}), #it should be list, not dict
+    ]
+)
+def test_parse_profiles(request, mocker, initappconfFixture, exp_profiles, sys_d, default_d):
+    logger.info(f'{request._pyfuncitem.name}()')
+
+    profiles = create_default_parser()._parse_profiles(sys_d, default_d)
+    pytest.assume(exp_profiles == profiles)
+
+
+@pytest.mark.parametrize(
+     'exp_value, default_d',
+
+    [
+        (False, {'general': {'whiteListSysOverride': ["general,app"]}}),
+        (False, {'general': {'whiteListSysOverride': ["general"]}}),
+        (True, {'general': {'whiteListSysOverride': []}}),
+        (False, {'general': {'whiteListSysOverride': ['']}}),
+        (False, {'general': {'whiteListSysOverride': [None]}}),
+        (True, {'general': {'whiteListSysOverride': None}}),
+    ]
+
+)
+
+def test_parse_white_list_implicitely(request, mocker, initappconfFixture, exp_value, default_d):
+    logger.info(f'{request._pyfuncitem.name}()')
+    result = create_default_parser()._parse_white_list_implicitely(default_d)
+    pytest.assume(exp_value==result)
+
+
+
+
+@pytest.mark.parametrize(
+     'default_d',
+
+    [
+        {'general': {'profiles': ["dev"]}, 'some_unique_key': 'value'},
+        {'general': {'profiles': ["dev"], 'whiteListSysOverride':None}, 'some_unique_key': 'value'},
+        {'general': {'profiles': ["dev"], 'whiteListSysOverride':[]}, 'some_unique_key': 'value'},
+    ]
+
+)
+
+def test_parse_white_list_implicit(request, mocker, initappconfFixture, default_d):
+    logger.info(f'{request._pyfuncitem.name}()')
+    #whiteListSysOverride
+
+    white_list = create_default_parser()._parse_white_list(default_d)
+    length = 0 if white_list is None else len(white_list)
+    pytest.assume(length==2)
+    pytest.assume('general' in white_list)
+    pytest.assume('some_unique_key' in white_list)
+
+def test_parse_white_list_explicit(request, mocker, initappconfFixture):
+    logger.info(f'{request._pyfuncitem.name}()')
+    #whiteListSysOverride
+    default_d={'general': {'profiles': ["dev"], 'whiteListSysOverride': ['general']},
+               'app': {
+                   'ignoredKey': 1,
+               }}
+
+    white_list = create_default_parser()._parse_white_list(default_d)
+    length = 0 if white_list is None else len(white_list)
+    pytest.assume(length==1)
+    pytest.assume('general' in white_list)
+    pytest.assume('app' not in white_list)
+
+def test_parse_white_list_explicit2(request, initappconfFixture, mocker):
+    logger.info(f'{request._pyfuncitem.name}()')
+    #whiteListSysOverride
+
+    default_d={'general': {'profiles': ["dev"],
+                           'log': None,
+                           'whiteListSysOverride': ['general', 'app']},
+               'app': {
+                  'ignoredKey': 1,
+                }
+    }
+
+    white_list = create_default_parser()._parse_white_list(default_d)
+    length = 0 if white_list is None else len(white_list)
+    pytest.assume(length==2)
+    pytest.assume('general' in white_list)
+    pytest.assume('app' in white_list)
+
+
+def test_parse_list_ensure(request, mocker, initappconfFixture):
+    logger.info(f'{request._pyfuncitem.name}()')
+    sys_d = {}
+    default_d={'general': {'listEnsure': ['general.profiles', 'general.listEnsure',
+                                          'general.listEnsure', 'general.whiteListSysOverride',
+                                          'app.check_list']}}
+
+    list_ensure = create_default_parser()._parse_list_ensure(sys_d, default_d)
+    length = 0 if list_ensure is None else len(list_ensure)
+    pytest.assume(length==1)
+    pytest.assume('app.check_list' in list_ensure)
+
+
+def test_parse_list_ensure_empty(request, mocker, initappconfFixture):
+    logger.info(f'{request._pyfuncitem.name}()')
+    sys_d = {}
+    default_d={'general': {'listEnsure': []}}
+
+    list_ensure = create_default_parser()._parse_list_ensure(sys_d, default_d)
+    length = 0 if list_ensure is None else len(list_ensure)
+    pytest.assume(length==0)
+
+def test_parse_list_ensure2(request, mocker, initappconfFixture):
+    logger.info(f'{request._pyfuncitem.name}()')
+    sys_d = {'general.listEnsure':'general.profiles,app.white_list'}
+
+    default_d={'general': {'listEnsure': ['general.profiles', 'general.listEnsure',
+                                          'general.listEnsure', 'general.whiteListSysOverride',
+                                          'app.check_list']}}
+
+    list_ensure = create_default_parser()._parse_list_ensure(sys_d, default_d)
+    length = 0 if list_ensure is None else len(list_ensure)
+    pytest.assume(length==1)
+    pytest.assume('app.white_list' in list_ensure)
+
+def test_get_white_listed_empty_src_d(request, mocker, initappconfFixture):
+    logger.info(f'{request._pyfuncitem.name}()')
+    exp_d = {}
+    d = create_default_parser()._get_white_listed({}, {'a':'b'})
+    pytest.assume(exp_d==d)
+
+def test_get_white_listed_empty_white_list_flat_keys(request, mocker, initappconfFixture):
+    logger.info(f'{request._pyfuncitem.name}()')
+    exp_d = {'general.profiles': "dev",
+             'app.white_list': 'one,two,three',
+             'app.as_str.alt_white_list': '10',
+             'app.as_str.bool1_scalar': 'True',
+             'db.unused': 'localhost',
+             }
+
+    sys_d = {'general.profiles': "dev",
+             'app.white_list': 'one,two,three',
+             'app.as_str.alt_white_list': '10',
+             'app.as_str.bool1_scalar': 'True',
+             'db.unused': 'localhost',
+             }
+
+    d = create_default_parser()._get_white_listed(sys_d, None)
+    pytest.assume(exp_d==d)
+
+def test_get_white_listed(request, mocker, initappconfFixture):
+    logger.info(f'{request._pyfuncitem.name}()')
+    exp_d = {'general.profiles': "dev",
+             'app.white_list': 'one,two,three',
+             'app.as_str.alt_white_list': '10',
+             'app.as_str.bool1_scalar': 'True',
+             }
+
+    sys_d = {'general.profiles': "dev",
+             'app.white_list': 'one,two,three',
+             'app.as_str.alt_white_list': '10',
+             'app.as_str.bool1_scalar': 'True',
+             'db.unused': 'localhost',
+             }
+
+    white_list_flat_keys = ['app', 'general']
+
+    d = create_default_parser()._get_white_listed(sys_d, white_list_flat_keys)
+    pytest.assume(exp_d==d)
+
+@pytest.mark.yml
+def test_parse_sys_args(request, mocker, ymlparsersSetup, ymlparsersCleanup, initappconfFixture):
+    logger.info(f'{request._pyfuncitem.name}()')
+
+    expdd = {
+        'general': {'profiles': ['dev'],  # list
+                    'log': {
+                        'formatters': {
+                            'detail': {
+                                'format': '%(message)s'
+                            }
+                        },
+                        'root': {
+                            'level': 20  # logging.INFO
+                        }
+                    },
+                    'listEnsure': ['app.white_list','app.alt_white_list']
+                    },  # list
+        'app': {'host_name': 'yahoo.com',
+                'portal': 'reddit.com',     #this will be proceses because of implicit general.whiteListSysOverride
+                'white_list': ['alpha', 'betha', 'gamma'],
+                'alt_white_list': [],  # not part of sys.args, so value from config.yml will be ignored
+                }
+    }
+
+    pck = '.'.join(['tests_data', __package__, 'initappconf'])
+    with path(pck, 'config.yml') as full_path:
+        argsv = f'--general.config.file={full_path} '\
+                '--general.profiles=dev ' \
+                '--general.log.formatters.detail.format=%(message)s ' \
+                '--general.log.root.level=20 ' \
+                '--general.listEnsure=app.white_list,app.alt_white_list ' \
+                '--app.host_name=yahoo.com ' \
+                '--app.portal=reddit.com ' \
+                '--app.white_list=alpha,betha,gamma ' \
+            .split()
+
+
+        dd, profiles, _, list_ensure, _ = create_default_parser()._parse_sys_args(None, argsv)
+        dd['general']['profiles'] = profiles
+        dd['general']['listEnsure'] = list_ensure
+
+        pytest.assume(expdd==dd)
+
+@pytest.mark.yml
+def test_parse_yml(request, mocker, ymlparsersSetup, ymlparsersCleanup, initappconfFixture):
+    logger.info(f'{request._pyfuncitem.name}()')
+
+    expdd = {
+        'general': {'profiles': ['dev'],  # list
+                    'log': {
+                        'version': 1,
+                        'disable_existing_loggers': False,
+                        'formatters': {
+                            'brief': {
+                                'format': '%(message)s'
+                            },
+                            'detail': {
+                                'format': '%(asctime)-15s %(levelname)s [%(name)s.%(funcName)s] %(message)s',
+                                'datefmt': '%Y-%m-%d %H:%M:%S'
+                            },
+                        },
+                        'root': {
+                            'level': 'INFO'  # logging.INFO
+                        }
+                    },
+                    'listEnsure': ['app.white_list', 'app.alt_white_list']
+                    },  # list
+        'app': {'host_name': 'yahoo.com',
+                'portal': 'reddit.com',  # this will be proceses because of implicit general.whiteListSysOverride
+                'news': 'cnn.com',
+                'white_list': ['alpha', 'betha', 'gamma'],
+                'alt_white_list': [100, 10.0],  #value from config.yml will be parsed
+                }
+    }
+
+
+
+    sys_d = {
+        'general': {'profiles': ['dev'],
+                    'listEnsure': ['app.white_list','app.alt_white_list']
+                    },
+        'app': {'host_name': 'yahoo.com',
+                'portal': 'reddit.com',     #this will be proceses because of implicit general.whiteListSysOverride
+                'white_list': ['alpha', 'betha', 'gamma'],
+                }
+    }
+
+    pck = '.'.join(['tests_data', __package__, 'initappconf'])
+    with path(pck, 'config.yml') as full_path:
+        dd = create_default_parser()._parse_yml(sys_d, ['dev'], config_file=full_path)
+        del dd['general']['log']['handlers']
+        del dd['general']['log']['root']['handlers']
+        pytest.assume(expdd==dd)
+
+@pytest.mark.yml
+def test_parse_config_true(request, mocker, ymlparsersSetup, ymlparsersCleanup, initappconfFixture):
+    logger.info(f'{request._pyfuncitem.name}()')
+
+    expdd = {
+        'general': {'profiles': ['dev'],
+                    'log': {
+                        'version': 1,
+                        'disable_existing_loggers': False,
+                        'formatters': {
+                            'brief': {
+                                'format': '%(message)s'
+                            },
+                            'detail': {
+                                'format': '%(asctime)-15s %(levelname)s [%(name)s.%(funcName)s] %(message)s',
+                                'datefmt': '%Y-%m-%d %H:%M:%S'
+                            },
+                        },
+                        'root': {
+                            'level': 'INFO'  # logging.INFO
+                        }
+                    },
+                    'config':{
+                        'file' : None   #will be be populated below
+                    },
+                    'whiteListSysOverride': ['general', 'app'],   #implictely populated
+                    'listEnsure': [],   #profile can be overridden in sysargs, regargless,  \
+                                        # we don't override any (other) list value from sysargs
+                    },  # list
+        'app': {'host_name': 'yahoo.com',
+                'news': 'cnn.com',
+                'portal': 'reddit.com',     #this will be proceses because of implicit general.whiteListSysOverride
+                'white_list': ['gamma', 'alpha', 'betha'],
+                'alt_white_list': [100, 10.0],
+                }
+    }
+
+    pck = '.'.join(['tests_data', __package__, 'initappconf'])
+
+    with path(pck, 'config.yml') as full_path:
+        expdd['general']['config']['file'] = str(full_path)
+
+        argsv = f'--general.config.file={full_path} '\
+                '--app.portal=reddit.com ' \
+                '--general.profiles=dev ' \
+            .split()
+
+
+        dd = parse_config(None, argsv)
+        del dd['general']['log']['handlers']
+        del dd['general']['log']['root']['handlers']
+
+        pytest.assume(expdd==dd)
+
+@pytest.mark.yml
+def test_parse_config_explicit_white_list(request, mocker, ymlparsersSetup, ymlparsersCleanup, initappconfFixture):
+    logger.info(f'{request._pyfuncitem.name}()')
+
+    expdd = {
+        'general': {'profiles': [],
+                    'log': {
+                        'version': 1,
+                        'disable_existing_loggers': False,
+                        'formatters': {
+                            'brief': {
+                                'format': '%(message)s'
+                            },
+                            'detail': {
+                                'format': '%(asctime)-15s %(levelname)s [%(name)s.%(funcName)s] %(message)s',
+                                'datefmt': '%Y-%m-%d %H:%M:%S'
+                            },
+                        },
+                        'root': {
+                            'level': 'DEBUG'
+                        }
+                    },
+                    'config':{
+                        'file' : None   #will be be populated below
+                    },
+                    'whiteListSysOverride': ['app.host_name'],   #explicetly populated
+                    'listEnsure': [],   #whiteListSysOverride can be overridden in sysargs, regargless,  \
+                                        # we don't override any (other) list value from sysargs
+                    },  # list
+        'app': {'host_name': '10.20.40.60',
+                'news': 'cnn.com',
+                #'portal': 'reddit.com',     #this will NOT be proceses because of explicit general.whiteListSysOverride
+                'white_list': ['gamma', 'alpha', 'betha'],
+                'alt_white_list': [100, 10.0],
+                }
+    }
+
+    pck = '.'.join(['tests_data', __package__, 'initappconf'])
+
+    with path(pck, 'confige.yml') as full_path:
+        expdd['general']['config']['file'] = str(full_path)
+
+        #app.host_name is in general.whiteListSysOverridem it will be process
+        #app.portal and last line will be ignored
+        argsv = f'--general.config.file={full_path} '\
+                '--app.portal=reddit.com ' \
+                '--app.host_name=10.20.40.60 ' \
+                '10.20.40.60:8082 ' \
+            .split()
+
+
+        dd = parse_config(None, argsv)
+        del dd['general']['log']['handlers']
+        del dd['general']['log']['root']['handlers']
+
+        pytest.assume(expdd==dd)
+
+@pytest.mark.yml
+def test_parse_config_false(request, mocker, ymlparsersSetup, ymlparsersCleanup, initappconfFixture):
+    logger.info(f'{request._pyfuncitem.name}()')
+    pck = '.'.join(['tests_data', __package__, 'initappconf'])
+    exp_disable_existing_loggers = 'False'
+
+    with path(pck, 'config.yml') as full_path:
+        argsv = f'--general.config.file={full_path} ' \
+                '--general.profiles=dev ' \
+                f'--general.log.disable_existing_loggers={exp_disable_existing_loggers} ' \
+            .split()
+
+        dd = parse_config(None, argsv, implicit_convert=False)
+        disable_existing_loggers = dd['general']['log']['disable_existing_loggers']
+        pytest.assume(exp_disable_existing_loggers==disable_existing_loggers)
+
+@pytest.mark.yml
+def test_parse_config_default_as_false(request, mocker, ymlparsersSetup, ymlparsersCleanup, initappconfFalseFixture):
+    logger.info(f'{request._pyfuncitem.name}()')
+    pck = '.'.join(['tests_data', __package__, 'initappconf'])
+    exp_disable_existing_loggers = 'False'
+
+    with path(pck, 'config.yml') as full_path:
+        argsv = f'--general.config.file={full_path} ' \
+                '--general.profiles=dev ' \
+                f'--general.log.disable_existing_loggers={exp_disable_existing_loggers} ' \
+            .split()
+
+        dd = parse_config(None, argsv)
+        disable_existing_loggers = dd['general']['log']['disable_existing_loggers']
+        pytest.assume(exp_disable_existing_loggers==disable_existing_loggers)
+
+@pytest.mark.yml
+def test_parse_config_default_as_true(request, mocker, ymlparsersSetup, ymlparsersCleanup, initappconfFixture):
+    logger.info(f'{request._pyfuncitem.name}()')
+    pck = '.'.join(['tests_data', __package__, 'initappconf'])
+    exp_disable_existing_loggers = False
+
+    with path(pck, 'config.yml') as full_path:
+        argsv = f'--general.config.file={full_path} ' \
+                '--general.profiles=dev ' \
+                f'--general.log.disable_existing_loggers={exp_disable_existing_loggers} ' \
+            .split()
+
+        dd = parse_config(None, argsv)
+        disable_existing_loggers = dd['general']['log']['disable_existing_loggers']
+        pytest.assume(exp_disable_existing_loggers==disable_existing_loggers)
+
+
+
+if __name__ == "__main__":
+    pytest.main([__file__])
+
+
```

### Comparing `alex_ber_utils-0.6.6b3/tests/utils/inspect_test.py` & `alex_ber_utils-0.7.0/tests/utils/inspect_test.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,176 +1,176 @@
-import logging
-import pytest
-import inspect
-from alexber.utils.inspects import issetdescriptor, ismethod, has_method
-from collections import OrderedDict
-
-logger = logging.getLogger(__name__)
-
-
-class Example(object):
-    def __init__(self, name, address=None, *args, **kwargs):
-        pass
-
-    def foo1(self):
-        pass
-
-    @staticmethod
-    def method1():
-        pass
-
-    @classmethod
-    def method2(cls):
-        pass
-
-    @property
-    def att1(self):
-        return 5
-
-    @att1.setter
-    def att1(self, value):
-        pass
-
-    @property
-    def att_get_only(self):
-        return 5
-
-    def _set_only(self):
-        pass
-
-    att_set_only = property(fset=_set_only)
-
-
-    def set_x(self, x):
-        pass
-
-    def baz(self, a, b, c):
-        pass
-
-    def seed(self, a=None, version=2):
-        pass
-
-class Base(object):
-
-    @property
-    def att1(self):
-        return 5
-
-    @att1.setter
-    def att1(self, value):
-        pass
-
-    @property
-    def att_get_only(self):
-        return 5
-
-    def set_x(self, x):
-        pass
-
-class Derived(Base):
-    def __init__(self, name, address=None, *args, **kwargs):
-        pass
-
-
-
-@pytest.mark.parametrize(
-     'obj',
-    (Example,
-     Derived),
-)
-def test_property_get_set(request, obj):
-    logger.info(f'{request._pyfuncitem.name}()')
-    results = inspect.getmembers(obj, predicate=issetdescriptor)
-    d = {key: value for key, value in results}
-
-    prop = d['att1']
-
-    setter = prop.fset
-    setter(self=None, value=100)
-
-    prop = d['att_get_only']
-    setter = prop.fset
-    assert setter is None
-
-
-@pytest.mark.parametrize(
-     'f',
-    (Example,
-     Derived),
-)
-def test_signature(request, f):
-    logger.info(f'{request._pyfuncitem.name}()')
-    sig = inspect.signature(f)
-
-    d = OrderedDict()
-    for var in sig.parameters.keys():
-        d[var] = None
-
-    var = d['name']
-
-    logger.debug(d)
-    logger.debug(var)
-
-@pytest.mark.parametrize(
-     'f',
-    (Example,
-     Derived),
-)
-#see https://stackoverflow.com/questions/218616/getting-method-parameter-names-in-python/45781963#45781963
-#see https://stackoverflow.com/questions/218616/getting-method-parameter-names-in-python/44261531#44261531
-def test_binding(request, f):
-    logger.info(f'{request._pyfuncitem.name}()')
-    d = OrderedDict()
-    d['name'] = 'metoo'
-
-    sig = inspect.signature(f)
-    bound_args = sig.bind(**d)
-    bound_args.apply_defaults()
-    kwargs = bound_args.arguments
-    obj = f(**kwargs)
-    assert obj is not None
-
-class SubDerived(Derived):
-    def set_x(self, x):
-        pass
-
-class Derivitive(SubDerived, Base):
-    def set_x(self, x):
-        pass
-
-    def cool(self):
-        pass
-
-@pytest.mark.parametrize(
-     'cls, method_name, exp_value',
-
-    [
-        (Example, '__init__', True),
-        (Example, 'foo1', True),
-        (Example, 'method1', True),
-        (Example, 'method2', True),
-        (Example, 'att1', True),
-        (Example, 'att_get_only', True),
-        (Example, '_set_only', True),
-        (Example, 'set_x', True),
-        (Example, 'baz', True),
-        (Example, '__init__', True),
-        (Example, 'seed', True),
-        (Example, 'this_is_method_is_not_here', False),
-        (Derived, '__init__', True),
-        (SubDerived, 'set_x', True),
-        (SubDerived, 'set_non_exists', False),
-        (Derivitive, 'set_x', True),
-        (Derivitive, 'cool', True),
-        (Derivitive, 'set_non_exists', False),
-
-
-    ]
-)
-def test_has_method(request, cls, method_name, exp_value):
-    logger.info(f'{request._pyfuncitem.name}()')
-
-    b = has_method(cls, method_name)
-    assert exp_value == b
-
-if __name__ == "__main__":
-    pytest.main([__file__])
+import logging
+import pytest
+import inspect
+from alexber.utils.inspects import issetdescriptor, ismethod, has_method
+from collections import OrderedDict
+
+logger = logging.getLogger(__name__)
+
+
+class Example(object):
+    def __init__(self, name, address=None, *args, **kwargs):
+        pass
+
+    def foo1(self):
+        pass
+
+    @staticmethod
+    def method1():
+        pass
+
+    @classmethod
+    def method2(cls):
+        pass
+
+    @property
+    def att1(self):
+        return 5
+
+    @att1.setter
+    def att1(self, value):
+        pass
+
+    @property
+    def att_get_only(self):
+        return 5
+
+    def _set_only(self):
+        pass
+
+    att_set_only = property(fset=_set_only)
+
+
+    def set_x(self, x):
+        pass
+
+    def baz(self, a, b, c):
+        pass
+
+    def seed(self, a=None, version=2):
+        pass
+
+class Base(object):
+
+    @property
+    def att1(self):
+        return 5
+
+    @att1.setter
+    def att1(self, value):
+        pass
+
+    @property
+    def att_get_only(self):
+        return 5
+
+    def set_x(self, x):
+        pass
+
+class Derived(Base):
+    def __init__(self, name, address=None, *args, **kwargs):
+        pass
+
+
+
+@pytest.mark.parametrize(
+     'obj',
+    (Example,
+     Derived),
+)
+def test_property_get_set(request, obj):
+    logger.info(f'{request._pyfuncitem.name}()')
+    results = inspect.getmembers(obj, predicate=issetdescriptor)
+    d = {key: value for key, value in results}
+
+    prop = d['att1']
+
+    setter = prop.fset
+    setter(self=None, value=100)
+
+    prop = d['att_get_only']
+    setter = prop.fset
+    assert setter is None
+
+
+@pytest.mark.parametrize(
+     'f',
+    (Example,
+     Derived),
+)
+def test_signature(request, f):
+    logger.info(f'{request._pyfuncitem.name}()')
+    sig = inspect.signature(f)
+
+    d = OrderedDict()
+    for var in sig.parameters.keys():
+        d[var] = None
+
+    var = d['name']
+
+    logger.debug(d)
+    logger.debug(var)
+
+@pytest.mark.parametrize(
+     'f',
+    (Example,
+     Derived),
+)
+#see https://stackoverflow.com/questions/218616/getting-method-parameter-names-in-python/45781963#45781963
+#see https://stackoverflow.com/questions/218616/getting-method-parameter-names-in-python/44261531#44261531
+def test_binding(request, f):
+    logger.info(f'{request._pyfuncitem.name}()')
+    d = OrderedDict()
+    d['name'] = 'metoo'
+
+    sig = inspect.signature(f)
+    bound_args = sig.bind(**d)
+    bound_args.apply_defaults()
+    kwargs = bound_args.arguments
+    obj = f(**kwargs)
+    assert obj is not None
+
+class SubDerived(Derived):
+    def set_x(self, x):
+        pass
+
+class Derivitive(SubDerived, Base):
+    def set_x(self, x):
+        pass
+
+    def cool(self):
+        pass
+
+@pytest.mark.parametrize(
+     'cls, method_name, exp_value',
+
+    [
+        (Example, '__init__', True),
+        (Example, 'foo1', True),
+        (Example, 'method1', True),
+        (Example, 'method2', True),
+        (Example, 'att1', True),
+        (Example, 'att_get_only', True),
+        (Example, '_set_only', True),
+        (Example, 'set_x', True),
+        (Example, 'baz', True),
+        (Example, '__init__', True),
+        (Example, 'seed', True),
+        (Example, 'this_is_method_is_not_here', False),
+        (Derived, '__init__', True),
+        (SubDerived, 'set_x', True),
+        (SubDerived, 'set_non_exists', False),
+        (Derivitive, 'set_x', True),
+        (Derivitive, 'cool', True),
+        (Derivitive, 'set_non_exists', False),
+
+
+    ]
+)
+def test_has_method(request, cls, method_name, exp_value):
+    logger.info(f'{request._pyfuncitem.name}()')
+
+    b = has_method(cls, method_name)
+    assert exp_value == b
+
+if __name__ == "__main__":
+    pytest.main([__file__])
```

### Comparing `alex_ber_utils-0.6.6b3/tests/utils/mains_test.py` & `alex_ber_utils-0.7.0/tests/utils/mains_test.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-import logging
-from pathlib import Path
-import pytest
-
-logger = logging.getLogger(__name__)
-
-from alexber.utils.mains import fixabscwd, logger as real_logger
-import os
-import sys
-
-
-_real_info = real_logger.info
-
-@pytest.fixture(scope='module')
-def loggingCaptureWarnings():
-    logging.captureWarnings(True)
-
-@pytest.fixture
-def mock_os(mocker):
-    ret_mock = mocker.patch('.'.join(['alexber.utils.mains', '_os']), autospec=True, spec_set=True)
-
-    cwd = str(Path(__file__).resolve().parent)
-    ret_mock.getcwd.return_value = cwd
-    ret_mock.path = os.path
-
-    return ret_mock
-
-@pytest.fixture
-def mock_info(mocker):
-    ret_mock = mocker.patch.object(real_logger, 'info', side_effect=_real_info, autospec=True, spec_set=True)
-    return ret_mock
-
-@pytest.fixture
-def mock_main_module(mocker):
-    ret_mock = sys.modules['__main__']
-    mocker.patch.object(ret_mock, '__file__', new=__file__)
-    return ret_mock
-
-
-def test_fixabscwd(request, loggingCaptureWarnings, mock_os, mock_info, mock_main_module):
-    logger.info(f'{request._pyfuncitem.name}()')
-
-    fixabscwd()
-
-    pytest.assume(mock_info.call_count > 0)
-
-    pytest.assume(mock_os.chdir.call_count == 1)
-    (newcwd,), _ = mock_os.chdir.call_args
-    pytest.assume(str(Path(__file__).parent)==newcwd)
-
-
-
-
-if __name__ == "__main__":
-    pytest.main([__file__])
+import logging
+from pathlib import Path
+import pytest
+
+logger = logging.getLogger(__name__)
+
+from alexber.utils.mains import fixabscwd, logger as real_logger
+import os
+import sys
+
+
+_real_info = real_logger.info
+
+@pytest.fixture(scope='module')
+def loggingCaptureWarnings():
+    logging.captureWarnings(True)
+
+@pytest.fixture
+def mock_os(mocker):
+    ret_mock = mocker.patch('.'.join(['alexber.utils.mains', '_os']), autospec=True, spec_set=True)
+
+    cwd = str(Path(__file__).resolve().parent)
+    ret_mock.getcwd.return_value = cwd
+    ret_mock.path = os.path
+
+    return ret_mock
+
+@pytest.fixture
+def mock_info(mocker):
+    ret_mock = mocker.patch.object(real_logger, 'info', side_effect=_real_info, autospec=True, spec_set=True)
+    return ret_mock
+
+@pytest.fixture
+def mock_main_module(mocker):
+    ret_mock = sys.modules['__main__']
+    mocker.patch.object(ret_mock, '__file__', new=__file__)
+    return ret_mock
+
+
+def test_fixabscwd(request, loggingCaptureWarnings, mock_os, mock_info, mock_main_module):
+    logger.info(f'{request._pyfuncitem.name}()')
+
+    fixabscwd()
+
+    pytest.assume(mock_info.call_count > 0)
+
+    pytest.assume(mock_os.chdir.call_count == 1)
+    (newcwd,), _ = mock_os.chdir.call_args
+    pytest.assume(str(Path(__file__).parent)==newcwd)
+
+
+
+
+if __name__ == "__main__":
+    pytest.main([__file__])
```

### Comparing `alex_ber_utils-0.6.6b3/tests/utils/method_overloading_test.py` & `alex_ber_utils-0.7.0/tests/utils/method_overloading_test.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,98 +1,98 @@
-import logging
-import sys
-import pytest
-
-logger = logging.getLogger(__name__)
-
-try:
-    #python3 -m pip uninstall multidispatch==0.2
-    from multidispatch import multimethod
-except ImportError:
-    class _dummy(object):
-        def dispatch(self, *types):
-            return self
-
-    def multimethod(func):
-        def with_md(*args, **kwargs):
-            return _dummy
-        return with_md
-
-from alexber.utils.importer import importer
-
-
-class Engine(object):
-
-
-    @multimethod(object)
-    def _set_playerA(self, player):
-        logging.debug('instance')
-        pass
-
-    @_set_playerA.dispatch(str)
-    def _(self, st):
-        logging.debug('str')
-        player_cls = importer(st)
-        player = player_cls()
-        player.say()
-        pass
-
-    #alternative (recent) syntax
-    # @_set_playerA.dispatch
-    # def _(self, st: str):
-    #     print('str')
-    #     player_cls = importer(st)
-    #     player = player_cls()
-    #     player.say()
-    #     pass
-
-
-    playerA = property(fset=_set_playerA)
-
-
-class Player(object):
-    def say(self):
-        logging.debug('hello')
-
-@pytest.mark.md
-def test_overloading_object(request, mocker):
-    logger.info(f'{request._pyfuncitem.name}()')
-    namespace = sys.modules[__name__]
-
-    importer = mocker.spy(namespace, 'importer')
-    engine = Engine()
-    input = Player()
-    engine.playerA= input
-
-    assert namespace.importer == importer
-    assert importer.call_count ==0, "Engine.playerA(str) was called, when Engine.playerA(object) was expected"
-                                                            # #we shouldn't use  importer when we have explicit object."
-    logger.info(dir(importer))
-
-@pytest.mark.md
-def test_overloading_str(request, mocker):
-    logger.info(f'{request._pyfuncitem.name}()')
-    namespace = sys.modules[__name__]
-
-    importer = mocker.spy(namespace, 'importer')
-    engine = Engine()
-    input = '.'.join([__name__, 'Player'])
-    engine.playerA = input
-
-    assert namespace.importer == importer
-    importer.assert_called_once_with(input)
-
-class PlayerPhilosopher:
-    def __init_subclass__(cls, default_name, **kwargs):
-        super().__init_subclass__(**kwargs)
-        logger.debug(f"Called __init_subclass({cls}, {default_name})")
-        cls.default_name = default_name
-
-
-class PlayerAustralianPhilosopher(PlayerPhilosopher, default_name="Bruce"):
-    pass
-
-
-
-if __name__ == "__main__":
-    import pytest
+import logging
+import sys
+import pytest
+
+logger = logging.getLogger(__name__)
+
+try:
+    #python3 -m pip uninstall multidispatch==0.2
+    from multidispatch import multimethod
+except ImportError:
+    class _dummy(object):
+        def dispatch(self, *types):
+            return self
+
+    def multimethod(func):
+        def with_md(*args, **kwargs):
+            return _dummy
+        return with_md
+
+from alexber.utils.importer import importer
+
+
+class Engine(object):
+
+
+    @multimethod(object)
+    def _set_playerA(self, player):
+        logging.debug('instance')
+        pass
+
+    @_set_playerA.dispatch(str)
+    def _(self, st):
+        logging.debug('str')
+        player_cls = importer(st)
+        player = player_cls()
+        player.say()
+        pass
+
+    #alternative (recent) syntax
+    # @_set_playerA.dispatch
+    # def _(self, st: str):
+    #     print('str')
+    #     player_cls = importer(st)
+    #     player = player_cls()
+    #     player.say()
+    #     pass
+
+
+    playerA = property(fset=_set_playerA)
+
+
+class Player(object):
+    def say(self):
+        logging.debug('hello')
+
+@pytest.mark.md
+def test_overloading_object(request, mocker):
+    logger.info(f'{request._pyfuncitem.name}()')
+    namespace = sys.modules[__name__]
+
+    importer = mocker.spy(namespace, 'importer')
+    engine = Engine()
+    input = Player()
+    engine.playerA= input
+
+    assert namespace.importer == importer
+    assert importer.call_count ==0, "Engine.playerA(str) was called, when Engine.playerA(object) was expected"
+                                                            # #we shouldn't use  importer when we have explicit object."
+    logger.info(dir(importer))
+
+@pytest.mark.md
+def test_overloading_str(request, mocker):
+    logger.info(f'{request._pyfuncitem.name}()')
+    namespace = sys.modules[__name__]
+
+    importer = mocker.spy(namespace, 'importer')
+    engine = Engine()
+    input = '.'.join([__name__, 'Player'])
+    engine.playerA = input
+
+    assert namespace.importer == importer
+    importer.assert_called_once_with(input)
+
+class PlayerPhilosopher:
+    def __init_subclass__(cls, default_name, **kwargs):
+        super().__init_subclass__(**kwargs)
+        logger.debug(f"Called __init_subclass({cls}, {default_name})")
+        cls.default_name = default_name
+
+
+class PlayerAustralianPhilosopher(PlayerPhilosopher, default_name="Bruce"):
+    pass
+
+
+
+if __name__ == "__main__":
+    import pytest
     pytest.main([__file__])
```

### Comparing `alex_ber_utils-0.6.6b3/tests/utils/parsers_test.py` & `alex_ber_utils-0.7.0/tests/utils/parsers_test.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,232 +1,232 @@
-import enum
-import logging
-
-import pytest
-
-from alexber.utils.enums import Enum
-from alexber.utils.parsers import ConfigParser, ArgumentParser, safe_eval, is_empty, parse_boolean, parse_sys_args
-
-logger = logging.getLogger(__name__)
-from decimal import Decimal
-from datetime import datetime
-from importlib.resources import path
-
-def test_parse_config(request):
-    logger.info(f'{request._pyfuncitem.name}()')
-
-    parser = ConfigParser()
-
-    pck = '.'.join(['tests_data', __package__, 'parser'])
-
-    with path(pck, 'config.ini') as f:
-        parser.read(f)
-
-    dd = parser.as_dict()
-    da = dd['playera']
-    clsa = da['cls']
-    namea = da['name']
-
-    db = dd['playerb']
-    clsb = db['cls']
-    nameb = db['name']
-
-    assert clsa==clsb
-    assert namea == nameb
-
-
-@pytest.fixture(params=[
-    #'args,exp_d',
-    ('--key=value --single',
-     dict([('key', 'value'), ('single', None)])),
-
-    ('wrong=pair',
-         dict([('wrong=pair', None)])),
-
-    ('--conf --prop1=value1 --prop2=value --prop1=value9',
-         dict([('conf', None), ('prop1', 'value9'), ('prop2', 'value')])),
-
-])
-def arg_parse_param(request):
-    return request.param
-
-def test_args_parse(request, mocker, arg_parse_param):
-    logger.info(f'{request._pyfuncitem.name}()')
-    args, exp_d = arg_parse_param
-
-    parser = ArgumentParser()
-
-    mock_args = mocker.patch('alexber.utils.parsers.sys.argv', new_callable=list)
-    mock_args.append(__file__)
-    mock_args[1:] = args.split()
-
-    d = parser.as_dict()
-    assert exp_d==d
-
-
-def test_args_parse_explicit_args(request, arg_parse_param):
-    logger.info(f'{request._pyfuncitem.name}()')
-    args, exp_d = arg_parse_param
-
-    parser = ArgumentParser()
-
-    sys_args = args.split()
-
-    d = parser.as_dict(args=sys_args)
-    assert exp_d==d
-
-
-@pytest.mark.parametrize(
-     'value, exp_value, exp_type',
-
-    [
-        ('John', 'John', str),
-        ('alexber.utils.players.ConstantPlayer', 'alexber.utils.players.ConstantPlayer', str),
-        ('1000', 1000, int),
-        ('0.1', 0.1, float),
-        ('0.0', 0.0, float),
-        ('-0.0', -0.0, float),
-        ('-5', -5, int),
-        ('0.1', None, Decimal),  #Not Supprted
-        ('2019-04-01 16:31:51.513383', None, datetime),  #Not Supprted
-        ('%(message)s','%(message)s', str),#https://github.com/alex-ber/AlexBerUtils/issues/2
-        ('(message)s','(message)s', str),
-        ('(message)','(message)', str),
-
-    ]
-)
-def test_convert(request, value, exp_value, exp_type):
-    logger.info(f'{request._pyfuncitem.name}()')
-    if exp_value is None:
-        logger.debug(f"Type {exp_type} is not supported.")
-        return
-
-
-    result = safe_eval(value)
-    type_result = type(result)
-    pytest.assume(exp_value == result)
-    pytest.assume(exp_type == type_result)
-
-
-@enum.unique
-class Color(Enum):
-    RED = 'r'
-    BLUE = 'b'
-    GREEN = 'g'
-
-
-@pytest.mark.parametrize(
-    'value, exp_result',
-    [
-     (True, False),
-     (False, True),
-     (None, True),
-
-     ("something", False),
-     ("", True),
-     #
-     (1, False),
-     (0, True),
-     (0.0, True),
-
-     ("1", False),
-     ("0", False),
-
-     (Color.RED, False),
-     ([], True),
-     ([None], False),
-     (['something'], False),
-     ]
-)
-def test_is_empty(request, value, exp_result):
-    logger.info(f'{request._pyfuncitem.name}()')
-
-    result = is_empty(value)
-    assert exp_result == result
-
-
-@pytest.mark.parametrize(
-    'value, exp_result',
-    [
-     (True, True),
-     (False, False),
-     (None, None),
-
-     ("True", True),
-     ("False", False),
-
-     ("TRUE", True),
-     ("FALSE", False),
-
-     ("tRuE", True),
-     ("fALsE", False),
-
-     ("true", True),
-     ("false", False),
-
-     (1, True),
-     (0, False),
-     (0.0, False),
-     ]
-)
-def test_parse_boolean(request, value, exp_result):
-    logger.info(f'{request._pyfuncitem.name}()')
-
-    result = parse_boolean(value)
-    assert exp_result == result
-
-@pytest.mark.parametrize(
-    'value',
-    [
-     ("gibrish123"),
-     ("T"),
-     ("F"),
-
-     ("t"),
-     ("f"),
-
-     ("1"),
-     ("0"),
-
-     (3.5),
-     ([]),
-     (5),
-     (2.01),
-
-    ]
-)
-
-
-def test_parse_boolean_invalid(request, value):
-    logger.info(f'{request._pyfuncitem.name}()')
-
-    with pytest.raises(ValueError, match='nknown'):
-        parse_boolean(value)
-
-
-
-def test_parse_sys_args(request):
-    logger.info(f'{request._pyfuncitem.name}()')
-    expdd = {
-        'general.profiles': "dev",
-        'general.log.formatters.detail.format': '%(message)s',
-        'general.log.root.level': '20', #logging.INFO
-        'app.inner_host_name': 'yahoo.com',
-        'app.white_list': 'gamma,alpha,betha',
-        'app.alt_white_list': '100,10.0'
-    }
-
-    argsv = '--general.profiles=dev ' \
-            '--general.log.formatters.detail.format=%(message)s ' \
-            '--general.log.root.level=20 ' \
-            '--app.inner_host_name=yahoo.com ' \
-            '--app.white_list=gamma,alpha,betha ' \
-            '--app.alt_white_list=100,10.0 ' \
-        .split()
-
-
-    _, dd = parse_sys_args(args=argsv)
-    assert expdd == dd
-
-
-if __name__ == "__main__":
-    pytest.main([__file__])
+import enum
+import logging
+
+import pytest
+
+from alexber.utils.enums import Enum
+from alexber.utils.parsers import ConfigParser, ArgumentParser, safe_eval, is_empty, parse_boolean, parse_sys_args
+
+logger = logging.getLogger(__name__)
+from decimal import Decimal
+from datetime import datetime
+from importlib.resources import path
+
+def test_parse_config(request):
+    logger.info(f'{request._pyfuncitem.name}()')
+
+    parser = ConfigParser()
+
+    pck = '.'.join(['tests_data', __package__, 'parser'])
+
+    with path(pck, 'config.ini') as f:
+        parser.read(f)
+
+    dd = parser.as_dict()
+    da = dd['playera']
+    clsa = da['cls']
+    namea = da['name']
+
+    db = dd['playerb']
+    clsb = db['cls']
+    nameb = db['name']
+
+    assert clsa==clsb
+    assert namea == nameb
+
+
+@pytest.fixture(params=[
+    #'args,exp_d',
+    ('--key=value --single',
+     dict([('key', 'value'), ('single', None)])),
+
+    ('wrong=pair',
+         dict([('wrong=pair', None)])),
+
+    ('--conf --prop1=value1 --prop2=value --prop1=value9',
+         dict([('conf', None), ('prop1', 'value9'), ('prop2', 'value')])),
+
+])
+def arg_parse_param(request):
+    return request.param
+
+def test_args_parse(request, mocker, arg_parse_param):
+    logger.info(f'{request._pyfuncitem.name}()')
+    args, exp_d = arg_parse_param
+
+    parser = ArgumentParser()
+
+    mock_args = mocker.patch('alexber.utils.parsers.sys.argv', new_callable=list)
+    mock_args.append(__file__)
+    mock_args[1:] = args.split()
+
+    d = parser.as_dict()
+    assert exp_d==d
+
+
+def test_args_parse_explicit_args(request, arg_parse_param):
+    logger.info(f'{request._pyfuncitem.name}()')
+    args, exp_d = arg_parse_param
+
+    parser = ArgumentParser()
+
+    sys_args = args.split()
+
+    d = parser.as_dict(args=sys_args)
+    assert exp_d==d
+
+
+@pytest.mark.parametrize(
+     'value, exp_value, exp_type',
+
+    [
+        ('John', 'John', str),
+        ('alexber.utils.players.ConstantPlayer', 'alexber.utils.players.ConstantPlayer', str),
+        ('1000', 1000, int),
+        ('0.1', 0.1, float),
+        ('0.0', 0.0, float),
+        ('-0.0', -0.0, float),
+        ('-5', -5, int),
+        ('0.1', None, Decimal),  #Not Supprted
+        ('2019-04-01 16:31:51.513383', None, datetime),  #Not Supprted
+        ('%(message)s','%(message)s', str),#https://github.com/alex-ber/AlexBerUtils/issues/2
+        ('(message)s','(message)s', str),
+        ('(message)','(message)', str),
+
+    ]
+)
+def test_convert(request, value, exp_value, exp_type):
+    logger.info(f'{request._pyfuncitem.name}()')
+    if exp_value is None:
+        logger.debug(f"Type {exp_type} is not supported.")
+        return
+
+
+    result = safe_eval(value)
+    type_result = type(result)
+    pytest.assume(exp_value == result)
+    pytest.assume(exp_type == type_result)
+
+
+@enum.unique
+class Color(Enum):
+    RED = 'r'
+    BLUE = 'b'
+    GREEN = 'g'
+
+
+@pytest.mark.parametrize(
+    'value, exp_result',
+    [
+     (True, False),
+     (False, True),
+     (None, True),
+
+     ("something", False),
+     ("", True),
+     #
+     (1, False),
+     (0, True),
+     (0.0, True),
+
+     ("1", False),
+     ("0", False),
+
+     (Color.RED, False),
+     ([], True),
+     ([None], False),
+     (['something'], False),
+     ]
+)
+def test_is_empty(request, value, exp_result):
+    logger.info(f'{request._pyfuncitem.name}()')
+
+    result = is_empty(value)
+    assert exp_result == result
+
+
+@pytest.mark.parametrize(
+    'value, exp_result',
+    [
+     (True, True),
+     (False, False),
+     (None, None),
+
+     ("True", True),
+     ("False", False),
+
+     ("TRUE", True),
+     ("FALSE", False),
+
+     ("tRuE", True),
+     ("fALsE", False),
+
+     ("true", True),
+     ("false", False),
+
+     (1, True),
+     (0, False),
+     (0.0, False),
+     ]
+)
+def test_parse_boolean(request, value, exp_result):
+    logger.info(f'{request._pyfuncitem.name}()')
+
+    result = parse_boolean(value)
+    assert exp_result == result
+
+@pytest.mark.parametrize(
+    'value',
+    [
+     ("gibrish123"),
+     ("T"),
+     ("F"),
+
+     ("t"),
+     ("f"),
+
+     ("1"),
+     ("0"),
+
+     (3.5),
+     ([]),
+     (5),
+     (2.01),
+
+    ]
+)
+
+
+def test_parse_boolean_invalid(request, value):
+    logger.info(f'{request._pyfuncitem.name}()')
+
+    with pytest.raises(ValueError, match='nknown'):
+        parse_boolean(value)
+
+
+
+def test_parse_sys_args(request):
+    logger.info(f'{request._pyfuncitem.name}()')
+    expdd = {
+        'general.profiles': "dev",
+        'general.log.formatters.detail.format': '%(message)s',
+        'general.log.root.level': '20', #logging.INFO
+        'app.inner_host_name': 'yahoo.com',
+        'app.white_list': 'gamma,alpha,betha',
+        'app.alt_white_list': '100,10.0'
+    }
+
+    argsv = '--general.profiles=dev ' \
+            '--general.log.formatters.detail.format=%(message)s ' \
+            '--general.log.root.level=20 ' \
+            '--app.inner_host_name=yahoo.com ' \
+            '--app.white_list=gamma,alpha,betha ' \
+            '--app.alt_white_list=100,10.0 ' \
+        .split()
+
+
+    _, dd = parse_sys_args(args=argsv)
+    assert expdd == dd
+
+
+if __name__ == "__main__":
+    pytest.main([__file__])
```

### Comparing `alex_ber_utils-0.6.6b3/tests/utils/processinvokes_test.py` & `alex_ber_utils-0.7.0/tests/utils/processinvokes_test.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,145 +1,145 @@
-import logging
-import shlex
-import os as _os
-import tempfile
-from pathlib import Path
-import pytest
-import alexber.utils.processinvokes as processinvokes
-from alexber.utils.processinvokes import LogPipe, LogSubProcessCall
-
-logger = logging.getLogger(__name__)
-process_invokes_logger = None
-_process_invokes_logger_log = None
-
-@pytest.fixture
-def mock_log(mocker):
-    ret_mock = mocker.patch.object(process_invokes_logger, 'log', side_effect=_process_invokes_logger_log, autospec=True, spec_set=True)
-    return ret_mock
-
-
-@pytest.fixture
-def mock_file(mocker):
-    open_mock = mocker.patch('.'.join(['alexber.utils.processinvokes', 'open']), create=True)
-    mock_close = mocker.MagicMock()
-    mock_write = mocker.MagicMock()
-    open_mock.return_value.close = mock_close
-    open_mock.return_value.write = mock_write
-
-    return open_mock
-
-
-def _reset_processinvokes():
-    processinvokes.default_log_name  = None
-    processinvokes.default_log_level = None
-    processinvokes.default_logpipe_cls = None
-
-    executor = processinvokes.executor
-    if executor is not None:
-        executor.shutdown(wait=False)
-        # see https://gist.github.com/clchiou/f2608cbe54403edb0b13
-        #import concurrent.futures.thread
-        #executor._threads.clear()
-        #concurrent.futures.thread._threads_queues.clear()
-    processinvokes.executor = None
-
-@pytest.fixture
-def processinvokesFixture(mocker):
-    _reset_processinvokes()
-
-    global process_invokes_logger
-    process_invokes_logger = logging.getLogger('process_invoke_run')
-    global _process_invokes_logger_log
-    _process_invokes_logger_log = process_invokes_logger.log
-    processinvokes.initConfig(**{'default_log_name': 'process_invoke_run'})
-    yield None
-    _reset_processinvokes()
-
-
-
-def test_process_invokes(request, mocker, processinvokesFixture, mock_log):
-    logger.info(f'{request._pyfuncitem.name}()')
-    exp_log_msg = "simulating run_sub_process"
-    process_invoke_run = f"echo '{exp_log_msg}'"
-    cmd = shlex.split(process_invoke_run)
-
-    process_invoke_cwd = _os.getcwd()
-    processinvokes.run_sub_process(*cmd, **{'kwargs':{'cwd':process_invoke_cwd}})
-
-    pytest.assume(mock_log.call_count == 1)
-    (_,logmsg), _ = mock_log.call_args
-    pytest.assume(exp_log_msg == logmsg)
-
-class MyLogPipe(LogPipe):
-    pass
-
-class MyLogSubProcessCall(LogSubProcessCall):
-    pass
-
-def test_init_config(request, mocker, processinvokesFixture):
-    logger.info(f'{request._pyfuncitem.name}()')
-
-    logPipeClassName = '.'.join([__name__, MyLogPipe.__name__])
-    logSubProcessCallClassName = '.'.join([__name__, MyLogSubProcessCall.__name__])
-
-    processinvokes.initConfig(**{'default_log_name': 'process_invoke_run',
-                                 'default_logpipe_cls': logPipeClassName,
-                                 'default_log_subprocess_cls': logSubProcessCallClassName,
-                                 })
-
-    pytest.assume(processinvokes.default_logpipe_cls == MyLogPipe)
-    pytest.assume(processinvokes.default_log_subprocess_cls == MyLogSubProcessCall)
-
-
-def test_process_invokes_file_pipe1(request, mocker, processinvokesFixture, mock_file):
-    logger.info(f'{request._pyfuncitem.name}()')
-    exp_log_msg = "simulating run_sub_process"
-    process_invoke_run = f"echo '{exp_log_msg}'"
-    cmd = shlex.split(process_invoke_run)
-
-    process_invoke_cwd = _os.getcwd()
-    filename = "my.log"
-    mock_close = mocker.MagicMock()
-    mock_write = mocker.MagicMock()
-    mock_file.close = mock_close
-    mock_file.write = mock_write
-    processinvokes.initConfig(**{'default_log_name': 'process_invoke_run',
-                                 'default_logpipe_cls': 'alexber.utils.processinvokes.FilePipe'
-                                 })
-
-    processinvokes.run_sub_process(*cmd, **{'cwd':process_invoke_cwd,
-                                                      'logPipe': {
-                                                          'kwargs' : {'fileName': filename}
-                                                      }
-                                                      })
-
-    pytest.assume(mock_file.return_value.close.call_count == 1)
-    pytest.assume(mock_file.return_value.write.call_count > 0)
-    (logmsg,), _ = mock_file.return_value.write.call_args
-    pytest.assume(f'{exp_log_msg}\n' == logmsg)
-
-def test_process_invokes_file_pipe2(request, mocker, processinvokesFixture, mock_file):
-    logger.info(f'{request._pyfuncitem.name}()')
-    exp_log_msg = "simulating run_sub_process"
-    process_invoke_run = f"echo '{exp_log_msg}'"
-    cmd = shlex.split(process_invoke_run)
-
-    process_invoke_cwd = _os.getcwd()
-    filename = "my.log"
-
-
-    processinvokes.run_sub_process(*cmd, **{'cwd':process_invoke_cwd,
-                                                  'logPipe': {
-                                                      'cls': 'alexber.utils.processinvokes.FilePipe',
-                                                      'kwargs' : {'fileName': filename}
-                                                  }
-                                                  })
-
-    pytest.assume(mock_file.return_value.close.call_count == 1)
-    pytest.assume(mock_file.return_value.write.call_count > 0)
-    (logmsg,), _ = mock_file.return_value.write.call_args
-    pytest.assume(f'{exp_log_msg}\n' == logmsg)
-
-
-
-if __name__ == "__main__":
-    pytest.main([__file__])
+import logging
+import shlex
+import os as _os
+import tempfile
+from pathlib import Path
+import pytest
+import alexber.utils.processinvokes as processinvokes
+from alexber.utils.processinvokes import LogPipe, LogSubProcessCall
+
+logger = logging.getLogger(__name__)
+process_invokes_logger = None
+_process_invokes_logger_log = None
+
+@pytest.fixture
+def mock_log(mocker):
+    ret_mock = mocker.patch.object(process_invokes_logger, 'log', side_effect=_process_invokes_logger_log, autospec=True, spec_set=True)
+    return ret_mock
+
+
+@pytest.fixture
+def mock_file(mocker):
+    open_mock = mocker.patch('.'.join(['alexber.utils.processinvokes', 'open']), create=True)
+    mock_close = mocker.MagicMock()
+    mock_write = mocker.MagicMock()
+    open_mock.return_value.close = mock_close
+    open_mock.return_value.write = mock_write
+
+    return open_mock
+
+
+def _reset_processinvokes():
+    processinvokes.default_log_name  = None
+    processinvokes.default_log_level = None
+    processinvokes.default_logpipe_cls = None
+
+    executor = processinvokes.executor
+    if executor is not None:
+        executor.shutdown(wait=False)
+        # see https://gist.github.com/clchiou/f2608cbe54403edb0b13
+        #import concurrent.futures.thread
+        #executor._threads.clear()
+        #concurrent.futures.thread._threads_queues.clear()
+    processinvokes.executor = None
+
+@pytest.fixture
+def processinvokesFixture(mocker):
+    _reset_processinvokes()
+
+    global process_invokes_logger
+    process_invokes_logger = logging.getLogger('process_invoke_run')
+    global _process_invokes_logger_log
+    _process_invokes_logger_log = process_invokes_logger.log
+    processinvokes.initConfig(**{'default_log_name': 'process_invoke_run'})
+    yield None
+    _reset_processinvokes()
+
+
+
+def test_process_invokes(request, mocker, processinvokesFixture, mock_log):
+    logger.info(f'{request._pyfuncitem.name}()')
+    exp_log_msg = "simulating run_sub_process"
+    process_invoke_run = f"echo '{exp_log_msg}'"
+    cmd = shlex.split(process_invoke_run)
+
+    process_invoke_cwd = _os.getcwd()
+    processinvokes.run_sub_process(*cmd, **{'kwargs':{'cwd':process_invoke_cwd}})
+
+    pytest.assume(mock_log.call_count == 1)
+    (_,logmsg), _ = mock_log.call_args
+    pytest.assume(exp_log_msg == logmsg)
+
+class MyLogPipe(LogPipe):
+    pass
+
+class MyLogSubProcessCall(LogSubProcessCall):
+    pass
+
+def test_init_config(request, mocker, processinvokesFixture):
+    logger.info(f'{request._pyfuncitem.name}()')
+
+    logPipeClassName = '.'.join([__name__, MyLogPipe.__name__])
+    logSubProcessCallClassName = '.'.join([__name__, MyLogSubProcessCall.__name__])
+
+    processinvokes.initConfig(**{'default_log_name': 'process_invoke_run',
+                                 'default_logpipe_cls': logPipeClassName,
+                                 'default_log_subprocess_cls': logSubProcessCallClassName,
+                                 })
+
+    pytest.assume(processinvokes.default_logpipe_cls == MyLogPipe)
+    pytest.assume(processinvokes.default_log_subprocess_cls == MyLogSubProcessCall)
+
+
+def test_process_invokes_file_pipe1(request, mocker, processinvokesFixture, mock_file):
+    logger.info(f'{request._pyfuncitem.name}()')
+    exp_log_msg = "simulating run_sub_process"
+    process_invoke_run = f"echo '{exp_log_msg}'"
+    cmd = shlex.split(process_invoke_run)
+
+    process_invoke_cwd = _os.getcwd()
+    filename = "my.log"
+    mock_close = mocker.MagicMock()
+    mock_write = mocker.MagicMock()
+    mock_file.close = mock_close
+    mock_file.write = mock_write
+    processinvokes.initConfig(**{'default_log_name': 'process_invoke_run',
+                                 'default_logpipe_cls': 'alexber.utils.processinvokes.FilePipe'
+                                 })
+
+    processinvokes.run_sub_process(*cmd, **{'cwd':process_invoke_cwd,
+                                                      'logPipe': {
+                                                          'kwargs' : {'fileName': filename}
+                                                      }
+                                                      })
+
+    pytest.assume(mock_file.return_value.close.call_count == 1)
+    pytest.assume(mock_file.return_value.write.call_count > 0)
+    (logmsg,), _ = mock_file.return_value.write.call_args
+    pytest.assume(f'{exp_log_msg}\n' == logmsg)
+
+def test_process_invokes_file_pipe2(request, mocker, processinvokesFixture, mock_file):
+    logger.info(f'{request._pyfuncitem.name}()')
+    exp_log_msg = "simulating run_sub_process"
+    process_invoke_run = f"echo '{exp_log_msg}'"
+    cmd = shlex.split(process_invoke_run)
+
+    process_invoke_cwd = _os.getcwd()
+    filename = "my.log"
+
+
+    processinvokes.run_sub_process(*cmd, **{'cwd':process_invoke_cwd,
+                                                  'logPipe': {
+                                                      'cls': 'alexber.utils.processinvokes.FilePipe',
+                                                      'kwargs' : {'fileName': filename}
+                                                  }
+                                                  })
+
+    pytest.assume(mock_file.return_value.close.call_count == 1)
+    pytest.assume(mock_file.return_value.write.call_count > 0)
+    (logmsg,), _ = mock_file.return_value.write.call_args
+    pytest.assume(f'{exp_log_msg}\n' == logmsg)
+
+
+
+if __name__ == "__main__":
+    pytest.main([__file__])
```

### Comparing `alex_ber_utils-0.6.6b3/tests/utils/properties_test.py` & `alex_ber_utils-0.7.0/tests/utils/properties_test.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-import logging
-logger = logging.getLogger(__name__)
-import pytest
-
-from alexber.utils.props import Properties
-from importlib.resources import open_text
-
-
-def test_parse_java_properties_alternative_delim(request, mocker):
-    logger.info(f'{request._pyfuncitem.name}()')
-    mocker.patch.object(Properties, 'PLACEHOLDER_TOKEN', new='@', spec_set=True)
-    exp_cls_name_a = 'alexber.rpsgame.players.ConstantPlayer'
-    exp_cls_name_b = exp_cls_name_a
-    expdd = {'playera.cls': 'alexber.rpsgame.players.ConstantPlayer',
-             'playerb.cls': 'alexber.rpsgame.players.ConstantPlayer', }
-
-
-    p = Properties()
-    pck = '.'.join(['tests_data', __package__])
-
-    with open_text(pck, 'config2.properties') as f:
-        p.load(f)
-    dd = p.as_dict()
-
-    assert expdd == dd
-
-
-def test_parse_java_properties(request):
-    logger.info(f'{request._pyfuncitem.name}()')
-    exp_cls_name_a = 'alexber.rpsgame.players.ConstantPlayer'
-    exp_cls_name_b = exp_cls_name_a
-    expdd = {'playera.cls': 'alexber.rpsgame.players.ConstantPlayer',
-             'playerb.cls': 'alexber.rpsgame.players.ConstantPlayer',}
-
-    p = Properties()
-    pck = '.'.join(['tests_data', __package__])
-    with open_text(pck, 'config.properties') as f:
-        p.load(f)
-    dd = p.as_dict()
-    #we want to ignore key inner.*
-    a_cls_name = dd['playera.cls']
-    b_cls_name = dd['playerb.cls']
-
-    d = {'playera.cls': a_cls_name,
-         'playerb.cls': b_cls_name,}
-
-    assert expdd==d
-
-
-
-
-
-if __name__ == "__main__":
-    pytest.main([__file__])
+import logging
+logger = logging.getLogger(__name__)
+import pytest
+
+from alexber.utils.props import Properties
+from importlib.resources import open_text
+
+
+def test_parse_java_properties_alternative_delim(request, mocker):
+    logger.info(f'{request._pyfuncitem.name}()')
+    mocker.patch.object(Properties, 'PLACEHOLDER_TOKEN', new='@', spec_set=True)
+    exp_cls_name_a = 'alexber.rpsgame.players.ConstantPlayer'
+    exp_cls_name_b = exp_cls_name_a
+    expdd = {'playera.cls': 'alexber.rpsgame.players.ConstantPlayer',
+             'playerb.cls': 'alexber.rpsgame.players.ConstantPlayer', }
+
+
+    p = Properties()
+    pck = '.'.join(['tests_data', __package__])
+
+    with open_text(pck, 'config2.properties') as f:
+        p.load(f)
+    dd = p.as_dict()
+
+    assert expdd == dd
+
+
+def test_parse_java_properties(request):
+    logger.info(f'{request._pyfuncitem.name}()')
+    exp_cls_name_a = 'alexber.rpsgame.players.ConstantPlayer'
+    exp_cls_name_b = exp_cls_name_a
+    expdd = {'playera.cls': 'alexber.rpsgame.players.ConstantPlayer',
+             'playerb.cls': 'alexber.rpsgame.players.ConstantPlayer',}
+
+    p = Properties()
+    pck = '.'.join(['tests_data', __package__])
+    with open_text(pck, 'config.properties') as f:
+        p.load(f)
+    dd = p.as_dict()
+    #we want to ignore key inner.*
+    a_cls_name = dd['playera.cls']
+    b_cls_name = dd['playerb.cls']
+
+    d = {'playera.cls': a_cls_name,
+         'playerb.cls': b_cls_name,}
+
+    assert expdd==d
+
+
+
+
+
+if __name__ == "__main__":
+    pytest.main([__file__])
```

### Comparing `alex_ber_utils-0.6.6b3/tests/utils/uuids_test.py` & `alex_ber_utils-0.7.0/tests/utils/uuids_test.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-import logging
-import pytest
-
-logger = logging.getLogger(__name__)
-
-from uuid import uuid1
-_int_from_bytes = int.from_bytes
-from os import urandom
-from alexber.utils import uuid1mc
-
-#refference implementation
-#https://stackoverflow.com/questions/1785503/when-should-i-use-uuid-uuid1-vs-uuid-uuid4-in-python
-def ref_uuid1mc():
-    return uuid1(_int_from_bytes(urandom(6), "big") | 0x010000000000)
-
-def test_uuid1mc(request, mocker):
-    logger.info(f'{request._pyfuncitem.name}()')
-    # logger.debug(urandom(6))
-    rnd = b'W\x91\x8e\xb3!\x08'
-
-    mocker.patch("random._urandom",  side_effect=lambda _: rnd, create=True)
-    mocker.patch('.'.join([__name__, 'urandom']),  side_effect=lambda _: rnd, create=True)
-    mocker.patch('.'.join([__name__, 'uuid1']), side_effect=lambda p:p, autospec=True, spec_set=True)
-    mocker.patch('.'.join(['alexber.utils.uuids', '_uuid1']), side_effect=lambda p: p, autospec=True, spec_set=True)
-
-    exp = ref_uuid1mc()
-    actual = uuid1mc()
-    assert  exp==actual
-
-
-
-
-
-if __name__ == "__main__":
-    pytest.main([__file__])
+import logging
+import pytest
+
+logger = logging.getLogger(__name__)
+
+from uuid import uuid1
+_int_from_bytes = int.from_bytes
+from os import urandom
+from alexber.utils import uuid1mc
+
+#refference implementation
+#https://stackoverflow.com/questions/1785503/when-should-i-use-uuid-uuid1-vs-uuid-uuid4-in-python
+def ref_uuid1mc():
+    return uuid1(_int_from_bytes(urandom(6), "big") | 0x010000000000)
+
+def test_uuid1mc(request, mocker):
+    logger.info(f'{request._pyfuncitem.name}()')
+    # logger.debug(urandom(6))
+    rnd = b'W\x91\x8e\xb3!\x08'
+
+    mocker.patch("random._urandom",  side_effect=lambda _: rnd, create=True)
+    mocker.patch('.'.join([__name__, 'urandom']),  side_effect=lambda _: rnd, create=True)
+    mocker.patch('.'.join([__name__, 'uuid1']), side_effect=lambda p:p, autospec=True, spec_set=True)
+    mocker.patch('.'.join(['alexber.utils.uuids', '_uuid1']), side_effect=lambda p: p, autospec=True, spec_set=True)
+
+    exp = ref_uuid1mc()
+    actual = uuid1mc()
+    assert  exp==actual
+
+
+
+
+
+if __name__ == "__main__":
+    pytest.main([__file__])
```

### Comparing `alex_ber_utils-0.6.6b3/tests/utils/ymlparsers_extra_test.py` & `alex_ber_utils-0.7.0/tests/utils/ymlparsers_extra_test.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,341 +1,341 @@
-import logging
-import pytest
-import alexber.utils._ymlparsers_extra as ymlparsers_extra
-from alexber.utils._ymlparsers_extra import _convert_template_to_string_format, \
-    __convert_template_to_string_format as uuconvert_template_to_string_format, \
-    format_template
-
-
-
-try:
-    from .ymlparsers_test import ymlparsersSetup, ymlparsersCleanup, ymlparsers, create_mock_lock
-    from alexber.utils._ymlparsers_extra import HiYaPyCo
-
-    from jinja2 import Environment as _Environment, \
-                 DebugUndefined as _DebugUndefined
-except ImportError:
-    pass
-
-logger = logging.getLogger(__name__)
-
-
-@pytest.fixture
-def ymlparsersExtraFixture(request, mocker, ymlparsersSetup, ymlparsersCleanup):
-    p_isHiYaPyCoAvailable = ymlparsers_extra._isHiYaPyCoAvailable
-    p_isJinja2DefaultAvailable = ymlparsers_extra._isJinja2DefaultAvailable
-
-    if p_isHiYaPyCoAvailable and p_isJinja2DefaultAvailable:
-        request_param = (p_isHiYaPyCoAvailable, p_isJinja2DefaultAvailable) if (not hasattr(request, 'param')) else request.param
-    else:
-        request_param = (False, False)
-    isHiYaPyCoAvailable, isJinja2DefaultAvailable = request_param
-
-    ymlparsers_extra._isHiYaPyCoAvailable = isHiYaPyCoAvailable
-    ymlparsers_extra._isJinja2DefaultAvailable = isJinja2DefaultAvailable
-    ymlparsers_extra._init_globals()
-
-    yield request_param
-    ymlparsers_extra._isHiYaPyCoAvailable = p_isHiYaPyCoAvailable
-    ymlparsers_extra._isJinja2DefaultAvailable = p_isJinja2DefaultAvailable
-    ymlparsers_extra._init_globals()
-
-
-
-@pytest.mark.parametrize(
-     'template, exp_value',
-
-    [
-        ('ping {{app.inner_host_name}}', 'ping {app_inner_host_name}'),
-        ('Hi, {{user}}. My name is {{app.first.name}}. Good Luck!', 'Hi, {user}. My name is {app_first_name}. Good Luck!'),
-        ('plain text', 'plain text'),
-        ('First. Second.', 'First. Second.'),
-        ('{{name}}', '{name}'),
-        ('{{app,name}}', '{app,name}'),
-        ('{{name}}.', '{name}.'),
-        ('{{app,name}}.', '{app,name}.'),
-        ('', ''),
-         (None, None),
-
-
-    ]
-)
-
-def test_uuconvert_template_to_string_format(request, mocker, template, exp_value):
-    logger.info(f'{request._pyfuncitem.name}()')
-
-    value = uuconvert_template_to_string_format(template,
-                                                default_start='{{',
-                                                default_end='}}'
-                                                )
-    pytest.assume(exp_value==value)
-
-
-
-def test_uuconvert_template_to_string_format_undocumented1(request, mocker):
-    logger.info(f'{request._pyfuncitem.name}()')
-    exp_value = 'ping {{app.inner_host_name}}'
-    value = uuconvert_template_to_string_format(exp_value, default_start=None, default_end=None)
-    pytest.assume(exp_value == value)
-
-def test_uuconvert_template_to_string_format_undocumented2(request, mocker):
-    logger.info(f'{request._pyfuncitem.name}()')
-    exp_value = 'ping {{app.inner_host_name}}'
-    value = uuconvert_template_to_string_format(exp_value)
-    pytest.assume(exp_value == value)
-
-
-def test_uuconvert_is_used_in_uconvert_template_to_string_format(request, mocker, ymlparsersExtraFixture):
-    logger.info(f'{request._pyfuncitem.name}()')
-
-    uconvert_mock=mocker.patch('alexber.utils._ymlparsers_extra.__convert_template_to_string_format',
-                               side_effect=uuconvert_template_to_string_format, autospec=True, spec_set=True)
-
-    exp_value = '{name}'
-    template = '{{name}}'
-    value = _convert_template_to_string_format(template)
-    pytest.assume(exp_value == value)
-    pytest.assume(uconvert_mock.call_count > 0)
-
-
-#isHiYaPyCoAvailable,isJinja2DefaultAvailable
-@pytest.mark.parametrize('ymlparsersExtraFixture', [(False, False), #minimal, no 3-rd party dependencies
-                                                    (True, True),   #maximal 3-rd party dependencies available, \
-                                                                    #but not customized
-                                                    (False, True),  #only Jinja2 avaialble
-                                                    (True, False),  #can't really happen
-                                                    ], indirect=True)
-def test_uconvert_template_to_string_format_minimal(request, mocker, ymlparsersExtraFixture):
-    logger.info(f'{request._pyfuncitem.name}{ymlparsersExtraFixture}')
-
-    exp_value = '{name}'
-    template = '{{name}}'
-    value = _convert_template_to_string_format(template)
-    pytest.assume(exp_value == value)
-
-
-#isHiYaPyCoAvailable,isJinja2DefaultAvailable
-@pytest.mark.parametrize('ymlparsersExtraFixture', [(False, True)  #only Jinja2 avaialble \
-                                                    ], indirect = True)
-@pytest.mark.yml
-def test_uconvert_template_to_string_jinja2DefaultChanged(request, mocker, ymlparsersExtraFixture):
-    logger.info(f'{request._pyfuncitem.name}{ymlparsersExtraFixture}')
-
-
-    mocker.patch('jinja2.defaults.VARIABLE_START_STRING', new='1_', spec_set=True)
-    mocker.patch('jinja2.defaults.VARIABLE_END_STRING', new='_1', spec_set=True)
-
-    ymlparsers_extra._init_globals()
-    exp_value = '{name}'
-    template = '1_name_1'
-    value = _convert_template_to_string_format(template)
-    pytest.assume(exp_value == value)
-
-#isHiYaPyCoAvailable,isJinja2DefaultAvailable
-@pytest.mark.parametrize('ymlparsersExtraFixture', [(True, False)
-                                                    ], indirect = True)
-@pytest.mark.yml
-def test_uconvert_template_to_string_HiYaPyCoDefault(request, mocker, ymlparsersExtraFixture):
-    logger.info(f'{request._pyfuncitem.name}{ymlparsersExtraFixture}')
-
-    ymlparsers.initConfig()
-
-    mock_lock = create_mock_lock(mocker)
-    init_jinja2ctx = HiYaPyCo.jinja2ctx
-    mocker.patch.object(HiYaPyCo, 'jinja2Lock', new=mock_lock, spec_set=True)
-    jinja2ctx_mock = mocker.patch.object(HiYaPyCo, 'jinja2ctx', spec_set=True)
-    mock_variable_start_string = mocker.PropertyMock(return_value=init_jinja2ctx.variable_start_string)
-    type(jinja2ctx_mock).variable_start_string = mock_variable_start_string
-    mock_variable_end_string = mocker.PropertyMock(return_value=init_jinja2ctx.variable_end_string)
-    type(jinja2ctx_mock).variable_end_string = mock_variable_end_string
-
-    exp_value = '{name}'
-    template = '{{name}}'
-    value = _convert_template_to_string_format(template)
-    pytest.assume(exp_value == value)
-
-    pytest.assume(mock_lock.acquire.call_count > 0)
-    pytest.assume(mock_lock.release.call_count == mock_lock.acquire.call_count)
-
-    pytest.assume(mock_variable_start_string.call_count > 0)
-    pytest.assume(mock_variable_end_string.call_count > 0)
-
-
-#isHiYaPyCoAvailable,isJinja2DefaultAvailable
-@pytest.mark.parametrize('ymlparsersExtraFixture', [(True, False)
-                                                    ], indirect = True)
-@pytest.mark.yml
-def test_uconvert_template_to_string_HiYaPyCoDefaultChanged(request, mocker, ymlparsersExtraFixture):
-    logger.info(f'{request._pyfuncitem.name}{ymlparsersExtraFixture}')
-
-
-    ymlparsers.initConfig(jinja2ctx={'variable_start_string':'2_', 'variable_end_string':'_2' })
-    init_jinja2ctx = HiYaPyCo.jinja2ctx
-
-    mock_lock = create_mock_lock(mocker)
-    mocker.patch.object(HiYaPyCo, 'jinja2Lock', new=mock_lock, spec_set=True)
-    jinja2ctx_mock = mocker.patch.object(HiYaPyCo, 'jinja2ctx', spec_set=True)
-    mock_variable_start_string = mocker.PropertyMock(return_value=init_jinja2ctx.variable_start_string)
-    type(jinja2ctx_mock).variable_start_string = mock_variable_start_string
-    mock_variable_end_string = mocker.PropertyMock(return_value=init_jinja2ctx.variable_end_string)
-    type(jinja2ctx_mock).variable_end_string = mock_variable_end_string
-
-    exp_value = '{name}'
-    template = '2_name_2'
-    value = _convert_template_to_string_format(template)
-    pytest.assume(exp_value == value)
-
-    pytest.assume(mock_lock.acquire.call_count > 0)
-    pytest.assume(mock_lock.release.call_count == mock_lock.acquire.call_count)
-
-    pytest.assume(mock_variable_start_string.call_count > 0)
-    pytest.assume(mock_variable_end_string.call_count > 0)
-
-@pytest.mark.yml
-def test_uconvert_template_to_string_explicit_param1_jinja2ctx(request, mocker, ymlparsersExtraFixture):
-    logger.info(f'{request._pyfuncitem.name}{ymlparsersExtraFixture}')
-
-    mock_lock = create_mock_lock(mocker)
-
-    exp_value = '{name}'
-    template = '3_name_3'
-
-    jinja2ctx = _Environment(undefined=_DebugUndefined, variable_start_string='3_', variable_end_string='_3')
-    value = _convert_template_to_string_format(template, jinja2ctx=jinja2ctx)
-    pytest.assume(exp_value == value)
-
-@pytest.mark.yml
-def test_uconvert_template_to_string_explicit_param1_jinja2Lock(request, mocker, ymlparsersExtraFixture):
-    logger.info(f'{request._pyfuncitem.name}{ymlparsersExtraFixture}')
-
-    mock_lock = create_mock_lock(mocker)
-    mocker.patch.object(HiYaPyCo, 'jinja2Lock', new=mock_lock, spec_set=True)
-
-    #exp_value = '{name}'
-    template = '{{name}}'   #HiYaPyCo.jinja2ctx is default one
-
-    jinja2Lock_param_lock = create_mock_lock(mocker)
-    with pytest.raises(ValueError):
-        _convert_template_to_string_format(template, jinja2Lock=jinja2Lock_param_lock)
-    #pytest.assume(exp_value == value)
-    pytest.assume(mock_lock.acquire.call_count == 0)
-    #pytest.assume(jinja2Lock_param_lock.acquire.call_count ==0)
-
-
-
-#isHiYaPyCoAvailable,isJinja2DefaultAvailable
-@pytest.mark.parametrize('ymlparsersExtraFixture', [(False, True)   #only Jinja2 avaialble \
-                                                    ], indirect = True)
-@pytest.mark.yml
-def test_uconvert_template_to_string_explicit_param1a_jinja2Lock(request, mocker, ymlparsersExtraFixture,
-                                                                ):
-    logger.info(f'{request._pyfuncitem.name}{ymlparsersExtraFixture}')
-
-    mock_lock = create_mock_lock(mocker)
-    mocker.patch.object(HiYaPyCo, 'jinja2Lock', new=mock_lock, spec_set=True)
-    jinja2ctx_mock = mocker.patch.object(HiYaPyCo, 'jinja2ctx', spec_set=True)
-
-    exp_value = '{name}'
-    template = '{{name}}'   #isHiYaPyCoAvailable is not available, global default are used and external lock
-                            # (will be ignored)
-
-    jinja2Lock_param_lock = create_mock_lock(mocker)
-    value = _convert_template_to_string_format(template, jinja2Lock=jinja2Lock_param_lock)
-    pytest.assume(exp_value == value)
-    pytest.assume(mock_lock.acquire.call_count == 0)
-    pytest.assume(jinja2ctx_mock.call_count == 0)
-
-@pytest.mark.yml
-def test_uconvert_template_to_string_explicit_param1b_jinja2Lock(request, mocker, ymlparsersExtraFixture,
-                                                               ):
-    logger.info(f'{request._pyfuncitem.name}{ymlparsersExtraFixture}')
-
-    ymlparsers.initConfig(jinja2ctx={'variable_start_string': '22_', 'variable_end_string': '_22'})
-
-    init_jinja2ctx = HiYaPyCo.jinja2ctx
-    mock_lock = create_mock_lock(mocker)
-    mocker.patch.object(HiYaPyCo, 'jinja2Lock', new=mock_lock, spec_set=True)
-    jinja2ctx_mock = mocker.patch.object(HiYaPyCo, 'jinja2ctx', spec_set=True)
-    mock_variable_start_string = mocker.PropertyMock(return_value=init_jinja2ctx.variable_start_string)
-    type(jinja2ctx_mock).variable_start_string = mock_variable_start_string
-    mock_variable_end_string = mocker.PropertyMock(return_value=init_jinja2ctx.variable_end_string)
-    type(jinja2ctx_mock).variable_end_string = mock_variable_end_string
-
-    #exp_value = '{name}'
-    template = '22_name_22'   #HiYaPyCo.jinja2ctx is non default one and external lock
-
-    jinja2Lock_param_lock = create_mock_lock(mocker)
-    with pytest.raises(ValueError):
-        _convert_template_to_string_format(template, jinja2Lock=jinja2Lock_param_lock)
-    #pytest.assume(exp_value == value)
-    pytest.assume(mock_lock.acquire.call_count == 0)
-    #pytest.assume(jinja2Lock_param_lock.acquire.call_count ==0)
-
-
-#isHiYaPyCoAvailable,isJinja2DefaultAvailable
-@pytest.mark.parametrize('ymlparsersExtraFixture', [(False, True)
-                                                    ], indirect = True)
-@pytest.mark.yml
-def test_uconvert_template_to_string_explicit_param1a_jinja2ctx(request, mocker, ymlparsersExtraFixture,
-                                                               ):
-    logger.info(f'{request._pyfuncitem.name}{ymlparsersExtraFixture}')
-
-    mock_lock = create_mock_lock(mocker)
-    mocker.patch.object(HiYaPyCo, 'jinja2Lock', new=mock_lock, spec_set=True)
-
-    exp_value = '{name}'
-    template = '33_name_33'
-
-    jinja2ctx = _Environment(undefined=_DebugUndefined, variable_start_string='33_', variable_end_string='_33')
-    value = _convert_template_to_string_format(template, jinja2ctx=jinja2ctx)
-
-    pytest.assume(exp_value == value)
-    pytest.assume(mock_lock.acquire.call_count == 0)
-
-
-@pytest.mark.yml
-def test_uconvert_template_to_string_explicit_param2(request, mocker, ymlparsersExtraFixture):
-    logger.info(f'{request._pyfuncitem.name}{ymlparsersExtraFixture}')
-
-    mock_lock = create_mock_lock(mocker)
-    mocker.patch.object(HiYaPyCo, 'jinja2Lock', new=mock_lock, spec_set=True)
-    mock_lock_inuse = create_mock_lock(mocker)
-
-    exp_value = '{name}'
-    template = '4_name_4'
-
-    jinja2ctx = _Environment(undefined=_DebugUndefined, variable_start_string='4_', variable_end_string='_4')
-    value = _convert_template_to_string_format(template, jinja2ctx=jinja2ctx, jinja2Lock=mock_lock_inuse)
-    pytest.assume(exp_value == value)
-
-    pytest.assume(mock_lock.acquire.call_count == 0)
-    pytest.assume(mock_lock_inuse.acquire.call_count >0)
-    pytest.assume(mock_lock_inuse.release.call_count == mock_lock_inuse.acquire.call_count)
-
-
-def test_format_template(request, mocker, ymlparsersExtraFixture):
-    logger.info(f'{request._pyfuncitem.name}()')
-
-    uconvert_mock=mocker.patch('alexber.utils._ymlparsers_extra._convert_template_to_string_format',
-                               side_effect=_convert_template_to_string_format, autospec=True, spec_set=True)
-
-    exp_value = 'Hello, John!'
-    template = 'Hello, {{name}}!'
-    value = format_template(template, name='John')
-    pytest.assume(exp_value == value)
-    pytest.assume(uconvert_mock.call_count > 0)
-
-def test_format_template_without_variables(request, mocker, ymlparsersExtraFixture):
-    logger.info(f'{request._pyfuncitem.name}()')
-
-    uconvert_mock=mocker.patch('alexber.utils._ymlparsers_extra._convert_template_to_string_format',
-                               side_effect=_convert_template_to_string_format, autospec=True, spec_set=True)
-
-    exp_value = 'Hello, World!'
-    template = 'Hello, World!'
-    value = format_template(template)
-    pytest.assume(exp_value == value)
-    pytest.assume(uconvert_mock.call_count > 0)
-
-
-if __name__ == "__main__":
-    pytest.main([__file__])
+import logging
+import pytest
+import alexber.utils._ymlparsers_extra as ymlparsers_extra
+from alexber.utils._ymlparsers_extra import _convert_template_to_string_format, \
+    __convert_template_to_string_format as uuconvert_template_to_string_format, \
+    format_template
+
+
+
+try:
+    from .ymlparsers_test import ymlparsersSetup, ymlparsersCleanup, ymlparsers, create_mock_lock
+    from alexber.utils._ymlparsers_extra import HiYaPyCo
+
+    from jinja2 import Environment as _Environment, \
+                 DebugUndefined as _DebugUndefined
+except ImportError:
+    pass
+
+logger = logging.getLogger(__name__)
+
+
+@pytest.fixture
+def ymlparsersExtraFixture(request, mocker, ymlparsersSetup, ymlparsersCleanup):
+    p_isHiYaPyCoAvailable = ymlparsers_extra._isHiYaPyCoAvailable
+    p_isJinja2DefaultAvailable = ymlparsers_extra._isJinja2DefaultAvailable
+
+    if p_isHiYaPyCoAvailable and p_isJinja2DefaultAvailable:
+        request_param = (p_isHiYaPyCoAvailable, p_isJinja2DefaultAvailable) if (not hasattr(request, 'param')) else request.param
+    else:
+        request_param = (False, False)
+    isHiYaPyCoAvailable, isJinja2DefaultAvailable = request_param
+
+    ymlparsers_extra._isHiYaPyCoAvailable = isHiYaPyCoAvailable
+    ymlparsers_extra._isJinja2DefaultAvailable = isJinja2DefaultAvailable
+    ymlparsers_extra._init_globals()
+
+    yield request_param
+    ymlparsers_extra._isHiYaPyCoAvailable = p_isHiYaPyCoAvailable
+    ymlparsers_extra._isJinja2DefaultAvailable = p_isJinja2DefaultAvailable
+    ymlparsers_extra._init_globals()
+
+
+
+@pytest.mark.parametrize(
+     'template, exp_value',
+
+    [
+        ('ping {{app.inner_host_name}}', 'ping {app_inner_host_name}'),
+        ('Hi, {{user}}. My name is {{app.first.name}}. Good Luck!', 'Hi, {user}. My name is {app_first_name}. Good Luck!'),
+        ('plain text', 'plain text'),
+        ('First. Second.', 'First. Second.'),
+        ('{{name}}', '{name}'),
+        ('{{app,name}}', '{app,name}'),
+        ('{{name}}.', '{name}.'),
+        ('{{app,name}}.', '{app,name}.'),
+        ('', ''),
+         (None, None),
+
+
+    ]
+)
+
+def test_uuconvert_template_to_string_format(request, mocker, template, exp_value):
+    logger.info(f'{request._pyfuncitem.name}()')
+
+    value = uuconvert_template_to_string_format(template,
+                                                default_start='{{',
+                                                default_end='}}'
+                                                )
+    pytest.assume(exp_value==value)
+
+
+
+def test_uuconvert_template_to_string_format_undocumented1(request, mocker):
+    logger.info(f'{request._pyfuncitem.name}()')
+    exp_value = 'ping {{app.inner_host_name}}'
+    value = uuconvert_template_to_string_format(exp_value, default_start=None, default_end=None)
+    pytest.assume(exp_value == value)
+
+def test_uuconvert_template_to_string_format_undocumented2(request, mocker):
+    logger.info(f'{request._pyfuncitem.name}()')
+    exp_value = 'ping {{app.inner_host_name}}'
+    value = uuconvert_template_to_string_format(exp_value)
+    pytest.assume(exp_value == value)
+
+
+def test_uuconvert_is_used_in_uconvert_template_to_string_format(request, mocker, ymlparsersExtraFixture):
+    logger.info(f'{request._pyfuncitem.name}()')
+
+    uconvert_mock=mocker.patch('alexber.utils._ymlparsers_extra.__convert_template_to_string_format',
+                               side_effect=uuconvert_template_to_string_format, autospec=True, spec_set=True)
+
+    exp_value = '{name}'
+    template = '{{name}}'
+    value = _convert_template_to_string_format(template)
+    pytest.assume(exp_value == value)
+    pytest.assume(uconvert_mock.call_count > 0)
+
+
+#isHiYaPyCoAvailable,isJinja2DefaultAvailable
+@pytest.mark.parametrize('ymlparsersExtraFixture', [(False, False), #minimal, no 3-rd party dependencies
+                                                    (True, True),   #maximal 3-rd party dependencies available, \
+                                                                    #but not customized
+                                                    (False, True),  #only Jinja2 avaialble
+                                                    (True, False),  #can't really happen
+                                                    ], indirect=True)
+def test_uconvert_template_to_string_format_minimal(request, mocker, ymlparsersExtraFixture):
+    logger.info(f'{request._pyfuncitem.name}{ymlparsersExtraFixture}')
+
+    exp_value = '{name}'
+    template = '{{name}}'
+    value = _convert_template_to_string_format(template)
+    pytest.assume(exp_value == value)
+
+
+#isHiYaPyCoAvailable,isJinja2DefaultAvailable
+@pytest.mark.parametrize('ymlparsersExtraFixture', [(False, True)  #only Jinja2 avaialble \
+                                                    ], indirect = True)
+@pytest.mark.yml
+def test_uconvert_template_to_string_jinja2DefaultChanged(request, mocker, ymlparsersExtraFixture):
+    logger.info(f'{request._pyfuncitem.name}{ymlparsersExtraFixture}')
+
+
+    mocker.patch('jinja2.defaults.VARIABLE_START_STRING', new='1_', spec_set=True)
+    mocker.patch('jinja2.defaults.VARIABLE_END_STRING', new='_1', spec_set=True)
+
+    ymlparsers_extra._init_globals()
+    exp_value = '{name}'
+    template = '1_name_1'
+    value = _convert_template_to_string_format(template)
+    pytest.assume(exp_value == value)
+
+#isHiYaPyCoAvailable,isJinja2DefaultAvailable
+@pytest.mark.parametrize('ymlparsersExtraFixture', [(True, False)
+                                                    ], indirect = True)
+@pytest.mark.yml
+def test_uconvert_template_to_string_HiYaPyCoDefault(request, mocker, ymlparsersExtraFixture):
+    logger.info(f'{request._pyfuncitem.name}{ymlparsersExtraFixture}')
+
+    ymlparsers.initConfig()
+
+    mock_lock = create_mock_lock(mocker)
+    init_jinja2ctx = HiYaPyCo.jinja2ctx
+    mocker.patch.object(HiYaPyCo, 'jinja2Lock', new=mock_lock, spec_set=True)
+    jinja2ctx_mock = mocker.patch.object(HiYaPyCo, 'jinja2ctx', spec_set=True)
+    mock_variable_start_string = mocker.PropertyMock(return_value=init_jinja2ctx.variable_start_string)
+    type(jinja2ctx_mock).variable_start_string = mock_variable_start_string
+    mock_variable_end_string = mocker.PropertyMock(return_value=init_jinja2ctx.variable_end_string)
+    type(jinja2ctx_mock).variable_end_string = mock_variable_end_string
+
+    exp_value = '{name}'
+    template = '{{name}}'
+    value = _convert_template_to_string_format(template)
+    pytest.assume(exp_value == value)
+
+    pytest.assume(mock_lock.acquire.call_count > 0)
+    pytest.assume(mock_lock.release.call_count == mock_lock.acquire.call_count)
+
+    pytest.assume(mock_variable_start_string.call_count > 0)
+    pytest.assume(mock_variable_end_string.call_count > 0)
+
+
+#isHiYaPyCoAvailable,isJinja2DefaultAvailable
+@pytest.mark.parametrize('ymlparsersExtraFixture', [(True, False)
+                                                    ], indirect = True)
+@pytest.mark.yml
+def test_uconvert_template_to_string_HiYaPyCoDefaultChanged(request, mocker, ymlparsersExtraFixture):
+    logger.info(f'{request._pyfuncitem.name}{ymlparsersExtraFixture}')
+
+
+    ymlparsers.initConfig(jinja2ctx={'variable_start_string':'2_', 'variable_end_string':'_2' })
+    init_jinja2ctx = HiYaPyCo.jinja2ctx
+
+    mock_lock = create_mock_lock(mocker)
+    mocker.patch.object(HiYaPyCo, 'jinja2Lock', new=mock_lock, spec_set=True)
+    jinja2ctx_mock = mocker.patch.object(HiYaPyCo, 'jinja2ctx', spec_set=True)
+    mock_variable_start_string = mocker.PropertyMock(return_value=init_jinja2ctx.variable_start_string)
+    type(jinja2ctx_mock).variable_start_string = mock_variable_start_string
+    mock_variable_end_string = mocker.PropertyMock(return_value=init_jinja2ctx.variable_end_string)
+    type(jinja2ctx_mock).variable_end_string = mock_variable_end_string
+
+    exp_value = '{name}'
+    template = '2_name_2'
+    value = _convert_template_to_string_format(template)
+    pytest.assume(exp_value == value)
+
+    pytest.assume(mock_lock.acquire.call_count > 0)
+    pytest.assume(mock_lock.release.call_count == mock_lock.acquire.call_count)
+
+    pytest.assume(mock_variable_start_string.call_count > 0)
+    pytest.assume(mock_variable_end_string.call_count > 0)
+
+@pytest.mark.yml
+def test_uconvert_template_to_string_explicit_param1_jinja2ctx(request, mocker, ymlparsersExtraFixture):
+    logger.info(f'{request._pyfuncitem.name}{ymlparsersExtraFixture}')
+
+    mock_lock = create_mock_lock(mocker)
+
+    exp_value = '{name}'
+    template = '3_name_3'
+
+    jinja2ctx = _Environment(undefined=_DebugUndefined, variable_start_string='3_', variable_end_string='_3')
+    value = _convert_template_to_string_format(template, jinja2ctx=jinja2ctx)
+    pytest.assume(exp_value == value)
+
+@pytest.mark.yml
+def test_uconvert_template_to_string_explicit_param1_jinja2Lock(request, mocker, ymlparsersExtraFixture):
+    logger.info(f'{request._pyfuncitem.name}{ymlparsersExtraFixture}')
+
+    mock_lock = create_mock_lock(mocker)
+    mocker.patch.object(HiYaPyCo, 'jinja2Lock', new=mock_lock, spec_set=True)
+
+    #exp_value = '{name}'
+    template = '{{name}}'   #HiYaPyCo.jinja2ctx is default one
+
+    jinja2Lock_param_lock = create_mock_lock(mocker)
+    with pytest.raises(ValueError):
+        _convert_template_to_string_format(template, jinja2Lock=jinja2Lock_param_lock)
+    #pytest.assume(exp_value == value)
+    pytest.assume(mock_lock.acquire.call_count == 0)
+    #pytest.assume(jinja2Lock_param_lock.acquire.call_count ==0)
+
+
+
+#isHiYaPyCoAvailable,isJinja2DefaultAvailable
+@pytest.mark.parametrize('ymlparsersExtraFixture', [(False, True)   #only Jinja2 avaialble \
+                                                    ], indirect = True)
+@pytest.mark.yml
+def test_uconvert_template_to_string_explicit_param1a_jinja2Lock(request, mocker, ymlparsersExtraFixture,
+                                                                ):
+    logger.info(f'{request._pyfuncitem.name}{ymlparsersExtraFixture}')
+
+    mock_lock = create_mock_lock(mocker)
+    mocker.patch.object(HiYaPyCo, 'jinja2Lock', new=mock_lock, spec_set=True)
+    jinja2ctx_mock = mocker.patch.object(HiYaPyCo, 'jinja2ctx', spec_set=True)
+
+    exp_value = '{name}'
+    template = '{{name}}'   #isHiYaPyCoAvailable is not available, global default are used and external lock
+                            # (will be ignored)
+
+    jinja2Lock_param_lock = create_mock_lock(mocker)
+    value = _convert_template_to_string_format(template, jinja2Lock=jinja2Lock_param_lock)
+    pytest.assume(exp_value == value)
+    pytest.assume(mock_lock.acquire.call_count == 0)
+    pytest.assume(jinja2ctx_mock.call_count == 0)
+
+@pytest.mark.yml
+def test_uconvert_template_to_string_explicit_param1b_jinja2Lock(request, mocker, ymlparsersExtraFixture,
+                                                               ):
+    logger.info(f'{request._pyfuncitem.name}{ymlparsersExtraFixture}')
+
+    ymlparsers.initConfig(jinja2ctx={'variable_start_string': '22_', 'variable_end_string': '_22'})
+
+    init_jinja2ctx = HiYaPyCo.jinja2ctx
+    mock_lock = create_mock_lock(mocker)
+    mocker.patch.object(HiYaPyCo, 'jinja2Lock', new=mock_lock, spec_set=True)
+    jinja2ctx_mock = mocker.patch.object(HiYaPyCo, 'jinja2ctx', spec_set=True)
+    mock_variable_start_string = mocker.PropertyMock(return_value=init_jinja2ctx.variable_start_string)
+    type(jinja2ctx_mock).variable_start_string = mock_variable_start_string
+    mock_variable_end_string = mocker.PropertyMock(return_value=init_jinja2ctx.variable_end_string)
+    type(jinja2ctx_mock).variable_end_string = mock_variable_end_string
+
+    #exp_value = '{name}'
+    template = '22_name_22'   #HiYaPyCo.jinja2ctx is non default one and external lock
+
+    jinja2Lock_param_lock = create_mock_lock(mocker)
+    with pytest.raises(ValueError):
+        _convert_template_to_string_format(template, jinja2Lock=jinja2Lock_param_lock)
+    #pytest.assume(exp_value == value)
+    pytest.assume(mock_lock.acquire.call_count == 0)
+    #pytest.assume(jinja2Lock_param_lock.acquire.call_count ==0)
+
+
+#isHiYaPyCoAvailable,isJinja2DefaultAvailable
+@pytest.mark.parametrize('ymlparsersExtraFixture', [(False, True)
+                                                    ], indirect = True)
+@pytest.mark.yml
+def test_uconvert_template_to_string_explicit_param1a_jinja2ctx(request, mocker, ymlparsersExtraFixture,
+                                                               ):
+    logger.info(f'{request._pyfuncitem.name}{ymlparsersExtraFixture}')
+
+    mock_lock = create_mock_lock(mocker)
+    mocker.patch.object(HiYaPyCo, 'jinja2Lock', new=mock_lock, spec_set=True)
+
+    exp_value = '{name}'
+    template = '33_name_33'
+
+    jinja2ctx = _Environment(undefined=_DebugUndefined, variable_start_string='33_', variable_end_string='_33')
+    value = _convert_template_to_string_format(template, jinja2ctx=jinja2ctx)
+
+    pytest.assume(exp_value == value)
+    pytest.assume(mock_lock.acquire.call_count == 0)
+
+
+@pytest.mark.yml
+def test_uconvert_template_to_string_explicit_param2(request, mocker, ymlparsersExtraFixture):
+    logger.info(f'{request._pyfuncitem.name}{ymlparsersExtraFixture}')
+
+    mock_lock = create_mock_lock(mocker)
+    mocker.patch.object(HiYaPyCo, 'jinja2Lock', new=mock_lock, spec_set=True)
+    mock_lock_inuse = create_mock_lock(mocker)
+
+    exp_value = '{name}'
+    template = '4_name_4'
+
+    jinja2ctx = _Environment(undefined=_DebugUndefined, variable_start_string='4_', variable_end_string='_4')
+    value = _convert_template_to_string_format(template, jinja2ctx=jinja2ctx, jinja2Lock=mock_lock_inuse)
+    pytest.assume(exp_value == value)
+
+    pytest.assume(mock_lock.acquire.call_count == 0)
+    pytest.assume(mock_lock_inuse.acquire.call_count >0)
+    pytest.assume(mock_lock_inuse.release.call_count == mock_lock_inuse.acquire.call_count)
+
+
+def test_format_template(request, mocker, ymlparsersExtraFixture):
+    logger.info(f'{request._pyfuncitem.name}()')
+
+    uconvert_mock=mocker.patch('alexber.utils._ymlparsers_extra._convert_template_to_string_format',
+                               side_effect=_convert_template_to_string_format, autospec=True, spec_set=True)
+
+    exp_value = 'Hello, John!'
+    template = 'Hello, {{name}}!'
+    value = format_template(template, name='John')
+    pytest.assume(exp_value == value)
+    pytest.assume(uconvert_mock.call_count > 0)
+
+def test_format_template_without_variables(request, mocker, ymlparsersExtraFixture):
+    logger.info(f'{request._pyfuncitem.name}()')
+
+    uconvert_mock=mocker.patch('alexber.utils._ymlparsers_extra._convert_template_to_string_format',
+                               side_effect=_convert_template_to_string_format, autospec=True, spec_set=True)
+
+    exp_value = 'Hello, World!'
+    template = 'Hello, World!'
+    value = format_template(template)
+    pytest.assume(exp_value == value)
+    pytest.assume(uconvert_mock.call_count > 0)
+
+
+if __name__ == "__main__":
+    pytest.main([__file__])
```

### Comparing `alex_ber_utils-0.6.6b3/tests/utils/ymlparsers_test.py` & `alex_ber_utils-0.7.0/tests/utils/ymlparsers_test.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,727 +1,727 @@
-import logging
-import time
-import threading
-import pytest
-import copy
-
-logger = logging.getLogger(__name__)
-
-from importlib.resources import path
-
-import collections
-from collections import OrderedDict
-import io
-import yaml
-from yaml import FullLoader
-from alexber.utils.inspects import has_method
-from alexber.utils._ymlparsers_extra import format_template
-
-
-try:
-    import alexber.utils.ymlparsers as ymlparsers
-    from alexber.utils.ymlparsers import HiYaPyCo
-    from alexber.utils.parsers import is_empty
-    from jinja2 import DebugUndefined, StrictUndefined, Environment
-    from hiyapyco import METHOD_SUBSTITUTE, METHOD_SIMPLE
-except ImportError:
-    pass
-
-def _reset_ymlparsers():
-    ymlparsers.HiYaPyCo.jinja2Lock = None
-    ymlparsers.HiYaPyCo.jinja2ctx = None
-    ymlparsers._load_d = None
-    ymlparsers._safe_dump_d = None
-
-@pytest.fixture
-@pytest.mark.yml
-def ymlparsersSetup(mocker):
-    _reset_ymlparsers()
-
-    ymlparsers.initConfig()
-
-@pytest.fixture(scope='session')
-@pytest.mark.yml
-def exp_config_d():
-    pck = '.'.join(['tests_data', __package__, 'ymlparsers'])
-
-    with path(pck, 'config.yml') as full_path:
-        with open(full_path, 'r') as f:
-            exp_d = yaml.load(f, FullLoader)
-    return exp_d
-
-
-
-@pytest.fixture
-@pytest.mark.yml
-def ymlparsersCleanup(mocker):
-    yield None
-    _reset_ymlparsers()
-
-class DymmyLock(object):
-    def acquire(self, blocking=True):
-        pass
-
-    def release(self):
-        pass
-
-def create_mock_lock(mocker):
-    mock_lock = DymmyLock()
-
-    def __enter__():
-        mock_lock.acquire()
-        return mock_lock
-
-    def __exit__(t, v, tb):
-        mock_lock.release()
-
-    mocker.patch.object(mock_lock, 'acquire', autospec=True, spec_set=True)
-    mocker.patch.object(mock_lock, 'release', autospec=True, spec_set=True)
-    mocker.patch.object(type(mock_lock), '__enter__', side_effect=__enter__, create=True)
-    mocker.patch.object(type(mock_lock), '__exit__', side_effect=__exit__, create=True)
-    return mock_lock
-
-
-class TestYmlparsersInit(object):
-    @pytest.mark.yml
-    def test_initConfig_default_params(self, request, mocker, ymlparsersCleanup):
-        logger.info(f'{request._pyfuncitem.name}()')
-        ymlparsers.initConfig()
-        lock = HiYaPyCo.jinja2Lock
-        pytest.assume(lock is not None)
-        lock_cls = type(lock)
-        b = has_method(lock_cls, 'acquire')
-        pytest.assume(b)
-        b = has_method(lock_cls, 'release')
-        pytest.assume(b)
-
-        jinja2Env = HiYaPyCo.jinja2ctx
-        pytest.assume(jinja2Env is not None)
-
-        jinja2EnvUndefined = jinja2Env.undefined
-        b = issubclass(jinja2EnvUndefined,DebugUndefined)
-        pytest.assume(b)
-
-        jinja2EnvGloblas = jinja2Env.globals
-        b = 'uname' in jinja2EnvGloblas
-        pytest.assume(b)
-
-        _load_d = ymlparsers._load_d
-        assert _load_d is not None
-        b = isinstance(_load_d, collections.abc.Mapping)
-        pytest.assume(b)
-
-        for k, exp_v in {'method':METHOD_SUBSTITUTE,
-                     'mergelists':False,
-                     'interpolate':True,
-                     'castinterpolated':True}.items():
-            v = _load_d[k]
-            pytest.assume(exp_v==v)
-
-
-        _safe_dump_d = ymlparsers._safe_dump_d
-        assert _safe_dump_d is not None
-        b= isinstance(_safe_dump_d, collections.abc.Mapping)
-        pytest.assume(b)
-
-        for k, exp_v in {'default_flow_style':False,
-                         'sort_keys':False}.items():
-            v = _safe_dump_d[k]
-            pytest.assume(exp_v==v)
-
-        pytest.assume("TODO: HiYaPyCo._substmerge() bug workarround, see https://github.com/zerwes/hiyapyco/pull/38",
-                      HiYaPyCo._deepmerge==HiYaPyCo._substmerge)
-
-    @pytest.mark.yml
-    def test_initConfig_other_params(self, request, mocker, ymlparsersCleanup):
-        logger.info(f'{request._pyfuncitem.name}()')
-
-        mock_lock = create_mock_lock(mocker)
-
-        p_load = {'method':METHOD_SIMPLE,
-               'mergelists':True,
-               'interpolate':False,
-               'castinterpolated':False}
-
-        p_safe_dump = {'default_flow_style':True,
-                       'sort_keys':True}
-
-        p_undefined = StrictUndefined
-
-        dumb = lambda:None
-
-        p_globals = {"foo":dumb,
-                     "uname":dumb}
-
-        ymlparsers.initConfig(jinja2Lock=mock_lock,
-                              jinja2ctx={'undefined':p_undefined,
-                                         'globals':p_globals
-                                         },
-                              load=p_load,
-                              safe_dump=p_safe_dump
-                              )
-        lock = HiYaPyCo.jinja2Lock
-        pytest.assume(lock is not None)
-        pytest.assume(lock==mock_lock)
-
-        pytest.assume(mock_lock.acquire.call_count > 0)
-        pytest.assume(mock_lock.release.call_count == mock_lock.acquire.call_count)
-
-        jinja2Env = HiYaPyCo.jinja2ctx
-        pytest.assume(jinja2Env is not None)
-
-        jinja2EnvUndefined = jinja2Env.undefined
-        b = issubclass(jinja2EnvUndefined, p_undefined)
-        pytest.assume(b)
-
-        jinja2EnvGloblas = jinja2Env.globals
-        f= jinja2EnvGloblas['uname']
-        pytest.assume(f==dumb)
-        f = jinja2EnvGloblas['foo']
-        pytest.assume(f == dumb)
-
-        _load_d = ymlparsers._load_d
-        assert _load_d is not None
-        b = isinstance(_load_d, collections.abc.Mapping)
-        pytest.assume(b)
-
-        for k, exp_v in p_load.items():
-            v = _load_d[k]
-            pytest.assume(exp_v ==v)
-
-        _safe_dump_d = ymlparsers._safe_dump_d
-        assert _safe_dump_d is not None
-        b = isinstance(_safe_dump_d, collections.abc.Mapping)
-        pytest.assume(b)
-
-        for k, exp_v in p_safe_dump.items():
-            v = _safe_dump_d[k]
-            pytest.assume(exp_v == v)
-
-class TestDisableVarSubst(object):
-
-    @pytest.mark.yml
-    def test_intented_usage(self, request, mocker, ymlparsersSetup, ymlparsersCleanup, exp_config_d):
-        logger.info(f'{request._pyfuncitem.name}()')
-
-        mock_lock = create_mock_lock(mocker)
-
-        orig_jinja2ctx = HiYaPyCo.jinja2ctx
-
-        mocker.patch.object(HiYaPyCo, 'jinja2Lock', new=mock_lock, spec_set=True)
-        jinja2ctx_mock = mocker.patch.object(HiYaPyCo, 'jinja2ctx', spec_set=True)
-
-        mock_variable_start_string = mocker.PropertyMock(return_value=orig_jinja2ctx.variable_start_string)
-        type(jinja2ctx_mock).variable_start_string = mock_variable_start_string
-        mock_variable_end_string = mocker.PropertyMock(return_value=orig_jinja2ctx.variable_end_string)
-        type(jinja2ctx_mock).variable_end_string = mock_variable_end_string
-        mock_block_start_string = mocker.PropertyMock(return_value=orig_jinja2ctx.block_start_string)
-        type(jinja2ctx_mock).block_start_string = mock_block_start_string
-        mock_block_end_string = mocker.PropertyMock(return_value=orig_jinja2ctx.block_end_string)
-        type(jinja2ctx_mock).block_end_string = mock_block_end_string
-
-        mocks = [mock_variable_start_string, mock_variable_end_string, mock_block_start_string, mock_block_end_string]
-
-        # orig_exit = ymlparsers.DisableVarSubst.__exit__
-        # mock_exit = mocker.patch.object(ymlparsers.DisableVarSubst, '__exit__', side_effect=orig_exit,
-        #                                 autospec=True, spec_set=True)
-
-
-
-        with ymlparsers.DisableVarSubst():
-            logger.debug("dff")
-            pass
-
-        # pytest.assume(mock_exit.call_count == 1)
-        pytest.assume(mock_lock.acquire.call_count > 0)
-        pytest.assume(mock_lock.release.call_count == mock_lock.acquire.call_count)
-
-        setter_called = None
-        for mock in mocks:
-            setter_called = None
-            pytest.assume(mock.call_count > 0)
-            for kall in mock.call_args_list:
-                #(param,), _ = kall
-                args, _ = kall
-                if not is_empty(args) and '|' in args[0]:
-                    setter_called = True
-                    break
-            pytest.assume(setter_called)
-
-        pytest.assume(jinja2ctx_mock.variable_start_string == orig_jinja2ctx.variable_start_string)
-        pytest.assume(jinja2ctx_mock.variable_end_string == orig_jinja2ctx.variable_end_string)
-        pytest.assume(jinja2ctx_mock.block_start_string == orig_jinja2ctx.block_start_string)
-        pytest.assume(jinja2ctx_mock.block_end_string == orig_jinja2ctx.block_end_string)
-
-    class DummyEnvironment(object):
-        def __init__(self, *args, **kwargs):
-            self.delegate = kwargs['delegate']
-            self._variable_start_string = self.delegate.variable_start_string
-            self._variable_end_string = self.delegate.variable_end_string
-            self._block_start_string =  self.delegate.block_start_string
-            self._block_end_string = self.delegate.block_end_string
-            self.raiseAlways = kwargs.get('raiseAlways', False)
-
-        @property
-        def variable_start_string(self):
-            return self._variable_start_string
-
-        @variable_start_string.setter
-        def variable_start_string(self, new_name):
-            self._variable_start_string = new_name
-
-        @property
-        def variable_end_string(self):
-            return self._variable_end_string
-
-        @variable_end_string.setter
-        def variable_end_string(self, new_name):
-            self._variable_end_string = new_name
-
-        @property
-        def block_start_string(self):
-            return self._block_start_string
-
-        @block_start_string.setter
-        def block_start_string(self, new_name):
-            self._block_start_string = new_name
-
-        @property
-        def block_end_string(self):
-            return self._block_end_string
-
-        @block_end_string.setter
-        def block_end_string(self, new_name):
-            if self.raiseAlways or ('|' not in new_name):
-                raise ValueError
-            self._block_end_string = new_name
-
-    @pytest.mark.yml
-    def test_exception_in_exit(self, request, mocker, ymlparsersSetup, ymlparsersCleanup, exp_config_d):
-        logger.info(f'{request._pyfuncitem.name}()')
-        #I check 2 things
-        #1. Explicately passing params
-        #2. Releasing lock even if exception occures in DisableVarSubst. __exit__
-
-        mock_lock = create_mock_lock(mocker)
-
-        orig_jinja2ctx = HiYaPyCo.jinja2ctx
-        duumy_jinja2ctx = TestDisableVarSubst.DummyEnvironment(delegate=orig_jinja2ctx)
-
-        #orig_exit = ymlparsers.DisableVarSubst.__exit__
-        # mock_exit = mocker.patch.object(ymlparsers.DisableVarSubst, '__exit__', side_effect=orig_exit,
-        #                                 autospec=True, spec_set=True)
-
-        with pytest.raises(ValueError):
-            with ymlparsers.DisableVarSubst(jinja2ctx=duumy_jinja2ctx, jinja2Lock=mock_lock):
-                pass
-
-        # pytest.assume(mock_exit.call_count == 1)
-        pytest.assume(mock_lock.acquire.call_count > 0)
-        pytest.assume(mock_lock.release.call_count == mock_lock.acquire.call_count)
-
-        pytest.assume(duumy_jinja2ctx != orig_jinja2ctx)
-        pytest.assume(mock_lock != orig_jinja2ctx)
-
-        pytest.assume(duumy_jinja2ctx.variable_start_string == orig_jinja2ctx.variable_start_string)
-        pytest.assume(duumy_jinja2ctx.variable_end_string == orig_jinja2ctx.variable_end_string)
-        pytest.assume(duumy_jinja2ctx.block_start_string == orig_jinja2ctx.block_start_string)
-        pytest.assume(duumy_jinja2ctx.block_end_string !=  orig_jinja2ctx.block_end_string )
-
-    @pytest.mark.yml
-    def test_exception_in_enter(self, request, mocker, ymlparsersSetup, ymlparsersCleanup, exp_config_d):
-        logger.info(f'{request._pyfuncitem.name}()')
-        #I check 2 things
-        #1. Explicately passing params
-        #2. Releasing lock even if exception occures in DisableVarSubst.__enter__
-
-        mock_lock = create_mock_lock(mocker)
-
-        orig_jinja2ctx = HiYaPyCo.jinja2ctx
-        duumy_jinja2ctx = TestDisableVarSubst.DummyEnvironment(delegate=orig_jinja2ctx, raiseAlways=True)
-
-        # orig_exit = ymlparsers.DisableVarSubst.__exit__
-        # mock_exit = mocker.patch.object(ymlparsers.DisableVarSubst, '__exit__', side_effect=orig_exit,
-        #                     autospec=True, spec_set=True)
-
-
-        with pytest.raises(ValueError):
-            with ymlparsers.DisableVarSubst(jinja2ctx=duumy_jinja2ctx, jinja2Lock=mock_lock):
-                pass
-
-        # pytest.assume(mock_exit.call_count == 0)
-        pytest.assume(mock_lock.acquire.call_count > 0)
-        pytest.assume(mock_lock.release.call_count == mock_lock.acquire.call_count)
-
-        pytest.assume(duumy_jinja2ctx != orig_jinja2ctx)
-        pytest.assume(mock_lock != orig_jinja2ctx)
-
-        pytest.assume(duumy_jinja2ctx.variable_start_string != orig_jinja2ctx.variable_start_string)
-        pytest.assume(duumy_jinja2ctx.variable_end_string != orig_jinja2ctx.variable_end_string)
-        pytest.assume(duumy_jinja2ctx.block_start_string != orig_jinja2ctx.block_start_string)
-        pytest.assume(duumy_jinja2ctx.block_end_string == orig_jinja2ctx.block_end_string)
-
-    @pytest.mark.yml
-    def test_exception_in_code(self, request, mocker, ymlparsersSetup, ymlparsersCleanup, exp_config_d):
-        logger.info(f'{request._pyfuncitem.name}()')
-        #I check 2 things
-        #1. Explicately passing params
-        #2. Releasing lock even if exception occures in the with
-
-        mock_lock = create_mock_lock(mocker)
-
-        orig_jinja2ctx = HiYaPyCo.jinja2ctx
-
-        mocker.patch.object(HiYaPyCo, 'jinja2Lock', new=mock_lock, spec_set=True)
-        jinja2ctx_mock = mocker.patch.object(HiYaPyCo, 'jinja2ctx', spec_set=True)
-
-        mock_variable_start_string = mocker.PropertyMock(return_value=orig_jinja2ctx.variable_start_string)
-        type(jinja2ctx_mock).variable_start_string = mock_variable_start_string
-        mock_variable_end_string = mocker.PropertyMock(return_value=orig_jinja2ctx.variable_end_string)
-        type(jinja2ctx_mock).variable_end_string = mock_variable_end_string
-        mock_block_start_string = mocker.PropertyMock(return_value=orig_jinja2ctx.block_start_string)
-        type(jinja2ctx_mock).block_start_string = mock_block_start_string
-        mock_block_end_string = mocker.PropertyMock(return_value=orig_jinja2ctx.block_end_string)
-        type(jinja2ctx_mock).block_end_string = mock_block_end_string
-
-        mocks = [mock_variable_start_string, mock_variable_end_string, mock_block_start_string, mock_block_end_string]
-        # orig_exit = ymlparsers.DisableVarSubst.__exit__
-        # mock_exit = mocker.patch.object(ymlparsers.DisableVarSubst, '__exit__', side_effect=orig_exit,
-        #                                 autospec=True, spec_set=True)
-
-        with pytest.raises(ValueError):
-            with ymlparsers.DisableVarSubst():
-                raise ValueError
-
-        # pytest.assume(mock_exit.call_count == 1)
-        pytest.assume(mock_lock.acquire.call_count > 0)
-        pytest.assume(mock_lock.release.call_count == mock_lock.acquire.call_count)
-
-        setter_called = None
-        for mock in mocks:
-            setter_called = None
-            pytest.assume(mock.call_count > 0)
-            for kall in mock.call_args_list:
-                # (param,), _ = kall
-                args, _ = kall
-                if not is_empty(args) and '|' in args[0]:
-                    setter_called = True
-                    break
-            pytest.assume(setter_called)
-
-        pytest.assume(jinja2ctx_mock.variable_start_string == orig_jinja2ctx.variable_start_string)
-        pytest.assume(jinja2ctx_mock.variable_end_string == orig_jinja2ctx.variable_end_string)
-        pytest.assume(jinja2ctx_mock.block_start_string == orig_jinja2ctx.block_start_string)
-        pytest.assume(jinja2ctx_mock.block_end_string == orig_jinja2ctx.block_end_string)
-
-
-@pytest.mark.yml
-def test_ymlparsers_load_single_no_substition(request, mocker, ymlparsersSetup, ymlparsersCleanup, exp_config_d):
-    logger.info(f'{request._pyfuncitem.name}()')
-
-    pck = '.'.join(['tests_data', __package__, 'ymlparsers'])
-
-    mock_lock = create_mock_lock(mocker)
-    mocker.patch.object(HiYaPyCo, 'jinja2Lock', new=mock_lock, spec_set=True)
-
-    with path(pck, 'config.yml') as full_path:
-        with ymlparsers.DisableVarSubst():
-            default_d = ymlparsers.load([str(full_path)])
-
-    # ymlparsers.load() when uses HiYaPyCo.jinja2ctx uses HiYaPyCo.jinja2Lock
-    # note, that ymlparsers.DisableVarSubst also use 1 time HiYaPyCo.jinja2Lock
-    pytest.assume(mock_lock.acquire.call_count > 1)
-    pytest.assume(mock_lock.release.call_count == mock_lock.acquire.call_count)
-
-
-    app_d = default_d.get('app', None)
-    exp_d = copy.deepcopy(exp_config_d)
-    exp_app_d = exp_d.get('app', None)
-
-    inner_host_name = app_d.get('inner_host_name', None)
-    exp_host_name = exp_app_d.get('inner_host_name', None)
-    pytest.assume(exp_host_name==inner_host_name)
-    cli_template = app_d.get('cli_template')
-    pytest.assume('inner_host_name' in cli_template)
-    pytest.assume(exp_config_d==default_d)
-
-
-@pytest.mark.yml
-def test_ymlparsers_load_single_with_substition(request, mocker, ymlparsersSetup, ymlparsersCleanup, exp_config_d):
-    logger.info(f'{request._pyfuncitem.name}()')
-
-    pck = '.'.join(['tests_data', __package__, 'ymlparsers'])
-
-
-    mock_lock = create_mock_lock(mocker)
-    mocker.patch.object(HiYaPyCo, 'jinja2Lock', new=mock_lock, spec_set=True)
-
-    with path(pck, 'config.yml') as full_path:
-        default_d = ymlparsers.load([str(full_path)])
-
-    pytest.assume(mock_lock.acquire.call_count > 1)
-    pytest.assume(mock_lock.release.call_count == mock_lock.acquire.call_count)
-
-    app_d = default_d['app']
-    exp_d = copy.deepcopy(exp_config_d)
-    exp_app_d = exp_d.get('app', None)
-
-    inner_host_name = app_d.get('inner_host_name', None)
-    exp_host_name = exp_app_d.get('inner_host_name', None)
-    pytest.assume(exp_host_name==inner_host_name)
-
-    exp_cli_template = exp_app_d.get('cli_template', None)
-    exp_cli_template = format_template(exp_cli_template, app_inner_host_name=exp_host_name)
-    exp_app_d['cli_template']=exp_cli_template
-
-
-    cli_template = app_d.get('cli_template')
-    pytest.assume('inner_host_name' not in cli_template)
-
-    cli_template = app_d['cli_template']
-    pytest.assume('inner_host_name' not in cli_template)
-    pytest.assume(exp_d==default_d)
-
-    white_list = app_d.get('white_list', None)
-    exp_white_list = exp_app_d.get('white_list', None)
-    pytest.assume(exp_white_list==white_list)
-
-
-#order is non-alephabetic intentionally
-_data_list = {'profiles': ['local', 'dev']}
-_data_dict = {'general':
-                 { 'whiteListSysOverrideKeys': ['app'],
-                   'profiles': ['local', 'dev']},
-              'app':
-                  {'host_name': 'google.com'},
-             }
-
-@pytest.mark.parametrize(
-     'data, kwds',
-
-    [
-        (_data_list, {}),
-
-        #sort_key is ignored
-        (_data_list, {'default_flow_style': None,  'sort_keys': True}),
-        (_data_list, {'default_flow_style': False, 'sort_keys': True}),
-        (_data_list, {'default_flow_style': True,  'sort_keys': True}),
-
-        (_data_dict, {'default_flow_style': None,  'sort_keys': True}),
-        (_data_dict, {'default_flow_style': False, 'sort_keys': True}),
-        (_data_dict, {'default_flow_style': True,  'sort_keys': True}),
-
-    ]
-)
-@pytest.mark.yml
-def test_safe_dump_composite(request, mocker, ymlparsersSetup, ymlparsersCleanup, data, kwds):
-    logger.info(f'{request._pyfuncitem.name}()')
-
-    default_flow_style = kwds.get('default_flow_style', False)
-
-    with io.StringIO() as buf:
-        ymlparsers.safe_dump(data, stream=buf, **kwds)
-        value = buf.getvalue()
-        logger.debug(value)
-        if default_flow_style is not None and not default_flow_style:
-            pytest.assume('-' in value)
-        else:
-            pytest.assume('[' in value)
-            pytest.assume(']' in value)
-
-        with ymlparsers.DisableVarSubst():
-            restored_d = ymlparsers.load(value)
-
-    pytest.assume(data == restored_d)
-
-@pytest.mark.yml
-def test_safe_dump(request, mocker, ymlparsersSetup, ymlparsersCleanup, exp_config_d):
-    logger.info(f'{request._pyfuncitem.name}()')
-
-    orig_d = dict(exp_config_d)
-    d = OrderedDict(exp_config_d)
-    d['general'] = OrderedDict(d['general'])
-    d['app'] = OrderedDict(d['app'])
-
-    with io.StringIO() as buf:
-        ymlparsers.safe_dump(d, stream=buf)
-        value = buf.getvalue()
-
-    with ymlparsers.DisableVarSubst():
-        restored_d = ymlparsers.load(value)
-
-    pytest.assume(orig_d==restored_d)
-
-@pytest.mark.yml
-def test_as_str(request, mocker, ymlparsersSetup, ymlparsersCleanup, exp_config_d):
-    logger.info(f'{request._pyfuncitem.name}()')
-
-    orig_d = dict(exp_config_d)
-    d = OrderedDict(exp_config_d)
-    d['general'] = OrderedDict(d['general'])
-    d['app'] = OrderedDict(d['app'])
-
-    orig_safe_dump = ymlparsers.safe_dump
-    mock_safe_dump = mocker.patch.object(ymlparsers, 'safe_dump', side_effect=orig_safe_dump,
-                                    autospec=True, spec_set=True)
-
-    value = ymlparsers.as_str(d)
-    pytest.assume(mock_safe_dump.call_count > 0)
-
-    with ymlparsers.DisableVarSubst():
-        restored_d = ymlparsers.load(value)
-
-    pytest.assume(orig_d==restored_d)
-
-@pytest.mark.yml
-def test_ymlparsers_load_multiple_no_substition(request, mocker, ymlparsersSetup, ymlparsersCleanup, exp_config_d):
-    logger.info(f'{request._pyfuncitem.name}()')
-
-    exp_d = copy.deepcopy(exp_config_d)
-    exp_d['general']['log']['formatters']['detail'] = {'format': \
-                                                '%(asctime)-14s %(levelname)s [%(name)s.%(funcName)s] %(message)s',
-                                                       'datefmt': \
-                                                '%Y-%m-%d %H:%M:%S'}
-    exp_d['general']['log']['root']['level'] = 'INFO'
-    exp_d['app']['inner_host_name'] = 'yahoo.com'
-    exp_d['app']['white_list'] = ['gamma', 'alpha', 'betha']
-    exp_d['app']['alt_white_list'] = ['c', 'b', 'a']
-
-
-
-    pck = '.'.join(['tests_data', __package__, 'ymlparsers'])
-
-    with path(pck, 'config.yml') as full_path:
-        with path(pck, 'config-dev.yml') as full_dev_path:
-            with ymlparsers.DisableVarSubst():
-                default_d = ymlparsers.load([str(full_path), str(full_dev_path)])
-
-
-    app_d = default_d.get('app', None)
-    exp_app_d = exp_d.get('app', None)
-
-    inner_host_name = app_d.get('inner_host_name', None)
-    exp_host_name = exp_app_d.get('inner_host_name', None)
-    pytest.assume(exp_host_name==inner_host_name)
-
-    cli_template = app_d.get('cli_template')
-    pytest.assume('inner_host_name' in cli_template)
-
-    pytest.assume(exp_d==default_d)
-
-@pytest.mark.yml
-def test_ymlparsers_load_multiple_with_substition(request, mocker, ymlparsersSetup, ymlparsersCleanup, exp_config_d):
-    logger.info(f'{request._pyfuncitem.name}()')
-
-    pck = '.'.join(['tests_data', __package__, 'ymlparsers'])
-
-    exp_d = copy.deepcopy(exp_config_d)
-    exp_d['general']['log']['formatters']['detail'] = {'format': \
-                                                           '%(asctime)-14s %(levelname)s [%(name)s.%(funcName)s] %(message)s',
-                                                       'datefmt': \
-                                                           '%Y-%m-%d %H:%M:%S'}
-    exp_d['general']['log']['root']['level'] = 'INFO'
-    exp_d['app']['inner_host_name'] = 'yahoo.com'
-    exp_d['app']['white_list'] = ['gamma', 'alpha', 'betha']
-    exp_d['app']['alt_white_list'] = ['c', 'b', 'a']
-
-    with path(pck, 'config.yml') as full_path:
-        with path(pck, 'config-dev.yml') as full_dev_path:
-            default_d = ymlparsers.load([str(full_path), str(full_dev_path)])
-
-
-    app_d = default_d['app']
-    exp_app_d = exp_d.get('app', None)
-
-    inner_host_name = app_d.get('inner_host_name', None)
-    exp_host_name = exp_app_d.get('inner_host_name', None)
-    pytest.assume(exp_host_name==inner_host_name)
-
-    exp_cli_template = exp_app_d.get('cli_template', None)
-    exp_cli_template = format_template(exp_cli_template, app_inner_host_name=exp_host_name)
-    exp_app_d['cli_template']=exp_cli_template
-
-
-    cli_template = app_d.get('cli_template')
-    pytest.assume('inner_host_name' not in cli_template)
-
-    cli_template = app_d['cli_template']
-    pytest.assume('inner_host_name' not in cli_template)
-
-    pytest.assume(exp_d==default_d)
-
-
-def _run_without_substition(content, exp_config_d, stop):
-    for i in range(stop):
-        with ymlparsers.DisableVarSubst():
-            default_d = ymlparsers.load([str(content)])
-
-            app_d = default_d.get('app', None)
-            exp_app_d = exp_config_d.get('app', None)
-
-            inner_host_name = app_d.get('inner_host_name', None)
-            exp_host_name = exp_app_d.get('inner_host_name', None)
-            pytest.assume(exp_host_name==inner_host_name)
-            cli_template = app_d.get('cli_template')
-            pytest.assume('inner_host_name' in cli_template)
-            pytest.assume(exp_config_d == default_d)
-
-def _run_with_substition(content, exp_config_d, stop):
-    for i in range(stop):
-        default_d = ymlparsers.load([str(content)])
-
-        app_d = default_d['app']
-        exp_app_d = exp_config_d.get('app', None)
-
-        inner_host_name = app_d.get('inner_host_name', None)
-        exp_host_name = exp_app_d.get('inner_host_name', None)
-        pytest.assume(exp_host_name==inner_host_name)
-
-        exp_cli_template = exp_app_d.get('cli_template', None)
-        exp_cli_template = format_template(exp_cli_template, app_inner_host_name=exp_host_name)
-
-        exp_app_d['cli_template'] = exp_cli_template
-
-        cli_template = app_d.get('cli_template')
-        pytest.assume('inner_host_name' not in cli_template)
-
-        cli_template = app_d['cli_template']
-        pytest.assume('inner_host_name' not in cli_template)
-        pytest.assume(exp_config_d == default_d)
-
-@pytest.mark.yml
-def test_ymlparsers_load_it(request, mocker, ymlparsersSetup, ymlparsersCleanup, exp_config_d):
-    logger.info(f'{request._pyfuncitem.name}()')
-    pck = '.'.join(['tests_data', __package__, 'ymlparsers'])
-
-    with path(pck, 'config.yml') as full_path:
-        with open(full_path, 'r') as f:
-            content = f.read()
-
-    stop = 10
-
-    exp_d = copy.deepcopy(exp_config_d)
-    exp_app_d = dict(exp_d.get('app', None))
-    if exp_app_d is not None:
-        exp_d['app'] = exp_app_d
-
-    exp_host_name = exp_app_d.get('inner_host_name', None)
-    exp_cli_template = exp_app_d.get('cli_template', None)
-    exp_cli_template = format_template(exp_cli_template, app_inner_host_name=exp_host_name)
-    exp_app_d['cli_template'] = exp_cli_template
-
-
-    th1 = threading.Thread(name="run_with_substition",
-        target=_run_with_substition, args=(content, exp_d, stop))
-
-    th2 = threading.Thread(name="run_without_substition",
-                           target=_run_without_substition, args=(str(content), copy.deepcopy(exp_config_d), stop))
-
-    th1.start()
-    time.sleep(2)
-    th2.start()
-    th1.join()
-    th2.join()
-
-
-if __name__ == "__main__":
-    pytest.main([__file__])
+import logging
+import time
+import threading
+import pytest
+import copy
+
+logger = logging.getLogger(__name__)
+
+from importlib.resources import path
+
+import collections
+from collections import OrderedDict
+import io
+import yaml
+from yaml import FullLoader
+from alexber.utils.inspects import has_method
+from alexber.utils._ymlparsers_extra import format_template
+
+
+try:
+    import alexber.utils.ymlparsers as ymlparsers
+    from alexber.utils.ymlparsers import HiYaPyCo
+    from alexber.utils.parsers import is_empty
+    from jinja2 import DebugUndefined, StrictUndefined, Environment
+    from hiyapyco import METHOD_SUBSTITUTE, METHOD_SIMPLE
+except ImportError:
+    pass
+
+def _reset_ymlparsers():
+    ymlparsers.HiYaPyCo.jinja2Lock = None
+    ymlparsers.HiYaPyCo.jinja2ctx = None
+    ymlparsers._load_d = None
+    ymlparsers._safe_dump_d = None
+
+@pytest.fixture
+@pytest.mark.yml
+def ymlparsersSetup(mocker):
+    _reset_ymlparsers()
+
+    ymlparsers.initConfig()
+
+@pytest.fixture(scope='session')
+@pytest.mark.yml
+def exp_config_d():
+    pck = '.'.join(['tests_data', __package__, 'ymlparsers'])
+
+    with path(pck, 'config.yml') as full_path:
+        with open(full_path, 'r') as f:
+            exp_d = yaml.load(f, FullLoader)
+    return exp_d
+
+
+
+@pytest.fixture
+@pytest.mark.yml
+def ymlparsersCleanup(mocker):
+    yield None
+    _reset_ymlparsers()
+
+class DymmyLock(object):
+    def acquire(self, blocking=True):
+        pass
+
+    def release(self):
+        pass
+
+def create_mock_lock(mocker):
+    mock_lock = DymmyLock()
+
+    def __enter__():
+        mock_lock.acquire()
+        return mock_lock
+
+    def __exit__(t, v, tb):
+        mock_lock.release()
+
+    mocker.patch.object(mock_lock, 'acquire', autospec=True, spec_set=True)
+    mocker.patch.object(mock_lock, 'release', autospec=True, spec_set=True)
+    mocker.patch.object(type(mock_lock), '__enter__', side_effect=__enter__, create=True)
+    mocker.patch.object(type(mock_lock), '__exit__', side_effect=__exit__, create=True)
+    return mock_lock
+
+
+class TestYmlparsersInit(object):
+    @pytest.mark.yml
+    def test_initConfig_default_params(self, request, mocker, ymlparsersCleanup):
+        logger.info(f'{request._pyfuncitem.name}()')
+        ymlparsers.initConfig()
+        lock = HiYaPyCo.jinja2Lock
+        pytest.assume(lock is not None)
+        lock_cls = type(lock)
+        b = has_method(lock_cls, 'acquire')
+        pytest.assume(b)
+        b = has_method(lock_cls, 'release')
+        pytest.assume(b)
+
+        jinja2Env = HiYaPyCo.jinja2ctx
+        pytest.assume(jinja2Env is not None)
+
+        jinja2EnvUndefined = jinja2Env.undefined
+        b = issubclass(jinja2EnvUndefined,DebugUndefined)
+        pytest.assume(b)
+
+        jinja2EnvGloblas = jinja2Env.globals
+        b = 'uname' in jinja2EnvGloblas
+        pytest.assume(b)
+
+        _load_d = ymlparsers._load_d
+        assert _load_d is not None
+        b = isinstance(_load_d, collections.abc.Mapping)
+        pytest.assume(b)
+
+        for k, exp_v in {'method':METHOD_SUBSTITUTE,
+                     'mergelists':False,
+                     'interpolate':True,
+                     'castinterpolated':True}.items():
+            v = _load_d[k]
+            pytest.assume(exp_v==v)
+
+
+        _safe_dump_d = ymlparsers._safe_dump_d
+        assert _safe_dump_d is not None
+        b= isinstance(_safe_dump_d, collections.abc.Mapping)
+        pytest.assume(b)
+
+        for k, exp_v in {'default_flow_style':False,
+                         'sort_keys':False}.items():
+            v = _safe_dump_d[k]
+            pytest.assume(exp_v==v)
+
+        pytest.assume("TODO: HiYaPyCo._substmerge() bug workarround, see https://github.com/zerwes/hiyapyco/pull/38",
+                      HiYaPyCo._deepmerge==HiYaPyCo._substmerge)
+
+    @pytest.mark.yml
+    def test_initConfig_other_params(self, request, mocker, ymlparsersCleanup):
+        logger.info(f'{request._pyfuncitem.name}()')
+
+        mock_lock = create_mock_lock(mocker)
+
+        p_load = {'method':METHOD_SIMPLE,
+               'mergelists':True,
+               'interpolate':False,
+               'castinterpolated':False}
+
+        p_safe_dump = {'default_flow_style':True,
+                       'sort_keys':True}
+
+        p_undefined = StrictUndefined
+
+        dumb = lambda:None
+
+        p_globals = {"foo":dumb,
+                     "uname":dumb}
+
+        ymlparsers.initConfig(jinja2Lock=mock_lock,
+                              jinja2ctx={'undefined':p_undefined,
+                                         'globals':p_globals
+                                         },
+                              load=p_load,
+                              safe_dump=p_safe_dump
+                              )
+        lock = HiYaPyCo.jinja2Lock
+        pytest.assume(lock is not None)
+        pytest.assume(lock==mock_lock)
+
+        pytest.assume(mock_lock.acquire.call_count > 0)
+        pytest.assume(mock_lock.release.call_count == mock_lock.acquire.call_count)
+
+        jinja2Env = HiYaPyCo.jinja2ctx
+        pytest.assume(jinja2Env is not None)
+
+        jinja2EnvUndefined = jinja2Env.undefined
+        b = issubclass(jinja2EnvUndefined, p_undefined)
+        pytest.assume(b)
+
+        jinja2EnvGloblas = jinja2Env.globals
+        f= jinja2EnvGloblas['uname']
+        pytest.assume(f==dumb)
+        f = jinja2EnvGloblas['foo']
+        pytest.assume(f == dumb)
+
+        _load_d = ymlparsers._load_d
+        assert _load_d is not None
+        b = isinstance(_load_d, collections.abc.Mapping)
+        pytest.assume(b)
+
+        for k, exp_v in p_load.items():
+            v = _load_d[k]
+            pytest.assume(exp_v ==v)
+
+        _safe_dump_d = ymlparsers._safe_dump_d
+        assert _safe_dump_d is not None
+        b = isinstance(_safe_dump_d, collections.abc.Mapping)
+        pytest.assume(b)
+
+        for k, exp_v in p_safe_dump.items():
+            v = _safe_dump_d[k]
+            pytest.assume(exp_v == v)
+
+class TestDisableVarSubst(object):
+
+    @pytest.mark.yml
+    def test_intented_usage(self, request, mocker, ymlparsersSetup, ymlparsersCleanup, exp_config_d):
+        logger.info(f'{request._pyfuncitem.name}()')
+
+        mock_lock = create_mock_lock(mocker)
+
+        orig_jinja2ctx = HiYaPyCo.jinja2ctx
+
+        mocker.patch.object(HiYaPyCo, 'jinja2Lock', new=mock_lock, spec_set=True)
+        jinja2ctx_mock = mocker.patch.object(HiYaPyCo, 'jinja2ctx', spec_set=True)
+
+        mock_variable_start_string = mocker.PropertyMock(return_value=orig_jinja2ctx.variable_start_string)
+        type(jinja2ctx_mock).variable_start_string = mock_variable_start_string
+        mock_variable_end_string = mocker.PropertyMock(return_value=orig_jinja2ctx.variable_end_string)
+        type(jinja2ctx_mock).variable_end_string = mock_variable_end_string
+        mock_block_start_string = mocker.PropertyMock(return_value=orig_jinja2ctx.block_start_string)
+        type(jinja2ctx_mock).block_start_string = mock_block_start_string
+        mock_block_end_string = mocker.PropertyMock(return_value=orig_jinja2ctx.block_end_string)
+        type(jinja2ctx_mock).block_end_string = mock_block_end_string
+
+        mocks = [mock_variable_start_string, mock_variable_end_string, mock_block_start_string, mock_block_end_string]
+
+        # orig_exit = ymlparsers.DisableVarSubst.__exit__
+        # mock_exit = mocker.patch.object(ymlparsers.DisableVarSubst, '__exit__', side_effect=orig_exit,
+        #                                 autospec=True, spec_set=True)
+
+
+
+        with ymlparsers.DisableVarSubst():
+            logger.debug("dff")
+            pass
+
+        # pytest.assume(mock_exit.call_count == 1)
+        pytest.assume(mock_lock.acquire.call_count > 0)
+        pytest.assume(mock_lock.release.call_count == mock_lock.acquire.call_count)
+
+        setter_called = None
+        for mock in mocks:
+            setter_called = None
+            pytest.assume(mock.call_count > 0)
+            for kall in mock.call_args_list:
+                #(param,), _ = kall
+                args, _ = kall
+                if not is_empty(args) and '|' in args[0]:
+                    setter_called = True
+                    break
+            pytest.assume(setter_called)
+
+        pytest.assume(jinja2ctx_mock.variable_start_string == orig_jinja2ctx.variable_start_string)
+        pytest.assume(jinja2ctx_mock.variable_end_string == orig_jinja2ctx.variable_end_string)
+        pytest.assume(jinja2ctx_mock.block_start_string == orig_jinja2ctx.block_start_string)
+        pytest.assume(jinja2ctx_mock.block_end_string == orig_jinja2ctx.block_end_string)
+
+    class DummyEnvironment(object):
+        def __init__(self, *args, **kwargs):
+            self.delegate = kwargs['delegate']
+            self._variable_start_string = self.delegate.variable_start_string
+            self._variable_end_string = self.delegate.variable_end_string
+            self._block_start_string =  self.delegate.block_start_string
+            self._block_end_string = self.delegate.block_end_string
+            self.raiseAlways = kwargs.get('raiseAlways', False)
+
+        @property
+        def variable_start_string(self):
+            return self._variable_start_string
+
+        @variable_start_string.setter
+        def variable_start_string(self, new_name):
+            self._variable_start_string = new_name
+
+        @property
+        def variable_end_string(self):
+            return self._variable_end_string
+
+        @variable_end_string.setter
+        def variable_end_string(self, new_name):
+            self._variable_end_string = new_name
+
+        @property
+        def block_start_string(self):
+            return self._block_start_string
+
+        @block_start_string.setter
+        def block_start_string(self, new_name):
+            self._block_start_string = new_name
+
+        @property
+        def block_end_string(self):
+            return self._block_end_string
+
+        @block_end_string.setter
+        def block_end_string(self, new_name):
+            if self.raiseAlways or ('|' not in new_name):
+                raise ValueError
+            self._block_end_string = new_name
+
+    @pytest.mark.yml
+    def test_exception_in_exit(self, request, mocker, ymlparsersSetup, ymlparsersCleanup, exp_config_d):
+        logger.info(f'{request._pyfuncitem.name}()')
+        #I check 2 things
+        #1. Explicately passing params
+        #2. Releasing lock even if exception occures in DisableVarSubst. __exit__
+
+        mock_lock = create_mock_lock(mocker)
+
+        orig_jinja2ctx = HiYaPyCo.jinja2ctx
+        duumy_jinja2ctx = TestDisableVarSubst.DummyEnvironment(delegate=orig_jinja2ctx)
+
+        #orig_exit = ymlparsers.DisableVarSubst.__exit__
+        # mock_exit = mocker.patch.object(ymlparsers.DisableVarSubst, '__exit__', side_effect=orig_exit,
+        #                                 autospec=True, spec_set=True)
+
+        with pytest.raises(ValueError):
+            with ymlparsers.DisableVarSubst(jinja2ctx=duumy_jinja2ctx, jinja2Lock=mock_lock):
+                pass
+
+        # pytest.assume(mock_exit.call_count == 1)
+        pytest.assume(mock_lock.acquire.call_count > 0)
+        pytest.assume(mock_lock.release.call_count == mock_lock.acquire.call_count)
+
+        pytest.assume(duumy_jinja2ctx != orig_jinja2ctx)
+        pytest.assume(mock_lock != orig_jinja2ctx)
+
+        pytest.assume(duumy_jinja2ctx.variable_start_string == orig_jinja2ctx.variable_start_string)
+        pytest.assume(duumy_jinja2ctx.variable_end_string == orig_jinja2ctx.variable_end_string)
+        pytest.assume(duumy_jinja2ctx.block_start_string == orig_jinja2ctx.block_start_string)
+        pytest.assume(duumy_jinja2ctx.block_end_string !=  orig_jinja2ctx.block_end_string )
+
+    @pytest.mark.yml
+    def test_exception_in_enter(self, request, mocker, ymlparsersSetup, ymlparsersCleanup, exp_config_d):
+        logger.info(f'{request._pyfuncitem.name}()')
+        #I check 2 things
+        #1. Explicately passing params
+        #2. Releasing lock even if exception occures in DisableVarSubst.__enter__
+
+        mock_lock = create_mock_lock(mocker)
+
+        orig_jinja2ctx = HiYaPyCo.jinja2ctx
+        duumy_jinja2ctx = TestDisableVarSubst.DummyEnvironment(delegate=orig_jinja2ctx, raiseAlways=True)
+
+        # orig_exit = ymlparsers.DisableVarSubst.__exit__
+        # mock_exit = mocker.patch.object(ymlparsers.DisableVarSubst, '__exit__', side_effect=orig_exit,
+        #                     autospec=True, spec_set=True)
+
+
+        with pytest.raises(ValueError):
+            with ymlparsers.DisableVarSubst(jinja2ctx=duumy_jinja2ctx, jinja2Lock=mock_lock):
+                pass
+
+        # pytest.assume(mock_exit.call_count == 0)
+        pytest.assume(mock_lock.acquire.call_count > 0)
+        pytest.assume(mock_lock.release.call_count == mock_lock.acquire.call_count)
+
+        pytest.assume(duumy_jinja2ctx != orig_jinja2ctx)
+        pytest.assume(mock_lock != orig_jinja2ctx)
+
+        pytest.assume(duumy_jinja2ctx.variable_start_string != orig_jinja2ctx.variable_start_string)
+        pytest.assume(duumy_jinja2ctx.variable_end_string != orig_jinja2ctx.variable_end_string)
+        pytest.assume(duumy_jinja2ctx.block_start_string != orig_jinja2ctx.block_start_string)
+        pytest.assume(duumy_jinja2ctx.block_end_string == orig_jinja2ctx.block_end_string)
+
+    @pytest.mark.yml
+    def test_exception_in_code(self, request, mocker, ymlparsersSetup, ymlparsersCleanup, exp_config_d):
+        logger.info(f'{request._pyfuncitem.name}()')
+        #I check 2 things
+        #1. Explicately passing params
+        #2. Releasing lock even if exception occures in the with
+
+        mock_lock = create_mock_lock(mocker)
+
+        orig_jinja2ctx = HiYaPyCo.jinja2ctx
+
+        mocker.patch.object(HiYaPyCo, 'jinja2Lock', new=mock_lock, spec_set=True)
+        jinja2ctx_mock = mocker.patch.object(HiYaPyCo, 'jinja2ctx', spec_set=True)
+
+        mock_variable_start_string = mocker.PropertyMock(return_value=orig_jinja2ctx.variable_start_string)
+        type(jinja2ctx_mock).variable_start_string = mock_variable_start_string
+        mock_variable_end_string = mocker.PropertyMock(return_value=orig_jinja2ctx.variable_end_string)
+        type(jinja2ctx_mock).variable_end_string = mock_variable_end_string
+        mock_block_start_string = mocker.PropertyMock(return_value=orig_jinja2ctx.block_start_string)
+        type(jinja2ctx_mock).block_start_string = mock_block_start_string
+        mock_block_end_string = mocker.PropertyMock(return_value=orig_jinja2ctx.block_end_string)
+        type(jinja2ctx_mock).block_end_string = mock_block_end_string
+
+        mocks = [mock_variable_start_string, mock_variable_end_string, mock_block_start_string, mock_block_end_string]
+        # orig_exit = ymlparsers.DisableVarSubst.__exit__
+        # mock_exit = mocker.patch.object(ymlparsers.DisableVarSubst, '__exit__', side_effect=orig_exit,
+        #                                 autospec=True, spec_set=True)
+
+        with pytest.raises(ValueError):
+            with ymlparsers.DisableVarSubst():
+                raise ValueError
+
+        # pytest.assume(mock_exit.call_count == 1)
+        pytest.assume(mock_lock.acquire.call_count > 0)
+        pytest.assume(mock_lock.release.call_count == mock_lock.acquire.call_count)
+
+        setter_called = None
+        for mock in mocks:
+            setter_called = None
+            pytest.assume(mock.call_count > 0)
+            for kall in mock.call_args_list:
+                # (param,), _ = kall
+                args, _ = kall
+                if not is_empty(args) and '|' in args[0]:
+                    setter_called = True
+                    break
+            pytest.assume(setter_called)
+
+        pytest.assume(jinja2ctx_mock.variable_start_string == orig_jinja2ctx.variable_start_string)
+        pytest.assume(jinja2ctx_mock.variable_end_string == orig_jinja2ctx.variable_end_string)
+        pytest.assume(jinja2ctx_mock.block_start_string == orig_jinja2ctx.block_start_string)
+        pytest.assume(jinja2ctx_mock.block_end_string == orig_jinja2ctx.block_end_string)
+
+
+@pytest.mark.yml
+def test_ymlparsers_load_single_no_substition(request, mocker, ymlparsersSetup, ymlparsersCleanup, exp_config_d):
+    logger.info(f'{request._pyfuncitem.name}()')
+
+    pck = '.'.join(['tests_data', __package__, 'ymlparsers'])
+
+    mock_lock = create_mock_lock(mocker)
+    mocker.patch.object(HiYaPyCo, 'jinja2Lock', new=mock_lock, spec_set=True)
+
+    with path(pck, 'config.yml') as full_path:
+        with ymlparsers.DisableVarSubst():
+            default_d = ymlparsers.load([str(full_path)])
+
+    # ymlparsers.load() when uses HiYaPyCo.jinja2ctx uses HiYaPyCo.jinja2Lock
+    # note, that ymlparsers.DisableVarSubst also use 1 time HiYaPyCo.jinja2Lock
+    pytest.assume(mock_lock.acquire.call_count > 1)
+    pytest.assume(mock_lock.release.call_count == mock_lock.acquire.call_count)
+
+
+    app_d = default_d.get('app', None)
+    exp_d = copy.deepcopy(exp_config_d)
+    exp_app_d = exp_d.get('app', None)
+
+    inner_host_name = app_d.get('inner_host_name', None)
+    exp_host_name = exp_app_d.get('inner_host_name', None)
+    pytest.assume(exp_host_name==inner_host_name)
+    cli_template = app_d.get('cli_template')
+    pytest.assume('inner_host_name' in cli_template)
+    pytest.assume(exp_config_d==default_d)
+
+
+@pytest.mark.yml
+def test_ymlparsers_load_single_with_substition(request, mocker, ymlparsersSetup, ymlparsersCleanup, exp_config_d):
+    logger.info(f'{request._pyfuncitem.name}()')
+
+    pck = '.'.join(['tests_data', __package__, 'ymlparsers'])
+
+
+    mock_lock = create_mock_lock(mocker)
+    mocker.patch.object(HiYaPyCo, 'jinja2Lock', new=mock_lock, spec_set=True)
+
+    with path(pck, 'config.yml') as full_path:
+        default_d = ymlparsers.load([str(full_path)])
+
+    pytest.assume(mock_lock.acquire.call_count > 1)
+    pytest.assume(mock_lock.release.call_count == mock_lock.acquire.call_count)
+
+    app_d = default_d['app']
+    exp_d = copy.deepcopy(exp_config_d)
+    exp_app_d = exp_d.get('app', None)
+
+    inner_host_name = app_d.get('inner_host_name', None)
+    exp_host_name = exp_app_d.get('inner_host_name', None)
+    pytest.assume(exp_host_name==inner_host_name)
+
+    exp_cli_template = exp_app_d.get('cli_template', None)
+    exp_cli_template = format_template(exp_cli_template, app_inner_host_name=exp_host_name)
+    exp_app_d['cli_template']=exp_cli_template
+
+
+    cli_template = app_d.get('cli_template')
+    pytest.assume('inner_host_name' not in cli_template)
+
+    cli_template = app_d['cli_template']
+    pytest.assume('inner_host_name' not in cli_template)
+    pytest.assume(exp_d==default_d)
+
+    white_list = app_d.get('white_list', None)
+    exp_white_list = exp_app_d.get('white_list', None)
+    pytest.assume(exp_white_list==white_list)
+
+
+#order is non-alephabetic intentionally
+_data_list = {'profiles': ['local', 'dev']}
+_data_dict = {'general':
+                 { 'whiteListSysOverrideKeys': ['app'],
+                   'profiles': ['local', 'dev']},
+              'app':
+                  {'host_name': 'google.com'},
+             }
+
+@pytest.mark.parametrize(
+     'data, kwds',
+
+    [
+        (_data_list, {}),
+
+        #sort_key is ignored
+        (_data_list, {'default_flow_style': None,  'sort_keys': True}),
+        (_data_list, {'default_flow_style': False, 'sort_keys': True}),
+        (_data_list, {'default_flow_style': True,  'sort_keys': True}),
+
+        (_data_dict, {'default_flow_style': None,  'sort_keys': True}),
+        (_data_dict, {'default_flow_style': False, 'sort_keys': True}),
+        (_data_dict, {'default_flow_style': True,  'sort_keys': True}),
+
+    ]
+)
+@pytest.mark.yml
+def test_safe_dump_composite(request, mocker, ymlparsersSetup, ymlparsersCleanup, data, kwds):
+    logger.info(f'{request._pyfuncitem.name}()')
+
+    default_flow_style = kwds.get('default_flow_style', False)
+
+    with io.StringIO() as buf:
+        ymlparsers.safe_dump(data, stream=buf, **kwds)
+        value = buf.getvalue()
+        logger.debug(value)
+        if default_flow_style is not None and not default_flow_style:
+            pytest.assume('-' in value)
+        else:
+            pytest.assume('[' in value)
+            pytest.assume(']' in value)
+
+        with ymlparsers.DisableVarSubst():
+            restored_d = ymlparsers.load(value)
+
+    pytest.assume(data == restored_d)
+
+@pytest.mark.yml
+def test_safe_dump(request, mocker, ymlparsersSetup, ymlparsersCleanup, exp_config_d):
+    logger.info(f'{request._pyfuncitem.name}()')
+
+    orig_d = dict(exp_config_d)
+    d = OrderedDict(exp_config_d)
+    d['general'] = OrderedDict(d['general'])
+    d['app'] = OrderedDict(d['app'])
+
+    with io.StringIO() as buf:
+        ymlparsers.safe_dump(d, stream=buf)
+        value = buf.getvalue()
+
+    with ymlparsers.DisableVarSubst():
+        restored_d = ymlparsers.load(value)
+
+    pytest.assume(orig_d==restored_d)
+
+@pytest.mark.yml
+def test_as_str(request, mocker, ymlparsersSetup, ymlparsersCleanup, exp_config_d):
+    logger.info(f'{request._pyfuncitem.name}()')
+
+    orig_d = dict(exp_config_d)
+    d = OrderedDict(exp_config_d)
+    d['general'] = OrderedDict(d['general'])
+    d['app'] = OrderedDict(d['app'])
+
+    orig_safe_dump = ymlparsers.safe_dump
+    mock_safe_dump = mocker.patch.object(ymlparsers, 'safe_dump', side_effect=orig_safe_dump,
+                                    autospec=True, spec_set=True)
+
+    value = ymlparsers.as_str(d)
+    pytest.assume(mock_safe_dump.call_count > 0)
+
+    with ymlparsers.DisableVarSubst():
+        restored_d = ymlparsers.load(value)
+
+    pytest.assume(orig_d==restored_d)
+
+@pytest.mark.yml
+def test_ymlparsers_load_multiple_no_substition(request, mocker, ymlparsersSetup, ymlparsersCleanup, exp_config_d):
+    logger.info(f'{request._pyfuncitem.name}()')
+
+    exp_d = copy.deepcopy(exp_config_d)
+    exp_d['general']['log']['formatters']['detail'] = {'format': \
+                                                '%(asctime)-14s %(levelname)s [%(name)s.%(funcName)s] %(message)s',
+                                                       'datefmt': \
+                                                '%Y-%m-%d %H:%M:%S'}
+    exp_d['general']['log']['root']['level'] = 'INFO'
+    exp_d['app']['inner_host_name'] = 'yahoo.com'
+    exp_d['app']['white_list'] = ['gamma', 'alpha', 'betha']
+    exp_d['app']['alt_white_list'] = ['c', 'b', 'a']
+
+
+
+    pck = '.'.join(['tests_data', __package__, 'ymlparsers'])
+
+    with path(pck, 'config.yml') as full_path:
+        with path(pck, 'config-dev.yml') as full_dev_path:
+            with ymlparsers.DisableVarSubst():
+                default_d = ymlparsers.load([str(full_path), str(full_dev_path)])
+
+
+    app_d = default_d.get('app', None)
+    exp_app_d = exp_d.get('app', None)
+
+    inner_host_name = app_d.get('inner_host_name', None)
+    exp_host_name = exp_app_d.get('inner_host_name', None)
+    pytest.assume(exp_host_name==inner_host_name)
+
+    cli_template = app_d.get('cli_template')
+    pytest.assume('inner_host_name' in cli_template)
+
+    pytest.assume(exp_d==default_d)
+
+@pytest.mark.yml
+def test_ymlparsers_load_multiple_with_substition(request, mocker, ymlparsersSetup, ymlparsersCleanup, exp_config_d):
+    logger.info(f'{request._pyfuncitem.name}()')
+
+    pck = '.'.join(['tests_data', __package__, 'ymlparsers'])
+
+    exp_d = copy.deepcopy(exp_config_d)
+    exp_d['general']['log']['formatters']['detail'] = {'format': \
+                                                           '%(asctime)-14s %(levelname)s [%(name)s.%(funcName)s] %(message)s',
+                                                       'datefmt': \
+                                                           '%Y-%m-%d %H:%M:%S'}
+    exp_d['general']['log']['root']['level'] = 'INFO'
+    exp_d['app']['inner_host_name'] = 'yahoo.com'
+    exp_d['app']['white_list'] = ['gamma', 'alpha', 'betha']
+    exp_d['app']['alt_white_list'] = ['c', 'b', 'a']
+
+    with path(pck, 'config.yml') as full_path:
+        with path(pck, 'config-dev.yml') as full_dev_path:
+            default_d = ymlparsers.load([str(full_path), str(full_dev_path)])
+
+
+    app_d = default_d['app']
+    exp_app_d = exp_d.get('app', None)
+
+    inner_host_name = app_d.get('inner_host_name', None)
+    exp_host_name = exp_app_d.get('inner_host_name', None)
+    pytest.assume(exp_host_name==inner_host_name)
+
+    exp_cli_template = exp_app_d.get('cli_template', None)
+    exp_cli_template = format_template(exp_cli_template, app_inner_host_name=exp_host_name)
+    exp_app_d['cli_template']=exp_cli_template
+
+
+    cli_template = app_d.get('cli_template')
+    pytest.assume('inner_host_name' not in cli_template)
+
+    cli_template = app_d['cli_template']
+    pytest.assume('inner_host_name' not in cli_template)
+
+    pytest.assume(exp_d==default_d)
+
+
+def _run_without_substition(content, exp_config_d, stop):
+    for i in range(stop):
+        with ymlparsers.DisableVarSubst():
+            default_d = ymlparsers.load([str(content)])
+
+            app_d = default_d.get('app', None)
+            exp_app_d = exp_config_d.get('app', None)
+
+            inner_host_name = app_d.get('inner_host_name', None)
+            exp_host_name = exp_app_d.get('inner_host_name', None)
+            pytest.assume(exp_host_name==inner_host_name)
+            cli_template = app_d.get('cli_template')
+            pytest.assume('inner_host_name' in cli_template)
+            pytest.assume(exp_config_d == default_d)
+
+def _run_with_substition(content, exp_config_d, stop):
+    for i in range(stop):
+        default_d = ymlparsers.load([str(content)])
+
+        app_d = default_d['app']
+        exp_app_d = exp_config_d.get('app', None)
+
+        inner_host_name = app_d.get('inner_host_name', None)
+        exp_host_name = exp_app_d.get('inner_host_name', None)
+        pytest.assume(exp_host_name==inner_host_name)
+
+        exp_cli_template = exp_app_d.get('cli_template', None)
+        exp_cli_template = format_template(exp_cli_template, app_inner_host_name=exp_host_name)
+
+        exp_app_d['cli_template'] = exp_cli_template
+
+        cli_template = app_d.get('cli_template')
+        pytest.assume('inner_host_name' not in cli_template)
+
+        cli_template = app_d['cli_template']
+        pytest.assume('inner_host_name' not in cli_template)
+        pytest.assume(exp_config_d == default_d)
+
+@pytest.mark.yml
+def test_ymlparsers_load_it(request, mocker, ymlparsersSetup, ymlparsersCleanup, exp_config_d):
+    logger.info(f'{request._pyfuncitem.name}()')
+    pck = '.'.join(['tests_data', __package__, 'ymlparsers'])
+
+    with path(pck, 'config.yml') as full_path:
+        with open(full_path, 'r') as f:
+            content = f.read()
+
+    stop = 10
+
+    exp_d = copy.deepcopy(exp_config_d)
+    exp_app_d = dict(exp_d.get('app', None))
+    if exp_app_d is not None:
+        exp_d['app'] = exp_app_d
+
+    exp_host_name = exp_app_d.get('inner_host_name', None)
+    exp_cli_template = exp_app_d.get('cli_template', None)
+    exp_cli_template = format_template(exp_cli_template, app_inner_host_name=exp_host_name)
+    exp_app_d['cli_template'] = exp_cli_template
+
+
+    th1 = threading.Thread(name="run_with_substition",
+        target=_run_with_substition, args=(content, exp_d, stop))
+
+    th2 = threading.Thread(name="run_without_substition",
+                           target=_run_without_substition, args=(str(content), copy.deepcopy(exp_config_d), stop))
+
+    th1.start()
+    time.sleep(2)
+    th2.start()
+    th1.join()
+    th2.join()
+
+
+if __name__ == "__main__":
+    pytest.main([__file__])
```

