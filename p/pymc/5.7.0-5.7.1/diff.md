# Comparing `tmp/pymc-5.7.0.tar.gz` & `tmp/pymc-5.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pymc-5.7.0.tar", last modified: Mon Jul 31 08:57:00 2023, max compression
+gzip compressed data, was "dist/pymc-5.7.1.tar", last modified: Fri Aug  4 07:14:28 2023, max compression
```

## Comparing `pymc-5.7.0.tar` & `pymc-5.7.1.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:57:00.000000 pymc-5.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-07-31 08:56:45.000000 pymc-5.7.0/ARCHITECTURE.md
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-31 08:56:45.000000 pymc-5.7.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-31 08:56:45.000000 pymc-5.7.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    42347 2023-07-31 08:56:45.000000 pymc-5.7.0/GOVERNANCE.md
--rw-r--r--   0 runner    (1001) docker     (123)    12865 2023-07-31 08:56:45.000000 pymc-5.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-31 08:56:45.000000 pymc-5.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11492 2023-07-31 08:57:00.000000 pymc-5.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9130 2023-07-31 08:56:45.000000 pymc-5.7.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)    81106 2023-07-31 08:56:45.000000 pymc-5.7.0/RELEASE-NOTES.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:57:00.000000 pymc-5.7.0/pymc/
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-31 08:57:00.000000 pymc-5.7.0/pymc/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:57:00.000000 pymc-5.7.0/pymc/backends/
--rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21822 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/backends/arviz.py
--rw-r--r--   0 runner    (1001) docker     (123)    19525 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10545 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/backends/mcbackend.py
--rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/backends/ndarray.py
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/backends/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/blocking.py
--rw-r--r--   0 runner    (1001) docker     (123)    16820 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:57:00.000000 pymc-5.7.0/pymc/distributions/
--rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/distributions/bound.py
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/distributions/censored.py
--rw-r--r--   0 runner    (1001) docker     (123)   118744 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/distributions/continuous.py
--rw-r--r--   0 runner    (1001) docker     (123)    42226 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/distributions/discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)    15229 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/distributions/dist_math.py
--rw-r--r--   0 runner    (1001) docker     (123)    46281 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/distributions/distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)    36248 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/distributions/mixture.py
--rw-r--r--   0 runner    (1001) docker     (123)    90174 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/distributions/multivariate.py
--rw-r--r--   0 runner    (1001) docker     (123)    18227 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/distributions/shape_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12579 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/distributions/simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)    38767 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/distributions/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)    12769 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/distributions/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    14684 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/distributions/truncated.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/func_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:57:00.000000 pymc-5.7.0/pymc/gp/
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/gp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38434 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/gp/cov.py
--rw-r--r--   0 runner    (1001) docker     (123)    49766 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/gp/gp.py
--rw-r--r--   0 runner    (1001) docker     (123)    14494 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/gp/hsgp_approx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/gp/mean.py
--rw-r--r--   0 runner    (1001) docker     (123)     7734 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/gp/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11097 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/initial_point.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:57:00.000000 pymc-5.7.0/pymc/logprob/
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/logprob/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/logprob/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)    22033 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/logprob/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/logprob/binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     8678 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/logprob/censoring.py
--rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/logprob/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/logprob/cumsum.py
--rw-r--r--   0 runner    (1001) docker     (123)    21040 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/logprob/mixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/logprob/order.py
--rw-r--r--   0 runner    (1001) docker     (123)    20077 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/logprob/rewriting.py
--rw-r--r--   0 runner    (1001) docker     (123)    22586 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/logprob/scan.py
--rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/logprob/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    35387 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/logprob/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     9828 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/logprob/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14409 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/math.py
--rw-r--r--   0 runner    (1001) docker     (123)    85727 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    16740 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/model_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:57:00.000000 pymc-5.7.0/pymc/ode/
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/ode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9657 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/ode/ode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/ode/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:57:00.000000 pymc-5.7.0/pymc/plots/
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10014 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/printing.py
--rw-r--r--   0 runner    (1001) docker     (123)    39422 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/pytensorf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:57:00.000000 pymc-5.7.0/pymc/sampling/
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/sampling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29883 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/sampling/forward.py
--rw-r--r--   0 runner    (1001) docker     (123)    25872 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/sampling/jax.py
--rw-r--r--   0 runner    (1001) docker     (123)    51405 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/sampling/mcmc.py
--rw-r--r--   0 runner    (1001) docker     (123)    15599 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/sampling/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)    15011 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/sampling/population.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/sampling_jax.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:57:00.000000 pymc-5.7.0/pymc/smc/
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/smc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24432 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/smc/kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)    14868 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/smc/sampling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:57:00.000000 pymc-5.7.0/pymc/stats/
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/stats/convergence.py
--rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/stats/log_likelihood.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:57:00.000000 pymc-5.7.0/pymc/step_methods/
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/step_methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/step_methods/arraystep.py
--rw-r--r--   0 runner    (1001) docker     (123)    11105 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/step_methods/compound.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:57:00.000000 pymc-5.7.0/pymc/step_methods/hmc/
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/step_methods/hmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9044 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/step_methods/hmc/base_hmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/step_methods/hmc/hmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/step_methods/hmc/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    17591 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/step_methods/hmc/nuts.py
--rw-r--r--   0 runner    (1001) docker     (123)    27526 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/step_methods/hmc/quadpotential.py
--rw-r--r--   0 runner    (1001) docker     (123)    36584 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/step_methods/metropolis.py
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/step_methods/slicer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/step_methods/step_sizes.py
--rw-r--r--   0 runner    (1001) docker     (123)    36022 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:57:00.000000 pymc-5.7.0/pymc/tuning/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/tuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/tuning/scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/tuning/starting.py
--rw-r--r--   0 runner    (1001) docker     (123)    16919 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:57:00.000000 pymc-5.7.0/pymc/variational/
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/variational/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13212 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/variational/approximations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/variational/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    28608 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/variational/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/variational/minibatch_rv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/variational/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)    57955 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/variational/opvi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/variational/stein.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/variational/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    37930 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/variational/updates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-31 08:56:45.000000 pymc-5.7.0/pymc/vartypes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:57:00.000000 pymc-5.7.0/pymc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11492 2023-07-31 08:57:00.000000 pymc-5.7.0/pymc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-31 08:57:00.000000 pymc-5.7.0/pymc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 08:57:00.000000 pymc-5.7.0/pymc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-31 08:57:00.000000 pymc-5.7.0/pymc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-31 08:57:00.000000 pymc-5.7.0/pymc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-31 08:56:45.000000 pymc-5.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-31 08:56:45.000000 pymc-5.7.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:57:00.000000 pymc-5.7.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      833 2023-07-31 08:56:45.000000 pymc-5.7.0/scripts/docker_container.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      181 2023-07-31 08:56:45.000000 pymc-5.7.0/scripts/test.sh
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-31 08:57:00.000000 pymc-5.7.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2653 2023-07-31 08:56:45.000000 pymc-5.7.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    81282 2023-07-31 08:56:45.000000 pymc-5.7.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:14:28.000000 pymc-5.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-08-04 07:14:17.000000 pymc-5.7.1/ARCHITECTURE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-08-04 07:14:17.000000 pymc-5.7.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-04 07:14:17.000000 pymc-5.7.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    42347 2023-08-04 07:14:17.000000 pymc-5.7.1/GOVERNANCE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12865 2023-08-04 07:14:17.000000 pymc-5.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-04 07:14:17.000000 pymc-5.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11492 2023-08-04 07:14:28.000000 pymc-5.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9130 2023-08-04 07:14:17.000000 pymc-5.7.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    81106 2023-08-04 07:14:17.000000 pymc-5.7.1/RELEASE-NOTES.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:14:28.000000 pymc-5.7.1/pymc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-08-04 07:14:28.000000 pymc-5.7.1/pymc/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:14:28.000000 pymc-5.7.1/pymc/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21822 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/backends/arviz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19525 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10545 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/backends/mcbackend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/backends/ndarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/backends/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/blocking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16820 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:14:28.000000 pymc-5.7.1/pymc/distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/distributions/bound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/distributions/censored.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118744 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/distributions/continuous.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42226 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/distributions/discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15229 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/distributions/dist_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46281 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/distributions/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36248 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/distributions/mixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90174 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/distributions/multivariate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18227 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/distributions/shape_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12579 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/distributions/simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38767 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/distributions/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12769 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/distributions/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14684 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/distributions/truncated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/func_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:14:28.000000 pymc-5.7.1/pymc/gp/
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/gp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38434 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/gp/cov.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49766 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/gp/gp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14494 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/gp/hsgp_approx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/gp/mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7734 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/gp/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11097 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/initial_point.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:14:28.000000 pymc-5.7.1/pymc/logprob/
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/logprob/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/logprob/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22033 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/logprob/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/logprob/binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8678 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/logprob/censoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/logprob/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/logprob/cumsum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21040 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/logprob/mixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/logprob/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20077 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/logprob/rewriting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22586 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/logprob/scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/logprob/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35387 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/logprob/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9828 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/logprob/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14409 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85727 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16740 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/model_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:14:28.000000 pymc-5.7.1/pymc/ode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/ode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9657 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/ode/ode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/ode/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:14:28.000000 pymc-5.7.1/pymc/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10014 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/printing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39422 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/pytensorf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:14:28.000000 pymc-5.7.1/pymc/sampling/
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/sampling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29883 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/sampling/forward.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25872 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/sampling/jax.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51405 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/sampling/mcmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15599 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/sampling/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15011 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/sampling/population.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/sampling_jax.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:14:28.000000 pymc-5.7.1/pymc/smc/
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/smc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24432 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/smc/kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14868 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/smc/sampling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:14:28.000000 pymc-5.7.1/pymc/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/stats/convergence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/stats/log_likelihood.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:14:28.000000 pymc-5.7.1/pymc/step_methods/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/step_methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/step_methods/arraystep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11105 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/step_methods/compound.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:14:28.000000 pymc-5.7.1/pymc/step_methods/hmc/
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/step_methods/hmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9044 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/step_methods/hmc/base_hmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/step_methods/hmc/hmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/step_methods/hmc/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17591 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/step_methods/hmc/nuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27526 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/step_methods/hmc/quadpotential.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36532 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/step_methods/metropolis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/step_methods/slicer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/step_methods/step_sizes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35828 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:14:28.000000 pymc-5.7.1/pymc/tuning/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/tuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/tuning/scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/tuning/starting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16919 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:14:28.000000 pymc-5.7.1/pymc/variational/
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/variational/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13212 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/variational/approximations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/variational/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28608 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/variational/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/variational/minibatch_rv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/variational/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57955 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/variational/opvi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/variational/stein.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/variational/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37930 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/variational/updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-08-04 07:14:17.000000 pymc-5.7.1/pymc/vartypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:14:28.000000 pymc-5.7.1/pymc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11492 2023-08-04 07:14:28.000000 pymc-5.7.1/pymc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-08-04 07:14:28.000000 pymc-5.7.1/pymc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 07:14:28.000000 pymc-5.7.1/pymc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-04 07:14:28.000000 pymc-5.7.1/pymc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-04 07:14:28.000000 pymc-5.7.1/pymc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-08-04 07:14:17.000000 pymc-5.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-04 07:14:17.000000 pymc-5.7.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 07:14:28.000000 pymc-5.7.1/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      833 2023-08-04 07:14:17.000000 pymc-5.7.1/scripts/docker_container.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      181 2023-08-04 07:14:17.000000 pymc-5.7.1/scripts/test.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-08-04 07:14:28.000000 pymc-5.7.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2653 2023-08-04 07:14:17.000000 pymc-5.7.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81282 2023-08-04 07:14:17.000000 pymc-5.7.1/versioneer.py
```

### Comparing `pymc-5.7.0/ARCHITECTURE.md` & `pymc-5.7.1/ARCHITECTURE.md`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/CODE_OF_CONDUCT.md` & `pymc-5.7.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/CONTRIBUTING.md` & `pymc-5.7.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/GOVERNANCE.md` & `pymc-5.7.1/GOVERNANCE.md`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/LICENSE` & `pymc-5.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/PKG-INFO` & `pymc-5.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymc
-Version: 5.7.0
+Version: 5.7.1
 Summary: Probabilistic Programming in Python: Bayesian Modeling and Probabilistic Machine Learning with PyTensor
 Home-page: http://github.com/pymc-devs/pymc
 Maintainer: PyMC Developers
 Maintainer-email: pymc.devs@gmail.com
 License: Apache License, Version 2.0
 Description: .. image:: https://cdn.rawgit.com/pymc-devs/pymc/main/docs/logos/svg/PyMC_banner.svg
             :height: 100px
```

### Comparing `pymc-5.7.0/README.rst` & `pymc-5.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/RELEASE-NOTES.md` & `pymc-5.7.1/RELEASE-NOTES.md`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/__init__.py` & `pymc-5.7.1/pymc/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/backends/__init__.py` & `pymc-5.7.1/pymc/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/backends/arviz.py` & `pymc-5.7.1/pymc/backends/arviz.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/backends/base.py` & `pymc-5.7.1/pymc/backends/base.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/backends/mcbackend.py` & `pymc-5.7.1/pymc/backends/mcbackend.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/backends/ndarray.py` & `pymc-5.7.1/pymc/backends/ndarray.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/backends/report.py` & `pymc-5.7.1/pymc/backends/report.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/blocking.py` & `pymc-5.7.1/pymc/blocking.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/data.py` & `pymc-5.7.1/pymc/data.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/distributions/__init__.py` & `pymc-5.7.1/pymc/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/distributions/bound.py` & `pymc-5.7.1/pymc/distributions/bound.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/distributions/censored.py` & `pymc-5.7.1/pymc/distributions/censored.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/distributions/continuous.py` & `pymc-5.7.1/pymc/distributions/continuous.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/distributions/discrete.py` & `pymc-5.7.1/pymc/distributions/discrete.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/distributions/dist_math.py` & `pymc-5.7.1/pymc/distributions/dist_math.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/distributions/distribution.py` & `pymc-5.7.1/pymc/distributions/distribution.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/distributions/mixture.py` & `pymc-5.7.1/pymc/distributions/mixture.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/distributions/multivariate.py` & `pymc-5.7.1/pymc/distributions/multivariate.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/distributions/shape_utils.py` & `pymc-5.7.1/pymc/distributions/shape_utils.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/distributions/simulator.py` & `pymc-5.7.1/pymc/distributions/simulator.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/distributions/timeseries.py` & `pymc-5.7.1/pymc/distributions/timeseries.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/distributions/transforms.py` & `pymc-5.7.1/pymc/distributions/transforms.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/distributions/truncated.py` & `pymc-5.7.1/pymc/distributions/truncated.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/exceptions.py` & `pymc-5.7.1/pymc/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/func_utils.py` & `pymc-5.7.1/pymc/func_utils.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/gp/__init__.py` & `pymc-5.7.1/pymc/gp/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/gp/cov.py` & `pymc-5.7.1/pymc/gp/cov.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/gp/gp.py` & `pymc-5.7.1/pymc/gp/gp.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/gp/hsgp_approx.py` & `pymc-5.7.1/pymc/gp/hsgp_approx.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/gp/mean.py` & `pymc-5.7.1/pymc/gp/mean.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/gp/util.py` & `pymc-5.7.1/pymc/gp/util.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/initial_point.py` & `pymc-5.7.1/pymc/initial_point.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/logprob/__init__.py` & `pymc-5.7.1/pymc/logprob/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/logprob/abstract.py` & `pymc-5.7.1/pymc/logprob/abstract.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/logprob/basic.py` & `pymc-5.7.1/pymc/logprob/basic.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/logprob/binary.py` & `pymc-5.7.1/pymc/logprob/binary.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/logprob/censoring.py` & `pymc-5.7.1/pymc/logprob/censoring.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/logprob/checks.py` & `pymc-5.7.1/pymc/logprob/checks.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/logprob/cumsum.py` & `pymc-5.7.1/pymc/logprob/cumsum.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/logprob/mixture.py` & `pymc-5.7.1/pymc/logprob/mixture.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/logprob/order.py` & `pymc-5.7.1/pymc/logprob/order.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/logprob/rewriting.py` & `pymc-5.7.1/pymc/logprob/rewriting.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/logprob/scan.py` & `pymc-5.7.1/pymc/logprob/scan.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/logprob/tensor.py` & `pymc-5.7.1/pymc/logprob/tensor.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/logprob/transforms.py` & `pymc-5.7.1/pymc/logprob/transforms.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/logprob/utils.py` & `pymc-5.7.1/pymc/logprob/utils.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/math.py` & `pymc-5.7.1/pymc/math.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/model.py` & `pymc-5.7.1/pymc/model.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/model_graph.py` & `pymc-5.7.1/pymc/model_graph.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/ode/__init__.py` & `pymc-5.7.1/pymc/ode/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/ode/ode.py` & `pymc-5.7.1/pymc/ode/ode.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/ode/utils.py` & `pymc-5.7.1/pymc/ode/utils.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/plots/__init__.py` & `pymc-5.7.1/pymc/plots/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/printing.py` & `pymc-5.7.1/pymc/printing.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/pytensorf.py` & `pymc-5.7.1/pymc/pytensorf.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/sampling/__init__.py` & `pymc-5.7.1/pymc/sampling/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/sampling/forward.py` & `pymc-5.7.1/pymc/sampling/forward.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/sampling/jax.py` & `pymc-5.7.1/pymc/sampling/jax.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/sampling/mcmc.py` & `pymc-5.7.1/pymc/sampling/mcmc.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/sampling/parallel.py` & `pymc-5.7.1/pymc/sampling/parallel.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/sampling/population.py` & `pymc-5.7.1/pymc/sampling/population.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/sampling_jax.py` & `pymc-5.7.1/pymc/sampling_jax.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/smc/__init__.py` & `pymc-5.7.1/pymc/smc/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/smc/kernels.py` & `pymc-5.7.1/pymc/smc/kernels.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/smc/sampling.py` & `pymc-5.7.1/pymc/smc/sampling.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/stats/__init__.py` & `pymc-5.7.1/pymc/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/stats/convergence.py` & `pymc-5.7.1/pymc/stats/convergence.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/stats/log_likelihood.py` & `pymc-5.7.1/pymc/stats/log_likelihood.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/step_methods/__init__.py` & `pymc-5.7.1/pymc/step_methods/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/step_methods/arraystep.py` & `pymc-5.7.1/pymc/step_methods/arraystep.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/step_methods/compound.py` & `pymc-5.7.1/pymc/step_methods/compound.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/step_methods/hmc/__init__.py` & `pymc-5.7.1/pymc/step_methods/hmc/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/step_methods/hmc/base_hmc.py` & `pymc-5.7.1/pymc/step_methods/hmc/base_hmc.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/step_methods/hmc/hmc.py` & `pymc-5.7.1/pymc/step_methods/hmc/hmc.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/step_methods/hmc/integration.py` & `pymc-5.7.1/pymc/step_methods/hmc/integration.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/step_methods/hmc/nuts.py` & `pymc-5.7.1/pymc/step_methods/hmc/nuts.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/step_methods/hmc/quadpotential.py` & `pymc-5.7.1/pymc/step_methods/hmc/quadpotential.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/step_methods/metropolis.py` & `pymc-5.7.1/pymc/step_methods/metropolis.py`

 * *Files 1% similar despite different names*

```diff
@@ -488,15 +488,14 @@
         if not all([v.dtype in pm.discrete_types for v in vars]):
             raise ValueError("All variables must be binary for BinaryGibbsMetropolis")
 
         super().__init__(vars, [model.compile_logp()])
 
     def reset_tuning(self):
         # There are no tuning parameters in this step method.
-        self.tune = False
         return
 
     def astep(self, apoint: RaveledVars, *args) -> Tuple[RaveledVars, StatsType]:
         logp: Callable[[RaveledVars], np.ndarray] = args[0]
         order = self.order
         if self.shuffle_dims:
             nr.shuffle(order)
@@ -616,15 +615,14 @@
         # that indicates whether a draw was done in a tuning phase.
         self.tune = True
 
         super().__init__(vars, [model.compile_logp()])
 
     def reset_tuning(self):
         # There are no tuning parameters in this step method.
-        self.tune = False
         return
 
     def astep_unif(self, apoint: RaveledVars, *args) -> Tuple[RaveledVars, StatsType]:
         logp = args[0]
         point_map_info = apoint.point_map_info
         q0 = apoint.data
```

### Comparing `pymc-5.7.0/pymc/step_methods/slicer.py` & `pymc-5.7.1/pymc/step_methods/slicer.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/step_methods/step_sizes.py` & `pymc-5.7.1/pymc/step_methods/step_sizes.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/testing.py` & `pymc-5.7.1/pymc/testing.py`

 * *Files 2% similar despite different names*

```diff
@@ -771,32 +771,15 @@
                 p = 1.0
             else:
                 _, p = st.chisquare(observed + 1, expected + 1)
             f -= 1
         assert p > alpha, str(point)
 
 
-class SeededTest:
-    random_seed = 20160911
-    random_state = None
-
-    @classmethod
-    def setup_class(cls):
-        nr.seed(cls.random_seed)
-
-    def setup_method(self):
-        nr.seed(self.random_seed)
-
-    def get_random_state(self, reset=False):
-        if self.random_state is None or reset:
-            self.random_state = nr.RandomState(self.random_seed)
-        return self.random_state
-
-
-class BaseTestDistributionRandom(SeededTest):
+class BaseTestDistributionRandom:
     """
     Base class for tests that new RandomVariables are correctly
     implemented, and that the mapping of parameters between the PyMC
     Distribution and the respective RandomVariable is correct.
 
     Three default tests are provided which check:
     1. Expected inputs are passed to the `rv_op` by the `dist` `classmethod`,
@@ -859,16 +842,17 @@
     checks_to_run: List[str] = []
     size = 15
     decimal = select_by_precision(float64=6, float32=3)
 
     sizes_to_check: Optional[List] = None
     sizes_expected: Optional[List] = None
     repeated_params_shape = 5
+    random_state = None
 
-    def test_distribution(self):
+    def test_distribution(self, seeded_test):
         self.validate_tests_list()
         if self.pymc_dist == pm.Wishart:
             with pytest.warns(UserWarning, match="can currently not be used for MCMC sampling"):
                 self._instantiate_pymc_rv()
         else:
             self._instantiate_pymc_rv()
         if self.reference_dist is not None:
@@ -882,14 +866,19 @@
                 )
             if self.pymc_dist == pm.Wishart and check_name.startswith("check_rv_size"):
                 with pytest.warns(UserWarning, match="can currently not be used for MCMC sampling"):
                     getattr(self, check_name)()
             else:
                 getattr(self, check_name)()
 
+    def get_random_state(self, reset=False):
+        if self.random_state is None or reset:
+            self.random_state = nr.RandomState(20160911)
+        return self.random_state
+
     def _instantiate_pymc_rv(self, dist_params=None):
         params = dist_params if dist_params else self.pymc_dist_params
         self.pymc_rv = self.pymc_dist.dist(
             **params, size=self.size, rng=pytensor.shared(self.get_random_state(reset=True))
         )
 
     def check_pymc_draws_match_reference(self):
```

### Comparing `pymc-5.7.0/pymc/tuning/__init__.py` & `pymc-5.7.1/pymc/tuning/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/tuning/scaling.py` & `pymc-5.7.1/pymc/tuning/scaling.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/tuning/starting.py` & `pymc-5.7.1/pymc/tuning/starting.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/util.py` & `pymc-5.7.1/pymc/util.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/variational/__init__.py` & `pymc-5.7.1/pymc/variational/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/variational/approximations.py` & `pymc-5.7.1/pymc/variational/approximations.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/variational/callbacks.py` & `pymc-5.7.1/pymc/variational/callbacks.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/variational/inference.py` & `pymc-5.7.1/pymc/variational/inference.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/variational/minibatch_rv.py` & `pymc-5.7.1/pymc/variational/minibatch_rv.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/variational/operators.py` & `pymc-5.7.1/pymc/variational/operators.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/variational/opvi.py` & `pymc-5.7.1/pymc/variational/opvi.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/variational/stein.py` & `pymc-5.7.1/pymc/variational/stein.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/variational/test_functions.py` & `pymc-5.7.1/pymc/variational/test_functions.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/variational/updates.py` & `pymc-5.7.1/pymc/variational/updates.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc/vartypes.py` & `pymc-5.7.1/pymc/vartypes.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/pymc.egg-info/PKG-INFO` & `pymc-5.7.1/pymc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymc
-Version: 5.7.0
+Version: 5.7.1
 Summary: Probabilistic Programming in Python: Bayesian Modeling and Probabilistic Machine Learning with PyTensor
 Home-page: http://github.com/pymc-devs/pymc
 Maintainer: PyMC Developers
 Maintainer-email: pymc.devs@gmail.com
 License: Apache License, Version 2.0
 Description: .. image:: https://cdn.rawgit.com/pymc-devs/pymc/main/docs/logos/svg/PyMC_banner.svg
             :height: 100px
```

### Comparing `pymc-5.7.0/pymc.egg-info/SOURCES.txt` & `pymc-5.7.1/pymc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/scripts/docker_container.sh` & `pymc-5.7.1/scripts/docker_container.sh`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/setup.py` & `pymc-5.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `pymc-5.7.0/versioneer.py` & `pymc-5.7.1/versioneer.py`

 * *Files identical despite different names*

