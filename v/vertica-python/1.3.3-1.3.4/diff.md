# Comparing `tmp/vertica-python-1.3.3.tar.gz` & `tmp/vertica-python-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vertica-python-1.3.3.tar", last modified: Tue Aug  1 03:55:29 2023, max compression
+gzip compressed data, was "vertica-python-1.3.4.tar", last modified: Fri Aug  4 06:58:42 2023, max compression
```

## Comparing `vertica-python-1.3.3.tar` & `vertica-python-1.3.4.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-08-01 03:55:29.734635 vertica-python-1.3.3/
--rw-rw-r--   0 sren      (1000) sren      (1000)    11357 2023-08-01 03:55:29.000000 vertica-python-1.3.3/LICENSE
--rw-rw-r--   0 sren      (1000) sren      (1000)      136 2023-08-01 03:55:29.000000 vertica-python-1.3.3/MANIFEST.in
--rw-rw-r--   0 sren      (1000) sren      (1000)     1393 2023-08-01 03:55:29.734635 vertica-python-1.3.3/PKG-INFO
--rw-rw-r--   0 sren      (1000) sren      (1000)    47396 2023-08-01 03:55:29.000000 vertica-python-1.3.3/README.md
--rw-rw-r--   0 sren      (1000) sren      (1000)       38 2023-08-01 03:55:29.734635 vertica-python-1.3.3/setup.cfg
--rw-rw-r--   0 sren      (1000) sren      (1000)     3662 2023-08-01 03:55:29.000000 vertica-python-1.3.3/setup.py
-drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-08-01 03:55:29.726635 vertica-python-1.3.3/vertica_python/
--rw-rw-r--   0 sren      (1000) sren      (1000)     3198 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/__init__.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     4947 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/compat.py
--rw-rw-r--   0 sren      (1000) sren      (1000)    21640 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/datatypes.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     5635 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/errors.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2254 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/os_utils.py
-drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-08-01 03:55:29.726635 vertica-python-1.3.3/vertica_python/tests/
--rw-rw-r--   0 sren      (1000) sren      (1000)     1734 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/tests/__init__.py
-drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-08-01 03:55:29.726635 vertica-python-1.3.3/vertica_python/tests/common/
--rw-rw-r--   0 sren      (1000) sren      (1000)     1734 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/tests/common/__init__.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     6312 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/tests/common/base.py
--rw-rw-r--   0 sren      (1000) sren      (1000)      821 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/tests/conftest.py
-drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-08-01 03:55:29.730635 vertica-python-1.3.3/vertica_python/tests/integration_tests/
--rw-rw-r--   0 sren      (1000) sren      (1000)     1734 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/tests/integration_tests/__init__.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     7779 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/tests/integration_tests/base.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     6453 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/tests/integration_tests/test_authentication.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     4269 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/tests/integration_tests/test_cancel.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     4643 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/tests/integration_tests/test_column.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     7087 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/tests/integration_tests/test_connection.py
--rw-rw-r--   0 sren      (1000) sren      (1000)    60985 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/tests/integration_tests/test_cursor.py
--rw-rw-r--   0 sren      (1000) sren      (1000)    42970 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/tests/integration_tests/test_datatypes.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     7524 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/tests/integration_tests/test_dates.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2859 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/tests/integration_tests/test_errors.py
--rw-rw-r--   0 sren      (1000) sren      (1000)    13199 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/tests/integration_tests/test_loadbalance.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     3843 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/tests/integration_tests/test_timezones.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     9225 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/tests/integration_tests/test_tls.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     5411 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/tests/integration_tests/test_transfer_format.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     4483 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/tests/integration_tests/test_unicode.py
-drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-08-01 03:55:29.730635 vertica-python-1.3.3/vertica_python/tests/unit_tests/
--rw-rw-r--   0 sren      (1000) sren      (1000)     1734 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/tests/unit_tests/__init__.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2361 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/tests/unit_tests/base.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     1967 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/tests/unit_tests/test_errors.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     1704 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/tests/unit_tests/test_logging.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     3233 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/tests/unit_tests/test_notice.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     4811 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/tests/unit_tests/test_parsedsn.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     3515 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/tests/unit_tests/test_sql_literal.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     4634 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/tests/unit_tests/test_timestamps.py
-drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-08-01 03:55:29.730635 vertica-python-1.3.3/vertica_python/vertica/
--rw-rw-r--   0 sren      (1000) sren      (1000)     1735 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/__init__.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     4861 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/column.py
--rw-rw-r--   0 sren      (1000) sren      (1000)    38153 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/connection.py
--rw-rw-r--   0 sren      (1000) sren      (1000)    45705 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/cursor.py
--rw-rw-r--   0 sren      (1000) sren      (1000)    25060 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/deserializer.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2575 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/log.py
-drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-08-01 03:55:29.730635 vertica-python-1.3.3/vertica_python/vertica/messages/
--rw-rw-r--   0 sren      (1000) sren      (1000)     2034 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/__init__.py
-drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-08-01 03:55:29.734635 vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/
--rw-rw-r--   0 sren      (1000) sren      (1000)     3383 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/__init__.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     3267 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/authentication.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2243 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/backend_key_data.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2008 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/bind_complete.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2010 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/close_complete.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2789 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/command_complete.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2979 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/command_description.py
--rw-rw-r--   0 sren      (1000) sren      (1000)      864 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/copy_done_response.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2182 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/copy_in_response.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2363 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/data_row.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2020 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/empty_query_response.py
--rw-rw-r--   0 sren      (1000) sren      (1000)      868 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/end_of_batch_response.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2137 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/error_response.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2401 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/load_balance_response.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     1079 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/load_file.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     1996 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/no_data.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     3878 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/notice_response.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     3542 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/parameter_description.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     3024 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/parameter_status.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2010 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/parse_complete.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2669 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/portal_suspended.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2530 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/ready_for_query.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     6516 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/row_description.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2220 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/unknown.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2080 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/verify_files.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2261 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/write_file.py
-drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-08-01 03:55:29.734635 vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/
--rw-rw-r--   0 sren      (1000) sren      (1000)     2753 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/__init__.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     4867 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/bind.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2868 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/cancel_request.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2890 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/close.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2314 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/copy_data.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     1905 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/copy_done.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     1611 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/copy_error.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2451 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/copy_fail.py
--rwxrwxr-x   0 sren      (1000) sren      (1000)    10264 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/crypt_windows.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     3396 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/describe.py
--rw-rw-r--   0 sren      (1000) sren      (1000)      973 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/end_of_batch_request.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2815 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/execute.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2274 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/flush.py
--rwxrwxr-x   0 sren      (1000) sren      (1000)     2078 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/load_balance_request.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2983 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/parse.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     4354 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/password.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2521 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/query.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2054 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/ssl_request.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     5059 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/startup.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     1901 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/sync.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     1906 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/terminate.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     1317 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/verified_files.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     5183 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/messages/message.py
-drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-08-01 03:55:29.734635 vertica-python-1.3.3/vertica_python/vertica/mixins/
--rw-rw-r--   0 sren      (1000) sren      (1000)      648 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/mixins/__init__.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     3524 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python/vertica/mixins/notice_response_attr.py
-drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-08-01 03:55:29.726635 vertica-python-1.3.3/vertica_python.egg-info/
--rw-rw-r--   0 sren      (1000) sren      (1000)     1393 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python.egg-info/PKG-INFO
--rw-rw-r--   0 sren      (1000) sren      (1000)     5243 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python.egg-info/SOURCES.txt
--rw-rw-r--   0 sren      (1000) sren      (1000)        1 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python.egg-info/dependency_links.txt
--rw-rw-r--   0 sren      (1000) sren      (1000)       33 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python.egg-info/requires.txt
--rw-rw-r--   0 sren      (1000) sren      (1000)       15 2023-08-01 03:55:29.000000 vertica-python-1.3.3/vertica_python.egg-info/top_level.txt
+drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-08-04 06:58:42.332222 vertica-python-1.3.4/
+-rw-rw-r--   0 sren      (1000) sren      (1000)    11357 2023-08-04 06:58:41.000000 vertica-python-1.3.4/LICENSE
+-rw-rw-r--   0 sren      (1000) sren      (1000)      136 2023-08-04 06:58:41.000000 vertica-python-1.3.4/MANIFEST.in
+-rw-rw-r--   0 sren      (1000) sren      (1000)     1393 2023-08-04 06:58:42.332222 vertica-python-1.3.4/PKG-INFO
+-rw-rw-r--   0 sren      (1000) sren      (1000)    47396 2023-08-04 06:58:41.000000 vertica-python-1.3.4/README.md
+-rw-rw-r--   0 sren      (1000) sren      (1000)       38 2023-08-04 06:58:42.332222 vertica-python-1.3.4/setup.cfg
+-rw-rw-r--   0 sren      (1000) sren      (1000)     3662 2023-08-04 06:58:41.000000 vertica-python-1.3.4/setup.py
+drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-08-04 06:58:42.324222 vertica-python-1.3.4/vertica_python/
+-rw-rw-r--   0 sren      (1000) sren      (1000)     3198 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/__init__.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     4947 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/compat.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)    21640 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/datatypes.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     5635 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/errors.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2254 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/os_utils.py
+drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-08-04 06:58:42.324222 vertica-python-1.3.4/vertica_python/tests/
+-rw-rw-r--   0 sren      (1000) sren      (1000)     1734 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/tests/__init__.py
+drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-08-04 06:58:42.324222 vertica-python-1.3.4/vertica_python/tests/common/
+-rw-rw-r--   0 sren      (1000) sren      (1000)     1734 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/tests/common/__init__.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     6312 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/tests/common/base.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)      821 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/tests/conftest.py
+drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-08-04 06:58:42.328222 vertica-python-1.3.4/vertica_python/tests/integration_tests/
+-rw-rw-r--   0 sren      (1000) sren      (1000)     1734 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/tests/integration_tests/__init__.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     7779 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/tests/integration_tests/base.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     6453 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/tests/integration_tests/test_authentication.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     4269 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/tests/integration_tests/test_cancel.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     4643 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/tests/integration_tests/test_column.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     7087 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/tests/integration_tests/test_connection.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)    60985 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/tests/integration_tests/test_cursor.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)    42970 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/tests/integration_tests/test_datatypes.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     7524 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/tests/integration_tests/test_dates.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2859 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/tests/integration_tests/test_errors.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)    13199 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/tests/integration_tests/test_loadbalance.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     3843 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/tests/integration_tests/test_timezones.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     9225 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/tests/integration_tests/test_tls.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     5411 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/tests/integration_tests/test_transfer_format.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     4483 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/tests/integration_tests/test_unicode.py
+drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-08-04 06:58:42.328222 vertica-python-1.3.4/vertica_python/tests/unit_tests/
+-rw-rw-r--   0 sren      (1000) sren      (1000)     1734 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/tests/unit_tests/__init__.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2361 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/tests/unit_tests/base.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     1967 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/tests/unit_tests/test_errors.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     1704 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/tests/unit_tests/test_logging.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     3233 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/tests/unit_tests/test_notice.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     4811 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/tests/unit_tests/test_parsedsn.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     3515 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/tests/unit_tests/test_sql_literal.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     4634 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/tests/unit_tests/test_timestamps.py
+drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-08-04 06:58:42.328222 vertica-python-1.3.4/vertica_python/vertica/
+-rw-rw-r--   0 sren      (1000) sren      (1000)     1735 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/vertica/__init__.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     4861 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/vertica/column.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)    38153 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/vertica/connection.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)    45794 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/vertica/cursor.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)    25060 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/vertica/deserializer.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2575 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/vertica/log.py
+drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-08-04 06:58:42.328222 vertica-python-1.3.4/vertica_python/vertica/messages/
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2034 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/vertica/messages/__init__.py
+drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-08-04 06:58:42.332222 vertica-python-1.3.4/vertica_python/vertica/messages/backend_messages/
+-rw-rw-r--   0 sren      (1000) sren      (1000)     3383 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/vertica/messages/backend_messages/__init__.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     3267 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/vertica/messages/backend_messages/authentication.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2243 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/vertica/messages/backend_messages/backend_key_data.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2008 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/vertica/messages/backend_messages/bind_complete.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2010 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/vertica/messages/backend_messages/close_complete.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2789 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/vertica/messages/backend_messages/command_complete.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2979 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/vertica/messages/backend_messages/command_description.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)      864 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/vertica/messages/backend_messages/copy_done_response.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2182 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/vertica/messages/backend_messages/copy_in_response.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2363 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/vertica/messages/backend_messages/data_row.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2020 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/vertica/messages/backend_messages/empty_query_response.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)      868 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/vertica/messages/backend_messages/end_of_batch_response.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2137 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/vertica/messages/backend_messages/error_response.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2401 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/vertica/messages/backend_messages/load_balance_response.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     1079 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/vertica/messages/backend_messages/load_file.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     1996 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/vertica/messages/backend_messages/no_data.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     3878 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/vertica/messages/backend_messages/notice_response.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     3542 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/vertica/messages/backend_messages/parameter_description.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     3024 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/vertica/messages/backend_messages/parameter_status.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2010 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/vertica/messages/backend_messages/parse_complete.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2669 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/vertica/messages/backend_messages/portal_suspended.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2530 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/vertica/messages/backend_messages/ready_for_query.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     6516 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/vertica/messages/backend_messages/row_description.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2220 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/vertica/messages/backend_messages/unknown.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2080 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/vertica/messages/backend_messages/verify_files.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2261 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/vertica/messages/backend_messages/write_file.py
+drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-08-04 06:58:42.332222 vertica-python-1.3.4/vertica_python/vertica/messages/frontend_messages/
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2753 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/vertica/messages/frontend_messages/__init__.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     4867 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/vertica/messages/frontend_messages/bind.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2868 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/vertica/messages/frontend_messages/cancel_request.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2890 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/vertica/messages/frontend_messages/close.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2314 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/vertica/messages/frontend_messages/copy_data.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     1905 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/vertica/messages/frontend_messages/copy_done.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     1611 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/vertica/messages/frontend_messages/copy_error.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2451 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/vertica/messages/frontend_messages/copy_fail.py
+-rwxrwxr-x   0 sren      (1000) sren      (1000)    10264 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/vertica/messages/frontend_messages/crypt_windows.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     3396 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/vertica/messages/frontend_messages/describe.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)      973 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/vertica/messages/frontend_messages/end_of_batch_request.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2815 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/vertica/messages/frontend_messages/execute.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2274 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/vertica/messages/frontend_messages/flush.py
+-rwxrwxr-x   0 sren      (1000) sren      (1000)     2078 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/vertica/messages/frontend_messages/load_balance_request.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2983 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/vertica/messages/frontend_messages/parse.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     4354 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/vertica/messages/frontend_messages/password.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2521 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/vertica/messages/frontend_messages/query.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2054 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/vertica/messages/frontend_messages/ssl_request.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     5059 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/vertica/messages/frontend_messages/startup.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     1901 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/vertica/messages/frontend_messages/sync.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     1906 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/vertica/messages/frontend_messages/terminate.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     1523 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/vertica/messages/frontend_messages/verified_files.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     5183 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/vertica/messages/message.py
+drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-08-04 06:58:42.332222 vertica-python-1.3.4/vertica_python/vertica/mixins/
+-rw-rw-r--   0 sren      (1000) sren      (1000)      648 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/vertica/mixins/__init__.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     3524 2023-08-04 06:58:41.000000 vertica-python-1.3.4/vertica_python/vertica/mixins/notice_response_attr.py
+drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-08-04 06:58:42.324222 vertica-python-1.3.4/vertica_python.egg-info/
+-rw-rw-r--   0 sren      (1000) sren      (1000)     1393 2023-08-04 06:58:42.000000 vertica-python-1.3.4/vertica_python.egg-info/PKG-INFO
+-rw-rw-r--   0 sren      (1000) sren      (1000)     5243 2023-08-04 06:58:42.000000 vertica-python-1.3.4/vertica_python.egg-info/SOURCES.txt
+-rw-rw-r--   0 sren      (1000) sren      (1000)        1 2023-08-04 06:58:42.000000 vertica-python-1.3.4/vertica_python.egg-info/dependency_links.txt
+-rw-rw-r--   0 sren      (1000) sren      (1000)       33 2023-08-04 06:58:42.000000 vertica-python-1.3.4/vertica_python.egg-info/requires.txt
+-rw-rw-r--   0 sren      (1000) sren      (1000)       15 2023-08-04 06:58:42.000000 vertica-python-1.3.4/vertica_python.egg-info/top_level.txt
```

### Comparing `vertica-python-1.3.3/LICENSE` & `vertica-python-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/PKG-INFO` & `vertica-python-1.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vertica-python
-Version: 1.3.3
+Version: 1.3.4
 Summary: Official native Python client for the Vertica database.
 Home-page: https://github.com/vertica/vertica-python
 Author: Justin Berka, Alex Kim, Siting Ren
 Author-email: justin.berka@gmail.com, alex.kim@uber.com, sitingren@hotmail.com
 License: Apache License 2.0
 Description: vertica-python is the official Vertica database client for the Python programming language. Please check the [project homepage](https://github.com/vertica/vertica-python) for the details.
 Keywords: database vertica
```

### Comparing `vertica-python-1.3.3/README.md` & `vertica-python-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/setup.py` & `vertica-python-1.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 ReqOpts = collections.namedtuple('ReqOpts', ['skip_requirements_regex', 'default_vcs'])
 
 opts = ReqOpts(None, 'git')
 
 # version should use the format 'x.x.x' (instead of 'vx.x.x')
 setup(
     name='vertica-python',
-    version='1.3.3',
+    version='1.3.4',
     description='Official native Python client for the Vertica database.',
     long_description="vertica-python is the official Vertica database client for the Python programming language. Please check the [project homepage](https://github.com/vertica/vertica-python) for the details.",
     long_description_content_type='text/markdown',
     author='Justin Berka, Alex Kim, Siting Ren',
     author_email='justin.berka@gmail.com, alex.kim@uber.com, sitingren@hotmail.com',
     url='https://github.com/vertica/vertica-python',
     keywords="database vertica",
```

### Comparing `vertica-python-1.3.3/vertica_python/__init__.py` & `vertica-python-1.3.4/vertica_python/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
 __all__ = ['Connection', 'PROTOCOL_VERSION', 'version_info', 'apilevel', 'threadsafety',
            'paramstyle', 'connect', 'parse_dsn', 'Error', 'Warning', 'DataError', 'DatabaseError',
            'IntegrityError', 'InterfaceError', 'InternalError', 'NotSupportedError',
            'OperationalError', 'ProgrammingError']
 
 # The version number of this library.
-version_info = (1, 3, 3)
+version_info = (1, 3, 4)
 __version__ = '.'.join(map(str, version_info))
 
 # The protocol version (3.15) implemented in this library.
 PROTOCOL_VERSION = 3 << 16 | 15
 
 apilevel = 2.0
 threadsafety = 1  # Threads may share the module, but not connections!
```

### Comparing `vertica-python-1.3.3/vertica_python/compat.py` & `vertica-python-1.3.4/vertica_python/compat.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/datatypes.py` & `vertica-python-1.3.4/vertica_python/datatypes.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/errors.py` & `vertica-python-1.3.4/vertica_python/errors.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/os_utils.py` & `vertica-python-1.3.4/vertica_python/os_utils.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/tests/__init__.py` & `vertica-python-1.3.4/vertica_python/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/tests/common/__init__.py` & `vertica-python-1.3.4/vertica_python/tests/common/__init__.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/tests/common/base.py` & `vertica-python-1.3.4/vertica_python/tests/common/base.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/tests/conftest.py` & `vertica-python-1.3.4/vertica_python/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/tests/integration_tests/__init__.py` & `vertica-python-1.3.4/vertica_python/tests/integration_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/tests/integration_tests/base.py` & `vertica-python-1.3.4/vertica_python/tests/integration_tests/base.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/tests/integration_tests/test_authentication.py` & `vertica-python-1.3.4/vertica_python/tests/integration_tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/tests/integration_tests/test_cancel.py` & `vertica-python-1.3.4/vertica_python/tests/integration_tests/test_cancel.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/tests/integration_tests/test_column.py` & `vertica-python-1.3.4/vertica_python/tests/integration_tests/test_column.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/tests/integration_tests/test_connection.py` & `vertica-python-1.3.4/vertica_python/tests/integration_tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/tests/integration_tests/test_cursor.py` & `vertica-python-1.3.4/vertica_python/tests/integration_tests/test_cursor.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/tests/integration_tests/test_datatypes.py` & `vertica-python-1.3.4/vertica_python/tests/integration_tests/test_datatypes.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/tests/integration_tests/test_dates.py` & `vertica-python-1.3.4/vertica_python/tests/integration_tests/test_dates.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/tests/integration_tests/test_errors.py` & `vertica-python-1.3.4/vertica_python/tests/integration_tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/tests/integration_tests/test_loadbalance.py` & `vertica-python-1.3.4/vertica_python/tests/integration_tests/test_loadbalance.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/tests/integration_tests/test_timezones.py` & `vertica-python-1.3.4/vertica_python/tests/integration_tests/test_timezones.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/tests/integration_tests/test_tls.py` & `vertica-python-1.3.4/vertica_python/tests/integration_tests/test_tls.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/tests/integration_tests/test_transfer_format.py` & `vertica-python-1.3.4/vertica_python/tests/integration_tests/test_transfer_format.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/tests/integration_tests/test_unicode.py` & `vertica-python-1.3.4/vertica_python/tests/integration_tests/test_unicode.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/tests/unit_tests/__init__.py` & `vertica-python-1.3.4/vertica_python/tests/unit_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/tests/unit_tests/base.py` & `vertica-python-1.3.4/vertica_python/tests/unit_tests/base.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/tests/unit_tests/test_errors.py` & `vertica-python-1.3.4/vertica_python/tests/unit_tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/tests/unit_tests/test_logging.py` & `vertica-python-1.3.4/vertica_python/tests/unit_tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/tests/unit_tests/test_notice.py` & `vertica-python-1.3.4/vertica_python/tests/unit_tests/test_notice.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/tests/unit_tests/test_parsedsn.py` & `vertica-python-1.3.4/vertica_python/tests/unit_tests/test_parsedsn.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/tests/unit_tests/test_sql_literal.py` & `vertica-python-1.3.4/vertica_python/tests/unit_tests/test_sql_literal.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/tests/unit_tests/test_timestamps.py` & `vertica-python-1.3.4/vertica_python/tests/unit_tests/test_timestamps.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/vertica/__init__.py` & `vertica-python-1.3.4/vertica_python/vertica/__init__.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/vertica/column.py` & `vertica-python-1.3.4/vertica_python/vertica/column.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/vertica/connection.py` & `vertica-python-1.3.4/vertica_python/vertica/connection.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/vertica/cursor.py` & `vertica-python-1.3.4/vertica_python/vertica/cursor.py`

 * *Files 0% similar despite different names*

```diff
@@ -773,15 +773,16 @@
                         ' invalid exceptions file path: {}'.format(exceptions_file))
                 os_utils.check_file_writable(exceptions_file)
                 self.valid_write_file_path.append(exceptions_file)
 
             # Check that the input files are readable
             self.valid_read_file_path = self._check_copy_local_files(input_files)
 
-            self.connection.write(messages.VerifiedFiles(self.valid_read_file_path))
+            self.connection.write(messages.VerifiedFiles(self.valid_read_file_path,
+                                  self.connection.parameters.get('protocol_version', 0)))
         except Exception as e:
             tb = sys.exc_info()[2]
             stk = traceback.extract_tb(tb, 1)
             self.connection.write(messages.CopyError(str(e), stk[0]))
             self.flush_to_query_ready()
             raise
```

### Comparing `vertica-python-1.3.3/vertica_python/vertica/deserializer.py` & `vertica-python-1.3.4/vertica_python/vertica/deserializer.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/vertica/log.py` & `vertica-python-1.3.4/vertica_python/vertica/log.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/vertica/messages/__init__.py` & `vertica-python-1.3.4/vertica_python/vertica/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/__init__.py` & `vertica-python-1.3.4/vertica_python/vertica/messages/backend_messages/__init__.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/authentication.py` & `vertica-python-1.3.4/vertica_python/vertica/messages/backend_messages/authentication.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/backend_key_data.py` & `vertica-python-1.3.4/vertica_python/vertica/messages/backend_messages/backend_key_data.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/bind_complete.py` & `vertica-python-1.3.4/vertica_python/vertica/messages/backend_messages/bind_complete.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/close_complete.py` & `vertica-python-1.3.4/vertica_python/vertica/messages/backend_messages/close_complete.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/command_complete.py` & `vertica-python-1.3.4/vertica_python/vertica/messages/backend_messages/command_complete.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/command_description.py` & `vertica-python-1.3.4/vertica_python/vertica/messages/backend_messages/command_description.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/copy_done_response.py` & `vertica-python-1.3.4/vertica_python/vertica/messages/backend_messages/copy_done_response.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/copy_in_response.py` & `vertica-python-1.3.4/vertica_python/vertica/messages/backend_messages/copy_in_response.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/data_row.py` & `vertica-python-1.3.4/vertica_python/vertica/messages/backend_messages/data_row.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/empty_query_response.py` & `vertica-python-1.3.4/vertica_python/vertica/messages/backend_messages/empty_query_response.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/end_of_batch_response.py` & `vertica-python-1.3.4/vertica_python/vertica/messages/backend_messages/end_of_batch_response.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/error_response.py` & `vertica-python-1.3.4/vertica_python/vertica/messages/backend_messages/error_response.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/load_balance_response.py` & `vertica-python-1.3.4/vertica_python/vertica/messages/backend_messages/load_balance_response.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/load_file.py` & `vertica-python-1.3.4/vertica_python/vertica/messages/backend_messages/load_file.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/no_data.py` & `vertica-python-1.3.4/vertica_python/vertica/messages/backend_messages/no_data.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/notice_response.py` & `vertica-python-1.3.4/vertica_python/vertica/messages/backend_messages/notice_response.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/parameter_description.py` & `vertica-python-1.3.4/vertica_python/vertica/messages/backend_messages/parameter_description.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/parameter_status.py` & `vertica-python-1.3.4/vertica_python/vertica/messages/backend_messages/parameter_status.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/parse_complete.py` & `vertica-python-1.3.4/vertica_python/vertica/messages/backend_messages/parse_complete.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/portal_suspended.py` & `vertica-python-1.3.4/vertica_python/vertica/messages/backend_messages/portal_suspended.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/ready_for_query.py` & `vertica-python-1.3.4/vertica_python/vertica/messages/backend_messages/ready_for_query.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/row_description.py` & `vertica-python-1.3.4/vertica_python/vertica/messages/backend_messages/row_description.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/unknown.py` & `vertica-python-1.3.4/vertica_python/vertica/messages/backend_messages/unknown.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/verify_files.py` & `vertica-python-1.3.4/vertica_python/vertica/messages/backend_messages/verify_files.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/vertica/messages/backend_messages/write_file.py` & `vertica-python-1.3.4/vertica_python/vertica/messages/backend_messages/write_file.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/__init__.py` & `vertica-python-1.3.4/vertica_python/vertica/messages/frontend_messages/__init__.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/bind.py` & `vertica-python-1.3.4/vertica_python/vertica/messages/frontend_messages/bind.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/cancel_request.py` & `vertica-python-1.3.4/vertica_python/vertica/messages/frontend_messages/cancel_request.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/close.py` & `vertica-python-1.3.4/vertica_python/vertica/messages/frontend_messages/close.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/copy_data.py` & `vertica-python-1.3.4/vertica_python/vertica/messages/frontend_messages/copy_data.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/copy_done.py` & `vertica-python-1.3.4/vertica_python/vertica/messages/frontend_messages/copy_done.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/copy_error.py` & `vertica-python-1.3.4/vertica_python/vertica/messages/frontend_messages/copy_error.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/copy_fail.py` & `vertica-python-1.3.4/vertica_python/vertica/messages/frontend_messages/copy_fail.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/crypt_windows.py` & `vertica-python-1.3.4/vertica_python/vertica/messages/frontend_messages/crypt_windows.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/describe.py` & `vertica-python-1.3.4/vertica_python/vertica/messages/frontend_messages/describe.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/end_of_batch_request.py` & `vertica-python-1.3.4/vertica_python/vertica/messages/frontend_messages/end_of_batch_request.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/execute.py` & `vertica-python-1.3.4/vertica_python/vertica/messages/frontend_messages/execute.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/flush.py` & `vertica-python-1.3.4/vertica_python/vertica/messages/frontend_messages/flush.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/load_balance_request.py` & `vertica-python-1.3.4/vertica_python/vertica/messages/frontend_messages/load_balance_request.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/parse.py` & `vertica-python-1.3.4/vertica_python/vertica/messages/frontend_messages/parse.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/password.py` & `vertica-python-1.3.4/vertica_python/vertica/messages/frontend_messages/password.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/query.py` & `vertica-python-1.3.4/vertica_python/vertica/messages/frontend_messages/query.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/ssl_request.py` & `vertica-python-1.3.4/vertica_python/vertica/messages/frontend_messages/ssl_request.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/startup.py` & `vertica-python-1.3.4/vertica_python/vertica/messages/frontend_messages/startup.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/sync.py` & `vertica-python-1.3.4/vertica_python/vertica/messages/frontend_messages/sync.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/terminate.py` & `vertica-python-1.3.4/vertica_python/vertica/messages/frontend_messages/terminate.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/vertica/messages/frontend_messages/verified_files.py` & `vertica-python-1.3.4/vertica_python/vertica/messages/frontend_messages/verified_files.py`

 * *Files 23% similar despite different names*

```diff
@@ -20,20 +20,24 @@
 
 from ..message import BulkFrontendMessage
 
 
 class VerifiedFiles(BulkFrontendMessage):
     message_id = b'F'
 
-    def __init__(self, file_list):
+    def __init__(self, file_list, protocol_version):
         BulkFrontendMessage.__init__(self)
         self.filenames = file_list
+        self.protocol_version = protocol_version
 
     def read_bytes(self):
-        bytes_ = pack('!I', len(self.filenames))
+        if self.protocol_version >= (3 << 16 | 15):
+            bytes_ = pack('!I', len(self.filenames)) # Int32
+        else:
+            bytes_ = pack('!H', len(self.filenames)) # Int16
         for filename in self.filenames:
             utf_filename = filename.encode('utf-8')
             bytes_ += pack('!{0}sx'.format(len(utf_filename)), utf_filename)
             bytes_ += pack('!Q', os.path.getsize(filename))
 
         return bytes_
```

### Comparing `vertica-python-1.3.3/vertica_python/vertica/messages/message.py` & `vertica-python-1.3.4/vertica_python/vertica/messages/message.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/vertica/mixins/__init__.py` & `vertica-python-1.3.4/vertica_python/vertica/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python/vertica/mixins/notice_response_attr.py` & `vertica-python-1.3.4/vertica_python/vertica/mixins/notice_response_attr.py`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.3/vertica_python.egg-info/PKG-INFO` & `vertica-python-1.3.4/vertica_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vertica-python
-Version: 1.3.3
+Version: 1.3.4
 Summary: Official native Python client for the Vertica database.
 Home-page: https://github.com/vertica/vertica-python
 Author: Justin Berka, Alex Kim, Siting Ren
 Author-email: justin.berka@gmail.com, alex.kim@uber.com, sitingren@hotmail.com
 License: Apache License 2.0
 Description: vertica-python is the official Vertica database client for the Python programming language. Please check the [project homepage](https://github.com/vertica/vertica-python) for the details.
 Keywords: database vertica
```

### Comparing `vertica-python-1.3.3/vertica_python.egg-info/SOURCES.txt` & `vertica-python-1.3.4/vertica_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

