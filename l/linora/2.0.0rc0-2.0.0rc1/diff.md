# Comparing `tmp/linora-2.0.0rc0.tar.gz` & `tmp/linora-2.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/linora-2.0.0rc0.tar", last modified: Fri Apr 28 01:24:56 2023, max compression
+gzip compressed data, was "dist/linora-2.0.0rc1.tar", last modified: Fri Aug  4 02:09:53 2023, max compression
```

## Comparing `linora-2.0.0rc0.tar` & `linora-2.0.0rc1.tar`

### file list

```diff
@@ -1,217 +1,218 @@
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/
--rw-r--r--   0 liyanpeng   (501) staff       (20)     3736 2023-04-28 01:24:56.000000 linora-2.0.0rc0/PKG-INFO
--rw-r--r--   0 liyanpeng   (501) staff       (20)     2148 2022-05-06 08:30:54.000000 linora-2.0.0rc0/README.md
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/
--rw-r--r--   0 liyanpeng   (501) staff       (20)      981 2023-03-28 07:21:23.000000 linora-2.0.0rc0/linora/__init__.py
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/audio/
--rw-r--r--   0 liyanpeng   (501) staff       (20)       75 2022-11-17 07:55:45.000000 linora-2.0.0rc0/linora/audio/__init__.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)    14608 2023-04-27 06:54:53.000000 linora-2.0.0rc0/linora/audio/_audio_io.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)      492 2022-11-17 07:55:32.000000 linora-2.0.0rc0/linora/audio/_audio_util.py
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/chart/
--rw-r--r--   0 liyanpeng   (501) staff       (20)      403 2022-07-14 05:53:05.000000 linora-2.0.0rc0/linora/chart/__init__.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     2453 2022-08-09 08:32:05.000000 linora-2.0.0rc0/linora/chart/_arrow.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     5625 2022-08-09 08:07:44.000000 linora-2.0.0rc0/linora/chart/_bar.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)    37257 2022-08-22 09:14:42.000000 linora-2.0.0rc0/linora/chart/_base.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     5507 2022-08-03 06:11:10.000000 linora-2.0.0rc0/linora/chart/_boxplot.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     1916 2022-08-09 08:11:23.000000 linora-2.0.0rc0/linora/chart/_circle.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     4479 2022-08-09 07:00:01.000000 linora-2.0.0rc0/linora/chart/_coherence.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     3883 2022-08-19 07:12:54.000000 linora-2.0.0rc0/linora/chart/_config.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     4940 2022-08-09 07:03:51.000000 linora-2.0.0rc0/linora/chart/_csd.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     2160 2022-08-09 08:12:42.000000 linora-2.0.0rc0/linora/chart/_ellipse.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     7443 2022-08-03 06:11:42.000000 linora-2.0.0rc0/linora/chart/_errorbar.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     1466 2022-04-24 14:02:43.000000 linora-2.0.0rc0/linora/chart/_feature.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     3870 2022-08-09 02:21:38.000000 linora-2.0.0rc0/linora/chart/_fillline.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     7720 2022-08-10 08:01:23.000000 linora-2.0.0rc0/linora/chart/_grid.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     6951 2022-08-09 02:21:56.000000 linora-2.0.0rc0/linora/chart/_hist.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     1004 2022-08-09 02:22:05.000000 linora-2.0.0rc0/linora/chart/_hist2d.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     1353 2022-08-09 02:22:40.000000 linora-2.0.0rc0/linora/chart/_hlines.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     4557 2022-08-09 02:22:54.000000 linora-2.0.0rc0/linora/chart/_line.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     4806 2022-08-09 02:23:07.000000 linora-2.0.0rc0/linora/chart/_line3D.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)    11321 2022-04-24 14:02:43.000000 linora-2.0.0rc0/linora/chart/_metrics.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     3835 2022-08-03 06:13:51.000000 linora-2.0.0rc0/linora/chart/_pie.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     8171 2022-08-09 08:34:12.000000 linora-2.0.0rc0/linora/chart/_plot.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     1983 2022-08-09 08:12:27.000000 linora-2.0.0rc0/linora/chart/_polygon.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     5312 2022-08-09 02:23:32.000000 linora-2.0.0rc0/linora/chart/_radar.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     2511 2022-08-09 08:11:53.000000 linora-2.0.0rc0/linora/chart/_rectangle.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     2242 2022-08-09 08:11:43.000000 linora-2.0.0rc0/linora/chart/_regularpolygon.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     5718 2022-08-09 02:23:50.000000 linora-2.0.0rc0/linora/chart/_scatter.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     6367 2022-08-09 02:24:07.000000 linora-2.0.0rc0/linora/chart/_scatter3D.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     1350 2022-08-09 02:24:44.000000 linora-2.0.0rc0/linora/chart/_vlines.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     2137 2022-08-09 08:08:19.000000 linora-2.0.0rc0/linora/chart/_wedge.py
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/data/
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/data/Dataset/
--rw-r--r--   0 liyanpeng   (501) staff       (20)       42 2022-06-08 08:59:03.000000 linora-2.0.0rc0/linora/data/Dataset/__init__.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)    27211 2022-08-29 09:18:04.000000 linora-2.0.0rc0/linora/data/Dataset/_data.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)    13157 2022-06-08 08:22:31.000000 linora-2.0.0rc0/linora/data/Dataset/_dataset.py
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/data/TextLineDataset/
--rw-r--r--   0 liyanpeng   (501) staff       (20)       50 2022-05-27 04:17:36.000000 linora-2.0.0rc0/linora/data/TextLineDataset/__init__.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)    15392 2022-05-27 08:07:05.000000 linora-2.0.0rc0/linora/data/TextLineDataset/_dataset.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)      215 2022-12-07 05:59:38.000000 linora-2.0.0rc0/linora/data/__init__.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     4007 2022-11-18 07:47:39.000000 linora-2.0.0rc0/linora/data/_compress.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)    11876 2022-12-07 06:31:44.000000 linora-2.0.0rc0/linora/data/_sql_io_dataset.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     1941 2022-06-01 08:26:01.000000 linora-2.0.0rc0/linora/data/_utils.py
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/data/datasets/
--rw-r--r--   0 liyanpeng   (501) staff       (20)       85 2022-08-19 09:00:53.000000 linora-2.0.0rc0/linora/data/datasets/__init__.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     2071 2022-12-01 09:47:11.000000 linora-2.0.0rc0/linora/data/datasets/_config_path.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)    19314 2022-06-08 08:37:02.000000 linora-2.0.0rc0/linora/data/datasets/_mnist.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     1293 2022-12-02 05:08:27.000000 linora-2.0.0rc0/linora/data/datasets/_utils.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)   264001 2022-08-22 01:29:59.000000 linora-2.0.0rc0/linora/data/datasets/_weather.py
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/feature_column/
--rw-r--r--   0 liyanpeng   (501) staff       (20)      277 2023-03-22 09:25:19.000000 linora-2.0.0rc0/linora/feature_column/__init__.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)    20098 2023-03-21 09:04:16.000000 linora-2.0.0rc0/linora/feature_column/_categorical.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     7622 2023-03-23 09:40:18.000000 linora-2.0.0rc0/linora/feature_column/_datetime.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     6523 2023-03-24 06:31:58.000000 linora-2.0.0rc0/linora/feature_column/_feature.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)    10691 2023-03-21 02:03:11.000000 linora-2.0.0rc0/linora/feature_column/_feature_categorical.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     3687 2023-03-23 09:10:38.000000 linora-2.0.0rc0/linora/feature_column/_feature_datetime.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     5298 2023-03-21 02:03:40.000000 linora-2.0.0rc0/linora/feature_column/_feature_normalize.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)    11083 2023-03-24 01:40:41.000000 linora-2.0.0rc0/linora/feature_column/_feature_numerical.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     8774 2023-03-21 09:03:05.000000 linora-2.0.0rc0/linora/feature_column/_normalize.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)    21492 2023-03-24 01:26:31.000000 linora-2.0.0rc0/linora/feature_column/_numerical.py
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/feature_column/boundary/
--rw-r--r--   0 liyanpeng   (501) staff       (20)       55 2022-04-24 14:02:43.000000 linora-2.0.0rc0/linora/feature_column/boundary/__init__.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     3495 2022-04-24 14:02:43.000000 linora-2.0.0rc0/linora/feature_column/boundary/_boundary.py
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/feature_selection/
--rw-r--r--   0 liyanpeng   (501) staff       (20)       94 2022-04-24 14:02:43.000000 linora-2.0.0rc0/linora/feature_selection/__init__.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     1780 2022-04-24 14:02:43.000000 linora-2.0.0rc0/linora/feature_selection/_credit.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     2622 2022-05-12 01:17:51.000000 linora-2.0.0rc0/linora/feature_selection/_select.py
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/gfile/
--rw-r--r--   0 liyanpeng   (501) staff       (20)       33 2022-04-24 14:02:43.000000 linora-2.0.0rc0/linora/gfile/__init__.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     5895 2022-11-23 09:16:08.000000 linora-2.0.0rc0/linora/gfile/_gfile.py
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/image/
--rw-r--r--   0 liyanpeng   (501) staff       (20)      636 2022-05-16 10:12:12.000000 linora-2.0.0rc0/linora/image/__init__.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     1442 2022-05-26 02:08:30.000000 linora-2.0.0rc0/linora/image/_image_aug.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     3596 2022-05-18 00:54:35.000000 linora-2.0.0rc0/linora/image/_image_box.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)    29992 2022-11-30 09:53:59.000000 linora-2.0.0rc0/linora/image/_image_color.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)    12038 2022-05-26 02:07:59.000000 linora-2.0.0rc0/linora/image/_image_color_aug.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     8666 2022-05-16 09:32:03.000000 linora-2.0.0rc0/linora/image/_image_crop.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     2963 2022-05-26 02:08:58.000000 linora-2.0.0rc0/linora/image/_image_crop_aug.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)    11337 2022-05-27 06:56:17.000000 linora-2.0.0rc0/linora/image/_image_draw.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     2305 2022-05-27 07:05:28.000000 linora-2.0.0rc0/linora/image/_image_draw_aug.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)    16607 2022-11-18 03:22:32.000000 linora-2.0.0rc0/linora/image/_image_feature.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     8805 2022-05-13 01:24:35.000000 linora-2.0.0rc0/linora/image/_image_filter.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     5629 2022-05-26 02:09:23.000000 linora-2.0.0rc0/linora/image/_image_filter_aug.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     7215 2022-08-01 08:30:47.000000 linora-2.0.0rc0/linora/image/_image_grid.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     2693 2023-03-22 09:47:31.000000 linora-2.0.0rc0/linora/image/_image_io.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     2345 2022-05-22 03:19:04.000000 linora-2.0.0rc0/linora/image/_image_io_aug.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)    13075 2022-05-17 03:28:28.000000 linora-2.0.0rc0/linora/image/_image_noise.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     7787 2022-05-26 02:09:49.000000 linora-2.0.0rc0/linora/image/_image_noise_aug.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     8431 2022-04-25 13:29:23.000000 linora-2.0.0rc0/linora/image/_image_pairs.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)    21630 2022-05-25 09:46:33.000000 linora-2.0.0rc0/linora/image/_image_position.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)    12989 2022-05-26 02:40:18.000000 linora-2.0.0rc0/linora/image/_image_position_aug.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     7012 2022-05-16 02:51:05.000000 linora-2.0.0rc0/linora/image/_image_rescale.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     4257 2022-05-26 02:10:15.000000 linora-2.0.0rc0/linora/image/_image_rescale_aug.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     2527 2022-05-25 02:36:08.000000 linora-2.0.0rc0/linora/image/_image_resize.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)      519 2022-05-09 09:56:14.000000 linora-2.0.0rc0/linora/image/_image_resize_aug.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)    41696 2022-05-27 06:48:41.000000 linora-2.0.0rc0/linora/image/_image_rgb.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     5315 2023-04-14 07:37:25.000000 linora-2.0.0rc0/linora/image/_image_util.py
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/metrics/
--rw-r--r--   0 liyanpeng   (501) staff       (20)      231 2022-04-24 14:02:43.000000 linora-2.0.0rc0/linora/metrics/__init__.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)    27844 2022-06-22 02:45:29.000000 linora-2.0.0rc0/linora/metrics/_classification.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     4966 2022-05-26 08:02:56.000000 linora-2.0.0rc0/linora/metrics/_image.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     2335 2022-05-26 07:22:49.000000 linora-2.0.0rc0/linora/metrics/_metrics.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     2568 2022-06-21 10:20:14.000000 linora-2.0.0rc0/linora/metrics/_rank.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)    18341 2022-11-21 07:42:50.000000 linora-2.0.0rc0/linora/metrics/_regression.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     2518 2023-02-24 06:52:37.000000 linora-2.0.0rc0/linora/metrics/_text.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)      370 2022-06-21 10:10:45.000000 linora-2.0.0rc0/linora/metrics/_utils.py
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/metrics/distance/
--rw-r--r--   0 liyanpeng   (501) staff       (20)       97 2022-04-24 14:02:43.000000 linora-2.0.0rc0/linora/metrics/distance/__init__.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)    10758 2022-06-22 01:50:38.000000 linora-2.0.0rc0/linora/metrics/distance/_distance.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     5635 2022-04-24 14:02:43.000000 linora-2.0.0rc0/linora/metrics/distance/_divergence.py
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/parallel/
--rw-r--r--   0 liyanpeng   (501) staff       (20)       77 2022-04-24 14:02:43.000000 linora-2.0.0rc0/linora/parallel/__init__.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     5619 2022-04-24 14:02:43.000000 linora-2.0.0rc0/linora/parallel/_process.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     5408 2022-04-24 14:02:43.000000 linora-2.0.0rc0/linora/parallel/_thread.py
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/param_search/
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/param_search/GEClassifier/
--rw-r--r--   0 liyanpeng   (501) staff       (20)     2941 2022-04-24 14:02:43.000000 linora-2.0.0rc0/linora/param_search/GEClassifier/_GridSearch.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     3182 2022-04-24 14:02:43.000000 linora-2.0.0rc0/linora/param_search/GEClassifier/_RandomSearch.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)      142 2022-04-24 14:02:43.000000 linora-2.0.0rc0/linora/param_search/GEClassifier/__init__.py
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/param_search/GERegressor/
--rw-r--r--   0 liyanpeng   (501) staff       (20)     3219 2022-04-24 14:02:43.000000 linora-2.0.0rc0/linora/param_search/GERegressor/_RandomSearch.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)       71 2022-04-24 14:02:43.000000 linora-2.0.0rc0/linora/param_search/GERegressor/__init__.py
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/param_search/LGBMClassifier/
--rw-r--r--   0 liyanpeng   (501) staff       (20)     7659 2022-05-20 03:53:11.000000 linora-2.0.0rc0/linora/param_search/LGBMClassifier/_GridSearch.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     7646 2022-05-20 03:52:49.000000 linora-2.0.0rc0/linora/param_search/LGBMClassifier/_RandomSearch.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)      144 2022-05-05 06:13:26.000000 linora-2.0.0rc0/linora/param_search/LGBMClassifier/__init__.py
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/param_search/LGBMRegressor/
--rw-r--r--   0 liyanpeng   (501) staff       (20)     7656 2022-05-20 03:53:26.000000 linora-2.0.0rc0/linora/param_search/LGBMRegressor/_GridSearch.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     7644 2022-05-20 03:52:33.000000 linora-2.0.0rc0/linora/param_search/LGBMRegressor/_RandomSearch.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)      141 2022-05-05 06:14:26.000000 linora-2.0.0rc0/linora/param_search/LGBMRegressor/__init__.py
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/param_search/XGBClassifier/
--rw-r--r--   0 liyanpeng   (501) staff       (20)     8752 2022-05-20 03:51:53.000000 linora-2.0.0rc0/linora/param_search/XGBClassifier/_GridSearch.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     8724 2022-05-20 03:52:15.000000 linora-2.0.0rc0/linora/param_search/XGBClassifier/_RandomSearch.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)      142 2022-04-24 14:02:43.000000 linora-2.0.0rc0/linora/param_search/XGBClassifier/__init__.py
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/param_search/XGBRanker/
--rw-r--r--   0 liyanpeng   (501) staff       (20)     5599 2022-04-24 14:02:43.000000 linora-2.0.0rc0/linora/param_search/XGBRanker/_GridSearch.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     5904 2022-04-24 14:02:43.000000 linora-2.0.0rc0/linora/param_search/XGBRanker/_RandomSearch.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)      138 2022-04-24 14:02:43.000000 linora-2.0.0rc0/linora/param_search/XGBRanker/__init__.py
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/param_search/XGBRegressor/
--rw-r--r--   0 liyanpeng   (501) staff       (20)     8912 2022-05-20 03:51:33.000000 linora-2.0.0rc0/linora/param_search/XGBRegressor/_GridSearch.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     8943 2022-05-20 03:51:09.000000 linora-2.0.0rc0/linora/param_search/XGBRegressor/_RandomSearch.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)      140 2022-04-24 14:02:43.000000 linora-2.0.0rc0/linora/param_search/XGBRegressor/__init__.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)    13838 2022-06-15 06:08:40.000000 linora-2.0.0rc0/linora/param_search/_HyperParameters.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     9259 2023-03-27 01:31:53.000000 linora-2.0.0rc0/linora/param_search/_Search.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)      177 2022-06-08 09:41:40.000000 linora-2.0.0rc0/linora/param_search/__init__.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     9231 2022-05-22 02:43:27.000000 linora-2.0.0rc0/linora/param_search/_config.py
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/sample/
--rw-r--r--   0 liyanpeng   (501) staff       (20)      162 2022-05-10 08:08:14.000000 linora-2.0.0rc0/linora/sample/__init__.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     4847 2022-11-04 06:31:17.000000 linora-2.0.0rc0/linora/sample/_fold.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     3542 2022-04-24 14:02:43.000000 linora-2.0.0rc0/linora/sample/_random_walker.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     7072 2022-11-24 03:05:14.000000 linora-2.0.0rc0/linora/sample/_sampling.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     4051 2022-04-27 01:42:13.000000 linora-2.0.0rc0/linora/sample/_timeseries_kfold.py
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/server/
--rw-r--r--   0 liyanpeng   (501) staff       (20)      109 2023-03-28 05:08:20.000000 linora-2.0.0rc0/linora/server/__init__.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)    19067 2023-03-27 01:12:25.000000 linora-2.0.0rc0/linora/server/_email.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)    17119 2023-03-27 01:12:06.000000 linora-2.0.0rc0/linora/server/_email_utils.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)    13495 2023-03-27 00:57:47.000000 linora-2.0.0rc0/linora/server/_schedulers.py
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/server/message/
--rw-r--r--   0 liyanpeng   (501) staff       (20)    11784 2022-06-14 08:26:34.000000 linora-2.0.0rc0/linora/server/message/_BotDingTalk.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)      520 2022-04-24 14:02:43.000000 linora-2.0.0rc0/linora/server/message/_BotFeiShu.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)       95 2023-03-28 05:07:33.000000 linora-2.0.0rc0/linora/server/message/__init__.py
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/text/
--rw-r--r--   0 liyanpeng   (501) staff       (20)      149 2022-04-24 14:02:43.000000 linora-2.0.0rc0/linora/text/__init__.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     6243 2022-04-24 14:02:43.000000 linora-2.0.0rc0/linora/text/_sequence.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     4002 2022-04-24 14:02:43.000000 linora-2.0.0rc0/linora/text/_util.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     2267 2022-04-24 14:02:43.000000 linora-2.0.0rc0/linora/text/_vectorizer.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     3037 2023-02-24 05:40:38.000000 linora-2.0.0rc0/linora/text/_word_processing.py
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/train/
--rw-r--r--   0 liyanpeng   (501) staff       (20)      308 2022-08-24 08:42:12.000000 linora-2.0.0rc0/linora/train/__init__.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     2922 2022-09-01 01:52:14.000000 linora-2.0.0rc0/linora/train/_callback.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     1781 2022-08-24 02:28:50.000000 linora-2.0.0rc0/linora/train/_csvlogger.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     2371 2022-08-25 05:33:20.000000 linora-2.0.0rc0/linora/train/_earlystopping.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     1768 2022-08-24 02:54:41.000000 linora-2.0.0rc0/linora/train/_modelcheckpoint.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     2193 2022-08-24 01:53:17.000000 linora-2.0.0rc0/linora/train/_remotemonitor.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     2180 2022-09-01 01:55:31.000000 linora-2.0.0rc0/linora/train/_terminateonnan.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     7364 2022-08-27 02:43:20.000000 linora-2.0.0rc0/linora/train/_visual.py
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/train/lr/
--rw-r--r--   0 liyanpeng   (501) staff       (20)       75 2022-08-25 02:12:32.000000 linora-2.0.0rc0/linora/train/lr/__init__.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)    12872 2022-08-26 07:47:29.000000 linora-2.0.0rc0/linora/train/lr/_lr.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     1991 2022-08-25 03:30:35.000000 linora-2.0.0rc0/linora/train/lr/_schedulers.py
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/utils/
--rw-r--r--   0 liyanpeng   (501) staff       (20)      241 2022-11-10 02:19:13.000000 linora-2.0.0rc0/linora/utils/__init__.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     1444 2022-04-24 14:02:43.000000 linora-2.0.0rc0/linora/utils/_config.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)    19259 2023-03-27 01:06:27.000000 linora-2.0.0rc0/linora/utils/_email.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)    17119 2022-11-23 01:25:02.000000 linora-2.0.0rc0/linora/utils/_email_utils.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     9213 2022-05-11 03:45:54.000000 linora-2.0.0rc0/linora/utils/_logger.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     4106 2022-05-31 11:52:27.000000 linora-2.0.0rc0/linora/utils/_progbar.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)    13658 2023-03-27 01:10:43.000000 linora-2.0.0rc0/linora/utils/_schedulers.py
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/utils/message/
--rw-r--r--   0 liyanpeng   (501) staff       (20)    11965 2023-03-28 05:06:17.000000 linora-2.0.0rc0/linora/utils/message/_BotDingTalk.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)      739 2023-03-28 05:05:36.000000 linora-2.0.0rc0/linora/utils/message/_BotFeiShu.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)       93 2023-03-28 05:03:07.000000 linora-2.0.0rc0/linora/utils/message/__init__.py
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/utils/pip/
--rw-r--r--   0 liyanpeng   (501) staff       (20)       35 2022-08-04 02:59:58.000000 linora-2.0.0rc0/linora/utils/pip/__init__.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)    14751 2022-08-05 04:59:06.000000 linora-2.0.0rc0/linora/utils/pip/_pip.py
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora/vedio/
--rw-r--r--   0 liyanpeng   (501) staff       (20)       75 2023-04-14 07:02:50.000000 linora-2.0.0rc0/linora/vedio/__init__.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)    17841 2023-04-27 07:03:50.000000 linora-2.0.0rc0/linora/vedio/_vedio_io.py
--rw-r--r--   0 liyanpeng   (501) staff       (20)     3801 2023-04-23 08:50:15.000000 linora-2.0.0rc0/linora/vedio/_vedio_util.py
-drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora.egg-info/
--rw-r--r--   0 liyanpeng   (501) staff       (20)     3736 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora.egg-info/PKG-INFO
--rw-r--r--   0 liyanpeng   (501) staff       (20)     5603 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora.egg-info/SOURCES.txt
--rw-r--r--   0 liyanpeng   (501) staff       (20)        1 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora.egg-info/dependency_links.txt
--rw-r--r--   0 liyanpeng   (501) staff       (20)        1 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora.egg-info/not-zip-safe
--rw-r--r--   0 liyanpeng   (501) staff       (20)       67 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora.egg-info/requires.txt
--rw-r--r--   0 liyanpeng   (501) staff       (20)        7 2023-04-28 01:24:56.000000 linora-2.0.0rc0/linora.egg-info/top_level.txt
--rw-r--r--   0 liyanpeng   (501) staff       (20)       79 2023-04-28 01:24:56.000000 linora-2.0.0rc0/setup.cfg
--rw-r--r--   0 liyanpeng   (501) staff       (20)     1631 2023-03-21 02:28:13.000000 linora-2.0.0rc0/setup.py
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-08-04 02:09:53.000000 linora-2.0.0rc1/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     3736 2023-08-04 02:09:53.000000 linora-2.0.0rc1/PKG-INFO
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     2148 2022-05-06 08:30:54.000000 linora-2.0.0rc1/README.md
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-08-04 02:09:53.000000 linora-2.0.0rc1/linora/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)      981 2023-08-04 02:07:03.000000 linora-2.0.0rc1/linora/__init__.py
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-08-04 02:09:53.000000 linora-2.0.0rc1/linora/audio/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)       75 2022-11-17 07:55:45.000000 linora-2.0.0rc1/linora/audio/__init__.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    14610 2023-06-25 08:43:10.000000 linora-2.0.0rc1/linora/audio/_audio_io.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)      492 2022-11-17 07:55:32.000000 linora-2.0.0rc1/linora/audio/_audio_util.py
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-08-04 02:09:53.000000 linora-2.0.0rc1/linora/chart/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)      403 2022-07-14 05:53:05.000000 linora-2.0.0rc1/linora/chart/__init__.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     2453 2022-08-09 08:32:05.000000 linora-2.0.0rc1/linora/chart/_arrow.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     5625 2022-08-09 08:07:44.000000 linora-2.0.0rc1/linora/chart/_bar.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    37257 2022-08-22 09:14:42.000000 linora-2.0.0rc1/linora/chart/_base.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     5507 2022-08-03 06:11:10.000000 linora-2.0.0rc1/linora/chart/_boxplot.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     1916 2022-08-09 08:11:23.000000 linora-2.0.0rc1/linora/chart/_circle.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     4479 2022-08-09 07:00:01.000000 linora-2.0.0rc1/linora/chart/_coherence.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     3883 2022-08-19 07:12:54.000000 linora-2.0.0rc1/linora/chart/_config.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     4940 2022-08-09 07:03:51.000000 linora-2.0.0rc1/linora/chart/_csd.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     2160 2022-08-09 08:12:42.000000 linora-2.0.0rc1/linora/chart/_ellipse.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     7443 2022-08-03 06:11:42.000000 linora-2.0.0rc1/linora/chart/_errorbar.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     1466 2022-04-24 14:02:43.000000 linora-2.0.0rc1/linora/chart/_feature.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     3870 2022-08-09 02:21:38.000000 linora-2.0.0rc1/linora/chart/_fillline.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     7720 2022-08-10 08:01:23.000000 linora-2.0.0rc1/linora/chart/_grid.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     6951 2022-08-09 02:21:56.000000 linora-2.0.0rc1/linora/chart/_hist.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     1004 2022-08-09 02:22:05.000000 linora-2.0.0rc1/linora/chart/_hist2d.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     1353 2022-08-09 02:22:40.000000 linora-2.0.0rc1/linora/chart/_hlines.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     4557 2022-08-09 02:22:54.000000 linora-2.0.0rc1/linora/chart/_line.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     4806 2022-08-09 02:23:07.000000 linora-2.0.0rc1/linora/chart/_line3D.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    11321 2022-04-24 14:02:43.000000 linora-2.0.0rc1/linora/chart/_metrics.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     3835 2022-08-03 06:13:51.000000 linora-2.0.0rc1/linora/chart/_pie.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     8171 2022-08-09 08:34:12.000000 linora-2.0.0rc1/linora/chart/_plot.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     1983 2022-08-09 08:12:27.000000 linora-2.0.0rc1/linora/chart/_polygon.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     5312 2022-08-09 02:23:32.000000 linora-2.0.0rc1/linora/chart/_radar.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     2511 2022-08-09 08:11:53.000000 linora-2.0.0rc1/linora/chart/_rectangle.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     2242 2022-08-09 08:11:43.000000 linora-2.0.0rc1/linora/chart/_regularpolygon.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     5718 2022-08-09 02:23:50.000000 linora-2.0.0rc1/linora/chart/_scatter.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     6367 2022-08-09 02:24:07.000000 linora-2.0.0rc1/linora/chart/_scatter3D.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     1350 2022-08-09 02:24:44.000000 linora-2.0.0rc1/linora/chart/_vlines.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     2137 2022-08-09 08:08:19.000000 linora-2.0.0rc1/linora/chart/_wedge.py
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-08-04 02:09:53.000000 linora-2.0.0rc1/linora/data/
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-08-04 02:09:53.000000 linora-2.0.0rc1/linora/data/Dataset/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)       42 2022-06-08 08:59:03.000000 linora-2.0.0rc1/linora/data/Dataset/__init__.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    27211 2022-08-29 09:18:04.000000 linora-2.0.0rc1/linora/data/Dataset/_data.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    13157 2022-06-08 08:22:31.000000 linora-2.0.0rc1/linora/data/Dataset/_dataset.py
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-08-04 02:09:53.000000 linora-2.0.0rc1/linora/data/TextLineDataset/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)       50 2022-05-27 04:17:36.000000 linora-2.0.0rc1/linora/data/TextLineDataset/__init__.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    15392 2022-05-27 08:07:05.000000 linora-2.0.0rc1/linora/data/TextLineDataset/_dataset.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)      215 2022-12-07 05:59:38.000000 linora-2.0.0rc1/linora/data/__init__.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     4001 2023-07-12 06:10:51.000000 linora-2.0.0rc1/linora/data/_compress.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    11876 2022-12-07 06:31:44.000000 linora-2.0.0rc1/linora/data/_sql_io_dataset.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     1941 2022-06-01 08:26:01.000000 linora-2.0.0rc1/linora/data/_utils.py
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-08-04 02:09:53.000000 linora-2.0.0rc1/linora/data/datasets/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)       85 2022-08-19 09:00:53.000000 linora-2.0.0rc1/linora/data/datasets/__init__.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     2071 2022-12-01 09:47:11.000000 linora-2.0.0rc1/linora/data/datasets/_config_path.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    19314 2022-06-08 08:37:02.000000 linora-2.0.0rc1/linora/data/datasets/_mnist.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     1293 2022-12-02 05:08:27.000000 linora-2.0.0rc1/linora/data/datasets/_utils.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)   264001 2022-08-22 01:29:59.000000 linora-2.0.0rc1/linora/data/datasets/_weather.py
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-08-04 02:09:53.000000 linora-2.0.0rc1/linora/feature_column/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)      277 2023-03-22 09:25:19.000000 linora-2.0.0rc1/linora/feature_column/__init__.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    20098 2023-03-21 09:04:16.000000 linora-2.0.0rc1/linora/feature_column/_categorical.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     7622 2023-03-23 09:40:18.000000 linora-2.0.0rc1/linora/feature_column/_datetime.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     6523 2023-03-24 06:31:58.000000 linora-2.0.0rc1/linora/feature_column/_feature.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    10691 2023-03-21 02:03:11.000000 linora-2.0.0rc1/linora/feature_column/_feature_categorical.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     3687 2023-03-23 09:10:38.000000 linora-2.0.0rc1/linora/feature_column/_feature_datetime.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     5298 2023-03-21 02:03:40.000000 linora-2.0.0rc1/linora/feature_column/_feature_normalize.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    11083 2023-03-24 01:40:41.000000 linora-2.0.0rc1/linora/feature_column/_feature_numerical.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     8774 2023-03-21 09:03:05.000000 linora-2.0.0rc1/linora/feature_column/_normalize.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    21492 2023-03-24 01:26:31.000000 linora-2.0.0rc1/linora/feature_column/_numerical.py
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-08-04 02:09:53.000000 linora-2.0.0rc1/linora/feature_column/boundary/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)       55 2022-04-24 14:02:43.000000 linora-2.0.0rc1/linora/feature_column/boundary/__init__.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     3495 2022-04-24 14:02:43.000000 linora-2.0.0rc1/linora/feature_column/boundary/_boundary.py
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-08-04 02:09:53.000000 linora-2.0.0rc1/linora/feature_selection/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)       94 2022-04-24 14:02:43.000000 linora-2.0.0rc1/linora/feature_selection/__init__.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     1780 2022-04-24 14:02:43.000000 linora-2.0.0rc1/linora/feature_selection/_credit.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     2622 2022-05-12 01:17:51.000000 linora-2.0.0rc1/linora/feature_selection/_select.py
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-08-04 02:09:53.000000 linora-2.0.0rc1/linora/gfile/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)       33 2022-04-24 14:02:43.000000 linora-2.0.0rc1/linora/gfile/__init__.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     5895 2022-11-23 09:16:08.000000 linora-2.0.0rc1/linora/gfile/_gfile.py
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-08-04 02:09:53.000000 linora-2.0.0rc1/linora/image/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)      636 2022-05-16 10:12:12.000000 linora-2.0.0rc1/linora/image/__init__.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     1442 2022-05-26 02:08:30.000000 linora-2.0.0rc1/linora/image/_image_aug.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     3596 2022-05-18 00:54:35.000000 linora-2.0.0rc1/linora/image/_image_box.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    29992 2022-11-30 09:53:59.000000 linora-2.0.0rc1/linora/image/_image_color.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    12038 2022-05-26 02:07:59.000000 linora-2.0.0rc1/linora/image/_image_color_aug.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     8666 2022-05-16 09:32:03.000000 linora-2.0.0rc1/linora/image/_image_crop.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     2963 2022-05-26 02:08:58.000000 linora-2.0.0rc1/linora/image/_image_crop_aug.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    11337 2022-05-27 06:56:17.000000 linora-2.0.0rc1/linora/image/_image_draw.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     2305 2022-05-27 07:05:28.000000 linora-2.0.0rc1/linora/image/_image_draw_aug.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    16607 2022-11-18 03:22:32.000000 linora-2.0.0rc1/linora/image/_image_feature.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     8805 2022-05-13 01:24:35.000000 linora-2.0.0rc1/linora/image/_image_filter.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     5629 2022-05-26 02:09:23.000000 linora-2.0.0rc1/linora/image/_image_filter_aug.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     7215 2022-08-01 08:30:47.000000 linora-2.0.0rc1/linora/image/_image_grid.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     2728 2023-08-04 02:03:22.000000 linora-2.0.0rc1/linora/image/_image_io.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     2345 2022-05-22 03:19:04.000000 linora-2.0.0rc1/linora/image/_image_io_aug.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    13075 2022-05-17 03:28:28.000000 linora-2.0.0rc1/linora/image/_image_noise.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     7787 2022-05-26 02:09:49.000000 linora-2.0.0rc1/linora/image/_image_noise_aug.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     8431 2022-04-25 13:29:23.000000 linora-2.0.0rc1/linora/image/_image_pairs.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    21630 2022-05-25 09:46:33.000000 linora-2.0.0rc1/linora/image/_image_position.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    12989 2022-05-26 02:40:18.000000 linora-2.0.0rc1/linora/image/_image_position_aug.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     7012 2022-05-16 02:51:05.000000 linora-2.0.0rc1/linora/image/_image_rescale.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     4257 2022-05-26 02:10:15.000000 linora-2.0.0rc1/linora/image/_image_rescale_aug.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     2527 2022-05-25 02:36:08.000000 linora-2.0.0rc1/linora/image/_image_resize.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)      519 2022-05-09 09:56:14.000000 linora-2.0.0rc1/linora/image/_image_resize_aug.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    41696 2022-05-27 06:48:41.000000 linora-2.0.0rc1/linora/image/_image_rgb.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     5315 2023-04-14 07:37:25.000000 linora-2.0.0rc1/linora/image/_image_util.py
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-08-04 02:09:53.000000 linora-2.0.0rc1/linora/metrics/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)      231 2022-04-24 14:02:43.000000 linora-2.0.0rc1/linora/metrics/__init__.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    27844 2022-06-22 02:45:29.000000 linora-2.0.0rc1/linora/metrics/_classification.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     4966 2022-05-26 08:02:56.000000 linora-2.0.0rc1/linora/metrics/_image.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     2335 2022-05-26 07:22:49.000000 linora-2.0.0rc1/linora/metrics/_metrics.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     2568 2022-06-21 10:20:14.000000 linora-2.0.0rc1/linora/metrics/_rank.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    18341 2022-11-21 07:42:50.000000 linora-2.0.0rc1/linora/metrics/_regression.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     2518 2023-02-24 06:52:37.000000 linora-2.0.0rc1/linora/metrics/_text.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)      370 2022-06-21 10:10:45.000000 linora-2.0.0rc1/linora/metrics/_utils.py
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-08-04 02:09:53.000000 linora-2.0.0rc1/linora/metrics/distance/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)       97 2022-04-24 14:02:43.000000 linora-2.0.0rc1/linora/metrics/distance/__init__.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    10758 2022-06-22 01:50:38.000000 linora-2.0.0rc1/linora/metrics/distance/_distance.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     5635 2022-04-24 14:02:43.000000 linora-2.0.0rc1/linora/metrics/distance/_divergence.py
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-08-04 02:09:53.000000 linora-2.0.0rc1/linora/parallel/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)       77 2022-04-24 14:02:43.000000 linora-2.0.0rc1/linora/parallel/__init__.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     5619 2022-04-24 14:02:43.000000 linora-2.0.0rc1/linora/parallel/_process.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     5408 2022-04-24 14:02:43.000000 linora-2.0.0rc1/linora/parallel/_thread.py
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-08-04 02:09:53.000000 linora-2.0.0rc1/linora/param_search/
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-08-04 02:09:53.000000 linora-2.0.0rc1/linora/param_search/GEClassifier/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     2941 2022-04-24 14:02:43.000000 linora-2.0.0rc1/linora/param_search/GEClassifier/_GridSearch.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     3182 2022-04-24 14:02:43.000000 linora-2.0.0rc1/linora/param_search/GEClassifier/_RandomSearch.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)      142 2022-04-24 14:02:43.000000 linora-2.0.0rc1/linora/param_search/GEClassifier/__init__.py
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-08-04 02:09:53.000000 linora-2.0.0rc1/linora/param_search/GERegressor/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     3219 2022-04-24 14:02:43.000000 linora-2.0.0rc1/linora/param_search/GERegressor/_RandomSearch.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)       71 2022-04-24 14:02:43.000000 linora-2.0.0rc1/linora/param_search/GERegressor/__init__.py
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-08-04 02:09:53.000000 linora-2.0.0rc1/linora/param_search/LGBMClassifier/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     7659 2022-05-20 03:53:11.000000 linora-2.0.0rc1/linora/param_search/LGBMClassifier/_GridSearch.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     7646 2022-05-20 03:52:49.000000 linora-2.0.0rc1/linora/param_search/LGBMClassifier/_RandomSearch.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)      144 2022-05-05 06:13:26.000000 linora-2.0.0rc1/linora/param_search/LGBMClassifier/__init__.py
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-08-04 02:09:53.000000 linora-2.0.0rc1/linora/param_search/LGBMRegressor/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     7656 2022-05-20 03:53:26.000000 linora-2.0.0rc1/linora/param_search/LGBMRegressor/_GridSearch.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     7644 2022-05-20 03:52:33.000000 linora-2.0.0rc1/linora/param_search/LGBMRegressor/_RandomSearch.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)      141 2022-05-05 06:14:26.000000 linora-2.0.0rc1/linora/param_search/LGBMRegressor/__init__.py
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-08-04 02:09:53.000000 linora-2.0.0rc1/linora/param_search/XGBClassifier/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     8752 2022-05-20 03:51:53.000000 linora-2.0.0rc1/linora/param_search/XGBClassifier/_GridSearch.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     8724 2022-05-20 03:52:15.000000 linora-2.0.0rc1/linora/param_search/XGBClassifier/_RandomSearch.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)      142 2022-04-24 14:02:43.000000 linora-2.0.0rc1/linora/param_search/XGBClassifier/__init__.py
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-08-04 02:09:53.000000 linora-2.0.0rc1/linora/param_search/XGBRanker/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     5599 2022-04-24 14:02:43.000000 linora-2.0.0rc1/linora/param_search/XGBRanker/_GridSearch.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     5904 2022-04-24 14:02:43.000000 linora-2.0.0rc1/linora/param_search/XGBRanker/_RandomSearch.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)      138 2022-04-24 14:02:43.000000 linora-2.0.0rc1/linora/param_search/XGBRanker/__init__.py
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-08-04 02:09:53.000000 linora-2.0.0rc1/linora/param_search/XGBRegressor/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     8912 2022-05-20 03:51:33.000000 linora-2.0.0rc1/linora/param_search/XGBRegressor/_GridSearch.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     8943 2022-05-20 03:51:09.000000 linora-2.0.0rc1/linora/param_search/XGBRegressor/_RandomSearch.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)      140 2022-04-24 14:02:43.000000 linora-2.0.0rc1/linora/param_search/XGBRegressor/__init__.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    13838 2022-06-15 06:08:40.000000 linora-2.0.0rc1/linora/param_search/_HyperParameters.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     9259 2023-03-27 01:31:53.000000 linora-2.0.0rc1/linora/param_search/_Search.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)      177 2022-06-08 09:41:40.000000 linora-2.0.0rc1/linora/param_search/__init__.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     9231 2022-05-22 02:43:27.000000 linora-2.0.0rc1/linora/param_search/_config.py
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-08-04 02:09:53.000000 linora-2.0.0rc1/linora/sample/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)      162 2022-05-10 08:08:14.000000 linora-2.0.0rc1/linora/sample/__init__.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     4847 2022-11-04 06:31:17.000000 linora-2.0.0rc1/linora/sample/_fold.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     3542 2022-04-24 14:02:43.000000 linora-2.0.0rc1/linora/sample/_random_walker.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     7072 2022-11-24 03:05:14.000000 linora-2.0.0rc1/linora/sample/_sampling.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     4051 2022-04-27 01:42:13.000000 linora-2.0.0rc1/linora/sample/_timeseries_kfold.py
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-08-04 02:09:53.000000 linora-2.0.0rc1/linora/server/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)      149 2023-07-17 10:05:23.000000 linora-2.0.0rc1/linora/server/__init__.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    19067 2023-03-27 01:12:25.000000 linora-2.0.0rc1/linora/server/_email.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    17119 2023-03-27 01:12:06.000000 linora-2.0.0rc1/linora/server/_email_utils.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     4652 2023-07-19 10:10:21.000000 linora-2.0.0rc1/linora/server/_monitor_sys.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    13495 2023-03-27 00:57:47.000000 linora-2.0.0rc1/linora/server/_schedulers.py
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-08-04 02:09:53.000000 linora-2.0.0rc1/linora/server/message/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    11784 2022-06-14 08:26:34.000000 linora-2.0.0rc1/linora/server/message/_BotDingTalk.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)      520 2022-04-24 14:02:43.000000 linora-2.0.0rc1/linora/server/message/_BotFeiShu.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)       95 2023-03-28 05:07:33.000000 linora-2.0.0rc1/linora/server/message/__init__.py
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-08-04 02:09:53.000000 linora-2.0.0rc1/linora/text/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)      149 2022-04-24 14:02:43.000000 linora-2.0.0rc1/linora/text/__init__.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     6243 2022-04-24 14:02:43.000000 linora-2.0.0rc1/linora/text/_sequence.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     4002 2022-04-24 14:02:43.000000 linora-2.0.0rc1/linora/text/_util.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     2267 2022-04-24 14:02:43.000000 linora-2.0.0rc1/linora/text/_vectorizer.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     3037 2023-02-24 05:40:38.000000 linora-2.0.0rc1/linora/text/_word_processing.py
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-08-04 02:09:53.000000 linora-2.0.0rc1/linora/train/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)      308 2022-08-24 08:42:12.000000 linora-2.0.0rc1/linora/train/__init__.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     2922 2022-09-01 01:52:14.000000 linora-2.0.0rc1/linora/train/_callback.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     1781 2022-08-24 02:28:50.000000 linora-2.0.0rc1/linora/train/_csvlogger.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     2371 2022-08-25 05:33:20.000000 linora-2.0.0rc1/linora/train/_earlystopping.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     1768 2022-08-24 02:54:41.000000 linora-2.0.0rc1/linora/train/_modelcheckpoint.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     2193 2022-08-24 01:53:17.000000 linora-2.0.0rc1/linora/train/_remotemonitor.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     2180 2022-09-01 01:55:31.000000 linora-2.0.0rc1/linora/train/_terminateonnan.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     7364 2022-08-27 02:43:20.000000 linora-2.0.0rc1/linora/train/_visual.py
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-08-04 02:09:53.000000 linora-2.0.0rc1/linora/train/lr/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)       75 2022-08-25 02:12:32.000000 linora-2.0.0rc1/linora/train/lr/__init__.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    12872 2022-08-26 07:47:29.000000 linora-2.0.0rc1/linora/train/lr/_lr.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     1991 2022-08-25 03:30:35.000000 linora-2.0.0rc1/linora/train/lr/_schedulers.py
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-08-04 02:09:53.000000 linora-2.0.0rc1/linora/utils/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)      241 2022-11-10 02:19:13.000000 linora-2.0.0rc1/linora/utils/__init__.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     1444 2022-04-24 14:02:43.000000 linora-2.0.0rc1/linora/utils/_config.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    19259 2023-03-27 01:06:27.000000 linora-2.0.0rc1/linora/utils/_email.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    17119 2022-11-23 01:25:02.000000 linora-2.0.0rc1/linora/utils/_email_utils.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     9213 2022-05-11 03:45:54.000000 linora-2.0.0rc1/linora/utils/_logger.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     4106 2022-05-31 11:52:27.000000 linora-2.0.0rc1/linora/utils/_progbar.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    13658 2023-03-27 01:10:43.000000 linora-2.0.0rc1/linora/utils/_schedulers.py
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-08-04 02:09:53.000000 linora-2.0.0rc1/linora/utils/message/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    11965 2023-03-28 05:06:17.000000 linora-2.0.0rc1/linora/utils/message/_BotDingTalk.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)      739 2023-03-28 05:05:36.000000 linora-2.0.0rc1/linora/utils/message/_BotFeiShu.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)       93 2023-03-28 05:03:07.000000 linora-2.0.0rc1/linora/utils/message/__init__.py
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-08-04 02:09:53.000000 linora-2.0.0rc1/linora/utils/pip/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)       35 2022-08-04 02:59:58.000000 linora-2.0.0rc1/linora/utils/pip/__init__.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    14751 2022-08-05 04:59:06.000000 linora-2.0.0rc1/linora/utils/pip/_pip.py
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-08-04 02:09:53.000000 linora-2.0.0rc1/linora/vedio/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)       75 2023-04-14 07:02:50.000000 linora-2.0.0rc1/linora/vedio/__init__.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)    18807 2023-07-28 01:59:16.000000 linora-2.0.0rc1/linora/vedio/_vedio_io.py
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     3801 2023-04-23 08:50:15.000000 linora-2.0.0rc1/linora/vedio/_vedio_util.py
+drwxr-xr-x   0 liyanpeng   (501) staff       (20)        0 2023-08-04 02:09:53.000000 linora-2.0.0rc1/linora.egg-info/
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     3736 2023-08-04 02:09:53.000000 linora-2.0.0rc1/linora.egg-info/PKG-INFO
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     5633 2023-08-04 02:09:53.000000 linora-2.0.0rc1/linora.egg-info/SOURCES.txt
+-rw-r--r--   0 liyanpeng   (501) staff       (20)        1 2023-08-04 02:09:53.000000 linora-2.0.0rc1/linora.egg-info/dependency_links.txt
+-rw-r--r--   0 liyanpeng   (501) staff       (20)        1 2023-08-04 02:09:53.000000 linora-2.0.0rc1/linora.egg-info/not-zip-safe
+-rw-r--r--   0 liyanpeng   (501) staff       (20)       70 2023-08-04 02:09:53.000000 linora-2.0.0rc1/linora.egg-info/requires.txt
+-rw-r--r--   0 liyanpeng   (501) staff       (20)        7 2023-08-04 02:09:53.000000 linora-2.0.0rc1/linora.egg-info/top_level.txt
+-rw-r--r--   0 liyanpeng   (501) staff       (20)       79 2023-08-04 02:09:53.000000 linora-2.0.0rc1/setup.cfg
+-rw-r--r--   0 liyanpeng   (501) staff       (20)     1647 2023-08-04 02:07:30.000000 linora-2.0.0rc1/setup.py
```

### Comparing `linora-2.0.0rc0/PKG-INFO` & `linora-2.0.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linora
-Version: 2.0.0rc0
+Version: 2.0.0rc1
 Summary: Simple and efficient tools for data mining and data analysis.
 Home-page: https://github.com/Hourout/linora
 Author: JinQing Lee
 Author-email: hourout@163.com
 License: Apache License Version 2.0
 Description: ![](https://github.com/Hourout/linora/blob/master/image/linora.png)
```

### Comparing `linora-2.0.0rc0/README.md` & `linora-2.0.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/__init__.py` & `linora-2.0.0rc1/linora/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from linora import sample
 from linora import server
 from linora import text
 from linora import train
 from linora import utils
 from linora import vedio
 
-__version__ = '2.0.0rc0'
+__version__ = '2.0.0rc1'
 __author__ = 'JinQing Lee'
 
 def _version():
     print(f"""
 ------------------------------------------------------------------------------------
       Linora
 --------------------
```

### Comparing `linora-2.0.0rc0/linora/audio/_audio_io.py` & `linora-2.0.0rc1/linora/audio/_audio_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 import av
 import numpy as np
 
 __all__ = ['read_audio', 'save_audio', 'AudioStream']
 
 
 def save_audio(filename, audio_array, audio_fps=44100, audio_codec=None, audio_options=None):
-    """
-    Writes a 2d array in [C, L] format in a audio file
+    """Writes a 2d array in [C, L] format in a audio file.
+    
     Args:
         filename: path where the video will be saved.
-        audio_array: array[C, N] containing the audio, where C is the number of channels
-            and N is the number of samples
+        audio_array: array[C, L] containing the audio, where C is the number of channels
+            and L is the number of samples.
         audio_fps: audio sample rate, typically 44100 or 48000
         audio_codec: the name of the audio codec, i.e. "mp3", "aac", etc.
         audio_options: dictionary containing options to be passed into the PyAV audio stream
     """
     audio_format_dtypes = {
             "dbl": "<f8",
             "dblp": "<f8",
```

### Comparing `linora-2.0.0rc0/linora/chart/_arrow.py` & `linora-2.0.0rc1/linora/chart/_arrow.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/chart/_bar.py` & `linora-2.0.0rc1/linora/chart/_bar.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/chart/_base.py` & `linora-2.0.0rc1/linora/chart/_base.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/chart/_boxplot.py` & `linora-2.0.0rc1/linora/chart/_boxplot.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/chart/_circle.py` & `linora-2.0.0rc1/linora/chart/_circle.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/chart/_coherence.py` & `linora-2.0.0rc1/linora/chart/_coherence.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/chart/_config.py` & `linora-2.0.0rc1/linora/chart/_config.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/chart/_csd.py` & `linora-2.0.0rc1/linora/chart/_csd.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/chart/_ellipse.py` & `linora-2.0.0rc1/linora/chart/_ellipse.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/chart/_errorbar.py` & `linora-2.0.0rc1/linora/chart/_errorbar.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/chart/_feature.py` & `linora-2.0.0rc1/linora/chart/_feature.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/chart/_fillline.py` & `linora-2.0.0rc1/linora/chart/_fillline.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/chart/_grid.py` & `linora-2.0.0rc1/linora/chart/_grid.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/chart/_hist.py` & `linora-2.0.0rc1/linora/chart/_hist.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/chart/_hist2d.py` & `linora-2.0.0rc1/linora/chart/_hist2d.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/chart/_hlines.py` & `linora-2.0.0rc1/linora/chart/_hlines.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/chart/_line.py` & `linora-2.0.0rc1/linora/chart/_line.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/chart/_line3D.py` & `linora-2.0.0rc1/linora/chart/_line3D.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/chart/_metrics.py` & `linora-2.0.0rc1/linora/chart/_metrics.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/chart/_pie.py` & `linora-2.0.0rc1/linora/chart/_pie.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/chart/_plot.py` & `linora-2.0.0rc1/linora/chart/_plot.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/chart/_polygon.py` & `linora-2.0.0rc1/linora/chart/_polygon.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/chart/_radar.py` & `linora-2.0.0rc1/linora/chart/_radar.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/chart/_rectangle.py` & `linora-2.0.0rc1/linora/chart/_rectangle.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/chart/_regularpolygon.py` & `linora-2.0.0rc1/linora/chart/_regularpolygon.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/chart/_scatter.py` & `linora-2.0.0rc1/linora/chart/_scatter.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/chart/_scatter3D.py` & `linora-2.0.0rc1/linora/chart/_scatter3D.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/chart/_vlines.py` & `linora-2.0.0rc1/linora/chart/_vlines.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/chart/_wedge.py` & `linora-2.0.0rc1/linora/chart/_wedge.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/data/Dataset/_data.py` & `linora-2.0.0rc1/linora/data/Dataset/_data.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/data/Dataset/_dataset.py` & `linora-2.0.0rc1/linora/data/Dataset/_dataset.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/data/TextLineDataset/_dataset.py` & `linora-2.0.0rc1/linora/data/TextLineDataset/_dataset.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/data/_compress.py` & `linora-2.0.0rc1/linora/data/_compress.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,22 +67,22 @@
         compression files name.
     """
     if gfile.isdir(files):
         mat = file.split('.')[-1]
         if mat in ['zip']:
             with zipfile.ZipFile(file, 'w', zipfile.ZIP_DEFLATED) as z:
                 for dirpath, dirnames, filenames in gfile.walk(files):
-                    fpath = dirpath.replace(startdir, '')
+                    fpath = dirpath.replace(files, '')
                     fpath = fpath and fpath + os.sep or ''
                     for filename in filenames:
                         z.write(gfile.path_join(dirpath, filename), gfile.path_join(fpath, filename))
         elif mat in ['tar']:
             with tarfile.open(file, 'w') as tar:
                 for dirpath, dirnames, filenames in gfile.walk(files):
-                    fpath = dirpath.replace(startdir, '')
+                    fpath = dirpath.replace(files, '')
                     fpath = fpath and fpath + os.sep or ''
                     for filename in filenames:
                         tar.add(gfile.path_join(dirpath, filename), gfile.path_join(fpath, filename))
         else:
             raise ValueError("`file` should be type of ['.tar', '.zip'].")
     else:
         if isinstance(files, str):
```

### Comparing `linora-2.0.0rc0/linora/data/_sql_io_dataset.py` & `linora-2.0.0rc1/linora/data/_sql_io_dataset.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/data/_utils.py` & `linora-2.0.0rc1/linora/data/_utils.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/data/datasets/_config_path.py` & `linora-2.0.0rc1/linora/data/datasets/_config_path.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/data/datasets/_mnist.py` & `linora-2.0.0rc1/linora/data/datasets/_mnist.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/data/datasets/_utils.py` & `linora-2.0.0rc1/linora/data/datasets/_utils.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/data/datasets/_weather.py` & `linora-2.0.0rc1/linora/data/datasets/_weather.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/feature_column/_categorical.py` & `linora-2.0.0rc1/linora/feature_column/_categorical.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/feature_column/_datetime.py` & `linora-2.0.0rc1/linora/feature_column/_datetime.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/feature_column/_feature.py` & `linora-2.0.0rc1/linora/feature_column/_feature.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/feature_column/_feature_categorical.py` & `linora-2.0.0rc1/linora/feature_column/_feature_categorical.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/feature_column/_feature_datetime.py` & `linora-2.0.0rc1/linora/feature_column/_feature_datetime.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/feature_column/_feature_normalize.py` & `linora-2.0.0rc1/linora/feature_column/_feature_normalize.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/feature_column/_feature_numerical.py` & `linora-2.0.0rc1/linora/feature_column/_feature_numerical.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/feature_column/_normalize.py` & `linora-2.0.0rc1/linora/feature_column/_normalize.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/feature_column/_numerical.py` & `linora-2.0.0rc1/linora/feature_column/_numerical.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/feature_column/boundary/_boundary.py` & `linora-2.0.0rc1/linora/feature_column/boundary/_boundary.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/feature_selection/_credit.py` & `linora-2.0.0rc1/linora/feature_selection/_credit.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/feature_selection/_select.py` & `linora-2.0.0rc1/linora/feature_selection/_select.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/gfile/_gfile.py` & `linora-2.0.0rc1/linora/gfile/_gfile.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/image/__init__.py` & `linora-2.0.0rc1/linora/image/__init__.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/image/_image_aug.py` & `linora-2.0.0rc1/linora/image/_image_aug.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/image/_image_box.py` & `linora-2.0.0rc1/linora/image/_image_box.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/image/_image_color.py` & `linora-2.0.0rc1/linora/image/_image_color.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/image/_image_color_aug.py` & `linora-2.0.0rc1/linora/image/_image_color_aug.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/image/_image_crop.py` & `linora-2.0.0rc1/linora/image/_image_crop.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/image/_image_crop_aug.py` & `linora-2.0.0rc1/linora/image/_image_crop_aug.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/image/_image_draw.py` & `linora-2.0.0rc1/linora/image/_image_draw.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/image/_image_draw_aug.py` & `linora-2.0.0rc1/linora/image/_image_draw_aug.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/image/_image_feature.py` & `linora-2.0.0rc1/linora/image/_image_feature.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/image/_image_filter.py` & `linora-2.0.0rc1/linora/image/_image_filter.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/image/_image_filter_aug.py` & `linora-2.0.0rc1/linora/image/_image_filter_aug.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/image/_image_grid.py` & `linora-2.0.0rc1/linora/image/_image_grid.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/image/_image_io.py` & `linora-2.0.0rc1/linora/image/_image_io.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import io
 import base64
 
 import requests
-from PIL import Image
+from PIL import Image, ImageOps
 
 from linora.gfile._gfile import exists
 
 __all__ = ['read_image', 'save_image', 'encode_base64', 'decode_base64']
 
 
 def read_image(filename):
@@ -23,15 +23,15 @@
                 image = Image.open(io.BytesIO(f.read()))
         else:
             image = Image.open(io.BytesIO(requests.get(filename).content), 'r')
     elif isinstance(filename, io.BytesIO):
         image = Image.open(filename)
     else:
         raise TypeError('path should be absolute path or io.BytesIO')
-    return image
+    return ImageOps.exif_transpose(image)
 
 
 def save_image(filename, image, file_format=None, **kwargs):
     """Saves an image stored as a Numpy array to a path or file object.
     
     if save gif image, please use save_image(filename, image, file_format=None, save_all=True, append_images=[im1, im2, ...])
```

### Comparing `linora-2.0.0rc0/linora/image/_image_io_aug.py` & `linora-2.0.0rc1/linora/image/_image_io_aug.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/image/_image_noise.py` & `linora-2.0.0rc1/linora/image/_image_noise.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/image/_image_noise_aug.py` & `linora-2.0.0rc1/linora/image/_image_noise_aug.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/image/_image_pairs.py` & `linora-2.0.0rc1/linora/image/_image_pairs.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/image/_image_position.py` & `linora-2.0.0rc1/linora/image/_image_position.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/image/_image_position_aug.py` & `linora-2.0.0rc1/linora/image/_image_position_aug.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/image/_image_rescale.py` & `linora-2.0.0rc1/linora/image/_image_rescale.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/image/_image_rescale_aug.py` & `linora-2.0.0rc1/linora/image/_image_rescale_aug.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/image/_image_resize.py` & `linora-2.0.0rc1/linora/image/_image_resize.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/image/_image_resize_aug.py` & `linora-2.0.0rc1/linora/image/_image_resize_aug.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/image/_image_rgb.py` & `linora-2.0.0rc1/linora/image/_image_rgb.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/image/_image_util.py` & `linora-2.0.0rc1/linora/image/_image_util.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/metrics/_classification.py` & `linora-2.0.0rc1/linora/metrics/_classification.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/metrics/_image.py` & `linora-2.0.0rc1/linora/metrics/_image.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/metrics/_metrics.py` & `linora-2.0.0rc1/linora/metrics/_metrics.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/metrics/_rank.py` & `linora-2.0.0rc1/linora/metrics/_rank.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/metrics/_regression.py` & `linora-2.0.0rc1/linora/metrics/_regression.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/metrics/_text.py` & `linora-2.0.0rc1/linora/metrics/_text.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/metrics/distance/_distance.py` & `linora-2.0.0rc1/linora/metrics/distance/_distance.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/metrics/distance/_divergence.py` & `linora-2.0.0rc1/linora/metrics/distance/_divergence.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/parallel/_process.py` & `linora-2.0.0rc1/linora/parallel/_process.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/parallel/_thread.py` & `linora-2.0.0rc1/linora/parallel/_thread.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/param_search/GEClassifier/_GridSearch.py` & `linora-2.0.0rc1/linora/param_search/GEClassifier/_GridSearch.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/param_search/GEClassifier/_RandomSearch.py` & `linora-2.0.0rc1/linora/param_search/GEClassifier/_RandomSearch.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/param_search/GERegressor/_RandomSearch.py` & `linora-2.0.0rc1/linora/param_search/GERegressor/_RandomSearch.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/param_search/LGBMClassifier/_GridSearch.py` & `linora-2.0.0rc1/linora/param_search/LGBMClassifier/_GridSearch.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/param_search/LGBMClassifier/_RandomSearch.py` & `linora-2.0.0rc1/linora/param_search/LGBMClassifier/_RandomSearch.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/param_search/LGBMRegressor/_GridSearch.py` & `linora-2.0.0rc1/linora/param_search/LGBMRegressor/_GridSearch.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/param_search/LGBMRegressor/_RandomSearch.py` & `linora-2.0.0rc1/linora/param_search/LGBMRegressor/_RandomSearch.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/param_search/XGBClassifier/_GridSearch.py` & `linora-2.0.0rc1/linora/param_search/XGBClassifier/_GridSearch.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/param_search/XGBClassifier/_RandomSearch.py` & `linora-2.0.0rc1/linora/param_search/XGBClassifier/_RandomSearch.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/param_search/XGBRanker/_GridSearch.py` & `linora-2.0.0rc1/linora/param_search/XGBRanker/_GridSearch.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/param_search/XGBRanker/_RandomSearch.py` & `linora-2.0.0rc1/linora/param_search/XGBRanker/_RandomSearch.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/param_search/XGBRegressor/_GridSearch.py` & `linora-2.0.0rc1/linora/param_search/XGBRegressor/_GridSearch.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/param_search/XGBRegressor/_RandomSearch.py` & `linora-2.0.0rc1/linora/param_search/XGBRegressor/_RandomSearch.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/param_search/_HyperParameters.py` & `linora-2.0.0rc1/linora/param_search/_HyperParameters.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/param_search/_Search.py` & `linora-2.0.0rc1/linora/param_search/_Search.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/param_search/_config.py` & `linora-2.0.0rc1/linora/param_search/_config.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/sample/_fold.py` & `linora-2.0.0rc1/linora/sample/_fold.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/sample/_random_walker.py` & `linora-2.0.0rc1/linora/sample/_random_walker.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/sample/_sampling.py` & `linora-2.0.0rc1/linora/sample/_sampling.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/sample/_timeseries_kfold.py` & `linora-2.0.0rc1/linora/sample/_timeseries_kfold.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/server/_email.py` & `linora-2.0.0rc1/linora/server/_email.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/server/_email_utils.py` & `linora-2.0.0rc1/linora/server/_email_utils.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/server/_schedulers.py` & `linora-2.0.0rc1/linora/server/_schedulers.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/server/message/_BotDingTalk.py` & `linora-2.0.0rc1/linora/server/message/_BotDingTalk.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/server/message/_BotFeiShu.py` & `linora-2.0.0rc1/linora/server/message/_BotFeiShu.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/text/_sequence.py` & `linora-2.0.0rc1/linora/text/_sequence.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/text/_util.py` & `linora-2.0.0rc1/linora/text/_util.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/text/_vectorizer.py` & `linora-2.0.0rc1/linora/text/_vectorizer.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/text/_word_processing.py` & `linora-2.0.0rc1/linora/text/_word_processing.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/train/_callback.py` & `linora-2.0.0rc1/linora/train/_callback.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/train/_csvlogger.py` & `linora-2.0.0rc1/linora/train/_csvlogger.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/train/_earlystopping.py` & `linora-2.0.0rc1/linora/train/_earlystopping.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/train/_modelcheckpoint.py` & `linora-2.0.0rc1/linora/train/_modelcheckpoint.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/train/_remotemonitor.py` & `linora-2.0.0rc1/linora/train/_remotemonitor.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/train/_terminateonnan.py` & `linora-2.0.0rc1/linora/train/_terminateonnan.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/train/_visual.py` & `linora-2.0.0rc1/linora/train/_visual.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/train/lr/_lr.py` & `linora-2.0.0rc1/linora/train/lr/_lr.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/train/lr/_schedulers.py` & `linora-2.0.0rc1/linora/train/lr/_schedulers.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/utils/_config.py` & `linora-2.0.0rc1/linora/utils/_config.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/utils/_email.py` & `linora-2.0.0rc1/linora/utils/_email.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/utils/_email_utils.py` & `linora-2.0.0rc1/linora/utils/_email_utils.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/utils/_logger.py` & `linora-2.0.0rc1/linora/utils/_logger.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/utils/_progbar.py` & `linora-2.0.0rc1/linora/utils/_progbar.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/utils/_schedulers.py` & `linora-2.0.0rc1/linora/utils/_schedulers.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/utils/message/_BotDingTalk.py` & `linora-2.0.0rc1/linora/utils/message/_BotDingTalk.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/utils/message/_BotFeiShu.py` & `linora-2.0.0rc1/linora/utils/message/_BotFeiShu.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/utils/pip/_pip.py` & `linora-2.0.0rc1/linora/utils/pip/_pip.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora/vedio/_vedio_io.py` & `linora-2.0.0rc1/linora/vedio/_vedio_io.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,41 +4,71 @@
 
 import av
 import numpy as np
 
 __all__ = ['read_vedio', 'read_vedio_timestamps', 'save_vedio', 'VedioStream']
 
 
-def format_convert(filename_in, filename_out):
-    """transform vedio file format.
+
+# def format_convert(filename_in, filename_out):
+#     """transform vedio file format.
     
-    Args
-        filename_in: input vedio path.
-        filename_out: output vedio path.
-    """
-    input_ = av.open(filename_in)
-    output = av.open(filename_out, "w")
+#     Args
+#         filename_in: input vedio path.
+#         filename_out: output vedio path.
+#     """
+#     input_ = av.open(filename_in)
+#     output = av.open(filename_out, "w")
+
+#     in_stream = input_.streams.video[0]
+#     out_stream = output.add_stream(template=in_stream)
+#     for packet in input_.demux(in_stream):
+#         if packet.dts is None:
+#             continue
+#         packet.stream = out_stream
+#         output.mux(packet)
+    
+#     in_audio = input_.streams.audio[0]
+#     out_audio = output.add_stream(template=in_audio)
+#     for packet in input_.demux(in_audio):
+#         if packet.dts is None:
+#             continue
+#         packet.stream = out_audio
+#         output.mux(packet)
 
-    in_stream = input_.streams.video[0]
-    out_stream = output.add_stream(template=in_stream)
+#     input_.close()
+#     output.close()
 
-    for packet in input_.demux(in_stream):
-        if packet.dts is None:
-            continue
-        packet.stream = out_stream
-        output.mux(packet)
+# def format_convert(filename_in, filename_out):
+#     """transform vedio file format.
+    
+#     Args
+#         filename_in: input vedio path.
+#         filename_out: output vedio path.
+#     """
+#     input_ = av.open(filename_in)
+#     output = av.open(filename_out, "w")
+
+#     in_stream = input_.streams.video[0]
+#     out_stream = output.add_stream(template=in_stream)
+
+#     for packet in input_.demux(in_stream):
+#         if packet.dts is None:
+#             continue
+#         packet.stream = out_stream
+#         output.mux(packet)
 
-    input_.close()
-    output.close()
+#     input_.close()
+#     output.close()
         
         
 def save_vedio(filename, video_array, video_fps, video_codec="libx264", options=None,
                audio_array=None, audio_fps=None, audio_codec=None, audio_options=None):
-    """
-    Writes a 4d array in [H, W, C, N] format in a video file
+    """Writes a 4d array in [H, W, C, N] format in a video file
+    
     Args:
         filename: path where the video will be saved
         video_array: array containing the individual frames, as a uint8 array in [H, W, C, N] format,
             or array of list or Image of list.
         video_fps: video frames per second
         video_codec: the name of the video codec, i.e. "libx264", "h264", etc.
         options: dictionary containing options to be passed into the PyAV video stream
@@ -126,14 +156,15 @@
     
     Args:
         src: path to the video file or bytes.
         start_sec: float, The start presentation time of the video.
         end_sec: float, The end presentation time of the video.
         vedio_format: The format of the output video shape. Can be "HWCN" (default), "Image" return pillow instance.
         vedio_type: The dtype of the output video.
+        audio_format: The format of the output audio shape. 'CL' or 'LC' e.g. 
     Returns:
         vedio: array[H, W, C, N]: the `N` video frames.
         audio: array[C, L]): the audio frames, where `C` is the number of channels and `L` is the number of points.
         metadata: metadata for the video and audio.
     """
     vedio_format = vedio_format.upper()
     if vedio_format!='IMAGE':
```

### Comparing `linora-2.0.0rc0/linora/vedio/_vedio_util.py` & `linora-2.0.0rc1/linora/vedio/_vedio_util.py`

 * *Files identical despite different names*

### Comparing `linora-2.0.0rc0/linora.egg-info/PKG-INFO` & `linora-2.0.0rc1/linora.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linora
-Version: 2.0.0rc0
+Version: 2.0.0rc1
 Summary: Simple and efficient tools for data mining and data analysis.
 Home-page: https://github.com/Hourout/linora
 Author: JinQing Lee
 Author-email: hourout@163.com
 License: Apache License Version 2.0
 Description: ![](https://github.com/Hourout/linora/blob/master/image/linora.png)
```

### Comparing `linora-2.0.0rc0/linora.egg-info/SOURCES.txt` & `linora-2.0.0rc1/linora.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -140,14 +140,15 @@
 linora/sample/_fold.py
 linora/sample/_random_walker.py
 linora/sample/_sampling.py
 linora/sample/_timeseries_kfold.py
 linora/server/__init__.py
 linora/server/_email.py
 linora/server/_email_utils.py
+linora/server/_monitor_sys.py
 linora/server/_schedulers.py
 linora/server/message/_BotDingTalk.py
 linora/server/message/_BotFeiShu.py
 linora/server/message/__init__.py
 linora/text/__init__.py
 linora/text/_sequence.py
 linora/text/_util.py
```

### Comparing `linora-2.0.0rc0/setup.py` & `linora-2.0.0rc1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 from setuptools import setup, find_packages
 
 def readme():
     with io.open('README.md', encoding='utf-8') as f:
         return f.read()
 
 setup(name='linora',
-      version='2.0.0rc0',
+      version='2.0.0rc1',
       install_requires=[
           'pandas>=1.5.2', 
           'Pillow>=9.3.0',
           'joblib>=1.2.0',
           'requests>=2.28.0',
-          'rarfile'
+          'rarfile',
+          'av'
       ],
       description='Simple and efficient tools for data mining and data analysis.',
       long_description=readme(),
       long_description_content_type='text/markdown',
       url='https://github.com/Hourout/linora',
       author='JinQing Lee',
       author_email='hourout@163.com',
```

