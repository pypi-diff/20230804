# Comparing `tmp/huhk-1.9.6.tar.gz` & `tmp/huhk-1.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huhk-1.9.6.tar", last modified: Tue Aug  1 02:51:39 2023, max compression
+gzip compressed data, was "huhk-1.9.7.tar", last modified: Fri Aug  4 06:33:09 2023, max compression
```

## Comparing `huhk-1.9.6.tar` & `huhk-1.9.7.tar`

### file list

```diff
@@ -1,481 +1,49 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.957186 huhk-1.9.6/
--rw-rw-rw-   0        0        0      223 2023-08-01 02:51:39.956323 huhk-1.9.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.004404 huhk-1.9.6/huhk/
--rw-rw-rw-   0        0        0      772 2023-07-17 02:44:39.000000 huhk-1.9.6/huhk/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.036353 huhk-1.9.6/huhk/case_project/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.9.6/huhk/case_project/__init__.py
--rw-rw-rw-   0        0        0      639 2023-07-12 01:13:24.000000 huhk-1.9.6/huhk/case_project/json_coder.py
--rw-rw-rw-   0        0        0     3258 2023-07-26 08:25:43.000000 huhk-1.9.6/huhk/case_project/main_fun.py
--rw-rw-rw-   0        0        0    21538 2023-08-01 01:55:58.000000 huhk-1.9.6/huhk/case_project/project_base.py
--rw-rw-rw-   0        0        0     1369 2023-08-01 02:06:27.000000 huhk-1.9.6/huhk/case_project/project_init.py
--rw-rw-rw-   0        0        0    18567 2023-07-31 08:18:51.000000 huhk-1.9.6/huhk/case_project/project_string.py
--rw-rw-rw-   0        0        0      895 2023-07-26 08:22:28.000000 huhk-1.9.6/huhk/case_project/setup_set.py
--rw-rw-rw-   0        0        0       17 2023-08-01 02:51:38.000000 huhk-1.9.6/huhk/case_project/version.py
--rw-rw-rw-   0        0        0     9925 2023-07-31 05:34:49.000000 huhk-1.9.6/huhk/init_project.py
--rw-rw-rw-   0        0        0     1267 2023-07-25 09:00:59.000000 huhk-1.9.6/huhk/main.py
--rw-rw-rw-   0        0        0      338 2023-08-01 01:48:08.000000 huhk-1.9.6/huhk/setup_run.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.038376 huhk-1.9.6/huhk/testcase/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.9.6/huhk/testcase/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.078871 huhk-1.9.6/huhk/testcase/apache/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.9.6/huhk/testcase/apache/__init__.py
--rw-rw-rw-   0        0        0     3355 2023-07-12 01:13:24.000000 huhk-1.9.6/huhk/testcase/apache/beam_class.py
--rw-rw-rw-   0        0        0     5523 2023-07-12 02:37:05.000000 huhk-1.9.6/huhk/testcase/apache/data.py
--rw-rw-rw-   0        0        0     1764 2023-07-12 01:13:24.000000 huhk-1.9.6/huhk/testcase/apache/par_do.py
--rw-rw-rw-   0        0        0     7257 2023-07-14 06:52:17.000000 huhk-1.9.6/huhk/testcase/apache/test_cogroupbykey.py
--rw-rw-rw-   0        0        0      476 2023-07-14 06:52:17.000000 huhk-1.9.6/huhk/testcase/apache/test_file.py
--rw-rw-rw-   0        0        0     1503 2023-07-14 06:52:17.000000 huhk-1.9.6/huhk/testcase/apache/test_fiter.py
--rw-rw-rw-   0        0        0     2103 2023-07-14 06:52:17.000000 huhk-1.9.6/huhk/testcase/apache/test_flatmap.py
--rw-rw-rw-   0        0        0      523 2023-07-14 06:52:17.000000 huhk-1.9.6/huhk/testcase/apache/test_map.py
--rw-rw-rw-   0        0        0     2632 2023-07-14 07:03:11.000000 huhk-1.9.6/huhk/testcase/apache/test_par_do.py
--rw-rw-rw-   0        0        0     1651 2023-07-14 06:52:17.000000 huhk-1.9.6/huhk/testcase/apache/test_regex.py
--rw-rw-rw-   0        0        0     1571 2023-07-14 06:52:17.000000 huhk-1.9.6/huhk/testcase/apache/test_time.py
--rw-rw-rw-   0        0        0      508 2023-07-14 06:52:16.000000 huhk-1.9.6/huhk/testcase/apache/test_to_string.py
--rw-rw-rw-   0        0        0    22615 2023-07-14 06:52:17.000000 huhk-1.9.6/huhk/unit_apache_beam.py
--rw-rw-rw-   0        0        0      352 2023-07-31 09:35:09.000000 huhk-1.9.6/huhk/unit_data.py
--rw-rw-rw-   0        0        0     4508 2023-07-12 01:13:24.000000 huhk-1.9.6/huhk/unit_dict.py
--rw-rw-rw-   0        0        0     3843 2023-07-12 01:13:24.000000 huhk-1.9.6/huhk/unit_encryption.py
--rw-rw-rw-   0        0        0    29577 2023-08-01 02:47:41.000000 huhk-1.9.6/huhk/unit_fun.py
--rw-rw-rw-   0        0        0     1242 2023-07-12 01:13:24.000000 huhk-1.9.6/huhk/unit_logger.py
--rw-rw-rw-   0        0        0     9960 2023-07-22 07:06:52.000000 huhk-1.9.6/huhk/unit_request.py
--rw-rw-rw-   0        0        0     2511 2023-07-24 06:56:32.000000 huhk-1.9.6/huhk/unit_tasks.py
--rw-rw-rw-   0        0        0      733 2023-07-12 01:13:24.000000 huhk-1.9.6/huhk/常用命令.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.017436 huhk-1.9.6/huhk.egg-info/
--rw-rw-rw-   0        0        0      223 2023-08-01 02:51:38.000000 huhk-1.9.6/huhk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    19653 2023-08-01 02:51:38.000000 huhk-1.9.6/huhk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 02:51:38.000000 huhk-1.9.6/huhk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-08-01 02:51:38.000000 huhk-1.9.6/huhk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      134 2023-08-01 02:51:38.000000 huhk-1.9.6/huhk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-08-01 02:51:38.000000 huhk-1.9.6/huhk.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.081864 huhk-1.9.6/service/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:00.000000 huhk-1.9.6/service/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.086814 huhk-1.9.6/service/app_a/
--rw-rw-rw-   0        0        0      420 2023-08-01 02:26:00.000000 huhk-1.9.6/service/app_a/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.101076 huhk-1.9.6/service/app_a/apis/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:00.000000 huhk-1.9.6/service/app_a/apis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.108058 huhk-1.9.6/service/app_a/apis/admin/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:01.000000 huhk-1.9.6/service/app_a/apis/admin/__init__.py
--rw-rw-rw-   0        0        0     1603 2023-08-01 02:26:01.000000 huhk-1.9.6/service/app_a/apis/admin/apis_admin_guc.py
--rw-rw-rw-   0        0        0      784 2023-08-01 02:26:01.000000 huhk-1.9.6/service/app_a/apis/admin/apis_admin_spa.py
--rw-rw-rw-   0        0        0     1105 2023-08-01 02:26:02.000000 huhk-1.9.6/service/app_a/apis/apis_activitymanager.py
--rw-rw-rw-   0        0        0     2049 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/apis/apis_app_a.py
--rw-rw-rw-   0        0        0     1072 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/apis/apis_area.py
--rw-rw-rw-   0        0        0      914 2023-08-01 02:26:05.000000 huhk-1.9.6/service/app_a/apis/apis_content.py
--rw-rw-rw-   0        0        0     2511 2023-08-01 02:26:06.000000 huhk-1.9.6/service/app_a/apis/apis_essay.py
--rw-rw-rw-   0        0        0     2187 2023-08-01 02:26:03.000000 huhk-1.9.6/service/app_a/apis/apis_testdrive.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.126036 huhk-1.9.6/service/app_a/apis/common/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:01.000000 huhk-1.9.6/service/app_a/apis/common/__init__.py
--rw-rw-rw-   0        0        0     1422 2023-08-01 02:26:01.000000 huhk-1.9.6/service/app_a/apis/common/apis_common_clue.py
--rw-rw-rw-   0        0        0     1071 2023-08-01 02:26:06.000000 huhk-1.9.6/service/app_a/apis/common/apis_common_common.py
--rw-rw-rw-   0        0        0     1945 2023-08-01 02:26:01.000000 huhk-1.9.6/service/app_a/apis/common/apis_common_remoteinterfacelog.py
--rw-rw-rw-   0        0        0     2922 2023-08-01 02:26:01.000000 huhk-1.9.6/service/app_a/apis/common/apis_common_systemversion.py
--rw-rw-rw-   0        0        0      867 2023-08-01 02:26:02.000000 huhk-1.9.6/service/app_a/apis/common/apis_common_user.py
--rw-rw-rw-   0        0        0    25061 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/apis/common/apis_common_user4c.py
--rw-rw-rw-   0        0        0     5938 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/apis/common/apis_common_userpointsmanage.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.175156 huhk-1.9.6/service/app_a/apis/content/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:01.000000 huhk-1.9.6/service/app_a/apis/content/__init__.py
--rw-rw-rw-   0        0        0    26441 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/apis/content/apis_content_activitymanager.py
--rw-rw-rw-   0        0        0    13587 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/apis/content/apis_content_adv.py
--rw-rw-rw-   0        0        0     1184 2023-08-01 02:26:06.000000 huhk-1.9.6/service/app_a/apis/content/apis_content_advplace.py
--rw-rw-rw-   0        0        0    10283 2023-08-01 02:26:06.000000 huhk-1.9.6/service/app_a/apis/content/apis_content_agreement.py
--rw-rw-rw-   0        0        0     8389 2023-08-01 02:26:01.000000 huhk-1.9.6/service/app_a/apis/content/apis_content_campmanager.py
--rw-rw-rw-   0        0        0     7639 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/apis/content/apis_content_comment.py
--rw-rw-rw-   0        0        0     8748 2023-08-01 02:26:06.000000 huhk-1.9.6/service/app_a/apis/content/apis_content_commonquestion.py
--rw-rw-rw-   0        0        0     1419 2023-08-01 02:26:06.000000 huhk-1.9.6/service/app_a/apis/content/apis_content_contentmanager.py
--rw-rw-rw-   0        0        0    14248 2023-08-01 02:26:07.000000 huhk-1.9.6/service/app_a/apis/content/apis_content_essay.py
--rw-rw-rw-   0        0        0     1317 2023-08-01 02:26:06.000000 huhk-1.9.6/service/app_a/apis/content/apis_content_essaycomment.py
--rw-rw-rw-   0        0        0     4566 2023-08-01 02:26:06.000000 huhk-1.9.6/service/app_a/apis/content/apis_content_essayweb.py
--rw-rw-rw-   0        0        0      859 2023-08-01 02:26:07.000000 huhk-1.9.6/service/app_a/apis/content/apis_content_hotcity.py
--rw-rw-rw-   0        0        0     2952 2023-08-01 02:26:07.000000 huhk-1.9.6/service/app_a/apis/content/apis_content_hotsearch.py
--rw-rw-rw-   0        0        0     6682 2023-08-01 02:26:07.000000 huhk-1.9.6/service/app_a/apis/content/apis_content_material.py
--rw-rw-rw-   0        0        0     9450 2023-08-01 02:26:03.000000 huhk-1.9.6/service/app_a/apis/content/apis_content_messagemanager.py
--rw-rw-rw-   0        0        0     3576 2023-08-01 02:26:03.000000 huhk-1.9.6/service/app_a/apis/content/apis_content_noticemanager.py
--rw-rw-rw-   0        0        0     5813 2023-08-01 02:26:07.000000 huhk-1.9.6/service/app_a/apis/content/apis_content_question.py
--rw-rw-rw-   0        0        0     2008 2023-08-01 02:26:06.000000 huhk-1.9.6/service/app_a/apis/content/apis_content_recruit.py
--rw-rw-rw-   0        0        0     5100 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/apis/content/apis_content_safecode.py
--rw-rw-rw-   0        0        0     9825 2023-08-01 02:26:07.000000 huhk-1.9.6/service/app_a/apis/content/apis_content_subject.py
--rw-rw-rw-   0        0        0     9388 2023-08-01 02:26:06.000000 huhk-1.9.6/service/app_a/apis/content/apis_content_subjectweb.py
--rw-rw-rw-   0        0        0     6365 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/apis/content/apis_content_topic4c.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.180116 huhk-1.9.6/service/app_a/apis/content/material/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/apis/content/material/__init__.py
--rw-rw-rw-   0        0        0     1474 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/apis/content/material/apis_content_material_getmateriallist.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.193117 huhk-1.9.6/service/app_a/apis/goods/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:01.000000 huhk-1.9.6/service/app_a/apis/goods/__init__.py
--rw-rw-rw-   0        0        0     9854 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/apis/goods/apis_goods_area.py
--rw-rw-rw-   0        0        0    12191 2023-08-01 02:26:05.000000 huhk-1.9.6/service/app_a/apis/goods/apis_goods_carmodel.py
--rw-rw-rw-   0        0        0    10643 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/apis/goods/apis_goods_configure.py
--rw-rw-rw-   0        0        0     6170 2023-08-01 02:26:03.000000 huhk-1.9.6/service/app_a/apis/goods/apis_goods_ordermain.py
--rw-rw-rw-   0        0        0     3147 2023-08-01 02:26:03.000000 huhk-1.9.6/service/app_a/apis/goods/apis_goods_testdrive.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.195076 huhk-1.9.6/service/app_a/apis/manageapi/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:04.000000 huhk-1.9.6/service/app_a/apis/manageapi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.200096 huhk-1.9.6/service/app_a/apis/manageapi/order/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:04.000000 huhk-1.9.6/service/app_a/apis/manageapi/order/__init__.py
--rw-rw-rw-   0        0        0     8140 2023-08-01 02:26:04.000000 huhk-1.9.6/service/app_a/apis/manageapi/order/apis_manageapi_order_mainorder.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.202093 huhk-1.9.6/service/app_a/apis/open/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:00.000000 huhk-1.9.6/service/app_a/apis/open/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.210071 huhk-1.9.6/service/app_a/apis/open/haohan/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:00.000000 huhk-1.9.6/service/app_a/apis/open/haohan/__init__.py
--rw-rw-rw-   0        0        0      816 2023-08-01 02:26:01.000000 huhk-1.9.6/service/app_a/apis/open/haohan/apis_open_haohan_relation.py
--rw-rw-rw-   0        0        0      849 2023-08-01 02:26:00.000000 huhk-1.9.6/service/app_a/apis/open/haohan/apis_open_haohan_rights.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.223002 huhk-1.9.6/service/app_a/apis/order/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:00.000000 huhk-1.9.6/service/app_a/apis/order/__init__.py
--rw-rw-rw-   0        0        0     2652 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/apis/order/apis_order_freeorder.py
--rw-rw-rw-   0        0        0    23046 2023-08-01 02:26:04.000000 huhk-1.9.6/service/app_a/apis/order/apis_order_mainorder.py
--rw-rw-rw-   0        0        0     3724 2023-08-01 02:26:03.000000 huhk-1.9.6/service/app_a/apis/order/apis_order_order.py
--rw-rw-rw-   0        0        0    11987 2023-08-01 02:26:04.000000 huhk-1.9.6/service/app_a/apis/order/apis_order_rightsorder.py
--rw-rw-rw-   0        0        0     2582 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/apis/order/apis_order_testdrive.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.228016 huhk-1.9.6/service/app_a/apis/order/mainorder/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:04.000000 huhk-1.9.6/service/app_a/apis/order/mainorder/__init__.py
--rw-rw-rw-   0        0        0     1125 2023-08-01 02:26:04.000000 huhk-1.9.6/service/app_a/apis/order/mainorder/apis_order_mainorder_scrm2app.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.232976 huhk-1.9.6/service/app_a/apis/order/rights/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:04.000000 huhk-1.9.6/service/app_a/apis/order/rights/__init__.py
--rw-rw-rw-   0        0        0    10735 2023-08-01 02:26:04.000000 huhk-1.9.6/service/app_a/apis/order/rights/apis_order_rights_rightsmanager.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.237988 huhk-1.9.6/service/app_a/apis/order/rightsorder/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:04.000000 huhk-1.9.6/service/app_a/apis/order/rightsorder/__init__.py
--rw-rw-rw-   0        0        0     2379 2023-08-01 02:26:04.000000 huhk-1.9.6/service/app_a/apis/order/rightsorder/apis_order_rightsorder_receive.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.242976 huhk-1.9.6/service/app_a/apis/pay/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:03.000000 huhk-1.9.6/service/app_a/apis/pay/__init__.py
--rw-rw-rw-   0        0        0      865 2023-08-01 02:26:03.000000 huhk-1.9.6/service/app_a/apis/pay/apis_pay_orderpaybill.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.256456 huhk-1.9.6/service/app_a/apis/radarpoints/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:02.000000 huhk-1.9.6/service/app_a/apis/radarpoints/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.258036 huhk-1.9.6/service/app_a/apis/radarpoints/adjustpoints/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:03.000000 huhk-1.9.6/service/app_a/apis/radarpoints/adjustpoints/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.266044 huhk-1.9.6/service/app_a/apis/radarpoints/adjustpoints/adjust/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:03.000000 huhk-1.9.6/service/app_a/apis/radarpoints/adjustpoints/adjust/__init__.py
--rw-rw-rw-   0        0        0     3883 2023-08-01 02:26:03.000000 huhk-1.9.6/service/app_a/apis/radarpoints/adjustpoints/adjust/apis_radarpoints_adjustpoints_adjust_batch.py
--rw-rw-rw-   0        0        0     1699 2023-08-01 02:26:03.000000 huhk-1.9.6/service/app_a/apis/radarpoints/adjustpoints/adjust/apis_radarpoints_adjustpoints_adjust_single.py
--rw-rw-rw-   0        0        0     6180 2023-08-01 02:26:03.000000 huhk-1.9.6/service/app_a/apis/radarpoints/apis_radarpoints_adjustpoints.py
--rw-rw-rw-   0        0        0     7225 2023-08-01 02:26:02.000000 huhk-1.9.6/service/app_a/apis/radarpoints/apis_radarpoints_pointsconfig.py
--rw-rw-rw-   0        0        0     3763 2023-08-01 02:26:02.000000 huhk-1.9.6/service/app_a/apis/radarpoints/apis_radarpoints_pointstask.py
--rw-rw-rw-   0        0        0     2247 2023-08-01 02:26:03.000000 huhk-1.9.6/service/app_a/apis/radarpoints/apis_radarpoints_summarystatistics.py
--rw-rw-rw-   0        0        0     6270 2023-08-01 02:26:03.000000 huhk-1.9.6/service/app_a/apis/radarpoints/apis_radarpoints_userpoints.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.273594 huhk-1.9.6/service/app_a/apis/radarpoints/userpoints/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:02.000000 huhk-1.9.6/service/app_a/apis/radarpoints/userpoints/__init__.py
--rw-rw-rw-   0        0        0     1871 2023-08-01 02:26:02.000000 huhk-1.9.6/service/app_a/apis/radarpoints/userpoints/apis_radarpoints_userpoints_exchangeinfo.py
--rw-rw-rw-   0        0        0     2061 2023-08-01 02:26:02.000000 huhk-1.9.6/service/app_a/apis/radarpoints/userpoints/apis_radarpoints_userpoints_pointsinfo.py
--rw-rw-rw-   0        0        0      752 2023-08-01 02:26:00.000000 huhk-1.9.6/service/app_a/app_a_fun.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.288596 huhk-1.9.6/service/app_a/asserts/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:00.000000 huhk-1.9.6/service/app_a/asserts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.295539 huhk-1.9.6/service/app_a/asserts/admin/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/asserts/admin/__init__.py
--rw-rw-rw-   0        0        0      941 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/asserts/admin/asserts_admin_guc.py
--rw-rw-rw-   0        0        0      552 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/asserts/admin/asserts_admin_spa.py
--rw-rw-rw-   0        0        0      626 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/asserts/asserts_activitymanager.py
--rw-rw-rw-   0        0        0      653 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/asserts/asserts_app_a.py
--rw-rw-rw-   0        0        0      525 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/asserts/asserts_area.py
--rw-rw-rw-   0        0        0      536 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/asserts/asserts_content.py
--rw-rw-rw-   0        0        0     1009 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/asserts/asserts_essay.py
--rw-rw-rw-   0        0        0      707 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/asserts/asserts_testdrive.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.320474 huhk-1.9.6/service/app_a/asserts/common/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/asserts/common/__init__.py
--rw-rw-rw-   0        0        0      587 2023-08-01 02:26:09.000000 huhk-1.9.6/service/app_a/asserts/common/asserts_common_clue.py
--rw-rw-rw-   0        0        0      581 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/asserts/common/asserts_common_common.py
--rw-rw-rw-   0        0        0      714 2023-08-01 02:26:09.000000 huhk-1.9.6/service/app_a/asserts/common/asserts_common_remoteinterfacelog.py
--rw-rw-rw-   0        0        0     1116 2023-08-01 02:26:09.000000 huhk-1.9.6/service/app_a/asserts/common/asserts_common_systemversion.py
--rw-rw-rw-   0        0        0      579 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/asserts/common/asserts_common_user.py
--rw-rw-rw-   0        0        0     6848 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/asserts/common/asserts_common_user4c.py
--rw-rw-rw-   0        0        0     2174 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/asserts/common/asserts_common_userpointsmanage.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.381025 huhk-1.9.6/service/app_a/asserts/content/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/asserts/content/__init__.py
--rw-rw-rw-   0        0        0     7782 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/asserts/content/asserts_content_activitymanager.py
--rw-rw-rw-   0        0        0     5226 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/asserts/content/asserts_content_adv.py
--rw-rw-rw-   0        0        0      653 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/asserts/content/asserts_content_advplace.py
--rw-rw-rw-   0        0        0     3600 2023-08-01 02:26:12.000000 huhk-1.9.6/service/app_a/asserts/content/asserts_content_agreement.py
--rw-rw-rw-   0        0        0     2959 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/asserts/content/asserts_content_campmanager.py
--rw-rw-rw-   0        0        0     2532 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/asserts/content/asserts_content_comment.py
--rw-rw-rw-   0        0        0     4032 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/asserts/content/asserts_content_commonquestion.py
--rw-rw-rw-   0        0        0      649 2023-08-01 02:26:12.000000 huhk-1.9.6/service/app_a/asserts/content/asserts_content_contentmanager.py
--rw-rw-rw-   0        0        0     4302 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/asserts/content/asserts_content_essay.py
--rw-rw-rw-   0        0        0      664 2023-08-01 02:26:12.000000 huhk-1.9.6/service/app_a/asserts/content/asserts_content_essaycomment.py
--rw-rw-rw-   0        0        0     1937 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/asserts/content/asserts_content_essayweb.py
--rw-rw-rw-   0        0        0      582 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/asserts/content/asserts_content_hotcity.py
--rw-rw-rw-   0        0        0     1432 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/asserts/content/asserts_content_hotsearch.py
--rw-rw-rw-   0        0        0     3121 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/asserts/content/asserts_content_material.py
--rw-rw-rw-   0        0        0     3611 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/asserts/content/asserts_content_messagemanager.py
--rw-rw-rw-   0        0        0     1560 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/asserts/content/asserts_content_noticemanager.py
--rw-rw-rw-   0        0        0     1960 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/asserts/content/asserts_content_question.py
--rw-rw-rw-   0        0        0      998 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/asserts/content/asserts_content_recruit.py
--rw-rw-rw-   0        0        0     2216 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/asserts/content/asserts_content_safecode.py
--rw-rw-rw-   0        0        0     3677 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/asserts/content/asserts_content_subject.py
--rw-rw-rw-   0        0        0     3368 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/asserts/content/asserts_content_subjectweb.py
--rw-rw-rw-   0        0        0     2290 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/asserts/content/asserts_content_topic4c.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.386551 huhk-1.9.6/service/app_a/asserts/content/material/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/asserts/content/material/__init__.py
--rw-rw-rw-   0        0        0      717 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/asserts/content/material/asserts_content_material_getmateriallist.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.400514 huhk-1.9.6/service/app_a/asserts/goods/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:09.000000 huhk-1.9.6/service/app_a/asserts/goods/__init__.py
--rw-rw-rw-   0        0        0     3466 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/asserts/goods/asserts_goods_area.py
--rw-rw-rw-   0        0        0     3208 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/asserts/goods/asserts_goods_carmodel.py
--rw-rw-rw-   0        0        0     2408 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/asserts/goods/asserts_goods_configure.py
--rw-rw-rw-   0        0        0     2048 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/asserts/goods/asserts_goods_ordermain.py
--rw-rw-rw-   0        0        0     1164 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/asserts/goods/asserts_goods_testdrive.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.402508 huhk-1.9.6/service/app_a/asserts/manageapi/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/asserts/manageapi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.408493 huhk-1.9.6/service/app_a/asserts/manageapi/order/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/asserts/manageapi/order/__init__.py
--rw-rw-rw-   0        0        0     1277 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/asserts/manageapi/order/asserts_manageapi_order_mainorder.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.410487 huhk-1.9.6/service/app_a/asserts/open/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/asserts/open/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.418466 huhk-1.9.6/service/app_a/asserts/open/haohan/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/asserts/open/haohan/__init__.py
--rw-rw-rw-   0        0        0      625 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/asserts/open/haohan/asserts_open_haohan_relation.py
--rw-rw-rw-   0        0        0      613 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/asserts/open/haohan/asserts_open_haohan_rights.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.432940 huhk-1.9.6/service/app_a/asserts/order/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/asserts/order/__init__.py
--rw-rw-rw-   0        0        0      824 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/asserts/order/asserts_order_freeorder.py
--rw-rw-rw-   0        0        0     7067 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/asserts/order/asserts_order_mainorder.py
--rw-rw-rw-   0        0        0     1428 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/asserts/order/asserts_order_order.py
--rw-rw-rw-   0        0        0     3268 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/asserts/order/asserts_order_rightsorder.py
--rw-rw-rw-   0        0        0     1108 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/asserts/order/asserts_order_testdrive.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.437927 huhk-1.9.6/service/app_a/asserts/order/mainorder/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/asserts/order/mainorder/__init__.py
--rw-rw-rw-   0        0        0      704 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/asserts/order/mainorder/asserts_order_mainorder_scrm2app.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.443910 huhk-1.9.6/service/app_a/asserts/order/rights/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/asserts/order/rights/__init__.py
--rw-rw-rw-   0        0        0     3944 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/asserts/order/rights/asserts_order_rights_rightsmanager.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.449898 huhk-1.9.6/service/app_a/asserts/order/rightsorder/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/asserts/order/rightsorder/__init__.py
--rw-rw-rw-   0        0        0      890 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/asserts/order/rightsorder/asserts_order_rightsorder_receive.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.456884 huhk-1.9.6/service/app_a/asserts/pay/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/asserts/pay/__init__.py
--rw-rw-rw-   0        0        0      611 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/asserts/pay/asserts_pay_orderpaybill.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.472840 huhk-1.9.6/service/app_a/asserts/radarpoints/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/asserts/radarpoints/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.475859 huhk-1.9.6/service/app_a/asserts/radarpoints/adjustpoints/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/asserts/radarpoints/adjustpoints/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.484462 huhk-1.9.6/service/app_a/asserts/radarpoints/adjustpoints/adjust/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/asserts/radarpoints/adjustpoints/adjust/__init__.py
--rw-rw-rw-   0        0        0     1319 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/asserts/radarpoints/adjustpoints/adjust/asserts_radarpoints_adjustpoints_adjust_batch.py
--rw-rw-rw-   0        0        0      817 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/asserts/radarpoints/adjustpoints/adjust/asserts_radarpoints_adjustpoints_adjust_single.py
--rw-rw-rw-   0        0        0     2203 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/asserts/radarpoints/asserts_radarpoints_adjustpoints.py
--rw-rw-rw-   0        0        0     2272 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/asserts/radarpoints/asserts_radarpoints_pointsconfig.py
--rw-rw-rw-   0        0        0     1275 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/asserts/radarpoints/asserts_radarpoints_pointstask.py
--rw-rw-rw-   0        0        0     1163 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/asserts/radarpoints/asserts_radarpoints_summarystatistics.py
--rw-rw-rw-   0        0        0     1660 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/asserts/radarpoints/asserts_radarpoints_userpoints.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.492440 huhk-1.9.6/service/app_a/asserts/radarpoints/userpoints/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/asserts/radarpoints/userpoints/__init__.py
--rw-rw-rw-   0        0        0      807 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/asserts/radarpoints/userpoints/asserts_radarpoints_userpoints_exchangeinfo.py
--rw-rw-rw-   0        0        0      783 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/asserts/radarpoints/userpoints/asserts_radarpoints_userpoints_pointsinfo.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.529884 huhk-1.9.6/service/app_a/funs/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:00.000000 huhk-1.9.6/service/app_a/funs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.537864 huhk-1.9.6/service/app_a/funs/admin/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/funs/admin/__init__.py
--rw-rw-rw-   0        0        0     1065 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/funs/admin/funs_admin_guc.py
--rw-rw-rw-   0        0        0      647 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/funs/admin/funs_admin_spa.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.561359 huhk-1.9.6/service/app_a/funs/common/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/funs/common/__init__.py
--rw-rw-rw-   0        0        0      928 2023-08-01 02:26:09.000000 huhk-1.9.6/service/app_a/funs/common/funs_common_clue.py
--rw-rw-rw-   0        0        0      709 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/funs/common/funs_common_common.py
--rw-rw-rw-   0        0        0     1795 2023-08-01 02:26:09.000000 huhk-1.9.6/service/app_a/funs/common/funs_common_remoteinterfacelog.py
--rw-rw-rw-   0        0        0     2804 2023-08-01 02:26:09.000000 huhk-1.9.6/service/app_a/funs/common/funs_common_systemversion.py
--rw-rw-rw-   0        0        0      729 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/funs/common/funs_common_user.py
--rw-rw-rw-   0        0        0    21622 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/funs/common/funs_common_user4c.py
--rw-rw-rw-   0        0        0     6180 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/funs/common/funs_common_userpointsmanage.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.615184 huhk-1.9.6/service/app_a/funs/content/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/funs/content/__init__.py
--rw-rw-rw-   0        0        0    26429 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/funs/content/funs_content_activitymanager.py
--rw-rw-rw-   0        0        0    11631 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/funs/content/funs_content_adv.py
--rw-rw-rw-   0        0        0     1482 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/funs/content/funs_content_advplace.py
--rw-rw-rw-   0        0        0     7550 2023-08-01 02:26:12.000000 huhk-1.9.6/service/app_a/funs/content/funs_content_agreement.py
--rw-rw-rw-   0        0        0     8084 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/funs/content/funs_content_campmanager.py
--rw-rw-rw-   0        0        0     7904 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/funs/content/funs_content_comment.py
--rw-rw-rw-   0        0        0     7209 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/funs/content/funs_content_commonquestion.py
--rw-rw-rw-   0        0        0     1082 2023-08-01 02:26:12.000000 huhk-1.9.6/service/app_a/funs/content/funs_content_contentmanager.py
--rw-rw-rw-   0        0        0    13476 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/funs/content/funs_content_essay.py
--rw-rw-rw-   0        0        0     1526 2023-08-01 02:26:12.000000 huhk-1.9.6/service/app_a/funs/content/funs_content_essaycomment.py
--rw-rw-rw-   0        0        0     4715 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/funs/content/funs_content_essayweb.py
--rw-rw-rw-   0        0        0      694 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/funs/content/funs_content_hotcity.py
--rw-rw-rw-   0        0        0     2656 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/funs/content/funs_content_hotsearch.py
--rw-rw-rw-   0        0        0     5431 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/funs/content/funs_content_material.py
--rw-rw-rw-   0        0        0    10631 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/funs/content/funs_content_messagemanager.py
--rw-rw-rw-   0        0        0     2868 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/funs/content/funs_content_noticemanager.py
--rw-rw-rw-   0        0        0     4376 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/funs/content/funs_content_question.py
--rw-rw-rw-   0        0        0     1529 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/funs/content/funs_content_recruit.py
--rw-rw-rw-   0        0        0     3317 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/funs/content/funs_content_safecode.py
--rw-rw-rw-   0        0        0     8951 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/funs/content/funs_content_subject.py
--rw-rw-rw-   0        0        0     9433 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/funs/content/funs_content_subjectweb.py
--rw-rw-rw-   0        0        0     4900 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/funs/content/funs_content_topic4c.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.620173 huhk-1.9.6/service/app_a/funs/content/material/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/funs/content/material/__init__.py
--rw-rw-rw-   0        0        0     1219 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/funs/content/material/funs_content_material_getmateriallist.py
--rw-rw-rw-   0        0        0     1130 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/funs/funs_activitymanager.py
--rw-rw-rw-   0        0        0      194 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/funs/funs_admin.py
--rw-rw-rw-   0        0        0     3167 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/funs/funs_app_a.py
--rw-rw-rw-   0        0        0      599 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/funs/funs_area.py
--rw-rw-rw-   0        0        0      761 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/funs/funs_common.py
--rw-rw-rw-   0        0        0     3099 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/funs/funs_content.py
--rw-rw-rw-   0        0        0     2527 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/funs/funs_essay.py
--rw-rw-rw-   0        0        0      506 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/funs/funs_goods.py
--rw-rw-rw-   0        0        0      140 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/funs/funs_manageapi.py
--rw-rw-rw-   0        0        0      118 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/funs/funs_open.py
--rw-rw-rw-   0        0        0      607 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/funs/funs_order.py
--rw-rw-rw-   0        0        0      131 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/funs/funs_pay.py
--rw-rw-rw-   0        0        0      698 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/funs/funs_radarpoints.py
--rw-rw-rw-   0        0        0     2813 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/funs/funs_testdrive.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.637124 huhk-1.9.6/service/app_a/funs/goods/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:09.000000 huhk-1.9.6/service/app_a/funs/goods/__init__.py
--rw-rw-rw-   0        0        0     6559 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/funs/goods/funs_goods_area.py
--rw-rw-rw-   0        0        0    11252 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/funs/goods/funs_goods_carmodel.py
--rw-rw-rw-   0        0        0    10293 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/funs/goods/funs_goods_configure.py
--rw-rw-rw-   0        0        0     5322 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/funs/goods/funs_goods_ordermain.py
--rw-rw-rw-   0        0        0     3626 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/funs/goods/funs_goods_testdrive.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.643109 huhk-1.9.6/service/app_a/funs/manageapi/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/funs/manageapi/__init__.py
--rw-rw-rw-   0        0        0      179 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/funs/manageapi/funs_manageapi_order.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.648097 huhk-1.9.6/service/app_a/funs/manageapi/order/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/funs/manageapi/order/__init__.py
--rw-rw-rw-   0        0        0     4282 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/funs/manageapi/order/funs_manageapi_order_mainorder.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.654014 huhk-1.9.6/service/app_a/funs/open/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/funs/open/__init__.py
--rw-rw-rw-   0        0        0      267 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/funs/open/funs_open_haohan.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.661992 huhk-1.9.6/service/app_a/funs/open/haohan/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/funs/open/haohan/__init__.py
--rw-rw-rw-   0        0        0      869 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/funs/open/haohan/funs_open_haohan_relation.py
--rw-rw-rw-   0        0        0      959 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/funs/open/haohan/funs_open_haohan_rights.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.679945 huhk-1.9.6/service/app_a/funs/order/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/funs/order/__init__.py
--rw-rw-rw-   0        0        0     3970 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/funs/order/funs_order_freeorder.py
--rw-rw-rw-   0        0        0    19335 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/funs/order/funs_order_mainorder.py
--rw-rw-rw-   0        0        0     2770 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/funs/order/funs_order_order.py
--rw-rw-rw-   0        0        0      176 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/funs/order/funs_order_rights.py
--rw-rw-rw-   0        0        0    12237 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/funs/order/funs_order_rightsorder.py
--rw-rw-rw-   0        0        0     2884 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/funs/order/funs_order_testdrive.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.684930 huhk-1.9.6/service/app_a/funs/order/mainorder/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/funs/order/mainorder/__init__.py
--rw-rw-rw-   0        0        0     1373 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/funs/order/mainorder/funs_order_mainorder_scrm2app.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.690915 huhk-1.9.6/service/app_a/funs/order/rights/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/funs/order/rights/__init__.py
--rw-rw-rw-   0        0        0     9168 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/funs/order/rights/funs_order_rights_rightsmanager.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.695903 huhk-1.9.6/service/app_a/funs/order/rightsorder/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/funs/order/rightsorder/__init__.py
--rw-rw-rw-   0        0        0     3959 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/funs/order/rightsorder/funs_order_rightsorder_receive.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.701552 huhk-1.9.6/service/app_a/funs/pay/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/funs/pay/__init__.py
--rw-rw-rw-   0        0        0      900 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/funs/pay/funs_pay_orderpaybill.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.717240 huhk-1.9.6/service/app_a/funs/radarpoints/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/funs/radarpoints/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.721950 huhk-1.9.6/service/app_a/funs/radarpoints/adjustpoints/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/funs/radarpoints/adjustpoints/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.730537 huhk-1.9.6/service/app_a/funs/radarpoints/adjustpoints/adjust/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/funs/radarpoints/adjustpoints/adjust/__init__.py
--rw-rw-rw-   0        0        0     4080 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/funs/radarpoints/adjustpoints/adjust/funs_radarpoints_adjustpoints_adjust_batch.py
--rw-rw-rw-   0        0        0     2099 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/funs/radarpoints/adjustpoints/adjust/funs_radarpoints_adjustpoints_adjust_single.py
--rw-rw-rw-   0        0        0      433 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/funs/radarpoints/adjustpoints/funs_radarpoints_adjustpoints_adjust.py
--rw-rw-rw-   0        0        0     5930 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/funs/radarpoints/funs_radarpoints_adjustpoints.py
--rw-rw-rw-   0        0        0     8017 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/funs/radarpoints/funs_radarpoints_pointsconfig.py
--rw-rw-rw-   0        0        0     4126 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/funs/radarpoints/funs_radarpoints_pointstask.py
--rw-rw-rw-   0        0        0     2339 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/funs/radarpoints/funs_radarpoints_summarystatistics.py
--rw-rw-rw-   0        0        0     7881 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/funs/radarpoints/funs_radarpoints_userpoints.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.737517 huhk-1.9.6/service/app_a/funs/radarpoints/userpoints/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/funs/radarpoints/userpoints/__init__.py
--rw-rw-rw-   0        0        0     2066 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/funs/radarpoints/userpoints/funs_radarpoints_userpoints_exchangeinfo.py
--rw-rw-rw-   0        0        0     2169 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/funs/radarpoints/userpoints/funs_radarpoints_userpoints_pointsinfo.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.754445 huhk-1.9.6/service/app_a/sqls/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:00.000000 huhk-1.9.6/service/app_a/sqls/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.762423 huhk-1.9.6/service/app_a/sqls/admin/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/sqls/admin/__init__.py
--rw-rw-rw-   0        0        0     1026 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/sqls/admin/sqls_admin_guc.py
--rw-rw-rw-   0        0        0      552 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/sqls/admin/sqls_admin_spa.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.781401 huhk-1.9.6/service/app_a/sqls/common/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/sqls/common/__init__.py
--rw-rw-rw-   0        0        0      563 2023-08-01 02:26:09.000000 huhk-1.9.6/service/app_a/sqls/common/sqls_common_clue.py
--rw-rw-rw-   0        0        0      562 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/sqls/common/sqls_common_common.py
--rw-rw-rw-   0        0        0      586 2023-08-01 02:26:09.000000 huhk-1.9.6/service/app_a/sqls/common/sqls_common_remoteinterfacelog.py
--rw-rw-rw-   0        0        0     1050 2023-08-01 02:26:09.000000 huhk-1.9.6/service/app_a/sqls/common/sqls_common_systemversion.py
--rw-rw-rw-   0        0        0      563 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/sqls/common/sqls_common_user.py
--rw-rw-rw-   0        0        0     6794 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/sqls/common/sqls_common_user4c.py
--rw-rw-rw-   0        0        0     2069 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/sqls/common/sqls_common_userpointsmanage.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.834628 huhk-1.9.6/service/app_a/sqls/content/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/sqls/content/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.841580 huhk-1.9.6/service/app_a/sqls/content/material/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/sqls/content/material/__init__.py
--rw-rw-rw-   0        0        0      602 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/sqls/content/material/sqls_content_material_getmateriallist.py
--rw-rw-rw-   0        0        0     7456 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/sqls/content/sqls_content_activitymanager.py
--rw-rw-rw-   0        0        0     5815 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/sqls/content/sqls_content_adv.py
--rw-rw-rw-   0        0        0      568 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/sqls/content/sqls_content_advplace.py
--rw-rw-rw-   0        0        0     3943 2023-08-01 02:26:12.000000 huhk-1.9.6/service/app_a/sqls/content/sqls_content_agreement.py
--rw-rw-rw-   0        0        0     2981 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/sqls/content/sqls_content_campmanager.py
--rw-rw-rw-   0        0        0     2480 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/sqls/content/sqls_content_comment.py
--rw-rw-rw-   0        0        0     4458 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/sqls/content/sqls_content_commonquestion.py
--rw-rw-rw-   0        0        0      581 2023-08-01 02:26:12.000000 huhk-1.9.6/service/app_a/sqls/content/sqls_content_contentmanager.py
--rw-rw-rw-   0        0        0     4379 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/sqls/content/sqls_content_essay.py
--rw-rw-rw-   0        0        0      575 2023-08-01 02:26:12.000000 huhk-1.9.6/service/app_a/sqls/content/sqls_content_essaycomment.py
--rw-rw-rw-   0        0        0     2002 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/sqls/content/sqls_content_essayweb.py
--rw-rw-rw-   0        0        0      560 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/sqls/content/sqls_content_hotcity.py
--rw-rw-rw-   0        0        0     1520 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/sqls/content/sqls_content_hotsearch.py
--rw-rw-rw-   0        0        0     3466 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/sqls/content/sqls_content_material.py
--rw-rw-rw-   0        0        0     3504 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/sqls/content/sqls_content_messagemanager.py
--rw-rw-rw-   0        0        0     1564 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/sqls/content/sqls_content_noticemanager.py
--rw-rw-rw-   0        0        0     2022 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/sqls/content/sqls_content_question.py
--rw-rw-rw-   0        0        0     1037 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/sqls/content/sqls_content_recruit.py
--rw-rw-rw-   0        0        0     2474 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/sqls/content/sqls_content_safecode.py
--rw-rw-rw-   0        0        0     3917 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/sqls/content/sqls_content_subject.py
--rw-rw-rw-   0        0        0     3455 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/sqls/content/sqls_content_subjectweb.py
--rw-rw-rw-   0        0        0     2470 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/sqls/content/sqls_content_topic4c.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.856576 huhk-1.9.6/service/app_a/sqls/goods/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:09.000000 huhk-1.9.6/service/app_a/sqls/goods/__init__.py
--rw-rw-rw-   0        0        0     3904 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/sqls/goods/sqls_goods_area.py
--rw-rw-rw-   0        0        0     3000 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/sqls/goods/sqls_goods_carmodel.py
--rw-rw-rw-   0        0        0     2521 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/sqls/goods/sqls_goods_configure.py
--rw-rw-rw-   0        0        0     2016 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/sqls/goods/sqls_goods_ordermain.py
--rw-rw-rw-   0        0        0     1043 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/sqls/goods/sqls_goods_testdrive.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.858536 huhk-1.9.6/service/app_a/sqls/manageapi/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/sqls/manageapi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.865518 huhk-1.9.6/service/app_a/sqls/manageapi/order/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/sqls/manageapi/order/__init__.py
--rw-rw-rw-   0        0        0     1070 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/sqls/manageapi/order/sqls_manageapi_order_mainorder.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.868512 huhk-1.9.6/service/app_a/sqls/open/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/sqls/open/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.876523 huhk-1.9.6/service/app_a/sqls/open/haohan/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/sqls/open/haohan/__init__.py
--rw-rw-rw-   0        0        0      571 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/sqls/open/haohan/sqls_open_haohan_relation.py
--rw-rw-rw-   0        0        0      567 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/sqls/open/haohan/sqls_open_haohan_rights.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.891482 huhk-1.9.6/service/app_a/sqls/order/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:08.000000 huhk-1.9.6/service/app_a/sqls/order/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.896435 huhk-1.9.6/service/app_a/sqls/order/mainorder/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/sqls/order/mainorder/__init__.py
--rw-rw-rw-   0        0        0      590 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/sqls/order/mainorder/sqls_order_mainorder_scrm2app.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.901429 huhk-1.9.6/service/app_a/sqls/order/rights/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/sqls/order/rights/__init__.py
--rw-rw-rw-   0        0        0     4025 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/sqls/order/rights/sqls_order_rights_rightsmanager.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.906411 huhk-1.9.6/service/app_a/sqls/order/rightsorder/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/sqls/order/rightsorder/__init__.py
--rw-rw-rw-   0        0        0      581 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/sqls/order/rightsorder/sqls_order_rightsorder_receive.py
--rw-rw-rw-   0        0        0      564 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/sqls/order/sqls_order_freeorder.py
--rw-rw-rw-   0        0        0     7363 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/sqls/order/sqls_order_mainorder.py
--rw-rw-rw-   0        0        0     1511 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/sqls/order/sqls_order_order.py
--rw-rw-rw-   0        0        0     2972 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/sqls/order/sqls_order_rightsorder.py
--rw-rw-rw-   0        0        0     1045 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/sqls/order/sqls_order_testdrive.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.911399 huhk-1.9.6/service/app_a/sqls/pay/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/sqls/pay/__init__.py
--rw-rw-rw-   0        0        0      569 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/sqls/pay/sqls_pay_orderpaybill.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.925985 huhk-1.9.6/service/app_a/sqls/radarpoints/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/sqls/radarpoints/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.927979 huhk-1.9.6/service/app_a/sqls/radarpoints/adjustpoints/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/sqls/radarpoints/adjustpoints/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.936516 huhk-1.9.6/service/app_a/sqls/radarpoints/adjustpoints/adjust/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/sqls/radarpoints/adjustpoints/adjust/__init__.py
--rw-rw-rw-   0        0        0     1101 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/sqls/radarpoints/adjustpoints/adjust/sqls_radarpoints_adjustpoints_adjust_batch.py
--rw-rw-rw-   0        0        0      604 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/sqls/radarpoints/adjustpoints/adjust/sqls_radarpoints_adjustpoints_adjust_single.py
--rw-rw-rw-   0        0        0     2076 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/sqls/radarpoints/sqls_radarpoints_adjustpoints.py
--rw-rw-rw-   0        0        0     2046 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/sqls/radarpoints/sqls_radarpoints_pointsconfig.py
--rw-rw-rw-   0        0        0     1062 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/sqls/radarpoints/sqls_radarpoints_pointstask.py
--rw-rw-rw-   0        0        0     1083 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/sqls/radarpoints/sqls_radarpoints_summarystatistics.py
--rw-rw-rw-   0        0        0     1062 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/sqls/radarpoints/sqls_radarpoints_userpoints.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.943498 huhk-1.9.6/service/app_a/sqls/radarpoints/userpoints/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/sqls/radarpoints/userpoints/__init__.py
--rw-rw-rw-   0        0        0      603 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/sqls/radarpoints/userpoints/sqls_radarpoints_userpoints_exchangeinfo.py
--rw-rw-rw-   0        0        0      599 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/sqls/radarpoints/userpoints/sqls_radarpoints_userpoints_pointsinfo.py
--rw-rw-rw-   0        0        0      574 2023-08-01 02:26:10.000000 huhk-1.9.6/service/app_a/sqls/sqls_activitymanager.py
--rw-rw-rw-   0        0        0      534 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/sqls/sqls_app_a.py
--rw-rw-rw-   0        0        0      546 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/sqls/sqls_area.py
--rw-rw-rw-   0        0        0      545 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/sqls/sqls_content.py
--rw-rw-rw-   0        0        0     1017 2023-08-01 02:26:13.000000 huhk-1.9.6/service/app_a/sqls/sqls_essay.py
--rw-rw-rw-   0        0        0      554 2023-08-01 02:26:11.000000 huhk-1.9.6/service/app_a/sqls/sqls_testdrive.py
--rw-rw-rw-   0        0        0       42 2023-08-01 02:51:39.957186 huhk-1.9.6/setup.cfg
--rw-rw-rw-   0        0        0        2 2023-07-03 11:51:22.000000 huhk-1.9.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.945454 huhk-1.9.6/testcase/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:00.000000 huhk-1.9.6/testcase/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:51:39.953365 huhk-1.9.6/testcase/app_a/
--rw-rw-rw-   0        0        0        0 2023-08-01 02:26:00.000000 huhk-1.9.6/testcase/app_a/__init__.py
--rw-rw-rw-   0        0        0      361 2023-08-01 02:26:00.000000 huhk-1.9.6/testcase/app_a/conftest.py
--rw-rw-rw-   0        0        0     3184 2023-08-01 02:26:13.000000 huhk-1.9.6/testcase/app_a/test_page.py
+drwxrwxrwx   0        0        0        0 2023-08-04 06:33:09.486734 huhk-1.9.7/
+-rw-rw-rw-   0        0        0      223 2023-08-04 06:33:09.485739 huhk-1.9.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-04 06:33:09.383516 huhk-1.9.7/huhk/
+-rw-rw-rw-   0        0        0      772 2023-07-17 02:44:39.000000 huhk-1.9.7/huhk/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-04 06:33:09.425403 huhk-1.9.7/huhk/case_project/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.9.7/huhk/case_project/__init__.py
+-rw-rw-rw-   0        0        0      639 2023-07-12 01:13:24.000000 huhk-1.9.7/huhk/case_project/json_coder.py
+-rw-rw-rw-   0        0        0     3253 2023-08-04 01:52:31.000000 huhk-1.9.7/huhk/case_project/main_fun.py
+-rw-rw-rw-   0        0        0    21477 2023-08-04 01:53:28.000000 huhk-1.9.7/huhk/case_project/project_base.py
+-rw-rw-rw-   0        0        0     1359 2023-08-04 01:36:40.000000 huhk-1.9.7/huhk/case_project/project_init.py
+-rw-rw-rw-   0        0        0    18564 2023-08-04 01:53:28.000000 huhk-1.9.7/huhk/case_project/project_string.py
+-rw-rw-rw-   0        0        0     1110 2023-08-04 02:28:29.000000 huhk-1.9.7/huhk/case_project/setup_set.py
+-rw-rw-rw-   0        0        0       17 2023-08-04 06:33:08.000000 huhk-1.9.7/huhk/case_project/version.py
+-rw-rw-rw-   0        0        0     9864 2023-08-04 01:53:28.000000 huhk-1.9.7/huhk/init_project.py
+-rw-rw-rw-   0        0        0     1277 2023-08-04 01:51:34.000000 huhk-1.9.7/huhk/main.py
+-rw-rw-rw-   0        0        0      338 2023-08-04 06:33:00.000000 huhk-1.9.7/huhk/setup_run.py
+drwxrwxrwx   0        0        0        0 2023-08-04 06:33:09.428395 huhk-1.9.7/huhk/testcase/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.9.7/huhk/testcase/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-04 06:33:09.479752 huhk-1.9.7/huhk/testcase/apache/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.9.7/huhk/testcase/apache/__init__.py
+-rw-rw-rw-   0        0        0     3355 2023-07-12 01:13:24.000000 huhk-1.9.7/huhk/testcase/apache/beam_class.py
+-rw-rw-rw-   0        0        0     5523 2023-07-12 02:37:05.000000 huhk-1.9.7/huhk/testcase/apache/data.py
+-rw-rw-rw-   0        0        0     1764 2023-07-12 01:13:24.000000 huhk-1.9.7/huhk/testcase/apache/par_do.py
+-rw-rw-rw-   0        0        0     7252 2023-08-04 01:32:03.000000 huhk-1.9.7/huhk/testcase/apache/test_cogroupbykey.py
+-rw-rw-rw-   0        0        0      471 2023-08-04 01:32:02.000000 huhk-1.9.7/huhk/testcase/apache/test_file.py
+-rw-rw-rw-   0        0        0     1498 2023-08-04 01:32:02.000000 huhk-1.9.7/huhk/testcase/apache/test_fiter.py
+-rw-rw-rw-   0        0        0     2098 2023-08-04 01:32:03.000000 huhk-1.9.7/huhk/testcase/apache/test_flatmap.py
+-rw-rw-rw-   0        0        0      518 2023-08-04 01:32:03.000000 huhk-1.9.7/huhk/testcase/apache/test_map.py
+-rw-rw-rw-   0        0        0     2627 2023-08-04 01:32:02.000000 huhk-1.9.7/huhk/testcase/apache/test_par_do.py
+-rw-rw-rw-   0        0        0     1646 2023-08-04 01:32:03.000000 huhk-1.9.7/huhk/testcase/apache/test_regex.py
+-rw-rw-rw-   0        0        0     1566 2023-08-04 01:32:02.000000 huhk-1.9.7/huhk/testcase/apache/test_time.py
+-rw-rw-rw-   0        0        0      503 2023-08-04 01:32:03.000000 huhk-1.9.7/huhk/testcase/apache/test_to_string.py
+-rw-rw-rw-   0        0        0    22615 2023-07-14 06:52:17.000000 huhk-1.9.7/huhk/unit_apache_beam.py
+-rw-rw-rw-   0        0        0      352 2023-07-31 09:35:09.000000 huhk-1.9.7/huhk/unit_data.py
+-rw-rw-rw-   0        0        0     4508 2023-07-12 01:13:24.000000 huhk-1.9.7/huhk/unit_dict.py
+-rw-rw-rw-   0        0        0     3843 2023-07-12 01:13:24.000000 huhk-1.9.7/huhk/unit_encryption.py
+-rw-rw-rw-   0        0        0    29677 2023-08-04 02:08:02.000000 huhk-1.9.7/huhk/unit_fun.py
+-rw-rw-rw-   0        0        0     1242 2023-07-12 01:13:24.000000 huhk-1.9.7/huhk/unit_logger.py
+-rw-rw-rw-   0        0        0    10048 2023-08-04 01:36:40.000000 huhk-1.9.7/huhk/unit_request.py
+-rw-rw-rw-   0        0        0     2591 2023-08-04 05:24:53.000000 huhk-1.9.7/huhk/unit_tasks.py
+-rw-rw-rw-   0        0        0      733 2023-07-12 01:13:24.000000 huhk-1.9.7/huhk/常用命令.py
+drwxrwxrwx   0        0        0        0 2023-08-04 06:33:09.399501 huhk-1.9.7/huhk.egg-info/
+-rw-rw-rw-   0        0        0      223 2023-08-04 06:33:09.000000 huhk-1.9.7/huhk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1156 2023-08-04 06:33:09.000000 huhk-1.9.7/huhk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 06:33:09.000000 huhk-1.9.7/huhk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-08-04 06:33:09.000000 huhk-1.9.7/huhk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      134 2023-08-04 06:33:09.000000 huhk-1.9.7/huhk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-08-04 06:33:09.000000 huhk-1.9.7/huhk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-04 06:33:09.486734 huhk-1.9.7/setup.cfg
```

### Comparing `huhk-1.9.6/huhk/__init__.py` & `huhk-1.9.7/huhk/__init__.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.6/huhk/case_project/json_coder.py` & `huhk-1.9.7/huhk/case_project/json_coder.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.6/huhk/case_project/main_fun.py` & `huhk-1.9.7/huhk/case_project/main_fun.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from huhk.case_project.version import version as _version
-from huhk.init_project import GetApi
+from init_project import GetApi
 
 
 def get_version():
     k = str(GetApi.get_main_key())
     v = str(GetApi.get_main_name())
     out_str = f"版本：{_version}\n--key：{k}\n--name：{v}"
     return out_str
```

### Comparing `huhk-1.9.6/huhk/case_project/project_base.py` & `huhk-1.9.7/huhk/case_project/project_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import json
 import os.path
 import re
-import sys
 import time
 
 import requests
 
 from huhk.case_project.project_string import ProjectString
-from huhk.unit_dict import Dict
-from huhk.unit_fun import FunBase
+from unit_dict import Dict
+from unit_fun import FunBase
 from huhk import projects_path
-from huhk.unit_logger import logger
+from unit_logger import logger
 
 
 class ProjectBase(ProjectString):
     def __init__(self, name=None, app_key=None, yapi_url=None, yapi_token=None, yapi_json_file=None, swagger_url=None):
         super().__init__(name, app_key, yapi_url, yapi_token, yapi_json_file, swagger_url)
         self.get_project()
 
@@ -389,10 +388,10 @@
                 i += 1
             FunBase.mkdir_file(fun_path.path, is_py=False)
             FunBase.write_file(fun_path.path, file_str)
 
 
 if __name__ == "__main__":
     a = ProjectBase(name="app_t")
-    a.dir = r"D:\projects\python_test\huhk-common"
+    a.dir = r"/"
     o = a.get_setting_path()
     print(o)
```

### Comparing `huhk-1.9.6/huhk/case_project/project_init.py` & `huhk-1.9.7/huhk/case_project/project_init.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from huhk import projects_path, admin_host
-from huhk.unit_dict import Dict
-from huhk.unit_data import size_names, page_names, before_names, end_names, page_and_size
+from unit_dict import Dict
+from unit_data import size_names, page_names, before_names, end_names, page_and_size
 
 
 class ProjectInIt:
     def __init__(self, name=None, app_key=None, yapi_url=None, yapi_token=None, yapi_json_file=None, swagger_url=None):
         """api_type: 0时，value是swagger的api，json的url
                      1时，value值为yapi项目token,
                      2时，value是yapi下载的json文件名，文件放在file目录下,
```

### Comparing `huhk-1.9.6/huhk/case_project/project_string.py` & `huhk-1.9.7/huhk/case_project/project_string.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import os
 import re
 
 import requests
 
 from huhk.case_project.project_init import ProjectInIt
-from huhk.unit_dict import Dict
+from unit_dict import Dict
 
 
 class ProjectString(ProjectInIt):
     def _get_description(self, req_body_other):
         try:
             if not req_body_other:
                 return []
@@ -225,15 +225,15 @@
     def get_assert_fun_str(self, fun_name):
         assert_fun_str = '    @allure.step(title="接口返回结果校验")\n    def assert_%s(self, _assert=True, **kwargs):\n' \
                          '        assert unit_request.is_assert_true(self.res, _assert), "校验接口返回，缺少成功标识"\n' \
                          '        # out = self.sql_%s(**kwargs)\n' % (fun_name, fun_name)
         assert_fun_str += '        # flag = self.compare_json_list(self.res, out, [%s])\n' % \
                           ', '.join(['"%s"' % i for i in self.this_fun_list.api[fun_name].input
                                      if str(i).lower() not in self.page_and_size])
-        assert_fun_str += '        assert True, "数据比较不一致"\n\n'
+        assert_fun_str += '        # assert flag, "数据比较不一致"\n\n'
         return assert_fun_str
 
     def get_api_fun_header_str(self, fun_name):
         assert_path = self.get_path(fun_name, fun_type='asserts')
         fun_path = self.get_path(fun_name, fun_type='funs')
         api_path = self.get_path(fun_name, fun_type='apis')
         header_str = "import allure\n\n"
```

### Comparing `huhk-1.9.6/huhk/init_project.py` & `huhk-1.9.7/huhk/init_project.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,13 @@
-import json
 import os.path
 import re
-import sys
-import requests
-import time
 
 from huhk.case_project.project_base import ProjectBase
-from huhk.unit_dict import Dict
-from huhk.unit_fun import FunBase
+from unit_dict import Dict
+from unit_fun import FunBase
 from huhk import projects_path
 
 
 class GetApi(ProjectBase):
     def __init__(self, name=None, app_key=None, yapi_url=None, yapi_token=None, yapi_json_file=None, swagger_url=None):
         """
         """
```

### Comparing `huhk-1.9.6/huhk/main.py` & `huhk-1.9.7/huhk/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import click
-from huhk.case_project.main_fun import *
-# from huhk.case_project.main_fun import get_version, set_key_name
+
+
+from huhk.case_project.main_fun import get_version, set_key_name, install_project, update_project, fun_project
 
 
 @click.command()
 @click.option('-v', '--version', help='版本, 当前--key/--name', is_eager=True, is_flag=True)
 @click.option('-k', '--key', help='项目key, 传*表示所有项目，不传默认去上一次key')
 @click.option('-n', '--name', help='项目名称, 传*表示所有项目，不传默认去上一次name')
 @click.option('-i', '--install', help='根据key创建项目, 项目存在则更新')
@@ -17,12 +18,12 @@
     else:
         set_key_name(key, name)
         if install:
             click.echo(install_project(install, name))
         elif update:
             click.echo(update_project(key, name))
         elif fun:
-            click.echo(fun_project(key=key, name=name, fun_url=fun))
+            click.echo(fun_project(app_key=key, name=name, fun_url=fun))
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `huhk-1.9.6/huhk/testcase/apache/beam_class.py` & `huhk-1.9.7/huhk/testcase/apache/beam_class.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.6/huhk/testcase/apache/data.py` & `huhk-1.9.7/huhk/testcase/apache/data.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.6/huhk/testcase/apache/par_do.py` & `huhk-1.9.7/huhk/testcase/apache/par_do.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.6/huhk/testcase/apache/test_cogroupbykey.py` & `huhk-1.9.7/huhk/testcase/apache/test_cogroupbykey.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from testcase.apache.beam_class import AverageFn, AverageFn2
-from huhk.unit_apache_beam import ApacheFun
+from unit_apache_beam import ApacheFun
 
 
 class TestPolymerization:
     # 通过键聚合所有输入元素，并允许下游处理使用与键关联的所有值
     def test_polymerization_001(self):
         ApacheFun(data_type=data_type).co_group_by_key(icons=data_list_tuple3, durations=data_list_tuple4).print()
```

### Comparing `huhk-1.9.6/huhk/testcase/apache/test_fiter.py` & `huhk-1.9.7/huhk/testcase/apache/test_fiter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from huhk.unit_apache_beam import ApacheFun
+from unit_apache_beam import ApacheFun
 
 
 class TestFiter:
     def setup(self):
         self.af = ApacheFun(data_list_dict, data_type=data_type)
 
     # 使用函数过滤
```

### Comparing `huhk-1.9.6/huhk/testcase/apache/test_flatmap.py` & `huhk-1.9.7/huhk/testcase/apache/test_flatmap.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from huhk.unit_apache_beam import ApacheFun
+from unit_apache_beam import ApacheFun
 
 
 class TestFlatmap:
     def setup(self):
         self.af = ApacheFun(data_list_str, data_type=data_type)
 
     # 带有预定义函数的 FlatMap
```

### Comparing `huhk-1.9.6/huhk/testcase/apache/test_map.py` & `huhk-1.9.7/huhk/testcase/apache/test_map.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from huhk.unit_apache_beam import ApacheFun
+from unit_apache_beam import ApacheFun
 
 
 class TestMap:
     # 带有预定义函数的 FlatMap
     def test_map_001(self):
         ApacheFun(data_list_str3, data_type=data_type).map(str.strip).print()
```

### Comparing `huhk-1.9.6/huhk/testcase/apache/test_par_do.py` & `huhk-1.9.7/huhk/testcase/apache/test_par_do.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import random
-from huhk.unit_apache_beam import ApacheFun
+from unit_apache_beam import ApacheFun
 from testcase.apache.beam_class import SplitWords, AnalyzeElement, DoFnMethods
 
 
 class TestParDo:
     # 有简单 DoFn 的 ParDo
     def test_par_do_001(self):
         ApacheFun(data_list_str2, data_type=data_type).par_do(SplitWords(',')).print()
```

### Comparing `huhk-1.9.6/huhk/testcase/apache/test_regex.py` & `huhk-1.9.7/huhk/testcase/apache/test_regex.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from huhk.unit_apache_beam import ApacheFun
+from unit_apache_beam import ApacheFun
 
 
 class TestRegex:
     # 正则表达式匹配
     def test_regex_001(self):
         ApacheFun(data_list_str4, data_type=data_type).regex_matches(r'(?P<icon>[^\s,]+), *(\w+), *(\w+)').print()
```

### Comparing `huhk-1.9.6/huhk/testcase/apache/test_time.py` & `huhk-1.9.7/huhk/testcase/apache/test_time.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from huhk.unit_apache_beam import ApacheFun
+from unit_apache_beam import ApacheFun
 
 
 class TestTimes:
     # 按事件时间标记时间戳
     def test_times_001(self):
         ApacheFun(data_list_dict3, data_type=data_type).timestamped_value("season").print()
```

### Comparing `huhk-1.9.6/huhk/unit_apache_beam.py` & `huhk-1.9.7/huhk/unit_apache_beam.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.6/huhk/unit_dict.py` & `huhk-1.9.7/huhk/unit_dict.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.6/huhk/unit_encryption.py` & `huhk-1.9.7/huhk/unit_encryption.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.6/huhk/unit_fun.py` & `huhk-1.9.7/huhk/unit_fun.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 import time
 import requests
 import datetime
 from pandas import DataFrame, ExcelWriter
 from typing import List
 from faker import Faker
 
-from huhk.unit_dict import Dict
-from huhk.unit_logger import logger
-from huhk.unit_data import page_and_size, before_and_end_re_str
+from unit_dict import Dict
+from unit_logger import logger
+from unit_data import page_and_size, before_and_end_re_str
 
 
 class FunBase:
     def __init__(self):
         self._time2 = 0
         self._time1 = 0
         self.sql_str = ""
@@ -608,16 +608,17 @@
         if version_l[2] > 9:
             version_l[1] += 1
             version_l[2] = 1
             if version_l[1] > 9:
                 version_l[0] += 1
                 version_l[1] = 1
         version = ".".join([str(i) for i in version_l])
-
-        with open("huhk/case_project/version.py", "w", encoding="utf-8") as f:
+        print(os.path.dirname(__file__))
+        version_path = os.path.join(os.path.dirname(__file__), "case_project", "version.py")
+        with open(version_path, "w", encoding="utf-8") as f:
             f.write("version='%s'\n" % version)
         return version
 
     def set_value(self, value_dict):
         caller = inspect.getframeinfo(inspect.currentframe().f_back)
         for k, v in value_dict.items():
             if k not in page_and_size:
```

### Comparing `huhk-1.9.6/huhk/unit_logger.py` & `huhk-1.9.7/huhk/unit_logger.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.6/huhk/unit_request.py` & `huhk-1.9.7/huhk/unit_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 import requests
 import json
 import time
 import urllib
 import os
 import hashlib
 
+from unit_fun import FunBase
 from requests import ReadTimeout, ConnectTimeout
 from requests.exceptions import MissingSchema
 from urllib.parse import urlencode
-from huhk.unit_dict import Dict
-from huhk.unit_logger import logger
+from unit_dict import Dict
+from unit_logger import logger
 from openpyxl.reader.excel import load_workbook
 from huhk import admin_host, projects_path
 
 
 class UnitRequest:
     def __init__(self, ZEST_ENV=None, APP_KEY=None, TIMEOUT=30000):
         self.ZEST_ENV = ZEST_ENV
@@ -112,14 +113,15 @@
             try:
                 res.rsp = Dict(json.loads(res.text)) if res.text else res.text
             except:
                 if "filename=" in str(res.raw.headers):
                     file_name = urllib.parse.unquote(re.findall(r'filename=(.+?)\'', str(res.raw.headers))[0])
                     if "xlsx" in file_name:
                         file_path = os.path.join(projects_path, "files", file_name)
+                        FunBase.mkdir_file(file_path, is_py=False)
                         with open(file_path, 'wb') as f:
                             f.write(res.content)
                         wb = load_workbook(file_path)
                         ws = wb.active
                         rows = [[cell.value for cell in row] for row in ws]
                         try:
                             data = [{c1: c2 for c1, c2 in zip(rows[0], row)} for row in rows[1:]]
```

### Comparing `huhk-1.9.6/huhk/unit_tasks.py` & `huhk-1.9.7/huhk/unit_tasks.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,15 @@
         else:
             Scheduler.scheduler = BlockingScheduler()
 
     @staticmethod
     def get_cron(corn_str):
         cron_list = re.split(r'\s+', corn_str.strip().replace('?', '*').replace('?', '？'))
         cron_list += ["*"] * 7
+        cron_list = [None if i in ("*", "?", "？") else i for i in cron_list]
         second = cron_list[0]
         minute = cron_list[1]
         hour = cron_list[2]
         day = cron_list[3]
         month = cron_list[4]
         day_of_week = '*' if cron_list[5] in ('?', '？') else cron_list[5]
         year = cron_list[6]
```

### Comparing `huhk-1.9.6/huhk/常用命令.py` & `huhk-1.9.7/huhk/常用命令.py`

 * *Files identical despite different names*

