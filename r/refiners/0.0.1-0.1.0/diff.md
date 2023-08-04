# Comparing `tmp/refiners-0.0.1.tar.gz` & `tmp/refiners-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refiners-0.0.1.tar", max compression
+gzip compressed data, was "refiners-0.1.0.tar", max compression
```

## Comparing `refiners-0.0.1.tar` & `refiners-0.1.0.tar`

### file list

```diff
@@ -1,4 +1,51 @@
--rw-r--r--   0        0        0        0 2023-07-06 13:10:02.929637 refiners-0.0.1/README.md
--rw-r--r--   0        0        0      318 2023-07-06 14:27:52.483161 refiners-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-06 13:10:54.631536 refiners-0.0.1/src/refiners/__init__.py
--rw-r--r--   0        0        0      374 1970-01-01 00:00:00.000000 refiners-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-08-04 17:45:44.212771 refiners-0.1.0/LICENSE
+-rw-r--r--   0        0        0    11873 2023-08-04 17:45:44.212875 refiners-0.1.0/README.md
+-rw-r--r--   0        0        0     1763 2023-08-04 17:45:44.216974 refiners-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-04 17:45:44.217889 refiners-0.1.0/src/refiners/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-04 17:45:44.217962 refiners-0.1.0/src/refiners/adapters/__init__.py
+-rw-r--r--   0        0        0     2325 2023-08-04 17:45:44.218031 refiners-0.1.0/src/refiners/adapters/adapter.py
+-rw-r--r--   0        0        0     3078 2023-08-04 17:45:44.218093 refiners-0.1.0/src/refiners/adapters/lora.py
+-rw-r--r--   0        0        0     2651 2023-08-04 17:45:44.218162 refiners-0.1.0/src/refiners/adapters/range_adapter.py
+-rw-r--r--   0        0        0      192 2023-08-04 17:45:44.218258 refiners-0.1.0/src/refiners/fluxion/__init__.py
+-rw-r--r--   0        0        0     1752 2023-08-04 17:45:44.218320 refiners-0.1.0/src/refiners/fluxion/context.py
+-rw-r--r--   0        0        0     1720 2023-08-04 17:45:44.218420 refiners-0.1.0/src/refiners/fluxion/layers/__init__.py
+-rw-r--r--   0        0        0     1660 2023-08-04 17:45:44.218486 refiners-0.1.0/src/refiners/fluxion/layers/activations.py
+-rw-r--r--   0        0        0     7063 2023-08-04 17:45:44.218558 refiners-0.1.0/src/refiners/fluxion/layers/attentions.py
+-rw-r--r--   0        0        0     5354 2023-08-04 17:45:44.218625 refiners-0.1.0/src/refiners/fluxion/layers/basics.py
+-rw-r--r--   0        0        0    16591 2023-08-04 17:45:44.218743 refiners-0.1.0/src/refiners/fluxion/layers/chain.py
+-rw-r--r--   0        0        0     2205 2023-08-04 17:45:44.218824 refiners-0.1.0/src/refiners/fluxion/layers/conv.py
+-rw-r--r--   0        0        0      748 2023-08-04 17:45:44.218900 refiners-0.1.0/src/refiners/fluxion/layers/embedding.py
+-rw-r--r--   0        0        0     1579 2023-08-04 17:45:44.218966 refiners-0.1.0/src/refiners/fluxion/layers/linear.py
+-rw-r--r--   0        0        0     3581 2023-08-04 17:45:44.219046 refiners-0.1.0/src/refiners/fluxion/layers/module.py
+-rw-r--r--   0        0        0     2415 2023-08-04 17:45:44.219122 refiners-0.1.0/src/refiners/fluxion/layers/norm.py
+-rw-r--r--   0        0        0     3460 2023-08-04 17:45:44.219191 refiners-0.1.0/src/refiners/fluxion/layers/sampling.py
+-rw-r--r--   0        0        0     9024 2023-08-04 17:45:44.219284 refiners-0.1.0/src/refiners/fluxion/utils.py
+-rw-r--r--   0        0        0        0 2023-08-04 17:45:44.219358 refiners-0.1.0/src/refiners/foundationals/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-04 17:45:44.219440 refiners-0.1.0/src/refiners/foundationals/clip/__init__.py
+-rw-r--r--   0        0        0  1356917 2023-08-04 17:45:44.220400 refiners-0.1.0/src/refiners/foundationals/clip/bpe_simple_vocab_16e6.txt.gz
+-rw-r--r--   0        0        0        0 2023-08-04 17:45:44.220808 refiners-0.1.0/src/refiners/foundationals/clip/image_encoder.py
+-rw-r--r--   0        0        0     7831 2023-08-04 17:45:44.220913 refiners-0.1.0/src/refiners/foundationals/clip/text_encoder.py
+-rw-r--r--   0        0        0     4649 2023-08-04 17:45:44.220991 refiners-0.1.0/src/refiners/foundationals/clip/tokenizer.py
+-rw-r--r--   0        0        0     7436 2023-08-04 17:45:44.221115 refiners-0.1.0/src/refiners/foundationals/latent_diffusion/__init__.py
+-rw-r--r--   0        0        0     8134 2023-08-04 17:45:44.221188 refiners-0.1.0/src/refiners/foundationals/latent_diffusion/auto_encoder.py
+-rw-r--r--   0        0        0     5768 2023-08-04 17:45:44.221268 refiners-0.1.0/src/refiners/foundationals/latent_diffusion/controlnet.py
+-rw-r--r--   0        0        0     7076 2023-08-04 17:45:44.221346 refiners-0.1.0/src/refiners/foundationals/latent_diffusion/cross_attention.py
+-rw-r--r--   0        0        0     4175 2023-08-04 17:45:44.221421 refiners-0.1.0/src/refiners/foundationals/latent_diffusion/lora.py
+-rw-r--r--   0        0        0      386 2023-08-04 17:45:44.221524 refiners-0.1.0/src/refiners/foundationals/latent_diffusion/schedulers/__init__.py
+-rw-r--r--   0        0        0     1806 2023-08-04 17:45:44.221609 refiners-0.1.0/src/refiners/foundationals/latent_diffusion/schedulers/ddim.py
+-rw-r--r--   0        0        0     4011 2023-08-04 17:45:44.221672 refiners-0.1.0/src/refiners/foundationals/latent_diffusion/schedulers/ddpm.py
+-rw-r--r--   0        0        0     4795 2023-08-04 17:45:44.221747 refiners-0.1.0/src/refiners/foundationals/latent_diffusion/schedulers/dpm_solver.py
+-rw-r--r--   0        0        0     3606 2023-08-04 17:45:44.221811 refiners-0.1.0/src/refiners/foundationals/latent_diffusion/schedulers/scheduler.py
+-rw-r--r--   0        0        0    11760 2023-08-04 17:45:44.221888 refiners-0.1.0/src/refiners/foundationals/latent_diffusion/sdxl_unet.py
+-rw-r--r--   0        0        0     4749 2023-08-04 17:45:44.221967 refiners-0.1.0/src/refiners/foundationals/latent_diffusion/self_attention_injection.py
+-rw-r--r--   0        0        0    11803 2023-08-04 17:45:44.222072 refiners-0.1.0/src/refiners/foundationals/latent_diffusion/unet.py
+-rw-r--r--   0        0        0        0 2023-08-04 17:45:44.222101 refiners-0.1.0/src/refiners/py.typed
+-rw-r--r--   0        0        0      548 2023-08-04 17:45:44.222207 refiners-0.1.0/src/refiners/training_utils/__init__.py
+-rw-r--r--   0        0        0     6644 2023-08-04 17:45:44.222277 refiners-0.1.0/src/refiners/training_utils/callback.py
+-rw-r--r--   0        0        0     7879 2023-08-04 17:45:44.222359 refiners-0.1.0/src/refiners/training_utils/config.py
+-rw-r--r--   0        0        0     7914 2023-08-04 17:45:44.222442 refiners-0.1.0/src/refiners/training_utils/dropout.py
+-rw-r--r--   0        0        0      788 2023-08-04 17:45:44.222500 refiners-0.1.0/src/refiners/training_utils/huggingface_datasets.py
+-rw-r--r--   0        0        0    10770 2023-08-04 17:45:44.222582 refiners-0.1.0/src/refiners/training_utils/latent_diffusion.py
+-rw-r--r--   0        0        0    21680 2023-08-04 17:45:44.222707 refiners-0.1.0/src/refiners/training_utils/trainer.py
+-rw-r--r--   0        0        0     1892 2023-08-04 17:45:44.222781 refiners-0.1.0/src/refiners/training_utils/wandb.py
+-rw-r--r--   0        0        0    13083 1970-01-01 00:00:00.000000 refiners-0.1.0/PKG-INFO
```

