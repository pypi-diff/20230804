# Comparing `tmp/sharetop-2.4.6.tar.gz` & `tmp/sharetop-2.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sharetop-2.4.6.tar", last modified: Mon Jul 31 15:09:29 2023, max compression
+gzip compressed data, was "sharetop-2.4.7.tar", last modified: Thu Aug  3 22:44:24 2023, max compression
```

## Comparing `sharetop-2.4.6.tar` & `sharetop-2.4.7.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 15:09:29.820037 sharetop-2.4.6/
--rw-rw-rw-   0        0        0     1066 2023-04-26 14:07:21.000000 sharetop-2.4.6/LICENSE
--rw-rw-rw-   0        0        0    51253 2023-07-31 15:09:29.817675 sharetop-2.4.6/PKG-INFO
--rw-rw-rw-   0        0        0    49774 2023-07-15 03:35:16.000000 sharetop-2.4.6/README.md
--rw-rw-rw-   0        0        0       42 2023-07-31 15:09:29.820037 sharetop-2.4.6/setup.cfg
--rw-rw-rw-   0        0        0     1219 2023-04-29 06:50:50.000000 sharetop-2.4.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-31 15:09:28.982454 sharetop-2.4.6/sharetop/
--rw-rw-rw-   0        0        0      297 2023-05-18 12:23:41.000000 sharetop-2.4.6/sharetop/__init__.py
--rw-rw-rw-   0        0        0      386 2023-07-31 15:08:44.000000 sharetop-2.4.6/sharetop/__version__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 15:09:29.044535 sharetop-2.4.6/sharetop/api/
--rw-rw-rw-   0        0        0      306 2023-07-02 13:11:41.000000 sharetop-2.4.6/sharetop/api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 15:09:29.064129 sharetop-2.4.6/sharetop/application/
--rw-rw-rw-   0        0        0       33 2023-04-21 11:53:52.000000 sharetop-2.4.6/sharetop/application/__init__.py
--rw-rw-rw-   0        0        0     4459 2023-07-16 22:42:50.000000 sharetop-2.4.6/sharetop/application/base.py
-drwxrwxrwx   0        0        0        0 2023-07-31 15:09:29.095302 sharetop-2.4.6/sharetop/core/
--rw-rw-rw-   0        0        0        0 2023-04-08 05:23:09.000000 sharetop-2.4.6/sharetop/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 15:09:29.174110 sharetop-2.4.6/sharetop/core/bond/
--rw-rw-rw-   0        0        0      592 2023-07-15 11:00:24.000000 sharetop-2.4.6/sharetop/core/bond/__init__.py
--rw-rw-rw-   0        0        0     1869 2023-04-24 04:28:03.000000 sharetop-2.4.6/sharetop/core/bond/config.py
--rw-rw-rw-   0        0        0     9571 2023-07-16 01:28:38.000000 sharetop-2.4.6/sharetop/core/bond/get_bond_info.py
--rw-rw-rw-   0        0        0    19614 2023-07-15 10:59:53.000000 sharetop-2.4.6/sharetop/core/bond/get_bond_public_info.py
--rw-rw-rw-   0        0        0      598 2023-04-10 05:06:06.000000 sharetop-2.4.6/sharetop/core/cache.py
-drwxrwxrwx   0        0        0        0 2023-07-31 15:09:29.198343 sharetop-2.4.6/sharetop/core/capital_flow/
--rw-rw-rw-   0        0        0      367 2023-07-15 15:19:38.000000 sharetop-2.4.6/sharetop/core/capital_flow/__init__.py
--rw-rw-rw-   0        0        0     6785 2023-07-25 15:02:39.000000 sharetop-2.4.6/sharetop/core/capital_flow/capital_flow_monitor.py
-drwxrwxrwx   0        0        0        0 2023-07-31 15:09:29.262406 sharetop-2.4.6/sharetop/core/common/
--rw-rw-rw-   0        0        0      188 2023-04-27 15:24:55.000000 sharetop-2.4.6/sharetop/core/common/__init__.py
--rw-rw-rw-   0        0        0     3727 2023-07-19 03:47:04.000000 sharetop-2.4.6/sharetop/core/common/common_base.py
--rw-rw-rw-   0        0        0     8688 2023-05-25 01:16:42.000000 sharetop-2.4.6/sharetop/core/common/config.py
--rw-rw-rw-   0        0        0    15132 2023-07-31 15:05:35.000000 sharetop-2.4.6/sharetop/core/common/explain_change.py
--rw-rw-rw-   0        0        0    12428 2023-07-16 01:53:16.000000 sharetop-2.4.6/sharetop/core/common/getter.py
--rw-rw-rw-   0        0        0      750 2023-04-09 05:42:43.000000 sharetop-2.4.6/sharetop/core/config.py
-drwxrwxrwx   0        0        0        0 2023-07-31 15:09:29.301096 sharetop-2.4.6/sharetop/core/country/
--rw-rw-rw-   0        0        0       91 2023-07-16 02:39:07.000000 sharetop-2.4.6/sharetop/core/country/__init__.py
--rw-rw-rw-   0        0        0      491 2023-05-09 01:30:20.000000 sharetop-2.4.6/sharetop/core/country/config.py
--rw-rw-rw-   0        0        0      697 2023-07-16 02:39:07.000000 sharetop-2.4.6/sharetop/core/country/country_base_info.py
-drwxrwxrwx   0        0        0        0 2023-07-31 15:09:29.406708 sharetop-2.4.6/sharetop/core/fund/
--rw-rw-rw-   0        0        0     1025 2023-07-31 14:59:03.000000 sharetop-2.4.6/sharetop/core/fund/__init__.py
--rw-rw-rw-   0        0        0      927 2023-07-28 01:21:27.000000 sharetop-2.4.6/sharetop/core/fund/config.py
--rw-rw-rw-   0        0        0     2727 2023-07-28 00:06:51.000000 sharetop-2.4.6/sharetop/core/fund/fund_list.py
--rw-rw-rw-   0        0        0     1857 2023-07-31 14:52:45.000000 sharetop-2.4.6/sharetop/core/fund/get_fund_base_info.py
--rw-rw-rw-   0        0        0     2624 2023-07-31 15:04:18.000000 sharetop-2.4.6/sharetop/core/fund/get_fund_history_data.py
--rw-rw-rw-   0        0        0     3716 2023-07-15 10:12:05.000000 sharetop-2.4.6/sharetop/core/fund/get_fund_industry_info.py
--rw-rw-rw-   0        0        0     5474 2023-07-15 10:19:50.000000 sharetop-2.4.6/sharetop/core/fund/get_fund_invest_info.py
--rw-rw-rw-   0        0        0    12432 2023-07-31 14:59:03.000000 sharetop-2.4.6/sharetop/core/fund/get_fund_rank.py
--rw-rw-rw-   0        0        0     1466 2023-04-22 03:27:53.000000 sharetop-2.4.6/sharetop/core/fund/get_fund_real_time.py
--rw-rw-rw-   0        0        0     2497 2023-07-15 10:37:11.000000 sharetop-2.4.6/sharetop/core/fund/get_period_change_info.py
--rw-rw-rw-   0        0        0     2451 2023-07-15 10:39:55.000000 sharetop-2.4.6/sharetop/core/fund/get_types_percentage_info.py
-drwxrwxrwx   0        0        0        0 2023-07-31 15:09:29.437035 sharetop-2.4.6/sharetop/core/futures/
--rw-rw-rw-   0        0        0      250 2023-07-16 02:07:46.000000 sharetop-2.4.6/sharetop/core/futures/__init__.py
--rw-rw-rw-   0        0        0    10057 2023-07-16 02:09:22.000000 sharetop-2.4.6/sharetop/core/futures/get_futures_info.py
-drwxrwxrwx   0        0        0        0 2023-07-31 15:09:29.472373 sharetop-2.4.6/sharetop/core/oil/
--rw-rw-rw-   0        0        0      402 2023-05-16 01:17:51.000000 sharetop-2.4.6/sharetop/core/oil/__init__.py
--rw-rw-rw-   0        0        0     1685 2023-05-15 00:28:25.000000 sharetop-2.4.6/sharetop/core/oil/config.py
--rw-rw-rw-   0        0        0     3614 2023-07-10 00:25:56.000000 sharetop-2.4.6/sharetop/core/oil/oil_detail.py
-drwxrwxrwx   0        0        0        0 2023-07-31 15:09:29.505159 sharetop-2.4.6/sharetop/core/pig/
--rw-rw-rw-   0        0        0       84 2023-07-15 10:46:51.000000 sharetop-2.4.6/sharetop/core/pig/__init__.py
--rw-rw-rw-   0        0        0      163 2023-05-16 00:42:46.000000 sharetop-2.4.6/sharetop/core/pig/config.py
--rw-rw-rw-   0        0        0     1428 2023-07-15 10:46:51.000000 sharetop-2.4.6/sharetop/core/pig/pig_detail.py
-drwxrwxrwx   0        0        0        0 2023-07-31 15:09:29.581350 sharetop-2.4.6/sharetop/core/stock/
--rw-rw-rw-   0        0        0      662 2023-07-15 09:27:19.000000 sharetop-2.4.6/sharetop/core/stock/__init__.py
--rw-rw-rw-   0        0        0     4834 2023-07-20 01:18:36.000000 sharetop-2.4.6/sharetop/core/stock/bill_monitor.py
--rw-rw-rw-   0        0        0     1163 2023-07-19 01:27:46.000000 sharetop-2.4.6/sharetop/core/stock/config.py
--rw-rw-rw-   0        0        0    15110 2023-07-20 01:10:32.000000 sharetop-2.4.6/sharetop/core/stock/getter.py
--rw-rw-rw-   0        0        0    10620 2023-07-19 01:27:46.000000 sharetop-2.4.6/sharetop/core/stock/quarterly_report.py
--rw-rw-rw-   0        0        0    10240 2023-07-27 23:27:15.000000 sharetop-2.4.6/sharetop/core/stock/rank_list.py
--rw-rw-rw-   0        0        0      693 2023-07-19 12:30:45.000000 sharetop-2.4.6/sharetop/core/stock/stock_base_info.py
--rw-rw-rw-   0        0        0     7299 2023-07-19 04:12:02.000000 sharetop-2.4.6/sharetop/core/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-31 15:09:29.614196 sharetop-2.4.6/sharetop/crawl/
--rw-rw-rw-   0        0        0       29 2023-04-09 23:19:21.000000 sharetop-2.4.6/sharetop/crawl/__init__.py
--rw-rw-rw-   0        0        0     1088 2023-07-19 05:03:18.000000 sharetop-2.4.6/sharetop/crawl/base.py
--rw-rw-rw-   0        0        0     3271 2023-07-09 23:57:40.000000 sharetop-2.4.6/sharetop/crawl/settings.py
-drwxrwxrwx   0        0        0        0 2023-07-31 15:09:29.648774 sharetop-2.4.6/sharetop/parser/
--rw-rw-rw-   0        0        0       27 2023-04-10 00:54:05.000000 sharetop-2.4.6/sharetop/parser/__init__.py
--rw-rw-rw-   0        0        0     4364 2023-07-19 04:59:24.000000 sharetop-2.4.6/sharetop/parser/base.py
--rw-rw-rw-   0        0        0     2911 2023-07-19 05:36:09.000000 sharetop-2.4.6/sharetop/parser/config.py
-drwxrwxrwx   0        0        0        0 2023-07-31 15:09:29.817107 sharetop-2.4.6/sharetop/test/
--rw-rw-rw-   0        0        0        0 2023-04-29 10:57:35.000000 sharetop-2.4.6/sharetop/test/__init__.py
--rw-rw-rw-   0        0        0      432 2023-07-16 01:29:33.000000 sharetop-2.4.6/sharetop/test/bond_test.py
--rw-rw-rw-   0        0        0      199 2023-05-17 04:49:54.000000 sharetop-2.4.6/sharetop/test/captial.py
--rw-rw-rw-   0        0        0      172 2023-07-16 02:38:09.000000 sharetop-2.4.6/sharetop/test/country_test.py
--rw-rw-rw-   0        0        0      582 2023-07-25 15:03:47.000000 sharetop-2.4.6/sharetop/test/flow_monitor_test.py
--rw-rw-rw-   0        0        0     1558 2023-07-31 15:01:19.000000 sharetop-2.4.6/sharetop/test/fund_test.py
--rw-rw-rw-   0        0        0      382 2023-07-16 02:09:22.000000 sharetop-2.4.6/sharetop/test/futures_test.py
--rw-rw-rw-   0        0        0      504 2023-07-10 00:25:56.000000 sharetop-2.4.6/sharetop/test/oil_test.py
--rw-rw-rw-   0        0        0      198 2023-07-15 10:47:58.000000 sharetop-2.4.6/sharetop/test/pig_test.py
--rw-rw-rw-   0        0        0     1205 2023-07-27 23:28:24.000000 sharetop-2.4.6/sharetop/test/stock_test.py
--rw-rw-rw-   0        0        0      992 2023-07-17 01:23:58.000000 sharetop-2.4.6/sharetop/test/test1.py
--rw-rw-rw-   0        0        0     1997 2023-05-02 03:48:40.000000 sharetop-2.4.6/sharetop/test/test2-akshare.py
--rw-rw-rw-   0        0        0     3709 2023-05-03 07:10:48.000000 sharetop-2.4.6/sharetop/test/test3.py
--rw-rw-rw-   0        0        0      221 2023-07-30 10:45:50.000000 sharetop-2.4.6/sharetop/test/test4.py
--rw-rw-rw-   0        0        0      690 2023-07-15 03:35:15.000000 sharetop-2.4.6/sharetop/test/test5.py
--rw-rw-rw-   0        0        0     1227 2023-07-15 03:35:15.000000 sharetop-2.4.6/sharetop/test/test6.py
--rw-rw-rw-   0        0        0      643 2023-07-05 12:16:23.000000 sharetop-2.4.6/sharetop/test/test7.py
-drwxrwxrwx   0        0        0        0 2023-07-31 15:09:29.032958 sharetop-2.4.6/sharetop.egg-info/
--rw-rw-rw-   0        0        0    51253 2023-07-31 15:09:28.000000 sharetop-2.4.6/sharetop.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2456 2023-07-31 15:09:28.000000 sharetop-2.4.6/sharetop.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 15:09:28.000000 sharetop-2.4.6/sharetop.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-07-31 15:09:28.000000 sharetop-2.4.6/sharetop.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-31 15:09:28.000000 sharetop-2.4.6/sharetop.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-03 22:44:24.452738 sharetop-2.4.7/
+-rw-rw-rw-   0        0        0     1066 2023-04-26 14:07:21.000000 sharetop-2.4.7/LICENSE
+-rw-rw-rw-   0        0        0    51253 2023-08-03 22:44:24.452340 sharetop-2.4.7/PKG-INFO
+-rw-rw-rw-   0        0        0    49774 2023-07-15 03:35:16.000000 sharetop-2.4.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-03 22:44:24.453401 sharetop-2.4.7/setup.cfg
+-rw-rw-rw-   0        0        0     1219 2023-04-29 06:50:50.000000 sharetop-2.4.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 22:44:23.854664 sharetop-2.4.7/sharetop/
+-rw-rw-rw-   0        0        0      297 2023-05-18 12:23:41.000000 sharetop-2.4.7/sharetop/__init__.py
+-rw-rw-rw-   0        0        0      386 2023-08-03 22:44:14.000000 sharetop-2.4.7/sharetop/__version__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 22:44:23.879446 sharetop-2.4.7/sharetop/api/
+-rw-rw-rw-   0        0        0      306 2023-07-02 13:11:41.000000 sharetop-2.4.7/sharetop/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 22:44:23.894585 sharetop-2.4.7/sharetop/application/
+-rw-rw-rw-   0        0        0       33 2023-04-21 11:53:52.000000 sharetop-2.4.7/sharetop/application/__init__.py
+-rw-rw-rw-   0        0        0     4461 2023-08-03 04:20:19.000000 sharetop-2.4.7/sharetop/application/base.py
+drwxrwxrwx   0        0        0        0 2023-08-03 22:44:23.916442 sharetop-2.4.7/sharetop/core/
+-rw-rw-rw-   0        0        0        0 2023-04-08 05:23:09.000000 sharetop-2.4.7/sharetop/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 22:44:23.965155 sharetop-2.4.7/sharetop/core/bond/
+-rw-rw-rw-   0        0        0      592 2023-07-15 11:00:24.000000 sharetop-2.4.7/sharetop/core/bond/__init__.py
+-rw-rw-rw-   0        0        0     1869 2023-04-24 04:28:03.000000 sharetop-2.4.7/sharetop/core/bond/config.py
+-rw-rw-rw-   0        0        0     9767 2023-08-01 15:18:53.000000 sharetop-2.4.7/sharetop/core/bond/get_bond_info.py
+-rw-rw-rw-   0        0        0    19614 2023-07-15 10:59:53.000000 sharetop-2.4.7/sharetop/core/bond/get_bond_public_info.py
+-rw-rw-rw-   0        0        0      598 2023-04-10 05:06:06.000000 sharetop-2.4.7/sharetop/core/cache.py
+drwxrwxrwx   0        0        0        0 2023-08-03 22:44:23.974500 sharetop-2.4.7/sharetop/core/capital_flow/
+-rw-rw-rw-   0        0        0      367 2023-07-15 15:19:38.000000 sharetop-2.4.7/sharetop/core/capital_flow/__init__.py
+-rw-rw-rw-   0        0        0     6785 2023-07-25 15:02:39.000000 sharetop-2.4.7/sharetop/core/capital_flow/capital_flow_monitor.py
+drwxrwxrwx   0        0        0        0 2023-08-03 22:44:24.029343 sharetop-2.4.7/sharetop/core/common/
+-rw-rw-rw-   0        0        0      188 2023-04-27 15:24:55.000000 sharetop-2.4.7/sharetop/core/common/__init__.py
+-rw-rw-rw-   0        0        0     3727 2023-07-19 03:47:04.000000 sharetop-2.4.7/sharetop/core/common/common_base.py
+-rw-rw-rw-   0        0        0     8688 2023-05-25 01:16:42.000000 sharetop-2.4.7/sharetop/core/common/config.py
+-rw-rw-rw-   0        0        0    22277 2023-08-03 04:22:52.000000 sharetop-2.4.7/sharetop/core/common/explain_change.py
+-rw-rw-rw-   0        0        0    12428 2023-07-16 01:53:16.000000 sharetop-2.4.7/sharetop/core/common/getter.py
+-rw-rw-rw-   0        0        0      750 2023-04-09 05:42:43.000000 sharetop-2.4.7/sharetop/core/config.py
+drwxrwxrwx   0        0        0        0 2023-08-03 22:44:24.059374 sharetop-2.4.7/sharetop/core/country/
+-rw-rw-rw-   0        0        0       91 2023-07-16 02:39:07.000000 sharetop-2.4.7/sharetop/core/country/__init__.py
+-rw-rw-rw-   0        0        0      491 2023-05-09 01:30:20.000000 sharetop-2.4.7/sharetop/core/country/config.py
+-rw-rw-rw-   0        0        0      807 2023-08-01 23:11:54.000000 sharetop-2.4.7/sharetop/core/country/country_base_info.py
+drwxrwxrwx   0        0        0        0 2023-08-03 22:44:24.164224 sharetop-2.4.7/sharetop/core/fund/
+-rw-rw-rw-   0        0        0      996 2023-08-01 14:51:48.000000 sharetop-2.4.7/sharetop/core/fund/__init__.py
+-rw-rw-rw-   0        0        0      927 2023-07-28 01:21:27.000000 sharetop-2.4.7/sharetop/core/fund/config.py
+-rw-rw-rw-   0        0        0     2727 2023-07-28 00:06:51.000000 sharetop-2.4.7/sharetop/core/fund/fund_list.py
+-rw-rw-rw-   0        0        0     1857 2023-07-31 14:52:45.000000 sharetop-2.4.7/sharetop/core/fund/get_fund_base_info.py
+-rw-rw-rw-   0        0        0     2624 2023-07-31 15:04:18.000000 sharetop-2.4.7/sharetop/core/fund/get_fund_history_data.py
+-rw-rw-rw-   0        0        0     3850 2023-08-01 14:19:07.000000 sharetop-2.4.7/sharetop/core/fund/get_fund_industry_info.py
+-rw-rw-rw-   0        0        0     5721 2023-08-01 14:30:58.000000 sharetop-2.4.7/sharetop/core/fund/get_fund_invest_info.py
+-rw-rw-rw-   0        0        0    12432 2023-07-31 14:59:03.000000 sharetop-2.4.7/sharetop/core/fund/get_fund_rank.py
+-rw-rw-rw-   0        0        0     1466 2023-04-22 03:27:53.000000 sharetop-2.4.7/sharetop/core/fund/get_fund_real_time.py
+-rw-rw-rw-   0        0        0     2631 2023-08-01 14:41:19.000000 sharetop-2.4.7/sharetop/core/fund/get_period_change_info.py
+-rw-rw-rw-   0        0        0     2561 2023-08-01 14:47:27.000000 sharetop-2.4.7/sharetop/core/fund/get_types_percentage_info.py
+drwxrwxrwx   0        0        0        0 2023-08-03 22:44:24.183500 sharetop-2.4.7/sharetop/core/futures/
+-rw-rw-rw-   0        0        0      250 2023-07-16 02:07:46.000000 sharetop-2.4.7/sharetop/core/futures/__init__.py
+-rw-rw-rw-   0        0        0    10308 2023-08-01 22:59:24.000000 sharetop-2.4.7/sharetop/core/futures/get_futures_info.py
+drwxrwxrwx   0        0        0        0 2023-08-03 22:44:24.206698 sharetop-2.4.7/sharetop/core/oil/
+-rw-rw-rw-   0        0        0      402 2023-05-16 01:17:51.000000 sharetop-2.4.7/sharetop/core/oil/__init__.py
+-rw-rw-rw-   0        0        0     1685 2023-05-15 00:28:25.000000 sharetop-2.4.7/sharetop/core/oil/config.py
+-rw-rw-rw-   0        0        0     4004 2023-08-02 04:17:10.000000 sharetop-2.4.7/sharetop/core/oil/oil_detail.py
+drwxrwxrwx   0        0        0        0 2023-08-03 22:44:24.236159 sharetop-2.4.7/sharetop/core/pig/
+-rw-rw-rw-   0        0        0       84 2023-07-15 10:46:51.000000 sharetop-2.4.7/sharetop/core/pig/__init__.py
+-rw-rw-rw-   0        0        0      163 2023-05-16 00:42:46.000000 sharetop-2.4.7/sharetop/core/pig/config.py
+-rw-rw-rw-   0        0        0     1538 2023-08-02 13:50:09.000000 sharetop-2.4.7/sharetop/core/pig/pig_detail.py
+drwxrwxrwx   0        0        0        0 2023-08-03 22:44:24.289402 sharetop-2.4.7/sharetop/core/stock/
+-rw-rw-rw-   0        0        0      662 2023-07-15 09:27:19.000000 sharetop-2.4.7/sharetop/core/stock/__init__.py
+-rw-rw-rw-   0        0        0     4834 2023-07-20 01:18:36.000000 sharetop-2.4.7/sharetop/core/stock/bill_monitor.py
+-rw-rw-rw-   0        0        0     1163 2023-07-19 01:27:46.000000 sharetop-2.4.7/sharetop/core/stock/config.py
+-rw-rw-rw-   0        0        0    15110 2023-07-20 01:10:32.000000 sharetop-2.4.7/sharetop/core/stock/getter.py
+-rw-rw-rw-   0        0        0    10620 2023-07-19 01:27:46.000000 sharetop-2.4.7/sharetop/core/stock/quarterly_report.py
+-rw-rw-rw-   0        0        0    10240 2023-07-27 23:27:15.000000 sharetop-2.4.7/sharetop/core/stock/rank_list.py
+-rw-rw-rw-   0        0        0      693 2023-07-19 12:30:45.000000 sharetop-2.4.7/sharetop/core/stock/stock_base_info.py
+-rw-rw-rw-   0        0        0     7299 2023-07-19 04:12:02.000000 sharetop-2.4.7/sharetop/core/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-03 22:44:24.304714 sharetop-2.4.7/sharetop/crawl/
+-rw-rw-rw-   0        0        0       29 2023-04-09 23:19:21.000000 sharetop-2.4.7/sharetop/crawl/__init__.py
+-rw-rw-rw-   0        0        0     1088 2023-07-19 05:03:18.000000 sharetop-2.4.7/sharetop/crawl/base.py
+-rw-rw-rw-   0        0        0     3271 2023-07-09 23:57:40.000000 sharetop-2.4.7/sharetop/crawl/settings.py
+drwxrwxrwx   0        0        0        0 2023-08-03 22:44:24.329809 sharetop-2.4.7/sharetop/parser/
+-rw-rw-rw-   0        0        0       27 2023-04-10 00:54:05.000000 sharetop-2.4.7/sharetop/parser/__init__.py
+-rw-rw-rw-   0        0        0     4364 2023-07-19 04:59:24.000000 sharetop-2.4.7/sharetop/parser/base.py
+-rw-rw-rw-   0        0        0     2911 2023-07-19 05:36:09.000000 sharetop-2.4.7/sharetop/parser/config.py
+drwxrwxrwx   0        0        0        0 2023-08-03 22:44:24.445429 sharetop-2.4.7/sharetop/test/
+-rw-rw-rw-   0        0        0        0 2023-04-29 10:57:35.000000 sharetop-2.4.7/sharetop/test/__init__.py
+-rw-rw-rw-   0        0        0      541 2023-08-01 15:19:39.000000 sharetop-2.4.7/sharetop/test/bond_test.py
+-rw-rw-rw-   0        0        0      199 2023-05-17 04:49:54.000000 sharetop-2.4.7/sharetop/test/captial.py
+-rw-rw-rw-   0        0        0      162 2023-08-01 23:04:30.000000 sharetop-2.4.7/sharetop/test/country_test.py
+-rw-rw-rw-   0        0        0      582 2023-07-25 15:03:47.000000 sharetop-2.4.7/sharetop/test/flow_monitor_test.py
+-rw-rw-rw-   0        0        0     1691 2023-08-01 14:51:22.000000 sharetop-2.4.7/sharetop/test/fund_test.py
+-rw-rw-rw-   0        0        0      418 2023-08-01 23:01:15.000000 sharetop-2.4.7/sharetop/test/futures_test.py
+-rw-rw-rw-   0        0        0      692 2023-08-02 04:13:46.000000 sharetop-2.4.7/sharetop/test/oil_test.py
+-rw-rw-rw-   0        0        0      217 2023-08-02 04:46:46.000000 sharetop-2.4.7/sharetop/test/pig_test.py
+-rw-rw-rw-   0        0        0     1255 2023-08-03 22:41:53.000000 sharetop-2.4.7/sharetop/test/stock_test.py
+-rw-rw-rw-   0        0        0      992 2023-07-17 01:23:58.000000 sharetop-2.4.7/sharetop/test/test1.py
+-rw-rw-rw-   0        0        0     1997 2023-05-02 03:48:40.000000 sharetop-2.4.7/sharetop/test/test2-akshare.py
+-rw-rw-rw-   0        0        0     3709 2023-05-03 07:10:48.000000 sharetop-2.4.7/sharetop/test/test3.py
+-rw-rw-rw-   0        0        0      221 2023-07-30 10:45:50.000000 sharetop-2.4.7/sharetop/test/test4.py
+-rw-rw-rw-   0        0        0      690 2023-07-15 03:35:15.000000 sharetop-2.4.7/sharetop/test/test5.py
+-rw-rw-rw-   0        0        0     1227 2023-07-15 03:35:15.000000 sharetop-2.4.7/sharetop/test/test6.py
+-rw-rw-rw-   0        0        0      643 2023-07-05 12:16:23.000000 sharetop-2.4.7/sharetop/test/test7.py
+drwxrwxrwx   0        0        0        0 2023-08-03 22:44:23.874347 sharetop-2.4.7/sharetop.egg-info/
+-rw-rw-rw-   0        0        0    51253 2023-08-03 22:44:23.000000 sharetop-2.4.7/sharetop.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2456 2023-08-03 22:44:23.000000 sharetop-2.4.7/sharetop.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 22:44:23.000000 sharetop-2.4.7/sharetop.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-08-03 22:44:23.000000 sharetop-2.4.7/sharetop.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-08-03 22:44:23.000000 sharetop-2.4.7/sharetop.egg-info/top_level.txt
```

### Comparing `sharetop-2.4.6/LICENSE` & `sharetop-2.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.6/PKG-INFO` & `sharetop-2.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sharetop
-Version: 2.4.6
+Version: 2.4.7
 Summary: Provide data related to the economic market
 Home-page: https://github.com/nrliangxy/sharetop
 Author: nrliangxy
 Author-email: nrliangxy@foxmail.com
 License: MIT
 Project-URL: Source, https://github.com/nrliangxy/sharetop
 Keywords: data,finance,quant,stock,fund,futures,share
```

### Comparing `sharetop-2.4.6/README.md` & `sharetop-2.4.7/README.md`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.6/setup.py` & `sharetop-2.4.7/setup.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.6/sharetop/application/base.py` & `sharetop-2.4.7/sharetop/application/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         r = {v: data.get(k) for k, v in fields_k_v.items()}
         return pd.DataFrame([r])
 
     def deal_market_realtime(self, columns):
         df = pd.DataFrame(self.json_data['data']['diff'])
         df = df.rename(columns=columns)
         df: pd.DataFrame = df[columns.values()]
-        df['行情ID'] = df['市场编号'].astype(str) + '.' + df['代码'].astype(str)
+        # df['行情ID'] = df['市场编号'].astype(str) + '.' + df['代码'].astype(str)
         df['市场类型'] = df['市场编号'].astype(str).apply(lambda x: MARKET_NUMBER_DICT.get(x))
         df['更新时间'] = df['更新时间戳'].apply(lambda x: str(datetime.fromtimestamp(x)))
         df['最新交易日'] = pd.to_datetime(df['最新交易日'], format='%Y%m%d').astype(str)
         tmp = df['最新交易日']
         del df['最新交易日']
         df['最新交易日'] = tmp
         del df['更新时间戳']
```

### Comparing `sharetop-2.4.6/sharetop/core/bond/__init__.py` & `sharetop-2.4.7/sharetop/core/bond/__init__.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.6/sharetop/core/bond/config.py` & `sharetop-2.4.7/sharetop/core/bond/config.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.6/sharetop/core/bond/get_bond_info.py` & `sharetop-2.4.7/sharetop/core/bond/get_bond_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 from typing import List
 from ..common.config import EASTMONEY_REQUEST_HEADERS, FS_DICT
 from .config import EASTMONEY_BOND_BASE_INFO_FIELDS
 from ..utils import requests_obj
 from ...crawl.settings import *
 from ..utils import to_numeric, process_dataframe_and_series, validate_request
 from ..common import get_market_realtime_by_fs
+from ..common.explain_change import exchange_explain
 
 
 @validate_request
-def get_bond_base_info_list(token: str) -> pd.DataFrame:
+def get_bond_base_info_list(token: str, is_explain: bool = False) -> pd.DataFrame:
     """
     获取全部债券基本信息列表
     Returns
     -------
     DataFrame
         债券一些基本信息
     Examples
@@ -50,20 +51,20 @@
         if json_response['result'] is None:
             break
         data = json_response['result']['data']
         df = pd.DataFrame(data).rename(columns=columns)[columns.values()]
         dfs.append(df)
         page += 1
     df = pd.concat(dfs, ignore_index=True)
-    return df
+    return exchange_explain(df, is_explain)
 
 
 @process_dataframe_and_series(remove_columns_and_indexes=['市场编号'])
 @to_numeric
-def get_bond_realtime_quotes(**kwargs) -> pd.DataFrame:
+def get_bond_realtime_quotes(is_explain: bool = False, **kwargs) -> pd.DataFrame:
     """
     获取沪深市场全部债券实时行情信息
     Returns
     -------
     DataFrame
         沪深市场全部债券实时行情信息
     Examples
@@ -79,50 +80,50 @@
     391  128017  金禾转债  -4.86  182.676  204.989   182.61  195.16  -9.324    35.58    2.0     -   196375   375750768.0   192.0  1008366222  1008366222  0.128017   深A
     392  113548  石英转债  -5.16   250.22   267.57   246.56   262.3  -13.61   143.32   0.72     -   175893   452796304.0  263.83   307086749   307086749  1.113548   沪A
     393  128093  百川转债  -5.71  429.042   449.97  426.078   443.1 -25.958   426.86   0.36     -   693261  3032643232.0   455.0   696810974   696810974  0.128093   深A
     394  123066  赛意转债   -6.0   193.08  203.999   193.08   203.0  -12.32   323.13   0.22     -   133317   261546032.0   205.4    79660753    79660753  0.123066   深A
     """
     df = get_market_realtime_by_fs(FS_DICT['bond'], **kwargs)
     df.rename(columns={'代码': '债券代码', '名称': '债券名称'}, inplace=True)
-    return df
+    return exchange_explain(df, is_explain)
 
 
 @validate_request
 @to_numeric
-def get_bond_base_info(token: str, bond_code: str) -> pd.Series:
+def get_bond_base_info(token: str, bond_code: str, is_explain: bool = False) -> pd.Series:
     """
     获取单只债券基本信息
     Parameters
     ----------
     bond_code : str
         债券代码
     Returns
     -------
     Series
         债券的一些基本信息
+        :param is_explain:
         :param bond_code:
         :param token:
     """
     columns = EASTMONEY_BOND_BASE_INFO_FIELDS
     params = (
         ('reportName', 'RPT_BOND_CB_LIST'),
         ('columns', 'ALL'),
         ('source', 'WEB'),
         ('client', 'WEB'),
         ('filter', f'(SECURITY_CODE="{bond_code}")'),
     )
     url = ''.join(bond_base_info_url)
     json_response = requests_obj.get(url, params, headers=EASTMONEY_REQUEST_HEADERS).json()
-    print("json_response============:", json_response)
     if json_response['result'] is None:
         return pd.Series(index=columns.values(), dtype='object')
     items = json_response['result']['data']
-    s = pd.Series(items[0]).rename(index=columns)
+    s = pd.DataFrame(items).rename(columns=columns)
     s = s[columns.values()]
-    return s
+    return exchange_explain(s, is_explain)
 
 
 @validate_request
 def get_bond_public(token: str) -> pd.DataFrame:
     """
     中国-债券信息披露-债券发行
     http://www.chinamoney.com.cn/chinese/xzjfx/
```

### Comparing `sharetop-2.4.6/sharetop/core/bond/get_bond_public_info.py` & `sharetop-2.4.7/sharetop/core/bond/get_bond_public_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.6/sharetop/core/cache.py` & `sharetop-2.4.7/sharetop/core/cache.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.6/sharetop/core/capital_flow/capital_flow_monitor.py` & `sharetop-2.4.7/sharetop/core/capital_flow/capital_flow_monitor.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.6/sharetop/core/common/common_base.py` & `sharetop-2.4.7/sharetop/core/common/common_base.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.6/sharetop/core/common/config.py` & `sharetop-2.4.7/sharetop/core/common/config.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.6/sharetop/core/common/explain_change.py` & `sharetop-2.4.7/sharetop/core/common/explain_change.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import inspect
 
+
 class Explain:
     get_stock_all_report_dates_fields = {
         "报告日期": "report_date",
         "季报名称": "quarterly_report_title"
     }
 
     get_stock_market_real_time_data_fields = {
@@ -19,15 +20,15 @@
         "量比": "volume_ratio",
         "动态市盈率": "price_to_earnings_ratio",
         "成交量": "trading_volume",
         "成交额": "volume",
         "昨日收盘": "previous_close",
         "总市值": "market_cap",
         "流通市值": "free_float_market_cap",
-        "行情ID": "item_id",
+        # "行情ID": "item_id",
         "市场类型": "market_type",
         "更新时间": "update_time",
         "最新交易日": "latest_trading_day"
     }
 
     get_stock_all_company_quarterly_report_fields = {
         "股票代码": "stock_code",
@@ -356,14 +357,220 @@
     get_fund_history_price_fields = {
         "日期": "date",
         "单位净值": "nav_per_unit",
         "累计净值": "cumulative_net_asset_value",
         "涨跌幅": "percentage_change"
     }
 
+    get_fund_industry_distribution_fields = {
+        "基金代码": "fund_code",
+        "行业名称": "industry_name",
+        "持仓比例": "position_ratio",
+        "公布日期": "announcement_date",
+        "市值": "market_cap"
+    }
+
+    get_fund_invest_position_fields = {
+        "基金代码": "fund_code",
+        "股票代码": "stock_code",
+        "股票简称": "stock_name",
+        "持仓占比": "weight",
+        "较上期变化": "change",
+        "公开日期": "pub_date"
+    }
+
+    get_fund_period_change_fields = {
+        "基金代码": "fund_code",
+        "收益率": "yield",
+        "同类平均": "category_average",
+        "同类排行": "category_ranking",
+        "同类总数": "total_number_categories",
+        "时间段": "time_period"
+    }
+
+    get_fund_types_percentage_fields = {
+        "基金代码": "fund_code",
+        "股票比重": "stock_weight",
+        "债券比重": "bond_weight",
+        "现金比重": "cash_weight",
+        "总规模(亿元)": "total_size",
+        "其他比重": "other_proportions"
+    }
+
+    get_bond_base_info_list_fields = {
+        "债券代码": "bond_code",
+        "债券名称": "bond_name",
+        "正股代码": "equity_code",
+        "正股名称": "equity_name",
+        "债券评级": "bond_rating",
+        "申购日期": "subscription_date",
+        "发行规模(亿)": "issuance_size",
+        "网上发行中签率(%)": "online_subscription_winning_rate",
+        "上市日期": "listing_date",
+        "到期日期": "maturity_date",
+        "期限(年)": "term",
+        "利率说明": "interest_rate_description"
+    }
+
+    get_bond_realtime_quotes_fields = {
+        "债券代码": "bond_code",
+        "债券名称": "bond_name",
+        "涨跌幅": "percentage_change",
+        "最新价": "last_price",
+        "最高": "high_price",
+        "最低": "low_price",
+        "今开": "open_price",
+        "涨跌额": "price_change",
+        "换手率": "turnover_rate",
+        "量比": "volume_ratio",
+        "动态市盈率": "price_to_earnings_ratio",
+        "成交量": "trading_volume",
+        "成交额": "volume",
+        "昨日收盘": "previous_close",
+        "总市值": "market_cap",
+        "流通市值": "free_float_market_cap",
+        "行情ID": "item_id",
+        "市场类型": "market_type",
+        "更新时间": "update_time",
+        "最新交易日": "latest_trading_day"
+    }
+
+    get_bond_base_info_fields = {
+        "债券代码": "bond_code",
+        "债券名称": "bond_name",
+        "正股代码": "equity_code",
+        "正股名称": "equity_name",
+        "债券评级": "bond_rating",
+        "申购日期": "subscription_date",
+        "发行规模(亿)": "issuance_size",
+        "网上发行中签率(%)": "online_subscription_winning_rate",
+        "上市日期": "listing_date",
+        "到期日期": "maturity_date",
+        "期限(年)": "term",
+        "利率说明": "interest_rate_description"
+    }
+
+    get_future_all_realtime_quotes_fields = {
+        "期货代码": "futures_code",
+        "期货名称": "futures_name",
+        "涨跌幅": "percentage_change",
+        "最新价": "last_price",
+        "最高": "high_price",
+        "最低": "low_price",
+        "今开": "open_price",
+        "涨跌额": "price_change",
+        "换手率": "turnover_rate",
+        "量比": "volume_ratio",
+        "动态市盈率": "price_to_earnings_ratio",
+        "成交量": "trading_volume",
+        "成交额": "volume",
+        "昨日收盘": "previous_close",
+        "总市值": "market_cap",
+        "流通市值": "free_float_market_cap",
+        "行情ID": "item_id",
+        "市场类型": "market_type",
+        "更新时间": "update_time",
+        "最新交易日": "latest_trading_day"
+    }
+
+    get_future_deal_detail_fields = {
+        "期货代码": "futures_code",
+        "期货名称": "futures_name",
+        "时间": "time",
+        "昨收": "previous_close",
+        "成交价": "transaction_price",
+        "成交量": "trading_volume",
+        "单数": "lot_size"
+    }
+
+    get_future_history_data_fields = {
+        "期货代码": "futures_code",
+        "期货名称": "futures_name",
+        "日期": "date",
+        "开盘": "opening_price",
+        "收盘": "closing_price",
+        "最高": "highest_price",
+        "最低": "low_price",
+        "成交量": "trading_volume",
+        "成交额": "volume",
+        "振幅": "amplitude",
+        "涨跌幅": "percentage_change",
+        "涨跌额": "price_change",
+        "换手率": "turnover_rate",
+        "盘后量": "after_hours_volume",
+        "盘后额": "after_hours_value"
+    }
+
+    get_country_list_fields = {
+        "国家简称": "country_abbreviation",
+        "国家全称": "country_full_name",
+        "英文简称": "english_abbreviation",
+        "英文全称": "english_full_name",
+        "土地面积(万平方公里)": "land_area",
+        "所属洲": "continent",
+        "机构类型": "institution_type",
+        "首都(中文)": "capital_ch",
+        "首都(英文)": "capital_en",
+        "所属组织": "organization"
+    }
+
+    get_oil_reserves_fields = {
+        "年份": "year",
+        "储量(十亿桶)": "reserves",
+        "总储量占比": "total_reserves_ratio",
+        "储产比": "rpr",
+        "产品名称": "product_name",
+        "机构名称": "institution_name"
+    }
+
+    get_oil_products_fields = {
+        "年份": "year",
+        "产量(千桶/天)": "production",
+        "总产量占比": "total_production_proportion",
+        "产品名称": "product_name",
+        "机构名称": "institution_name"
+    }
+
+    get_oil_consumption_fields = {
+        "年份": "year",
+        "产量(千桶/天)": "production",
+        "总产量占比": "total_production_proportion",
+        "产品名称": "product_name",
+        "机构名称": "institution_name"
+    }
+
+    get_oil_refinerythroughput_fields = {
+        "年份": "year",
+        "加工量(千桶/天)": "processing_volume",
+        "总产量占比": "total_production_proportion",
+        "产品名称": "product_name",
+        "机构名称": "institution_name"
+    }
+
+    get_oil_refinerycapacity_fields = {
+        "年份": "year",
+        "产能(千桶/天)": "production_capacity",
+        "总产能占比": "total_production_capacity_ratio",
+        "产品名称": "product_name",
+        "机构名称": "institution_name"
+    }
+
+    get_oil_crudeoilpricehistory_fields = {
+        "年份": "year",
+        "价格(当年真实价格)": "current_year_real_price",
+        "价格(按2022年美国消费者物价指数平减)": "2022_price",
+        "产品名称": "product_name"
+    }
+
+    get_pig_fcr_fields = {
+        "发布时间": "pub_date",
+        "生猪(外三元)(元/公斤)": "pork_duroc_price",
+        "猪粮比": "fcr"
+    }
+
 
 def exchange_explain_one(df, exchange_fields, is_explain):
     if not is_explain:
         df.rename(columns=exchange_fields, inplace=True)
     return df
```

### Comparing `sharetop-2.4.6/sharetop/core/common/getter.py` & `sharetop-2.4.7/sharetop/core/common/getter.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.6/sharetop/core/config.py` & `sharetop-2.4.7/sharetop/core/config.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.6/sharetop/core/country/country_base_info.py` & `sharetop-2.4.7/sharetop/core/country/country_base_info.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import pandas as pd
 from .config import country_base_url, country_field_dict
 from ...crawl.settings import *
 from ..utils import to_numeric, requests_obj, parse_obj
+from ..common.explain_change import exchange_explain
 
 
 @to_numeric
-def get_country_list(token: str, limit: int = None) -> pd.DataFrame:
+def get_country_list(token: str, limit: int = None, is_explain: bool = False) -> pd.DataFrame:
     """
     国家基本信息列表
     :param token:
     :param limit:
     :return:
     """
     headers = {"token": token}
     base_url_list.append(country_base_url)
     data = {"limit": limit}
     r = requests_obj.get("".join(base_url_list), data=data, headers=headers)
     if isinstance(r, dict):
         return r
     data_json = r.json()
     df = parse_obj.parse_god_cup_json(data_json, country_field_dict)
-    return df
+    return exchange_explain(df, is_explain)
```

### Comparing `sharetop-2.4.6/sharetop/core/fund/__init__.py` & `sharetop-2.4.7/sharetop/core/fund/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from .fund_list import get_fund_codes
-from .get_fund_real_time import get_fund_real_time_god
+# from .get_fund_real_time import get_fund_real_time_god
 from .get_fund_history_data import get_fund_history_price
 from .get_fund_invest_info import get_fund_invest_position, get_fund_public_dates
 from .get_period_change_info import get_fund_period_change
 from .get_types_percentage_info import get_fund_types_percentage
 from .get_fund_base_info import get_fund_base_info
 from .get_fund_industry_info import get_fund_industry_distribution
 from .get_fund_rank import (
@@ -11,15 +11,14 @@
     get_fund_exchange_rank,
     get_fund_money_rank,
     get_fund_hk_rank
 )
 
 __all__ = [
     'get_fund_codes',
-    'get_fund_real_time_god',
     'get_fund_history_price',
     'get_fund_invest_position',
     'get_fund_public_dates',
     'get_fund_period_change',
     'get_fund_types_percentage',
     'get_fund_base_info',
     'get_fund_industry_distribution',
```

### Comparing `sharetop-2.4.6/sharetop/core/fund/config.py` & `sharetop-2.4.7/sharetop/core/fund/config.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.6/sharetop/core/fund/fund_list.py` & `sharetop-2.4.7/sharetop/core/fund/fund_list.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.6/sharetop/core/fund/get_fund_base_info.py` & `sharetop-2.4.7/sharetop/core/fund/get_fund_base_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.6/sharetop/core/fund/get_fund_history_data.py` & `sharetop-2.4.7/sharetop/core/fund/get_fund_history_data.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.6/sharetop/core/fund/get_fund_industry_info.py` & `sharetop-2.4.7/sharetop/core/fund/get_fund_industry_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import uuid
 import pandas as pd
 from typing import List, Union
 from ..utils import to_numeric, requests_obj, validate_request
 from ...crawl.settings import *
 from .config import EastmoneyFundHeaders
+from ..common.explain_change import exchange_explain
 
 
 @validate_request
 @to_numeric
 def get_fund_industry_distribution(
-    token: str, fund_code: str, dates: Union[str, List[str]] = None
+    token: str, fund_code: str, dates: Union[str, List[str]] = None, is_explain: bool = False
 ) -> pd.DataFrame:
     """
     获取指定基金行业分布信息
     Parameters
     ----------
     fund_code : str
         6 位基金代码
@@ -45,14 +46,15 @@
     13  161725            住宿和餐饮业     --  2021-06-30              --
     14  161725              房地产业     --  2021-06-30              --
     15  161725     居民服务、修理和其他服务业     --  2021-06-30              --
     16  161725           卫生和社会工作     --  2021-06-30              --
     17  161725         文化、体育和娱乐业     --  2021-06-30              --
     18  161725                综合     --  2021-06-30              --
     19  161725                合计  93.08  2021-06-30  6493286.808514
+    :param is_explain:
     :param dates:
     :param fund_code:
     :param token:
     """
     columns = {'HYMC': '行业名称', 'ZJZBL': '持仓比例', 'FSRQ': '公布日期', 'SZ': '市值'}
     str_uuid = str(uuid.uuid4()).upper()
     df = pd.DataFrame(columns=columns.values())
@@ -77,8 +79,8 @@
         response = requests_obj.get(url, params, headers=EastmoneyFundHeaders)
         datas = response.json()['Datas']
         _df = pd.DataFrame(datas)
         _df = _df.rename(columns=columns)
         df = pd.concat([df, _df], axis=0, ignore_index=True)
     df.insert(0, '基金代码', fund_code)
     df = df.drop_duplicates()
-    return df
+    return exchange_explain(df, is_explain)
```

### Comparing `sharetop-2.4.6/sharetop/core/fund/get_fund_invest_info.py` & `sharetop-2.4.7/sharetop/core/fund/get_fund_invest_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import uuid
 import pandas as pd
 from typing import List, Union
 from retry import retry
 from ..utils import to_numeric, requests_obj, validate_request
 from jsonpath import jsonpath
 from .config import EastmoneyFundHeaders
+from ..common.explain_change import exchange_explain
 
 
 @validate_request
 @retry(tries=3)
 @to_numeric
 def get_fund_invest_position(token: str,
-    fund_code: str, dates: Union[str, List[str]] = None
-) -> pd.DataFrame:
+                             fund_code: str, dates: Union[str, List[str]] = None, is_explain: bool = False
+                             ) -> pd.DataFrame:
     """
     获取基金持仓占比数据
     Parameters
     ----------
     fund_code : str
         基金代码
     dates : Union[str, List[str]], optional
@@ -61,17 +62,20 @@
     13  161725  000858   五粮液  14.09   0.87  2021-12-31
     14  161725  002304  洋河股份  10.67  -1.34  2021-12-31
     15  161725  000799   酒鬼酒   4.31   0.09  2021-12-31
     16  161725  603369   今世缘   3.79   0.81  2021-12-31
     17  161725  000596  古井贡酒   3.51  -0.69  2021-12-31
     18  161725  600779   水井坊   2.85  -0.41  2021-12-31
     19  161725  603589   口子窖   2.68   2.68  2021-12-31
+    :param token:
+    :param fund_code:
+    :param dates:
+    :param is_explain:
 
     """
-
     columns = {
         'GPDM': '股票代码',
         'GPJC': '股票简称',
         'JZBL': '持仓占比',
         'PCTNVCHG': '较上期变化',
     }
     str_uuid = str(uuid.uuid4()).upper()
@@ -103,15 +107,15 @@
         _df['公开日期'] = date
         _df.insert(0, '基金代码', fund_code)
         dfs.append(_df)
     fields = ['基金代码'] + list(columns.values()) + ['公开日期']
     if not dfs:
         return pd.DataFrame(columns=fields)
     df = pd.concat(dfs, axis=0, ignore_index=True).rename(columns=columns)[fields]
-    return df
+    return exchange_explain(df, is_explain)
 
 
 @validate_request
 def get_fund_public_dates(token: str, fund_code: str) -> List[str]:
     """
     获取历史上更新持仓情况的日期列表
     Parameters
```

### Comparing `sharetop-2.4.6/sharetop/core/fund/get_fund_rank.py` & `sharetop-2.4.7/sharetop/core/fund/get_fund_rank.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.6/sharetop/core/fund/get_fund_real_time.py` & `sharetop-2.4.7/sharetop/core/fund/get_fund_real_time.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.6/sharetop/core/fund/get_period_change_info.py` & `sharetop-2.4.7/sharetop/core/fund/get_period_change_info.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import uuid
 import pandas as pd
 from retry import retry
 from ..utils import to_numeric, requests_obj, validate_request
 from .config import EastmoneyFundHeaders
 from ...crawl.settings import *
+from ..common.explain_change import exchange_explain
 
 
 @validate_request
 @retry(tries=3)
 @to_numeric
-def get_fund_period_change(token: str, fund_code: str) -> pd.DataFrame:
+def get_fund_period_change(token: str, fund_code: str, is_explain: bool = False) -> pd.DataFrame:
     """
     获取基金阶段涨跌幅度
     Parameters
     ----------
     fund_code : str
         6 位基金代码
     Returns
@@ -29,14 +30,15 @@
     3  161725   22.93  10.39    79  1223   近六月
     4  161725  103.76  33.58     7  1118   近一年
     5  161725  166.59  55.42     9   796   近两年
     6  161725  187.50  48.17     2   611   近三年
     7  161725  519.44  61.62     1   389   近五年
     8  161725    6.46   5.03   423  1243  今年以来
     9  161725  477.00                     成立以来
+    :param is_explain:
     :param fund_code:
     :param token:
     """
     str_uuid = str(uuid.uuid4()).upper()
     params = (
         ('AppVersion', '6.3.8'),
         ('FCODE', fund_code),
@@ -70,8 +72,8 @@
     }
     # 发行时间
     ESTABDATE = json_response['Expansion']['ESTABDATE']
     df = pd.DataFrame(json_response['Datas'])
     df = df[list(columns.keys())].rename(columns=columns)
     df['时间段'] = titles.values()
     df.insert(0, '基金代码', fund_code)
-    return df
+    return exchange_explain(df, is_explain)
```

### Comparing `sharetop-2.4.6/sharetop/core/fund/get_types_percentage_info.py` & `sharetop-2.4.7/sharetop/core/fund/get_types_percentage_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from retry import retry
 from ..utils import to_numeric, requests_obj, validate_request
 from .config import EastmoneyFundHeaders
 from typing import List, Union
 from ...crawl.settings import *
 import pandas as pd
+from ..common.explain_change import exchange_explain
 
 
 @validate_request
 @retry(tries=3)
 @to_numeric
 def get_fund_types_percentage(
-    token: str, fund_code: str, dates: Union[List[str], str, None] = None
+    token: str, fund_code: str, dates: Union[List[str], str, None] = None, is_explain: bool = False
 ) -> pd.DataFrame:
     """
     获取指定基金不同类型占比信息
     Parameters
     ----------
     fund_code : str
         6 位基金代码
@@ -61,8 +62,8 @@
         json_response = requests_obj.get(url, params, headers=EastmoneyFundHeaders).json()
         if len(json_response['Datas']) == 0:
             continue
         _df = pd.DataFrame(json_response['Datas'])[columns.keys()]
         _df = _df.rename(columns=columns)
         df = pd.concat([df, _df], axis=0, ignore_index=True)
     df.insert(0, '基金代码', fund_code)
-    return df
+    return exchange_explain(df, is_explain)
```

### Comparing `sharetop-2.4.6/sharetop/core/futures/get_futures_info.py` & `sharetop-2.4.7/sharetop/core/futures/get_futures_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import pandas as pd
 from ..common.config import FS_DICT
 from typing import Dict, List, Union
 from ..common.getter import get_market_realtime_by_fs, get_deal_detail
 from ..utils import process_dataframe_and_series, validate_request
 from ..common import get_history as get_quote_history_for_futures
+from ..common.explain_change import exchange_explain
 
 
 @validate_request
 def get_futures_base_info(token: str) -> pd.DataFrame:
     """
     获取四个交易所全部期货基本信息
     Returns
@@ -41,14 +42,15 @@
 def get_future_history_data(
     token: str,
     quote_ids: Union[str, List[str]],
     beg: str = '19000101',
     end: str = '20500101',
     klt: int = 101,
     fqt: int = 1,
+    is_explain: bool = False,
     **kwargs
 ) -> pd.DataFrame:
     """
     获取期货历史行情信息
 
     Parameters
     ----------
@@ -108,34 +110,35 @@
     4     动力煤主力  ZCM  2015-05-22  439.2  441.4  443.8  439.2     34  1.502500e+06  1.04  0.09   0.4  0.0
     ...     ...  ...         ...    ...    ...    ...    ...    ...           ...   ...   ...   ...  ...
     1524  动力煤主力  ZCM  2021-08-17  755.0  770.8  776.0  750.6  82373  6.288355e+09  3.25 -1.26  -9.8  0.0
     1525  动力煤主力  ZCM  2021-08-18  770.8  776.8  785.8  766.0  77392  6.016454e+09  2.59  1.76  13.4  0.0
     1526  动力煤主力  ZCM  2021-08-19  776.8  777.6  798.0  764.6  97229  7.597474e+09  4.30  0.03   0.2  0.0
     1527  动力煤主力  ZCM  2021-08-20  778.0  793.0  795.0  775.2  70549  5.553617e+09  2.53  1.48  11.6  0.0
     1528  动力煤主力  ZCM  2021-08-23  796.8  836.6  843.8  796.8  82954  6.850341e+09  5.97  6.28  49.4  0.0
+    :param is_explain:
 
     """
     df = get_quote_history_for_futures(
         quote_ids, beg=beg, end=end, klt=klt, fqt=fqt, quote_id_mode=True
     )
     if isinstance(df, pd.DataFrame):
 
         df.rename(columns={'代码': '期货代码', '名称': '期货名称'}, inplace=True)
     elif isinstance(df, dict):
         for stock_code in df.keys():
             df[stock_code].rename(columns={'代码': '期货代码', '名称': '期货名称'}, inplace=True)
             # NOTE 扩展接口 设定此关键词即返回 DataFrame 而不是 dict
         if kwargs.get('return_df'):
             df: pd.DataFrame = pd.concat(df, axis=0, ignore_index=True)
-    return df
+    return exchange_explain(df, is_explain)
 
 
 @validate_request
 @process_dataframe_and_series(remove_columns_and_indexes=['市场编号'])
-def get_future_all_realtime_quotes(token: str) -> pd.DataFrame:
+def get_future_all_realtime_quotes(token: str, is_explain: bool = False) -> pd.DataFrame:
     """
     获取期货最新行情总体情况
     Returns
     -------
     DataFrame
         期货市场的最新行情信息（涨跌幅、换手率等信息）
 
@@ -157,18 +160,18 @@
     Notes
     -----
     来获取期货 K 线数据
     """
     fs = FS_DICT['futures']
     df = get_market_realtime_by_fs(fs)
     df = df.rename(columns={'代码': '期货代码', '名称': '期货名称'})
-    return df
+    return exchange_explain(df, is_explain)
 
 
-def get_future_deal_detail(quote_id: str, max_count: int = 1000000) -> pd.DataFrame:
+def get_future_deal_detail(quote_id: str, max_count: int = 1000000, is_explain: bool = False) -> pd.DataFrame:
     """
     获取期货最新交易日成交明细
     Parameters
     ----------
     quote_id : str
         期货行情ID
     max_count : int, optional
@@ -187,8 +190,8 @@
     0  动力煤主力  ZCM  21:00:00  0.0  879.0   23    0.0
     1  动力煤主力  ZCM  21:00:00  0.0  879.0    0 -373.0
     2  动力煤主力  ZCM  21:00:00  0.0  879.0    0    0.0
 
     """
     df = get_deal_detail(quote_id, max_count=max_count)
     df.rename(columns={'代码': '期货代码', '名称': '期货名称'}, inplace=True)
-    return df
+    return exchange_explain(df, is_explain)
```

### Comparing `sharetop-2.4.6/sharetop/core/oil/config.py` & `sharetop-2.4.7/sharetop/core/oil/config.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.6/sharetop/core/oil/oil_detail.py` & `sharetop-2.4.7/sharetop/core/oil/oil_detail.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import copy
 from .config import oil_reserves_url, oil_reserves_field_dict, oil_products_field_dict, oil_products_url, \
     oil_consumption_url, oil_consumption_field_dict, oil_refinerythroughput_field_dict, oil_refinerythroughput_url, \
     oil_refinerycapacity_url, oil_refinerycapacity_field_dict, oil_crudeoilpricehistory_field_dict, \
     oil_crudeoilpricehistory_url
 from ...crawl.settings import *
 from ..utils import to_numeric, requests_obj, parse_obj
+from ..common.explain_change import exchange_explain
 
 
 @to_numeric
 def get_oil_data_common(token: str, oil_url: str, field_dict: dict, data_type: str = None,
                         limit: int = None) -> pd.DataFrame:
     """
     :param token:
@@ -31,70 +32,70 @@
     if isinstance(r, dict):
         return r
     data_json = r.json()
     df = parse_obj.parse_god_cup_json(data_json, field_dict)
     return df
 
 
-def get_oil_reserves(token: str, data_type: str = None, limit: int = None) -> pd.DataFrame:
+def get_oil_reserves(token: str, data_type: str = None, limit: int = None, is_explain: bool = False) -> pd.DataFrame:
     """
     获取机构的石油储量
     :param token:
     :param data_type: 1为国家数据 2为机构数据 4为大洲数据
     :param limit:
     :return:
     """
-    return get_oil_data_common(token, oil_reserves_url, oil_reserves_field_dict, data_type, limit)
+    return exchange_explain(get_oil_data_common(token, oil_reserves_url, oil_reserves_field_dict, data_type, limit), is_explain)
 
 
-def get_oil_products(token: str, data_type: str = None, limit: int = None) -> pd.DataFrame:
+def get_oil_products(token: str, data_type: str = None, limit: int = None, is_explain: bool = False) -> pd.DataFrame:
     """
     获取机构的石油产量
     :param token:
     :param data_type: 1为国家数据 2为机构数据 4为大洲数据
     :param limit:
     :return:
     """
-    return get_oil_data_common(token, oil_products_url, oil_products_field_dict, data_type, limit)
+    return exchange_explain(get_oil_data_common(token, oil_products_url, oil_products_field_dict, data_type, limit), is_explain)
 
 
-def get_oil_consumption(token: str, data_type: str = None, limit: int = None) -> pd.DataFrame:
+def get_oil_consumption(token: str, data_type: str = None, limit: int = None, is_explain: bool = False) -> pd.DataFrame:
     """
     获取机构的消费量
     :param token:
     :param data_type: 1为国家数据 2为机构数据 4为大洲数据
     :param limit:
     :return:
     """
-    return get_oil_data_common(token, oil_consumption_url, oil_consumption_field_dict, data_type, limit)
+    return exchange_explain(get_oil_data_common(token, oil_consumption_url, oil_consumption_field_dict, data_type, limit), is_explain)
 
 
-def get_oil_refinerythroughput(token: str, data_type: str = None, limit: int = None) -> pd.DataFrame:
+def get_oil_refinerythroughput(token: str, data_type: str = None, limit: int = None, is_explain: bool = False) -> pd.DataFrame:
     """
     获取石油的加工量
     :param token:
     :param data_type: 1为国家数据 2为机构数据 4为大洲数据
     :param limit:
     :return:
     """
-    return get_oil_data_common(token, oil_refinerythroughput_url, oil_refinerythroughput_field_dict, data_type, limit)
+    return exchange_explain(get_oil_data_common(token, oil_refinerythroughput_url, oil_refinerythroughput_field_dict, data_type, limit), is_explain)
 
 
-def get_oil_refinerycapacity(token: str, data_type: str = None, limit: int = None) -> pd.DataFrame:
+def get_oil_refinerycapacity(token: str, data_type: str = None, limit: int = None, is_explain: bool = False) -> pd.DataFrame:
     """
     获取石油的产能
     :param token:
     :param data_type: 1为国家数据 2为机构数据 4为大洲数据
     :param limit:
     :return:
     """
-    return get_oil_data_common(token, oil_refinerycapacity_url, oil_refinerycapacity_field_dict, data_type, limit)
+    return exchange_explain(get_oil_data_common(token, oil_refinerycapacity_url, oil_refinerycapacity_field_dict, data_type, limit), is_explain)
 
 
-def get_oil_crudeoilpricehistory(token: str, limit: int = None) -> pd.DataFrame:
+def get_oil_crudeoilpricehistory(token: str, limit: int = None, is_explain: bool = False) -> pd.DataFrame:
     """
     获取石油的历史价格
     :param token:
     :param limit: 数据限制
     :return:
     """
-    return get_oil_data_common(token, oil_crudeoilpricehistory_url, oil_crudeoilpricehistory_field_dict, limit=limit)
+    return exchange_explain(get_oil_data_common(token, oil_crudeoilpricehistory_url, oil_crudeoilpricehistory_field_dict, limit=limit), is_explain)
```

### Comparing `sharetop-2.4.6/sharetop/core/pig/pig_detail.py` & `sharetop-2.4.7/sharetop/core/pig/pig_detail.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import copy
 import pandas as pd
 from .config import pig_fcr_url, pig_fcr_field_dict
 from ...crawl.settings import *
 from ..utils import to_numeric, requests_obj, parse_obj
+from ..common.explain_change import exchange_explain
 
 
 @to_numeric
 def get_pig_data_common(token: str, pig_url: str, field_dict: dict, start_date: str, end_date: str, limit: int) -> pd.DataFrame:
     """
     :param token:
     :param field_dict:
@@ -30,17 +31,17 @@
     if isinstance(r, dict):
         return r
     data_json = r.json()
     df = parse_obj.parse_god_cup_json(data_json, field_dict)
     return df
 
 
-def get_pig_fcr(token: str, start_date: str = None, end_date: str = None, limit: int = None) -> pd.DataFrame:
+def get_pig_fcr(token: str, start_date: str = None, end_date: str = None, limit: int = None, is_explain: bool = False) -> pd.DataFrame:
     """
     获取猪周期的历史猪肉价格和猪粮比
     :param token:
     :param end_date:
     :param start_date:
     :param limit:
     :return:
     """
-    return get_pig_data_common(token, pig_fcr_url, pig_fcr_field_dict, start_date, end_date,  limit)
+    return exchange_explain(get_pig_data_common(token, pig_fcr_url, pig_fcr_field_dict, start_date, end_date,  limit), is_explain)
```

### Comparing `sharetop-2.4.6/sharetop/core/stock/__init__.py` & `sharetop-2.4.7/sharetop/core/stock/__init__.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.6/sharetop/core/stock/bill_monitor.py` & `sharetop-2.4.7/sharetop/core/stock/bill_monitor.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.6/sharetop/core/stock/config.py` & `sharetop-2.4.7/sharetop/core/stock/config.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.6/sharetop/core/stock/getter.py` & `sharetop-2.4.7/sharetop/core/stock/getter.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.6/sharetop/core/stock/quarterly_report.py` & `sharetop-2.4.7/sharetop/core/stock/quarterly_report.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.6/sharetop/core/stock/rank_list.py` & `sharetop-2.4.7/sharetop/core/stock/rank_list.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.6/sharetop/core/stock/stock_base_info.py` & `sharetop-2.4.7/sharetop/core/stock/stock_base_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.6/sharetop/core/utils.py` & `sharetop-2.4.7/sharetop/core/utils.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.6/sharetop/crawl/base.py` & `sharetop-2.4.7/sharetop/crawl/base.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.6/sharetop/crawl/settings.py` & `sharetop-2.4.7/sharetop/crawl/settings.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.6/sharetop/parser/base.py` & `sharetop-2.4.7/sharetop/parser/base.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.6/sharetop/parser/config.py` & `sharetop-2.4.7/sharetop/parser/config.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.6/sharetop/test/flow_monitor_test.py` & `sharetop-2.4.7/sharetop/test/flow_monitor_test.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.6/sharetop/test/fund_test.py` & `sharetop-2.4.7/sharetop/test/fund_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,20 +2,22 @@
 from sharetop.core.fund.get_fund_base_info import get_fund_base_info
 from sharetop.core.fund.get_fund_history_data import get_fund_history_price
 from sharetop.core.fund.get_fund_industry_info import get_fund_industry_distribution
 from sharetop.core.fund.get_fund_invest_info import get_fund_public_dates, get_fund_invest_position
 from sharetop.core.fund.get_fund_rank import get_fund_open_rank, get_fund_exchange_rank, get_fund_money_rank, get_fund_hk_rank
 from sharetop.core.fund.get_period_change_info import get_fund_period_change
 from sharetop.core.fund.get_types_percentage_info import get_fund_types_percentage
+from sharetop.core.fund.get_fund_real_time import get_fund_real_time_god
+
 
 token = "f109298d079b5f60"
 
 # d = get_fund_base_info(token, "001299")
 
-d = get_fund_history_price(token, "001299")
+# d = get_fund_history_price(token, "001299", is_explain=True)
 
 # d = get_public_dates(token, "001299")
 
 # d = get_fund_industry_distribution(token, "161725", "2023-03-31")
 
 # d = get_fund_invest_position(token, "161725", "2023-03-31")
 
@@ -29,14 +31,15 @@
 
 # d = get_fund_money_rank(token)
 
 # d = get_fund_period_change(token, "161725")
 
 # d = get_fund_types_percentage(token, "161725")
 
+d = get_fund_real_time_god("161725")
 # d = fund_money_rank(token)
 
 # d = get_period_change(token, "001299")
 
 # d = get_types_percentage(token, "001299")
 
 # d = get_fund_codes(token, is_explain=True)
```

### Comparing `sharetop-2.4.6/sharetop/test/stock_test.py` & `sharetop-2.4.7/sharetop/test/stock_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,23 +12,25 @@
 
 # d = get_real_time_bill("002714")
 
 # d = get_history_data(token, "002714", klt=102)
 
 # d = get_real_time_data(["002714", "516110"])
 
-# d = get_stock_market_real_time_data(token, is_explain=True)
+# d = get_stock_market_real_time_data(token, is_explain=False)
 
 # d = get_stock_company_report_data(token, '002714', "一季报", False)
 
 # d = get_stock_all_company_quarterly_report(token, '2021-03-31', True)
 
-d = get_stock_dragon_tiger_list(token, is_explain=True)
+# d = get_stock_dragon_tiger_list(token, is_explain=True)
 
 # d = get_stock_base_info(["002714", "562510"])
 # d = get_stock_base_info(["002714", "600809"], is_explain=True)
 
-# d = get_stock_all_report_dates(token, is_explain=True)
+d = get_stock_all_report_dates(token, is_explain=False)
 
 # d = get_stock_real_time_data("002714", is_explain=False)
 
-print(d.to_dict("records"))
+print(d)
+
+# print(type(d.to_dict("records")[0]['free_float_market_cap']))
```

### Comparing `sharetop-2.4.6/sharetop/test/test1.py` & `sharetop-2.4.7/sharetop/test/test1.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.6/sharetop/test/test2-akshare.py` & `sharetop-2.4.7/sharetop/test/test2-akshare.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.6/sharetop/test/test3.py` & `sharetop-2.4.7/sharetop/test/test3.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.6/sharetop/test/test5.py` & `sharetop-2.4.7/sharetop/test/test5.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.6/sharetop/test/test6.py` & `sharetop-2.4.7/sharetop/test/test6.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.6/sharetop/test/test7.py` & `sharetop-2.4.7/sharetop/test/test7.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.6/sharetop.egg-info/PKG-INFO` & `sharetop-2.4.7/sharetop.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sharetop
-Version: 2.4.6
+Version: 2.4.7
 Summary: Provide data related to the economic market
 Home-page: https://github.com/nrliangxy/sharetop
 Author: nrliangxy
 Author-email: nrliangxy@foxmail.com
 License: MIT
 Project-URL: Source, https://github.com/nrliangxy/sharetop
 Keywords: data,finance,quant,stock,fund,futures,share
```

### Comparing `sharetop-2.4.6/sharetop.egg-info/SOURCES.txt` & `sharetop-2.4.7/sharetop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

