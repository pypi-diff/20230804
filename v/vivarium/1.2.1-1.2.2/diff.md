# Comparing `tmp/vivarium-1.2.1.tar.gz` & `tmp/vivarium-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vivarium-1.2.1.tar", last modified: Wed Jul 12 23:25:05 2023, max compression
+gzip compressed data, was "vivarium-1.2.2.tar", last modified: Fri Aug  4 17:38:58 2023, max compression
```

## Comparing `vivarium-1.2.1.tar` & `vivarium-1.2.2.tar`

### file list

```diff
@@ -1,262 +1,262 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:25:05.332761 vivarium-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-12 23:24:48.000000 vivarium-1.2.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:25:05.292761 vivarium-1.2.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-12 23:24:48.000000 vivarium-1.2.1/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-12 23:24:48.000000 vivarium-1.2.1/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:25:05.292761 vivarium-1.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-12 23:24:48.000000 vivarium-1.2.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-12 23:24:48.000000 vivarium-1.2.1/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-12 23:24:48.000000 vivarium-1.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-12 23:24:48.000000 vivarium-1.2.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-12 23:24:48.000000 vivarium-1.2.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-12 23:24:48.000000 vivarium-1.2.1/.zenodo.json
--rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-07-12 23:24:48.000000 vivarium-1.2.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-07-12 23:24:48.000000 vivarium-1.2.1/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-12 23:24:48.000000 vivarium-1.2.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-12 23:24:48.000000 vivarium-1.2.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-12 23:24:48.000000 vivarium-1.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-07-12 23:25:05.332761 vivarium-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-12 23:24:48.000000 vivarium-1.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:25:05.292761 vivarium-1.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/nitpick-exceptions
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:25:05.296761 vivarium-1.2.1/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:25:05.296761 vivarium-1.2.1/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/_static/style.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:25:05.296761 vivarium-1.2.1/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/_templates/layout.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:25:05.296761 vivarium-1.2.1/docs/source/api_reference/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/api_reference/config_tree.rst
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/api_reference/exceptions.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:25:05.304761 vivarium-1.2.1/docs/source/api_reference/framework/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:25:05.304761 vivarium-1.2.1/docs/source/api_reference/framework/artifact/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/api_reference/framework/artifact/artifact.rst
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/api_reference/framework/artifact/hdf.rst
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/api_reference/framework/artifact/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/api_reference/framework/artifact/manager.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:25:05.304761 vivarium-1.2.1/docs/source/api_reference/framework/components/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/api_reference/framework/components/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/api_reference/framework/components/manager.rst
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/api_reference/framework/components/parser.rst
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/api_reference/framework/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/api_reference/framework/engine.rst
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/api_reference/framework/event.rst
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/api_reference/framework/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/api_reference/framework/lifecycle.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:25:05.304761 vivarium-1.2.1/docs/source/api_reference/framework/logging/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/api_reference/framework/logging/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/api_reference/framework/logging/manager.rst
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/api_reference/framework/logging/utilities.rst
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/api_reference/framework/lookup.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/api_reference/framework/metrics.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/api_reference/framework/plugins.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:25:05.304761 vivarium-1.2.1/docs/source/api_reference/framework/population/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/api_reference/framework/population/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/api_reference/framework/population/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/api_reference/framework/population/manager.rst
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/api_reference/framework/population/population_view.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:25:05.304761 vivarium-1.2.1/docs/source/api_reference/framework/randomness/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/api_reference/framework/randomness/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/api_reference/framework/randomness/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/api_reference/framework/randomness/index_map.rst
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/api_reference/framework/randomness/manager.rst
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/api_reference/framework/randomness/stream.rst
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/api_reference/framework/resource.rst
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/api_reference/framework/state_machine.rst
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/api_reference/framework/time.rst
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/api_reference/framework/utilities.rst
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/api_reference/framework/values.rst
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/api_reference/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:25:05.304761 vivarium-1.2.1/docs/source/api_reference/interface/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/api_reference/interface/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/api_reference/interface/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/api_reference/interface/interactive.rst
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/api_reference/interface/utilities.rst
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/api_reference/interpolation.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/api_reference/testing_utilities.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:25:05.308761 vivarium-1.2.1/docs/source/concepts/
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/concepts/builder.rst
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/concepts/components.rst
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/concepts/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/concepts/crn.rst
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/concepts/data.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/concepts/entry_points.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/concepts/event.rst
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/concepts/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/concepts/interpolation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8511 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/concepts/lifecycle.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/concepts/logging.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9744 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/concepts/lookup.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:25:05.308761 vivarium-1.2.1/docs/source/concepts/model_specification/
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/concepts/model_specification/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/concepts/model_specification/yaml_basics.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/concepts/population.rst
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/concepts/resource.rst
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/concepts/time.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/concepts/values.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/glossary.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:25:05.312761 vivarium-1.2.1/docs/source/images/
--rw-r--r--   0 runner    (1001) docker     (123)    32924 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/images/crn_compare_cubes.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   474719 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/images/crn_cube.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   736204 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/images/crn_sim_alignment.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    12794 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/images/pipeline.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:25:05.312761 vivarium-1.2.1/docs/source/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/tutorials/artifact.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12496 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/tutorials/boids.rst
--rw-r--r--   0 runner    (1001) docker     (123)    30080 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/tutorials/disease_model.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11860 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/tutorials/exploration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/tutorials/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/tutorials/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:25:05.312761 vivarium-1.2.1/docs/source/tutorials/running_a_simulation/
--rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/tutorials/running_a_simulation/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/tutorials/running_a_simulation/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14686 2023-07-12 23:24:48.000000 vivarium-1.2.1/docs/source/tutorials/running_a_simulation/interactive.rst
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-12 23:24:48.000000 vivarium-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 23:25:05.332761 vivarium-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-07-12 23:24:48.000000 vivarium-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:25:05.280761 vivarium-1.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:25:05.312761 vivarium-1.2.1/src/vivarium/
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-12 23:24:48.000000 vivarium-1.2.1/src/vivarium/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-12 23:24:48.000000 vivarium-1.2.1/src/vivarium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-12 23:25:04.000000 vivarium-1.2.1/src/vivarium/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    20046 2023-07-12 23:24:48.000000 vivarium-1.2.1/src/vivarium/config_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:25:05.316761 vivarium-1.2.1/src/vivarium/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 23:24:48.000000 vivarium-1.2.1/src/vivarium/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:25:05.316761 vivarium-1.2.1/src/vivarium/examples/boids/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-12 23:24:48.000000 vivarium-1.2.1/src/vivarium/examples/boids/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-12 23:24:48.000000 vivarium-1.2.1/src/vivarium/examples/boids/location.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-12 23:24:48.000000 vivarium-1.2.1/src/vivarium/examples/boids/neighbors.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-12 23:24:48.000000 vivarium-1.2.1/src/vivarium/examples/boids/population.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-12 23:24:48.000000 vivarium-1.2.1/src/vivarium/examples/boids/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:25:05.316761 vivarium-1.2.1/src/vivarium/examples/disease_model/
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-12 23:24:48.000000 vivarium-1.2.1/src/vivarium/examples/disease_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7405 2023-07-12 23:24:48.000000 vivarium-1.2.1/src/vivarium/examples/disease_model/disease.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-12 23:24:48.000000 vivarium-1.2.1/src/vivarium/examples/disease_model/disease_model.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-12 23:24:48.000000 vivarium-1.2.1/src/vivarium/examples/disease_model/intervention.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-12 23:24:48.000000 vivarium-1.2.1/src/vivarium/examples/disease_model/mortality.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-12 23:24:48.000000 vivarium-1.2.1/src/vivarium/examples/disease_model/observer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-07-12 23:24:48.000000 vivarium-1.2.1/src/vivarium/examples/disease_model/population.py
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-07-12 23:24:48.000000 vivarium-1.2.1/src/vivarium/examples/disease_model/risk.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-12 23:24:48.000000 vivarium-1.2.1/src/vivarium/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:25:05.316761 vivarium-1.2.1/src/vivarium/framework/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 23:24:48.000000 vivarium-1.2.1/src/vivarium/framework/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:25:05.320762 vivarium-1.2.1/src/vivarium/framework/artifact/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-12 23:24:48.000000 vivarium-1.2.1/src/vivarium/framework/artifact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10295 2023-07-12 23:24:48.000000 vivarium-1.2.1/src/vivarium/framework/artifact/artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)    13292 2023-07-12 23:24:48.000000 vivarium-1.2.1/src/vivarium/framework/artifact/hdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-07-12 23:24:48.000000 vivarium-1.2.1/src/vivarium/framework/artifact/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:25:05.320762 vivarium-1.2.1/src/vivarium/framework/components/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-12 23:24:48.000000 vivarium-1.2.1/src/vivarium/framework/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11649 2023-07-12 23:24:48.000000 vivarium-1.2.1/src/vivarium/framework/components/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     9449 2023-07-12 23:24:48.000000 vivarium-1.2.1/src/vivarium/framework/components/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-07-12 23:24:48.000000 vivarium-1.2.1/src/vivarium/framework/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    15142 2023-07-12 23:24:48.000000 vivarium-1.2.1/src/vivarium/framework/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    10920 2023-07-12 23:24:48.000000 vivarium-1.2.1/src/vivarium/framework/event.py
--rw-r--r--   0 runner    (1001) docker     (123)    22771 2023-07-12 23:24:48.000000 vivarium-1.2.1/src/vivarium/framework/lifecycle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:25:05.320762 vivarium-1.2.1/src/vivarium/framework/logging/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-12 23:24:48.000000 vivarium-1.2.1/src/vivarium/framework/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-12 23:24:48.000000 vivarium-1.2.1/src/vivarium/framework/logging/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-07-12 23:24:48.000000 vivarium-1.2.1/src/vivarium/framework/logging/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    15012 2023-07-12 23:24:48.000000 vivarium-1.2.1/src/vivarium/framework/lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-12 23:24:48.000000 vivarium-1.2.1/src/vivarium/framework/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-07-12 23:24:48.000000 vivarium-1.2.1/src/vivarium/framework/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:25:05.320762 vivarium-1.2.1/src/vivarium/framework/population/
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-12 23:24:48.000000 vivarium-1.2.1/src/vivarium/framework/population/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-12 23:24:48.000000 vivarium-1.2.1/src/vivarium/framework/population/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    17485 2023-07-12 23:24:48.000000 vivarium-1.2.1/src/vivarium/framework/population/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    21337 2023-07-12 23:24:48.000000 vivarium-1.2.1/src/vivarium/framework/population/population_view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:25:05.320762 vivarium-1.2.1/src/vivarium/framework/randomness/
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-12 23:24:48.000000 vivarium-1.2.1/src/vivarium/framework/randomness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-12 23:24:48.000000 vivarium-1.2.1/src/vivarium/framework/randomness/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9897 2023-07-12 23:24:48.000000 vivarium-1.2.1/src/vivarium/framework/randomness/index_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     9250 2023-07-12 23:24:48.000000 vivarium-1.2.1/src/vivarium/framework/randomness/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    15022 2023-07-12 23:24:48.000000 vivarium-1.2.1/src/vivarium/framework/randomness/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)    12195 2023-07-12 23:24:48.000000 vivarium-1.2.1/src/vivarium/framework/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:25:05.320762 vivarium-1.2.1/src/vivarium/framework/results/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-12 23:24:48.000000 vivarium-1.2.1/src/vivarium/framework/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-07-12 23:24:48.000000 vivarium-1.2.1/src/vivarium/framework/results/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-12 23:24:48.000000 vivarium-1.2.1/src/vivarium/framework/results/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-07-12 23:24:48.000000 vivarium-1.2.1/src/vivarium/framework/results/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     9546 2023-07-12 23:24:48.000000 vivarium-1.2.1/src/vivarium/framework/results/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-07-12 23:24:48.000000 vivarium-1.2.1/src/vivarium/framework/results/stratification.py
--rw-r--r--   0 runner    (1001) docker     (123)    17217 2023-07-12 23:24:48.000000 vivarium-1.2.1/src/vivarium/framework/state_machine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-07-12 23:24:48.000000 vivarium-1.2.1/src/vivarium/framework/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-07-12 23:24:48.000000 vivarium-1.2.1/src/vivarium/framework/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    23704 2023-07-12 23:24:48.000000 vivarium-1.2.1/src/vivarium/framework/values.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:25:05.324761 vivarium-1.2.1/src/vivarium/interface/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-12 23:24:48.000000 vivarium-1.2.1/src/vivarium/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6673 2023-07-12 23:24:48.000000 vivarium-1.2.1/src/vivarium/interface/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8523 2023-07-12 23:24:48.000000 vivarium-1.2.1/src/vivarium/interface/interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)     4512 2023-07-12 23:24:48.000000 vivarium-1.2.1/src/vivarium/interface/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    12964 2023-07-12 23:24:48.000000 vivarium-1.2.1/src/vivarium/interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6897 2023-07-12 23:24:48.000000 vivarium-1.2.1/src/vivarium/testing_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:25:05.312761 vivarium-1.2.1/src/vivarium.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-07-12 23:25:05.000000 vivarium-1.2.1/src/vivarium.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8373 2023-07-12 23:25:05.000000 vivarium-1.2.1/src/vivarium.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 23:25:05.000000 vivarium-1.2.1/src/vivarium.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-12 23:25:05.000000 vivarium-1.2.1/src/vivarium.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 23:25:05.000000 vivarium-1.2.1/src/vivarium.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-12 23:25:05.000000 vivarium-1.2.1/src/vivarium.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-12 23:25:05.000000 vivarium-1.2.1/src/vivarium.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:25:05.324761 vivarium-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 23:24:48.000000 vivarium-1.2.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:25:05.324761 vivarium-1.2.1/tests/config_tree/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 23:24:48.000000 vivarium-1.2.1/tests/config_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15651 2023-07-12 23:24:48.000000 vivarium-1.2.1/tests/config_tree/test_basic_functionality.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-12 23:24:48.000000 vivarium-1.2.1/tests/config_tree/test_ingestion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-07-12 23:24:48.000000 vivarium-1.2.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:25:05.324761 vivarium-1.2.1/tests/framework/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 23:24:48.000000 vivarium-1.2.1/tests/framework/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:25:05.324761 vivarium-1.2.1/tests/framework/artifact/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 23:24:48.000000 vivarium-1.2.1/tests/framework/artifact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16988 2023-07-12 23:24:48.000000 vivarium-1.2.1/tests/framework/artifact/test_artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)    11995 2023-07-12 23:24:48.000000 vivarium-1.2.1/tests/framework/artifact/test_hdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-07-12 23:24:48.000000 vivarium-1.2.1/tests/framework/artifact/test_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:25:05.324761 vivarium-1.2.1/tests/framework/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 23:24:48.000000 vivarium-1.2.1/tests/framework/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-07-12 23:24:48.000000 vivarium-1.2.1/tests/framework/components/mocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     9933 2023-07-12 23:24:48.000000 vivarium-1.2.1/tests/framework/components/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-07-12 23:24:48.000000 vivarium-1.2.1/tests/framework/components/test_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:25:05.328761 vivarium-1.2.1/tests/framework/population/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 23:24:48.000000 vivarium-1.2.1/tests/framework/population/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-07-12 23:24:48.000000 vivarium-1.2.1/tests/framework/population/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    26165 2023-07-12 23:24:48.000000 vivarium-1.2.1/tests/framework/population/test_population_view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:25:05.328761 vivarium-1.2.1/tests/framework/randomness/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 23:24:48.000000 vivarium-1.2.1/tests/framework/randomness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-12 23:24:48.000000 vivarium-1.2.1/tests/framework/randomness/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9924 2023-07-12 23:24:48.000000 vivarium-1.2.1/tests/framework/randomness/test_crn.py
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-07-12 23:24:48.000000 vivarium-1.2.1/tests/framework/randomness/test_index_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-07-12 23:24:48.000000 vivarium-1.2.1/tests/framework/randomness/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-07-12 23:24:48.000000 vivarium-1.2.1/tests/framework/randomness/test_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:25:05.328761 vivarium-1.2.1/tests/framework/results/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 23:24:48.000000 vivarium-1.2.1/tests/framework/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-12 23:24:48.000000 vivarium-1.2.1/tests/framework/results/mocks.py
--rw-r--r--   0 runner    (1001) docker     (123)    14210 2023-07-12 23:24:48.000000 vivarium-1.2.1/tests/framework/results/test_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-07-12 23:24:48.000000 vivarium-1.2.1/tests/framework/results/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-07-12 23:24:48.000000 vivarium-1.2.1/tests/framework/results/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-07-12 23:24:48.000000 vivarium-1.2.1/tests/framework/results/test_stratification.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-07-12 23:24:48.000000 vivarium-1.2.1/tests/framework/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     8985 2023-07-12 23:24:48.000000 vivarium-1.2.1/tests/framework/test_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-07-12 23:24:48.000000 vivarium-1.2.1/tests/framework/test_event.py
--rw-r--r--   0 runner    (1001) docker     (123)    12409 2023-07-12 23:24:48.000000 vivarium-1.2.1/tests/framework/test_lifecycle.py
--rw-r--r--   0 runner    (1001) docker     (123)     9776 2023-07-12 23:24:48.000000 vivarium-1.2.1/tests/framework/test_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-07-12 23:24:48.000000 vivarium-1.2.1/tests/framework/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-07-12 23:24:48.000000 vivarium-1.2.1/tests/framework/test_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-07-12 23:24:48.000000 vivarium-1.2.1/tests/framework/test_state_machine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-07-12 23:24:48.000000 vivarium-1.2.1/tests/framework/test_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-12 23:24:48.000000 vivarium-1.2.1/tests/framework/test_values.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:25:05.328761 vivarium-1.2.1/tests/interface/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 23:24:48.000000 vivarium-1.2.1/tests/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-12 23:24:48.000000 vivarium-1.2.1/tests/interface/test_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:25:05.332761 vivarium-1.2.1/tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)  1835468 2023-07-12 23:24:48.000000 vivarium-1.2.1/tests/test_data/artifact.hdf
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-12 23:24:48.000000 vivarium-1.2.1/tests/test_data/bad_model_specification.txt
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-12 23:24:48.000000 vivarium-1.2.1/tests/test_data/mock_model_specification.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-12 23:24:48.000000 vivarium-1.2.1/tests/test_data/mock_model_specification.yml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 23:24:48.000000 vivarium-1.2.1/tests/test_data/mock_user_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 23:24:48.000000 vivarium-1.2.1/tests/test_data/mock_user_config.yml
--rw-r--r--   0 runner    (1001) docker     (123)    18136 2023-07-12 23:24:48.000000 vivarium-1.2.1/tests/test_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-12 23:24:48.000000 vivarium-1.2.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:38:58.969883 vivarium-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-04 17:38:45.000000 vivarium-1.2.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:38:58.941881 vivarium-1.2.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-04 17:38:45.000000 vivarium-1.2.2/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-08-04 17:38:45.000000 vivarium-1.2.2/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:38:58.941881 vivarium-1.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-08-04 17:38:45.000000 vivarium-1.2.2/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-08-04 17:38:45.000000 vivarium-1.2.2/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-08-04 17:38:45.000000 vivarium-1.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-04 17:38:45.000000 vivarium-1.2.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-08-04 17:38:45.000000 vivarium-1.2.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-08-04 17:38:45.000000 vivarium-1.2.2/.zenodo.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10130 2023-08-04 17:38:45.000000 vivarium-1.2.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-08-04 17:38:45.000000 vivarium-1.2.2/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-08-04 17:38:45.000000 vivarium-1.2.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-08-04 17:38:45.000000 vivarium-1.2.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-08-04 17:38:45.000000 vivarium-1.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-08-04 17:38:58.969883 vivarium-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-08-04 17:38:45.000000 vivarium-1.2.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:38:58.941881 vivarium-1.2.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/nitpick-exceptions
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:38:58.941881 vivarium-1.2.2/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:38:58.941881 vivarium-1.2.2/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/_static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:38:58.941881 vivarium-1.2.2/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/_templates/layout.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:38:58.941881 vivarium-1.2.2/docs/source/api_reference/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/api_reference/config_tree.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/api_reference/exceptions.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:38:58.945881 vivarium-1.2.2/docs/source/api_reference/framework/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:38:58.945881 vivarium-1.2.2/docs/source/api_reference/framework/artifact/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/api_reference/framework/artifact/artifact.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/api_reference/framework/artifact/hdf.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/api_reference/framework/artifact/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/api_reference/framework/artifact/manager.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:38:58.945881 vivarium-1.2.2/docs/source/api_reference/framework/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/api_reference/framework/components/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/api_reference/framework/components/manager.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/api_reference/framework/components/parser.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/api_reference/framework/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/api_reference/framework/engine.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/api_reference/framework/event.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/api_reference/framework/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/api_reference/framework/lifecycle.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:38:58.945881 vivarium-1.2.2/docs/source/api_reference/framework/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/api_reference/framework/logging/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/api_reference/framework/logging/manager.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/api_reference/framework/logging/utilities.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/api_reference/framework/lookup.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/api_reference/framework/metrics.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/api_reference/framework/plugins.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:38:58.945881 vivarium-1.2.2/docs/source/api_reference/framework/population/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/api_reference/framework/population/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/api_reference/framework/population/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/api_reference/framework/population/manager.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/api_reference/framework/population/population_view.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:38:58.945881 vivarium-1.2.2/docs/source/api_reference/framework/randomness/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/api_reference/framework/randomness/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/api_reference/framework/randomness/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/api_reference/framework/randomness/index_map.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/api_reference/framework/randomness/manager.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/api_reference/framework/randomness/stream.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/api_reference/framework/resource.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/api_reference/framework/state_machine.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/api_reference/framework/time.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/api_reference/framework/utilities.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/api_reference/framework/values.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/api_reference/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:38:58.945881 vivarium-1.2.2/docs/source/api_reference/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/api_reference/interface/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/api_reference/interface/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/api_reference/interface/interactive.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/api_reference/interface/utilities.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/api_reference/interpolation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/api_reference/testing_utilities.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:38:58.949881 vivarium-1.2.2/docs/source/concepts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/concepts/builder.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/concepts/components.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/concepts/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/concepts/crn.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/concepts/data.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/concepts/entry_points.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/concepts/event.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/concepts/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/concepts/interpolation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8511 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/concepts/lifecycle.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/concepts/logging.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9744 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/concepts/lookup.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:38:58.949881 vivarium-1.2.2/docs/source/concepts/model_specification/
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/concepts/model_specification/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/concepts/model_specification/yaml_basics.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/concepts/population.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/concepts/resource.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/concepts/time.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/concepts/values.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/glossary.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:38:58.949881 vivarium-1.2.2/docs/source/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    32924 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/images/crn_compare_cubes.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   474719 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/images/crn_cube.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   736204 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/images/crn_sim_alignment.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    12794 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/images/pipeline.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:38:58.949881 vivarium-1.2.2/docs/source/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/tutorials/artifact.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12496 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/tutorials/boids.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    30080 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/tutorials/disease_model.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11860 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/tutorials/exploration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/tutorials/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/tutorials/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:38:58.949881 vivarium-1.2.2/docs/source/tutorials/running_a_simulation/
+-rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/tutorials/running_a_simulation/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/tutorials/running_a_simulation/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14686 2023-08-04 17:38:45.000000 vivarium-1.2.2/docs/source/tutorials/running_a_simulation/interactive.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-04 17:38:45.000000 vivarium-1.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 17:38:58.969883 vivarium-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-08-04 17:38:45.000000 vivarium-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:38:58.937880 vivarium-1.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:38:58.953882 vivarium-1.2.2/src/vivarium/
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-08-04 17:38:45.000000 vivarium-1.2.2/src/vivarium/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-08-04 17:38:45.000000 vivarium-1.2.2/src/vivarium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 17:38:58.000000 vivarium-1.2.2/src/vivarium/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20046 2023-08-04 17:38:45.000000 vivarium-1.2.2/src/vivarium/config_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:38:58.953882 vivarium-1.2.2/src/vivarium/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 17:38:45.000000 vivarium-1.2.2/src/vivarium/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:38:58.953882 vivarium-1.2.2/src/vivarium/examples/boids/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-08-04 17:38:45.000000 vivarium-1.2.2/src/vivarium/examples/boids/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-08-04 17:38:45.000000 vivarium-1.2.2/src/vivarium/examples/boids/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-08-04 17:38:45.000000 vivarium-1.2.2/src/vivarium/examples/boids/neighbors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-04 17:38:45.000000 vivarium-1.2.2/src/vivarium/examples/boids/population.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-08-04 17:38:45.000000 vivarium-1.2.2/src/vivarium/examples/boids/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:38:58.953882 vivarium-1.2.2/src/vivarium/examples/disease_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-08-04 17:38:45.000000 vivarium-1.2.2/src/vivarium/examples/disease_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7405 2023-08-04 17:38:45.000000 vivarium-1.2.2/src/vivarium/examples/disease_model/disease.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-08-04 17:38:45.000000 vivarium-1.2.2/src/vivarium/examples/disease_model/disease_model.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-08-04 17:38:45.000000 vivarium-1.2.2/src/vivarium/examples/disease_model/intervention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-08-04 17:38:45.000000 vivarium-1.2.2/src/vivarium/examples/disease_model/mortality.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-08-04 17:38:45.000000 vivarium-1.2.2/src/vivarium/examples/disease_model/observer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-08-04 17:38:45.000000 vivarium-1.2.2/src/vivarium/examples/disease_model/population.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-08-04 17:38:45.000000 vivarium-1.2.2/src/vivarium/examples/disease_model/risk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-08-04 17:38:45.000000 vivarium-1.2.2/src/vivarium/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:38:58.957882 vivarium-1.2.2/src/vivarium/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 17:38:45.000000 vivarium-1.2.2/src/vivarium/framework/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:38:58.957882 vivarium-1.2.2/src/vivarium/framework/artifact/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-08-04 17:38:45.000000 vivarium-1.2.2/src/vivarium/framework/artifact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10295 2023-08-04 17:38:45.000000 vivarium-1.2.2/src/vivarium/framework/artifact/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13292 2023-08-04 17:38:45.000000 vivarium-1.2.2/src/vivarium/framework/artifact/hdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-08-04 17:38:45.000000 vivarium-1.2.2/src/vivarium/framework/artifact/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:38:58.957882 vivarium-1.2.2/src/vivarium/framework/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-04 17:38:45.000000 vivarium-1.2.2/src/vivarium/framework/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11649 2023-08-04 17:38:45.000000 vivarium-1.2.2/src/vivarium/framework/components/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9449 2023-08-04 17:38:45.000000 vivarium-1.2.2/src/vivarium/framework/components/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-08-04 17:38:45.000000 vivarium-1.2.2/src/vivarium/framework/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15142 2023-08-04 17:38:45.000000 vivarium-1.2.2/src/vivarium/framework/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10920 2023-08-04 17:38:45.000000 vivarium-1.2.2/src/vivarium/framework/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22771 2023-08-04 17:38:45.000000 vivarium-1.2.2/src/vivarium/framework/lifecycle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:38:58.957882 vivarium-1.2.2/src/vivarium/framework/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-08-04 17:38:45.000000 vivarium-1.2.2/src/vivarium/framework/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-08-04 17:38:45.000000 vivarium-1.2.2/src/vivarium/framework/logging/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-08-04 17:38:45.000000 vivarium-1.2.2/src/vivarium/framework/logging/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15012 2023-08-04 17:38:45.000000 vivarium-1.2.2/src/vivarium/framework/lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-08-04 17:38:45.000000 vivarium-1.2.2/src/vivarium/framework/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-08-04 17:38:45.000000 vivarium-1.2.2/src/vivarium/framework/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:38:58.957882 vivarium-1.2.2/src/vivarium/framework/population/
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-08-04 17:38:45.000000 vivarium-1.2.2/src/vivarium/framework/population/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-08-04 17:38:45.000000 vivarium-1.2.2/src/vivarium/framework/population/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17485 2023-08-04 17:38:45.000000 vivarium-1.2.2/src/vivarium/framework/population/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21337 2023-08-04 17:38:45.000000 vivarium-1.2.2/src/vivarium/framework/population/population_view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:38:58.961882 vivarium-1.2.2/src/vivarium/framework/randomness/
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-08-04 17:38:45.000000 vivarium-1.2.2/src/vivarium/framework/randomness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-08-04 17:38:45.000000 vivarium-1.2.2/src/vivarium/framework/randomness/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9897 2023-08-04 17:38:45.000000 vivarium-1.2.2/src/vivarium/framework/randomness/index_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9250 2023-08-04 17:38:45.000000 vivarium-1.2.2/src/vivarium/framework/randomness/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15022 2023-08-04 17:38:45.000000 vivarium-1.2.2/src/vivarium/framework/randomness/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12195 2023-08-04 17:38:45.000000 vivarium-1.2.2/src/vivarium/framework/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:38:58.961882 vivarium-1.2.2/src/vivarium/framework/results/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-08-04 17:38:45.000000 vivarium-1.2.2/src/vivarium/framework/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-08-04 17:38:45.000000 vivarium-1.2.2/src/vivarium/framework/results/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-08-04 17:38:45.000000 vivarium-1.2.2/src/vivarium/framework/results/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-08-04 17:38:45.000000 vivarium-1.2.2/src/vivarium/framework/results/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10860 2023-08-04 17:38:45.000000 vivarium-1.2.2/src/vivarium/framework/results/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-08-04 17:38:45.000000 vivarium-1.2.2/src/vivarium/framework/results/stratification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17217 2023-08-04 17:38:45.000000 vivarium-1.2.2/src/vivarium/framework/state_machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-08-04 17:38:45.000000 vivarium-1.2.2/src/vivarium/framework/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-08-04 17:38:45.000000 vivarium-1.2.2/src/vivarium/framework/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23704 2023-08-04 17:38:45.000000 vivarium-1.2.2/src/vivarium/framework/values.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:38:58.961882 vivarium-1.2.2/src/vivarium/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-04 17:38:45.000000 vivarium-1.2.2/src/vivarium/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6673 2023-08-04 17:38:45.000000 vivarium-1.2.2/src/vivarium/interface/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8523 2023-08-04 17:38:45.000000 vivarium-1.2.2/src/vivarium/interface/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4512 2023-08-04 17:38:45.000000 vivarium-1.2.2/src/vivarium/interface/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12964 2023-08-04 17:38:45.000000 vivarium-1.2.2/src/vivarium/interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6897 2023-08-04 17:38:45.000000 vivarium-1.2.2/src/vivarium/testing_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:38:58.953882 vivarium-1.2.2/src/vivarium.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-08-04 17:38:58.000000 vivarium-1.2.2/src/vivarium.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8373 2023-08-04 17:38:58.000000 vivarium-1.2.2/src/vivarium.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 17:38:58.000000 vivarium-1.2.2/src/vivarium.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-04 17:38:58.000000 vivarium-1.2.2/src/vivarium.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 17:38:58.000000 vivarium-1.2.2/src/vivarium.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-08-04 17:38:58.000000 vivarium-1.2.2/src/vivarium.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-04 17:38:58.000000 vivarium-1.2.2/src/vivarium.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:38:58.961882 vivarium-1.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 17:38:45.000000 vivarium-1.2.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:38:58.961882 vivarium-1.2.2/tests/config_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 17:38:45.000000 vivarium-1.2.2/tests/config_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15651 2023-08-04 17:38:45.000000 vivarium-1.2.2/tests/config_tree/test_basic_functionality.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-04 17:38:45.000000 vivarium-1.2.2/tests/config_tree/test_ingestion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-08-04 17:38:45.000000 vivarium-1.2.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:38:58.965883 vivarium-1.2.2/tests/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 17:38:45.000000 vivarium-1.2.2/tests/framework/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:38:58.965883 vivarium-1.2.2/tests/framework/artifact/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 17:38:45.000000 vivarium-1.2.2/tests/framework/artifact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16988 2023-08-04 17:38:45.000000 vivarium-1.2.2/tests/framework/artifact/test_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11995 2023-08-04 17:38:45.000000 vivarium-1.2.2/tests/framework/artifact/test_hdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-08-04 17:38:45.000000 vivarium-1.2.2/tests/framework/artifact/test_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:38:58.965883 vivarium-1.2.2/tests/framework/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 17:38:45.000000 vivarium-1.2.2/tests/framework/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-08-04 17:38:45.000000 vivarium-1.2.2/tests/framework/components/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9933 2023-08-04 17:38:45.000000 vivarium-1.2.2/tests/framework/components/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-08-04 17:38:45.000000 vivarium-1.2.2/tests/framework/components/test_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:38:58.965883 vivarium-1.2.2/tests/framework/population/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 17:38:45.000000 vivarium-1.2.2/tests/framework/population/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-08-04 17:38:45.000000 vivarium-1.2.2/tests/framework/population/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26165 2023-08-04 17:38:45.000000 vivarium-1.2.2/tests/framework/population/test_population_view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:38:58.965883 vivarium-1.2.2/tests/framework/randomness/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 17:38:45.000000 vivarium-1.2.2/tests/framework/randomness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-08-04 17:38:45.000000 vivarium-1.2.2/tests/framework/randomness/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9924 2023-08-04 17:38:45.000000 vivarium-1.2.2/tests/framework/randomness/test_crn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-08-04 17:38:45.000000 vivarium-1.2.2/tests/framework/randomness/test_index_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-08-04 17:38:45.000000 vivarium-1.2.2/tests/framework/randomness/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-08-04 17:38:45.000000 vivarium-1.2.2/tests/framework/randomness/test_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:38:58.965883 vivarium-1.2.2/tests/framework/results/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 17:38:45.000000 vivarium-1.2.2/tests/framework/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-08-04 17:38:45.000000 vivarium-1.2.2/tests/framework/results/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14210 2023-08-04 17:38:45.000000 vivarium-1.2.2/tests/framework/results/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-08-04 17:38:45.000000 vivarium-1.2.2/tests/framework/results/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-08-04 17:38:45.000000 vivarium-1.2.2/tests/framework/results/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-08-04 17:38:45.000000 vivarium-1.2.2/tests/framework/results/test_stratification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-08-04 17:38:45.000000 vivarium-1.2.2/tests/framework/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8985 2023-08-04 17:38:45.000000 vivarium-1.2.2/tests/framework/test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-08-04 17:38:45.000000 vivarium-1.2.2/tests/framework/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12409 2023-08-04 17:38:45.000000 vivarium-1.2.2/tests/framework/test_lifecycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9776 2023-08-04 17:38:45.000000 vivarium-1.2.2/tests/framework/test_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-08-04 17:38:45.000000 vivarium-1.2.2/tests/framework/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-08-04 17:38:45.000000 vivarium-1.2.2/tests/framework/test_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-08-04 17:38:45.000000 vivarium-1.2.2/tests/framework/test_state_machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-08-04 17:38:45.000000 vivarium-1.2.2/tests/framework/test_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-08-04 17:38:45.000000 vivarium-1.2.2/tests/framework/test_values.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:38:58.965883 vivarium-1.2.2/tests/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 17:38:45.000000 vivarium-1.2.2/tests/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-08-04 17:38:45.000000 vivarium-1.2.2/tests/interface/test_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:38:58.969883 vivarium-1.2.2/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)  1835468 2023-08-04 17:38:45.000000 vivarium-1.2.2/tests/test_data/artifact.hdf
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-08-04 17:38:45.000000 vivarium-1.2.2/tests/test_data/bad_model_specification.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-08-04 17:38:45.000000 vivarium-1.2.2/tests/test_data/mock_model_specification.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-08-04 17:38:45.000000 vivarium-1.2.2/tests/test_data/mock_model_specification.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 17:38:45.000000 vivarium-1.2.2/tests/test_data/mock_user_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 17:38:45.000000 vivarium-1.2.2/tests/test_data/mock_user_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    18136 2023-08-04 17:38:45.000000 vivarium-1.2.2/tests/test_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-04 17:38:45.000000 vivarium-1.2.2/tox.ini
```

### Comparing `vivarium-1.2.1/.github/pull_request_template.md` & `vivarium-1.2.2/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/.github/workflows/build.yml` & `vivarium-1.2.2/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/.github/workflows/deploy.yml` & `vivarium-1.2.2/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/.gitignore` & `vivarium-1.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/.zenodo.json` & `vivarium-1.2.2/.zenodo.json`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/CHANGELOG.rst` & `vivarium-1.2.2/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+**1.2.2 - 08/04/23**
+
+ - Bugfix to include all metrics outputs in results manager
+
 **1.2.1 - 07/12/23**
 
  - Adds logging for registering stratifications and observations
  - Changes version metadata to use setuptools_scm
 
 **1.2.0 - 06/01/23**
```

### Comparing `vivarium-1.2.1/CODE_OF_CONDUCT.rst` & `vivarium-1.2.2/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/CONTRIBUTING.rst` & `vivarium-1.2.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/LICENSE.txt` & `vivarium-1.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/PKG-INFO` & `vivarium-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vivarium
-Version: 1.2.1
+Version: 1.2.2
 Summary: vivarium is a microsimulation framework built on top of the standard scientific python stack.
 Home-page: https://github.com/ihmeuw/vivarium
 Author: The vivarium developers
 Author-email: vivarium.dev@gmail.com
 License: BSD-3-Clause
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `vivarium-1.2.1/README.rst` & `vivarium-1.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/docs/Makefile` & `vivarium-1.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/docs/nitpick-exceptions` & `vivarium-1.2.2/docs/nitpick-exceptions`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/docs/source/concepts/builder.rst` & `vivarium-1.2.2/docs/source/concepts/builder.rst`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/docs/source/concepts/crn.rst` & `vivarium-1.2.2/docs/source/concepts/crn.rst`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/docs/source/concepts/entry_points.rst` & `vivarium-1.2.2/docs/source/concepts/entry_points.rst`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/docs/source/concepts/event.rst` & `vivarium-1.2.2/docs/source/concepts/event.rst`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/docs/source/concepts/lifecycle.rst` & `vivarium-1.2.2/docs/source/concepts/lifecycle.rst`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/docs/source/concepts/lookup.rst` & `vivarium-1.2.2/docs/source/concepts/lookup.rst`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/docs/source/concepts/model_specification/index.rst` & `vivarium-1.2.2/docs/source/concepts/model_specification/index.rst`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/docs/source/concepts/model_specification/yaml_basics.rst` & `vivarium-1.2.2/docs/source/concepts/model_specification/yaml_basics.rst`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/docs/source/concepts/population.rst` & `vivarium-1.2.2/docs/source/concepts/population.rst`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/docs/source/concepts/values.rst` & `vivarium-1.2.2/docs/source/concepts/values.rst`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/docs/source/conf.py` & `vivarium-1.2.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/docs/source/glossary.rst` & `vivarium-1.2.2/docs/source/glossary.rst`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/docs/source/images/crn_compare_cubes.jpg` & `vivarium-1.2.2/docs/source/images/crn_compare_cubes.jpg`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/docs/source/images/crn_cube.jpg` & `vivarium-1.2.2/docs/source/images/crn_cube.jpg`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/docs/source/images/crn_sim_alignment.jpg` & `vivarium-1.2.2/docs/source/images/crn_sim_alignment.jpg`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/docs/source/images/pipeline.jpg` & `vivarium-1.2.2/docs/source/images/pipeline.jpg`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/docs/source/installation.rst` & `vivarium-1.2.2/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/docs/source/tutorials/artifact.rst` & `vivarium-1.2.2/docs/source/tutorials/artifact.rst`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/docs/source/tutorials/boids.rst` & `vivarium-1.2.2/docs/source/tutorials/boids.rst`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/docs/source/tutorials/disease_model.rst` & `vivarium-1.2.2/docs/source/tutorials/disease_model.rst`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/docs/source/tutorials/exploration.rst` & `vivarium-1.2.2/docs/source/tutorials/exploration.rst`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/docs/source/tutorials/getting_started.rst` & `vivarium-1.2.2/docs/source/tutorials/getting_started.rst`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/docs/source/tutorials/running_a_simulation/cli.rst` & `vivarium-1.2.2/docs/source/tutorials/running_a_simulation/cli.rst`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/docs/source/tutorials/running_a_simulation/interactive.rst` & `vivarium-1.2.2/docs/source/tutorials/running_a_simulation/interactive.rst`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/setup.py` & `vivarium-1.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/src/vivarium/config_tree.py` & `vivarium-1.2.2/src/vivarium/config_tree.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/src/vivarium/examples/boids/location.py` & `vivarium-1.2.2/src/vivarium/examples/boids/location.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/src/vivarium/examples/boids/neighbors.py` & `vivarium-1.2.2/src/vivarium/examples/boids/neighbors.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/src/vivarium/examples/boids/population.py` & `vivarium-1.2.2/src/vivarium/examples/boids/population.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/src/vivarium/examples/disease_model/__init__.py` & `vivarium-1.2.2/src/vivarium/examples/disease_model/__init__.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/src/vivarium/examples/disease_model/disease.py` & `vivarium-1.2.2/src/vivarium/examples/disease_model/disease.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/src/vivarium/examples/disease_model/disease_model.yaml` & `vivarium-1.2.2/src/vivarium/examples/disease_model/disease_model.yaml`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/src/vivarium/examples/disease_model/intervention.py` & `vivarium-1.2.2/src/vivarium/examples/disease_model/intervention.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/src/vivarium/examples/disease_model/mortality.py` & `vivarium-1.2.2/src/vivarium/examples/disease_model/mortality.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/src/vivarium/examples/disease_model/observer.py` & `vivarium-1.2.2/src/vivarium/examples/disease_model/observer.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/src/vivarium/examples/disease_model/population.py` & `vivarium-1.2.2/src/vivarium/examples/disease_model/population.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/src/vivarium/examples/disease_model/risk.py` & `vivarium-1.2.2/src/vivarium/examples/disease_model/risk.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/src/vivarium/framework/artifact/artifact.py` & `vivarium-1.2.2/src/vivarium/framework/artifact/artifact.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/src/vivarium/framework/artifact/hdf.py` & `vivarium-1.2.2/src/vivarium/framework/artifact/hdf.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/src/vivarium/framework/artifact/manager.py` & `vivarium-1.2.2/src/vivarium/framework/artifact/manager.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/src/vivarium/framework/components/manager.py` & `vivarium-1.2.2/src/vivarium/framework/components/manager.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/src/vivarium/framework/components/parser.py` & `vivarium-1.2.2/src/vivarium/framework/components/parser.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/src/vivarium/framework/configuration.py` & `vivarium-1.2.2/src/vivarium/framework/configuration.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/src/vivarium/framework/engine.py` & `vivarium-1.2.2/src/vivarium/framework/engine.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/src/vivarium/framework/event.py` & `vivarium-1.2.2/src/vivarium/framework/event.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/src/vivarium/framework/lifecycle.py` & `vivarium-1.2.2/src/vivarium/framework/lifecycle.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/src/vivarium/framework/logging/manager.py` & `vivarium-1.2.2/src/vivarium/framework/logging/manager.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/src/vivarium/framework/logging/utilities.py` & `vivarium-1.2.2/src/vivarium/framework/logging/utilities.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/src/vivarium/framework/lookup.py` & `vivarium-1.2.2/src/vivarium/framework/lookup.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/src/vivarium/framework/metrics.py` & `vivarium-1.2.2/src/vivarium/framework/metrics.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/src/vivarium/framework/plugins.py` & `vivarium-1.2.2/src/vivarium/framework/plugins.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/src/vivarium/framework/population/__init__.py` & `vivarium-1.2.2/src/vivarium/framework/population/__init__.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/src/vivarium/framework/population/manager.py` & `vivarium-1.2.2/src/vivarium/framework/population/manager.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/src/vivarium/framework/population/population_view.py` & `vivarium-1.2.2/src/vivarium/framework/population/population_view.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/src/vivarium/framework/randomness/__init__.py` & `vivarium-1.2.2/src/vivarium/framework/randomness/__init__.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/src/vivarium/framework/randomness/index_map.py` & `vivarium-1.2.2/src/vivarium/framework/randomness/index_map.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/src/vivarium/framework/randomness/manager.py` & `vivarium-1.2.2/src/vivarium/framework/randomness/manager.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/src/vivarium/framework/randomness/stream.py` & `vivarium-1.2.2/src/vivarium/framework/randomness/stream.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/src/vivarium/framework/resource.py` & `vivarium-1.2.2/src/vivarium/framework/resource.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/src/vivarium/framework/results/context.py` & `vivarium-1.2.2/src/vivarium/framework/results/context.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/src/vivarium/framework/results/interface.py` & `vivarium-1.2.2/src/vivarium/framework/results/interface.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/src/vivarium/framework/results/manager.py` & `vivarium-1.2.2/src/vivarium/framework/results/manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import itertools
 from collections import Counter
 from enum import Enum
 from typing import TYPE_CHECKING, Callable, List, Union
 
 import pandas as pd
 
 from vivarium.framework.event import Event
@@ -54,25 +55,53 @@
     # noinspection PyAttributeOutsideInit
     def setup(self, builder: "Builder"):
         self.logger = builder.logging.get_logger(self.name)
         self.population_view = builder.population.get_view([])
         self.clock = builder.time.clock()
         self.step_size = builder.time.step_size()
 
+        builder.event.register_listener("post_setup", self.on_post_setup)
         builder.event.register_listener("time_step__prepare", self.on_time_step_prepare)
         builder.event.register_listener("time_step", self.on_time_step)
         builder.event.register_listener("time_step__cleanup", self.on_time_step_cleanup)
         builder.event.register_listener("collect_metrics", self.on_collect_metrics)
 
         self.get_value = builder.value.get_value
 
         self.set_default_stratifications(builder)
 
         builder.value.register_value_modifier("metrics", self.get_results)
 
+    def on_post_setup(self, event: Event):
+        # update self._metrics to have all output keys
+        def create_measure_specific_keys(measure: str, stratifications: List[str]) -> None:
+            measure_str = f"MEASURE_{measure}_"
+            individual_stratification_strings = [
+                [
+                    f"{stratification.name.upper()}_{category}"
+                    for category in stratification.categories
+                ]
+                for stratification in sorted(
+                    self._results_context.stratifications, key=lambda x: x.name
+                )
+                if stratification.name in stratifications
+            ]
+            for complete_stratifications in itertools.product(
+                *individual_stratification_strings
+            ):
+                key = measure_str + "_".join(complete_stratifications)
+                self._metrics[key] = 0
+
+        for event in self._results_context.observations:
+            for (_, stratifications), observations in self._results_context.observations[
+                event
+            ].items():
+                for measure, *_ in observations:
+                    create_measure_specific_keys(measure, stratifications)
+
     def on_time_step_prepare(self, event: Event):
         self.gather_results("time_step__prepare", event)
 
     def on_time_step(self, event: Event):
         self.gather_results("time_step", event)
 
     def on_time_step_cleanup(self, event: Event):
```

### Comparing `vivarium-1.2.1/src/vivarium/framework/results/stratification.py` & `vivarium-1.2.2/src/vivarium/framework/results/stratification.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/src/vivarium/framework/state_machine.py` & `vivarium-1.2.2/src/vivarium/framework/state_machine.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/src/vivarium/framework/time.py` & `vivarium-1.2.2/src/vivarium/framework/time.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/src/vivarium/framework/utilities.py` & `vivarium-1.2.2/src/vivarium/framework/utilities.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/src/vivarium/framework/values.py` & `vivarium-1.2.2/src/vivarium/framework/values.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/src/vivarium/interface/cli.py` & `vivarium-1.2.2/src/vivarium/interface/cli.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/src/vivarium/interface/interactive.py` & `vivarium-1.2.2/src/vivarium/interface/interactive.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/src/vivarium/interface/utilities.py` & `vivarium-1.2.2/src/vivarium/interface/utilities.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/src/vivarium/interpolation.py` & `vivarium-1.2.2/src/vivarium/interpolation.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/src/vivarium/testing_utilities.py` & `vivarium-1.2.2/src/vivarium/testing_utilities.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/src/vivarium.egg-info/PKG-INFO` & `vivarium-1.2.2/src/vivarium.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vivarium
-Version: 1.2.1
+Version: 1.2.2
 Summary: vivarium is a microsimulation framework built on top of the standard scientific python stack.
 Home-page: https://github.com/ihmeuw/vivarium
 Author: The vivarium developers
 Author-email: vivarium.dev@gmail.com
 License: BSD-3-Clause
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `vivarium-1.2.1/src/vivarium.egg-info/SOURCES.txt` & `vivarium-1.2.2/src/vivarium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/tests/config_tree/test_basic_functionality.py` & `vivarium-1.2.2/tests/config_tree/test_basic_functionality.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/tests/config_tree/test_ingestion.py` & `vivarium-1.2.2/tests/config_tree/test_ingestion.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/tests/conftest.py` & `vivarium-1.2.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/tests/framework/artifact/test_artifact.py` & `vivarium-1.2.2/tests/framework/artifact/test_artifact.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/tests/framework/artifact/test_hdf.py` & `vivarium-1.2.2/tests/framework/artifact/test_hdf.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/tests/framework/artifact/test_manager.py` & `vivarium-1.2.2/tests/framework/artifact/test_manager.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/tests/framework/components/mocks.py` & `vivarium-1.2.2/tests/framework/components/mocks.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/tests/framework/components/test_manager.py` & `vivarium-1.2.2/tests/framework/components/test_manager.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/tests/framework/components/test_parser.py` & `vivarium-1.2.2/tests/framework/components/test_parser.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/tests/framework/population/test_manager.py` & `vivarium-1.2.2/tests/framework/population/test_manager.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/tests/framework/population/test_population_view.py` & `vivarium-1.2.2/tests/framework/population/test_population_view.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/tests/framework/randomness/conftest.py` & `vivarium-1.2.2/tests/framework/randomness/conftest.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/tests/framework/randomness/test_crn.py` & `vivarium-1.2.2/tests/framework/randomness/test_crn.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/tests/framework/randomness/test_index_map.py` & `vivarium-1.2.2/tests/framework/randomness/test_index_map.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/tests/framework/randomness/test_manager.py` & `vivarium-1.2.2/tests/framework/randomness/test_manager.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/tests/framework/randomness/test_stream.py` & `vivarium-1.2.2/tests/framework/randomness/test_stream.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/tests/framework/results/mocks.py` & `vivarium-1.2.2/tests/framework/results/mocks.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/tests/framework/results/test_context.py` & `vivarium-1.2.2/tests/framework/results/test_context.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/tests/framework/results/test_interface.py` & `vivarium-1.2.2/tests/framework/results/test_interface.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/tests/framework/results/test_manager.py` & `vivarium-1.2.2/tests/framework/results/test_manager.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/tests/framework/results/test_stratification.py` & `vivarium-1.2.2/tests/framework/results/test_stratification.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/tests/framework/test_configuration.py` & `vivarium-1.2.2/tests/framework/test_configuration.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/tests/framework/test_engine.py` & `vivarium-1.2.2/tests/framework/test_engine.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/tests/framework/test_event.py` & `vivarium-1.2.2/tests/framework/test_event.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/tests/framework/test_lifecycle.py` & `vivarium-1.2.2/tests/framework/test_lifecycle.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/tests/framework/test_lookup.py` & `vivarium-1.2.2/tests/framework/test_lookup.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/tests/framework/test_plugins.py` & `vivarium-1.2.2/tests/framework/test_plugins.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/tests/framework/test_resource.py` & `vivarium-1.2.2/tests/framework/test_resource.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/tests/framework/test_state_machine.py` & `vivarium-1.2.2/tests/framework/test_state_machine.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/tests/framework/test_utilities.py` & `vivarium-1.2.2/tests/framework/test_utilities.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/tests/framework/test_values.py` & `vivarium-1.2.2/tests/framework/test_values.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/tests/interface/test_utilities.py` & `vivarium-1.2.2/tests/interface/test_utilities.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/tests/test_data/artifact.hdf` & `vivarium-1.2.2/tests/test_data/artifact.hdf`

 * *Files identical despite different names*

### Comparing `vivarium-1.2.1/tests/test_interpolation.py` & `vivarium-1.2.2/tests/test_interpolation.py`

 * *Files identical despite different names*

