# Comparing `tmp/zhousf-lib-0.9.2.tar.gz` & `tmp/zhousf-lib-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhousf-lib-0.9.2.tar", last modified: Tue Jul 25 08:05:06 2023, max compression
+gzip compressed data, was "zhousf-lib-0.9.3.tar", last modified: Fri Aug  4 01:40:33 2023, max compression
```

## Comparing `zhousf-lib-0.9.2.tar` & `zhousf-lib-0.9.3.tar`

### file list

```diff
@@ -1,93 +1,94 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 08:05:06.483425 zhousf-lib-0.9.2/
--rw-rw-rw-   0        0        0     1086 2023-06-06 02:24:10.000000 zhousf-lib-0.9.2/LICENSE
--rw-rw-rw-   0        0        0     2073 2023-07-25 08:05:06.482423 zhousf-lib-0.9.2/PKG-INFO
--rw-rw-rw-   0        0        0     1179 2023-06-09 06:54:16.000000 zhousf-lib-0.9.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-25 08:05:06.483425 zhousf-lib-0.9.2/setup.cfg
--rw-rw-rw-   0        0        0     4289 2023-07-25 08:05:02.000000 zhousf-lib-0.9.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-25 08:05:06.396455 zhousf-lib-0.9.2/zhousf_lib.egg-info/
--rw-rw-rw-   0        0        0     2073 2023-07-25 08:05:06.000000 zhousf-lib-0.9.2/zhousf_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2341 2023-07-25 08:05:06.000000 zhousf-lib-0.9.2/zhousf_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 08:05:06.000000 zhousf-lib-0.9.2/zhousf_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-25 08:05:06.000000 zhousf-lib-0.9.2/zhousf_lib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-25 08:05:06.397424 zhousf-lib-0.9.2/zhousflib/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:49:13.000000 zhousf-lib-0.9.2/zhousflib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 08:05:06.398424 zhousf-lib-0.9.2/zhousflib/datasets/
--rw-rw-rw-   0        0        0       84 2023-06-06 02:39:10.000000 zhousf-lib-0.9.2/zhousflib/datasets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 08:05:06.400425 zhousf-lib-0.9.2/zhousflib/datasets/classification/
--rw-rw-rw-   0        0        0       73 2023-06-07 01:45:12.000000 zhousf-lib-0.9.2/zhousflib/datasets/classification/__init__.py
--rw-rw-rw-   0        0        0     4895 2023-06-13 08:58:42.000000 zhousf-lib-0.9.2/zhousflib/datasets/classification/classification_dataset_split.py
-drwxrwxrwx   0        0        0        0 2023-07-25 08:05:06.406423 zhousf-lib-0.9.2/zhousflib/datasets/coco/
--rw-rw-rw-   0        0        0       73 2023-07-11 01:24:38.000000 zhousf-lib-0.9.2/zhousflib/datasets/coco/__init__.py
--rw-rw-rw-   0        0        0     8251 2023-06-07 07:58:31.000000 zhousf-lib-0.9.2/zhousflib/datasets/coco/coco_bbox_extract.py
--rw-rw-rw-   0        0        0     5484 2023-06-12 06:00:08.000000 zhousf-lib-0.9.2/zhousflib/datasets/coco/coco_bbox_update.py
--rw-rw-rw-   0        0        0     6637 2023-06-08 02:33:01.000000 zhousf-lib-0.9.2/zhousflib/datasets/coco/coco_bbox_vis.py
--rw-rw-rw-   0        0        0     2896 2023-06-07 07:55:47.000000 zhousf-lib-0.9.2/zhousflib/datasets/coco/coco_dataset_merge.py
--rw-rw-rw-   0        0        0     6278 2023-06-09 06:13:45.000000 zhousf-lib-0.9.2/zhousflib/datasets/coco/coco_dataset_split.py
-drwxrwxrwx   0        0        0        0 2023-07-25 08:05:06.412424 zhousf-lib-0.9.2/zhousflib/datasets/labelme/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:45:12.000000 zhousf-lib-0.9.2/zhousflib/datasets/labelme/__init__.py
--rw-rw-rw-   0        0        0     3825 2023-06-07 01:45:12.000000 zhousf-lib-0.9.2/zhousflib/datasets/labelme/labelme_clip.py
--rw-rw-rw-   0        0        0     8090 2023-06-07 01:45:12.000000 zhousf-lib-0.9.2/zhousflib/datasets/labelme/labelme_convert_coco.py
--rw-rw-rw-   0        0        0     9622 2023-06-06 09:07:37.000000 zhousf-lib-0.9.2/zhousflib/datasets/labelme/labelme_convert_seg.py
--rw-rw-rw-   0        0        0     3827 2023-06-07 01:45:12.000000 zhousf-lib-0.9.2/zhousflib/datasets/labelme/labelme_dataset_clip.py
-drwxrwxrwx   0        0        0        0 2023-07-25 08:05:06.414423 zhousf-lib-0.9.2/zhousflib/datasets/segmentation/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:45:12.000000 zhousf-lib-0.9.2/zhousflib/datasets/segmentation/__init__.py
--rw-rw-rw-   0        0        0     2871 2023-06-06 09:07:37.000000 zhousf-lib-0.9.2/zhousflib/datasets/segmentation/seg_dataset_split.py
-drwxrwxrwx   0        0        0        0 2023-07-25 08:05:06.416450 zhousf-lib-0.9.2/zhousflib/datasets/uiex/
--rw-rw-rw-   0        0        0       60 2023-07-24 09:12:22.000000 zhousf-lib-0.9.2/zhousflib/datasets/uiex/__init__.py
--rw-rw-rw-   0        0        0     4363 2023-07-25 02:02:21.000000 zhousf-lib-0.9.2/zhousflib/datasets/uiex/labelme_convert_uiex.py
-drwxrwxrwx   0        0        0        0 2023-07-25 08:05:06.418449 zhousf-lib-0.9.2/zhousflib/db/
--rw-rw-rw-   0        0        0       60 2023-06-15 07:08:53.000000 zhousf-lib-0.9.2/zhousflib/db/__init__.py
--rw-rw-rw-   0        0        0     2343 2023-06-15 07:08:53.000000 zhousf-lib-0.9.2/zhousflib/db/lmdb_master.py
-drwxrwxrwx   0        0        0        0 2023-07-25 08:05:06.421457 zhousf-lib-0.9.2/zhousflib/decorator/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:45:12.000000 zhousf-lib-0.9.2/zhousflib/decorator/__init__.py
--rw-rw-rw-   0        0        0      504 2023-07-18 05:47:21.000000 zhousf-lib-0.9.2/zhousflib/decorator/except_util.py
--rw-rw-rw-   0        0        0     1094 2023-06-07 01:49:12.000000 zhousf-lib-0.9.2/zhousflib/decorator/interceptor_util.py
-drwxrwxrwx   0        0        0        0 2023-07-25 08:05:06.424424 zhousf-lib-0.9.2/zhousflib/download/
--rw-rw-rw-   0        0        0       60 2023-06-16 08:05:46.000000 zhousf-lib-0.9.2/zhousflib/download/__init__.py
--rw-rw-rw-   0        0        0     4646 2023-06-16 08:07:58.000000 zhousf-lib-0.9.2/zhousflib/download/download_util.py
-drwxrwxrwx   0        0        0        0 2023-07-25 08:05:06.439425 zhousf-lib-0.9.2/zhousflib/font/
--rw-rw-rw-   0        0        0 15320040 2023-03-31 01:19:09.000000 zhousf-lib-0.9.2/zhousflib/font/SimSun.ttf
--rw-rw-rw-   0        0        0  2152796 2023-03-31 01:19:09.000000 zhousf-lib-0.9.2/zhousflib/font/Symbola.ttf
--rw-rw-rw-   0        0        0      763 2023-06-09 05:53:49.000000 zhousf-lib-0.9.2/zhousflib/font/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 08:05:06.443423 zhousf-lib-0.9.2/zhousflib/locust/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:49:12.000000 zhousf-lib-0.9.2/zhousflib/locust/__init__.py
--rw-rw-rw-   0        0        0     1521 2023-06-15 07:08:53.000000 zhousf-lib-0.9.2/zhousflib/locust/locust_demo.py
-drwxrwxrwx   0        0        0        0 2023-07-25 08:05:06.446423 zhousf-lib-0.9.2/zhousflib/pandas/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:49:13.000000 zhousf-lib-0.9.2/zhousflib/pandas/__init__.py
--rw-rw-rw-   0        0        0     4761 2023-06-19 03:04:32.000000 zhousf-lib-0.9.2/zhousflib/pandas/openpyxl_util.py
--rw-rw-rw-   0        0        0     5872 2023-06-19 03:04:56.000000 zhousf-lib-0.9.2/zhousflib/pandas/pandas_util.py
-drwxrwxrwx   0        0        0        0 2023-07-25 08:05:06.448425 zhousf-lib-0.9.2/zhousflib/pdf/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:49:12.000000 zhousf-lib-0.9.2/zhousflib/pdf/__init__.py
--rw-rw-rw-   0        0        0     1845 2023-06-07 01:49:12.000000 zhousf-lib-0.9.2/zhousflib/pdf/export_image.py
--rw-rw-rw-   0        0        0     1465 2023-06-15 07:08:53.000000 zhousf-lib-0.9.2/zhousflib/pdf/pdfplumber_util.py
-drwxrwxrwx   0        0        0        0 2023-07-25 08:05:06.452424 zhousf-lib-0.9.2/zhousflib/so/
--rw-rw-rw-   0        0        0       85 2023-06-29 06:08:24.000000 zhousf-lib-0.9.2/zhousflib/so/__init__.py
--rw-rw-rw-   0        0        0     3736 2023-06-27 03:01:19.000000 zhousf-lib-0.9.2/zhousflib/so/project_to_so.py
--rw-rw-rw-   0        0        0      273 2023-06-27 03:01:19.000000 zhousf-lib-0.9.2/zhousflib/so/py_to_so.py
-drwxrwxrwx   0        0        0        0 2023-07-25 08:05:06.477425 zhousf-lib-0.9.2/zhousflib/util/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:49:12.000000 zhousf-lib-0.9.2/zhousflib/util/__init__.py
--rw-rw-rw-   0        0        0     3151 2023-07-19 06:01:50.000000 zhousf-lib-0.9.2/zhousflib/util/calculater_util.py
--rw-rw-rw-   0        0        0     2067 2023-06-27 02:49:36.000000 zhousf-lib-0.9.2/zhousflib/util/char_util.py
--rw-rw-rw-   0        0        0      635 2023-06-07 01:49:12.000000 zhousf-lib-0.9.2/zhousflib/util/cv_util.py
--rw-rw-rw-   0        0        0     2609 2023-06-16 08:07:58.000000 zhousf-lib-0.9.2/zhousflib/util/dict_util.py
--rw-rw-rw-   0        0        0     2193 2023-06-07 01:49:13.000000 zhousf-lib-0.9.2/zhousflib/util/encrypt_util.py
--rw-rw-rw-   0        0        0     1593 2023-06-29 06:32:27.000000 zhousf-lib-0.9.2/zhousflib/util/img_util.py
--rw-rw-rw-   0        0        0    13590 2023-07-18 09:25:11.000000 zhousf-lib-0.9.2/zhousflib/util/iou_util.py
--rw-rw-rw-   0        0        0     3373 2023-06-07 01:49:12.000000 zhousf-lib-0.9.2/zhousflib/util/json_util.py
--rw-rw-rw-   0        0        0     1907 2023-07-19 06:44:54.000000 zhousf-lib-0.9.2/zhousflib/util/list_util.py
--rw-rw-rw-   0        0        0     1432 2023-06-16 08:43:33.000000 zhousf-lib-0.9.2/zhousflib/util/math_util.py
--rw-rw-rw-   0        0        0     1358 2023-06-07 01:49:12.000000 zhousf-lib-0.9.2/zhousflib/util/permission_util.py
--rw-rw-rw-   0        0        0     3524 2023-06-07 01:49:11.000000 zhousf-lib-0.9.2/zhousflib/util/poly_util.py
--rw-rw-rw-   0        0        0      502 2023-06-16 08:10:19.000000 zhousf-lib-0.9.2/zhousflib/util/random_util.py
--rw-rw-rw-   0        0        0      633 2023-06-07 01:49:12.000000 zhousf-lib-0.9.2/zhousflib/util/re_util.py
--rw-rw-rw-   0        0        0      520 2023-06-07 01:49:12.000000 zhousf-lib-0.9.2/zhousflib/util/singleton.py
--rw-rw-rw-   0        0        0     4989 2023-06-14 07:42:54.000000 zhousf-lib-0.9.2/zhousflib/util/string_util.py
--rw-rw-rw-   0        0        0     2209 2023-06-16 08:11:27.000000 zhousf-lib-0.9.2/zhousflib/util/thread_util.py
--rw-rw-rw-   0        0        0      794 2023-06-16 08:11:54.000000 zhousf-lib-0.9.2/zhousflib/util/threadpool_util.py
--rw-rw-rw-   0        0        0     4663 2023-06-07 01:49:11.000000 zhousf-lib-0.9.2/zhousflib/util/time_util.py
--rw-rw-rw-   0        0        0     3122 2023-06-16 08:43:33.000000 zhousf-lib-0.9.2/zhousflib/util/zip_util.py
-drwxrwxrwx   0        0        0        0 2023-07-25 08:05:06.481423 zhousf-lib-0.9.2/zhousflib/web/
--rw-rw-rw-   0        0        0       60 2023-06-07 01:49:12.000000 zhousf-lib-0.9.2/zhousflib/web/__init__.py
--rw-rw-rw-   0        0        0     3105 2023-06-07 01:49:12.000000 zhousf-lib-0.9.2/zhousflib/web/log_util.py
--rw-rw-rw-   0        0        0     3458 2023-07-25 08:04:56.000000 zhousf-lib-0.9.2/zhousflib/web/logger.py
--rw-rw-rw-   0        0        0     1340 2023-06-07 01:49:13.000000 zhousf-lib-0.9.2/zhousflib/web/response.py
+drwxrwxrwx   0        0        0        0 2023-08-04 01:40:33.601065 zhousf-lib-0.9.3/
+-rw-rw-rw-   0        0        0     1086 2023-06-06 02:24:10.000000 zhousf-lib-0.9.3/LICENSE
+-rw-rw-rw-   0        0        0     2073 2023-08-04 01:40:33.600066 zhousf-lib-0.9.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1179 2023-06-09 06:54:16.000000 zhousf-lib-0.9.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-04 01:40:33.601065 zhousf-lib-0.9.3/setup.cfg
+-rw-rw-rw-   0        0        0     4289 2023-08-04 01:40:27.000000 zhousf-lib-0.9.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 01:40:32.964067 zhousf-lib-0.9.3/zhousf_lib.egg-info/
+-rw-rw-rw-   0        0        0     2073 2023-08-04 01:40:32.000000 zhousf-lib-0.9.3/zhousf_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2368 2023-08-04 01:40:32.000000 zhousf-lib-0.9.3/zhousf_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 01:40:32.000000 zhousf-lib-0.9.3/zhousf_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-08-04 01:40:32.000000 zhousf-lib-0.9.3/zhousf_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-04 01:40:32.965066 zhousf-lib-0.9.3/zhousflib/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:49:13.000000 zhousf-lib-0.9.3/zhousflib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-04 01:40:32.966067 zhousf-lib-0.9.3/zhousflib/datasets/
+-rw-rw-rw-   0        0        0       84 2023-06-06 02:39:10.000000 zhousf-lib-0.9.3/zhousflib/datasets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-04 01:40:32.968066 zhousf-lib-0.9.3/zhousflib/datasets/classification/
+-rw-rw-rw-   0        0        0       73 2023-06-07 01:45:12.000000 zhousf-lib-0.9.3/zhousflib/datasets/classification/__init__.py
+-rw-rw-rw-   0        0        0     4895 2023-06-13 08:58:42.000000 zhousf-lib-0.9.3/zhousflib/datasets/classification/classification_dataset_split.py
+drwxrwxrwx   0        0        0        0 2023-08-04 01:40:33.047067 zhousf-lib-0.9.3/zhousflib/datasets/coco/
+-rw-rw-rw-   0        0        0       73 2023-07-11 01:24:38.000000 zhousf-lib-0.9.3/zhousflib/datasets/coco/__init__.py
+-rw-rw-rw-   0        0        0     8251 2023-06-07 07:58:31.000000 zhousf-lib-0.9.3/zhousflib/datasets/coco/coco_bbox_extract.py
+-rw-rw-rw-   0        0        0     5484 2023-06-12 06:00:08.000000 zhousf-lib-0.9.3/zhousflib/datasets/coco/coco_bbox_update.py
+-rw-rw-rw-   0        0        0     6637 2023-06-08 02:33:01.000000 zhousf-lib-0.9.3/zhousflib/datasets/coco/coco_bbox_vis.py
+-rw-rw-rw-   0        0        0     2896 2023-06-07 07:55:47.000000 zhousf-lib-0.9.3/zhousflib/datasets/coco/coco_dataset_merge.py
+-rw-rw-rw-   0        0        0     6278 2023-06-09 06:13:45.000000 zhousf-lib-0.9.3/zhousflib/datasets/coco/coco_dataset_split.py
+drwxrwxrwx   0        0        0        0 2023-08-04 01:40:33.092093 zhousf-lib-0.9.3/zhousflib/datasets/labelme/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:45:12.000000 zhousf-lib-0.9.3/zhousflib/datasets/labelme/__init__.py
+-rw-rw-rw-   0        0        0     3825 2023-06-07 01:45:12.000000 zhousf-lib-0.9.3/zhousflib/datasets/labelme/labelme_clip.py
+-rw-rw-rw-   0        0        0     8090 2023-06-07 01:45:12.000000 zhousf-lib-0.9.3/zhousflib/datasets/labelme/labelme_convert_coco.py
+-rw-rw-rw-   0        0        0     9622 2023-06-06 09:07:37.000000 zhousf-lib-0.9.3/zhousflib/datasets/labelme/labelme_convert_seg.py
+-rw-rw-rw-   0        0        0     3827 2023-06-07 01:45:12.000000 zhousf-lib-0.9.3/zhousflib/datasets/labelme/labelme_dataset_clip.py
+drwxrwxrwx   0        0        0        0 2023-08-04 01:40:33.095069 zhousf-lib-0.9.3/zhousflib/datasets/segmentation/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:45:12.000000 zhousf-lib-0.9.3/zhousflib/datasets/segmentation/__init__.py
+-rw-rw-rw-   0        0        0     2871 2023-06-06 09:07:37.000000 zhousf-lib-0.9.3/zhousflib/datasets/segmentation/seg_dataset_split.py
+drwxrwxrwx   0        0        0        0 2023-08-04 01:40:33.104067 zhousf-lib-0.9.3/zhousflib/datasets/uiex/
+-rw-rw-rw-   0        0        0       60 2023-07-24 09:12:22.000000 zhousf-lib-0.9.3/zhousflib/datasets/uiex/__init__.py
+-rw-rw-rw-   0        0        0     8611 2023-07-31 09:30:14.000000 zhousf-lib-0.9.3/zhousflib/datasets/uiex/labelme_convert_uiex.py
+drwxrwxrwx   0        0        0        0 2023-08-04 01:40:33.115099 zhousf-lib-0.9.3/zhousflib/db/
+-rw-rw-rw-   0        0        0       60 2023-06-15 07:08:53.000000 zhousf-lib-0.9.3/zhousflib/db/__init__.py
+-rw-rw-rw-   0        0        0     2343 2023-06-15 07:08:53.000000 zhousf-lib-0.9.3/zhousflib/db/lmdb_master.py
+drwxrwxrwx   0        0        0        0 2023-08-04 01:40:33.128067 zhousf-lib-0.9.3/zhousflib/decorator/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:45:12.000000 zhousf-lib-0.9.3/zhousflib/decorator/__init__.py
+-rw-rw-rw-   0        0        0      504 2023-07-18 05:47:21.000000 zhousf-lib-0.9.3/zhousflib/decorator/except_util.py
+-rw-rw-rw-   0        0        0     1094 2023-06-07 01:49:12.000000 zhousf-lib-0.9.3/zhousflib/decorator/interceptor_util.py
+drwxrwxrwx   0        0        0        0 2023-08-04 01:40:33.155068 zhousf-lib-0.9.3/zhousflib/download/
+-rw-rw-rw-   0        0        0       60 2023-06-16 08:05:46.000000 zhousf-lib-0.9.3/zhousflib/download/__init__.py
+-rw-rw-rw-   0        0        0     4646 2023-06-16 08:07:58.000000 zhousf-lib-0.9.3/zhousflib/download/download_util.py
+drwxrwxrwx   0        0        0        0 2023-08-04 01:40:33.287067 zhousf-lib-0.9.3/zhousflib/font/
+-rw-rw-rw-   0        0        0 15320040 2023-03-31 01:19:09.000000 zhousf-lib-0.9.3/zhousflib/font/SimSun.ttf
+-rw-rw-rw-   0        0        0  2152796 2023-03-31 01:19:09.000000 zhousf-lib-0.9.3/zhousflib/font/Symbola.ttf
+-rw-rw-rw-   0        0        0      763 2023-06-09 05:53:49.000000 zhousf-lib-0.9.3/zhousflib/font/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-04 01:40:33.297068 zhousf-lib-0.9.3/zhousflib/locust/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:49:12.000000 zhousf-lib-0.9.3/zhousflib/locust/__init__.py
+-rw-rw-rw-   0        0        0     1521 2023-06-15 07:08:53.000000 zhousf-lib-0.9.3/zhousflib/locust/locust_demo.py
+drwxrwxrwx   0        0        0        0 2023-08-04 01:40:33.322067 zhousf-lib-0.9.3/zhousflib/pandas/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:49:13.000000 zhousf-lib-0.9.3/zhousflib/pandas/__init__.py
+-rw-rw-rw-   0        0        0     4761 2023-06-19 03:04:32.000000 zhousf-lib-0.9.3/zhousflib/pandas/openpyxl_util.py
+-rw-rw-rw-   0        0        0     5872 2023-06-19 03:04:56.000000 zhousf-lib-0.9.3/zhousflib/pandas/pandas_util.py
+drwxrwxrwx   0        0        0        0 2023-08-04 01:40:33.345069 zhousf-lib-0.9.3/zhousflib/pdf/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:49:12.000000 zhousf-lib-0.9.3/zhousflib/pdf/__init__.py
+-rw-rw-rw-   0        0        0     1845 2023-06-07 01:49:12.000000 zhousf-lib-0.9.3/zhousflib/pdf/export_image.py
+-rw-rw-rw-   0        0        0     1465 2023-06-15 07:08:53.000000 zhousf-lib-0.9.3/zhousflib/pdf/pdfplumber_util.py
+drwxrwxrwx   0        0        0        0 2023-08-04 01:40:33.376066 zhousf-lib-0.9.3/zhousflib/so/
+-rw-rw-rw-   0        0        0       85 2023-06-29 06:08:24.000000 zhousf-lib-0.9.3/zhousflib/so/__init__.py
+-rw-rw-rw-   0        0        0     3736 2023-06-27 03:01:19.000000 zhousf-lib-0.9.3/zhousflib/so/project_to_so.py
+-rw-rw-rw-   0        0        0      273 2023-06-27 03:01:19.000000 zhousf-lib-0.9.3/zhousflib/so/py_to_so.py
+drwxrwxrwx   0        0        0        0 2023-08-04 01:40:33.559068 zhousf-lib-0.9.3/zhousflib/util/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:49:12.000000 zhousf-lib-0.9.3/zhousflib/util/__init__.py
+-rw-rw-rw-   0        0        0     3151 2023-07-19 06:01:50.000000 zhousf-lib-0.9.3/zhousflib/util/calculater_util.py
+-rw-rw-rw-   0        0        0     2067 2023-06-27 02:49:36.000000 zhousf-lib-0.9.3/zhousflib/util/char_util.py
+-rw-rw-rw-   0        0        0      635 2023-06-07 01:49:12.000000 zhousf-lib-0.9.3/zhousflib/util/cv_util.py
+-rw-rw-rw-   0        0        0     2609 2023-06-16 08:07:58.000000 zhousf-lib-0.9.3/zhousflib/util/dict_util.py
+-rw-rw-rw-   0        0        0     2193 2023-06-07 01:49:13.000000 zhousf-lib-0.9.3/zhousflib/util/encrypt_util.py
+-rw-rw-rw-   0        0        0     1593 2023-06-29 06:32:27.000000 zhousf-lib-0.9.3/zhousflib/util/img_util.py
+-rw-rw-rw-   0        0        0    11914 2023-08-04 01:40:12.000000 zhousf-lib-0.9.3/zhousflib/util/iou_util.py
+-rw-rw-rw-   0        0        0     3373 2023-06-07 01:49:12.000000 zhousf-lib-0.9.3/zhousflib/util/json_util.py
+-rw-rw-rw-   0        0        0     1907 2023-07-19 06:44:54.000000 zhousf-lib-0.9.3/zhousflib/util/list_util.py
+-rw-rw-rw-   0        0        0     1432 2023-06-16 08:43:33.000000 zhousf-lib-0.9.3/zhousflib/util/math_util.py
+-rw-rw-rw-   0        0        0     1358 2023-06-07 01:49:12.000000 zhousf-lib-0.9.3/zhousflib/util/permission_util.py
+-rw-rw-rw-   0        0        0     3490 2023-07-31 02:53:12.000000 zhousf-lib-0.9.3/zhousflib/util/pil_util.py
+-rw-rw-rw-   0        0        0     3524 2023-06-07 01:49:11.000000 zhousf-lib-0.9.3/zhousflib/util/poly_util.py
+-rw-rw-rw-   0        0        0      502 2023-06-16 08:10:19.000000 zhousf-lib-0.9.3/zhousflib/util/random_util.py
+-rw-rw-rw-   0        0        0      633 2023-06-07 01:49:12.000000 zhousf-lib-0.9.3/zhousflib/util/re_util.py
+-rw-rw-rw-   0        0        0      520 2023-06-07 01:49:12.000000 zhousf-lib-0.9.3/zhousflib/util/singleton.py
+-rw-rw-rw-   0        0        0     4989 2023-06-14 07:42:54.000000 zhousf-lib-0.9.3/zhousflib/util/string_util.py
+-rw-rw-rw-   0        0        0     2209 2023-06-16 08:11:27.000000 zhousf-lib-0.9.3/zhousflib/util/thread_util.py
+-rw-rw-rw-   0        0        0      794 2023-06-16 08:11:54.000000 zhousf-lib-0.9.3/zhousflib/util/threadpool_util.py
+-rw-rw-rw-   0        0        0     4663 2023-06-07 01:49:11.000000 zhousf-lib-0.9.3/zhousflib/util/time_util.py
+-rw-rw-rw-   0        0        0     3122 2023-06-16 08:43:33.000000 zhousf-lib-0.9.3/zhousflib/util/zip_util.py
+drwxrwxrwx   0        0        0        0 2023-08-04 01:40:33.582065 zhousf-lib-0.9.3/zhousflib/web/
+-rw-rw-rw-   0        0        0       60 2023-06-07 01:49:12.000000 zhousf-lib-0.9.3/zhousflib/web/__init__.py
+-rw-rw-rw-   0        0        0     3105 2023-06-07 01:49:12.000000 zhousf-lib-0.9.3/zhousflib/web/log_util.py
+-rw-rw-rw-   0        0        0     3458 2023-07-25 08:04:56.000000 zhousf-lib-0.9.3/zhousflib/web/logger.py
+-rw-rw-rw-   0        0        0     1340 2023-06-07 01:49:13.000000 zhousf-lib-0.9.3/zhousflib/web/response.py
```

### Comparing `zhousf-lib-0.9.2/LICENSE` & `zhousf-lib-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.9.2/PKG-INFO` & `zhousf-lib-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhousf-lib
-Version: 0.9.2
+Version: 0.9.3
 Summary: a python library of zhousf
 Home-page: https://github.com/MrZhousf/ZhousfLib
 Author: zhousf
 Author-email: 442553199@qq.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `zhousf-lib-0.9.2/README.md` & `zhousf-lib-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.9.2/setup.py` & `zhousf-lib-0.9.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # 打包：python setup.py upload
 NAME = 'zhousf-lib'
 DESCRIPTION = 'a python library of zhousf'
 URL = 'https://github.com/MrZhousf/ZhousfLib'
 EMAIL = '442553199@qq.com'
 AUTHOR = 'zhousf'
 REQUIRES_PYTHON = '>=3.6.13'
-VERSION = '0.9.2'
+VERSION = '0.9.3'
 PACKAGE_DATA = {'': ['*.yaml', '*.ttf', '*.txt', '*.md']}
 
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 # What packages are required for this module to be executed?
```

### Comparing `zhousf-lib-0.9.2/zhousf_lib.egg-info/PKG-INFO` & `zhousf-lib-0.9.3/zhousf_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhousf-lib
-Version: 0.9.2
+Version: 0.9.3
 Summary: a python library of zhousf
 Home-page: https://github.com/MrZhousf/ZhousfLib
 Author: zhousf
 Author-email: 442553199@qq.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `zhousf-lib-0.9.2/zhousf_lib.egg-info/SOURCES.txt` & `zhousf-lib-0.9.3/zhousf_lib.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 zhousflib/util/encrypt_util.py
 zhousflib/util/img_util.py
 zhousflib/util/iou_util.py
 zhousflib/util/json_util.py
 zhousflib/util/list_util.py
 zhousflib/util/math_util.py
 zhousflib/util/permission_util.py
+zhousflib/util/pil_util.py
 zhousflib/util/poly_util.py
 zhousflib/util/random_util.py
 zhousflib/util/re_util.py
 zhousflib/util/singleton.py
 zhousflib/util/string_util.py
 zhousflib/util/thread_util.py
 zhousflib/util/threadpool_util.py
```

### Comparing `zhousf-lib-0.9.2/zhousflib/datasets/classification/classification_dataset_split.py` & `zhousf-lib-0.9.3/zhousflib/datasets/classification/classification_dataset_split.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.9.2/zhousflib/datasets/coco/coco_bbox_extract.py` & `zhousf-lib-0.9.3/zhousflib/datasets/coco/coco_bbox_extract.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.9.2/zhousflib/datasets/coco/coco_bbox_update.py` & `zhousf-lib-0.9.3/zhousflib/datasets/coco/coco_bbox_update.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.9.2/zhousflib/datasets/coco/coco_bbox_vis.py` & `zhousf-lib-0.9.3/zhousflib/datasets/coco/coco_bbox_vis.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.9.2/zhousflib/datasets/coco/coco_dataset_merge.py` & `zhousf-lib-0.9.3/zhousflib/datasets/coco/coco_dataset_merge.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.9.2/zhousflib/datasets/coco/coco_dataset_split.py` & `zhousf-lib-0.9.3/zhousflib/datasets/coco/coco_dataset_split.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.9.2/zhousflib/datasets/labelme/labelme_clip.py` & `zhousf-lib-0.9.3/zhousflib/datasets/labelme/labelme_clip.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.9.2/zhousflib/datasets/labelme/labelme_convert_coco.py` & `zhousf-lib-0.9.3/zhousflib/datasets/labelme/labelme_convert_coco.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.9.2/zhousflib/datasets/labelme/labelme_convert_seg.py` & `zhousf-lib-0.9.3/zhousflib/datasets/labelme/labelme_convert_seg.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.9.2/zhousflib/datasets/labelme/labelme_dataset_clip.py` & `zhousf-lib-0.9.3/zhousflib/datasets/labelme/labelme_dataset_clip.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.9.2/zhousflib/datasets/segmentation/seg_dataset_split.py` & `zhousf-lib-0.9.3/zhousflib/datasets/segmentation/seg_dataset_split.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.9.2/zhousflib/db/lmdb_master.py` & `zhousf-lib-0.9.3/zhousflib/db/lmdb_master.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.9.2/zhousflib/decorator/interceptor_util.py` & `zhousf-lib-0.9.3/zhousflib/decorator/interceptor_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.9.2/zhousflib/download/download_util.py` & `zhousf-lib-0.9.3/zhousflib/download/download_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.9.2/zhousflib/font/SimSun.ttf` & `zhousf-lib-0.9.3/zhousflib/font/SimSun.ttf`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.9.2/zhousflib/font/Symbola.ttf` & `zhousf-lib-0.9.3/zhousflib/font/Symbola.ttf`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.9.2/zhousflib/font/__init__.py` & `zhousf-lib-0.9.3/zhousflib/font/__init__.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.9.2/zhousflib/locust/locust_demo.py` & `zhousf-lib-0.9.3/zhousflib/locust/locust_demo.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.9.2/zhousflib/pandas/openpyxl_util.py` & `zhousf-lib-0.9.3/zhousflib/pandas/openpyxl_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.9.2/zhousflib/pandas/pandas_util.py` & `zhousf-lib-0.9.3/zhousflib/pandas/pandas_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.9.2/zhousflib/pdf/export_image.py` & `zhousf-lib-0.9.3/zhousflib/pdf/export_image.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.9.2/zhousflib/pdf/pdfplumber_util.py` & `zhousf-lib-0.9.3/zhousflib/pdf/pdfplumber_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.9.2/zhousflib/so/project_to_so.py` & `zhousf-lib-0.9.3/zhousflib/so/project_to_so.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.9.2/zhousflib/util/calculater_util.py` & `zhousf-lib-0.9.3/zhousflib/util/calculater_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.9.2/zhousflib/util/char_util.py` & `zhousf-lib-0.9.3/zhousflib/util/char_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.9.2/zhousflib/util/cv_util.py` & `zhousf-lib-0.9.3/zhousflib/util/cv_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.9.2/zhousflib/util/dict_util.py` & `zhousf-lib-0.9.3/zhousflib/util/dict_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.9.2/zhousflib/util/encrypt_util.py` & `zhousf-lib-0.9.3/zhousflib/util/encrypt_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.9.2/zhousflib/util/img_util.py` & `zhousf-lib-0.9.3/zhousflib/util/img_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.9.2/zhousflib/util/json_util.py` & `zhousf-lib-0.9.3/zhousflib/util/json_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.9.2/zhousflib/util/list_util.py` & `zhousf-lib-0.9.3/zhousflib/util/list_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.9.2/zhousflib/util/math_util.py` & `zhousf-lib-0.9.3/zhousflib/util/math_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.9.2/zhousflib/util/permission_util.py` & `zhousf-lib-0.9.3/zhousflib/util/permission_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.9.2/zhousflib/util/poly_util.py` & `zhousf-lib-0.9.3/zhousflib/util/poly_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.9.2/zhousflib/util/re_util.py` & `zhousf-lib-0.9.3/zhousflib/util/re_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.9.2/zhousflib/util/singleton.py` & `zhousf-lib-0.9.3/zhousflib/util/singleton.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.9.2/zhousflib/util/string_util.py` & `zhousf-lib-0.9.3/zhousflib/util/string_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.9.2/zhousflib/util/thread_util.py` & `zhousf-lib-0.9.3/zhousflib/util/thread_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.9.2/zhousflib/util/threadpool_util.py` & `zhousf-lib-0.9.3/zhousflib/util/threadpool_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.9.2/zhousflib/util/time_util.py` & `zhousf-lib-0.9.3/zhousflib/util/time_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.9.2/zhousflib/util/zip_util.py` & `zhousf-lib-0.9.3/zhousflib/util/zip_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.9.2/zhousflib/web/log_util.py` & `zhousf-lib-0.9.3/zhousflib/web/log_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.9.2/zhousflib/web/logger.py` & `zhousf-lib-0.9.3/zhousflib/web/logger.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-0.9.2/zhousflib/web/response.py` & `zhousf-lib-0.9.3/zhousflib/web/response.py`

 * *Files identical despite different names*

