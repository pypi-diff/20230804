# Comparing `tmp/erwin-1.0.2.tar.gz` & `tmp/erwin-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erwin-1.0.2.tar", last modified: Wed Apr 13 09:44:19 2022, max compression
+gzip compressed data, was "erwin-1.1.0.tar", last modified: Fri Aug  4 10:39:12 2023, max compression
```

## Comparing `erwin-1.0.2.tar` & `erwin-1.1.0.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxr-xr-x   0 lamy      (1265) staff       (20)        0 2022-04-13 09:44:19.776281 erwin-1.0.2/
--rw-r--r--   0 lamy      (1265) staff       (20)       92 2022-04-13 09:42:28.000000 erwin-1.0.2/.bumpversion.cfg
--rw-r--r--   0 lamy      (1265) staff       (20)      290 2021-11-06 08:55:34.000000 erwin-1.0.2/.readthedocs.yaml
--rw-r-----   0 lamy      (1265) staff       (20)     1508 2021-10-30 16:47:16.000000 erwin-1.0.2/CONTRIBUTING.md
--rw-rw----   0 lamy      (1265) staff       (20)     1092 2021-10-30 16:45:51.000000 erwin-1.0.2/LICENSE
--rw-r--r--   0 lamy      (1265) staff       (20)     6360 2022-04-13 09:44:19.775915 erwin-1.0.2/PKG-INFO
--rw-rw----   0 lamy      (1265) staff       (20)     5290 2021-11-06 11:03:29.000000 erwin-1.0.2/README.md
-drwxr-xr-x   0 lamy      (1265) staff       (20)        0 2022-04-13 09:44:19.724938 erwin-1.0.2/doc/
--rw-rw----   0 lamy      (1265) staff       (20)      634 2021-11-05 07:29:11.000000 erwin-1.0.2/doc/Makefile
--rw-rw----   0 lamy      (1265) staff       (20)      777 2021-11-05 18:21:02.000000 erwin-1.0.2/doc/conf.py
--rw-rw----   0 lamy      (1265) staff       (20)     1404 2021-11-06 11:03:51.000000 erwin-1.0.2/doc/index.rst
--rw-r--r--   0 lamy      (1265) staff       (20)     1142 2021-11-06 10:54:35.000000 erwin-1.0.2/doc/install.rst
--rw-rw----   0 lamy      (1265) staff       (20)      795 2021-11-05 07:29:11.000000 erwin-1.0.2/doc/make.bat
-drwxr-xr-x   0 lamy      (1265) staff       (20)        0 2022-04-13 09:44:19.733291 erwin-1.0.2/doc/methods/
--rw-r--r--   0 lamy      (1265) staff       (20)      110 2021-11-05 18:07:53.000000 erwin-1.0.2/doc/methods/b0_map.rst
--rw-r--r--   0 lamy      (1265) staff       (20)      103 2021-11-05 16:23:55.000000 erwin-1.0.2/doc/methods/b1_map.rst
--rw-r--r--   0 lamy      (1265) staff       (20)      137 2021-11-05 17:43:36.000000 erwin-1.0.2/doc/methods/cbf.rst
--rw-r--r--   0 lamy      (1265) staff       (20)      942 2021-11-05 17:48:18.000000 erwin-1.0.2/doc/methods/diffusion.rst
--rw-r--r--   0 lamy      (1265) staff       (20)      284 2021-11-06 10:59:37.000000 erwin-1.0.2/doc/methods/index.rst
--rw-r--r--   0 lamy      (1265) staff       (20)       99 2021-11-05 18:10:07.000000 erwin-1.0.2/doc/methods/meta_data.rst
--rw-r--r--   0 lamy      (1265) staff       (20)      110 2021-11-05 18:13:05.000000 erwin-1.0.2/doc/methods/misc.rst
--rw-r--r--   0 lamy      (1265) staff       (20)      133 2021-11-05 18:16:36.000000 erwin-1.0.2/doc/methods/moco.rst
--rw-r--r--   0 lamy      (1265) staff       (20)      150 2021-11-05 18:13:41.000000 erwin-1.0.2/doc/methods/mt_map.rst
--rw-r--r--   0 lamy      (1265) staff       (20)      268 2021-11-05 18:15:08.000000 erwin-1.0.2/doc/methods/qsm.rst
--rw-r--r--   0 lamy      (1265) staff       (20)      101 2021-11-05 18:15:34.000000 erwin-1.0.2/doc/methods/segmentation.rst
--rw-r--r--   0 lamy      (1265) staff       (20)      103 2021-11-05 18:17:20.000000 erwin-1.0.2/doc/methods/t1_map.rst
--rw-r--r--   0 lamy      (1265) staff       (20)      140 2021-11-05 18:17:50.000000 erwin-1.0.2/doc/methods/t2_map.rst
--rw-r--r--   0 lamy      (1265) staff       (20)       14 2021-11-06 08:28:53.000000 erwin-1.0.2/doc/requirements.txt
--rw-r--r--   0 lamy      (1265) staff       (20)     3569 2021-11-06 11:02:30.000000 erwin-1.0.2/doc/usage.rst
--rw-r--r--   0 lamy      (1265) staff       (20)       38 2022-04-13 09:44:19.776383 erwin-1.0.2/setup.cfg
--rw-rw----   0 lamy      (1265) staff       (20)     2332 2022-04-13 09:42:28.000000 erwin-1.0.2/setup.py
-drwxr-xr-x   0 lamy      (1265) staff       (20)        0 2022-04-13 09:44:19.713935 erwin-1.0.2/src/
-drwxr-xr-x   0 lamy      (1265) staff       (20)        0 2022-04-13 09:44:19.735122 erwin-1.0.2/src/erwin/
--rw-r--r--   0 lamy      (1265) staff       (20)     2505 2021-11-06 10:10:45.000000 erwin-1.0.2/src/erwin/__init__.py
--rw-rw----   0 lamy      (1265) staff       (20)     3837 2021-11-06 09:02:26.000000 erwin-1.0.2/src/erwin/__main__.py
-drwxr-xr-x   0 lamy      (1265) staff       (20)        0 2022-04-13 09:44:19.738450 erwin-1.0.2/src/erwin/b0_map/
--rw-rw----   0 lamy      (1265) staff       (20)       58 2021-10-25 20:49:41.000000 erwin-1.0.2/src/erwin/b0_map/__init__.py
--rw-r--r--   0 lamy      (1265) staff       (20)     1995 2021-11-05 16:19:49.000000 erwin-1.0.2/src/erwin/b0_map/double_echo.py
-drwxr-xr-x   0 lamy      (1265) staff       (20)        0 2022-04-13 09:44:19.739519 erwin-1.0.2/src/erwin/b1_map/
--rw-rw----   0 lamy      (1265) staff       (20)       43 2021-10-26 14:50:09.000000 erwin-1.0.2/src/erwin/b1_map/__init__.py
--rw-rw----   0 lamy      (1265) staff       (20)     1541 2021-11-05 17:36:34.000000 erwin-1.0.2/src/erwin/b1_map/afi.py
-drwxr-xr-x   0 lamy      (1265) staff       (20)        0 2022-04-13 09:44:19.741212 erwin-1.0.2/src/erwin/cbf/
--rw-rw----   0 lamy      (1265) staff       (20)       94 2021-10-30 16:34:02.000000 erwin-1.0.2/src/erwin/cbf/__init__.py
--rw-rw----   0 lamy      (1265) staff       (20)     2407 2021-11-05 17:44:47.000000 erwin-1.0.2/src/erwin/cbf/asl_bold_to_asl.py
--rw-rw----   0 lamy      (1265) staff       (20)     3794 2021-11-05 17:44:38.000000 erwin-1.0.2/src/erwin/cbf/pasl.py
--rw-r--r--   0 lamy      (1265) staff       (20)     5387 2021-11-06 09:26:32.000000 erwin-1.0.2/src/erwin/cli.py
-drwxr-xr-x   0 lamy      (1265) staff       (20)        0 2022-04-13 09:44:19.752094 erwin-1.0.2/src/erwin/diffusion/
--rw-rw----   0 lamy      (1265) staff       (20)      648 2021-11-06 10:10:13.000000 erwin-1.0.2/src/erwin/diffusion/__init__.py
--rw-r--r--   0 lamy      (1265) staff       (20)      859 2021-11-06 09:26:05.000000 erwin-1.0.2/src/erwin/diffusion/b_zero.py
--rw-r--r--   0 lamy      (1265) staff       (20)     4245 2021-11-05 16:33:00.000000 erwin-1.0.2/src/erwin/diffusion/bruker_to_mif.py
--rw-r--r--   0 lamy      (1265) staff       (20)     1456 2021-11-05 16:34:09.000000 erwin-1.0.2/src/erwin/diffusion/fod_segmentation.py
--rw-rw----   0 lamy      (1265) staff       (20)      584 2021-11-05 16:34:32.000000 erwin-1.0.2/src/erwin/diffusion/mask.py
--rw-rw----   0 lamy      (1265) staff       (20)      662 2021-11-05 16:35:01.000000 erwin-1.0.2/src/erwin/diffusion/mean_response.py
--rw-rw----   0 lamy      (1265) staff       (20)     4158 2021-03-24 07:59:22.000000 erwin-1.0.2/src/erwin/diffusion/mif_io.py
--rw-r--r--   0 lamy      (1265) staff       (20)      912 2021-11-05 16:35:43.000000 erwin-1.0.2/src/erwin/diffusion/multi_tissue_normalization.py
--rw-r--r--   0 lamy      (1265) staff       (20)     5426 2021-11-05 17:48:34.000000 erwin-1.0.2/src/erwin/diffusion/noddi.py
--rw-r--r--   0 lamy      (1265) staff       (20)     2219 2021-11-05 16:36:56.000000 erwin-1.0.2/src/erwin/diffusion/noddi_responses.py
--rw-rw----   0 lamy      (1265) staff       (20)     1926 2021-11-05 16:42:45.000000 erwin-1.0.2/src/erwin/diffusion/preprocessing.py
--rw-rw----   0 lamy      (1265) staff       (20)     4334 2021-11-05 16:43:21.000000 erwin-1.0.2/src/erwin/diffusion/siemens_to_mif.py
--rw-rw----   0 lamy      (1265) staff       (20)     1172 2021-11-05 16:43:58.000000 erwin-1.0.2/src/erwin/diffusion/spherical_deconvolution_response.py
--rw-rw----   0 lamy      (1265) staff       (20)     1235 2021-11-05 16:44:48.000000 erwin-1.0.2/src/erwin/diffusion/spherical_harmonics.py
--rw-rw----   0 lamy      (1265) staff       (20)     1439 2021-11-05 16:48:25.000000 erwin-1.0.2/src/erwin/diffusion/tensor.py
--rw-rw----   0 lamy      (1265) staff       (20)     1206 2021-11-05 16:47:05.000000 erwin-1.0.2/src/erwin/diffusion/tensor_metric.py
-drwxr-xr-x   0 lamy      (1265) staff       (20)        0 2022-04-13 09:44:19.753975 erwin-1.0.2/src/erwin/meta_data/
--rw-r--r--   0 lamy      (1265) staff       (20)       78 2021-11-04 11:40:58.000000 erwin-1.0.2/src/erwin/meta_data/__init__.py
--rw-r--r--   0 lamy      (1265) staff       (20)     3466 2021-11-07 15:30:48.000000 erwin-1.0.2/src/erwin/meta_data/get.py
--rw-r--r--   0 lamy      (1265) staff       (20)     6539 2021-11-04 14:45:33.000000 erwin-1.0.2/src/erwin/meta_data/siemens.py
-drwxr-xr-x   0 lamy      (1265) staff       (20)        0 2022-04-13 09:44:19.755096 erwin-1.0.2/src/erwin/misc/
--rw-rw----   0 lamy      (1265) staff       (20)       68 2021-11-05 17:40:40.000000 erwin-1.0.2/src/erwin/misc/__init__.py
--rw-rw----   0 lamy      (1265) staff       (20)     1134 2021-11-05 16:53:11.000000 erwin-1.0.2/src/erwin/misc/time_to_rate.py
-drwxr-xr-x   0 lamy      (1265) staff       (20)        0 2022-04-13 09:44:19.756820 erwin-1.0.2/src/erwin/moco/
--rw-rw----   0 lamy      (1265) staff       (20)       84 2021-10-30 13:41:14.000000 erwin-1.0.2/src/erwin/moco/__init__.py
--rw-rw----   0 lamy      (1265) staff       (20)     1689 2021-11-05 16:54:22.000000 erwin-1.0.2/src/erwin/moco/ants.py
--rw-rw----   0 lamy      (1265) staff       (20)     3043 2021-11-05 16:54:52.000000 erwin-1.0.2/src/erwin/moco/apply_ants.py
-drwxr-xr-x   0 lamy      (1265) staff       (20)        0 2022-04-13 09:44:19.760524 erwin-1.0.2/src/erwin/mt_map/
--rw-rw----   0 lamy      (1265) staff       (20)       91 2021-10-30 13:42:04.000000 erwin-1.0.2/src/erwin/mt_map/__init__.py
--rw-r--r--   0 lamy      (1265) staff       (20)   142902 2022-01-29 09:22:10.000000 erwin-1.0.2/src/erwin/mt_map/mpf.c
--rw-rw----   0 lamy      (1265) staff       (20)     1685 2021-03-24 07:59:22.000000 erwin-1.0.2/src/erwin/mt_map/mpf.pyx
--rw-rw----   0 lamy      (1265) staff       (20)     1537 2021-11-05 16:55:55.000000 erwin-1.0.2/src/erwin/mt_map/mtr.py
--rw-rw----   0 lamy      (1265) staff       (20)     8745 2021-11-05 16:58:08.000000 erwin-1.0.2/src/erwin/mt_map/single_point.py
-drwxr-xr-x   0 lamy      (1265) staff       (20)        0 2022-04-13 09:44:19.763829 erwin-1.0.2/src/erwin/qsm/
--rw-rw----   0 lamy      (1265) staff       (20)      230 2021-10-30 13:42:18.000000 erwin-1.0.2/src/erwin/qsm/__init__.py
--rw-r--r--   0 lamy      (1265) staff       (20)     1870 2021-11-05 16:59:48.000000 erwin-1.0.2/src/erwin/qsm/background_field_removal.py
--rw-r--r--   0 lamy      (1265) staff       (20)     4267 2021-11-05 17:02:09.000000 erwin-1.0.2/src/erwin/qsm/medi_l1.py
--rw-r--r--   0 lamy      (1265) staff       (20)     1606 2021-11-05 17:03:03.000000 erwin-1.0.2/src/erwin/qsm/r2_star.py
--rw-r--r--   0 lamy      (1265) staff       (20)     4265 2021-11-05 17:03:52.000000 erwin-1.0.2/src/erwin/qsm/total_field.py
--rw-r--r--   0 lamy      (1265) staff       (20)     1499 2021-11-05 17:04:14.000000 erwin-1.0.2/src/erwin/qsm/ventricles_mask.py
-drwxr-xr-x   0 lamy      (1265) staff       (20)        0 2022-04-13 09:44:19.765014 erwin-1.0.2/src/erwin/segmentation/
--rw-rw----   0 lamy      (1265) staff       (20)       49 2021-10-30 13:42:44.000000 erwin-1.0.2/src/erwin/segmentation/__init__.py
--rw-rw----   0 lamy      (1265) staff       (20)     5024 2022-04-13 08:10:41.000000 erwin-1.0.2/src/erwin/segmentation/bet.py
-drwxr-xr-x   0 lamy      (1265) staff       (20)        0 2022-04-13 09:44:19.765944 erwin-1.0.2/src/erwin/t1_map/
--rw-rw----   0 lamy      (1265) staff       (20)       48 2021-10-30 13:52:17.000000 erwin-1.0.2/src/erwin/t1_map/__init__.py
--rw-rw----   0 lamy      (1265) staff       (20)     5859 2021-11-05 17:39:25.000000 erwin-1.0.2/src/erwin/t1_map/vfa.py
-drwxr-xr-x   0 lamy      (1265) staff       (20)        0 2022-04-13 09:44:19.767506 erwin-1.0.2/src/erwin/t2_map/
--rw-rw----   0 lamy      (1265) staff       (20)       77 2021-10-30 13:43:41.000000 erwin-1.0.2/src/erwin/t2_map/__init__.py
--rwxrwx--x   0 lamy      (1265) staff       (20)     3604 2021-11-05 17:13:44.000000 erwin-1.0.2/src/erwin/t2_map/bssfp.py
--rw-rw----   0 lamy      (1265) staff       (20)     3769 2021-11-05 18:21:22.000000 erwin-1.0.2/src/erwin/t2_map/pssfp.py
-drwxr-xr-x   0 lamy      (1265) staff       (20)        0 2022-04-13 09:44:19.737271 erwin-1.0.2/src/erwin.egg-info/
--rw-rw----   0 lamy      (1265) staff       (20)     6360 2022-04-13 09:44:18.000000 erwin-1.0.2/src/erwin.egg-info/PKG-INFO
--rw-rw----   0 lamy      (1265) staff       (20)     2721 2022-04-13 09:44:19.000000 erwin-1.0.2/src/erwin.egg-info/SOURCES.txt
--rw-rw----   0 lamy      (1265) staff       (20)        1 2022-04-13 09:44:18.000000 erwin-1.0.2/src/erwin.egg-info/dependency_links.txt
--rw-rw----   0 lamy      (1265) staff       (20)       46 2022-04-13 09:44:18.000000 erwin-1.0.2/src/erwin.egg-info/entry_points.txt
--rw-rw----   0 lamy      (1265) staff       (20)      102 2022-04-13 09:44:18.000000 erwin-1.0.2/src/erwin.egg-info/requires.txt
--rw-rw----   0 lamy      (1265) staff       (20)        6 2022-04-13 09:44:18.000000 erwin-1.0.2/src/erwin.egg-info/top_level.txt
-drwxr-xr-x   0 lamy      (1265) staff       (20)        0 2022-04-13 09:44:19.767982 erwin-1.0.2/tests/
-drwxr-xr-x   0 lamy      (1265) staff       (20)        0 2022-04-13 09:44:19.769211 erwin-1.0.2/tests/code/
-drwxr-xr-x   0 lamy      (1265) staff       (20)        0 2022-04-13 09:44:19.770581 erwin-1.0.2/tests/code/b0_map/
--rw-r--r--   0 lamy      (1265) staff       (20)        0 2021-11-03 21:12:28.000000 erwin-1.0.2/tests/code/b0_map/__init__.py
--rw-r--r--   0 lamy      (1265) staff       (20)     2188 2021-11-04 11:47:36.000000 erwin-1.0.2/tests/code/b0_map/test_double_echo.py
-drwxr-xr-x   0 lamy      (1265) staff       (20)        0 2022-04-13 09:44:19.772439 erwin-1.0.2/tests/code/diffusion/
--rw-r--r--   0 lamy      (1265) staff       (20)        0 2021-11-06 11:40:44.000000 erwin-1.0.2/tests/code/diffusion/__init__.py
--rw-r--r--   0 lamy      (1265) staff       (20)     1912 2021-11-06 13:38:36.000000 erwin-1.0.2/tests/code/diffusion/test_b_zero.py
--rw-r--r--   0 lamy      (1265) staff       (20)     1038 2021-11-06 12:17:09.000000 erwin-1.0.2/tests/code/diffusion/test_siemens_to_mif.py
-drwxr-xr-x   0 lamy      (1265) staff       (20)        0 2022-04-13 09:44:19.773391 erwin-1.0.2/tests/code/meta_data/
--rw-r--r--   0 lamy      (1265) staff       (20)        0 2021-11-04 14:31:11.000000 erwin-1.0.2/tests/code/meta_data/__init__.py
--rw-r--r--   0 lamy      (1265) staff       (20)     1498 2021-11-06 11:39:15.000000 erwin-1.0.2/tests/code/meta_data/test_get.py
--rw-r--r--   0 lamy      (1265) staff       (20)     3158 2021-11-06 13:38:55.000000 erwin-1.0.2/tests/code/module_and_cli_test_case.py
-drwxr-xr-x   0 lamy      (1265) staff       (20)        0 2022-04-13 09:44:19.774283 erwin-1.0.2/tests/code/t1_map/
--rw-r--r--   0 lamy      (1265) staff       (20)        0 2021-11-03 21:13:34.000000 erwin-1.0.2/tests/code/t1_map/__init__.py
--rw-r--r--   0 lamy      (1265) staff       (20)     2110 2021-11-04 11:45:14.000000 erwin-1.0.2/tests/code/t1_map/test_vfa.py
-drwxr-xr-x   0 lamy      (1265) staff       (20)        0 2022-04-13 09:44:19.775262 erwin-1.0.2/tests/code/t2_map/
--rw-r--r--   0 lamy      (1265) staff       (20)        0 2021-11-03 21:12:49.000000 erwin-1.0.2/tests/code/t2_map/__init__.py
--rw-r--r--   0 lamy      (1265) staff       (20)     2138 2021-11-04 11:53:24.000000 erwin-1.0.2/tests/code/t2_map/test_bssfp.py
--rw-r--r--   0 lamy      (1265) staff       (20)      401 2021-11-06 09:42:55.000000 erwin-1.0.2/tests/code/test_main.py
--rwxrwx--x   0 lamy      (1265) staff       (20)      216 2021-11-06 16:55:51.000000 erwin-1.0.2/tests/download_data
+drwxr-xr-x   0 lamy      (1265) lamy      (1265)        0 2023-08-04 10:39:12.852359 erwin-1.1.0/
+-rw-r--r--   0 lamy      (1265) lamy      (1265)       92 2023-08-04 10:38:19.000000 erwin-1.1.0/.bumpversion.cfg
+-rw-r--r--   0 lamy      (1265) lamy      (1265)      290 2021-11-06 08:55:34.000000 erwin-1.1.0/.readthedocs.yaml
+-rw-r-----   0 lamy      (1265) lamy      (1265)     1508 2021-10-30 16:47:16.000000 erwin-1.1.0/CONTRIBUTING.md
+-rw-rw----   0 lamy      (1265) lamy      (1265)     1092 2021-10-30 16:45:51.000000 erwin-1.1.0/LICENSE
+-rw-r--r--   0 lamy      (1265) lamy      (1265)     6340 2023-08-04 10:39:12.852359 erwin-1.1.0/PKG-INFO
+-rw-rw----   0 lamy      (1265) lamy      (1265)     5290 2021-11-06 11:03:29.000000 erwin-1.1.0/README.md
+drwxr-xr-x   0 lamy      (1265) lamy      (1265)        0 2023-08-04 10:39:12.848359 erwin-1.1.0/doc/
+-rw-rw----   0 lamy      (1265) lamy      (1265)      634 2021-11-05 07:29:11.000000 erwin-1.1.0/doc/Makefile
+-rw-rw----   0 lamy      (1265) lamy      (1265)      777 2021-11-05 18:21:02.000000 erwin-1.1.0/doc/conf.py
+-rw-rw----   0 lamy      (1265) lamy      (1265)     1404 2021-11-06 11:03:51.000000 erwin-1.1.0/doc/index.rst
+-rw-r--r--   0 lamy      (1265) lamy      (1265)     1204 2023-04-30 08:18:11.000000 erwin-1.1.0/doc/install.rst
+-rw-rw----   0 lamy      (1265) lamy      (1265)      795 2021-11-05 07:29:11.000000 erwin-1.1.0/doc/make.bat
+drwxr-xr-x   0 lamy      (1265) lamy      (1265)        0 2023-08-04 10:39:12.848359 erwin-1.1.0/doc/methods/
+-rw-r--r--   0 lamy      (1265) lamy      (1265)      110 2021-11-05 18:07:53.000000 erwin-1.1.0/doc/methods/b0_map.rst
+-rw-r--r--   0 lamy      (1265) lamy      (1265)      103 2021-11-05 16:23:55.000000 erwin-1.1.0/doc/methods/b1_map.rst
+-rw-r--r--   0 lamy      (1265) lamy      (1265)      137 2021-11-05 17:43:36.000000 erwin-1.1.0/doc/methods/cbf.rst
+-rw-r--r--   0 lamy      (1265) lamy      (1265)      942 2021-11-05 17:48:18.000000 erwin-1.1.0/doc/methods/diffusion.rst
+-rw-r--r--   0 lamy      (1265) lamy      (1265)      284 2021-11-06 10:59:37.000000 erwin-1.1.0/doc/methods/index.rst
+-rw-r--r--   0 lamy      (1265) lamy      (1265)       99 2021-11-05 18:10:07.000000 erwin-1.1.0/doc/methods/meta_data.rst
+-rw-r--r--   0 lamy      (1265) lamy      (1265)      110 2021-11-05 18:13:05.000000 erwin-1.1.0/doc/methods/misc.rst
+-rw-r--r--   0 lamy      (1265) lamy      (1265)      133 2021-11-05 18:16:36.000000 erwin-1.1.0/doc/methods/moco.rst
+-rw-r--r--   0 lamy      (1265) lamy      (1265)      150 2021-11-05 18:13:41.000000 erwin-1.1.0/doc/methods/mt_map.rst
+-rw-r--r--   0 lamy      (1265) lamy      (1265)      268 2021-11-05 18:15:08.000000 erwin-1.1.0/doc/methods/qsm.rst
+-rw-r--r--   0 lamy      (1265) lamy      (1265)      101 2021-11-05 18:15:34.000000 erwin-1.1.0/doc/methods/segmentation.rst
+-rw-r--r--   0 lamy      (1265) lamy      (1265)      103 2021-11-05 18:17:20.000000 erwin-1.1.0/doc/methods/t1_map.rst
+-rw-r--r--   0 lamy      (1265) lamy      (1265)      140 2021-11-05 18:17:50.000000 erwin-1.1.0/doc/methods/t2_map.rst
+-rw-r--r--   0 lamy      (1265) lamy      (1265)       14 2021-11-06 08:28:53.000000 erwin-1.1.0/doc/requirements.txt
+-rw-r--r--   0 lamy      (1265) lamy      (1265)     3569 2021-11-06 11:02:30.000000 erwin-1.1.0/doc/usage.rst
+-rw-r--r--   0 lamy      (1265) lamy      (1265)       38 2023-08-04 10:39:12.852359 erwin-1.1.0/setup.cfg
+-rw-r--r--   0 lamy      (1265) lamy      (1265)     2318 2023-08-04 10:38:19.000000 erwin-1.1.0/setup.py
+drwxr-xr-x   0 lamy      (1265) lamy      (1265)        0 2023-08-04 10:39:12.844359 erwin-1.1.0/src/
+drwxr-xr-x   0 lamy      (1265) lamy      (1265)        0 2023-08-04 10:39:12.848359 erwin-1.1.0/src/erwin/
+-rw-r--r--   0 lamy      (1265) lamy      (1265)     4099 2023-07-30 12:26:04.000000 erwin-1.1.0/src/erwin/__init__.py
+-rw-rw----   0 lamy      (1265) lamy      (1265)     3837 2021-11-06 09:02:26.000000 erwin-1.1.0/src/erwin/__main__.py
+drwxr-xr-x   0 lamy      (1265) lamy      (1265)        0 2023-08-04 10:39:12.848359 erwin-1.1.0/src/erwin/b0_map/
+-rw-rw----   0 lamy      (1265) lamy      (1265)       58 2021-10-25 20:49:41.000000 erwin-1.1.0/src/erwin/b0_map/__init__.py
+-rw-r--r--   0 lamy      (1265) lamy      (1265)     2018 2022-05-31 10:23:53.000000 erwin-1.1.0/src/erwin/b0_map/double_echo.py
+drwxr-xr-x   0 lamy      (1265) lamy      (1265)        0 2023-08-04 10:39:12.848359 erwin-1.1.0/src/erwin/b1_map/
+-rw-rw----   0 lamy      (1265) lamy      (1265)       43 2021-10-26 14:50:09.000000 erwin-1.1.0/src/erwin/b1_map/__init__.py
+-rw-rw----   0 lamy      (1265) lamy      (1265)     1576 2022-09-06 09:52:38.000000 erwin-1.1.0/src/erwin/b1_map/afi.py
+drwxr-xr-x   0 lamy      (1265) lamy      (1265)        0 2023-08-04 10:39:12.848359 erwin-1.1.0/src/erwin/cbf/
+-rw-rw----   0 lamy      (1265) lamy      (1265)       94 2021-10-30 16:34:02.000000 erwin-1.1.0/src/erwin/cbf/__init__.py
+-rw-rw----   0 lamy      (1265) lamy      (1265)     2407 2021-11-05 17:44:47.000000 erwin-1.1.0/src/erwin/cbf/asl_bold_to_asl.py
+-rw-rw----   0 lamy      (1265) lamy      (1265)     3794 2021-11-05 17:44:38.000000 erwin-1.1.0/src/erwin/cbf/pasl.py
+-rw-r--r--   0 lamy      (1265) lamy      (1265)     5474 2022-09-05 13:36:16.000000 erwin-1.1.0/src/erwin/cli.py
+drwxr-xr-x   0 lamy      (1265) lamy      (1265)        0 2023-08-04 10:39:12.848359 erwin-1.1.0/src/erwin/diffusion/
+-rw-rw----   0 lamy      (1265) lamy      (1265)      648 2021-11-06 10:10:13.000000 erwin-1.1.0/src/erwin/diffusion/__init__.py
+-rw-r--r--   0 lamy      (1265) lamy      (1265)      859 2023-08-04 10:33:19.000000 erwin-1.1.0/src/erwin/diffusion/b_zero.py
+-rw-r--r--   0 lamy      (1265) lamy      (1265)     4199 2023-07-02 07:03:52.000000 erwin-1.1.0/src/erwin/diffusion/bruker_to_mif.py
+-rw-r--r--   0 lamy      (1265) lamy      (1265)     1456 2021-11-05 16:34:09.000000 erwin-1.1.0/src/erwin/diffusion/fod_segmentation.py
+-rw-rw----   0 lamy      (1265) lamy      (1265)      584 2021-11-05 16:34:32.000000 erwin-1.1.0/src/erwin/diffusion/mask.py
+-rw-rw----   0 lamy      (1265) lamy      (1265)      662 2021-11-05 16:35:01.000000 erwin-1.1.0/src/erwin/diffusion/mean_response.py
+-rw-rw----   0 lamy      (1265) lamy      (1265)     4158 2021-03-24 07:59:22.000000 erwin-1.1.0/src/erwin/diffusion/mif_io.py
+-rw-r--r--   0 lamy      (1265) lamy      (1265)      912 2021-11-05 16:35:43.000000 erwin-1.1.0/src/erwin/diffusion/multi_tissue_normalization.py
+-rw-r--r--   0 lamy      (1265) lamy      (1265)     5503 2022-09-05 13:37:40.000000 erwin-1.1.0/src/erwin/diffusion/noddi.py
+-rw-r--r--   0 lamy      (1265) lamy      (1265)     2266 2022-09-05 13:37:54.000000 erwin-1.1.0/src/erwin/diffusion/noddi_responses.py
+-rw-rw----   0 lamy      (1265) lamy      (1265)     2685 2023-04-30 07:00:14.000000 erwin-1.1.0/src/erwin/diffusion/preprocessing.py
+-rw-rw----   0 lamy      (1265) lamy      (1265)     4334 2021-11-05 16:43:21.000000 erwin-1.1.0/src/erwin/diffusion/siemens_to_mif.py
+-rw-rw----   0 lamy      (1265) lamy      (1265)     1419 2023-08-03 12:44:56.000000 erwin-1.1.0/src/erwin/diffusion/spherical_deconvolution_response.py
+-rw-rw----   0 lamy      (1265) lamy      (1265)     1558 2023-08-03 12:44:49.000000 erwin-1.1.0/src/erwin/diffusion/spherical_harmonics.py
+-rw-rw----   0 lamy      (1265) lamy      (1265)     1439 2021-11-05 16:48:25.000000 erwin-1.1.0/src/erwin/diffusion/tensor.py
+-rw-rw----   0 lamy      (1265) lamy      (1265)     1206 2021-11-05 16:47:05.000000 erwin-1.1.0/src/erwin/diffusion/tensor_metric.py
+drwxr-xr-x   0 lamy      (1265) lamy      (1265)        0 2023-08-04 10:39:12.848359 erwin-1.1.0/src/erwin/meta_data/
+-rw-r--r--   0 lamy      (1265) lamy      (1265)       78 2021-11-04 11:40:58.000000 erwin-1.1.0/src/erwin/meta_data/__init__.py
+-rw-r--r--   0 lamy      (1265) lamy      (1265)     3466 2021-11-07 15:30:48.000000 erwin-1.1.0/src/erwin/meta_data/get.py
+-rw-r--r--   0 lamy      (1265) lamy      (1265)     6539 2021-11-04 14:45:33.000000 erwin-1.1.0/src/erwin/meta_data/siemens.py
+drwxr-xr-x   0 lamy      (1265) lamy      (1265)        0 2023-08-04 10:39:12.848359 erwin-1.1.0/src/erwin/misc/
+-rw-rw----   0 lamy      (1265) lamy      (1265)       68 2021-11-05 17:40:40.000000 erwin-1.1.0/src/erwin/misc/__init__.py
+-rw-rw----   0 lamy      (1265) lamy      (1265)     1134 2021-11-05 16:53:11.000000 erwin-1.1.0/src/erwin/misc/time_to_rate.py
+drwxr-xr-x   0 lamy      (1265) lamy      (1265)        0 2023-08-04 10:39:12.848359 erwin-1.1.0/src/erwin/moco/
+-rw-rw----   0 lamy      (1265) lamy      (1265)       84 2021-10-30 13:41:14.000000 erwin-1.1.0/src/erwin/moco/__init__.py
+-rw-rw----   0 lamy      (1265) lamy      (1265)     1689 2021-11-05 16:54:22.000000 erwin-1.1.0/src/erwin/moco/ants.py
+-rw-rw----   0 lamy      (1265) lamy      (1265)     3043 2021-11-05 16:54:52.000000 erwin-1.1.0/src/erwin/moco/apply_ants.py
+drwxr-xr-x   0 lamy      (1265) lamy      (1265)        0 2023-08-04 10:39:12.848359 erwin-1.1.0/src/erwin/mt_map/
+-rw-rw----   0 lamy      (1265) lamy      (1265)       91 2021-10-30 13:42:04.000000 erwin-1.1.0/src/erwin/mt_map/__init__.py
+-rw-r--r--   0 lamy      (1265) lamy      (1265)   146211 2023-07-02 06:15:59.000000 erwin-1.1.0/src/erwin/mt_map/mpf.c
+-rw-rw----   0 lamy      (1265) lamy      (1265)     1685 2021-03-24 07:59:22.000000 erwin-1.1.0/src/erwin/mt_map/mpf.pyx
+-rw-rw----   0 lamy      (1265) lamy      (1265)     1537 2021-11-05 16:55:55.000000 erwin-1.1.0/src/erwin/mt_map/mtr.py
+-rw-rw----   0 lamy      (1265) lamy      (1265)     8765 2022-05-31 10:45:25.000000 erwin-1.1.0/src/erwin/mt_map/single_point.py
+drwxr-xr-x   0 lamy      (1265) lamy      (1265)        0 2023-08-04 10:39:12.848359 erwin-1.1.0/src/erwin/qsm/
+-rw-rw----   0 lamy      (1265) lamy      (1265)      230 2021-10-30 13:42:18.000000 erwin-1.1.0/src/erwin/qsm/__init__.py
+-rw-r--r--   0 lamy      (1265) lamy      (1265)     1870 2021-11-05 16:59:48.000000 erwin-1.1.0/src/erwin/qsm/background_field_removal.py
+-rw-r--r--   0 lamy      (1265) lamy      (1265)     4267 2021-11-05 17:02:09.000000 erwin-1.1.0/src/erwin/qsm/medi_l1.py
+-rw-r--r--   0 lamy      (1265) lamy      (1265)     1606 2021-11-05 17:03:03.000000 erwin-1.1.0/src/erwin/qsm/r2_star.py
+-rw-r--r--   0 lamy      (1265) lamy      (1265)     4265 2022-06-16 16:42:04.000000 erwin-1.1.0/src/erwin/qsm/total_field.py
+-rw-r--r--   0 lamy      (1265) lamy      (1265)     1499 2021-11-05 17:04:14.000000 erwin-1.1.0/src/erwin/qsm/ventricles_mask.py
+drwxr-xr-x   0 lamy      (1265) lamy      (1265)        0 2023-08-04 10:39:12.848359 erwin-1.1.0/src/erwin/segmentation/
+-rw-rw----   0 lamy      (1265) lamy      (1265)       49 2021-10-30 13:42:44.000000 erwin-1.1.0/src/erwin/segmentation/__init__.py
+-rw-rw----   0 lamy      (1265) lamy      (1265)     5024 2022-04-13 08:10:41.000000 erwin-1.1.0/src/erwin/segmentation/bet.py
+drwxr-xr-x   0 lamy      (1265) lamy      (1265)        0 2023-08-04 10:39:12.848359 erwin-1.1.0/src/erwin/t1_map/
+-rw-rw----   0 lamy      (1265) lamy      (1265)       48 2021-10-30 13:52:17.000000 erwin-1.1.0/src/erwin/t1_map/__init__.py
+-rw-rw----   0 lamy      (1265) lamy      (1265)     5882 2022-05-31 10:25:07.000000 erwin-1.1.0/src/erwin/t1_map/vfa.py
+drwxr-xr-x   0 lamy      (1265) lamy      (1265)        0 2023-08-04 10:39:12.848359 erwin-1.1.0/src/erwin/t2_map/
+-rw-rw----   0 lamy      (1265) lamy      (1265)       77 2021-10-30 13:43:41.000000 erwin-1.1.0/src/erwin/t2_map/__init__.py
+-rwxrwx--x   0 lamy      (1265) lamy      (1265)     3604 2021-11-05 17:13:44.000000 erwin-1.1.0/src/erwin/t2_map/bssfp.py
+-rw-rw----   0 lamy      (1265) lamy      (1265)     3769 2021-11-05 18:21:22.000000 erwin-1.1.0/src/erwin/t2_map/pssfp.py
+drwxr-xr-x   0 lamy      (1265) lamy      (1265)        0 2023-08-04 10:39:12.848359 erwin-1.1.0/src/erwin.egg-info/
+-rw-rw----   0 lamy      (1265) lamy      (1265)     6340 2023-08-04 10:39:12.000000 erwin-1.1.0/src/erwin.egg-info/PKG-INFO
+-rw-rw----   0 lamy      (1265) lamy      (1265)     2721 2023-08-04 10:39:12.000000 erwin-1.1.0/src/erwin.egg-info/SOURCES.txt
+-rw-rw----   0 lamy      (1265) lamy      (1265)        1 2023-08-04 10:39:12.000000 erwin-1.1.0/src/erwin.egg-info/dependency_links.txt
+-rw-rw----   0 lamy      (1265) lamy      (1265)       46 2023-08-04 10:39:12.000000 erwin-1.1.0/src/erwin.egg-info/entry_points.txt
+-rw-rw----   0 lamy      (1265) lamy      (1265)       91 2023-08-04 10:39:12.000000 erwin-1.1.0/src/erwin.egg-info/requires.txt
+-rw-rw----   0 lamy      (1265) lamy      (1265)        6 2023-08-04 10:39:12.000000 erwin-1.1.0/src/erwin.egg-info/top_level.txt
+drwxr-xr-x   0 lamy      (1265) lamy      (1265)        0 2023-08-04 10:39:12.848359 erwin-1.1.0/tests/
+drwxr-xr-x   0 lamy      (1265) lamy      (1265)        0 2023-08-04 10:39:12.848359 erwin-1.1.0/tests/code/
+drwxr-xr-x   0 lamy      (1265) lamy      (1265)        0 2023-08-04 10:39:12.848359 erwin-1.1.0/tests/code/b0_map/
+-rw-r--r--   0 lamy      (1265) lamy      (1265)        0 2021-11-03 21:12:28.000000 erwin-1.1.0/tests/code/b0_map/__init__.py
+-rw-r--r--   0 lamy      (1265) lamy      (1265)     2188 2021-11-04 11:47:36.000000 erwin-1.1.0/tests/code/b0_map/test_double_echo.py
+drwxr-xr-x   0 lamy      (1265) lamy      (1265)        0 2023-08-04 10:39:12.848359 erwin-1.1.0/tests/code/diffusion/
+-rw-r--r--   0 lamy      (1265) lamy      (1265)        0 2021-11-06 11:40:44.000000 erwin-1.1.0/tests/code/diffusion/__init__.py
+-rw-r--r--   0 lamy      (1265) lamy      (1265)     1912 2021-11-06 13:38:36.000000 erwin-1.1.0/tests/code/diffusion/test_b_zero.py
+-rw-r--r--   0 lamy      (1265) lamy      (1265)     1038 2021-11-06 12:17:09.000000 erwin-1.1.0/tests/code/diffusion/test_siemens_to_mif.py
+drwxr-xr-x   0 lamy      (1265) lamy      (1265)        0 2023-08-04 10:39:12.852359 erwin-1.1.0/tests/code/meta_data/
+-rw-r--r--   0 lamy      (1265) lamy      (1265)        0 2021-11-04 14:31:11.000000 erwin-1.1.0/tests/code/meta_data/__init__.py
+-rw-r--r--   0 lamy      (1265) lamy      (1265)     1498 2021-11-06 11:39:15.000000 erwin-1.1.0/tests/code/meta_data/test_get.py
+-rw-r--r--   0 lamy      (1265) lamy      (1265)     3158 2021-11-06 13:38:55.000000 erwin-1.1.0/tests/code/module_and_cli_test_case.py
+drwxr-xr-x   0 lamy      (1265) lamy      (1265)        0 2023-08-04 10:39:12.852359 erwin-1.1.0/tests/code/t1_map/
+-rw-r--r--   0 lamy      (1265) lamy      (1265)        0 2021-11-03 21:13:34.000000 erwin-1.1.0/tests/code/t1_map/__init__.py
+-rw-r--r--   0 lamy      (1265) lamy      (1265)     2110 2021-11-04 11:45:14.000000 erwin-1.1.0/tests/code/t1_map/test_vfa.py
+drwxr-xr-x   0 lamy      (1265) lamy      (1265)        0 2023-08-04 10:39:12.852359 erwin-1.1.0/tests/code/t2_map/
+-rw-r--r--   0 lamy      (1265) lamy      (1265)        0 2021-11-03 21:12:49.000000 erwin-1.1.0/tests/code/t2_map/__init__.py
+-rw-r--r--   0 lamy      (1265) lamy      (1265)     2138 2021-11-04 11:53:24.000000 erwin-1.1.0/tests/code/t2_map/test_bssfp.py
+-rw-r--r--   0 lamy      (1265) lamy      (1265)      401 2021-11-06 09:42:55.000000 erwin-1.1.0/tests/code/test_main.py
+-rwxrwx--x   0 lamy      (1265) lamy      (1265)      216 2021-11-06 16:55:51.000000 erwin-1.1.0/tests/download_data
```

### Comparing `erwin-1.0.2/CONTRIBUTING.md` & `erwin-1.1.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `erwin-1.0.2/LICENSE` & `erwin-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `erwin-1.0.2/PKG-INFO` & `erwin-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: erwin
-Version: 1.0.2
+Version: 1.1.0
 Summary: Toolbox to generate quantitative maps from MRI images
 Home-page: https://github.com/lamyj/erwin
 Author: J. Lamy, M. Mondino, P. Loureiro de Sousa
 Maintainer: Julien Lamy
 Maintainer-email: lamy@unistra.fr
 License: MIT
 Keywords: MRI,quantitative,field mapping,B0,B1,CBF,cerebral blood flow,ASL,arterial spin labeling,pASL,diffusion,DTI,diffusion tensor,spherical harmonics,MT,magnetization transfer,relaxometry,T1,VFA,T2,bSSFP
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Image Processing
@@ -120,9 +119,7 @@
 [Dicomifier]: https://dicomifier.readthedocs.io/
 [doit]: https://pydoit.org/
 [MEDI]: http://pre.weill.cornell.edu/mri/pages/qsm.html
 [MRtrix]: https://www.mrtrix.org/
 [pip]: https://pip.pypa.io/en/stable/
 [PyPi]: https://pypi.org/
 [Spire]: https://github.com/lamyj/spire
-
-
```

### Comparing `erwin-1.0.2/README.md` & `erwin-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `erwin-1.0.2/doc/Makefile` & `erwin-1.1.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `erwin-1.0.2/doc/conf.py` & `erwin-1.1.0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `erwin-1.0.2/doc/index.rst` & `erwin-1.1.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `erwin-1.0.2/doc/install.rst` & `erwin-1.1.0/doc/install.rst`

 * *Files 5% similar despite different names*

```diff
@@ -9,17 +9,19 @@
 - upgrade ``pip`` (``python3 -m pip install --upgrade pip``, especially on Debian ≤ 10 and Ubuntu ≤ 18.04)
 - install `Cython`_ (``apt-get install -y cython3`` on Debian, Ubuntu and other Debian derivatives)
 - install BLAS and LAPACK (``apt-get install -y gfortran libblas-dev liblapack-dev`` on Debian, Ubuntu and other Debian derivatives)
 
 Using the following methods requires additional dependencies:
 
 - Diffusion tensor and spherical harmonics: `MRtrix`_; conversion from Bruker or Siemens DICOM also requires `Dicomifier`_
+- NODDI: `AMICO`_
 - Motion correction: `ANTs`_
 - QSM: `MEDI`_
 
+.. _AMICO: https://github.com/daducci/AMICO
 .. _ANTs: https://github.com/ANTsX/ANTs
 .. _Cython: https://cython.org/
 .. _Dicomifier: https://dicomifier.readthedocs.io/
 .. _MEDI: http://pre.weill.cornell.edu/mri/pages/qsm.html
 .. _MRtrix: https://www.mrtrix.org/
 .. _pip: https://pip.pypa.io/en/stable/
 .. _PyPi: https://pypi.org/
```

### Comparing `erwin-1.0.2/doc/make.bat` & `erwin-1.1.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `erwin-1.0.2/doc/methods/diffusion.rst` & `erwin-1.1.0/doc/methods/diffusion.rst`

 * *Files identical despite different names*

### Comparing `erwin-1.0.2/doc/usage.rst` & `erwin-1.1.0/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `erwin-1.0.2/setup.py` & `erwin-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         
         super().finalize_options()
         self.distribution.ext_modules = Cython.Build.cythonize(
             [mpf_extension], language_level=3)
 
 setuptools.setup(
     name="erwin",
-    version="1.0.2",
+    version="1.1.0",
     
     description="Toolbox to generate quantitative maps from MRI images",
     long_description=long_description,
     long_description_content_type="text/markdown",
     
     url="https://github.com/lamyj/erwin",
     
@@ -66,12 +66,12 @@
     
     python_requires=">=3.7",
     
     setup_requires=["cython"],
     cmdclass={"build": build},
     
     install_requires=[
-        "cython", "dmri-amico", "docutils", "doit", "meg", "nibabel", "numpy",
+        "cython", "docutils", "doit", "meg", "nibabel", "numpy",
         "pydicom", "scipy", "sphinx", "spire-pipeline>=1.1.1", "sycomore"],
     
     entry_points={ "console_scripts": [ "erwin=erwin.__main__:main"] },
 )
```

### Comparing `erwin-1.0.2/src/erwin/__main__.py` & `erwin-1.1.0/src/erwin/__main__.py`

 * *Files identical despite different names*

### Comparing `erwin-1.0.2/src/erwin/b0_map/double_echo.py` & `erwin-1.1.0/src/erwin/b0_map/double_echo.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import nibabel
 import numpy
 import spire
 
-from .. import entrypoint
+from .. import entrypoint, get_path, load
 from ..cli import *
 
 class DoubleEcho(spire.TaskFactory):
     """ ΔB₀ map (in Hz) using the phase difference between two echoes.
         
         Reference: "An in vivo automated shimming method taking into account
         shim current constraints". Wen & Jaffer. Magnetic Resonance in Medicine
@@ -20,24 +20,24 @@
             :param phase: Path to phase images
             :param echo_times: Echo times (s)
             :param target: Path to target ΔB₀ map (Hz)
         """
         
         spire.TaskFactory.__init__(self, str(target))
         
-        self.file_dep = [*magnitude, *phase]
+        self.file_dep = [get_path(x) for x in [*magnitude, *phase]]
         self.targets = [target]
         
         self.actions = [
             (DoubleEcho.b0_map, (magnitude, phase, echo_times, target))]
     
     @staticmethod
     def b0_map(magnitude_paths, phase_paths, echo_times, B0_map_path):
-        magnitude = [nibabel.load(x) for x in magnitude_paths]
-        phase = [nibabel.load(x) for x in phase_paths]
+        magnitude = [load(x) for x in magnitude_paths]
+        phase = [load(x) for x in phase_paths]
         
         # Complex signal for the two echoes
         S = [
             m.get_fdata() * numpy.exp(1j*p.get_fdata())
             for m,p in zip(magnitude, phase)]
         
         # Un-normalized, complex, phase difference
```

### Comparing `erwin-1.0.2/src/erwin/b1_map/afi.py` & `erwin-1.1.0/src/erwin/b1_map/afi.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import nibabel
 import numpy
 import spire
 
-from .. import entrypoint
+from .. import entrypoint, get_path, load
 from ..cli import *
 
 class AFI(spire.TaskFactory):
     """ Relative B1 map from an AFI sequence.
         
         Reference: Actual flip-angle imaging in the pulsed steady state: A 
         method for rapid three-dimensional mapping of the transmitted 
@@ -20,28 +20,28 @@
         """ :param sources: Path to the magnitude images
             :param flip_angle: Flip angle (rad)
             :param tr_ratio: Ratio between the two TR
             :param target: Path to the target relative B1 map
         """
         spire.TaskFactory.__init__(self, str(target))
         
-        self.file_dep = sources
+        self.file_dep = [get_path(x) for x in sources]
         self.targets = [target]
         
         self.actions = [(AFI.b1_map, (sources, flip_angle, tr_ratio, target))]
     
     @staticmethod
     def b1_map(sources_path, flip_angle, tr_ratio, target_path):
-        images = [nibabel.load(x) for x in sources_path]
+        images = [load(x) for x in sources_path]
         data = [x.get_fdata() for x in images]
         
         with numpy.errstate(divide="ignore", invalid="ignore"):
             r = data[1] / data[0]
         n = tr_ratio
         actual_fa = numpy.arccos((r*n - 1)/(n-r))
         
         nibabel.save(
-            nibabel.Nifti1Image(actual_fa/flip_angle, image.affine), 
+            nibabel.Nifti1Image(actual_fa/flip_angle, images[0].affine), 
             target_path)
         
 def main():
     return entrypoint(AFI)
```

### Comparing `erwin-1.0.2/src/erwin/cbf/asl_bold_to_asl.py` & `erwin-1.1.0/src/erwin/cbf/asl_bold_to_asl.py`

 * *Files identical despite different names*

### Comparing `erwin-1.0.2/src/erwin/cbf/pasl.py` & `erwin-1.1.0/src/erwin/cbf/pasl.py`

 * *Files identical despite different names*

### Comparing `erwin-1.0.2/src/erwin/cli.py` & `erwin-1.1.0/src/erwin/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,25 +28,29 @@
         return "foo"
 
 class Flag(object): 
     """ Type hint, equivalent to a boolean, corresponding to a command-line flag
     """
     pass
 
-original_stringify = sphinx.util.typing.stringify
-def stringify(annotation: typing.Any) -> str:
-    if isinstance(annotation, Choice):
-        return "{}[{}]".format(
-            annotation.__class__.__name__,
-            ", ".join(repr(x) for x in annotation.__args__))
-    elif annotation == Flag:
-        return original_stringify(typing.Optional[bool])
-    else:
-        return original_stringify(annotation)
-sphinx.util.typing.stringify = stringify
+try:
+    original_stringify = sphinx.util.typing.stringify
+except AttributeError:
+    pass
+else:
+    def stringify(annotation: typing.Any) -> str:
+        if isinstance(annotation, Choice):
+            return "{}[{}]".format(
+                annotation.__class__.__name__,
+                ", ".join(repr(x) for x in annotation.__args__))
+        elif annotation == Flag:
+            return original_stringify(typing.Optional[bool])
+        else:
+            return original_stringify(annotation)
+    sphinx.util.typing.stringify = stringify
 
 def get_arguments(class_):
     """ Using the class docstring, and the type hints and docstring of the class
         __init__, return a list of (name, options) to pass to 
         ArgumentParser.add_argument
     """
     arguments = []
```

### Comparing `erwin-1.0.2/src/erwin/diffusion/__init__.py` & `erwin-1.1.0/src/erwin/diffusion/__init__.py`

 * *Files identical despite different names*

### Comparing `erwin-1.0.2/src/erwin/diffusion/b_zero.py` & `erwin-1.1.0/src/erwin/diffusion/b_zero.py`

 * *Files identical despite different names*

### Comparing `erwin-1.0.2/src/erwin/diffusion/bruker_to_mif.py` & `erwin-1.1.0/src/erwin/diffusion/bruker_to_mif.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import itertools
 import json
 import os
 import re
 import struct
 import tempfile
 
+import dicomifier
 import nibabel
 import numpy
 import spire
 
 from .. import entrypoint
 from ..cli import *
 
@@ -63,33 +64,32 @@
     
     @staticmethod
     def phase_encoding_scheme(source_path, meta_data_path, scheme_path):
         with open(meta_data_path) as fd:
             meta_data = json.load(fd)
         
         bruker_data = json.loads(
-            base64.b64decode(meta_data["EncapsulatedDocument"][0]))
+            base64.b64decode(meta_data["EncapsulatedDocument"][0]).strip(b" \0"))
         
         # acqp = dicomifier.bruker.Dataset()
         # with tempfile.NamedTemporaryFile("w") as fd:
         #     fd.write(bruker_data["acqp"])
         #     acqp.load(fd.name)
         # # NOTE: ACQ_grad_matrix is "independent of the patient orientation"
         # # (D02_PvParams.pdf, p. D-2-36)
         # gradients = numpy.reshape(acqp["ACQ_grad_matrix"].value, (-1, 3, 3))
         # phase_directions = gradients[:,1]
         
         method = dicomifier.bruker.Dataset()
         with tempfile.NamedTemporaryFile("w") as fd:
             fd.write(bruker_data["method"])
             method.load(fd.name)
-        # NOTE: is this still valid for multi-shot data?
-        # cf. PVM_EpiNShots
+        
         total_readout_time = 1e-3*(
-            (method["PVM_EpiNEchoes"].value[0]-1) 
+            (method["PVM_EpiNEchoes"].value[0]) 
             * method["PVM_EpiEchoSpacing"].value[0])
         
         phase_gradient = numpy.around(
             numpy.reshape(method["PVM_SPackArrGradOrient"].value, (3,3))[1])
         
         entry = numpy.hstack((phase_gradient, [total_readout_time]))
```

### Comparing `erwin-1.0.2/src/erwin/diffusion/fod_segmentation.py` & `erwin-1.1.0/src/erwin/diffusion/fod_segmentation.py`

 * *Files identical despite different names*

### Comparing `erwin-1.0.2/src/erwin/diffusion/mask.py` & `erwin-1.1.0/src/erwin/diffusion/mask.py`

 * *Files identical despite different names*

### Comparing `erwin-1.0.2/src/erwin/diffusion/mean_response.py` & `erwin-1.1.0/src/erwin/diffusion/mean_response.py`

 * *Files identical despite different names*

### Comparing `erwin-1.0.2/src/erwin/diffusion/mif_io.py` & `erwin-1.1.0/src/erwin/diffusion/mif_io.py`

 * *Files identical despite different names*

### Comparing `erwin-1.0.2/src/erwin/diffusion/multi_tissue_normalization.py` & `erwin-1.1.0/src/erwin/diffusion/multi_tissue_normalization.py`

 * *Files identical despite different names*

### Comparing `erwin-1.0.2/src/erwin/diffusion/noddi.py` & `erwin-1.1.0/src/erwin/diffusion/noddi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import gzip
 import os
 
-import amico
 import nibabel
 import numpy
 import spire
 
 from .. import entrypoint
 from ..cli import *
 from . import mif_io
@@ -36,14 +35,16 @@
             :param mask: Path to mask image
             :param shell_width: Width used to group the real b-values in ideal shells (s/mm^2)
             :param b0_threshold: Lower b-value threshold (s/mm^2)
             :param lmax: Maximum order of spherical harmonics
             :param ndirs: Number of directions on the hemisphere
         """
         
+        import amico
+        
         spire.TaskFactory.__init__(self, str(ic_vf))
         
         model = amico.models.NODDI()
         self.file_dep = (
             [dwi, principal_direction]
             + ([mask] if mask else [])
             + [
@@ -59,14 +60,16 @@
     
     @staticmethod
     def noddi(
             dwi_path, response_directory, principal_direction_path,
             ic_vf_path, iso_vf_path, od_path,  
             mask_path=None, shell_width=0, b0_threshold=0, lmax=12, ndirs=32761):
         
+        import amico
+        
         amico.core.setup(lmax, ndirs)
         
         scheme = NODDI.amico_scheme(dwi_path, shell_width, b0_threshold)
         
         # Resample the responses to the actual acquisition scheme
         shells, harmonics = amico.lut.aux_structures_resample(scheme, lmax)
         model = amico.models.NODDI()
@@ -123,14 +126,16 @@
                 path = od_path
             else:
                 print("Skipping {}: unknown map".format(name))
             nibabel.save(map_image, path)
     
     @staticmethod
     def amico_scheme(dwi_path, shell_width=0, b0_threshold=0):
+        import amico
+        
         if str(dwi_path).endswith(".gz"):
             fd = gzip.GzipFile(dwi_path)
         else:
             fd = open(dwi_path, "rb")
         header = mif_io.read_header(fd)
         
         # Amico expects x,y,z (which frame?), b-value (s/mm^2), as MRtrix
```

### Comparing `erwin-1.0.2/src/erwin/diffusion/noddi_responses.py` & `erwin-1.1.0/src/erwin/diffusion/noddi_responses.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import os
 
-import amico
 import spire
 
 from .. import entrypoint
 from ..cli import *
 from .noddi import NODDI
 
 class NODDIResponses(spire.TaskFactory):
@@ -22,14 +21,16 @@
             :param response_directory: Path to target response directory
             :param shell_width: Width used to group the real b-values in ideal shells (s/mm^2)
             :param b0_threshold: Lower b-value threshold (s/mm^2)
             :param lmax: Maximum order of spherical harmonics
             :param ndirs: Number of directions on the hemisphere
         """
         
+        import amico
+        
         spire.TaskFactory.__init__(self, str(response_directory))
         self.file_dep = [dwi]
         
         model = amico.models.NODDI()
         self.targets = [
             os.path.join(response_directory, "A_{:03}.npy".format(1+x))
             for x in range(1+len(model.IC_ODs)*len(model.IC_VFs))]
@@ -41,14 +42,16 @@
         ]
     
     @staticmethod
     def responses(
             dwi, response_directory, 
             shell_width=0, b0_threshold=0, lmax=12, ndirs=32761):
         
+        import amico
+        
         amico.core.setup(lmax, ndirs)
         
         scheme = NODDI.amico_scheme(dwi, shell_width, b0_threshold)
         
         rotation_matrices = amico.lut.load_precomputed_rotation_matrices(
             lmax, ndirs)
         shells, harmonics = amico.lut.aux_structures_generate(scheme, lmax)
```

### Comparing `erwin-1.0.2/src/erwin/diffusion/siemens_to_mif.py` & `erwin-1.1.0/src/erwin/diffusion/siemens_to_mif.py`

 * *Files identical despite different names*

### Comparing `erwin-1.0.2/src/erwin/diffusion/spherical_deconvolution_response.py` & `erwin-1.1.0/src/erwin/diffusion/spherical_deconvolution_response.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,43 @@
+import os
+
 import spire
 
 from .. import entrypoint
 from ..cli import *
 
 class SphericalDeconvolutionResponse(spire.TaskFactory):
     """ Estimation of WM, GM and CSF response functions.
         
-        This wraps "dwi2response dhollander" from MRtrix3.
+        This wraps dwi2response from MRtrix3.
     """
     
-    def __init__(self, source: str, prefix: str, mask: Optional[str]=None):
+    def __init__(
+            self, source: str, target: str, mask: Optional[str]=None,
+            algorithm: Optional[Choice["tournier", "dhollander"]]="dhollander"):
         """ :param source: Path to the source diffusion-weighted image
-            :param prefix: Prefix of the targets response files
+            :param target: Prefix (dhollander) or path (tournier) to the response
             :param mask: Path to the binary mask
+            :param algorithm: Name of the estimation algorithm 
         """
         
-        spire.TaskFactory.__init__(self, prefix+"*.response")
+        spire.TaskFactory.__init__(
+            self, str(
+                "{}wm.response".format(target) if algorithm=="dhollander"
+                else target))
         
         self.file_dep = [source]
         if mask is not None:
             self.file_dep.append(mask)
         
-        self.targets = [
-            "{}{}.response".format(prefix, x) for x in ["wm", "gm", "csf"]]
+        if algorithm == "dhollander":
+            self.targets = [
+                "{}{}.response".format(target, x) for x in ["wm", "gm", "csf"]]
+        else:
+            self.targets = [target]
         
         self.actions = [
-            # DWI-based response estimation
-            # As of Mrtrix 3.0.0, this is the "improved" Dhollander method.
-            ["dwi2response", "dhollander", "-force"]
+            ["dwi2response", algorithm, "-force"]
                 + [source] + (["-mask", mask] if mask else []) + self.targets]
 
 def main():
     return entrypoint(SphericalDeconvolutionResponse)
```

### Comparing `erwin-1.0.2/src/erwin/diffusion/spherical_harmonics.py` & `erwin-1.1.0/src/erwin/diffusion/spherical_harmonics.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,49 @@
 import itertools
+import os
 
 import spire
 
 from .. import entrypoint
 from ..cli import *
 
 class SphericalHarmonics(spire.TaskFactory):
     """ Perform multi-shell multi-tissue CSD.
         
-        This wraps dwi2fod msmt_csd from MRtrix3.
+        This wraps dwi2fod from MRtrix3.
     """
     
     def __init__(
-            self, source: str, global_response: Tuple[str, ...], prefix=str,
-            mask: Optional[str]=None):
+            self, source: str, response: Tuple[str, ...], target=str,
+            mask: Optional[str]=None,
+            algorithm: Optional[Choice["csd", "msmt_csd"]]="msmt_csd"):
         """ :param source: Path to the source diffusion-weighted image
-            :param global_response: Path to the single-fiber response files
-            :param prefix: Prefix of the target harmonics files
+            :param response: Path to the single-fiber response file(s)
+            :param target: Prefix (msmt_csd) or path (csd) to the harmonics files
             :param mask: Path to the binary mask
         """
         
-        spire.TaskFactory.__init__(self, prefix+"*.mif.gz")
+        spire.TaskFactory.__init__(
+            self, str(
+                "{}wm.mif.gz".format(target) if algorithm=="msmt_csd"
+                else target))
         
-        self.file_dep = [source, *global_response]
+        if algorithm == "csd":
+            response = (response, )
+        self.file_dep = [source, *response]
         if mask is not None:
             self.file_dep.append(mask)
         
-        self.targets = [
-            "{}{}.mif.gz".format(prefix, x) for x in ["wm", "gm", "csf"]]
+        if algorithm == "msmt_csd":
+            self.targets = [
+                "{}{}.mif.gz".format(target, x) for x in ["wm", "gm", "csf"]]
+        else:
+            self.targets = [target]
         
         self.actions = [
-            ["dwi2fod", "-force", "msmt_csd", source]
+            ["dwi2fod", "-force", algorithm, source]
                 + (["-mask", mask] if mask else [])
-                + list(itertools.chain(*zip(global_response, self.targets)))
+                + list(itertools.chain(*zip(response, self.targets)))
         ]
 
 def main():
     return entrypoint(SphericalHarmonics)
```

### Comparing `erwin-1.0.2/src/erwin/diffusion/tensor.py` & `erwin-1.1.0/src/erwin/diffusion/tensor.py`

 * *Files identical despite different names*

### Comparing `erwin-1.0.2/src/erwin/diffusion/tensor_metric.py` & `erwin-1.1.0/src/erwin/diffusion/tensor_metric.py`

 * *Files identical despite different names*

### Comparing `erwin-1.0.2/src/erwin/meta_data/get.py` & `erwin-1.1.0/src/erwin/meta_data/get.py`

 * *Files identical despite different names*

### Comparing `erwin-1.0.2/src/erwin/meta_data/siemens.py` & `erwin-1.1.0/src/erwin/meta_data/siemens.py`

 * *Files identical despite different names*

### Comparing `erwin-1.0.2/src/erwin/misc/time_to_rate.py` & `erwin-1.1.0/src/erwin/misc/time_to_rate.py`

 * *Files identical despite different names*

### Comparing `erwin-1.0.2/src/erwin/moco/ants.py` & `erwin-1.1.0/src/erwin/moco/ants.py`

 * *Files identical despite different names*

### Comparing `erwin-1.0.2/src/erwin/moco/apply_ants.py` & `erwin-1.1.0/src/erwin/moco/apply_ants.py`

 * *Files identical despite different names*

### Comparing `erwin-1.0.2/src/erwin/mt_map/mpf.c` & `erwin-1.1.0/src/erwin/mt_map/mpf.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.26 */
+/* Generated by Cython 0.29.32 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "name": "erwin.mt_map.mpf",
         "sources": [
@@ -18,16 +18,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_26"
-#define CYTHON_HEX_VERSION 0x001D1AF0
+#define CYTHON_ABI "0_29_32"
+#define CYTHON_HEX_VERSION 0x001D20F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -58,14 +58,15 @@
 #ifndef Py_HUGE_VAL
   #define Py_HUGE_VAL HUGE_VAL
 #endif
 #ifdef PYPY_VERSION
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
   #define CYTHON_USE_TYPE_SLOTS 0
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #if PY_VERSION_HEX < 0x03050000
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
@@ -94,18 +95,22 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC (PYPY_VERSION_HEX >= 0x07030900)
+  #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #undef CYTHON_USE_ASYNC_SLOTS
   #define CYTHON_USE_ASYNC_SLOTS 0
@@ -135,18 +140,67 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
+#elif defined(PY_NOGIL)
+  #define CYTHON_COMPILING_IN_PYPY 0
+  #define CYTHON_COMPILING_IN_PYSTON 0
+  #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 1
+  #ifndef CYTHON_USE_TYPE_SLOTS
+    #define CYTHON_USE_TYPE_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYTYPE_LOOKUP
+  #define CYTHON_USE_PYTYPE_LOOKUP 0
+  #ifndef CYTHON_USE_ASYNC_SLOTS
+    #define CYTHON_USE_ASYNC_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYLIST_INTERNALS
+  #define CYTHON_USE_PYLIST_INTERNALS 0
+  #ifndef CYTHON_USE_UNICODE_INTERNALS
+    #define CYTHON_USE_UNICODE_INTERNALS 1
+  #endif
+  #undef CYTHON_USE_UNICODE_WRITER
+  #define CYTHON_USE_UNICODE_WRITER 0
+  #undef CYTHON_USE_PYLONG_INTERNALS
+  #define CYTHON_USE_PYLONG_INTERNALS 0
+  #ifndef CYTHON_AVOID_BORROWED_REFS
+    #define CYTHON_AVOID_BORROWED_REFS 0
+  #endif
+  #ifndef CYTHON_ASSUME_SAFE_MACROS
+    #define CYTHON_ASSUME_SAFE_MACROS 1
+  #endif
+  #ifndef CYTHON_UNPACK_METHODS
+    #define CYTHON_UNPACK_METHODS 1
+  #endif
+  #undef CYTHON_FAST_THREAD_STATE
+  #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_PYCALL
+  #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
+  #ifndef CYTHON_USE_TP_FINALIZE
+    #define CYTHON_USE_TP_FINALIZE 1
+  #endif
+  #undef CYTHON_USE_DICT_VERSIONS
+  #define CYTHON_USE_DICT_VERSIONS 0
+  #undef CYTHON_USE_EXC_INFO_STACK
+  #define CYTHON_USE_EXC_INFO_STACK 0
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYTYPE_LOOKUP
     #define CYTHON_USE_PYTYPE_LOOKUP 0
   #elif !defined(CYTHON_USE_PYTYPE_LOOKUP)
@@ -181,32 +235,41 @@
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
-  #ifndef CYTHON_FAST_THREAD_STATE
+  #if PY_VERSION_HEX >= 0x030B00A4
+    #undef CYTHON_FAST_THREAD_STATE
+    #define CYTHON_FAST_THREAD_STATE 0
+  #elif !defined(CYTHON_FAST_THREAD_STATE)
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
   #ifndef CYTHON_FAST_PYCALL
-    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030B00A1)
+    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030A0000)
   #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
     #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
   #endif
-  #ifndef CYTHON_USE_EXC_INFO_STACK
+  #if PY_VERSION_HEX >= 0x030B00A4
+    #undef CYTHON_USE_EXC_INFO_STACK
+    #define CYTHON_USE_EXC_INFO_STACK 0
+  #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if CYTHON_USE_PYLONG_INTERNALS
   #if PY_MAJOR_VERSION < 3
     #include "longintrepr.h"
@@ -650,16 +713,18 @@
     typedef struct {
         unaryfunc am_await;
         unaryfunc am_aiter;
         unaryfunc am_anext;
     } __Pyx_PyAsyncMethodsStruct;
 #endif
 
-#if defined(WIN32) || defined(MS_WINDOWS)
-  #define _USE_MATH_DEFINES
+#if defined(_WIN32) || defined(WIN32) || defined(MS_WINDOWS)
+  #if !defined(_USE_MATH_DEFINES)
+    #define _USE_MATH_DEFINES
+  #endif
 #endif
 #include <math.h>
 #ifdef NAN
 #define __PYX_NAN() ((float) NAN)
 #else
 static CYTHON_INLINE float __PYX_NAN() {
   float value;
@@ -2594,14 +2659,20 @@
     Py_INCREF(code_object);
 }
 
 /* AddTraceback */
 #include "compile.h"
 #include "frameobject.h"
 #include "traceback.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
 static PyCodeObject* __Pyx_CreateCodeObjectForTraceback(
             const char *funcname, int c_line,
             int py_line, const char *filename) {
     PyCodeObject *py_code = NULL;
     PyObject *py_funcname = NULL;
     #if PY_MAJOR_VERSION < 3
     PyObject *py_srcfile = NULL;
@@ -2657,22 +2728,32 @@
     return NULL;
 }
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename) {
     PyCodeObject *py_code = 0;
     PyFrameObject *py_frame = 0;
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
+    PyObject *ptype, *pvalue, *ptraceback;
     if (c_line) {
         c_line = __Pyx_CLineForTraceback(tstate, c_line);
     }
     py_code = __pyx_find_code_object(c_line ? -c_line : py_line);
     if (!py_code) {
+        __Pyx_ErrFetchInState(tstate, &ptype, &pvalue, &ptraceback);
         py_code = __Pyx_CreateCodeObjectForTraceback(
             funcname, c_line, py_line, filename);
-        if (!py_code) goto bad;
+        if (!py_code) {
+            /* If the code object creation fails, then we should clear the
+               fetched exception references and propagate the new exception */
+            Py_XDECREF(ptype);
+            Py_XDECREF(pvalue);
+            Py_XDECREF(ptraceback);
+            goto bad;
+        }
+        __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
         __pyx_insert_code_object(c_line ? -c_line : py_line, py_code);
     }
     py_frame = PyFrame_New(
         tstate,            /*PyThreadState *tstate,*/
         py_code,           /*PyCodeObject *code,*/
         __pyx_d,    /*PyObject *globals,*/
         0                  /*PyObject *locals*/
@@ -3235,19 +3316,41 @@
     }
     return (PyErr_GivenExceptionMatches(err, exc_type1) || PyErr_GivenExceptionMatches(err, exc_type2));
 }
 #endif
 
 /* CheckBinaryVersion */
 static int __Pyx_check_binary_version(void) {
-    char ctversion[4], rtversion[4];
-    PyOS_snprintf(ctversion, 4, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
-    PyOS_snprintf(rtversion, 4, "%s", Py_GetVersion());
-    if (ctversion[0] != rtversion[0] || ctversion[2] != rtversion[2]) {
+    char ctversion[5];
+    int same=1, i, found_dot;
+    const char* rt_from_call = Py_GetVersion();
+    PyOS_snprintf(ctversion, 5, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
+    found_dot = 0;
+    for (i = 0; i < 4; i++) {
+        if (!ctversion[i]) {
+            same = (rt_from_call[i] < '0' || rt_from_call[i] > '9');
+            break;
+        }
+        if (rt_from_call[i] != ctversion[i]) {
+            same = 0;
+            break;
+        }
+    }
+    if (!same) {
+        char rtversion[5] = {'\0'};
         char message[200];
+        for (i=0; i<4; ++i) {
+            if (rt_from_call[i] == '.') {
+                if (found_dot) break;
+                found_dot = 1;
+            } else if (rt_from_call[i] < '0' || rt_from_call[i] > '9') {
+                break;
+            }
+            rtversion[i] = rt_from_call[i];
+        }
         PyOS_snprintf(message, sizeof(message),
                       "compiletime version %s of module '%.100s' "
                       "does not match runtime version %s",
                       ctversion, __Pyx_MODULE_NAME, rtversion);
         return PyErr_WarnEx(NULL, message, 1);
     }
     return 0;
```

### Comparing `erwin-1.0.2/src/erwin/mt_map/mpf.pyx` & `erwin-1.1.0/src/erwin/mt_map/mpf.pyx`

 * *Files identical despite different names*

### Comparing `erwin-1.0.2/src/erwin/mt_map/mtr.py` & `erwin-1.1.0/src/erwin/mt_map/mtr.py`

 * *Files identical despite different names*

### Comparing `erwin-1.0.2/src/erwin/mt_map/single_point.py` & `erwin-1.1.0/src/erwin/mt_map/single_point.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import nibabel
 import numpy
 import scipy.integrate
 import scipy.optimize
 import spire
 
-from .. import entrypoint
+from .. import entrypoint, get_path, load
 from ..cli import *
 
 import pyximport
 pyximport.install()
 from . import mpf
 
 class SinglePoint(spire.TaskFactory):
@@ -43,15 +43,16 @@
         
         spire.TaskFactory.__init__(self, str(MPF_map))
         
         self.B0_map = B0_map
         self.B1_map = B1_map
         self.T1_map = T1_map
         
-        self.file_dep = [MT_off, MT_on, B0_map, B1_map, T1_map]
+        self.file_dep = [
+            get_path(x) for x in [MT_off, MT_on, B0_map, B1_map, T1_map]]
         self.targets = [MPF_map]
         
         self.actions = [
             (
                 SinglePoint.mpf_map, 
                 (
                     MT_off, MT_on,
@@ -64,18 +65,18 @@
             MT_off_path, MT_on_path, 
             mt_flip_angle, mt_duration, mt_frequency_offset, 
             flip_angle, repetition_time,
             B0_map_path, B1_map_path, T1_map_path, 
             MPF_map_path):
         
         # Load the images
-        MT_off, MT_on = [nibabel.load(x) for x in [MT_off_path, MT_on_path]]
-        B0_map = nibabel.load(B0_map_path)
-        B1_map = nibabel.load(B1_map_path)
-        T1_map = nibabel.load(T1_map_path)
+        MT_off, MT_on = [load(x) for x in [MT_off_path, MT_on_path]]
+        B0_map = load(B0_map_path)
+        B1_map = load(B1_map_path)
+        T1_map = load(T1_map_path)
         
         # Derived data
         T1 = T1_map.get_fdata()
         with numpy.errstate(divide="ignore", invalid="ignore"):
             R1 = 1/T1
         T2_free = 0.022*T1
         delta_omega = mt_frequency_offset - B0_map.get_fdata()
```

### Comparing `erwin-1.0.2/src/erwin/qsm/background_field_removal.py` & `erwin-1.1.0/src/erwin/qsm/background_field_removal.py`

 * *Files identical despite different names*

### Comparing `erwin-1.0.2/src/erwin/qsm/medi_l1.py` & `erwin-1.1.0/src/erwin/qsm/medi_l1.py`

 * *Files identical despite different names*

### Comparing `erwin-1.0.2/src/erwin/qsm/r2_star.py` & `erwin-1.1.0/src/erwin/qsm/r2_star.py`

 * *Files identical despite different names*

### Comparing `erwin-1.0.2/src/erwin/qsm/total_field.py` & `erwin-1.1.0/src/erwin/qsm/total_field.py`

 * *Files identical despite different names*

### Comparing `erwin-1.0.2/src/erwin/qsm/ventricles_mask.py` & `erwin-1.1.0/src/erwin/qsm/ventricles_mask.py`

 * *Files identical despite different names*

### Comparing `erwin-1.0.2/src/erwin/segmentation/bet.py` & `erwin-1.1.0/src/erwin/segmentation/bet.py`

 * *Files identical despite different names*

### Comparing `erwin-1.0.2/src/erwin/t1_map/vfa.py` & `erwin-1.1.0/src/erwin/t1_map/vfa.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import nibabel
 import numpy
 import spire
 import sycomore
 from sycomore.units import *
 
-from .. import entrypoint
+from .. import entrypoint, get_path, load
 from ..cli import *
 
 class VFA(spire.TaskFactory):
     """ Compute the T1 map based on SPGR images acquired with a VFA scheme.
         
         Reference: T1 Mapping Using Spoiled FLASH-EPI Hybrid Sequences and 
         Varying Flip Angles. Preibisch & Deichmann. Magnetic Resonance in 
@@ -24,33 +24,33 @@
             :param repetition_time: Repetition time (s)
             :param B1_map: Path to relative B₁ map
             :param target: Path to target T₁ map (s)
         """
         
         spire.TaskFactory.__init__(self, str(target))
         
-        self.file_dep = [*sources, B1_map]
+        self.file_dep = [get_path(x) for x in [*sources, B1_map]]
         self.targets = [target]
         
         self.actions = [
             (VFA.t1_map, (
                 sources, flip_angles, echo_time, repetition_time, B1_map,
                 target))]
     
     def t1_map(
             source_paths, flip_angles, echo_time, repetition_time, B1_map_path,
             T1_map_path):
         """T1 map generation"""
         
         # Load the VFA signal
-        sources = [nibabel.load(x) for x in source_paths]
+        sources = [load(x) for x in source_paths]
         signal = numpy.asarray([x.get_fdata() for x in sources])
         
         # Compute a flip angle map from the nominal flip angles
-        B1_map = nibabel.load(B1_map_path).get_fdata()
+        B1_map = load(B1_map_path).get_fdata()
         flip_angle_map = numpy.asarray([B1_map * x for x in flip_angles])
         
         # Compute the B1-corrected T1 map
         with numpy.errstate(divide="ignore", invalid="ignore"):
             X = signal / numpy.tan(flip_angle_map)
             Y = signal / numpy.sin(flip_angle_map)
             # Eq. 3b
```

### Comparing `erwin-1.0.2/src/erwin/t2_map/bssfp.py` & `erwin-1.1.0/src/erwin/t2_map/bssfp.py`

 * *Files identical despite different names*

### Comparing `erwin-1.0.2/src/erwin/t2_map/pssfp.py` & `erwin-1.1.0/src/erwin/t2_map/pssfp.py`

 * *Files identical despite different names*

### Comparing `erwin-1.0.2/src/erwin.egg-info/PKG-INFO` & `erwin-1.1.0/src/erwin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: erwin
-Version: 1.0.2
+Version: 1.1.0
 Summary: Toolbox to generate quantitative maps from MRI images
 Home-page: https://github.com/lamyj/erwin
 Author: J. Lamy, M. Mondino, P. Loureiro de Sousa
 Maintainer: Julien Lamy
 Maintainer-email: lamy@unistra.fr
 License: MIT
 Keywords: MRI,quantitative,field mapping,B0,B1,CBF,cerebral blood flow,ASL,arterial spin labeling,pASL,diffusion,DTI,diffusion tensor,spherical harmonics,MT,magnetization transfer,relaxometry,T1,VFA,T2,bSSFP
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Image Processing
@@ -120,9 +119,7 @@
 [Dicomifier]: https://dicomifier.readthedocs.io/
 [doit]: https://pydoit.org/
 [MEDI]: http://pre.weill.cornell.edu/mri/pages/qsm.html
 [MRtrix]: https://www.mrtrix.org/
 [pip]: https://pip.pypa.io/en/stable/
 [PyPi]: https://pypi.org/
 [Spire]: https://github.com/lamyj/spire
-
-
```

### Comparing `erwin-1.0.2/src/erwin.egg-info/SOURCES.txt` & `erwin-1.1.0/src/erwin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `erwin-1.0.2/tests/code/b0_map/test_double_echo.py` & `erwin-1.1.0/tests/code/b0_map/test_double_echo.py`

 * *Files identical despite different names*

### Comparing `erwin-1.0.2/tests/code/diffusion/test_b_zero.py` & `erwin-1.1.0/tests/code/diffusion/test_b_zero.py`

 * *Files identical despite different names*

### Comparing `erwin-1.0.2/tests/code/diffusion/test_siemens_to_mif.py` & `erwin-1.1.0/tests/code/diffusion/test_siemens_to_mif.py`

 * *Files identical despite different names*

### Comparing `erwin-1.0.2/tests/code/meta_data/test_get.py` & `erwin-1.1.0/tests/code/meta_data/test_get.py`

 * *Files identical despite different names*

### Comparing `erwin-1.0.2/tests/code/module_and_cli_test_case.py` & `erwin-1.1.0/tests/code/module_and_cli_test_case.py`

 * *Files identical despite different names*

### Comparing `erwin-1.0.2/tests/code/t1_map/test_vfa.py` & `erwin-1.1.0/tests/code/t1_map/test_vfa.py`

 * *Files identical despite different names*

### Comparing `erwin-1.0.2/tests/code/t2_map/test_bssfp.py` & `erwin-1.1.0/tests/code/t2_map/test_bssfp.py`

 * *Files identical despite different names*

