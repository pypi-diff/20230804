# Comparing `tmp/dingo-gw-0.5.3.tar.gz` & `tmp/dingo-gw-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dingo-gw-0.5.3.tar", last modified: Wed May 10 16:03:24 2023, max compression
+gzip compressed data, was "dingo-gw-0.5.4.tar", last modified: Fri Aug  4 16:00:34 2023, max compression
```

## Comparing `dingo-gw-0.5.3.tar` & `dingo-gw-0.5.4.tar`

### file list

```diff
@@ -1,230 +1,230 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:03:24.399811 dingo-gw-0.5.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:03:24.351811 dingo-gw-0.5.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:03:24.359811 dingo-gw-0.5.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-05-10 16:03:24.399811 dingo-gw-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:03:24.359811 dingo-gw-0.5.3/compatibility/
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/compatibility/remove_domain_window_factor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/compatibility/update_model_input_dims.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/compatibility/update_model_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/compatibility/update_saved_model_for_train_stages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/compatibility/update_saved_model_gnpe_context_names.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/compatibility/update_saved_model_new_gnpe.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/compatibility/update_saved_model_new_truncation.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/compatibility/update_waveform_dataset_svd_refactor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:03:24.359811 dingo-gw-0.5.3/dingo/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-10 16:03:24.000000 dingo-gw-0.5.3/dingo/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:03:24.363811 dingo-gw-0.5.3/dingo/asimov/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/asimov/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10315 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/asimov/asimov.py
--rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/asimov/dingo.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:03:24.363811 dingo-gw-0.5.3/dingo/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/core/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:03:24.363811 dingo-gw-0.5.3/dingo/core/density/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/core/density/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/core/density/interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/core/density/nde_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/core/density/unconditional_density_estimation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/core/likelihood.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:03:24.363811 dingo-gw-0.5.3/dingo/core/models/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/core/models/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16789 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/core/models/posterior_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/core/multiprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:03:24.363811 dingo-gw-0.5.3/dingo/core/nn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/core/nn/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14095 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/core/nn/enets.py
--rw-r--r--   0 runner    (1001) docker     (123)    14037 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/core/nn/nsf.py
--rw-r--r--   0 runner    (1001) docker     (123)    25730 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/core/result.py
--rw-r--r--   0 runner    (1001) docker     (123)    21593 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/core/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/core/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:03:24.367811 dingo-gw-0.5.3/dingo/core/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/core/utils/condor_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/core/utils/gnpeutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/core/utils/logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/core/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/core/utils/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/core/utils/pt_to_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)     8069 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/core/utils/torchutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8031 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/core/utils/trainutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:03:24.367811 dingo-gw-0.5.3/dingo/gw/
--rw-r--r--   0 runner    (1001) docker     (123)     7991 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/gw/SVD.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/gw/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:03:24.371811 dingo-gw-0.5.3/dingo/gw/conversion/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/gw/conversion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6072 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/gw/conversion/spin_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:03:24.371811 dingo-gw-0.5.3/dingo/gw/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/gw/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/gw/data/data_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/gw/data/data_preparation.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/gw/data/event_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:03:24.371811 dingo-gw-0.5.3/dingo/gw/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/gw/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10182 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/gw/dataset/generate_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10094 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/gw/dataset/generate_dataset_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/gw/dataset/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9199 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/gw/dataset/waveform_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    21281 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/gw/domains.py
--rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/gw/download_strain_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/gw/gwutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:03:24.371811 dingo-gw-0.5.3/dingo/gw/importance_sampling/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/gw/importance_sampling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8273 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/gw/importance_sampling/diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/gw/importance_sampling/importance_weights.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:03:24.371811 dingo-gw-0.5.3/dingo/gw/inference/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/gw/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13654 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/gw/inference/gw_samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12606 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/gw/inference/inference_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/gw/inference/visualization.py
--rw-r--r--   0 runner    (1001) docker     (123)    14315 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/gw/injection.py
--rw-r--r--   0 runner    (1001) docker     (123)    31426 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/gw/likelihood.py
--rw-r--r--   0 runner    (1001) docker     (123)     6318 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/gw/ls_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:03:24.375811 dingo-gw-0.5.3/dingo/gw/noise/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/gw/noise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/gw/noise/asd_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/gw/noise/asd_estimation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/gw/noise/generate_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/gw/noise/generate_dataset_dag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:03:24.375811 dingo-gw-0.5.3/dingo/gw/noise/synthetic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/gw/noise/synthetic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10235 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/gw/noise/synthetic/asd_parameterization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/gw/noise/synthetic/asd_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/gw/noise/synthetic/generate_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/gw/noise/synthetic/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/gw/noise/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/gw/prior.py
--rw-r--r--   0 runner    (1001) docker     (123)    24817 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/gw/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/gw/temporary_debug_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:03:24.375811 dingo-gw-0.5.3/dingo/gw/training/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/gw/training/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12660 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/gw/training/train_builders.py
--rw-r--r--   0 runner    (1001) docker     (123)    12949 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/gw/training/train_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/gw/training/train_pipeline_condor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/gw/training/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:03:24.379811 dingo-gw-0.5.3/dingo/gw/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/gw/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15842 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/gw/transforms/detector_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/gw/transforms/general_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     9324 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/gw/transforms/gnpe_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/gw/transforms/inference_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7141 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/gw/transforms/noise_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7427 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/gw/transforms/parameter_transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:03:24.379811 dingo-gw-0.5.3/dingo/gw/waveform_generator/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/gw/waveform_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/gw/waveform_generator/frame_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    57836 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/gw/waveform_generator/waveform_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/gw/waveform_generator/wfg_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:03:24.379811 dingo-gw-0.5.3/dingo/pipe/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/pipe/ACKNOWLEDGMENT.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/pipe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/pipe/dag_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10503 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/pipe/data_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/pipe/default_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/pipe/dingo_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     7962 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/pipe/importance_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)    12384 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/pipe/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:03:24.383811 dingo-gw-0.5.3/dingo/pipe/nodes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/pipe/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/pipe/nodes/generation_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/pipe/nodes/importance_sampling_node.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/pipe/nodes/merge_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/pipe/nodes/pe_summary_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/pipe/nodes/plot_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/pipe/nodes/sampling_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    44434 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/pipe/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/pipe/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/pipe/sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/dingo/pipe/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:03:24.383811 dingo-gw-0.5.3/dingo_gw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-05-10 16:03:24.000000 dingo-gw-0.5.3/dingo_gw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-05-10 16:03:24.000000 dingo-gw-0.5.3/dingo_gw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 16:03:24.000000 dingo-gw-0.5.3/dingo_gw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-10 16:03:24.000000 dingo-gw-0.5.3/dingo_gw.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-10 16:03:24.000000 dingo-gw-0.5.3/dingo_gw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-10 16:03:24.000000 dingo-gw-0.5.3/dingo_gw.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:03:24.383811 dingo-gw-0.5.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:03:24.387811 dingo-gw-0.5.3/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/docs/source/code_design.md
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     9051 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/docs/source/dingo_pipe.md
--rw-r--r--   0 runner    (1001) docker     (123)     4319 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/docs/source/example_gnpe_model.md
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/docs/source/example_injection.md
--rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/docs/source/example_npe_model.md
--rw-r--r--   0 runner    (1001) docker     (123)    13566 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/docs/source/example_toy_npe_model.md
--rw-r--r--   0 runner    (1001) docker     (123)    42481 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/docs/source/generating_waveforms.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    30150 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/docs/source/gibbs_figure.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/docs/source/gnpe.md
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/docs/source/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/docs/source/inference.md
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/docs/source/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/docs/source/network_architecture.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    12693 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/docs/source/noise_dataset.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/docs/source/overview.md
--rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/docs/source/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/docs/source/refs.bib
--rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/docs/source/result.md
--rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/docs/source/sbi.md
--rw-r--r--   0 runner    (1001) docker     (123)    11832 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/docs/source/training.md
--rw-r--r--   0 runner    (1001) docker     (123)    13311 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/docs/source/training_transforms.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    25491 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/docs/source/waveform_dataset.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:03:24.387811 dingo-gw-0.5.3/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/examples/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:03:24.391811 dingo-gw-0.5.3/examples/dataset_generation/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/examples/dataset_generation/asd_dataset_settings_synthetic.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:03:24.391811 dingo-gw-0.5.3/examples/gnpe_model/
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/examples/gnpe_model/GW150914.ini
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/examples/gnpe_model/asd_dataset_settings.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/examples/gnpe_model/asd_dataset_settings_fiducial.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/examples/gnpe_model/train_settings.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/examples/gnpe_model/train_settings_init.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/examples/gnpe_model/waveform_dataset_settings.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:03:24.391811 dingo-gw-0.5.3/examples/misc/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1153 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/examples/misc/is_settings.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/examples/misc/stage_settings.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:03:24.391811 dingo-gw-0.5.3/examples/npe_model/
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/examples/npe_model/GW150914.ini
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/examples/npe_model/asd_dataset_settings.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/examples/npe_model/asd_dataset_settings_fiducial.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/examples/npe_model/train_settings.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/examples/npe_model/waveform_dataset_settings.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:03:24.391811 dingo-gw-0.5.3/examples/toy_npe_model/
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/examples/toy_npe_model/GW150914.ini
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/examples/toy_npe_model/asd_dataset_settings.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/examples/toy_npe_model/train_settings.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/examples/toy_npe_model/waveform_dataset_settings.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 16:03:24.399811 dingo-gw-0.5.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:03:24.355811 dingo-gw-0.5.3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:03:24.395811 dingo-gw-0.5.3/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)     9346 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/tests/core/test_enets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/tests/core/test_nsf.py
--rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/tests/core/test_posterior_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/tests/core/testutils_enets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:03:24.395811 dingo-gw-0.5.3/tests/gw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:03:24.395811 dingo-gw-0.5.3/tests/gw/conversion/
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/tests/gw/conversion/test_spin_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/tests/gw/conversion/test_time_delay_from_geocenter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10652 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/tests/gw/test_domains.py
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/tests/gw/test_injection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/tests/gw/test_noise_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/tests/gw/test_prior_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/tests/gw/test_waveform_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:03:24.395811 dingo-gw-0.5.3/tests/gw/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/tests/gw/transforms/test_detector_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/tests/gw/transforms/test_general_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/tests/gw/transforms/test_gnpe_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/tests/gw/transforms/test_parameter_transforms.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   263605 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/tests/gw/transforms/waveform_data.npy
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:03:24.395811 dingo-gw-0.5.3/tests/gw/waveform_generator/
--rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/tests/gw/waveform_generator/test_wfg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5164 2023-05-10 16:03:09.000000 dingo-gw-0.5.3/tests/gw/waveform_generator/test_wfg_m.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:00:34.985680 dingo-gw-0.5.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:00:34.953680 dingo-gw-0.5.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:00:34.961680 dingo-gw-0.5.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-08-04 16:00:34.985680 dingo-gw-0.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:00:34.961680 dingo-gw-0.5.4/compatibility/
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/compatibility/remove_domain_window_factor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/compatibility/update_model_input_dims.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/compatibility/update_model_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/compatibility/update_saved_model_for_train_stages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/compatibility/update_saved_model_gnpe_context_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/compatibility/update_saved_model_new_gnpe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/compatibility/update_saved_model_new_truncation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/compatibility/update_waveform_dataset_svd_refactor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:00:34.961680 dingo-gw-0.5.4/dingo/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-04 16:00:34.000000 dingo-gw-0.5.4/dingo/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:00:34.961680 dingo-gw-0.5.4/dingo/asimov/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/asimov/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10315 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/asimov/asimov.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/asimov/dingo.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:00:34.961680 dingo-gw-0.5.4/dingo/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/core/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:00:34.961680 dingo-gw-0.5.4/dingo/core/density/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/core/density/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/core/density/interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/core/density/nde_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/core/density/unconditional_density_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/core/likelihood.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:00:34.961680 dingo-gw-0.5.4/dingo/core/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/core/models/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16789 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/core/models/posterior_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/core/multiprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:00:34.965680 dingo-gw-0.5.4/dingo/core/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/core/nn/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14095 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/core/nn/enets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14037 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/core/nn/nsf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25730 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/core/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21593 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/core/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/core/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:00:34.965680 dingo-gw-0.5.4/dingo/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/core/utils/condor_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/core/utils/gnpeutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/core/utils/logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/core/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/core/utils/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/core/utils/pt_to_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8069 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/core/utils/torchutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8031 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/core/utils/trainutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:00:34.965680 dingo-gw-0.5.4/dingo/gw/
+-rw-r--r--   0 runner    (1001) docker     (123)     7991 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/gw/SVD.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/gw/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:00:34.965680 dingo-gw-0.5.4/dingo/gw/conversion/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/gw/conversion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6072 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/gw/conversion/spin_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:00:34.969680 dingo-gw-0.5.4/dingo/gw/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/gw/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/gw/data/data_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/gw/data/data_preparation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/gw/data/event_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:00:34.969680 dingo-gw-0.5.4/dingo/gw/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/gw/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10182 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/gw/dataset/generate_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10094 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/gw/dataset/generate_dataset_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/gw/dataset/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9199 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/gw/dataset/waveform_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21281 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/gw/domains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/gw/download_strain_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/gw/gwutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:00:34.969680 dingo-gw-0.5.4/dingo/gw/importance_sampling/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/gw/importance_sampling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8273 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/gw/importance_sampling/diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/gw/importance_sampling/importance_weights.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:00:34.969680 dingo-gw-0.5.4/dingo/gw/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/gw/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13654 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/gw/inference/gw_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12606 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/gw/inference/inference_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/gw/inference/visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14315 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/gw/injection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31426 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/gw/likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6318 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/gw/ls_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:00:34.969680 dingo-gw-0.5.4/dingo/gw/noise/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/gw/noise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/gw/noise/asd_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/gw/noise/asd_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/gw/noise/generate_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/gw/noise/generate_dataset_dag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:00:34.969680 dingo-gw-0.5.4/dingo/gw/noise/synthetic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/gw/noise/synthetic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10235 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/gw/noise/synthetic/asd_parameterization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/gw/noise/synthetic/asd_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/gw/noise/synthetic/generate_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/gw/noise/synthetic/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/gw/noise/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/gw/prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24817 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/gw/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/gw/temporary_debug_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:00:34.973680 dingo-gw-0.5.4/dingo/gw/training/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/gw/training/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12660 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/gw/training/train_builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12949 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/gw/training/train_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/gw/training/train_pipeline_condor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/gw/training/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:00:34.973680 dingo-gw-0.5.4/dingo/gw/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/gw/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15842 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/gw/transforms/detector_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/gw/transforms/general_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9324 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/gw/transforms/gnpe_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/gw/transforms/inference_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7141 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/gw/transforms/noise_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7427 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/gw/transforms/parameter_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:00:34.973680 dingo-gw-0.5.4/dingo/gw/waveform_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/gw/waveform_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/gw/waveform_generator/frame_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57932 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/gw/waveform_generator/waveform_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/gw/waveform_generator/wfg_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:00:34.973680 dingo-gw-0.5.4/dingo/pipe/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/pipe/ACKNOWLEDGMENT.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/pipe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/pipe/dag_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10503 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/pipe/data_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/pipe/default_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/pipe/dingo_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7962 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/pipe/importance_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12384 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/pipe/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:00:34.977680 dingo-gw-0.5.4/dingo/pipe/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/pipe/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/pipe/nodes/generation_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/pipe/nodes/importance_sampling_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/pipe/nodes/merge_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/pipe/nodes/pe_summary_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/pipe/nodes/plot_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/pipe/nodes/sampling_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44434 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/pipe/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/pipe/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/pipe/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/dingo/pipe/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:00:34.977680 dingo-gw-0.5.4/dingo_gw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-08-04 16:00:34.000000 dingo-gw-0.5.4/dingo_gw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-08-04 16:00:34.000000 dingo-gw-0.5.4/dingo_gw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 16:00:34.000000 dingo-gw-0.5.4/dingo_gw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-08-04 16:00:34.000000 dingo-gw-0.5.4/dingo_gw.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-08-04 16:00:34.000000 dingo-gw-0.5.4/dingo_gw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-04 16:00:34.000000 dingo-gw-0.5.4/dingo_gw.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:00:34.977680 dingo-gw-0.5.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:00:34.981680 dingo-gw-0.5.4/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/docs/source/code_design.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9051 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/docs/source/dingo_pipe.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4319 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/docs/source/example_gnpe_model.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/docs/source/example_injection.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/docs/source/example_npe_model.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13566 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/docs/source/example_toy_npe_model.md
+-rw-r--r--   0 runner    (1001) docker     (123)    42481 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/docs/source/generating_waveforms.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    30150 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/docs/source/gibbs_figure.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/docs/source/gnpe.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/docs/source/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/docs/source/inference.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/docs/source/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/docs/source/network_architecture.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12693 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/docs/source/noise_dataset.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/docs/source/overview.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/docs/source/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/docs/source/refs.bib
+-rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/docs/source/result.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/docs/source/sbi.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11832 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/docs/source/training.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13311 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/docs/source/training_transforms.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    25491 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/docs/source/waveform_dataset.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:00:34.981680 dingo-gw-0.5.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/examples/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:00:34.981680 dingo-gw-0.5.4/examples/dataset_generation/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/examples/dataset_generation/asd_dataset_settings_synthetic.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:00:34.981680 dingo-gw-0.5.4/examples/gnpe_model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/examples/gnpe_model/GW150914.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/examples/gnpe_model/asd_dataset_settings.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/examples/gnpe_model/asd_dataset_settings_fiducial.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/examples/gnpe_model/train_settings.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/examples/gnpe_model/train_settings_init.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/examples/gnpe_model/waveform_dataset_settings.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:00:34.981680 dingo-gw-0.5.4/examples/misc/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1153 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/examples/misc/is_settings.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/examples/misc/stage_settings.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:00:34.981680 dingo-gw-0.5.4/examples/npe_model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/examples/npe_model/GW150914.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/examples/npe_model/asd_dataset_settings.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/examples/npe_model/asd_dataset_settings_fiducial.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/examples/npe_model/train_settings.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/examples/npe_model/waveform_dataset_settings.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:00:34.981680 dingo-gw-0.5.4/examples/toy_npe_model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/examples/toy_npe_model/GW150914.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/examples/toy_npe_model/asd_dataset_settings.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/examples/toy_npe_model/train_settings.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/examples/toy_npe_model/waveform_dataset_settings.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 16:00:34.985680 dingo-gw-0.5.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:00:34.957680 dingo-gw-0.5.4/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:00:34.985680 dingo-gw-0.5.4/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     9346 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/tests/core/test_enets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/tests/core/test_nsf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/tests/core/test_posterior_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/tests/core/testutils_enets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:00:34.985680 dingo-gw-0.5.4/tests/gw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:00:34.985680 dingo-gw-0.5.4/tests/gw/conversion/
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/tests/gw/conversion/test_spin_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/tests/gw/conversion/test_time_delay_from_geocenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10652 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/tests/gw/test_domains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/tests/gw/test_injection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/tests/gw/test_noise_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/tests/gw/test_prior_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/tests/gw/test_waveform_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:00:34.985680 dingo-gw-0.5.4/tests/gw/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/tests/gw/transforms/test_detector_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/tests/gw/transforms/test_general_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/tests/gw/transforms/test_gnpe_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/tests/gw/transforms/test_parameter_transforms.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   263605 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/tests/gw/transforms/waveform_data.npy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:00:34.985680 dingo-gw-0.5.4/tests/gw/waveform_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/tests/gw/waveform_generator/test_wfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5164 2023-08-04 16:00:22.000000 dingo-gw-0.5.4/tests/gw/waveform_generator/test_wfg_m.py
```

### Comparing `dingo-gw-0.5.3/.github/workflows/python-publish.yml` & `dingo-gw-0.5.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/.readthedocs.yaml` & `dingo-gw-0.5.4/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/LICENSE` & `dingo-gw-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/PKG-INFO` & `dingo-gw-0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dingo-gw
-Version: 0.5.3
+Version: 0.5.4
 Summary: Deep inference for gravitational-wave observations
 Author-email: Maximilian Dax <maximilian.dax@tuebingen.mpg.de>, Stephen Green <Stephen.Green2@nottingham.ac.uk>
 License: MIT
 Project-URL: homepage, https://github.com/dingo-gw/dingo
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dingo-gw-0.5.3/README.md` & `dingo-gw-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/compatibility/remove_domain_window_factor.py` & `dingo-gw-0.5.4/compatibility/remove_domain_window_factor.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/compatibility/update_model_input_dims.py` & `dingo-gw-0.5.4/compatibility/update_model_input_dims.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/compatibility/update_model_metadata.py` & `dingo-gw-0.5.4/compatibility/update_model_metadata.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/compatibility/update_saved_model_for_train_stages.py` & `dingo-gw-0.5.4/compatibility/update_saved_model_for_train_stages.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/compatibility/update_saved_model_gnpe_context_names.py` & `dingo-gw-0.5.4/compatibility/update_saved_model_gnpe_context_names.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/compatibility/update_saved_model_new_gnpe.py` & `dingo-gw-0.5.4/compatibility/update_saved_model_new_gnpe.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/compatibility/update_saved_model_new_truncation.py` & `dingo-gw-0.5.4/compatibility/update_saved_model_new_truncation.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/asimov/asimov.py` & `dingo-gw-0.5.4/dingo/asimov/asimov.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/asimov/dingo.ini` & `dingo-gw-0.5.4/dingo/asimov/dingo.ini`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/core/dataset.py` & `dingo-gw-0.5.4/dingo/core/dataset.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/core/density/interpolation.py` & `dingo-gw-0.5.4/dingo/core/density/interpolation.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/core/density/nde_settings.py` & `dingo-gw-0.5.4/dingo/core/density/nde_settings.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/core/density/unconditional_density_estimation.py` & `dingo-gw-0.5.4/dingo/core/density/unconditional_density_estimation.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/core/likelihood.py` & `dingo-gw-0.5.4/dingo/core/likelihood.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/core/models/posterior_model.py` & `dingo-gw-0.5.4/dingo/core/models/posterior_model.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/core/multiprocessing.py` & `dingo-gw-0.5.4/dingo/core/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/core/nn/enets.py` & `dingo-gw-0.5.4/dingo/core/nn/enets.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/core/nn/nsf.py` & `dingo-gw-0.5.4/dingo/core/nn/nsf.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/core/result.py` & `dingo-gw-0.5.4/dingo/core/result.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/core/samplers.py` & `dingo-gw-0.5.4/dingo/core/samplers.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/core/utils/condor_utils.py` & `dingo-gw-0.5.4/dingo/core/utils/condor_utils.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/core/utils/gnpeutils.py` & `dingo-gw-0.5.4/dingo/core/utils/gnpeutils.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/core/utils/logging_utils.py` & `dingo-gw-0.5.4/dingo/core/utils/logging_utils.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/core/utils/misc.py` & `dingo-gw-0.5.4/dingo/core/utils/misc.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/core/utils/plotting.py` & `dingo-gw-0.5.4/dingo/core/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/core/utils/pt_to_hdf5.py` & `dingo-gw-0.5.4/dingo/core/utils/pt_to_hdf5.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/core/utils/torchutils.py` & `dingo-gw-0.5.4/dingo/core/utils/torchutils.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/core/utils/trainutils.py` & `dingo-gw-0.5.4/dingo/core/utils/trainutils.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/gw/SVD.py` & `dingo-gw-0.5.4/dingo/gw/SVD.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/gw/conversion/spin_conversion.py` & `dingo-gw-0.5.4/dingo/gw/conversion/spin_conversion.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/gw/data/data_download.py` & `dingo-gw-0.5.4/dingo/gw/data/data_download.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/gw/data/data_preparation.py` & `dingo-gw-0.5.4/dingo/gw/data/data_preparation.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/gw/dataset/generate_dataset.py` & `dingo-gw-0.5.4/dingo/gw/dataset/generate_dataset.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/gw/dataset/generate_dataset_dag.py` & `dingo-gw-0.5.4/dingo/gw/dataset/generate_dataset_dag.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/gw/dataset/utils.py` & `dingo-gw-0.5.4/dingo/gw/dataset/utils.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/gw/dataset/waveform_dataset.py` & `dingo-gw-0.5.4/dingo/gw/dataset/waveform_dataset.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/gw/domains.py` & `dingo-gw-0.5.4/dingo/gw/domains.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/gw/download_strain_data.py` & `dingo-gw-0.5.4/dingo/gw/download_strain_data.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/gw/gwutils.py` & `dingo-gw-0.5.4/dingo/gw/gwutils.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/gw/importance_sampling/diagnostics.py` & `dingo-gw-0.5.4/dingo/gw/importance_sampling/diagnostics.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/gw/importance_sampling/importance_weights.py` & `dingo-gw-0.5.4/dingo/gw/importance_sampling/importance_weights.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/gw/inference/gw_samplers.py` & `dingo-gw-0.5.4/dingo/gw/inference/gw_samplers.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/gw/inference/inference_pipeline.py` & `dingo-gw-0.5.4/dingo/gw/inference/inference_pipeline.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/gw/inference/visualization.py` & `dingo-gw-0.5.4/dingo/gw/inference/visualization.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/gw/injection.py` & `dingo-gw-0.5.4/dingo/gw/injection.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/gw/likelihood.py` & `dingo-gw-0.5.4/dingo/gw/likelihood.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/gw/ls_cli.py` & `dingo-gw-0.5.4/dingo/gw/ls_cli.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/gw/noise/asd_dataset.py` & `dingo-gw-0.5.4/dingo/gw/noise/asd_dataset.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/gw/noise/asd_estimation.py` & `dingo-gw-0.5.4/dingo/gw/noise/asd_estimation.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/gw/noise/generate_dataset.py` & `dingo-gw-0.5.4/dingo/gw/noise/generate_dataset.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/gw/noise/generate_dataset_dag.py` & `dingo-gw-0.5.4/dingo/gw/noise/generate_dataset_dag.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/gw/noise/synthetic/asd_parameterization.py` & `dingo-gw-0.5.4/dingo/gw/noise/synthetic/asd_parameterization.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/gw/noise/synthetic/asd_sampling.py` & `dingo-gw-0.5.4/dingo/gw/noise/synthetic/asd_sampling.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/gw/noise/synthetic/generate_dataset.py` & `dingo-gw-0.5.4/dingo/gw/noise/synthetic/generate_dataset.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/gw/noise/synthetic/utils.py` & `dingo-gw-0.5.4/dingo/gw/noise/synthetic/utils.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/gw/noise/utils.py` & `dingo-gw-0.5.4/dingo/gw/noise/utils.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/gw/prior.py` & `dingo-gw-0.5.4/dingo/gw/prior.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/gw/result.py` & `dingo-gw-0.5.4/dingo/gw/result.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/gw/temporary_debug_utils.py` & `dingo-gw-0.5.4/dingo/gw/temporary_debug_utils.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/gw/training/train_builders.py` & `dingo-gw-0.5.4/dingo/gw/training/train_builders.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/gw/training/train_pipeline.py` & `dingo-gw-0.5.4/dingo/gw/training/train_pipeline.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/gw/training/train_pipeline_condor.py` & `dingo-gw-0.5.4/dingo/gw/training/train_pipeline_condor.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/gw/training/utils.py` & `dingo-gw-0.5.4/dingo/gw/training/utils.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/gw/transforms/detector_transforms.py` & `dingo-gw-0.5.4/dingo/gw/transforms/detector_transforms.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/gw/transforms/gnpe_transforms.py` & `dingo-gw-0.5.4/dingo/gw/transforms/gnpe_transforms.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/gw/transforms/inference_transforms.py` & `dingo-gw-0.5.4/dingo/gw/transforms/inference_transforms.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/gw/transforms/noise_transforms.py` & `dingo-gw-0.5.4/dingo/gw/transforms/noise_transforms.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/gw/transforms/parameter_transforms.py` & `dingo-gw-0.5.4/dingo/gw/transforms/parameter_transforms.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/gw/waveform_generator/frame_utils.py` & `dingo-gw-0.5.4/dingo/gw/waveform_generator/frame_utils.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/gw/waveform_generator/waveform_generator.py` & `dingo-gw-0.5.4/dingo/gw/waveform_generator/waveform_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -786,14 +786,19 @@
     def _convert_parameters(
         self,
         parameter_dict: Dict,
         lal_params=None,
     ):
         # Transform mass, spin, and distance parameters
         p, _ = convert_to_lal_binary_black_hole_parameters(parameter_dict)
+
+        # Convert to SI units
+        p["mass_1"] *= lal.MSUN_SI
+        p["mass_2"] *= lal.MSUN_SI
+    
         # Transform to lal source frame: iota and Cartesian spin components
         param_keys_in = (
             "theta_jn",
             "phi_jl",
             "tilt_1",
             "tilt_2",
             "phi_12",
@@ -821,16 +826,16 @@
             f_min = self.f_start
         else:
             f_min = self.domain.f_min
         # parameters needed for TD waveforms
         delta_t = 0.5 / self.domain.f_max
 
         params_gwsignal = {
-            "mass1": p["mass_1"] * u.solMass,
-            "mass2": p["mass_2"] * u.solMass,
+            "mass1": p["mass_1"] * u.kg,
+            "mass2": p["mass_2"] * u.kg,
             "spin1x": s1x * u.dimensionless_unscaled,
             "spin1y": s1y * u.dimensionless_unscaled,
             "spin1z": s1z * u.dimensionless_unscaled,
             "spin2x": s2x * u.dimensionless_unscaled,
             "spin2y": s2y * u.dimensionless_unscaled,
             "spin2z": s2z * u.dimensionless_unscaled,
             "deltaT": delta_t * u.s,
```

### Comparing `dingo-gw-0.5.3/dingo/gw/waveform_generator/wfg_utils.py` & `dingo-gw-0.5.4/dingo/gw/waveform_generator/wfg_utils.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/pipe/dag_creator.py` & `dingo-gw-0.5.4/dingo/pipe/dag_creator.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/pipe/data_generation.py` & `dingo-gw-0.5.4/dingo/pipe/data_generation.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/pipe/default_settings.py` & `dingo-gw-0.5.4/dingo/pipe/default_settings.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/pipe/dingo_result.py` & `dingo-gw-0.5.4/dingo/pipe/dingo_result.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/pipe/importance_sampling.py` & `dingo-gw-0.5.4/dingo/pipe/importance_sampling.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/pipe/main.py` & `dingo-gw-0.5.4/dingo/pipe/main.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/pipe/nodes/generation_node.py` & `dingo-gw-0.5.4/dingo/pipe/nodes/generation_node.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/pipe/nodes/importance_sampling_node.py` & `dingo-gw-0.5.4/dingo/pipe/nodes/importance_sampling_node.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/pipe/nodes/merge_node.py` & `dingo-gw-0.5.4/dingo/pipe/nodes/merge_node.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/pipe/nodes/pe_summary_node.py` & `dingo-gw-0.5.4/dingo/pipe/nodes/pe_summary_node.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/pipe/nodes/plot_node.py` & `dingo-gw-0.5.4/dingo/pipe/nodes/plot_node.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/pipe/nodes/sampling_node.py` & `dingo-gw-0.5.4/dingo/pipe/nodes/sampling_node.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/pipe/parser.py` & `dingo-gw-0.5.4/dingo/pipe/parser.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/pipe/plot.py` & `dingo-gw-0.5.4/dingo/pipe/plot.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo/pipe/sampling.py` & `dingo-gw-0.5.4/dingo/pipe/sampling.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo_gw.egg-info/PKG-INFO` & `dingo-gw-0.5.4/dingo_gw.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dingo-gw
-Version: 0.5.3
+Version: 0.5.4
 Summary: Deep inference for gravitational-wave observations
 Author-email: Maximilian Dax <maximilian.dax@tuebingen.mpg.de>, Stephen Green <Stephen.Green2@nottingham.ac.uk>
 License: MIT
 Project-URL: homepage, https://github.com/dingo-gw/dingo
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dingo-gw-0.5.3/dingo_gw.egg-info/SOURCES.txt` & `dingo-gw-0.5.4/dingo_gw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/dingo_gw.egg-info/entry_points.txt` & `dingo-gw-0.5.4/dingo_gw.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/docs/Makefile` & `dingo-gw-0.5.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/docs/README.md` & `dingo-gw-0.5.4/docs/README.md`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/docs/make.bat` & `dingo-gw-0.5.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/docs/source/code_design.md` & `dingo-gw-0.5.4/docs/source/code_design.md`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/docs/source/conf.py` & `dingo-gw-0.5.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/docs/source/dingo_pipe.md` & `dingo-gw-0.5.4/docs/source/dingo_pipe.md`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/docs/source/example_gnpe_model.md` & `dingo-gw-0.5.4/docs/source/example_gnpe_model.md`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/docs/source/example_injection.md` & `dingo-gw-0.5.4/docs/source/example_injection.md`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/docs/source/example_npe_model.md` & `dingo-gw-0.5.4/docs/source/example_npe_model.md`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/docs/source/example_toy_npe_model.md` & `dingo-gw-0.5.4/docs/source/example_toy_npe_model.md`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/docs/source/generating_waveforms.ipynb` & `dingo-gw-0.5.4/docs/source/generating_waveforms.ipynb`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/docs/source/gibbs_figure.jpg` & `dingo-gw-0.5.4/docs/source/gibbs_figure.jpg`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/docs/source/gnpe.md` & `dingo-gw-0.5.4/docs/source/gnpe.md`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/docs/source/index.md` & `dingo-gw-0.5.4/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/docs/source/inference.md` & `dingo-gw-0.5.4/docs/source/inference.md`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/docs/source/installation.md` & `dingo-gw-0.5.4/docs/source/installation.md`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/docs/source/network_architecture.ipynb` & `dingo-gw-0.5.4/docs/source/network_architecture.ipynb`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/docs/source/noise_dataset.ipynb` & `dingo-gw-0.5.4/docs/source/noise_dataset.ipynb`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/docs/source/overview.md` & `dingo-gw-0.5.4/docs/source/overview.md`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/docs/source/quickstart.md` & `dingo-gw-0.5.4/docs/source/quickstart.md`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/docs/source/refs.bib` & `dingo-gw-0.5.4/docs/source/refs.bib`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/docs/source/result.md` & `dingo-gw-0.5.4/docs/source/result.md`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/docs/source/sbi.md` & `dingo-gw-0.5.4/docs/source/sbi.md`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/docs/source/training.md` & `dingo-gw-0.5.4/docs/source/training.md`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/docs/source/training_transforms.ipynb` & `dingo-gw-0.5.4/docs/source/training_transforms.ipynb`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/docs/source/waveform_dataset.ipynb` & `dingo-gw-0.5.4/docs/source/waveform_dataset.ipynb`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/examples/README.md` & `dingo-gw-0.5.4/examples/README.md`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/examples/dataset_generation/asd_dataset_settings_synthetic.yaml` & `dingo-gw-0.5.4/examples/dataset_generation/asd_dataset_settings_synthetic.yaml`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/examples/gnpe_model/GW150914.ini` & `dingo-gw-0.5.4/examples/gnpe_model/GW150914.ini`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/examples/gnpe_model/asd_dataset_settings.yaml` & `dingo-gw-0.5.4/examples/gnpe_model/asd_dataset_settings.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 dataset_settings:
 #  f_min: 0         # defaults to 0
 #  f_max: 2048      # defaults to f_s/2
   f_s: 4096
   time_psd: 1024
-  T: 4
+  T: 8.0
   window:
     roll_off: 0.4
     type: tukey
   time_gap: 0          # specifies the time skipped between to consecutive PSD estimates. If set < 0, the time segments overlap
   num_psds_max: 0   # if set > 0, only a subset of all available PSDs will be used
 #  channels:
 #    H1: H1:DCS-CALIB_STRAIN_C02
```

### Comparing `dingo-gw-0.5.3/examples/gnpe_model/train_settings.yaml` & `dingo-gw-0.5.4/examples/gnpe_model/train_settings.yaml`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/examples/gnpe_model/train_settings_init.yaml` & `dingo-gw-0.5.4/examples/gnpe_model/train_settings_init.yaml`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/examples/gnpe_model/waveform_dataset_settings.yaml` & `dingo-gw-0.5.4/examples/gnpe_model/waveform_dataset_settings.yaml`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/examples/misc/is_settings.yaml` & `dingo-gw-0.5.4/examples/misc/is_settings.yaml`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/examples/npe_model/GW150914.ini` & `dingo-gw-0.5.4/examples/npe_model/GW150914.ini`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/examples/npe_model/asd_dataset_settings.yaml` & `dingo-gw-0.5.4/examples/npe_model/asd_dataset_settings.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 dataset_settings:
 #  f_min: 0         # defaults to 0
 #  f_max: 2048      # defaults to f_s/2
   f_s: 4096
   time_psd: 1024
-  T: 8
+  T: 8.0
   window:
     roll_off: 0.4
     type: tukey
   time_gap: 0          # specifies the time skipped between to consecutive PSD estimates. If set < 0, the time segments overlap
   num_psds_max: 0   # if set > 0, only a subset of all available PSDs will be used
 #  channels:
 #    H1: H1:DCS-CALIB_STRAIN_C02
```

### Comparing `dingo-gw-0.5.3/examples/npe_model/train_settings.yaml` & `dingo-gw-0.5.4/examples/npe_model/train_settings.yaml`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/examples/npe_model/waveform_dataset_settings.yaml` & `dingo-gw-0.5.4/examples/npe_model/waveform_dataset_settings.yaml`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/examples/toy_npe_model/GW150914.ini` & `dingo-gw-0.5.4/examples/toy_npe_model/GW150914.ini`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/examples/toy_npe_model/asd_dataset_settings.yaml` & `dingo-gw-0.5.4/examples/toy_npe_model/asd_dataset_settings.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 dataset_settings:
 #  f_min: 0         # defaults to 0
 #  f_max: 2048      # defaults to f_s/2
   f_s: 4096
   time_psd: 1024
-  T: 8
+  T: 4.0
   window:
     roll_off: 0.4
     type: tukey
   time_gap: 0          # specifies the time skipped between to consecutive PSD estimates. If set < 0, the time segments overlap
   num_psds_max: 1   # if set > 0, only a subset of all available PSDs will be used
 #  channels:
 #    H1: H1:DCS-CALIB_STRAIN_C02
```

### Comparing `dingo-gw-0.5.3/examples/toy_npe_model/train_settings.yaml` & `dingo-gw-0.5.4/examples/toy_npe_model/train_settings.yaml`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/examples/toy_npe_model/waveform_dataset_settings.yaml` & `dingo-gw-0.5.4/examples/toy_npe_model/waveform_dataset_settings.yaml`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/pyproject.toml` & `dingo-gw-0.5.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/tests/core/test_enets.py` & `dingo-gw-0.5.4/tests/core/test_enets.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/tests/core/test_nsf.py` & `dingo-gw-0.5.4/tests/core/test_nsf.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/tests/core/test_posterior_model.py` & `dingo-gw-0.5.4/tests/core/test_posterior_model.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/tests/core/testutils_enets.py` & `dingo-gw-0.5.4/tests/core/testutils_enets.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/tests/gw/conversion/test_spin_conversion.py` & `dingo-gw-0.5.4/tests/gw/conversion/test_spin_conversion.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/tests/gw/conversion/test_time_delay_from_geocenter.py` & `dingo-gw-0.5.4/tests/gw/conversion/test_time_delay_from_geocenter.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/tests/gw/test_domains.py` & `dingo-gw-0.5.4/tests/gw/test_domains.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/tests/gw/test_injection.py` & `dingo-gw-0.5.4/tests/gw/test_injection.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/tests/gw/test_noise_dataset.py` & `dingo-gw-0.5.4/tests/gw/test_noise_dataset.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/tests/gw/test_prior_split.py` & `dingo-gw-0.5.4/tests/gw/test_prior_split.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/tests/gw/test_waveform_dataset.py` & `dingo-gw-0.5.4/tests/gw/test_waveform_dataset.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/tests/gw/transforms/test_detector_projection.py` & `dingo-gw-0.5.4/tests/gw/transforms/test_detector_projection.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/tests/gw/transforms/test_gnpe_transforms.py` & `dingo-gw-0.5.4/tests/gw/transforms/test_gnpe_transforms.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/tests/gw/transforms/test_parameter_transforms.py` & `dingo-gw-0.5.4/tests/gw/transforms/test_parameter_transforms.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/tests/gw/transforms/waveform_data.npy` & `dingo-gw-0.5.4/tests/gw/transforms/waveform_data.npy`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/tests/gw/waveform_generator/test_wfg.py` & `dingo-gw-0.5.4/tests/gw/waveform_generator/test_wfg.py`

 * *Files identical despite different names*

### Comparing `dingo-gw-0.5.3/tests/gw/waveform_generator/test_wfg_m.py` & `dingo-gw-0.5.4/tests/gw/waveform_generator/test_wfg_m.py`

 * *Files identical despite different names*

