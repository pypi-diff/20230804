# Comparing `tmp/fusionlab-0.1.5.tar.gz` & `tmp/fusionlab-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fusionlab-0.1.5.tar", last modified: Fri Jul 14 03:52:39 2023, max compression
+gzip compressed data, was "fusionlab-0.1.6.tar", last modified: Fri Aug  4 08:27:27 2023, max compression
```

## Comparing `fusionlab-0.1.5.tar` & `fusionlab-0.1.6.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-14 03:52:39.859478 fusionlab-0.1.5/
--rw-r--r--   0 cyli       (502) staff       (20)     1060 2022-12-31 04:40:09.000000 fusionlab-0.1.5/LICENSE
--rw-r--r--   0 cyli       (502) staff       (20)     3730 2023-07-14 03:52:39.859354 fusionlab-0.1.5/PKG-INFO
--rw-r--r--   0 cyli       (502) staff       (20)     3267 2023-07-08 09:17:08.000000 fusionlab-0.1.5/README.md
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-14 03:52:39.844439 fusionlab-0.1.5/fusionlab/
--rw-r--r--   0 cyli       (502) staff       (20)      993 2023-06-02 08:43:17.000000 fusionlab-0.1.5/fusionlab/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)       63 2023-07-14 03:50:01.000000 fusionlab-0.1.5/fusionlab/__version__.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-14 03:52:39.846464 fusionlab-0.1.5/fusionlab/classification/
--rw-r--r--   0 cyli       (502) staff       (20)      387 2023-07-01 03:49:33.000000 fusionlab-0.1.5/fusionlab/classification/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     3353 2023-07-01 03:49:33.000000 fusionlab-0.1.5/fusionlab/classification/base.py
--rw-r--r--   0 cyli       (502) staff       (20)      711 2023-07-01 03:49:33.000000 fusionlab-0.1.5/fusionlab/classification/lstm.py
--rw-r--r--   0 cyli       (502) staff       (20)     1473 2023-07-01 03:49:33.000000 fusionlab-0.1.5/fusionlab/classification/vgg.py
--rw-r--r--   0 cyli       (502) staff       (20)       32 2023-06-02 08:43:17.000000 fusionlab-0.1.5/fusionlab/configs.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-14 03:52:39.847878 fusionlab-0.1.5/fusionlab/datasets/
--rw-r--r--   0 cyli       (502) staff       (20)      558 2023-07-01 03:49:44.000000 fusionlab-0.1.5/fusionlab/datasets/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     1181 2023-05-20 16:17:41.000000 fusionlab-0.1.5/fusionlab/datasets/a12lead.py
--rw-r--r--   0 cyli       (502) staff       (20)     5456 2023-06-02 08:43:17.000000 fusionlab-0.1.5/fusionlab/datasets/cinc2017.py
--rw-r--r--   0 cyli       (502) staff       (20)      325 2023-06-02 08:43:17.000000 fusionlab-0.1.5/fusionlab/datasets/csvread.py
--rw-r--r--   0 cyli       (502) staff       (20)    13273 2023-07-01 03:49:33.000000 fusionlab-0.1.5/fusionlab/datasets/ludb.py
--rw-r--r--   0 cyli       (502) staff       (20)    12053 2023-05-20 16:17:41.000000 fusionlab-0.1.5/fusionlab/datasets/muse.py
--rw-r--r--   0 cyli       (502) staff       (20)     4586 2023-07-01 03:49:44.000000 fusionlab-0.1.5/fusionlab/datasets/utils.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-14 03:52:39.848113 fusionlab-0.1.5/fusionlab/encoders/
--rw-r--r--   0 cyli       (502) staff       (20)      906 2023-07-08 09:17:08.000000 fusionlab-0.1.5/fusionlab/encoders/__init__.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-14 03:52:39.848607 fusionlab-0.1.5/fusionlab/encoders/alexnet/
--rw-r--r--   0 cyli       (502) staff       (20)        0 2023-05-20 16:17:41.000000 fusionlab-0.1.5/fusionlab/encoders/alexnet/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     1751 2023-07-01 03:49:33.000000 fusionlab-0.1.5/fusionlab/encoders/alexnet/alexnet.py
--rw-r--r--   0 cyli       (502) staff       (20)     1186 2022-12-31 04:40:09.000000 fusionlab-0.1.5/fusionlab/encoders/alexnet/tfalexnet.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-14 03:52:39.848914 fusionlab-0.1.5/fusionlab/encoders/convnext/
--rw-r--r--   0 cyli       (502) staff       (20)        0 2023-07-08 09:17:08.000000 fusionlab-0.1.5/fusionlab/encoders/convnext/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     8194 2023-07-08 09:17:08.000000 fusionlab-0.1.5/fusionlab/encoders/convnext/convnext.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-14 03:52:39.849256 fusionlab-0.1.5/fusionlab/encoders/efficientnet/
--rw-r--r--   0 cyli       (502) staff       (20)        0 2023-07-08 09:17:08.000000 fusionlab-0.1.5/fusionlab/encoders/efficientnet/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)    12573 2023-07-08 09:19:15.000000 fusionlab-0.1.5/fusionlab/encoders/efficientnet/efficientnet.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-14 03:52:39.849865 fusionlab-0.1.5/fusionlab/encoders/inceptionv1/
--rw-r--r--   0 cyli       (502) staff       (20)        0 2023-05-20 16:17:41.000000 fusionlab-0.1.5/fusionlab/encoders/inceptionv1/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     3650 2023-07-01 03:49:33.000000 fusionlab-0.1.5/fusionlab/encoders/inceptionv1/inceptionv1.py
--rw-r--r--   0 cyli       (502) staff       (20)     3029 2023-01-03 10:19:18.000000 fusionlab-0.1.5/fusionlab/encoders/inceptionv1/tfinceptionv1.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-14 03:52:39.850516 fusionlab-0.1.5/fusionlab/encoders/resnetv1/
--rw-r--r--   0 cyli       (502) staff       (20)        0 2023-05-20 16:17:41.000000 fusionlab-0.1.5/fusionlab/encoders/resnetv1/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     4838 2023-07-01 03:49:33.000000 fusionlab-0.1.5/fusionlab/encoders/resnetv1/resnetv1.py
--rw-r--r--   0 cyli       (502) staff       (20)     4183 2023-01-05 10:15:54.000000 fusionlab-0.1.5/fusionlab/encoders/resnetv1/tfresnetv1.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-14 03:52:39.851205 fusionlab-0.1.5/fusionlab/encoders/vgg/
--rw-r--r--   0 cyli       (502) staff       (20)        0 2023-05-20 16:17:41.000000 fusionlab-0.1.5/fusionlab/encoders/vgg/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     4206 2022-12-31 04:40:09.000000 fusionlab-0.1.5/fusionlab/encoders/vgg/tfvgg.py
--rw-r--r--   0 cyli       (502) staff       (20)     4753 2023-07-01 03:49:33.000000 fusionlab-0.1.5/fusionlab/encoders/vgg/vgg.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-14 03:52:39.852383 fusionlab-0.1.5/fusionlab/functional/
--rw-r--r--   0 cyli       (502) staff       (20)      347 2023-05-20 16:17:41.000000 fusionlab-0.1.5/fusionlab/functional/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)      420 2023-05-20 16:17:41.000000 fusionlab-0.1.5/fusionlab/functional/dice.py
--rw-r--r--   0 cyli       (502) staff       (20)      486 2023-05-20 16:17:41.000000 fusionlab-0.1.5/fusionlab/functional/iou.py
--rw-r--r--   0 cyli       (502) staff       (20)      661 2023-05-20 16:17:41.000000 fusionlab-0.1.5/fusionlab/functional/tfdice.py
--rw-r--r--   0 cyli       (502) staff       (20)      718 2023-05-20 16:17:41.000000 fusionlab-0.1.5/fusionlab/functional/tfiou.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-14 03:52:39.852927 fusionlab-0.1.5/fusionlab/layers/
--rw-r--r--   0 cyli       (502) staff       (20)      289 2023-07-08 09:17:08.000000 fusionlab-0.1.5/fusionlab/layers/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     3599 2023-07-14 03:24:02.000000 fusionlab-0.1.5/fusionlab/layers/base.py
--rw-r--r--   0 cyli       (502) staff       (20)    17832 2023-07-08 09:17:08.000000 fusionlab-0.1.5/fusionlab/layers/factories.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-14 03:52:39.853623 fusionlab-0.1.5/fusionlab/layers/squeeze_excitation/
--rw-r--r--   0 cyli       (502) staff       (20)        0 2023-07-07 10:44:19.000000 fusionlab-0.1.5/fusionlab/layers/squeeze_excitation/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     2187 2023-07-08 09:17:08.000000 fusionlab-0.1.5/fusionlab/layers/squeeze_excitation/se.py
--rw-r--r--   0 cyli       (502) staff       (20)      748 2023-01-05 10:57:39.000000 fusionlab-0.1.5/fusionlab/layers/squeeze_excitation/tfse.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-14 03:52:39.853878 fusionlab-0.1.5/fusionlab/losses/
--rw-r--r--   0 cyli       (502) staff       (20)      405 2023-05-20 16:17:41.000000 fusionlab-0.1.5/fusionlab/losses/__init__.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-14 03:52:39.854330 fusionlab-0.1.5/fusionlab/losses/diceloss/
--rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-31 09:07:31.000000 fusionlab-0.1.5/fusionlab/losses/diceloss/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     3650 2023-01-31 09:07:31.000000 fusionlab-0.1.5/fusionlab/losses/diceloss/dice.py
--rw-r--r--   0 cyli       (502) staff       (20)     4142 2023-05-21 07:24:23.000000 fusionlab-0.1.5/fusionlab/losses/diceloss/tfdice.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-14 03:52:39.854881 fusionlab-0.1.5/fusionlab/losses/iouloss/
--rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-31 09:07:31.000000 fusionlab-0.1.5/fusionlab/losses/iouloss/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     2773 2023-01-31 09:07:31.000000 fusionlab-0.1.5/fusionlab/losses/iouloss/iou.py
--rw-r--r--   0 cyli       (502) staff       (20)     3102 2023-05-21 07:24:23.000000 fusionlab-0.1.5/fusionlab/losses/iouloss/tfiou.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-14 03:52:39.855500 fusionlab-0.1.5/fusionlab/losses/tversky/
--rw-r--r--   0 cyli       (502) staff       (20)        0 2023-04-13 01:08:31.000000 fusionlab-0.1.5/fusionlab/losses/tversky/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     4440 2023-04-13 01:08:31.000000 fusionlab-0.1.5/fusionlab/losses/tversky/tftversky.py
--rw-r--r--   0 cyli       (502) staff       (20)     3897 2023-04-13 01:08:31.000000 fusionlab-0.1.5/fusionlab/losses/tversky/tversky.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-14 03:52:39.855739 fusionlab-0.1.5/fusionlab/metrics/
--rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-31 09:07:31.000000 fusionlab-0.1.5/fusionlab/metrics/__init__.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-14 03:52:39.856330 fusionlab-0.1.5/fusionlab/segmentation/
--rw-r--r--   0 cyli       (502) staff       (20)      420 2023-07-01 03:49:33.000000 fusionlab-0.1.5/fusionlab/segmentation/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     1770 2023-07-01 03:49:33.000000 fusionlab-0.1.5/fusionlab/segmentation/base.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-14 03:52:39.856730 fusionlab-0.1.5/fusionlab/segmentation/resunet/
--rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-14 03:30:01.000000 fusionlab-0.1.5/fusionlab/segmentation/resunet/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     5271 2023-07-01 03:49:33.000000 fusionlab-0.1.5/fusionlab/segmentation/resunet/resunet.py
--rw-r--r--   0 cyli       (502) staff       (20)     4476 2023-05-20 16:17:41.000000 fusionlab-0.1.5/fusionlab/segmentation/resunet/tfresunet.py
--rw-r--r--   0 cyli       (502) staff       (20)      683 2023-05-20 16:17:41.000000 fusionlab-0.1.5/fusionlab/segmentation/tfbase.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-14 03:52:39.857104 fusionlab-0.1.5/fusionlab/segmentation/unet/
--rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-07 18:27:01.000000 fusionlab-0.1.5/fusionlab/segmentation/unet/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     4168 2023-05-20 16:17:41.000000 fusionlab-0.1.5/fusionlab/segmentation/unet/tfunet.py
--rw-r--r--   0 cyli       (502) staff       (20)     5414 2023-07-01 03:49:33.000000 fusionlab-0.1.5/fusionlab/segmentation/unet/unet.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-14 03:52:39.857443 fusionlab-0.1.5/fusionlab/segmentation/unet2plus/
--rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-12 08:11:48.000000 fusionlab-0.1.5/fusionlab/segmentation/unet2plus/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     4622 2023-05-20 16:17:41.000000 fusionlab-0.1.5/fusionlab/segmentation/unet2plus/tfunet2plus.py
--rw-r--r--   0 cyli       (502) staff       (20)     5662 2023-07-01 03:49:33.000000 fusionlab-0.1.5/fusionlab/segmentation/unet2plus/unet2plus.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-14 03:52:39.858153 fusionlab-0.1.5/fusionlab/trainers/
--rw-r--r--   0 cyli       (502) staff       (20)      224 2023-05-20 16:17:41.000000 fusionlab-0.1.5/fusionlab/trainers/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     6521 2023-06-02 08:43:17.000000 fusionlab-0.1.5/fusionlab/trainers/dcgan.py
--rw-r--r--   0 cyli       (502) staff       (20)       72 2023-05-20 16:17:48.000000 fusionlab-0.1.5/fusionlab/trainers/test.py
--rw-r--r--   0 cyli       (502) staff       (20)     4784 2023-06-02 08:43:17.000000 fusionlab-0.1.5/fusionlab/trainers/trainer.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-14 03:52:39.859069 fusionlab-0.1.5/fusionlab/utils/
--rw-r--r--   0 cyli       (502) staff       (20)      106 2023-07-14 03:23:23.000000 fusionlab-0.1.5/fusionlab/utils/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)      789 2023-07-14 03:23:06.000000 fusionlab-0.1.5/fusionlab/utils/basic.py
--rw-r--r--   0 cyli       (502) staff       (20)      406 2023-07-01 03:49:44.000000 fusionlab-0.1.5/fusionlab/utils/plots.py
--rw-r--r--   0 cyli       (502) staff       (20)      825 2023-06-02 08:43:17.000000 fusionlab-0.1.5/fusionlab/utils/trace.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-14 03:52:39.845280 fusionlab-0.1.5/fusionlab.egg-info/
--rw-r--r--   0 cyli       (502) staff       (20)     3730 2023-07-14 03:52:39.000000 fusionlab-0.1.5/fusionlab.egg-info/PKG-INFO
--rw-r--r--   0 cyli       (502) staff       (20)     2723 2023-07-14 03:52:39.000000 fusionlab-0.1.5/fusionlab.egg-info/SOURCES.txt
--rw-r--r--   0 cyli       (502) staff       (20)        1 2023-07-14 03:52:39.000000 fusionlab-0.1.5/fusionlab.egg-info/dependency_links.txt
--rw-r--r--   0 cyli       (502) staff       (20)      177 2023-07-14 03:52:39.000000 fusionlab-0.1.5/fusionlab.egg-info/requires.txt
--rw-r--r--   0 cyli       (502) staff       (20)       10 2023-07-14 03:52:39.000000 fusionlab-0.1.5/fusionlab.egg-info/top_level.txt
--rw-r--r--   0 cyli       (502) staff       (20)       38 2023-07-14 03:52:39.859518 fusionlab-0.1.5/setup.cfg
--rw-r--r--   0 cyli       (502) staff       (20)     3989 2023-05-21 07:24:23.000000 fusionlab-0.1.5/setup.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-08-04 08:27:27.757124 fusionlab-0.1.6/
+-rw-r--r--   0 cyli       (502) staff       (20)     1060 2022-12-31 04:40:09.000000 fusionlab-0.1.6/LICENSE
+-rw-r--r--   0 cyli       (502) staff       (20)     3948 2023-08-04 08:27:27.756999 fusionlab-0.1.6/PKG-INFO
+-rw-r--r--   0 cyli       (502) staff       (20)     3485 2023-08-04 08:25:22.000000 fusionlab-0.1.6/README.md
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-08-04 08:27:27.737030 fusionlab-0.1.6/fusionlab/
+-rw-r--r--   0 cyli       (502) staff       (20)      720 2023-08-04 08:24:07.000000 fusionlab-0.1.6/fusionlab/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)       63 2023-08-04 08:26:04.000000 fusionlab-0.1.6/fusionlab/__version__.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-08-04 08:27:27.738562 fusionlab-0.1.6/fusionlab/classification/
+-rw-r--r--   0 cyli       (502) staff       (20)      278 2023-08-04 08:24:07.000000 fusionlab-0.1.6/fusionlab/classification/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     3353 2023-07-01 03:49:33.000000 fusionlab-0.1.6/fusionlab/classification/base.py
+-rw-r--r--   0 cyli       (502) staff       (20)      711 2023-07-01 03:49:33.000000 fusionlab-0.1.6/fusionlab/classification/lstm.py
+-rw-r--r--   0 cyli       (502) staff       (20)     1473 2023-07-01 03:49:33.000000 fusionlab-0.1.6/fusionlab/classification/vgg.py
+-rw-r--r--   0 cyli       (502) staff       (20)       21 2023-08-04 08:24:07.000000 fusionlab-0.1.6/fusionlab/configs.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-08-04 08:27:27.741781 fusionlab-0.1.6/fusionlab/datasets/
+-rw-r--r--   0 cyli       (502) staff       (20)      455 2023-08-04 08:24:07.000000 fusionlab-0.1.6/fusionlab/datasets/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     1181 2023-05-20 16:17:41.000000 fusionlab-0.1.6/fusionlab/datasets/a12lead.py
+-rw-r--r--   0 cyli       (502) staff       (20)     5456 2023-06-02 08:43:17.000000 fusionlab-0.1.6/fusionlab/datasets/cinc2017.py
+-rw-r--r--   0 cyli       (502) staff       (20)      325 2023-06-02 08:43:17.000000 fusionlab-0.1.6/fusionlab/datasets/csvread.py
+-rw-r--r--   0 cyli       (502) staff       (20)    13273 2023-07-01 03:49:33.000000 fusionlab-0.1.6/fusionlab/datasets/ludb.py
+-rw-r--r--   0 cyli       (502) staff       (20)    12053 2023-05-20 16:17:41.000000 fusionlab-0.1.6/fusionlab/datasets/muse.py
+-rw-r--r--   0 cyli       (502) staff       (20)     5492 2023-08-04 08:24:07.000000 fusionlab-0.1.6/fusionlab/datasets/utils.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-08-04 08:27:27.742097 fusionlab-0.1.6/fusionlab/encoders/
+-rw-r--r--   0 cyli       (502) staff       (20)      879 2023-08-04 08:24:07.000000 fusionlab-0.1.6/fusionlab/encoders/__init__.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-08-04 08:27:27.743034 fusionlab-0.1.6/fusionlab/encoders/alexnet/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-05-20 16:17:41.000000 fusionlab-0.1.6/fusionlab/encoders/alexnet/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     1751 2023-07-01 03:49:33.000000 fusionlab-0.1.6/fusionlab/encoders/alexnet/alexnet.py
+-rw-r--r--   0 cyli       (502) staff       (20)     1186 2022-12-31 04:40:09.000000 fusionlab-0.1.6/fusionlab/encoders/alexnet/tfalexnet.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-08-04 08:27:27.743509 fusionlab-0.1.6/fusionlab/encoders/convnext/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-07-08 09:17:08.000000 fusionlab-0.1.6/fusionlab/encoders/convnext/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     8194 2023-08-04 08:24:07.000000 fusionlab-0.1.6/fusionlab/encoders/convnext/convnext.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-08-04 08:27:27.743903 fusionlab-0.1.6/fusionlab/encoders/efficientnet/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-07-08 09:17:08.000000 fusionlab-0.1.6/fusionlab/encoders/efficientnet/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)    12542 2023-08-04 08:24:07.000000 fusionlab-0.1.6/fusionlab/encoders/efficientnet/efficientnet.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-08-04 08:27:27.744641 fusionlab-0.1.6/fusionlab/encoders/inceptionv1/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-05-20 16:17:41.000000 fusionlab-0.1.6/fusionlab/encoders/inceptionv1/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     3650 2023-07-01 03:49:33.000000 fusionlab-0.1.6/fusionlab/encoders/inceptionv1/inceptionv1.py
+-rw-r--r--   0 cyli       (502) staff       (20)     3029 2023-01-03 10:19:18.000000 fusionlab-0.1.6/fusionlab/encoders/inceptionv1/tfinceptionv1.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-08-04 08:27:27.745505 fusionlab-0.1.6/fusionlab/encoders/resnetv1/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-05-20 16:17:41.000000 fusionlab-0.1.6/fusionlab/encoders/resnetv1/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)    11811 2023-08-04 08:24:07.000000 fusionlab-0.1.6/fusionlab/encoders/resnetv1/resnetv1.py
+-rw-r--r--   0 cyli       (502) staff       (20)     4183 2023-01-05 10:15:54.000000 fusionlab-0.1.6/fusionlab/encoders/resnetv1/tfresnetv1.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-08-04 08:27:27.747716 fusionlab-0.1.6/fusionlab/encoders/vgg/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-05-20 16:17:41.000000 fusionlab-0.1.6/fusionlab/encoders/vgg/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     4206 2022-12-31 04:40:09.000000 fusionlab-0.1.6/fusionlab/encoders/vgg/tfvgg.py
+-rw-r--r--   0 cyli       (502) staff       (20)     4753 2023-07-01 03:49:33.000000 fusionlab-0.1.6/fusionlab/encoders/vgg/vgg.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-08-04 08:27:27.749397 fusionlab-0.1.6/fusionlab/functional/
+-rw-r--r--   0 cyli       (502) staff       (20)      289 2023-08-04 08:24:07.000000 fusionlab-0.1.6/fusionlab/functional/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)      420 2023-05-20 16:17:41.000000 fusionlab-0.1.6/fusionlab/functional/dice.py
+-rw-r--r--   0 cyli       (502) staff       (20)      486 2023-05-20 16:17:41.000000 fusionlab-0.1.6/fusionlab/functional/iou.py
+-rw-r--r--   0 cyli       (502) staff       (20)      661 2023-05-20 16:17:41.000000 fusionlab-0.1.6/fusionlab/functional/tfdice.py
+-rw-r--r--   0 cyli       (502) staff       (20)      718 2023-05-20 16:17:41.000000 fusionlab-0.1.6/fusionlab/functional/tfiou.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-08-04 08:27:27.749946 fusionlab-0.1.6/fusionlab/layers/
+-rw-r--r--   0 cyli       (502) staff       (20)      231 2023-08-04 08:24:07.000000 fusionlab-0.1.6/fusionlab/layers/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     3599 2023-07-14 05:09:36.000000 fusionlab-0.1.6/fusionlab/layers/base.py
+-rw-r--r--   0 cyli       (502) staff       (20)    18028 2023-08-04 08:24:07.000000 fusionlab-0.1.6/fusionlab/layers/factories.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-08-04 08:27:27.750907 fusionlab-0.1.6/fusionlab/layers/squeeze_excitation/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-07-07 10:44:19.000000 fusionlab-0.1.6/fusionlab/layers/squeeze_excitation/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     2187 2023-07-08 09:17:08.000000 fusionlab-0.1.6/fusionlab/layers/squeeze_excitation/se.py
+-rw-r--r--   0 cyli       (502) staff       (20)      748 2023-01-05 10:57:39.000000 fusionlab-0.1.6/fusionlab/layers/squeeze_excitation/tfse.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-08-04 08:27:27.751130 fusionlab-0.1.6/fusionlab/losses/
+-rw-r--r--   0 cyli       (502) staff       (20)      346 2023-08-04 08:24:07.000000 fusionlab-0.1.6/fusionlab/losses/__init__.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-08-04 08:27:27.751571 fusionlab-0.1.6/fusionlab/losses/diceloss/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-31 09:07:31.000000 fusionlab-0.1.6/fusionlab/losses/diceloss/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     3650 2023-01-31 09:07:31.000000 fusionlab-0.1.6/fusionlab/losses/diceloss/dice.py
+-rw-r--r--   0 cyli       (502) staff       (20)     4142 2023-05-21 07:24:23.000000 fusionlab-0.1.6/fusionlab/losses/diceloss/tfdice.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-08-04 08:27:27.752100 fusionlab-0.1.6/fusionlab/losses/iouloss/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-31 09:07:31.000000 fusionlab-0.1.6/fusionlab/losses/iouloss/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     2773 2023-01-31 09:07:31.000000 fusionlab-0.1.6/fusionlab/losses/iouloss/iou.py
+-rw-r--r--   0 cyli       (502) staff       (20)     3102 2023-05-21 07:24:23.000000 fusionlab-0.1.6/fusionlab/losses/iouloss/tfiou.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-08-04 08:27:27.752636 fusionlab-0.1.6/fusionlab/losses/tversky/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-04-13 01:08:31.000000 fusionlab-0.1.6/fusionlab/losses/tversky/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     4440 2023-04-13 01:08:31.000000 fusionlab-0.1.6/fusionlab/losses/tversky/tftversky.py
+-rw-r--r--   0 cyli       (502) staff       (20)     3897 2023-04-13 01:08:31.000000 fusionlab-0.1.6/fusionlab/losses/tversky/tversky.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-08-04 08:27:27.752862 fusionlab-0.1.6/fusionlab/metrics/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-31 09:07:31.000000 fusionlab-0.1.6/fusionlab/metrics/__init__.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-08-04 08:27:27.753373 fusionlab-0.1.6/fusionlab/segmentation/
+-rw-r--r--   0 cyli       (502) staff       (20)      362 2023-08-04 08:24:07.000000 fusionlab-0.1.6/fusionlab/segmentation/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     1770 2023-07-01 03:49:33.000000 fusionlab-0.1.6/fusionlab/segmentation/base.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-08-04 08:27:27.753892 fusionlab-0.1.6/fusionlab/segmentation/resunet/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-14 03:30:01.000000 fusionlab-0.1.6/fusionlab/segmentation/resunet/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     5271 2023-07-01 03:49:33.000000 fusionlab-0.1.6/fusionlab/segmentation/resunet/resunet.py
+-rw-r--r--   0 cyli       (502) staff       (20)     4476 2023-05-20 16:17:41.000000 fusionlab-0.1.6/fusionlab/segmentation/resunet/tfresunet.py
+-rw-r--r--   0 cyli       (502) staff       (20)      683 2023-05-20 16:17:41.000000 fusionlab-0.1.6/fusionlab/segmentation/tfbase.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-08-04 08:27:27.754289 fusionlab-0.1.6/fusionlab/segmentation/unet/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-07 18:27:01.000000 fusionlab-0.1.6/fusionlab/segmentation/unet/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     4168 2023-05-20 16:17:41.000000 fusionlab-0.1.6/fusionlab/segmentation/unet/tfunet.py
+-rw-r--r--   0 cyli       (502) staff       (20)     5414 2023-07-01 03:49:33.000000 fusionlab-0.1.6/fusionlab/segmentation/unet/unet.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-08-04 08:27:27.754653 fusionlab-0.1.6/fusionlab/segmentation/unet2plus/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-12 08:11:48.000000 fusionlab-0.1.6/fusionlab/segmentation/unet2plus/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     4622 2023-05-20 16:17:41.000000 fusionlab-0.1.6/fusionlab/segmentation/unet2plus/tfunet2plus.py
+-rw-r--r--   0 cyli       (502) staff       (20)     5662 2023-07-01 03:49:33.000000 fusionlab-0.1.6/fusionlab/segmentation/unet2plus/unet2plus.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-08-04 08:27:27.755531 fusionlab-0.1.6/fusionlab/trainers/
+-rw-r--r--   0 cyli       (502) staff       (20)      102 2023-08-04 08:24:07.000000 fusionlab-0.1.6/fusionlab/trainers/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     6521 2023-06-02 08:43:17.000000 fusionlab-0.1.6/fusionlab/trainers/dcgan.py
+-rw-r--r--   0 cyli       (502) staff       (20)       72 2023-05-20 16:17:48.000000 fusionlab-0.1.6/fusionlab/trainers/test.py
+-rw-r--r--   0 cyli       (502) staff       (20)     4784 2023-06-02 08:43:17.000000 fusionlab-0.1.6/fusionlab/trainers/trainer.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-08-04 08:27:27.756688 fusionlab-0.1.6/fusionlab/utils/
+-rw-r--r--   0 cyli       (502) staff       (20)      106 2023-07-14 05:09:36.000000 fusionlab-0.1.6/fusionlab/utils/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)      789 2023-07-14 05:09:36.000000 fusionlab-0.1.6/fusionlab/utils/basic.py
+-rw-r--r--   0 cyli       (502) staff       (20)      406 2023-07-01 03:49:44.000000 fusionlab-0.1.6/fusionlab/utils/plots.py
+-rw-r--r--   0 cyli       (502) staff       (20)      825 2023-06-02 08:43:17.000000 fusionlab-0.1.6/fusionlab/utils/trace.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-08-04 08:27:27.737705 fusionlab-0.1.6/fusionlab.egg-info/
+-rw-r--r--   0 cyli       (502) staff       (20)     3948 2023-08-04 08:27:27.000000 fusionlab-0.1.6/fusionlab.egg-info/PKG-INFO
+-rw-r--r--   0 cyli       (502) staff       (20)     2723 2023-08-04 08:27:27.000000 fusionlab-0.1.6/fusionlab.egg-info/SOURCES.txt
+-rw-r--r--   0 cyli       (502) staff       (20)        1 2023-08-04 08:27:27.000000 fusionlab-0.1.6/fusionlab.egg-info/dependency_links.txt
+-rw-r--r--   0 cyli       (502) staff       (20)      177 2023-08-04 08:27:27.000000 fusionlab-0.1.6/fusionlab.egg-info/requires.txt
+-rw-r--r--   0 cyli       (502) staff       (20)       10 2023-08-04 08:27:27.000000 fusionlab-0.1.6/fusionlab.egg-info/top_level.txt
+-rw-r--r--   0 cyli       (502) staff       (20)       38 2023-08-04 08:27:27.757166 fusionlab-0.1.6/setup.cfg
+-rw-r--r--   0 cyli       (502) staff       (20)     3989 2023-05-21 07:24:23.000000 fusionlab-0.1.6/setup.py
```

### Comparing `fusionlab-0.1.5/LICENSE` & `fusionlab-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.5/PKG-INFO` & `fusionlab-0.1.6/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusionlab
-Version: 0.1.5
+Version: 0.1.6
 Summary: Useful packages for DL
 Home-page: https://github.com/taipingeric/fusionlab
 Author: Chih-Yang Li
 Author-email: taipingeric@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -21,26 +21,28 @@
     <br>
     <img src="assets/imgs/fusionlab_banner.png" width="400"/>
     <br>
 <p>
 
 [![PyPI version](https://badge.fury.io/py/fusionlab.svg)](https://badge.fury.io/py/fusionlab) ![Test](https://github.com/taipingeric/fusionlab/actions/workflows/python-app.yml/badge.svg)  [![Downloads](https://static.pepy.tech/badge/fusionlab)](https://pepy.tech/project/fusionlab)
 
+[![Documentation](https://img.shields.io/badge/view-Documentation-blue?style=for-the-badge)](https://fusionlab.readthedocs.io/)
+
 FusionLab is an open-source frameworks built for Deep Learning research written in PyTorch and Tensorflow. The code is easy to read and modify 
 especially for newbie. Feel free to send pull requests :D
 
-* [What's New](#News)
-* [Installation](#Installation)
-* [How to use](#How-to-use)
-* [Encoders](#Encoders)
-* [Losses](#Losses)
-* [Segmentation](#Segmentation)
+* [What's New](#news)
+* [Installation](#installation)
+* [How to use](#how-to-use)
+* [Encoders](#encoders)
+* [Losses](#losses)
+* [Segmentation](#segmentation)
 * [1D, 2D, 3D Model](#n-dimensional-model)
-* [Acknowledgements](#Acknowledgements)
-
+* [Acknowledgements](#acknowledgements)
+      
 ## Installation
 
 ### With pip
 
 ```bash
 pip install fusionlab
 ```
@@ -56,14 +58,18 @@
 # PyTorch
 encoder = fl.encoders.VGG16()
 # Tensorflow
 encoder = fl.encoders.TFVGG16()
 
 ```
 
+## Documentation
+
+[Doc](https://fusionlab.readthedocs.io/en/latest/encoders.html)
+
 ## Encoders
 
 [encoder list](fusionlab/encoders/README.md)
 
 ## Losses
 
 [Loss func list](fusionlab/losses/README.md)
```

### Comparing `fusionlab-0.1.5/README.md` & `fusionlab-0.1.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -4,26 +4,28 @@
     <br>
     <img src="assets/imgs/fusionlab_banner.png" width="400"/>
     <br>
 <p>
 
 [![PyPI version](https://badge.fury.io/py/fusionlab.svg)](https://badge.fury.io/py/fusionlab) ![Test](https://github.com/taipingeric/fusionlab/actions/workflows/python-app.yml/badge.svg)  [![Downloads](https://static.pepy.tech/badge/fusionlab)](https://pepy.tech/project/fusionlab)
 
+[![Documentation](https://img.shields.io/badge/view-Documentation-blue?style=for-the-badge)](https://fusionlab.readthedocs.io/)
+
 FusionLab is an open-source frameworks built for Deep Learning research written in PyTorch and Tensorflow. The code is easy to read and modify 
 especially for newbie. Feel free to send pull requests :D
 
-* [What's New](#News)
-* [Installation](#Installation)
-* [How to use](#How-to-use)
-* [Encoders](#Encoders)
-* [Losses](#Losses)
-* [Segmentation](#Segmentation)
+* [What's New](#news)
+* [Installation](#installation)
+* [How to use](#how-to-use)
+* [Encoders](#encoders)
+* [Losses](#losses)
+* [Segmentation](#segmentation)
 * [1D, 2D, 3D Model](#n-dimensional-model)
-* [Acknowledgements](#Acknowledgements)
-
+* [Acknowledgements](#acknowledgements)
+      
 ## Installation
 
 ### With pip
 
 ```bash
 pip install fusionlab
 ```
@@ -39,14 +41,18 @@
 # PyTorch
 encoder = fl.encoders.VGG16()
 # Tensorflow
 encoder = fl.encoders.TFVGG16()
 
 ```
 
+## Documentation
+
+[Doc](https://fusionlab.readthedocs.io/en/latest/encoders.html)
+
 ## Encoders
 
 [encoder list](fusionlab/encoders/README.md)
 
 ## Losses
 
 [Loss func list](fusionlab/losses/README.md)
```

### Comparing `fusionlab-0.1.5/fusionlab/classification/base.py` & `fusionlab-0.1.6/fusionlab/classification/base.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.5/fusionlab/classification/lstm.py` & `fusionlab-0.1.6/fusionlab/classification/lstm.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.5/fusionlab/classification/vgg.py` & `fusionlab-0.1.6/fusionlab/classification/vgg.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.5/fusionlab/datasets/a12lead.py` & `fusionlab-0.1.6/fusionlab/datasets/a12lead.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.5/fusionlab/datasets/cinc2017.py` & `fusionlab-0.1.6/fusionlab/datasets/cinc2017.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.5/fusionlab/datasets/ludb.py` & `fusionlab-0.1.6/fusionlab/datasets/ludb.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.5/fusionlab/datasets/muse.py` & `fusionlab-0.1.6/fusionlab/datasets/muse.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.5/fusionlab/datasets/utils.py` & `fusionlab-0.1.6/fusionlab/datasets/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -106,7 +106,39 @@
         mask = torch.from_numpy(mask).long()
         return signals, mask
     
     def preprocess(self, signals):
         # normalization by channel
         signals = (signals - signals.mean(axis=0)) / signals.std(axis=0)
         return signals
+
+# TODO: add test
+def count_parameters(
+        model: torch.nn.Module, 
+        trainable_only: bool = False
+    ) -> int:
+    """
+    Returns the number of parameters in a model
+
+    Args:
+        model: a pytorch model
+        trainable_only: if True, only count trainable parameters
+
+    Returns:
+        num_parameters: number of parameters in the model
+
+    Reference: https://discuss.pytorch.org/t/how-do-i-check-the-number-of-parameters-of-a-model/4325/9
+    """
+    if trainable_only:
+        return sum(p.numel() for p in model.parameters() if p.requires_grad)
+    else:
+        return sum(p.numel() for p in model.parameters())
+
+
+if __name__ == '__main__':
+    import torch.nn as nn
+    layer = nn.Linear(10, 10)
+    
+    for p in layer.parameters():
+        p.requires_grad = False
+    print(count_parameters(layer, trainable_only=False))
+    print(count_parameters(layer, trainable_only=True))
```

### Comparing `fusionlab-0.1.5/fusionlab/encoders/__init__.py` & `fusionlab-0.1.6/fusionlab/encoders/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from fusionlab.configs import BACKEND
-if BACKEND == 'torch':
+from fusionlab import BACKEND
+if BACKEND['torch']:
     from .alexnet.alexnet import AlexNet
     from .vgg.vgg import VGG16, VGG19
     from .inceptionv1.inceptionv1 import InceptionNetV1
-    from .resnetv1.resnetv1 import ResNet50V1
+    from .resnetv1.resnetv1 import *
     from .efficientnet.efficientnet import (
+        EfficientNet,
         EfficientNetB0, 
         EfficientNetB1,
         EfficientNetB2,
         EfficientNetB3,
         EfficientNetB4,
         EfficientNetB5,
         EfficientNetB6,
         EfficientNetB7
     )
     from .convnext.convnext import (
+        ConvNeXt,
         ConvNeXtTiny,
         ConvNeXtSmall,
         ConvNeXtBase,
         ConvNeXtLarge,
         ConvNeXtXLarge
     )
-elif BACKEND == 'tf':
+if BACKEND['tf']:
     from .alexnet.tfalexnet import TFAlexNet
     from .vgg.tfvgg import TFVGG16, TFVGG19
     from .inceptionv1.tfinceptionv1 import TFInceptionNetV1
     from .resnetv1.tfresnetv1 import TFResNet50V1
-else:
-    print('backend not supported!!!')
```

### Comparing `fusionlab-0.1.5/fusionlab/encoders/alexnet/alexnet.py` & `fusionlab-0.1.6/fusionlab/encoders/alexnet/alexnet.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.5/fusionlab/encoders/alexnet/tfalexnet.py` & `fusionlab-0.1.6/fusionlab/encoders/alexnet/tfalexnet.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.5/fusionlab/encoders/convnext/convnext.py` & `fusionlab-0.1.6/fusionlab/encoders/convnext/convnext.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,43 +135,43 @@
             x = F.layer_norm(x, self.normalized_shape, self.weight, self.bias, self.eps)
             x = rearrange(x, 'N ... C -> N C ...')
             return x
         elif self.data_format == "channels_last":
             return F.layer_norm(x, self.normalized_shape, self.weight, self.bias, self.eps)
 
 class ConvNeXtTiny(ConvNeXt):
-    def __init__(self, spatial_dims=2, cin=3):
+    def __init__(self, cin=3, spatial_dims=2):
         super().__init__(depths=[3, 3, 9, 3], 
                          dims=[96, 192, 384, 768],
                          in_chans=cin,
                          spatial_dims=spatial_dims)
 
 class ConvNeXtSmall(ConvNeXt):
-    def __init__(self, spatial_dims=2, cin=3):
+    def __init__(self, cin=3, spatial_dims=2):
         super().__init__(depths=[3, 3, 27, 3], 
                          dims=[96, 192, 384, 768],
                          in_chans=cin,
                          spatial_dims=spatial_dims)
 
 class ConvNeXtBase(ConvNeXt):
-    def __init__(self, spatial_dims=2, cin=3):
+    def __init__(self, cin=3, spatial_dims=2):
         super().__init__(depths=[3, 3, 27, 3], 
                          dims=[128, 256, 512, 1024],
                          in_chans=cin,
                          spatial_dims=spatial_dims)
         
 class ConvNeXtLarge(ConvNeXt):
-    def __init__(self, spatial_dims=2, cin=3):
+    def __init__(self, cin=3, spatial_dims=2):
         super().__init__(depths=[3, 3, 27, 3], 
                          dims=[192, 384, 768, 1536],
                          in_chans=cin,
                          spatial_dims=spatial_dims)
         
 class ConvNeXtXLarge(ConvNeXt):
-    def __init__(self, spatial_dims=2, cin=3):
+    def __init__(self, cin=3, spatial_dims=2):
         super().__init__(depths=[3, 3, 27, 3], 
                          dims=[256, 512, 1024, 2048],
                          in_chans=cin,
                          spatial_dims=spatial_dims)
 
 
 if __name__ == '__main__':
```

### Comparing `fusionlab-0.1.5/fusionlab/encoders/efficientnet/efficientnet.py` & `fusionlab-0.1.6/fusionlab/encoders/efficientnet/efficientnet.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,14 @@
         stride: int,
         input_channels: int,
         out_channels: int,
         num_layers: int,
         width_mult: float = 1.0,
         depth_mult: float = 1.0,
         block: Optional[Callable[..., nn.Module]] = None,
-        spatial_dims: int = 2,
     ) -> None:
         input_channels = self.adjust_channels(input_channels, width_mult)
         out_channels = self.adjust_channels(out_channels, width_mult)
         num_layers = self.adjust_depth(num_layers, depth_mult)
         if block is None:
             block = MBConv
         super().__init__(expand_ratio, kernel, stride, input_channels, out_channels, num_layers, block)
@@ -262,99 +261,99 @@
         mb_cfg(6, 3, 2, 40, 80, 3),
         mb_cfg(6, 5, 1, 80, 112, 3),
         mb_cfg(6, 5, 2, 112, 192, 4),
         mb_cfg(6, 3, 1, 192, 320, 1),
     ]
 
 class EfficientNetB0(EfficientNet):
-    def __init__(self, spatial_dims=2, cin=3):
+    def __init__(self, cin=3, spatial_dims=2):
         config = _build_efficient_cfg(1.0, 1.0)
         last_channel = None
         super().__init__(
             inverted_residual_setting=config, 
             cin=cin,
             stochastic_depth_prob=0.2, 
             last_channel=last_channel, 
             spatial_dims=spatial_dims
         )
 
 class EfficientNetB1(EfficientNet):
-    def __init__(self, spatial_dims=2, cin=3):
+    def __init__(self, cin=3, spatial_dims=2):
         config = _build_efficient_cfg(1.0, 1.1)
         last_channel = None
         super().__init__(
             inverted_residual_setting=config, 
             cin=cin,
             stochastic_depth_prob=0.2, 
             last_channel=last_channel, 
             spatial_dims=spatial_dims
         )
 
 class EfficientNetB2(EfficientNet):
-    def __init__(self, spatial_dims=2, cin=3):
+    def __init__(self, cin=3, spatial_dims=2):
         config = _build_efficient_cfg(1.1, 1.2)
         last_channel = None
         super().__init__(
             inverted_residual_setting=config, 
             cin=cin,
             stochastic_depth_prob=0.3, 
             last_channel=last_channel, 
             spatial_dims=spatial_dims
         )
 
 class EfficientNetB3(EfficientNet):
-    def __init__(self, spatial_dims=2, cin=3):
+    def __init__(self, cin=3, spatial_dims=2):
         config = _build_efficient_cfg(1.2, 1.4)
         last_channel = None
         super().__init__(
             inverted_residual_setting=config, 
             cin=cin,
             stochastic_depth_prob=0.3, 
             last_channel=last_channel, 
             spatial_dims=spatial_dims
         )
 
 class EfficientNetB4(EfficientNet):
-    def __init__(self, spatial_dims=2, cin=3):
+    def __init__(self, cin=3, spatial_dims=2):
         config = _build_efficient_cfg(1.4, 1.8)
         last_channel = None
         super().__init__(
             inverted_residual_setting=config, 
             cin=cin,
             stochastic_depth_prob=0.4, 
             last_channel=last_channel, 
             spatial_dims=spatial_dims
         )
 
 class EfficientNetB5(EfficientNet):
-    def __init__(self, spatial_dims=2, cin=3):
+    def __init__(self, cin=3, spatial_dims=2):
         config = _build_efficient_cfg(1.6, 2.2)
         last_channel = None
         super().__init__(
             inverted_residual_setting=config, 
             cin=cin,
             stochastic_depth_prob=0.4, 
             last_channel=last_channel, 
             spatial_dims=spatial_dims
         )
 
 class EfficientNetB6(EfficientNet):
-    def __init__(self, spatial_dims=2, cin=3):
+    def __init__(self, cin=3, spatial_dims=2):
         config = _build_efficient_cfg(1.8, 2.6)
         last_channel = None
         super().__init__(
             inverted_residual_setting=config, 
             cin=cin,
             stochastic_depth_prob=0.5, 
             last_channel=last_channel, 
             spatial_dims=spatial_dims
         )
 
 class EfficientNetB7(EfficientNet):
-    def __init__(self, spatial_dims=2, cin=3):
+    def __init__(self, cin=3, spatial_dims=2):
         config = _build_efficient_cfg(2.0, 3.1)
         last_channel = None
         super().__init__(
             inverted_residual_setting=config, 
             cin=cin,
             stochastic_depth_prob=0.5, 
             last_channel=last_channel,
```

### Comparing `fusionlab-0.1.5/fusionlab/encoders/inceptionv1/inceptionv1.py` & `fusionlab-0.1.6/fusionlab/encoders/inceptionv1/inceptionv1.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.5/fusionlab/encoders/inceptionv1/tfinceptionv1.py` & `fusionlab-0.1.6/fusionlab/encoders/inceptionv1/tfinceptionv1.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.5/fusionlab/encoders/resnetv1/resnetv1.py` & `fusionlab-0.1.6/fusionlab/encoders/resnetv1/tfresnetv1.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,140 +1,130 @@
-import torch
-import torch.nn as nn
-from fusionlab.layers.factories import ConvND, MaxPool, BatchNorm
-
-from fusionlab.utils import autopad
+import tensorflow as tf
+from tensorflow.keras import Model, Sequential, layers
 
 # ResNet50
 # Ref:
 # https://github.com/keras-team/keras-applications/blob/master/keras_applications/resnet50.py
+# https://github.com/raghakot/keras-resnet/blob/master/README.md
+
+
+class Identity(layers.Layer):
+    def __init__(self):
+        super(Identity, self).__init__()
+
+    def call(self, inputs, training=None):
+        return inputs
 
-class ConvBlock(nn.Module):
-    def __init__(self, cin, cout, kernel_size=3, spatial_dims=2, stride=1, activation=True, padding=True):
+
+class ConvBlock(Model):
+    def __init__(self, cout, kernel_size=3, stride=1, activation=True, padding=True):
         super().__init__()
-        self.conv = ConvND(spatial_dims, cin, cout, kernel_size, stride, autopad(kernel_size))
-        self.bn = BatchNorm(spatial_dims, cout)
-        self.act = nn.ReLU(inplace=True) if activation else nn.Identity()
-
-    def forward(self, x):
-        x = self.conv(x)
-        x = self.bn(x)
+        self.conv = layers.Conv2D(cout, kernel_size, stride,
+                                  padding='same' if padding else 'valid')
+        self.bn = layers.BatchNormalization()
+        self.act = layers.ReLU() if activation else Identity()
+
+    def call(self, inputs, training=None):
+        x = self.conv(inputs)
+        x = self.bn(x, training)
         x = self.act(x)
         return x
 
 
-class Bottleneck(nn.Module):
-    def __init__(self, cin, dims, kernel_size=3, spatial_dims=2, stride=None):
+class Bottleneck(Model):
+    def __init__(self, dims, kernel_size=3, stride=None):
         super().__init__()
-        dim1, dim2 = dims
-        self.conv1 = ConvBlock(cin, dim1, 1, spatial_dims)
-        self.conv2 = ConvBlock(dim1, dim1, kernel_size, spatial_dims,
+        dim1, dim2, dim3 = dims
+        self.conv1 = ConvBlock(dim1, kernel_size=1)
+        self.conv2 = ConvBlock(dim2, kernel_size=kernel_size,
                                stride=stride if stride else 1)
-        self.conv3 = ConvBlock(dim1, dim2, 1, spatial_dims, activation=False)
-        self.act = nn.ReLU(inplace=True)
-        self.skip = nn.Identity() if not stride else ConvBlock(cin, dim2, 
-                                                               1,
-                                                               spatial_dims,
-                                                               stride=stride,
-                                                               activation=False)
-
-    def forward(self, x):
-        identity = self.skip(x)
-
-        x = self.conv1(x)
-        x = self.conv2(x)
-        x = self.conv3(x)
+        self.conv3 = ConvBlock(dim3, kernel_size=1, activation=False)
+        self.act = layers.ReLU()
+        self.skip = Identity() if not stride else ConvBlock(dim3,
+                                                            kernel_size=1,
+                                                            stride=stride,
+                                                            activation=False)
+
+    def call(self, inputs, training=None):
+        identity = self.skip(inputs, training)
+
+        x = self.conv1(inputs, training)
+        x = self.conv2(x, training)
+        x = self.conv3(x, training)
 
         x += identity
         x = self.act(x)
         return x
 
 
-class Stem(nn.Sequential):
-    def __init__(self, cin, spatial_dims=2):
-        super().__init__(
-            ConvBlock(cin, 64, 7, spatial_dims, stride=2),
-            MaxPool(spatial_dims, 3, 2, padding=autopad(3))
-        )
-
-
-class StageBlock(nn.Sequential):
-    def __init__(self, cin, dims, stride, repeats):
-        super().__init__()
-
-
-class ResNet50V1(nn.Module):
-    def __init__(self, cin=3, spatial_dims=2):
-        super().__init__()
-        self.conv1 = Stem(cin, spatial_dims)
-        self.conv2 = nn.Sequential(
-            Bottleneck(64, [64, 256], 3, spatial_dims, stride=1),
-            Bottleneck(256, [64, 256], 3, spatial_dims),
-            Bottleneck(256, [64, 256], 3, spatial_dims),
-        )
-        self.conv3 = nn.Sequential(
-            Bottleneck(256, [128, 512], 3, spatial_dims, stride=2),
-            Bottleneck(512, [128, 512], 3, spatial_dims),
-            Bottleneck(512, [128, 512], 3, spatial_dims),
-            Bottleneck(512, [128, 512], 3, spatial_dims),
-        )
-        self.conv4 = nn.Sequential(
-            Bottleneck(512, [256, 1024], 3, spatial_dims, stride=2),
-            Bottleneck(1024, [256, 1024], 3, spatial_dims),
-            Bottleneck(1024, [256, 1024], 3, spatial_dims),
-            Bottleneck(1024, [256, 1024], 3, spatial_dims),
-            Bottleneck(1024, [256, 1024], 3, spatial_dims),
-            Bottleneck(1024, [256, 1024], 3, spatial_dims),
-        )
-        self.conv5 = nn.Sequential(
-            Bottleneck(1024, [512, 2048], 3, spatial_dims, stride=2),
-            Bottleneck(2048, [512, 2048], 3, spatial_dims),
-            Bottleneck(2048, [512, 2048], 3, spatial_dims),
-        )
-    def forward(self, x):
-        x = self.conv1(x)
-        x = self.conv2(x)
-        x = self.conv3(x)
-        x = self.conv4(x)
-        x = self.conv5(x)
+class TFResNet50V1(Model):
+    def __init__(self):
+        super(TFResNet50V1, self).__init__()
+        self.conv1 = Sequential([
+            ConvBlock(64, 7, stride=2),
+            layers.MaxPool2D(3, strides=2, padding='same'),
+        ])
+        self.conv2 = Sequential([
+            Bottleneck([64, 64, 256], 3, stride=1),
+            Bottleneck([64, 64, 256], 3),
+            Bottleneck([64, 64, 256], 3),
+        ])
+        self.conv3 = Sequential([
+            Bottleneck([128, 128, 512], 3, stride=2),
+            Bottleneck([128, 128, 512], 3),
+            Bottleneck([128, 128, 512], 3),
+            Bottleneck([128, 128, 512], 3),
+        ])
+        self.conv4 = Sequential([
+            Bottleneck([256, 256, 1024], 3, stride=2),
+            Bottleneck([256, 256, 1024], 3),
+            Bottleneck([256, 256, 1024], 3),
+            Bottleneck([256, 256, 1024], 3),
+            Bottleneck([256, 256, 1024], 3),
+            Bottleneck([256, 256, 1024], 3),
+        ])
+        self.conv5 = Sequential([
+            Bottleneck([512, 512, 2048], 3, stride=2),
+            Bottleneck([512, 512, 2048], 3),
+            Bottleneck([512, 512, 2048], 3),
+        ])
+
+    def call(self, inputs, training=None):
+        x = self.conv1(inputs, training)
+        x = self.conv2(x, training)
+        x = self.conv3(x, training)
+        x = self.conv4(x, training)
+        x = self.conv5(x, training)
         return x
 
 
 if __name__ == '__main__':
-    cin = 128
-    inputs = torch.normal(0, 1, (1, cin, 224, 224))
-
-    output = Bottleneck(cin, [64, 128], spatial_dims=2)(inputs)
-    shape = list(output.shape)
+    inputs = tf.random.normal((1, 224, 224, 128))
+    output = Bottleneck([64, 64, 128])(inputs)
+    shape = output.shape
     print("Bottleneck", shape)
-    assert shape == [1, 128, 224, 224]
+    assert shape == (1, 224, 224, 128)
 
-    output = Bottleneck(cin, [128, 256], spatial_dims=2, stride=1)(inputs)
-    shape = list(output.shape)
+    output = Bottleneck([128, 128, 256], stride=1)(inputs)
+    shape = output.shape
     print("Bottleneck first conv for aligh dims", shape)
-    assert shape == [1, 256, 224, 224]
+    assert shape == (1, 224, 224, 256)
 
-    output = Bottleneck(cin, [64, 128], spatial_dims=2, stride=2)(inputs)
-    shape = list(output.shape)
+    output = Bottleneck([64, 64, 128], stride=2)(inputs)
+    shape = output.shape
     print("Bottleneck downsample", shape)
-    assert shape == [1, 128, 112, 112]
+    assert shape == (1, 112, 112, 128)
+
+    output = Identity()(inputs)
+    shape = output.shape
+    print("Identity", shape)
+    assert shape == (1, 224, 224, 128)
+
+
+    output = TFResNet50V1()(inputs)
+    shape = output.shape
+    print("TFResNet50V1", shape)
+    assert  shape == (1, 7, 7, 2048)
+
 
-    output = ResNet50V1(cin, spatial_dims=2)(inputs)
-    shape = list(output.shape)
-    print("ResNet50V1", shape)
-    assert shape == [1, 2048, 7, 7]
-
-    print("1D ResNet50V1")
-    inputs = torch.normal(0, 1, (1, cin, 224))
-    output = ResNet50V1(cin, spatial_dims=1)(inputs)
-    shape = list(output.shape)
-    print("ResNet50V1", shape)
-    assert shape == [1, 2048, 7]
-
-    print("3D ResNet50V1")
-    D = H = W = 64
-    inputs = torch.rand(1, 3, D, H, W)
-    model = ResNet50V1(3, spatial_dims=3)
-    output = model(inputs)
-    print(output.shape)
```

### Comparing `fusionlab-0.1.5/fusionlab/encoders/vgg/tfvgg.py` & `fusionlab-0.1.6/fusionlab/encoders/vgg/tfvgg.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.5/fusionlab/encoders/vgg/vgg.py` & `fusionlab-0.1.6/fusionlab/encoders/vgg/vgg.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.5/fusionlab/functional/tfdice.py` & `fusionlab-0.1.6/fusionlab/functional/tfdice.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.5/fusionlab/functional/tfiou.py` & `fusionlab-0.1.6/fusionlab/functional/tfiou.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.5/fusionlab/layers/base.py` & `fusionlab-0.1.6/fusionlab/layers/base.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.5/fusionlab/layers/factories.py` & `fusionlab-0.1.6/fusionlab/layers/factories.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,24 @@
 from typing import Union, Sequence
 import torch
 from torch import nn
 
+__all__ = [
+    'ConvND',
+    'ConvT',
+    'Upsample',
+    'BatchNorm',
+    'MaxPool',
+    'AvgPool',
+    'AdaptiveMaxPool',
+    'AdaptiveAvgPool',
+    'ReplicationPad',
+    'ConstantPad'
+]
+
 class ConvND:
     """
     Factory class for creating convolutional layers. 
     This class is used to create convolutional layers with the same configuration.
 
     Args:
         spatial_dims (int): number of spatial dimensions of the input data.
@@ -17,15 +30,15 @@
         dilation (int or tuple, optional): spacing between kernel elements. Default: 1
         groups (int, optional): number of blocked connections from input channels to output channels. Default: 1
         bias (bool, optional): whether to add a bias to the convolution. Default: True
         padding_mode (str, optional): type of padding. Default: 'zeros'
 
     """
     def __new__(cls, 
-                spatial_dims, 
+                spatial_dims: int, 
                 in_channels: int,
                 out_channels: int,
                 kernel_size: Union[Sequence[int], int],
                 stride: Union[Sequence[int], int] = 1,
                 padding: Union[Sequence[int], str] = 0,
                 dilation: Union[Sequence[int], int] = 1,
                 groups: int = 1,
```

### Comparing `fusionlab-0.1.5/fusionlab/layers/squeeze_excitation/se.py` & `fusionlab-0.1.6/fusionlab/layers/squeeze_excitation/se.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.5/fusionlab/layers/squeeze_excitation/tfse.py` & `fusionlab-0.1.6/fusionlab/layers/squeeze_excitation/tfse.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.5/fusionlab/losses/diceloss/dice.py` & `fusionlab-0.1.6/fusionlab/losses/diceloss/dice.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.5/fusionlab/losses/diceloss/tfdice.py` & `fusionlab-0.1.6/fusionlab/losses/diceloss/tfdice.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.5/fusionlab/losses/iouloss/iou.py` & `fusionlab-0.1.6/fusionlab/losses/iouloss/iou.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.5/fusionlab/losses/iouloss/tfiou.py` & `fusionlab-0.1.6/fusionlab/losses/iouloss/tfiou.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.5/fusionlab/losses/tversky/tftversky.py` & `fusionlab-0.1.6/fusionlab/losses/tversky/tftversky.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.5/fusionlab/losses/tversky/tversky.py` & `fusionlab-0.1.6/fusionlab/losses/tversky/tversky.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.5/fusionlab/segmentation/base.py` & `fusionlab-0.1.6/fusionlab/segmentation/base.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.5/fusionlab/segmentation/resunet/resunet.py` & `fusionlab-0.1.6/fusionlab/segmentation/resunet/resunet.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.5/fusionlab/segmentation/resunet/tfresunet.py` & `fusionlab-0.1.6/fusionlab/segmentation/resunet/tfresunet.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.5/fusionlab/segmentation/tfbase.py` & `fusionlab-0.1.6/fusionlab/segmentation/tfbase.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.5/fusionlab/segmentation/unet/tfunet.py` & `fusionlab-0.1.6/fusionlab/segmentation/unet/tfunet.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.5/fusionlab/segmentation/unet/unet.py` & `fusionlab-0.1.6/fusionlab/segmentation/unet/unet.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.5/fusionlab/segmentation/unet2plus/tfunet2plus.py` & `fusionlab-0.1.6/fusionlab/segmentation/unet2plus/tfunet2plus.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.5/fusionlab/segmentation/unet2plus/unet2plus.py` & `fusionlab-0.1.6/fusionlab/segmentation/unet2plus/unet2plus.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.5/fusionlab/trainers/dcgan.py` & `fusionlab-0.1.6/fusionlab/trainers/dcgan.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.5/fusionlab/trainers/trainer.py` & `fusionlab-0.1.6/fusionlab/trainers/trainer.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.5/fusionlab/utils/basic.py` & `fusionlab-0.1.6/fusionlab/utils/basic.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.5/fusionlab/utils/trace.py` & `fusionlab-0.1.6/fusionlab/utils/trace.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.5/fusionlab.egg-info/PKG-INFO` & `fusionlab-0.1.6/fusionlab.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusionlab
-Version: 0.1.5
+Version: 0.1.6
 Summary: Useful packages for DL
 Home-page: https://github.com/taipingeric/fusionlab
 Author: Chih-Yang Li
 Author-email: taipingeric@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -21,26 +21,28 @@
     <br>
     <img src="assets/imgs/fusionlab_banner.png" width="400"/>
     <br>
 <p>
 
 [![PyPI version](https://badge.fury.io/py/fusionlab.svg)](https://badge.fury.io/py/fusionlab) ![Test](https://github.com/taipingeric/fusionlab/actions/workflows/python-app.yml/badge.svg)  [![Downloads](https://static.pepy.tech/badge/fusionlab)](https://pepy.tech/project/fusionlab)
 
+[![Documentation](https://img.shields.io/badge/view-Documentation-blue?style=for-the-badge)](https://fusionlab.readthedocs.io/)
+
 FusionLab is an open-source frameworks built for Deep Learning research written in PyTorch and Tensorflow. The code is easy to read and modify 
 especially for newbie. Feel free to send pull requests :D
 
-* [What's New](#News)
-* [Installation](#Installation)
-* [How to use](#How-to-use)
-* [Encoders](#Encoders)
-* [Losses](#Losses)
-* [Segmentation](#Segmentation)
+* [What's New](#news)
+* [Installation](#installation)
+* [How to use](#how-to-use)
+* [Encoders](#encoders)
+* [Losses](#losses)
+* [Segmentation](#segmentation)
 * [1D, 2D, 3D Model](#n-dimensional-model)
-* [Acknowledgements](#Acknowledgements)
-
+* [Acknowledgements](#acknowledgements)
+      
 ## Installation
 
 ### With pip
 
 ```bash
 pip install fusionlab
 ```
@@ -56,14 +58,18 @@
 # PyTorch
 encoder = fl.encoders.VGG16()
 # Tensorflow
 encoder = fl.encoders.TFVGG16()
 
 ```
 
+## Documentation
+
+[Doc](https://fusionlab.readthedocs.io/en/latest/encoders.html)
+
 ## Encoders
 
 [encoder list](fusionlab/encoders/README.md)
 
 ## Losses
 
 [Loss func list](fusionlab/losses/README.md)
```

### Comparing `fusionlab-0.1.5/fusionlab.egg-info/SOURCES.txt` & `fusionlab-0.1.6/fusionlab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.5/setup.py` & `fusionlab-0.1.6/setup.py`

 * *Files identical despite different names*

