# Comparing `tmp/eis1600-0.9.7.tar.gz` & `tmp/eis1600-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eis1600-0.9.7.tar", last modified: Wed Jul 12 09:03:52 2023, max compression
+gzip compressed data, was "eis1600-1.0.1.tar", last modified: Fri Aug  4 07:20:03 2023, max compression
```

## Comparing `eis1600-0.9.7.tar` & `eis1600-1.0.1.tar`

### file list

```diff
@@ -1,88 +1,96 @@
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-07-12 09:03:52.829389 eis1600-0.9.7/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1046 2022-09-21 09:22:30.000000 eis1600-0.9.7/LICENSE
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    10441 2023-07-12 09:03:52.829389 eis1600-0.9.7/PKG-INFO
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     7967 2023-07-03 10:37:00.000000 eis1600-0.9.7/README.md
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-07-12 09:03:52.817389 eis1600-0.9.7/eis1600/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-09-19 09:55:48.000000 eis1600-0.9.7/eis1600/__init__.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-07-12 09:03:52.817389 eis1600-0.9.7/eis1600/dates/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      911 2023-04-05 11:10:16.000000 eis1600-0.9.7/eis1600/dates/Date.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.9.7/eis1600/dates/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     6116 2023-07-10 10:56:25.000000 eis1600-0.9.7/eis1600/dates/date_patterns.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5111 2023-07-07 07:47:22.000000 eis1600-0.9.7/eis1600/dates/methods.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-07-12 09:03:52.817389 eis1600-0.9.7/eis1600/gazetteers/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4245 2023-05-26 10:11:18.000000 eis1600-0.9.7/eis1600/gazetteers/Onomastics.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3476 2023-06-14 10:59:59.000000 eis1600-0.9.7/eis1600/gazetteers/Toponyms.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-03-09 08:52:31.000000 eis1600-0.9.7/eis1600/gazetteers/__init__.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-07-12 09:03:52.821389 eis1600-0.9.7/eis1600/gazetteers/data/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.9.7/eis1600/gazetteers/data/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    96536 2023-04-17 09:44:13.000000 eis1600-0.9.7/eis1600/gazetteers/data/onomastic_gazetteer.csv
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1307 2023-04-03 09:19:01.000000 eis1600-0.9.7/eis1600/gazetteers/data/spelling_gazetteer.csv
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)   264282 2023-06-14 10:40:04.000000 eis1600-0.9.7/eis1600/gazetteers/data/toponyms_gazetteer.csv
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-07-12 09:03:52.821389 eis1600-0.9.7/eis1600/helper/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      990 2023-05-25 16:02:00.000000 eis1600-0.9.7/eis1600/helper/EntityTags.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      393 2023-07-12 08:58:30.000000 eis1600-0.9.7/eis1600/helper/EvalResultsEncoder.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1280 2023-04-24 10:02:09.000000 eis1600-0.9.7/eis1600/helper/Singleton.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-10-20 15:09:05.000000 eis1600-0.9.7/eis1600/helper/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1030 2023-04-06 13:50:26.000000 eis1600-0.9.7/eis1600/helper/ar_normalization.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-07-12 09:03:52.821389 eis1600-0.9.7/eis1600/helper/data/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-04-03 10:40:59.000000 eis1600-0.9.7/eis1600/helper/data/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      324 2023-05-17 14:58:12.000000 eis1600-0.9.7/eis1600/helper/data/entity_tags.csv
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     6547 2023-07-12 09:00:06.000000 eis1600-0.9.7/eis1600/helper/eval_date_model.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1247 2023-05-26 10:15:41.000000 eis1600-0.9.7/eis1600/helper/fix_miu_annotation.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      377 2023-05-26 10:20:20.000000 eis1600-0.9.7/eis1600/helper/logging.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      707 2023-05-10 14:33:13.000000 eis1600-0.9.7/eis1600/helper/markdown_methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3915 2023-07-06 08:53:43.000000 eis1600-0.9.7/eis1600/helper/markdown_patterns.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     6461 2023-03-09 10:15:31.000000 eis1600-0.9.7/eis1600/helper/miu_random_revisions.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    11325 2023-07-12 07:09:47.000000 eis1600-0.9.7/eis1600/helper/repo.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2746 2023-07-12 07:01:24.000000 eis1600-0.9.7/eis1600/helper/top_tags_to_bio.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      383 2023-05-24 09:09:03.000000 eis1600-0.9.7/eis1600/helper/yml_methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1667 2023-06-23 09:40:16.000000 eis1600-0.9.7/eis1600/helper/yml_to_json.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-07-12 09:03:52.825389 eis1600-0.9.7/eis1600/markdown/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1822 2023-04-12 07:11:17.000000 eis1600-0.9.7/eis1600/markdown/UIDs.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-09-30 09:01:09.000000 eis1600-0.9.7/eis1600/markdown/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4809 2023-05-26 10:21:31.000000 eis1600-0.9.7/eis1600/markdown/convert_mARkdown_to_EIS1600TMP.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4589 2023-05-26 10:14:46.000000 eis1600-0.9.7/eis1600/markdown/insert_uids.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2945 2023-07-10 10:38:20.000000 eis1600-0.9.7/eis1600/markdown/md_to_bio.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    12973 2023-06-08 07:44:43.000000 eis1600-0.9.7/eis1600/markdown/methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2875 2023-05-26 10:22:35.000000 eis1600-0.9.7/eis1600/markdown/update_uids.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5268 2023-05-26 10:25:25.000000 eis1600-0.9.7/eis1600/markdown/update_uids_old_process.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-07-12 09:03:52.825389 eis1600-0.9.7/eis1600/miu/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3481 2023-05-26 10:15:16.000000 eis1600-0.9.7/eis1600/miu/HeadingTracker.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     7927 2023-06-23 09:37:32.000000 eis1600-0.9.7/eis1600/miu/YAMLHandler.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-08 08:28:10.000000 eis1600-0.9.7/eis1600/miu/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2773 2023-05-26 10:23:54.000000 eis1600-0.9.7/eis1600/miu/disassemble_into_miu_files.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     9846 2023-07-12 09:03:43.000000 eis1600-0.9.7/eis1600/miu/methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2605 2023-05-26 10:26:08.000000 eis1600-0.9.7/eis1600/miu/reassemble_from_miu_files.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    10503 2023-06-23 07:37:45.000000 eis1600-0.9.7/eis1600/miu/yml_handling.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-07-12 09:03:52.825389 eis1600-0.9.7/eis1600/nlp/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-17 12:10:00.000000 eis1600-0.9.7/eis1600/nlp/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3560 2023-07-12 09:03:43.000000 eis1600-0.9.7/eis1600/nlp/cameltools.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3577 2023-06-08 07:55:51.000000 eis1600-0.9.7/eis1600/nlp/ner_annotate_mius.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     7565 2023-07-12 09:03:43.000000 eis1600-0.9.7/eis1600/nlp/utils.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-07-12 09:03:52.825389 eis1600-0.9.7/eis1600/onomastics/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-03-02 09:23:30.000000 eis1600-0.9.7/eis1600/onomastics/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1358 2023-05-25 14:13:19.000000 eis1600-0.9.7/eis1600/onomastics/annotation.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    10544 2023-06-08 08:49:39.000000 eis1600-0.9.7/eis1600/onomastics/methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1966 2023-04-17 09:33:17.000000 eis1600-0.9.7/eis1600/onomastics/re_pattern.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-07-12 09:03:52.825389 eis1600-0.9.7/eis1600/processing/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.9.7/eis1600/processing/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4724 2023-06-08 07:25:33.000000 eis1600-0.9.7/eis1600/processing/postprocessing.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5019 2023-06-22 10:57:07.000000 eis1600-0.9.7/eis1600/processing/preprocessing.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-07-12 09:03:52.825389 eis1600-0.9.7/eis1600/stats/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-02-17 08:45:10.000000 eis1600-0.9.7/eis1600/stats/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      842 2023-02-17 15:06:29.000000 eis1600-0.9.7/eis1600/stats/methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1978 2023-02-17 15:05:56.000000 eis1600-0.9.7/eis1600/stats/miu_stats.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-07-12 09:03:52.829389 eis1600-0.9.7/eis1600/toponyms/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-05-17 10:52:32.000000 eis1600-0.9.7/eis1600/toponyms/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2371 2023-06-22 10:57:07.000000 eis1600-0.9.7/eis1600/toponyms/annotation.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3153 2023-06-22 10:57:07.000000 eis1600-0.9.7/eis1600/toponyms/methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1076 2023-07-12 07:17:22.000000 eis1600-0.9.7/eis1600/toponyms/toponym_categories.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-07-12 09:03:52.817389 eis1600-0.9.7/eis1600.egg-info/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    10441 2023-07-12 09:03:52.000000 eis1600-0.9.7/eis1600.egg-info/PKG-INFO
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2185 2023-07-12 09:03:52.000000 eis1600-0.9.7/eis1600.egg-info/SOURCES.txt
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        1 2023-07-12 09:03:52.000000 eis1600-0.9.7/eis1600.egg-info/dependency_links.txt
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      915 2023-07-12 09:03:52.000000 eis1600-0.9.7/eis1600.egg-info/entry_points.txt
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      108 2023-07-12 09:03:52.000000 eis1600-0.9.7/eis1600.egg-info/requires.txt
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        8 2023-07-12 09:03:52.000000 eis1600-0.9.7/eis1600.egg-info/top_level.txt
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)       38 2023-07-12 09:03:52.829389 eis1600-0.9.7/setup.cfg
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2562 2023-07-12 09:02:05.000000 eis1600-0.9.7/setup.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-08-04 07:20:03.862836 eis1600-1.0.1/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1046 2022-09-21 09:22:30.000000 eis1600-1.0.1/LICENSE
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    10441 2023-08-04 07:20:03.862836 eis1600-1.0.1/PKG-INFO
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     7967 2023-07-03 10:37:00.000000 eis1600-1.0.1/README.md
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-08-04 07:20:03.842836 eis1600-1.0.1/eis1600/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-09-19 09:55:48.000000 eis1600-1.0.1/eis1600/__init__.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-08-04 07:20:03.846835 eis1600-1.0.1/eis1600/dates/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      911 2023-04-05 11:10:16.000000 eis1600-1.0.1/eis1600/dates/Date.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-1.0.1/eis1600/dates/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     6396 2023-08-03 09:42:54.000000 eis1600-1.0.1/eis1600/dates/date_patterns.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5303 2023-08-03 09:42:54.000000 eis1600-1.0.1/eis1600/dates/methods.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-08-04 07:20:03.846835 eis1600-1.0.1/eis1600/gazetteers/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4245 2023-05-26 10:11:18.000000 eis1600-1.0.1/eis1600/gazetteers/Onomastics.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3476 2023-06-14 10:59:59.000000 eis1600-1.0.1/eis1600/gazetteers/Toponyms.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-03-09 08:52:31.000000 eis1600-1.0.1/eis1600/gazetteers/__init__.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-08-04 07:20:03.850835 eis1600-1.0.1/eis1600/gazetteers/data/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-1.0.1/eis1600/gazetteers/data/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      536 2023-07-19 09:36:14.000000 eis1600-1.0.1/eis1600/gazetteers/data/days_gazetteer.csv
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      587 2023-07-19 09:36:14.000000 eis1600-1.0.1/eis1600/gazetteers/data/months_gazetteer.csv
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    96536 2023-04-17 09:44:13.000000 eis1600-1.0.1/eis1600/gazetteers/data/onomastic_gazetteer.csv
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1307 2023-04-03 09:19:01.000000 eis1600-1.0.1/eis1600/gazetteers/data/spelling_gazetteer.csv
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)   264282 2023-06-14 10:40:04.000000 eis1600-1.0.1/eis1600/gazetteers/data/toponyms_gazetteer.csv
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2604 2023-07-19 09:36:14.000000 eis1600-1.0.1/eis1600/gazetteers/data/years_gazetteer.csv
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-08-04 07:20:03.854836 eis1600-1.0.1/eis1600/helper/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      986 2023-07-20 11:42:11.000000 eis1600-1.0.1/eis1600/helper/EntityTags.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      393 2023-07-12 08:58:30.000000 eis1600-1.0.1/eis1600/helper/EvalResultsEncoder.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1280 2023-04-24 10:02:09.000000 eis1600-1.0.1/eis1600/helper/Singleton.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-10-20 15:09:05.000000 eis1600-1.0.1/eis1600/helper/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1030 2023-04-06 13:50:26.000000 eis1600-1.0.1/eis1600/helper/ar_normalization.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-08-04 07:20:03.854836 eis1600-1.0.1/eis1600/helper/data/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-04-03 10:40:59.000000 eis1600-1.0.1/eis1600/helper/data/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      363 2023-07-20 09:30:08.000000 eis1600-1.0.1/eis1600/helper/data/entity_tags.csv
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     7721 2023-08-03 09:42:54.000000 eis1600-1.0.1/eis1600/helper/eval_date_model.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1247 2023-05-26 10:15:41.000000 eis1600-1.0.1/eis1600/helper/fix_miu_annotation.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2593 2023-07-20 11:42:11.000000 eis1600-1.0.1/eis1600/helper/fix_ono_p_tags_order.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      377 2023-05-26 10:20:20.000000 eis1600-1.0.1/eis1600/helper/logging.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      707 2023-05-10 14:33:13.000000 eis1600-1.0.1/eis1600/helper/markdown_methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3962 2023-08-03 09:42:54.000000 eis1600-1.0.1/eis1600/helper/markdown_patterns.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     6461 2023-03-09 10:15:31.000000 eis1600-1.0.1/eis1600/helper/miu_random_revisions.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    11360 2023-08-03 10:35:19.000000 eis1600-1.0.1/eis1600/helper/repo.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2678 2023-07-17 10:52:47.000000 eis1600-1.0.1/eis1600/helper/topo_tags_to_bio.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      383 2023-05-24 09:09:03.000000 eis1600-1.0.1/eis1600/helper/yml_methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1667 2023-06-23 09:40:16.000000 eis1600-1.0.1/eis1600/helper/yml_to_json.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-08-04 07:20:03.854836 eis1600-1.0.1/eis1600/markdown/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1822 2023-04-12 07:11:17.000000 eis1600-1.0.1/eis1600/markdown/UIDs.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-09-30 09:01:09.000000 eis1600-1.0.1/eis1600/markdown/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4809 2023-05-26 10:21:31.000000 eis1600-1.0.1/eis1600/markdown/convert_mARkdown_to_EIS1600TMP.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4589 2023-05-26 10:14:46.000000 eis1600-1.0.1/eis1600/markdown/insert_uids.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     6163 2023-07-20 11:42:11.000000 eis1600-1.0.1/eis1600/markdown/md_to_bio.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    12973 2023-06-08 07:44:43.000000 eis1600-1.0.1/eis1600/markdown/methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2875 2023-05-26 10:22:35.000000 eis1600-1.0.1/eis1600/markdown/update_uids.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5268 2023-05-26 10:25:25.000000 eis1600-1.0.1/eis1600/markdown/update_uids_old_process.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-08-04 07:20:03.858836 eis1600-1.0.1/eis1600/miu/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3513 2023-07-20 08:28:39.000000 eis1600-1.0.1/eis1600/miu/HeadingTracker.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     8456 2023-08-03 11:06:27.000000 eis1600-1.0.1/eis1600/miu/YAMLHandler.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-08 08:28:10.000000 eis1600-1.0.1/eis1600/miu/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2773 2023-05-26 10:23:54.000000 eis1600-1.0.1/eis1600/miu/disassemble_into_miu_files.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     9800 2023-08-03 09:42:54.000000 eis1600-1.0.1/eis1600/miu/methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2605 2023-05-26 10:26:08.000000 eis1600-1.0.1/eis1600/miu/reassemble_from_miu_files.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    11014 2023-08-03 09:42:58.000000 eis1600-1.0.1/eis1600/miu/yml_handling.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-08-04 07:20:03.858836 eis1600-1.0.1/eis1600/nlp/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-17 12:10:00.000000 eis1600-1.0.1/eis1600/nlp/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4151 2023-07-17 12:34:42.000000 eis1600-1.0.1/eis1600/nlp/cameltools.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3577 2023-08-02 13:03:28.000000 eis1600-1.0.1/eis1600/nlp/ner_annotate_mius.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5587 2023-07-20 08:28:39.000000 eis1600-1.0.1/eis1600/nlp/utils.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-08-04 07:20:03.858836 eis1600-1.0.1/eis1600/onomastics/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-03-02 09:23:30.000000 eis1600-1.0.1/eis1600/onomastics/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1358 2023-05-25 14:13:19.000000 eis1600-1.0.1/eis1600/onomastics/annotation.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    10544 2023-06-08 08:49:39.000000 eis1600-1.0.1/eis1600/onomastics/methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1966 2023-04-17 09:33:17.000000 eis1600-1.0.1/eis1600/onomastics/re_pattern.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-08-04 07:20:03.858836 eis1600-1.0.1/eis1600/processing/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-1.0.1/eis1600/processing/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4426 2023-07-20 11:34:46.000000 eis1600-1.0.1/eis1600/processing/postprocessing.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5019 2023-07-17 10:11:06.000000 eis1600-1.0.1/eis1600/processing/preprocessing.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-08-04 07:20:03.858836 eis1600-1.0.1/eis1600/statistics/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-08-03 09:44:33.000000 eis1600-1.0.1/eis1600/statistics/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3742 2023-08-04 07:19:55.000000 eis1600-1.0.1/eis1600/statistics/count_tokens_per_miu.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      925 2023-08-04 07:19:55.000000 eis1600-1.0.1/eis1600/statistics/methods.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-08-04 07:20:03.858836 eis1600-1.0.1/eis1600/stats/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-02-17 08:45:10.000000 eis1600-1.0.1/eis1600/stats/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      842 2023-02-17 15:06:29.000000 eis1600-1.0.1/eis1600/stats/methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1978 2023-02-17 15:05:56.000000 eis1600-1.0.1/eis1600/stats/miu_stats.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-08-04 07:20:03.862836 eis1600-1.0.1/eis1600/toponyms/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-05-17 10:52:32.000000 eis1600-1.0.1/eis1600/toponyms/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2371 2023-08-02 09:51:48.000000 eis1600-1.0.1/eis1600/toponyms/annotation.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3153 2023-06-22 10:57:07.000000 eis1600-1.0.1/eis1600/toponyms/methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1076 2023-07-12 07:17:22.000000 eis1600-1.0.1/eis1600/toponyms/toponym_categories.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-08-04 07:20:03.846835 eis1600-1.0.1/eis1600.egg-info/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    10441 2023-08-04 07:20:03.000000 eis1600-1.0.1/eis1600.egg-info/PKG-INFO
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2461 2023-08-04 07:20:03.000000 eis1600-1.0.1/eis1600.egg-info/SOURCES.txt
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        1 2023-08-04 07:20:03.000000 eis1600-1.0.1/eis1600.egg-info/dependency_links.txt
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1049 2023-08-04 07:20:03.000000 eis1600-1.0.1/eis1600.egg-info/entry_points.txt
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      119 2023-08-04 07:20:03.000000 eis1600-1.0.1/eis1600.egg-info/requires.txt
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        8 2023-08-04 07:20:03.000000 eis1600-1.0.1/eis1600.egg-info/top_level.txt
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)       38 2023-08-04 07:20:03.862836 eis1600-1.0.1/setup.cfg
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2752 2023-08-03 14:31:05.000000 eis1600-1.0.1/setup.py
```

### Comparing `eis1600-0.9.7/LICENSE` & `eis1600-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.7/PKG-INFO` & `eis1600-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eis1600
-Version: 0.9.7
+Version: 1.0.1
 Summary: EIS1600 project tools and utilities
 Home-page: https://github.com/EIS1600/eis1600-pkg
 Author: Lisa Mischer
 Author-email: mischer.lisa@gmail.com
 License: MIT License
 Description: # EIS1600 Tools
```

### Comparing `eis1600-0.9.7/README.md` & `eis1600-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.7/eis1600/dates/Date.py` & `eis1600-1.0.1/eis1600/dates/Date.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.7/eis1600/dates/date_patterns.py` & `eis1600-1.0.1/eis1600/dates/date_patterns.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,42 +3,47 @@
 from openiti.helper.ara import denormalize
 
 from eis1600.helper.ar_normalization import normalize_dict
 from eis1600.helper.markdown_patterns import WORD
 
 ONES = {
         'واحد': 1, 'احدى': 1, 'احد': 1, 'اثنين': 2, 'اثنتين': 2, 'اثنتي': 2, 'ثلاث': 3, 'ثلث': 3, 'اربع': 4, 'خمس': 5,
-        'ست': 6, 'سبع': 7, 'ثماني': 8, 'ثمان': 8, 'تسع': 9
+        'ست': 6, 'سبع': 7, 'ثماني': 8, 'ثمان': 8, 'تسع': 9, 'نيف': 5, 'بضع': 5
 }
-# TODO integrate
-INDETERMINATES = ['بضع', 'في حدود', 'نيف']
-
 ONES_NOR = normalize_dict(ONES)
 TEN = {
         'عشرة': 10, 'عشري': 10, 'عشر': 10, 'عشرين': 20, 'ثلاثين': 30, 'اربعين': 40, 'خمسين': 50, 'ستين': 60,
         'سبعين': 70,
         'ثمانين': 80, 'تسعين': 90
 }
 TEN_NOR = normalize_dict(TEN)
 HUNDRED = {
-        'مائة': 100, 'ماية': 100, 'مية': 100, 'مئة': 100, 'مائتين': 200, 'مايتين': 200, 'ميتين': 200,
-        'ثلاثمائة': 300, 'ثلاث مائة': 300, 'ثلثمائة': 300, 'ثلث مائة': 300, 'اربعمائة': 400, 'اربع مائة': 400,
-        'خمسمائة': 500, 'خمس مائة': 500, 'ستمائة': 600, 'ست مائة': 600, 'سبعمائة': 700, 'سبع مائة': 700,
-        'ثمانمائة': 800, 'ثمان مائة': 800, 'ثمانيمائة': 800, 'ثماني مائة': 800, 'تسعمائة': 900, 'تسع مائة': 900,
-        'ثلاثماية': 300, 'ثلاث ماية': 300, 'ثلثماية': 300, 'ثلث ماية': 300, 'اربعماية': 400, 'اربع ماية': 400,
-        'خمسماية': 500, 'خمس ماية': 500, 'ستماية': 600, 'ست ماية': 600, 'سبعماية': 700, 'سبع ماية': 700,
-        'ثمانماية': 800, 'ثمان ماية': 800, 'ثمانيماية': 800, 'ثماني ماية': 800, 'تسعماية': 900, 'تسع ماية': 900,
-        'ثلاثمية': 300, 'ثلاث مية': 300, 'ثلثمية': 300, 'ثلث مية': 300, 'اربعمية': 400, 'اربع مية': 400, 'خمسمية': 500,
-        'خمس مية': 500, 'ستمية': 600, 'ست مية': 600, 'سبعمية': 700, 'سبع مية': 700, 'ثمانمية': 800, 'ثمان مية': 800,
-        'ثمانيمية': 800, 'ثماني مية': 800, 'تسعمية': 900, 'تسع مية': 900, 'ثلاثمئة': 300, 'ثلاث مئة': 300,
-        'ثلثمئة': 300, 'ثلث مئة': 300, 'اربعمئة': 400, 'اربع مئة': 400, 'خمسمئة': 500, 'خمس مئة': 500, 'ستمئة': 600,
-        'ست مئة': 600, 'سبعمئة': 700, 'سبع مئة': 700, 'ثمانمئة': 800, 'ثمان مئة': 800, 'ثمانيمئة': 800,
-        'ثماني مئة': 800, 'تسعمئة': 900, 'تسع مئة': 900
+        'مائة': 100, 'ماية': 100, 'مية': 100, 'مئة': 100,
+        'المائة': 100, 'الماية': 100, 'المية': 100, 'المئة': 100,
+        'مائتين': 200, 'مايتين': 200, 'ميتين': 200,
+        'ثلاثمائة': 300, 'ثلاث مائة': 300, 'ثلثمائة': 300, 'ثلث مائة': 300, 'ثلاثماية': 300, 'ثلاث ماية': 300,
+        'ثلثماية': 300, 'ثلث ماية': 300, 'ثلاثمية': 300, 'ثلاث مية': 300, 'ثلثمية': 300, 'ثلث مية': 300,
+        'ثلاثمئة': 300, 'ثلاث مئة': 300, 'ثلثمئة': 300, 'ثلث مئة': 300,
+        'اربعمائة': 400, 'اربع مائة': 400, 'اربعماية': 400, 'اربع ماية': 400, 'اربعمية': 400, 'اربع مية': 400,
+        'اربعمئة': 400, 'اربع مئة': 400,
+        'خمسمائة': 500, 'خمس مائة': 500, 'خمسماية': 500, 'خمس ماية': 500, 'خمسمية': 500, 'خمس مية': 500, 'خمسمئة': 500,
+        'خمس مئة': 500,
+        'ستمائة': 600, 'ست مائة': 600, 'ستماية': 600, 'ست ماية': 600, 'ستمية': 600, 'ست مية': 600, 'ستمئة': 600,
+        'ست مئة': 600,
+        'سبعمائة': 700, 'سبع مائة': 700, 'سبعماية': 700, 'سبع ماية': 700, 'سبعمية': 700, 'سبع مية': 700, 'سبعمئة': 700,
+        'سبع مئة': 700,
+        'ثمانمائة': 800, 'ثمان مائة': 800, 'ثمانيمائة': 800, 'ثماني مائة': 800, 'ثمانماية': 800, 'ثمان ماية': 800,
+        'ثمانيماية': 800, 'ثماني ماية': 800, 'ثمانمية': 800, 'ثمان مية': 800, 'ثمانيمية': 800, 'ثماني مية': 800,
+        'ثمانمئة': 800, 'ثمان مئة': 800, 'ثمانيمئة': 800, 'ثماني مئة': 800,
+        'تسعمائة': 900, 'تسع مائة': 900, 'تسعماية': 900, 'تسع ماية': 900, 'تسعمية': 900, 'تسع مية': 900, 'تسعمئة': 900,
+        'تسع مئة': 900
 }
 HUNDRED_NOR = normalize_dict(HUNDRED)
+THOUSAND = normalize_dict({'ألف': 1000})
+THOUSAND_NOR = normalize_dict(THOUSAND)
 
 DAY_ONES = {
         'واحد': 1, 'حادي': 1, 'ثاني': 2, 'ثالث': 3, 'رابع': 4, 'خامس': 5, 'خميس': 5, 'سادس': 6, 'سابع': 7,
         'ثامن': 8, 'تاسع': 9, 'عاشر': 10
 }
 DAY_ONES_NOR = normalize_dict(DAY_ONES)
 DAY_TEN = {'عشرة': 10, 'عشري': 10, 'عشر': 10, 'عشرين': 20, 'عشرون': 20, 'ثلاثين': 30, 'ثلاثون': 30}
@@ -53,31 +58,35 @@
         'محرم': 1, 'شهر الله المحرم': 1, 'صفر': 2, 'صفر الخير': 2, 'ربيع': 3, 'ربيع الاول': 3, 'ربيع الثاني': 4,
         'ربيع الاخر': 4, 'جمادى الاول': 5, 'جمادى الاولى': 5, 'جمادى الاخرة': 6, 'جمادى الاخر': 6, 'جمادى الثانية': 6,
         'رجب': 7, 'رجب الفرد': 7, 'رجب المبارك': 7, 'شعبان': 8, 'شعبان المكرم': 8, 'رمضان': 9,
         'رمضان المعظم': 9, 'شوال': 10, 'ذي القعدة': 11, 'ذي قعدة': 11, 'ذي الحجة': 12, 'ذي حجة': 12, 'ذو القعدة': 11,
         'ذو قعدة': 11, 'ذو الحجة': 12, 'ذو حجة': 12, 'اخر': -1
 }
 MONTHS_NOR = normalize_dict(MONTHS)
+SANA = ['سنة', 'عام', 'في حدود']
 
-AR_MONTHS = '|'.join(['(?:' + r'\s'.join(denormalize(key).split()) + ')' for key in MONTHS.keys()])
+AR_MONTHS = '|'.join([denormalize(key) for key in MONTHS.keys()])
 AR_ONES = '|'.join([denormalize(key) for key in ONES.keys()])
 AR_TEN = '|'.join([denormalize(key) for key in TEN.keys()])
-AR_HUNDRED = '|'.join(['(?:' + r'\s'.join(denormalize(key).split()) + ')' for key in HUNDRED.keys()])
+AR_HUNDRED = '|'.join([denormalize(key) for key in HUNDRED.keys()])
+AR_THOUSAND = '|'.join([denormalize(key) for key in THOUSAND.keys()])
 AR_ONES_DAY = '|'.join([denormalize(key) for key in DAY_ONES.keys()])
 AR_TEN_DAY = '|'.join([denormalize(key) for key in DAY_TEN.keys()])
-AR_WEEKDAY = '|'.join(['(?:' + r'\s'.join(key.split()) + ')' for key in WEEKDAYS.keys()])
+AR_WEEKDAY = '|'.join([denormalize(key) for key in WEEKDAYS.keys()])
+AR_SANA = '|'.join([denormalize(s) for s in SANA])
 DATE = r'(?P<context>' + WORD + r'{0,10}?' + r'(?:\s(?:ف[يى]|تقريبا))?' + WORD + r'{0,9}?)' + \
        r'(?:\s(?P<weekday>' + AR_WEEKDAY + r'))?' + \
        r'(?:\s(:?ال)?(?P<day_ones>' + AR_ONES_DAY + r'))?(?:\s(:?و)?(:?ال)?(?P<day_ten>' + AR_TEN_DAY + r'))?' + \
        r'(?:\s(?:(?:من\s)?(?:شهر\s)?)?(?:ال)?(?P<month>' + AR_MONTHS + r')(?:\s(?:من|ف[يى])(?:\sشهور)?)?)?' + \
-       r'\s(?P<sana>سن[ةه]|عام)' + \
        r'(?P<year>' + \
-              r'(?:\s(?P<ones>' + AR_ONES + r'))?' + \
-              r'(?:\s[و]?(?P<ten>' + AR_TEN + r'))?' + \
-              r'(?:\s[و]?(?P<hundred>' + AR_HUNDRED + r'))?' + \
+       r'\s(?P<sana>' + AR_SANA + ')' + \
+       r'(?:\s(?P<ones>' + AR_ONES + r'))?' + \
+       r'(?:\s[و]?(?P<ten>' + AR_TEN + r'))?' + \
+       r'(?:\s[و]?(?P<hundred>' + AR_HUNDRED + r'))?' + \
+       r'(?:\s[و]?(?P<thousand>' + AR_THOUSAND + r'))?' + \
        r')' + \
        r'(?=(?:' + WORD + r'|[\s\.,]|$))'
 
 DATE_PATTERN = compile(DATE)
 MONTH_PATTERN = compile(AR_MONTHS)
 
 DATE_CATEGORIES_DICT = {
```

### Comparing `eis1600-0.9.7/eis1600/dates/methods.py` & `eis1600-1.0.1/eis1600/dates/methods.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,30 +4,33 @@
 
 from openiti.helper.ara import normalize_ara_heavy
 
 from eis1600.dates.Date import Date
 from eis1600.dates.date_patterns import DATE_CATEGORIES_NOR, DATE_CATEGORY_PATTERN, DATE_PATTERN, \
     DAY_ONES_NOR, \
     DAY_TEN_NOR, MONTHS_NOR, \
-    WEEKDAYS_NOR, ONES_NOR, TEN_NOR, HUNDRED_NOR
+    WEEKDAYS_NOR, ONES_NOR, TEN_NOR, HUNDRED_NOR, THOUSAND_NOR
 from eis1600.processing.preprocessing import get_tokens_and_tags
 
 
 def parse_year(m: Match[str]) -> (int, int):
     year = 0
-    length = 1  # word sana
+    length = len(m.group('sana').split())  # (?P<sana>سنة|عام|في حدود)
     if m.group('ones'):
         year += ONES_NOR.get(normalize_ara_heavy(m.group('ones')))
         length += 1
     if m.group('ten'):
         year += TEN_NOR.get(normalize_ara_heavy(m.group('ten')))
         length += 1
     if m.group('hundred'):
         year += HUNDRED_NOR.get(normalize_ara_heavy(m.group('hundred')))
         length += len(m.group('hundred').split())
+    if m.group('thousand'):
+        year += THOUSAND_NOR.get(normalize_ara_heavy(m.group('thousand')))
+        length += 1
 
     return year, length
 
 
 def get_dates_headings(yml_handler: YAMLHandler) -> None:
     """Checks the headings for date statements and if a such a statement is found, it is converted into a tag and
     added to the yml header.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `eis1600-0.9.7/eis1600/gazetteers/Onomastics.py` & `eis1600-1.0.1/eis1600/gazetteers/Onomastics.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.7/eis1600/gazetteers/Toponyms.py` & `eis1600-1.0.1/eis1600/gazetteers/Toponyms.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.7/eis1600/gazetteers/data/onomastic_gazetteer.csv` & `eis1600-1.0.1/eis1600/gazetteers/data/onomastic_gazetteer.csv`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.7/eis1600/gazetteers/data/spelling_gazetteer.csv` & `eis1600-1.0.1/eis1600/gazetteers/data/spelling_gazetteer.csv`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.7/eis1600/gazetteers/data/toponyms_gazetteer.csv` & `eis1600-1.0.1/eis1600/gazetteers/data/toponyms_gazetteer.csv`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.7/eis1600/helper/EntityTags.py` & `eis1600-1.0.1/eis1600/helper/EntityTags.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,26 +7,26 @@
 entities_path = files('eis1600.helper.data').joinpath('entity_tags.csv')
 
 
 @Singleton
 class EntityTags:
     __entity_tags_df = None
     __tag_list = None
-    __nasab_tag_list = None
+    __onom_tag_list = None
 
     def __init__(self) -> None:
         entity_tags_df = read_csv(entities_path)
         EntityTags.__entity_tags_df = entity_tags_df
         EntityTags.__tag_list = entity_tags_df.loc[entity_tags_df['CATEGORY'].notna(), 'TAG'].to_list()
-        EntityTags.__nasab_tag_list = entity_tags_df.loc[entity_tags_df['CATEGORY'] == 'ONOMASTIC', 'TAG'].to_list()
+        EntityTags.__onom_tag_list = entity_tags_df.loc[entity_tags_df['CATEGORY'] == 'ONOMASTIC', 'TAG'].to_list()
 
     @staticmethod
     def get_entity_tags_df() -> DataFrame:
         return EntityTags.__entity_tags_df
 
     @staticmethod
     def get_entity_tags() -> List[str]:
         return EntityTags.__tag_list
 
     @staticmethod
-    def get_nasab_tags() -> List[str]:
-        return EntityTags.__nasab_tag_list
+    def get_onom_tags() -> List[str]:
+        return EntityTags.__onom_tag_list
```

### Comparing `eis1600-0.9.7/eis1600/helper/Singleton.py` & `eis1600-1.0.1/eis1600/helper/Singleton.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.7/eis1600/helper/ar_normalization.py` & `eis1600-1.0.1/eis1600/helper/ar_normalization.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.7/eis1600/helper/eval_date_model.py` & `eis1600-1.0.1/eis1600/helper/eval_date_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,36 +16,49 @@
 
 from eis1600.dates.date_patterns import DATE_CATEGORIES
 from eis1600.dates.methods import date_annotate_miu_text
 from eis1600.helper.EvalResultsEncoder import EvalResultsEncoder
 from eis1600.helper.markdown_patterns import YEAR_PATTERN
 from eis1600.helper.repo import TRAINING_DATA_REPO, TRAINING_RESULTS_REPO
 from eis1600.miu.methods import get_yml_and_miu_df
-from eis1600.markdown.md_to_bio import get_label_dict, md_to_bio
+from eis1600.markdown.md_to_bio import get_bio_dict, md_to_bio
 
 
 def reconstruct_automated_tag(row) -> str:
     return 'ÜY' + row['num_tokens'] + row['cat'] + row['written'] + 'Y'
 
 
-def get_year_true_pred(row) -> Series:
+def get_year_true_pred(row: Series) -> Series:
+    """Get numerical values for ground-truth and prediction.
+
+    :param Series row: row has values for 'written_true' and 'written_pred'.
+    :return Series: Series of 'true' and 'pred'.
+    """
     if notna(row['written_true']):
         v_true = int(row['written_true'])
     else:
         v_true = nan
 
     if notna(row['written_pred']) and row['written_pred'] != 'None':
         v_pred = int(row['written_pred'])
     else:
         v_pred = nan
 
     return Series([v_true, v_pred], index=['true', 'pred'])
 
 
-def get_dates_true_and_pred(file: str, label_dict: Dict) -> Tuple[DataFrame, Dict, Dict]:
+def get_dates_true_and_pred(file: str, bio_dict: Dict) -> Tuple[DataFrame, Dict, Dict]:
+    """Get ground-truth and prediction on labels and numerical values for MIU.
+
+    :param str file: file path for MIU file.
+    :param Dict bio_dict: BIO labels dictionary.
+    :return Tuple[DataFrame, Dict, Dict]: DataFrame year contains two columns ('true' and 'pred'), the other two are
+    dictionaries, one with the BIO labels derived from the ground-truth and the other with the BIO labels based on
+    the predictions.
+    """
     with open(file, 'r', encoding='utf-8') as miu_file_object:
         yml_handler, df = get_yml_and_miu_df(miu_file_object)
 
     # Extract the ground-truth annotated with EIS1600 tags
     s_notna = df['TAGS_LISTS'].loc[df['TAGS_LISTS'].notna()].apply(lambda tag_list: ','.join(tag_list))
     df_true = s_notna.str.extract(YEAR_PATTERN).dropna(how='all')
     dates = df_true.apply(reconstruct_automated_tag, axis=1)
@@ -78,43 +91,50 @@
 
     # Parse EIS1600 tags to BIO tags for predictions and ground-truth
     bio_true = md_to_bio(
             df[['TOKENS', 'DATES_TRUE']],
             'DATES_TRUE',
             YEAR_PATTERN,
             'YY',
-            label_dict
+            bio_dict
     )
     bio_pred = md_to_bio(
             df[['TOKENS', 'DATES_PRED']],
             'DATES_PRED',
             YEAR_PATTERN,
             'YY',
-            label_dict
+            bio_dict
     )
 
     return year, bio_true, bio_pred
 
 
-def eval_dates_entity_recognition_and_classification(truth: List[List[str]], predictions: List[List[str]]):
+def eval_dates_entity_recognition_and_classification(truth: List[List[str]], predictions: List[List[str]]) -> Dict:
     """Evaluates predicted BIO-labels based on their ground-truth.
 
     Evaluates predicted BIO-labels based on their ground-truth, giving each of the following metrics for every class:
     precision, recall, F1-score, accuracy.
 
     :param List[List[str]] truth: A list of records, where each record is a list of the true BIO-tags for that text.
     :param List[List[str]] predictions: A list of records, where each record is a list of the predicted BIO-tags for
     that text.
+    :return Dict: Dict containing the evaluation results: precision, recall, F1 for each class.
     """
     all_metrics = evaluate.load("seqeval").compute(predictions=predictions, references=truth)
 
     return all_metrics
 
 
-def eval_year(year: DataFrame):
+def eval_year(year: DataFrame) -> Dict:
+    """Evaluates the predictions of the numerical value of all recognized date with MAPE and MAE.
+
+    :param DataFrame year: DataFrame with two columns, column 'true' with the ground-truth values and column 'pred'
+    with the predicted values.
+    :return Dict: Dict containing the evaluation results: Mean Average Percentage Error and Mean Average Error.
+    """
     all_metrics = {}
     truth = constant(year['true'].astype('float32'))
     predictions = constant(year['pred'].astype('float32'))
 
     mape = MeanAbsolutePercentageError()
     mape.update_state(y_true=truth, y_pred=predictions)
     mae_no_nan = MeanAbsoluteError()
@@ -138,23 +158,24 @@
 
     with open(TRAINING_DATA_REPO + 'gold_standard.txt', 'r', encoding='utf-8') as fh:
         files_txt = fh.read().splitlines()
 
     infiles = [TRAINING_DATA_REPO + 'gold_standard/' + file for file in files_txt if Path(
             TRAINING_DATA_REPO + 'gold_standard/' + file).exists()]
 
-    label_dict = get_label_dict('YY', DATE_CATEGORIES)
+    # BIO labels for dates have this pattern: [BI]-YY[<DATE_CATEGORIES>]
+    bio_dict = get_bio_dict('YY', DATE_CATEGORIES)
 
     res = []
     if debug:
         for i, file in enumerate(infiles[1180:]):
             print(i + 1180, file)
-            res.append(get_dates_true_and_pred(file, label_dict))
+            res.append(get_dates_true_and_pred(file, bio_dict))
     else:
-        res += p_uimap(partial(get_dates_true_and_pred, label_dict=label_dict), infiles)
+        res += p_uimap(partial(get_dates_true_and_pred, label_dict=bio_dict), infiles)
 
         years, truth, predictions = zip(*res)
 
         with open(TRAINING_DATA_REPO + 'dates_truth.json', 'w', encoding='utf-8') as fh:
             dump(truth, fh, indent=4, ensure_ascii=False)
         with open(TRAINING_DATA_REPO + 'dates_predictions.json', 'w', encoding='utf-8') as fh:
             dump(predictions, fh, indent=4, ensure_ascii=False)
```

### Comparing `eis1600-0.9.7/eis1600/helper/fix_miu_annotation.py` & `eis1600-1.0.1/eis1600/helper/fix_miu_annotation.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.7/eis1600/helper/markdown_methods.py` & `eis1600-1.0.1/eis1600/helper/markdown_methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.7/eis1600/helper/markdown_patterns.py` & `eis1600-1.0.1/eis1600/helper/markdown_patterns.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,20 +46,21 @@
 TAG_AND_TEXT_SAME_LINE = r'([$@]+' + NOR_DIGIT_NOR_AR_STR + r'\d*' + NOR_DIGIT_NOR_AR_STR + r') ?((?:[(\[] ?)?' + AR_STR + r')'
 UID_TAG_AND_TEXT_SAME_LINE_PATTERN = compile(
         r'(_ء_#=\d{12}= )' + TAG_AND_TEXT_SAME_LINE)
 MIU_TAG_AND_TEXT_PATTERN = compile(r'(' + MIU_UID + r'[$@]+?(?: \d+)?)\n((?:\( ?)?' + AR_STR + r')')
 
 # MIU entity tags
 entity_tags = '|'.join(EntityTags.instance().get_entity_tags())
-ENTITY_TAGS_PATTERN = compile(r'Ü?(?P<entity>' + entity_tags + r')(?P<length>\d{1,2})(?:(?P<sub_cat>[A-Z]+)|['
-                                                               r'A-Z0-9]+)?\b')
+ENTITY_TAGS_PATTERN = compile(r'\bÜ?(?P<full_tag>'
+                              r'(?P<entity>' + entity_tags + r')(?P<length>\d{1,2})'
+                                                             r'(?:(?P<sub_cat>[A-Z]+)|['r'A-Z0-9]+)?)\b')
 YEAR_PATTERN = compile(r'Ü?Y(?P<num_tokens>\d{1,2})(?P<cat>[A-Z])(?P<written>\d{4}|None)(?P<i>I)?Y(?P<real>\d{4})?')
 AGE_PATTERN = compile(r'Ü?A\d(?P<cat>[A-Z])(?P<written>\d{2,3})(?P<i>I)?A(?P<real>\d{2,3})?')
-nasab_tags = '|'.join(EntityTags.instance().get_nasab_tags())
-NASAB_TAGS_PATTERN = compile(r'Ü?(?P<entity>' + nasab_tags + r')(?P<length>\d{1,2})')
+onom_tags = '|'.join(EntityTags.instance().get_onom_tags())
+ONOM_TAGS_PATTERN = compile(r'Ü?(?P<entity>' + onom_tags + r')(?P<length>\d{1,2})')
 
 # EIS1600 light mARkdown
 HEADING_OR_BIO_PATTERN = compile(r'# [|$]+')
 MIU_LIGHT_OR_EIS1600_PATTERN = compile(r'#|_ء_#')
 
 # Fix mARkdown files
 SPACES_CROWD_PATTERN = compile(r' +')
```

### Comparing `eis1600-0.9.7/eis1600/helper/miu_random_revisions.py` & `eis1600-1.0.1/eis1600/helper/miu_random_revisions.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.7/eis1600/helper/repo.py` & `eis1600-1.0.1/eis1600/helper/repo.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 TEXT_REPO = 'OpenITI_EIS1600_Texts/'
 TRAINING_DATA_REPO = 'Training_Data/'
 TRAINING_RESULTS_REPO = 'Training_Results/'
 GAZETTEERS_REPO = 'gazetteers/'
 MC_REPO = 'MasterChronicle/'
 BACKEND_REPO = 'backend/'
 TOPO_TRAINING_REPO = 'topo_training/data/'
+STATISTICS_REPO = 'research_data/'
 
 
 def get_entry(file_name: str, checked_entry: bool) -> str:
     """Formats README entry for that file_name.
 
     Only used internally.
     :param str file_name: The name of the file whose entry is added to the README
```

### Comparing `eis1600-0.9.7/eis1600/helper/top_tags_to_bio.py` & `eis1600-1.0.1/eis1600/helper/topo_tags_to_bio.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from re import compile
 from json import dump
 
 from p_tqdm import p_uimap
 from numpy import nan
 
 from eis1600.helper.repo import TOPO_TRAINING_REPO, TRAINING_DATA_REPO
-from eis1600.markdown.md_to_bio import get_label_dict, md_to_bio
+from eis1600.markdown.md_to_bio import get_bio_dict, md_to_bio
 from eis1600.processing.preprocessing import get_yml_and_miu_df
 from eis1600.toponyms.toponym_categories import TOPONYM_CATEGORIES
 
 CATS = ''.join(TOPONYM_CATEGORIES)
 TOP_PATTERN = compile(r"T(?P<num_tokens>\d)(?P<cat>[" + CATS + "])")
 
 
@@ -49,33 +49,32 @@
 
 def main():
     arg_parser = ArgumentParser(
             prog=argv[0], formatter_class=RawDescriptionHelpFormatter,
             description='''Script to annotate onomastic information in gold-standard MIUs.'''
     )
     arg_parser.add_argument('-D', '--debug', action='store_true')
-    arg_parser.add_argument('-K', '--keep', action='store_true')
 
     args = arg_parser.parse_args()
     debug = args.debug
-    keep = args.keep
+    keep = True
 
     with open(TRAINING_DATA_REPO + 'gold_standard.txt', 'r', encoding='utf-8') as fh:
         files_txt = fh.read().splitlines()
 
     infiles = [TRAINING_DATA_REPO + 'gold_standard_topo/' + file for file in files_txt if Path(
             TRAINING_DATA_REPO + 'gold_standard_topo/' + file).exists()]
 
-    label_dict = get_label_dict('TO', TOPONYM_CATEGORIES)
+    label_dict = get_bio_dict('TO', TOPONYM_CATEGORIES)
 
     res = []
     if debug:
-        for file in infiles[20:40]:
+        for file in infiles[40:60]:
             print(file)
-            res.append(get_tops_true(file, label_dict))
+            res.append(get_tops_true(file, label_dict, keep))
     else:
         res += p_uimap(partial(get_tops_true, label_dict=label_dict, keep_automatic_tags=keep), infiles)
 
     with open(TOPO_TRAINING_REPO + 'toponyms_category_training_data.json', 'w', encoding='utf-8') as fh:
         dump(res, fh, indent=4, ensure_ascii=False)
 
     print('Done')
```

### Comparing `eis1600-0.9.7/eis1600/helper/yml_to_json.py` & `eis1600-1.0.1/eis1600/helper/yml_to_json.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.7/eis1600/markdown/UIDs.py` & `eis1600-1.0.1/eis1600/markdown/UIDs.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.7/eis1600/markdown/convert_mARkdown_to_EIS1600TMP.py` & `eis1600-1.0.1/eis1600/markdown/convert_mARkdown_to_EIS1600TMP.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.7/eis1600/markdown/insert_uids.py` & `eis1600-1.0.1/eis1600/markdown/insert_uids.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.7/eis1600/markdown/methods.py` & `eis1600-1.0.1/eis1600/markdown/methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.7/eis1600/markdown/update_uids.py` & `eis1600-1.0.1/eis1600/markdown/update_uids.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.7/eis1600/markdown/update_uids_old_process.py` & `eis1600-1.0.1/eis1600/markdown/update_uids_old_process.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.7/eis1600/miu/HeadingTracker.py` & `eis1600-1.0.1/eis1600/miu/HeadingTracker.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
         self.h1 = None
         self.h2 = None
         self.h3 = None
         self.h4 = None
         self.page_tag = None
 
-        if headings_dict:
+        if headings_dict and type(headings_dict) == dict:
             for key, val in headings_dict.items():
                 self.__setattr__(key, val)
 
     def __iter__(self):
         """Iterate over headings which are not None. Omits page_tag."""
         for key, val in self.__dict__.items():
             if key.startswith('h') and val is not None:
```

### Comparing `eis1600-0.9.7/eis1600/miu/YAMLHandler.py` & `eis1600-1.0.1/eis1600/miu/YAMLHandler.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,16 +19,17 @@
     :ivar List[str] dates_headings: List of dates tags contained in headings.
     :ivar List[int] dates: List of dates contained in the text.
     :ivar Dict onomstics: contains onomastic elements by category.
     :ivar str category: String categorising the type of the entry, bio, chr, dict, etc.
     """
     # Only attributes named in the following list are allowed to be added to the YAMLHeader - add any new attribute
     # to that list
-    __attr_from_annotation = ['dates', 'min_date', 'max_date', 'ages', 'onomastics', 'ambiguous_toponyms', 'toponyms',
-                              'settlements', 'provinces', 'edges_settlements', 'edges_provinces', 'books', 'miscs']
+    __attr_from_annotation = ['dates', 'min_date', 'max_date', 'ages', 'onomastics', 'ambiguous_toponyms', 'persons',
+                              'toponyms', 'settlements', 'provinces', 'edges_settlements', 'edges_provinces',
+                              'books', 'miscs']
 
     @staticmethod
     def __parse_yml_val(val: str) -> Any:
         if val.isdigit():
             return int(val)
         if len(val.split('.')) == 2 and val.split('.')[0].isdigit() and val.split('.')[1].isdigit():
             return float(val)
@@ -49,14 +50,16 @@
                 values = []
                 for v in val_list:
                     t = v.split(', ')
                     values.append((YAMLHandler.__parse_yml_val(t[0]), YAMLHandler.__parse_yml_val(t[1])))
             elif raw_val_list.startswith('[') or raw_val_list.startswith('{'):
                 # Nested lists
                 values = literal_eval(val)
+            elif raw_val_list == '':
+                return None
             else:
                 # List of other values
                 val_list = raw_val_list.split(', ')
                 values = [YAMLHandler.__parse_yml_val(v) for v in val_list]
             return values
         else:
             return val
@@ -89,27 +92,36 @@
                 elif val == '':
                     # Go one level deeper, add key and empty dict for that new level
                     level.append((key, {}))
                 else:
                     # Add key, val to the top level
                     yml[key] = YAMLHandler.__parse_yml_val(val)
 
-        if len(level):
+        while len(level) > 0:
             dict_key = level[-1][0]
             dict_val = level[-1][1]
-            yml[dict_key] = dict_val
+            if len(level) > 1:
+                level[-2][1][dict_key] = dict_val
+            else:
+                yml[dict_key] = dict_val
+            level.pop()
+
+        # This is fix for old files, nas should be part of onomastics
+        if hasattr(yml, 'nas'):
+            delattr(yml, 'nas')
 
         return yml
 
     def __init__(self, yml: Optional[Dict] = None) -> None:
         self.reviewed = 'NOT REVIEWED'
         self.reviewer = None
         self.category = None
         self.headings = None
         self.dates_headings = None
+        self.number_of_tokens = None
 
         for key in YAMLHandler.__attr_from_annotation:
             if key == 'ambiguous_toponyms':
                 self.__setattr__(key, False)
             else:
                 self.__setattr__(key, None)
 
@@ -126,14 +138,17 @@
     def from_yml_str(cls, yml_str: str) -> YAMLHandler:
         """Return instance with attr set from the yml_str."""
         return cls(YAMLHandler.__parse_yml(yml_str))
 
     def set_category(self, category: str) -> None:
         self.category = category
 
+    def set_number_of_tokens(self, number_of_tokens: int) -> None:
+        self.number_of_tokens = number_of_tokens
+
     def set_ambiguous_toponyms(self) -> None:
         self.ambiguous_toponyms = True
 
     def set_headings(self, headings: HeadingTracker) -> None:
         self.headings = headings
 
     def unset_reviewed(self) -> None:
```

### Comparing `eis1600-0.9.7/eis1600/miu/disassemble_into_miu_files.py` & `eis1600-1.0.1/eis1600/miu/disassemble_into_miu_files.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.7/eis1600/miu/methods.py` & `eis1600-1.0.1/eis1600/miu/methods.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from glob import glob
 from os.path import splitext, split, exists
 from typing import List, Optional
 from pathlib import Path
 
+from eis1600.markdown.md_to_bio import bio_to_md
+
 from eis1600.dates.methods import date_annotate_miu_text
 from eis1600.helper.markdown_patterns import CATEGORY_PATTERN, HEADER_END_PATTERN, HEADING_PATTERN, MIU_TAG_PATTERN, \
     MIU_UID_PATTERN, PAGE_TAG_PATTERN
 from eis1600.miu.HeadingTracker import HeadingTracker
 from eis1600.miu.yml_handling import create_yml_header, extract_yml_header_and_text
-from eis1600.nlp.utils import camel2md_as_list, annotate_miu_text, insert_nasab_tag, insert_onomastic_tags,\
-    aggregate_STFCON_classes, merge_ner_with_person_classes
-from eis1600.onomastics.methods import nasab_annotate_miu
+from eis1600.nlp.utils import annotate_miu_text, insert_nasab_tag, insert_onomastic_tags,aggregate_STFCON_classes, \
+    merge_ner_with_person_classes, merge_ner_with_toponym_classes
 from eis1600.processing.postprocessing import write_updated_miu_to_file
 from eis1600.processing.preprocessing import get_yml_and_miu_df
-from eis1600.toponyms.methods import toponym_category_annotate_miu
 
 
 def disassemble_text(infile: str, out_path: str, verbose: Optional[bool] = None) -> None:
     """Disassemble text into MIU files.
 
     Retrieve MIU files by disassembling the text based on the EIS1600 mARkdown.
     :param str infile: Path to the file which is to be disassembled.
@@ -165,50 +165,45 @@
     if exists(tsv_path) and not force_annotation:
         return
 
     with open(path, 'r+', encoding='utf-8') as miu_file_object:
         # 1. open miu file and disassemble the file to its parts
         yml_handler, df = get_yml_and_miu_df(miu_file_object)
 
-        # 2. annotate NEs and lemmatize
-        df['NER_LABELS'], df['LEMMAS'], df['POS_TAGS'], ST_labels, FCO_labels = annotate_miu_text(df)
+        # 2. annotate NEs, POS and lemmatize. NE are: person + relation(s), toponym + relation, onomastic information
+        df['NER_LABELS'], df['LEMMAS'], df['POS_TAGS'], df['ROOTS'], ST_labels, FCO_labels, \
+            df['TOPONYM_LABELS'] = annotate_miu_text(df)
 
         # 3. convert cameltools labels format to markdown format
         aggregated_stfco_labels = aggregate_STFCON_classes(ST_labels, FCO_labels)
-        ner_tags = camel2md_as_list(df['NER_LABELS'].tolist())
-        df['NER_TAGS'] = merge_ner_with_person_classes(ner_tags, aggregated_stfco_labels)
+        ner_tags = bio_to_md(df['NER_LABELS'].to_list())  # camel2md_as_list(df['NER_LABELS'].tolist())
+        ner_tags_with_person_classes = merge_ner_with_person_classes(ner_tags, aggregated_stfco_labels)
+        toponym_labels_md = bio_to_md(df['TOPONYM_LABELS'].to_list(), sub_class=True)
+        df['NER_TAGS'] = merge_ner_with_toponym_classes(ner_tags_with_person_classes, toponym_labels_md)
 
         # 4. annotate dates
         df['DATE_TAGS'] = date_annotate_miu_text(df[['TOKENS']], yml_handler)
 
-        # 5. insert BNASAB and ENASAB tags with the pretrained transformer model
+        # 5. insert BONOM and EONOM tags with the pretrained transformer model
         df['NASAB_TAGS'] = insert_nasab_tag(df)
 
         # 6. annotate onomastic information
-        df['ONONMASTIC_TAGS'] = insert_onomastic_tags(df)
-
-        # 5. annotate onomastic information (Rule-Based model, an alternative to ML model insert_onomastic_tags
-        # df['ONONMASTIC_TAGS'] = nasab_annotate_miu(df, yml_handler, path)
-
-        # TODO 6. disambiguation of toponyms (same toponym, different places) --> replace ambigious toponyms flag
-
-        # 7. toponym categorization
-        df['NER_TAGS'] = toponym_category_annotate_miu(df['TOKENS'], df['NER_TAGS'])
+        df['ONOMASTIC_TAGS'] = insert_onomastic_tags(df)
 
-        # TODO 8. assign roles for persons
+        # TODO 6. disambiguation of toponyms (same toponym, different places) --> replace ambiguous toponyms flag
         # TODO 9. get frequencies of unidentified entities (toponyms, nisbas)
 
         # 10. save csv file
         df.to_csv(tsv_path, index=False, sep='\t')
 
         # 11. reconstruct the text, populate yml with annotated entities and save it to the output file
         if output_path == path:
             write_updated_miu_to_file(
-                miu_file_object, yml_handler, df[['SECTIONS', 'TOKENS', 'TAGS_LISTS', 'NER_TAGS',
-                                                 'DATE_TAGS', 'NASAB_TAGS', 'ONONMASTIC_TAGS']]
+                miu_file_object, yml_handler, df[['SECTIONS', 'TOKENS', 'TAGS_LISTS', 'DATE_TAGS', 'NASAB_TAGS',
+                                                  'ONOMASTIC_TAGS', 'NER_TAGS']]
                 )
         else:
             with open(output_path, 'w', encoding='utf-8') as out_file_object:
                 write_updated_miu_to_file(
-                        out_file_object, yml_handler, df[['SECTIONS', 'TOKENS', 'TAGS_LISTS', 'NER_TAGS',
-                                                         'DATE_TAGS', 'NASAB_TAGS', 'ONONMASTIC_TAGS']]
+                        out_file_object, yml_handler, df[['SECTIONS', 'TOKENS', 'TAGS_LISTS', 'DATE_TAGS', 'NASAB_TAGS',
+                                                          'ONOMASTIC_TAGS', 'NER_TAGS']]
                 )
```

### Comparing `eis1600-0.9.7/eis1600/miu/reassemble_from_miu_files.py` & `eis1600-1.0.1/eis1600/miu/reassemble_from_miu_files.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.7/eis1600/miu/yml_handling.py` & `eis1600-1.0.1/eis1600/miu/yml_handling.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from itertools import combinations
+from operator import itemgetter
 from os import makedirs
 from os.path import dirname, split, splitext
 from typing import Dict, List, Optional, Set, TextIO, Tuple, Union
 
+from pandas import DataFrame, notna
+
 from eis1600.gazetteers.Toponyms import Toponyms
 from eis1600.helper.EntityTags import EntityTags
 from eis1600.helper.logging import setup_logger
 from eis1600.helper.markdown_methods import get_yrs_tag_value
 from eis1600.helper.markdown_patterns import ENTITY_TAGS_PATTERN, MIU_HEADER_PATTERN, NEWLINES_CROWD_PATTERN
 from eis1600.helper.repo import GAZETTEERS_REPO
 from eis1600.miu.HeadingTracker import HeadingTracker
@@ -82,75 +85,81 @@
     """
     cat = cat.lower() + 's'
     if tag:
         tag = tag.lower()
     if cat in entities_dict.keys():
         if cat == 'onomastics' and tag:
             if tag in entities_dict[cat].keys():
-                entities_dict[cat][tag].append(entity)
+                entities_dict[cat][tag].add(entity)
             else:
-                entities_dict[cat][tag] = [entity]
+                entities_dict[cat][tag] = {entity}
         else:
             entities_dict[cat].append(entity)
     else:
         if cat == 'onomastics' and tag:
             entities_dict[cat] = {}
-            entities_dict[cat][tag] = [entity]
+            entities_dict[cat][tag] = {entity}
         elif isinstance(entity, list):
             entities_dict[cat] = entity
         else:
             entities_dict[cat] = [entity]
 
 
 def add_annotated_entities_to_yml(
-        text_with_tags: str,
+        df: DataFrame,
         yml_handler: YAMLHandler,
         file_path: str,
 ) -> None:
     """Populates YAMLHeader with annotated entities.
 
     Extract annotated entities as metadata. While doing so, identify toponyms and calculate active period for the
     biographee.
-    :param str text_with_tags: Text with inserted tags of the MIU.
+    :param DataFrame df: DataFrame with two columns 'TAGS_LISTS' and 'TOKENS'.
     :param YAMLHandler yml_handler: YAMLHandler of the MIU.
     :param str file_path: Filename of the current MIU (used in error msg).
     """
     # We do not need to differentiate between automated and manual tags
-    text_with_tags = text_with_tags.replace('Ü', '')
     tg = Toponyms.instance()
     entity_tags_df = EntityTags.instance().get_entity_tags_df()
     entities_dict = {}
     nas_dict = {}
     nas_counter = 0
     settlements_set: Set[str] = set()
     provinces_set: Set[str] = set()
     ambiguous_toponyms = False
 
-    m = ENTITY_TAGS_PATTERN.search(text_with_tags)
-    while m:
-        tag = m.group('entity')
-        length = int(m.group('length'))
-        sub_cat = None
-        if m.group('sub_cat'):
-            # Person, toponyms and books are sub-classified based on their relation to the biographee
-            sub_cat = m.group('sub_cat')
-        entity = ' '.join(text_with_tags[m.end():].split(maxsplit=length)[:length])
-
+    # Get all tags with their information extracted into individual elements
+    s_notna = df['TAGS_LISTS'].loc[df['TAGS_LISTS'].notna()].apply(lambda tag_list: ','.join(tag_list))
+    df_matches = s_notna.str.extractall(ENTITY_TAGS_PATTERN).dropna(how='all')
+
+    # Interpret extracted information for each tag
+    for index_tuple, row in df_matches.iterrows():
+        # Since there can be multiple tags for the same tokens df_matches has a multi-index
+        index = index_tuple[0]
+        tag = row['entity']
+        length = int(row['length'])
+        sub_cat = row['sub_cat']
+        try:
+            entity = ' '.join(df['TOKENS'].iloc[index:index+length].to_list())
+        except TypeError:
+            print(f'Something is at odd here: {row["full_tag"]}\nCheck: {file_path}')
+            return
         cat = entity_tags_df.loc[entity_tags_df['TAG'].str.fullmatch(tag), 'CATEGORY'].iloc[0]
+
         if cat == 'DATE' or cat == 'AGE':
             try:
-                val, e_cat = get_yrs_tag_value(m.group(0))
+                val, e_cat = get_yrs_tag_value(row['full_tag'])
                 add_to_entities_dict(entities_dict, cat, {'entity': entity, cat.lower(): val, 'cat': e_cat})
             except ValueError:
-                print(f'Tag is neither year nor age: {m.group(0)}\nCheck: {file_path}')
+                print(f'Tag is neither year nor age: {row["full_tag"]}\nCheck: {file_path}')
                 return
         elif cat == 'TOPONYM':
             # Identify toponym
             place, uris_tag, list_of_uris, list_of_provinces = tg.look_up_entity(entity)
-            if sub_cat:
+            if notna(sub_cat):
                 add_to_entities_dict(entities_dict, cat, {'entity': place, 'URI': uris_tag, 'cat': sub_cat})
             else:
                 add_to_entities_dict(entities_dict, cat, {'entity': place, 'URI': uris_tag})
             if len(list_of_uris) == 0:
                 path, uri = split(file_path)
                 uri, ext = splitext(uri)
                 LOGGER_TOPONYMS_UNKNOWN.info(f'{uri},{entity}')
@@ -168,33 +177,35 @@
         elif cat == 'ONOMASTIC':
             if tag.startswith('SHR') and entity.startswith('ب'):
                 entity = entity[1:]
                 add_to_entities_dict(entities_dict, cat, entity, tag)
             elif tag.startswith('NAS'):
                 nas_dict['nas_' + str(nas_counter)] = entity
                 nas_counter += 1
-            add_to_entities_dict(entities_dict, cat, entity, tag)
+            else:
+                add_to_entities_dict(entities_dict, cat, entity, tag)
             LOGGER_NASAB_KNOWN.info(f'{tag},{entity}')
         elif cat == 'BOOK':
-            if sub_cat:
+            if notna(sub_cat):
                 add_to_entities_dict(entities_dict, cat, {'entity': entity, 'cat': sub_cat}, tag)
         else:
             add_to_entities_dict(entities_dict, cat, entity, tag)
 
-        m = ENTITY_TAGS_PATTERN.search(text_with_tags, m.end())
-
     if nas_dict != {}:
         if 'onomastics' in entities_dict.keys():
             entities_dict['onomastics']['nas'] = nas_dict
         else:
             entities_dict['onomastics'] = {'nas': nas_dict}
 
     if 'onomastics' in entities_dict.keys():
         # Sort dict by keys
-        entities_dict['onomastics'] = dict(sorted(entities_dict.get('onomastics').items()))
+        entities_dict['onomastics'] = dict(sorted(
+                [(k, list(v)) if isinstance(v, set) else (k, v) for k,  v in entities_dict.get('onomastics').items()],
+                key=itemgetter(0)
+        ))
 
     # Generate edges
     if settlements_set:
         entities_dict['settlements'] = list(settlements_set)
         entities_dict['edges_settlements'] = [[a, b] for a, b in combinations(settlements_set, 2) if a != b]
     if provinces_set:
         entities_dict['provinces'] = list(provinces_set)
```

### Comparing `eis1600-0.9.7/eis1600/nlp/cameltools.py` & `eis1600-1.0.1/eis1600/nlp/cameltools.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 from camel_tools.ner import NERecognizer
 from camel_tools.tokenizers.word import simple_word_tokenize
 from camel_tools.disambig.mle import MLEDisambiguator
 from camel_tools.tagger.default import DefaultTagger
 from camel_tools.utils.dediac import dediac_ar
-from typing import Union
+from typing import Iterator, Tuple, Union
 
 
 class CamelToolsModels:
     __pos_tagger = None
     __mled_disambiguator = None
     __lemmatizer = None
     __ner_tagger = None
     __nasab_tagger = None
     __onomastic_tagger = None
     __st_tagger = None
     __fco_tagger = None
+    __toponym_tagger = None
 
     __NASAB_MODEL_PATH = "EIS1600_Pretrained_Models/camelbert-ca-finetuned_nasab/"
     __NER_MODEL_PATH = "EIS1600_Pretrained_Models/camelbert-ca-finetuned_ner/"
     __ONOMASTIC_MODEL_PATH = "EIS1600_Pretrained_Models/camelbert-ca-finetuned_onomastic/"
-    __STN_MODEL_PATH = "EIS1600_Pretrained_Models/camelbert-ca-finetuned_onomastic/"
-    __FCON_MODEL_PATH = "EIS1600_Pretrained_Models/camelbert-ca-finetuned_onomastic/"
-
+    __STN_MODEL_PATH = "EIS1600_Pretrained_Models/camelbert-ca-finetuned_person_classification_STN/"
+    __FCON_MODEL_PATH = "EIS1600_Pretrained_Models/camelbert-ca-finetuned_person_classification_FCN/"
+    __TOPO_MODEL_PATH = "EIS1600_Pretrained_Models/camelbert-ca-finetuned_toponyms/"
 
     @staticmethod
     def getInstance():
         """ Static access method. """
         if CamelToolsModels.__ner_tagger is None or CamelToolsModels.__lemmatizer is None:
             CamelToolsModels()
-        return CamelToolsModels.__ner_tagger, CamelToolsModels.__lemmatizer, CamelToolsModels.__pos_tagger,\
-            CamelToolsModels.__st_tagger, CamelToolsModels.__fco_tagger
+        return CamelToolsModels.__mled_disambiguator, CamelToolsModels.__ner_tagger, CamelToolsModels.__lemmatizer, \
+               CamelToolsModels.__pos_tagger, CamelToolsModels.__st_tagger, CamelToolsModels.__fco_tagger, \
+               CamelToolsModels.__toponym_tagger
 
     @staticmethod
     def getNasabModel():
         """ Static access method. """
         if CamelToolsModels.__nasab_tagger is None:
             CamelToolsModels.__nasab_tagger = NERecognizer(CamelToolsModels.__NASAB_MODEL_PATH)
         return CamelToolsModels.__nasab_tagger
@@ -49,28 +51,34 @@
         """ Virtually private constructor. """
         if CamelToolsModels.__ner_tagger is not None:
             raise Exception("This class is a singleton!")
         else:
             CamelToolsModels.__mled_disambiguator = MLEDisambiguator.pretrained()
             CamelToolsModels.__lemmatizer = DefaultTagger(CamelToolsModels.__mled_disambiguator, 'lex')
             CamelToolsModels.__pos_tagger = DefaultTagger(CamelToolsModels.__mled_disambiguator, 'pos')
-            CamelToolsModels.__ner_tagger = NERecognizer(CamelToolsModels.__NER_MODEL_PATH) # .pretrained
+            CamelToolsModels.__ner_tagger = NERecognizer(CamelToolsModels.__NER_MODEL_PATH)  # .pretrained
             CamelToolsModels.__st_tagger = NERecognizer(CamelToolsModels.__STN_MODEL_PATH)
             CamelToolsModels.__fco_tagger = NERecognizer(CamelToolsModels.__FCON_MODEL_PATH)
+            CamelToolsModels.__toponym_tagger = NERecognizer(CamelToolsModels.__TOPO_MODEL_PATH)
+
 
-def lemmatize_and_tag_ner(tokens: Union[str, list]) -> list:
+def lemmatize_and_tag_ner(tokens: Union[str, list]) -> Iterator[Tuple[str, ...]]:
     """Lemmatize the text and annotate named-entities.
 
-        Lemmatize the text and annotated named-entities using Camel Tools models.
-        :param tokens: a  string or a list of tokens to be annotated
-        """
-    ner_tagger, lemmatizer, pos_tagger, st_tager, fco_tagger = CamelToolsModels.getInstance()
+    Lemmatize the text and annotated named-entities using Camel Tools models.
+    :param tokens: a  string or a list of tokens to be annotated
+    """
+    mled_disambiguator, ner_tagger, lemmatizer, pos_tagger, st_tager, fco_tagger, toponym_tagger = \
+        CamelToolsModels.getInstance()
     # if tokens is a string, then tokenize it
     if isinstance(tokens, str):
         tokens = simple_word_tokenize(tokens)
     ner_labels = ner_tagger.predict_sentence(tokens)
     st_labels = st_tager.predict_sentence(tokens)
     fco_labels = fco_tagger.predict_sentence(tokens)
+    toponym_labels = toponym_tagger.predict_sentence(tokens)
     lemmas = lemmatizer.tag(tokens)
     pos_tags = pos_tagger.tag(tokens)
+    root_tags = [d.analyses[0].analysis['root'] for d in mled_disambiguator.disambiguate(tokens)]
     dediac_lemmas = [dediac_ar(lemma) for lemma in lemmas]
-    return list(zip(tokens, ner_labels, lemmas, dediac_lemmas, pos_tags, st_labels, fco_labels))
+
+    return zip(tokens, ner_labels, lemmas, dediac_lemmas, pos_tags, root_tags, st_labels, fco_labels, toponym_labels)
```

### Comparing `eis1600-0.9.7/eis1600/nlp/ner_annotate_mius.py` & `eis1600-1.0.1/eis1600/nlp/ner_annotate_mius.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.7/eis1600/onomastics/annotation.py` & `eis1600-1.0.1/eis1600/onomastics/annotation.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.7/eis1600/onomastics/methods.py` & `eis1600-1.0.1/eis1600/onomastics/methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.7/eis1600/onomastics/re_pattern.py` & `eis1600-1.0.1/eis1600/onomastics/re_pattern.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.7/eis1600/processing/postprocessing.py` & `eis1600-1.0.1/eis1600/processing/postprocessing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from typing import Iterator, List, TextIO, Tuple, Union
 
 from os import path
 from pandas import DataFrame, notna
-from camel_tools.utils.charsets import UNICODE_PUNCT_CHARSET
 
 from eis1600.helper.markdown_patterns import ENTITY_TAGS_PATTERN
 from eis1600.miu.YAMLHandler import YAMLHandler
 from eis1600.miu.yml_handling import add_annotated_entities_to_yml
 
 
 def get_text_with_annotation_only(
@@ -56,18 +55,15 @@
     # TODO NASAB tag after token
     for section, token, tags in text_and_tags_iter:
         if notna(section):
             reconstructed_text += '\n\n' + section + '\n_ء_'
         if isinstance(tags, list):
             reconstructed_text += ' ' + ' '.join(tags)
         if notna(token):
-            if token in UNICODE_PUNCT_CHARSET:
-                reconstructed_text += token
-            else:
-                reconstructed_text += ' ' + token
+            reconstructed_text += ' ' + token
 
     reconstructed_text += '\n\n'
     reconstructed_text = reconstructed_text.replace(' NEWLINE ', '\n_ء_ ')
     reconstructed_text = reconstructed_text.replace('HEMISTICH', '%~%')
     return reconstructed_text
 
 
@@ -86,27 +82,25 @@
         yml_handler: YAMLHandler,
         df: DataFrame,
 ) -> None:
     """Write MIU file with annotations and populated YAML header.
 
     :param TextIO miu_file_object: Path to the MIU file to write
     :param YAMLHandler yml_handler: The YAMLHandler of the MIU.
-    :param DataFrame df: df containing the columns ['SECTIONS', 'TOKENS', 'TAGS_LISTS'] and optional 'ÜTAGS_LISTS'.
+    :param DataFrame df: df containing the columns ['SECTIONS', 'TOKENS', 'TAGS_LISTS'].
     :return None:
     """
     if not yml_handler.is_reviewed():
-        columns_of_automated_tags = ['NER_TAGS', 'DATE_TAGS', 'NASAB_TAGS', 'ONONMASTIC_TAGS']
-        df['ÜTAGS'] = df['TAGS_LISTS']
+        columns_of_automated_tags = ['DATE_TAGS', 'NASAB_TAGS', 'ONOMASTIC_TAGS', 'NER_TAGS']
         for col in columns_of_automated_tags:
             if col in df.columns:
-                df['ÜTAGS'] = df.apply(lambda x: merge_tagslists(x['ÜTAGS'], x[col]), axis=1)
-        df_subset = df[['SECTIONS', 'TOKENS', 'ÜTAGS']]
+                df['TAGS_LISTS'] = df.apply(lambda x: merge_tagslists(x['TAGS_LISTS'], x[col]), axis=1)
+        df_subset = df[['SECTIONS', 'TOKENS', 'TAGS_LISTS']]
     else:
         df_subset = df[['SECTIONS', 'TOKENS', 'TAGS_LISTS']]
 
-    text_with_tags = get_text_with_annotation_only(df_subset)
-    add_annotated_entities_to_yml(text_with_tags, yml_handler, path.realpath(miu_file_object.name))
+    add_annotated_entities_to_yml(df_subset, yml_handler, path.realpath(miu_file_object.name))
     updated_text = reconstruct_miu_text_with_tags(df_subset)
 
     miu_file_object.seek(0)
     miu_file_object.write(str(yml_handler) + updated_text)
     miu_file_object.truncate()
```

### Comparing `eis1600-0.9.7/eis1600/processing/preprocessing.py` & `eis1600-1.0.1/eis1600/processing/preprocessing.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.7/eis1600/stats/methods.py` & `eis1600-1.0.1/eis1600/stats/methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.7/eis1600/stats/miu_stats.py` & `eis1600-1.0.1/eis1600/stats/miu_stats.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.7/eis1600/toponyms/annotation.py` & `eis1600-1.0.1/eis1600/toponyms/annotation.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.7/eis1600/toponyms/methods.py` & `eis1600-1.0.1/eis1600/toponyms/methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.7/eis1600/toponyms/toponym_categories.py` & `eis1600-1.0.1/eis1600/toponyms/toponym_categories.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.7/eis1600.egg-info/PKG-INFO` & `eis1600-1.0.1/eis1600.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eis1600
-Version: 0.9.7
+Version: 1.0.1
 Summary: EIS1600 project tools and utilities
 Home-page: https://github.com/EIS1600/eis1600-pkg
 Author: Lisa Mischer
 Author-email: mischer.lisa@gmail.com
 License: MIT License
 Description: # EIS1600 Tools
```

### Comparing `eis1600-0.9.7/eis1600.egg-info/SOURCES.txt` & `eis1600-1.0.1/eis1600.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -12,30 +12,34 @@
 eis1600/dates/__init__.py
 eis1600/dates/date_patterns.py
 eis1600/dates/methods.py
 eis1600/gazetteers/Onomastics.py
 eis1600/gazetteers/Toponyms.py
 eis1600/gazetteers/__init__.py
 eis1600/gazetteers/data/__init__.py
+eis1600/gazetteers/data/days_gazetteer.csv
+eis1600/gazetteers/data/months_gazetteer.csv
 eis1600/gazetteers/data/onomastic_gazetteer.csv
 eis1600/gazetteers/data/spelling_gazetteer.csv
 eis1600/gazetteers/data/toponyms_gazetteer.csv
+eis1600/gazetteers/data/years_gazetteer.csv
 eis1600/helper/EntityTags.py
 eis1600/helper/EvalResultsEncoder.py
 eis1600/helper/Singleton.py
 eis1600/helper/__init__.py
 eis1600/helper/ar_normalization.py
 eis1600/helper/eval_date_model.py
 eis1600/helper/fix_miu_annotation.py
+eis1600/helper/fix_ono_p_tags_order.py
 eis1600/helper/logging.py
 eis1600/helper/markdown_methods.py
 eis1600/helper/markdown_patterns.py
 eis1600/helper/miu_random_revisions.py
 eis1600/helper/repo.py
-eis1600/helper/top_tags_to_bio.py
+eis1600/helper/topo_tags_to_bio.py
 eis1600/helper/yml_methods.py
 eis1600/helper/yml_to_json.py
 eis1600/helper/data/__init__.py
 eis1600/helper/data/entity_tags.csv
 eis1600/markdown/UIDs.py
 eis1600/markdown/__init__.py
 eis1600/markdown/convert_mARkdown_to_EIS1600TMP.py
@@ -58,14 +62,17 @@
 eis1600/onomastics/__init__.py
 eis1600/onomastics/annotation.py
 eis1600/onomastics/methods.py
 eis1600/onomastics/re_pattern.py
 eis1600/processing/__init__.py
 eis1600/processing/postprocessing.py
 eis1600/processing/preprocessing.py
+eis1600/statistics/__init__.py
+eis1600/statistics/count_tokens_per_miu.py
+eis1600/statistics/methods.py
 eis1600/stats/__init__.py
 eis1600/stats/methods.py
 eis1600/stats/miu_stats.py
 eis1600/toponyms/__init__.py
 eis1600/toponyms/annotation.py
 eis1600/toponyms/methods.py
 eis1600/toponyms/toponym_categories.py
```

### Comparing `eis1600-0.9.7/setup.py` & `eis1600-1.0.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='eis1600',
-      version='0.9.7',
+      version='1.0.1',
       description='EIS1600 project tools and utilities',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='https://github.com/EIS1600/eis1600-pkg',
       author='Lisa Mischer',
       author_email='mischer.lisa@gmail.com',
       license='MIT License',
       packages=find_packages(include=['eis1600', 'eis1600.*'], exclude=['excluded']),
       package_data={'eis1600.gazetteers.data': ['*.csv'], 'eis1600.helper.data': ['*.csv']},
       entry_points={
           'console_scripts': [
                   'annotate_mius = eis1600.nlp.ner_annotate_mius:main [NER]',
                   'convert_mARkdown_to_EIS1600TMP = eis1600.markdown.convert_mARkdown_to_EIS1600TMP:main',
+                  'count_tokens_per_miu = eis1600.statistics.count_tokens_per_miu:main',
                   'disassemble_into_miu_files = eis1600.miu.disassemble_into_miu_files:main',
                   'eval_date_model = eis1600.helper.eval_date_model:main [EVAL]',
+                  'fix_ono_p_tags_order = eis1600.helper.fix_ono_p_tags_order:main',
                   'fix_miu_annotation = eis1600.helper.fix_miu_annotation:main',
                   'insert_uids = eis1600.markdown.insert_uids:main',
-                  'top_tags_to_bio = eis1600.helper.top_tags_to_bio:main',
+                  'topo_tags_to_bio = eis1600.helper.topo_tags_to_bio:main',
                   'miu_random_revisions = eis1600.helper.miu_random_revisions:main',
                   'miu_stats = eis1600.stats.miu_stats:main',
                   'onomastic_annotation = eis1600.onomastics.annotation:main',
                   'toponym_annotation = eis1600.toponyms.annotation:main',
                   'reassemble_from_miu_files = eis1600.miu.reassemble_from_miu_files:main',
                   'update_uids = eis1600.markdown.update_uids:main',
                   'xx_update_uids_old_process = eis1600.markdown.update_uids_old_process:main',
@@ -39,14 +41,14 @@
               'pandas',
               'numpy',
               'tqdm',
               'p_tqdm',
               'importlib_resources',
               'jsonpickle'
       ],
-      extras_require={'NER': ['camel-tools'], 'EVAL': ['evaluate', 'seqeval']},
+      extras_require={'NER': ['camel-tools'], 'EVAL': ['evaluate', 'seqeval', 'tensorflow']},
       classifiers=['Programming Language :: Python :: 3',
                    'License :: OSI Approved :: MIT License',
                    'Operating System :: OS Independent',
                    'Development Status :: 1 - Planning',
                    'Intended Audience :: Science/Research']
       )
```

