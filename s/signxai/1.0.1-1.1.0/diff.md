# Comparing `tmp/signxai-1.0.1.tar.gz` & `tmp/signxai-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/nils/PycharmProjects/SIGN-XAI/dist/tmpzwnlkmen/signxai-1.0.1.tar", last modified: Mon Jul 10 13:44:54 2023, max compression
+gzip compressed data, was "/home/nils/PycharmProjects/SIGN-XAI/dist/tmpvlma2qok/signxai-1.1.0.tar", last modified: Fri Aug  4 10:31:00 2023, max compression
```

## Comparing `signxai-1.0.1.tar` & `signxai-1.1.0.tar`

### file list

```diff
@@ -1,102 +1,103 @@
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 13:44:54.000000 signxai-1.0.1/
--rw-rw-r--   0 nils      (1000) nils      (1000)       38 2023-07-10 13:44:54.000000 signxai-1.0.1/setup.cfg
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 13:44:54.000000 signxai-1.0.1/signxai/
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 13:44:54.000000 signxai-1.0.1/signxai/examples/
--rw-rw-r--   0 nils      (1000) nils      (1000)        0 2021-10-06 10:51:00.000000 signxai-1.0.1/signxai/examples/__init__.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     1046 2023-07-10 11:53:28.000000 signxai-1.0.1/signxai/examples/vgg16.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 13:44:54.000000 signxai-1.0.1/signxai/methods/
--rw-rw-r--   0 nils      (1000) nils      (1000)      253 2023-04-27 08:51:48.000000 signxai-1.0.1/signxai/methods/signed.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 13:44:54.000000 signxai-1.0.1/signxai/methods/innvestigate/
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 13:44:54.000000 signxai-1.0.1/signxai/methods/innvestigate/tools/
--rw-rw-r--   0 nils      (1000) nils      (1000)      225 2022-02-16 10:22:41.000000 signxai-1.0.1/signxai/methods/innvestigate/tools/__init__.py
--rw-rw-r--   0 nils      (1000) nils      (1000)    19540 2022-02-16 10:22:41.000000 signxai-1.0.1/signxai/methods/innvestigate/tools/pattern.py
--rw-rw-r--   0 nils      (1000) nils      (1000)    18118 2022-02-16 10:22:41.000000 signxai-1.0.1/signxai/methods/innvestigate/tools/perturbate.py
--rw-rw-r--   0 nils      (1000) nils      (1000)    19365 2022-02-16 10:22:41.000000 signxai-1.0.1/signxai/methods/innvestigate/layers.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 13:44:54.000000 signxai-1.0.1/signxai/methods/innvestigate/applications/
--rw-rw-r--   0 nils      (1000) nils      (1000)    10473 2022-02-16 10:22:41.000000 signxai-1.0.1/signxai/methods/innvestigate/applications/imagenet.py
--rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-1.0.1/signxai/methods/innvestigate/applications/__init__.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     4256 2022-02-16 10:22:41.000000 signxai-1.0.1/signxai/methods/innvestigate/applications/mnist.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 13:44:54.000000 signxai-1.0.1/signxai/methods/innvestigate/tests/
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 13:44:54.000000 signxai-1.0.1/signxai/methods/innvestigate/tests/tools/
--rw-rw-r--   0 nils      (1000) nils      (1000)     3969 2022-02-16 10:22:41.000000 signxai-1.0.1/signxai/methods/innvestigate/tests/tools/test_perturbate.py
--rw-rw-r--   0 nils      (1000) nils      (1000)    12358 2022-05-24 09:53:27.000000 signxai-1.0.1/signxai/methods/innvestigate/tests/tools/test_pattern.py
--rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-1.0.1/signxai/methods/innvestigate/tests/tools/__init__.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 13:44:54.000000 signxai-1.0.1/signxai/methods/innvestigate/tests/analyzer/
--rw-rw-r--   0 nils      (1000) nils      (1000)    10210 2022-02-16 10:22:41.000000 signxai-1.0.1/signxai/methods/innvestigate/tests/analyzer/test_relevance_based.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     3790 2022-02-16 10:22:41.000000 signxai-1.0.1/signxai/methods/innvestigate/tests/analyzer/test_wrapper.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     1303 2022-02-16 10:22:41.000000 signxai-1.0.1/signxai/methods/innvestigate/tests/analyzer/test_misc.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     3948 2022-02-16 10:22:41.000000 signxai-1.0.1/signxai/methods/innvestigate/tests/analyzer/test_deeplift.py
--rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-1.0.1/signxai/methods/innvestigate/tests/analyzer/__init__.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     3025 2022-02-16 10:22:41.000000 signxai-1.0.1/signxai/methods/innvestigate/tests/analyzer/test_pattern_based.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     4878 2022-02-16 10:22:41.000000 signxai-1.0.1/signxai/methods/innvestigate/tests/analyzer/test_base.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     7771 2022-02-16 10:22:41.000000 signxai-1.0.1/signxai/methods/innvestigate/tests/analyzer/test_gradient_based.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     1847 2022-02-16 10:22:41.000000 signxai-1.0.1/signxai/methods/innvestigate/tests/analyzer/test_deeptaylor.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     1511 2022-02-16 10:22:41.000000 signxai-1.0.1/signxai/methods/innvestigate/tests/analyzer/test_init.py
--rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-1.0.1/signxai/methods/innvestigate/tests/__init__.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 13:44:54.000000 signxai-1.0.1/signxai/methods/innvestigate/tests/utils/
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 13:44:54.000000 signxai-1.0.1/signxai/methods/innvestigate/tests/utils/keras/
--rw-rw-r--   0 nils      (1000) nils      (1000)     1759 2022-02-16 10:22:41.000000 signxai-1.0.1/signxai/methods/innvestigate/tests/utils/keras/test_graph.py
--rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-1.0.1/signxai/methods/innvestigate/tests/utils/keras/__init__.py
--rw-rw-r--   0 nils      (1000) nils      (1000)      967 2022-02-16 10:22:41.000000 signxai-1.0.1/signxai/methods/innvestigate/tests/utils/test_visualizations.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 13:44:54.000000 signxai-1.0.1/signxai/methods/innvestigate/tests/utils/tests/
--rw-rw-r--   0 nils      (1000) nils      (1000)     1189 2022-02-16 10:22:41.000000 signxai-1.0.1/signxai/methods/innvestigate/tests/utils/tests/test_dryrun.py
--rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-1.0.1/signxai/methods/innvestigate/tests/utils/tests/__init__.py
--rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-1.0.1/signxai/methods/innvestigate/tests/utils/__init__.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 13:44:54.000000 signxai-1.0.1/signxai/methods/innvestigate/analyzer/
--rw-rw-r--   0 nils      (1000) nils      (1000)     8539 2023-07-10 11:08:26.000000 signxai-1.0.1/signxai/methods/innvestigate/analyzer/pattern_based.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     1948 2022-02-16 10:22:41.000000 signxai-1.0.1/signxai/methods/innvestigate/analyzer/misc.py
--rw-rw-r--   0 nils      (1000) nils      (1000)    14700 2023-07-10 11:08:26.000000 signxai-1.0.1/signxai/methods/innvestigate/analyzer/gradient_based.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     7094 2022-02-16 10:22:41.000000 signxai-1.0.1/signxai/methods/innvestigate/analyzer/deeptaylor.py
--rw-rw-r--   0 nils      (1000) nils      (1000)    13638 2023-07-10 11:08:26.000000 signxai-1.0.1/signxai/methods/innvestigate/analyzer/wrapper.py
--rw-rw-r--   0 nils      (1000) nils      (1000)    26365 2022-05-11 10:33:05.000000 signxai-1.0.1/signxai/methods/innvestigate/analyzer/reverse_map.py
--rw-rw-r--   0 nils      (1000) nils      (1000)    20907 2022-04-06 15:20:24.000000 signxai-1.0.1/signxai/methods/innvestigate/analyzer/base.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     4395 2022-07-20 07:31:35.000000 signxai-1.0.1/signxai/methods/innvestigate/analyzer/__init__.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 13:44:54.000000 signxai-1.0.1/signxai/methods/innvestigate/analyzer/canonization/
--rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-1.0.1/signxai/methods/innvestigate/analyzer/canonization/__init__.py
--rw-rw-r--   0 nils      (1000) nils      (1000)    15327 2022-02-16 10:22:41.000000 signxai-1.0.1/signxai/methods/innvestigate/analyzer/deeplift.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 13:44:54.000000 signxai-1.0.1/signxai/methods/innvestigate/analyzer/relevance_based/
--rw-rw-r--   0 nils      (1000) nils      (1000)     3842 2022-02-16 10:22:41.000000 signxai-1.0.1/signxai/methods/innvestigate/analyzer/relevance_based/utils.py
--rw-rw-r--   0 nils      (1000) nils      (1000)       65 2022-02-16 10:22:41.000000 signxai-1.0.1/signxai/methods/innvestigate/analyzer/relevance_based/__init__.py
--rw-rw-r--   0 nils      (1000) nils      (1000)    24163 2023-07-10 11:08:25.000000 signxai-1.0.1/signxai/methods/innvestigate/analyzer/relevance_based/relevance_analyzer.py
--rw-rw-r--   0 nils      (1000) nils      (1000)    52929 2023-07-10 09:21:05.000000 signxai-1.0.1/signxai/methods/innvestigate/analyzer/relevance_based/relevance_rule_base.py
--rw-rw-r--   0 nils      (1000) nils      (1000)      216 2022-02-16 10:22:41.000000 signxai-1.0.1/signxai/methods/innvestigate/__init__.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 13:44:54.000000 signxai-1.0.1/signxai/methods/innvestigate/backend/
--rw-rw-r--   0 nils      (1000) nils      (1000)     1234 2022-02-16 10:22:41.000000 signxai-1.0.1/signxai/methods/innvestigate/backend/__init__.py
--rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-1.0.1/signxai/methods/innvestigate/backend/tensorflow.py
--rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-1.0.1/signxai/methods/innvestigate/backend/torch.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 13:44:54.000000 signxai-1.0.1/signxai/methods/innvestigate/utils/
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 13:44:54.000000 signxai-1.0.1/signxai/methods/innvestigate/utils/keras/
--rw-rw-r--   0 nils      (1000) nils      (1000)     5921 2022-02-16 10:22:41.000000 signxai-1.0.1/signxai/methods/innvestigate/utils/keras/backend.py
--rw-rw-r--   0 nils      (1000) nils      (1000)    14517 2022-04-06 15:20:24.000000 signxai-1.0.1/signxai/methods/innvestigate/utils/keras/checks.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     2318 2022-02-16 10:22:41.000000 signxai-1.0.1/signxai/methods/innvestigate/utils/keras/__init__.py
--rw-rw-r--   0 nils      (1000) nils      (1000)    43869 2022-02-16 10:22:41.000000 signxai-1.0.1/signxai/methods/innvestigate/utils/keras/graph.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     4925 2022-02-16 10:22:41.000000 signxai-1.0.1/signxai/methods/innvestigate/utils/visualizations.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 13:44:54.000000 signxai-1.0.1/signxai/methods/innvestigate/utils/tests/
--rw-rw-r--   0 nils      (1000) nils      (1000)     2818 2022-02-16 10:22:41.000000 signxai-1.0.1/signxai/methods/innvestigate/utils/tests/dryrun.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 13:44:54.000000 signxai-1.0.1/signxai/methods/innvestigate/utils/tests/cases/
--rw-rw-r--   0 nils      (1000) nils      (1000)     1313 2022-02-16 10:22:41.000000 signxai-1.0.1/signxai/methods/innvestigate/utils/tests/cases/mlp.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     1634 2022-02-16 10:22:41.000000 signxai-1.0.1/signxai/methods/innvestigate/utils/tests/cases/special.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     1383 2022-02-16 10:22:41.000000 signxai-1.0.1/signxai/methods/innvestigate/utils/tests/cases/helper.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     3322 2022-02-16 10:22:41.000000 signxai-1.0.1/signxai/methods/innvestigate/utils/tests/cases/cnn.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     2457 2022-02-16 10:22:41.000000 signxai-1.0.1/signxai/methods/innvestigate/utils/tests/cases/__init__.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     1592 2022-02-16 10:22:41.000000 signxai-1.0.1/signxai/methods/innvestigate/utils/tests/cases/trivia.py
--rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-1.0.1/signxai/methods/innvestigate/utils/tests/__init__.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     5791 2022-02-16 10:22:41.000000 signxai-1.0.1/signxai/methods/innvestigate/utils/__init__.py
--rw-rw-r--   0 nils      (1000) nils      (1000)        0 2021-10-06 10:51:00.000000 signxai-1.0.1/signxai/methods/__init__.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     2603 2022-09-16 14:59:58.000000 signxai-1.0.1/signxai/methods/grad_cam.py
--rw-rw-r--   0 nils      (1000) nils      (1000)    25764 2023-07-10 11:08:25.000000 signxai-1.0.1/signxai/methods/wrappers.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     1499 2022-04-26 09:45:35.000000 signxai-1.0.1/signxai/methods/guided_backprop.py
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 13:44:54.000000 signxai-1.0.1/signxai/utils/
--rw-rw-r--   0 nils      (1000) nils      (1000)     1898 2023-07-10 11:52:53.000000 signxai-1.0.1/signxai/utils/utils.py
--rw-rw-r--   0 nils      (1000) nils      (1000)        0 2023-07-10 10:28:07.000000 signxai-1.0.1/signxai/utils/__init__.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     2403 2023-07-10 11:58:43.000000 signxai-1.0.1/README.md
--rw-rw-r--   0 nils      (1000) nils      (1000)       33 2023-07-10 11:40:05.000000 signxai-1.0.1/MANIFEST.in
-drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-07-10 13:44:54.000000 signxai-1.0.1/signxai.egg-info/
--rw-rw-r--   0 nils      (1000) nils      (1000)       53 2023-07-10 13:44:54.000000 signxai-1.0.1/signxai.egg-info/requires.txt
--rw-rw-r--   0 nils      (1000) nils      (1000)        1 2023-07-10 13:44:54.000000 signxai-1.0.1/signxai.egg-info/dependency_links.txt
--rw-rw-r--   0 nils      (1000) nils      (1000)     3706 2023-07-10 13:44:54.000000 signxai-1.0.1/signxai.egg-info/SOURCES.txt
--rw-rw-r--   0 nils      (1000) nils      (1000)        8 2023-07-10 13:44:54.000000 signxai-1.0.1/signxai.egg-info/top_level.txt
--rw-rw-r--   0 nils      (1000) nils      (1000)     3202 2023-07-10 13:44:54.000000 signxai-1.0.1/signxai.egg-info/PKG-INFO
--rw-rw-r--   0 nils      (1000) nils      (1000)     2010 2023-07-10 13:44:35.000000 signxai-1.0.1/setup.py
--rw-rw-r--   0 nils      (1000) nils      (1000)     3202 2023-07-10 13:44:54.000000 signxai-1.0.1/PKG-INFO
--rw-rw-r--   0 nils      (1000) nils      (1000)     2182 2023-07-10 08:27:19.000000 signxai-1.0.1/LICENSE
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-08-04 10:31:00.000000 signxai-1.1.0/
+-rw-rw-r--   0 nils      (1000) nils      (1000)       38 2023-08-04 10:31:00.000000 signxai-1.1.0/setup.cfg
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-08-04 10:31:00.000000 signxai-1.1.0/signxai/
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-08-04 10:31:00.000000 signxai-1.1.0/signxai/examples/
+-rw-rw-r--   0 nils      (1000) nils      (1000)        0 2021-10-06 10:51:00.000000 signxai-1.1.0/signxai/examples/__init__.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     1609 2023-08-04 10:28:40.000000 signxai-1.1.0/signxai/examples/mnist.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     1602 2023-08-04 10:24:24.000000 signxai-1.1.0/signxai/examples/vgg16.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-08-04 10:31:00.000000 signxai-1.1.0/signxai/methods/
+-rw-rw-r--   0 nils      (1000) nils      (1000)      253 2023-04-27 08:51:48.000000 signxai-1.1.0/signxai/methods/signed.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-08-04 10:31:00.000000 signxai-1.1.0/signxai/methods/innvestigate/
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-08-04 10:31:00.000000 signxai-1.1.0/signxai/methods/innvestigate/tools/
+-rw-rw-r--   0 nils      (1000) nils      (1000)      225 2022-02-16 10:22:41.000000 signxai-1.1.0/signxai/methods/innvestigate/tools/__init__.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)    19540 2022-02-16 10:22:41.000000 signxai-1.1.0/signxai/methods/innvestigate/tools/pattern.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)    18118 2022-02-16 10:22:41.000000 signxai-1.1.0/signxai/methods/innvestigate/tools/perturbate.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)    19365 2022-02-16 10:22:41.000000 signxai-1.1.0/signxai/methods/innvestigate/layers.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-08-04 10:31:00.000000 signxai-1.1.0/signxai/methods/innvestigate/applications/
+-rw-rw-r--   0 nils      (1000) nils      (1000)    10473 2022-02-16 10:22:41.000000 signxai-1.1.0/signxai/methods/innvestigate/applications/imagenet.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-1.1.0/signxai/methods/innvestigate/applications/__init__.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     4256 2022-02-16 10:22:41.000000 signxai-1.1.0/signxai/methods/innvestigate/applications/mnist.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-08-04 10:31:00.000000 signxai-1.1.0/signxai/methods/innvestigate/tests/
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-08-04 10:31:00.000000 signxai-1.1.0/signxai/methods/innvestigate/tests/tools/
+-rw-rw-r--   0 nils      (1000) nils      (1000)     3969 2022-02-16 10:22:41.000000 signxai-1.1.0/signxai/methods/innvestigate/tests/tools/test_perturbate.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)    12358 2022-05-24 09:53:27.000000 signxai-1.1.0/signxai/methods/innvestigate/tests/tools/test_pattern.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-1.1.0/signxai/methods/innvestigate/tests/tools/__init__.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-08-04 10:31:00.000000 signxai-1.1.0/signxai/methods/innvestigate/tests/analyzer/
+-rw-rw-r--   0 nils      (1000) nils      (1000)    10210 2022-02-16 10:22:41.000000 signxai-1.1.0/signxai/methods/innvestigate/tests/analyzer/test_relevance_based.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     3790 2022-02-16 10:22:41.000000 signxai-1.1.0/signxai/methods/innvestigate/tests/analyzer/test_wrapper.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     1303 2022-02-16 10:22:41.000000 signxai-1.1.0/signxai/methods/innvestigate/tests/analyzer/test_misc.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     3948 2022-02-16 10:22:41.000000 signxai-1.1.0/signxai/methods/innvestigate/tests/analyzer/test_deeplift.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-1.1.0/signxai/methods/innvestigate/tests/analyzer/__init__.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     3025 2022-02-16 10:22:41.000000 signxai-1.1.0/signxai/methods/innvestigate/tests/analyzer/test_pattern_based.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     4878 2022-02-16 10:22:41.000000 signxai-1.1.0/signxai/methods/innvestigate/tests/analyzer/test_base.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     7771 2022-02-16 10:22:41.000000 signxai-1.1.0/signxai/methods/innvestigate/tests/analyzer/test_gradient_based.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     1847 2022-02-16 10:22:41.000000 signxai-1.1.0/signxai/methods/innvestigate/tests/analyzer/test_deeptaylor.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     1511 2022-02-16 10:22:41.000000 signxai-1.1.0/signxai/methods/innvestigate/tests/analyzer/test_init.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-1.1.0/signxai/methods/innvestigate/tests/__init__.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-08-04 10:31:00.000000 signxai-1.1.0/signxai/methods/innvestigate/tests/utils/
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-08-04 10:31:00.000000 signxai-1.1.0/signxai/methods/innvestigate/tests/utils/keras/
+-rw-rw-r--   0 nils      (1000) nils      (1000)     1759 2022-02-16 10:22:41.000000 signxai-1.1.0/signxai/methods/innvestigate/tests/utils/keras/test_graph.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-1.1.0/signxai/methods/innvestigate/tests/utils/keras/__init__.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)      967 2022-02-16 10:22:41.000000 signxai-1.1.0/signxai/methods/innvestigate/tests/utils/test_visualizations.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-08-04 10:31:00.000000 signxai-1.1.0/signxai/methods/innvestigate/tests/utils/tests/
+-rw-rw-r--   0 nils      (1000) nils      (1000)     1189 2022-02-16 10:22:41.000000 signxai-1.1.0/signxai/methods/innvestigate/tests/utils/tests/test_dryrun.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-1.1.0/signxai/methods/innvestigate/tests/utils/tests/__init__.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-1.1.0/signxai/methods/innvestigate/tests/utils/__init__.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-08-04 10:31:00.000000 signxai-1.1.0/signxai/methods/innvestigate/analyzer/
+-rw-rw-r--   0 nils      (1000) nils      (1000)     8539 2023-07-10 11:08:26.000000 signxai-1.1.0/signxai/methods/innvestigate/analyzer/pattern_based.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     1948 2022-02-16 10:22:41.000000 signxai-1.1.0/signxai/methods/innvestigate/analyzer/misc.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)    14700 2023-07-10 11:08:26.000000 signxai-1.1.0/signxai/methods/innvestigate/analyzer/gradient_based.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     7094 2022-02-16 10:22:41.000000 signxai-1.1.0/signxai/methods/innvestigate/analyzer/deeptaylor.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)    13638 2023-07-10 11:08:26.000000 signxai-1.1.0/signxai/methods/innvestigate/analyzer/wrapper.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)    26365 2022-05-11 10:33:05.000000 signxai-1.1.0/signxai/methods/innvestigate/analyzer/reverse_map.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)    20907 2022-04-06 15:20:24.000000 signxai-1.1.0/signxai/methods/innvestigate/analyzer/base.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     4395 2022-07-20 07:31:35.000000 signxai-1.1.0/signxai/methods/innvestigate/analyzer/__init__.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-08-04 10:31:00.000000 signxai-1.1.0/signxai/methods/innvestigate/analyzer/canonization/
+-rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-1.1.0/signxai/methods/innvestigate/analyzer/canonization/__init__.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)    15327 2022-02-16 10:22:41.000000 signxai-1.1.0/signxai/methods/innvestigate/analyzer/deeplift.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-08-04 10:31:00.000000 signxai-1.1.0/signxai/methods/innvestigate/analyzer/relevance_based/
+-rw-rw-r--   0 nils      (1000) nils      (1000)     3842 2022-02-16 10:22:41.000000 signxai-1.1.0/signxai/methods/innvestigate/analyzer/relevance_based/utils.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)       65 2022-02-16 10:22:41.000000 signxai-1.1.0/signxai/methods/innvestigate/analyzer/relevance_based/__init__.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)    24163 2023-07-10 11:08:25.000000 signxai-1.1.0/signxai/methods/innvestigate/analyzer/relevance_based/relevance_analyzer.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)    52929 2023-07-10 09:21:05.000000 signxai-1.1.0/signxai/methods/innvestigate/analyzer/relevance_based/relevance_rule_base.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)      216 2022-02-16 10:22:41.000000 signxai-1.1.0/signxai/methods/innvestigate/__init__.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-08-04 10:31:00.000000 signxai-1.1.0/signxai/methods/innvestigate/backend/
+-rw-rw-r--   0 nils      (1000) nils      (1000)     1234 2022-02-16 10:22:41.000000 signxai-1.1.0/signxai/methods/innvestigate/backend/__init__.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-1.1.0/signxai/methods/innvestigate/backend/tensorflow.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-1.1.0/signxai/methods/innvestigate/backend/torch.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-08-04 10:31:00.000000 signxai-1.1.0/signxai/methods/innvestigate/utils/
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-08-04 10:31:00.000000 signxai-1.1.0/signxai/methods/innvestigate/utils/keras/
+-rw-rw-r--   0 nils      (1000) nils      (1000)     5921 2022-02-16 10:22:41.000000 signxai-1.1.0/signxai/methods/innvestigate/utils/keras/backend.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)    12901 2023-08-04 09:17:51.000000 signxai-1.1.0/signxai/methods/innvestigate/utils/keras/checks.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     2318 2022-02-16 10:22:41.000000 signxai-1.1.0/signxai/methods/innvestigate/utils/keras/__init__.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)    43869 2022-02-16 10:22:41.000000 signxai-1.1.0/signxai/methods/innvestigate/utils/keras/graph.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     4925 2022-02-16 10:22:41.000000 signxai-1.1.0/signxai/methods/innvestigate/utils/visualizations.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-08-04 10:31:00.000000 signxai-1.1.0/signxai/methods/innvestigate/utils/tests/
+-rw-rw-r--   0 nils      (1000) nils      (1000)     2818 2022-02-16 10:22:41.000000 signxai-1.1.0/signxai/methods/innvestigate/utils/tests/dryrun.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-08-04 10:31:00.000000 signxai-1.1.0/signxai/methods/innvestigate/utils/tests/cases/
+-rw-rw-r--   0 nils      (1000) nils      (1000)     1313 2022-02-16 10:22:41.000000 signxai-1.1.0/signxai/methods/innvestigate/utils/tests/cases/mlp.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     1634 2022-02-16 10:22:41.000000 signxai-1.1.0/signxai/methods/innvestigate/utils/tests/cases/special.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     1383 2022-02-16 10:22:41.000000 signxai-1.1.0/signxai/methods/innvestigate/utils/tests/cases/helper.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     3322 2022-02-16 10:22:41.000000 signxai-1.1.0/signxai/methods/innvestigate/utils/tests/cases/cnn.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     2457 2022-02-16 10:22:41.000000 signxai-1.1.0/signxai/methods/innvestigate/utils/tests/cases/__init__.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     1592 2022-02-16 10:22:41.000000 signxai-1.1.0/signxai/methods/innvestigate/utils/tests/cases/trivia.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)        0 2022-02-16 10:22:41.000000 signxai-1.1.0/signxai/methods/innvestigate/utils/tests/__init__.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     5791 2022-02-16 10:22:41.000000 signxai-1.1.0/signxai/methods/innvestigate/utils/__init__.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)        0 2021-10-06 10:51:00.000000 signxai-1.1.0/signxai/methods/__init__.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     2603 2022-09-16 14:59:58.000000 signxai-1.1.0/signxai/methods/grad_cam.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)    25764 2023-07-10 11:08:25.000000 signxai-1.1.0/signxai/methods/wrappers.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     1499 2022-04-26 09:45:35.000000 signxai-1.1.0/signxai/methods/guided_backprop.py
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-08-04 10:31:00.000000 signxai-1.1.0/signxai/utils/
+-rw-rw-r--   0 nils      (1000) nils      (1000)     2093 2023-08-04 10:25:36.000000 signxai-1.1.0/signxai/utils/utils.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)        0 2023-07-10 10:28:07.000000 signxai-1.1.0/signxai/utils/__init__.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     4726 2023-08-04 10:29:25.000000 signxai-1.1.0/README.md
+-rw-rw-r--   0 nils      (1000) nils      (1000)       33 2023-07-10 11:40:05.000000 signxai-1.1.0/MANIFEST.in
+drwxrwxr-x   0 nils      (1000) nils      (1000)        0 2023-08-04 10:31:00.000000 signxai-1.1.0/signxai.egg-info/
+-rw-rw-r--   0 nils      (1000) nils      (1000)       75 2023-08-04 10:31:00.000000 signxai-1.1.0/signxai.egg-info/requires.txt
+-rw-rw-r--   0 nils      (1000) nils      (1000)        1 2023-08-04 10:31:00.000000 signxai-1.1.0/signxai.egg-info/dependency_links.txt
+-rw-rw-r--   0 nils      (1000) nils      (1000)     3732 2023-08-04 10:31:00.000000 signxai-1.1.0/signxai.egg-info/SOURCES.txt
+-rw-rw-r--   0 nils      (1000) nils      (1000)        8 2023-08-04 10:31:00.000000 signxai-1.1.0/signxai.egg-info/top_level.txt
+-rw-rw-r--   0 nils      (1000) nils      (1000)     5525 2023-08-04 10:31:00.000000 signxai-1.1.0/signxai.egg-info/PKG-INFO
+-rw-rw-r--   0 nils      (1000) nils      (1000)     2035 2023-08-04 10:30:30.000000 signxai-1.1.0/setup.py
+-rw-rw-r--   0 nils      (1000) nils      (1000)     5525 2023-08-04 10:31:00.000000 signxai-1.1.0/PKG-INFO
+-rw-rw-r--   0 nils      (1000) nils      (1000)     2182 2023-07-10 08:27:19.000000 signxai-1.1.0/LICENSE
```

### Comparing `signxai-1.0.1/signxai/examples/vgg16.py` & `signxai-1.1.0/signxai/examples/vgg16.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 import numpy as np
 import matplotlib.pyplot as plt
 from tensorflow.keras.applications.vgg16 import VGG16
 from signxai.methods.wrappers import calculate_relevancemap
-from signxai.utils.utils import load_image, aggregate_and_normalize_relevancemap_rgb, download_image
+from signxai.utils.utils import (load_image, aggregate_and_normalize_relevancemap_rgb, download_image, 
+                                 calculate_explanation_innvestigate)
 
 # Load model
 model = VGG16(weights='imagenet')
 
 #  Remove last layer's softmax activation (we need the raw values!)
 model.layers[-1].activation = None
 
 # Load example image
-path = 'example.png'
+path = 'example.jpg'
 download_image(path)
 img, x = load_image(path)
 
 # Calculate relevancemaps
 R1 = calculate_relevancemap('lrpz_epsilon_0_1_std_x', np.array(x), model)
 R2 = calculate_relevancemap('lrpsign_epsilon_0_1_std_x', np.array(x), model)
 
-# Aggregate and normalize relevancemaps for visualization
-H1 = aggregate_and_normalize_relevancemap_rgb(R1)
-H2 = aggregate_and_normalize_relevancemap_rgb(R2)
+# Equivalent relevance maps as for R1 and R2, but with direct access to innvestigate and parameters
+R3 = calculate_explanation_innvestigate(model, x, method='lrp.stdxepsilon', stdfactor=0.1, input_layer_rule='Z')
+R4 = calculate_explanation_innvestigate(model, x, method='lrp.stdxepsilon', stdfactor=0.1, input_layer_rule='SIGN')
 
 # Visualize heatmaps
-fig, axs = plt.subplots(ncols=3, figsize=(18, 6))
-axs[0].imshow(img)
-axs[1].matshow(H1, cmap='seismic', clim=(-1, 1))
-axs[2].matshow(H2, cmap='seismic', clim=(-1, 1))
+fig, axs = plt.subplots(ncols=3, nrows=2, figsize=(18, 12))
+axs[0][0].imshow(img)
+axs[1][0].imshow(img)
+axs[0][1].matshow(aggregate_and_normalize_relevancemap_rgb(R1), cmap='seismic', clim=(-1, 1))
+axs[0][2].matshow(aggregate_and_normalize_relevancemap_rgb(R2), cmap='seismic', clim=(-1, 1))
+axs[1][1].matshow(aggregate_and_normalize_relevancemap_rgb(R3), cmap='seismic', clim=(-1, 1))
+axs[1][2].matshow(aggregate_and_normalize_relevancemap_rgb(R4), cmap='seismic', clim=(-1, 1))
 
 plt.show()
```

### Comparing `signxai-1.0.1/signxai/methods/innvestigate/tools/pattern.py` & `signxai-1.1.0/signxai/methods/innvestigate/tools/pattern.py`

 * *Files identical despite different names*

### Comparing `signxai-1.0.1/signxai/methods/innvestigate/tools/perturbate.py` & `signxai-1.1.0/signxai/methods/innvestigate/tools/perturbate.py`

 * *Files identical despite different names*

### Comparing `signxai-1.0.1/signxai/methods/innvestigate/layers.py` & `signxai-1.1.0/signxai/methods/innvestigate/layers.py`

 * *Files identical despite different names*

### Comparing `signxai-1.0.1/signxai/methods/innvestigate/applications/imagenet.py` & `signxai-1.1.0/signxai/methods/innvestigate/applications/imagenet.py`

 * *Files identical despite different names*

### Comparing `signxai-1.0.1/signxai/methods/innvestigate/applications/mnist.py` & `signxai-1.1.0/signxai/methods/innvestigate/applications/mnist.py`

 * *Files identical despite different names*

### Comparing `signxai-1.0.1/signxai/methods/innvestigate/tests/tools/test_perturbate.py` & `signxai-1.1.0/signxai/methods/innvestigate/tests/tools/test_perturbate.py`

 * *Files identical despite different names*

### Comparing `signxai-1.0.1/signxai/methods/innvestigate/tests/tools/test_pattern.py` & `signxai-1.1.0/signxai/methods/innvestigate/tests/tools/test_pattern.py`

 * *Files identical despite different names*

### Comparing `signxai-1.0.1/signxai/methods/innvestigate/tests/analyzer/test_relevance_based.py` & `signxai-1.1.0/signxai/methods/innvestigate/tests/analyzer/test_relevance_based.py`

 * *Files identical despite different names*

### Comparing `signxai-1.0.1/signxai/methods/innvestigate/tests/analyzer/test_wrapper.py` & `signxai-1.1.0/signxai/methods/innvestigate/tests/analyzer/test_wrapper.py`

 * *Files identical despite different names*

### Comparing `signxai-1.0.1/signxai/methods/innvestigate/tests/analyzer/test_misc.py` & `signxai-1.1.0/signxai/methods/innvestigate/tests/analyzer/test_misc.py`

 * *Files identical despite different names*

### Comparing `signxai-1.0.1/signxai/methods/innvestigate/tests/analyzer/test_deeplift.py` & `signxai-1.1.0/signxai/methods/innvestigate/tests/analyzer/test_deeplift.py`

 * *Files identical despite different names*

### Comparing `signxai-1.0.1/signxai/methods/innvestigate/tests/analyzer/test_pattern_based.py` & `signxai-1.1.0/signxai/methods/innvestigate/tests/analyzer/test_pattern_based.py`

 * *Files identical despite different names*

### Comparing `signxai-1.0.1/signxai/methods/innvestigate/tests/analyzer/test_base.py` & `signxai-1.1.0/signxai/methods/innvestigate/tests/analyzer/test_base.py`

 * *Files identical despite different names*

### Comparing `signxai-1.0.1/signxai/methods/innvestigate/tests/analyzer/test_gradient_based.py` & `signxai-1.1.0/signxai/methods/innvestigate/tests/analyzer/test_gradient_based.py`

 * *Files identical despite different names*

### Comparing `signxai-1.0.1/signxai/methods/innvestigate/tests/analyzer/test_deeptaylor.py` & `signxai-1.1.0/signxai/methods/innvestigate/tests/analyzer/test_deeptaylor.py`

 * *Files identical despite different names*

### Comparing `signxai-1.0.1/signxai/methods/innvestigate/tests/analyzer/test_init.py` & `signxai-1.1.0/signxai/methods/innvestigate/tests/analyzer/test_init.py`

 * *Files identical despite different names*

### Comparing `signxai-1.0.1/signxai/methods/innvestigate/tests/utils/keras/test_graph.py` & `signxai-1.1.0/signxai/methods/innvestigate/tests/utils/keras/test_graph.py`

 * *Files identical despite different names*

### Comparing `signxai-1.0.1/signxai/methods/innvestigate/tests/utils/test_visualizations.py` & `signxai-1.1.0/signxai/methods/innvestigate/tests/utils/test_visualizations.py`

 * *Files identical despite different names*

### Comparing `signxai-1.0.1/signxai/methods/innvestigate/tests/utils/tests/test_dryrun.py` & `signxai-1.1.0/signxai/methods/innvestigate/tests/utils/tests/test_dryrun.py`

 * *Files identical despite different names*

### Comparing `signxai-1.0.1/signxai/methods/innvestigate/analyzer/pattern_based.py` & `signxai-1.1.0/signxai/methods/innvestigate/analyzer/pattern_based.py`

 * *Files identical despite different names*

### Comparing `signxai-1.0.1/signxai/methods/innvestigate/analyzer/misc.py` & `signxai-1.1.0/signxai/methods/innvestigate/analyzer/misc.py`

 * *Files identical despite different names*

### Comparing `signxai-1.0.1/signxai/methods/innvestigate/analyzer/gradient_based.py` & `signxai-1.1.0/signxai/methods/innvestigate/analyzer/gradient_based.py`

 * *Files identical despite different names*

### Comparing `signxai-1.0.1/signxai/methods/innvestigate/analyzer/deeptaylor.py` & `signxai-1.1.0/signxai/methods/innvestigate/analyzer/deeptaylor.py`

 * *Files identical despite different names*

### Comparing `signxai-1.0.1/signxai/methods/innvestigate/analyzer/wrapper.py` & `signxai-1.1.0/signxai/methods/innvestigate/analyzer/wrapper.py`

 * *Files identical despite different names*

### Comparing `signxai-1.0.1/signxai/methods/innvestigate/analyzer/reverse_map.py` & `signxai-1.1.0/signxai/methods/innvestigate/analyzer/reverse_map.py`

 * *Files identical despite different names*

### Comparing `signxai-1.0.1/signxai/methods/innvestigate/analyzer/base.py` & `signxai-1.1.0/signxai/methods/innvestigate/analyzer/base.py`

 * *Files identical despite different names*

### Comparing `signxai-1.0.1/signxai/methods/innvestigate/analyzer/__init__.py` & `signxai-1.1.0/signxai/methods/innvestigate/analyzer/__init__.py`

 * *Files identical despite different names*

### Comparing `signxai-1.0.1/signxai/methods/innvestigate/analyzer/deeplift.py` & `signxai-1.1.0/signxai/methods/innvestigate/analyzer/deeplift.py`

 * *Files identical despite different names*

### Comparing `signxai-1.0.1/signxai/methods/innvestigate/analyzer/relevance_based/utils.py` & `signxai-1.1.0/signxai/methods/innvestigate/analyzer/relevance_based/utils.py`

 * *Files identical despite different names*

### Comparing `signxai-1.0.1/signxai/methods/innvestigate/analyzer/relevance_based/relevance_analyzer.py` & `signxai-1.1.0/signxai/methods/innvestigate/analyzer/relevance_based/relevance_analyzer.py`

 * *Files identical despite different names*

### Comparing `signxai-1.0.1/signxai/methods/innvestigate/analyzer/relevance_based/relevance_rule_base.py` & `signxai-1.1.0/signxai/methods/innvestigate/analyzer/relevance_based/relevance_rule_base.py`

 * *Files identical despite different names*

### Comparing `signxai-1.0.1/signxai/methods/innvestigate/backend/__init__.py` & `signxai-1.1.0/signxai/methods/innvestigate/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `signxai-1.0.1/signxai/methods/innvestigate/utils/keras/backend.py` & `signxai-1.1.0/signxai/methods/innvestigate/utils/keras/backend.py`

 * *Files identical despite different names*

### Comparing `signxai-1.0.1/signxai/methods/innvestigate/utils/keras/__init__.py` & `signxai-1.1.0/signxai/methods/innvestigate/utils/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `signxai-1.0.1/signxai/methods/innvestigate/utils/keras/graph.py` & `signxai-1.1.0/signxai/methods/innvestigate/utils/keras/graph.py`

 * *Files identical despite different names*

### Comparing `signxai-1.0.1/signxai/methods/innvestigate/utils/visualizations.py` & `signxai-1.1.0/signxai/methods/innvestigate/utils/visualizations.py`

 * *Files identical despite different names*

### Comparing `signxai-1.0.1/signxai/methods/innvestigate/utils/tests/dryrun.py` & `signxai-1.1.0/signxai/methods/innvestigate/utils/tests/dryrun.py`

 * *Files identical despite different names*

### Comparing `signxai-1.0.1/signxai/methods/innvestigate/utils/tests/cases/mlp.py` & `signxai-1.1.0/signxai/methods/innvestigate/utils/tests/cases/mlp.py`

 * *Files identical despite different names*

### Comparing `signxai-1.0.1/signxai/methods/innvestigate/utils/tests/cases/special.py` & `signxai-1.1.0/signxai/methods/innvestigate/utils/tests/cases/special.py`

 * *Files identical despite different names*

### Comparing `signxai-1.0.1/signxai/methods/innvestigate/utils/tests/cases/helper.py` & `signxai-1.1.0/signxai/methods/innvestigate/utils/tests/cases/helper.py`

 * *Files identical despite different names*

### Comparing `signxai-1.0.1/signxai/methods/innvestigate/utils/tests/cases/cnn.py` & `signxai-1.1.0/signxai/methods/innvestigate/utils/tests/cases/cnn.py`

 * *Files identical despite different names*

### Comparing `signxai-1.0.1/signxai/methods/innvestigate/utils/tests/cases/__init__.py` & `signxai-1.1.0/signxai/methods/innvestigate/utils/tests/cases/__init__.py`

 * *Files identical despite different names*

### Comparing `signxai-1.0.1/signxai/methods/innvestigate/utils/tests/cases/trivia.py` & `signxai-1.1.0/signxai/methods/innvestigate/utils/tests/cases/trivia.py`

 * *Files identical despite different names*

### Comparing `signxai-1.0.1/signxai/methods/innvestigate/utils/__init__.py` & `signxai-1.1.0/signxai/methods/innvestigate/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `signxai-1.0.1/signxai/methods/grad_cam.py` & `signxai-1.1.0/signxai/methods/grad_cam.py`

 * *Files identical despite different names*

### Comparing `signxai-1.0.1/signxai/methods/wrappers.py` & `signxai-1.1.0/signxai/methods/wrappers.py`

 * *Files identical despite different names*

### Comparing `signxai-1.0.1/signxai/methods/guided_backprop.py` & `signxai-1.1.0/signxai/methods/guided_backprop.py`

 * *Files identical despite different names*

### Comparing `signxai-1.0.1/signxai/utils/utils.py` & `signxai-1.1.0/signxai/utils/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,14 +52,19 @@
 
 
 def download_image(path):
     r = requests.get("https://raw.githubusercontent.com/nilsgumpfer/SIGN-XAI/main/signxai/examples/7867854122_b26957e9e3_o.jpg")
     with open(path, 'wb') as f:
         f.write(r.content)
 
+def download_model(path):
+    r = requests.get("https://github.com/nilsgumpfer/SIGN-XAI/raw/main/signxai/examples/DENSEMNIST10INV.h5")
+    with open(path, 'wb') as f:
+        f.write(r.content)
+
 
 def aggregate_and_normalize_relevancemap_rgb(R):
     # Aggregate along color channels and normalize to [-1, 1]
     a = R.sum(axis=2)
     a = normalize_heatmap(a)
 
     return a
```

### Comparing `signxai-1.0.1/signxai.egg-info/SOURCES.txt` & `signxai-1.1.0/signxai.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 setup.py
 signxai.egg-info/PKG-INFO
 signxai.egg-info/SOURCES.txt
 signxai.egg-info/dependency_links.txt
 signxai.egg-info/requires.txt
 signxai.egg-info/top_level.txt
 signxai/examples/__init__.py
+signxai/examples/mnist.py
 signxai/examples/vgg16.py
 signxai/methods/__init__.py
 signxai/methods/grad_cam.py
 signxai/methods/guided_backprop.py
 signxai/methods/signed.py
 signxai/methods/wrappers.py
 signxai/methods/innvestigate/__init__.py
```

### Comparing `signxai-1.0.1/setup.py` & `signxai-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(
     name='signxai',
-    version='1.0.1',
+    version='1.1.0',
     packages=['signxai.methods', 'signxai.methods.innvestigate', 'signxai.methods.innvestigate.tests', 'signxai.methods.innvestigate.tests.tools',
               'signxai.methods.innvestigate.tests.utils', 'signxai.methods.innvestigate.tests.utils.keras',
               'signxai.methods.innvestigate.tests.utils.tests', 'signxai.methods.innvestigate.tests.analyzer',
               'signxai.methods.innvestigate.tools', 'signxai.methods.innvestigate.utils', 'signxai.methods.innvestigate.utils.keras',
               'signxai.methods.innvestigate.utils.tests', 'signxai.methods.innvestigate.utils.tests.cases',
               'signxai.methods.innvestigate.backend', 'signxai.methods.innvestigate.analyzer',
               'signxai.methods.innvestigate.analyzer.canonization', 'signxai.methods.innvestigate.analyzer.relevance_based',
@@ -29,10 +29,10 @@
         'Operating System :: OS Independent',
         'License :: OSI Approved :: BSD License',
         'Development Status :: 5 - Production/Stable',
         'Environment :: Console',
         'Intended Audience :: Science/Research',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
     ],
-    install_requires=['tensorflow>=2.2.0', 'matplotlib>=3.3.4', 'requests>=2.27.1'],
+    install_requires=['tensorflow>=2.2.0', 'matplotlib>=3.3.4', 'requests>=2.27.1', 'version-parser>=1.0.1'],
     include_package_data=True,
 )
```

### Comparing `signxai-1.0.1/LICENSE` & `signxai-1.1.0/LICENSE`

 * *Files identical despite different names*

