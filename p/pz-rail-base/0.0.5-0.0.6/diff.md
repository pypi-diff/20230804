# Comparing `tmp/pz-rail-base-0.0.5.tar.gz` & `tmp/pz-rail-base-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz-rail-base-0.0.5.tar", last modified: Fri Jul 14 23:10:18 2023, max compression
+gzip compressed data, was "pz-rail-base-0.0.6.tar", last modified: Thu Aug  3 23:27:19 2023, max compression
```

## Comparing `pz-rail-base-0.0.5.tar` & `pz-rail-base-0.0.6.tar`

### file list

```diff
@@ -1,139 +1,143 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.166426 pz-rail-base-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.130423 pz-rail-base-0.0.5/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.130423 pz-rail-base-0.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/.github/workflows/add-issue-to-project-tracker.yml
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-07-14 23:10:18.166426 pz-rail-base-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/rail_packages.yml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 23:10:18.166426 pz-rail-base-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.114422 pz-rail-base-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.134424 pz-rail-base-0.0.5/src/pz_rail_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-07-14 23:10:18.000000 pz-rail-base-0.0.5/src/pz_rail_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-07-14 23:10:18.000000 pz-rail-base-0.0.5/src/pz_rail_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 23:10:18.000000 pz-rail-base-0.0.5/src/pz_rail_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-14 23:10:18.000000 pz-rail-base-0.0.5/src/pz_rail_base.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-14 23:10:18.000000 pz-rail-base-0.0.5/src/pz_rail_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-14 23:10:18.000000 pz-rail-base-0.0.5/src/pz_rail_base.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.122423 pz-rail-base-0.0.5/src/rail/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.134424 pz-rail-base-0.0.5/src/rail/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/cli/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/cli/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/cli/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.138424 pz-rail-base-0.0.5/src/rail/core/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-14 23:10:17.000000 pz-rail-base-0.0.5/src/rail/core/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/core/algo_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/core/common_params.py
--rw-r--r--   0 runner    (1001) docker     (123)    16251 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/core/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    10923 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/core/introspection.py
--rw-r--r--   0 runner    (1001) docker     (123)    14109 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/core/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/core/utilStages.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.138424 pz-rail-base-0.0.5/src/rail/creation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.138424 pz-rail-base-0.0.5/src/rail/creation/degradation/
--rw-r--r--   0 runner    (1001) docker     (123)    30116 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/creation/degradation/lsst_error_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/creation/degradation/quantityCut.py
--rw-r--r--   0 runner    (1001) docker     (123)    22286 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/creation/degradation/spectroscopic_selections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/creation/degrader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/creation/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.142424 pz-rail-base-0.0.5/src/rail/estimation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.142424 pz-rail-base-0.0.5/src/rail/estimation/algos/
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/estimation/algos/naive_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/estimation/algos/point_est_hist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/estimation/algos/random_gauss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/estimation/algos/train_z.py
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/estimation/algos/var_inf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/estimation/estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/estimation/summarizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.142424 pz-rail-base-0.0.5/src/rail/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/evaluation/evaluator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.142424 pz-rail-base-0.0.5/src/rail/evaluation/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/evaluation/metrics/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/evaluation/metrics/cdeloss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/evaluation/metrics/pointestimates.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/evaluation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.142424 pz-rail-base-0.0.5/src/rail/examples_data/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.118423 pz-rail-base-0.0.5/src/rail/examples_data/creation_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.142424 pz-rail-base-0.0.5/src/rail/examples_data/creation_data/configs/
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/creation_data/configs/flowModeler.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.146425 pz-rail-base-0.0.5/src/rail/examples_data/creation_data/data/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/creation_data/data/HSC_grid_settings.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/creation_data/data/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.146425 pz-rail-base-0.0.5/src/rail/examples_data/creation_data/data/success_rate_data/
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/creation_data/data/success_rate_data/DEEP2_success.txt
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_I_success.txt
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_bright_success.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_deep_success.txt
--rw-r--r--   0 runner    (1001) docker     (123)  1000000 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/creation_data/data/success_rate_data/hsc_success.txt
--rw-r--r--   0 runner    (1001) docker     (123)   431705 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/creation_data/data/success_rate_data/zCOSMOS_success.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.122423 pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.150425 pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.150425 pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/AB/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/AB/dummy.txt
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/CWW_HDFN_prior.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.150425 pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/FILTER/
--rw-r--r--   0 runner    (1001) docker     (123)    98003 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_g.res
--rw-r--r--   0 runner    (1001) docker     (123)    95326 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_i.res
--rw-r--r--   0 runner    (1001) docker     (123)    96635 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_r.res
--rw-r--r--   0 runner    (1001) docker     (123)    90216 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_u.res
--rw-r--r--   0 runner    (1001) docker     (123)   100126 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_y.res
--rw-r--r--   0 runner    (1001) docker     (123)    93013 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_z.res
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.154425 pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/SED/
--rwxr-xr-x   0 runner    (1001) docker     (123)      125 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/SED/CWWSB4.list
--rwxr-xr-x   0 runner    (1001) docker     (123)    43750 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/SED/El_B2004a.sed
--rwxr-xr-x   0 runner    (1001) docker     (123)    42830 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/SED/Im_B2004a.sed
--rwxr-xr-x   0 runner    (1001) docker     (123)    72228 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/SED/SB2_B2004a.sed
--rwxr-xr-x   0 runner    (1001) docker     (123)    68560 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/SED/SB3_B2004a.sed
--rwxr-xr-x   0 runner    (1001) docker     (123)    43351 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/SED/Sbc_B2004a.sed
--rwxr-xr-x   0 runner    (1001) docker     (123)    42789 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/SED/Scd_B2004a.sed
--rwxr-xr-x   0 runner    (1001) docker     (123)   179585 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/SED/ssp_25Myr_z008.sed
--rwxr-xr-x   0 runner    (1001) docker     (123)   179584 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/SED/ssp_5Myr_z008.sed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.154425 pz-rail-base-0.0.5/src/rail/examples_data/goldenspike_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.154425 pz-rail-base-0.0.5/src/rail/examples_data/goldenspike_data/configs/
--rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/goldenspike_data/configs/goldenspike_config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.154425 pz-rail-base-0.0.5/src/rail/examples_data/goldenspike_data/data/
--rw-r--r--   0 runner    (1001) docker     (123)  1158108 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/goldenspike_data/data/pretrained_flow.pkl
--rw-r--r--   0 runner    (1001) docker     (123)   873947 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/goldenspike_data/data/test_flow_data.pq
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/goldenspike_data/goldenspike.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.166426 pz-rail-base-0.0.5/src/rail/examples_data/testdata/
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/testdata/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    91936 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/testdata/lsst_filters.npy
--rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/testdata/make_rail_sample_data.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    43200 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/testdata/output_BPZ_lite.fits
--rw-r--r--   0 runner    (1001) docker     (123)    24574 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/testdata/rubin_dm_dc2_example.pq
--rw-r--r--   0 runner    (1001) docker     (123)   662976 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/testdata/test_dc2_training_9816.hdf5
--rw-r--r--   0 runner    (1001) docker     (123)   873930 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/testdata/test_dc2_training_9816.pq
--rw-r--r--   0 runner    (1001) docker     (123)  1192254 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/testdata/test_dc2_training_9816_hyperbolic.pq
--rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/testdata/test_dc2_training_9816_smoothing_params.pq
--rw-r--r--   0 runner    (1001) docker     (123)  1316984 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/testdata/test_dc2_validation_9816.hdf5
--rw-r--r--   0 runner    (1001) docker     (123)    15192 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/testdata/training_100gal.hdf5
--rw-r--r--   0 runner    (1001) docker     (123)     9200 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/testdata/validation_10gal.hdf5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.166426 pz-rail-base-0.0.5/src/rail/stages/
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/stages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.126423 pz-rail-base-0.0.5/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.166426 pz-rail-base-0.0.5/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/tests/cli/test_scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.166426 pz-rail-base-0.0.5/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)     8903 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/tests/core/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    11733 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/tests/core/test_degraders.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/tests/core/test_introspection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/tests/core/test_pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.166426 pz-rail-base-0.0.5/tests/estimation/
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/tests/estimation/test_algos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/tests/estimation/test_summarizers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.166426 pz-rail-base-0.0.5/tests/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/tests/evaluation/test_evaluation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:27:19.396597 pz-rail-base-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:27:19.364597 pz-rail-base-0.0.6/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:27:19.364597 pz-rail-base-0.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/.github/workflows/add-issue-to-project-tracker.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-08-03 23:27:19.396597 pz-rail-base-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/rail_packages.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 23:27:19.396597 pz-rail-base-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:27:19.356597 pz-rail-base-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:27:19.364597 pz-rail-base-0.0.6/src/pz_rail_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-08-03 23:27:19.000000 pz-rail-base-0.0.6/src/pz_rail_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-08-03 23:27:19.000000 pz-rail-base-0.0.6/src/pz_rail_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 23:27:19.000000 pz-rail-base-0.0.6/src/pz_rail_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-03 23:27:19.000000 pz-rail-base-0.0.6/src/pz_rail_base.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-08-03 23:27:19.000000 pz-rail-base-0.0.6/src/pz_rail_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-03 23:27:19.000000 pz-rail-base-0.0.6/src/pz_rail_base.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:27:19.360597 pz-rail-base-0.0.6/src/rail/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:27:19.368597 pz-rail-base-0.0.6/src/rail/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/cli/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/cli/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/cli/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:27:19.368597 pz-rail-base-0.0.6/src/rail/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-03 23:27:19.000000 pz-rail-base-0.0.6/src/rail/core/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/core/algo_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/core/common_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16251 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/core/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10923 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/core/introspection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14109 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/core/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/core/utilStages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:27:19.368597 pz-rail-base-0.0.6/src/rail/creation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:27:19.368597 pz-rail-base-0.0.6/src/rail/creation/degradation/
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/creation/degradation/quantityCut.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22286 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/creation/degradation/spectroscopic_selections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/creation/degrader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/creation/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:27:19.372597 pz-rail-base-0.0.6/src/rail/estimation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:27:19.372597 pz-rail-base-0.0.6/src/rail/estimation/algos/
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/estimation/algos/equal_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/estimation/algos/naive_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/estimation/algos/point_est_hist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/estimation/algos/random_gauss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/estimation/algos/train_z.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/estimation/algos/uniform_binning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/estimation/algos/var_inf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/estimation/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/estimation/estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/estimation/informer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6774 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/estimation/summarizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:27:19.372597 pz-rail-base-0.0.6/src/rail/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/evaluation/evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:27:19.372597 pz-rail-base-0.0.6/src/rail/evaluation/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/evaluation/metrics/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/evaluation/metrics/cdeloss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/evaluation/metrics/pointestimates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/evaluation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:27:19.372597 pz-rail-base-0.0.6/src/rail/examples_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/examples_data/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:27:19.360597 pz-rail-base-0.0.6/src/rail/examples_data/creation_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:27:19.372597 pz-rail-base-0.0.6/src/rail/examples_data/creation_data/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/examples_data/creation_data/configs/flowModeler.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:27:19.372597 pz-rail-base-0.0.6/src/rail/examples_data/creation_data/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/examples_data/creation_data/data/HSC_grid_settings.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/examples_data/creation_data/data/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:27:19.376597 pz-rail-base-0.0.6/src/rail/examples_data/creation_data/data/success_rate_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/examples_data/creation_data/data/success_rate_data/DEEP2_success.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_I_success.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_bright_success.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_deep_success.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  1000000 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/examples_data/creation_data/data/success_rate_data/hsc_success.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   431705 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/examples_data/creation_data/data/success_rate_data/zCOSMOS_success.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:27:19.360597 pz-rail-base-0.0.6/src/rail/examples_data/estimation_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:27:19.376597 pz-rail-base-0.0.6/src/rail/examples_data/estimation_data/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/examples_data/estimation_data/data/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:27:19.376597 pz-rail-base-0.0.6/src/rail/examples_data/estimation_data/data/AB/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/examples_data/estimation_data/data/AB/dummy.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/examples_data/estimation_data/data/CWW_HDFN_prior.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:27:19.380597 pz-rail-base-0.0.6/src/rail/examples_data/estimation_data/data/FILTER/
+-rw-r--r--   0 runner    (1001) docker     (123)    98003 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_g.res
+-rw-r--r--   0 runner    (1001) docker     (123)    95326 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_i.res
+-rw-r--r--   0 runner    (1001) docker     (123)    96635 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_r.res
+-rw-r--r--   0 runner    (1001) docker     (123)    90216 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_u.res
+-rw-r--r--   0 runner    (1001) docker     (123)   100126 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_y.res
+-rw-r--r--   0 runner    (1001) docker     (123)    93013 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_z.res
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:27:19.384597 pz-rail-base-0.0.6/src/rail/examples_data/estimation_data/data/SED/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      125 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/examples_data/estimation_data/data/SED/CWWSB4.list
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43750 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/examples_data/estimation_data/data/SED/El_B2004a.sed
+-rwxr-xr-x   0 runner    (1001) docker     (123)    42830 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/examples_data/estimation_data/data/SED/Im_B2004a.sed
+-rwxr-xr-x   0 runner    (1001) docker     (123)    72228 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/examples_data/estimation_data/data/SED/SB2_B2004a.sed
+-rwxr-xr-x   0 runner    (1001) docker     (123)    68560 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/examples_data/estimation_data/data/SED/SB3_B2004a.sed
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43351 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/examples_data/estimation_data/data/SED/Sbc_B2004a.sed
+-rwxr-xr-x   0 runner    (1001) docker     (123)    42789 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/examples_data/estimation_data/data/SED/Scd_B2004a.sed
+-rwxr-xr-x   0 runner    (1001) docker     (123)   179585 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/examples_data/estimation_data/data/SED/ssp_25Myr_z008.sed
+-rwxr-xr-x   0 runner    (1001) docker     (123)   179584 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/examples_data/estimation_data/data/SED/ssp_5Myr_z008.sed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:27:19.384597 pz-rail-base-0.0.6/src/rail/examples_data/goldenspike_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:27:19.384597 pz-rail-base-0.0.6/src/rail/examples_data/goldenspike_data/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/examples_data/goldenspike_data/configs/goldenspike_config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:27:19.384597 pz-rail-base-0.0.6/src/rail/examples_data/goldenspike_data/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  1158108 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/examples_data/goldenspike_data/data/pretrained_flow.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)   873947 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/examples_data/goldenspike_data/data/test_flow_data.pq
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/examples_data/goldenspike_data/goldenspike.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:27:19.396597 pz-rail-base-0.0.6/src/rail/examples_data/testdata/
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/examples_data/testdata/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    91936 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/examples_data/testdata/lsst_filters.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/examples_data/testdata/make_rail_sample_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    43200 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/examples_data/testdata/output_BPZ_lite.fits
+-rw-r--r--   0 runner    (1001) docker     (123)    24574 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/examples_data/testdata/rubin_dm_dc2_example.pq
+-rw-r--r--   0 runner    (1001) docker     (123)   662976 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/examples_data/testdata/test_dc2_training_9816.hdf5
+-rw-r--r--   0 runner    (1001) docker     (123)   873930 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/examples_data/testdata/test_dc2_training_9816.pq
+-rw-r--r--   0 runner    (1001) docker     (123)  1192254 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/examples_data/testdata/test_dc2_training_9816_hyperbolic.pq
+-rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/examples_data/testdata/test_dc2_training_9816_smoothing_params.pq
+-rw-r--r--   0 runner    (1001) docker     (123)  1316984 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/examples_data/testdata/test_dc2_validation_9816.hdf5
+-rw-r--r--   0 runner    (1001) docker     (123)    15192 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/examples_data/testdata/training_100gal.hdf5
+-rw-r--r--   0 runner    (1001) docker     (123)     9200 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/examples_data/testdata/validation_10gal.hdf5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:27:19.396597 pz-rail-base-0.0.6/src/rail/stages/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/src/rail/stages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:27:19.360597 pz-rail-base-0.0.6/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:27:19.396597 pz-rail-base-0.0.6/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/tests/cli/test_scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:27:19.396597 pz-rail-base-0.0.6/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     8903 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/tests/core/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/tests/core/test_degraders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/tests/core/test_introspection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/tests/core/test_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:27:19.396597 pz-rail-base-0.0.6/tests/estimation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/tests/estimation/test_algos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/tests/estimation/test_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/tests/estimation/test_summarizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:27:19.396597 pz-rail-base-0.0.6/tests/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-08-03 23:27:03.000000 pz-rail-base-0.0.6/tests/evaluation/test_evaluation.py
```

### Comparing `pz-rail-base-0.0.5/.github/pull_request_template.md` & `pz-rail-base-0.0.6/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/.github/workflows/linting.yml` & `pz-rail-base-0.0.6/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/.github/workflows/publish-to-pypi.yml` & `pz-rail-base-0.0.6/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/.github/workflows/smoke-test.yml` & `pz-rail-base-0.0.6/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/.github/workflows/testing-and-coverage.yml` & `pz-rail-base-0.0.6/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/.gitignore` & `pz-rail-base-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/.pre-commit-config.yaml` & `pz-rail-base-0.0.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/LICENSE` & `pz-rail-base-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/PKG-INFO` & `pz-rail-base-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-base
-Version: 0.0.5
+Version: 0.0.6
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <later@later.com>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pz-rail-base-0.0.5/README.md` & `pz-rail-base-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/pyproject.toml` & `pz-rail-base-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/src/pz_rail_base.egg-info/PKG-INFO` & `pz-rail-base-0.0.6/src/pz_rail_base.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-base
-Version: 0.0.5
+Version: 0.0.6
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <later@later.com>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pz-rail-base-0.0.5/src/pz_rail_base.egg-info/SOURCES.txt` & `pz-rail-base-0.0.6/src/pz_rail_base.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -29,23 +29,26 @@
 src/rail/core/data.py
 src/rail/core/introspection.py
 src/rail/core/stage.py
 src/rail/core/utilStages.py
 src/rail/core/utils.py
 src/rail/creation/degrader.py
 src/rail/creation/engine.py
-src/rail/creation/degradation/lsst_error_model.py
 src/rail/creation/degradation/quantityCut.py
 src/rail/creation/degradation/spectroscopic_selections.py
+src/rail/estimation/classifier.py
 src/rail/estimation/estimator.py
+src/rail/estimation/informer.py
 src/rail/estimation/summarizer.py
+src/rail/estimation/algos/equal_count.py
 src/rail/estimation/algos/naive_stack.py
 src/rail/estimation/algos/point_est_hist.py
 src/rail/estimation/algos/random_gauss.py
 src/rail/estimation/algos/train_z.py
+src/rail/estimation/algos/uniform_binning.py
 src/rail/estimation/algos/var_inf.py
 src/rail/evaluation/evaluator.py
 src/rail/evaluation/utils.py
 src/rail/evaluation/metrics/base.py
 src/rail/evaluation/metrics/cdeloss.py
 src/rail/evaluation/metrics/pointestimates.py
 src/rail/examples_data/.gitignore
@@ -95,9 +98,10 @@
 src/rail/stages/__init__.py
 tests/cli/test_scripts.py
 tests/core/test_core.py
 tests/core/test_degraders.py
 tests/core/test_introspection.py
 tests/core/test_pipeline.py
 tests/estimation/test_algos.py
+tests/estimation/test_classifier.py
 tests/estimation/test_summarizers.py
 tests/evaluation/test_evaluation.py
```

### Comparing `pz-rail-base-0.0.5/src/rail/cli/commands.py` & `pz-rail-base-0.0.6/src/rail/cli/commands.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,16 +25,26 @@
 @options.git_mode()
 @options.dry_run()
 @options.package_file()
 def clone_source(outdir, git_mode, dry_run, package_file, **kwargs):
     """Install packages from source"""
     scripts.clone_source(outdir, git_mode, dry_run, package_file)
     return 0
+   
+    
+@cli.command()
+@options.outdir(default='..')
+@options.dry_run()
+@options.package_file()
+def update_source(outdir, dry_run, package_file, **kwargs):
+    """Update packages from source"""
+    scripts.update_source(outdir, dry_run, package_file)
+    return 0
+    
     
-
 @cli.command()
 @options.outdir(default='..')
 @options.dry_run()
 @options.from_source()
 @options.package_file()
 def install(outdir, dry_run, from_source, package_file, **kwargs):
     """Install rail packages one by one, to be fault tolerant"""
```

### Comparing `pz-rail-base-0.0.5/src/rail/cli/options.py` & `pz-rail-base-0.0.6/src/rail/cli/options.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/src/rail/cli/scripts.py` & `pz-rail-base-0.0.6/src/rail/cli/scripts.py`

 * *Files 11% similar despite different names*

```diff
@@ -67,14 +67,35 @@
             com_line = f"gh repo clone LSSTDESC/{key} {outdir}/{key}"
 
         if dry_run:
             print(com_line)
         else:
             os.system(com_line)
 
+            
+def update_source(outdir, dry_run, package_file):
+
+    with open(package_file) as pfile:
+        package_dict = yaml.safe_load(pfile)
+
+    currentpath = os.path.abspath('.')    
+    for key, val in package_dict.items():
+        abspath = os.path.abspath(f"{outdir}/{key}")
+
+        if os.path.exists(f"{outdir}/{key}") is not True:
+            print(f"Package {outdir}/{key} does not exist!")
+            continue            
+                
+        com_line = f"cd {abspath} && git pull && cd {currentpath}"
+
+        if dry_run:
+            print(com_line)
+        else:
+            os.system(com_line)
+            
 
 def install(outdir, from_source, dry_run, package_file):
 
     with open(package_file) as pfile:
         package_dict = yaml.safe_load(pfile)
 
     for key, val in package_dict.items():
```

### Comparing `pz-rail-base-0.0.5/src/rail/core/__init__.py` & `pz-rail-base-0.0.6/src/rail/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/src/rail/core/algo_utils.py` & `pz-rail-base-0.0.6/src/rail/core/algo_utils.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/src/rail/core/common_params.py` & `pz-rail-base-0.0.6/src/rail/core/common_params.py`

 * *Files 26% similar despite different names*

```diff
@@ -23,15 +23,17 @@
     nzbins=Param(int, 301, msg="The number of gridpoints in the z grid"),
     dz=Param(float, 0.01, msg="delta z in grid"),
     nondetect_val=Param(float, 99.0, msg="value to be replaced with magnitude limit for non detects"),
     bands=Param(list, lsst_mag_cols, msg="Names of columns for magnitgude by filter band"),
     err_bands=Param(list, lsst_mag_err_cols, msg="Names of columns for magnitgude errors by filter band"),
     mag_limits=Param(dict, lsst_def_maglims, msg="Limiting magnitdues by filter"),
     ref_band=Param(str, "mag_i_lsst", msg="band to use in addition to colors"),
-    redshift_col=Param(str, 'redshift', msg="name of redshift column")
+    redshift_col=Param(str, 'redshift', msg="name of redshift column"),
+    calculated_point_estimates=Param(dtype=list, default=[],
+                                     msg="List of strings defining which point estimates to automatically calculate using `qp.Ensemble`. Options include, 'mean', 'mode', 'median'.")
 )
 
 
 def copy_param(param_name):
     """Return a copy of one of the shared parameters"""
     return SHARED_PARAMS.get(param_name).copy()
```

### Comparing `pz-rail-base-0.0.5/src/rail/core/data.py` & `pz-rail-base-0.0.6/src/rail/core/data.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/src/rail/core/introspection.py` & `pz-rail-base-0.0.6/src/rail/core/introspection.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/src/rail/core/stage.py` & `pz-rail-base-0.0.6/src/rail/core/stage.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/src/rail/core/utilStages.py` & `pz-rail-base-0.0.6/src/rail/core/utilStages.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/src/rail/core/utils.py` & `pz-rail-base-0.0.6/src/rail/core/utils.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/src/rail/creation/degradation/quantityCut.py` & `pz-rail-base-0.0.6/src/rail/creation/degradation/quantityCut.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/src/rail/creation/degradation/spectroscopic_selections.py` & `pz-rail-base-0.0.6/src/rail/creation/degradation/spectroscopic_selections.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/src/rail/creation/degrader.py` & `pz-rail-base-0.0.6/src/rail/creation/degrader.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/src/rail/creation/engine.py` & `pz-rail-base-0.0.6/src/rail/creation/engine.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/src/rail/estimation/algos/naive_stack.py` & `pz-rail-base-0.0.6/src/rail/estimation/algos/naive_stack.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/src/rail/estimation/algos/point_est_hist.py` & `pz-rail-base-0.0.6/src/rail/estimation/algos/point_est_hist.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/src/rail/estimation/algos/random_gauss.py` & `pz-rail-base-0.0.6/src/rail/estimation/algos/random_gauss.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/src/rail/estimation/algos/train_z.py` & `pz-rail-base-0.0.6/src/rail/estimation/algos/train_z.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,13 +77,13 @@
         if self.model is None:  # pragma: no cover
             return
         self.zgrid = self.model.zgrid
         self.train_pdf = self.model.pdf
         self.zmode = self.model.zmode
 
     def _process_chunk(self, start, end, data, first):
-        test_size = len(data['mag_i_lsst'])
+        test_size = end - start
         zmode = np.repeat(self.zmode, test_size)
         qp_d = qp.Ensemble(qp.interp,
                            data=dict(xvals=self.zgrid, yvals=np.tile(self.train_pdf, (test_size, 1))))
         qp_d.set_ancil(dict(zmode=zmode))
         self._do_chunk_output(qp_d, start, end, first)
```

### Comparing `pz-rail-base-0.0.5/src/rail/estimation/algos/var_inf.py` & `pz-rail-base-0.0.6/src/rail/estimation/algos/var_inf.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/src/rail/estimation/estimator.py` & `pz-rail-base-0.0.6/src/rail/estimation/estimator.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,37 @@
 """
-Abstract base classes defining redshift estimations Informers and Estimators
+Abstract base classes defining Estimators of individual galaxy redshift uncertainties
 """
 
+from rail.core.common_params import SHARED_PARAMS
 from rail.core.data import TableHandle, QPHandle, ModelHandle
 from rail.core.stage import RailStage
+
 import gc
 
+from rail.estimation.informer import CatInformer
+# for backwards compatibility
+
 class CatEstimator(RailStage):
     """The base class for making photo-z posterior estimates from catalog-like inputs
     (i.e., tables with fluxes in photometric bands among the set of columns)
 
     Estimators use a generic "model", the details of which depends on the sub-class.
 
     They take as "input" tabular data, apply the photo-z estimation and
     provide as "output" a QPEnsemble, with per-object p(z).
 
     """
 
     name = 'CatEstimator'
     config_options = RailStage.config_options.copy()
-    config_options.update(chunk_size=10000, hdf5_groupname=str)
+    config_options.update(
+        chunk_size=10000,
+        hdf5_groupname=SHARED_PARAMS['hdf5_groupname'],
+        calculated_point_estimates=SHARED_PARAMS['calculated_point_estimates'])
     inputs = [('model', ModelHandle),
               ('input', TableHandle)]
     outputs = [('output', QPHandle)]
 
     def __init__(self, args, comm=None):
         """Initialize Estimator"""
         RailStage.__init__(self, args, comm=comm)
@@ -119,63 +127,7 @@
             self._output_handle = self.add_handle('output', data = qp_dstn)
             self._output_handle.initialize_write(self._input_length, communicator = self.comm)
         self._output_handle.set_data(qp_dstn, partial=True)
         self._output_handle.write_chunk(start, end)
 
 
 
-class CatInformer(RailStage):
-    """The base class for informing models used to make photo-z posterior estimates
-    from catalog-like inputs (i.e., tables with fluxes in photometric bands among
-    the set of columns).
-
-    Estimators use a generic "model", the details of which depends on the sub-class.
-    Most estimators will have associated Informer classes, which can be used to inform
-    those models.
-
-    (Note, "Inform" is more generic than "Train" as it also applies to algorithms that
-    are template-based rather than machine learning-based.)
-
-    Informer will produce as output a generic "model", the details of which depends on the sub-class.
-
-    They take as "input" catalog-like tabular data, which is used to "inform" the model.
-    """
-
-    name = 'Informer'
-    config_options = RailStage.config_options.copy()
-    config_options.update(hdf5_groupname=str, save_train=True)
-    inputs = [('input', TableHandle)]
-    outputs = [('model', ModelHandle)]
-
-    def __init__(self, args, comm=None):
-        """Initialize Informer that can inform models for redshift estimation """
-        RailStage.__init__(self, args, comm=comm)
-        self.model = None
-
-    def inform(self, training_data):
-        """The main interface method for Informers
-
-        This will attach the input_data to this `Informer`
-        (for introspection and provenance tracking).
-
-        Then it will call the run() and finalize() methods, which need to
-        be implemented by the sub-classes.
-
-        The run() method will need to register the model that it creates to this Estimator
-        by using `self.add_data('model', model)`.
-
-        Finally, this will return a ModelHandle providing access to the trained model.
-
-        Parameters
-        ----------
-        input_data : `dict` or `TableHandle`
-            dictionary of all input data, or a `TableHandle` providing access to it
-
-        Returns
-        -------
-        model : ModelHandle
-            Handle providing access to trained model
-        """
-        self.set_data('input', training_data)
-        self.run()
-        self.finalize()
-        return self.get_handle('model')
```

### Comparing `pz-rail-base-0.0.5/src/rail/estimation/summarizer.py` & `pz-rail-base-0.0.6/src/rail/estimation/summarizer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 """
-Abstract base classes defining redshift estimations Informers and Estimators
+Abstract base classes defining Summarizers of the redshift distribution of an ensemble of galaxies
 """
 from rail.core.data import QPHandle, TableHandle, ModelHandle
 from rail.core.stage import RailStage
 
+from rail.estimation.informer import PzInformer
+# for backwards compatibility
 
-class CatSummarizer(RailStage):  #pragma: no cover
+
+class CatSummarizer(RailStage):  
     """The base class for classes that go from catalog-like tables
     to ensemble NZ estimates.
 
     CatSummarizer take as "input" a catalog-like table.  I.e., a
     table with fluxes in photometric bands among the set of columns.
 
     provide as "output" a QPEnsemble, with per-ensemble n(z).
@@ -100,15 +103,15 @@
         """
         self.set_data('input', input_data)
         self.run()
         self.finalize()
         return self.get_handle('output')
 
 
-class SZPZSummarizer(RailStage):  #pragma: no cover
+class SZPZSummarizer(RailStage): 
     """The base class for classes that use two sets of data: a photometry sample with
     spec-z values, and a photometry sample with unknown redshifts, e.g. minisom_som and
     outputs a QP Ensemble with bootstrap realization of the N(z) distribution
     """
     name = 'SZPZtoNZSummarizer'
     config_options = RailStage.config_options.copy()
     config_options.update(chunk_size=10000)
@@ -183,61 +186,7 @@
         self.set_data('input', input_data)
         self.set_data('spec_input', spec_data)
         self.run()
         self.finalize()
         return self.get_handle('output')
 
 
-class PzInformer(RailStage):  #pragma: no cover
-    """The base class for informing models used to summarize photo-z posterior estimates
-    from ensembles of p(z) distributions.
-
-    PzSummarizers can use a generic "model", the details of which depends on the sub-class.
-    Some summaer will have associated PzInformer classes, which can be used to inform
-    those models.
-
-    (Note, "Inform" is more generic than "Train" as it also applies to algorithms that
-    are template-based rather than machine learning-based.)
-
-    PzInformer will produce as output a generic "model", the details of which depends on the sub-class.
-
-    They take as "input" a qp.Ensemble of per-galaxy p(z) data, which is used to "inform" the model.
-    """
-
-    name = 'Informer'
-    config_options = RailStage.config_options.copy()
-    inputs = [('input', QPHandle)]
-    outputs = [('model', ModelHandle)]
-
-    def __init__(self, args, comm=None):
-        """Initialize Informer that can inform models for redshift estimation """
-        RailStage.__init__(self, args, comm=comm)
-        self.model = None
-
-    def inform(self, training_data):
-        """The main interface method for Informers
-
-        This will attach the input_data to this `Informer`
-        (for introspection and provenance tracking).
-
-        Then it will call the run() and finalize() methods, which need to
-        be implemented by the sub-classes.
-
-        The run() method will need to register the model that it creates to this Estimator
-        by using `self.add_data('model', model)`.
-
-        Finally, this will return a ModelHandle providing access to the trained model.
-
-        Parameters
-        ----------
-        input_data :  `qp.Ensemble`
-            Per-galaxy p(z), and any ancilary data associated with it
-
-        Returns
-        -------
-        model : ModelHandle
-            Handle providing access to trained model
-        """
-        self.set_data('input', training_data)
-        self.run()
-        self.finalize()
-        return self.get_handle('model')
```

### Comparing `pz-rail-base-0.0.5/src/rail/evaluation/evaluator.py` & `pz-rail-base-0.0.6/src/rail/evaluation/evaluator.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/src/rail/evaluation/metrics/base.py` & `pz-rail-base-0.0.6/src/rail/evaluation/metrics/base.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/src/rail/evaluation/metrics/cdeloss.py` & `pz-rail-base-0.0.6/src/rail/evaluation/metrics/cdeloss.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/src/rail/evaluation/metrics/pointestimates.py` & `pz-rail-base-0.0.6/src/rail/evaluation/metrics/pointestimates.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/src/rail/examples_data/creation_data/data/success_rate_data/DEEP2_success.txt` & `pz-rail-base-0.0.6/src/rail/examples_data/creation_data/data/success_rate_data/DEEP2_success.txt`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_bright_success.txt` & `pz-rail-base-0.0.6/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_bright_success.txt`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_deep_success.txt` & `pz-rail-base-0.0.6/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_deep_success.txt`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/src/rail/examples_data/creation_data/data/success_rate_data/hsc_success.txt` & `pz-rail-base-0.0.6/src/rail/examples_data/creation_data/data/success_rate_data/hsc_success.txt`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/src/rail/examples_data/creation_data/data/success_rate_data/zCOSMOS_success.txt` & `pz-rail-base-0.0.6/src/rail/examples_data/creation_data/data/success_rate_data/zCOSMOS_success.txt`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_g.res` & `pz-rail-base-0.0.6/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_g.res`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_i.res` & `pz-rail-base-0.0.6/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_i.res`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_r.res` & `pz-rail-base-0.0.6/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_r.res`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_u.res` & `pz-rail-base-0.0.6/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_u.res`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_y.res` & `pz-rail-base-0.0.6/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_y.res`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_z.res` & `pz-rail-base-0.0.6/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_z.res`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/SED/El_B2004a.sed` & `pz-rail-base-0.0.6/src/rail/examples_data/estimation_data/data/SED/El_B2004a.sed`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/SED/Im_B2004a.sed` & `pz-rail-base-0.0.6/src/rail/examples_data/estimation_data/data/SED/Im_B2004a.sed`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/SED/SB2_B2004a.sed` & `pz-rail-base-0.0.6/src/rail/examples_data/estimation_data/data/SED/SB2_B2004a.sed`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/SED/SB3_B2004a.sed` & `pz-rail-base-0.0.6/src/rail/examples_data/estimation_data/data/SED/SB3_B2004a.sed`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/SED/Sbc_B2004a.sed` & `pz-rail-base-0.0.6/src/rail/examples_data/estimation_data/data/SED/Sbc_B2004a.sed`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/SED/Scd_B2004a.sed` & `pz-rail-base-0.0.6/src/rail/examples_data/estimation_data/data/SED/Scd_B2004a.sed`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/SED/ssp_25Myr_z008.sed` & `pz-rail-base-0.0.6/src/rail/examples_data/estimation_data/data/SED/ssp_25Myr_z008.sed`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/SED/ssp_5Myr_z008.sed` & `pz-rail-base-0.0.6/src/rail/examples_data/estimation_data/data/SED/ssp_5Myr_z008.sed`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/src/rail/examples_data/goldenspike_data/configs/goldenspike_config.yml` & `pz-rail-base-0.0.6/src/rail/examples_data/goldenspike_data/configs/goldenspike_config.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/src/rail/examples_data/goldenspike_data/data/pretrained_flow.pkl` & `pz-rail-base-0.0.6/src/rail/examples_data/goldenspike_data/data/pretrained_flow.pkl`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/src/rail/examples_data/goldenspike_data/data/test_flow_data.pq` & `pz-rail-base-0.0.6/src/rail/examples_data/goldenspike_data/data/test_flow_data.pq`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/src/rail/examples_data/goldenspike_data/goldenspike.yml` & `pz-rail-base-0.0.6/src/rail/examples_data/goldenspike_data/goldenspike.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/src/rail/examples_data/testdata/README.md` & `pz-rail-base-0.0.6/src/rail/examples_data/testdata/README.md`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/src/rail/examples_data/testdata/lsst_filters.npy` & `pz-rail-base-0.0.6/src/rail/examples_data/testdata/lsst_filters.npy`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/src/rail/examples_data/testdata/make_rail_sample_data.ipynb` & `pz-rail-base-0.0.6/src/rail/examples_data/testdata/make_rail_sample_data.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/src/rail/examples_data/testdata/output_BPZ_lite.fits` & `pz-rail-base-0.0.6/src/rail/examples_data/testdata/output_BPZ_lite.fits`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/src/rail/examples_data/testdata/rubin_dm_dc2_example.pq` & `pz-rail-base-0.0.6/src/rail/examples_data/testdata/rubin_dm_dc2_example.pq`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/src/rail/examples_data/testdata/test_dc2_training_9816.hdf5` & `pz-rail-base-0.0.6/src/rail/examples_data/testdata/test_dc2_training_9816.hdf5`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/src/rail/examples_data/testdata/test_dc2_training_9816.pq` & `pz-rail-base-0.0.6/src/rail/examples_data/testdata/test_dc2_training_9816.pq`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/src/rail/examples_data/testdata/test_dc2_training_9816_hyperbolic.pq` & `pz-rail-base-0.0.6/src/rail/examples_data/testdata/test_dc2_training_9816_hyperbolic.pq`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/src/rail/examples_data/testdata/test_dc2_training_9816_smoothing_params.pq` & `pz-rail-base-0.0.6/src/rail/examples_data/testdata/test_dc2_training_9816_smoothing_params.pq`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/src/rail/examples_data/testdata/test_dc2_validation_9816.hdf5` & `pz-rail-base-0.0.6/src/rail/examples_data/testdata/test_dc2_validation_9816.hdf5`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/src/rail/examples_data/testdata/training_100gal.hdf5` & `pz-rail-base-0.0.6/src/rail/examples_data/testdata/training_100gal.hdf5`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/src/rail/examples_data/testdata/validation_10gal.hdf5` & `pz-rail-base-0.0.6/src/rail/examples_data/testdata/validation_10gal.hdf5`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/src/rail/stages/__init__.py` & `pz-rail-base-0.0.6/src/rail/stages/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from rail.estimation.algos.train_z import *
 from rail.estimation.algos.var_inf import *
 
 from rail.creation.degrader import *
 #from rail.creation.degradation.spectroscopic_degraders import *
 from rail.creation.degradation.spectroscopic_selections import *
 from rail.creation.degradation.quantityCut import *
-from rail.creation.degradation.lsst_error_model import *
 
 from rail.creation.engine import *
 #from rail.creation.engines.flowEngine import *
 #from rail.creation.engines.galaxy_population_components import *
 #from rail.creation.engines.dsps_photometry_creator import *
 #from rail.creation.engines.dsps_sed_modeler import *
```

### Comparing `pz-rail-base-0.0.5/tests/cli/test_scripts.py` & `pz-rail-base-0.0.6/tests/cli/test_scripts.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 
 
 def test_clone_source():
     scripts.clone_source('..', GitMode.ssh, True, 'rail_packages.yml')
     scripts.clone_source('..', GitMode.https, True, 'rail_packages.yml')
     scripts.clone_source('..', GitMode.cli, True, 'rail_packages.yml')
 
+    
+def test_update_source():
+    scripts.update_source('..', True, 'rail_packages.yml')
+
 
 def test_install():
     scripts.install('..', False, True, 'rail_packages.yml')
     scripts.install('..', True, True, 'rail_packages.yml')
 
 
 def test_info():
```

### Comparing `pz-rail-base-0.0.5/tests/core/test_core.py` & `pz-rail-base-0.0.6/tests/core/test_core.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/tests/core/test_introspection.py` & `pz-rail-base-0.0.6/tests/core/test_introspection.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/tests/core/test_pipeline.py` & `pz-rail-base-0.0.6/tests/core/test_pipeline.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,46 +4,41 @@
 import numpy as np
 
 import rail
 from rail.core.data import TableHandle
 from rail.core.stage import RailPipeline, RailStage
 from rail.core.utils import RAILDIR
 from rail.core.utilStages import ColumnMapper, TableConverter
-from rail.creation.degradation.lsst_error_model import LSSTErrorModel
 from rail.creation.degradation.quantityCut import QuantityCut
 
 def test_pipeline():
     DS = RailStage.data_store
     DS.__class__.allow_overwrite = True
     DS.clear()
 
     input_file = os.path.join(RAILDIR, "rail/examples_data/goldenspike_data/data//test_flow_data.pq")
     bands = ["u", "g", "r", "i", "z", "y"]
     band_dict = {band: f"mag_{band}_lsst" for band in bands}
-    rename_dict = {f"mag_{band}_lsst_err": f"mag_err_{band}_lsst" for band in bands}
+    rename_dict = {f"mag_{band}_lsst": f"{band}_lsst" for band in bands}
     post_grid = [float(x) for x in np.linspace(0.0, 5, 21)]
 
-    lsst_error_model_test = LSSTErrorModel.make_stage(name="lsst_error_model_test", bandNames=band_dict)
-
     col_remapper_test = ColumnMapper.make_stage(
         name="col_remapper_test", hdf5_groupname="", columns=rename_dict
     )
 
     table_conv_test = TableConverter.make_stage(name="table_conv_test", output_format="numpyDict", seed=12345)
 
     pipe = ceci.Pipeline.interactive()
     stages = [
-        lsst_error_model_test,
         col_remapper_test,
         table_conv_test,
     ]
     for stage in stages:
         pipe.add_stage(stage)
 
-    col_remapper_test.connect_input(lsst_error_model_test)
     table_conv_test.connect_input(col_remapper_test)
 
     pipe.initialize(dict(input=input_file), dict(output_dir=".", log_dir=".", resume=False), None)
 
     pipe.save("stage.yaml")
 
     pr = ceci.Pipeline.read("stage.yaml")
@@ -71,26 +66,21 @@
     DS.__class__.allow_overwrite = True
     DS.clear()
     pipe = RailPipeline()
 
     input_file = os.path.join(RAILDIR, "rail/examples_data/goldenspike_data/data//test_flow_data.pq")
     bands = ["u", "g", "r", "i", "z", "y"]
     band_dict = {band: f"mag_{band}_lsst" for band in bands}
-    rename_dict = {f"mag_{band}_lsst_err": f"mag_err_{band}_lsst" for band in bands}
+    rename_dict = {f"mag_{band}_lsst": f"{band}_lsst" for band in bands}
     post_grid = [float(x) for x in np.linspace(0.0, 5, 21)]
 
-    pipe.lsst_error_model_test = LSSTErrorModel.build(
-        bandNames=band_dict,
-    )
-
     pipe.col_remapper_test = ColumnMapper.build(
-        connections=dict(input=pipe.lsst_error_model_test.io.output),
-        hdf5_groupname="",
-        columns=rename_dict,
-    )
+         hdf5_groupname="",
+         columns=rename_dict,
+     )
 
     pipe.table_conv_test = TableConverter.build(
         connections=dict(input=pipe.col_remapper_test.io.output),
         output_format="numpyDict",
         seed=12345,
     )
```

### Comparing `pz-rail-base-0.0.5/tests/estimation/test_algos.py` & `pz-rail-base-0.0.6/tests/estimation/test_algos.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,9 +47,7 @@
     train_algo = train_z.TrainZInformer
     pz_algo = train_z.TrainZEstimator
     results, rerun_results, rerun3_results = one_algo(
         "TrainZ", train_algo, pz_algo, train_config_dict, estim_config_dict
     )
     assert np.isclose(results.ancil["zmode"], zb_expected).all()
     assert np.isclose(results.ancil["zmode"], rerun_results.ancil["zmode"]).all()
-
-
```

### Comparing `pz-rail-base-0.0.5/tests/estimation/test_summarizers.py` & `pz-rail-base-0.0.6/tests/estimation/test_summarizers.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.5/tests/evaluation/test_evaluation.py` & `pz-rail-base-0.0.6/tests/evaluation/test_evaluation.py`

 * *Files identical despite different names*

