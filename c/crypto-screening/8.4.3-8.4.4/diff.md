# Comparing `tmp/crypto-screening-8.4.3.tar.gz` & `tmp/crypto-screening-8.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-8.4.3.tar", last modified: Wed Aug  2 20:06:37 2023, max compression
+gzip compressed data, was "crypto-screening-8.4.4.tar", last modified: Fri Aug  4 14:46:50 2023, max compression
```

## Comparing `crypto-screening-8.4.3.tar` & `crypto-screening-8.4.4.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 20:06:37.458855 crypto-screening-8.4.3/
--rw-rw-rw-   0        0        0      196 2023-08-02 20:06:35.000000 crypto-screening-8.4.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2059 2023-08-02 20:06:37.458855 crypto-screening-8.4.3/PKG-INFO
--rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-8.4.3/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-8.4.3/build.py
-drwxrwxrwx   0        0        0        0 2023-08-02 20:06:37.222874 crypto-screening-8.4.3/crypto_screening/
-drwxrwxrwx   0        0        0        0 2023-08-02 20:06:37.259839 crypto-screening-8.4.3/crypto_screening/collect/
--rw-rw-rw-   0        0        0    16968 2023-08-02 06:37:38.000000 crypto-screening-8.4.3/crypto_screening/collect/assets.py
-drwxrwxrwx   0        0        0        0 2023-08-02 20:06:37.265839 crypto-screening-8.4.3/crypto_screening/collect/foundation/
--rw-rw-rw-   0        0        0     4943 2023-07-31 16:05:02.000000 crypto-screening-8.4.3/crypto_screening/collect/foundation/exchanges.py
-drwxrwxrwx   0        0        0        0 2023-08-02 20:06:37.296875 crypto-screening-8.4.3/crypto_screening/collect/market/
--rw-rw-rw-   0        0        0      288 2023-07-24 09:23:18.000000 crypto-screening-8.4.3/crypto_screening/collect/market/__init__.py
--rw-rw-rw-   0        0        0    19611 2023-07-24 09:29:05.000000 crypto-screening-8.4.3/crypto_screening/collect/market/ohlcv.py
--rw-rw-rw-   0        0        0    17318 2023-07-24 09:53:00.000000 crypto-screening-8.4.3/crypto_screening/collect/market/orderbook.py
--rw-rw-rw-   0        0        0    12521 2023-07-24 09:29:05.000000 crypto-screening-8.4.3/crypto_screening/collect/market/orders.py
-drwxrwxrwx   0        0        0        0 2023-08-02 20:06:37.323430 crypto-screening-8.4.3/crypto_screening/collect/market/state/
--rw-rw-rw-   0        0        0      136 2023-07-24 09:51:18.000000 crypto-screening-8.4.3/crypto_screening/collect/market/state/__init__.py
--rw-rw-rw-   0        0        0    24329 2023-07-30 10:08:09.000000 crypto-screening-8.4.3/crypto_screening/collect/market/state/assets.py
--rw-rw-rw-   0        0        0    15451 2023-07-30 10:04:40.000000 crypto-screening-8.4.3/crypto_screening/collect/market/state/base.py
--rw-rw-rw-   0        0        0    21291 2023-07-30 10:08:09.000000 crypto-screening-8.4.3/crypto_screening/collect/market/state/symbols.py
--rw-rw-rw-   0        0        0    15119 2023-07-31 16:05:02.000000 crypto-screening-8.4.3/crypto_screening/collect/market/trades.py
--rw-rw-rw-   0        0        0    21356 2023-07-31 05:18:32.000000 crypto-screening-8.4.3/crypto_screening/collect/screeners.py
--rw-rw-rw-   0        0        0    21677 2023-08-02 06:37:38.000000 crypto-screening-8.4.3/crypto_screening/collect/symbols.py
--rw-rw-rw-   0        0        0    15804 2023-07-30 10:04:16.000000 crypto-screening-8.4.3/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0     1055 2023-07-22 15:46:14.000000 crypto-screening-8.4.3/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0     5404 2023-07-29 10:34:48.000000 crypto-screening-8.4.3/crypto_screening/interval.py
-drwxrwxrwx   0        0        0        0 2023-08-02 20:06:37.385903 crypto-screening-8.4.3/crypto_screening/screeners/
--rw-rw-rw-   0        0        0      508 2023-07-24 09:41:28.000000 crypto-screening-8.4.3/crypto_screening/screeners/__init__.py
--rw-rw-rw-   0        0        0    24218 2023-07-31 04:58:29.000000 crypto-screening-8.4.3/crypto_screening/screeners/base.py
-drwxrwxrwx   0        0        0        0 2023-08-02 20:06:37.409925 crypto-screening-8.4.3/crypto_screening/screeners/callbacks/
--rw-rw-rw-   0        0        0      193 2023-07-24 09:32:57.000000 crypto-screening-8.4.3/crypto_screening/screeners/callbacks/__init__.py
--rw-rw-rw-   0        0        0     6494 2023-07-24 09:18:38.000000 crypto-screening-8.4.3/crypto_screening/screeners/callbacks/base.py
--rw-rw-rw-   0        0        0     4400 2023-07-30 10:12:51.000000 crypto-screening-8.4.3/crypto_screening/screeners/callbacks/database.py
--rw-rw-rw-   0        0        0     5605 2023-07-24 09:29:05.000000 crypto-screening-8.4.3/crypto_screening/screeners/callbacks/sockets.py
-drwxrwxrwx   0        0        0        0 2023-08-02 20:06:37.429888 crypto-screening-8.4.3/crypto_screening/screeners/collectors/
--rw-rw-rw-   0        0        0      196 2023-07-24 09:51:10.000000 crypto-screening-8.4.3/crypto_screening/screeners/collectors/__init__.py
--rw-rw-rw-   0        0        0     6253 2023-07-30 10:04:48.000000 crypto-screening-8.4.3/crypto_screening/screeners/collectors/base.py
--rw-rw-rw-   0        0        0     4190 2023-07-24 09:45:56.000000 crypto-screening-8.4.3/crypto_screening/screeners/collectors/database.py
--rw-rw-rw-   0        0        0     6143 2023-07-24 09:29:05.000000 crypto-screening-8.4.3/crypto_screening/screeners/collectors/sockets.py
--rw-rw-rw-   0        0        0    12263 2023-07-24 09:38:16.000000 crypto-screening-8.4.3/crypto_screening/screeners/combined.py
--rw-rw-rw-   0        0        0    10775 2023-07-24 09:29:30.000000 crypto-screening-8.4.3/crypto_screening/screeners/container.py
--rw-rw-rw-   0        0        0    11146 2023-07-31 16:05:02.000000 crypto-screening-8.4.3/crypto_screening/screeners/database.py
-drwxrwxrwx   0        0        0        0 2023-08-02 20:06:37.445856 crypto-screening-8.4.3/crypto_screening/screeners/foundation/
--rw-rw-rw-   0        0        0    11112 2023-08-02 19:51:16.000000 crypto-screening-8.4.3/crypto_screening/screeners/foundation/data.py
--rw-rw-rw-   0        0        0      840 2023-07-18 21:26:30.000000 crypto-screening-8.4.3/crypto_screening/screeners/foundation/protocols.py
--rw-rw-rw-   0        0        0     1203 2023-07-24 09:37:42.000000 crypto-screening-8.4.3/crypto_screening/screeners/foundation/state.py
--rw-rw-rw-   0        0        0     6966 2023-07-24 09:37:50.000000 crypto-screening-8.4.3/crypto_screening/screeners/foundation/waiting.py
--rw-rw-rw-   0        0        0    15098 2023-07-24 09:29:05.000000 crypto-screening-8.4.3/crypto_screening/screeners/market.py
--rw-rw-rw-   0        0        0    22149 2023-07-27 14:51:51.000000 crypto-screening-8.4.3/crypto_screening/screeners/ohlcv.py
--rw-rw-rw-   0        0        0    11836 2023-07-27 14:51:29.000000 crypto-screening-8.4.3/crypto_screening/screeners/orderbook.py
--rw-rw-rw-   0        0        0    11432 2023-07-27 14:51:23.000000 crypto-screening-8.4.3/crypto_screening/screeners/orders.py
--rw-rw-rw-   0        0        0    17092 2023-08-02 19:54:34.000000 crypto-screening-8.4.3/crypto_screening/screeners/recorder.py
--rw-rw-rw-   0        0        0    11501 2023-07-27 14:51:13.000000 crypto-screening-8.4.3/crypto_screening/screeners/trades.py
--rw-rw-rw-   0        0        0     3831 2023-07-24 09:40:07.000000 crypto-screening-8.4.3/crypto_screening/screeners/waiting.py
-drwxrwxrwx   0        0        0        0 2023-08-02 20:06:37.184429 crypto-screening-8.4.3/crypto_screening/source/
-drwxrwxrwx   0        0        0        0 2023-08-02 20:06:37.445856 crypto-screening-8.4.3/crypto_screening/source/data/
--rw-rw-rw-   0        0        0   284601 2023-07-21 09:53:03.000000 crypto-screening-8.4.3/crypto_screening/source/data/all_exchanges_symbols.json
--rw-rw-rw-   0        0        0    10527 2023-07-31 05:20:01.000000 crypto-screening-8.4.3/crypto_screening/symbols.py
-drwxrwxrwx   0        0        0        0 2023-08-02 20:06:37.457886 crypto-screening-8.4.3/crypto_screening/utils/
--rw-rw-rw-   0        0        0     1012 2023-07-22 15:52:54.000000 crypto-screening-8.4.3/crypto_screening/utils/base.py
--rw-rw-rw-   0        0        0     2765 2023-07-24 18:15:45.000000 crypto-screening-8.4.3/crypto_screening/utils/process.py
--rw-rw-rw-   0        0        0     3855 2023-08-02 06:33:48.000000 crypto-screening-8.4.3/crypto_screening/validate.py
-drwxrwxrwx   0        0        0        0 2023-08-02 20:06:37.239872 crypto-screening-8.4.3/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2059 2023-08-02 20:06:37.000000 crypto-screening-8.4.3/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2156 2023-08-02 20:06:37.000000 crypto-screening-8.4.3/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 20:06:37.000000 crypto-screening-8.4.3/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      113 2023-08-02 20:06:37.000000 crypto-screening-8.4.3/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-08-02 20:06:37.000000 crypto-screening-8.4.3/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-08-02 20:06:35.000000 crypto-screening-8.4.3/pyproject.toml
--rw-rw-rw-   0        0        0      120 2023-07-17 22:21:20.000000 crypto-screening-8.4.3/requirements-dev.txt
--rw-rw-rw-   0        0        0       77 2023-07-17 20:19:29.000000 crypto-screening-8.4.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-08-02 20:06:37.459856 crypto-screening-8.4.3/setup.cfg
--rw-rw-rw-   0        0        0     1649 2023-08-02 19:57:42.000000 crypto-screening-8.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 14:46:50.130484 crypto-screening-8.4.4/
+-rw-rw-rw-   0        0        0      196 2023-08-04 14:46:49.000000 crypto-screening-8.4.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     2059 2023-08-04 14:46:50.129486 crypto-screening-8.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-8.4.4/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-8.4.4/build.py
+drwxrwxrwx   0        0        0        0 2023-08-04 14:46:49.896766 crypto-screening-8.4.4/crypto_screening/
+drwxrwxrwx   0        0        0        0 2023-08-04 14:46:49.929309 crypto-screening-8.4.4/crypto_screening/collect/
+-rw-rw-rw-   0        0        0    16968 2023-08-02 06:37:38.000000 crypto-screening-8.4.4/crypto_screening/collect/assets.py
+drwxrwxrwx   0        0        0        0 2023-08-04 14:46:49.934306 crypto-screening-8.4.4/crypto_screening/collect/foundation/
+-rw-rw-rw-   0        0        0     4943 2023-07-31 16:05:02.000000 crypto-screening-8.4.4/crypto_screening/collect/foundation/exchanges.py
+drwxrwxrwx   0        0        0        0 2023-08-04 14:46:49.963801 crypto-screening-8.4.4/crypto_screening/collect/market/
+-rw-rw-rw-   0        0        0      288 2023-07-24 09:23:18.000000 crypto-screening-8.4.4/crypto_screening/collect/market/__init__.py
+-rw-rw-rw-   0        0        0    19611 2023-07-24 09:29:05.000000 crypto-screening-8.4.4/crypto_screening/collect/market/ohlcv.py
+-rw-rw-rw-   0        0        0    17318 2023-07-24 09:53:00.000000 crypto-screening-8.4.4/crypto_screening/collect/market/orderbook.py
+-rw-rw-rw-   0        0        0    12521 2023-07-24 09:29:05.000000 crypto-screening-8.4.4/crypto_screening/collect/market/orders.py
+drwxrwxrwx   0        0        0        0 2023-08-04 14:46:49.986249 crypto-screening-8.4.4/crypto_screening/collect/market/state/
+-rw-rw-rw-   0        0        0      136 2023-07-24 09:51:18.000000 crypto-screening-8.4.4/crypto_screening/collect/market/state/__init__.py
+-rw-rw-rw-   0        0        0    24329 2023-07-30 10:08:09.000000 crypto-screening-8.4.4/crypto_screening/collect/market/state/assets.py
+-rw-rw-rw-   0        0        0    15451 2023-07-30 10:04:40.000000 crypto-screening-8.4.4/crypto_screening/collect/market/state/base.py
+-rw-rw-rw-   0        0        0    21291 2023-07-30 10:08:09.000000 crypto-screening-8.4.4/crypto_screening/collect/market/state/symbols.py
+-rw-rw-rw-   0        0        0    15119 2023-07-31 16:05:02.000000 crypto-screening-8.4.4/crypto_screening/collect/market/trades.py
+-rw-rw-rw-   0        0        0    21356 2023-07-31 05:18:32.000000 crypto-screening-8.4.4/crypto_screening/collect/screeners.py
+-rw-rw-rw-   0        0        0    21677 2023-08-02 06:37:38.000000 crypto-screening-8.4.4/crypto_screening/collect/symbols.py
+-rw-rw-rw-   0        0        0    15804 2023-07-30 10:04:16.000000 crypto-screening-8.4.4/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0     1055 2023-07-22 15:46:14.000000 crypto-screening-8.4.4/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0     5404 2023-07-29 10:34:48.000000 crypto-screening-8.4.4/crypto_screening/interval.py
+drwxrwxrwx   0        0        0        0 2023-08-04 14:46:50.052839 crypto-screening-8.4.4/crypto_screening/screeners/
+-rw-rw-rw-   0        0        0      508 2023-07-24 09:41:28.000000 crypto-screening-8.4.4/crypto_screening/screeners/__init__.py
+-rw-rw-rw-   0        0        0    24218 2023-07-31 04:58:29.000000 crypto-screening-8.4.4/crypto_screening/screeners/base.py
+drwxrwxrwx   0        0        0        0 2023-08-04 14:46:50.075977 crypto-screening-8.4.4/crypto_screening/screeners/callbacks/
+-rw-rw-rw-   0        0        0      193 2023-07-24 09:32:57.000000 crypto-screening-8.4.4/crypto_screening/screeners/callbacks/__init__.py
+-rw-rw-rw-   0        0        0     6494 2023-07-24 09:18:38.000000 crypto-screening-8.4.4/crypto_screening/screeners/callbacks/base.py
+-rw-rw-rw-   0        0        0     4400 2023-07-30 10:12:51.000000 crypto-screening-8.4.4/crypto_screening/screeners/callbacks/database.py
+-rw-rw-rw-   0        0        0     5605 2023-07-24 09:29:05.000000 crypto-screening-8.4.4/crypto_screening/screeners/callbacks/sockets.py
+drwxrwxrwx   0        0        0        0 2023-08-04 14:46:50.098497 crypto-screening-8.4.4/crypto_screening/screeners/collectors/
+-rw-rw-rw-   0        0        0      196 2023-07-24 09:51:10.000000 crypto-screening-8.4.4/crypto_screening/screeners/collectors/__init__.py
+-rw-rw-rw-   0        0        0     6253 2023-07-30 10:04:48.000000 crypto-screening-8.4.4/crypto_screening/screeners/collectors/base.py
+-rw-rw-rw-   0        0        0     4190 2023-07-24 09:45:56.000000 crypto-screening-8.4.4/crypto_screening/screeners/collectors/database.py
+-rw-rw-rw-   0        0        0     6143 2023-07-24 09:29:05.000000 crypto-screening-8.4.4/crypto_screening/screeners/collectors/sockets.py
+-rw-rw-rw-   0        0        0    12296 2023-08-04 14:46:12.000000 crypto-screening-8.4.4/crypto_screening/screeners/combined.py
+-rw-rw-rw-   0        0        0    10775 2023-07-24 09:29:30.000000 crypto-screening-8.4.4/crypto_screening/screeners/container.py
+-rw-rw-rw-   0        0        0    11146 2023-07-31 16:05:02.000000 crypto-screening-8.4.4/crypto_screening/screeners/database.py
+drwxrwxrwx   0        0        0        0 2023-08-04 14:46:50.115458 crypto-screening-8.4.4/crypto_screening/screeners/foundation/
+-rw-rw-rw-   0        0        0    11778 2023-08-04 14:21:19.000000 crypto-screening-8.4.4/crypto_screening/screeners/foundation/data.py
+-rw-rw-rw-   0        0        0      840 2023-07-18 21:26:30.000000 crypto-screening-8.4.4/crypto_screening/screeners/foundation/protocols.py
+-rw-rw-rw-   0        0        0     1203 2023-07-24 09:37:42.000000 crypto-screening-8.4.4/crypto_screening/screeners/foundation/state.py
+-rw-rw-rw-   0        0        0     6966 2023-07-24 09:37:50.000000 crypto-screening-8.4.4/crypto_screening/screeners/foundation/waiting.py
+-rw-rw-rw-   0        0        0    15098 2023-07-24 09:29:05.000000 crypto-screening-8.4.4/crypto_screening/screeners/market.py
+-rw-rw-rw-   0        0        0    22149 2023-07-27 14:51:51.000000 crypto-screening-8.4.4/crypto_screening/screeners/ohlcv.py
+-rw-rw-rw-   0        0        0    11836 2023-07-27 14:51:29.000000 crypto-screening-8.4.4/crypto_screening/screeners/orderbook.py
+-rw-rw-rw-   0        0        0    11432 2023-07-27 14:51:23.000000 crypto-screening-8.4.4/crypto_screening/screeners/orders.py
+-rw-rw-rw-   0        0        0    17092 2023-08-02 19:54:34.000000 crypto-screening-8.4.4/crypto_screening/screeners/recorder.py
+-rw-rw-rw-   0        0        0    11501 2023-07-27 14:51:13.000000 crypto-screening-8.4.4/crypto_screening/screeners/trades.py
+-rw-rw-rw-   0        0        0     3831 2023-07-24 09:40:07.000000 crypto-screening-8.4.4/crypto_screening/screeners/waiting.py
+drwxrwxrwx   0        0        0        0 2023-08-04 14:46:49.862395 crypto-screening-8.4.4/crypto_screening/source/
+drwxrwxrwx   0        0        0        0 2023-08-04 14:46:50.116431 crypto-screening-8.4.4/crypto_screening/source/data/
+-rw-rw-rw-   0        0        0   284601 2023-07-21 09:53:03.000000 crypto-screening-8.4.4/crypto_screening/source/data/all_exchanges_symbols.json
+-rw-rw-rw-   0        0        0    10527 2023-07-31 05:20:01.000000 crypto-screening-8.4.4/crypto_screening/symbols.py
+drwxrwxrwx   0        0        0        0 2023-08-04 14:46:50.128486 crypto-screening-8.4.4/crypto_screening/utils/
+-rw-rw-rw-   0        0        0     1012 2023-07-22 15:52:54.000000 crypto-screening-8.4.4/crypto_screening/utils/base.py
+-rw-rw-rw-   0        0        0     2765 2023-07-24 18:15:45.000000 crypto-screening-8.4.4/crypto_screening/utils/process.py
+-rw-rw-rw-   0        0        0     3855 2023-08-02 06:33:48.000000 crypto-screening-8.4.4/crypto_screening/validate.py
+drwxrwxrwx   0        0        0        0 2023-08-04 14:46:49.910791 crypto-screening-8.4.4/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2059 2023-08-04 14:46:49.000000 crypto-screening-8.4.4/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2156 2023-08-04 14:46:49.000000 crypto-screening-8.4.4/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 14:46:49.000000 crypto-screening-8.4.4/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      113 2023-08-04 14:46:49.000000 crypto-screening-8.4.4/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-08-04 14:46:49.000000 crypto-screening-8.4.4/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-08-04 14:46:49.000000 crypto-screening-8.4.4/pyproject.toml
+-rw-rw-rw-   0        0        0      120 2023-07-17 22:21:20.000000 crypto-screening-8.4.4/requirements-dev.txt
+-rw-rw-rw-   0        0        0       77 2023-07-17 20:19:29.000000 crypto-screening-8.4.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-08-04 14:46:50.130484 crypto-screening-8.4.4/setup.cfg
+-rw-rw-rw-   0        0        0     1649 2023-08-04 14:46:39.000000 crypto-screening-8.4.4/setup.py
```

### Comparing `crypto-screening-8.4.3/PKG-INFO` & `crypto-screening-8.4.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 8.4.3
+Version: 8.4.4
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-8.4.3/README.md` & `crypto-screening-8.4.4/README.md`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.3/build.py` & `crypto-screening-8.4.4/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.3/crypto_screening/collect/assets.py` & `crypto-screening-8.4.4/crypto_screening/collect/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.3/crypto_screening/collect/foundation/exchanges.py` & `crypto-screening-8.4.4/crypto_screening/collect/foundation/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.3/crypto_screening/collect/market/ohlcv.py` & `crypto-screening-8.4.4/crypto_screening/collect/market/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.3/crypto_screening/collect/market/orderbook.py` & `crypto-screening-8.4.4/crypto_screening/collect/market/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.3/crypto_screening/collect/market/orders.py` & `crypto-screening-8.4.4/crypto_screening/collect/market/orders.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.3/crypto_screening/collect/market/state/assets.py` & `crypto-screening-8.4.4/crypto_screening/collect/market/state/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.3/crypto_screening/collect/market/state/base.py` & `crypto-screening-8.4.4/crypto_screening/collect/market/state/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.3/crypto_screening/collect/market/state/symbols.py` & `crypto-screening-8.4.4/crypto_screening/collect/market/state/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.3/crypto_screening/collect/market/trades.py` & `crypto-screening-8.4.4/crypto_screening/collect/market/trades.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.3/crypto_screening/collect/screeners.py` & `crypto-screening-8.4.4/crypto_screening/collect/screeners.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.3/crypto_screening/collect/symbols.py` & `crypto-screening-8.4.4/crypto_screening/collect/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.3/crypto_screening/dataset.py` & `crypto-screening-8.4.4/crypto_screening/dataset.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.3/crypto_screening/exchanges.py` & `crypto-screening-8.4.4/crypto_screening/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.3/crypto_screening/interval.py` & `crypto-screening-8.4.4/crypto_screening/interval.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.3/crypto_screening/screeners/base.py` & `crypto-screening-8.4.4/crypto_screening/screeners/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.3/crypto_screening/screeners/callbacks/base.py` & `crypto-screening-8.4.4/crypto_screening/screeners/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.3/crypto_screening/screeners/callbacks/database.py` & `crypto-screening-8.4.4/crypto_screening/screeners/callbacks/database.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.3/crypto_screening/screeners/callbacks/sockets.py` & `crypto-screening-8.4.4/crypto_screening/screeners/callbacks/sockets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.3/crypto_screening/screeners/collectors/base.py` & `crypto-screening-8.4.4/crypto_screening/screeners/collectors/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.3/crypto_screening/screeners/collectors/database.py` & `crypto-screening-8.4.4/crypto_screening/screeners/collectors/database.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.3/crypto_screening/screeners/collectors/sockets.py` & `crypto-screening-8.4.4/crypto_screening/screeners/collectors/sockets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.3/crypto_screening/screeners/combined.py` & `crypto-screening-8.4.4/crypto_screening/screeners/combined.py`

 * *Files 1% similar despite different names*

```diff
@@ -324,15 +324,15 @@
     OrderbookCategory: orderbook_market_screener,
     OHLCVCategory: ohlcv_market_screener,
     TradesCategory: trades_market_screener,
     OrdersCategory: orders_market_screener
 }
 
 def combined_market_screener(
-        data: Dict[str, Iterable[str]],
+        data: Dict[str, Iterable[Union[str, Dict[str, Iterable[str]]]]],
         categories: Optional[Type[CategoryBase]] = None,
         location: Optional[str] = None,
         cancel: Optional[Union[float, dt.timedelta]] = None,
         delay: Optional[Union[float, dt.timedelta]] = None,
         limited: Optional[bool] = None,
         handler: Optional[MarketHandler] = None,
         amount: Optional[int] = None,
```

### Comparing `crypto-screening-8.4.3/crypto_screening/screeners/container.py` & `crypto-screening-8.4.4/crypto_screening/screeners/container.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.3/crypto_screening/screeners/database.py` & `crypto-screening-8.4.4/crypto_screening/screeners/database.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.3/crypto_screening/screeners/foundation/data.py` & `crypto-screening-8.4.4/crypto_screening/screeners/foundation/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,49 @@
 # data.py
 
 import warnings
 import datetime as dt
 import time
 from abc import ABCMeta, abstractmethod
 import threading
+from itertools import chain
 from typing import Optional, Union, Dict, Any
 
 from represent import represent
 
 
 from crypto_screening.screeners.foundation.state import WaitingState
 
 __all__ = [
     "DataCollector"
 ]
 
+def extract_attributes(data: Any, /) -> Dict[str, Any]:
+    """
+    Gets all attributes of an object.
+
+    :param data: The object.
+
+    :return: The attributes of the object.
+    """
+
+    return {
+        **(data.__dict__ if hasattr(data, '__dict__') else {}),
+        **(
+            {
+                key: getattr(data, key)
+                for key in chain.from_iterable(
+                    getattr(cls, '__slots__', [])
+                    for cls in type(data).__mro__
+                ) if hasattr(data, key)
+            } if hasattr(data, '__slots__') else {}
+        )
+    }
+# end extract_attributes
+
 @represent
 class DataCollector(metaclass=ABCMeta):
     """A class to represent an abstract parent class of data collectors."""
 
     LOCATION = "datasets"
 
     DELAY = 0
@@ -72,15 +96,15 @@
     def __getstate__(self) -> Dict[str, Any]:
         """
         Returns the data of the object.
 
         :return: The state of the object.
         """
 
-        data = self.__dict__.copy()
+        data = extract_attributes(self)
 
         for key, value in data.items():
             if isinstance(value, threading.Thread):
                 data[key] = None
             # end if
         # end for
```

### Comparing `crypto-screening-8.4.3/crypto_screening/screeners/foundation/protocols.py` & `crypto-screening-8.4.4/crypto_screening/screeners/foundation/protocols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.3/crypto_screening/screeners/foundation/state.py` & `crypto-screening-8.4.4/crypto_screening/screeners/foundation/state.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.3/crypto_screening/screeners/foundation/waiting.py` & `crypto-screening-8.4.4/crypto_screening/screeners/foundation/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.3/crypto_screening/screeners/market.py` & `crypto-screening-8.4.4/crypto_screening/screeners/market.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.3/crypto_screening/screeners/ohlcv.py` & `crypto-screening-8.4.4/crypto_screening/screeners/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.3/crypto_screening/screeners/orderbook.py` & `crypto-screening-8.4.4/crypto_screening/screeners/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.3/crypto_screening/screeners/orders.py` & `crypto-screening-8.4.4/crypto_screening/screeners/orders.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.3/crypto_screening/screeners/recorder.py` & `crypto-screening-8.4.4/crypto_screening/screeners/recorder.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.3/crypto_screening/screeners/trades.py` & `crypto-screening-8.4.4/crypto_screening/screeners/trades.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.3/crypto_screening/screeners/waiting.py` & `crypto-screening-8.4.4/crypto_screening/screeners/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.3/crypto_screening/source/data/all_exchanges_symbols.json` & `crypto-screening-8.4.4/crypto_screening/source/data/all_exchanges_symbols.json`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.3/crypto_screening/symbols.py` & `crypto-screening-8.4.4/crypto_screening/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.3/crypto_screening/utils/base.py` & `crypto-screening-8.4.4/crypto_screening/utils/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.3/crypto_screening/utils/process.py` & `crypto-screening-8.4.4/crypto_screening/utils/process.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.3/crypto_screening/validate.py` & `crypto-screening-8.4.4/crypto_screening/validate.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.3/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-8.4.4/crypto_screening.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 8.4.3
+Version: 8.4.4
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-8.4.3/crypto_screening.egg-info/SOURCES.txt` & `crypto-screening-8.4.4/crypto_screening.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.3/pyproject.toml` & `crypto-screening-8.4.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'crypto-screening'
-version = '8.4.3'
+version = '8.4.4'
 description = 'A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `crypto-screening-8.4.3/setup.py` & `crypto-screening-8.4.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         ],
         include=[
             "crypto_screening/source"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='crypto-screening',
-        version='8.4.3',
+        version='8.4.4',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

