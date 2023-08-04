# Comparing `tmp/bofire-0.0.4.tar.gz` & `tmp/bofire-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bofire-0.0.4.tar", last modified: Fri May  5 13:01:54 2023, max compression
+gzip compressed data, was "bofire-0.0.5.tar", last modified: Fri Aug  4 07:31:38 2023, max compression
```

## Comparing `bofire-0.0.4.tar` & `bofire-0.0.5.tar`

### file list

```diff
@@ -1,253 +1,382 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.681670 bofire-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-05 13:01:43.000000 bofire-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-05-05 13:01:54.681670 bofire-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-05 13:01:43.000000 bofire-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.629670 bofire-0.0.4/bofire/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.633670 bofire-0.0.4/bofire/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/benchmarks/aspen_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/benchmarks/benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.633670 bofire-0.0.4/bofire/benchmarks/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/benchmarks/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8591 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/benchmarks/data/aniline_cn_crosscoupling.py
--rw-r--r--   0 runner    (1001) docker     (123)    21299 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/benchmarks/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)    12080 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/benchmarks/single.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.633670 bofire-0.0.4/bofire/data_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.633670 bofire-0.0.4/bofire/data_models/acquisition_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/acquisition_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/acquisition_functions/acquisition_function.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/acquisition_functions/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.637670 bofire-0.0.4/bofire/data_models/constraints/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/constraints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/constraints/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/constraints/constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     7039 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/constraints/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/constraints/nchoosek.py
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/constraints/nonlinear.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.637670 bofire-0.0.4/bofire/data_models/domain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/domain/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/domain/constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)    26770 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/domain/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)    26741 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/domain/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/enum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.641670 bofire-0.0.4/bofire/data_models/features/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/features/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14122 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/features/categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/features/continuous.py
--rw-r--r--   0 runner    (1001) docker     (123)    10262 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/features/descriptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/features/discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/features/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/features/molecular.py
--rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/features/numerical.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.641670 bofire-0.0.4/bofire/data_models/kernels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/kernels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/kernels/aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/kernels/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/kernels/categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/kernels/continuous.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/kernels/kernel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.641670 bofire-0.0.4/bofire/data_models/objectives/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/objectives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/objectives/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/objectives/identity.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/objectives/objective.py
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/objectives/sigmoid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/objectives/target.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.645670 bofire-0.0.4/bofire/data_models/priors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/priors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/priors/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/priors/gamma.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/priors/normal.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/priors/prior.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.645670 bofire-0.0.4/bofire/data_models/strategies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/strategies/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/strategies/doe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.645670 bofire-0.0.4/bofire/data_models/strategies/predictives/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/strategies/predictives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/strategies/predictives/botorch.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/strategies/predictives/multiobjective.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/strategies/predictives/predictive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/strategies/predictives/qehvi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/strategies/predictives/qnehvi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/strategies/predictives/qparego.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/strategies/predictives/sobo.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/strategies/random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.645670 bofire-0.0.4/bofire/data_models/strategies/samplers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/strategies/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/strategies/samplers/polytope.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/strategies/samplers/rejection.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/strategies/samplers/sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/strategies/strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.649670 bofire-0.0.4/bofire/data_models/surrogates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/surrogates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/surrogates/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/surrogates/botorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/surrogates/botorch_surrogates.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/surrogates/empirical.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/surrogates/fully_bayesian.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/surrogates/mixed_single_task_gp.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/surrogates/mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/surrogates/random_forest.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/surrogates/scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/surrogates/single_task_gp.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/surrogates/surrogate.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/unions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/validated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.649670 bofire-0.0.4/bofire/plot/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/plot/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/plot/feature_importance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/plot/objective.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/plot/prior.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.653670 bofire-0.0.4/bofire/strategies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/strategies/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.653670 bofire-0.0.4/bofire/strategies/data_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/strategies/data_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/strategies/data_models/candidate.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/strategies/data_models/values.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.653670 bofire-0.0.4/bofire/strategies/doe/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/strategies/doe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9466 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/strategies/doe/design.py
--rw-r--r--   0 runner    (1001) docker     (123)    16789 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/strategies/doe/objective.py
--rw-r--r--   0 runner    (1001) docker     (123)    18128 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/strategies/doe/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/strategies/doe_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/strategies/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/strategies/mapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.657670 bofire-0.0.4/bofire/strategies/predictives/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/strategies/predictives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19396 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/strategies/predictives/botorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/strategies/predictives/predictive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/strategies/predictives/qehvi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/strategies/predictives/qnehvi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/strategies/predictives/qparego.py
--rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/strategies/predictives/sobo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/strategies/random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.657670 bofire-0.0.4/bofire/strategies/samplers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/strategies/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6764 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/strategies/samplers/polytope.py
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/strategies/samplers/rejection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/strategies/samplers/sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8150 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/strategies/strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.661670 bofire-0.0.4/bofire/surrogates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/surrogates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/surrogates/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/surrogates/botorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/surrogates/botorch_surrogates.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/surrogates/cloudpickle_module.py
--rw-r--r--   0 runner    (1001) docker     (123)    15738 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/surrogates/diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/surrogates/empirical.py
--rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/surrogates/feature_importance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/surrogates/fully_bayesian.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/surrogates/mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/surrogates/mixed_single_task_gp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7367 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/surrogates/mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/surrogates/random_forest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/surrogates/single_task_gp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/surrogates/surrogate.py
--rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/surrogates/trainable.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/surrogates/values.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.665670 bofire-0.0.4/bofire/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/utils/cheminformatics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/utils/doe.py
--rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/utils/multiobjective.py
--rw-r--r--   0 runner    (1001) docker     (123)    15585 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/utils/reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/utils/subdomain.py
--rw-r--r--   0 runner    (1001) docker     (123)    14283 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/utils/torch_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.629670 bofire-0.0.4/bofire.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-05-05 13:01:54.000000 bofire-0.0.4/bofire.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8354 2023-05-05 13:01:54.000000 bofire-0.0.4/bofire.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 13:01:54.000000 bofire-0.0.4/bofire.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-05 13:01:54.000000 bofire-0.0.4/bofire.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-05 13:01:54.000000 bofire-0.0.4/bofire.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-05 13:01:54.681670 bofire-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-05 13:01:43.000000 bofire-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.665670 bofire-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.665670 bofire-0.0.4/tests/bofire/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.665670 bofire-0.0.4/tests/bofire/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/benchmarks/test_aspen_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/benchmarks/test_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/benchmarks/test_multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/benchmarks/test_single.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.669670 bofire-0.0.4/tests/bofire/data_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/data_models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.669670 bofire-0.0.4/tests/bofire/data_models/serialization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/data_models/serialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/data_models/serialization/test_deserialization.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/data_models/serialization/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/data_models/serialization/test_serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.673670 bofire-0.0.4/tests/bofire/data_models/specs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/data_models/specs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/data_models/specs/acquisition_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/data_models/specs/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/data_models/specs/constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/data_models/specs/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/data_models/specs/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/data_models/specs/kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/data_models/specs/objectives.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/data_models/specs/priors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/data_models/specs/specs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/data_models/specs/strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/data_models/specs/surrogates.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/data_models/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/data_models/test_constraint_fulfillment.py
--rw-r--r--   0 runner    (1001) docker     (123)     6499 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/data_models/test_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)    22806 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/data_models/test_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     9961 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/data_models/test_domain_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)    55338 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/data_models/test_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     7296 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/data_models/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/data_models/test_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/data_models/test_molecular.py
--rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/data_models/test_nchoosek_combinatorics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/data_models/test_numeric.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/data_models/test_priors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/data_models/test_samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/data_models/test_unions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7296 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/data_models/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.677670 bofire-0.0.4/tests/bofire/strategies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/strategies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.677670 bofire-0.0.4/tests/bofire/strategies/doe/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/strategies/doe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15025 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/strategies/doe/test_design.py
--rw-r--r--   0 runner    (1001) docker     (123)    20262 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/strategies/doe/test_objective.py
--rw-r--r--   0 runner    (1001) docker     (123)    21977 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/strategies/doe/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/strategies/dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)    10648 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/strategies/specs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/strategies/test_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/strategies/test_ask.py
--rw-r--r--   0 runner    (1001) docker     (123)    27492 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/strategies/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/strategies/test_doe.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/strategies/test_from_data_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/strategies/test_model_specs_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8383 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/strategies/test_qehvi.py
--rw-r--r--   0 runner    (1001) docker     (123)     7171 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/strategies/test_qparego.py
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/strategies/test_random.py
--rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/strategies/test_sobo.py
--rw-r--r--   0 runner    (1001) docker     (123)    15655 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/strategies/test_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.681670 bofire-0.0.4/tests/bofire/surrogates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/surrogates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/surrogates/test_cross_validate.py
--rw-r--r--   0 runner    (1001) docker     (123)    13140 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/surrogates/test_diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/surrogates/test_feature_importance.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/surrogates/test_from_data_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/surrogates/test_fully_bayesian.py
--rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/surrogates/test_gps.py
--rw-r--r--   0 runner    (1001) docker     (123)     7702 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/surrogates/test_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/surrogates/test_random_forest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/surrogates/test_surrogates.py
--rw-r--r--   0 runner    (1001) docker     (123)    34238 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/surrogates/test_torch_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/test_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:38.656606 bofire-0.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:38.576605 bofire-0.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:38.580605 bofire-0.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-08-04 07:31:29.000000 bofire-0.0.5/.github/workflows/docs-build.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-08-04 07:31:29.000000 bofire-0.0.5/.github/workflows/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-08-04 07:31:29.000000 bofire-0.0.5/.github/workflows/lint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-04 07:31:29.000000 bofire-0.0.5/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-08-04 07:31:29.000000 bofire-0.0.5/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-08-04 07:31:29.000000 bofire-0.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-08-04 07:31:29.000000 bofire-0.0.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-08-04 07:31:29.000000 bofire-0.0.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-08-04 07:31:29.000000 bofire-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-08-04 07:31:38.656606 bofire-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-08-04 07:31:29.000000 bofire-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:38.584605 bofire-0.0.5/bofire/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:38.584605 bofire-0.0.5/bofire/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/benchmarks/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8065 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/benchmarks/aspen_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/benchmarks/benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:38.584605 bofire-0.0.5/bofire/benchmarks/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/benchmarks/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8591 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/benchmarks/data/aniline_cn_crosscoupling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/benchmarks/hyperopt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21299 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/benchmarks/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12171 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/benchmarks/single.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:38.584605 bofire-0.0.5/bofire/data_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:38.584605 bofire-0.0.5/bofire/data_models/acquisition_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/acquisition_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/acquisition_functions/acquisition_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/acquisition_functions/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:38.584605 bofire-0.0.5/bofire/data_models/constraints/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/constraints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/constraints/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/constraints/constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7039 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/constraints/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/constraints/nchoosek.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/constraints/nonlinear.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:38.588605 bofire-0.0.5/bofire/data_models/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/domain/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/domain/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26982 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/domain/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28757 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/domain/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/enum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:38.588605 bofire-0.0.5/bofire/data_models/features/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/features/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14127 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/features/categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/features/continuous.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10185 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/features/descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/features/discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/features/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/features/molecular.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/features/numerical.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:38.592605 bofire-0.0.5/bofire/data_models/kernels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/kernels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/kernels/aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/kernels/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/kernels/categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/kernels/continuous.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/kernels/kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/kernels/molecular.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:38.592605 bofire-0.0.5/bofire/data_models/molfeatures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/molfeatures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/molfeatures/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/molfeatures/molfeatures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28410 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/molfeatures/names.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:38.592605 bofire-0.0.5/bofire/data_models/objectives/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/objectives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/objectives/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/objectives/identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/objectives/objective.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/objectives/sigmoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/objectives/target.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:38.592605 bofire-0.0.5/bofire/data_models/outlier_detection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/outlier_detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/outlier_detection/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/outlier_detection/outlier_detection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:38.596605 bofire-0.0.5/bofire/data_models/priors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/priors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/priors/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/priors/gamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/priors/normal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/priors/prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:38.596605 bofire-0.0.5/bofire/data_models/strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/strategies/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/strategies/doe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/strategies/factorial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:38.600605 bofire-0.0.5/bofire/data_models/strategies/predictives/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/strategies/predictives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/strategies/predictives/botorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/strategies/predictives/multiobjective.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/strategies/predictives/predictive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/strategies/predictives/qehvi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/strategies/predictives/qnehvi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/strategies/predictives/qparego.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/strategies/predictives/sobo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/strategies/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:38.600605 bofire-0.0.5/bofire/data_models/strategies/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/strategies/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/strategies/samplers/polytope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/strategies/samplers/rejection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/strategies/samplers/sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:38.600605 bofire-0.0.5/bofire/data_models/strategies/stepwise/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/strategies/stepwise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/strategies/stepwise/conditions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/strategies/stepwise/stepwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/strategies/strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:38.604605 bofire-0.0.5/bofire/data_models/surrogates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/surrogates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/surrogates/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/surrogates/botorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/surrogates/botorch_surrogates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/surrogates/empirical.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/surrogates/fully_bayesian.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/surrogates/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/surrogates/mixed_single_task_gp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/surrogates/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/surrogates/random_forest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/surrogates/scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/surrogates/single_task_gp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/surrogates/surrogate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/surrogates/tanimoto_gp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/surrogates/trainable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/surrogates/xgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/unions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/data_models/validated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:38.604605 bofire-0.0.5/bofire/kernels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/kernels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/kernels/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:38.604605 bofire-0.0.5/bofire/kernels/fingerprint_kernels/
+-rw-r--r--   0 runner    (1001) docker     (123)     5308 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/kernels/fingerprint_kernels/base_fingerprint_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/kernels/fingerprint_kernels/tanimoto_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/kernels/mapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:38.604605 bofire-0.0.5/bofire/outlier_detection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/outlier_detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/outlier_detection/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/outlier_detection/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/outlier_detection/outlier_detection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:38.608605 bofire-0.0.5/bofire/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/plot/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/plot/feature_importance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/plot/objective.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/plot/prior.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:38.608605 bofire-0.0.5/bofire/priors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/priors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/priors/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/priors/mapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:38.608605 bofire-0.0.5/bofire/strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/strategies/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:38.612605 bofire-0.0.5/bofire/strategies/data_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/strategies/data_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/strategies/data_models/candidate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/strategies/data_models/values.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:38.612605 bofire-0.0.5/bofire/strategies/doe/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/strategies/doe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9511 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/strategies/doe/design.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16789 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/strategies/doe/objective.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18121 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/strategies/doe/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/strategies/doe_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/strategies/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/strategies/factorial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/strategies/mapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:38.612605 bofire-0.0.5/bofire/strategies/predictives/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/strategies/predictives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19396 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/strategies/predictives/botorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/strategies/predictives/predictive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/strategies/predictives/qehvi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/strategies/predictives/qnehvi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/strategies/predictives/qparego.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7195 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/strategies/predictives/sobo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/strategies/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:38.612605 bofire-0.0.5/bofire/strategies/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/strategies/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6764 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/strategies/samplers/polytope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/strategies/samplers/rejection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/strategies/samplers/sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:38.616605 bofire-0.0.5/bofire/strategies/stepwise/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/strategies/stepwise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/strategies/stepwise/conditions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/strategies/stepwise/stepwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8487 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/strategies/strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:38.620605 bofire-0.0.5/bofire/surrogates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/surrogates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/surrogates/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/surrogates/botorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/surrogates/botorch_surrogates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/surrogates/cloudpickle_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15855 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/surrogates/diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/surrogates/empirical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/surrogates/feature_importance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/surrogates/fully_bayesian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/surrogates/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/surrogates/mixed_single_task_gp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/surrogates/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/surrogates/random_forest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/surrogates/single_task_gp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/surrogates/surrogate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7771 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/surrogates/trainable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/surrogates/values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/surrogates/xgb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:38.620605 bofire-0.0.5/bofire/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/utils/cheminformatics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/utils/doe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/utils/multiobjective.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15571 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/utils/reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/utils/subdomain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/utils/tmpfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15517 2023-08-04 07:31:29.000000 bofire-0.0.5/bofire/utils/torch_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-04 07:31:38.000000 bofire-0.0.5/bofire/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:38.584605 bofire-0.0.5/bofire.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-08-04 07:31:38.000000 bofire-0.0.5/bofire.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12134 2023-08-04 07:31:38.000000 bofire-0.0.5/bofire.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 07:31:38.000000 bofire-0.0.5/bofire.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-08-04 07:31:38.000000 bofire-0.0.5/bofire.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-04 07:31:38.000000 bofire-0.0.5/bofire.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:38.628605 bofire-0.0.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)  1133101 2023-08-04 07:31:29.000000 bofire-0.0.5/docs/basic_examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-08-04 07:31:29.000000 bofire-0.0.5/docs/data_models_functionals.md
+-rw-r--r--   0 runner    (1001) docker     (123)   128161 2023-08-04 07:31:29.000000 bofire-0.0.5/docs/design_with_explicit_formula.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-08-04 07:31:29.000000 bofire-0.0.5/docs/examples.md
+-rw-r--r--   0 runner    (1001) docker     (123)   573008 2023-08-04 07:31:29.000000 bofire-0.0.5/docs/getting_started.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-08-04 07:31:29.000000 bofire-0.0.5/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-08-04 07:31:29.000000 bofire-0.0.5/docs/install.md
+-rw-r--r--   0 runner    (1001) docker     (123)    25540 2023-08-04 07:31:29.000000 bofire-0.0.5/docs/nchoosek_constraint.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   212106 2023-08-04 07:31:29.000000 bofire-0.0.5/docs/optimality_criteria.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-04 07:31:29.000000 bofire-0.0.5/docs/ref-constraints.md
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-04 07:31:29.000000 bofire-0.0.5/docs/ref-domain-util.md
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-04 07:31:29.000000 bofire-0.0.5/docs/ref-domain.md
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-04 07:31:29.000000 bofire-0.0.5/docs/ref-features.md
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-04 07:31:29.000000 bofire-0.0.5/docs/ref-mappers.md
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-04 07:31:29.000000 bofire-0.0.5/docs/ref-objectives.md
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-04 07:31:29.000000 bofire-0.0.5/docs/ref-utils.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:38.580605 bofire-0.0.5/graphics/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:38.628605 bofire-0.0.5/graphics/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)   106480 2023-08-04 07:31:29.000000 bofire-0.0.5/graphics/tutorials/aspen_benchmark_flowsheet.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-08-04 07:31:29.000000 bofire-0.0.5/mkdocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-08-04 07:31:29.000000 bofire-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-04 07:31:29.000000 bofire-0.0.5/pyrightconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:38.628605 bofire-0.0.5/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-08-04 07:31:29.000000 bofire-0.0.5/scripts/run_tutorials.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 07:31:38.656606 bofire-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-08-04 07:31:29.000000 bofire-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:38.628605 bofire-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:38.628605 bofire-0.0.5/tests/bofire/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:38.628605 bofire-0.0.5/tests/bofire/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/benchmarks/test_aspen_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/benchmarks/test_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/benchmarks/test_hyperopt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/benchmarks/test_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/benchmarks/test_single.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:38.636605 bofire-0.0.5/tests/bofire/data_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/data_models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:38.636605 bofire-0.0.5/tests/bofire/data_models/serialization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/data_models/serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/data_models/serialization/test_deserialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/data_models/serialization/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/data_models/serialization/test_serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:38.640606 bofire-0.0.5/tests/bofire/data_models/specs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/data_models/specs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/data_models/specs/acquisition_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/data_models/specs/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/data_models/specs/conditions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/data_models/specs/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/data_models/specs/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/data_models/specs/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/data_models/specs/kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/data_models/specs/molfeatures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/data_models/specs/objectives.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/data_models/specs/outlier_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/data_models/specs/priors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/data_models/specs/specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/data_models/specs/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/data_models/specs/surrogates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/data_models/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/data_models/test_constraint_fulfillment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6499 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/data_models/test_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22806 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/data_models/test_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10465 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/data_models/test_domain_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68677 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/data_models/test_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7296 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/data_models/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6955 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/data_models/test_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20979 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/data_models/test_molecular.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/data_models/test_molfeatures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/data_models/test_nchoosek_combinatorics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/data_models/test_nonlinear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/data_models/test_numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/data_models/test_priors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/data_models/test_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/data_models/test_unions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7296 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/data_models/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:38.640606 bofire-0.0.5/tests/bofire/outlier_detection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/outlier_detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/outlier_detection/test_outlier_detection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:38.640606 bofire-0.0.5/tests/bofire/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/plot/test_plot_feature_importance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/plot/test_plot_objective.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/plot/test_plot_prior.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:38.640606 bofire-0.0.5/tests/bofire/priors/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/priors/test_priors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:38.644605 bofire-0.0.5/tests/bofire/strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/strategies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:38.644605 bofire-0.0.5/tests/bofire/strategies/doe/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/strategies/doe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15123 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/strategies/doe/test_design.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20427 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/strategies/doe/test_objective.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21976 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/strategies/doe/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/strategies/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10648 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/strategies/specs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:38.644605 bofire-0.0.5/tests/bofire/strategies/stepwise/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/strategies/stepwise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/strategies/stepwise/test_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/strategies/stepwise/test_stepwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/strategies/test_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/strategies/test_ask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27144 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/strategies/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6072 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/strategies/test_doe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/strategies/test_factorial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/strategies/test_from_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/strategies/test_model_specs_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8383 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/strategies/test_qehvi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/strategies/test_qparego.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/strategies/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8633 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/strategies/test_sobo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15649 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/strategies/test_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:38.648605 bofire-0.0.5/tests/bofire/surrogates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/surrogates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/surrogates/test_cross_validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13560 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/surrogates/test_diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/surrogates/test_feature_importance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/surrogates/test_from_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/surrogates/test_fully_bayesian.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16129 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/surrogates/test_gps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/surrogates/test_linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/surrogates/test_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/surrogates/test_random_forest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/surrogates/test_surrogates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34120 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/surrogates/test_torch_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/surrogates/test_xgb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:38.652605 bofire-0.0.5/tests/bofire/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     7994 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/utils/test_cheminformatics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/utils/test_doe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7533 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/utils/test_multiobjective.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18666 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/utils/test_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23591 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/bofire/utils/test_torch_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-08-04 07:31:29.000000 bofire-0.0.5/tests/test_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:38.652605 bofire-0.0.5/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-08-04 07:31:29.000000 bofire-0.0.5/tutorials/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:38.652605 bofire-0.0.5/tutorials/basic_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    42310 2023-08-04 07:31:29.000000 bofire-0.0.5/tutorials/basic_examples/Model_Fitting_and_analysis.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    67375 2023-08-04 07:31:29.000000 bofire-0.0.5/tutorials/basic_examples/Reaction_Optimization_Example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-08-04 07:31:29.000000 bofire-0.0.5/tutorials/basic_examples/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:38.656606 bofire-0.0.5/tutorials/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-08-04 07:31:29.000000 bofire-0.0.5/tutorials/benchmarks/001-Himmelblau.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    49045 2023-08-04 07:31:29.000000 bofire-0.0.5/tutorials/benchmarks/002-DTLZ2.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    16870 2023-08-04 07:31:29.000000 bofire-0.0.5/tutorials/benchmarks/004-Aspen_benchmark.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11109 2023-08-04 07:31:29.000000 bofire-0.0.5/tutorials/benchmarks/005-Hartmann_with_nchoosek.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-08-04 07:31:29.000000 bofire-0.0.5/tutorials/benchmarks/006-30dimBranin.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:31:38.656606 bofire-0.0.5/tutorials/doe/
+-rw-r--r--   0 runner    (1001) docker     (123)  1133101 2023-08-04 07:31:29.000000 bofire-0.0.5/tutorials/doe/basic_examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   128161 2023-08-04 07:31:29.000000 bofire-0.0.5/tutorials/doe/design_with_explicit_formula.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    25540 2023-08-04 07:31:29.000000 bofire-0.0.5/tutorials/doe/nchoosek_constraint.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   212106 2023-08-04 07:31:29.000000 bofire-0.0.5/tutorials/doe/optimality_criteria.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   573008 2023-08-04 07:31:29.000000 bofire-0.0.5/tutorials/getting_started.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    31710 2023-08-04 07:31:29.000000 bofire-0.0.5/tutorials/models_serial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6256 2023-08-04 07:31:29.000000 bofire-0.0.5/tutorials/random_forest_in_bofire.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    20095 2023-08-04 07:31:29.000000 bofire-0.0.5/tutorials/strategies_serial.ipynb
```

### Comparing `bofire-0.0.4/LICENSE` & `bofire-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/PKG-INFO` & `bofire-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: bofire
-Version: 0.0.4
+Version: 0.0.5
 Home-page: https://github.com/experimental-design/bofire
 Author: 
 License: BSD-3
 Keywords: Bayesian optimization,Multi-objective optimization,Experimental design
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: optimization
+Provides-Extra: xgb
 Provides-Extra: cheminfo
 Provides-Extra: tests
 Provides-Extra: docs
 License-File: LICENSE
 
 # BoFire
```

### Comparing `bofire-0.0.4/README.md` & `bofire-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/bofire/benchmarks/aspen_benchmark.py` & `bofire-0.0.5/bofire/benchmarks/aspen_benchmark.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     """
 
     def __init__(
         self,
         filename: str,
         domain: Domain,
         paths: Dict[str, str],
-        additional_output_keys: List = [],
+        additional_output_keys: Optional[List] = None,
         translate_into_aspen_readable: Optional[
             Callable[[Domain, pd.DataFrame], pd.DataFrame]
         ] = None,
     ) -> None:
         """Initializes Aspen_benchmark. A class that connects to Aspen plus.
 
         Args:
@@ -56,15 +56,15 @@
         if os.path.exists(filename):
             self.filename = filename
         else:
             raise ValueError("Unable to find Aspen file " + filename)
 
         self.translate_into_aspen_readable = translate_into_aspen_readable
         self._domain = domain
-        self.additional_output_keys = additional_output_keys
+        self.additional_output_keys = additional_output_keys or []
 
         for key in self.domain.get_feature_keys():
             # Check, if every input and output variable has a path to Aspen provided.
             if key not in paths.keys():
                 raise ValueError("Path for " + key + " is not provided.")
 
         self.paths = paths
```

### Comparing `bofire-0.0.4/bofire/benchmarks/benchmark.py` & `bofire-0.0.5/bofire/benchmarks/benchmark.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/bofire/benchmarks/data/aniline_cn_crosscoupling.py` & `bofire-0.0.5/bofire/benchmarks/data/aniline_cn_crosscoupling.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/bofire/benchmarks/multi.py` & `bofire-0.0.5/bofire/benchmarks/multi.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,20 +170,22 @@
 
 
 class SnarBenchmark(Benchmark):
     """Nucleophilic aromatic substitution problem as a multiobjective test function for optimization algorithms.
     Solving of a differential equation system with varying intitial values.
     """
 
-    def __init__(self, C_i: Optional[np.ndarray] = np.ndarray((1, 1))):
+    def __init__(self, C_i: Optional[np.ndarray] = None):
         """Initializes multiobjective test function object of type SnarBenchmark.
 
         Args:
             C_i (Optional[np.ndarray]): Input concentrations. Defaults to [1, 1]
         """
+        if C_i is None:
+            C_i = np.array([1, 1])
         self.C_i = C_i
 
         # Decision variables
         # "residence time in minutes"
         inputs = [
             ContinuousInput(key="tau", bounds=(0.5, 2)),
             # "equivalents of pyrrolidine"
@@ -220,15 +222,15 @@
             candidates (pd.DataFrame): Input vector. Columns: tau, equiv_pldn, conc_dfnb, temperature
 
         Returns:
             pd.DataFrame: Output vector. Columns: sty, e_factor
         """
         stys = []
         e_factors = []
-        for i, candidate in candidates.iterrows():
+        for _, candidate in candidates.iterrows():
             tau = float(candidate["tau"])
             equiv_pldn = float(candidate["equiv_pldn"])
             conc_dfnb = float(candidate["conc_dfnb"])
             T = float(candidate["temperature"])
             y, e_factor, res = self._integrate_equations(tau, equiv_pldn, conc_dfnb, T)
             stys.append(y)
             e_factors.append(e_factor)
@@ -293,19 +295,18 @@
 
     def _integrand(self, t, C, T):
         # Kinetic Constants
         R = 8.314 / 1000  # kJ/K/mol
         T_ref = 90 + 273.71  # Convert to deg K
         T = T + 273.71  # Convert to deg K
         # Need to convert from 10^-2 M^-1s^-1 to M^-1min^-1
-        k = (
-            lambda k_ref, E_a, temp: 0.6
-            * k_ref
-            * np.exp(-E_a / R * (1 / temp - 1 / T_ref))
-        )
+
+        def k(k_ref, E_a, temp):
+            return 0.6 * k_ref * np.exp(-E_a / R * (1 / temp - 1 / T_ref))
+
         k_a = k(57.9, 33.3, T)
         k_b = k(2.70, 35.3, T)
         k_c = k(0.865, 38.9, T)
         k_d = k(1.63, 44.8, T)
 
         # Reaction Rates
         r = np.zeros(5)
@@ -452,19 +453,19 @@
             "base": CategoricalEncodingEnum.DESCRIPTOR,
         }
 
         # Objectives: yield and cost
         outputs = [
             ContinuousOutput(
                 key="yield",
-                objective=MaximizeObjective(w=1.0, lower_bound=0.0, upper_bound=1.0),
+                objective=MaximizeObjective(w=1.0, bounds=(0.0, 1.0)),
             ),
             ContinuousOutput(
                 key="cost",
-                objective=MinimizeObjective(w=1.0, lower_bound=0.0, upper_bound=1.0),
+                objective=MinimizeObjective(w=1.0, bounds=(0.0, 1.0)),
             ),
         ]
         self.ref_point = {"yield": 0.0, "cost": 1.0}
 
         self._domain = Domain(
             inputs=Inputs(features=inputs),
             outputs=Outputs(features=outputs),
@@ -474,15 +475,15 @@
 
         data = data.rename(columns={"base_equivalents": "base_eq", "yld": "yield"})
         data["valid_yield"] = 1
 
         data_model = SingleTaskGPSurrogate(
             inputs=Inputs(features=inputs),
             outputs=Outputs(features=[outputs[0]]),
-            input_preprocessing_specs=input_preprocessing_specs,
+            input_preprocessing_specs=input_preprocessing_specs,  # type: ignore
         )
         ground_truth_yield = surrogates.map(data_model)
 
         ground_truth_yield.fit(experiments=data)  # type: ignore
         self.ground_truth_yield = ground_truth_yield
 
     def _f(self, candidates: pd.DataFrame) -> pd.DataFrame:
```

### Comparing `bofire-0.0.4/bofire/benchmarks/single.py` & `bofire-0.0.5/bofire/benchmarks/single.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         num_categories: PositiveInt = 3,
         categorical: bool = False,
         descriptor: bool = False,
         dim: PositiveInt = 2,
         lower: float = -32.768,
         upper: float = 32.768,
         best_possible_f: float = 0.0,
-        evaluated_points=[],
+        evaluated_points: Optional[list] = None,
     ):
         """Initializes benchmark function of type Ackley.
 
         Args:
             num_categories (PositiveInt, optional): Number of categories. Defaults to 3.
             categorical (bool, optional): Use categorical inputs. Defaults to False.
             descriptor (bool, optional): Use descriptive inputs. Defaults to False.
@@ -70,14 +70,16 @@
         self.num_categories = num_categories
         self.categorical = categorical
         self.descriptor = descriptor
         self.dim = dim
         self.lower = lower
         self.upper = upper
         self.best_possible_f = best_possible_f
+        if evaluated_points is None:
+            evaluated_points = []
         self.evaluated_points = evaluated_points
 
         input_feature_list = []
         # Decision variables
         if self.categorical:
             input_feature_list.append(
                 CategoricalInput(
```

### Comparing `bofire-0.0.4/bofire/data_models/acquisition_functions/acquisition_function.py` & `bofire-0.0.5/bofire/data_models/acquisition_functions/acquisition_function.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/bofire/data_models/api.py` & `bofire-0.0.5/bofire/data_models/api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,61 +1,69 @@
 from bofire.data_models import unions
-from bofire.data_models.acquisition_functions.api import (  # noqa: F401
+from bofire.data_models.acquisition_functions.api import (
     AcquisitionFunction,
     AnyAcquisitionFunction,
 )
-from bofire.data_models.constraints.api import AnyConstraint, Constraint  # noqa: F401
-from bofire.data_models.domain.api import (  # noqa: F401
-    Domain,
-    Features,
-    Inputs,
-    Outputs,
-)
-from bofire.data_models.features.api import (  # noqa: F401
+from bofire.data_models.constraints.api import AnyConstraint, Constraint
+from bofire.data_models.domain.api import Domain, Features, Inputs, Outputs
+from bofire.data_models.features.api import (
     AnyFeature,
     AnyInput,
     AnyOutput,
     Feature,
     Input,
     Output,
 )
 
 try:
     # in case of the minimal installation these import are not available
-    from bofire.data_models.kernels.api import AnyKernel, Kernel  # noqa: F401
-    from bofire.data_models.objectives.api import AnyObjective, Objective  # noqa: F401
-    from bofire.data_models.priors.api import AnyPrior, Prior  # noqa: F401
-    from bofire.data_models.strategies.api import (  # noqa: F401
+    from bofire.data_models.kernels.api import AnyKernel, Kernel
+    from bofire.data_models.molfeatures.api import (  # noqa: F401
+        AnyMolFeatures,
+        MolFeatures,
+    )
+    from bofire.data_models.objectives.api import AnyObjective, Objective
+    from bofire.data_models.outlier_detection.api import (
+        AnyOutlierDetection,
+        OutlierDetection,
+    )
+    from bofire.data_models.priors.api import AnyPrior, Prior
+    from bofire.data_models.strategies.api import (
+        AnyCondition,
         AnyPredictive,
         AnySampler,
         AnyStrategy,
         PredictiveStrategy,
         SamplerStrategy,
         Strategy,
     )
-    from bofire.data_models.surrogates.api import (  # noqa: F401
+    from bofire.data_models.surrogates.api import (
         AnyBotorchSurrogate,
         AnySurrogate,
         BotorchSurrogate,
         Surrogate,
     )
 
     data_model_list = [
         AnyAcquisitionFunction,
         AnyConstraint,
         AnyFeature,
         AnyKernel,
         AnySurrogate,
+        AnyOutlierDetection,
         AnyObjective,
         AnyPrior,
         AnyStrategy,
+        AnyMolFeatures,
         Domain,
     ]
 except ImportError:
     data_model_list = [
         AnyAcquisitionFunction,
         AnyConstraint,
         AnyFeature,
         Domain,
     ]
 
 AnyThing = [model for models in data_model_list for model in unions.to_list(models)]
+
+AnyThing = [model for models in data_model_list for model in unions.to_list(models)]
```

### Comparing `bofire-0.0.4/bofire/data_models/base.py` & `bofire-0.0.5/bofire/data_models/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import collections.abc as collections
 from typing import Any, Callable, List, Sequence, Type, Union, get_args, get_origin
 
 import pandas as pd
 from pydantic import BaseModel as PydanticBaseModel
+from pydantic import Extra
 
 
 class BaseModel(PydanticBaseModel):
     class Config:
-        # TODO: forbid extra fields in data models
-        # extra = "forbid"
         validate_assignment = True
         arbitrary_types_allowed = False
         copy_on_model_validation = "none"
+        extra = Extra.forbid
+
         json_encoders = {
             pd.DataFrame: lambda x: x.to_dict(orient="list"),
             pd.Series: lambda x: x.to_list(),
         }
 
 
 def filter_by_attribute(
```

### Comparing `bofire-0.0.4/bofire/data_models/constraints/api.py` & `bofire-0.0.5/bofire/data_models/constraints/api.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 from typing import Union
 
-from bofire.data_models.constraints.constraint import Constraint
+from bofire.data_models.constraints.constraint import (
+    Constraint,
+    ConstraintError,
+    ConstraintNotFulfilledError,
+)
 from bofire.data_models.constraints.linear import (
     LinearConstraint,
     LinearEqualityConstraint,
     LinearInequalityConstraint,
 )
 from bofire.data_models.constraints.nchoosek import NChooseKConstraint
 from bofire.data_models.constraints.nonlinear import (
@@ -22,7 +26,11 @@
 AnyConstraint = Union[
     LinearEqualityConstraint,
     LinearInequalityConstraint,
     NonlinearEqualityConstraint,
     NonlinearInequalityConstraint,
     NChooseKConstraint,
 ]
+
+AnyConstraintError = Union[ConstraintError, ConstraintNotFulfilledError]
+
+# %%
```

### Comparing `bofire-0.0.4/bofire/data_models/constraints/constraint.py` & `bofire-0.0.5/bofire/data_models/constraints/constraint.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from abc import abstractmethod
-from typing import Annotated, List, Optional
+from typing import List, Optional
 
 import pandas as pd
 from pydantic import Field
+from typing_extensions import Annotated
 
 from bofire.data_models.base import BaseModel
 
 
 class Constraint(BaseModel):
     """Abstract base class to define constraints on the optimization space."""
 
@@ -47,9 +48,21 @@
             experiments (pd.DataFrame): Dataframe to evaluate the constraint on.
         Returns:
             pd.DataFrame: the i-th row contains the jacobian evaluated at the i-th experiment
         """
         pass
 
 
+class ConstraintError(Exception):
+    """Base Error for Constraints"""
+
+    pass
+
+
+class ConstraintNotFulfilledError(ConstraintError):
+    """Raised when an constraint is not fulfilled."""
+
+    pass
+
+
 FeatureKeys = Annotated[List[str], Field(min_items=2)]
 Coefficients = Annotated[List[float], Field(min_items=2)]
```

### Comparing `bofire-0.0.4/bofire/data_models/constraints/linear.py` & `bofire-0.0.5/bofire/data_models/constraints/linear.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/bofire/data_models/constraints/nchoosek.py` & `bofire-0.0.5/bofire/data_models/constraints/nchoosek.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/bofire/data_models/constraints/nonlinear.py` & `bofire-0.0.5/bofire/data_models/constraints/nonlinear.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,61 @@
+import warnings
 from typing import Literal, Optional
 
 import numpy as np
 import pandas as pd
+from pydantic import validator
 
 from bofire.data_models.constraints.constraint import Constraint, FeatureKeys
 
 
 class NonlinearConstraint(Constraint):
     """Base class for nonlinear equality and inequality constraints.
 
     Attributes:
         expression (str): Mathematical expression that can be evaluated by `pandas.eval`.
         jacobian_expression (str): Mathematical expression that that can be evaluated by `pandas.eval`.
         features (list): list of feature keys (str) on which the constraint works on.
     """
 
     expression: str
-    jacobian_expression: Optional[str] = None
     features: Optional[FeatureKeys] = None
+    jacobian_expression: Optional[str] = None
+
+    @validator("jacobian_expression", always=True)
+    def set_jacobian_expression(cls, jacobian_expression, values):
+        try:
+            import sympy  # type: ignore
+        except ImportError as e:
+            warnings.warn(e.msg)
+            warnings.warn("please run `pip install sympy` for this functionality.")
+            return jacobian_expression
+
+        if (
+            jacobian_expression is None
+            and "features" in values
+            and "expression" in values
+        ):
+            if values["features"] is not None:
+                return (
+                    "["
+                    + ", ".join(
+                        [
+                            str(sympy.S(values["expression"]).diff(key))
+                            for key in values["features"]
+                        ]
+                    )
+                    + "]"
+                )
+        return jacobian_expression
 
     def __call__(self, experiments: pd.DataFrame) -> pd.Series:
         return experiments.eval(self.expression)
 
     def jacobian(self, experiments: pd.DataFrame) -> pd.DataFrame:
-
         if self.jacobian_expression is not None:
             res = experiments.eval(self.jacobian_expression)
             for i, col in enumerate(res):
                 if not hasattr(col, "__iter__"):
                     res[i] = pd.Series(np.repeat(col, experiments.shape[0]))
 
             if self.features is not None:
```

### Comparing `bofire-0.0.4/bofire/data_models/domain/constraints.py` & `bofire-0.0.5/bofire/data_models/domain/constraints.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/bofire/data_models/domain/domain.py` & `bofire-0.0.5/bofire/data_models/domain/domain.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import collections.abc
 import itertools
+import warnings
 from typing import (
     Any,
     Dict,
     List,
     Literal,
     Optional,
     Sequence,
@@ -17,14 +18,15 @@
 import numpy as np
 import pandas as pd
 from pydantic import Field, validator
 
 from bofire.data_models.base import BaseModel
 from bofire.data_models.constraints.api import (
     AnyConstraint,
+    ConstraintNotFulfilledError,
     LinearConstraint,
     NChooseKConstraint,
 )
 from bofire.data_models.domain.constraints import Constraints
 from bofire.data_models.domain.features import Features, Inputs, Outputs
 from bofire.data_models.features.api import (
     AnyInput,
@@ -301,15 +303,15 @@
             used_features_list = []
 
             if exhaustive:
                 for n in range(con.min_count, con.max_count + 1):
                     used_features_list.extend(itertools.combinations(con.features, n))
 
                 if con.none_also_valid:
-                    used_features_list.append(tuple([]))
+                    used_features_list.append(())
             else:
                 used_features_list.extend(
                     itertools.combinations(con.features, con.max_count)
                 )
 
             used_features_list_all.append(used_features_list)
 
@@ -493,15 +495,14 @@
             f"valid_{output_feature_key}"
             for output_feature_key in self.get_feature_keys(Output)
         ]
         for valid_key in valid_keys:
             if valid_key not in experiments:
                 experiments[valid_key] = True
         # check all cols
-        expected = feature_keys + valid_keys
         cols = list(experiments.columns)
         # we allow here for a column named labcode used to identify experiments
         if "labcode" in cols:
             # test that labcodes are not na
             if experiments.labcode.isnull().to_numpy().any():
                 raise ValueError("there are labcodes with null value")
             if experiments.labcode.isna().to_numpy().any():
@@ -510,18 +511,14 @@
             if (
                 len(set(experiments.labcode.to_numpy().tolist()))
                 != experiments.shape[0]
             ):
                 raise ValueError("labcodes are not unique")
             # we remove the labcode from the cols list to proceed as before
             cols.remove("labcode")
-        if len(expected) != len(cols):
-            raise ValueError(f"expected the following cols: `{expected}`, got `{cols}`")
-        if len(set(expected + cols)) != len(cols):
-            raise ValueError(f"expected the following cols: `{expected}`, got `{cols}`")
         # check values of continuous input features
         if experiments[self.get_feature_keys(Input)].isnull().to_numpy().any():
             raise ValueError("there are null values")
         if experiments[self.get_feature_keys(Input)].isna().to_numpy().any():
             raise ValueError("there are na values")
         # run the individual validators
         for feat in self.get_features(Input):
@@ -553,40 +550,50 @@
             preprocessed.shape[0],
         ]
         return pd.DataFrame.from_dict(
             data, orient="index", columns=["measured", "valid"]
         )
 
     def validate_candidates(
-        self, candidates: pd.DataFrame, only_inputs: bool = False, tol: float = 1e-5
+        self,
+        candidates: pd.DataFrame,
+        only_inputs: bool = False,
+        tol: float = 1e-5,
+        raise_validation_error: bool = True,
     ) -> pd.DataFrame:
         """Method to check the validty of porposed candidates
 
         Args:
             candidates (pd.DataFrame): Dataframe with suggested new experiments (candidates)
             only_inputs (bool,optional): If True, only the input columns are validated. Defaults to False.
             tol (float,optional): tolerance parameter for constraints. A constraint is considered as not fulfilled if the violation
                 is larger than tol. Defaults to 1e-6.
+            raise_validation_error (bool, optional): If true an error will be raised if candidates violate constraints,
+                otherwise only a warning will be displayed. Defaults to True.
 
         Raises:
             ValueError: when a column is missing for a defined input feature
             ValueError: when a column is missing for a defined output feature
             ValueError: when a non-numerical value is proposed
-            ValueError: when the constraints are not fulfilled
             ValueError: when an additional column is found
+            ConstraintNotFulfilledError: when the constraints are not fulfilled and `raise_validation_error = True`
 
         Returns:
             pd.DataFrame: dataframe with suggested experiments (candidates)
         """
         # check that each input feature has a col and is valid in itself
         assert isinstance(self.inputs, Inputs)
         self.inputs.validate_inputs(candidates)
         # check if all constraints are fulfilled
         if not self.constraints.is_fulfilled(candidates, tol=tol).all():
-            raise ValueError(f"Constraints not fulfilled: {candidates}")
+            if raise_validation_error:
+                raise ConstraintNotFulfilledError(
+                    f"Constraints not fulfilled: {candidates}"
+                )
+            warnings.warn("Not all constraints are fulfilled.")
         # for each continuous output feature with an attached objective object
         if not only_inputs:
             assert isinstance(self.outputs, Outputs)
 
             cols = list(
                 itertools.chain.from_iterable(
                     [
```

### Comparing `bofire-0.0.4/bofire/data_models/domain/features.py` & `bofire-0.0.5/bofire/data_models/domain/features.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,17 +18,19 @@
     AnyOutput,
     CategoricalDescriptorInput,
     CategoricalInput,
     ContinuousInput,
     ContinuousOutput,
     DiscreteInput,
     Input,
+    MolecularInput,
     Output,
     TInputTransformSpecs,
 )
+from bofire.data_models.molfeatures.api import MolFeatures
 from bofire.data_models.objectives.api import AbstractObjective, Objective
 
 FeatureSequence = Union[List[AnyFeature], Tuple[AnyFeature]]
 
 
 class Features(BaseModel):
     """Container of features, both input and output features are allowed.
@@ -249,15 +251,15 @@
 
     def validate_experiments(
         self, experiments: pd.DataFrame, strict=False
     ) -> pd.DataFrame:
         for feature in self:
             if feature.key not in experiments:
                 raise ValueError(f"no col for input feature `{feature.key}`")
-            feature.validate_experimental(experiments[feature.key], strict=strict)  # type: ignore
+            experiments[feature.key] = feature.validate_experimental(experiments[feature.key], strict=strict)  # type: ignore
         return experiments
 
     def get_categorical_combinations(
         self,
         include: Union[Type, List[Type]] = Input,
         exclude: Union[Type, List[Type]] = None,
     ):
@@ -344,14 +346,26 @@
                 features2idx[feat.key] = tuple(
                     (np.array(range(len(feat.descriptors))) + counter).tolist()
                 )
                 features2names[feat.key] = tuple(
                     [f"{feat.key}{_CAT_SEP}{d}" for d in feat.descriptors]
                 )
                 counter += len(feat.descriptors)
+            elif isinstance(specs[feat.key], MolFeatures):
+                assert isinstance(feat, MolecularInput)
+                descriptor_names = specs[
+                    feat.key
+                ].get_descriptor_names()  # type: ignore
+                features2idx[feat.key] = tuple(
+                    (np.array(range(len(descriptor_names))) + counter).tolist()
+                )
+                features2names[feat.key] = tuple(
+                    [f"{feat.key}{_CAT_SEP}{d}" for d in descriptor_names]
+                )
+                counter += len(descriptor_names)
         return features2idx, features2names
 
     def transform(
         self, experiments: pd.DataFrame, specs: TInputTransformSpecs
     ) -> pd.DataFrame:
         """Transform a dataframe to the represenation specified in `specs`.
 
@@ -379,14 +393,17 @@
                 transformed.append(feat.to_ordinal_encoding(s))
             elif specs[feat.key] == CategoricalEncodingEnum.DUMMY:
                 assert isinstance(feat, CategoricalInput)
                 transformed.append(feat.to_dummy_encoding(s))
             elif specs[feat.key] == CategoricalEncodingEnum.DESCRIPTOR:
                 assert isinstance(feat, CategoricalDescriptorInput)
                 transformed.append(feat.to_descriptor_encoding(s))
+            elif isinstance(specs[feat.key], MolFeatures):
+                assert isinstance(feat, MolecularInput)
+                transformed.append(feat.to_descriptor_encoding(specs[feat.key], s))  # type: ignore
         return pd.concat(transformed, axis=1)
 
     def inverse_transform(
         self, experiments: pd.DataFrame, specs: TInputTransformSpecs
     ) -> pd.DataFrame:
         """Transform a dataframe back to the original representations.
 
@@ -416,41 +433,65 @@
                 transformed.append(feat.from_ordinal_encoding(experiments[feat.key]))
             elif specs[feat.key] == CategoricalEncodingEnum.DUMMY:
                 assert isinstance(feat, CategoricalInput)
                 transformed.append(feat.from_dummy_encoding(experiments))
             elif specs[feat.key] == CategoricalEncodingEnum.DESCRIPTOR:
                 assert isinstance(feat, CategoricalDescriptorInput)
                 transformed.append(feat.from_descriptor_encoding(experiments))
+
         return pd.concat(transformed, axis=1)
 
     def _validate_transform_specs(self, specs: TInputTransformSpecs):
         """Checks the validity of the transform specs .
 
         Args:
             specs (TInputTransformSpecs): Transform specs to be validated.
         """
         # first check that the keys in the specs dict are correct also correct feature keys
-        if len(set(specs.keys()) - set(self.get_keys(CategoricalInput))) > 0:
+        if (
+            len(
+                set(specs.keys())
+                - set(self.get_keys(CategoricalInput))
+                - set(self.get_keys(MolecularInput))
+            )
+            > 0
+        ):
             raise ValueError("Unknown features specified in transform specs.")
-        # next check that all values are of type CategoricalEncodingEnum
+        # next check that all values are of type CategoricalEncodingEnum or MolFeatures
         if not (
-            all([isinstance(enc, CategoricalEncodingEnum) for enc in specs.values()])
+            all(
+                isinstance(enc, (CategoricalEncodingEnum, MolFeatures))
+                for enc in specs.values()
+            )
         ):
             raise ValueError("Unknown transform specified.")
-        # next check that only Categoricalwithdescriptor have the value DESCRIPTOR
-        descriptor_keys = [
-            key
-            for key, value in specs.items()
-            if value == CategoricalEncodingEnum.DESCRIPTOR
-        ]
+        # next check that only CategoricalDescriptorInput can have the value DESCRIPTOR
+        descriptor_keys = []
+        for key, value in specs.items():
+            if value == CategoricalEncodingEnum.DESCRIPTOR:
+                descriptor_keys.append(key)
         if (
             len(set(descriptor_keys) - set(self.get_keys(CategoricalDescriptorInput)))
             > 0
         ):
             raise ValueError("Wrong features types assigned to DESCRIPTOR transform.")
+        # next check if MolFeatures have been assigned to feature types other than MolecularInput
+        molfeature_keys = []
+        for key, value in specs.items():
+            if isinstance(value, MolFeatures):
+                molfeature_keys.append(key)
+        if len(set(molfeature_keys) - set(self.get_keys(MolecularInput))) > 0:
+            raise ValueError("Wrong features types assigned to MolFeatures transforms.")
+        # next check that all MolecularInput have MolFeatures transforms
+        for feat in self.get(includes=[MolecularInput]):
+            mol_encoding = specs.get(feat.key)
+            if mol_encoding is None:
+                raise ValueError("No transform assigned to MolecularInput.")
+            elif not isinstance(mol_encoding, MolFeatures):
+                raise ValueError("Incorrect transform assigned to MolecularInput.")
         return specs
 
     def get_bounds(
         self,
         specs: TInputTransformSpecs,
         experiments: Optional[pd.DataFrame] = None,
     ) -> Tuple[List[float], List[float]]:
@@ -473,20 +514,20 @@
         """
         self._validate_transform_specs(specs=specs)
 
         lower = []
         upper = []
 
         for feat in self.get():
-            l, u = feat.get_bounds(  # type: ignore
+            lo, up = feat.get_bounds(  # type: ignore
                 transform_type=specs.get(feat.key),  # type: ignore
-                values=experiments[feat.key] if experiments is not None else None,
+                values=experiments[feat.key] if experiments is not None else None,  # type: ignore
             )
-            lower += l
-            upper += u
+            lower += lo
+            upper += up
         return lower, upper
 
 
 class Outputs(Features):
     """Container of output features, only output features are allowed.
 
     Attributes:
```

### Comparing `bofire-0.0.4/bofire/data_models/enum.py` & `bofire-0.0.5/bofire/data_models/enum.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/bofire/data_models/features/api.py` & `bofire-0.0.5/bofire/data_models/features/api.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/bofire/data_models/features/categorical.py` & `bofire-0.0.5/bofire/data_models/features/categorical.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-from typing import Annotated, ClassVar, Dict, List, Literal, Optional, Tuple, Union
+from typing import ClassVar, Dict, List, Literal, Optional, Tuple, Union
 
 import numpy as np
 import pandas as pd
 from pydantic import Field, root_validator, validator
+from typing_extensions import Annotated
 
 from bofire.data_models.enum import CategoricalEncodingEnum
 from bofire.data_models.features.feature import (
     _CAT_SEP,
     Input,
     Output,
     TAllowedVals,
@@ -38,15 +39,15 @@
 
         Raises:
             ValueError: when categories have non-unique names
 
         Returns:
             List[str]: List of the categories
         """
-        categories = [name for name in categories]
+        categories = list(categories)
         if len(categories) != len(set(categories)):
             raise ValueError("categories must be unique")
         return categories
 
     @root_validator(pre=False, skip_on_failure=True)
     def init_allowed(cls, values):
         """validates the list of allowed/not allowed categories
@@ -128,14 +129,15 @@
         Raises:
             ValueError: when an entry is not in the list of allowed categories
             ValueError: when there is no variation in a feature provided by the experimental data
 
         Returns:
             pd.Series: A dataFrame with experiments
         """
+        values = values.map(str)
         if sum(values.isin(self.categories)) != len(values):
             raise ValueError(
                 f"invalid values for `{self.key}`, allowed are: `{self.categories}`"
             )
         if strict:
             possible_categories = self.get_possible_categories(values)
             if len(possible_categories) != len(self.categories):
@@ -176,17 +178,15 @@
 
         Args:
             values (pd.Series): Series with the values for this feature
 
         Returns:
             list: list of possible categories
         """
-        return sorted(
-            list(set(list(set(values.tolist())) + self.get_allowed_categories()))
-        )
+        return sorted(set(list(set(values.tolist())) + self.get_allowed_categories()))
 
     def to_onehot_encoding(self, values: pd.Series) -> pd.DataFrame:
         """Converts values to a one-hot encoding.
 
         Args:
             values (pd.Series): Series to be transformed.
 
@@ -214,15 +214,15 @@
         cat_cols = [f"{self.key}{_CAT_SEP}{c}" for c in self.categories]
         # we allow here explicitly that the dataframe can have more columns than needed to have it
         # easier in the backtransform.
         if np.any([c not in values.columns for c in cat_cols]):
             raise ValueError(
                 f"{self.key}: Column names don't match categorical levels: {values.columns}, {cat_cols}."
             )
-        s = values[cat_cols].idxmax(1).str.split(_CAT_SEP, expand=True)[1]
+        s = values[cat_cols].idxmax(1).str.split(_CAT_SEP, expand=True).iloc[:, -1]
         s.name = self.key
         return s
 
     def to_dummy_encoding(self, values: pd.Series) -> pd.DataFrame:
         """Converts values to a dummy-hot encoding, dropping the first categorical level.
 
         Args:
@@ -254,15 +254,15 @@
         # easier in the backtransform.
         if np.any([c not in values.columns for c in cat_cols[1:]]):
             raise ValueError(
                 f"{self.key}: Column names don't match categorical levels: {values.columns}, {cat_cols[1:]}."
             )
         values = values.copy()
         values[cat_cols[0]] = 1 - values[cat_cols[1:]].sum(axis=1)
-        s = values[cat_cols].idxmax(1).str.split(_CAT_SEP, expand=True)[1]
+        s = values[cat_cols].idxmax(1).str.split(_CAT_SEP, expand=True).iloc[:, -1]
         s.name = self.key
         return s
 
     def to_ordinal_encoding(self, values: pd.Series) -> pd.Series:
         """Converts values to an ordinal integer based encoding.
 
         Args:
@@ -364,15 +364,15 @@
 
         Raises:
             ValueError: when categories have non-unique names
 
         Returns:
             List[str]: List of the categories
         """
-        categories = [name for name in categories]
+        categories = list(categories)
         if len(categories) != len(set(categories)):
             raise ValueError("categories must be unique")
         return categories
 
     @validator("objective")
     def validate_objective(cls, objective, values):
         if len(objective) != len(values["categories"]):
@@ -382,11 +382,11 @@
                 raise ValueError("Objective values has to be smaller equal than 1.")
             if o < 0:
                 raise ValueError("Objective values has to be larger equal than zero")
         return objective
 
     def to_dict(self) -> Dict:
         """Returns the catergories and corresponding objective values as dictionary"""
-        return {cat: obj for cat, obj in zip(self.categories, self.objective)}
+        return dict(zip(self.categories, self.objective))
 
     def __call__(self, values: pd.Series) -> pd.Series:
         return values.map(self.to_dict()).astype(float)
```

### Comparing `bofire-0.0.4/bofire/data_models/features/continuous.py` & `bofire-0.0.5/bofire/data_models/features/continuous.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/bofire/data_models/features/descriptor.py` & `bofire-0.0.5/bofire/data_models/features/descriptor.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
         Args:
             descriptors (List[str]): List of descriptor names
 
         Returns:
             List[str]: List of valid keys
         """
-        return [name for name in descriptors]
+        return list(descriptors)
 
     @root_validator(pre=False, skip_on_failure=True)
     def validate_list_lengths(cls, values):
         """compares the length of the defined descriptors list with the provided values
 
         Args:
             values (Dict): Dictionary with all attribues
@@ -100,15 +100,15 @@
 
         Raises:
             ValueError: when descriptors have non-unique names
 
         Returns:
             List[str]: List of the descriptors
         """
-        descriptors = [name for name in descriptors]
+        descriptors = list(descriptors)
         if len(descriptors) != len(set(descriptors)):
             raise ValueError("descriptors must be unique")
         return descriptors
 
     @validator("values")
     def validate_values(cls, v, values):
         """validates the compatability of passed values for the descriptors and the defined categories
@@ -129,24 +129,24 @@
             raise ValueError("values must have same length as categories")
         for row in v:
             if len(row) != len(values["descriptors"]):
                 raise ValueError("rows in values must have same length as descriptors")
         a = np.array(v)
         for i, d in enumerate(values["descriptors"]):
             if len(set(a[:, i])) == 1:
-                raise ValueError("No variation for descriptor {d}.")
+                raise ValueError(f"No variation for descriptor {d}.")
         return v
 
     def to_df(self):
         """tabular overview of the feature as DataFrame
 
         Returns:
             pd.DataFrame: tabular overview of the feature as DataFrame
         """
-        data = {cat: values for cat, values in zip(self.categories, self.values)}
+        data = dict(zip(self.categories, self.values))
         return pd.DataFrame.from_dict(data, orient="index", columns=self.descriptors)
 
     def fixed_value(
         self, transform_type: Optional[TTransform] = None
     ) -> Union[List[str], List[float], None]:
         """Returns the categories to which the feature is fixed, None if the feature is not fixed
 
@@ -230,15 +230,15 @@
             values (pd.Series): Values to transform.
 
         Returns:
             pd.DataFrame: Descriptor encoded dataframe.
         """
         return pd.DataFrame(
             data=values.map(
-                {cat: value for cat, value in zip(self.categories, self.values)}
+                dict(zip(self.categories, self.values))
             ).values.tolist(),  # type: ignore
             columns=[f"{self.key}{_CAT_SEP}{d}" for d in self.descriptors],
             index=values.index,
         )
 
     def from_descriptor_encoding(self, values: pd.DataFrame) -> pd.Series:
         """Converts values back from descriptor encoding.
```

### Comparing `bofire-0.0.4/bofire/data_models/features/discrete.py` & `bofire-0.0.5/bofire/data_models/features/discrete.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/bofire/data_models/features/feature.py` & `bofire-0.0.5/bofire/data_models/features/feature.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from abc import abstractmethod
-from typing import Annotated, ClassVar, Dict, List, Optional, Tuple, Union
+from typing import ClassVar, Dict, List, Optional, Tuple, Union
 
 import pandas as pd
 from pydantic import Field
+from typing_extensions import Annotated
 
 from bofire.data_models.base import BaseModel
 from bofire.data_models.enum import CategoricalEncodingEnum
+from bofire.data_models.molfeatures.api import AnyMolFeatures
 from bofire.data_models.surrogates.scaler import ScalerEnum
 
 TTransform = Union[CategoricalEncodingEnum, ScalerEnum]
 
 
 class Feature(BaseModel):
     """The base class for all features."""
@@ -136,15 +138,15 @@
     return s.apply(lambda s: pd.to_numeric(s, errors="coerce").notnull().all()).all()  # type: ignore
 
 
 def is_categorical(s: pd.Series, categories: List[str]):
     return sum(s.isin(categories)) == len(s)
 
 
-TInputTransformSpecs = Dict[str, CategoricalEncodingEnum]
+TInputTransformSpecs = Dict[str, Union[CategoricalEncodingEnum, AnyMolFeatures]]
 
 
 TDescriptors = Annotated[List[str], Field(min_items=1)]
 
 
 TCategoryVals = Annotated[List[str], Field(min_items=2)]
 TAllowedVals = Optional[Annotated[List[bool], Field(min_items=2)]]
@@ -153,9 +155,8 @@
 TCategoricalDescriptorVals = Annotated[
     Union[List[List[float]], List[List[int]]],
     Field(min_items=1),
 ]
 
 TDiscreteVals = Annotated[List[float], Field(min_items=1)]
 
-
 _CAT_SEP = "_"
```

### Comparing `bofire-0.0.4/bofire/data_models/features/numerical.py` & `bofire-0.0.5/bofire/data_models/features/numerical.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/bofire/data_models/objectives/api.py` & `bofire-0.0.5/bofire/data_models/objectives/api.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/bofire/data_models/objectives/identity.py` & `bofire-0.0.5/bofire/data_models/objectives/identity.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,45 +1,51 @@
-from typing import Literal, Union
+from typing import Literal, Tuple, Union
 
 import numpy as np
 import pandas as pd
 from pydantic import root_validator
 
 from bofire.data_models.objectives.objective import Objective, TWeight
 
 
 class IdentityObjective(Objective):
     """An objective returning the identity as reward.
     The return can be scaled, when a lower and upper bound are provided.
 
     Attributes:
         w (float): float between zero and one for weighting the objective
-        lower_bound (float, optional): Lower bound for normalizing the objective between zero and one. Defaults to zero.
-        upper_bound (float, optional): Upper bound for normalizing the objective between zero and one. Defaults to one.
+        bounds (Tuple[float], optional): Bound for normalizing the objective between zero and one. Defaults to (0,1).
     """
 
     type: Literal["IdentityObjective"] = "IdentityObjective"
     w: TWeight = 1
-    lower_bound: float = 0
-    upper_bound: float = 1
+    bounds: Tuple[float, float] = (0, 1)
+
+    @property
+    def lower_bound(self) -> float:
+        return self.bounds[0]
+
+    @property
+    def upper_bound(self) -> float:
+        return self.bounds[1]
 
     @root_validator(pre=False, skip_on_failure=True)
     def validate_lower_upper(cls, values):
         """Validation function to ensure that lower bound is always greater the upper bound
 
         Args:
             values (Dict): The attributes of the class
 
         Raises:
             ValueError: when a lower bound higher than the upper bound is passed
 
         Returns:
             Dict: The attributes of the class
         """
-        if values["lower_bound"] > values["upper_bound"]:
+        if values["bounds"][0] > values["bounds"][1]:
             raise ValueError(
                 f'lower bound must be <= upper bound, got {values["lower_bound"]} > {values["upper_bound"]}'
             )
         return values
 
     def __call__(self, x: Union[pd.Series, np.ndarray]) -> Union[pd.Series, np.ndarray]:
         """The call function returning a reward for passed x values
@@ -54,28 +60,26 @@
 
 
 class MaximizeObjective(IdentityObjective):
     """Child class from the identity function without modifications, since the parent class is already defined as maximization
 
     Attributes:
         w (float): float between zero and one for weighting the objective
-        lower_bound (float, optional): Lower bound for normalizing the objective between zero and one. Defaults to zero.
-        upper_bound (float, optional): Upper bound for normalizing the objective between zero and one. Defaults to one.
+        bounds (Tuple[float], optional): Bound for normalizing the objective between zero and one. Defaults to (0,1).
     """
 
     type: Literal["MaximizeObjective"] = "MaximizeObjective"
 
 
 class MinimizeObjective(IdentityObjective):
     """Class returning the negative identity as reward.
 
     Attributes:
         w (float): float between zero and one for weighting the objective
-        lower_bound (float, optional): Lower bound for normalizing the objective between zero and one. Defaults to zero.
-        upper_bound (float, optional): Upper bound for normalizing the objective between zero and one. Defaults to one.
+        bounds (Tuple[float], optional): Bound for normalizing the objective between zero and one. Defaults to (0,1).
     """
 
     type: Literal["MinimizeObjective"] = "MinimizeObjective"
 
     def __call__(self, x: Union[pd.Series, np.ndarray]) -> Union[pd.Series, np.ndarray]:
         """The call function returning a reward for passed x values
```

### Comparing `bofire-0.0.4/bofire/data_models/objectives/objective.py` & `bofire-0.0.5/bofire/data_models/objectives/objective.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from abc import abstractmethod
-from typing import Annotated, Union
+from typing import Union
 
 import numpy as np
 import pandas as pd
 from pydantic import Field
+from typing_extensions import Annotated
 
 from bofire.data_models.base import BaseModel
 
 
 class Objective(BaseModel):
     """The base class for all objectives"""
```

### Comparing `bofire-0.0.4/bofire/data_models/objectives/sigmoid.py` & `bofire-0.0.5/bofire/data_models/objectives/sigmoid.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/bofire/data_models/objectives/target.py` & `bofire-0.0.5/bofire/data_models/objectives/target.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/bofire/data_models/priors/api.py` & `bofire-0.0.5/bofire/data_models/priors/api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from functools import partial
 from typing import Union
 
 from bofire.data_models.priors.gamma import GammaPrior
 from bofire.data_models.priors.normal import NormalPrior
 from bofire.data_models.priors.prior import Prior
 
 AbstractPrior = Prior
@@ -9,18 +10,18 @@
 AnyPrior = Union[
     GammaPrior,
     NormalPrior,
 ]
 
 # default priors of interest
 # botorch defaults
-BOTORCH_LENGTHCALE_PRIOR = GammaPrior(concentration=3.0, rate=6.0)
-BOTORCH_NOISE_PRIOR = GammaPrior(concentration=1.1, rate=0.05)
-BOTORCH_SCALE_PRIOR = GammaPrior(concentration=2.0, rate=0.15)
+BOTORCH_LENGTHCALE_PRIOR = partial(GammaPrior, concentration=3.0, rate=6.0)
+BOTORCH_NOISE_PRIOR = partial(GammaPrior, concentration=1.1, rate=0.05)
+BOTORCH_SCALE_PRIOR = partial(GammaPrior, concentration=2.0, rate=0.15)
 
 # mbo priors
 # By default BoTorch places a highly informative prior on the kernel lengthscales,
 # which easily leads to overfitting. Here we set a broader prior distribution for the
 # lengthscale. The priors for the noise and signal variance are set more tightly.
-MBO_LENGTHCALE_PRIOR = GammaPrior(concentration=2.0, rate=0.2)
-MBO_NOISE_PRIOR = GammaPrior(concentration=2.0, rate=4.0)
-MBO_OUTPUTSCALE_PRIOR = GammaPrior(concentration=2.0, rate=4.0)
+MBO_LENGTHCALE_PRIOR = partial(GammaPrior, concentration=2.0, rate=0.2)
+MBO_NOISE_PRIOR = partial(GammaPrior, concentration=2.0, rate=4.0)
+MBO_OUTPUTSCALE_PRIOR = partial(GammaPrior, concentration=2.0, rate=4.0)
```

### Comparing `bofire-0.0.4/bofire/data_models/strategies/api.py` & `bofire-0.0.5/bofire/data_models/strategies/api.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,56 +1,71 @@
 from typing import Union
 
 from bofire.data_models.strategies.doe import DoEStrategy
+from bofire.data_models.strategies.factorial import FactorialStrategy
 from bofire.data_models.strategies.predictives.botorch import BotorchStrategy
 from bofire.data_models.strategies.predictives.multiobjective import (
     MultiobjectiveStrategy,
 )
 from bofire.data_models.strategies.predictives.predictive import PredictiveStrategy
 from bofire.data_models.strategies.predictives.qehvi import QehviStrategy
 from bofire.data_models.strategies.predictives.qnehvi import QnehviStrategy
 from bofire.data_models.strategies.predictives.qparego import QparegoStrategy
 from bofire.data_models.strategies.predictives.sobo import (
     AdditiveSoboStrategy,
+    CustomSoboStrategy,
     MultiplicativeSoboStrategy,
     SoboStrategy,
 )
 from bofire.data_models.strategies.random import RandomStrategy
 from bofire.data_models.strategies.samplers.polytope import PolytopeSampler
 from bofire.data_models.strategies.samplers.rejection import RejectionSampler
 from bofire.data_models.strategies.samplers.sampler import SamplerStrategy
+from bofire.data_models.strategies.stepwise.conditions import (  # noqa: F401
+    AlwaysTrueCondition,
+    CombiCondition,
+    NumberOfExperimentsCondition,
+)
+from bofire.data_models.strategies.stepwise.stepwise import (  # noqa: F401
+    Step,
+    StepwiseStrategy,
+)
 from bofire.data_models.strategies.strategy import Strategy
 
 AbstractStrategy = Union[
     Strategy,
     BotorchStrategy,
     SamplerStrategy,
     PredictiveStrategy,
     MultiobjectiveStrategy,
 ]
 
 AnyStrategy = Union[
     SoboStrategy,
     AdditiveSoboStrategy,
     MultiplicativeSoboStrategy,
+    CustomSoboStrategy,
     QehviStrategy,
     QnehviStrategy,
     QparegoStrategy,
     PolytopeSampler,
     RejectionSampler,
     RandomStrategy,
     DoEStrategy,
+    StepwiseStrategy,
+    FactorialStrategy,
 ]
 
 AnyPredictive = Union[
     SoboStrategy,
     AdditiveSoboStrategy,
     MultiplicativeSoboStrategy,
+    CustomSoboStrategy,
     QehviStrategy,
     QnehviStrategy,
     QparegoStrategy,
 ]
 
-AnySampler = Union[
-    PolytopeSampler,
-    RejectionSampler,
-]
+AnySampler = Union[PolytopeSampler, RejectionSampler]
+
+
+AnyCondition = Union[NumberOfExperimentsCondition, CombiCondition, AlwaysTrueCondition]
```

### Comparing `bofire-0.0.4/bofire/data_models/strategies/doe.py` & `bofire-0.0.5/bofire/data_models/strategies/doe.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/bofire/data_models/strategies/predictives/botorch.py` & `bofire-0.0.5/bofire/data_models/strategies/predictives/botorch.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/bofire/data_models/strategies/predictives/multiobjective.py` & `bofire-0.0.5/bofire/data_models/strategies/predictives/multiobjective.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 from pydantic import validator
 
-from bofire.data_models.objectives.api import MaximizeObjective, MinimizeObjective
+from bofire.data_models.objectives.api import (
+    CloseToTargetObjective,
+    MaximizeObjective,
+    MinimizeObjective,
+)
 from bofire.data_models.strategies.predictives.botorch import BotorchStrategy
 
 
 class MultiobjectiveStrategy(BotorchStrategy):
     @validator("domain")
     def validate_domain_is_multiobjective(cls, v, values):
         """Validate that the domain is multiobjective."""
-        feats = v.outputs.get_by_objective([MaximizeObjective, MinimizeObjective])
+        feats = v.outputs.get_by_objective(
+            [MaximizeObjective, MinimizeObjective, CloseToTargetObjective]
+        )
         if len(feats) < 2:
             raise ValueError(
                 "At least two output features with MaximizeObjective or MinimizeObjective has to be defined in the domain."
             )
         for feat in feats:
             if feat.objective.w != 1.0:  # type: ignore
                 raise ValueError(
```

### Comparing `bofire-0.0.4/bofire/data_models/strategies/predictives/predictive.py` & `bofire-0.0.5/bofire/data_models/strategies/predictives/predictive.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/bofire/data_models/strategies/predictives/qehvi.py` & `bofire-0.0.5/bofire/data_models/strategies/predictives/qehvi.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/bofire/data_models/strategies/predictives/qnehvi.py` & `bofire-0.0.5/bofire/data_models/strategies/predictives/qnehvi.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/bofire/data_models/strategies/predictives/qparego.py` & `bofire-0.0.5/bofire/data_models/strategies/predictives/qparego.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/bofire/data_models/strategies/predictives/sobo.py` & `bofire-0.0.5/bofire/data_models/strategies/predictives/sobo.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from typing import Literal, Type
+from typing import Literal, Optional, Type
 
-from pydantic import validator
+from pydantic import Field, validator
 
-from bofire.data_models.acquisition_functions.api import AnyAcquisitionFunction
+from bofire.data_models.acquisition_functions.api import AnyAcquisitionFunction, qNEI
 from bofire.data_models.features.api import CategoricalOutput, Feature
 from bofire.data_models.objectives.api import ConstrainedObjective, Objective
 from bofire.data_models.strategies.predictives.botorch import BotorchStrategy
 
 
 class SoboBaseStrategy(BotorchStrategy):
-    acquisition_function: AnyAcquisitionFunction
+    acquisition_function: AnyAcquisitionFunction = Field(default_factory=lambda: qNEI())
 
     @classmethod
     def is_feature_implemented(cls, my_type: Type[Feature]) -> bool:
         """Method to check if a specific feature type is implemented for the strategy
 
         Args:
             my_type (Type[Feature]): Feature class
@@ -58,7 +58,13 @@
 class AdditiveSoboStrategy(SoboBaseStrategy):
     type: Literal["AdditiveSoboStrategy"] = "AdditiveSoboStrategy"
     use_output_constraints: bool = True
 
 
 class MultiplicativeSoboStrategy(SoboBaseStrategy):
     type: Literal["MultiplicativeSoboStrategy"] = "MultiplicativeSoboStrategy"
+
+
+class CustomSoboStrategy(SoboBaseStrategy):
+    type: Literal["CustomSoboStrategy"] = "CustomSoboStrategy"
+    use_output_constraints: bool = True
+    dump: Optional[str] = None
```

### Comparing `bofire-0.0.4/bofire/data_models/strategies/random.py` & `bofire-0.0.5/bofire/data_models/strategies/random.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/bofire/data_models/strategies/samplers/polytope.py` & `bofire-0.0.5/bofire/data_models/strategies/samplers/polytope.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/bofire/data_models/strategies/samplers/rejection.py` & `bofire-0.0.5/bofire/data_models/strategies/samplers/rejection.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/bofire/data_models/strategies/strategy.py` & `bofire-0.0.5/bofire/data_models/strategies/strategy.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/bofire/data_models/surrogates/api.py` & `bofire-0.0.5/bofire/data_models/surrogates/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,53 @@
 from typing import Union
 
-from bofire.data_models.surrogates.scaler import ScalerEnum  # noqa: F401
+from bofire.data_models.surrogates.scaler import ScalerEnum
 
 try:
     from bofire.data_models.surrogates.botorch import BotorchSurrogate
-    from bofire.data_models.surrogates.botorch_surrogates import (  # noqa: F401
+    from bofire.data_models.surrogates.botorch_surrogates import (
         AnyBotorchSurrogate,
         BotorchSurrogates,
     )
     from bofire.data_models.surrogates.empirical import EmpiricalSurrogate
     from bofire.data_models.surrogates.fully_bayesian import SaasSingleTaskGPSurrogate
-    from bofire.data_models.surrogates.mixed_single_task_gp import (  # noqa: F401
+    from bofire.data_models.surrogates.linear import LinearSurrogate
+    from bofire.data_models.surrogates.mixed_single_task_gp import (
         MixedSingleTaskGPSurrogate,
     )
     from bofire.data_models.surrogates.mlp import MLPEnsemble
     from bofire.data_models.surrogates.random_forest import RandomForestSurrogate
-    from bofire.data_models.surrogates.single_task_gp import SingleTaskGPSurrogate
+    from bofire.data_models.surrogates.single_task_gp import (
+        SingleTaskGPHyperconfig,
+        SingleTaskGPSurrogate,
+    )
     from bofire.data_models.surrogates.surrogate import Surrogate
+    from bofire.data_models.surrogates.tanimoto_gp import TanimotoGPSurrogate
+    from bofire.data_models.surrogates.xgb import XGBoostSurrogate
 
     AbstractSurrogate = Union[Surrogate, BotorchSurrogate, EmpiricalSurrogate]
 
     AnySurrogate = Union[
         EmpiricalSurrogate,
         RandomForestSurrogate,
         SingleTaskGPSurrogate,
         MixedSingleTaskGPSurrogate,
         MLPEnsemble,
         SaasSingleTaskGPSurrogate,
+        XGBoostSurrogate,
+        LinearSurrogate,
+        TanimotoGPSurrogate,
+    ]
+
+    AnyTrainableSurrogate = Union[
+        RandomForestSurrogate,
+        SingleTaskGPSurrogate,
+        MixedSingleTaskGPSurrogate,
+        MLPEnsemble,
+        SaasSingleTaskGPSurrogate,
+        XGBoostSurrogate,
+        LinearSurrogate,
+        TanimotoGPSurrogate,
     ]
 except ImportError:
     # with the minimal installationwe don't have botorch
     pass
```

### Comparing `bofire-0.0.4/bofire/data_models/surrogates/botorch_surrogates.py` & `bofire-0.0.5/bofire/data_models/surrogates/botorch_surrogates.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/bofire/data_models/surrogates/fully_bayesian.py` & `bofire-0.0.5/bofire/data_models/surrogates/fully_bayesian.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from typing import Literal
 
 from pydantic import conint, validator
 
 from bofire.data_models.surrogates.botorch import BotorchSurrogate
 from bofire.data_models.surrogates.scaler import ScalerEnum
+from bofire.data_models.surrogates.trainable import TrainableSurrogate
 
 
-class SaasSingleTaskGPSurrogate(BotorchSurrogate):
+class SaasSingleTaskGPSurrogate(BotorchSurrogate, TrainableSurrogate):
     type: Literal["SaasSingleTaskGPSurrogate"] = "SaasSingleTaskGPSurrogate"
     warmup_steps: conint(ge=1) = 256  # type: ignore
     num_samples: conint(ge=1) = 128  # type: ignore
     thinning: conint(ge=1) = 16  # type: ignore
     scaler: ScalerEnum = ScalerEnum.NORMALIZE
 
     @validator("thinning")
```

### Comparing `bofire-0.0.4/bofire/data_models/surrogates/mixed_single_task_gp.py` & `bofire-0.0.5/bofire/data_models/surrogates/mixed_single_task_gp.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,17 +7,18 @@
     AnyCategoricalKernal,
     AnyContinuousKernel,
     HammondDistanceKernel,
     MaternKernel,
 )
 from bofire.data_models.surrogates.botorch import BotorchSurrogate
 from bofire.data_models.surrogates.single_task_gp import ScalerEnum
+from bofire.data_models.surrogates.trainable import TrainableSurrogate
 
 
-class MixedSingleTaskGPSurrogate(BotorchSurrogate):
+class MixedSingleTaskGPSurrogate(BotorchSurrogate, TrainableSurrogate):
     type: Literal["MixedSingleTaskGPSurrogate"] = "MixedSingleTaskGPSurrogate"
     continuous_kernel: AnyContinuousKernel = Field(
         default_factory=lambda: MaternKernel(ard=True, nu=2.5)
     )
     categorical_kernel: AnyCategoricalKernal = Field(
         default_factory=lambda: HammondDistanceKernel(ard=True)
     )
```

### Comparing `bofire-0.0.4/bofire/data_models/surrogates/mlp.py` & `bofire-0.0.5/bofire/data_models/surrogates/mlp.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Literal, Sequence
 
 from bofire.data_models.surrogates.botorch import BotorchSurrogate
 from bofire.data_models.surrogates.scaler import ScalerEnum
+from bofire.data_models.surrogates.trainable import TrainableSurrogate
 
 
-class MLPEnsemble(BotorchSurrogate):
+class MLPEnsemble(BotorchSurrogate, TrainableSurrogate):
     type: Literal["MLPEnsemble"] = "MLPEnsemble"
     n_estimators: int
     hidden_layer_sizes: Sequence = (100,)
     activation: Literal["relu", "logistic", "tanh"] = "relu"
     dropout: float = 0.0
     batch_size: int = 10
     n_epochs: int = 200
```

### Comparing `bofire-0.0.4/bofire/data_models/surrogates/random_forest.py` & `bofire-0.0.5/bofire/data_models/surrogates/random_forest.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-from typing import Annotated, Literal, Optional, Union
+from typing import Literal, Optional, Union
 
 from pydantic import Field
+from typing_extensions import Annotated
 
 from bofire.data_models.surrogates.botorch import BotorchSurrogate
+from bofire.data_models.surrogates.trainable import TrainableSurrogate
 
 
-class RandomForestSurrogate(BotorchSurrogate):
+class RandomForestSurrogate(BotorchSurrogate, TrainableSurrogate):
     type: Literal["RandomForestSurrogate"] = "RandomForestSurrogate"
 
     # hyperparams passed down to `RandomForestRegressor`
     n_estimators: int = 100
     criterion: Literal[
         "squared_error",
         "absolute_error",
```

### Comparing `bofire-0.0.4/bofire/data_models/surrogates/surrogate.py` & `bofire-0.0.5/bofire/data_models/surrogates/surrogate.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/bofire/data_models/validated.py` & `bofire-0.0.5/bofire/data_models/validated.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/bofire/plot/feature_importance.py` & `bofire-0.0.5/bofire/plot/feature_importance.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/bofire/plot/objective.py` & `bofire-0.0.5/bofire/plot/objective.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 def plot_objective_plotly(
     feature: ContinuousOutput,
     lower: float,
     upper: float,
     values: Optional[pd.Series] = None,
-    layout_options: Dict = {},
+    layout_options: Optional[Dict] = None,
 ):
     """Plot the assigned objective.
 
     Args:
         feature (ContinuousOutput): Output feature, whose objective should be visualized.
         lower (float): lower bound for the plot
         upper (float): upper bound for the plot
@@ -39,11 +39,11 @@
             x=values,
             y=feature.objective.__call__(values),
         )
         fig = go.Figure(data=fig1.data + fig2.data)  # type: ignore
     else:
         fig = fig1
 
-    if len(layout_options) > 0:
+    if layout_options is not None:
         fig.update_layout(layout_options)
 
     return fig
```

### Comparing `bofire-0.0.4/bofire/plot/prior.py` & `bofire-0.0.5/bofire/plot/prior.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-from typing import Dict
+from typing import Dict, Optional
 
 import numpy as np
 import plotly.express as px
 import torch
 
+import bofire.priors.api as priors
 from bofire.data_models.priors.api import AnyPrior
 
 
 def plot_prior_pdf_plotly(
     prior: AnyPrior,
     lower: float,
     upper: float,
-    layout_options: Dict = {},
+    layout_options: Optional[Dict] = None,
 ):
     """Plot the probability density function of the prior with plotly.
 
     Args:
         prior (AnyPrior): The prior that should be plotted.
         lower (float): lower bound for computing the prior pdf.
         upper (float): upper bound for computing the prior pdf.
@@ -25,14 +26,14 @@
         fig, ax objects of the plot.
     """
 
     x = np.linspace(lower, upper, 1000)
 
     fig = px.line(
         x=x,
-        y=np.exp(prior.to_gpytorch().log_prob(torch.from_numpy(x)).numpy()),
+        y=np.exp(priors.map(prior).log_prob(torch.from_numpy(x)).numpy()),
     )
 
-    if len(layout_options) > 0:
+    if layout_options is not None:
         fig.update_layout(layout_options)
 
     return fig
```

### Comparing `bofire-0.0.4/bofire/strategies/api.py` & `bofire-0.0.5/bofire/strategies/api.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 from bofire.strategies.predictives.botorch import BotorchStrategy  # noqa: F401
 from bofire.strategies.predictives.predictive import PredictiveStrategy  # noqa: F401
 from bofire.strategies.predictives.qehvi import QehviStrategy  # noqa: F401
 from bofire.strategies.predictives.qnehvi import QnehviStrategy  # noqa: F401
 from bofire.strategies.predictives.qparego import QparegoStrategy  # noqa: F401
 from bofire.strategies.predictives.sobo import (  # noqa: F401
     AdditiveSoboStrategy,
+    CustomSoboStrategy,
     MultiplicativeSoboStrategy,
     SoboStrategy,
 )
 from bofire.strategies.random import RandomStrategy  # noqa: F401
 from bofire.strategies.samplers.polytope import PolytopeSampler  # noqa: F401
 from bofire.strategies.samplers.rejection import RejectionSampler  # noqa: F401
 from bofire.strategies.samplers.sampler import SamplerStrategy  # noqa: F401
+from bofire.strategies.stepwise.stepwise import StepwiseStrategy  # noqa: F401
 from bofire.strategies.strategy import Strategy  # noqa: F401
```

### Comparing `bofire-0.0.4/bofire/strategies/data_models/candidate.py` & `bofire-0.0.5/bofire/strategies/data_models/candidate.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/bofire/strategies/data_models/values.py` & `bofire-0.0.5/bofire/strategies/data_models/values.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from typing import Annotated, Union
+from typing import Union
 
 from pydantic import Field
+from typing_extensions import Annotated
 
 from bofire.data_models.base import BaseModel
 
 Value = Union[float, str, int]
 
 
 class InputValue(BaseModel):
```

### Comparing `bofire-0.0.4/bofire/strategies/doe/design.py` & `bofire-0.0.5/bofire/strategies/doe/design.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,28 +24,28 @@
 
 
 def find_local_max_ipopt(
     domain: Domain,
     model_type: Union[str, Formula],
     n_experiments: Optional[int] = None,
     delta: float = 1e-7,
-    ipopt_options: Dict = {},
+    ipopt_options: Optional[Dict] = None,
     sampling: Optional[pd.DataFrame] = None,
     fixed_experiments: Optional[pd.DataFrame] = None,
     objective: OptimalityCriterionEnum = OptimalityCriterionEnum.D_OPTIMALITY,
 ) -> pd.DataFrame:
-    """Function computing a d-optimal design" for a given domain and model.
+    """Function computing an optimal design for a given domain and model.
     Args:
         domain (Domain): domain containing the inputs and constraints.
         model_type (str, Formula): keyword or formulaic Formula describing the model. Known keywords
             are "linear", "linear-and-interactions", "linear-and-quadratic", "fully-quadratic".
         n_experiments (int): Number of experiments. By default the value corresponds to
             the number of model terms - dimension of ker() + 3.
         delta (float): Regularization parameter. Default value is 1e-3.
-        ipopt_options (Dict): options for IPOPT. For more information see [this link](https://coin-or.github.io/Ipopt/OPTIONS.html)
+        ipopt_options (Dict, optional): options for IPOPT. For more information see [this link](https://coin-or.github.io/Ipopt/OPTIONS.html)
         sampling (Sampling, np.ndarray): Sampling class or a np.ndarray object containing the initial guess.
         fixed_experiments (pd.DataFrame): dataframe containing experiments that will be definitely part of the design.
             Values are set before the optimization.
         objective (OptimalityCriterionEnum): OptimalityCriterionEnum object indicating which objective function to use.
     Returns:
         A pd.DataFrame object containing the best found input for the experiments. In general, this is only a
         local optimum.
@@ -72,19 +72,17 @@
                 "Nonlinear constraints were detected. Not all features and checks are supported for this type of constraints. \
                 Using them can lead to unexpected behaviour. Please make sure to provide jacobians for nonlinear constraints.",
                 UserWarning,
             )
 
     # check that NChooseK constraints only impose an upper bound on the number of nonzero components (and no lower bound)
     assert all(
-        [
-            c.min_count == 0
-            for c in domain.constraints
-            if isinstance(c, NChooseKConstraint)
-        ]
+        c.min_count == 0
+        for c in domain.constraints
+        if isinstance(c, NChooseKConstraint)
     ), "NChooseKConstraint with min_count !=0 is not supported!"
 
     # determine number of experiments (only relevant if n_experiments is not provided by the user)
     n_experiments = get_n_experiments(
         domain=domain, model_type=model_type, n_experiments=n_experiments
     )
 
@@ -136,14 +134,16 @@
         domain.validate_candidates(fixed_experiments, only_inputs=True)
         fixed_experiments = np.array(fixed_experiments.values)
         for i, val in enumerate(fixed_experiments.flatten()):
             bounds[i] = (val, val)
             x0[i] = val
 
     # set ipopt options
+    if ipopt_options is None:
+        ipopt_options = {}
     _ipopt_options = {"maxiter": 500, "disp": 0}
     for key in ipopt_options.keys():
         _ipopt_options[key] = ipopt_options[key]
     if _ipopt_options["disp"] > 12:
         _ipopt_options["disp"] = 0
 
     #
```

### Comparing `bofire-0.0.4/bofire/strategies/doe/objective.py` & `bofire-0.0.5/bofire/strategies/doe/objective.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/bofire/strategies/doe/utils.py` & `bofire-0.0.5/bofire/strategies/doe/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -470,15 +470,15 @@
                 ind = [
                     i
                     for i, p in enumerate(domain.inputs.get_keys())
                     if p in constraint.features
                 ]
 
                 # find and shuffle all combinations of elements of ind of length max_active
-                ind = np.array([c for c in combinations(ind, r=n_inactive)])
+                ind = np.array(list(combinations(ind, r=n_inactive)))
                 np.random.shuffle(ind)
 
                 # set bounds to zero in each experiments for the variables that should be inactive
                 for i in range(n_experiments):
                     ind_vanish = ind[i % len(ind)]
                     bounds[ind_vanish + i * len(domain.inputs), :] = [0, 0]
     else:
```

### Comparing `bofire-0.0.4/bofire/strategies/doe_strategy.py` & `bofire-0.0.5/bofire/strategies/doe_strategy.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/bofire/strategies/mapper.py` & `bofire-0.0.5/bofire/strategies/mapper.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,43 @@
 from typing import Dict, Type
 
 import bofire.data_models.strategies.api as data_models
 from bofire.strategies.doe_strategy import DoEStrategy  # noqa: F401
+from bofire.strategies.factorial import FactorialStrategy
 from bofire.strategies.predictives.botorch import BotorchStrategy  # noqa: F401
 from bofire.strategies.predictives.predictive import PredictiveStrategy  # noqa: F401
 from bofire.strategies.predictives.qehvi import QehviStrategy  # noqa: F401
 from bofire.strategies.predictives.qnehvi import QnehviStrategy  # noqa: F401
 from bofire.strategies.predictives.qparego import QparegoStrategy  # noqa: F401
 from bofire.strategies.predictives.sobo import (  # noqa: F401
     AdditiveSoboStrategy,
+    CustomSoboStrategy,
     MultiplicativeSoboStrategy,
     SoboStrategy,
 )
 from bofire.strategies.random import RandomStrategy  # noqa: F401
 from bofire.strategies.samplers.polytope import PolytopeSampler  # noqa: F401
 from bofire.strategies.samplers.rejection import RejectionSampler  # noqa: F401
 from bofire.strategies.samplers.sampler import SamplerStrategy  # noqa: F401
+from bofire.strategies.stepwise.stepwise import StepwiseStrategy
 from bofire.strategies.strategy import Strategy  # noqa: F401
 
 STRATEGY_MAP: Dict[Type[data_models.Strategy], Type[Strategy]] = {
     data_models.RandomStrategy: RandomStrategy,
     data_models.SoboStrategy: SoboStrategy,
     data_models.AdditiveSoboStrategy: AdditiveSoboStrategy,
     data_models.MultiplicativeSoboStrategy: MultiplicativeSoboStrategy,
+    data_models.CustomSoboStrategy: CustomSoboStrategy,
     data_models.QehviStrategy: QehviStrategy,
     data_models.QnehviStrategy: QnehviStrategy,
     data_models.QparegoStrategy: QparegoStrategy,
     data_models.PolytopeSampler: PolytopeSampler,
     data_models.RejectionSampler: RejectionSampler,
     data_models.DoEStrategy: DoEStrategy,
+    data_models.StepwiseStrategy: StepwiseStrategy,
+    data_models.FactorialStrategy: FactorialStrategy,
 }
 
 
 def map(data_model: data_models.Strategy) -> Strategy:
     cls = STRATEGY_MAP[data_model.__class__]
     return cls.from_spec(data_model=data_model)
```

### Comparing `bofire-0.0.4/bofire/strategies/predictives/botorch.py` & `bofire-0.0.5/bofire/strategies/predictives/botorch.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/bofire/strategies/predictives/predictive.py` & `bofire-0.0.5/bofire/strategies/predictives/predictive.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,29 +31,35 @@
     def input_preprocessing_specs(self) -> TInputTransformSpecs:
         pass
 
     def ask(
         self,
         candidate_count: Optional[PositiveInt] = None,
         add_pending: bool = False,
+        raise_validation_error: bool = True,
     ) -> pd.DataFrame:
         """Function to generate new candidates.
 
         Args:
             candidate_count (PositiveInt, optional): Number of candidates to be generated. If not provided, the number of candidates is determined automatically. Defaults to None.
             add_pending (bool, optional): If true the proposed candidates are added to the set of pending experiments. Defaults to False.
+            raise_validation_error (bool, optional): If true an error will be raised if candidates violate constraints,
+                otherwise only a warning will be displayed. Defaults to True.
 
         Returns:
             pd.DataFrame: DataFrame with candidates (proposed experiments)
         """
         candidates = super().ask(
             candidate_count=candidate_count,
             add_pending=add_pending,
+            raise_validation_error=raise_validation_error,
+        )
+        self.domain.validate_candidates(
+            candidates=candidates, raise_validation_error=raise_validation_error
         )
-        self.domain.validate_candidates(candidates=candidates)
         return candidates
 
     def tell(
         self, experiments: pd.DataFrame, replace: bool = False, retrain: bool = True
     ):
         """This function passes new experimental data to the optimizer.
```

### Comparing `bofire-0.0.4/bofire/strategies/predictives/qehvi.py` & `bofire-0.0.5/bofire/strategies/predictives/qehvi.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/bofire/strategies/predictives/qnehvi.py` & `bofire-0.0.5/bofire/strategies/predictives/qnehvi.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/bofire/strategies/predictives/qparego.py` & `bofire-0.0.5/bofire/strategies/predictives/qparego.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/bofire/strategies/predictives/sobo.py` & `bofire-0.0.5/bofire/strategies/predictives/sobo.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,36 @@
+import base64
+import warnings
 from typing import List, Union
 
+try:
+    import cloudpickle
+except ModuleNotFoundError:
+    warnings.warn(
+        "Cloudpickle is not available. CustomSoboStrategy's `f` cannot be dumped or loaded."
+    )
+
 import torch
 from botorch.acquisition import get_acquisition_function
 from botorch.acquisition.acquisition import AcquisitionFunction
 from botorch.acquisition.objective import ConstrainedMCObjective, GenericMCObjective
 from botorch.models.gpytorch import GPyTorchModel
 
 from bofire.data_models.acquisition_functions.api import qPI, qUCB
 from bofire.data_models.objectives.api import ConstrainedObjective
 from bofire.data_models.strategies.api import AdditiveSoboStrategy as AdditiveDataModel
+from bofire.data_models.strategies.api import CustomSoboStrategy as CustomDataModel
 from bofire.data_models.strategies.api import (
     MultiplicativeSoboStrategy as MultiplicativeDataModel,
 )
 from bofire.data_models.strategies.predictives.sobo import SoboBaseStrategy as DataModel
 from bofire.strategies.predictives.botorch import BotorchStrategy
 from bofire.utils.torch_tools import (
     get_additive_botorch_objective,
+    get_custom_botorch_objective,
     get_multiplicative_botorch_objective,
     get_objective_callable,
     get_output_constraints,
     tkwargs,
 )
 
 
@@ -124,7 +135,58 @@
 
     def _get_objective(self) -> GenericMCObjective:
         return GenericMCObjective(
             objective=get_multiplicative_botorch_objective(  # type: ignore
                 outputs=self.domain.outputs
             )
         )
+
+
+class CustomSoboStrategy(SoboStrategy):
+    def __init__(
+        self,
+        data_model: CustomDataModel,
+        **kwargs,
+    ):
+        super().__init__(data_model=data_model, **kwargs)
+        self.use_output_constraints = data_model.use_output_constraints
+        if data_model.dump is not None:
+            self.loads(data_model.dump)
+        else:
+            self.f = None
+
+    def _get_objective(self) -> GenericMCObjective:
+        if self.f is None:
+            raise ValueError("No function has been provided for the strategy")
+
+        if (
+            self.use_output_constraints
+            and len(self.domain.outputs.get_by_objective(ConstrainedObjective)) > 0
+        ):
+            constraints, etas = get_output_constraints(outputs=self.domain.outputs)
+            objective = get_custom_botorch_objective(
+                outputs=self.domain.outputs, f=self.f, exclude_constraints=True
+            )
+            return ConstrainedMCObjective(
+                objective=objective,  # type: ignore
+                constraints=constraints,
+                eta=torch.tensor(etas).to(**tkwargs),
+                infeasible_cost=self.get_infeasible_cost(objective=objective),
+            )
+
+        return GenericMCObjective(
+            objective=get_custom_botorch_objective(
+                outputs=self.domain.outputs, f=self.f, exclude_constraints=False
+            )
+        )
+
+    def dumps(self) -> str:
+        """Dumps the function to a string via pickle as this is not directly json serializable."""
+        if self.f is None:
+            raise ValueError("No function has been provided for the strategy")
+        f_bytes_dump = cloudpickle.dumps(self.f)
+        return base64.b64encode(f_bytes_dump).decode()
+
+    def loads(self, data: str):
+        """Loads the function from a base64 encoded pickle bytes object and writes it to the `model` attribute."""
+        f_bytes_load = base64.b64decode(data.encode())
+        self.f = cloudpickle.loads(f_bytes_load)
```

### Comparing `bofire-0.0.4/bofire/strategies/random.py` & `bofire-0.0.5/bofire/strategies/random.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/bofire/strategies/samplers/polytope.py` & `bofire-0.0.5/bofire/strategies/samplers/polytope.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         self.fallback_sampling_method = data_model.fallback_sampling_method
 
     def _ask(self, n: int) -> pd.DataFrame:
         if len(self.domain.constraints) == 0:
             return self.domain.inputs.sample(n, self.fallback_sampling_method)
 
         # check if we have pseudo fixed features in the linear equality constraints
-        # a pseude fixed is a linear euquality constraint with only one feature included
+        # a pseudo fixed is a linear euquality constraint with only one feature included
         # this can happen when fixing features when sampling with NChooseK constraints
         eqs = get_linear_constraints(
             domain=self.domain,
             constraint=LinearEqualityConstraint,  # type: ignore
             unit_scaled=False,
         )
         cleaned_eqs = []
```

### Comparing `bofire-0.0.4/bofire/strategies/samplers/rejection.py` & `bofire-0.0.5/bofire/strategies/samplers/rejection.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/bofire/strategies/strategy.py` & `bofire-0.0.5/bofire/strategies/strategy.py`

 * *Files 12% similar despite different names*

```diff
@@ -83,21 +83,24 @@
         """Method to allow for customized tell functions in addition to self.tell()"""
         pass
 
     def ask(
         self,
         candidate_count: Optional[PositiveInt] = None,
         add_pending: bool = False,
+        raise_validation_error: bool = True,
     ) -> pd.DataFrame:
         """Function to generate new candidates.
 
         Args:
             candidate_count (PositiveInt, optional): Number of candidates to be generated. If not provided, the number
                 of candidates is determined automatically. Defaults to None.
             add_pending (bool, optional): If true the proposed candidates are added to the set of pending experiments. Defaults to False.
+            raise_validation_error (bool, optional): If true an error will be raised if candidates violate constraints,
+                otherwise only a warning will be displayed. Defaults to True.
 
 
         Raises:
             ValueError: if candidate count is smaller than 1
             ValueError: if not enough experiments are available to execute the strategy
             ValueError: if the number of generated candidates does not match the requested number
 
@@ -111,15 +114,19 @@
         if not self.has_sufficient_experiments():
             raise ValueError(
                 "Not enough experiments available to execute the strategy."
             )
 
         candidates = self._ask(candidate_count=candidate_count)
 
-        self.domain.validate_candidates(candidates=candidates, only_inputs=True)
+        self.domain.validate_candidates(
+            candidates=candidates,
+            only_inputs=True,
+            raise_validation_error=raise_validation_error,
+        )
 
         if candidate_count is not None:
             if len(candidates) != candidate_count:
                 raise ValueError(
                     f"expected {candidate_count} candidates, got {len(candidates)}"
                 )
```

### Comparing `bofire-0.0.4/bofire/surrogates/botorch.py` & `bofire-0.0.5/bofire/surrogates/botorch.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/bofire/surrogates/botorch_surrogates.py` & `bofire-0.0.5/bofire/surrogates/botorch_surrogates.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/bofire/surrogates/diagnostics.py` & `bofire-0.0.5/bofire/surrogates/diagnostics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import warnings
 from typing import Dict, List, Optional, Sequence
 
 import numpy as np
 import pandas as pd
 from pydantic import Field, root_validator, validator
 from scipy.stats import fisher_exact, pearsonr, spearmanr
 from sklearn.metrics import (
@@ -258,15 +259,18 @@
         Args:
             metric (RegressionMetricsEnum): Metric to calculate.
 
         Returns:
             float: Metric value.
         """
         if self.n_samples == 1:
-            raise ValueError("Metric cannot be calculated for only one sample.")
+            warnings.warn(
+                "Metric cannot be calculated for only one sample. Null value will be returned"
+            )
+            return np.nan
         return metrics[metric](self.observed.values, self.predicted.values, self.standard_deviation)  # type: ignore
 
 
 class CvResults(BaseModel):
     """Container holding all cv folds of a cross-validation run.
 
     Attributes:
@@ -289,17 +293,17 @@
                 has_i = getattr(i, field) is not None
                 if has_field != has_i:
                     raise ValueError(
                         f"Either all or none `CvResult` objects contain {field}."
                     )
         # check columns of X
         if v[0].X is not None:
-            cols = sorted(list(v[0].X.columns))
+            cols = sorted(v[0].X.columns)
             for i in v:
-                if sorted(list(i.X.columns)) != cols:
+                if sorted(i.X.columns) != cols:
                     raise ValueError("Columns of X do not match.")
         return v
 
     def __len__(self) -> int:
         return len(self.results)
 
     def __iter__(self):
@@ -427,11 +431,11 @@
         cvResults[cv.key].append(
             CrossValidationValues(
                 observed=fold.observed.tolist(),
                 predicted=fold.predicted.tolist(),
                 standardDeviation=fold.standard_deviation.tolist()
                 if fold.standard_deviation is not None
                 else None,
-                metrics=metrics.loc[i].to_dict(),
+                metrics=metrics.loc[i].to_dict() if fold.n_samples > 1 else None,
             )
         )
     return cvResults
```

### Comparing `bofire-0.0.4/bofire/surrogates/empirical.py` & `bofire-0.0.5/bofire/surrogates/empirical.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/bofire/surrogates/feature_importance.py` & `bofire-0.0.5/bofire/surrogates/feature_importance.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/bofire/surrogates/fully_bayesian.py` & `bofire-0.0.5/bofire/surrogates/fully_bayesian.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/bofire/surrogates/mapper.py` & `bofire-0.0.5/bofire/surrogates/mapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,21 +4,25 @@
 from bofire.surrogates.empirical import EmpiricalSurrogate
 from bofire.surrogates.fully_bayesian import SaasSingleTaskGPSurrogate
 from bofire.surrogates.mixed_single_task_gp import MixedSingleTaskGPSurrogate
 from bofire.surrogates.mlp import MLPEnsemble
 from bofire.surrogates.random_forest import RandomForestSurrogate
 from bofire.surrogates.single_task_gp import SingleTaskGPSurrogate
 from bofire.surrogates.surrogate import Surrogate
+from bofire.surrogates.xgb import XGBoostSurrogate
 
 SURROGATE_MAP: Dict[Type[data_models.Surrogate], Type[Surrogate]] = {
     data_models.EmpiricalSurrogate: EmpiricalSurrogate,
     data_models.RandomForestSurrogate: RandomForestSurrogate,
     data_models.SingleTaskGPSurrogate: SingleTaskGPSurrogate,
     data_models.MixedSingleTaskGPSurrogate: MixedSingleTaskGPSurrogate,
     data_models.MLPEnsemble: MLPEnsemble,
     data_models.SaasSingleTaskGPSurrogate: SaasSingleTaskGPSurrogate,
+    data_models.XGBoostSurrogate: XGBoostSurrogate,
+    data_models.LinearSurrogate: SingleTaskGPSurrogate,
+    data_models.TanimotoGPSurrogate: SingleTaskGPSurrogate,
 }
 
 
 def map(data_model: data_models.Surrogate) -> Surrogate:
     cls = SURROGATE_MAP[data_model.__class__]
     return cls.from_spec(data_model=data_model)
```

### Comparing `bofire-0.0.4/bofire/surrogates/mixed_single_task_gp.py` & `bofire-0.0.5/bofire/surrogates/mixed_single_task_gp.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+from functools import partial
 from typing import Dict, Optional
 
 import botorch
 import pandas as pd
 import torch
 from botorch.fit import fit_gpytorch_mll
 from botorch.models.transforms.input import ChainedInputTransform, OneHotToNumeric
 from botorch.models.transforms.outcome import Standardize
 from gpytorch.mlls import ExactMarginalLogLikelihood
 
+import bofire.kernels.api as kernels
 from bofire.data_models.enum import CategoricalEncodingEnum, OutputFilteringEnum
 from bofire.data_models.surrogates.api import MixedSingleTaskGPSurrogate as DataModel
 from bofire.surrogates.botorch import BotorchSurrogate
 from bofire.surrogates.single_task_gp import get_scaler
 from bofire.surrogates.trainable import TrainableSurrogate
 from bofire.utils.torch_tools import tkwargs
 
@@ -66,20 +68,21 @@
         }
 
         o2n = OneHotToNumeric(
             dim=tX.shape[1],
             categorical_features=categorical_features,
             transform_on_train=False,
         )
-        tf = ChainedInputTransform(tf1=scaler, tf2=o2n)
+        tf = ChainedInputTransform(tf1=scaler, tf2=o2n) if scaler is not None else o2n
 
         # fit the model
         self.model = botorch.models.MixedSingleTaskGP(
             train_X=o2n.transform(tX),
             train_Y=tY,
             cat_dims=cat_dims,
-            cont_kernel_factory=self.continuous_kernel.to_gpytorch,
+            # cont_kernel_factory=self.continuous_kernel.to_gpytorch,
+            cont_kernel_factory=partial(kernels.map, data_model=self.continuous_kernel),
             outcome_transform=Standardize(m=tY.shape[-1]),
             input_transform=tf,
         )
         mll = ExactMarginalLogLikelihood(self.model.likelihood, self.model)
         fit_gpytorch_mll(mll, options=self.training_specs)
```

### Comparing `bofire-0.0.4/bofire/surrogates/mlp.py` & `bofire-0.0.5/bofire/surrogates/mlp.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,15 +128,15 @@
     """
     mlp.train()
     train_loader = DataLoader(dataset=dataset, batch_size=batch_size, shuffle=shuffle)
     loss_function = nn.L1Loss()
     optimizer = torch.optim.Adam(mlp.parameters(), lr=lr, weight_decay=weight_decay)
     for _ in range(n_epoches):
         current_loss = 0.0
-        for i, data in enumerate(train_loader, 0):
+        for data in train_loader:
             # Get and prepare inputs
             inputs, targets = data
             if len(targets.shape) == 1:
                 targets = targets.reshape((targets.shape[0], 1))
 
             # Zero the gradients
             optimizer.zero_grad()
@@ -177,22 +177,22 @@
 
     def _fit(self, X: pd.DataFrame, Y: pd.DataFrame):
         scaler = get_scaler(self.inputs, self.input_preprocessing_specs, self.scaler, X)
         transformed_X = self.inputs.transform(X, self.input_preprocessing_specs)
 
         mlps = []
         subsample_size = round(self.subsample_fraction * X.shape[0])
-        for i in range(self.n_estimators):
+        for _ in range(self.n_estimators):
             # resample X and Y
             sample_idx = np.random.choice(X.shape[0], replace=True, size=subsample_size)
             tX = torch.from_numpy(transformed_X.values[sample_idx]).to(**tkwargs)
             ty = torch.from_numpy(Y.values[sample_idx]).to(**tkwargs)
 
             dataset = RegressionDataSet(
-                X=scaler.transform(tX),
+                X=scaler.transform(tX) if scaler is not None else tX,
                 y=ty,
             )
             mlp = MLP(
                 input_size=transformed_X.shape[1],
                 output_size=1,
                 hidden_layer_sizes=self.hidden_layer_sizes,
                 activation=self.activation,  # type: ignore
@@ -205,8 +205,9 @@
                 n_epoches=self.n_epochs,
                 lr=self.lr,
                 shuffle=self.shuffle,
                 weight_decay=self.weight_decay,
             )
             mlps.append(mlp)
         self.model = _MLPEnsemble(mlps=mlps)
-        self.model.input_transform = scaler
+        if scaler is not None:
+            self.model.input_transform = scaler
```

### Comparing `bofire-0.0.4/bofire/surrogates/random_forest.py` & `bofire-0.0.5/bofire/surrogates/random_forest.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/bofire/surrogates/single_task_gp.py` & `bofire-0.0.5/bofire/surrogates/single_task_gp.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,87 +4,98 @@
 import pandas as pd
 import torch
 from botorch.fit import fit_gpytorch_mll
 from botorch.models.transforms.input import InputStandardize, Normalize
 from botorch.models.transforms.outcome import Standardize
 from gpytorch.mlls import ExactMarginalLogLikelihood
 
+import bofire.kernels.api as kernels
+import bofire.priors.api as priors
 from bofire.data_models.domain.api import Inputs
 from bofire.data_models.enum import CategoricalEncodingEnum, OutputFilteringEnum
+from bofire.data_models.features.api import TInputTransformSpecs
+from bofire.data_models.molfeatures.api import MolFeatures
 from bofire.data_models.surrogates.api import SingleTaskGPSurrogate as DataModel
 from bofire.data_models.surrogates.scaler import ScalerEnum
 from bofire.surrogates.botorch import BotorchSurrogate
 from bofire.surrogates.trainable import TrainableSurrogate
 from bofire.utils.torch_tools import tkwargs
 
 
 def get_scaler(
     inputs: Inputs,
-    input_preprocessing_specs: Dict[str, CategoricalEncodingEnum],
+    input_preprocessing_specs: TInputTransformSpecs,
     scaler: ScalerEnum,
     X: pd.DataFrame,
-) -> Union[InputStandardize, Normalize]:
+) -> Union[InputStandardize, Normalize, None]:
     """Returns the instanitated scaler object for a set of input features and
     input_preprocessing_specs.
 
 
     Args:
         inputs (Inputs): Input features.
-        input_preprocessing_specs (Dict[str, CategoricalEncodingEnum]): Dictionary how to treat
-            the categoricals.
+        input_preprocessing_specs (TInputTransformSpecs): Dictionary how to treat
+            the categoricals and/or molecules.
         scaler (ScalerEnum): Enum indicating the scaler of interest.
         X (pd.DataFrame): The dataset of interest.
 
     Returns:
         Union[InputStandardize, Normalize]: The instantiated scaler class
     """
-    features2idx, _ = inputs._get_transform_info(input_preprocessing_specs)
+    if scaler != ScalerEnum.IDENTITY:
+        features2idx, _ = inputs._get_transform_info(input_preprocessing_specs)
 
-    d = 0
-    for indices in features2idx.values():
-        d += len(indices)
-
-    non_numerical_features = [
-        key
-        for key, value in input_preprocessing_specs.items()
-        if value != CategoricalEncodingEnum.DESCRIPTOR
-    ]
-
-    ord_dims = []
-    for feat in inputs.get():
-        if feat.key not in non_numerical_features:
-            ord_dims += features2idx[feat.key]
-
-    if scaler == ScalerEnum.NORMALIZE:
-        lower, upper = inputs.get_bounds(specs=input_preprocessing_specs, experiments=X)
-        scaler_transform = Normalize(
-            d=d,
-            bounds=torch.tensor([lower, upper]).to(**tkwargs),
-            indices=ord_dims,
-            batch_shape=torch.Size(),
-        )
-    elif scaler == ScalerEnum.STANDARDIZE:
-        scaler_transform = InputStandardize(
-            d=d,
-            indices=ord_dims,
-            batch_shape=torch.Size(),
-        )
+        d = 0
+        for indices in features2idx.values():
+            d += len(indices)
+
+        non_numerical_features = [
+            key
+            for key, value in input_preprocessing_specs.items()
+            if value != CategoricalEncodingEnum.DESCRIPTOR
+            and not isinstance(value, MolFeatures)
+        ]
+
+        ord_dims = []
+        for feat in inputs.get():
+            if feat.key not in non_numerical_features:
+                ord_dims += features2idx[feat.key]
+
+        if scaler == ScalerEnum.NORMALIZE:
+            lower, upper = inputs.get_bounds(
+                specs=input_preprocessing_specs, experiments=X
+            )
+            scaler_transform = Normalize(
+                d=d,
+                bounds=torch.tensor([lower, upper]).to(**tkwargs),
+                indices=ord_dims,
+                batch_shape=torch.Size(),
+            )
+        elif scaler == ScalerEnum.STANDARDIZE:
+            scaler_transform = InputStandardize(
+                d=d,
+                indices=ord_dims,
+                batch_shape=torch.Size(),
+            )
+        else:
+            raise ValueError("Scaler enum not known.")
+        return scaler_transform
     else:
-        raise ValueError("Scaler enum not known.")
-    return scaler_transform
+        return None
 
 
 class SingleTaskGPSurrogate(BotorchSurrogate, TrainableSurrogate):
     def __init__(
         self,
         data_model: DataModel,
         **kwargs,
     ):
         self.kernel = data_model.kernel
         self.scaler = data_model.scaler
+        self.noise_prior = data_model.noise_prior
         super().__init__(data_model=data_model, **kwargs)
 
     model: Optional[botorch.models.SingleTaskGP] = None
     _output_filtering: OutputFilteringEnum = OutputFilteringEnum.ALL
     training_specs: Dict = {}
 
     def _fit(self, X: pd.DataFrame, Y: pd.DataFrame):
@@ -94,18 +105,21 @@
         tX, tY = torch.from_numpy(transformed_X.values).to(**tkwargs), torch.from_numpy(
             Y.values
         ).to(**tkwargs)
 
         self.model = botorch.models.SingleTaskGP(  # type: ignore
             train_X=tX,
             train_Y=tY,
-            covar_module=self.kernel.to_gpytorch(
+            covar_module=kernels.map(
+                self.kernel,
                 batch_shape=torch.Size(),
                 active_dims=list(range(tX.shape[1])),
                 ard_num_dims=1,  # this keyword is ingored
             ),
             outcome_transform=Standardize(m=tY.shape[-1]),
             input_transform=scaler,
         )
 
+        self.model.likelihood.noise_covar.noise_prior = priors.map(self.noise_prior)  # type: ignore
+
         mll = ExactMarginalLogLikelihood(self.model.likelihood, self.model)
         fit_gpytorch_mll(mll, options=self.training_specs, max_attempts=10)
```

### Comparing `bofire-0.0.4/bofire/surrogates/surrogate.py` & `bofire-0.0.5/bofire/surrogates/surrogate.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         # return
         return predictions
 
     def validate_predictions(self, predictions: pd.DataFrame) -> pd.DataFrame:
         expected_cols = [
             f"{key}_{t}" for key in self.outputs.get_keys() for t in ["pred", "sd"]
         ]
-        if sorted(list(predictions.columns)) != sorted(expected_cols):
+        if sorted(predictions.columns) != sorted(expected_cols):
             raise ValueError(
                 f"Predictions are ill-formatted. Expected: {expected_cols}, got: {list(predictions.columns)}."
             )
         # check that values are numeric
         if not is_numeric(predictions):
             raise ValueError("Not all values in predictions are numeric.")
         return predictions
@@ -90,15 +90,15 @@
         """Dumps the actual model to a string as this is not directly json serializable."""
         if not self.is_fitted:
             raise ValueError("Model has to be fitted before dumping")
         self._prepare_for_dump()
         return self._dumps()
 
     @abstractmethod
-    def _dumps() -> str:
+    def _dumps(self) -> str:
         pass
 
     def _prepare_for_dump(self):
         """Prepares the model before the dump."""
         pass
 
     @abstractmethod
```

### Comparing `bofire-0.0.4/bofire/surrogates/trainable.py` & `bofire-0.0.5/bofire/surrogates/trainable.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import warnings
 from abc import ABC, abstractmethod
 from typing import Any, Callable, Dict, List, Optional, Tuple
 
 import pandas as pd
 from sklearn.model_selection import KFold
 
 from bofire.data_models.enum import OutputFilteringEnum
@@ -48,36 +49,40 @@
 
     def cross_validate(
         self,
         experiments: pd.DataFrame,
         folds: int = -1,
         include_X: bool = False,
         include_labcodes: bool = False,
-        hooks: Dict[
-            str,
-            Callable[
-                [
-                    Surrogate,
-                    pd.DataFrame,
-                    pd.DataFrame,
-                    pd.DataFrame,
-                    pd.DataFrame,
+        random_state: Optional[int] = None,
+        hooks: Optional[
+            Dict[
+                str,
+                Callable[
+                    [
+                        Surrogate,
+                        pd.DataFrame,
+                        pd.DataFrame,
+                        pd.DataFrame,
+                        pd.DataFrame,
+                    ],
+                    Any,
                 ],
-                Any,
-            ],
-        ] = {},
-        hook_kwargs: Dict[str, Dict[str, Any]] = {},
+            ]
+        ] = None,
+        hook_kwargs: Optional[Dict[str, Dict[str, Any]]] = None,
     ) -> Tuple[CvResults, CvResults, Dict[str, List[Any]]]:
         """Perform a cross validation for the provided training data.
 
         Args:
             experiments (pd.DataFrame): Data on which the cross validation should be performed.
             folds (int, optional): Number of folds. -1 is equal to LOO CV. Defaults to -1.
             include_X (bool, optional): If true the X values of the fold are written to respective CvResult objects for
                 later analysis. Defaults ot False.
+            random_state (int, optional): Controls the randomness of the indices in the train and test sets of each fold.
             hooks (Dict[str, Callable[[Model, pd.DataFrame, pd.DataFrame, pd.DataFrame, pd.DataFrame], Any]], optional):
                 Dictionary of callable hooks that are called within the CV loop. The callable retrieves the current trained
                 modeld and the current CV folds in the following order: X_train, y_train, X_test, y_test. Defaults to {}.
             hook_kwargs (Dict[str, Dict[str, Any]], optional): Dictionary holding hook specefic keyword arguments.
                 Defaults to {}.
 
         Returns:
@@ -89,27 +94,32 @@
 
         if len(self.outputs) > 1:  # type: ignore
             raise NotImplementedError(
                 "Cross validation not implemented for multi-output models"
             )
         n = len(experiments)
         if folds > n:
-            raise ValueError(
-                f"Training data only has {n} experiments, which is less than folds"
+            warnings.warn(
+                f"Training data only has {n} experiments, which is less than folds, fallback to LOOCV."
             )
+            folds = n
         elif n == 0:
             raise ValueError("Experiments is empty.")
         elif folds < 2 and folds != -1:
             raise ValueError("Folds must be -1 for LOO, or > 1.")
         elif folds == -1:
             folds = n
         # preprocess hooks
+        if hooks is None:
+            hooks = {}
+        if hook_kwargs is None:
+            hook_kwargs = {}
         hook_results = {key: [] for key in hooks.keys()}
         # instantiate kfold object
-        cv = KFold(n_splits=folds, shuffle=True)
+        cv = KFold(n_splits=folds, shuffle=True, random_state=random_state)
         key = self.outputs.get_keys()[0]  # type: ignore
         # first filter the experiments based on the model setting
         experiments = self._preprocess_experiments(experiments)
         train_results = []
         test_results = []
         # now get the indices for the split
         for train_index, test_index in cv.split(experiments):
```

### Comparing `bofire-0.0.4/bofire/surrogates/values.py` & `bofire-0.0.5/bofire/surrogates/values.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/bofire/utils/doe.py` & `bofire-0.0.5/bofire/utils/doe.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import itertools
 import warnings
-from typing import List
+from typing import List, Optional
 
 import pandas as pd
 from sklearn.preprocessing import MinMaxScaler
 
 from bofire.data_models.domain.api import Inputs
 from bofire.data_models.features.api import CategoricalInput, ContinuousInput
 
 
 def get_confounding_matrix(
     inputs: Inputs,
     design: pd.DataFrame,
-    powers: List[int] = [],
-    interactions: List[int] = [2],
+    powers: Optional[List[int]] = None,
+    interactions: Optional[List[int]] = None,
 ):
     """Analyzes the confounding of a design and returns the confounding matrix.
 
     Only takes continuous features into account.
 
     Args:
         inputs (Inputs): Input features.
@@ -35,20 +35,26 @@
 
     keys = inputs.get_keys(ContinuousInput)
     scaler = MinMaxScaler(feature_range=(-1, 1))
     scaled_design = pd.DataFrame(
         data=scaler.fit_transform(design[keys]),
         columns=keys,
     )
+
     # add powers
-    for p in powers:
-        assert p > 1, "Power has to be at least of degree two."
-        for key in keys:
-            scaled_design[f"{key}**{p}"] = scaled_design[key] ** p
+    if powers is not None:
+        for p in powers:
+            assert p > 1, "Power has to be at least of degree two."
+            for key in keys:
+                scaled_design[f"{key}**{p}"] = scaled_design[key] ** p
 
     # add interactions
+    if interactions is None:
+        interactions = [2]
+
     for i in interactions:
         assert i > 1, "Interaction has to be at least of degree two."
         assert i < len(keys) + 1, f"Interaction has to be smaller than {len(keys)+1}."
         for combi in itertools.combinations(keys, i):
             scaled_design[":".join(combi)] = scaled_design[list(combi)].prod(axis=1)
+
     return scaled_design.corr()
```

### Comparing `bofire-0.0.4/bofire/utils/multiobjective.py` & `bofire-0.0.5/bofire/utils/multiobjective.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/bofire/utils/reduce.py` & `bofire-0.0.5/bofire/utils/reduce.py`

 * *Files 1% similar despite different names*

```diff
@@ -287,15 +287,15 @@
     M = len(inputs_names)
 
     # write the equalities for the backtransformation into one matrix
     inputs_dict = {inputs_names[i]: i for i in range(M)}
 
     # build up dict from domain.equalities e.g. {"xi1": [coeff(xj1), ..., coeff(xjn)], ... "xik":...}
     coeffs_dict = {}
-    for i, e in enumerate(transform.equalities):
+    for e in transform.equalities:
         coeffs = np.zeros(M + 1)
         for j, name in enumerate(e[1]):
             coeffs[inputs_dict[name]] = e[2][j]
         coeffs[-1] = e[2][-1]
         coeffs_dict[e[0]] = coeffs
 
     constraints = []
```

### Comparing `bofire-0.0.4/bofire/utils/subdomain.py` & `bofire-0.0.5/bofire/utils/subdomain.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/bofire/utils/torch_tools.py` & `bofire-0.0.5/bofire/utils/torch_tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -259,14 +259,54 @@
         )
     else:
         raise NotImplementedError(
             f"Objective {objective.__class__.__name__} not implemented."
         )
 
 
+def get_custom_botorch_objective(
+    outputs: Outputs,
+    f: Callable[
+        [
+            Tensor,
+            List[Callable[[Tensor, Optional[Tensor]], Tensor]],
+            List[float],
+            Tensor,
+        ],
+        Tensor,
+    ],
+    exclude_constraints: bool = True,
+) -> Callable[[Tensor, Tensor], Tensor]:
+    callables = [
+        get_objective_callable(idx=i, objective=feat.objective)  # type: ignore
+        for i, feat in enumerate(outputs.get())
+        if feat.objective is not None  # type: ignore
+        and (
+            not isinstance(feat.objective, ConstrainedObjective)  # type: ignore
+            if exclude_constraints
+            else True
+        )
+    ]
+    weights = [
+        feat.objective.w  # type: ignore
+        for i, feat in enumerate(outputs.get())
+        if feat.objective is not None  # type: ignore
+        and (
+            not isinstance(feat.objective, ConstrainedObjective)  # type: ignore
+            if exclude_constraints
+            else True
+        )
+    ]
+
+    def objective(samples: torch.Tensor, X: torch.Tensor) -> torch.Tensor:
+        return f(samples, callables, weights, X)
+
+    return objective
+
+
 def get_multiplicative_botorch_objective(
     outputs: Outputs,
 ) -> Callable[[Tensor, Tensor], Tensor]:
     callables = [
         get_objective_callable(idx=i, objective=feat.objective)  # type: ignore
         for i, feat in enumerate(outputs.get())
         if feat.objective is not None  # type: ignore
@@ -345,15 +385,15 @@
 
     return objective
 
 
 def get_initial_conditions_generator(
     strategy: Strategy,
     transform_specs: Dict,
-    ask_options: Dict = {},
+    ask_options: Optional[Dict] = None,
     sequential: bool = True,
 ) -> Callable[[int, int, int], Tensor]:
     """Takes a strategy object and returns a callable which uses this
     strategy to return a generator callable which can be used in botorch`s
     `gen_batch_initial_conditions` to generate samples.
 
     Args:
@@ -366,14 +406,16 @@
             generate indepenent from each other. If False, the `n x q` samples
             are generated at once.
 
     Returns:
         Callable[[int, int, int], Tensor]: Callable that can be passed to
             `batch_initial_conditions`.
     """
+    if ask_options is None:
+        ask_options = {}
 
     def generator(n: int, q: int, seed: int) -> Tensor:
         if sequential:
             initial_conditions = []
             for _ in range(n):
                 candidates = strategy.ask(q, **ask_options)
                 # transform it
```

### Comparing `bofire-0.0.4/bofire.egg-info/PKG-INFO` & `bofire-0.0.5/bofire.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: bofire
-Version: 0.0.4
+Version: 0.0.5
 Home-page: https://github.com/experimental-design/bofire
 Author: 
 License: BSD-3
 Keywords: Bayesian optimization,Multi-objective optimization,Experimental design
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: optimization
+Provides-Extra: xgb
 Provides-Extra: cheminfo
 Provides-Extra: tests
 Provides-Extra: docs
 License-File: LICENSE
 
 # BoFire
```

### Comparing `bofire-0.0.4/setup.py` & `bofire-0.0.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,13 @@
 import os.path
 
 from setuptools import find_packages, setup
 
 sklearn_dependency = "scikit-learn>=1.0.0"
 
-
-def get_version():
-    here = os.path.abspath(os.path.dirname(__file__))
-    fp = os.path.join(here, "bofire/__init__.py")
-    for line in open(fp).readlines():
-        if line.startswith("__version__"):
-            return line.split('"')[1]
-    return ""
-
-
 root_dir = os.path.dirname(__file__)
 with open(os.path.join(root_dir, "README.md"), "r") as f:
     long_description = f.read()
 
 
 setup(
     name="bofire",
@@ -36,35 +26,37 @@
         "License :: OSI Approved :: BSD License",
         "Topic :: Scientific/Engineering",
         "Intended Audience :: Science/Research",
         "Intended Audience :: Developers",
     ],
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version=get_version(),
-    python_requires=">=3.9",
+    python_requires=">=3.8",
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         "numpy",
         "pandas",
         "pydantic>=1.10.0,<2.0",
         "scipy>=1.7",
+        "typing-extensions",
     ],
     extras_require={
         "optimization": [
             "torch>=1.12",
-            "botorch>=0.8.4",
+            "botorch==0.8.5",
             "multiprocess",
             "plotly",
             "formulaic>=0.6.0",
             "cloudpickle>=2.0.0",
+            "sympy>=1.12",
             sklearn_dependency,
         ],
-        "cheminfo": ["rdkit", sklearn_dependency],
+        "xgb": ["xgboost>=1.7.5"],
+        "cheminfo": ["rdkit>=2023.3.2", sklearn_dependency, "mordred"],
         "tests": [
             "mock",
             "mopti",
             "pyright==1.1.305",
             "pytest",
             "pytest-cov",
             "papermill",
```

### Comparing `bofire-0.0.4/tests/bofire/benchmarks/test_aspen_benchmark.py` & `bofire-0.0.5/tests/bofire/benchmarks/test_aspen_benchmark.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/tests/bofire/benchmarks/test_benchmark.py` & `bofire-0.0.5/tests/bofire/benchmarks/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/tests/bofire/benchmarks/test_multi.py` & `bofire-0.0.5/tests/bofire/benchmarks/test_multi.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/tests/bofire/benchmarks/test_single.py` & `bofire-0.0.5/tests/bofire/benchmarks/test_single.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/tests/bofire/conftest.py` & `bofire-0.0.5/tests/bofire/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,9 +42,21 @@
     def prior_spec(request) -> specs.Spec:
         return request.param
 
     @fixture(params=specs.kernels.valids)
     def kernel_spec(request) -> specs.Spec:
         return request.param
 
+    @fixture(params=specs.conditions.valids)
+    def condition_spec(request) -> specs.Spec:
+        return request.param
+
+    @fixture(params=specs.outlier_detection.valids)
+    def outlier_detection_spec(request) -> specs.Spec:
+        return request.param
+
+    @fixture(params=specs.molfeatures.valids)
+    def molfeatures_spec(request) -> specs.Spec:
+        return request.param
+
 except AttributeError:
     pass
```

### Comparing `bofire-0.0.4/tests/bofire/data_models/serialization/test_deserialization.py` & `bofire-0.0.5/tests/bofire/data_models/serialization/test_deserialization.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from pydantic import parse_obj_as
 
 from bofire.data_models.api import (
     AnyAcquisitionFunction,
+    AnyCondition,
     AnyConstraint,
     AnyFeature,
     AnyKernel,
+    AnyMolFeatures,
     AnyObjective,
+    AnyOutlierDetection,
     AnyPrior,
     AnyStrategy,
     AnySurrogate,
     Domain,
 )
 from tests.bofire.data_models.specs.api import Spec
 
@@ -60,17 +63,32 @@
     obj = acquisition_function_spec.obj()
     deserialized = parse_obj_as(AnyAcquisitionFunction, obj.dict())
     assert obj == deserialized
 
 
 def test_strategy_should_be_deserializable(strategy_spec: Spec):
     obj = strategy_spec.obj()
-    print("obj:", type(obj))
-    print(obj)
-    print(obj.dict().keys())
     deserialized = parse_obj_as(AnyStrategy, obj.dict())
     # TODO: can we unhide the comparison of surrogate_specs?
     obj = {k: v for k, v in obj.dict().items() if k != "surrogate_specs"}
     deserialized = {
         k: v for k, v in deserialized.dict().items() if k != "surrogate_specs"
     }
     assert obj == deserialized
+
+
+def test_condition_should_be_deserializable(condition_spec: Spec):
+    obj = condition_spec.obj()
+    deserialized = parse_obj_as(AnyCondition, obj.dict())
+    assert obj == deserialized
+
+
+def test_outlier_detection_should_be_deserializable(outlier_detection_spec: Spec):
+    obj = outlier_detection_spec.obj()
+    deserialized = parse_obj_as(AnyOutlierDetection, obj.dict())
+    assert obj == deserialized
+
+
+def test_molfeatures_should_be_deserializable(molfeatures_spec: Spec):
+    obj = molfeatures_spec.obj()
+    deserialized = parse_obj_as(AnyMolFeatures, obj.dict())
+    assert obj == deserialized
```

### Comparing `bofire-0.0.4/tests/bofire/data_models/serialization/test_serialization.py` & `bofire-0.0.5/tests/bofire/data_models/serialization/test_serialization.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,7 +54,25 @@
     spec = strategy_spec.typed_spec()
     obj = strategy_spec.cls(**spec)
     # TODO: can we unhide the comparison of surrogate_specs?
     data = {k: v for k, v in obj.dict().items() if k != "surrogate_specs"}
     for k, v in data.items():
         if v is not None:
             assert v == spec[k]
+
+
+def test_condition_should_be_serializable(condition_spec: Spec):
+    spec = condition_spec.typed_spec()
+    obj = condition_spec.cls(**spec)
+    assert obj.dict() == spec
+
+
+def test_outlier_detection_should_be_serializable(outlier_detection_spec: Spec):
+    spec = outlier_detection_spec.typed_spec()
+    obj = outlier_detection_spec.cls(**spec)
+    assert obj.dict() == spec
+
+
+def test_molfeatures_should_be_serializable(molfeatures_spec: Spec):
+    spec = molfeatures_spec.typed_spec()
+    obj = molfeatures_spec.cls(**spec)
+    assert obj.dict() == spec
```

### Comparing `bofire-0.0.4/tests/bofire/data_models/specs/acquisition_functions.py` & `bofire-0.0.5/tests/bofire/data_models/specs/acquisition_functions.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/tests/bofire/data_models/specs/api.py` & `bofire-0.0.5/tests/bofire/data_models/specs/api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-from tests.bofire.data_models.specs.acquisition_functions import (  # noqa: F401
+from tests.bofire.data_models.specs.acquisition_functions import (
     specs as acquisition_functions,
 )
-from tests.bofire.data_models.specs.constraints import (  # noqa: F401
-    specs as constraints,
-)
-from tests.bofire.data_models.specs.domain import specs as domain  # noqa: F401
-from tests.bofire.data_models.specs.features import specs as features  # noqa: F401
-from tests.bofire.data_models.specs.objectives import specs as objectives  # noqa: F401
-from tests.bofire.data_models.specs.specs import Spec, Specs  # noqa: F401
+from tests.bofire.data_models.specs.constraints import specs as constraints
+from tests.bofire.data_models.specs.domain import specs as domain
+from tests.bofire.data_models.specs.features import specs as features
+from tests.bofire.data_models.specs.objectives import specs as objectives
+from tests.bofire.data_models.specs.specs import Spec, Specs
 
 try:
     # in case of the minimal installation these import are not available
-    from tests.bofire.data_models.specs.kernels import specs as kernels  # noqa: F401
-    from tests.bofire.data_models.specs.priors import specs as priors  # noqa: F401
-    from tests.bofire.data_models.specs.strategies import (  # noqa: F401
-        specs as strategies,
+    from tests.bofire.data_models.specs.conditions import specs as conditions
+    from tests.bofire.data_models.specs.kernels import specs as kernels
+    from tests.bofire.data_models.specs.molfeatures import (
+        specs as molfeatures,
     )
-    from tests.bofire.data_models.specs.surrogates import (  # noqa: F401
-        specs as surrogates,
+    from tests.bofire.data_models.specs.outlier_detection import (
+        specs as outlier_detection,
     )
+    from tests.bofire.data_models.specs.priors import specs as priors
+    from tests.bofire.data_models.specs.strategies import specs as strategies
+    from tests.bofire.data_models.specs.surrogates import specs as surrogates
 except ImportError:
     pass
```

### Comparing `bofire-0.0.4/tests/bofire/data_models/specs/constraints.py` & `bofire-0.0.5/tests/bofire/data_models/specs/constraints.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/tests/bofire/data_models/specs/domain.py` & `bofire-0.0.5/tests/bofire/data_models/specs/domain.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/tests/bofire/data_models/specs/features.py` & `bofire-0.0.5/tests/bofire/data_models/specs/features.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+# import importlib
 import random
 import uuid
 
 import bofire.data_models.features.api as features
 from bofire.data_models.objectives.api import MaximizeObjective
 from tests.bofire.data_models.specs.objectives import specs as objectives
 from tests.bofire.data_models.specs.specs import Specs
 
+# RDKIT_AVAILABLE = importlib.util.find_spec("rdkit") is not None
+
 specs = Specs([])
 
 specs.add_valid(
     features.DiscreteInput,
     lambda: {
         "key": str(uuid.uuid4()),
         "values": [random.random(), random.random() + 3],
@@ -65,20 +68,14 @@
             [1.0, 2.0],
             [3.0, 7.0],
             [5.0, 1.0],
         ],
     },
 )
 specs.add_valid(
-    features.MolecularInput,
-    lambda: {
-        "key": str(uuid.uuid4()),
-    },
-)
-specs.add_valid(
     features.ContinuousOutput,
     lambda: {
         "key": str(uuid.uuid4()),
         "objective": objectives.valid(MaximizeObjective).typed_spec(),
         "unit": random.choice(["%", "area %", None]),
     },
 )
@@ -87,7 +84,13 @@
     features.CategoricalOutput,
     lambda: {
         "key": str(uuid.uuid4()),
         "categories": ["a", "b", "c"],
         "objective": [0.0, 1.0, 0.0],
     },
 )
+specs.add_valid(
+    features.MolecularInput,
+    lambda: {
+        "key": str(uuid.uuid4()),
+    },
+)
```

### Comparing `bofire-0.0.4/tests/bofire/data_models/specs/kernels.py` & `bofire-0.0.5/tests/bofire/data_models/specs/kernels.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     kernels.HammondDistanceKernel,
     lambda: {
         "ard": False,
     },
 )
 specs.add_valid(
     kernels.LinearKernel,
-    lambda: {},
+    lambda: {"variance_prior": priors.valid().obj()},
 )
 specs.add_valid(
     kernels.MaternKernel,
     lambda: {
         "ard": True,
         "nu": random.random(),
         "lengthscale_prior": priors.valid().obj(),
@@ -52,7 +52,13 @@
     lambda: {
         "kernels": [
             specs.valid(kernels.LinearKernel).obj(),
             specs.valid(kernels.MaternKernel).obj(),
         ]
     },
 )
+specs.add_valid(
+    kernels.TanimotoKernel,
+    lambda: {
+        "ard": True,
+    },
+)
```

### Comparing `bofire-0.0.4/tests/bofire/data_models/specs/objectives.py` & `bofire-0.0.5/tests/bofire/data_models/specs/objectives.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,36 +9,34 @@
         "target_value": 42,
         "exponent": 2,
         "w": 1.0,
     },
 )
 specs.add_valid(
     objectives.MaximizeObjective,
-    lambda: {
-        "w": 1.0,
-        "lower_bound": 0.1,
-        "upper_bound": 0.9,
-    },
+    lambda: {"w": 1.0, "bounds": (0.1, 0.9)},
 )
 specs.add_valid(
     objectives.MaximizeSigmoidObjective,
     lambda: {
         "steepness": 0.2,
         "tp": 0.3,
         "w": 1.0,
     },
 )
 specs.add_valid(
     objectives.MinimizeObjective,
-    lambda: {
-        "w": 1.0,
-        "lower_bound": 0.1,
-        "upper_bound": 0.9,
-    },
+    lambda: {"w": 1.0, "bounds": (0.1, 0.9)},
+)
+
+specs.add_invalid(
+    objectives.MinimizeObjective,
+    lambda: {"w": 1.0, "lower_bound": 0.1, "upper_bound": 0.9},
 )
+
 specs.add_valid(
     objectives.MinimizeSigmoidObjective,
     lambda: {
         "steepness": 0.2,
         "tp": 0.3,
         "w": 1.0,
     },
```

### Comparing `bofire-0.0.4/tests/bofire/data_models/specs/specs.py` & `bofire-0.0.5/tests/bofire/data_models/specs/specs.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         self.overwrites = overwrites
 
     def invalidate(self, spec: Spec) -> List[Spec]:
         data: dict = spec.spec()
         if self.key not in data:
             return []
         return [
-            Spec(spec.cls, lambda: {**data, **overwrite})
+            Spec(spec.cls, lambda data=data, overwrite=overwrite: {**data, **overwrite})
             for overwrite in self.overwrites
         ]
 
 
 class Specs:
     """Collection of valid and invalid specs.
```

### Comparing `bofire-0.0.4/tests/bofire/data_models/specs/strategies.py` & `bofire-0.0.5/tests/bofire/data_models/specs/strategies.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 import bofire.data_models.strategies.api as strategies
 from bofire.benchmarks.single import Himmelblau
 from bofire.data_models.acquisition_functions.api import qPI
 from bofire.data_models.domain.api import Domain, Inputs
 from bofire.data_models.enum import CategoricalMethodEnum, SamplingMethodEnum
-from bofire.data_models.features.api import ContinuousInput
+from bofire.data_models.features.api import (
+    CategoricalInput,
+    ContinuousInput,
+    DiscreteInput,
+)
 from tests.bofire.data_models.specs.api import domain
 from tests.bofire.data_models.specs.specs import Specs
 
 specs = Specs([])
 
 
 strategy_commons = {
@@ -66,14 +70,23 @@
     lambda: {
         "domain": domain.valid().obj().dict(),
         **strategy_commons,
         "acquisition_function": qPI(tau=0.1).dict(),
     },
 )
 specs.add_valid(
+    strategies.CustomSoboStrategy,
+    lambda: {
+        "domain": domain.valid().obj().dict(),
+        **strategy_commons,
+        "acquisition_function": qPI(tau=0.1).dict(),
+        "use_output_constraints": True,
+    },
+)
+specs.add_valid(
     strategies.RandomStrategy,
     lambda: {
         "domain": domain.valid().obj().dict(),
         "seed": 42,
     },
 )
 
@@ -100,20 +113,58 @@
                     ContinuousInput(key=f"x_{i}", bounds=(0, 1)) for i in range(2)
                 ]
             )
         ),
         "max_iters": 1000,
         "num_base_samples": 1000,
         "sampling_method": SamplingMethodEnum.UNIFORM,
-        "num_base_samples": 1000,
-        "max_iters": 1000,
         "seed": 42,
     },
 )
 specs.add_valid(
     strategies.DoEStrategy,
     lambda: {
         "domain": domain.valid().obj().dict(),
         "formula": "linear",
         "seed": 42,
     },
 )
+
+tempdomain = domain.valid().obj().dict()
+
+specs.add_valid(
+    strategies.StepwiseStrategy,
+    lambda: {
+        "domain": tempdomain,
+        "steps": [
+            strategies.Step(
+                strategy_data=strategies.RandomStrategy(domain=tempdomain),
+                condition=strategies.NumberOfExperimentsCondition(n_experiments=10),
+                max_parallelism=2,
+            ).dict(),
+            strategies.Step(
+                strategy_data=strategies.QehviStrategy(
+                    domain=tempdomain,
+                ),
+                condition=strategies.NumberOfExperimentsCondition(n_experiments=30),
+                max_parallelism=2,
+            ).dict(),
+        ],
+        "seed": 42,
+    },
+)
+
+
+specs.add_valid(
+    strategies.FactorialStrategy,
+    lambda: {
+        "domain": Domain(
+            inputs=Inputs(
+                features=[
+                    CategoricalInput(key="alpha", categories=["a", "b", "c"]),
+                    DiscreteInput(key="beta", values=[1.0, 2, 3.0, 4.0]),
+                ]
+            )
+        ),
+        "seed": 42,
+    },
+)
```

### Comparing `bofire-0.0.4/tests/bofire/data_models/specs/surrogates.py` & `bofire-0.0.5/tests/bofire/data_models/specs/surrogates.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,22 +3,30 @@
 import bofire.data_models.surrogates.api as models
 from bofire.data_models.domain.api import Inputs, Outputs
 from bofire.data_models.enum import CategoricalEncodingEnum
 from bofire.data_models.features.api import (
     CategoricalInput,
     ContinuousInput,
     ContinuousOutput,
+    MolecularInput,
 )
 from bofire.data_models.kernels.api import (
     HammondDistanceKernel,
     MaternKernel,
     ScaleKernel,
+    TanimotoKernel,
+)
+from bofire.data_models.molfeatures.api import Fingerprints
+from bofire.data_models.priors.api import (
+    BOTORCH_LENGTHCALE_PRIOR,
+    BOTORCH_NOISE_PRIOR,
+    BOTORCH_SCALE_PRIOR,
 )
-from bofire.data_models.priors.api import BOTORCH_LENGTHCALE_PRIOR, BOTORCH_SCALE_PRIOR
 from bofire.data_models.surrogates.api import ScalerEnum
+from bofire.data_models.surrogates.single_task_gp import SingleTaskGPHyperconfig
 from tests.bofire.data_models.specs.features import specs as features
 from tests.bofire.data_models.specs.specs import Specs
 
 specs = Specs([])
 
 specs.add_valid(
     models.SaasSingleTaskGPSurrogate,
@@ -36,14 +44,15 @@
         ),
         "warmup_steps": 16,
         "num_samples": 4,
         "thinning": 2,
         "scaler": ScalerEnum.NORMALIZE,
         "input_preprocessing_specs": {"cat1": CategoricalEncodingEnum.ONE_HOT},
         "dump": None,
+        "hyperconfig": None,
     },
 )
 
 specs.add_valid(
     models.MixedSingleTaskGPSurrogate,
     lambda: {
         "inputs": Inputs(
@@ -58,14 +67,15 @@
             ]
         ),
         "continuous_kernel": MaternKernel(ard=True, nu=random.random()),
         "categorical_kernel": HammondDistanceKernel(ard=True),
         "scaler": ScalerEnum.NORMALIZE,
         "input_preprocessing_specs": {"cat1": CategoricalEncodingEnum.ONE_HOT},
         "dump": None,
+        "hyperconfig": None,
     },
 )
 specs.add_valid(
     models.SingleTaskGPSurrogate,
     lambda: {
         "inputs": Inputs(
             features=[
@@ -75,21 +85,23 @@
         "outputs": Outputs(
             features=[
                 features.valid(ContinuousOutput).obj(),
             ]
         ),
         "kernel": ScaleKernel(
             base_kernel=MaternKernel(
-                ard=True, nu=2.5, lengthscale_prior=BOTORCH_LENGTHCALE_PRIOR
+                ard=True, nu=2.5, lengthscale_prior=BOTORCH_LENGTHCALE_PRIOR()
             ),
-            outputscale_prior=BOTORCH_SCALE_PRIOR,
+            outputscale_prior=BOTORCH_SCALE_PRIOR(),
         ),
         "scaler": ScalerEnum.NORMALIZE,
+        "noise_prior": BOTORCH_NOISE_PRIOR(),
         "input_preprocessing_specs": {},
         "dump": None,
+        "hyperconfig": SingleTaskGPHyperconfig(),
     },
 )
 specs.add_valid(
     models.RandomForestSurrogate,
     lambda: {
         "inputs": Inputs(
             features=[
@@ -113,14 +125,15 @@
         "min_impurity_decrease": 0.0,
         "bootstrap": True,
         "oob_score": False,
         "random_state": None,
         "ccp_alpha": 0.0,
         "max_samples": None,
         "dump": None,
+        "hyperconfig": None,
     },
 )
 specs.add_valid(
     models.MLPEnsemble,
     lambda: {
         "inputs": Inputs(
             features=[
@@ -141,9 +154,77 @@
         "lr": 1e-4,
         "weight_decay": 0.0,
         "subsample_fraction": 1.0,
         "shuffle": True,
         "scaler": ScalerEnum.NORMALIZE,
         "input_preprocessing_specs": {},
         "dump": None,
+        "hyperconfig": None,
+    },
+)
+
+specs.add_valid(
+    models.XGBoostSurrogate,
+    lambda: {
+        "inputs": Inputs(
+            features=[
+                features.valid(ContinuousInput).obj(),
+            ]
+        ),
+        "outputs": Outputs(
+            features=[
+                features.valid(ContinuousOutput).obj(),
+            ]
+        ),
+        "n_estimators": 10,
+        "max_depth": 6,
+        "max_leaves": 0,
+        "max_bin": 256,
+        "grow_policy": "depthwise",
+        "learning_rate": 0.3,
+        "objective": "reg:squarederror",
+        "booster": "gbtree",
+        "n_jobs": 1,
+        "gamma": 0.0,
+        "min_child_weight": 1.0,
+        "max_delta_step": 0.0,
+        "subsample": 1.0,
+        "sampling_method": "uniform",
+        "colsample_bytree": 1.0,
+        "colsample_bylevel": 1.0,
+        "colsample_bynode": 1.0,
+        "reg_alpha": 0.0,
+        "reg_lambda": 1.0,
+        "scale_pos_weight": 1,
+        "random_state": None,
+        "num_parallel_tree": 1,
+        "input_preprocessing_specs": {},
+        "dump": None,
+        "hyperconfig": None,
+    },
+)
+specs.add_valid(
+    models.TanimotoGPSurrogate,
+    lambda: {
+        "inputs": Inputs(
+            features=[
+                MolecularInput(key="mol1"),
+            ]
+        ),
+        "outputs": Outputs(
+            features=[
+                features.valid(ContinuousOutput).obj(),
+            ]
+        ),
+        "kernel": ScaleKernel(
+            base_kernel=TanimotoKernel(
+                ard=True,
+            ),
+            outputscale_prior=BOTORCH_SCALE_PRIOR(),
+        ),
+        "scaler": ScalerEnum.NORMALIZE,
+        "noise_prior": BOTORCH_NOISE_PRIOR(),
+        "input_preprocessing_specs": {"mol1": Fingerprints(n_bits=32, bond_radius=3)},
+        "dump": None,
+        "hyperconfig": None,
     },
 )
```

### Comparing `bofire-0.0.4/tests/bofire/data_models/test_base.py` & `bofire-0.0.5/tests/bofire/data_models/test_base.py`

 * *Files 21% similar despite different names*

```diff
@@ -30,7 +30,12 @@
     bla.a = a
     assert bla.a == a
 
 
 def test_assignment_validation_invalid(bla, b):
     with pytest.raises(ValidationError):
         bla.a = b
+
+
+def test_forbid_extra():
+    with pytest.raises(ValidationError):
+        Bla(a=2, mama="papa")
```

### Comparing `bofire-0.0.4/tests/bofire/data_models/test_constraint_fulfillment.py` & `bofire-0.0.5/tests/bofire/data_models/test_constraint_fulfillment.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 C = list(range(1, 11))
 
 
 def get_row(features, value: float = None, values: List[float] = None):
     if values is None:
         values = [value for _ in range(len(features))]
-    return pd.DataFrame.from_dict([{f: v for f, v in zip(features, values)}])
+    return pd.DataFrame.from_dict([dict(zip(features, values))])
 
 
 @pytest.mark.parametrize(
     "df, constraint, fulfilled",
     [
         (
             get_row(F[:4], 1),
```

### Comparing `bofire-0.0.4/tests/bofire/data_models/test_constraints.py` & `bofire-0.0.5/tests/bofire/data_models/test_constraints.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/tests/bofire/data_models/test_domain.py` & `bofire-0.0.5/tests/bofire/data_models/test_domain.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/tests/bofire/data_models/test_domain_validators.py` & `bofire-0.0.5/tests/bofire/data_models/test_domain_validators.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,18 @@
 from typing import List
 
 import numpy as np
 import pandas as pd
 import pytest
 
 import tests.bofire.data_models.specs.api as specs
-from bofire.data_models.constraints.api import LinearEqualityConstraint
+from bofire.data_models.constraints.api import (
+    ConstraintNotFulfilledError,
+    LinearEqualityConstraint,
+)
 from bofire.data_models.domain.api import Domain
 from bofire.data_models.features.api import (
     CategoricalDescriptorInput,
     CategoricalInput,
     ContinuousInput,
     ContinuousOutput,
     DiscreteInput,
@@ -197,19 +200,16 @@
 ):
     domain.validate_experiments(experiments)
 
 
 @pytest.mark.parametrize(
     "domain, experiments, strict",
     [
-        (d1, generate_experiments(d2), strict)
-        for strict in [True, False]
-        for d1 in domains
-        for d2 in domains
-        if d1 != d2
+        (domains[0], generate_experiments(domains[1]), True),
+        (domains[0], generate_experiments(domains[1]), False),
     ],
 )
 def test_domain_validate_experiments_invalid(
     domain: Domain, experiments: pd.DataFrame, strict: bool
 ):
     with pytest.raises(ValueError):
         domain.validate_experiments(experiments, strict=strict)
@@ -339,12 +339,29 @@
 ):
     candidates[key] = str(uuid.uuid4())
     with pytest.raises(ValueError):
         domain.validate_candidates(candidates)
 
 
 @pytest.mark.parametrize(
-    "domain, candidates", [(d, generate_candidates(d)) for d in [domain7]]
+    "domain, candidates, raise_validation_error",
+    [
+        (d, generate_candidates(d), raise_validation_error)
+        for d in [domain7]
+        for raise_validation_error in [True, False]
+    ],
 )
-def test_domain_validate_candidates_constraint_not_fulfilled(domain, candidates):
-    with pytest.raises(ValueError):
-        domain.validate_candidates(candidates)
+def test_domain_validate_candidates_constraint_not_fulfilled(
+    domain, candidates, raise_validation_error
+):
+    if raise_validation_error:
+        with pytest.raises(ConstraintNotFulfilledError):
+            domain.validate_candidates(
+                candidates, raise_validation_error=raise_validation_error
+            )
+    else:
+        assert isinstance(
+            domain.validate_candidates(
+                candidates, raise_validation_error=raise_validation_error
+            ),
+            pd.DataFrame,
+        )
```

### Comparing `bofire-0.0.4/tests/bofire/data_models/test_features.py` & `bofire-0.0.5/tests/bofire/data_models/test_features.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import importlib
 import random
 
 import numpy as np
 import pandas as pd
 import pytest
 from pandas.testing import assert_frame_equal, assert_series_equal
 from pydantic.error_wrappers import ValidationError
@@ -17,19 +18,27 @@
     ContinuousInput,
     ContinuousOutput,
     DiscreteInput,
     Feature,
     MolecularInput,
     Output,
 )
+from bofire.data_models.molfeatures.api import (
+    Fingerprints,
+    FingerprintsFragments,
+    Fragments,
+    MordredDescriptors,
+)
 from bofire.data_models.objectives.api import MinimizeObjective, Objective
 from bofire.data_models.surrogates.api import ScalerEnum
 
 objective = MinimizeObjective(w=1)
 
+RDKIT_AVAILABLE = importlib.util.find_spec("rdkit") is not None
+
 
 @pytest.mark.parametrize(
     "spec, n",
     [
         (spec, n)
         for spec in specs.features.valids
         if (spec.cls != ContinuousOutput)
@@ -442,32 +451,22 @@
             pd.Series([random.choice(["a", "b", "c"]) for _ in range(20)]),
             # CategoricalInput(**VALID_FIXED_CATEGORICAL_INPUT_FEATURE_SPEC),
             # pd.Series([random.choice(["c1", "c2", "c3"]) for _ in range(20)]),
             True,
         ),
         (
             specs.features.valid(CategoricalInput).obj(
-                categories=["a", "b", "c"],
+                categories=["1", "2", "3"],
                 allowed=[True, False, False],
             ),
-            pd.Series([random.choice(["a", "b", "c"]) for _ in range(20)]),
+            pd.Series([random.choice([1, 2, 3]) for _ in range(20)]),
             # CategoricalInput(**VALID_FIXED_CATEGORICAL_INPUT_FEATURE_SPEC),
             # pd.Series([random.choice(["c1", "c2", "c3"]) for _ in range(20)]),
             False,
         ),
-        (
-            specs.features.valid(CategoricalInput).obj(
-                categories=["a", "b", "c"],
-                allowed=[True, False, False],
-            ),
-            pd.Series(["a", "a"]),
-            # CategoricalInput(**VALID_FIXED_CATEGORICAL_INPUT_FEATURE_SPEC),
-            # pd.Series(["c1", "c1"]),
-            False,
-        ),
     ],
 )
 def test_categorical_input_feature_validate_valid(input_feature, values, strict):
     input_feature.validate_experimental(values, strict)
 
 
 @pytest.mark.parametrize(
@@ -495,14 +494,34 @@
             specs.features.valid(CategoricalInput).obj(
                 categories=["a", "b", "c"],
                 allowed=[True, False, False],
             ),
             pd.Series(["a", "b"]),
             True,
         ),
+        (
+            specs.features.valid(CategoricalInput).obj(
+                categories=["1", "2", "3"],
+                allowed=[True, False, False],
+            ),
+            pd.Series([1, 2]),
+            # CategoricalInput(**VALID_FIXED_CATEGORICAL_INPUT_FEATURE_SPEC),
+            # pd.Series([random.choice(["c1", "c2", "c3"]) for _ in range(20)]),
+            True,
+        ),
+        (
+            specs.features.valid(CategoricalInput).obj(
+                categories=["one", "two", "three"],
+                allowed=[True, False, False],
+            ),
+            pd.Series([1, 2, 3]),
+            # CategoricalInput(**VALID_FIXED_CATEGORICAL_INPUT_FEATURE_SPEC),
+            # pd.Series([random.choice(["c1", "c2", "c3"]) for _ in range(20)]),
+            True,
+        ),
     ],
 )
 def test_categorical_input_feature_validate_invalid(input_feature, values, strict):
     with pytest.raises(ValueError):
         input_feature.validate_experimental(values, strict)
 
 
@@ -544,33 +563,35 @@
     ],
 )
 def test_categorical_input_feature_validate_candidental_invalid(input_feature, values):
     with pytest.raises(ValueError):
         input_feature.validate_candidental(values)
 
 
-def test_categorical_to_one_hot_encoding():
-    c = CategoricalInput(key="c", categories=["B", "A", "C"])
+@pytest.mark.parametrize("key", ["c", "c_alpha"])
+def test_categorical_to_one_hot_encoding(key):
+    c = CategoricalInput(key=key, categories=["B", "A", "C"])
     samples = pd.Series(["A", "A", "C", "B"])
     t_samples = c.to_onehot_encoding(samples)
     assert_frame_equal(
         t_samples,
         pd.DataFrame(
             data=[[0.0, 1.0, 0.0], [0.0, 1.0, 0.0], [0.0, 0.0, 1.0], [1.0, 0.0, 0.0]],
-            columns=["c_B", "c_A", "c_C"],
+            columns=[f"{key}_B", f"{key}_A", f"{key}_C"],
         ),
     )
     untransformed = c.from_onehot_encoding(t_samples)
     assert np.all(samples == untransformed)
 
 
-def test_categorical_from_one_hot_encoding():
-    c = CategoricalInput(key="c", categories=["B", "A", "C"])
+@pytest.mark.parametrize("key", ["c", "c_alpha"])
+def test_categorical_from_one_hot_encoding(key):
+    c = CategoricalInput(key=key, categories=["B", "A", "C"])
     one_hot_values = pd.DataFrame(
-        columns=["c_B", "c_A", "c_C", "misc"],
+        columns=[f"{key}_B", f"{key}_A", f"{key}_C", "misc"],
         data=[[0.9, 0.4, 0.2, 6], [0.8, 0.7, 0.9, 9]],
     )
     samples = c.from_onehot_encoding(one_hot_values)
     assert np.all(samples == pd.Series(["B", "C"]))
 
 
 def test_categorical_from_one_hot_encoding_invalid():
@@ -586,33 +607,35 @@
             [0.8, 0.7, 0.9],
         ],
     )
     with pytest.raises(ValueError):
         c.from_onehot_encoding(one_hot_values)
 
 
-def test_categorical_to_dummy_encoding():
-    c = CategoricalInput(key="c", categories=["B", "A", "C"])
+@pytest.mark.parametrize("key", ["c", "c_alpha"])
+def test_categorical_to_dummy_encoding(key):
+    c = CategoricalInput(key=key, categories=["B", "A", "C"])
     samples = pd.Series(["A", "A", "C", "B"])
     t_samples = c.to_dummy_encoding(samples)
     assert_frame_equal(
         t_samples,
         pd.DataFrame(
             data=[[1.0, 0.0], [1.0, 0.0], [0.0, 1.0], [0.0, 0.0]],
-            columns=["c_A", "c_C"],
+            columns=[f"{key}_A", f"{key}_C"],
         ),
     )
     untransformed = c.from_dummy_encoding(t_samples)
     assert np.all(samples == untransformed)
 
 
-def test_categorical_from_dummy_encoding():
-    c = CategoricalInput(key="c", categories=["B", "A", "C"])
+@pytest.mark.parametrize("key", ["c", "c_alpha"])
+def test_categorical_from_dummy_encoding(key):
+    c = CategoricalInput(key=key, categories=["B", "A", "C"])
     one_hot_values = pd.DataFrame(
-        columns=["c_A", "c_C", "misc"],
+        columns=[f"{key}_A", f"{key}_C", "misc"],
         data=[[0.9, 0.05, 6], [0.1, 0.1, 9]],
     )
     samples = c.from_dummy_encoding(one_hot_values)
     assert np.all(samples == pd.Series(["A", "B"]))
 
 
 def test_categorical_to_label_encoding():
@@ -852,14 +875,24 @@
                     [3, 7],
                     [3, 1],
                 ],
             ),
             pd.Series(["c2", "c3"]),
             False,
         ),
+        (
+            specs.features.valid(CategoricalDescriptorInput).obj(
+                categories=["1", "2", "3"],
+                allowed=[True, False, False],
+            ),
+            pd.Series([random.choice([1, 2, 3]) for _ in range(20)]),
+            # CategoricalInput(**VALID_FIXED_CATEGORICAL_INPUT_FEATURE_SPEC),
+            # pd.Series([random.choice(["c1", "c2", "c3"]) for _ in range(20)]),
+            False,
+        ),
     ],
 )
 def test_categorical_descriptor_input_feature_validate_valid(
     input_feature, values, strict
 ):
     input_feature.validate_experimental(values, strict)
 
@@ -901,14 +934,24 @@
                     [3, 7],
                     [3, 1],
                 ],
             ),
             pd.Series(["c2", "c3"]),
             True,
         ),
+        (
+            specs.features.valid(CategoricalInput).obj(
+                categories=["1", "2", "3"],
+                allowed=[True, False, False],
+            ),
+            pd.Series([1, 2]),
+            # CategoricalInput(**VALID_FIXED_CATEGORICAL_INPUT_FEATURE_SPEC),
+            # pd.Series([random.choice(["c1", "c2", "c3"]) for _ in range(20)]),
+            True,
+        ),
     ],
 )
 def test_categorical_descriptor_input_feature_validate_invalid(
     input_feature, values, strict
 ):
     with pytest.raises(ValueError):
         input_feature.validate_experimental(values, strict)
@@ -1073,15 +1116,15 @@
         ),
     ],
 )
 def test_categorical_descriptor_input_feature_from_dataframe(
     categories, descriptors, values
 ):
     df = pd.DataFrame.from_dict(
-        {category: v for category, v in zip(categories, values)},
+        dict(zip(categories, values)),
         orient="index",
         columns=descriptors,
     )
     f = CategoricalDescriptorInput.from_df("k", df)
     assert f.categories == categories
     assert f.descriptors == descriptors
     assert f.values == values
@@ -1111,15 +1154,15 @@
         (
             [out, cont],
             [cont, out],
         ),
     ],
 )
 def test_feature_sorting(unsorted_list, sorted_list):
-    assert list(sorted(unsorted_list)) == sorted_list
+    assert sorted(unsorted_list) == sorted_list
 
 
 # test features container
 if1 = specs.features.valid(ContinuousInput).obj(key="if1")
 if2 = specs.features.valid(ContinuousInput).obj(key="if2")
 if3 = specs.features.valid(ContinuousInput).obj(key="if3", bounds=(3, 3))
 if4 = specs.features.valid(CategoricalInput).obj(
@@ -1306,14 +1349,18 @@
 @pytest.mark.parametrize(
     "specs",
     [
         ({"x4": CategoricalEncodingEnum.ONE_HOT}),
         ({"x1": CategoricalEncodingEnum.ONE_HOT}),
         ({"x2": ScalerEnum.NORMALIZE}),
         ({"x2": CategoricalEncodingEnum.DESCRIPTOR}),
+        ({"x1": Fingerprints()}),
+        ({"x2": Fragments()}),
+        ({"x3": FingerprintsFragments()}),
+        ({"x3": MordredDescriptors(descriptors=["NssCH2", "ATSC2d"])}),
     ],
 )
 def test_inputs_validate_transform_specs_invalid(specs):
     inps = Inputs(
         features=[
             ContinuousInput(key="x1", bounds=(0, 1)),
             CategoricalInput(key="x2", categories=["apple", "banana"]),
@@ -1356,81 +1403,177 @@
             ),
         ]
     )
     inps._validate_transform_specs(specs)
 
 
 @pytest.mark.parametrize(
+    "specs",
+    [
+        ({"x2": CategoricalEncodingEnum.ONE_HOT}),
+        ({"x3": CategoricalEncodingEnum.DESCRIPTOR}),
+        ({"x4": CategoricalEncodingEnum.ONE_HOT}),
+        ({"x4": ScalerEnum.NORMALIZE}),
+        ({"x4": CategoricalEncodingEnum.DESCRIPTOR}),
+        (
+            {
+                "x2": CategoricalEncodingEnum.ONE_HOT,
+                "x3": CategoricalEncodingEnum.DESCRIPTOR,
+            }
+        ),
+    ],
+)
+# Invalid when no specs do not contain transform information for x4, or when the transform is not a MolFeatures type
+def test_inputs_validate_transform_specs_molecular_input_invalid(specs):
+    inps = Inputs(
+        features=[
+            ContinuousInput(key="x1", bounds=(0, 1)),
+            CategoricalInput(key="x2", categories=["apple", "banana"]),
+            CategoricalDescriptorInput(
+                key="x3",
+                categories=["apple", "banana"],
+                descriptors=["d1", "d2"],
+                values=[[1, 2], [3, 4]],
+            ),
+            MolecularInput(key="x4"),
+        ]
+    )
+    with pytest.raises(ValueError):
+        inps._validate_transform_specs(specs)
+
+
+@pytest.mark.skipif(not RDKIT_AVAILABLE, reason="requires rdkit")
+@pytest.mark.parametrize(
+    "specs",
+    [
+        ({"x4": Fingerprints()}),
+        ({"x4": Fragments()}),
+        ({"x4": FingerprintsFragments()}),
+        ({"x4": MordredDescriptors(descriptors=["NssCH2", "ATSC2d"])}),
+        (
+            {
+                "x2": CategoricalEncodingEnum.ONE_HOT,
+                "x4": Fingerprints(),
+            }
+        ),
+        (
+            {
+                "x3": CategoricalEncodingEnum.DESCRIPTOR,
+                "x4": Fingerprints(),
+            }
+        ),
+        (
+            {
+                "x2": CategoricalEncodingEnum.ONE_HOT,
+                "x3": CategoricalEncodingEnum.DESCRIPTOR,
+                "x4": Fingerprints(),
+            }
+        ),
+    ],
+)
+def test_inputs_validate_transform_specs_molecular_input_valid(specs):
+    inps = Inputs(
+        features=[
+            ContinuousInput(key="x1", bounds=(0, 1)),
+            CategoricalInput(key="x2", categories=["apple", "banana"]),
+            CategoricalDescriptorInput(
+                key="x3",
+                categories=["apple", "banana"],
+                descriptors=["d1", "d2"],
+                values=[[1, 2], [3, 4]],
+            ),
+            MolecularInput(key="x4"),
+        ]
+    )
+    inps._validate_transform_specs(specs)
+
+
+@pytest.mark.skipif(not RDKIT_AVAILABLE, reason="requires rdkit")
+@pytest.mark.parametrize(
     "specs, expected_features2idx, expected_features2names",
     [
         (
-            {"x2": CategoricalEncodingEnum.ONE_HOT},
-            {"x1": (0,), "x2": (2, 3, 4), "x3": (1,)},
+            {"x2": CategoricalEncodingEnum.ONE_HOT, "x4": Fingerprints(n_bits=2048)},
+            {
+                "x1": (2048,),
+                "x2": (2050, 2051, 2052),
+                "x3": (2049,),
+                "x4": tuple(range(2048)),
+            },
             {
                 "x1": ("x1",),
                 "x2": ("x2_apple", "x2_banana", "x2_orange"),
                 "x3": ("x3",),
+                "x4": tuple(f"x4_fingerprint_{i}" for i in range(2048)),
             },
         ),
         (
-            {"x2": CategoricalEncodingEnum.DUMMY},
-            {"x1": (0,), "x2": (2, 3), "x3": (1,)},
-            {"x1": ("x1",), "x2": ("x2_banana", "x2_orange"), "x3": ("x3",)},
-        ),
-        (
-            {"x2": CategoricalEncodingEnum.ORDINAL},
-            {"x1": (0,), "x2": (2,), "x3": (1,)},
-            {"x1": ("x1",), "x2": ("x2",), "x3": ("x3",)},
-        ),
-        (
-            {"x3": CategoricalEncodingEnum.ONE_HOT},
-            {"x1": (0,), "x2": (5,), "x3": (1, 2, 3, 4)},
+            {
+                "x2": CategoricalEncodingEnum.DUMMY,
+                "x4": Fragments(fragments=["fr_unbrch_alkane", "fr_thiocyan"]),
+            },
+            {"x1": (2,), "x2": (4, 5), "x3": (3,), "x4": (0, 1)},
             {
                 "x1": ("x1",),
-                "x2": ("x2",),
-                "x3": ("x3_apple", "x3_banana", "x3_orange", "x3_cherry"),
+                "x2": ("x2_banana", "x2_orange"),
+                "x3": ("x3",),
+                "x4": ("x4_fr_unbrch_alkane", "x4_fr_thiocyan"),
             },
         ),
         (
-            {"x3": CategoricalEncodingEnum.DESCRIPTOR},
-            {"x1": (0,), "x2": (3,), "x3": (1, 2)},
+            {
+                "x2": CategoricalEncodingEnum.ORDINAL,
+                "x4": FingerprintsFragments(
+                    n_bits=2048, fragments=["fr_unbrch_alkane", "fr_thiocyan"]
+                ),
+            },
+            {
+                "x1": (2050,),
+                "x2": (2052,),
+                "x3": (2051,),
+                "x4": tuple(range(2048 + 2)),
+            },
             {
                 "x1": ("x1",),
                 "x2": ("x2",),
-                "x3": (
-                    "x3_d1",
-                    "x3_d2",
+                "x3": ("x3",),
+                "x4": tuple(
+                    [f"x4_fingerprint_{i}" for i in range(2048)]
+                    + ["x4_fr_unbrch_alkane", "x4_fr_thiocyan"]
                 ),
             },
         ),
         (
             {
-                "x2": CategoricalEncodingEnum.ONE_HOT,
-                "x3": CategoricalEncodingEnum.DESCRIPTOR,
+                "x3": CategoricalEncodingEnum.ONE_HOT,
+                "x4": MordredDescriptors(descriptors=["NssCH2", "ATSC2d"]),
             },
-            {"x1": (0,), "x2": (3, 4, 5), "x3": (1, 2)},
+            {"x1": (2,), "x2": (7,), "x3": (3, 4, 5, 6), "x4": (0, 1)},
             {
                 "x1": ("x1",),
-                "x2": ("x2_apple", "x2_banana", "x2_orange"),
-                "x3": (
-                    "x3_d1",
-                    "x3_d2",
-                ),
+                "x2": ("x2",),
+                "x3": ("x3_apple", "x3_banana", "x3_orange", "x3_cherry"),
+                "x4": ("x4_NssCH2", "x4_ATSC2d"),
             },
         ),
         (
             {
                 "x2": CategoricalEncodingEnum.ONE_HOT,
-                "x3": CategoricalEncodingEnum.ONE_HOT,
+                "x3": CategoricalEncodingEnum.DESCRIPTOR,
+                "x4": MordredDescriptors(descriptors=["NssCH2", "ATSC2d"]),
             },
-            {"x1": (0,), "x2": (5, 6, 7), "x3": (1, 2, 3, 4)},
+            {"x1": (2,), "x2": (5, 6, 7), "x3": (3, 4), "x4": (0, 1)},
             {
                 "x1": ("x1",),
                 "x2": ("x2_apple", "x2_banana", "x2_orange"),
-                "x3": ("x3_apple", "x3_banana", "x3_orange", "x3_cherry"),
+                "x3": (
+                    "x3_d1",
+                    "x3_d2",
+                ),
+                "x4": ("x4_NssCH2", "x4_ATSC2d"),
             },
         ),
     ],
 )
 def test_inputs_get_transform_info(
     specs, expected_features2idx, expected_features2names
 ):
@@ -1440,14 +1583,15 @@
             CategoricalInput(key="x2", categories=["apple", "banana", "orange"]),
             CategoricalDescriptorInput(
                 key="x3",
                 categories=["apple", "banana", "orange", "cherry"],
                 descriptors=["d1", "d2"],
                 values=[[1, 2], [3, 4], [5, 6], [7, 8]],
             ),
+            MolecularInput(key="x4"),
         ]
     )
     features2idx, features2names = inps._get_transform_info(specs)
     assert features2idx == expected_features2idx
     assert features2names == expected_features2names
 
 
@@ -1495,14 +1639,171 @@
     samples = inps.sample(n=100)
     samples = samples.sample(40)
     transformed = inps.transform(experiments=samples, specs=specs)
     untransformed = inps.inverse_transform(experiments=transformed, specs=specs)
     assert_frame_equal(samples, untransformed)
 
 
+@pytest.mark.skipif(not RDKIT_AVAILABLE, reason="requires rdkit")
+@pytest.mark.parametrize(
+    "specs, expected",
+    [
+        (
+            {"x2": CategoricalEncodingEnum.ONE_HOT, "x4": Fingerprints(n_bits=32)},
+            {
+                "x4_fingerprint_0": {0: 1.0, 1: 1.0, 2: 0.0, 3: 0.0},
+                "x4_fingerprint_1": {0: 1.0, 1: 0.0, 2: 1.0, 3: 1.0},
+                "x4_fingerprint_2": {0: 1.0, 1: 0.0, 2: 1.0, 3: 0.0},
+                "x4_fingerprint_3": {0: 1.0, 1: 0.0, 2: 0.0, 3: 1.0},
+                "x4_fingerprint_4": {0: 1.0, 1: 0.0, 2: 0.0, 3: 0.0},
+                "x4_fingerprint_5": {0: 1.0, 1: 1.0, 2: 0.0, 3: 1.0},
+                "x4_fingerprint_6": {0: 0.0, 1: 0.0, 2: 1.0, 3: 0.0},
+                "x4_fingerprint_7": {0: 1.0, 1: 0.0, 2: 1.0, 3: 1.0},
+                "x4_fingerprint_8": {0: 1.0, 1: 0.0, 2: 0.0, 3: 1.0},
+                "x4_fingerprint_9": {0: 1.0, 1: 0.0, 2: 0.0, 3: 0.0},
+                "x4_fingerprint_10": {0: 1.0, 1: 0.0, 2: 0.0, 3: 1.0},
+                "x4_fingerprint_11": {0: 1.0, 1: 0.0, 2: 0.0, 3: 0.0},
+                "x4_fingerprint_12": {0: 0.0, 1: 0.0, 2: 0.0, 3: 0.0},
+                "x4_fingerprint_13": {0: 1.0, 1: 0.0, 2: 0.0, 3: 1.0},
+                "x4_fingerprint_14": {0: 0.0, 1: 0.0, 2: 0.0, 3: 0.0},
+                "x4_fingerprint_15": {0: 1.0, 1: 0.0, 2: 0.0, 3: 0.0},
+                "x4_fingerprint_16": {0: 1.0, 1: 1.0, 2: 1.0, 3: 0.0},
+                "x4_fingerprint_17": {0: 1.0, 1: 1.0, 2: 0.0, 3: 0.0},
+                "x4_fingerprint_18": {0: 1.0, 1: 0.0, 2: 0.0, 3: 1.0},
+                "x4_fingerprint_19": {0: 0.0, 1: 0.0, 2: 0.0, 3: 1.0},
+                "x4_fingerprint_20": {0: 0.0, 1: 0.0, 2: 0.0, 3: 0.0},
+                "x4_fingerprint_21": {0: 0.0, 1: 0.0, 2: 0.0, 3: 0.0},
+                "x4_fingerprint_22": {0: 1.0, 1: 0.0, 2: 0.0, 3: 0.0},
+                "x4_fingerprint_23": {0: 1.0, 1: 0.0, 2: 0.0, 3: 1.0},
+                "x4_fingerprint_24": {0: 0.0, 1: 0.0, 2: 0.0, 3: 0.0},
+                "x4_fingerprint_25": {0: 1.0, 1: 0.0, 2: 0.0, 3: 1.0},
+                "x4_fingerprint_26": {0: 0.0, 1: 0.0, 2: 0.0, 3: 0.0},
+                "x4_fingerprint_27": {0: 1.0, 1: 0.0, 2: 0.0, 3: 0.0},
+                "x4_fingerprint_28": {0: 1.0, 1: 0.0, 2: 0.0, 3: 0.0},
+                "x4_fingerprint_29": {0: 1.0, 1: 0.0, 2: 0.0, 3: 1.0},
+                "x4_fingerprint_30": {0: 0.0, 1: 0.0, 2: 1.0, 3: 0.0},
+                "x4_fingerprint_31": {0: 0.0, 1: 0.0, 2: 0.0, 3: 0.0},
+                "x1": {0: 0.1, 1: 0.3, 2: 0.5, 3: 1.0},
+                "x3": {0: "banana", 1: "orange", 2: "apple", 3: "cherry"},
+                "x2_apple": {0: 1.0, 1: 0.0, 2: 1.0, 3: 0.0},
+                "x2_banana": {0: 0.0, 1: 1.0, 2: 0.0, 3: 0.0},
+                "x2_orange": {0: 0.0, 1: 0.0, 2: 0.0, 3: 1.0},
+            },
+        ),
+        (
+            {
+                "x2": CategoricalEncodingEnum.DUMMY,
+                "x4": Fragments(fragments=["fr_unbrch_alkane", "fr_thiocyan"]),
+            },
+            {
+                "x4_fr_unbrch_alkane": {0: 0.0, 1: 0.0, 2: 0.0, 3: 0.0},
+                "x4_fr_thiocyan": {0: 0.0, 1: 0.0, 2: 0.0, 3: 0.0},
+                "x1": {0: 0.1, 1: 0.3, 2: 0.5, 3: 1.0},
+                "x3": {0: "banana", 1: "orange", 2: "apple", 3: "cherry"},
+                "x2_banana": {0: 0.0, 1: 1.0, 2: 0.0, 3: 0.0},
+                "x2_orange": {0: 0.0, 1: 0.0, 2: 0.0, 3: 1.0},
+            },
+        ),
+        (
+            {
+                "x2": CategoricalEncodingEnum.ORDINAL,
+                "x4": FingerprintsFragments(
+                    n_bits=32, fragments=["fr_unbrch_alkane", "fr_thiocyan"]
+                ),
+            },
+            {
+                "x4_fingerprint_0": {0: 1.0, 1: 1.0, 2: 0.0, 3: 0.0},
+                "x4_fingerprint_1": {0: 1.0, 1: 0.0, 2: 1.0, 3: 1.0},
+                "x4_fingerprint_2": {0: 1.0, 1: 0.0, 2: 1.0, 3: 0.0},
+                "x4_fingerprint_3": {0: 1.0, 1: 0.0, 2: 0.0, 3: 1.0},
+                "x4_fingerprint_4": {0: 1.0, 1: 0.0, 2: 0.0, 3: 0.0},
+                "x4_fingerprint_5": {0: 1.0, 1: 1.0, 2: 0.0, 3: 1.0},
+                "x4_fingerprint_6": {0: 0.0, 1: 0.0, 2: 1.0, 3: 0.0},
+                "x4_fingerprint_7": {0: 1.0, 1: 0.0, 2: 1.0, 3: 1.0},
+                "x4_fingerprint_8": {0: 1.0, 1: 0.0, 2: 0.0, 3: 1.0},
+                "x4_fingerprint_9": {0: 1.0, 1: 0.0, 2: 0.0, 3: 0.0},
+                "x4_fingerprint_10": {0: 1.0, 1: 0.0, 2: 0.0, 3: 1.0},
+                "x4_fingerprint_11": {0: 1.0, 1: 0.0, 2: 0.0, 3: 0.0},
+                "x4_fingerprint_12": {0: 0.0, 1: 0.0, 2: 0.0, 3: 0.0},
+                "x4_fingerprint_13": {0: 1.0, 1: 0.0, 2: 0.0, 3: 1.0},
+                "x4_fingerprint_14": {0: 0.0, 1: 0.0, 2: 0.0, 3: 0.0},
+                "x4_fingerprint_15": {0: 1.0, 1: 0.0, 2: 0.0, 3: 0.0},
+                "x4_fingerprint_16": {0: 1.0, 1: 1.0, 2: 1.0, 3: 0.0},
+                "x4_fingerprint_17": {0: 1.0, 1: 1.0, 2: 0.0, 3: 0.0},
+                "x4_fingerprint_18": {0: 1.0, 1: 0.0, 2: 0.0, 3: 1.0},
+                "x4_fingerprint_19": {0: 0.0, 1: 0.0, 2: 0.0, 3: 1.0},
+                "x4_fingerprint_20": {0: 0.0, 1: 0.0, 2: 0.0, 3: 0.0},
+                "x4_fingerprint_21": {0: 0.0, 1: 0.0, 2: 0.0, 3: 0.0},
+                "x4_fingerprint_22": {0: 1.0, 1: 0.0, 2: 0.0, 3: 0.0},
+                "x4_fingerprint_23": {0: 1.0, 1: 0.0, 2: 0.0, 3: 1.0},
+                "x4_fingerprint_24": {0: 0.0, 1: 0.0, 2: 0.0, 3: 0.0},
+                "x4_fingerprint_25": {0: 1.0, 1: 0.0, 2: 0.0, 3: 1.0},
+                "x4_fingerprint_26": {0: 0.0, 1: 0.0, 2: 0.0, 3: 0.0},
+                "x4_fingerprint_27": {0: 1.0, 1: 0.0, 2: 0.0, 3: 0.0},
+                "x4_fingerprint_28": {0: 1.0, 1: 0.0, 2: 0.0, 3: 0.0},
+                "x4_fingerprint_29": {0: 1.0, 1: 0.0, 2: 0.0, 3: 1.0},
+                "x4_fingerprint_30": {0: 0.0, 1: 0.0, 2: 1.0, 3: 0.0},
+                "x4_fingerprint_31": {0: 0.0, 1: 0.0, 2: 0.0, 3: 0.0},
+                "x4_fr_unbrch_alkane": {0: 0.0, 1: 0.0, 2: 0.0, 3: 0.0},
+                "x4_fr_thiocyan": {0: 0.0, 1: 0.0, 2: 0.0, 3: 0.0},
+                "x1": {0: 0.1, 1: 0.3, 2: 0.5, 3: 1.0},
+                "x3": {0: "banana", 1: "orange", 2: "apple", 3: "cherry"},
+                "x2": {0: 0, 1: 1, 2: 0, 3: 2},
+            },
+        ),
+        (
+            {
+                "x2": CategoricalEncodingEnum.ONE_HOT,
+                "x3": CategoricalEncodingEnum.DESCRIPTOR,
+                "x4": MordredDescriptors(descriptors=["NssCH2", "ATSC2d"]),
+            },
+            {
+                "x4_NssCH2": {
+                    0: 0.5963718820861676,
+                    1: -1.5,
+                    2: -0.28395061728395066,
+                    3: -8.34319526627219,
+                },
+                "x4_ATSC2d": {0: 0.0, 1: 0.0, 2: 1.0, 3: 0.0},
+                "x1": {0: 0.1, 1: 0.3, 2: 0.5, 3: 1.0},
+                "x3_d1": {0: 3.0, 1: 5.0, 2: 1.0, 3: 7.0},
+                "x3_d2": {0: 4.0, 1: 6.0, 2: 2.0, 3: 8.0},
+                "x2_apple": {0: 1.0, 1: 0.0, 2: 1.0, 3: 0.0},
+                "x2_banana": {0: 0.0, 1: 1.0, 2: 0.0, 3: 0.0},
+                "x2_orange": {0: 0.0, 1: 0.0, 2: 0.0, 3: 1.0},
+            },
+        ),
+    ],
+)
+def test_inputs_transform_molecular(specs, expected):
+    experiments = [
+        [0.1, "apple", "banana", "CC(=O)Oc1ccccc1C(=O)O", 88.0],
+        [0.3, "banana", "orange", "c1ccccc1", 35.0],
+        [0.5, "apple", "apple", "[CH3][CH2][OH]", 69.0],
+        [1.0, "orange", "cherry", "N[C@](C)(F)C(=O)O", 20.0],
+    ]
+    experiments = pd.DataFrame(experiments, columns=["x1", "x2", "x3", "x4", "y"])
+    experiments["valid_y"] = 1
+    inps = Inputs(
+        features=[
+            ContinuousInput(key="x1", bounds=(0, 1)),
+            CategoricalInput(key="x2", categories=["apple", "banana", "orange"]),
+            CategoricalDescriptorInput(
+                key="x3",
+                categories=["apple", "banana", "orange", "cherry"],
+                descriptors=["d1", "d2"],
+                values=[[1, 2], [3, 4], [5, 6], [7, 8]],
+            ),
+            MolecularInput(key="x4"),
+        ]
+    )
+    transformed = inps.transform(experiments=experiments, specs=specs)
+    assert_frame_equal(transformed, pd.DataFrame.from_dict(expected))
+
+
 if1 = specs.features.valid(ContinuousInput).obj(key="if1")
 if2 = specs.features.valid(ContinuousInput).obj(key="if2", bounds=(3, 3))
 if3 = specs.features.valid(CategoricalInput).obj(
     key="if3",
     categories=["c1", "c2", "c3"],
     allowed=[True, True, True],
 )
```

### Comparing `bofire-0.0.4/tests/bofire/data_models/test_filters.py` & `bofire-0.0.5/tests/bofire/data_models/test_filters.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/tests/bofire/data_models/test_kernels.py` & `bofire-0.0.5/tests/bofire/data_models/test_kernels.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,22 +2,25 @@
 
 import gpytorch
 import gpytorch.kernels
 import pytest
 import torch
 from pydantic import parse_obj_as
 
+import bofire
+import bofire.kernels.api as kernels
 from bofire.data_models.kernels.api import (
     AdditiveKernel,
     AnyKernel,
     LinearKernel,
     MaternKernel,
     MultiplicativeKernel,
     RBFKernel,
     ScaleKernel,
+    TanimotoKernel,
 )
 from bofire.data_models.priors.api import BOTORCH_SCALE_PRIOR, GammaPrior
 
 
 def get_invalids(valid: dict) -> List[dict]:
     return [
         {k: v for k, v in valid.items() if k != k_}
@@ -29,14 +32,15 @@
 EQUIVALENTS = {
     RBFKernel: gpytorch.kernels.RBFKernel,
     MaternKernel: gpytorch.kernels.MaternKernel,
     LinearKernel: gpytorch.kernels.LinearKernel,
     ScaleKernel: gpytorch.kernels.ScaleKernel,
     AdditiveKernel: gpytorch.kernels.AdditiveKernel,
     MultiplicativeKernel: gpytorch.kernels.ProductKernel,
+    TanimotoKernel: bofire.kernels.fingerprint_kernels.tanimoto_kernel.TanimotoKernel,
 }
 
 VALID_RBF_SPEC = {
     "type": "RBFKernel",
     "ard": True,
 }
 VALID_MATERN_SPEC = {
@@ -51,14 +55,19 @@
 VALID_ADDITIVE_SPEC = {"type": "AdditiveKernel", "kernels": [RBFKernel(), RBFKernel()]}
 
 VALID_MULTIPLICATIVE_SPEC = {
     "type": "MultiplicativeKernel",
     "kernels": [RBFKernel(), RBFKernel()],
 }
 
+VALID_TANIMOTO_SPEC = {
+    "type": "TanimotoKernel",
+    "ard": True,
+}
+
 KERNEL_SPECS = {
     RBFKernel: {
         "valids": [
             VALID_RBF_SPEC,
         ],
         "invalids": [
             *get_invalids(VALID_RBF_SPEC),
@@ -75,57 +84,73 @@
     LinearKernel: {
         "valids": [
             VALID_LINEAR_SPEC,
         ],
         "invalids": [
             *get_invalids(VALID_LINEAR_SPEC),
         ],
-        ScaleKernel: {
-            "valids": [VALID_SCALE_SPEC],
-            "invalids": [
-                *get_invalids(VALID_SCALE_SPEC),
-            ],
-        },
-        MultiplicativeKernel: {
-            "valids": [VALID_MULTIPLICATIVE_SPEC],
-            "invalids": [
-                *get_invalids(VALID_SCALE_SPEC),
-            ],
-        },
+    },
+    ScaleKernel: {
+        "valids": [VALID_SCALE_SPEC],
+        "invalids": [
+            *get_invalids(VALID_SCALE_SPEC),
+        ],
+    },
+    MultiplicativeKernel: {
+        "valids": [VALID_MULTIPLICATIVE_SPEC],
+        "invalids": [
+            *get_invalids(VALID_SCALE_SPEC),
+        ],
+    },
+    AdditiveKernel: {
+        "valids": [VALID_ADDITIVE_SPEC],
+        "invalids": [
+            *get_invalids(VALID_SCALE_SPEC),
+        ],
+    },
+    TanimotoKernel: {
+        "valids": [VALID_TANIMOTO_SPEC],
+        "invalids": [
+            *get_invalids(VALID_TANIMOTO_SPEC),
+        ],
     },
 }
 
 
 @pytest.mark.parametrize(
     "cls, spec",
     [(cls, valid) for cls, data in KERNEL_SPECS.items() for valid in data["valids"]],
 )
 def test_valid_kernel_specs(cls, spec):
     res = cls(**spec)
     assert isinstance(res, cls)
     assert isinstance(res.__str__(), str)
-    gkernel = res.to_gpytorch(
-        batch_shape=torch.Size(), ard_num_dims=10, active_dims=list(range(5))
+    gkernel = kernels.map(
+        res, batch_shape=torch.Size(), ard_num_dims=10, active_dims=list(range(5))
     )
     assert isinstance(gkernel, EQUIVALENTS[cls])
     res2 = parse_obj_as(AnyKernel, res.dict())
     assert res == res2
 
 
 def test_scale_kernel():
-    kernel = ScaleKernel(base_kernel=RBFKernel(), outputscale_prior=BOTORCH_SCALE_PRIOR)
-    k = kernel.to_gpytorch(
+    kernel = ScaleKernel(
+        base_kernel=RBFKernel(), outputscale_prior=BOTORCH_SCALE_PRIOR()
+    )
+    k = kernels.map(
+        kernel,
         batch_shape=torch.Size(),
         ard_num_dims=10,
         active_dims=list(range(5)),
     )
     assert hasattr(k, "outputscale_prior")
     assert isinstance(k.outputscale_prior, gpytorch.priors.GammaPrior)
     kernel = ScaleKernel(base_kernel=RBFKernel())
-    k = kernel.to_gpytorch(
+    k = kernels.map(
+        kernel,
         batch_shape=torch.Size(),
         ard_num_dims=10,
         active_dims=list(range(5)),
     )
     assert hasattr(k, "outputscale_prior") is False
 
 
@@ -169,16 +194,19 @@
             list(range(5)),
             gpytorch.kernels.MaternKernel,
         ),
         (LinearKernel(), 10, list(range(5)), gpytorch.kernels.LinearKernel),
     ],
 )
 def test_continuous_kernel(kernel, ard_num_dims, active_dims, expected_kernel):
-    k = kernel.to_gpytorch(
-        batch_shape=torch.Size(), ard_num_dims=ard_num_dims, active_dims=active_dims
+    k = kernels.map(
+        kernel,
+        batch_shape=torch.Size(),
+        ard_num_dims=ard_num_dims,
+        active_dims=active_dims,
     )
     assert isinstance(k, expected_kernel)
     if isinstance(kernel, LinearKernel):
         return
     if kernel.lengthscale_prior is not None:
         assert hasattr(k, "lengthscale_prior")
         assert isinstance(k.lengthscale_prior, gpytorch.priors.GammaPrior)
@@ -189,7 +217,40 @@
         assert k.ard_num_dims is None
     else:
         assert k.ard_num_dims == len(active_dims)
     assert torch.eq(k.active_dims, torch.tensor(active_dims, dtype=torch.int64)).all()
 
     if isinstance(kernel, gpytorch.kernels.MaternKernel):
         assert kernel.nu == k.nu
+
+
+@pytest.mark.parametrize(
+    "kernel, ard_num_dims, active_dims, expected_kernel",
+    [
+        (
+            TanimotoKernel(ard=False),
+            10,
+            list(range(5)),
+            bofire.kernels.fingerprint_kernels.tanimoto_kernel.TanimotoKernel,
+        ),
+        (
+            TanimotoKernel(ard=True),
+            10,
+            list(range(5)),
+            bofire.kernels.fingerprint_kernels.tanimoto_kernel.TanimotoKernel,
+        ),
+    ],
+)
+def test_molecular_kernel(kernel, ard_num_dims, active_dims, expected_kernel):
+    k = kernels.map(
+        kernel,
+        batch_shape=torch.Size(),
+        ard_num_dims=ard_num_dims,
+        active_dims=active_dims,
+    )
+    assert isinstance(k, expected_kernel)
+
+    if kernel.ard is False:
+        assert k.ard_num_dims is None
+    else:
+        assert k.ard_num_dims == len(active_dims)
+    assert torch.eq(k.active_dims, torch.tensor(active_dims, dtype=torch.int64)).all()
```

### Comparing `bofire-0.0.4/tests/bofire/data_models/test_nchoosek_combinatorics.py` & `bofire-0.0.5/tests/bofire/data_models/test_nchoosek_combinatorics.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/tests/bofire/data_models/test_numeric.py` & `bofire-0.0.5/tests/bofire/data_models/test_numeric.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/tests/bofire/data_models/test_samplers.py` & `bofire-0.0.5/tests/bofire/data_models/test_samplers.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/tests/bofire/data_models/test_unions.py` & `bofire-0.0.5/tests/bofire/data_models/test_unions.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/tests/bofire/data_models/test_util.py` & `bofire-0.0.5/tests/bofire/data_models/test_util.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/tests/bofire/strategies/doe/test_design.py` & `bofire-0.0.5/tests/bofire/strategies/doe/test_design.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 def test_raise_error_if_cyipopt_not_available():
     pytest.raises(ImportError)
 
 
 @pytest.mark.skipif(not CYIPOPT_AVAILABLE, reason="requires cyipopt")
 def test_find_local_max_ipopt_no_constraint():
     # Design for a problem with an n-choose-k constraint
-    domain = Domain(
+    domain = Domain.from_lists(
         inputs=[
             ContinuousInput(
                 key=f"x{i+1}",
                 bounds=(0, 1),
             )
             for i in range(4)
         ],
@@ -58,15 +58,15 @@
     inputs = [
         ContinuousInput(
             key=f"x{i+1}",
             bounds=(0, 1),
         )
         for i in range(4)
     ]
-    domain = Domain(
+    domain = Domain.from_lists(
         inputs=inputs,
         outputs=[ContinuousOutput(key="y")],
         constraints=[
             NChooseKConstraint(
                 features=[f"x{i+1}" for i in range(4)],
                 min_count=0,
                 max_count=3,
@@ -94,15 +94,15 @@
     inputs = [
         ContinuousInput(
             key=f"x{i+1}",
             bounds=(0, 1),
         )
         for i in range(4)
     ]
-    domain = Domain(
+    domain = Domain.from_lists(
         inputs=inputs,
         outputs=[ContinuousOutput(key="y")],
         constraints=[
             LinearEqualityConstraint(
                 features=[f"x{i+1}" for i in range(4)], coefficients=[1, 1, 1, 1], rhs=1
             )
         ],
@@ -127,15 +127,15 @@
             bounds=(0, 1),
         ),
         ContinuousInput(
             key=f"x{3}",
             bounds=(0, 1),
         ),
     ]
-    domain = Domain(
+    domain = Domain.from_lists(
         inputs=inputs,
         outputs=[ContinuousOutput(key="y")],
         constraints=[
             LinearEqualityConstraint(
                 features=[f"x{i+1}" for i in range(3)], coefficients=[1, 1, 1], rhs=1
             ),
             NChooseKConstraint(
@@ -147,31 +147,31 @@
         ],
     )
 
     # with pytest.warns(ValueError):
     A = find_local_max_ipopt(domain, "fully-quadratic", ipopt_options={"maxiter": 100})
     opt = np.eye(3)
     for row in A.to_numpy():
-        assert any([np.allclose(row, o, atol=1e-2) for o in opt])
+        assert any(np.allclose(row, o, atol=1e-2) for o in opt)
     for o in opt:
-        assert any([np.allclose(o, row, atol=1e-2) for row in A.to_numpy()])
+        assert any(np.allclose(o, row, atol=1e-2) for row in A.to_numpy())
 
 
 @pytest.mark.skipif(not CYIPOPT_AVAILABLE, reason="requires cyipopt")
 def test_find_local_max_ipopt_results():
     # define problem: no NChooseK constraints
     inputs = [
         ContinuousInput(
             key=f"x{1}",
             bounds=(0, 1),
         ),
         ContinuousInput(key=f"x{2}", bounds=(0.1, 1)),
         ContinuousInput(key=f"x{3}", bounds=(0, 0.6)),
     ]
-    domain = Domain(
+    domain = Domain.from_lists(
         inputs=inputs,
         outputs=[ContinuousOutput(key="y")],
         constraints=[
             LinearEqualityConstraint(
                 features=[f"x{i+1}" for i in range(3)], coefficients=[1, 1, 1], rhs=1
             ),
             LinearInequalityConstraint(
@@ -182,17 +182,17 @@
             ),
         ],
     )
     np.random.seed(1)
     A = find_local_max_ipopt(domain, "linear", n_experiments=12)
     opt = np.array([[0.2, 0.2, 0.6], [0.3, 0.6, 0.1], [0.7, 0.1, 0.2], [0.3, 0.1, 0.6]])
     for row in A.to_numpy():
-        assert any([np.allclose(row, o, atol=1e-2) for o in opt])
+        assert any(np.allclose(row, o, atol=1e-2) for o in opt)
     for o in opt[:-1]:
-        assert any([np.allclose(o, row, atol=1e-2) for row in A.to_numpy()])
+        assert any(np.allclose(o, row, atol=1e-2) for row in A.to_numpy())
 
 
 # def test_find_local_max_ipopt_sampling():
 #     # define problem
 #     problem = opti.Problem(
 #         inputs=[opti.Continuous(f"x{i}", [0, 1]) for i in range(3)],
 #         outputs=[opti.Continuous("y")],
@@ -215,15 +215,15 @@
         ContinuousInput(
             key=f"x{1}",
             bounds=(0, 1),
         ),
         ContinuousInput(key=f"x{2}", bounds=(0.1, 1)),
         ContinuousInput(key=f"x{3}", bounds=(0, 0.6)),
     ]
-    domain = Domain(
+    domain = Domain.from_lists(
         inputs=inputs,
         outputs=[ContinuousOutput(key="y")],
         constraints=[
             LinearEqualityConstraint(
                 features=[f"x{i+1}" for i in range(3)], coefficients=[1, 1, 1], rhs=1
             ),
             LinearInequalityConstraint(
@@ -280,15 +280,15 @@
             bounds=(0, 1),
         ),
         ContinuousInput(
             key=f"x{3}",
             bounds=(0, 1),
         ),
     ]
-    domain = Domain(
+    domain = Domain.from_lists(
         inputs=inputs,
         outputs=[ContinuousOutput(key="y")],
         constraints=[
             LinearEqualityConstraint(
                 features=[f"x{i+1}" for i in range(3)], coefficients=[1, 1, 1], rhs=1
             ),
             NChooseKConstraint(
@@ -306,17 +306,17 @@
         domain,
         "fully-quadratic",
         ipopt_options={"maxiter": 100},
         fixed_experiments=pd.DataFrame([[1, 0, 0], [0, 1, 0]], columns=["x1", "x2", "x3"]),  # type: ignore
     )
     opt = np.eye(3)
     for row in A.to_numpy():
-        assert any([np.allclose(row, o, atol=1e-2) for o in opt])
+        assert any(np.allclose(row, o, atol=1e-2) for o in opt)
     for o in opt:
-        assert any([np.allclose(o, row, atol=1e-2) for row in A.to_numpy()])
+        assert any(np.allclose(o, row, atol=1e-2) for row in A.to_numpy())
     assert np.allclose(A.to_numpy()[:2, :], opt[:2, :])
 
 
 @pytest.mark.skipif(not CYIPOPT_AVAILABLE, reason="requires cyipopt")
 def test_check_fixed_experiments():
     # define problem: everything fine
     inputs = [
@@ -329,15 +329,15 @@
             bounds=(0, 1),
         ),
         ContinuousInput(
             key=f"x{3}",
             bounds=(0, 1),
         ),
     ]
-    domain = Domain(
+    domain = Domain.from_lists(
         inputs=inputs,
         outputs=[ContinuousOutput(key="y")],
         constraints=[
             LinearEqualityConstraint(
                 features=[f"x{i+1}" for i in range(3)], coefficients=[1, 1, 1], rhs=1
             ),
             NChooseKConstraint(
@@ -429,15 +429,15 @@
 #     with warnings.catch_warnings():
 #         warnings.simplefilter("error")
 #         domain.validate_candidates(candidates=A, only_inputs=True)
 
 
 @pytest.mark.skipif(not CYIPOPT_AVAILABLE, reason="requires cyipopt")
 def test_find_local_max_ipopt_nonlinear_constraint():
-    domain = Domain(
+    domain = Domain.from_lists(
         inputs=[
             ContinuousInput(key="x1", bounds=(-1, 1)),
             ContinuousInput(key="x2", bounds=(-1, 1)),
             ContinuousInput(key="x3", bounds=(0, 1)),
         ],
         outputs=[ContinuousOutput(key="y")],
         constraints=[
@@ -451,15 +451,15 @@
 
     result = find_local_max_ipopt(domain, "linear", ipopt_options={"maxiter": 100})
 
     assert np.allclose(domain.constraints(result), 0, atol=1e-6)
 
 
 def test_get_n_experiments():
-    domain = Domain(
+    domain = Domain.from_lists(
         inputs=[
             ContinuousInput(key="x1", bounds=(-1, 1)),
             ContinuousInput(key="x2", bounds=(-1, 1)),
             ContinuousInput(key="x3", bounds=(0, 1)),
         ],
         outputs=[ContinuousOutput(key="y")],
     )
```

### Comparing `bofire-0.0.4/tests/bofire/strategies/doe/test_objective.py` & `bofire-0.0.5/tests/bofire/strategies/doe/test_objective.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     SpaceFilling,
 )
 from bofire.strategies.doe.utils import get_formula_from_string
 
 
 def test_Objective_model_jacobian_t():
     # "small" model
-    domain = Domain(
+    domain = Domain.from_lists(
         inputs=[
             ContinuousInput(
                 key=f"x{i+1}",
                 bounds=(0, 1),
             )
             for i in range(3)
         ],
@@ -77,15 +77,15 @@
         ],
     )
     B = B[model_terms].to_numpy()
 
     assert np.allclose(B, model_jacobian_t(x)[0])
 
     # fully cubic model
-    domain = Domain(
+    domain = Domain.from_lists(
         inputs=[
             ContinuousInput(
                 key=f"x{i+1}",
                 bounds=(0, 1),
             )
             for i in range(5)
         ],
@@ -362,15 +362,15 @@
 
     B = B[objective.model_terms].to_numpy()
 
     assert np.allclose(B, model_jacobian_t(x)[0])
 
 
 def test_Objective_convert_input_to_model_tensor():
-    domain = Domain(
+    domain = Domain.from_lists(
         inputs=[
             ContinuousInput(
                 key=f"x{i+1}",
                 bounds=(0, 1),
             )
             for i in range(3)
         ],
@@ -383,15 +383,15 @@
     print(domain.inputs)
     X = d_optimality._convert_input_to_model_tensor(x).detach().numpy()
     assert np.allclose(X, np.array([[1, 1, 0, 0], [1, 0, 2, 0], [1, 0, 0, 3]]))
 
 
 def test_DOptimality_instantiation():
     # default jacobian building block
-    domain = Domain(
+    domain = Domain.from_lists(
         inputs=[
             ContinuousInput(
                 key=f"x{i+1}",
                 bounds=(0, 1),
             )
             for i in range(3)
         ],
@@ -430,15 +430,15 @@
 
     assert np.allclose(B, d_optimality._model_jacobian_t(x))
     assert np.shape(
         d_optimality.evaluate_jacobian(np.array([[1, 1, 1], [2, 2, 2]]))
     ) == (6,)
 
     # 5th order model
-    domain = Domain(
+    domain = Domain.from_lists(
         inputs=[
             ContinuousInput(
                 key=f"x{i+1}",
                 bounds=(0, 1),
             )
             for i in range(3)
         ],
@@ -464,15 +464,15 @@
 
 
 def test_DOptimality_evaluate_jacobian():
     # n_experiment = 1, n_inputs = 2, model: x1 + x2
     def jacobian(x: np.ndarray, delta=1e-3) -> np.ndarray:  # type: ignore
         return -2 * x / (x[0] ** 2 + x[1] ** 2 + delta)
 
-    domain = Domain(
+    domain = Domain.from_lists(
         inputs=[
             ContinuousInput(
                 key=f"x{i+1}",
                 bounds=(0, 1),
             )
             for i in range(2)
         ],
@@ -601,15 +601,15 @@
     np.random.seed(1)
     for _ in range(10):
         x = np.random.rand(4)
         assert np.allclose(d_optimality.evaluate_jacobian(x), jacobian(x), rtol=1e-3)
 
 
 def test_DOptimality_evaluate():
-    domain = Domain(
+    domain = Domain.from_lists(
         inputs=[
             ContinuousInput(
                 key=f"x{i+1}",
                 bounds=(0, 1),
             )
             for i in range(3)
         ],
@@ -619,15 +619,15 @@
 
     d_optimality = DOptimality(domain=domain, model=model, n_experiments=3)
     x = np.array([1, 0, 0, 0, 1, 0, 0, 0, 1])
     assert np.allclose(d_optimality.evaluate(x), -np.log(4) - np.log(1e-7))
 
 
 def test_AOptimality_evaluate():
-    domain = Domain(
+    domain = Domain.from_lists(
         inputs=[
             ContinuousInput(
                 key=f"x{i+1}",
                 bounds=(0, 1),
             )
             for i in range(3)
         ],
@@ -638,15 +638,15 @@
     a_optimality = AOptimality(domain=domain, model=model, n_experiments=4)
 
     x = np.array([1, 0, 0, 0, 1, 0, 0, 0, 1, 0, 0, 0])
     assert np.allclose(a_optimality.evaluate(x), 3 * 1.9999991 + 0.9999996)
 
 
 def test_AOptimality_evaluate_jacobian():
-    domain = Domain(
+    domain = Domain.from_lists(
         inputs=[ContinuousInput(key="x1", bounds=(0, 1))],
         outputs=[ContinuousOutput(key="y")],
     )
     model = get_formula_from_string("linear", domain=domain)
 
     a_optimality = AOptimality(domain=domain, model=model, n_experiments=2, delta=0)
 
@@ -659,15 +659,15 @@
             / (x[0] - x[1]) ** 3
         )
 
     assert np.allclose(a_optimality.evaluate_jacobian(x), grad(x))
 
 
 def test_EOptimality_evaluate():
-    domain = Domain(
+    domain = Domain.from_lists(
         inputs=[ContinuousInput(key="x1", bounds=(0, 1))],
         outputs=[ContinuousOutput(key="y")],
     )
     model = get_formula_from_string("linear", domain=domain)
 
     e_optimality = EOptimality(domain=domain, model=model, n_experiments=2, delta=0)
 
@@ -682,15 +682,15 @@
         + 2
     )
 
     assert np.allclose(e_optimality.evaluate(x), -min_eigval)
 
 
 def test_EOptimality_evaluate_jacobian():
-    domain = Domain(
+    domain = Domain.from_lists(
         inputs=[ContinuousInput(key="x1", bounds=(0, 1))],
         outputs=[ContinuousOutput(key="y")],
     )
     model = get_formula_from_string("linear", domain=domain)
 
     e_optimality = EOptimality(domain=domain, model=model, n_experiments=2, delta=0)
 
@@ -707,15 +707,15 @@
             ]
         )
 
     assert np.allclose(e_optimality.evaluate_jacobian(x), grad(x))
 
 
 def test_GOptimality_evaluate():
-    domain = Domain(
+    domain = Domain.from_lists(
         inputs=[ContinuousInput(key="x1", bounds=(0, 1))],
         outputs=[ContinuousOutput(key="y")],
     )
     model = get_formula_from_string("linear", domain=domain)
 
     g_optimality = GOptimality(domain=domain, model=model, n_experiments=2, delta=0)
 
@@ -723,15 +723,15 @@
 
     # all eigenvalues are 1 since A = [[1,1],[1,0.5]] is invertible and therefore H = A (A.T A)^-1 A.T = A A^-1 A.T^-1 A.T = 1
 
     assert np.allclose(g_optimality.evaluate(x), 1)
 
 
 def test_GOptimality_evaluate_jacobian():
-    domain = Domain(
+    domain = Domain.from_lists(
         inputs=[ContinuousInput(key="x1", bounds=(0, 1))],
         outputs=[ContinuousOutput(key="y")],
     )
     model = get_formula_from_string("linear", domain=domain)
 
     g_optimality = GOptimality(domain=domain, model=model, n_experiments=2, delta=0)
 
@@ -740,29 +740,29 @@
     # all eigenvalues are 1 since A = [[1,1],[1,0.5]] is invertible and therefore H = A (A.T A)^-1 A.T = A A^-1 A.T^-1 A.T = 1
     # thus, the jacobian vanishes.
 
     assert np.allclose(g_optimality.evaluate_jacobian(x), np.zeros(2))
 
 
 def test_SpaceFilling_evaluate():
-    domain = Domain(
+    domain = Domain.from_lists(
         inputs=[ContinuousInput(key="x1", bounds=(0, 1))],
         outputs=[ContinuousOutput(key="y")],
     )
     model = get_formula_from_string("linear", domain=domain)
 
     space_filling = SpaceFilling(domain=domain, model=model, n_experiments=4, delta=0)
 
     x = np.array([1, 0.6, 0.1, 0.3])
 
     assert np.allclose(space_filling.evaluate(x), -1.4)
 
 
 def test_SpaceFilling_evaluate_jacobian():
-    domain = Domain(
+    domain = Domain.from_lists(
         inputs=[ContinuousInput(key="x1", bounds=(0, 1))],
         outputs=[ContinuousOutput(key="y")],
     )
     model = get_formula_from_string("linear", domain=domain)
 
     space_filling = SpaceFilling(domain=domain, model=model, n_experiments=4, delta=0)
```

### Comparing `bofire-0.0.4/tests/bofire/strategies/doe/test_utils.py` & `bofire-0.0.5/tests/bofire/strategies/doe/test_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -589,15 +589,14 @@
                 max_count=1,
                 min_count=0,
                 none_also_valid=True,
             ),
         ],
     )
     with pytest.raises(ValueError):
-
         check_nchoosek_constraints_as_bounds(domain)  # FIXME: should be allowed
 
     # Not allowed: names parameters of two NChooseK overlap
     domain = Domain.from_lists(
         inputs=[ContinuousInput(key=f"x{i+1}", bounds=(0, 1)) for i in range(4)],
         outputs=[ContinuousOutput(key="y")],
         constraints=[
```

### Comparing `bofire-0.0.4/tests/bofire/strategies/dummy.py` & `bofire-0.0.5/tests/bofire/strategies/dummy.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/tests/bofire/strategies/specs.py` & `bofire-0.0.5/tests/bofire/strategies/specs.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/tests/bofire/strategies/test_all.py` & `bofire-0.0.5/tests/bofire/strategies/test_all.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/tests/bofire/strategies/test_ask.py` & `bofire-0.0.5/tests/bofire/strategies/test_ask.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 STRATEGY_SPECS_SINGLE_OBJECTIVE = {
     # BoTorchSoboAdditiveStrategy: VALID_BOTORCH_SOBO_STRATEGY_SPEC,
     data_models.MultiplicativeSoboStrategy: VALID_BOTORCH_SOBO_STRATEGY_SPEC,
 }
 STRATEGY_SPECS_MULTI_OBJECTIVE = {
     data_models.QehviStrategy: VALID_BOTORCH_QEHVI_STRATEGY_SPEC,
-    data_models.QnehviStrategy: VALID_BOTORCH_SOBO_STRATEGY_SPEC,
+    data_models.QnehviStrategy: VALID_BOTORCH_QEHVI_STRATEGY_SPEC,
 }
 
 
 # TODO: check this properly
 @pytest.mark.parametrize(
     "cls, spec, categorical, descriptor, candidate_count",
     [
```

### Comparing `bofire-0.0.4/tests/bofire/strategies/test_base.py` & `bofire-0.0.5/tests/bofire/strategies/test_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -283,15 +283,15 @@
             "valid_of1": [1, 0, 1, 0],
             "valid_of2": [0, 1, 1, 0],
         }
     ),
 ]
 
 
-@pytest.mark.parametrize("domain", [(domain) for domain in domains])
+@pytest.mark.parametrize("domain", list(domains))
 def test_base_create(domain: Domain):
     with pytest.raises(ValueError, match="number sobol samples"):
         DummyStrategyDataModel(domain=domain, num_sobol_samples=5)
 
     with pytest.raises(ValueError, match="number raw samples"):
         DummyStrategyDataModel(domain=domain, num_raw_samples=5)
 
@@ -648,50 +648,44 @@
     with pytest.raises(ValueError):
         DummyStrategyDataModel(
             domain=domain, categorical_encoding="ORDINAL", categorical_method="FREE"
         )
 
 
 @pytest.mark.parametrize(
-    "domain, data, acquisition_function",
+    "domain, data",
     [
         (
             domains[0],
             generate_experiments(
                 domains[0], row_count=5, tol=1.0, force_all_categories=True
             ),
-            specs.acquisition_functions.valid().obj().dict(),
         ),
         (
             domains[1],
             generate_experiments(
                 domains[1], row_count=5, tol=1.0, force_all_categories=True
             ),
-            specs.acquisition_functions.valid().obj().dict(),
         ),
         (
             domains[2],
             generate_experiments(
                 domains[2], row_count=5, tol=1.0, force_all_categories=True
             ),
-            specs.acquisition_functions.valid().obj().dict(),
         ),
         (
             domains[4],
             generate_experiments(
                 domains[4], row_count=5, tol=1.0, force_all_categories=True
             ),
-            specs.acquisition_functions.valid().obj().dict(),
         ),
     ],
 )
-def test_base_fit(domain, data, acquisition_function):
-    data_model = DummyStrategyDataModel(
-        domain=domain, acquisition_function=acquisition_function
-    )
+def test_base_fit(domain, data):
+    data_model = DummyStrategyDataModel(domain=domain)
     myStrategy = DummyStrategy(data_model=data_model)
     myStrategy.set_experiments(data)
     myStrategy.fit()
 
 
 # TODO: replace this with proper benchmark methods
 @pytest.mark.parametrize(
@@ -727,16 +721,17 @@
         #     ),
         #     specs.acquisition_functions.valid().obj(),
         # ),
     ],
 )
 def test_base_predict(domain, data, acquisition_function):
     data_model = DummyStrategyDataModel(
-        domain=domain, acquisition_function=acquisition_function
-    )
+        domain=domain
+    )  # , acquisition_function=acquisition_function
+    # )
     myStrategy = DummyStrategy(data_model=data_model)
     myStrategy.tell(experiments=data)
     predictions = myStrategy.predict(data)
     assert len(predictions.columns.tolist()) == 3 * len(domain.get_feature_keys(Output))
     assert data.index[-1] == predictions.index[-1]
 
 
@@ -752,15 +747,15 @@
 )
 def test_base_setup_ask_fixed_features(
     categorical_method, descriptor_method, discrete_method
 ):
     # test for fixed features list
     data_model = DummyStrategyDataModel(
         domain=domains[0],
-        acquisition_function=specs.acquisition_functions.valid().obj(),
+        # acquisition_function=specs.acquisition_functions.valid().obj(),
         categorical_method=categorical_method,
         descriptor_method=descriptor_method,
         discrete_method=discrete_method,
         surrogate_specs=surrogate_data_models.BotorchSurrogates(
             surrogates=[
                 surrogate_data_models.SingleTaskGPSurrogate(
                     inputs=domains[0].inputs,
@@ -791,15 +786,15 @@
         assert fixed_features_list is not None
     else:
         assert fixed_features == {}
         assert fixed_features_list is None
 
     data_model = DummyStrategyDataModel(
         domain=domains[3],
-        acquisition_function=specs.acquisition_functions.valid().obj(),
+        # acquisition_function=specs.acquisition_functions.valid().obj(),
         categorical_method=categorical_method,
         descriptor_method=descriptor_method,
         discrete_method=discrete_method,
     )
     myStrategy = DummyStrategy(data_model=data_model)
     (
         bounds,
@@ -814,15 +809,15 @@
 
 
 def test_base_setup_ask():
     # test for no nchooseks
     benchmark = Hartmann()
     data_model = DummyStrategyDataModel(
         domain=benchmark.domain,
-        acquisition_function=specs.acquisition_functions.valid().obj(),
+        # acquisition_function=specs.acquisition_functions.valid().obj(),
     )
     myStrategy = DummyStrategy(data_model=data_model)
     (
         bounds,
         ic_generator,
         ic_gen_kwargs,
         nchooseks,
@@ -838,15 +833,15 @@
     assert nchooseks is None
     assert fixed_features == {}
     assert fixed_features_list is None
     # test for nchooseks
     benchmark = Hartmann(dim=6, allowed_k=3)
     data_model = DummyStrategyDataModel(
         domain=benchmark.domain,
-        acquisition_function=specs.acquisition_functions.valid().obj(),
+        # acquisition_function=specs.acquisition_functions.valid().obj(),
     )
     myStrategy = DummyStrategy(data_model=data_model)
     (
         bounds,
         ic_generator,
         ic_gen_kwargs,
         nchooseks,
```

### Comparing `bofire-0.0.4/tests/bofire/strategies/test_doe.py` & `bofire-0.0.5/tests/bofire/strategies/test_doe.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,14 @@
     data_model = data_models.DoEStrategy(domain=domain, formula="linear")
     strategy = DoEStrategy(data_model=data_model)
     candidates = strategy.ask(candidate_count=12)
     assert candidates.shape == (12, 3)
 
 
 def test_formulas_implemented():
-
     expected_num_candidates = {
         "linear": 7,  # 1+a+b+c+3
         "linear-and-quadratic": 10,  # 1+a+b+c+a**2+b**2+c**2+3
         "linear-and-interactions": 10,  # 1+a+b+c+ab+ac+bc+3
         "fully-quadratic": 13,  # 1+a+b+c+a**2+b**2+c**2+ab+ac+bc+3
     }
 
@@ -150,17 +149,17 @@
     candidates = strategy.ask(candidate_count=12)
 
     np.random.seed(1)
     candidates_expected = np.array(
         [[0.2, 0.2, 0.6], [0.3, 0.6, 0.1], [0.7, 0.1, 0.2], [0.3, 0.1, 0.6]]
     )
     for row in candidates.to_numpy():
-        assert any([np.allclose(row, o, atol=1e-2) for o in candidates_expected])
+        assert any(np.allclose(row, o, atol=1e-2) for o in candidates_expected)
     for o in candidates_expected[:-1]:
-        assert any([np.allclose(o, row, atol=1e-2) for row in candidates.to_numpy()])
+        assert any(np.allclose(o, row, atol=1e-2) for row in candidates.to_numpy())
 
 
 def test_doe_strategy_amount_of_candidates():
     candidates_fixed = pd.DataFrame(
         np.array([[0.2, 0.2, 0.6], [0.3, 0.6, 0.1], [0.7, 0.1, 0.2], [0.3, 0.1, 0.6]]),
         columns=["x1", "x2", "x3"],
     )
```

### Comparing `bofire-0.0.4/tests/bofire/strategies/test_model_specs_generator.py` & `bofire-0.0.5/tests/bofire/strategies/test_model_specs_generator.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/tests/bofire/strategies/test_qehvi.py` & `bofire-0.0.5/tests/bofire/strategies/test_qehvi.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/tests/bofire/strategies/test_qparego.py` & `bofire-0.0.5/tests/bofire/strategies/test_qparego.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import pytest
 import torch
 from botorch.acquisition.objective import ConstrainedMCObjective, GenericMCObjective
 from pydantic import ValidationError
 
 import bofire.data_models.strategies.api as data_models
 import bofire.data_models.surrogates.api as surrogate_data_models
-import tests.bofire.data_models.specs.api as specs
 from bofire.benchmarks.multi import C2DTLZ2, DTLZ2, CrossCoupling
 from bofire.data_models.domain.api import Outputs
 from bofire.data_models.strategies.api import (
     PolytopeSampler as PolytopeSamplerDataModel,
 )
 from bofire.strategies.api import PolytopeSampler, QparegoStrategy
 from tests.bofire.strategies.test_base import domains
@@ -29,15 +28,15 @@
             surrogate_data_models.SingleTaskGPSurrogate(
                 inputs=domains[6].inputs,
                 outputs=Outputs(features=[domains[6].outputs.get_by_key("of2")]),
             ),
         ]
     ),
     "descriptor_method": "FREE",
-    "acquisition_function": specs.acquisition_functions.valid().obj(),
+    # "acquisition_function": specs.acquisition_functions.valid().obj(),
     "categorical_method": "FREE",
 }
 
 # BotorchSurrogates(
 #                models=[
 #                    SingleTaskGPSurrogate(
 #                        inputs=domains[1].inputs,
@@ -59,22 +58,20 @@
             "surrogate_specs": surrogate_data_models.BotorchSurrogates(
                 surrogates=[
                     surrogate_data_models.MixedSingleTaskGPSurrogate(
                         inputs=domains[2].inputs,
                         outputs=Outputs(
                             features=[domains[2].outputs.get_by_key("of1")]
                         ),
-                        constraints=[],
                     ),
                     surrogate_data_models.MixedSingleTaskGPSurrogate(
                         inputs=domains[2].inputs,
                         outputs=Outputs(
                             features=[domains[2].outputs.get_by_key("of2")]
                         ),
-                        constraints=[],
                     ),
                 ]
             ),
             "descriptor_method": "EXHAUSTIVE",
             "categorical_method": "EXHAUSTIVE",
         },
         {**VALID_BOTORCH_QPAREGO_STRATEGY_SPEC, "seed": 1},
@@ -98,15 +95,15 @@
 def test_invalid_qparego_init_domain(domain):
     with pytest.raises(ValidationError):
         data_models.QparegoStrategy(domain=domain)
 
 
 @pytest.mark.parametrize(
     "num_test_candidates",
-    [num_test_candidates for num_test_candidates in range(1, 2)],
+    list(range(1, 2)),
 )
 def test_qparego(num_test_candidates):
     # generate data
     benchmark = DTLZ2(dim=6)
     random_strategy = PolytopeSampler(
         data_model=PolytopeSamplerDataModel(domain=benchmark.domain)
     )
@@ -123,15 +120,15 @@
     # ask
     candidates = my_strategy.ask(num_test_candidates)
     assert len(candidates) == num_test_candidates
 
 
 @pytest.mark.parametrize(
     "num_test_candidates",
-    [num_test_candidates for num_test_candidates in range(1, 2)],
+    list(range(1, 2)),
 )
 def test_qparego_constraints(num_test_candidates):
     # generate data
     benchmark = C2DTLZ2(dim=4)
     random_strategy = PolytopeSampler(
         data_model=PolytopeSamplerDataModel(domain=benchmark.domain)
     )
```

### Comparing `bofire-0.0.4/tests/bofire/strategies/test_random.py` & `bofire-0.0.5/tests/bofire/strategies/test_random.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/tests/bofire/strategies/test_sobo.py` & `bofire-0.0.5/tests/bofire/strategies/test_sobo.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,23 +6,25 @@
 from botorch.acquisition import (
     qExpectedImprovement,
     qNoisyExpectedImprovement,
     qProbabilityOfImprovement,
     qSimpleRegret,
     qUpperConfidenceBound,
 )
+from botorch.acquisition.objective import GenericMCObjective
 
 import bofire.data_models.strategies.api as data_models
 import tests.bofire.data_models.specs.api as specs
+from bofire.benchmarks.multi import DTLZ2
 from bofire.benchmarks.single import Himmelblau
 from bofire.data_models.acquisition_functions.api import qEI, qNEI, qPI, qSR, qUCB
 from bofire.data_models.strategies.api import (
     PolytopeSampler as PolytopeSamplerDataModel,
 )
-from bofire.strategies.api import PolytopeSampler, SoboStrategy
+from bofire.strategies.api import CustomSoboStrategy, PolytopeSampler, SoboStrategy
 from tests.bofire.strategies.test_base import domains
 
 # from tests.bofire.strategies.botorch.test_model_spec import VALID_MODEL_SPEC_LIST
 
 VALID_BOTORCH_SOBO_STRATEGY_SPEC = {
     "domain": domains[1],
     "acquisition_function": specs.acquisition_functions.valid().obj(),
@@ -174,7 +176,95 @@
         num_experiments,
         len(set(chain(*names.values()))),
     )
     assert X_pending.shape == (
         num_candidates,
         len(set(chain(*names.values()))),
     )
+
+
+def test_custom_get_objective():
+    def f(samples, callables, weights, X):
+        outputs_list = []
+        for c, w in zip(callables, weights):
+            outputs_list.append(c(samples, None) ** w)
+        samples = torch.stack(outputs_list, dim=-1)
+
+        return (samples[..., 0] + samples[..., 1]) * (samples[..., 0] * samples[..., 1])
+
+    benchmark = DTLZ2(3)
+    data_model = data_models.CustomSoboStrategy(
+        domain=benchmark.domain, acquisition_function=qNEI()
+    )
+    strategy = CustomSoboStrategy(data_model=data_model)
+    strategy.f = f
+    generic_objective = strategy._get_objective()
+    assert isinstance(generic_objective, GenericMCObjective)
+
+
+def test_custom_get_objective_invalid():
+    benchmark = DTLZ2(3)
+    data_model = data_models.CustomSoboStrategy(
+        domain=benchmark.domain, acquisition_function=qNEI()
+    )
+    strategy = CustomSoboStrategy(data_model=data_model)
+
+    with pytest.raises(ValueError):
+        strategy._get_objective()
+
+
+def test_custom_dumps_loads():
+    def f(samples, callables, weights, X):
+        outputs_list = []
+        for c, w in zip(callables, weights):
+            outputs_list.append(c(samples, None) ** w)
+        samples = torch.stack(outputs_list, dim=-1)
+
+        return (samples[..., 0] + samples[..., 1]) * (samples[..., 0] * samples[..., 1])
+
+    benchmark = DTLZ2(3)
+    data_model1 = data_models.CustomSoboStrategy(
+        domain=benchmark.domain,
+        acquisition_function=qNEI(),
+        use_output_constraints=False,
+    )
+    strategy1 = CustomSoboStrategy(data_model=data_model1)
+    strategy1.f = f
+    f_str = strategy1.dumps()
+
+    data_model2 = data_models.CustomSoboStrategy(
+        domain=benchmark.domain,
+        acquisition_function=qNEI(),
+        use_output_constraints=False,
+        dump=f_str,
+    )
+    strategy2 = CustomSoboStrategy(data_model=data_model2)
+
+    data_model3 = data_models.CustomSoboStrategy(
+        domain=benchmark.domain, acquisition_function=qNEI()
+    )
+    strategy3 = CustomSoboStrategy(data_model=data_model3)
+    strategy3.loads(f_str)
+
+    assert isinstance(strategy2.f, type(f))
+    assert isinstance(strategy3.f, type(f))
+
+    samples = torch.rand(30, 2, requires_grad=True) * 5
+    objective1 = strategy1._get_objective()
+    output1 = objective1.forward(samples)
+    objective2 = strategy2._get_objective()
+    output2 = objective2.forward(samples)
+    objective3 = strategy3._get_objective()
+    output3 = objective3.forward(samples)
+
+    torch.testing.assert_close(output1, output2)
+    torch.testing.assert_close(output1, output3)
+
+
+def test_custom_dumps_invalid():
+    benchmark = DTLZ2(3)
+    data_model = data_models.CustomSoboStrategy(
+        domain=benchmark.domain, acquisition_function=qNEI()
+    )
+    strategy = CustomSoboStrategy(data_model=data_model)
+    with pytest.raises(ValueError):
+        strategy.dumps()
```

### Comparing `bofire-0.0.4/tests/bofire/strategies/test_strategy.py` & `bofire-0.0.5/tests/bofire/strategies/test_strategy.py`

 * *Files 0% similar despite different names*

```diff
@@ -517,15 +517,15 @@
 )
 def test_predictive_strategy_predict(domain, experiments):
     strategy = dummy.DummyPredictiveStrategy(
         data_model=dummy.DummyPredictiveStrategyDataModel(domain=domain)
     )
     strategy.tell(experiments)
     preds = strategy.predict(generate_candidates(domain=domain))
-    assert sorted(list(preds.columns)) == sorted(
+    assert sorted(preds.columns) == sorted(
         [
             "of1_pred",
             "of2_pred",
             "of1_sd",
             "of2_sd",
             "of1_des",
             "of2_des",
```

### Comparing `bofire-0.0.4/tests/bofire/surrogates/test_cross_validate.py` & `bofire-0.0.5/tests/bofire/surrogates/test_cross_validate.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,15 +175,15 @@
     assert len(hook_results.keys()) == 2
     assert len(hook_results["hook1"]) == 5
     assert hook_results["hook1"] == [(8, 2), (8, 2), (8, 2), (8, 2), (8, 2)]
     assert len(hook_results["hook2"]) == 5
     assert hook_results["hook2"] == [(8, 2), (8, 2), (8, 2), (8, 2), (8, 2)]
 
 
-@pytest.mark.parametrize("folds", [-2, 0, 1, 11])
+@pytest.mark.parametrize("folds", [-2, 0, 1])
 def test_model_cross_validate_invalid(folds):
     inputs = Inputs(
         features=[
             ContinuousInput(
                 key=f"x_{i+1}",
                 bounds=(-4, 4),
             )
```

### Comparing `bofire-0.0.4/tests/bofire/surrogates/test_diagnostics.py` & `bofire-0.0.5/tests/bofire/surrogates/test_diagnostics.py`

 * *Files 3% similar despite different names*

```diff
@@ -198,16 +198,15 @@
         key="a",
         bounds=(10, 20),
     )
     observed = feature.sample(n=n_samples)
     predicted = observed + np.random.normal(loc=0, scale=1, size=n_samples)
     cv = CvResult(key=feature.key, observed=observed, predicted=predicted)
     for metric in metrics.keys():
-        with pytest.raises(ValueError):
-            cv.get_metric(metric)
+        np.isnan(cv.get_metric(metric=metric))
 
 
 def test_cvresults_invalid():
     # test for empty results
     with pytest.raises(ValueError):
         CvResults(results=[])
     # test for wrong keys
@@ -417,7 +416,20 @@
                 cv_results.results[i].standard_deviation.values,
                 transformed["a"][i].standardDeviation,
             )
         else:
             assert transformed["a"][i].standardDeviation is None
         for m in metrics.columns:
             assert metrics.loc[i, m] == transformed["a"][i].metrics[m]
+
+
+def test_CvResults2CrossValidationValues_minimal():
+    cv_results = CvResults(
+        results=[generate_cvresult(key="a", n_samples=2) for _ in range(4)]
+        + [generate_cvresult(key="a", n_samples=1)]
+    )
+    transformed = CvResults2CrossValidationValues(cv_results)
+    for i in range(5):
+        if i < 4:
+            assert transformed["a"][i].metrics is not None
+        else:
+            assert transformed["a"][i].metrics is None
```

### Comparing `bofire-0.0.4/tests/bofire/surrogates/test_feature_importance.py` & `bofire-0.0.5/tests/bofire/surrogates/test_feature_importance.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,9 +87,9 @@
         folds=n_folds,
         hooks={"pemutation_importance": permutation_importance_hook},
     )
     for m in metrics.keys():
         importance = combine_permutation_importances(
             importances=pi["pemutation_importance"], metric=m
         )
-        list(importance.columns) == model.inputs.get_keys()
+        assert list(importance.columns) == model.inputs.get_keys()
         assert len(importance) == n_folds
```

### Comparing `bofire-0.0.4/tests/bofire/surrogates/test_fully_bayesian.py` & `bofire-0.0.5/tests/bofire/surrogates/test_fully_bayesian.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/tests/bofire/surrogates/test_mlp.py` & `bofire-0.0.5/tests/bofire/surrogates/test_mlp.py`

 * *Files 16% similar despite different names*

```diff
@@ -158,42 +158,49 @@
     assert pred.shape == torch.Size((2, 10, 1))
     # test with batches
     batch = torch.from_numpy(experiments[["x_1", "x_2"]].values).unsqueeze(0)
     pred = ens.forward(batch)
     assert pred.shape == torch.Size((1, 2, 10, 1))
 
 
-@pytest.mark.parametrize("scaler", [ScalerEnum.NORMALIZE, ScalerEnum.STANDARDIZE])
+@pytest.mark.parametrize(
+    "scaler", [ScalerEnum.NORMALIZE, ScalerEnum.STANDARDIZE, ScalerEnum.IDENTITY]
+)
 def test_mlp_ensemble_fit(scaler):
     bench = Himmelblau()
     samples = bench.domain.inputs.sample(10)
     experiments = bench.f(samples, return_complete=True)
     ens = MLPEnsemble(
         inputs=bench.domain.inputs,
         outputs=bench.domain.outputs,
         n_estimators=2,
         n_epochs=5,
         scaler=scaler,
     )
     surrogate = surrogates.map(ens)
 
     surrogate.fit(experiments=experiments)
-    assert isinstance(
-        surrogate.model.input_transform,
-        Normalize if scaler == ScalerEnum.NORMALIZE else InputStandardize,
-    )
+    if scaler == ScalerEnum.NORMALIZE:
+        assert isinstance(surrogate.model.input_transform, Normalize)
+    elif scaler == ScalerEnum.STANDARDIZE:
+        assert isinstance(surrogate.model.input_transform, InputStandardize)
+    else:
+        with pytest.raises(AttributeError):
+            assert surrogate.model.input_transform is None
     preds = surrogate.predict(experiments)
     dump = surrogate.dumps()
     surrogate2 = surrogates.map(ens)
     surrogate2.loads(dump)
     preds2 = surrogate2.predict(experiments)
     assert_frame_equal(preds, preds2)
 
 
-@pytest.mark.parametrize("scaler", [ScalerEnum.NORMALIZE, ScalerEnum.STANDARDIZE])
+@pytest.mark.parametrize(
+    "scaler", [ScalerEnum.NORMALIZE, ScalerEnum.STANDARDIZE, ScalerEnum.IDENTITY]
+)
 def test_mlp_ensemble_fit_categorical(scaler):
     inputs = Inputs(
         features=[
             ContinuousInput(
                 key=f"x_{i+1}",
                 bounds=(-4, 4),
             )
@@ -209,24 +216,32 @@
     experiments["valid_y"] = 1
 
     ens = MLPEnsemble(
         inputs=inputs,
         outputs=outputs,
         n_estimators=2,
         n_epochs=5,
-        scaler=ScalerEnum.STANDARDIZE,
+        scaler=scaler,
     )
     surrogate = surrogates.map(ens)
     surrogate.fit(experiments=experiments)
-    assert isinstance(
-        surrogate.model.input_transform,
-        InputStandardize,
-    )
-    assert torch.eq(
-        surrogate.model.input_transform.indices, torch.tensor([0, 1], dtype=torch.int64)
-    ).all()
+    if scaler == ScalerEnum.NORMALIZE:
+        assert isinstance(surrogate.model.input_transform, Normalize)
+        assert torch.eq(
+            surrogate.model.input_transform.indices,
+            torch.tensor([0, 1], dtype=torch.int64),
+        ).all()
+    elif scaler == ScalerEnum.STANDARDIZE:
+        assert isinstance(surrogate.model.input_transform, InputStandardize)
+        assert torch.eq(
+            surrogate.model.input_transform.indices,
+            torch.tensor([0, 1], dtype=torch.int64),
+        ).all()
+    else:
+        with pytest.raises(AttributeError):
+            assert surrogate.model.input_transform is None
     preds = surrogate.predict(experiments)
     dump = surrogate.dumps()
     surrogate2 = surrogates.map(ens)
     surrogate2.loads(dump)
     preds2 = surrogate2.predict(experiments)
     assert_frame_equal(preds, preds2)
```

### Comparing `bofire-0.0.4/tests/bofire/surrogates/test_random_forest.py` & `bofire-0.0.5/tests/bofire/surrogates/test_random_forest.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/tests/bofire/surrogates/test_surrogates.py` & `bofire-0.0.5/tests/bofire/surrogates/test_surrogates.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/tests/bofire/surrogates/test_torch_models.py` & `bofire-0.0.5/tests/bofire/surrogates/test_torch_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     OneHotToNumeric,
 )
 from pandas.testing import assert_frame_equal
 from torch import Tensor
 
 import bofire.data_models.surrogates.api as data_models
 import bofire.surrogates.api as surrogates
-from bofire.data_models.domain.api import Constraints, Inputs, Outputs
+from bofire.data_models.domain.api import Inputs, Outputs
 from bofire.data_models.enum import CategoricalEncodingEnum
 from bofire.data_models.features.api import (
     CategoricalDescriptorInput,
     CategoricalInput,
     ContinuousInput,
     ContinuousOutput,
 )
@@ -57,26 +57,24 @@
             ),
         ]
     )
     outputs = Outputs(features=[ContinuousOutput(key="y")])
     data_model = modelclass(
         inputs=inputs,
         outputs=outputs,
-        constraints=Constraints(),
     )
     surrogate = surrogates.map(data_model)
     assert surrogate.input_preprocessing_specs == {
         "x_cat": CategoricalEncodingEnum.ONE_HOT,
         "cat": CategoricalEncodingEnum.DESCRIPTOR,
     }
     # test that it can also handle incomplete specs
     data_model = modelclass(
         inputs=inputs,
         outputs=outputs,
-        constraints=Constraints(),
         input_preprocessing_specs={"x_cat": CategoricalEncodingEnum.ONE_HOT},
     )
     surrogate = surrogates.map(data_model)
     assert surrogate.input_preprocessing_specs == {
         "x_cat": CategoricalEncodingEnum.ONE_HOT,
         "cat": CategoricalEncodingEnum.DESCRIPTOR,
     }
@@ -865,15 +863,14 @@
     experiments2.loc[experiments2.x_cat == "papa", "y2"] /= 2.0
     experiments2["valid_y2"] = 1
     data_model2 = data_models.MixedSingleTaskGPSurrogate(
         inputs=inputs,
         outputs=outputs,
         input_preprocessing_specs={"x_cat": CategoricalEncodingEnum.ONE_HOT},
         scaler=ScalerEnum.STANDARDIZE,
-        constraints=Constraints(),
     )
     # create models
     data_model = data_models.BotorchSurrogates(surrogates=[data_model1, data_model2])
     botorch_surrogates = BotorchSurrogates(data_model=data_model)
     # unite experiments
     experiments = pd.concat(
         [experiments1, experiments2[["x_cat", "y2", "valid_y2"]]],
```

### Comparing `bofire-0.0.4/tests/conftest.py` & `bofire-0.0.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `bofire-0.0.4/tests/test_docs.py` & `bofire-0.0.5/tests/test_docs.py`

 * *Files identical despite different names*

