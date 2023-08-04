# Comparing `tmp/ml-starter-0.1.45.tar.gz` & `tmp/ml-starter-0.1.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-starter-0.1.45.tar", last modified: Wed Aug  2 19:28:08 2023, max compression
+gzip compressed data, was "ml-starter-0.1.46.tar", last modified: Fri Aug  4 04:33:32 2023, max compression
```

## Comparing `ml-starter-0.1.45.tar` & `ml-starter-0.1.46.tar`

### file list

```diff
@@ -1,190 +1,190 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:28:08.282239 ml-starter-0.1.45/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-02 19:27:54.000000 ml-starter-0.1.45/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-08-02 19:27:54.000000 ml-starter-0.1.45/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-08-02 19:28:08.282239 ml-starter-0.1.45/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-08-02 19:27:54.000000 ml-starter-0.1.45/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:28:08.262239 ml-starter-0.1.45/ml/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11683 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:28:08.262239 ml-starter-0.1.45/ml/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/core/common_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/core/env.py
--rw-r--r--   0 runner    (1001) docker     (123)    26830 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/core/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/core/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:28:08.262239 ml-starter-0.1.45/ml/launchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/launchers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/launchers/mp.py
--rw-r--r--   0 runner    (1001) docker     (123)     9584 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/launchers/sagemaker.py
--rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/launchers/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/launchers/torchrun.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:28:08.262239 ml-starter-0.1.45/ml/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/loggers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/loggers/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)    46173 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/loggers/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/loggers/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)    14894 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/loggers/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:28:08.266239 ml-starter-0.1.45/ml/lr_schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/lr_schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/lr_schedulers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/lr_schedulers/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/lr_schedulers/cosine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/lr_schedulers/cosine_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/lr_schedulers/gan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/lr_schedulers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/lr_schedulers/linear_no_decay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:28:08.266239 ml-starter-0.1.45/ml/lr_schedulers/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/lr_schedulers/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/lr_schedulers/scripts/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:28:08.266239 ml-starter-0.1.45/ml/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/models/activations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:28:08.266239 ml-starter-0.1.45/ml/models/architectures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/models/architectures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/models/architectures/bifpn.py
--rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/models/architectures/unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    17536 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/models/codebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/models/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/models/gan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/models/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/models/kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)    56335 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/models/lora.py
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/models/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/models/norms.py
--rw-r--r--   0 runner    (1001) docker     (123)    16373 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/models/parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:28:08.270239 ml-starter-0.1.45/ml/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/optimizers/adan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/optimizers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/optimizers/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/optimizers/gan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/optimizers/lion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/optimizers/sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/optimizers/shampoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/optimizers/types.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:28:08.270239 ml-starter-0.1.45/ml/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/scripts/launch.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/scripts/resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/scripts/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/scripts/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:28:08.270239 ml-starter-0.1.45/ml/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19167 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/tasks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:28:08.270239 ml-starter-0.1.45/ml/tasks/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/tasks/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/tasks/datasets/async_iterable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/tasks/datasets/clippify.py
--rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/tasks/datasets/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/tasks/datasets/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/tasks/datasets/multi_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/tasks/datasets/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/tasks/datasets/streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/tasks/datasets/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/tasks/datasets/video_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:28:08.270239 ml-starter-0.1.45/ml/tasks/diffusion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/tasks/diffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/tasks/diffusion/beta_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)    10070 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/tasks/diffusion/gaussian.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:28:08.270239 ml-starter-0.1.45/ml/tasks/environments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/tasks/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/tasks/environments/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/tasks/environments/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/tasks/environments/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:28:08.270239 ml-starter-0.1.45/ml/tasks/gan/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/tasks/gan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/tasks/gan/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:28:08.274239 ml-starter-0.1.45/ml/tasks/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/tasks/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6136 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/tasks/losses/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)    10058 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/tasks/losses/image.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/tasks/losses/kl.py
--rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/tasks/losses/loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:28:08.274239 ml-starter-0.1.45/ml/tasks/rl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/tasks/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18539 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/tasks/rl/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/tasks/rl/replay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:28:08.274239 ml-starter-0.1.45/ml/tasks/sl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/tasks/sl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/tasks/sl/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:28:08.274239 ml-starter-0.1.45/ml/trainers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27997 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/trainers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11061 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/trainers/gan.py
--rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/trainers/learning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:28:08.274239 ml-starter-0.1.45/ml/trainers/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/trainers/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/trainers/mixins/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9388 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/trainers/mixins/cpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/trainers/mixins/data_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8968 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/trainers/mixins/gpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/trainers/mixins/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     7007 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/trainers/mixins/mixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/trainers/mixins/monitor_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/trainers/mixins/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/trainers/mixins/step_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/trainers/rl.py
--rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/trainers/sl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:28:08.278239 ml-starter-0.1.45/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/amp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/atomic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    38804 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     8942 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:28:08.278239 ml-starter-0.1.45/ml/utils/device/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/device/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/device/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/device/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/device/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/device/metal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/large_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/mixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/networking.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11253 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)    16064 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/spectrogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/staging.py
--rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13431 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     8077 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/torch_distributed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:28:08.282239 ml-starter-0.1.45/ml/utils/triton/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/triton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/triton/kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/triton/lion.py
--rw-r--r--   0 runner    (1001) docker     (123)    21038 2023-08-02 19:27:54.000000 ml-starter-0.1.45/ml/utils/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:28:08.282239 ml-starter-0.1.45/ml_starter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-08-02 19:28:08.000000 ml-starter-0.1.45/ml_starter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-08-02 19:28:08.000000 ml-starter-0.1.45/ml_starter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 19:28:08.000000 ml-starter-0.1.45/ml_starter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-08-02 19:28:08.000000 ml-starter-0.1.45/ml_starter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-08-02 19:28:08.000000 ml-starter-0.1.45/ml_starter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-08-02 19:27:54.000000 ml-starter-0.1.45/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-02 19:28:08.282239 ml-starter-0.1.45/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-08-02 19:27:54.000000 ml-starter-0.1.45/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 04:33:32.397548 ml-starter-0.1.46/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-04 04:33:19.000000 ml-starter-0.1.46/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-08-04 04:33:19.000000 ml-starter-0.1.46/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-08-04 04:33:32.397548 ml-starter-0.1.46/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-08-04 04:33:19.000000 ml-starter-0.1.46/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 04:33:32.373548 ml-starter-0.1.46/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11683 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 04:33:32.373548 ml-starter-0.1.46/ml/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/core/common_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/core/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26830 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/core/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 04:33:32.373548 ml-starter-0.1.46/ml/launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/launchers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/launchers/mp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9584 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/launchers/sagemaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/launchers/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/launchers/torchrun.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 04:33:32.373548 ml-starter-0.1.46/ml/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/loggers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/loggers/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46173 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/loggers/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/loggers/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14894 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/loggers/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 04:33:32.377548 ml-starter-0.1.46/ml/lr_schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/lr_schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/lr_schedulers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/lr_schedulers/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/lr_schedulers/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/lr_schedulers/cosine_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/lr_schedulers/gan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/lr_schedulers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/lr_schedulers/linear_no_decay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 04:33:32.377548 ml-starter-0.1.46/ml/lr_schedulers/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/lr_schedulers/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/lr_schedulers/scripts/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 04:33:32.377548 ml-starter-0.1.46/ml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/models/activations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 04:33:32.377548 ml-starter-0.1.46/ml/models/architectures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/models/architectures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/models/architectures/bifpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/models/architectures/unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17536 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/models/codebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/models/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/models/gan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/models/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/models/kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56335 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/models/lora.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/models/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/models/norms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16373 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/models/parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 04:33:32.381548 ml-starter-0.1.46/ml/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/optimizers/adan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/optimizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/optimizers/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/optimizers/gan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/optimizers/lion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/optimizers/sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/optimizers/shampoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/optimizers/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 04:33:32.381548 ml-starter-0.1.46/ml/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/scripts/launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/scripts/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/scripts/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/scripts/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 04:33:32.381548 ml-starter-0.1.46/ml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19167 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/tasks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 04:33:32.381548 ml-starter-0.1.46/ml/tasks/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/tasks/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/tasks/datasets/async_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/tasks/datasets/clippify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/tasks/datasets/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/tasks/datasets/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/tasks/datasets/multi_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/tasks/datasets/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/tasks/datasets/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/tasks/datasets/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/tasks/datasets/video_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 04:33:32.385548 ml-starter-0.1.46/ml/tasks/diffusion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/tasks/diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/tasks/diffusion/beta_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10070 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/tasks/diffusion/gaussian.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 04:33:32.385548 ml-starter-0.1.46/ml/tasks/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/tasks/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/tasks/environments/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/tasks/environments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/tasks/environments/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 04:33:32.385548 ml-starter-0.1.46/ml/tasks/gan/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/tasks/gan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/tasks/gan/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 04:33:32.385548 ml-starter-0.1.46/ml/tasks/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/tasks/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6136 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/tasks/losses/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10058 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/tasks/losses/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/tasks/losses/kl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/tasks/losses/loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 04:33:32.385548 ml-starter-0.1.46/ml/tasks/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/tasks/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18539 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/tasks/rl/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/tasks/rl/replay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 04:33:32.385548 ml-starter-0.1.46/ml/tasks/sl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/tasks/sl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/tasks/sl/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 04:33:32.385548 ml-starter-0.1.46/ml/trainers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27533 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/trainers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11061 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/trainers/gan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/trainers/learning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 04:33:32.389548 ml-starter-0.1.46/ml/trainers/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/trainers/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/trainers/mixins/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9388 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/trainers/mixins/cpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/trainers/mixins/data_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8968 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/trainers/mixins/gpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/trainers/mixins/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7007 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/trainers/mixins/mixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/trainers/mixins/monitor_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/trainers/mixins/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/trainers/mixins/step_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/trainers/rl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/trainers/sl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 04:33:32.393548 ml-starter-0.1.46/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/utils/amp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/utils/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/utils/atomic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/utils/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38804 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/utils/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/utils/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/utils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8942 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/utils/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/utils/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/utils/datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 04:33:32.393548 ml-starter-0.1.46/ml/utils/device/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/utils/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/utils/device/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/utils/device/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/utils/device/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/utils/device/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/utils/device/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/utils/large_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/utils/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/utils/mixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/utils/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/utils/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11253 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/utils/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16064 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/utils/spectrogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/utils/staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/utils/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13431 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/utils/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8438 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/utils/torch_distributed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 04:33:32.393548 ml-starter-0.1.46/ml/utils/triton/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/utils/triton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/utils/triton/kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/utils/triton/lion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21038 2023-08-04 04:33:19.000000 ml-starter-0.1.46/ml/utils/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 04:33:32.397548 ml-starter-0.1.46/ml_starter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-08-04 04:33:32.000000 ml-starter-0.1.46/ml_starter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-08-04 04:33:32.000000 ml-starter-0.1.46/ml_starter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 04:33:32.000000 ml-starter-0.1.46/ml_starter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-08-04 04:33:32.000000 ml-starter-0.1.46/ml_starter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-08-04 04:33:32.000000 ml-starter-0.1.46/ml_starter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-08-04 04:33:19.000000 ml-starter-0.1.46/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-04 04:33:32.397548 ml-starter-0.1.46/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-08-04 04:33:19.000000 ml-starter-0.1.46/setup.py
```

### Comparing `ml-starter-0.1.45/LICENSE` & `ml-starter-0.1.46/LICENSE`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/PKG-INFO` & `ml-starter-0.1.46/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.1.45
+Version: 0.1.46
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.1.45/README.md` & `ml-starter-0.1.46/README.md`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/api.py` & `ml-starter-0.1.46/ml/api.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/core/common_types.py` & `ml-starter-0.1.46/ml/core/common_types.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/core/config.py` & `ml-starter-0.1.46/ml/core/config.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/core/env.py` & `ml-starter-0.1.46/ml/core/env.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/core/registry.py` & `ml-starter-0.1.46/ml/core/registry.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/core/state.py` & `ml-starter-0.1.46/ml/core/state.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/launchers/base.py` & `ml-starter-0.1.46/ml/launchers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/launchers/mp.py` & `ml-starter-0.1.46/ml/launchers/mp.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/launchers/sagemaker.py` & `ml-starter-0.1.46/ml/launchers/sagemaker.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/launchers/slurm.py` & `ml-starter-0.1.46/ml/launchers/slurm.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/launchers/torchrun.py` & `ml-starter-0.1.46/ml/launchers/torchrun.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/loggers/base.py` & `ml-starter-0.1.46/ml/loggers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/loggers/meter.py` & `ml-starter-0.1.46/ml/loggers/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/loggers/multi.py` & `ml-starter-0.1.46/ml/loggers/multi.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/loggers/stdout.py` & `ml-starter-0.1.46/ml/loggers/stdout.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/loggers/tensorboard.py` & `ml-starter-0.1.46/ml/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/lr_schedulers/base.py` & `ml-starter-0.1.46/ml/lr_schedulers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/lr_schedulers/constant.py` & `ml-starter-0.1.46/ml/lr_schedulers/constant.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/lr_schedulers/cosine.py` & `ml-starter-0.1.46/ml/lr_schedulers/cosine.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/lr_schedulers/cosine_decay.py` & `ml-starter-0.1.46/ml/lr_schedulers/cosine_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/lr_schedulers/gan.py` & `ml-starter-0.1.46/ml/lr_schedulers/gan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/lr_schedulers/linear.py` & `ml-starter-0.1.46/ml/lr_schedulers/linear.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/lr_schedulers/linear_no_decay.py` & `ml-starter-0.1.46/ml/lr_schedulers/linear_no_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/lr_schedulers/scripts/plot.py` & `ml-starter-0.1.46/ml/lr_schedulers/scripts/plot.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/models/activations.py` & `ml-starter-0.1.46/ml/models/activations.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/models/architectures/bifpn.py` & `ml-starter-0.1.46/ml/models/architectures/bifpn.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/models/architectures/unet.py` & `ml-starter-0.1.46/ml/models/architectures/unet.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/models/base.py` & `ml-starter-0.1.46/ml/models/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/models/codebook.py` & `ml-starter-0.1.46/ml/models/codebook.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/models/embeddings.py` & `ml-starter-0.1.46/ml/models/embeddings.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/models/gan.py` & `ml-starter-0.1.46/ml/models/gan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/models/init.py` & `ml-starter-0.1.46/ml/models/init.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/models/kmeans.py` & `ml-starter-0.1.46/ml/models/kmeans.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/models/lora.py` & `ml-starter-0.1.46/ml/models/lora.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/models/modules.py` & `ml-starter-0.1.46/ml/models/modules.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/models/norms.py` & `ml-starter-0.1.46/ml/models/norms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/models/parallel.py` & `ml-starter-0.1.46/ml/models/parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/optimizers/adam.py` & `ml-starter-0.1.46/ml/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/optimizers/adan.py` & `ml-starter-0.1.46/ml/optimizers/adan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/optimizers/base.py` & `ml-starter-0.1.46/ml/optimizers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/optimizers/common.py` & `ml-starter-0.1.46/ml/optimizers/common.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/optimizers/gan.py` & `ml-starter-0.1.46/ml/optimizers/gan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/optimizers/lion.py` & `ml-starter-0.1.46/ml/optimizers/lion.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/optimizers/sgd.py` & `ml-starter-0.1.46/ml/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/optimizers/shampoo.py` & `ml-starter-0.1.46/ml/optimizers/shampoo.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/scripts/cli.py` & `ml-starter-0.1.46/ml/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/scripts/stage.py` & `ml-starter-0.1.46/ml/scripts/stage.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/scripts/train.py` & `ml-starter-0.1.46/ml/scripts/train.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/tasks/base.py` & `ml-starter-0.1.46/ml/tasks/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/tasks/datasets/async_iterable.py` & `ml-starter-0.1.46/ml/tasks/datasets/async_iterable.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/tasks/datasets/clippify.py` & `ml-starter-0.1.46/ml/tasks/datasets/clippify.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/tasks/datasets/collate.py` & `ml-starter-0.1.46/ml/tasks/datasets/collate.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/tasks/datasets/error_handling.py` & `ml-starter-0.1.46/ml/tasks/datasets/error_handling.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/tasks/datasets/multi_iter.py` & `ml-starter-0.1.46/ml/tasks/datasets/multi_iter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/tasks/datasets/samplers.py` & `ml-starter-0.1.46/ml/tasks/datasets/samplers.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/tasks/datasets/streaming.py` & `ml-starter-0.1.46/ml/tasks/datasets/streaming.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/tasks/datasets/transforms.py` & `ml-starter-0.1.46/ml/tasks/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/tasks/datasets/video_file.py` & `ml-starter-0.1.46/ml/tasks/datasets/video_file.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/tasks/diffusion/beta_schedule.py` & `ml-starter-0.1.46/ml/tasks/diffusion/beta_schedule.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/tasks/diffusion/gaussian.py` & `ml-starter-0.1.46/ml/tasks/diffusion/gaussian.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/tasks/environments/base.py` & `ml-starter-0.1.46/ml/tasks/environments/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/tasks/environments/utils.py` & `ml-starter-0.1.46/ml/tasks/environments/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/tasks/environments/worker.py` & `ml-starter-0.1.46/ml/tasks/environments/worker.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/tasks/gan/base.py` & `ml-starter-0.1.46/ml/tasks/gan/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/tasks/losses/audio.py` & `ml-starter-0.1.46/ml/tasks/losses/audio.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/tasks/losses/image.py` & `ml-starter-0.1.46/ml/tasks/losses/image.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/tasks/losses/kl.py` & `ml-starter-0.1.46/ml/tasks/losses/kl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/tasks/losses/loss.py` & `ml-starter-0.1.46/ml/tasks/losses/loss.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/tasks/rl/base.py` & `ml-starter-0.1.46/ml/tasks/rl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/tasks/rl/replay.py` & `ml-starter-0.1.46/ml/tasks/rl/replay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/tasks/sl/base.py` & `ml-starter-0.1.46/ml/tasks/sl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/trainers/base.py` & `ml-starter-0.1.46/ml/trainers/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from pathlib import Path
 from typing import Any, Callable, Generic, Literal, TypeVar, cast, get_args
 
 import safetensors
 import torch
 from omegaconf import II, MISSING, DictConfig, ListConfig, OmegaConf
 from safetensors.torch import _remove_duplicate_names, save_file as safetensors_save_file
-from torch import Tensor, nn
+from torch import Tensor
 from torch.optim.optimizer import Optimizer
 
 from ml.core.config import BaseConfig, BaseObject, conf_field
 from ml.core.env import get_ml_config_path
 from ml.core.state import State
 from ml.loggers.base import BaseLogger
 from ml.loggers.multi import MultiLogger
@@ -220,15 +220,14 @@
 
 @dataclass
 class CheckpointConfig:
     save_every_n_steps: int | None = conf_field(None, help="Save a checkpoint every N steps")
     save_every_n_seconds: int | None = conf_field(None, help="Save a checkpoint every N seconds")
     only_save_most_recent: bool = conf_field(False, help="Only keep the most recent checkpoint")
     load_from_ckpt_path: str | None = conf_field(None, help="If set, load initial model weights from this path")
-    save_no_grad: bool = conf_field(False, help="If set, also save tensors which don't require gradients")
     load_strict: bool = conf_field(True, help="If set, only load weights for which have a matching key in the model")
 
 
 @dataclass
 class BaseTrainerConfig(BaseConfig):
     """Defines the base config for all trainers."""
 
@@ -482,26 +481,21 @@
                     for k, v in d.items():
                         if isinstance(v, dict):
                             return_dict.update({f"{k}.{k2}": v2 for k2, v2 in get_flat_dict(v).items()})
                         else:
                             return_dict[k] = v
                     return return_dict
 
-                def get_state_dict(module: nn.Module, prefix: str) -> dict[str, Any]:
-                    parameters = module.named_parameters(prefix=prefix, recurse=True, remove_duplicate=True)
-                    save_no_grad = self.config.checkpoint.save_no_grad
-                    return {k: v for k, v in parameters if save_no_grad or v.requires_grad}
-
                 def add_state_dict(key: str, sd: dict[str, Any]) -> None:
                     sd = get_flat_dict(sd)
                     state_dict.update({k: v for k, v in sd.items() if isinstance(v, Tensor)})
                     metadata[key] = json.dumps({k: v for k, v in sd.items() if not isinstance(v, Tensor)})
 
-                add_state_dict("model", get_state_dict(model, "model"))
-                add_state_dict("task", get_state_dict(task, "task"))
+                add_state_dict("model", model.state_dict(prefix="model."))
+                add_state_dict("task", task.state_dict(prefix="task."))
 
                 metadata["state"] = json.dumps(asdict(state))
 
                 if optims is not None:
                     if isinstance(optims, dict):
                         osd = {f"optim.{k}.{kk}": vv for k, v in optims.items() for kk, vv in v.state_dict().items()}
                     else:
```

### Comparing `ml-starter-0.1.45/ml/trainers/gan.py` & `ml-starter-0.1.46/ml/trainers/gan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/trainers/learning.py` & `ml-starter-0.1.46/ml/trainers/learning.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/trainers/mixins/compile.py` & `ml-starter-0.1.46/ml/trainers/mixins/compile.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/trainers/mixins/cpu_stats.py` & `ml-starter-0.1.46/ml/trainers/mixins/cpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/trainers/mixins/data_parallel.py` & `ml-starter-0.1.46/ml/trainers/mixins/data_parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/trainers/mixins/gpu_stats.py` & `ml-starter-0.1.46/ml/trainers/mixins/gpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/trainers/mixins/heartbeat.py` & `ml-starter-0.1.46/ml/trainers/mixins/heartbeat.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/trainers/mixins/mixed_precision.py` & `ml-starter-0.1.46/ml/trainers/mixins/mixed_precision.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/trainers/mixins/monitor_process.py` & `ml-starter-0.1.46/ml/trainers/mixins/monitor_process.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/trainers/mixins/profiler.py` & `ml-starter-0.1.46/ml/trainers/mixins/profiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/trainers/mixins/step_wrapper.py` & `ml-starter-0.1.46/ml/trainers/mixins/step_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/trainers/rl.py` & `ml-starter-0.1.46/ml/trainers/rl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/trainers/sl.py` & `ml-starter-0.1.46/ml/trainers/sl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/utils/amp.py` & `ml-starter-0.1.46/ml/utils/amp.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/utils/argparse.py` & `ml-starter-0.1.46/ml/utils/argparse.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/utils/atomic.py` & `ml-starter-0.1.46/ml/utils/atomic.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/utils/attention.py` & `ml-starter-0.1.46/ml/utils/attention.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/utils/audio.py` & `ml-starter-0.1.46/ml/utils/audio.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/utils/augmentation.py` & `ml-starter-0.1.46/ml/utils/augmentation.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/utils/caching.py` & `ml-starter-0.1.46/ml/utils/caching.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/utils/checkpoint.py` & `ml-starter-0.1.46/ml/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/utils/cli.py` & `ml-starter-0.1.46/ml/utils/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/utils/colors.py` & `ml-starter-0.1.46/ml/utils/colors.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/utils/containers.py` & `ml-starter-0.1.46/ml/utils/containers.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/utils/data.py` & `ml-starter-0.1.46/ml/utils/data.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/utils/datetime.py` & `ml-starter-0.1.46/ml/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/utils/device/auto.py` & `ml-starter-0.1.46/ml/utils/device/auto.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/utils/device/base.py` & `ml-starter-0.1.46/ml/utils/device/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/utils/device/cpu.py` & `ml-starter-0.1.46/ml/utils/device/cpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/utils/device/gpu.py` & `ml-starter-0.1.46/ml/utils/device/gpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/utils/device/metal.py` & `ml-starter-0.1.46/ml/utils/device/metal.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/utils/distributed.py` & `ml-starter-0.1.46/ml/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/utils/exceptions.py` & `ml-starter-0.1.46/ml/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/utils/image.py` & `ml-starter-0.1.46/ml/utils/image.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/utils/io.py` & `ml-starter-0.1.46/ml/utils/io.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/utils/large_models.py` & `ml-starter-0.1.46/ml/utils/large_models.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/utils/logging.py` & `ml-starter-0.1.46/ml/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/utils/meter.py` & `ml-starter-0.1.46/ml/utils/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/utils/mixed_precision.py` & `ml-starter-0.1.46/ml/utils/mixed_precision.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/utils/networking.py` & `ml-starter-0.1.46/ml/utils/networking.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/utils/numpy.py` & `ml-starter-0.1.46/ml/utils/numpy.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/utils/parallel.py` & `ml-starter-0.1.46/ml/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/utils/spectrogram.py` & `ml-starter-0.1.46/ml/utils/spectrogram.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/utils/staging.py` & `ml-starter-0.1.46/ml/utils/staging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/utils/testing.py` & `ml-starter-0.1.46/ml/utils/testing.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/utils/timer.py` & `ml-starter-0.1.46/ml/utils/timer.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/utils/tokens.py` & `ml-starter-0.1.46/ml/utils/tokens.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/utils/torch_distributed.py` & `ml-starter-0.1.46/ml/utils/torch_distributed.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import functools
 import logging
 import os
 import sys
 import traceback
 from dataclasses import dataclass
-from typing import Callable
+from typing import Callable, ParamSpec
 
 import torch
 import torch.distributed
 import torch.distributed as dist
 import torch.multiprocessing as mp
 from omegaconf import MISSING
 
@@ -25,14 +25,16 @@
 from ml.utils.distributed import get_init_method, get_rank, get_world_size, set_dist
 from ml.utils.logging import INFOALL, configure_logging
 from ml.utils.networking import get_unused_port
 from ml.utils.parallel import init_parallelism
 
 logger: logging.Logger = logging.getLogger(__name__)
 
+P = ParamSpec("P")
+
 
 @dataclass
 class MultiprocessConfig:
     rank: int = conf_field(-1, help="The rank of the process")
     local_rank: int = conf_field(-1, help="The local rank of the process")
     world_size: int = conf_field(MISSING, help="The total number of processes")
     local_world_size: int = conf_field(MISSING, help="The number of processes per machine")
@@ -115,15 +117,20 @@
     return dist.Backend(os.environ.get("TORCH_DISTRIBUTED_BACKEND", default_backend()))
 
 
 def set_distributed_backend(backend: str) -> None:
     os.environ["TORCH_DISTRIBUTED_BACKEND"] = backend
 
 
-def init_and_run(func: Callable[[], None], cfg: MultiprocessConfig) -> None:
+def init_and_run(
+    func: Callable[P, None],
+    cfg: MultiprocessConfig,
+    *args: P.args,
+    **kwargs: P.kwargs,
+) -> None:
     configure_logging(rank=cfg.rank, world_size=cfg.world_size)
 
     init_dist(
         rank=cfg.rank,
         local_rank=cfg.local_rank,
         world_size=cfg.world_size,
         local_world_size=cfg.local_world_size,
@@ -137,52 +144,58 @@
         model_parallelism=cfg.model_parallelism,
         pipeline_parallelism=cfg.pipeline_parallelism,
         mp_backend=cfg.backend if cfg.model_parallel_backend is None else cfg.model_parallel_backend,
         pp_backend=cfg.backend if cfg.pipeline_parallel_backend is None else cfg.pipeline_parallel_backend,
         dp_backend=cfg.backend if cfg.data_parallel_backend is None else cfg.data_parallel_backend,
     )
 
-    func()
+    func(*args, **kwargs)
 
 
 def _func_wrapped(
-    func: Callable[[], None],
+    func: Callable[P, None],
     setup: Callable[[], None] | None,
     cfg: MultiprocessConfig,
     error_queue: "mp.SimpleQueue[str | None]",
+    *args: P.args,
+    **kwargs: P.kwargs,
 ) -> None:
     try:
         if setup is not None:
             setup()
 
-        init_and_run(func, cfg)
+        init_and_run(func, cfg, *args, **kwargs)
 
     except KeyboardInterrupt:
         logger.info("Caught KeyboardInterrupt; exiting")
 
     except Exception:
         error_queue.put(traceback.format_exc())
         sys.exit(1)
 
     error_queue.put(None)
 
 
 def launch_subprocesses(
-    func: Callable[[], None],
+    func: Callable[P, None],
     cfg: MultiprocessConfig,
     setup: Callable[[], None] | None = None,
     rank_offset: int = 0,
+    *args: P.args,
+    **kwargs: P.kwargs,
 ) -> None:
     """Launches a function in multiple subprocesses.
 
     Args:
         func: The function to launch.
         cfg: The configuration for the function.
+        args: The positional arguments to pass to the function.
         setup: A function to run before launching the subprocesses.
         rank_offset: The offset to add to the rank of each subprocess.
+        kwargs: The keyword arguments to pass to the function.
 
     Raises:
         RuntimeError: If the function fails in any subprocess.
     """
     MultiprocessConfig.resolve(cfg)
 
     if cfg.world_size <= 1:
@@ -198,15 +211,16 @@
     for rank in range(cfg.world_size):
         rank = rank + rank_offset
         error_queue = ctx.SimpleQueue()
         cfg.rank = rank
         cfg.local_rank = rank % cfg.local_world_size
         proc = ctx.Process(
             target=_func_wrapped,
-            args=(func, setup, cfg, error_queue),
+            args=[func, setup, cfg, error_queue, *args],
+            kwargs=kwargs,
             daemon=False,
             name=f"worker-{rank}",
         )
         logger.debug("Started process %d", rank)
         proc.start()
         error_queues.append(error_queue)
         procs.append(proc)
```

### Comparing `ml-starter-0.1.45/ml/utils/triton/kmeans.py` & `ml-starter-0.1.46/ml/utils/triton/kmeans.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/utils/triton/lion.py` & `ml-starter-0.1.46/ml/utils/triton/lion.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml/utils/video.py` & `ml-starter-0.1.46/ml/utils/video.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/ml_starter.egg-info/PKG-INFO` & `ml-starter-0.1.46/ml_starter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.1.45
+Version: 0.1.46
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.1.45/ml_starter.egg-info/SOURCES.txt` & `ml-starter-0.1.46/ml_starter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/pyproject.toml` & `ml-starter-0.1.46/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.45/setup.py` & `ml-starter-0.1.46/setup.py`

 * *Files identical despite different names*

