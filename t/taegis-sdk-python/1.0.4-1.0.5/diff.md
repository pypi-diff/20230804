# Comparing `tmp/taegis-sdk-python-1.0.4.tar.gz` & `tmp/taegis-sdk-python-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taegis-sdk-python-1.0.4.tar", last modified: Thu Aug  3 16:39:13 2023, max compression
+gzip compressed data, was "taegis-sdk-python-1.0.5.tar", last modified: Fri Aug  4 17:24:23 2023, max compression
```

## Comparing `taegis-sdk-python-1.0.4.tar` & `taegis-sdk-python-1.0.5.tar`

### file list

```diff
@@ -1,214 +1,220 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.770345 taegis-sdk-python-1.0.4/
--rw-rw-rw-   0 root         (0) root         (0)    10173 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       84 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6228 2023-08-03 16:39:13.770345 taegis-sdk-python-1.0.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5793 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/README.md
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/requirements-dev.txt
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/requirements-test.txt
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-03 16:39:13.770345 taegis-sdk-python-1.0.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1571 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.738347 taegis-sdk-python-1.0.4/taegis_sdk_python/
--rw-rw-rw-   0 root         (0) root         (0)      896 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1135 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/_consts.py
--rw-rw-rw-   0 root         (0) root         (0)       23 2023-08-03 16:39:13.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     8618 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/authentication.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/config.py
--rw-rw-rw-   0 root         (0) root         (0)     2637 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/errors.py
--rw-rw-rw-   0 root         (0) root         (0)    10654 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/service_core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.742347 taegis-sdk-python-1.0.4/taegis_sdk_python/services/
--rw-rw-rw-   0 root         (0) root         (0)    14015 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.742347 taegis-sdk-python-1.0.4/taegis_sdk_python/services/access_points/
--rw-rw-rw-   0 root         (0) root         (0)      976 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/access_points/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2419 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/access_points/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     1814 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/access_points/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      893 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/access_points/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1145 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/access_points/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.742347 taegis-sdk-python-1.0.4/taegis_sdk_python/services/agent/
--rw-rw-rw-   0 root         (0) root         (0)     1154 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/agent/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      829 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/agent/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     2609 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/agent/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      841 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/agent/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     4740 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/agent/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.742347 taegis-sdk-python-1.0.4/taegis_sdk_python/services/alerts/
--rw-rw-rw-   0 root         (0) root         (0)      892 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/alerts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3900 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/alerts/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     6693 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/alerts/queries.py
--rw-rw-rw-   0 root         (0) root         (0)     1724 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/alerts/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    78106 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/alerts/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.746347 taegis-sdk-python-1.0.4/taegis_sdk_python/services/assets/
--rw-rw-rw-   0 root         (0) root         (0)      893 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/assets/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6375 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/assets/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    14954 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/assets/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      848 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/assets/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    23548 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/assets/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.746347 taegis-sdk-python-1.0.4/taegis_sdk_python/services/assets2/
--rw-rw-rw-   0 root         (0) root         (0)      905 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/assets2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9308 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/assets2/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    12807 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/assets2/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      855 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/assets2/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    26822 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/assets2/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.746347 taegis-sdk-python-1.0.4/taegis_sdk_python/services/audits/
--rw-rw-rw-   0 root         (0) root         (0)      893 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/audits/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1361 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/audits/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     3089 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/audits/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      848 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/audits/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    10314 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/audits/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.746347 taegis-sdk-python-1.0.4/taegis_sdk_python/services/clients/
--rw-rw-rw-   0 root         (0) root         (0)      905 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/clients/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3892 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/clients/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     2562 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/clients/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      855 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/clients/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3135 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/clients/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.750346 taegis-sdk-python-1.0.4/taegis_sdk_python/services/collector/
--rw-rw-rw-   0 root         (0) root         (0)      929 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/collector/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15823 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/collector/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    24262 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/collector/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      869 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/collector/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    31817 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/collector/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.750346 taegis-sdk-python-1.0.4/taegis_sdk_python/services/comments/
--rw-rw-rw-   0 root         (0) root         (0)      917 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/comments/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4946 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/comments/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     7300 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/comments/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      862 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/comments/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     5118 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/comments/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.750346 taegis-sdk-python-1.0.4/taegis_sdk_python/services/detector_registry/
--rw-rw-rw-   0 root         (0) root         (0)     1034 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/detector_registry/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      909 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/detector_registry/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     3194 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/detector_registry/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      921 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/detector_registry/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2932 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/detector_registry/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.750346 taegis-sdk-python-1.0.4/taegis_sdk_python/services/endpoint_command_manager/
--rw-rw-rw-   0 root         (0) root         (0)     1381 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/endpoint_command_manager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7325 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/endpoint_command_manager/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     3523 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/endpoint_command_manager/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      983 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/endpoint_command_manager/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     8546 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/endpoint_command_manager/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.754346 taegis-sdk-python-1.0.4/taegis_sdk_python/services/endpoint_management_service/
--rw-rw-rw-   0 root         (0) root         (0)     1417 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/endpoint_management_service/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3998 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/endpoint_management_service/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     5485 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/endpoint_management_service/queries.py
--rw-rw-rw-   0 root         (0) root         (0)     1004 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/endpoint_management_service/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     7782 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/endpoint_management_service/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.754346 taegis-sdk-python-1.0.4/taegis_sdk_python/services/entity_profile/
--rw-rw-rw-   0 root         (0) root         (0)      998 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/entity_profile/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      888 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/entity_profile/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     1818 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/entity_profile/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      900 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/entity_profile/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1090 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/entity_profile/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.754346 taegis-sdk-python-1.0.4/taegis_sdk_python/services/event_search/
--rw-rw-rw-   0 root         (0) root         (0)      965 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/event_search/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1619 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/event_search/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     2129 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/event_search/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      886 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/event_search/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     4437 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/event_search/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.754346 taegis-sdk-python-1.0.4/taegis_sdk_python/services/events/
--rw-rw-rw-   0 root         (0) root         (0)     1169 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/events/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1346 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/events/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     2775 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/events/queries.py
--rw-rw-rw-   0 root         (0) root         (0)     2508 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/events/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    10901 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/events/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.758346 taegis-sdk-python-1.0.4/taegis_sdk_python/services/exports/
--rw-rw-rw-   0 root         (0) root         (0)      905 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/exports/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12999 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/exports/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    10457 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/exports/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      855 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/exports/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    24620 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/exports/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.758346 taegis-sdk-python-1.0.4/taegis_sdk_python/services/fast_ioc/
--rw-rw-rw-   0 root         (0) root         (0)     1201 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/fast_ioc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      846 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/fast_ioc/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     3177 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/fast_ioc/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      858 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/fast_ioc/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3467 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/fast_ioc/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.758346 taegis-sdk-python-1.0.4/taegis_sdk_python/services/investigations/
--rw-rw-rw-   0 root         (0) root         (0)     1007 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/investigations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22228 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/investigations/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    28008 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/investigations/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      904 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/investigations/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    37546 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/investigations/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.758346 taegis-sdk-python-1.0.4/taegis_sdk_python/services/investigations2/
--rw-rw-rw-   0 root         (0) root         (0)     1019 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/investigations2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12204 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/investigations2/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     7214 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/investigations2/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      911 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/investigations2/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    42368 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/investigations2/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.762346 taegis-sdk-python-1.0.4/taegis_sdk_python/services/mitre_attack_info/
--rw-rw-rw-   0 root         (0) root         (0)     1025 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/mitre_attack_info/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      905 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/mitre_attack_info/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     9291 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/mitre_attack_info/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      917 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/mitre_attack_info/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3202 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/mitre_attack_info/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.762346 taegis-sdk-python-1.0.4/taegis_sdk_python/services/notebooks/
--rw-rw-rw-   0 root         (0) root         (0)      928 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/notebooks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2253 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/notebooks/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     1286 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/notebooks/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      869 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/notebooks/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1085 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/notebooks/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.762346 taegis-sdk-python-1.0.4/taegis_sdk_python/services/notifications/
--rw-rw-rw-   0 root         (0) root         (0)      986 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/notifications/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6858 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/notifications/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     2462 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/notifications/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      897 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/notifications/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     8811 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/notifications/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.762346 taegis-sdk-python-1.0.4/taegis_sdk_python/services/preferences/
--rw-rw-rw-   0 root         (0) root         (0)      962 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/preferences/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5923 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/preferences/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     5961 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/preferences/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      883 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/preferences/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    12949 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/preferences/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.766346 taegis-sdk-python-1.0.4/taegis_sdk_python/services/roadrunner/
--rw-rw-rw-   0 root         (0) root         (0)      941 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/roadrunner/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6287 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/roadrunner/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     6660 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/roadrunner/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      876 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/roadrunner/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    13046 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/roadrunner/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.766346 taegis-sdk-python-1.0.4/taegis_sdk_python/services/rules/
--rw-rw-rw-   0 root         (0) root         (0)      881 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/rules/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14207 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/rules/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    16097 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/rules/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      841 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/rules/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    22172 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/rules/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.766346 taegis-sdk-python-1.0.4/taegis_sdk_python/services/sharelinks/
--rw-rw-rw-   0 root         (0) root         (0)      941 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/sharelinks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1426 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/sharelinks/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     1381 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/sharelinks/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      876 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/sharelinks/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2578 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/sharelinks/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.766346 taegis-sdk-python-1.0.4/taegis_sdk_python/services/tenant_profiles/
--rw-rw-rw-   0 root         (0) root         (0)     1010 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/tenant_profiles/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17210 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/tenant_profiles/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     9170 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/tenant_profiles/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      907 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/tenant_profiles/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    19048 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/tenant_profiles/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.766346 taegis-sdk-python-1.0.4/taegis_sdk_python/services/tenants/
--rw-rw-rw-   0 root         (0) root         (0)     1303 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/tenants/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12659 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/tenants/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     5913 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/tenants/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      855 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/tenants/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    34203 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/tenants/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.770345 taegis-sdk-python-1.0.4/taegis_sdk_python/services/threat/
--rw-rw-rw-   0 root         (0) root         (0)      893 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/threat/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3443 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/threat/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    13781 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/threat/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      848 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/threat/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    53278 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/threat/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.770345 taegis-sdk-python-1.0.4/taegis_sdk_python/services/trip/
--rw-rw-rw-   0 root         (0) root         (0)      869 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/trip/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4135 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/trip/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     3905 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/trip/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      834 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/trip/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     7993 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/trip/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.770345 taegis-sdk-python-1.0.4/taegis_sdk_python/services/users/
--rw-rw-rw-   0 root         (0) root         (0)      881 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/users/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11558 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/users/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     7075 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/users/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      841 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/users/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    25732 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/services/users/types.py
--rw-rw-rw-   0 root         (0) root         (0)      979 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/tokens.py
--rw-rw-rw-   0 root         (0) root         (0)     7548 2023-08-03 16:38:50.000000 taegis-sdk-python-1.0.4/taegis_sdk_python/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 16:39:13.742347 taegis-sdk-python-1.0.4/taegis_sdk_python.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6228 2023-08-03 16:39:13.000000 taegis-sdk-python-1.0.4/taegis_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8488 2023-08-03 16:39:13.000000 taegis-sdk-python-1.0.4/taegis_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 16:39:13.000000 taegis-sdk-python-1.0.4/taegis_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      121 2023-08-03 16:39:13.000000 taegis-sdk-python-1.0.4/taegis_sdk_python.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-08-03 16:39:13.000000 taegis-sdk-python-1.0.4/taegis_sdk_python.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 17:24:23.391655 taegis-sdk-python-1.0.5/
+-rw-rw-rw-   0 root         (0) root         (0)    10173 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       84 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6228 2023-08-04 17:24:23.391655 taegis-sdk-python-1.0.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5793 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/requirements-dev.txt
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/requirements-test.txt
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-04 17:24:23.391655 taegis-sdk-python-1.0.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1571 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 17:24:23.367655 taegis-sdk-python-1.0.5/taegis_sdk_python/
+-rw-rw-rw-   0 root         (0) root         (0)      896 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1135 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/_consts.py
+-rw-rw-rw-   0 root         (0) root         (0)       23 2023-08-04 17:24:23.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     8618 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/authentication.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2637 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)    10654 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/service_core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 17:24:23.367655 taegis-sdk-python-1.0.5/taegis_sdk_python/services/
+-rw-rw-rw-   0 root         (0) root         (0)    14403 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 17:24:23.367655 taegis-sdk-python-1.0.5/taegis_sdk_python/services/access_points/
+-rw-rw-rw-   0 root         (0) root         (0)      976 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/access_points/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2419 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/access_points/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1814 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/access_points/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      893 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/access_points/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1145 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/access_points/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 17:24:23.367655 taegis-sdk-python-1.0.5/taegis_sdk_python/services/agent/
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/agent/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      829 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/agent/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3289 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/agent/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      841 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/agent/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     5205 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/agent/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 17:24:23.371655 taegis-sdk-python-1.0.5/taegis_sdk_python/services/alerts/
+-rw-rw-rw-   0 root         (0) root         (0)      892 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/alerts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4065 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/alerts/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     6693 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/alerts/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)     1724 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/alerts/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    79662 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/alerts/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 17:24:23.371655 taegis-sdk-python-1.0.5/taegis_sdk_python/services/assets/
+-rw-rw-rw-   0 root         (0) root         (0)      893 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/assets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6375 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/assets/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    14954 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/assets/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      848 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/assets/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    23548 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/assets/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 17:24:23.371655 taegis-sdk-python-1.0.5/taegis_sdk_python/services/assets2/
+-rw-rw-rw-   0 root         (0) root         (0)      905 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/assets2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9308 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/assets2/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    12807 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/assets2/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      855 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/assets2/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    26822 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/assets2/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 17:24:23.371655 taegis-sdk-python-1.0.5/taegis_sdk_python/services/audits/
+-rw-rw-rw-   0 root         (0) root         (0)      893 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/audits/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1361 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/audits/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3089 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/audits/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      848 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/audits/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    10314 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/audits/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 17:24:23.371655 taegis-sdk-python-1.0.5/taegis_sdk_python/services/clients/
+-rw-rw-rw-   0 root         (0) root         (0)      905 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/clients/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3892 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/clients/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2562 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/clients/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      855 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/clients/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3135 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/clients/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 17:24:23.375655 taegis-sdk-python-1.0.5/taegis_sdk_python/services/collector/
+-rw-rw-rw-   0 root         (0) root         (0)      929 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/collector/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15823 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/collector/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    25773 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/collector/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      869 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/collector/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    31924 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/collector/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 17:24:23.375655 taegis-sdk-python-1.0.5/taegis_sdk_python/services/comments/
+-rw-rw-rw-   0 root         (0) root         (0)      917 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/comments/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4946 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/comments/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     7300 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/comments/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      862 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/comments/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     5118 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/comments/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 17:24:23.375655 taegis-sdk-python-1.0.5/taegis_sdk_python/services/detector_registry/
+-rw-rw-rw-   0 root         (0) root         (0)     1034 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/detector_registry/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      909 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/detector_registry/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3194 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/detector_registry/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      921 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/detector_registry/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2932 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/detector_registry/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 17:24:23.375655 taegis-sdk-python-1.0.5/taegis_sdk_python/services/endpoint_command_manager/
+-rw-rw-rw-   0 root         (0) root         (0)     1381 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/endpoint_command_manager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7325 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/endpoint_command_manager/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3523 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/endpoint_command_manager/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      983 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/endpoint_command_manager/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     8546 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/endpoint_command_manager/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 17:24:23.375655 taegis-sdk-python-1.0.5/taegis_sdk_python/services/endpoint_management_service/
+-rw-rw-rw-   0 root         (0) root         (0)     1417 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/endpoint_management_service/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3998 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/endpoint_management_service/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     5485 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/endpoint_management_service/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)     1004 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/endpoint_management_service/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     7782 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/endpoint_management_service/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 17:24:23.379655 taegis-sdk-python-1.0.5/taegis_sdk_python/services/entity_profile/
+-rw-rw-rw-   0 root         (0) root         (0)      998 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/entity_profile/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      888 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/entity_profile/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1818 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/entity_profile/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      900 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/entity_profile/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1090 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/entity_profile/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 17:24:23.379655 taegis-sdk-python-1.0.5/taegis_sdk_python/services/event_search/
+-rw-rw-rw-   0 root         (0) root         (0)      965 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/event_search/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1619 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/event_search/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2129 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/event_search/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      886 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/event_search/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     4228 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/event_search/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 17:24:23.379655 taegis-sdk-python-1.0.5/taegis_sdk_python/services/events/
+-rw-rw-rw-   0 root         (0) root         (0)     1169 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/events/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1346 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/events/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2775 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/events/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)     2508 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/events/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    10901 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/events/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 17:24:23.379655 taegis-sdk-python-1.0.5/taegis_sdk_python/services/exports/
+-rw-rw-rw-   0 root         (0) root         (0)      905 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/exports/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12999 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/exports/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    10457 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/exports/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      855 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/exports/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    24620 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/exports/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 17:24:23.379655 taegis-sdk-python-1.0.5/taegis_sdk_python/services/fast_ioc/
+-rw-rw-rw-   0 root         (0) root         (0)     1201 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/fast_ioc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      846 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/fast_ioc/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3177 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/fast_ioc/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      858 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/fast_ioc/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3467 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/fast_ioc/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 17:24:23.379655 taegis-sdk-python-1.0.5/taegis_sdk_python/services/investigations/
+-rw-rw-rw-   0 root         (0) root         (0)     1007 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/investigations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22228 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/investigations/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    28008 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/investigations/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      904 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/investigations/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    37546 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/investigations/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 17:24:23.383655 taegis-sdk-python-1.0.5/taegis_sdk_python/services/investigations2/
+-rw-rw-rw-   0 root         (0) root         (0)     1019 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/investigations2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12204 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/investigations2/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     7214 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/investigations2/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      911 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/investigations2/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    45195 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/investigations2/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 17:24:23.383655 taegis-sdk-python-1.0.5/taegis_sdk_python/services/mitre_attack_info/
+-rw-rw-rw-   0 root         (0) root         (0)     1025 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/mitre_attack_info/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      905 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/mitre_attack_info/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     9291 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/mitre_attack_info/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      917 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/mitre_attack_info/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3202 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/mitre_attack_info/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 17:24:23.383655 taegis-sdk-python-1.0.5/taegis_sdk_python/services/multi_tenant_context/
+-rw-rw-rw-   0 root         (0) root         (0)     1061 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/multi_tenant_context/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4567 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/multi_tenant_context/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     5648 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/multi_tenant_context/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      955 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/multi_tenant_context/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     6279 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/multi_tenant_context/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 17:24:23.383655 taegis-sdk-python-1.0.5/taegis_sdk_python/services/notebooks/
+-rw-rw-rw-   0 root         (0) root         (0)      928 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/notebooks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2253 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/notebooks/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1286 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/notebooks/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      869 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/notebooks/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1085 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/notebooks/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 17:24:23.383655 taegis-sdk-python-1.0.5/taegis_sdk_python/services/notifications/
+-rw-rw-rw-   0 root         (0) root         (0)      986 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/notifications/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6858 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/notifications/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2462 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/notifications/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      897 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/notifications/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     8811 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/notifications/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 17:24:23.387655 taegis-sdk-python-1.0.5/taegis_sdk_python/services/preferences/
+-rw-rw-rw-   0 root         (0) root         (0)      962 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/preferences/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5923 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/preferences/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     5961 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/preferences/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      883 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/preferences/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    12949 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/preferences/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 17:24:23.387655 taegis-sdk-python-1.0.5/taegis_sdk_python/services/roadrunner/
+-rw-rw-rw-   0 root         (0) root         (0)      941 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/roadrunner/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6287 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/roadrunner/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     6063 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/roadrunner/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      876 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/roadrunner/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    13046 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/roadrunner/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 17:24:23.387655 taegis-sdk-python-1.0.5/taegis_sdk_python/services/rules/
+-rw-rw-rw-   0 root         (0) root         (0)      881 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/rules/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14207 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/rules/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    16097 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/rules/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      841 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/rules/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    22172 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/rules/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 17:24:23.387655 taegis-sdk-python-1.0.5/taegis_sdk_python/services/sharelinks/
+-rw-rw-rw-   0 root         (0) root         (0)      941 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/sharelinks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1426 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/sharelinks/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1381 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/sharelinks/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      876 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/sharelinks/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2578 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/sharelinks/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 17:24:23.387655 taegis-sdk-python-1.0.5/taegis_sdk_python/services/tenant_profiles/
+-rw-rw-rw-   0 root         (0) root         (0)     1010 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/tenant_profiles/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17210 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/tenant_profiles/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     9170 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/tenant_profiles/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      907 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/tenant_profiles/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    19048 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/tenant_profiles/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 17:24:23.391655 taegis-sdk-python-1.0.5/taegis_sdk_python/services/tenants/
+-rw-rw-rw-   0 root         (0) root         (0)     1303 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/tenants/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12659 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/tenants/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     5913 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/tenants/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      855 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/tenants/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    34227 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/tenants/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 17:24:23.391655 taegis-sdk-python-1.0.5/taegis_sdk_python/services/threat/
+-rw-rw-rw-   0 root         (0) root         (0)      893 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/threat/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3443 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/threat/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    13781 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/threat/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      848 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/threat/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    53278 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/threat/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 17:24:23.391655 taegis-sdk-python-1.0.5/taegis_sdk_python/services/trip/
+-rw-rw-rw-   0 root         (0) root         (0)      869 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/trip/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4135 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/trip/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3905 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/trip/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      834 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/trip/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     7993 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/trip/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 17:24:23.391655 taegis-sdk-python-1.0.5/taegis_sdk_python/services/users/
+-rw-rw-rw-   0 root         (0) root         (0)      881 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/users/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12152 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/users/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     7075 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/users/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      841 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/users/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    25732 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/services/users/types.py
+-rw-rw-rw-   0 root         (0) root         (0)      979 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/tokens.py
+-rw-rw-rw-   0 root         (0) root         (0)     7548 2023-08-04 17:24:05.000000 taegis-sdk-python-1.0.5/taegis_sdk_python/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 17:24:23.367655 taegis-sdk-python-1.0.5/taegis_sdk_python.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6228 2023-08-04 17:24:23.000000 taegis-sdk-python-1.0.5/taegis_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8790 2023-08-04 17:24:23.000000 taegis-sdk-python-1.0.5/taegis_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 17:24:23.000000 taegis-sdk-python-1.0.5/taegis_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      121 2023-08-04 17:24:23.000000 taegis-sdk-python-1.0.5/taegis_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-08-04 17:24:23.000000 taegis-sdk-python-1.0.5/taegis_sdk_python.egg-info/top_level.txt
```

### Comparing `taegis-sdk-python-1.0.4/LICENSE` & `taegis-sdk-python-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/PKG-INFO` & `taegis-sdk-python-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taegis-sdk-python
-Version: 1.0.4
+Version: 1.0.5
 Summary: Taegis Python SDK
 Home-page: https://github.com/secureworks/taegis-sdk-python
 Author: Secureworks
 Author-email: sdks@secureworks.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `taegis-sdk-python-1.0.4/README.md` & `taegis-sdk-python-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/setup.py` & `taegis-sdk-python-1.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/__init__.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/_consts.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/_consts.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/authentication.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/authentication.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/config.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/config.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/errors.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/errors.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/service_core.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/service_core.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/__init__.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 from taegis_sdk_python.services.event_search import EventSearchService
 from taegis_sdk_python.services.events import EventsService
 from taegis_sdk_python.services.exports import ExportsService
 from taegis_sdk_python.services.fast_ioc import FastIocService
 from taegis_sdk_python.services.investigations import InvestigationsService
 from taegis_sdk_python.services.investigations2 import Investigations2Service
 from taegis_sdk_python.services.mitre_attack_info import MitreAttackInfoService
+from taegis_sdk_python.services.multi_tenant_context import MultiTenantContextService
 from taegis_sdk_python.services.notebooks import NotebooksService
 from taegis_sdk_python.services.notifications import NotificationsService
 from taegis_sdk_python.services.preferences import PreferencesService
 from taegis_sdk_python.services.roadrunner import RoadrunnerService
 from taegis_sdk_python.services.rules import RulesService
 from taegis_sdk_python.services.sharelinks import SharelinksService
 from taegis_sdk_python.services.tenant_profiles import TenantProfilesService
@@ -110,14 +111,15 @@
         self._event_search = None
         self._events = None
         self._exports = None
         self._fast_ioc = None
         self._investigations = None
         self._investigations2 = None
         self._mitre_attack_info = None
+        self._multi_tenant_context = None
         self._notebooks = None
         self._notifications = None
         self._preferences = None
         self._roadrunner = None
         self._rules = None
         self._core = None
         self._sharelinks = None
@@ -342,14 +344,21 @@
     def mitre_attack_info(self):
         """MitreAttackInfo Service Endpoint."""
         if not self._mitre_attack_info:
             self._mitre_attack_info = MitreAttackInfoService(self)
         return self._mitre_attack_info
 
     @property
+    def multi_tenant_context(self):
+        """MultiTenantContext Service Endpoint."""
+        if not self._multi_tenant_context:
+            self._multi_tenant_context = MultiTenantContextService(self)
+        return self._multi_tenant_context
+
+    @property
     def notebooks(self):
         """Notebooks Service Endpoint."""
         if not self._notebooks:
             self._notebooks = NotebooksService(self)
         return self._notebooks
 
     @property
```

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/access_points/__init__.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/access_points/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/access_points/mutations.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/access_points/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/access_points/queries.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/access_points/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/access_points/subscriptions.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/access_points/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/access_points/types.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/access_points/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/agent/__init__.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/agent/mutations.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/agent/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/agent/queries.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/agent/queries.py`

 * *Files 8% similar despite different names*

```diff
@@ -76,7 +76,26 @@
                 "id": prepare_input(id_),
             },
             output=build_output_string(PackageSignedUrl),
         )
         if result.get(endpoint) is not None:
             return PackageSignedUrl.from_dict(result.get(endpoint))
         raise GraphQLNoRowsInResultSetError("for query agentPackageSignedUrlByID")
+
+    def available_channels(
+        self, platform: Optional[AgentPlatform] = None
+    ) -> List[ReleaseChannelsConfig]:
+        """None."""
+        endpoint = "availableChannels"
+
+        result = self.service.execute_query(
+            endpoint=endpoint,
+            variables={
+                "platform": prepare_input(platform),
+            },
+            output=build_output_string(ReleaseChannelsConfig),
+        )
+        if result.get(endpoint) is not None:
+            return ReleaseChannelsConfig.schema().load(
+                [r or {} for r in result.get(endpoint)], many=True
+            )
+        raise GraphQLNoRowsInResultSetError("for query availableChannels")
```

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/agent/subscriptions.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/agent/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/agent/types.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/agent/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,17 +40,18 @@
     PKG = "PKG"
     GPG = "GPG"
 
 
 class AgentChannel(str, Enum):
     """AgentChannel."""
 
-    BETA = "BETA"
-    PREVIEW = "PREVIEW"
     STABLE = "STABLE"
+    PREVIEW = "PREVIEW"
+    BETA = "BETA"
+    INTERNAL_PREVIEW = "INTERNAL_PREVIEW"
     DEV = "DEV"
     CANARY = "CANARY"
     QE_PREV = "QE_PREV"
     QE_NEXT = "QE_NEXT"
     WEEKLY = "WEEKLY"
     WEEKLY_NEXT = "WEEKLY_NEXT"
 
@@ -81,14 +82,28 @@
     signed_url: Optional[str] = field(
         default=None, metadata=config(field_name="signedUrl")
     )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
+class ReleaseChannelsConfig:
+    """ReleaseChannelsConfig."""
+
+    name: Optional[str] = field(default=None, metadata=config(field_name="name"))
+    description: Optional[str] = field(
+        default=None, metadata=config(field_name="description")
+    )
+    internal: Optional[bool] = field(
+        default=None, metadata=config(field_name="internal")
+    )
+
+
+@dataclass_json
+@dataclass(order=True, eq=True, frozen=True)
 class PackageDownloadInput:
     """PackageDownloadInput."""
 
     version: Optional[str] = field(default=None, metadata=config(field_name="version"))
     language: Optional[str] = field(
         default=None, metadata=config(field_name="language")
     )
```

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/alerts/__init__.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/alerts/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/alerts/mutations.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/alerts/mutations.py`

 * *Files 6% similar despite different names*

```diff
@@ -89,14 +89,18 @@
 
     def alerts_service_evict(
         self, in_: Optional[EvictRequestInput] = None
     ) -> EvictResponse:
         """DEPRECATED: Does not do anything other than to return OK. No replacement necessary.."""
         endpoint = "alertsServiceEvict"
 
+        log.warning(
+            f"GraphQL Mutation `{endpoint}` is deprecated: 'does not do anything other than to return OK. no replacement necessary'"
+        )
+
         result = self.service.execute_mutation(
             endpoint=endpoint,
             variables={
                 "in": prepare_input(in_),
             },
             output=build_output_string(EvictResponse),
         )
```

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/alerts/queries.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/alerts/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/alerts/subscriptions.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/alerts/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/alerts/types.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/alerts/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,15 +143,22 @@
     """BulkInvestigationsRequestInput."""
 
     query: Optional[str] = field(default=None, metadata=config(field_name="query"))
     investigation_id: Optional[str] = field(
         default=None, metadata=config(field_name="investigation_id")
     )
     genesis_alerts: Optional[List[str]] = field(
-        default=None, metadata=config(field_name="genesis_alerts")
+        default=None,
+        metadata=config(
+            metadata={
+                "deprecated": True,
+                "deprecation_reason": "used to flag specific alerts as the genesis of the investigation",
+            },
+            field_name="genesis_alerts",
+        ),
     )
     alerts: Optional[List[str]] = field(
         default=None, metadata=config(field_name="alerts")
     )
     tenant: Optional[str] = field(default=None, metadata=config(field_name="tenant"))
 
 
@@ -186,15 +193,24 @@
 @dataclass(order=True, eq=True, frozen=True)
 class PollRequestInput:
     """PollRequestInput."""
 
     search_id: Optional[str] = field(
         default=None, metadata=config(field_name="search_id")
     )
-    part_id: Optional[int] = field(default=None, metadata=config(field_name="part_id"))
+    part_id: Optional[int] = field(
+        default=None,
+        metadata=config(
+            metadata={
+                "deprecated": True,
+                "deprecation_reason": "part id is advanced transparently with each new call now",
+            },
+            field_name="part_id",
+        ),
+    )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
 class SearchRequestInput:
     """SearchRequestInput."""
 
@@ -477,19 +493,19 @@
 
     key: Optional[str] = field(default=None, metadata=config(field_name="key"))
     value: Optional[str] = field(default=None, metadata=config(field_name="value"))
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
-class AggregationResponse:
-    """AggregationResponse."""
+class AggregationKeys:
+    """AggregationKeys."""
 
     key: Optional[str] = field(default=None, metadata=config(field_name="key"))
-    value: Optional[float] = field(default=None, metadata=config(field_name="value"))
+    value: Optional[str] = field(default=None, metadata=config(field_name="value"))
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
 class AlertRuleReference:
     """AlertRuleReference."""
 
@@ -544,15 +560,22 @@
 class AuthScanLogonAttempt:
     """AuthScanLogonAttempt."""
 
     target_user_name: Optional[str] = field(
         default=None, metadata=config(field_name="target_user_name")
     )
     has_logon_success: Optional[bool] = field(
-        default=None, metadata=config(field_name="has_logon_success")
+        default=None,
+        metadata=config(
+            metadata={
+                "deprecated": True,
+                "deprecation_reason": "see list in successful_logon_attempts",
+            },
+            field_name="has_logon_success",
+        ),
     )
     num_attempts: Optional[int] = field(
         default=None, metadata=config(field_name="num_attempts")
     )
 
 
 @dataclass_json
@@ -1043,15 +1066,19 @@
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
 class Investigation:
     """Investigation."""
 
     id: Optional[str] = field(default=None, metadata=config(field_name="id"))
     genesis_alerts_flag: Optional[str] = field(
-        default=None, metadata=config(field_name="GenesisAlertsFlag")
+        default=None,
+        metadata=config(
+            metadata={"deprecated": True, "deprecation_reason": "not in use anymore"},
+            field_name="GenesisAlertsFlag",
+        ),
     )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
 class Collection:
     """Collection."""
@@ -1156,14 +1183,35 @@
     record: Optional[List[KeyValueRecordIndexed]] = field(
         default=None, metadata=config(field_name="record")
     )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
+class AggregationResponse:
+    """AggregationResponse."""
+
+    key: Optional[str] = field(
+        default=None,
+        metadata=config(
+            metadata={
+                "deprecated": True,
+                "deprecation_reason": "use keys instead for the broken out name/value pairs",
+            },
+            field_name="key",
+        ),
+    )
+    value: Optional[float] = field(default=None, metadata=config(field_name="value"))
+    keys: Optional[List[AggregationKeys]] = field(
+        default=None, metadata=config(field_name="keys")
+    )
+
+
+@dataclass_json
+@dataclass(order=True, eq=True, frozen=True)
 class AlertPriority:
     """AlertPriority."""
 
     value: Optional[float] = field(default=None, metadata=config(field_name="value"))
     prioritizer: Optional[str] = field(
         default=None, metadata=config(field_name="prioritizer")
     )
@@ -1753,15 +1801,22 @@
 class UpdateInvestigationRequestInput:
     """UpdateInvestigationRequestInput."""
 
     investigation_id: Optional[str] = field(
         default=None, metadata=config(field_name="investigation_id")
     )
     genesis_alerts: Optional[List[str]] = field(
-        default=None, metadata=config(field_name="genesis_alerts")
+        default=None,
+        metadata=config(
+            metadata={
+                "deprecated": True,
+                "deprecation_reason": "was used to flag specific alerts as the genesis of the investigation",
+            },
+            field_name="genesis_alerts",
+        ),
     )
     alerts: Optional[List[str]] = field(
         default=None, metadata=config(field_name="alerts")
     )
     tenant: Optional[str] = field(default=None, metadata=config(field_name="tenant"))
     user_id: Optional[str] = field(default=None, metadata=config(field_name="user_id"))
     operation: Optional[InvestigationOperation] = field(
```

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/assets/__init__.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/assets/mutations.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/assets/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/assets/queries.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/assets/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/assets/subscriptions.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/assets/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/assets/types.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/assets/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/assets2/__init__.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/assets2/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/assets2/mutations.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/assets2/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/assets2/queries.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/assets2/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/assets2/subscriptions.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/assets2/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/assets2/types.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/assets2/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/audits/__init__.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/audits/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/audits/mutations.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/audits/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/audits/queries.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/audits/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/audits/subscriptions.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/audits/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/audits/types.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/audits/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/clients/__init__.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/clients/mutations.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/clients/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/clients/queries.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/clients/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/clients/subscriptions.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/clients/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/clients/types.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/clients/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/collector/__init__.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/collector/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/collector/mutations.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/collector/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/collector/queries.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/collector/queries.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,14 +81,54 @@
         )
         if result.get(endpoint) is not None:
             return ClusterNodeTimeSeries.schema().load(
                 [r or {} for r in result.get(endpoint)], many=True
             )
         raise GraphQLNoRowsInResultSetError("for query getClusterBacklogAge")
 
+    def get_cluster_transmit_bytes(
+        self, cluster_id: str, time_range: TimeRange
+    ) -> List[ClusterNodeTimeSeries]:
+        """None."""
+        endpoint = "getClusterTransmitBytes"
+
+        result = self.service.execute_query(
+            endpoint=endpoint,
+            variables={
+                "clusterID": prepare_input(cluster_id),
+                "timeRange": prepare_input(time_range),
+            },
+            output=build_output_string(ClusterNodeTimeSeries),
+        )
+        if result.get(endpoint) is not None:
+            return ClusterNodeTimeSeries.schema().load(
+                [r or {} for r in result.get(endpoint)], many=True
+            )
+        raise GraphQLNoRowsInResultSetError("for query getClusterTransmitBytes")
+
+    def get_cluster_receive_bytes(
+        self, cluster_id: str, time_range: TimeRange
+    ) -> List[ClusterNodeTimeSeries]:
+        """None."""
+        endpoint = "getClusterReceiveBytes"
+
+        result = self.service.execute_query(
+            endpoint=endpoint,
+            variables={
+                "clusterID": prepare_input(cluster_id),
+                "timeRange": prepare_input(time_range),
+            },
+            output=build_output_string(ClusterNodeTimeSeries),
+        )
+        if result.get(endpoint) is not None:
+            return ClusterNodeTimeSeries.schema().load(
+                [r or {} for r in result.get(endpoint)], many=True
+            )
+        raise GraphQLNoRowsInResultSetError("for query getClusterReceiveBytes")
+
     def get_clusters_by_ids(self, cluster_ids: List[str]) -> List[Cluster]:
         """Get clusters by IDs."""
         endpoint = "getClustersByIDs"
 
         result = self.service.execute_query(
             endpoint=endpoint,
             variables={
```

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/collector/subscriptions.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/collector/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/collector/types.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/collector/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -637,14 +637,17 @@
         default=None, metadata=config(field_name="clusterID")
     )
     tenant: Optional[str] = field(default=None, metadata=config(field_name="tenant"))
     node_id: Optional[str] = field(default=None, metadata=config(field_name="nodeId"))
     node_name: Optional[str] = field(
         default=None, metadata=config(field_name="nodeName")
     )
+    ip_address: Optional[str] = field(
+        default=None, metadata=config(field_name="ipAddress")
+    )
     val: Optional[List[TimeSeries]] = field(
         default=None, metadata=config(field_name="val")
     )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
```

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/comments/__init__.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/comments/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/comments/mutations.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/comments/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/comments/queries.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/comments/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/comments/subscriptions.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/comments/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/comments/types.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/comments/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/detector_registry/__init__.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/detector_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/detector_registry/mutations.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/detector_registry/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/detector_registry/queries.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/detector_registry/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/detector_registry/subscriptions.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/detector_registry/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/detector_registry/types.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/detector_registry/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/endpoint_command_manager/__init__.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/endpoint_command_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/endpoint_command_manager/mutations.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/endpoint_command_manager/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/endpoint_command_manager/queries.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/endpoint_command_manager/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/endpoint_command_manager/subscriptions.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/endpoint_command_manager/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/endpoint_command_manager/types.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/endpoint_command_manager/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/endpoint_management_service/__init__.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/endpoint_management_service/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/endpoint_management_service/mutations.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/endpoint_management_service/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/endpoint_management_service/queries.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/endpoint_management_service/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/endpoint_management_service/subscriptions.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/endpoint_management_service/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/endpoint_management_service/types.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/endpoint_management_service/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/entity_profile/__init__.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/entity_profile/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/entity_profile/mutations.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/entity_profile/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/entity_profile/queries.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/entity_profile/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/entity_profile/subscriptions.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/entity_profile/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/entity_profile/types.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/entity_profile/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/event_search/__init__.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/event_search/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/event_search/mutations.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/event_search/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/event_search/queries.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/event_search/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/event_search/subscriptions.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/event_search/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/event_search/types.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/event_search/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,22 +42,15 @@
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
 class AuxiliaryEventsByIDOptions:
     """AuxiliaryEventsByIDOptions."""
 
     search_events_api_first: Optional[bool] = field(
-        default=None,
-        metadata=config(
-            metadata={
-                "deprecated": True,
-                "deprecation_reason": "Obsolete. Events-API is now used automatically only if needed",
-            },
-            field_name="searchEventsAPIFirst",
-        ),
+        default=None, metadata=config(field_name="searchEventsAPIFirst")
     )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
 class AsynchronousEventsSearchPrepInputResponse:
     """AsynchronousEventsSearchPrepInputResponse."""
```

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/events/__init__.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/events/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/events/mutations.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/events/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/events/queries.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/events/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/events/subscriptions.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/events/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/events/types.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/events/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/exports/__init__.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/exports/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/exports/mutations.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/exports/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/exports/queries.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/exports/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/exports/subscriptions.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/exports/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/exports/types.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/exports/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/fast_ioc/__init__.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/fast_ioc/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/fast_ioc/mutations.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/fast_ioc/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/fast_ioc/queries.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/fast_ioc/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/fast_ioc/subscriptions.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/fast_ioc/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/fast_ioc/types.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/fast_ioc/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/investigations/__init__.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/investigations/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/investigations/mutations.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/investigations/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/investigations/queries.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/investigations/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/investigations/subscriptions.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/investigations/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/investigations/types.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/investigations/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/investigations2/__init__.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/investigations2/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/investigations2/mutations.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/investigations2/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/investigations2/queries.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/investigations2/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/investigations2/subscriptions.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/investigations2/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/investigations2/types.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/investigations2/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,17 @@
     SECURITY_INVESTIGATION = "SECURITY_INVESTIGATION"
     INCIDENT_RESPONSE = "INCIDENT_RESPONSE"
     THREAT_HUNT = "THREAT_HUNT"
     MANAGED_XDR_THREAT_HUNT = "MANAGED_XDR_THREAT_HUNT"
     CTU_THREAT_HUNT = "CTU_THREAT_HUNT"
     MANAGED_XDR_ELITE_THREAT_HUNT = "MANAGED_XDR_ELITE_THREAT_HUNT"
     SECUREWORKS_INCIDENT_RESPONSE = "SECUREWORKS_INCIDENT_RESPONSE"
+    UNLIMITED_RESPONSE = "UNLIMITED_RESPONSE"
+    MANAGED_XDR_OT_INVESTIGATION = "MANAGED_XDR_OT_INVESTIGATION"
+    OT_INVESTIGATION = "OT_INVESTIGATION"
 
 
 class InvestigationProcessingState(str, Enum):
     """InvestigationProcessingState."""
 
     SUCCESS = "SUCCESS"
     FAILED = "FAILED"
@@ -159,14 +162,76 @@
     """ArchiveInvestigationInput."""
 
     id: Optional[str] = field(default=None, metadata=config(field_name="id"))
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
+class Metric:
+    """Metric."""
+
+    draft_promoted_at: Optional[str] = field(
+        default=None, metadata=config(field_name="draftPromotedAt")
+    )
+    time_to_draft_promotion: Optional[int] = field(
+        default=None, metadata=config(field_name="timeToDraftPromotion")
+    )
+    draft_promoted_by: Optional[str] = field(
+        default=None, metadata=config(field_name="draftPromotedBy")
+    )
+    handed_off_at: Optional[str] = field(
+        default=None, metadata=config(field_name="handedOffAt")
+    )
+    time_to_hand_off: Optional[int] = field(
+        default=None, metadata=config(field_name="timeToHandOff")
+    )
+    handed_off_by: Optional[str] = field(
+        default=None, metadata=config(field_name="handedOffBy")
+    )
+    acknowledged_at: Optional[str] = field(
+        default=None, metadata=config(field_name="acknowledgedAt")
+    )
+    time_to_acknowledgement: Optional[int] = field(
+        default=None, metadata=config(field_name="timeToAcknowledgement")
+    )
+    acknowledged_by: Optional[str] = field(
+        default=None, metadata=config(field_name="acknowledgedBy")
+    )
+    resolved_at: Optional[str] = field(
+        default=None, metadata=config(field_name="resolvedAt")
+    )
+    time_to_resolution: Optional[int] = field(
+        default=None, metadata=config(field_name="timeToResolution")
+    )
+    resolved_by: Optional[str] = field(
+        default=None, metadata=config(field_name="resolvedBy")
+    )
+
+
+@dataclass_json
+@dataclass(order=True, eq=True, frozen=True)
+class Metrics:
+    """Metrics."""
+
+    mean_time_to_handoff: Optional[int] = field(
+        default=None, metadata=config(field_name="meanTimeToHandoff")
+    )
+    mean_time_to_acknowledgement: Optional[int] = field(
+        default=None, metadata=config(field_name="meanTimeToAcknowledgement")
+    )
+    mean_time_to_resolution: Optional[int] = field(
+        default=None, metadata=config(field_name="meanTimeToResolution")
+    )
+    mean_time_to_draft_promotion: Optional[int] = field(
+        default=None, metadata=config(field_name="meanTimeToDraftPromotion")
+    )
+
+
+@dataclass_json
+@dataclass(order=True, eq=True, frozen=True)
 class AddEvidenceToInvestigationResult:
     """AddEvidenceToInvestigationResult."""
 
     investigation_id: Optional[str] = field(
         default=None, metadata=config(field_name="investigationId")
     )
     alerts: Optional[List[str]] = field(
@@ -384,14 +449,17 @@
 class AddCommentToInvestigationInput:
     """AddCommentToInvestigationInput."""
 
     comment: Optional[str] = field(default=None, metadata=config(field_name="comment"))
     investigation_id: Optional[str] = field(
         default=None, metadata=config(field_name="investigationId")
     )
+    is_internal: Optional[bool] = field(
+        default=None, metadata=config(field_name="isInternal")
+    )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
 class UpdateInvestigationCommentInput:
     """UpdateInvestigationCommentInput."""
 
@@ -909,14 +977,17 @@
     )
     mentions_ids: Optional[List[str]] = field(
         default=None, metadata=config(field_name="mentionsIds")
     )
     read_by_ids: Optional[List[str]] = field(
         default=None, metadata=config(field_name="readByIds")
     )
+    is_internal: Optional[bool] = field(
+        default=None, metadata=config(field_name="isInternal")
+    )
     author: Optional[TDRUser] = field(
         default=None, metadata=config(field_name="author")
     )
     mentions_users: Optional[List[TDRUser]] = field(
         default=None, metadata=config(field_name="mentionsUsers")
     )
     read_by: Optional[List[TDRUser]] = field(
@@ -1126,27 +1197,15 @@
     )
     processing_status: Optional[InvestigationProcessingStatus] = field(
         default=None, metadata=config(field_name="processingStatus")
     )
     comments_count: Optional[InvestigationCommentsCount] = field(
         default=None, metadata=config(field_name="commentsCount")
     )
-
-
-@dataclass_json
-@dataclass(order=True, eq=True, frozen=True)
-class InvestigationsV2:
-    """InvestigationsV2."""
-
-    total_count: Optional[int] = field(
-        default=None, metadata=config(field_name="totalCount")
-    )
-    investigations: Optional[List[InvestigationV2]] = field(
-        default=None, metadata=config(field_name="investigations")
-    )
+    metric: Optional[Metric] = field(default=None, metadata=config(field_name="metric"))
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
 class InvestigationTemplates:
     """InvestigationTemplates."""
 
@@ -1195,16 +1254,35 @@
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
 class CommentsV2:
     """CommentsV2."""
 
+    total_count: Optional[int] = field(
+        default=None, metadata=config(field_name="totalCount")
+    )
     comments: Optional[List[CommentV2]] = field(
         default=None, metadata=config(field_name="comments")
     )
 
 
+@dataclass_json
+@dataclass(order=True, eq=True, frozen=True)
+class InvestigationsV2:
+    """InvestigationsV2."""
+
+    total_count: Optional[int] = field(
+        default=None, metadata=config(field_name="totalCount")
+    )
+    investigations: Optional[List[InvestigationV2]] = field(
+        default=None, metadata=config(field_name="investigations")
+    )
+    metrics: Optional[Metrics] = field(
+        default=None, metadata=config(field_name="metrics")
+    )
+
+
 InvestigationResource = Union[
     InvestigationTemplate,
     InvestigationRule,
 ]
```

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/mitre_attack_info/__init__.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/mitre_attack_info/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/mitre_attack_info/mutations.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/mitre_attack_info/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/mitre_attack_info/queries.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/mitre_attack_info/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/mitre_attack_info/subscriptions.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/mitre_attack_info/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/mitre_attack_info/types.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/mitre_attack_info/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/notebooks/__init__.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/notebooks/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/notebooks/mutations.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/notebooks/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/notebooks/queries.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/notebooks/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/notebooks/subscriptions.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/notebooks/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/notebooks/types.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/notebooks/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/notifications/__init__.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/notifications/mutations.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/notifications/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/notifications/queries.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/notifications/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/notifications/subscriptions.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/notifications/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/notifications/types.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/notifications/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/preferences/__init__.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/preferences/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/preferences/mutations.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/preferences/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/preferences/queries.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/preferences/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/preferences/subscriptions.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/preferences/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/preferences/types.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/preferences/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/roadrunner/__init__.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/roadrunner/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/roadrunner/mutations.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/roadrunner/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/roadrunner/queries.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/roadrunner/queries.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,31 +43,14 @@
         )
         if result.get(endpoint) is not None:
             return SyslogSample.schema().load(
                 [r or {} for r in result.get(endpoint)], many=True
             )
         raise GraphQLNoRowsInResultSetError("for query syslogSample")
 
-    def syslog_message_count(
-        self, options: SyslogMessageCountOptions
-    ) -> SyslogMessageCount:
-        """None."""
-        endpoint = "syslogMessageCount"
-
-        result = self.service.execute_query(
-            endpoint=endpoint,
-            variables={
-                "options": prepare_input(options),
-            },
-            output=build_output_string(SyslogMessageCount),
-        )
-        if result.get(endpoint) is not None:
-            return SyslogMessageCount.from_dict(result.get(endpoint))
-        raise GraphQLNoRowsInResultSetError("for query syslogMessageCount")
-
     def all_parsers(self) -> List[Parser]:
         """None."""
         endpoint = "allParsers"
 
         result = self.service.execute_query(
             endpoint=endpoint, variables={}, output=build_output_string(Parser)
         )
```

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/roadrunner/subscriptions.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/roadrunner/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/roadrunner/types.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/roadrunner/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/rules/__init__.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/rules/mutations.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/rules/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/rules/queries.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/rules/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/rules/subscriptions.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/rules/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/rules/types.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/rules/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/sharelinks/__init__.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/sharelinks/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/sharelinks/mutations.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/sharelinks/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/sharelinks/queries.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/sharelinks/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/sharelinks/subscriptions.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/sharelinks/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/sharelinks/types.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/sharelinks/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/tenant_profiles/__init__.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/tenant_profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/tenant_profiles/mutations.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/tenant_profiles/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/tenant_profiles/queries.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/tenant_profiles/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/tenant_profiles/subscriptions.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/tenant_profiles/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/tenant_profiles/types.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/tenant_profiles/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/tenants/__init__.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/tenants/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/tenants/mutations.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/tenants/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/tenants/queries.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/tenants/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/tenants/subscriptions.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/tenants/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/tenants/types.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/tenants/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 class TenantEnvironment(str, Enum):
     """TenantEnvironment."""
 
     PILOT = "pilot"
     CHARLIE = "charlie"
     ECHO = "echo"
     DELTA = "delta"
+    FOXTROT = "foxtrot"
 
 
 class SSOEnvironment(str, Enum):
     """SSOEnvironment."""
 
     PILOT = "pilot"
     PRODUCTION = "production"
```

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/threat/__init__.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/threat/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/threat/mutations.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/threat/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/threat/queries.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/threat/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/threat/subscriptions.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/threat/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/threat/types.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/threat/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/trip/__init__.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/trip/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/trip/mutations.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/trip/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/trip/queries.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/trip/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/trip/subscriptions.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/trip/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/trip/types.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/trip/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/users/__init__.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/users/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/users/mutations.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/users/mutations.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,14 +189,27 @@
             },
             output=build_output_string(TDRUser),
         )
         if result.get(endpoint) is not None:
             return TDRUser.from_dict(result.get(endpoint))
         raise GraphQLNoRowsInResultSetError("for mutation updateTDRUserInfo")
 
+    def current_user_reset_mfa(self) -> MFAResetResponse:
+        """Reset MFA while logged in. This will read the access token from the authorization header to get the target user."""
+        endpoint = "currentUserResetMFA"
+
+        result = self.service.execute_mutation(
+            endpoint=endpoint,
+            variables={},
+            output=build_output_string(MFAResetResponse),
+        )
+        if result.get(endpoint) is not None:
+            return MFAResetResponse.from_dict(result.get(endpoint))
+        raise GraphQLNoRowsInResultSetError("for mutation currentUserResetMFA")
+
     def register_partner_user(
         self, registration_input: PartnerRegistrationInput
     ) -> TDRUser:
         """Creates a pre-verified Partner User. Requires active SSO connection for the user's email domain."""
         endpoint = "registerPartnerUser"
 
         result = self.service.execute_mutation(
```

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/users/queries.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/users/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/users/subscriptions.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/users/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/services/users/types.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/services/users/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/tokens.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/tokens.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python/utils.py` & `taegis-sdk-python-1.0.5/taegis_sdk_python/utils.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python.egg-info/PKG-INFO` & `taegis-sdk-python-1.0.5/taegis_sdk_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taegis-sdk-python
-Version: 1.0.4
+Version: 1.0.5
 Summary: Taegis Python SDK
 Home-page: https://github.com/secureworks/taegis-sdk-python
 Author: Secureworks
 Author-email: sdks@secureworks.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `taegis-sdk-python-1.0.4/taegis_sdk_python.egg-info/SOURCES.txt` & `taegis-sdk-python-1.0.5/taegis_sdk_python.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -116,14 +116,19 @@
 taegis_sdk_python/services/investigations2/subscriptions.py
 taegis_sdk_python/services/investigations2/types.py
 taegis_sdk_python/services/mitre_attack_info/__init__.py
 taegis_sdk_python/services/mitre_attack_info/mutations.py
 taegis_sdk_python/services/mitre_attack_info/queries.py
 taegis_sdk_python/services/mitre_attack_info/subscriptions.py
 taegis_sdk_python/services/mitre_attack_info/types.py
+taegis_sdk_python/services/multi_tenant_context/__init__.py
+taegis_sdk_python/services/multi_tenant_context/mutations.py
+taegis_sdk_python/services/multi_tenant_context/queries.py
+taegis_sdk_python/services/multi_tenant_context/subscriptions.py
+taegis_sdk_python/services/multi_tenant_context/types.py
 taegis_sdk_python/services/notebooks/__init__.py
 taegis_sdk_python/services/notebooks/mutations.py
 taegis_sdk_python/services/notebooks/queries.py
 taegis_sdk_python/services/notebooks/subscriptions.py
 taegis_sdk_python/services/notebooks/types.py
 taegis_sdk_python/services/notifications/__init__.py
 taegis_sdk_python/services/notifications/mutations.py
```

